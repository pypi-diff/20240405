# Comparing `tmp/nakivo_prometheus_exporter-0.2.1.tar.gz` & `tmp/nakivo_prometheus_exporter-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nakivo_prometheus_exporter-0.2.1.tar", last modified: Wed Apr  3 14:01:21 2024, max compression
+gzip compressed data, was "nakivo_prometheus_exporter-0.2.2.tar", last modified: Fri Apr  5 14:14:44 2024, max compression
```

## Comparing `nakivo_prometheus_exporter-0.2.1.tar` & `nakivo_prometheus_exporter-0.2.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 14:01:21.332663 nakivo_prometheus_exporter-0.2.1/
--rw-rw-rw-   0        0        0     5002 2024-04-03 14:01:21.331659 nakivo_prometheus_exporter-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     3448 2024-04-03 14:00:52.000000 nakivo_prometheus_exporter-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-03 14:01:21.318660 nakivo_prometheus_exporter-0.2.1/nakivo_prometheus_exporter/
--rw-rw-rw-   0        0        0      104 2024-04-03 14:00:52.000000 nakivo_prometheus_exporter-0.2.1/nakivo_prometheus_exporter/__init__.py
--rw-rw-rw-   0        0        0      433 2024-04-03 14:00:52.000000 nakivo_prometheus_exporter-0.2.1/nakivo_prometheus_exporter/__version__.py
--rw-rw-rw-   0        0        0     3375 2024-04-03 14:00:52.000000 nakivo_prometheus_exporter-0.2.1/nakivo_prometheus_exporter/metrics.py
--rw-rw-rw-   0        0        0     4081 2024-04-03 14:00:52.000000 nakivo_prometheus_exporter-0.2.1/nakivo_prometheus_exporter/nakivo_api.py
--rw-rw-rw-   0        0        0     9955 2024-04-03 14:00:52.000000 nakivo_prometheus_exporter-0.2.1/nakivo_prometheus_exporter/prom_parser.py
--rw-rw-rw-   0        0        0     4659 2024-04-03 14:00:52.000000 nakivo_prometheus_exporter-0.2.1/nakivo_prometheus_exporter/server.py
-drwxrwxrwx   0        0        0        0 2024-04-03 14:01:21.329659 nakivo_prometheus_exporter-0.2.1/nakivo_prometheus_exporter.egg-info/
--rw-rw-rw-   0        0        0     5002 2024-04-03 14:01:21.000000 nakivo_prometheus_exporter-0.2.1/nakivo_prometheus_exporter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      559 2024-04-03 14:01:21.000000 nakivo_prometheus_exporter-0.2.1/nakivo_prometheus_exporter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 14:01:21.000000 nakivo_prometheus_exporter-0.2.1/nakivo_prometheus_exporter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       86 2024-04-03 14:01:21.000000 nakivo_prometheus_exporter-0.2.1/nakivo_prometheus_exporter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      169 2024-04-03 14:01:21.000000 nakivo_prometheus_exporter-0.2.1/nakivo_prometheus_exporter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2024-04-03 14:01:21.000000 nakivo_prometheus_exporter-0.2.1/nakivo_prometheus_exporter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-03 14:01:21.332663 nakivo_prometheus_exporter-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     5248 2024-04-03 14:00:52.000000 nakivo_prometheus_exporter-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 14:14:44.941533 nakivo_prometheus_exporter-0.2.2/
+-rw-rw-rw-   0        0        0     5683 2024-04-05 14:14:44.941533 nakivo_prometheus_exporter-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3816 2024-04-05 13:49:48.000000 nakivo_prometheus_exporter-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-05 14:14:44.891649 nakivo_prometheus_exporter-0.2.2/nakivo_prometheus_exporter/
+-rw-rw-rw-   0        0        0     1651 2024-04-05 13:26:41.000000 nakivo_prometheus_exporter-0.2.2/nakivo_prometheus_exporter/__debug__.py
+-rw-rw-rw-   0        0        0      104 2024-03-26 13:49:20.000000 nakivo_prometheus_exporter-0.2.2/nakivo_prometheus_exporter/__init__.py
+-rw-rw-rw-   0        0        0      440 2024-04-05 14:13:45.000000 nakivo_prometheus_exporter-0.2.2/nakivo_prometheus_exporter/__version__.py
+-rw-rw-rw-   0        0        0     3382 2024-04-05 13:24:38.000000 nakivo_prometheus_exporter-0.2.2/nakivo_prometheus_exporter/metrics.py
+-rw-rw-rw-   0        0        0     4088 2024-04-05 13:24:38.000000 nakivo_prometheus_exporter-0.2.2/nakivo_prometheus_exporter/nakivo_api.py
+-rw-rw-rw-   0        0        0    11030 2024-04-05 13:58:47.000000 nakivo_prometheus_exporter-0.2.2/nakivo_prometheus_exporter/prom_parser.py
+-rw-rw-rw-   0        0        0     4715 2024-04-05 13:54:13.000000 nakivo_prometheus_exporter-0.2.2/nakivo_prometheus_exporter/server.py
+drwxrwxrwx   0        0        0        0 2024-04-05 14:14:44.932890 nakivo_prometheus_exporter-0.2.2/nakivo_prometheus_exporter.egg-info/
+-rw-rw-rw-   0        0        0     5683 2024-04-05 14:14:44.000000 nakivo_prometheus_exporter-0.2.2/nakivo_prometheus_exporter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      599 2024-04-05 14:14:44.000000 nakivo_prometheus_exporter-0.2.2/nakivo_prometheus_exporter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 14:14:44.000000 nakivo_prometheus_exporter-0.2.2/nakivo_prometheus_exporter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       86 2024-04-05 14:14:44.000000 nakivo_prometheus_exporter-0.2.2/nakivo_prometheus_exporter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      169 2024-04-05 14:14:44.000000 nakivo_prometheus_exporter-0.2.2/nakivo_prometheus_exporter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2024-04-05 14:14:44.000000 nakivo_prometheus_exporter-0.2.2/nakivo_prometheus_exporter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-05 14:14:44.944702 nakivo_prometheus_exporter-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     5248 2024-03-26 16:09:56.000000 nakivo_prometheus_exporter-0.2.2/setup.py
```

### Comparing `nakivo_prometheus_exporter-0.2.1/PKG-INFO` & `nakivo_prometheus_exporter-0.2.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nakivo_prometheus_exporter
-Version: 0.2.1
+Version: 0.2.2
 Summary: Connecto to Nakivo API and export metrics to Prometheus
 Home-page: https://github.com/netinvent/nakivo_prometheus_exporter
 Author: NetInvent - Orsiris de Jong
 Author-email: contact@netinvent.fr
 License: GPLv3
 Keywords: shell,backup,prometheus,linux,cli
 Classifier: Development Status :: 5 - Production/Stable
