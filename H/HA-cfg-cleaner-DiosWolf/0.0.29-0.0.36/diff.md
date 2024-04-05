# Comparing `tmp/HA_cfg_cleaner_DiosWolf-0.0.29.tar.gz` & `tmp/HA_cfg_cleaner_DiosWolf-0.0.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HA_cfg_cleaner_DiosWolf-0.0.29.tar", last modified: Thu Mar 14 17:16:19 2024, max compression
+gzip compressed data, was "HA_cfg_cleaner_DiosWolf-0.0.36.tar", last modified: Mon Mar 18 11:04:32 2024, max compression
```

## Comparing `HA_cfg_cleaner_DiosWolf-0.0.29.tar` & `HA_cfg_cleaner_DiosWolf-0.0.36.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-03-14 17:16:19.726467 HA_cfg_cleaner_DiosWolf-0.0.29/
-drwxrwxrwx   0        0        0        0 2024-03-14 17:16:19.710467 HA_cfg_cleaner_DiosWolf-0.0.29/HA_cfg_cleaner_DiosWolf/
--rw-rw-rw-   0        0        0       24 2024-03-14 17:16:15.000000 HA_cfg_cleaner_DiosWolf-0.0.29/HA_cfg_cleaner_DiosWolf/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-14 17:16:19.714471 HA_cfg_cleaner_DiosWolf-0.0.29/HA_cfg_cleaner_DiosWolf/castom_errors/
--rw-rw-rw-   0        0        0      132 2024-03-14 17:15:22.000000 HA_cfg_cleaner_DiosWolf-0.0.29/HA_cfg_cleaner_DiosWolf/castom_errors/castom_errors.py
-drwxrwxrwx   0        0        0        0 2024-03-14 17:16:19.716468 HA_cfg_cleaner_DiosWolf-0.0.29/HA_cfg_cleaner_DiosWolf/configs_HA/
--rw-rw-rw-   0        0        0     3308 2024-03-14 14:55:50.000000 HA_cfg_cleaner_DiosWolf-0.0.29/HA_cfg_cleaner_DiosWolf/configs_HA/config_HA.json
--rw-rw-rw-   0        0        0     3840 2024-03-07 12:10:34.000000 HA_cfg_cleaner_DiosWolf-0.0.29/HA_cfg_cleaner_DiosWolf/configs_HA/config_HA_wind.json
-drwxrwxrwx   0        0        0        0 2024-03-14 17:16:19.717468 HA_cfg_cleaner_DiosWolf-0.0.29/HA_cfg_cleaner_DiosWolf/data_classes_json/
--rw-rw-rw-   0        0        0      111 2024-02-27 12:45:26.000000 HA_cfg_cleaner_DiosWolf-0.0.29/HA_cfg_cleaner_DiosWolf/data_classes_json/args_parse.py
--rw-rw-rw-   0        0        0     1156 2024-03-06 23:10:06.000000 HA_cfg_cleaner_DiosWolf-0.0.29/HA_cfg_cleaner_DiosWolf/data_classes_json/file_config.py
--rw-rw-rw-   0        0        0     1426 2024-03-12 11:31:44.000000 HA_cfg_cleaner_DiosWolf-0.0.29/HA_cfg_cleaner_DiosWolf/data_classes_json/instructions.py
-drwxrwxrwx   0        0        0        0 2024-03-14 17:16:19.722467 HA_cfg_cleaner_DiosWolf-0.0.29/HA_cfg_cleaner_DiosWolf/files_editors/
--rw-rw-rw-   0        0        0     1104 2024-03-14 17:14:21.000000 HA_cfg_cleaner_DiosWolf-0.0.29/HA_cfg_cleaner_DiosWolf/files_editors/addons_editor.py
--rw-rw-rw-   0        0        0     2593 2024-03-06 22:32:05.000000 HA_cfg_cleaner_DiosWolf-0.0.29/HA_cfg_cleaner_DiosWolf/files_editors/automations_editor.py
--rw-rw-rw-   0        0        0     2045 2024-03-05 22:25:38.000000 HA_cfg_cleaner_DiosWolf-0.0.29/HA_cfg_cleaner_DiosWolf/files_editors/editor_restore_state.py
--rw-rw-rw-   0        0        0     2420 2024-03-14 11:32:15.000000 HA_cfg_cleaner_DiosWolf-0.0.29/HA_cfg_cleaner_DiosWolf/files_editors/fileIO_cls.py
--rw-rw-rw-   0        0        0      442 2024-02-26 18:57:11.000000 HA_cfg_cleaner_DiosWolf-0.0.29/HA_cfg_cleaner_DiosWolf/files_editors/file_folder_editor_cls.py
--rw-rw-rw-   0        0        0     1990 2024-03-05 22:25:38.000000 HA_cfg_cleaner_DiosWolf-0.0.29/HA_cfg_cleaner_DiosWolf/files_editors/find_in_files_cls.py
--rw-rw-rw-   0        0        0     3096 2024-03-05 22:12:50.000000 HA_cfg_cleaner_DiosWolf-0.0.29/HA_cfg_cleaner_DiosWolf/files_editors/integrations_cls.py
--rw-rw-rw-   0        0        0      711 2024-03-06 22:24:58.000000 HA_cfg_cleaner_DiosWolf-0.0.29/HA_cfg_cleaner_DiosWolf/files_editors/script_editor_cls.py
-drwxrwxrwx   0        0        0        0 2024-03-14 17:16:19.723467 HA_cfg_cleaner_DiosWolf-0.0.29/HA_cfg_cleaner_DiosWolf/ha_requests/
--rw-rw-rw-   0        0        0      978 2024-03-14 14:51:38.000000 HA_cfg_cleaner_DiosWolf-0.0.29/HA_cfg_cleaner_DiosWolf/ha_requests/ha_request.py
-drwxrwxrwx   0        0        0        0 2024-03-14 17:16:19.723467 HA_cfg_cleaner_DiosWolf-0.0.29/HA_cfg_cleaner_DiosWolf/instruction_classes/
--rw-rw-rw-   0        0        0    11979 2024-03-14 17:16:00.000000 HA_cfg_cleaner_DiosWolf-0.0.29/HA_cfg_cleaner_DiosWolf/instruction_classes/instruction_executor.py
--rw-rw-rw-   0        0        0     2702 2024-03-14 14:47:59.000000 HA_cfg_cleaner_DiosWolf-0.0.29/HA_cfg_cleaner_DiosWolf/main.py
-drwxrwxrwx   0        0        0        0 2024-03-14 17:16:19.725468 HA_cfg_cleaner_DiosWolf-0.0.29/HA_cfg_cleaner_DiosWolf/parse_classes/
--rw-rw-rw-   0        0        0     1464 2024-03-14 14:51:26.000000 HA_cfg_cleaner_DiosWolf-0.0.29/HA_cfg_cleaner_DiosWolf/parse_classes/arguments_parse.py
--rw-rw-rw-   0        0        0      171 2024-02-23 13:52:30.000000 HA_cfg_cleaner_DiosWolf-0.0.29/HA_cfg_cleaner_DiosWolf/parse_classes/parse_cls.py
-drwxrwxrwx   0        0        0        0 2024-03-14 17:16:19.725468 HA_cfg_cleaner_DiosWolf-0.0.29/HA_cfg_cleaner_DiosWolf.egg-info/
--rw-rw-rw-   0        0        0      275 2024-03-14 17:16:19.000000 HA_cfg_cleaner_DiosWolf-0.0.29/HA_cfg_cleaner_DiosWolf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1417 2024-03-14 17:16:19.000000 HA_cfg_cleaner_DiosWolf-0.0.29/HA_cfg_cleaner_DiosWolf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-14 17:16:19.000000 HA_cfg_cleaner_DiosWolf-0.0.29/HA_cfg_cleaner_DiosWolf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2024-03-14 17:16:19.000000 HA_cfg_cleaner_DiosWolf-0.0.29/HA_cfg_cleaner_DiosWolf.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       70 2024-03-14 17:16:19.000000 HA_cfg_cleaner_DiosWolf-0.0.29/HA_cfg_cleaner_DiosWolf.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-03-14 17:16:19.000000 HA_cfg_cleaner_DiosWolf-0.0.29/HA_cfg_cleaner_DiosWolf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1088 2024-02-27 18:02:40.000000 HA_cfg_cleaner_DiosWolf-0.0.29/LICENSE
--rw-rw-rw-   0        0        0       61 2024-02-27 18:45:02.000000 HA_cfg_cleaner_DiosWolf-0.0.29/MANIFEST.in
--rw-rw-rw-   0        0        0      275 2024-03-14 17:16:19.726467 HA_cfg_cleaner_DiosWolf-0.0.29/PKG-INFO
--rw-rw-rw-   0        0        0       43 2024-02-28 18:51:58.000000 HA_cfg_cleaner_DiosWolf-0.0.29/README.txt
--rw-rw-rw-   0        0        0       42 2024-03-14 17:16:19.727466 HA_cfg_cleaner_DiosWolf-0.0.29/setup.cfg
--rw-rw-rw-   0        0        0      636 2024-03-05 22:25:38.000000 HA_cfg_cleaner_DiosWolf-0.0.29/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-18 11:04:32.924819 HA_cfg_cleaner_DiosWolf-0.0.36/
+drwxrwxrwx   0        0        0        0 2024-03-18 11:04:32.910746 HA_cfg_cleaner_DiosWolf-0.0.36/HA_cfg_cleaner_DiosWolf/
+-rw-rw-rw-   0        0        0       26 2024-03-18 11:04:30.000000 HA_cfg_cleaner_DiosWolf-0.0.36/HA_cfg_cleaner_DiosWolf/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-18 11:04:32.914749 HA_cfg_cleaner_DiosWolf-0.0.36/HA_cfg_cleaner_DiosWolf/castom_errors/
+-rw-rw-rw-   0        0        0      107 2024-03-14 17:17:58.000000 HA_cfg_cleaner_DiosWolf-0.0.36/HA_cfg_cleaner_DiosWolf/castom_errors/castom_errors.py
+drwxrwxrwx   0        0        0        0 2024-03-18 11:04:32.915746 HA_cfg_cleaner_DiosWolf-0.0.36/HA_cfg_cleaner_DiosWolf/configs_HA/
+-rw-rw-rw-   0        0        0     3459 2024-03-18 10:54:43.000000 HA_cfg_cleaner_DiosWolf-0.0.36/HA_cfg_cleaner_DiosWolf/configs_HA/config_HA.json
+-rw-rw-rw-   0        0        0     4025 2024-03-18 10:27:12.000000 HA_cfg_cleaner_DiosWolf-0.0.36/HA_cfg_cleaner_DiosWolf/configs_HA/config_HA_wind.json
+drwxrwxrwx   0        0        0        0 2024-03-18 11:04:32.917746 HA_cfg_cleaner_DiosWolf-0.0.36/HA_cfg_cleaner_DiosWolf/data_classes_json/
+-rw-rw-rw-   0        0        0      593 2024-03-18 09:54:43.000000 HA_cfg_cleaner_DiosWolf-0.0.36/HA_cfg_cleaner_DiosWolf/data_classes_json/args_parse.py
+-rw-rw-rw-   0        0        0     1218 2024-03-18 10:01:35.000000 HA_cfg_cleaner_DiosWolf-0.0.36/HA_cfg_cleaner_DiosWolf/data_classes_json/file_config.py
+-rw-rw-rw-   0        0        0     1568 2024-03-18 10:34:52.000000 HA_cfg_cleaner_DiosWolf-0.0.36/HA_cfg_cleaner_DiosWolf/data_classes_json/instructions.py
+drwxrwxrwx   0        0        0        0 2024-03-18 11:04:32.921819 HA_cfg_cleaner_DiosWolf-0.0.36/HA_cfg_cleaner_DiosWolf/files_editors/
+-rw-rw-rw-   0        0        0     2509 2024-03-18 10:30:35.000000 HA_cfg_cleaner_DiosWolf-0.0.36/HA_cfg_cleaner_DiosWolf/files_editors/addons_editor.py
+-rw-rw-rw-   0        0        0     2820 2024-03-18 10:12:22.000000 HA_cfg_cleaner_DiosWolf-0.0.36/HA_cfg_cleaner_DiosWolf/files_editors/automations_editor.py
+-rw-rw-rw-   0        0        0     2045 2024-03-05 22:25:38.000000 HA_cfg_cleaner_DiosWolf-0.0.36/HA_cfg_cleaner_DiosWolf/files_editors/editor_restore_state.py
+-rw-rw-rw-   0        0        0     2420 2024-03-14 11:32:15.000000 HA_cfg_cleaner_DiosWolf-0.0.36/HA_cfg_cleaner_DiosWolf/files_editors/fileIO_cls.py
+-rw-rw-rw-   0        0        0      442 2024-02-26 18:57:11.000000 HA_cfg_cleaner_DiosWolf-0.0.36/HA_cfg_cleaner_DiosWolf/files_editors/file_folder_editor_cls.py
+-rw-rw-rw-   0        0        0     1990 2024-03-05 22:25:38.000000 HA_cfg_cleaner_DiosWolf-0.0.36/HA_cfg_cleaner_DiosWolf/files_editors/find_in_files_cls.py
+-rw-rw-rw-   0        0        0     3096 2024-03-05 22:12:50.000000 HA_cfg_cleaner_DiosWolf-0.0.36/HA_cfg_cleaner_DiosWolf/files_editors/integrations_cls.py
+-rw-rw-rw-   0        0        0      711 2024-03-06 22:24:58.000000 HA_cfg_cleaner_DiosWolf-0.0.36/HA_cfg_cleaner_DiosWolf/files_editors/script_editor_cls.py
+drwxrwxrwx   0        0        0        0 2024-03-18 11:04:32.921819 HA_cfg_cleaner_DiosWolf-0.0.36/HA_cfg_cleaner_DiosWolf/ha_requests/
+-rw-rw-rw-   0        0        0      760 2024-03-18 10:11:55.000000 HA_cfg_cleaner_DiosWolf-0.0.36/HA_cfg_cleaner_DiosWolf/ha_requests/ha_request.py
+drwxrwxrwx   0        0        0        0 2024-03-18 11:04:32.922819 HA_cfg_cleaner_DiosWolf-0.0.36/HA_cfg_cleaner_DiosWolf/instruction_classes/
+-rw-rw-rw-   0        0        0    12718 2024-03-18 11:03:54.000000 HA_cfg_cleaner_DiosWolf-0.0.36/HA_cfg_cleaner_DiosWolf/instruction_classes/instruction_executor.py
+-rw-rw-rw-   0        0        0     2803 2024-03-18 10:44:06.000000 HA_cfg_cleaner_DiosWolf-0.0.36/HA_cfg_cleaner_DiosWolf/main.py
+drwxrwxrwx   0        0        0        0 2024-03-18 11:04:32.923819 HA_cfg_cleaner_DiosWolf-0.0.36/HA_cfg_cleaner_DiosWolf/parse_classes/
+-rw-rw-rw-   0        0        0     1464 2024-03-14 14:51:26.000000 HA_cfg_cleaner_DiosWolf-0.0.36/HA_cfg_cleaner_DiosWolf/parse_classes/arguments_parse.py
+-rw-rw-rw-   0        0        0      171 2024-02-23 13:52:30.000000 HA_cfg_cleaner_DiosWolf-0.0.36/HA_cfg_cleaner_DiosWolf/parse_classes/parse_cls.py
+drwxrwxrwx   0        0        0        0 2024-03-18 11:04:32.923819 HA_cfg_cleaner_DiosWolf-0.0.36/HA_cfg_cleaner_DiosWolf.egg-info/
+-rw-rw-rw-   0        0        0      275 2024-03-18 11:04:32.000000 HA_cfg_cleaner_DiosWolf-0.0.36/HA_cfg_cleaner_DiosWolf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1417 2024-03-18 11:04:32.000000 HA_cfg_cleaner_DiosWolf-0.0.36/HA_cfg_cleaner_DiosWolf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-18 11:04:32.000000 HA_cfg_cleaner_DiosWolf-0.0.36/HA_cfg_cleaner_DiosWolf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2024-03-18 11:04:32.000000 HA_cfg_cleaner_DiosWolf-0.0.36/HA_cfg_cleaner_DiosWolf.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       70 2024-03-18 11:04:32.000000 HA_cfg_cleaner_DiosWolf-0.0.36/HA_cfg_cleaner_DiosWolf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       35 2024-03-18 11:04:32.000000 HA_cfg_cleaner_DiosWolf-0.0.36/HA_cfg_cleaner_DiosWolf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1088 2024-02-27 18:02:40.000000 HA_cfg_cleaner_DiosWolf-0.0.36/LICENSE
+-rw-rw-rw-   0        0        0       61 2024-02-27 18:45:02.000000 HA_cfg_cleaner_DiosWolf-0.0.36/MANIFEST.in
+-rw-rw-rw-   0        0        0      275 2024-03-18 11:04:32.924819 HA_cfg_cleaner_DiosWolf-0.0.36/PKG-INFO
+-rw-rw-rw-   0        0        0       43 2024-02-28 18:51:58.000000 HA_cfg_cleaner_DiosWolf-0.0.36/README.txt
+-rw-rw-rw-   0        0        0       42 2024-03-18 11:04:32.925819 HA_cfg_cleaner_DiosWolf-0.0.36/setup.cfg
+-rw-rw-rw-   0        0        0      636 2024-03-05 22:25:38.000000 HA_cfg_cleaner_DiosWolf-0.0.36/setup.py
```

### Comparing `HA_cfg_cleaner_DiosWolf-0.0.29/HA_cfg_cleaner_DiosWolf/configs_HA/config_HA.json` & `HA_cfg_cleaner_DiosWolf-0.0.36/HA_cfg_cleaner_DiosWolf/configs_HA/config_HA.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.945%*

 * *Differences: {"'host_info'": "{'api_key': 'Bearer ', 'addons_options_url': "*

 * *                "'http://172.30.32.2/addons/{addon_id}/options'}",*

 * * "'ssh_commands'": "{'get_supervisor_api': ['docker', 'inspect', 'homeassistant']}"}*

