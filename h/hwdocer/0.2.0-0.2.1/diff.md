# Comparing `tmp/hwdocer-0.2.0.tar.gz` & `tmp/hwdocer-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hwdocer-0.2.0.tar", max compression
+gzip compressed data, was "hwdocer-0.2.1.tar", max compression
```

## Comparing `hwdocer-0.2.0.tar` & `hwdocer-0.2.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     3134 2024-04-03 19:29:01.034792 hwdocer-0.2.0/doc/release.md
--rw-r--r--   0        0        0     1986 2024-04-03 19:30:08.088584 hwdocer-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2845 2024-04-03 19:29:01.034792 hwdocer-0.2.0/readme.md
--rw-r--r--   0        0        0       22 2024-04-03 19:30:08.088584 hwdocer-0.2.0/src/hwdocer/__init__.py
--rw-r--r--   0        0        0      139 2024-03-25 19:30:35.876996 hwdocer-0.2.0/src/hwdocer/__main__.py
--rw-r--r--   0        0        0    17957 2024-04-03 19:29:01.034792 hwdocer-0.2.0/src/hwdocer/hwdocer.py
--rw-r--r--   0        0        0     4644 1970-01-01 00:00:00.000000 hwdocer-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     4495 2024-04-04 22:13:50.943539 hwdocer-0.2.1/doc/release.md
+-rw-r--r--   0        0        0     1999 2024-04-04 22:18:33.910169 hwdocer-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2845 2024-04-03 19:29:01.034792 hwdocer-0.2.1/readme.md
+-rw-r--r--   0        0        0       22 2024-04-04 22:16:42.129870 hwdocer-0.2.1/src/hwdocer/__init__.py
+-rw-r--r--   0        0        0      139 2024-03-25 19:30:35.876996 hwdocer-0.2.1/src/hwdocer/__main__.py
+-rw-r--r--   0        0        0    18828 2024-04-04 22:11:19.220564 hwdocer-0.2.1/src/hwdocer/hwdocer.py
+-rw-r--r--   0        0        0     4679 1970-01-01 00:00:00.000000 hwdocer-0.2.1/PKG-INFO
```

### Comparing `hwdocer-0.2.0/pyproject.toml` & `hwdocer-0.2.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "hwdocer"
-version = "0.2.0"
+version = "0.2.1"
 description = "Wireviz, drawio and other documentation build tool"
 authors = ["Laurence DV <laurencedv@realee.tech>"]
 homepage = "https://gitlab.com/real-ee/public/hwdocer"
 repository = "https://gitlab.com/real-ee/public/hwdocer"
 documentation = "https://gitlab.com/real-ee/public/hwdocer/-/tree/master/doc"
 readme = "readme.md"
 license = "GPL-3.0-or-later"
 keywords = ["drawio", "wireviz", "toolchain", "automation", "documentation"]
 classifiers = [
-    "Development Status :: 2 - Pre-Alpha",
+    "Development Status :: 3 - Alpha",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Operating System :: POSIX :: Linux",
     "Topic :: Documentation",
     "Topic :: Multimedia :: Graphics",
     "Topic :: Scientific/Engineering",
@@ -33,21 +33,22 @@
 hwdocer = "hwdocer.__main__:main"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 wireviz = "^0.3.2"
 drawio = "^0.0.10"
 pyyaml = "^6.0.1"
+rich = "^13.7.1"
 
 [tool.poetry.group.dev.dependencies]
 bumpver = "^2023.1129"
 pytest = "^7.4.0"
 
 [tool.bumpver]
-current_version = "0.2.0"
+current_version = "0.2.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "Version increase {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `hwdocer-0.2.0/readme.md` & `hwdocer-0.2.1/readme.md`

 * *Files identical despite different names*

### Comparing `hwdocer-0.2.0/src/hwdocer/hwdocer.py` & `hwdocer-0.2.1/src/hwdocer/hwdocer.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,19 +6,21 @@
 import sys
 import glob
 import shutil
 import argparse
 import pathlib
 import time
 import yaml
-from subprocess import DEVNULL, check_call
+from subprocess import DEVNULL, check_call, run
+from rich import print
 
 # logging
-from multiprocessing import Process, Queue, current_process, Pool
+from multiprocessing import Process, Queue, current_process
 from logging.handlers import TimedRotatingFileHandler, QueueHandler
+from rich.logging import RichHandler
 import logging
 
 
 class HwDocer(object):
 
     __def_output__ = '_build'
     __def_input__ = './'
@@ -92,116 +94,117 @@
             self.exec_timeout = self.__def_timeout__
         else:
             self.exec_timeout = self.args.timeout
         self.logger.debug(f'args - timeout: {self.exec_timeout} sec')
 
         # param - diagram format
         self.dia_format = self.args.dia
-        self.logger.debug(f'args - dia format: {self.dia_format}')
+        self.logger.debug(f'args - dia format: \'{self.dia_format}\'')
 
         # arg - harness format
         self.hrs_format = self.args.hrs
-        self.logger.debug(f'args - hrs format: {self.hrs_format}')
+        self.logger.debug(f'args - hrs format: \'{self.hrs_format}\'')
 
         # start with empty work queues
         self.work_q = Queue()
         self.done_q = Queue()
         self.logger.debug(f'work queue: {id(self.work_q)}, done queue: {id(self.done_q)}')
 
         self.time_creation = time.time()
         self.logger.debug(f'{__name__} created successfully in {self.time_creation - self.time_start:.6f} sec')
 
     def _search_and_copy_files(self):
-        self.logger.debug(f'searching in \'{self.src_path}\' for {self.__search_folder__}')     # first search all subfolder to known the complete structure
+        self.logger.debug(f'searching in {self.src_path} for {self.__search_folder__}')     # first search all subfolder to known the complete structure
 
         # searching in subfolders
         for folder in glob.iglob(self.src_path + self.__search_folder__, recursive=True):
-            self.logger.debug(f'folder found: \'{folder}\'')
+            self.logger.debug(f'folder found: {folder}')
 
             # searching for harnesses
-            self.logger.debug(f'searching in \'{folder}\' for {self.__search_hrs__}')
+            self.logger.debug(f'searching in {folder} for {self.__search_hrs__}')
             for file in glob.iglob(folder + self.__search_hrs__):
-                self.logger.debug(f'harness found: \'{os.path.basename(file)}\'')
+                self.logger.debug(f'harness found: {os.path.basename(file)}')
                 copied_file = self._copy_src_files(file)
                 if os.path.basename(copied_file) == os.path.basename(file):     # ensure the copied file atleast as the same name as original
-                    self.logger.debug(f'work added: \'{os.path.basename(copied_file)}\'')
+                    self.logger.debug(f'work added: {os.path.basename(copied_file)}')
                     self.work_q.put(copied_file)
 
             # searching for diagrams
-            self.logger.debug(f'searching in \'{folder}\' for {self.__search_dia__}')
+            self.logger.debug(f'searching in {folder} for {self.__search_dia__}')
             for file in glob.iglob(folder + self.__search_dia__):
-                self.logger.debug(f'diagram found: \'{os.path.basename(file)}\'')
+                self.logger.debug(f'diagram found: {os.path.basename(file)}')
                 copied_file = self._copy_src_files(file)
                 if os.path.basename(copied_file) == os.path.basename(file):     # ensure the copied file atleast as the same name as original
-                    self.logger.debug(f'work added: \'{os.path.basename(copied_file)}\'')
+                    self.logger.debug(f'work added: {os.path.basename(copied_file)}')
                     self.work_q.put(copied_file)
 
         self.time_search = time.time()
         self.logger.info(f'found {self.work_q.qsize()} buildable files in {self.time_search - self.time_creation:.6f} sec')
 
     def _prep_output(self):
         self.logger.debug(f'outut folder preparation')
 
         # Folder structure recreation
         try:
             # ensure root folder exists
             if not os.path.exists(self.dst_path):
-                self.logger.info(f'creating output folder: \'{self.dst_path}\'')
+                self.logger.info(f'creating output folder: {self.dst_path}')
                 os.makedirs(self.dst_path)
             else:
-                self.logger.debug(f'output folder: \'{self.dst_path}\' already existed')
+                self.logger.debug(f'output folder: {self.dst_path} already existed')
         except Exception as e:
-            self.logger.error(f'failed to create output folder \'{self.dst_path}\'')
+            self.logger.error(f'failed to create output folder {self.dst_path}')
             raise e
 
     def _silentremove(self, file):
         try:
             os.remove(file)
         except OSError as e:
-            self.logger.debug(f'tried to delete \'{file}\' but wasn\'t present')
+            self.logger.debug(f'tried to delete {file} but wasn\'t present')
             if e.errno != errno.ENOENT:
                 raise
 
     def build_hrs(self, hrs) -> int:
-        self.logger.info(f'hrs building: \'{os.path.basename(hrs)}\'')
+        self.logger.info(f'hrs building: {os.path.basename(hrs)}')
         exec_status = -1
 
         # Building
         try:
-            exec_status = check_call(['wireviz', hrs], stdout=DEVNULL, stderr=DEVNULL)
+            exec_status = run(['wireviz', hrs])
         except Exception as e:
-            self.logger.error(f'wireviz failed: \'{e}\'')
+            self.logger.error(f'wireviz failed: {e}')
 
         # Cleanup unwanted output
         for hrsformat in self.__hrs_format_choices__:   # delete all files that weren't mentionned to be kept
             if hrsformat not in self.hrs_format:
                 # handle special cases
                 if hrsformat == 'bom':
                     hrsformat = 'bom.tsv'   # extension of bom file is special
                 elif hrsformat == 'pdf(NOT IMPLEMENTED)':
                     hrsformat = 'pdf'
                 # delete the file with absolute path
                 file2del = os.path.dirname(hrs) + '/' + pathlib.Path(hrs).stem + '.' + hrsformat
-                self.logger.debug(f'deleting file \'{file2del}\'')
+                self.logger.debug(f'deleting file {file2del}')
                 self._silentremove(file2del)
 
-        self.logger.debug(f'hrs built: \'{hrs}\'')
-        return exec_status
+        self.logger.debug(f'hrs built: {hrs}')
+        return exec_status.returncode
 
     def build_dia(self, dia) -> int:
-        self.logger.info(f'dia building: \'{os.path.basename(dia)}\'')
+        self.logger.info(f'dia building: {os.path.basename(dia)}')
         exec_status = -1
 
         # Building
         try:
+            # This still need to be sushed (check_call vs run) because of all the gpu error and chatter in stdout
             exec_status = check_call(['drawio', '-x', '-t', '-f', self.dia_format, dia], stdout=DEVNULL, stderr=DEVNULL)
         except Exception as e:
-            self.logger.error(f'drawio failed: \'{e}\'')
+            self.logger.error(f'drawio failed: {e}')
 
-        self.logger.debug(f'dia built \'{dia}\'')
+        self.logger.debug(f'dia built {dia}')
         return exec_status
 
     def _get_diffpath(self, basepath: pathlib.Path, filepath: pathlib.Path) -> pathlib.Path:
         subpath = '.'
         if basepath is not None and filepath is not None:
             commonpath = os.path.commonpath([basepath, filepath])
             subpath = os.path.dirname(filepath).replace(commonpath, '')
@@ -212,51 +215,51 @@
             file = pathlib.Path(file)  # ensure the file is a valid path
             resulting_file = pathlib.Path()
             # 1. Create subfolder in destination
             try:
                 subfolder = self._get_diffpath(self.src_path, file)
                 destination = pathlib.Path(str(self.dst_path) + str(subfolder))
                 if not os.path.exists(destination):
-                    self.logger.info(f'creating folder: \'{destination}\'')
+                    self.logger.info(f'creating folder: {destination}')
                     os.makedirs(destination)
                 else:
-                    self.logger.debug(f'folder: \'{destination}\' already existed')
+                    self.logger.debug(f'folder: {destination} already existed')
             except Exception as e:
-                self.logger.error(f'failed to create folder: \'{destination}\'')
+                self.logger.error(f'failed to create folder: {destination}')
                 raise e
             # 2. Copy source file
             try:
-                self.logger.info(f'copying \'{file}\'to \'{destination}\'')
+                self.logger.info(f'copying {file}to {destination}')
                 shutil.copy2(file, destination)
                 resulting_file = os.path.join(destination, os.path.basename(file))
             except Exception as e:
-                self.logger.error(f'failed to copy file: \'{file}\'')
+                self.logger.error(f'failed to copy file: {file}')
                 raise e
             # 3. If harness, also copy images
             try:
                 if file.suffix == self.__suffix_hrs__:
                     img_list = self._get_all_img_path_from_hrs(file)
                     if len(img_list) > 0:
-                        self.logger.info(f'copying {len(img_list)} image(s) linked in \'{file}\'')
+                        self.logger.info(f'copying {len(img_list)} image(s) linked in {file}')
                     for image in img_list:
                         # compute the complete destination path
                         subfolder = self._get_diffpath(self.src_path, image)
                         destination = pathlib.Path(str(self.dst_path) + str(subfolder) + '/' + os.path.basename(image))
-                        self.logger.debug(f'copying image: \'{image}\' to \'{destination}\'')
+                        self.logger.debug(f'copying image: {image} to {destination}')
                         # make sure directory exist at destination
                         os.makedirs(os.path.dirname(destination), exist_ok=True)
 
                         if not os.path.exists(os.path.join(destination, os.path.basename(image))):
                             shutil.copy2(image, destination)
                         else:
-                            self.logger.debug(f'\'{image}\' already exist')
+                            self.logger.debug(f'{image} already exist')
             except Exception as e:
-                self.logger.warning(f'failed to copy image: \'{destination}\'')
+                self.logger.warning(f'failed to copy image: {destination} from {file}')
 
-            self.logger.debug(f'successfully copied: \'{resulting_file}\'')
+            self.logger.debug(f'successfully copied: {resulting_file}')
             return resulting_file
 
     def _get_all_img_path_from_hrs(self, hrs_path: pathlib.Path) -> list:
         image_list = []
 
         try:
             with open(hrs_path, 'r') as file:
@@ -265,18 +268,18 @@
                     if key == 'connectors' or key == 'cables':      # top level
                         for key2, val2 in val.items():              # connectors & cables listing level
                             for key3, val3 in val2.items():         # each conn/cable element level
                                 if key3 == 'image':                 # we only care for the image element
                                     for key4, val4 in val3.items():  # image element level
                                         if key4 == 'src':           # we find the source path of it
                                             image = os.path.normpath(os.path.join(os.path.dirname(hrs_path), val4))
-                                            self.logger.debug(f'image found: \'{val4}\' for {key2}')
+                                            self.logger.debug(f'image found: {val4} for {key2}')
                                             image_list.append(image)
         except Exception as e:
-            self.logger.warning(f'failed to open \'{hrs_path}\'')
+            self.logger.warning(f'failed to open {hrs_path}')
         # end try
         return image_list
 
     def run(self):
         status = 0
 
         self.logger.info(f'S execution, pid: {current_process().pid}')
@@ -308,16 +311,27 @@
                 self.logger.warning(f'timeout reached after {waited:.3f} sec')
                 for i in range(len(processes)):
                     # TODO: send explicit stop signal to workers
                     pass
                 break
             time.sleep(0.1)
 
+        # work stats
+        hrs_count = 0
+        dia_count = 0
+        for _ in range(self.done_q.qsize()):
+            file = self.done_q.get()
+            if pathlib.Path(file).suffix == self.__suffix_hrs__:
+                hrs_count += 1
+            elif pathlib.Path(file).suffix == self.__suffix_dia__:
+                dia_count += 1
+
         # graceful end of exec
-        self.logger.info(f'P execution, pid: {current_process().pid}, total time: {self.time_done - self.time_start:.6f} sec')
+        print(f'built [dark_orange bold]{hrs_count} harnesses[/] and [purple bold]{dia_count} diagrams[/] in {self.time_done - self.time_start:.6f} sec')
+        self.logger.info(f'P execution, pid: {current_process().pid}, built {hrs_count} harnesses and {dia_count} diagrams in {self.time_done - self.time_start:.6f} sec')
         self.log_q.put(None)
         return status
 
     def worker_process(self, log_q: Queue, q_in: Queue, q_out: Queue) -> int:
         """worker isolated process to generate output files from input file
 
         Args:
@@ -376,27 +390,32 @@
         # Create a separate folder for logs if it doesn't exist
         log_dir = 'log'
         if not os.path.exists(log_dir):
             os.makedirs(log_dir)
 
         # Formater
         formatter = logging.Formatter('%(asctime)s.%(msecs)03d | %(name)-15s | %(levelname)-8s | %(message)s', datefmt='%Y-%m-%dT%H:%M:%S')
+        rich_formatter = logging.Formatter('[light_sea_green]%(name)-15s[/] %(message)s')
 
         # File logging
         log_filename = os.path.join(log_dir, f'hwdocer_{time.strftime("%Y-%m-%d_%H-%M-%S")}.log')
         file_handler = TimedRotatingFileHandler(log_filename, when='midnight', backupCount=4)
         file_handler.setFormatter(formatter)
 
         # Console logging
+        rich_handler = RichHandler(rich_tracebacks=True, markup=True)
+        rich_handler.setLevel(self.verbosity)
+        rich_handler.setFormatter(rich_formatter)
         stream_handler = logging.StreamHandler(sys.stdout)
         stream_handler.setLevel(self.verbosity)  # Set the level as needed
         stream_handler.setFormatter(formatter)
 
         logger.addHandler(file_handler)
-        logger.addHandler(stream_handler)
+        # logger.addHandler(stream_handler)
+        logger.addHandler(rich_handler)
 
         logger.info(f'S execution, pid: {current_process().pid}')
 
         # process loop
         while True:
             msg = queue.get()       # pull new message from queue
             if msg is None:         # exit process on special None message
```

### Comparing `hwdocer-0.2.0/PKG-INFO` & `hwdocer-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: hwdocer
-Version: 0.2.0
+Version: 0.2.1
 Summary: Wireviz, drawio and other documentation build tool
 Home-page: https://gitlab.com/real-ee/public/hwdocer
 License: GPL-3.0-or-later
 Keywords: drawio,wireviz,toolchain,automation,documentation
 Author: Laurence DV
 Author-email: laurencedv@realee.tech
 Requires-Python: >=3.8,<4.0
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -22,14 +22,15 @@
 Classifier: Topic :: Documentation
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Utilities
 Requires-Dist: drawio (>=0.0.10,<0.0.11)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
+Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: wireviz (>=0.3.2,<0.4.0)
 Project-URL: Changelog, https://gitlab.com/real-ee/public/hwdocer/-/blob/master/doc/release.md
 Project-URL: Contribution, https://gitlab.com/real-ee/public/hwdocer/-/blob/master/doc/contrib.md?ref_type=heads
 Project-URL: Documentation, https://gitlab.com/real-ee/public/hwdocer/-/tree/master/doc
 Project-URL: Issue, https://gitlab.com/real-ee/public/hwdocer/-/issues
 Project-URL: Repository, https://gitlab.com/real-ee/public/hwdocer
 Project-URL: Roadmap, https://gitlab.com/real-ee/public/hwdocer/-/blob/master/doc/roadmap.md
```

