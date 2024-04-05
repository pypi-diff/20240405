# Comparing `tmp/procustodibus_agent-1.4.5.tar.gz` & `tmp/procustodibus_agent-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "procustodibus_agent-1.4.5.tar", last modified: Tue Jan 16 00:04:56 2024, max compression
+gzip compressed data, was "procustodibus_agent-1.5.0.tar", last modified: Fri Apr  5 20:29:39 2024, max compression
```

## Comparing `procustodibus_agent-1.4.5.tar` & `procustodibus_agent-1.5.0.tar`

### file list

```diff
@@ -1,38 +1,45 @@
-drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2024-01-16 00:04:56.294914 procustodibus_agent-1.4.5/
--rw-rw-r--   0 justin    (1000) justin    (1000)     1076 2024-01-15 23:37:44.000000 procustodibus_agent-1.4.5/LICENSE
--rw-rw-r--   0 justin    (1000) justin    (1000)       30 2021-11-09 19:41:28.000000 procustodibus_agent-1.4.5/MANIFEST.in
--rw-r--r--   0 justin    (1000) justin    (1000)     7025 2024-01-16 00:04:56.294914 procustodibus_agent-1.4.5/PKG-INFO
--rw-rw-r--   0 justin    (1000) justin    (1000)     3927 2023-12-27 16:47:03.000000 procustodibus_agent-1.4.5/README.md
-drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2024-01-16 00:04:56.282858 procustodibus_agent-1.4.5/procustodibus_agent/
--rw-rw-r--   0 justin    (1000) justin    (1000)      208 2024-01-15 23:48:29.000000 procustodibus_agent-1.4.5/procustodibus_agent/__init__.py
--rw-rw-r--   0 justin    (1000) justin    (1000)     2898 2023-10-08 21:10:01.000000 procustodibus_agent-1.4.5/procustodibus_agent/agent.py
--rw-rw-r--   0 justin    (1000) justin    (1000)    10970 2023-12-10 23:12:39.000000 procustodibus_agent-1.4.5/procustodibus_agent/api.py
--rw-rw-r--   0 justin    (1000) justin    (1000)     1889 2023-12-10 23:12:39.000000 procustodibus_agent-1.4.5/procustodibus_agent/cli.py
--rw-rw-r--   0 justin    (1000) justin    (1000)    16781 2023-12-27 16:47:02.000000 procustodibus_agent-1.4.5/procustodibus_agent/cnf.py
--rw-rw-r--   0 justin    (1000) justin    (1000)     5464 2024-01-15 23:37:44.000000 procustodibus_agent-1.4.5/procustodibus_agent/connectivity.py
--rw-rw-r--   0 justin    (1000) justin    (1000)     1398 2022-06-29 01:32:50.000000 procustodibus_agent-1.4.5/procustodibus_agent/credentials.py
--rw-rw-r--   0 justin    (1000) justin    (1000)    40414 2023-10-08 21:10:01.000000 procustodibus_agent-1.4.5/procustodibus_agent/executor.py
--rw-rw-r--   0 justin    (1000) justin    (1000)     4950 2023-10-08 21:10:01.000000 procustodibus_agent-1.4.5/procustodibus_agent/ip_route.py
-drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2024-01-16 00:04:56.286876 procustodibus_agent-1.4.5/procustodibus_agent/mfa/
--rw-rw-r--   0 justin    (1000) justin    (1000)     7123 2022-06-29 01:32:56.000000 procustodibus_agent-1.4.5/procustodibus_agent/mfa/__init__.py
--rw-rw-r--   0 justin    (1000) justin    (1000)     2656 2023-03-17 00:35:09.000000 procustodibus_agent-1.4.5/procustodibus_agent/mfa/api.py
--rw-rw-r--   0 justin    (1000) justin    (1000)     4347 2022-06-29 01:32:56.000000 procustodibus_agent-1.4.5/procustodibus_agent/mfa/cli.py
--rw-rw-r--   0 justin    (1000) justin    (1000)     4073 2021-08-02 23:52:55.000000 procustodibus_agent-1.4.5/procustodibus_agent/resolve_hostname.py
--rw-rw-r--   0 justin    (1000) justin    (1000)     3841 2021-05-16 20:05:23.000000 procustodibus_agent-1.4.5/procustodibus_agent/wg.py
--rw-rw-r--   0 justin    (1000) justin    (1000)    13166 2023-12-27 16:47:02.000000 procustodibus_agent-1.4.5/procustodibus_agent/wg_cnf.py
-drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2024-01-16 00:04:56.286876 procustodibus_agent-1.4.5/procustodibus_agent.egg-info/
--rw-r--r--   0 justin    (1000) justin    (1000)     7025 2024-01-16 00:04:56.000000 procustodibus_agent-1.4.5/procustodibus_agent.egg-info/PKG-INFO
--rw-rw-r--   0 justin    (1000) justin    (1000)      919 2024-01-16 00:04:56.000000 procustodibus_agent-1.4.5/procustodibus_agent.egg-info/SOURCES.txt
--rw-rw-r--   0 justin    (1000) justin    (1000)        1 2024-01-16 00:04:56.000000 procustodibus_agent-1.4.5/procustodibus_agent.egg-info/dependency_links.txt
--rw-rw-r--   0 justin    (1000) justin    (1000)      187 2024-01-16 00:04:56.000000 procustodibus_agent-1.4.5/procustodibus_agent.egg-info/entry_points.txt
--rw-rw-r--   0 justin    (1000) justin    (1000)      671 2024-01-16 00:04:56.000000 procustodibus_agent-1.4.5/procustodibus_agent.egg-info/requires.txt
--rw-rw-r--   0 justin    (1000) justin    (1000)       20 2024-01-16 00:04:56.000000 procustodibus_agent-1.4.5/procustodibus_agent.egg-info/top_level.txt
--rw-rw-r--   0 justin    (1000) justin    (1000)        1 2020-08-17 01:25:01.000000 procustodibus_agent-1.4.5/procustodibus_agent.egg-info/zip-safe
--rw-rw-r--   0 justin    (1000) justin    (1000)       92 2022-09-26 02:20:41.000000 procustodibus_agent-1.4.5/pyproject.toml
-drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2024-01-16 00:04:56.286876 procustodibus_agent-1.4.5/requirements/
--rw-rw-r--   0 justin    (1000) justin    (1000)       50 2020-08-14 21:08:08.000000 procustodibus_agent-1.4.5/requirements/dev.txt
--rw-rw-r--   0 justin    (1000) justin    (1000)      585 2023-03-17 00:35:09.000000 procustodibus_agent-1.4.5/requirements/lint.txt
--rw-rw-r--   0 justin    (1000) justin    (1000)       82 2023-03-16 01:04:31.000000 procustodibus_agent-1.4.5/requirements/prod.txt
--rw-rw-r--   0 justin    (1000) justin    (1000)       73 2020-10-09 21:04:40.000000 procustodibus_agent-1.4.5/requirements/test.txt
--rw-rw-r--   0 justin    (1000) justin    (1000)      556 2024-01-16 00:04:56.294914 procustodibus_agent-1.4.5/setup.cfg
--rw-rw-r--   0 justin    (1000) justin    (1000)     2194 2023-12-27 16:47:03.000000 procustodibus_agent-1.4.5/setup.py
+drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2024-04-05 20:29:39.370915 procustodibus_agent-1.5.0/
+-rw-rw-r--   0 justin    (1000) justin    (1000)     1076 2024-01-15 23:37:44.000000 procustodibus_agent-1.5.0/LICENSE
+-rw-rw-r--   0 justin    (1000) justin    (1000)       30 2021-11-09 19:41:28.000000 procustodibus_agent-1.5.0/MANIFEST.in
+-rw-r--r--   0 justin    (1000) justin    (1000)     7885 2024-04-05 20:29:39.370915 procustodibus_agent-1.5.0/PKG-INFO
+-rw-rw-r--   0 justin    (1000) justin    (1000)     4732 2024-04-05 18:04:50.000000 procustodibus_agent-1.5.0/README.md
+drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2024-04-05 20:29:39.354905 procustodibus_agent-1.5.0/procustodibus_agent/
+-rw-rw-r--   0 justin    (1000) justin    (1000)      208 2024-04-05 18:04:51.000000 procustodibus_agent-1.5.0/procustodibus_agent/__init__.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)     2898 2023-10-08 21:10:01.000000 procustodibus_agent-1.5.0/procustodibus_agent/agent.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)    10970 2023-12-10 23:12:39.000000 procustodibus_agent-1.5.0/procustodibus_agent/api.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)     1889 2023-12-10 23:12:39.000000 procustodibus_agent-1.5.0/procustodibus_agent/cli.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)    17905 2024-04-05 18:04:49.000000 procustodibus_agent-1.5.0/procustodibus_agent/cnf.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)     5464 2024-01-15 23:37:44.000000 procustodibus_agent-1.5.0/procustodibus_agent/connectivity.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)     1398 2022-06-29 01:32:50.000000 procustodibus_agent-1.5.0/procustodibus_agent/credentials.py
+drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2024-04-05 20:29:39.358908 procustodibus_agent-1.5.0/procustodibus_agent/executor/
+-rw-rw-r--   0 justin    (1000) justin    (1000)      122 2024-04-05 18:04:48.000000 procustodibus_agent-1.5.0/procustodibus_agent/executor/__init__.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)    34310 2024-04-05 18:04:49.000000 procustodibus_agent-1.5.0/procustodibus_agent/executor/execution.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)    20632 2024-04-05 18:04:49.000000 procustodibus_agent-1.5.0/procustodibus_agent/executor/sys_cmd.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)     7432 2024-04-05 18:04:47.000000 procustodibus_agent-1.5.0/procustodibus_agent/ip_route.py
+drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2024-04-05 20:29:39.362910 procustodibus_agent-1.5.0/procustodibus_agent/mfa/
+-rw-rw-r--   0 justin    (1000) justin    (1000)     7123 2022-06-29 01:32:56.000000 procustodibus_agent-1.5.0/procustodibus_agent/mfa/__init__.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)     2656 2023-03-17 00:35:09.000000 procustodibus_agent-1.5.0/procustodibus_agent/mfa/api.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)     4347 2022-06-29 01:32:56.000000 procustodibus_agent-1.5.0/procustodibus_agent/mfa/cli.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)     4073 2021-08-02 23:52:55.000000 procustodibus_agent-1.5.0/procustodibus_agent/resolve_hostname.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)     3841 2021-05-16 20:05:23.000000 procustodibus_agent-1.5.0/procustodibus_agent/wg.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)    13359 2024-04-05 18:04:49.000000 procustodibus_agent-1.5.0/procustodibus_agent/wg_cnf.py
+drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2024-04-05 20:29:39.362910 procustodibus_agent-1.5.0/procustodibus_agent/windows/
+-rw-rw-r--   0 justin    (1000) justin    (1000)     5763 2024-04-05 18:04:50.000000 procustodibus_agent-1.5.0/procustodibus_agent/windows/cnf.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)     2132 2024-04-05 18:04:50.000000 procustodibus_agent-1.5.0/procustodibus_agent/windows/service.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)      344 2024-04-05 18:04:49.000000 procustodibus_agent-1.5.0/procustodibus_agent/windows/service_config.py
+drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2024-04-05 20:29:39.362910 procustodibus_agent-1.5.0/procustodibus_agent.egg-info/
+-rw-r--r--   0 justin    (1000) justin    (1000)     7885 2024-04-05 20:29:39.000000 procustodibus_agent-1.5.0/procustodibus_agent.egg-info/PKG-INFO
+-rw-rw-r--   0 justin    (1000) justin    (1000)     1130 2024-04-05 20:29:39.000000 procustodibus_agent-1.5.0/procustodibus_agent.egg-info/SOURCES.txt
+-rw-rw-r--   0 justin    (1000) justin    (1000)        1 2024-04-05 20:29:39.000000 procustodibus_agent-1.5.0/procustodibus_agent.egg-info/dependency_links.txt
+-rw-rw-r--   0 justin    (1000) justin    (1000)      187 2024-04-05 20:29:39.000000 procustodibus_agent-1.5.0/procustodibus_agent.egg-info/entry_points.txt
+-rw-rw-r--   0 justin    (1000) justin    (1000)      714 2024-04-05 20:29:39.000000 procustodibus_agent-1.5.0/procustodibus_agent.egg-info/requires.txt
+-rw-rw-r--   0 justin    (1000) justin    (1000)       20 2024-04-05 20:29:39.000000 procustodibus_agent-1.5.0/procustodibus_agent.egg-info/top_level.txt
+-rw-rw-r--   0 justin    (1000) justin    (1000)        1 2020-08-17 01:25:01.000000 procustodibus_agent-1.5.0/procustodibus_agent.egg-info/zip-safe
+-rw-rw-r--   0 justin    (1000) justin    (1000)       92 2024-03-17 03:21:19.000000 procustodibus_agent-1.5.0/pyproject.toml
+drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2024-04-05 20:29:39.362910 procustodibus_agent-1.5.0/requirements/
+-rw-rw-r--   0 justin    (1000) justin    (1000)       50 2020-08-14 21:08:08.000000 procustodibus_agent-1.5.0/requirements/dev.txt
+-rw-rw-r--   0 justin    (1000) justin    (1000)      585 2023-03-17 00:35:09.000000 procustodibus_agent-1.5.0/requirements/lint.txt
+-rw-rw-r--   0 justin    (1000) justin    (1000)      124 2024-04-05 18:04:49.000000 procustodibus_agent-1.5.0/requirements/prod.txt
+-rw-rw-r--   0 justin    (1000) justin    (1000)       73 2020-10-09 21:04:40.000000 procustodibus_agent-1.5.0/requirements/test.txt
+-rw-rw-r--   0 justin    (1000) justin    (1000)      591 2024-04-05 20:29:39.370915 procustodibus_agent-1.5.0/setup.cfg
+-rw-rw-r--   0 justin    (1000) justin    (1000)     2273 2024-04-05 18:04:49.000000 procustodibus_agent-1.5.0/setup.py
```

### Comparing `procustodibus_agent-1.4.5/LICENSE` & `procustodibus_agent-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.4.5/PKG-INFO` & `procustodibus_agent-1.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: procustodibus_agent
-Version: 1.4.5
+Version: 1.5.0
 Summary: Synchronizes your WireGuard settings with Pro Custodibus.
 Home-page: https://www.procustodibus.com/
 Author: Arcem Tene
 Author-email: dev@arcemtene.com
 License: MIT
 Project-URL: Changelog, https://docs.procustodibus.com/guide/agents/download/#changelog
 Project-URL: Documentation, https://docs.procustodibus.com/guide/agents/run/