```diff
@@ -80,15 +80,16 @@
             "on_off_field": "disabled_by",
             "path": "./config/.storage/",
             "second_key": "entities",
             "type_cfg": ".json"
         }
     ],
     "host_info": {
-        "api_key": "Bearer",
+        "addons_options_url": "http://172.30.32.2/addons/{addon_id}/options",
+        "api_key": "Bearer ",
         "automations_off_url": "/api/services/homeassistant/turn_off",
         "host": "http://localhost",
         "port": "8123"
     },
     "ssh_commands": {
         "change_cfg_addons": [
             "ha",
@@ -101,10 +102,15 @@
             "addon",
             "uninstall"
         ],
         "disable_addons": [
             "ha",
             "addon",
             "stop"
+        ],
+        "get_supervisor_api": [
+            "docker",
+            "inspect",
+            "homeassistant"
         ]
     }
 }
```

### Comparing `HA_cfg_cleaner_DiosWolf-0.0.29/HA_cfg_cleaner_DiosWolf/configs_HA/config_HA_wind.json` & `HA_cfg_cleaner_DiosWolf-0.0.36/HA_cfg_cleaner_DiosWolf/configs_HA/config_HA_wind.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.945%*

 * *Differences: {"'host_info'": "{'host': 'http://localhost', 'addons_options_url': '/addons/{addon_id}/options'}",*

 * * "'ssh_commands'": "{'get_supervisor_api': ['docker', 'inspect', 'homeassistant']}"}*