@@ -27,14 +27,23 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: POSIX :: Linux
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Requires-Dist: ruamel.yaml
+Requires-Dist: ofunctions.requestor>=1.1.0
+Requires-Dist: ofunctions.logger_utils
+Requires-Dist: ofunctions.logger_utils>=2.4.0
+Requires-Dist: gunicorn
+Requires-Dist: uvicorn[standard]
+Requires-Dist: fastapi
+Requires-Dist: fastapi-offline>=1.5.0
+Requires-Dist: pydantic~=2.6.3
 
 [![License](https://img.shields.io/badge/license-GPLv3-blu.svg)](https://opensource.org/licenses/GPL-3.0)
 [![Percentage of issues still open](http://isitmaintained.com/badge/open/netinvent/nakivo_prometheus_exporter.svg)](http://isitmaintained.com/project/netinvent/nakivo_prometheus_exporter "Percentage of issues still open")
 [![GitHub Release](https://img.shields.io/github/release/netinvent/nakivo_prometheus_exporter.svg?label=Latest)](https://github.com/netinvent/nakivo_prometheus_exporter/releases/latest)
 [![Linux linter](https://github.com/netinvent/nakivo_prometheus_exporter/actions/workflows/pylint-linux.yaml/badge.svg)](https://github.com/netinvent/nakivo_prometheus_exporter/actions/workflows/pylint-linux.yaml)
 
 ## Nakivo Prometheus exporter
@@ -42,27 +51,35 @@
 This tool connects to Navkio Backup & Replication API endpoints, and fetches licensing and backup  information in order to present this data as prometheus metrics that can be pulled via a `/metrics` endpoint.
 
 ## Compatibility
 
 This project has been tested on Nakivo Backup & Replication v9 and v10.  
 It runs on most Linux flavors that have Python 3.6+, and can even run on Windows.
 
+So far, Nakivo requires you to have an enterprise plus license to be able to use the API.
+
+Requires python-pip for setup via `dnf install python3-pip` or `apt-get install python3-pip`
+
 ## Grafana dashboard
 
 The exporter comes with a basic Grafana Dashboard, showing:
 - Licensing status
 - Backup states for objects of per job
 - Backup sizes
 - Backup durations
 
 ![image](examples/grafana_dashboard_v0.1b.png)
 ![image](examples/grafana_dashboard_v0.1.png)
 
 ## Quick start
 
+Create a readonly API user (View only role) so your exporter doesn't have more rights than it should.
+![image](examples/nakivo_readonly_user.png)
+
+
 Grab yourself a copy of `nakivo_prometheus_exporter` by running
 ```
 python3 pip install nakivo_prometheus_exporter
 ```
 
 Create your YAML config file in let's say `/etc/nakivo_prometheus_exporter.yaml`
 ```
@@ -92,15 +109,15 @@
 nakivo_prometheus_exporter --config-file=/etc/nakivo_prometheus_eporter.yaml
 ```
 Once running, you might want to check the metrics with:
 ```
 curl http://localhost:9119/metrics
 ```
 
-If everything works, you can use the provided systemd service file, copy it into `/etc/systemd/system` and run the service with
+If everything works, you can use the provided systemd service file from the systemd directory, copy it into `/etc/systemd/system` and run the service with
 ```
 systemctl enable --now nakivo_prometheus_exporter
 ```
 
 ## Caveats
 
 Since on every scraping, the exporter connects to *ALL* Nakivo API endpoints defined in the host section, you should set the scraper interval to something reasonable like 1 hour.
```

### Comparing `nakivo_prometheus_exporter-0.2.1/README.md` & `nakivo_prometheus_exporter-0.2.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -8,27 +8,35 @@
 This tool connects to Navkio Backup & Replication API endpoints, and fetches licensing and backup  information in order to present this data as prometheus metrics that can be pulled via a `/metrics` endpoint.
 
 ## Compatibility
 
 This project has been tested on Nakivo Backup & Replication v9 and v10.  
 It runs on most Linux flavors that have Python 3.6+, and can even run on Windows.
 
+So far, Nakivo requires you to have an enterprise plus license to be able to use the API.
+
+Requires python-pip for setup via `dnf install python3-pip` or `apt-get install python3-pip`
+
 ## Grafana dashboard
 
 The exporter comes with a basic Grafana Dashboard, showing:
 - Licensing status
 - Backup states for objects of per job
 - Backup sizes
 - Backup durations
 
 ![image](examples/grafana_dashboard_v0.1b.png)
 ![image](examples/grafana_dashboard_v0.1.png)
 
 ## Quick start
 
+Create a readonly API user (View only role) so your exporter doesn't have more rights than it should.
+![image](examples/nakivo_readonly_user.png)
+
+
 Grab yourself a copy of `nakivo_prometheus_exporter` by running
 ```
 python3 pip install nakivo_prometheus_exporter
 ```
 
 Create your YAML config file in let's say `/etc/nakivo_prometheus_exporter.yaml`
 ```
@@ -58,15 +66,15 @@
 nakivo_prometheus_exporter --config-file=/etc/nakivo_prometheus_eporter.yaml
 ```
 Once running, you might want to check the metrics with:
 ```
 curl http://localhost:9119/metrics
 ```
 
-If everything works, you can use the provided systemd service file, copy it into `/etc/systemd/system` and run the service with
+If everything works, you can use the provided systemd service file from the systemd directory, copy it into `/etc/systemd/system` and run the service with
 ```
 systemctl enable --now nakivo_prometheus_exporter
 ```
 
 ## Caveats
 
 Since on every scraping, the exporter connects to *ALL* Nakivo API endpoints defined in the host section, you should set the scraper interval to something reasonable like 1 hour.
```

### Comparing `nakivo_prometheus_exporter-0.2.1/nakivo_prometheus_exporter/metrics.py` & `nakivo_prometheus_exporter-0.2.2/nakivo_prometheus_exporter/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #! /usr/bin/env python
 #  -*- coding: utf-8 -*-
 #
 # This file is part of nakivo_prometheus_exporter
 
 __appname__ = "nakivo_prometheus_exporter"
 __author__ = "Orsiris de Jong"
-__site__ = "https://www.netperfect.fr/nakivo_prometheus_exporter"
+__site__ = "https://www.github.com/netinvent/nakivo_prometheus_exporter"
 __description__ = "Naviko API Prometheus data exporter"
 __copyright__ = "Copyright (C) 2024 NetInvent"
 __license__ = "GPL-3.0-only"
 __build__ = "2024032601"
 
 
 import logging
```

### Comparing `nakivo_prometheus_exporter-0.2.1/nakivo_prometheus_exporter/nakivo_api.py` & `nakivo_prometheus_exporter-0.2.2/nakivo_prometheus_exporter/nakivo_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #! /usr/bin/env python
 #  -*- coding: utf-8 -*-
 #
 # This file is part of nakivo_prometheus_exporter
 
 __appname__ = "nakivo_prometheus_exporter"
 __author__ = "Orsiris de Jong"
-__site__ = "https://www.netperfect.fr/nakivo_prometheus_exporter"
+__site__ = "https://www.github.com/netinvent/nakivo_prometheus_exporter"
 __description__ = "Naviko API Prometheus data exporter"
 __copyright__ = "Copyright (C) 2024 NetInvent"
 __license__ = "GPL-3.0-only"
 __build__ = "2024032601"
 
 from typing import Union, List
 from ofunctions.requestor import Requestor
```

### Comparing `nakivo_prometheus_exporter-0.2.1/nakivo_prometheus_exporter/prom_parser.py` & `nakivo_prometheus_exporter-0.2.2/nakivo_prometheus_exporter/prom_parser.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 #! /usr/bin/env python
 #  -*- coding: utf-8 -*-
 #
 # This file is part of nakivo_prometheus_exporter
 
 __appname__ = "nakivo_prometheus_exporter"
 __author__ = "Orsiris de Jong"
-__site__ = "https://www.netperfect.fr/nakivo_prometheus_exporter"
+__site__ = "https://www.github.com/netinvent/nakivo_prometheus_exporter"
 __description__ = "Naviko API Prometheus data exporter"
 __copyright__ = "Copyright (C) 2024 NetInvent"
 __license__ = "GPL-3.0-only"
-__build__ = "2024040301"
+__build__ = "2024040501"
 
 
 import sys
 from argparse import ArgumentParser
 from typing import Union
 from ruamel.yaml import YAML
 from pathlib import Path
-from ofunctions.logger_utils import logger_get_logger
+from logging import getLogger
 from nakivo_prometheus_exporter.nakivo_api import NakivoAPI
 
-logger = logger_get_logger()
+logger = getLogger()
 
 
 # Monkeypatching ruamel.yaml ordreddict so we get to use pseudo dot notations
 # eg data.g('my.array.keys') == data['my']['array']['keys']
 # and data.s('my.array.keys', 'new_value')
 def g(self, path, sep=".", default=None, list_ok=False):
     """
@@ -47,63 +47,79 @@
                 return False
             return full_config
     except OSError:
         logger.critical(f"Cannot load configuration file from {config_file}")
         return False
 
 
+def intercept_api_errors(api_return: dict, host: str):
+    """
+    Intercept API return and check for errors
+    """
+    try:
+        if api_return["type"] == "exception":
+            logger.error(f"API replied: {api_return['message']}")
+            logger.debug(f"Full API return: {api_return}")
+            return True
+    except (IndexError, KeyError, TypeError, AttributeError):
+        pass
+
+
 def license_to_prometheus(license_data: dict, host: str):
     """
     Extract Nakivo license status from Job result
     """
+    if intercept_api_errors(license_data, host):
+        return False
+
     try:
         installed = 1 if license_data["data"]["installed"] else 0
-    except KeyError:
+    except (IndexError, KeyError, TypeError, AttributeError):
         installed = 0
     try:
         client = license_data["data"]["client"]
-    except KeyError:
+    except (IndexError, KeyError, TypeError, AttributeError):
         client = None
     try:
         vmcount = license_data["data"]["usedVms"]
-    except KeyError:
+    except (IndexError, KeyError, TypeError, AttributeError):
         vmcount = 0
     try:
         sockets = license_data["data"]["usedSockets"]
-    except KeyError:
+    except (IndexError, KeyError, TypeError, AttributeError):
         sockets = 0
     try:
         ec2 = license_data["data"]["usedEc2Instances"]
-    except KeyError:
+    except (IndexError, KeyError, TypeError, AttributeError):
         ec2 = 0
     try:
         physical_servers = license_data["data"]["usedPhysicalServers"]
-    except KeyError:
+    except (IndexError, KeyError, TypeError, AttributeError):
         physical_servers = 0
     try:
         physical_workstations = license_data["data"]["usedPhysicalWorkstations"]
-    except KeyError:
+    except (IndexError, KeyError, TypeError, AttributeError):
         physical_workstations = 0
     try:
         o365users = license_data["data"]["usedOffice365Users"]
-    except KeyError:
+    except (IndexError, KeyError, TypeError, AttributeError):
         o365users = 0
     try:
         oracledb = license_data["data"]["usedOracleDatabases"]
-    except KeyError:
+    except (IndexError, KeyError, TypeError, AttributeError):
         oracledb = 0
     try:
         monitoredvm = license_data["data"]["usedMonitoredVms"]
-    except KeyError:
+    except (IndexError, KeyError, TypeError, AttributeError):
         monitoredvm = 0
     try:
         expiration = round(
             license_data["data"]["expiresIn"] / 1000
         )  # milliseconds to seconds
-    except KeyError:
+    except (IndexError, KeyError, TypeError, AttributeError):
         expiration = 0
 
     prom_data = f'# HELP nakivo_license_installed Is the Nakivo instance licensed\n\
 # TYPE nakivo_license_installed gauge\n\
 nakivo_license_installed{{host="{host}",client="{client}"}} {installed}\n\
 # HELP nakivo_license_vmcount How many VMs do we backup\n\
 # TYPE nakivo_license_vmcount gauge\n\
@@ -135,14 +151,17 @@
     return prom_data
 
 
 def get_vm_backup_result(job_result: dict, host: str, filter_active_only: bool = True):
     """
     Extract VM backup status from Nakvio Job result
     """
+    if intercept_api_errors(job_result, host):
+        return False
+
     vm_job_state = []
     prom_data = "# HELP nakivo_backup_state When will the license expire (seconds)\n\
 # TYPE nakivo_backup_state gauge\n\
 # HELP nakivo_backup_state Backup duration (seconds)\n\
 # TYPE nakivo_backup_state gauge\n\
 # HELP nakivo_backup_state Backup size (bytes)\n\
 # TYPE nakivo_backup_state gauge\n"
@@ -201,23 +220,25 @@
         if not license:
             logger.error(f"Cannot get license data for {host}")
             prom_data = f'nakivo_license_installed{{host="{host}"}} 0'
         else:
             prom_data = license_to_prometheus(license, host)
     except Exception as exc:
         logger.error(f"Cannot retrieve license data for {host}: {exc}")
+        logger.debug("Trace", exc_info=True)
 
     try:
         jobs = api.get_jobs()
         if not jobs:
             logger.error(f"Cannot get job info for {host}")
         else:
             prom_data += get_vm_backup_result(jobs, host)
     except Exception as exc:
         logger.error(f"Cannot retrieve job data for {host}: {exc}")
+        logger.debug("Trace", exc_info=True)
     return prom_data
 
 
 def main():
     default_config_file = "nakivo_prometheus_exporter.yaml"
 
     parser = ArgumentParser(
```

### Comparing `nakivo_prometheus_exporter-0.2.1/nakivo_prometheus_exporter/server.py` & `nakivo_prometheus_exporter-0.2.2/nakivo_prometheus_exporter/server.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #! /usr/bin/env python
 #  -*- coding: utf-8 -*-
 #
 # This file is part of nakivo_prometheus_exporter
 
 __appname__ = "nakivo_prometheus_exporter"
 __author__ = "Orsiris de Jong"
-__site__ = "https://www.netperfect.fr/nakivo_prometheus_exporter"
+__site__ = "https://www.github.com/netinvent/nakivo_prometheus_exporter"
 __description__ = "Naviko API Prometheus data exporter"
 __copyright__ = "Copyright (C) 2024 NetInvent"
 __license__ = "GPL-3.0-only"
 __build__ = "2024032601"
 
 
 import sys
@@ -17,19 +17,20 @@
 
 # Fix dev env module import
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
 from pathlib import Path
 from argparse import ArgumentParser
 from nakivo_prometheus_exporter.prom_parser import load_config_file
 from nakivo_prometheus_exporter import metrics
+from nakivo_prometheus_exporter.__debug__ import _DEBUG
 from ofunctions.logger_utils import logger_get_logger
 
 
 def main():
-    logger = logger_get_logger()
+    logger = logger_get_logger(debug=_DEBUG)
     _DEV = os.environ.get("_DEV", False)
 
     default_config_file = "nakivo_prometheus_exporter.yaml"
 
     parser = ArgumentParser(
         prog=f"{__appname__}",
         description="""Naviko API Prometheus exporter\n
@@ -59,15 +60,15 @@
 
     config_dict = load_config_file(config_file)
     if not config_dict:
         logger.critical(f"Cannot load configuration file {config_file}")
         sys.exit(1)
 
     try:
-        logger = logger_get_logger(config_dict["http_server"]["log_file"])
+        logger = logger_get_logger(config_dict["http_server"]["log_file"], debug=_DEBUG)
     except (AttributeError, KeyError, IndexError, TypeError):
         pass
 
     if args.dev:
         _DEV = True
 
     try:
@@ -75,15 +76,14 @@
     except (TypeError, KeyError):
         listen = None
     try:
         port = config_dict["http_server"]["port"]
     except (TypeError, KeyError):
         port = None
 
-    logger = logger_get_logger()
     # Cannot use gunicorn on Windows
     if _DEV or os.name == "nt":
         logger.info("Running dev version")
         import uvicorn
 
         server_args = {
             "workers": 1,
```

### Comparing `nakivo_prometheus_exporter-0.2.1/nakivo_prometheus_exporter.egg-info/PKG-INFO` & `nakivo_prometheus_exporter-0.2.2/nakivo_prometheus_exporter.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: nakivo-prometheus-exporter
-Version: 0.2.1
+Name: nakivo_prometheus_exporter
+Version: 0.2.2
 Summary: Connecto to Nakivo API and export metrics to Prometheus
 Home-page: https://github.com/netinvent/nakivo_prometheus_exporter
 Author: NetInvent - Orsiris de Jong
 Author-email: contact@netinvent.fr
 License: GPLv3
 Keywords: shell,backup,prometheus,linux,cli
 Classifier: Development Status :: 5 - Production/Stable
@@ -27,14 +27,23 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: POSIX :: Linux
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Requires-Dist: ruamel.yaml
+Requires-Dist: ofunctions.requestor>=1.1.0
+Requires-Dist: ofunctions.logger_utils
+Requires-Dist: ofunctions.logger_utils>=2.4.0
+Requires-Dist: gunicorn
+Requires-Dist: uvicorn[standard]
+Requires-Dist: fastapi
+Requires-Dist: fastapi-offline>=1.5.0
+Requires-Dist: pydantic~=2.6.3
 
 [![License](https://img.shields.io/badge/license-GPLv3-blu.svg)](https://opensource.org/licenses/GPL-3.0)
 [![Percentage of issues still open](http://isitmaintained.com/badge/open/netinvent/nakivo_prometheus_exporter.svg)](http://isitmaintained.com/project/netinvent/nakivo_prometheus_exporter "Percentage of issues still open")
 [![GitHub Release](https://img.shields.io/github/release/netinvent/nakivo_prometheus_exporter.svg?label=Latest)](https://github.com/netinvent/nakivo_prometheus_exporter/releases/latest)
 [![Linux linter](https://github.com/netinvent/nakivo_prometheus_exporter/actions/workflows/pylint-linux.yaml/badge.svg)](https://github.com/netinvent/nakivo_prometheus_exporter/actions/workflows/pylint-linux.yaml)
 
 ## Nakivo Prometheus exporter
@@ -42,27 +51,35 @@
 This tool connects to Navkio Backup & Replication API endpoints, and fetches licensing and backup  information in order to present this data as prometheus metrics that can be pulled via a `/metrics` endpoint.
 
 ## Compatibility
 
 This project has been tested on Nakivo Backup & Replication v9 and v10.  
 It runs on most Linux flavors that have Python 3.6+, and can even run on Windows.
 
+So far, Nakivo requires you to have an enterprise plus license to be able to use the API.
+
+Requires python-pip for setup via `dnf install python3-pip` or `apt-get install python3-pip`
+
 ## Grafana dashboard
 
 The exporter comes with a basic Grafana Dashboard, showing:
 - Licensing status
 - Backup states for objects of per job
 - Backup sizes
 - Backup durations
 
 ![image](examples/grafana_dashboard_v0.1b.png)
 ![image](examples/grafana_dashboard_v0.1.png)
 
 ## Quick start
 
+Create a readonly API user (View only role) so your exporter doesn't have more rights than it should.
+![image](examples/nakivo_readonly_user.png)
+
+
 Grab yourself a copy of `nakivo_prometheus_exporter` by running
 ```
 python3 pip install nakivo_prometheus_exporter
 ```
 
 Create your YAML config file in let's say `/etc/nakivo_prometheus_exporter.yaml`
 ```
@@ -92,15 +109,15 @@
 nakivo_prometheus_exporter --config-file=/etc/nakivo_prometheus_eporter.yaml
 ```
 Once running, you might want to check the metrics with:
 ```
 curl http://localhost:9119/metrics
 ```
 
-If everything works, you can use the provided systemd service file, copy it into `/etc/systemd/system` and run the service with
+If everything works, you can use the provided systemd service file from the systemd directory, copy it into `/etc/systemd/system` and run the service with
 ```
 systemctl enable --now nakivo_prometheus_exporter
 ```
 
 ## Caveats
 
 Since on every scraping, the exporter connects to *ALL* Nakivo API endpoints defined in the host section, you should set the scraper interval to something reasonable like 1 hour.
```

### Comparing `nakivo_prometheus_exporter-0.2.1/nakivo_prometheus_exporter.egg-info/SOURCES.txt` & `nakivo_prometheus_exporter-0.2.2/nakivo_prometheus_exporter.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 README.md
 setup.py
+nakivo_prometheus_exporter/__debug__.py
 nakivo_prometheus_exporter/__init__.py
 nakivo_prometheus_exporter/__version__.py
 nakivo_prometheus_exporter/metrics.py
 nakivo_prometheus_exporter/nakivo_api.py
 nakivo_prometheus_exporter/prom_parser.py
 nakivo_prometheus_exporter/server.py
 nakivo_prometheus_exporter.egg-info/PKG-INFO
```

### Comparing `nakivo_prometheus_exporter-0.2.1/setup.py` & `nakivo_prometheus_exporter-0.2.2/setup.py`

 * *Files identical despite different names*

