# Comparing `tmp/haiqv_dev-240405rc1-py3-none-any.whl.zip` & `tmp/haiqv_dev-240405rc2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 16023 bytes, number of entries: 31
+Zip file size: 16071 bytes, number of entries: 31
 -rw-rw-rw-  2.0 fat      110 b- defN 23-Oct-30 11:46 haiqv/.env
 -rw-rw-rw-  2.0 fat      865 b- defN 24-Apr-05 01:34 haiqv/__init__.py
--rw-rw-rw-  2.0 fat     8771 b- defN 24-Apr-05 01:21 haiqv/api.py
--rw-rw-rw-  2.0 fat    11183 b- defN 24-Apr-05 01:03 haiqv/client.py
+-rw-rw-rw-  2.0 fat     8782 b- defN 24-Apr-05 02:28 haiqv/api.py
+-rw-rw-rw-  2.0 fat    11704 b- defN 24-Apr-05 02:37 haiqv/client.py
 -rw-rw-rw-  2.0 fat       96 b- defN 23-Sep-11 06:53 haiqv/binding/__init__.py
 -rw-rw-rw-  2.0 fat     1152 b- defN 23-Sep-08 15:30 haiqv/binding/args_bind.py
 -rw-rw-rw-  2.0 fat     3107 b- defN 23-Sep-18 05:53 haiqv/binding/std_bind.py
 -rw-rw-rw-  2.0 fat      774 b- defN 23-Sep-08 15:40 haiqv/binding/yaml_bind.py
 -rw-rw-rw-  2.0 fat       34 b- defN 24-Feb-22 23:13 haiqv/common/__init__.py
 -rw-rw-rw-  2.0 fat     1123 b- defN 24-Apr-04 15:00 haiqv/common/keepalive.py
 -rw-rw-rw-  2.0 fat       58 b- defN 23-Sep-11 06:52 haiqv/entities/__init__.py
@@ -22,12 +22,12 @@
 -rw-rw-rw-  2.0 fat      208 b- defN 24-Apr-05 01:30 haiqv/store/log.py
 -rw-rw-rw-  2.0 fat     1661 b- defN 24-Feb-22 23:13 haiqv/store/notebook.py
 -rw-rw-rw-  2.0 fat     1078 b- defN 23-Oct-06 09:38 haiqv/store/run.py
 -rw-rw-rw-  2.0 fat      299 b- defN 24-Feb-22 23:13 haiqv/utils/__init__.py
 -rw-rw-rw-  2.0 fat      455 b- defN 23-Oct-06 14:32 haiqv/utils/common.py
 -rw-rw-rw-  2.0 fat     1570 b- defN 23-Oct-06 15:46 haiqv/utils/files.py
 -rw-rw-rw-  2.0 fat     1356 b- defN 24-Apr-05 01:30 haiqv/utils/log_config.py
--rw-rw-rw-  2.0 fat      463 b- defN 24-Apr-05 01:36 haiqv_dev-240405rc1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-05 01:36 haiqv_dev-240405rc1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 24-Apr-05 01:36 haiqv_dev-240405rc1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     2435 b- defN 24-Apr-05 01:36 haiqv_dev-240405rc1.dist-info/RECORD
-31 files, 40393 bytes uncompressed, 12147 bytes compressed:  69.9%
+-rw-rw-rw-  2.0 fat      463 b- defN 24-Apr-05 13:49 haiqv_dev-240405rc2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-05 13:49 haiqv_dev-240405rc2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 24-Apr-05 13:49 haiqv_dev-240405rc2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     2435 b- defN 24-Apr-05 13:49 haiqv_dev-240405rc2.dist-info/RECORD
+31 files, 40925 bytes uncompressed, 12195 bytes compressed:  70.2%
```

## zipnote {}

```diff
@@ -75,20 +75,20 @@
 
 Filename: haiqv/utils/files.py
 Comment: 
 
 Filename: haiqv/utils/log_config.py
 Comment: 
 
-Filename: haiqv_dev-240405rc1.dist-info/METADATA
+Filename: haiqv_dev-240405rc2.dist-info/METADATA
 Comment: 
 