```diff
@@ -80,17 +80,18 @@
             "on_off_field": "disabled_by",
             "path": "C:\\Users\\wolkm\\OneDrive\\\u0420\u043e\u0431\u043e\u0447\u0438\u0439 \u0441\u0442\u0456\u043b\\file_checker\\save_folder\\config\\.storage\\",
             "second_key": "entities",
             "type_cfg": ".json"
         }
     ],
     "host_info": {
+        "addons_options_url": "/addons/{addon_id}/options",
         "api_key": "Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiIxODM1ZmY4NzlhMDI0OGUyYjQwNGU1Y2U5ZjUxODYyNSIsImlhdCI6MTcwOTY0NTc3NSwiZXhwIjoyMDI1MDA1Nzc1fQ.gWQHqgCd8GxXp9QG6gRRKsOENi88MmnLYbelb0vmFqw",
         "automations_off_url": "/api/services/homeassistant/turn_off",
-        "host": "http://172.16.16.78",
+        "host": "http://localhost",
         "port": "8123"
     },
     "ssh_commands": {
         "change_cfg_addons": [
             "ha",
             "addons",
             "update",
@@ -101,10 +102,15 @@
             "addon",
             "uninstall"
         ],
         "disable_addons": [
             "ha",
             "addon",
             "stop"
+        ],
+        "get_supervisor_api": [
+            "docker",
+            "inspect",
+            "homeassistant"
         ]
     }
 }
```

