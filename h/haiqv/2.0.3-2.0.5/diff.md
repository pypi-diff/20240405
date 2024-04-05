# Comparing `tmp/haiqv-2.0.3-py3-none-any.whl.zip` & `tmp/haiqv-2.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,30 +1,33 @@
-Zip file size: 14730 bytes, number of entries: 28
+Zip file size: 15996 bytes, number of entries: 31
 -rw-rw-rw-  2.0 fat      110 b- defN 23-Oct-30 11:46 haiqv/.env
--rw-rw-rw-  2.0 fat      821 b- defN 23-Oct-06 14:36 haiqv/__init__.py
--rw-rw-rw-  2.0 fat     6017 b- defN 23-Oct-30 11:46 haiqv/api.py
--rw-rw-rw-  2.0 fat     5526 b- defN 23-Oct-30 11:46 haiqv/client.py
--rw-rw-rw-  2.0 fat      115 b- defN 23-Sep-05 12:32 haiqv/constants.py
--rw-rw-rw-  2.0 fat     6086 b- defN 23-Oct-14 09:29 haiqv/track.py
+-rw-rw-rw-  2.0 fat      865 b- defN 24-Apr-05 01:34 haiqv/__init__.py
+-rw-rw-rw-  2.0 fat     8802 b- defN 24-Apr-05 14:54 haiqv/api.py
+-rw-rw-rw-  2.0 fat    11704 b- defN 24-Apr-05 02:37 haiqv/client.py
 -rw-rw-rw-  2.0 fat       96 b- defN 23-Sep-11 06:53 haiqv/binding/__init__.py
 -rw-rw-rw-  2.0 fat     1152 b- defN 23-Sep-08 15:30 haiqv/binding/args_bind.py
 -rw-rw-rw-  2.0 fat     3107 b- defN 23-Sep-18 05:53 haiqv/binding/std_bind.py
 -rw-rw-rw-  2.0 fat      774 b- defN 23-Sep-08 15:40 haiqv/binding/yaml_bind.py
+-rw-rw-rw-  2.0 fat       34 b- defN 24-Feb-22 23:13 haiqv/common/__init__.py
+-rw-rw-rw-  2.0 fat     1123 b- defN 24-Apr-04 15:00 haiqv/common/keepalive.py
 -rw-rw-rw-  2.0 fat       58 b- defN 23-Sep-11 06:52 haiqv/entities/__init__.py
 -rw-rw-rw-  2.0 fat      395 b- defN 23-Sep-08 15:35 haiqv/entities/experiment.py
--rw-rw-rw-  2.0 fat      275 b- defN 23-Oct-06 14:33 haiqv/entities/run.py
+-rw-rw-rw-  2.0 fat      409 b- defN 24-Mar-21 15:43 haiqv/entities/run.py
 -rw-rw-rw-  2.0 fat       42 b- defN 23-Sep-11 06:50 haiqv/error/__init__.py
--rw-rw-rw-  2.0 fat      212 b- defN 23-Oct-06 14:33 haiqv/error/value_error.py
--rw-rw-rw-  2.0 fat       45 b- defN 23-Sep-11 06:50 haiqv/job/__init__.py
+-rw-rw-rw-  2.0 fat      213 b- defN 24-Feb-22 23:13 haiqv/error/value_error.py
+-rw-rw-rw-  2.0 fat       88 b- defN 24-Feb-22 23:13 haiqv/job/__init__.py
 -rw-rw-rw-  2.0 fat     1302 b- defN 23-Oct-06 14:33 haiqv/job/background_task.py
--rw-rw-rw-  2.0 fat      173 b- defN 23-Oct-30 11:46 haiqv/store/__init__.py
+-rw-rw-rw-  2.0 fat      625 b- defN 24-Feb-22 23:13 haiqv/job/keepalive_task.py
+-rw-rw-rw-  2.0 fat      217 b- defN 24-Apr-04 14:46 haiqv/store/__init__.py
 -rw-rw-rw-  2.0 fat      206 b- defN 23-Sep-08 15:35 haiqv/store/client.py
--rw-rw-rw-  2.0 fat     1659 b- defN 23-Oct-30 11:46 haiqv/store/notebook.py
+-rw-rw-rw-  2.0 fat      208 b- defN 24-Apr-05 01:30 haiqv/store/log.py
+-rw-rw-rw-  2.0 fat     1661 b- defN 24-Feb-22 23:13 haiqv/store/notebook.py
 -rw-rw-rw-  2.0 fat     1078 b- defN 23-Oct-06 09:38 haiqv/store/run.py