-Filename: haiqv_dev-240405rc1.dist-info/WHEEL
+Filename: haiqv_dev-240405rc2.dist-info/WHEEL
 Comment: 
 
-Filename: haiqv_dev-240405rc1.dist-info/top_level.txt
+Filename: haiqv_dev-240405rc2.dist-info/top_level.txt
 Comment: 
 
-Filename: haiqv_dev-240405rc1.dist-info/RECORD
+Filename: haiqv_dev-240405rc2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## haiqv/api.py

```diff
@@ -266,15 +266,15 @@
         __log_write('warning', 'log_model_metadata - has not active run')
 
 
 def __log_write(level: str, message: Any):
     global __logger
     if __logger is None:
         __logger = setup_logger('api', LogStore.level())
-    client.create_logger(level)
+    client.create_logger(LogStore.level())
 
     if __logger:
         if level == 'info':
             __logger.info(message)
         elif level == 'debug':
             __logger.debug(message)
         elif level == 'warning':
```

## haiqv/client.py

```diff
@@ -9,19 +9,21 @@
 
 from .entities import run
 from .error.value_error import HaiqvValueError
 from .utils.files import guess_mime_type
 from .utils.log_config import setup_logger
 
 __logger = None
+__session = requests.Session()
+__timeout = 3
 
 # Notebook
 def get_notebook_info(client_ip: str) -> Any:
     try:
-        notebook_info = requests.get(f'{os.environ.get("_HAIQV_PLAT_URL")}/platform/resource/get-notebook-info?ip={client_ip}')
+        notebook_info = __session.get(f'{os.environ.get("_HAIQV_PLAT_URL")}/platform/resource/get-notebook-info?ip={client_ip}', timeout=__timeout)
 
         if notebook_info.status_code == 200:
             return notebook_info.json()
         else:
             __log_write('warning', f'notebook info fetch failed - client_ip: {client_ip} -> {notebook_info.text}')
             return HaiqvValueError(notebook_info.text)
     except Exception as e:
@@ -39,17 +41,18 @@
         'notebook_id': notebook_id,
         'notebook_name': notebook_name,
         'owner': owner,
         'owner_name': owner_name,
     }
 
     try:
-        run_info = requests.post(f'{os.environ.get("_HAIQV_BASE_URL")}/experiment/run',
+        run_info = __session.post(f'{os.environ.get("_HAIQV_BASE_URL")}/experiment/run',
                                  data=json.dumps(data),
-                                 headers={'Content-Type': 'application/json'})
+                                 headers={'Content-Type': 'application/json'},
+                                 timeout=__timeout)
 
         if run_info.status_code == 200:
             __log_write('info', f'create_run ok - exp_name: {exp_name}, run_name: {run_name}')
             return run.Run(id=run_info.json()['run_id'], name=run_name)
         else:
             __log_write('warning', f'create_run failed - exp_name: {exp_name}, run_name: {run_name} -> {run_info.text}')
             return HaiqvValueError(run_info.text)
@@ -61,15 +64,15 @@
 
 def update_run(
         run_id: str,
         status: Optional[str] = None,
         is_end: Optional[bool] = False,
 ) -> Any:
     try:
-        res = requests.post(f'{os.environ.get("_HAIQV_BASE_URL")}/experiment/run/update?run_id={run_id}&status={status}&is_end={is_end}')
+        res = __session.post(f'{os.environ.get("_HAIQV_BASE_URL")}/experiment/run/update?run_id={run_id}&status={status}&is_end={is_end}', timeout=__timeout)
 
         if res.status_code == 200:
             __log_write('info', f'update_run ok - status: {status}, is_end: {is_end}')
         else:
             __log_write('warning', f'update_run failed - status: {status}, is_end: {is_end} -> {res.text}')
             return HaiqvValueError(res.text)
     except Exception as e:
@@ -82,33 +85,35 @@
 def log_param(run_id: str, key: str, value: Any) -> Any:
     data = [
         {
             key: str(value)
         }
     ]
     try:
-        res = requests.post(f'{os.environ.get("_HAIQV_BASE_URL")}/experiment/logging/batch-params?run_id={run_id}',
+        res = __session.post(f'{os.environ.get("_HAIQV_BASE_URL")}/experiment/logging/batch-params?run_id={run_id}',
                             data=json.dumps(data),
-                            headers={'Content-Type': 'application/json'})
+                            headers={'Content-Type': 'application/json'},
+                            timeout=__timeout)
         if res.status_code == 200:
             __log_write('info', f'log_param ok - key: {key}, value: {value}')
         else:
             __log_write('warning', f'log_param failed - key: {key}, value: {value} -> {res.text}')
             return HaiqvValueError(res.text)
     except Exception as e:
         __log_write('warning', f'log_param exception - key: {key}, value: {value}')
         __log_write('debug', e)
         return None
 
 
 def log_params(run_id: str, data: Any) -> Any:
     try:
-        res = requests.post(f'{os.environ.get("_HAIQV_BASE_URL")}/experiment/logging/batch-params?run_id={run_id}',
+        res = __session.post(f'{os.environ.get("_HAIQV_BASE_URL")}/experiment/logging/batch-params?run_id={run_id}',
                             data=json.dumps(data),
-                            headers={'Content-Type': 'application/json'})
+                            headers={'Content-Type': 'application/json'},
+                            timeout=__timeout)
         if res.status_code == 200:
             __log_write('info', f'log_params ok - data: {data}')
         else:
             __log_write('warning', f'log_params failed - data: {data} -> {res.text}')
             return HaiqvValueError(res.text)
     except Exception as e:
         __log_write('warning', f'log_params exception - data: {data}')
@@ -122,33 +127,35 @@
         {
             'key': key,
             'value': str(value),
             'step': step
         }
     ]
     try:
-        res = requests.post(f'{os.environ.get("_HAIQV_BASE_URL")}/experiment/logging/batch-metrics?run_id={run_id}',
+        res = __session.post(f'{os.environ.get("_HAIQV_BASE_URL")}/experiment/logging/batch-metrics?run_id={run_id}',
                             data=json.dumps(data),
-                            headers={'Content-Type': 'application/json'})
+                            headers={'Content-Type': 'application/json'},
+                            timeout=__timeout)
         if res.status_code == 200:
             __log_write('info', f'log_metric ok - key: {key}, value: {value}, step={step}')
         else:
             __log_write('warning', f'log_metric failed - key: {key}, value: {value}, step={step} -> {res.text}')
             return HaiqvValueError(res.text)
     except Exception as e:
         __log_write('warning', f'log_metric exception - key: {key}, value: {value}, step={step}')
         __log_write('debug', e)
         return None
 
 
 def log_metrics(run_id: str, data: Any) -> Any:
     try:
-        res = requests.post(f'{os.environ.get("_HAIQV_BASE_URL")}/experiment/logging/batch-metrics?run_id={run_id}',
+        res = __session.post(f'{os.environ.get("_HAIQV_BASE_URL")}/experiment/logging/batch-metrics?run_id={run_id}',
                             data=json.dumps(data),
-                            headers={'Content-Type': 'application/json'})
+                            headers={'Content-Type': 'application/json'},
+                            timeout=__timeout)
         if res.status_code == 200:
             __log_write('info', f'log_metrics ok - data: {data}')
         else:
             __log_write('warning', f'log_metrics failed - data: {data} -> {res.text}')
             return HaiqvValueError(res.text)
     except Exception as e:
         __log_write('warning', f'log_metrics exception - data: {data}')
@@ -158,17 +165,18 @@
 
 # Artifact
 def log_artifact(run_id: str, local_file: str, artifact_path: str) -> Any:
     try:
         filename = os.path.basename(local_file)
         mime = guess_mime_type(filename)
         with open(local_file, 'rb') as f:
-            res = requests.post(
+            res = __session.post(
                 f'{os.environ.get("_HAIQV_BASE_URL")}/experiment/logging/artifacts?run_id={run_id}&artifact_path={artifact_path}',
-                files={'local_file': (filename, f, mime)}
+                files={'local_file': (filename, f, mime)},
+                timeout=__timeout
             )
             if res.status_code == 200:
                 __log_write('info', f'log_artifact ok - local_file: {local_file}, artifact_path: {artifact_path}')
             else:
                 __log_write('warning', f'log_artifact failed - local_file: {local_file}, artifact_path: {artifact_path} -> {res.text}')
                 return HaiqvValueError(res.text)
     except Exception as e:
@@ -188,47 +196,50 @@
         __log_write('debug', e)
         return None
 
 
 # metadata
 def log_dataset_metadata(run_id: str, name: str, path: str, desc: str = None) -> Any:
     try:
-        res = requests.post(f'{os.environ.get("_HAIQV_BASE_URL")}/experiment/logging/metadata-dataset?run_id={run_id}&name={name}&path={path}&description={desc}',
-                            headers={'Content-Type': 'application/json'})
+        res = __session.post(f'{os.environ.get("_HAIQV_BASE_URL")}/experiment/logging/metadata-dataset?run_id={run_id}&name={name}&path={path}&description={desc}',
+                            headers={'Content-Type': 'application/json'},
+                            timeout=__timeout)
         if res.status_code == 200:
             __log_write('info', f'log_dataset_metadata ok - name: {name}, path: {path}, desc: {desc}')
         else:
             __log_write('warning', f'log_dataset_metadata failed - name: {name}, path: {path}, desc: {desc} -> {res.text}')
             return HaiqvValueError(res.text)
     except Exception as e:
         __log_write('warning', f'log_dataset_metadata exception - name: {name}, path: {path}, desc: {desc}')
         __log_write('debug', e)
         return None
 
 
 def log_model_metadata(run_id: str, name: str, path: str, step: int, volume_name: str, volume_path: str, metric: Optional[dict] = None) -> Any:
     try:
-        res = requests.post(f'{os.environ.get("_HAIQV_BASE_URL")}/experiment/logging/metadata-model?run_id={run_id}&name={name}&path={path}&step={step}&volume_name={volume_name}&volume_path={volume_path}',
+        res = __session.post(f'{os.environ.get("_HAIQV_BASE_URL")}/experiment/logging/metadata-model?run_id={run_id}&name={name}&path={path}&step={step}&volume_name={volume_name}&volume_path={volume_path}',
                             data=json.dumps(metric),
-                            headers={'Content-Type': 'application/json'})
+                            headers={'Content-Type': 'application/json'},
+                            timeout=__timeout)
         if res.status_code == 200:
             __log_write('info', f'log_model_metadata ok - name: {name}, path: {path}, step: {step}, metric: {metric}, volume_name: {volume_name}, volume_path: {volume_path}')
         else:
             __log_write('warning', f'log_model_metadata failed - name: {name}, path: {path}, step: {step}, metric: {metric}, volume_name: {volume_name}, volume_path: {volume_path} -> {res.text}')
             return HaiqvValueError(res.text)
     except Exception as e:
         __log_write('warning', f'log_model_metadata exception - name: {name}, path: {path}, step: {step}, metric: {metric}, volume_name: {volume_name}, volume_path: {volume_path}')
         __log_write('debug', e)
         return None
 
 
 def keepalive(run_id: str) -> Optional[HaiqvValueError]:
     try:
-        res = requests.post(f'{os.environ.get("_HAIQV_BASE_URL")}/experiment/run/heartbeat?run_id={run_id}',
-                            headers={'Content-Type': 'application/json'})
+        res = __session.post(f'{os.environ.get("_HAIQV_BASE_URL")}/experiment/run/heartbeat?run_id={run_id}',
+                            headers={'Content-Type': 'application/json'},
+                            timeout=__timeout)
         if res.status_code != 200:
             __log_write('warning', f'keepalive failed -> {res.text}')
             return HaiqvValueError(res.text)
     except Exception as e:
         __log_write('warning', 'keepalive failed')
         __log_write('debug', e)
         return None
```