### Comparing `HA_cfg_cleaner_DiosWolf-0.0.29/HA_cfg_cleaner_DiosWolf/data_classes_json/file_config.py` & `HA_cfg_cleaner_DiosWolf-0.0.36/HA_cfg_cleaner_DiosWolf/data_classes_json/file_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,22 +36,23 @@
 
 @dataclass
 class HostInfo:
     api_key: str
     host: str
     port: str
     automations_off_url: str
+    addons_options_url: str
 
 
 @dataclass
 class SshCommands:
     delete_addons: list[str]
     disable_addons: list[str]
     change_cfg_addons: list[str]
-
+    get_supervisor_api: list[str]
 
 @dataclass
 class ConfigurationFile:
     configurations: list[Configuration]
     automations_cfg: list[Configuration]
     config_restore_state: ConfigRestoreState
     host_info: HostInfo
```

### Comparing `HA_cfg_cleaner_DiosWolf-0.0.29/HA_cfg_cleaner_DiosWolf/data_classes_json/instructions.py` & `HA_cfg_cleaner_DiosWolf-0.0.36/HA_cfg_cleaner_DiosWolf/data_classes_json/instructions.py`

 * *Files 8% similar despite different names*

```diff
@@ -57,21 +57,28 @@
 
 @dataclass
 class DisableAutomations(BaseListIds):
     host_info: HostInst | None
 
 
 @dataclass