--rw-rw-rw-  2.0 fat      263 b- defN 23-Oct-06 14:32 haiqv/utils/__init__.py
+-rw-rw-rw-  2.0 fat      299 b- defN 24-Feb-22 23:13 haiqv/utils/__init__.py
 -rw-rw-rw-  2.0 fat      455 b- defN 23-Oct-06 14:32 haiqv/utils/common.py
 -rw-rw-rw-  2.0 fat     1570 b- defN 23-Oct-06 15:46 haiqv/utils/files.py
--rw-rw-rw-  2.0 fat      380 b- defN 23-Oct-30 11:49 haiqv-2.0.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Oct-30 11:49 haiqv-2.0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 23-Oct-30 11:49 haiqv-2.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     2147 b- defN 23-Oct-30 11:49 haiqv-2.0.3.dist-info/RECORD
-28 files, 34162 bytes uncompressed, 11320 bytes compressed:  66.9%
+-rw-rw-rw-  2.0 fat     1335 b- defN 24-Apr-05 15:01 haiqv/utils/log_config.py
+-rw-rw-rw-  2.0 fat      455 b- defN 24-Apr-05 15:31 haiqv-2.0.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-05 15:31 haiqv-2.0.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 24-Apr-05 15:31 haiqv-2.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     2403 b- defN 24-Apr-05 15:31 haiqv-2.0.5.dist-info/RECORD
+31 files, 40884 bytes uncompressed, 12184 bytes compressed:  70.2%
```

## zipnote {}

```diff
@@ -6,32 +6,32 @@
 
 Filename: haiqv/api.py
 Comment: 
 
 Filename: haiqv/client.py
 Comment: 
 
-Filename: haiqv/constants.py
-Comment: 
-
-Filename: haiqv/track.py
-Comment: 
-
 Filename: haiqv/binding/__init__.py
 Comment: 
 
 Filename: haiqv/binding/args_bind.py
 Comment: 
 
 Filename: haiqv/binding/std_bind.py
 Comment: 
 
 Filename: haiqv/binding/yaml_bind.py
 Comment: 
 
+Filename: haiqv/common/__init__.py
+Comment: 
+
+Filename: haiqv/common/keepalive.py
+Comment: 
+
 Filename: haiqv/entities/__init__.py
 Comment: 
 
 Filename: haiqv/entities/experiment.py
 Comment: 
 
 Filename: haiqv/entities/run.py
@@ -45,20 +45,26 @@
 
 Filename: haiqv/job/__init__.py
 Comment: 
 
 Filename: haiqv/job/background_task.py
 Comment: 
 
+Filename: haiqv/job/keepalive_task.py
+Comment: 
+
 Filename: haiqv/store/__init__.py
 Comment: 
 
 Filename: haiqv/store/client.py
 Comment: 
 
+Filename: haiqv/store/log.py
+Comment: 
+
 Filename: haiqv/store/notebook.py
 Comment: 
 
 Filename: haiqv/store/run.py
 Comment: 
 
 Filename: haiqv/utils/__init__.py
@@ -66,20 +72,23 @@
 
 Filename: haiqv/utils/common.py
 Comment: 
 
 Filename: haiqv/utils/files.py
 Comment: 
 
-Filename: haiqv-2.0.3.dist-info/METADATA
+Filename: haiqv/utils/log_config.py
+Comment: 
+
+Filename: haiqv-2.0.5.dist-info/METADATA
 Comment: 
 
-Filename: haiqv-2.0.3.dist-info/WHEEL
+Filename: haiqv-2.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: haiqv-2.0.3.dist-info/top_level.txt
+Filename: haiqv-2.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: haiqv-2.0.3.dist-info/RECORD
+Filename: haiqv-2.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## haiqv/__init__.py

```diff
@@ -4,19 +4,20 @@
 
 stage = os.environ.get('STAGE', None)
 if stage == 'dev':
     load_dotenv(f'{pathlib.Path(__file__).parent.resolve()}/.env.develop')
 else:    
     load_dotenv(f'{pathlib.Path(__file__).parent.resolve()}/.env')
 
-from . import client
+# from . import client
 
 from .api import (
     set_client_ip,
     get_client_ip,
+    set_log_level,
     init,
     finalize,
     get_run_name,
     log_param,
     log_params,
     log_metric,
     log_metrics,
@@ -24,14 +25,15 @@
     log_dataset_metadata,
     log_model_metadata,
     )
 
 __all__ = [
     "set_client_ip",
     "get_client_ip",
+    "set_log_level",
     "init",
     "finalize",
     "get_run_name",
     "log_param",
     "log_params",
     "log_metric",
     "log_metrics",
```

## haiqv/api.py

