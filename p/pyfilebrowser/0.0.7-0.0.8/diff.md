# Comparing `tmp/pyfilebrowser-0.0.7-py3-none-any.whl.zip` & `tmp/pyfilebrowser-0.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 16892 bytes, number of entries: 14
--rw-r--r--  2.0 unx      105 b- defN 24-Mar-26 02:56 pyfilebrowser/__init__.py
--rw-r--r--  2.0 unx     7279 b- defN 24-Mar-26 02:56 pyfilebrowser/main.py
--rw-r--r--  2.0 unx       72 b- defN 24-Mar-26 02:56 pyfilebrowser/requirements.txt
--rw-r--r--  2.0 unx     5473 b- defN 24-Mar-26 02:56 pyfilebrowser/modals/config.py
--rw-r--r--  2.0 unx     1765 b- defN 24-Mar-26 02:56 pyfilebrowser/modals/models.py
--rw-r--r--  2.0 unx     1603 b- defN 24-Mar-26 02:56 pyfilebrowser/modals/users.py
--rw-r--r--  2.0 unx     9719 b- defN 24-Mar-26 02:56 pyfilebrowser/squire/download.py
--rw-r--r--  2.0 unx     4077 b- defN 24-Mar-26 02:56 pyfilebrowser/squire/steward.py
--rw-r--r--  2.0 unx     4418 b- defN 24-Mar-26 02:56 pyfilebrowser/squire/subtitles.py
--rw-r--r--  2.0 unx     1068 b- defN 24-Mar-26 02:56 pyfilebrowser-0.0.7.dist-info/LICENSE
--rw-r--r--  2.0 unx     8321 b- defN 24-Mar-26 02:56 pyfilebrowser-0.0.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-26 02:56 pyfilebrowser-0.0.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 24-Mar-26 02:56 pyfilebrowser-0.0.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1187 b- defN 24-Mar-26 02:56 pyfilebrowser-0.0.7.dist-info/RECORD
-14 files, 45193 bytes uncompressed, 14906 bytes compressed:  67.0%
+Zip file size: 17046 bytes, number of entries: 14
+-rw-r--r--  2.0 unx      105 b- defN 24-Apr-05 10:09 pyfilebrowser/__init__.py
+-rw-r--r--  2.0 unx     8736 b- defN 24-Apr-05 10:09 pyfilebrowser/main.py
+-rw-r--r--  2.0 unx       89 b- defN 24-Apr-05 10:09 pyfilebrowser/requirements.txt
+-rw-r--r--  2.0 unx     5452 b- defN 24-Apr-05 10:09 pyfilebrowser/modals/config.py
+-rw-r--r--  2.0 unx     1765 b- defN 24-Apr-05 10:09 pyfilebrowser/modals/models.py
+-rw-r--r--  2.0 unx     1603 b- defN 24-Apr-05 10:09 pyfilebrowser/modals/users.py
+-rw-r--r--  2.0 unx    10178 b- defN 24-Apr-05 10:09 pyfilebrowser/squire/download.py
+-rw-r--r--  2.0 unx     4525 b- defN 24-Apr-05 10:09 pyfilebrowser/squire/steward.py
+-rw-r--r--  2.0 unx     3056 b- defN 24-Apr-05 10:09 pyfilebrowser/squire/struct.py
+-rw-r--r--  2.0 unx     1068 b- defN 24-Apr-05 10:09 pyfilebrowser-0.0.8.dist-info/LICENSE
+-rw-r--r--  2.0 unx     8354 b- defN 24-Apr-05 10:09 pyfilebrowser-0.0.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-05 10:09 pyfilebrowser-0.0.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 24-Apr-05 10:09 pyfilebrowser-0.0.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1185 b- defN 24-Apr-05 10:09 pyfilebrowser-0.0.8.dist-info/RECORD
+14 files, 46222 bytes uncompressed, 15066 bytes compressed:  67.4%
```

## zipnote {}

```diff
@@ -18,26 +18,26 @@
 
 Filename: pyfilebrowser/squire/download.py
 Comment: 
 
 Filename: pyfilebrowser/squire/steward.py
 Comment: 
 