+class ChangeAddonsOptions:
+    addon_id: str
+    addon_options: dict
+
+
+@dataclass
 class Instructions:
     delete_integrations: BaseListIds
     enable_integration: BaseListIds
     disable_integration: BaseListIds
     delete_automations: BaseListIds
     delete_objects: list[DeleteObjects]
     delete_script: list[DeleteScript]
     clean_folders: list[CleanFolders]
     clean_files: list[CleanFiles]
     change_files: list[ChangeFiles]
     find_in_all_files: FindInFiles
     disable_automations: DisableAutomations
     disable_addons: BaseListIds
     delete_addons: BaseListIds
+    change_addons_options: list[ChangeAddonsOptions]
```

### Comparing `HA_cfg_cleaner_DiosWolf-0.0.29/HA_cfg_cleaner_DiosWolf/files_editors/automations_editor.py` & `HA_cfg_cleaner_DiosWolf-0.0.36/HA_cfg_cleaner_DiosWolf/files_editors/automations_editor.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,21 +5,22 @@
     HostInfo,
 )
 from HA_cfg_cleaner_DiosWolf.ha_requests.ha_request import HARequests
 
 
 class AutomationsEditor:
     def __init__(
-        self, configuration: Configuration, full_cfg: dict, host_cfg: HostInfo = None
+            self, configuration: Configuration, full_cfg: dict, host_cfg: HostInfo = None
     ):
         self.configuration = configuration
         self.full_cfg = full_cfg
 
         if host_cfg:
-            self.ha_request = HARequests(host_cfg)
+            self.host_cfg = host_cfg
+            self.ha_request = HARequests(host_cfg, host_cfg.api_key)
 
     def __get_editable_cfg(self) -> dict:
         if self.configuration.first_key is None:
             return self.full_cfg
 
         elif self.configuration.second_key is None:
             return self.full_cfg[self.configuration.first_key]
@@ -65,11 +66,15 @@
             if config_dict[self.configuration.id_key] not in integrations_list:
                 new_cfg_list.append(config_dict)
 
         return self.__set_editable_cfg(new_cfg_list)
 
     def disable_automation(self, automations_ids: list[str]) -> Response:
         automations_entities_ids = self.__get_entities_ids(automations_ids)
-
+        url = (self.host_cfg.host
+               + ":"
+               + self.host_cfg.port
+               + self.host_cfg.automations_off_url
+               )
         if automations_entities_ids:
             data = {self.configuration.on_off_field: automations_entities_ids}
-            return self.ha_request.post_requests(data)
+            return self.ha_request.post_requests(url, data)
```

### Comparing `HA_cfg_cleaner_DiosWolf-0.0.29/HA_cfg_cleaner_DiosWolf/files_editors/editor_restore_state.py` & `HA_cfg_cleaner_DiosWolf-0.0.36/HA_cfg_cleaner_DiosWolf/files_editors/editor_restore_state.py`

 * *Files identical despite different names*

### Comparing `HA_cfg_cleaner_DiosWolf-0.0.29/HA_cfg_cleaner_DiosWolf/files_editors/fileIO_cls.py` & `HA_cfg_cleaner_DiosWolf-0.0.36/HA_cfg_cleaner_DiosWolf/files_editors/fileIO_cls.py`

 * *Files identical despite different names*

### Comparing `HA_cfg_cleaner_DiosWolf-0.0.29/HA_cfg_cleaner_DiosWolf/files_editors/find_in_files_cls.py` & `HA_cfg_cleaner_DiosWolf-0.0.36/HA_cfg_cleaner_DiosWolf/files_editors/find_in_files_cls.py`

 * *Files identical despite different names*

### Comparing `HA_cfg_cleaner_DiosWolf-0.0.29/HA_cfg_cleaner_DiosWolf/files_editors/integrations_cls.py` & `HA_cfg_cleaner_DiosWolf-0.0.36/HA_cfg_cleaner_DiosWolf/files_editors/integrations_cls.py`

 * *Files identical despite different names*

### Comparing `HA_cfg_cleaner_DiosWolf-0.0.29/HA_cfg_cleaner_DiosWolf/files_editors/script_editor_cls.py` & `HA_cfg_cleaner_DiosWolf-0.0.36/HA_cfg_cleaner_DiosWolf/files_editors/script_editor_cls.py`

 * *Files identical despite different names*

### Comparing `HA_cfg_cleaner_DiosWolf-0.0.29/HA_cfg_cleaner_DiosWolf/instruction_classes/instruction_executor.py` & `HA_cfg_cleaner_DiosWolf-0.0.36/HA_cfg_cleaner_DiosWolf/instruction_classes/instruction_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 
 from HA_cfg_cleaner_DiosWolf.castom_errors.castom_errors import AddonError
 from HA_cfg_cleaner_DiosWolf.data_classes_json.file_config import ConfigurationFile