```diff
@@ -1,28 +1,32 @@
 import os
 import pkg_resources
+from importlib_metadata import distributions
 import __main__
 import signal
 
 from typing import Any, Dict, Optional
 from datetime import datetime
 
 from .binding.args_bind import ArgBind
 from .binding.yaml_bind import YamlBind
 from .entities.run import Run
-from .store import ClientStore, RunStore, NotebookStore
+from .store import ClientStore, RunStore, NotebookStore, LogStore
 from .utils import get_ip
 from .job.background_task import BackGroundTask
-from .error.value_error import HaiqvValueError
+from .job.keepalive_task import KeepAliveTask
 from . import client
+from .error.value_error import HaiqvValueError
+from .utils.log_config import setup_logger
 
 
 __HAIQV_UPLOAD_INTERVAL = 2
 __HAIQV_STD_LOG_FILE = 'output_'
 __active_run = None
+__logger = None
 
 
 class ActiveRun(Run):
 
     def __init__(self, run=None):
         if run is not None:
             Run.__init__(self, run.info)
@@ -30,34 +34,31 @@
     def __enter__(self):
         return self
 
     def __del__(self):
         finalize()
 
     def __exit__(self, exc_type, exc_val, exc_tb):
-        status = 'FINISHED' if exc_type is None else 'FAILED'
+        status = 'Finished' if exc_type is None else 'Failed'
         finalize(status)
 
 
 def signal_handler(signum, frame):
     if signum == signal.SIGINT:
-        finalize("KILLED")
+        finalize("Killed")
         exit(1)
 
     if signum == signal.SIGTERM:
-        finalize("FINISHED")
+        finalize("Finished")
         exit(0)
 
 
-signal.signal(signal.SIGTERM, signal_handler)
-signal.signal(signal.SIGINT, signal_handler)
-
-
-def _get_current_active_run() -> Run:
-    assert RunStore.status() and RunStore.id() is not None, 'has not active runs, please run init() command first'
+def _get_current_active_run() -> Optional[Run]:
+    if RunStore.id() is None:
+        return None
     return RunStore()
 
 
 def set_client_ip(client_ip: str):
     ClientStore(client_ip)
 
 
@@ -65,33 +66,44 @@
     if ClientStore.ip() is not None:
         return ClientStore.ip()
     else:
         return get_ip()
 
 
 def get_run_name() -> str:
-    assert RunStore.status() and RunStore.id() is not None, 'has not active runs, please run init() command first'
+    # assert RunStore.status() and RunStore.id() is not None, 'has not active runs, please run init() command first'
+    if RunStore.id() is None:
+        __log_write('warning', 'get_run_name - has not active runs')
+        return ''
     return RunStore().name
 
 
+def set_log_level(log_level: str):
+    LogStore(log_level)
+
+
 def init(
         experiment_name: str,
         run_name: Optional[str] = None,
         auto_track_args: Optional[bool] = False,
         enable_output_upload: Optional[bool] = False
 ) -> ActiveRun:
-    assert experiment_name, 'init need experiment name'
+    assert experiment_name, 'init requires experiment name'
 
     client_ip = ClientStore.ip()
     if client_ip is None:
         client_ip = get_ip()
     assert client_ip, 'has not valid IP. You can specify IP address using set_client_ip() command before init()'
 
     notebook_info = client.get_notebook_info(client_ip)
-    assert not isinstance(notebook_info, HaiqvValueError), 'init fail reason:' + notebook_info.get_error()
+    if notebook_info is None or isinstance(notebook_info, HaiqvValueError):
+        return ActiveRun(None)
+
+    notebook_name = notebook_info.get('name', '')
+    __log_write('info', f'notebook name: {notebook_name}')
     NotebookStore(notebook_info)
 
     if RunStore.status():
         RunStore.flush()
 
     if run_name:
         run_name_final = f"{run_name}-{datetime.now().strftime('%Y%m%d%H%M%S')}"
@@ -103,30 +115,31 @@
         run_name=run_name_final,
         namespace=NotebookStore.namespace(),
         notebook_id=NotebookStore.id(),
         notebook_name=NotebookStore.name(),
         owner=NotebookStore.owner(),
         owner_name=NotebookStore.owner_name()
     )
-
-    assert not isinstance(run_info, HaiqvValueError), 'init fail reason:' + run_info.get_error()
+    if run_info is None or isinstance(run_info, HaiqvValueError):
+        return ActiveRun(None)
 
     if not RunStore.status():
         RunStore(run_info)
 
     client.update_run(
         run_id=run_info.id,
         status='Running'
     )
 
     running_file = __main__.__file__
     if os.path.getsize(running_file) > 0:
         log_artifact(running_file, "code")
 
-    dists = [str(d).replace(" ", "==") for d in pkg_resources.working_set]
+    # dists = [str(d).replace(" ", "==") for d in pkg_resources.working_set]
+    dists = [f"{dist.metadata['Name']}=={dist.version}" for dist in distributions()]
     client.log_requirements(run_info.id, '\n'.join(dists), "requirements.txt")
 
     if auto_track_args:
         ArgBind.patch_argparse(log_params)
         YamlBind.patch_load(log_params)
 
     if enable_output_upload:
@@ -136,72 +149,144 @@
         bg.start_std_log()
 
     run = ActiveRun()
 
     global __active_run
     __active_run = run
 
+    ka = KeepAliveTask()
+    ka.set_fn(keepalive)
+    ka.start(run_info.interval)
+
+    # signal
+    signal.signal(signal.SIGTERM, signal_handler)
+    signal.signal(signal.SIGINT, signal_handler)
+
     return run
 
 
-def finalize(status: str = "FINISHED") -> None:
+def finalize(status: str = "Finished") -> None:
     bg = BackGroundTask()
     if bg is not None:
         bg.end_std_log()
+    ka = KeepAliveTask()
+    if ka is not None:
+        ka.stop()
     if RunStore.status():
-        client.update_run(
-            run_id=_get_current_active_run().id,
-            status=status,
-            is_end=True,
-        )
+        active_run = _get_current_active_run()
+        if active_run is not None:
+            l_level = 'info'
+            if status == 'Killed':
+                l_level = 'warning'
+            __log_write(l_level, f'finalize run name: {active_run.name}, status: {status}')
+            client.update_run(
+                run_id=active_run.id,
+                status=status,
+                is_end=True,
+            )
         RunStore.flush()
 
 
 def log_param(key: str, value: Any) -> None:
-    run_id = _get_current_active_run().id
-    client.log_param(run_id=run_id, key=key, value=value)
+    active_run = _get_current_active_run()
+    if active_run is not None:
+        run_id = active_run.id
+        client.log_param(run_id=run_id, key=key, value=value)
+    else:
+        __log_write('warning', 'log_param - has not active run')
 
 
 def log_params(params: Dict[str, Any]) -> None:
-    run_id = _get_current_active_run().id
-    data = [{key: str(value)} for key, value in params.items()]
-    client.log_params(run_id=run_id, data=data)
+    active_run = _get_current_active_run()
+    if active_run is not None:
+        run_id = active_run.id
+        data = [{key: str(value)} for key, value in params.items()]
+        client.log_params(run_id=run_id, data=data)
+    else:
+        __log_write('warning', 'log_params - has not active run')
 
 
 def log_metric(key: str, value: float, step: int) -> None:
-    run_id = _get_current_active_run().id
-    client.log_metric(run_id=run_id, key=key, value=value, step=step)
+    active_run = _get_current_active_run()
+    if active_run is not None:
+        run_id = active_run.id
+        client.log_metric(run_id=run_id, key=key, value=value, step=step)
+    else:
+        __log_write('warning', 'log_metric - has not active run')
 
 
 def log_metrics(metrics: Dict[str, float], step: int) -> None:
-    run_id = _get_current_active_run().id
-    data = [{'key': key, 'value': str(value), 'step': step} for key, value in metrics.items()]
-    client.log_metrics(run_id=run_id, data=data)
+    active_run = _get_current_active_run()
+    if active_run is not None:
+        run_id = active_run.id
+        data = [{'key': key, 'value': str(value), 'step': step} for key, value in metrics.items()]
+        client.log_metrics(run_id=run_id, data=data)
+    else:
+        __log_write('warning', 'log_metrics - has not active run')
+
 
 
 def log_artifact(local_file: str, artifact_path: Optional[str] = None) -> None:
-    run_id = _get_current_active_run().id
-    client.log_artifact(run_id=run_id, local_file=local_file, artifact_path=f'{artifact_path}')
+    active_run = _get_current_active_run()
+    if active_run is not None:
+        run_id = active_run.id
+        client.log_artifact(run_id=run_id, local_file=local_file, artifact_path=f'{artifact_path}')
+    else:
+        __log_write('warning', 'log_artifact - has not active run')
 
 
 def log_dataset_metadata(name: str, path: str, desc: str = None):
-    run_id = _get_current_active_run().id
-    client.log_dataset_metadata(
-        run_id=run_id,
-        name=name,
-        path=path,
-        desc=desc
-    )
+    active_run = _get_current_active_run()
+    if active_run is not None:
+        run_id = active_run.id
+        client.log_dataset_metadata(
+            run_id=run_id,
+            name=name,
+            path=path,
+            desc=desc
+        )
+    else:
+        __log_write('warning', 'log_dataset_metadata - has not active run')
 
 
 def log_model_metadata(name: str, path: str, step: int, metric: Optional[dict] = None):
-    run_id = _get_current_active_run().id
-    volume_name, volume_path = NotebookStore.get_volume_info(path)
-    client.log_model_metadata(
-        run_id=run_id,
-        name=name,
-        path=path,
-        step=step,
-        volume_name=volume_name,
-        volume_path=volume_path,
-        metric=metric
-    )
+    active_run = _get_current_active_run()
+    if active_run is not None:
+        run_id = active_run.id
+        volume_name, volume_path = NotebookStore.get_volume_info(path)
+        client.log_model_metadata(
+            run_id=run_id,
+            name=name,
+            path=path,
+            step=step,
+            volume_name=volume_name,
+            volume_path=volume_path,
+            metric=metric
+        )
+    else:
+        __log_write('warning', 'log_model_metadata - has not active run')
+
+
+def __log_write(level: str, message: Any):
+    global __logger
+    if __logger is None:
+        __logger = setup_logger('api', LogStore.level())
+    client.create_logger(LogStore.level())
+
+    if __logger:
+        if level == 'info':
+            __logger.info(message)
+        elif level == 'debug':
+            __logger.debug(message)
+        elif level == 'warning':
+            __logger.warning(message)
+        elif level == 'error':
+            __logger.error(message)
+        else:
+            return
+
+
+def keepalive() -> None:
+    active_run = _get_current_active_run()
+    if active_run is not None:
+        run_id = active_run.id
+        client.keepalive(run_id=run_id)
```