-Filename: pyfilebrowser/squire/subtitles.py
+Filename: pyfilebrowser/squire/struct.py
 Comment: 
 
-Filename: pyfilebrowser-0.0.7.dist-info/LICENSE
+Filename: pyfilebrowser-0.0.8.dist-info/LICENSE
 Comment: 
 
-Filename: pyfilebrowser-0.0.7.dist-info/METADATA
+Filename: pyfilebrowser-0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: pyfilebrowser-0.0.7.dist-info/WHEEL
+Filename: pyfilebrowser-0.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: pyfilebrowser-0.0.7.dist-info/top_level.txt
+Filename: pyfilebrowser-0.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: pyfilebrowser-0.0.7.dist-info/RECORD
+Filename: pyfilebrowser-0.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyfilebrowser/__init__.py

```diff
@@ -1,5 +1,5 @@
 """Module for packaging."""
 
 from pyfilebrowser.main import FileBrowser  # noqa: F401
 
-version = "0.0.7"
+version = "0.0.8"
```

## pyfilebrowser/main.py

```diff
@@ -1,18 +1,19 @@
 import json
+import logging
+import multiprocessing
 import os
 import subprocess
+import time
 import warnings
-from multiprocessing.context import \
-    TimeoutError as ThreadTimeoutError  # noqa: PyProtectedMember
-from multiprocessing.pool import ThreadPool
-from typing import List
+from typing import Dict, List
 
 from pyfilebrowser.modals import models
-from pyfilebrowser.squire import download, steward, subtitles
+from pyfilebrowser.proxy import proxy_server, proxy_settings
+from pyfilebrowser.squire import download, steward, struct
 
 
 class FileBrowser:
     """Object to handle the filebrowser streaming.
 
     >>> FileBrowser
 
@@ -21,42 +22,44 @@
     def __init__(self, **kwargs):
         """Instantiates the object.
 
         Keyword Args:
             logger: Bring your own logger.
         """
         self.env = steward.EnvConfig(**kwargs)
-        if self.env.config_settings.server.log == models.Log.file:
-            # Reset to stdout, so the log output stream can be controlled with custom logging
-            self.env.config_settings.server.log = models.Log.stdout
-            self.logger = kwargs.get('logger', steward.default_logger(True))
-        else:
-            self.logger = kwargs.get('logger', steward.default_logger(False))
+        # Reset to stdout, so the log output stream can be controlled with custom logging
+        self.env.config_settings.server.log = models.Log.stdout
+        self.logger = kwargs.get('logger',
+                                 steward.default_logger(self.env.config_settings.server.log == models.Log.file))
         github = download.GitHub(**kwargs)
         if not os.path.isfile(download.executable.filebrowser_bin):
             download.binary(logger=self.logger, github=github)
-        self.converted = None
+        self.proxy_engine: multiprocessing.Process | None = None
 
-    def exit_process(self):
+    def exit_process(self) -> None:
         """Deletes the database file, and all the subtitles that were created by this application."""
         if os.path.isfile(download.executable.filebrowser_db):
-            self.logger.info(f"Removing database {download.executable.filebrowser_db}")
+            self.logger.info("Removing database %s", download.executable.filebrowser_db)
             os.remove(download.executable.filebrowser_db)
-        if self.converted:
-            try:
-                files_removed = []
-                for file in self.converted.get(timeout=5):
-                    try:
-                        os.remove(file)
-                        files_removed.append(file.name)
-                    except FileNotFoundError:
-                        continue
-                self.logger.info(f"Subtitles removed automatically [{len(files_removed)}]: {', '.join(files_removed)}")
-            except ThreadTimeoutError as error:
-                self.logger.error(error)
+        if self.proxy_engine:
+            self.logger.info("Stopping proxy service")
+            self.proxy_engine.terminate()
+            for i in range(5):
+                if self.proxy_engine.is_alive():
+                    self.proxy_engine.kill()
+                else:
+                    self.logger.info("Daemon process terminated in %s attempt", steward.ordinal(i))
+                    self.proxy_engine.close()
+                    break
+                time.sleep(1e-1)  # 0.1s
+            else:
+                warnings.warn(
+                    f"Failed to terminate daemon process PID: [{self.proxy_engine.pid}] within 5 attempts",
+                    RuntimeWarning
+                )
 
     def run_subprocess(self, arguments: List[str] = None, failed_msg: str = None, stdout: bool = False) -> None:
         """Run ``filebrowser`` commands as subprocess.
 
         Args:
             arguments: Arguments to pass to the binary.
             failed_msg: Failure message in case of bad return code.
@@ -72,78 +75,120 @@
                 for line in process.stdout:
                     self.logger.info(steward.remove_prefix(line))
             process.wait()
             for line in process.stderr:
                 self.logger.warning(steward.remove_prefix(line))
             assert process.returncode == 0, failed_msg
         except KeyboardInterrupt:
-            self.logger.warning("Interrupted manually")
             if process.poll() is None:
                 for line in process.stdout:
                     self.logger.info(steward.remove_prefix(line))
                 process.terminate()
             self.exit_process()
 
-    def create_users(self) -> None:
-        """Creates the JSON file for user profiles."""
+    def create_users(self) -> Dict[str, str]:
+        """Creates the JSON file for user profiles.
+
+        Returns:
+            Dict[str, str]:
+            Authentication map provided as environment variables.
+        """
         final_settings = []
         user_profiles = self.env.user_profiles or self.env.load_user_profiles()
+        auth_map = {}
         for idx, profile in enumerate(user_profiles):
             if profile.authentication.admin:
                 profile.perm = models.admin_perm()
             else:
                 profile.perm = models.default_perm()
+            auth_map[profile.authentication.username] = profile.authentication.password
             hashed_password = steward.hash_password(profile.authentication.password)
             assert steward.validate_password(profile.authentication.password, hashed_password), "Validation failed!"
             profile.authentication.password = hashed_password
             model_settings = json.loads(profile.model_dump_json())
             user_settings = {'id': idx + 1}
             model_settings['authentication'].pop('admin', None)  # remove custom 'admin' model within authentication
             user_settings.update(model_settings['authentication'])  # insert custom 'authentication' model into new dict
             model_settings.pop('authentication', None)  # remove custom 'authentication' model from 'model_settings'
             user_settings.update(model_settings)  # insert cleaned 'model_settings' into new dict 'user_settings'
             final_settings.append(user_settings)
         with open(steward.fileio.users, 'w') as file:
             json.dump(final_settings, file, indent=4)
             file.flush()
+        return auth_map
 
-    def create_config(self) -> None:
-        """Creates the JSON file for configuration."""
-        config_settings = self.env.config_settings
-        if str(config_settings.settings.branding.files) == ".":
-            config_settings.settings.branding.files = ""
-        config_settings.server.port = str(config_settings.server.port)
+    def create_config(self, proxy: bool) -> None:
+        """Creates the JSON file for configuration.
+
+        Args:
+            proxy: Boolean flag to enable proxy.
+        """
+        if proxy:
+            self.env.config_settings.settings.authMethod = "json"
+            self.env.config_settings.settings.authHeader = ""
+        if str(self.env.config_settings.settings.branding.files) == ".":
+            self.env.config_settings.settings.branding.files = ""
+        self.env.config_settings.server.port = str(self.env.config_settings.server.port)
         with warnings.catch_warnings(action="ignore"):
-            final_settings = steward.remove_trailing_underscore(json.loads(config_settings.model_dump_json()))
+            final_settings = steward.remove_trailing_underscore(json.loads(self.env.config_settings.model_dump_json()))
         with open(steward.fileio.config, 'w') as file:
             json.dump(final_settings, file, indent=4)
             file.flush()
 
-    def import_config(self) -> None:
-        """Imports the configuration file into filebrowser."""
-        self.logger.info(f"Importing configuration from {steward.fileio.config!r}")
-        self.create_config()
+    def import_config(self, proxy: bool) -> None:
+        """Imports the configuration file into filebrowser.
+
+        Args:
+            proxy: Boolean flag to enable proxy.
+        """
+        self.logger.info("Importing configuration from %s", steward.fileio.config)
+        self.create_config(proxy)
         assert os.path.isfile(steward.fileio.config), f"{steward.fileio.config!r} doesn't exist"
         self.run_subprocess(["config", "import", steward.fileio.config],
                             "Failed to import configuration")
 
-    def import_users(self) -> None:
-        """Imports the user profiles into filebrowser."""
-        self.logger.info(f"Importing user profiles from {steward.fileio.users!r}")
-        self.create_users()
+    def import_users(self) -> Dict[str, str]:
+        """Imports the user profiles into filebrowser.
+
+        Returns:
+            Dict[str, str]:
+            Authentication map provided as environment variables.
+        """
+        self.logger.info("Importing user profiles from %s", steward.fileio.users)
+        auth_map = self.create_users()
         assert os.path.isfile(steward.fileio.users), f"{steward.fileio.users!r} doesn't exist"
         self.run_subprocess(["users", "import", steward.fileio.users],
                             "Failed to import user profiles")
+        return auth_map
+
+    def background_tasks(self, auth_map: Dict[str, str], proxy: bool) -> None:
+        """Initiates the proxy engine and subtitles' format conversion as background tasks.
 
-    def start(self) -> None:
-        """Handler for all the functions above."""
+        Args:
+            auth_map: Authentication map provided as environment variables.
+            proxy: Boolean flag to enable proxy.
+        """
+        if proxy:
+            assert proxy_settings.port != int(self.env.config_settings.server.port), \
+                f"\n\tProxy server can't run on the same port [{proxy_settings.port}] as the server!!"
+            log_config = struct.LoggerConfig(self.logger).get()
+            if proxy_settings.debug:
+                log_config = struct.update_log_level(log_config, logging.DEBUG)
+            # noinspection HttpUrlsUsage
+            self.proxy_engine = multiprocessing.Process(
+                target=proxy_server, daemon=True,
+                args=(f"http://{self.env.config_settings.server.address}:{self.env.config_settings.server.port}",
+                      log_config, auth_map)
+            )
+            self.proxy_engine.start()
+
+    def start(self, proxy: bool = False) -> None:
+        """Handler for all the functions above.
+
+        Args:
+            proxy: Boolean flag to enable proxy.
+        """
         if os.path.isfile(download.executable.filebrowser_db):
             os.remove(download.executable.filebrowser_db)
-        self.import_config()
-        self.import_users()
-        # noinspection HttpUrlsUsage
-        self.logger.info(f"Initiating filebrowser on "
-                         f"http://{self.env.config_settings.server.address}:{self.env.config_settings.server.port}")
-        self.converted = ThreadPool(processes=1).apply_async(func=subtitles.auto_convert,
-                                                             kwds=dict(root=self.env.config_settings.server.root,
-                                                                       logger=self.logger))
+        self.import_config(proxy)
+        self.background_tasks(self.import_users(), proxy)
         self.run_subprocess([], "Failed to run the server", True)
```