-from HA_cfg_cleaner_DiosWolf.data_classes_json.instructions import Instructions
+from HA_cfg_cleaner_DiosWolf.data_classes_json.instructions import Instructions, ChangeAddonsOptions
 from HA_cfg_cleaner_DiosWolf.files_editors.addons_editor import AddonsEditor
 from HA_cfg_cleaner_DiosWolf.files_editors.automations_editor import AutomationsEditor
 from HA_cfg_cleaner_DiosWolf.files_editors.editor_restore_state import EditorRestoreFile
 from HA_cfg_cleaner_DiosWolf.files_editors.fileIO_cls import FileIO
 from HA_cfg_cleaner_DiosWolf.files_editors.file_folder_editor_cls import (
     FileFoldersEditor,
 )
@@ -166,21 +166,37 @@
                 print("Error, check log file")
                 logging.error(f"Exception {e.error_text}")
 
     def disable_addons(self):
         ids_list: list[str] = self.all_instructions.disable_addons.ids_list
         for addon_id in ids_list:
             try:
+                addon_editor = AddonsEditor(self.all_configs.ssh_commands, self.all_configs.host_info)
+                addon_editor.stop_autoboot(addon_id)
+
                 addon_editor = AddonsEditor(self.all_configs.ssh_commands)
                 addon_editor.use_ssh_addon(
                     addon_id, self.all_configs.ssh_commands.disable_addons
                 )