@@ -22,14 +22,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: docopt-ng~=0.7
 Requires-Dist: inflection~=0.5
 Requires-Dist: pynacl~=1.5
+Requires-Dist: pywin32~=306.0; sys_platform == "win32"
 Requires-Dist: requests~=2.27
 Requires-Dist: tabulate~=0.8
 Provides-Extra: lint
 Requires-Dist: cohesion; extra == "lint"
 Requires-Dist: darglint; extra == "lint"
 Requires-Dist: dlint; extra == "lint"
 Requires-Dist: flake8; extra == "lint"
@@ -73,25 +74,25 @@
 
 [Pro Custodibus](https://www.procustodibus.com/) is a service that makes [WireGuard](https://www.wireguard.com/) networks easy to deploy and manage. You run the Pro Custodibus agent on each WireGuard host you want to manage, and the agent monitors and synchronizes the hosts' WireGuard settings with the remote Pro Custodibus service.
 
 
 Installing
 ----------
 
-Requires python 3.7 or newer and libsodium. Installer script can install requirements, plus the agent itself, on most linuxes. Install from source like the following:
+Requires python 3.7 or newer and libsodium. Installer script can install requirements, plus the agent itself, on most linuxes, FreeBSD, OpenBSD, and macOS (if macOS has [Homebrew](https://brew.sh/)). Install from source like the following:
 ```
 ./install.sh --install
 ```
 
 Or run it like the following to see more options:
 ```
 ./install.sh --help
 ```
 
-See the [Installer Documentation](https://docs.procustodibus.com/guide/agents/install/) for full details.
+See the [Installer Documentation](https://docs.procustodibus.com/guide/agents/install/) for full details (or to download the pre-built Windows installer).
 
 
 Docker
 ------
 
 The [docker/wireguard.dockerfile](https://git.sr.ht/~arx10/procustodibus-agent/tree/main/item/docker/wireguard.dockerfile) is built weekly and pushed to the [docker.io/procustodibus/wireguard](https://hub.docker.com/r/procustodibus/wireguard) repository. It produces a base WireGuard image without the agent.
 
@@ -169,14 +170,47 @@
 ```
 
 Manually run pre-push hook on all version-controlled files:
 ```
 tox -e pre-commit -- run -a --hook-stage push
 ```
 
+### Build Windows installer
+
+1. Install [Python](https://www.python.org/downloads/).
+
+2. Install [Inno Setup](https://jrsoftware.org/isdl.php).
+
+3. Create a virtualenv:
+    ```
+    python -m venv C:\venvs\procustodibus-agent
+    ```
+
+4. Activate the virtualenv:
+    ```
+    C:\venvs\procustodibus-agent\Scripts\activate.bat
+    ```
+
+5. Install tox:
+    ```
+    pip install tox
+    ```
+
+6. Build the Windows executables with cx_freeze:
+    ```
+    tox -e build_exe
+    ```
+
+7. Build the Windows installer with Inno Setup:
+    ```
+    "C:\Program Files (x86)\Inno Setup 6\ISCC.exe" installer\windows.iss
+    ```
+
+The installer will be built as `dist\ProCustodibusAgentInstaller.exe`.
+
 
 Contributing
 ------------
 
 * [Code of Conduct](https://docs.procustodibus.com/community/conduct/)
 * [File a Bug](https://docs.procustodibus.com/guide/community/bugs/)
 * [Report a Vulnerability](https://docs.procustodibus.com/guide/community/vulns/)
```

### Comparing `procustodibus_agent-1.4.5/README.md` & `procustodibus_agent-1.5.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 
 [Pro Custodibus](https://www.procustodibus.com/) is a service that makes [WireGuard](https://www.wireguard.com/) networks easy to deploy and manage. You run the Pro Custodibus agent on each WireGuard host you want to manage, and the agent monitors and synchronizes the hosts' WireGuard settings with the remote Pro Custodibus service.
 
 
 Installing
 ----------
 
-Requires python 3.7 or newer and libsodium. Installer script can install requirements, plus the agent itself, on most linuxes. Install from source like the following:
+Requires python 3.7 or newer and libsodium. Installer script can install requirements, plus the agent itself, on most linuxes, FreeBSD, OpenBSD, and macOS (if macOS has [Homebrew](https://brew.sh/)). Install from source like the following:
 ```
 ./install.sh --install
 ```
 
 Or run it like the following to see more options:
 ```
 ./install.sh --help
 ```
 
-See the [Installer Documentation](https://docs.procustodibus.com/guide/agents/install/) for full details.
+See the [Installer Documentation](https://docs.procustodibus.com/guide/agents/install/) for full details (or to download the pre-built Windows installer).
 
 
 Docker
 ------
 
 The [docker/wireguard.dockerfile](https://git.sr.ht/~arx10/procustodibus-agent/tree/main/item/docker/wireguard.dockerfile) is built weekly and pushed to the [docker.io/procustodibus/wireguard](https://hub.docker.com/r/procustodibus/wireguard) repository. It produces a base WireGuard image without the agent.
 
@@ -99,14 +99,47 @@
 ```
 
 Manually run pre-push hook on all version-controlled files:
 ```
 tox -e pre-commit -- run -a --hook-stage push
 ```
 
+### Build Windows installer
+
+1. Install [Python](https://www.python.org/downloads/).
+
+2. Install [Inno Setup](https://jrsoftware.org/isdl.php).
+
+3. Create a virtualenv:
+    ```
+    python -m venv C:\venvs\procustodibus-agent
+    ```
+
+4. Activate the virtualenv:
+    ```
+    C:\venvs\procustodibus-agent\Scripts\activate.bat
+    ```
+
+5. Install tox:
+    ```
+    pip install tox
+    ```
+
+6. Build the Windows executables with cx_freeze:
+    ```
+    tox -e build_exe
+    ```
+
+7. Build the Windows installer with Inno Setup:
+    ```
+    "C:\Program Files (x86)\Inno Setup 6\ISCC.exe" installer\windows.iss
+    ```
+
+The installer will be built as `dist\ProCustodibusAgentInstaller.exe`.
+
 
 Contributing
 ------------
 
 * [Code of Conduct](https://docs.procustodibus.com/community/conduct/)
 * [File a Bug](https://docs.procustodibus.com/guide/community/bugs/)
 * [Report a Vulnerability](https://docs.procustodibus.com/guide/community/vulns/)
```

### Comparing `procustodibus_agent-1.4.5/procustodibus_agent/agent.py` & `procustodibus_agent-1.5.0/procustodibus_agent/agent.py`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.4.5/procustodibus_agent/api.py` & `procustodibus_agent-1.5.0/procustodibus_agent/api.py`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.4.5/procustodibus_agent/cli.py` & `procustodibus_agent-1.5.0/procustodibus_agent/cli.py`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.4.5/procustodibus_agent/cnf.py` & `procustodibus_agent-1.5.0/procustodibus_agent/cnf.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 # -*- coding: utf-8 -*-
 """Config utilities."""
 
 import logging
 import logging.config
 import os
 import sys
+from contextlib import contextmanager
 from os import environ
 from pathlib import Path
 from re import IGNORECASE
 from re import compile as compile_re
 from re import fullmatch, match, split, sub
 
 from inflection import underscore
 
 from procustodibus_agent import DEFAULT_API_URL, DEFAULT_APP_URL
+from procustodibus_agent.windows.cnf import open_dpapi
 
 DEFAULT_WG_CNF_DIRS = [
+    "C:/Program Files/WireGuard/Data/Configurations",
     "/opt/homebrew/etc/wireguard",
     "/usr/local/etc/wireguard",
     "/etc/wireguard",
 ]
 DEFAULT_CNF_DIRS = [
     ".",
+    "C:/Program Files/Pro Custodibus Agent/cnf",
     "/usr/local/etc/procustodibus",
     "/etc/procustodibus",
 ] + DEFAULT_WG_CNF_DIRS
 DEFAULT_LOGGING_FORMAT = "%(asctime)s %(name)s %(levelname)s: %(message)s"
 DEFAULT_LOGGING_LEVEL = "WARNING"
 
 PROCUSTODIBUS_SPLITTABLE = {
@@ -74,26 +78,59 @@
     Arguments:
         log_format (str): Log format.
         log_level (str): Log level.
     """
     logging.basicConfig(format=log_format, level=log_level, stream=sys.stdout)
 
 
+@contextmanager
+def open_ini(path, method="r"):
+    """Opens the specified ini file for reading or writing (handling DPAPI encryption).
+
+    Arguments:
+        path (str): Path to file.
+        method (str): "r" or "w" to read or write file (default "r").
+
+    Yields:
+        Stream object to read or write.
+    """
+    o = open_dpapi if str(path).endswith(".dpapi") else open
+    with o(path, method) as f:
+        yield f
+
+
+def rename_ini(old_path, new_path):
+    """Renames the specified ini file (handling DPAPI encryption).
+
+    Arguments:
+        old_path (str): Old path to file.
+        new_path (str): New path to file.
+    """
+    old_path = Path(old_path)
+    if old_path.suffix == ".dpapi":
+        with open_dpapi(old_path, "r") as r:
+            with open_dpapi(new_path, "w") as w:
+                w.write(r.read())
+        old_path.unlink()
+    else:
+        old_path.rename(new_path)
+
+
 def find_default_cnf():
     """Finds the path to an existing config file.
 
     Returns:
         str: Path to an existing config file, or blank.
     """
     path = environ.get("PROCUSTODIBUS_CONF")
     if path:
         return path
 
     for directory in DEFAULT_CNF_DIRS:
-        path = f"{directory}/procustodibus.conf"
+        path = os.path.join(directory, "procustodibus.conf")
         if os.path.exists(path):
             return path
 
     return ""
 
 
 def load_cnf(cnf_file):
@@ -127,15 +164,15 @@
         return result
 
     section = {}
     _add_ini_value(result, "preface", section)
     if not splittable:
         splittable = {}
 
-    with open(ini_file) as f:
+    with open_ini(ini_file) as f:
         for line in f:
             line = sub("#.*", "", line).strip()
             section_match = fullmatch(r"\s*\[([^\]]+)\]\s*", line)
             if section_match:
                 section_name = underscore(section_match[1])
                 section = {}
                 _add_ini_value(result, section_name, section)
@@ -204,15 +241,15 @@
     """
     if not ini_file:
         return []
 
     section = []
     result = [section]
 
-    with open(ini_file) as f:
+    with open_ini(ini_file) as f:
         for line in f:
             section_match = match(r"\s*\[([^\]]+)\]", line)
             if section_match:
                 section = _init_next_loaded_ini_section(result)
             section.append(line.rstrip("\n"))
 
     return [x for x in result if x]
@@ -284,15 +321,15 @@
     """Saves the specified ini config file from a list of lines in a list of sections.
 
     Arguments:
         ini_file (str): Path to config file.
         sections (list): List of list of lines.
         chmod (int): Optional octal mode value to set on file.
     """
-    with open(ini_file, "w") as f:
+    with open_ini(ini_file, "w") as f:
         for lines in sections:
             for line in lines:
                 # print to file
                 print(line, file=f)  # noqa: T201
 
     if chmod:
         ini_file.chmod(chmod)
```

### Comparing `procustodibus_agent-1.4.5/procustodibus_agent/connectivity.py` & `procustodibus_agent-1.5.0/procustodibus_agent/connectivity.py`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.4.5/procustodibus_agent/credentials.py` & `procustodibus_agent-1.5.0/procustodibus_agent/credentials.py`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.4.5/procustodibus_agent/executor.py` & `procustodibus_agent-1.5.0/procustodibus_agent/executor/execution.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,17 @@
 # -*- coding: utf-8 -*-
-"""Executor utilities."""
+"""Executor logic."""
 
-from logging import getLogger
-from pathlib import Path
-from re import match, search
-from subprocess import PIPE, STDOUT, CompletedProcess, run  # noqa: S404
+from subprocess import CompletedProcess  # noqa: S404
 from tempfile import NamedTemporaryFile
 
+from procustodibus_agent.executor.sys_cmd import get_sys_cmd
 from procustodibus_agent.resolve_hostname import split_endpoint_address_and_port
-from procustodibus_agent.wg_cnf import (
-    delete_wg_cnf,
-    find_wg_cnf_path,
-    rename_wg_cnf,
-    update_wg_cnf,
-)
+
+SYS_CMD = get_sys_cmd()
 
 
 def execute_desired(cnf, interfaces, data):
     """Executes desired changes from API.
 
     Arguments:
         cnf (Config): Config object.
@@ -109,16 +103,17 @@
 
     if next((x for x in results if x.returncode), None):
         output.append(f"fail {change['key']}")
     elif results:
         output.append(f"success {change['key']}")
 
     for x in results:
-        if x.stdout:
-            output.append(x.stdout)
+        stdout = x.stdout.strip() if x.stdout else ""
+        if stdout not in ("", "Ok."):
+            output.append(stdout)
 
     return "\n".join(output)
 
 
 def shut_down_interfaces(cnf, interfaces, data):
     """Shuts down interfaces for desired change objects.
 
@@ -300,43 +295,37 @@
         interfaces (dict): Interface info parsed from wg etc.
         change (dict): Desired change object.
     """
     results = change["results"]
     name = change["interface"]
     # remove to signal to other steps that the interface is down
     interface = interfaces.pop(name, {})
-    manager = interface.get("manager") or cnf.manager
 
     # start back up at end if renaming and was previously up
     if (
         interface
         and change["attributes"].get("rename")
         and change["attributes"].get("up") is not False
     ):
         change["attributes"]["up"] = True
 
-    if manager == "systemd":
-        results.append(_cmd("systemctl", "stop", f"wg-quick@{name}.service"))
-        results.append(_cmd("systemctl", "disable", f"wg-quick@{name}.service"))
-    else:
-        results.append(_cmd(cnf.wg_quick, "down", name))
+    SYS_CMD.stop_service(cnf, name, results)
 
 
 def delete_interface(cnf, interfaces, change):
     """Deletes an existing interface from a desired change object.
 
     Arguments:
         cnf (Config): Config object.
         interfaces (dict): Interface info parsed from wg etc.
         change (dict): Desired change object.
     """
     results = change["results"]
     name = change["interface"]
-    description = f"rm {find_wg_cnf_path(cnf, name)}"
-    results.append(_as_cmd(description, lambda: delete_wg_cnf(cnf, name)))
+    SYS_CMD.delete_wg_cnf(cnf, name, results)
 
 
 def delete_endpoint(cnf, interfaces, change):
     """Deletes an existing peer from a desired change object.
 
     Arguments:
         cnf (Config): Config object.
@@ -346,19 +335,19 @@
     results = change["results"]
     name = change["interface"]
     interface = interfaces.get(name)
     pk = change["attributes"].get("public_key")
     peer = interface["peers"].get(pk) if interface else None
 
     if peer:
-        results.append(_cmd(cnf.wg, "set", name, "peer", pk, "remove"))
+        SYS_CMD.set_peer(cnf, name, pk, "remove", "", results)
         _delete_endpoint_routes(interface, peer, change)
 
-    if find_wg_cnf_path(cnf, name).exists():
-        results.append(_update_wg_cnf_as_cmd(cnf, name, {}, [change["attributes"]]))
+    if SYS_CMD.check_wg_cnf(cnf, name, results) == "found":
+        SYS_CMD.update_wg_cnf(cnf, name, {}, [change["attributes"]], results)
     else:
         results.append(CompletedProcess([], 0))
 
 
 # simpler to keep this logic together rather than subdivide it more functions
 def _delete_endpoint_routes(interface, peer, change):  # noqa: CCR001
     """Deletes an existing peer from a desired change object.
@@ -375,15 +364,15 @@
     allowed_ips = peer.get("allowed_ips") or []
     default_route = _uses_default_route(allowed_ips)
 
     if table != "auto" or not default_route:
         name = change["interface"]
         results = change["results"]
         for x in allowed_ips:
-            _update_route("del", x, name, table, results)
+            SYS_CMD.update_route("del", x, name, table, results)
     else:
         change["restart"] = True
 
 
 def update_interface(cnf, interfaces, change):
     """Updates an existing interface from a desired change object.
 
@@ -398,22 +387,22 @@
     interface = interfaces.get(name)
 
     _update_interface_private_key(cnf, interface, change, name, to_set, results)
 
     port = change["attributes"].get("listen_port") or change["attributes"].get("port")
     if port is not None and port != interface.get("listen_port"):
         to_set["port"] = port
-        results.append(_cmd(cnf.wg, "set", name, "listen-port", str(port)))
+        SYS_CMD.set_interface(cnf, name, "listen-port", str(port), results)
 
     fwmark = change["attributes"].get("fwmark")
     if fwmark is not None and fwmark != interface.get("fwmark"):
         to_set["fwmark"] = fwmark
         change["restart"] = True
 
-    results.append(_update_wg_cnf_as_cmd(cnf, name, to_set))
+    SYS_CMD.update_wg_cnf(cnf, name, to_set, None, results)
 
 
 def _update_interface_private_key(cnf, interface, change, name, to_set, results):
     """Updates the private key of an existing interface from a desired change object.
 
     Arguments:
         cnf (Config): Config object.
@@ -426,17 +415,17 @@
     pk = change["attributes"].get("private_key")
     if pk is not None and pk != interface.get("private_key"):
         to_set["private_key"] = pk
         if pk:
             with NamedTemporaryFile(mode="w", buffering=1) as f:
                 f.write(pk)
                 f.write("\n")
-                results.append(_cmd(cnf.wg, "set", name, "private-key", f.name))
+                SYS_CMD.set_interface(cnf, name, "private-key", f.name, results)
         else:
-            results.append(_cmd(cnf.wg, "set", name, "private-key", "/dev/null"))
+            SYS_CMD.set_interface(cnf, name, "private-key", "/dev/null", results)
 
 
 def update_routing(cnf, interfaces, change):
     """Updates the routing info for an existing interface from a desired change object.
 
     Arguments:
         cnf (Config): Config object.
@@ -450,15 +439,15 @@
 
     _update_routing_address(cnf, interface, change, name, to_set, results)
     _update_routing_dns(cnf, interface, change, name, to_set, results)
     _update_routing_mtu(cnf, interface, change, name, to_set, results)
     _update_routing_table(cnf, interface, change, name, to_set, results)
     _update_routing_scripts(cnf, interface, change, name, to_set, results)
 
-    results.append(_update_wg_cnf_as_cmd(cnf, name, to_set))
+    SYS_CMD.update_wg_cnf(cnf, name, to_set, None, results)
 
 
 # simpler to keep this logic together rather than subdivide it more functions
 def _update_routing_address(  # noqa: CCR001
     cnf, interface, change, name, to_set, results
 ):
     """Updates the address list of an existing interface from a desired change object.
@@ -473,25 +462,19 @@
     """
     new_addresses = change["attributes"].get("address")
     old_addresses = interface.get("address") or []
     if new_addresses is not None:
         for x in old_addresses:
             if x not in new_addresses:
                 to_set["address"] = new_addresses
-                family = calculate_ip_family(x)
-                results.append(
-                    _cmd("ip", f"-{family}", "address", "del", x, "dev", name)
-                )
+                SYS_CMD.update_address("del", x, name, results)
         for x in new_addresses:
             if x not in old_addresses:
                 to_set["address"] = new_addresses
-                family = calculate_ip_family(x)
-                results.append(
-                    _cmd("ip", f"-{family}", "address", "add", x, "dev", name)
-                )
+                SYS_CMD.update_address("add", x, name, results)
 
 
 def _update_routing_dns(cnf, interface, change, name, to_set, results):
     """Updates the DNS list of an existing interface from a desired change object.
 
     Arguments:
         cnf (Config): Config object.
@@ -504,35 +487,15 @@
     dns = change["attributes"].get("dns")
     search = change["attributes"].get("search")
     if dns is None or search is None or (dns + search) == interface.get("dns"):
         return
 
     to_set["dns"] = dns
     to_set["search"] = search
-
-    resolvconf_name = f"{resolvconf_interface_prefix()}{name}"
-    results.append(_cmd("resolvconf", "-d", resolvconf_name, "-f"))
-    resolvconf_input = []
-
-    if dns:
-        resolvconf_input.append(f"nameserver {','.join(dns)}\n")
-    if search:
-        resolvconf_input.append(f"search {','.join(search)}\n")
-    if resolvconf_input:
-        results.append(
-            _cmd(
-                "resolvconf",
-                "-a",
-                resolvconf_name,
-                "-m",
-                "0",
-                "-x",
-                stdin="".join(resolvconf_input),
-            )
-        )
+    SYS_CMD.update_dns(dns, search, name, results)
 
 
 def _update_routing_mtu(cnf, interface, change, name, to_set, results):
     """Updates the MTU of an existing interface from a desired change object.
 
     Arguments:
         cnf (Config): Config object.
@@ -544,17 +507,15 @@
     """
     mtu = change["attributes"].get("mtu")
     if mtu is not None and mtu != interface.get("mtu"):
         to_set["mtu"] = mtu
         if mtu == 0:
             change["restart"] = True
         else:
-            results.append(
-                _cmd("ip", "link", "set", "mtu", str(mtu), "up", "dev", name)
-            )
+            SYS_CMD.update_mtu(mtu, name, results)
 
 
 def _update_routing_table(cnf, interface, change, name, to_set, results):
     """Updates the routing table of an existing interface from a desired change object.
 
     Arguments:
         cnf (Config): Config object.
@@ -635,21 +596,23 @@
                 results,
             )
         _update_endpoint_address(cnf, peer, change, name, pk, to_set, results)
 
         keepalive = change["attributes"].get("keepalive")
         if keepalive is not None and keepalive != peer.get("persistent_keepalive"):
             to_set["keepalive"] = keepalive
-            _wg_set_peer(cnf, name, pk, "persistent-keepalive", str(keepalive), results)
+            SYS_CMD.set_peer(
+                cnf, name, pk, "persistent-keepalive", str(keepalive), results
+            )
 
     else:
         to_set = change["attributes"]
         change["restart"] = True
 
-    results.append(_update_wg_cnf_as_cmd(cnf, name, {}, [to_set]))
+    SYS_CMD.update_wg_cnf(cnf, name, {}, [to_set], results)
 
 
 def _uses_default_route(ips):
     """True if the specified AllowedIPs list should override the default route.
 
     Arguments:
         ips (list): AllowedIPs list (eg ['0.0.0.0/0, ::/0']).
@@ -682,18 +645,18 @@
     shared = change["attributes"].get("preshared_key")
     if shared is not None and shared != peer.get("preshared_key"):
         if shared and shared != "off":
             to_set["preshared_key"] = shared
             with NamedTemporaryFile(mode="w", buffering=1) as f:
                 f.write(shared)
                 f.write("\n")
-                _wg_set_peer(cnf, name, pk, "preshared-key", f.name, results)
+                SYS_CMD.set_peer(cnf, name, pk, "preshared-key", f.name, results)
         else:
             to_set["preshared_key"] = ""
-            _wg_set_peer(cnf, name, pk, "preshared-key", "/dev/null", results)
+            SYS_CMD.set_peer(cnf, name, pk, "preshared-key", "/dev/null", results)
 
 
 # simpler to keep this logic together rather than subdivide it more functions
 def _update_endpoint_allowed_ips(  # noqa: CCR001, CFQ002
     cnf,
     old_allowed_ips,
     new_allowed_ips,
@@ -714,44 +677,25 @@
         pk (str): Peer public key (eg 'ABC...123=').
         old_table (str): Old route table name (eg 'auto').
         new_table (str): New route table name (eg 'off').
         to_set (dict): Dict of peer properties to set (to add to).
         results (list): List of completed proccess objects (to add to).
     """
     to_set["allowed_ips"] = new_allowed_ips
-    _wg_set_peer(cnf, name, pk, "allowed-ips", ",".join(new_allowed_ips), results)
+    SYS_CMD.set_peer(cnf, name, pk, "allowed-ips", ",".join(new_allowed_ips), results)
 
     if old_table != "off":
         for x in old_allowed_ips:
             if x not in new_allowed_ips:
-                _update_route("del", x, name, old_table, results)
+                SYS_CMD.update_route("del", x, name, old_table, results)
 
     if new_table != "off":
         for x in new_allowed_ips:
             if x not in old_allowed_ips:
-                _update_route("add", x, name, new_table, results)
-
-
-def _update_route(action, to, dev, table, results):
-    """Adds or removes the specified route.
-
-    Arguments:
-        action (str): "add" or "del".
-        to (str): IP address or CIDR (eg '10.0.0.0/24').
-        dev (str): Interface name (eg 'wg0').
-        table (str): Route table name (eg 'auto').
-        results (list): List of completed proccess objects (to add to).
-    """
-    family = calculate_ip_family(to)
-
-    args = ["ip", f"-{family}", "route", action, to, "dev", dev]
-    if table != "auto":
-        args += ["table", table]
-
-    results.append(_cmd(*args))
+                SYS_CMD.update_route("add", x, name, new_table, results)
 
 
 # simpler to keep this logic together rather than subdivide it more functions
 def _update_endpoint_address(  # noqa: CCR001, CFQ002
     cnf, peer, change, name, pk, to_set, results
 ):
     """Updates the endpoint address an existing peer from a desired change object.
@@ -776,44 +720,30 @@
         old_endpoint = (
             f"{old_hostname}:{old_port}" if old_port != 51820 else old_hostname
         )
 
     if endpoint != old_endpoint:
         to_set["endpoint"] = endpoint
         if endpoint:
-            _wg_set_peer(cnf, name, pk, "endpoint", endpoint, results)
-
-
-def _wg_set_peer(cnf, name, pk, setting, value, results):
-    """Sets the specified wg setting for the specified peer.
-
-    Arguments:
-        cnf (Config): Config object.
-        name (str): Interface name (eg 'wg0').
-        pk (str): Peer public key.
-        setting (str): Setting name (eg 'allowed-ips').
-        value (str): Setting value (eg '10.0.0.1/24,fc00:0:0:1::/64').
-        results (list): List to append the results of the command to.
-    """
-    results.append(_cmd(cnf.wg, "set", name, "peer", pk, setting, value))
+            SYS_CMD.set_peer(cnf, name, pk, "endpoint", endpoint, results)
 
 
 def create_interface(cnf, interfaces, change):
     """Sets up a new interface from a desired change object.
 
     Arguments:
         cnf (Config): Config object.
         interfaces (dict): Interface info parsed from wg etc.
         change (dict): Desired change object.
     """
     change["restart"] = True
     results = change["results"]
     name = change["interface"]
     to_set = change["attributes"]
-    results.append(_update_wg_cnf_as_cmd(cnf, name, to_set))
+    SYS_CMD.create_wg_cnf(cnf, name, to_set, None, results)
 
 
 def create_routing(cnf, interfaces, change):
     """Sets up the routing info for a new interface from a desired change object.
 
     Arguments:
         cnf (Config): Config object.
@@ -831,41 +761,35 @@
         interfaces (dict): Interface info parsed from wg etc.
         change (dict): Desired change object.
     """
     change["restart"] = True
     results = change["results"]
     name = change["interface"]
     to_set = change["attributes"]
-    results.append(_update_wg_cnf_as_cmd(cnf, name, {}, [to_set]))
+    SYS_CMD.update_wg_cnf(cnf, name, {}, [to_set], results)
 
 
 def rename_interface(cnf, interfaces, change):
     """Renames an existing interface from a desired change object.
 
     Arguments:
         cnf (Config): Config object.
         interfaces (dict): Interface info parsed from wg etc.
         change (dict): Desired change object.
     """
     results = change["results"]
     old_name = change["interface"]
-    old_path = find_wg_cnf_path(cnf, old_name)
     new_name = change["attributes"].get("rename")
 
     if not new_name or new_name == old_name:
         update_interface(cnf, interfaces, change)
-    elif old_path.exists():
+    elif SYS_CMD.check_wg_cnf(cnf, old_name, results) == "found":
         change["interface"] = new_name
         change["restart"] = True
-        results.append(
-            _as_cmd(
-                f"mv {old_path} {find_wg_cnf_path(cnf, new_name)}",
-                lambda: rename_wg_cnf(cnf, old_name, new_name),
-            )
-        )
+        SYS_CMD.rename_wg_cnf(cnf, old_name, new_name, results)
     else:
         change["interface"] = new_name
         create_interface(cnf, interfaces, change)
 
 
 def start_up_interface(cnf, interfaces, name, changes):
     """Starts up a new or existing interface for a list of desired changes.
@@ -873,27 +797,15 @@
     Arguments:
         cnf (Config): Config object.
         interfaces (dict): Interface info parsed from wg etc.
         name (str): Interface name to start up (eg `wg0`).
         changes (list): List of desired change objects.
     """
     results = []
-    interface = interfaces.get(name) or {}
-    manager = interface.get("manager") or cnf.manager
-
-    if manager == "systemd":
-        # stop first, and ignore shutdown output/errors
-        _cmd("systemctl", "stop", f"wg-quick@{name}.service")
-        results.append(_cmd("systemctl", "start", f"wg-quick@{name}.service"))
-        results.append(_cmd("systemctl", "enable", f"wg-quick@{name}.service"))
-    else:
-        # stop first, and ignore shutdown output/errors
-        _cmd(cnf.wg_quick, "down", name)
-        results.append(_cmd(cnf.wg_quick, "up", name))
-
+    SYS_CMD.start_service(cnf, name, results)
     for x in changes:
         x["results"].extend(results)
 
 
 def update_down_script(cnf, interfaces, change):
     """Updates the routing info for an existing interface from a desired change object.
 
@@ -908,89 +820,15 @@
     interface = interfaces.get(name)
 
     for key in ["pre_down", "post_down"]:
         value = change["attributes"].get(key)
         if value is not None and value != interface.get(key):
             to_set[key] = value
 
-    results.append(_update_wg_cnf_as_cmd(cnf, name, to_set))
-
-
-def _cmd(*args, stdin=None):
-    """Executes a command with the specified arguments.
-
-    Arguments:
-        *args (list): Command arguments.
-        stdin (str): Optional command input.
-
-    Returns:
-        Completed process object.
-    """
-    try:
-        if stdin:
-            completed = run(  # noqa: S603 S607
-                args,
-                input=stdin,
-                stdout=PIPE,
-                stderr=STDOUT,
-                timeout=30,
-                universal_newlines=True,
-            )
-        else:
-            completed = run(  # noqa: S603 S607
-                args, stdout=PIPE, stderr=STDOUT, timeout=30, universal_newlines=True
-            )
-    except Exception as e:
-        completed = CompletedProcess([], 1, stdout=str(e))
-
-    output = " ".join(args)
-    if completed.stdout:
-        output = f"{output}\n{completed.stdout}"
-
-    if completed.returncode:
-        getLogger(__name__).warning("err # %s", output)
-    else:
-        getLogger(__name__).info("ok  # %s", output)
-
-    return completed
-
-
-def _as_cmd(description, function):
-    """Runs the specified function and returns a CompletedProcess object as the result.
-
-    Arguments:
-        description (str): Command description (eg 'update config file').
-        function (lambda): Zero-argument function to run.
-
-    Returns:
-        Completed process object.
-    """
-    try:
-        function()
-        getLogger(__name__).info("ok  # %s", description)
-        return CompletedProcess([], 0)
-    except Exception as e:
-        getLogger(__name__).warning("err # %s", description, exc_info=True)
-        return CompletedProcess([], 1, stdout=str(e))
-
-
-def _update_wg_cnf_as_cmd(cnf, name, interface, peers=None):
-    """Updates the cnf file for the specified interface with the specified properties.
-
-    Arguments:
-        cnf (Config): Config object.
-        name (str): Name of interface to update (eg 'wg0').
-        interface (dict): Properties of interface to update.
-        peers (list): List of dicts with peer properties to update.
-
-    Returns:
-        Completed process object.
-    """
-    description = f"procustodibus_agent setconf {name} {find_wg_cnf_path(cnf, name)}"
-    return _as_cmd(description, lambda: update_wg_cnf(cnf, name, interface, peers))
+    SYS_CMD.update_wg_cnf(cnf, name, to_set, None, results)
 
 
 def _is_shut_down_interface(interfaces, change):
     """Checks if the specified change object should shut down an interface.
 
     Arguments:
         interfaces (dict): Interface info parsed from wg etc.
@@ -1179,38 +1017,7 @@
         interfaces (dict): Interface info parsed from wg etc.
         change (dict): Desired change object.
 
     Returns:
         boolean: True if should update the down scripts.
     """
     return change["type"] == "desired_routings" and interfaces.get(change["interface"])
-
-
-def calculate_ip_family(address):
-    """Determines whether the specified IP address is IPv4 or IPv6.
-
-    Arguments:
-        address (str): IP address (eg 'fc00:0:0:1::').
-
-    Returns:
-        int: 4 or 6.
-    """
-    return 6 if search(r":.*:", address) else 4
-
-
-def resolvconf_interface_prefix(file="/etc/resolvconf/interface-order"):
-    """Returns the prefix to append to an interface name for resolvconf commands.
-
-    Arguments:
-        file (str): Resolvconf interface-order file path to check.
-
-    Returns:
-        str: Prefix (eg 'tun') or blank ('').
-    """
-    path = Path(file)
-    if path.exists():
-        with open(path) as f:
-            for line in f:
-                interface_match = match(r"([A-Za-z0-9-]+)\*", line)
-                if interface_match:
-                    return interface_match[1]
-    return ""
```

### Comparing `procustodibus_agent-1.4.5/procustodibus_agent/ip_route.py` & `procustodibus_agent-1.5.0/procustodibus_agent/ip_route.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 """Routing and addressing utilities."""
 
 from ipaddress import IPv4Address, IPv4Interface
+from itertools import zip_longest
 from json import loads
 from platform import system
-from re import fullmatch, sub
+from re import fullmatch, match, sub
 from subprocess import PIPE, run  # noqa: S404
 
 
 def run_ip_address_show(device):
     """Runs `ip address show` command for specified device.
 
     Arguments:
@@ -19,14 +20,44 @@
     """
     args = ["ip", "--json", "address", "show", "dev", device]
     result = run(args, stdout=PIPE)  # noqa: S603 S607
     output = result.stdout.decode("utf-8")
     return loads(output)[0] if fullmatch(r"\[\{.*\}\]\s*", output) else {}
 
 
+def run_netsh_show_addresses(device):
+    """Runs `netsh` command for specified device.
+
+    Arguments:
+        device (str): Device name (eg 'wg0').
+
+    Returns:
+        list: Lines from `netsh` command.
+    """
+    ipv4 = _run_netsh_show_addresses_for_family(device, "ipv4")
+    ipv6 = _run_netsh_show_addresses_for_family(device, "ipv6")
+    return ipv4 + ipv6
+
+
+def _run_netsh_show_addresses_for_family(device, family):
+    """Runs `netsh` command for specified device and IP version.
+
+    Arguments:
+        device (str): Device name (eg 'wg0').
+        family (str): IP family ('ipv4' or 'ipv6')
+
+    Returns:
+        list: Lines from `netsh` command.
+    """
+    args = ["netsh", "interface", family, "show", "addresses", device]
+    result = run(args, stdout=PIPE)  # noqa: S603 S607
+    output = result.stdout.decode("utf-8")
+    return [x.strip() for x in output.split("\n")]
+
+
 def run_ifconfig(device):
     """Runs `ifconfig` command for specified device.
 
     Arguments:
         device (str): Device name (eg 'wg0').
 
     Returns:
@@ -60,14 +91,16 @@
         properties (dict): Dict of interface properties.
 
     Returns:
         dict: Same dict with additional properties.
     """
     if system() == "Linux":
         _annotate_interface_with_ip_address_show(name, properties)
+    elif system() == "Windows":
+        _annotate_interface_with_netsh_show_addresses(name, properties)
     else:
         _annotate_interface_with_ifconfig(name, properties)
     return properties
 
 
 def _annotate_interface_with_ip_address_show(name, properties):
     """Annotates specified dict with wg config for specified interface.
@@ -93,14 +126,61 @@
 
     Returns:
         string: CIDR.
     """
     return "{}/{}".format(info["local"], info["prefixlen"])
 
 
+def _annotate_interface_with_netsh_show_addresses(name, properties):
+    """Annotates specified dict with wg config for specified interface.
+
+    Arguments:
+        name (str): Interface name (eg 'wg0').
+        properties (dict): Dict of interface properties.
+
+    Returns:
+        dict: Same dict with additional properties.
+    """
+    output = run_netsh_show_addresses(name)
+    addresses = list(filter(None, [_parse_netsh_address(x) for x in output]))
+
+    if addresses:
+        prefixes = list(filter(None, [_parse_netsh_prefix_length(x) for x in output]))
+        combined = [f"{a}/{p}" if p else a for a, p in zip_longest(addresses, prefixes)]
+        properties["address"] = combined
+
+    return properties
+
+
+def _parse_netsh_address(line):
+    """Parses the ip address out of the specified netsh output line.
+
+    Arguments:
+        line (str): netsh output line (eg 'IP Address:    10.0.0.1').
+
+    Returns:
+        str: Address or empty string (eg '10.0.0.1').
+    """
+    m = match(r"(?:IP )?Address:?\s+([\da-f.:%]+)", line)
+    return m.group(1) if m else ""
+
+
+def _parse_netsh_prefix_length(line):
+    """Parses the subnet prefix length out of the specified netsh output line.
+
+    Arguments:
+        line (str): netsh output line (eg 'Subnet Prefix:    10.0.0.0/24').
+
+    Returns:
+        int: Prefix or None (eg 0).
+    """
+    m = match(r"Subnet Prefix:\s+[\da-f.:%]+/(\d+).*", line)
+    return int(m.group(1)) if m else None
+
+
 def _annotate_interface_with_ifconfig(name, properties):
     """Annotates specified dict with wg config for specified interface.
 
     Arguments:
         name (str): Interface name (eg 'wg0').
         properties (dict): Dict of interface properties.
```

### Comparing `procustodibus_agent-1.4.5/procustodibus_agent/mfa/__init__.py` & `procustodibus_agent-1.5.0/procustodibus_agent/mfa/__init__.py`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.4.5/procustodibus_agent/mfa/api.py` & `procustodibus_agent-1.5.0/procustodibus_agent/mfa/api.py`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.4.5/procustodibus_agent/mfa/cli.py` & `procustodibus_agent-1.5.0/procustodibus_agent/mfa/cli.py`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.4.5/procustodibus_agent/resolve_hostname.py` & `procustodibus_agent-1.5.0/procustodibus_agent/resolve_hostname.py`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.4.5/procustodibus_agent/wg.py` & `procustodibus_agent-1.5.0/procustodibus_agent/wg.py`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.4.5/procustodibus_agent/wg_cnf.py` & `procustodibus_agent-1.5.0/procustodibus_agent/wg_cnf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # -*- coding: utf-8 -*-
 """Utilities for manipulating wq conf ini."""
 
 from contextlib import suppress
 from pathlib import Path
+from platform import system
 from re import match, sub
 
 from inflection import underscore
 
 from procustodibus_agent import __version__ as version
 from procustodibus_agent.api import format_datetime
 from procustodibus_agent.cnf import (
     WIREGUARD_SPLITTABLE,
     find_ini_section_with_line,
     load_ini,
     load_ini_lines,
+    rename_ini,
     replace_ini_line_value,
     save_ini_lines,
 )
 
 
 def annotate_wg_show_with_wg_cnf(cnf, interfaces):
     """Annotates parsed output of `wg show` with wg config.
@@ -41,15 +43,16 @@
         cnf (Config): Config object.
         name (str): Interface name (eg 'wg0').
 
     Returns:
         Path: Path to ini file (eg '/etc/wireguard/wg0.conf').
     """
     directory = cnf.wg_cnf_dir or "/etc/wireguard"
-    return Path(directory, f"{name}.conf")
+    file_name = f"{name}.conf.dpapi" if system() == "Windows" else f"{name}.conf"
+    return Path(directory, file_name)
 
 
 def _annotate_interface(cnf, name, properties):
     """Annotates specified dict with wg config for specified interface.
 
     Arguments:
         cnf (Config): Config object.
@@ -167,17 +170,18 @@
     """Renames the cnf file for the specified interface to the specified new name.
 
     Arguments:
         cnf (Config): Config object.
         old_name (str): Existing name (eg 'wg0').
         new_name (str): New name (eg 'wg100').
     """
-    path = find_wg_cnf_path(cnf, old_name)
-    if path.exists():
-        path.rename(find_wg_cnf_path(cnf, new_name))
+    if old_name and new_name and old_name != new_name:
+        path = find_wg_cnf_path(cnf, old_name)
+        if path.exists():
+            rename_ini(path, find_wg_cnf_path(cnf, new_name))
 
 
 def update_wg_cnf(cnf, name, interface, peers=None):
     """Updates the cnf file for the specified interface with the specified properties.
 
     Arguments:
         cnf (Config): Config object.
```

### Comparing `procustodibus_agent-1.4.5/procustodibus_agent.egg-info/PKG-INFO` & `procustodibus_agent-1.5.0/procustodibus_agent.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: procustodibus_agent
-Version: 1.4.5
+Version: 1.5.0
 Summary: Synchronizes your WireGuard settings with Pro Custodibus.
 Home-page: https://www.procustodibus.com/
 Author: Arcem Tene
 Author-email: dev@arcemtene.com
 License: MIT
 Project-URL: Changelog, https://docs.procustodibus.com/guide/agents/download/#changelog
 Project-URL: Documentation, https://docs.procustodibus.com/guide/agents/run/
@@ -22,14 +22,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: docopt-ng~=0.7
 Requires-Dist: inflection~=0.5
 Requires-Dist: pynacl~=1.5
+Requires-Dist: pywin32~=306.0; sys_platform == "win32"
 Requires-Dist: requests~=2.27
 Requires-Dist: tabulate~=0.8
 Provides-Extra: lint
 Requires-Dist: cohesion; extra == "lint"
 Requires-Dist: darglint; extra == "lint"
 Requires-Dist: dlint; extra == "lint"
 Requires-Dist: flake8; extra == "lint"
@@ -73,25 +74,25 @@
 
 [Pro Custodibus](https://www.procustodibus.com/) is a service that makes [WireGuard](https://www.wireguard.com/) networks easy to deploy and manage. You run the Pro Custodibus agent on each WireGuard host you want to manage, and the agent monitors and synchronizes the hosts' WireGuard settings with the remote Pro Custodibus service.
 
 
 Installing
 ----------
 
-Requires python 3.7 or newer and libsodium. Installer script can install requirements, plus the agent itself, on most linuxes. Install from source like the following:
+Requires python 3.7 or newer and libsodium. Installer script can install requirements, plus the agent itself, on most linuxes, FreeBSD, OpenBSD, and macOS (if macOS has [Homebrew](https://brew.sh/)). Install from source like the following:
 ```
 ./install.sh --install
 ```
 
 Or run it like the following to see more options:
 ```
 ./install.sh --help
 ```
 
-See the [Installer Documentation](https://docs.procustodibus.com/guide/agents/install/) for full details.
+See the [Installer Documentation](https://docs.procustodibus.com/guide/agents/install/) for full details (or to download the pre-built Windows installer).
 
 
 Docker
 ------
 
 The [docker/wireguard.dockerfile](https://git.sr.ht/~arx10/procustodibus-agent/tree/main/item/docker/wireguard.dockerfile) is built weekly and pushed to the [docker.io/procustodibus/wireguard](https://hub.docker.com/r/procustodibus/wireguard) repository. It produces a base WireGuard image without the agent.
 
@@ -169,14 +170,47 @@
 ```
 
 Manually run pre-push hook on all version-controlled files:
 ```
 tox -e pre-commit -- run -a --hook-stage push
 ```
 
+### Build Windows installer
+
+1. Install [Python](https://www.python.org/downloads/).
+
+2. Install [Inno Setup](https://jrsoftware.org/isdl.php).
+
+3. Create a virtualenv:
+    ```
+    python -m venv C:\venvs\procustodibus-agent
+    ```
+
+4. Activate the virtualenv:
+    ```
+    C:\venvs\procustodibus-agent\Scripts\activate.bat
+    ```
+
+5. Install tox:
+    ```
+    pip install tox
+    ```
+
+6. Build the Windows executables with cx_freeze:
+    ```
+    tox -e build_exe
+    ```
+
+7. Build the Windows installer with Inno Setup:
+    ```
+    "C:\Program Files (x86)\Inno Setup 6\ISCC.exe" installer\windows.iss
+    ```
+
+The installer will be built as `dist\ProCustodibusAgentInstaller.exe`.
+
 
 Contributing
 ------------
 
 * [Code of Conduct](https://docs.procustodibus.com/community/conduct/)
 * [File a Bug](https://docs.procustodibus.com/guide/community/bugs/)
 * [Report a Vulnerability](https://docs.procustodibus.com/guide/community/vulns/)
```

### Comparing `procustodibus_agent-1.4.5/procustodibus_agent.egg-info/SOURCES.txt` & `procustodibus_agent-1.5.0/procustodibus_agent.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -7,26 +7,31 @@
 procustodibus_agent/__init__.py
 procustodibus_agent/agent.py
 procustodibus_agent/api.py
 procustodibus_agent/cli.py
 procustodibus_agent/cnf.py
 procustodibus_agent/connectivity.py
 procustodibus_agent/credentials.py
-procustodibus_agent/executor.py
 procustodibus_agent/ip_route.py
 procustodibus_agent/resolve_hostname.py
 procustodibus_agent/wg.py
 procustodibus_agent/wg_cnf.py
 procustodibus_agent.egg-info/PKG-INFO
 procustodibus_agent.egg-info/SOURCES.txt
 procustodibus_agent.egg-info/dependency_links.txt
 procustodibus_agent.egg-info/entry_points.txt
 procustodibus_agent.egg-info/requires.txt
 procustodibus_agent.egg-info/top_level.txt
 procustodibus_agent.egg-info/zip-safe
+procustodibus_agent/executor/__init__.py
+procustodibus_agent/executor/execution.py
+procustodibus_agent/executor/sys_cmd.py
 procustodibus_agent/mfa/__init__.py
 procustodibus_agent/mfa/api.py
 procustodibus_agent/mfa/cli.py
+procustodibus_agent/windows/cnf.py
+procustodibus_agent/windows/service.py
+procustodibus_agent/windows/service_config.py
 requirements/dev.txt
 requirements/lint.txt
 requirements/prod.txt
 requirements/test.txt
```

### Comparing `procustodibus_agent-1.4.5/procustodibus_agent.egg-info/requires.txt` & `procustodibus_agent-1.5.0/procustodibus_agent.egg-info/requires.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 docopt-ng~=0.7
 inflection~=0.5
 pynacl~=1.5
 requests~=2.27
 tabulate~=0.8
 
+[:sys_platform == "win32"]
+pywin32~=306.0
+
 [lint]
 cohesion
 darglint
 dlint
 flake8
 flake8-alfred
 flake8-bandit
```

### Comparing `procustodibus_agent-1.4.5/requirements/lint.txt` & `procustodibus_agent-1.5.0/requirements/lint.txt`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.4.5/setup.cfg` & `procustodibus_agent-1.5.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -12,14 +12,14 @@
 	conftest.py: I900, W0621
 	test_*: D103, D105, D107, I900, S101, W0613
 	install_*: D103, D105, D107, I900, S101, W0613
 use-class-attributes-order-strict-mode = True
 docstring-convention = google
 max-returns-amount = 9
 pytest-parametrize-names-type = csv
-known-modules = docopt-ng:[docopt],pynacl:[nacl.encoding,nacl.signing]
+known-modules = docopt-ng:[docopt],pynacl:[nacl.encoding,nacl.signing],pywin32:[win32crypt,win32security]
 requirements-max-depth = 5
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `procustodibus_agent-1.4.5/setup.py` & `procustodibus_agent-1.5.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -42,15 +42,17 @@
         "Programming Language :: Python :: 3.12",
     ],
     license="MIT",
     author="Arcem Tene",
     author_email="dev@arcemtene.com",
     packages=[
         "procustodibus_agent",
+        "procustodibus_agent.executor",
         "procustodibus_agent.mfa",
+        "procustodibus_agent.windows",
     ],
     entry_points={
         "console_scripts": [
             "procustodibus-agent = procustodibus_agent.cli:main",
             "procustodibus-credentials = procustodibus_agent.credentials:main",
             "procustodibus-mfa = procustodibus_agent.mfa.cli:main",
         ],
```