## pyfilebrowser/requirements.txt

```diff
@@ -1,4 +1,5 @@
 bcrypt==4.1.*
+fastapi==0.110.*
 pydantic==2.6.*
 pydantic-settings==2.2.*
 requests==2.31.*
```

## pyfilebrowser/modals/config.py

```diff
@@ -141,15 +141,15 @@
     authHook: Optional[str] = ""
     tokenExpirationTime: Optional[str] = ""
 
     class Config:
         """Environment variables configuration."""
 
         env_prefix = ""
-        env_file = os.environ.get("env_file", os.environ.get("ENV_FILE", ".config.env"))
+        env_file = ".config.env"
         extra = "ignore"
 
 
 class Config(BaseSettings):
     """Configuration settings [``config`` section] for the server.
 
     >>> Config
@@ -157,14 +157,15 @@
     """
 
     signup: Optional[bool] = False
     createUserDir: Optional[bool] = False
     userHomeBasePath: Optional[str] = os.path.join(os.path.expanduser('~'), 'users')
     defaults: Optional[Defaults] = Defaults()
     authMethod: Optional[str] = "json"
+    authHeader: Optional[str] = ""
     branding: Optional[Branding] = Branding()
     tus: Optional[Tus] = Tus()
     commands: Optional[Commands] = Commands()
     shell_: Optional[List[str]] = []
     rules: Optional[List[str]] = []
 
     class Config:
```