+
+            except Exception as e:
+                print("Error, check log file")
+                logging.error("Exception", exc_info=True)
+
+    def change_addons_options(self):
+        addons_dict: list[ChangeAddonsOptions] = self.all_instructions.change_addons_options
+        for addon_dict in addons_dict:
+
+            try:
+                addon_editor = AddonsEditor(self.all_configs.ssh_commands, self.all_configs.host_info)
+                addon_editor.change_addon_options(addon_dict.addon_id, addon_dict.addon_options)
+
             except Exception as e:
                 print("Error, check log file")
-                logging.error("Exception")
+                logging.error("Exception", exc_info=True)
 
     def del_script(self):
         for instruction in self.all_instructions.delete_script:
 
             full_cfg = self.file_io.read_with_type(instruction.path)
             script_editor = ScriptsEditor(full_cfg)
```

### Comparing `HA_cfg_cleaner_DiosWolf-0.0.29/HA_cfg_cleaner_DiosWolf/main.py` & `HA_cfg_cleaner_DiosWolf-0.0.36/HA_cfg_cleaner_DiosWolf/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,14 +35,16 @@
         self.instruction_executor.del_automations_restore_state()
         print("disabling automations")
         self.instruction_executor.disable_automations()
         print("deletion addons")
         self.instruction_executor.del_addons()
         print("disabling addons")
         self.instruction_executor.disable_addons()
+        print("changing addons options")
+        self.instruction_executor.change_addons_options()
         print("changing files")
         self.instruction_executor.change_files()
         print("deletion scripts")
         self.instruction_executor.del_script()
         self.instruction_executor.del_script_restore_state()
         print("deletion objects")
         self.instruction_executor.del_objects()
```

### Comparing `HA_cfg_cleaner_DiosWolf-0.0.29/HA_cfg_cleaner_DiosWolf/parse_classes/arguments_parse.py` & `HA_cfg_cleaner_DiosWolf-0.0.36/HA_cfg_cleaner_DiosWolf/parse_classes/arguments_parse.py`

 * *Files identical despite different names*

### Comparing `HA_cfg_cleaner_DiosWolf-0.0.29/HA_cfg_cleaner_DiosWolf.egg-info/SOURCES.txt` & `HA_cfg_cleaner_DiosWolf-0.0.36/HA_cfg_cleaner_DiosWolf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `HA_cfg_cleaner_DiosWolf-0.0.29/LICENSE` & `HA_cfg_cleaner_DiosWolf-0.0.36/LICENSE`

 * *Files identical despite different names*

### Comparing `HA_cfg_cleaner_DiosWolf-0.0.29/setup.py` & `HA_cfg_cleaner_DiosWolf-0.0.36/setup.py`

 * *Files identical despite different names*