## haiqv/client.py

```diff
@@ -6,145 +6,272 @@
 import contextlib
 
 from typing import Optional, Any
 
 from .entities import run
 from .error.value_error import HaiqvValueError
 from .utils.files import guess_mime_type
+from .utils.log_config import setup_logger
 
+__logger = None
+__session = requests.Session()
+__timeout = 3
 
 # Notebook
 def get_notebook_info(client_ip: str) -> Any:
-    notebook_info = requests.get(f'{os.environ.get("_HAIQV_PLAT_URL")}/platform/resource/get-notebook-info?ip={client_ip}')
+    try:
+        notebook_info = __session.get(f'{os.environ.get("_HAIQV_PLAT_URL")}/platform/resource/get-notebook-info?ip={client_ip}', timeout=__timeout)
 
-    if notebook_info.status_code == 200:
-        return notebook_info.json()
-    else:
-        raise HaiqvValueError(notebook_info.text)
+        if notebook_info.status_code == 200:
+            return notebook_info.json()
+        else:
+            __log_write('warning', f'notebook info fetch failed - client_ip: {client_ip} -> {notebook_info.text}')
+            return HaiqvValueError(notebook_info.text)
+    except Exception as e:
+        __log_write('warning', f'notebook info fetch exception - client_ip: {client_ip}')
+        __log_write('debug', e)
+        return None
 
 
 # Run
-def create_run(exp_name: str, run_name: str, namespace: str, notebook_id: int, notebook_name: str, owner: str, owner_name: str) -> run.Run:
+def create_run(exp_name: str, run_name: str, namespace: str, notebook_id: int, notebook_name: str, owner: str, owner_name: str) -> Any:
     data = {
         'exp_name': exp_name,
         'run_name': run_name,
         'namespace': namespace,
         'notebook_id': notebook_id,
         'notebook_name': notebook_name,
         'owner': owner,
         'owner_name': owner_name,
     }
 
-    run_info = requests.post(f'{os.environ.get("_HAIQV_BASE_URL")}/experiment/run',
-                             data=json.dumps(data),
-                             headers={'Content-Type': 'application/json'})
-
-    if run_info.status_code == 200:
-        return run.Run(id=run_info.json()['run_id'], name=run_name)
-    else:
-        raise HaiqvValueError(run_info.text)
+    try:
+        run_info = __session.post(f'{os.environ.get("_HAIQV_BASE_URL")}/experiment/run',
+                                 data=json.dumps(data),
+                                 headers={'Content-Type': 'application/json'},
+                                 timeout=__timeout)
+
+        if run_info.status_code == 200:
+            __log_write('info', f'create_run ok - exp_name: {exp_name}, run_name: {run_name}')
+            return run.Run(id=run_info.json()['run_id'], name=run_name)
+        else:
+            __log_write('warning', f'create_run failed - exp_name: {exp_name}, run_name: {run_name} -> {run_info.text}')
+            return HaiqvValueError(run_info.text)
+    except Exception as e:
+        __log_write('warning', f'create_run exception - exp_name: {exp_name}, run_name: {run_name}')
+        __log_write('debug', e)
+        return None
 
 
 def update_run(
         run_id: str,
         status: Optional[str] = None,
         is_end: Optional[bool] = False,
-) -> None:
-    res = requests.post(f'{os.environ.get("_HAIQV_BASE_URL")}/experiment/run/update?run_id={run_id}&status={status}&is_end={is_end}')
-
-    if res.status_code != 200:
-        raise HaiqvValueError(res.text)
+) -> Any:
+    try:
+        res = __session.post(f'{os.environ.get("_HAIQV_BASE_URL")}/experiment/run/update?run_id={run_id}&status={status}&is_end={is_end}', timeout=__timeout)
+
+        if res.status_code == 200:
+            __log_write('info', f'update_run ok - status: {status}, is_end: {is_end}')
+        else:
+            __log_write('warning', f'update_run failed - status: {status}, is_end: {is_end} -> {res.text}')
+            return HaiqvValueError(res.text)
+    except Exception as e:
+        __log_write('warning', f'update_run exception - status: {status}, is_end: {is_end}')
+        __log_write('debug', e)
+        return None
 
 
 # Parameter
-def log_param(run_id: str, key: str, value: Any) -> None:
+def log_param(run_id: str, key: str, value: Any) -> Any:
     data = [
         {
             key: str(value)
         }
     ]
-    res = requests.post(f'{os.environ.get("_HAIQV_BASE_URL")}/experiment/logging/batch-params?run_id={run_id}',
-                        data=json.dumps(data),
-                        headers={'Content-Type': 'application/json'})
-    if res.status_code != 200:
-        raise HaiqvValueError(res.text)
-
-
-def log_params(run_id: str, data: Any) -> None:
-    res = requests.post(f'{os.environ.get("_HAIQV_BASE_URL")}/experiment/logging/batch-params?run_id={run_id}',
-                        data=json.dumps(data),
-                        headers={'Content-Type': 'application/json'})
-    if res.status_code != 200:
-        raise HaiqvValueError(res.text)
+    try:
+        res = __session.post(f'{os.environ.get("_HAIQV_BASE_URL")}/experiment/logging/batch-params?run_id={run_id}',
+                            data=json.dumps(data),
+                            headers={'Content-Type': 'application/json'},
+                            timeout=__timeout)
+        if res.status_code == 200:
+            __log_write('info', f'log_param ok - key: {key}, value: {value}')
+        else:
+            __log_write('warning', f'log_param failed - key: {key}, value: {value} -> {res.text}')
+            return HaiqvValueError(res.text)
+    except Exception as e:
+        __log_write('warning', f'log_param exception - key: {key}, value: {value}')
+        __log_write('debug', e)
+        return None
+
+
+def log_params(run_id: str, data: Any) -> Any:
+    try:
+        res = __session.post(f'{os.environ.get("_HAIQV_BASE_URL")}/experiment/logging/batch-params?run_id={run_id}',
+                            data=json.dumps(data),
+                            headers={'Content-Type': 'application/json'},
+                            timeout=__timeout)
+        if res.status_code == 200:
+            __log_write('info', f'log_params ok - data: {data}')
+        else:
+            __log_write('warning', f'log_params failed - data: {data} -> {res.text}')
+            return HaiqvValueError(res.text)
+    except Exception as e:
+        __log_write('warning', f'log_params exception - data: {data}')
+        __log_write('debug', e)
+        return None
 
 
 # Metric
-def log_metric(run_id: str, key: str, value: float, step: int) -> None:
+def log_metric(run_id: str, key: str, value: float, step: int) -> Any:
     data = [
         {
             'key': key,
             'value': str(value),
             'step': step
         }
     ]
-    res = requests.post(f'{os.environ.get("_HAIQV_BASE_URL")}/experiment/logging/batch-metrics?run_id={run_id}',
-                        data=json.dumps(data),
-                        headers={'Content-Type': 'application/json'})
-    if res.status_code != 200:
-        raise HaiqvValueError(res.text)
-
-
-def log_metrics(run_id: str, data: Any) -> None:
-    res = requests.post(f'{os.environ.get("_HAIQV_BASE_URL")}/experiment/logging/batch-metrics?run_id={run_id}',
-                        data=json.dumps(data),
-                        headers={'Content-Type': 'application/json'})
-    if res.status_code != 200:
-        raise HaiqvValueError(res.text)
+    try:
+        res = __session.post(f'{os.environ.get("_HAIQV_BASE_URL")}/experiment/logging/batch-metrics?run_id={run_id}',
+                            data=json.dumps(data),
+                            headers={'Content-Type': 'application/json'},
+                            timeout=__timeout)
+        if res.status_code == 200:
+            __log_write('info', f'log_metric ok - key: {key}, value: {value}, step={step}')
+        else:
+            __log_write('warning', f'log_metric failed - key: {key}, value: {value}, step={step} -> {res.text}')
+            return HaiqvValueError(res.text)
+    except Exception as e:
+        __log_write('warning', f'log_metric exception - key: {key}, value: {value}, step={step}')
+        __log_write('debug', e)
+        return None
+
+
+def log_metrics(run_id: str, data: Any) -> Any:
+    try:
+        res = __session.post(f'{os.environ.get("_HAIQV_BASE_URL")}/experiment/logging/batch-metrics?run_id={run_id}',
+                            data=json.dumps(data),
+                            headers={'Content-Type': 'application/json'},
+                            timeout=__timeout)
+        if res.status_code == 200:
+            __log_write('info', f'log_metrics ok - data: {data}')
+        else:
+            __log_write('warning', f'log_metrics failed - data: {data} -> {res.text}')
+            return HaiqvValueError(res.text)
+    except Exception as e:
+        __log_write('warning', f'log_metrics exception - data: {data}')
+        __log_write('debug', e)
+        return None
 
 
 # Artifact
-def log_artifact(run_id: str, local_file: str, artifact_path: str) -> None:
-    filename = os.path.basename(local_file)
-    mime = guess_mime_type(filename)
-    with open(local_file, 'rb') as f:
-        res = requests.post(
-            f'{os.environ.get("_HAIQV_BASE_URL")}/experiment/logging/artifacts?run_id={run_id}&artifact_path={artifact_path}',
-            files={'local_file': (filename, f, mime)}
-        )
-        if res.status_code != 200:
-            raise HaiqvValueError(res)
+def log_artifact(run_id: str, local_file: str, artifact_path: str) -> Any:
+    try:
+        filename = os.path.basename(local_file)
+        mime = guess_mime_type(filename)
+        with open(local_file, 'rb') as f:
+            res = __session.post(
+                f'{os.environ.get("_HAIQV_BASE_URL")}/experiment/logging/artifacts?run_id={run_id}&artifact_path={artifact_path}',
+                files={'local_file': (filename, f, mime)},
+                timeout=__timeout
+            )
+            if res.status_code == 200:
+                __log_write('info', f'log_artifact ok - local_file: {local_file}, artifact_path: {artifact_path}')
+            else:
+                __log_write('warning', f'log_artifact failed - local_file: {local_file}, artifact_path: {artifact_path} -> {res.text}')
+                return HaiqvValueError(res.text)
+    except Exception as e:
+        __log_write('warning', f'log_artifact exception - local_file: {local_file}, artifact_path: {artifact_path}')
+        __log_write('debug', e)
+        return None
 
 
 # Requirements
-def log_requirements(run_id: str, text: str, requirement_file: str) -> None:
-    with _log_artifact_helper(run_id, requirement_file) as tmp_path:
-        with open(tmp_path, "w", encoding="utf-8") as f:
-            f.write(text)
+def log_requirements(run_id: str, text: str, requirement_file: str) -> Any:
+    try:
+        with _log_artifact_helper(run_id, requirement_file) as tmp_path:
+            with open(tmp_path, "w", encoding="utf-8") as f:
+                f.write(text)
+    except Exception as e:
+        __log_write('warning', 'log_requirements exception')
+        __log_write('debug', e)
+        return None
 
 
 # metadata
-def log_dataset_metadata(run_id: str, name: str, path: str, desc: str = None):
-    res = requests.post(f'{os.environ.get("_HAIQV_BASE_URL")}/experiment/logging/metadata-dataset?run_id={run_id}&name={name}&path={path}&description={desc}',
-                        headers={'Content-Type': 'application/json'})
-    if res.status_code != 200:
-        raise HaiqvValueError(res.text)
-
-
-def log_model_metadata(run_id: str, name: str, path: str, step: int, volume_name: str, volume_path: str, metric: Optional[dict] = None):
-    res = requests.post(f'{os.environ.get("_HAIQV_BASE_URL")}/experiment/logging/metadata-model?run_id={run_id}&name={name}&path={path}&step={step}&volume_name={volume_name}&volume_path={volume_path}',
-                        data=json.dumps(metric),
-                        headers={'Content-Type': 'application/json'})
-    if res.status_code != 200:
-        raise HaiqvValueError(res.text)
+def log_dataset_metadata(run_id: str, name: str, path: str, desc: str = None) -> Any:
+    try:
+        res = __session.post(f'{os.environ.get("_HAIQV_BASE_URL")}/experiment/logging/metadata-dataset?run_id={run_id}&name={name}&path={path}&description={desc}',
+                            headers={'Content-Type': 'application/json'},
+                            timeout=__timeout)
+        if res.status_code == 200:
+            __log_write('info', f'log_dataset_metadata ok - name: {name}, path: {path}, desc: {desc}')
+        else:
+            __log_write('warning', f'log_dataset_metadata failed - name: {name}, path: {path}, desc: {desc} -> {res.text}')
+            return HaiqvValueError(res.text)
+    except Exception as e:
+        __log_write('warning', f'log_dataset_metadata exception - name: {name}, path: {path}, desc: {desc}')
+        __log_write('debug', e)
+        return None
+
+
+def log_model_metadata(run_id: str, name: str, path: str, step: int, volume_name: str, volume_path: str, metric: Optional[dict] = None) -> Any:
+    try:
+        res = __session.post(f'{os.environ.get("_HAIQV_BASE_URL")}/experiment/logging/metadata-model?run_id={run_id}&name={name}&path={path}&step={step}&volume_name={volume_name}&volume_path={volume_path}',
+                            data=json.dumps(metric),
+                            headers={'Content-Type': 'application/json'},
+                            timeout=__timeout)
+        if res.status_code == 200:
+            __log_write('info', f'log_model_metadata ok - name: {name}, path: {path}, step: {step}, metric: {metric}, volume_name: {volume_name}, volume_path: {volume_path}')
+        else:
+            __log_write('warning', f'log_model_metadata failed - name: {name}, path: {path}, step: {step}, metric: {metric}, volume_name: {volume_name}, volume_path: {volume_path} -> {res.text}')
+            return HaiqvValueError(res.text)
+    except Exception as e:
+        __log_write('warning', f'log_model_metadata exception - name: {name}, path: {path}, step: {step}, metric: {metric}, volume_name: {volume_name}, volume_path: {volume_path}')
+        __log_write('debug', e)
+        return None
+
+
+def keepalive(run_id: str) -> Optional[HaiqvValueError]:
+    try:
+        res = __session.post(f'{os.environ.get("_HAIQV_BASE_URL")}/experiment/run/heartbeat?run_id={run_id}',
+                            headers={'Content-Type': 'application/json'},
+                            timeout=__timeout)
+        if res.status_code != 200:
+            __log_write('warning', f'keepalive failed -> {res.text}')
+            return HaiqvValueError(res.text)
+    except Exception as e:
+        __log_write('warning', 'keepalive failed')
+        __log_write('debug', e)
+        return None
 
 
 @contextlib.contextmanager
 def _log_artifact_helper(run_id, artifact_file):
     norm_path = posixpath.normpath(artifact_file)
     filename = posixpath.basename(norm_path)
     artifact_dir = posixpath.dirname(norm_path)
 
     with tempfile.TemporaryDirectory() as tmp_dir:
         tmp_path = os.path.join(tmp_dir, filename)
         yield tmp_path
         log_artifact(run_id, tmp_path, artifact_dir)
 
+
+def create_logger(level: str):
+    global __logger
+    if __logger is None:
+        __logger = setup_logger('client', level)
+
+
+def __log_write(level: str, message: Any):
+    if __logger:
+        if level == 'info':
+            __logger.info(message)
+        elif level == 'debug':
+            __logger.debug(message)
+        elif level == 'warning':
+            __logger.warning(message)
+        elif level == 'error':
+            __logger.error(message)
+        else:
+            return
```