## Comparing `haiqv_dev-240405rc1.dist-info/RECORD` & `haiqv_dev-240405rc2.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 haiqv/.env,sha256=bBm0oc8lfX2xFpIT9DwnsA0yWn9J2qcdZkuMTsx8o6Q,110
 haiqv/__init__.py,sha256=12wRk0tZxD85Sj4zWAAfUm4oHLs7MD5sxOi4FmxsoM8,865
-haiqv/api.py,sha256=GGub8VTh8-NCHmm7st7vANWHeoRCo7VPFLes-d6WAvg,8771
-haiqv/client.py,sha256=EEGigyTQ20KYmIcUj4Drwl7_f4A4RyUdy9CCWzNQOXk,11183
+haiqv/api.py,sha256=bp97dazfUDwnty2fT4jrAtYvtPElwVpMDSChRP9kxDU,8782
+haiqv/client.py,sha256=cIX0_hFLtNy3TVSHQklIC1TYDF0G5_S5qIxikGqVv0k,11704
 haiqv/binding/__init__.py,sha256=WMCLDB06c6N2n9d23lYw0D9yvHgo4pZrXoluK8-KPiY,96
 haiqv/binding/args_bind.py,sha256=zJsSN7k9qZKCdYG14l6uqbjoVrIvSn2c72wWRZvG06Q,1152
 haiqv/binding/std_bind.py,sha256=jQd_AnKBiC2CmT8OQnZaQygodIkWKu91vmi620Di5wc,3107
 haiqv/binding/yaml_bind.py,sha256=384asQbh3Ij1eZTmmsxYVDpUAMO2RUJxVGj3GdLJpbk,774
 haiqv/common/__init__.py,sha256=sF9I5DcPYIHYPqRCyPdKCZedbbgUaHm8Bz50HY2hOi4,34
 haiqv/common/keepalive.py,sha256=53Pzi4J3Z7Z9eOukYGHAJDb8uQwqyb1M0iVCkJOvp0k,1123
 haiqv/entities/__init__.py,sha256=QuaXQhl_jFmSJqfzpkD_5ElOip-VTnQ71OBMqKKqFhc,58