## pyfilebrowser/squire/download.py

```diff
@@ -100,20 +100,21 @@
 
     See Also:
         - This model is to load GitHub arguments, which is used to download the appropriate asset from source control.
         - Dot env ``(.env)`` files are not supported. Regular env variables are required.
     """
 
     model_config = ExtendedSettingsConfigDict(
-        env_prefixes=["git_", "github_"]
+        env_prefixes=["git_", "github_", "filebrowser_"]
     )
 
     owner: str = "filebrowser"
     repo: str = "filebrowser"
     token: str | None = None
+    version: str = "latest"
 
 
 class Executable(BaseModel):
     """Executable object to load all the objects to download the executable from releases.
 
     >>> Executable
 
@@ -171,27 +172,30 @@
 def binary(logger: logging.Logger, github: GitHub) -> None:
     """Downloads the latest released binary asset.
 
     Args:
         logger: Bring your own logger.
         github: Custom GitHub source configuration.
     """
-    logger.info(f"Source Repository: 'https://github.com/{github.owner}/{github.repo}'")
-    logger.info(f"Targeted Asset: {executable.filebrowser_file!r}")
+    logger.info("Source Repository: 'https://github.com/%s/%s'", github.owner, github.repo)
+    logger.info("Targeted Asset: '%s'", executable.filebrowser_file)
     headers = {"Authorization": f"Bearer {github.token}"} if github.token else {}
-    # Get the latest release
-    response = requests.get(f"https://api.github.com/repos/{github.owner}/{github.repo}/releases/latest",
-                            headers=headers)
+    # Get the release from the specified version
+    if github.version == "latest":
+        release_url = f"https://api.github.com/repos/{github.owner}/{github.repo}/releases/{github.version}"
+    else:
+        release_url = f"https://api.github.com/repos/{github.owner}/{github.repo}/releases/tags/{github.version}"
+    response = requests.get(release_url, headers=headers)
     response.raise_for_status()
     release_info = response.json()
 
-    # Print the download URL, to download manually
+    # Log the download URL
     filebrowser_url = f"https://github.com/{github.owner}/{github.repo}/releases/download/" \
                       f"{release_info['tag_name']}/{executable.filebrowser_file}"
-    logger.info(f"Download URL: {filebrowser_url}")
+    logger.info("Download URL: %s", filebrowser_url)
 
     # Get asset id
     existing = []
     for asset in release_info['assets']:
         if asset.get('name') == executable.filebrowser_file:
             asset_id = asset['id']
             break
@@ -222,26 +226,32 @@
         with gzip.open(executable.filebrowser_file, 'rb') as f_in:
             with open(tar_file, 'wb') as f_out:
                 f_out.write(f_in.read())
                 f_out.flush()
         assert os.path.isfile(tar_file), f"Failed to gunzip {executable.filebrowser_file}"
         os.remove(executable.filebrowser_file)
 
-        # Read the tar file and extract it in the current working directory
-        content_dir = tar_file.removesuffix('.tar')
+        # Read the tar file and extract its content
         with tarfile.open(tar_file, 'r') as tar:
             tar.extractall()
+        # Catches the use case where binary might be directly archived
+        if os.path.isfile(executable.filebrowser_bin):
+            return
+        content_dir = tar_file.removesuffix('.tar')
         assert os.path.isdir(content_dir) and os.path.isfile(os.path.join(content_dir, executable.filebrowser_bin)), \
             f"Failed to unarchive {tar_file}"
         os.remove(tar_file)
     elif executable.filebrowser_file.endswith(".zip"):
-        # Read the zip file and extract it in the current working directory
-        content_dir = executable.filebrowser_file.removesuffix(".zip")
+        # Read the zip file and extract its content
         with zipfile.ZipFile(executable.filebrowser_file, 'r') as zip_ref:
             zip_ref.extractall()
+        # Catches the use case where binary might be directly zipped
+        if os.path.isfile(executable.filebrowser_bin):
+            return
+        content_dir = executable.filebrowser_file.removesuffix(".zip")
         assert os.path.isdir(content_dir) and os.path.isfile(os.path.join(content_dir, executable.filebrowser_bin)), \
             f"Failed to unzip {executable.filebrowser_file}"
         os.remove(executable.filebrowser_file)
     else:
         raise OSError(
             f"Invalid filename: {executable.filebrowser_file}"
         )
@@ -252,8 +262,8 @@
     shutil.rmtree(content_dir)
 
     # Change file permissions and set as executable
     # os.chmod(executable.filebrowser_bin, 0o755)
     # basically, chmod +x => -rwxr-xr-x
     os.chmod(executable.filebrowser_bin, stat.S_IRWXU | stat.S_IRGRP | stat.S_IXGRP | stat.S_IROTH | stat.S_IXOTH)
 
-    logger.info(f"Asset {executable.filebrowser_bin!r} is ready to be used")
+    logger.info("Asset %s is ready to be used", executable.filebrowser_bin)
```