## haiqv/entities/run.py

```diff
@@ -1,16 +1,22 @@
 class Run:
     def __init__(
             self,
             id,
             name=None,
+            interval=60,
     ):
         self._id = id
         self._name = name
+        self._interval = interval
 
     @property
     def id(self):
         return self._id
 
     @property
     def name(self):
         return self._name
+
+    @property
+    def interval(self):
+        return self._interval
```

## haiqv/error/value_error.py

```diff
@@ -1,9 +1,9 @@
 class HaiqvValueError(Exception):
-    def __init__(self, error: dict):
+    def __init__(self, error: any):
         self.error = error
 
     def __str__(self):
         return str(self.error)
 
     def get_error(self):
-        return self.error
+        return self.error
```

## haiqv/job/__init__.py

```diff
@@ -1 +1,2 @@
 from .background_task import BackGroundTask
+from .keepalive_task import KeepAliveTask
```

## haiqv/store/__init__.py

```diff
@@ -1,9 +1,11 @@
 from .client import ClientStore
 from .run import RunStore
 from .notebook import NotebookStore
+from .log import LogStore
 
 __all__ = [
     "ClientStore",
     "RunStore",
-    "NotebookStore"
+    "NotebookStore",
+    "LogStore"
 ]
```

## haiqv/store/notebook.py

```diff
@@ -1,9 +1,10 @@
 import os
 
+
 class NotebookStore:
     __notebook_info = None
 
     @classmethod
     def __init__(cls, notebook_info):
         cls.__notebook_info = notebook_info
```

## haiqv/utils/__init__.py

```diff
@@ -1,8 +1,8 @@
 from .common import get_millis
 from .common import key_subset_split
 from .common import get_ip
 from .files import relative_path_to_artifact_path
 from .files import path_not_unique
 from .files import get_text_extensions
 from .files import guess_mime_type
-
+from .log_config import setup_logger
```