@@ -21,11 +21,11 @@
 haiqv/store/log.py,sha256=rHSRA4DVwkmgLLT29n7QVYQOHYIp9jIkzqVzKiVkAGI,208
 haiqv/store/notebook.py,sha256=F-7worOcqfVK7tWfc401Abi7e88uQzy6gBipmRjk-yM,1661
 haiqv/store/run.py,sha256=j6WDspjJ9kN8l1iwXJ7oiSeU_7YWCmmn1JGFhoMbxLY,1078
 haiqv/utils/__init__.py,sha256=rjY9t2z9cSkEkDEsdAJh_B7MfSJ15UwhRTZgNAaBjK8,299
 haiqv/utils/common.py,sha256=Kb3Hg7LE1Gzkx7izxukThWUW39DN3ZVNN1p7yAAs8Jo,455
 haiqv/utils/files.py,sha256=lTjgWgQjPBn5tEYa8VZSPjgRnchSDycyX1M56euBwsM,1570
 haiqv/utils/log_config.py,sha256=iHX6PB3jQK7bkDJSbCSZbtOMJ0qyFV0VM7HDkuntYXw,1356
-haiqv_dev-240405rc1.dist-info/METADATA,sha256=82r0gFHEfBZ_xE_f_1CrzgDLwk_CYKjm62s5jT-UilM,463
-haiqv_dev-240405rc1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-haiqv_dev-240405rc1.dist-info/top_level.txt,sha256=52YfvrdtWlmTWTttjb58LZWM39jxBZivosJGgv7BqXg,6
-haiqv_dev-240405rc1.dist-info/RECORD,,
+haiqv_dev-240405rc2.dist-info/METADATA,sha256=6P9w3z9xdnDPOdw7RhxfGNcJpd4smQTessh2ZiryvMc,463
+haiqv_dev-240405rc2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+haiqv_dev-240405rc2.dist-info/top_level.txt,sha256=52YfvrdtWlmTWTttjb58LZWM39jxBZivosJGgv7BqXg,6
+haiqv_dev-240405rc2.dist-info/RECORD,,
```