## pyfilebrowser/squire/steward.py

```diff
@@ -8,14 +8,32 @@
 from pydantic import BaseModel, DirectoryPath, FilePath
 
 from pyfilebrowser.modals import config, users
 
 DATETIME_PATTERN = re.compile(r'^\d{4}/\d{2}/\d{2} \d{2}:\d{2}:\d{2} ')
 
 
+def ordinal(n: int) -> str:
+    """Returns the ordinal representation of a given number.
+
+    Args:
+        n: The number for which the ordinal representation is to be determined.
+
+    Returns:
+        str:
+        The ordinal representation of the input number.
+    """
+    if 10 < n % 100 < 20:
+        suffix = "th"
+    else:
+        suffixes = {1: "st", 2: "nd", 3: "rd"}
+        suffix = suffixes.get(n % 10, "th")
+    return f"{n}{suffix}"
+
+
 def default_logger(log_to_file: bool) -> logging.Logger:
     """Generates a default console logger.
 
     Args:
         log_to_file: Boolean flag to stream logs to a file.
 
     Returns:
```

## Comparing `pyfilebrowser-0.0.7.dist-info/LICENSE` & `pyfilebrowser-0.0.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyfilebrowser-0.0.7.dist-info/METADATA` & `pyfilebrowser-0.0.8.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfilebrowser
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python module designed to streamline interactions with filebrowser
 Author-email: Vignesh Rao <svignesh1793@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Vignesh Rao
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -37,14 +37,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Communications :: File Sharing
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: bcrypt ==4.1.*
+Requires-Dist: fastapi ==0.110.*
 Requires-Dist: pydantic ==2.6.*
 Requires-Dist: pydantic-settings ==2.2.*
 Requires-Dist: requests ==2.31.*
 Provides-Extra: dev
 Requires-Dist: sphinx ==5.1.1 ; extra == 'dev'
 Requires-Dist: pre-commit ; extra == 'dev'
 Requires-Dist: recommonmark ; extra == 'dev'
```

## Comparing `pyfilebrowser-0.0.7.dist-info/RECORD` & `pyfilebrowser-0.0.8.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-pyfilebrowser/__init__.py,sha256=EfpHAKTwZ4n0o0SDfnOUz-eeX3jyTd1C3BmFjrawpxw,105
-pyfilebrowser/main.py,sha256=BjFjAb0y08caye3Af0Z5VoBFvKAgNEEgZAWzZqHNJbA,7279
-pyfilebrowser/requirements.txt,sha256=-XD6RWAlSiWBvhueeDvM2kG9ncaZQ1uyq0SUdvN9GFE,72
-pyfilebrowser/modals/config.py,sha256=jBNLDxccrvxue9Y_jkYWwNe1SeoQx1y7H_tZPDGqVhQ,5473
+pyfilebrowser/__init__.py,sha256=J6Tuo-HN2MdoRA3ykq-f7jKbtoB8f41wFmp5FLKTFkU,105
+pyfilebrowser/main.py,sha256=Xmguv0jTcDLfDnYFctk82LXNwIozscezSU0z-xLxCUs,8736
+pyfilebrowser/requirements.txt,sha256=iqRgXyC9MTSdgB8LD5yJDMfc7c5Zmuf82M2AqTakh1w,89
+pyfilebrowser/modals/config.py,sha256=nMRWu1esluHosN3wUw3w5EooubJuBTzpxIoHWcDZB6M,5452
 pyfilebrowser/modals/models.py,sha256=1RVSZaNgWChLv8c0-zMXgSpLDonitMgrc9fYvlzEs3U,1765
 pyfilebrowser/modals/users.py,sha256=xKdpMrcbWTza2llFTRPkKJG3ySEVlvC03rSMA4KgK5s,1603
-pyfilebrowser/squire/download.py,sha256=4IPD585-5YH5MhvyTC8a3xqpWfgtfavC2Jnihr3wP-s,9719
-pyfilebrowser/squire/steward.py,sha256=dU_ocQsHeNYhVRpriRkYlg2VQbzxxv5rQ7fUvL43iz0,4077
-pyfilebrowser/squire/subtitles.py,sha256=-ySR6axeZQ0f39dj33XDLSjNzj_lIWSbr-pVQ1WnKCc,4418
-pyfilebrowser-0.0.7.dist-info/LICENSE,sha256=xnHdLNCLt4RW3vtnE_TfN_cjViUHyIv0m8024fS4bws,1068
-pyfilebrowser-0.0.7.dist-info/METADATA,sha256=YvOFV_ZHE2mU6JNQEuOEhrh1Jm-STUhu0R1Lz-wmSqw,8321
-pyfilebrowser-0.0.7.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-pyfilebrowser-0.0.7.dist-info/top_level.txt,sha256=RrwbvxqHTriDpUwaZC3F5o53eZtUKODCQQ0iRryM_Zo,14
-pyfilebrowser-0.0.7.dist-info/RECORD,,
+pyfilebrowser/squire/download.py,sha256=FI_1GZrjcTtYBE3bXOSa4f-FSgjU9ejANW-NdEZq2KQ,10178
+pyfilebrowser/squire/steward.py,sha256=hVoWBrJWa2HSvR56JKnk_vXh0Qm0jPbEGwQ4dWtpXM8,4525
+pyfilebrowser/squire/struct.py,sha256=rg19tpW1iX17792uFWLQAhVZ2PLiHYETYc21GFulldE,3056
+pyfilebrowser-0.0.8.dist-info/LICENSE,sha256=xnHdLNCLt4RW3vtnE_TfN_cjViUHyIv0m8024fS4bws,1068
+pyfilebrowser-0.0.8.dist-info/METADATA,sha256=HhFlxavpr9gHo_b9rPiLDHXvEbokg3TrxRZJx9u0l1Q,8354
+pyfilebrowser-0.0.8.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+pyfilebrowser-0.0.8.dist-info/top_level.txt,sha256=RrwbvxqHTriDpUwaZC3F5o53eZtUKODCQQ0iRryM_Zo,14
+pyfilebrowser-0.0.8.dist-info/RECORD,,
```

