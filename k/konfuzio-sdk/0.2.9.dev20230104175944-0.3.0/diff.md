# Comparing `tmp/konfuzio_sdk-0.2.9.dev20230104175944.tar.gz` & `tmp/konfuzio_sdk-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "konfuzio_sdk-0.2.9.dev20230104175944.tar", last modified: Thu Jan  5 03:29:15 2023, max compression
+gzip compressed data, was "konfuzio_sdk-0.3.0.tar", last modified: Fri Apr  5 07:50:52 2024, max compression
```

## Comparing `konfuzio_sdk-0.2.9.dev20230104175944.tar` & `konfuzio_sdk-0.3.0.tar`

### file list

```diff
@@ -1,33 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 03:29:15.634518 konfuzio_sdk-0.2.9.dev20230104175944/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-01-05 03:29:07.000000 konfuzio_sdk-0.2.9.dev20230104175944/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     9656 2023-01-05 03:29:15.634518 konfuzio_sdk-0.2.9.dev20230104175944/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9337 2023-01-05 03:29:07.000000 konfuzio_sdk-0.2.9.dev20230104175944/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 03:29:15.630517 konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-01-05 03:29:07.000000 konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19149 2023-01-05 03:29:07.000000 konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-01-05 03:29:07.000000 konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)   123551 2023-01-05 03:29:07.000000 konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    20038 2023-01-05 03:29:07.000000 konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)    24739 2023-01-05 03:29:07.000000 konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk/normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)    12225 2023-01-05 03:29:07.000000 konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk/regex.py
--rw-r--r--   0 runner    (1001) docker     (123)    18869 2023-01-05 03:29:07.000000 konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk/samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-01-05 03:29:07.000000 konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk/settings_importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 03:29:15.634518 konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk/tokenizer/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-01-05 03:29:07.000000 konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk/tokenizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-01-05 03:29:07.000000 konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk/tokenizer/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9332 2023-01-05 03:29:07.000000 konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk/tokenizer/regex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 03:29:15.634518 konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-01-05 03:29:07.000000 konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-01-05 03:29:07.000000 konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk/trainer/document_categorization.py
--rw-r--r--   0 runner    (1001) docker     (123)   107540 2023-01-05 03:29:07.000000 konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk/trainer/information_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-01-05 03:29:07.000000 konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    40041 2023-01-05 03:29:07.000000 konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 03:29:15.634518 konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9656 2023-01-05 03:29:15.000000 konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-01-05 03:29:15.000000 konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-05 03:29:15.000000 konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-01-05 03:29:15.000000 konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-01-05 03:29:15.000000 konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-01-05 03:29:15.000000 konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-01-05 03:29:15.634518 konfuzio_sdk-0.2.9.dev20230104175944/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-01-05 03:29:07.000000 konfuzio_sdk-0.2.9.dev20230104175944/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:50:52.407203 konfuzio_sdk-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-05 07:50:41.000000 konfuzio_sdk-0.3.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8267 2024-04-05 07:50:52.407203 konfuzio_sdk-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6105 2024-04-05 07:50:41.000000 konfuzio_sdk-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:50:52.395203 konfuzio_sdk-0.3.0/konfuzio_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-05 07:50:41.000000 konfuzio_sdk-0.3.0/konfuzio_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33726 2024-04-05 07:50:41.000000 konfuzio_sdk-0.3.0/konfuzio_sdk/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-05 07:50:41.000000 konfuzio_sdk-0.3.0/konfuzio_sdk/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)   202574 2024-04-05 07:50:41.000000 konfuzio_sdk-0.3.0/konfuzio_sdk/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44747 2024-04-05 07:50:41.000000 konfuzio_sdk-0.3.0/konfuzio_sdk/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-04-05 07:50:41.000000 konfuzio_sdk-0.3.0/konfuzio_sdk/extras.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27450 2024-04-05 07:50:41.000000 konfuzio_sdk-0.3.0/konfuzio_sdk/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12222 2024-04-05 07:50:41.000000 konfuzio_sdk-0.3.0/konfuzio_sdk/regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27029 2024-04-05 07:50:41.000000 konfuzio_sdk-0.3.0/konfuzio_sdk/samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-05 07:50:41.000000 konfuzio_sdk-0.3.0/konfuzio_sdk/settings_importer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:50:52.399203 konfuzio_sdk-0.3.0/konfuzio_sdk/tokenizer/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-05 07:50:41.000000 konfuzio_sdk-0.3.0/konfuzio_sdk/tokenizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13180 2024-04-05 07:50:41.000000 konfuzio_sdk-0.3.0/konfuzio_sdk/tokenizer/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15231 2024-04-05 07:50:41.000000 konfuzio_sdk-0.3.0/konfuzio_sdk/tokenizer/paragraph_and_sentence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9141 2024-04-05 07:50:41.000000 konfuzio_sdk-0.3.0/konfuzio_sdk/tokenizer/regex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:50:52.399203 konfuzio_sdk-0.3.0/konfuzio_sdk/trainer/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-05 07:50:41.000000 konfuzio_sdk-0.3.0/konfuzio_sdk/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11598 2024-04-05 07:50:41.000000 konfuzio_sdk-0.3.0/konfuzio_sdk/trainer/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75617 2024-04-05 07:50:41.000000 konfuzio_sdk-0.3.0/konfuzio_sdk/trainer/document_categorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50589 2024-04-05 07:50:41.000000 konfuzio_sdk-0.3.0/konfuzio_sdk/trainer/file_splitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-04-05 07:50:41.000000 konfuzio_sdk-0.3.0/konfuzio_sdk/trainer/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)   101643 2024-04-05 07:50:41.000000 konfuzio_sdk-0.3.0/konfuzio_sdk/trainer/information_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12209 2024-04-05 07:50:41.000000 konfuzio_sdk-0.3.0/konfuzio_sdk/trainer/tokenization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-04-05 07:50:41.000000 konfuzio_sdk-0.3.0/konfuzio_sdk/trainer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11834 2024-04-05 07:50:41.000000 konfuzio_sdk-0.3.0/konfuzio_sdk/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37377 2024-04-05 07:50:41.000000 konfuzio_sdk-0.3.0/konfuzio_sdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:50:52.403203 konfuzio_sdk-0.3.0/konfuzio_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8267 2024-04-05 07:50:52.000000 konfuzio_sdk-0.3.0/konfuzio_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-05 07:50:52.000000 konfuzio_sdk-0.3.0/konfuzio_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 07:50:52.000000 konfuzio_sdk-0.3.0/konfuzio_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-05 07:50:52.000000 konfuzio_sdk-0.3.0/konfuzio_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-05 07:50:52.000000 konfuzio_sdk-0.3.0/konfuzio_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-05 07:50:52.000000 konfuzio_sdk-0.3.0/konfuzio_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-05 07:50:41.000000 konfuzio_sdk-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 07:50:52.407203 konfuzio_sdk-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-04-05 07:50:41.000000 konfuzio_sdk-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:50:52.403203 konfuzio_sdk-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    22465 2024-04-05 07:50:42.000000 konfuzio_sdk-0.3.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-04-05 07:50:42.000000 konfuzio_sdk-0.3.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)   167058 2024-04-05 07:50:42.000000 konfuzio_sdk-0.3.0/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80271 2024-04-05 07:50:42.000000 konfuzio_sdk-0.3.0/tests/test_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-05 07:50:42.000000 konfuzio_sdk-0.3.0/tests/test_extras.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10164 2024-04-05 07:50:42.000000 konfuzio_sdk-0.3.0/tests/test_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41449 2024-04-05 07:50:42.000000 konfuzio_sdk-0.3.0/tests/test_regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-05 07:50:42.000000 konfuzio_sdk-0.3.0/tests/test_samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9505 2024-04-05 07:50:42.000000 konfuzio_sdk-0.3.0/tests/test_urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20678 2024-04-05 07:50:42.000000 konfuzio_sdk-0.3.0/tests/test_utils.py
```

### Comparing `konfuzio_sdk-0.2.9.dev20230104175944/LICENSE.md` & `konfuzio_sdk-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk/cli.py` & `konfuzio_sdk-0.3.0/konfuzio_sdk/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """Command Line interface to the konfuzio_sdk package."""
 
 import logging
 import sys
 from getpass import getpass
 
-from konfuzio_sdk.api import create_new_project
-from konfuzio_sdk.data import download_training_and_test_data
-from konfuzio_sdk.api import init_env
+from konfuzio_sdk.api import create_new_project, init_env
+from konfuzio_sdk.data import Project
 
 sys.tracebacklimit = 0
 
 logger = logging.getLogger(__name__)
 
 CLI_ERROR = """
 Please enter a valid command line option.
@@ -18,40 +17,49 @@
 
 konfuzio_sdk init
     add the API Token as .env file to connect to the Konfuzio Server, i.e. Host
 konfuzio_sdk create_Project >NAME<
     Create a new Project on the Konfuzio Server. Returns the ID of the new Project.
 konfuzio_sdk export_project >ID<
     Download the data from a Project by ID to migrate it to another Host.
+konfuzio_sdk export_project >ID< include_ai
+    Download the data of a Project by ID to migrate it to another Host, including the (status) Done & Activated AI
+    models
 
 These commands should be run inside of your working directory.
 
 A bug report can be filed at https://github.com/konfuzio-ai/document-ai-python-sdk/issues. Thanks!
 """
 
 
 def credentials():
     """Retrieve user input."""
-    user = input("Username you use to login to Konfuzio Server: ")
-    password = getpass("Password you use to login to Konfuzio Server: ")
-    host = str(input("Server Host URL (press [ENTER] for https://app.konfuzio.com): ") or 'https://app.konfuzio.com')
+    user = input('Username you use to login to Konfuzio Server: ')
+    password = getpass('Password you use to login to Konfuzio Server: ')
+    host = str(
+        input('Server Host URL (press [ENTER] for https://app.konfuzio.com): ') or 'https://app.konfuzio.com'
+    ).rstrip('/')
     return user, password, host
 
 
 def main():
     """CLI of Konfuzio SDK."""
-    _cli_file_path = sys.argv.pop(0)  # NOQA
+    _cli_file_path = sys.argv.pop(0)
     if len(sys.argv) == 1 and sys.argv[0] == 'init':
         user, password, host = credentials()
         init_env(user=user, password=password, host=host)
-    elif len(sys.argv) == 2 and sys.argv[0] == 'export_project' and sys.argv[1].isdigit():
-        download_training_and_test_data(id_=int(sys.argv[1]))
+    elif len(sys.argv) in range(2, 4) and sys.argv[0] == 'export_project' and sys.argv[1].isdigit():
+        include_ais = False
+        if len(sys.argv) == 3:
+            include_ais = True if sys.argv[2] == 'include_ai' else False
+        project = Project(id_=int(sys.argv[1]))
+        project.export_project_data(include_ais=include_ais)
     elif len(sys.argv) == 2 and sys.argv[0] == 'create_project' and sys.argv[1]:
         create_new_project(sys.argv[1])
     else:
         print(CLI_ERROR)
         return -1
     return 0
 
 
-if __name__ == "__main__":
+if __name__ == '__main__':
     main()  # pragma: no cover
```

### Comparing `konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk/data.py` & `konfuzio_sdk-0.3.0/konfuzio_sdk/data.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,57 +1,74 @@
 """Handle data from the API."""
 import io
 import itertools
 import json
 import logging
 import os
 import pathlib
-import regex as re
 import shutil
 import time
 import zipfile
-from typing import Optional, List, Union, Tuple, Dict
+from copy import deepcopy
+from enum import Enum
+from typing import Dict, Iterable, List, Optional, Tuple, Union
 from warnings import warn
 
 import dateutil.parser
+import regex as re
 from PIL import Image, ImageDraw, ImageFont
+from requests import HTTPError
 from tqdm import tqdm
 
 from konfuzio_sdk.api import (
-    _konfuzio_session,
+    delete_document_annotation,
+    delete_file_konfuzio_api,
     download_file_konfuzio_api,
+    export_ai_models,
+    get_all_project_ais,
+    get_document_annotations,
+    get_document_bbox,
+    get_document_details,
     get_meta_of_files,
-    get_project_details,
+    get_page_image,
+    get_project_categories,
+    get_results_from_segmentation,
+    konfuzio_session,
     post_document_annotation,
-    get_document_details,
     update_document_konfuzio_api,
-    get_page_image,
-    delete_document_annotation,
+    upload_file_konfuzio_api,
 )
 from konfuzio_sdk.normalize import normalize
-from konfuzio_sdk.regex import get_best_regex, regex_matches, suggest_regex_for_string, merge_regex
+from konfuzio_sdk.regex import get_best_regex, merge_regex, regex_matches, suggest_regex_for_string
 from konfuzio_sdk.urls import get_annotation_view_url
-from konfuzio_sdk.utils import get_missing_offsets
-from konfuzio_sdk.utils import is_file, convert_to_bio_scheme, amend_file_name, sdk_isinstance
+from konfuzio_sdk.utils import (
+    amend_file_name,
+    convert_to_bio_scheme,
+    exception_or_log_error,
+    get_file_type_and_extension,
+    get_missing_offsets,
+    is_file,
+    sdk_isinstance,
+)
 
 logger = logging.getLogger(__name__)
 
 
 class Data:
     """Collect general functionality to work with data from API."""
 
     id_iter = itertools.count()
     id_ = None
     id_local = None
-    session = _konfuzio_session()
+    session = konfuzio_session()
     _update = False
     _force_offline = False
 
     def __eq__(self, other) -> bool:
-        """Compare any point of data with their ID, overwrite if needed."""
+        """Compare any point of Data with their ID, overwrite if needed."""
         if self.id_ is None and other and other.id_ is None:
             # Compare to virtual instances
             return self.id_local == other.id_local
         else:
             return self.id_ is not None and other is not None and other.id_ is not None and self.id_ == other.id_
 
     def __hash__(self):
@@ -74,44 +91,91 @@
     # todo require to overwrite lose_weight via @abstractmethod
     def lose_weight(self):
         """Delete data of the instance."""
         self.session = None
         return self
 
     def set_offline(self):
-        """Force data into offline mode."""
+        """Force Data into offline mode."""
         self._force_offline = True
         self._update = False
 
 
 class Page(Data):
-    """Access the information about one Page of a document."""
+    """
+    Access the information about one Page of a Document.
+
+    For more details see https://dev.konfuzio.com/sdk/explanations.html#page-concept
+    """
 
     def __init__(
         self,
         id_: Union[int, None],
         document: 'Document',
-        start_offset: int,
-        end_offset: int,
         number: int,
         original_size: Tuple[float, float],
+        image_size: Tuple[int, int] = (None, None),
+        start_offset: Optional[int] = None,
+        end_offset: Optional[int] = None,
+        copy_of_id: Optional[int] = None,
     ):
-        """Create a Page for a Document."""
+        """
+        Create a Page for a Document.
+
+        :param id_: ID of the Page
+        :param document: Document the Page belongs to
+        :param number: Page number in Document (1-based indexing)
+        :param original_size: Size of original Document file Page (all Document Bboxes are based on this scale)
+        :param image_size: Size of the image representation of the Page
+        :param start_offset: Start of the Page in the text of the Document
+        :param end_offset: End of the Page in the text of the Document
+        :param category: The Category the Page belongs to, if any
+        :param copy_of_id: The ID of the Page that this Page is a copy of, if any
+        """
         self.id_ = id_
         self.document = document
         self.number = number
         self.index = number - 1
         document.add_page(self)
         self.start_offset = start_offset
         self.end_offset = end_offset
-        self.image = None
+        if start_offset is None or end_offset is None:
+            page_texts = self.document.text.split('\f')
+            self.start_offset = sum([len(page_text) for page_text in page_texts[: self.index]]) + self.index
+            self.end_offset = self.start_offset + len(page_texts[self.index])
+
+        self.copy_of_id = copy_of_id
+        self.text_encoded: List[int] = None
+        self.image: Optional[Image.Image] = None
+        self.image_bytes: Optional[bytes] = None
         self._original_size = original_size
         self.width = self._original_size[0]
         self.height = self._original_size[1]
-        self.image_path = os.path.join(self.document.document_folder, f'page_{self.number}.png')
+        self._image_size = image_size
+        self.image_width = self._image_size[0]
+        self.image_height = self._image_size[1]
+
+        document_folder = (
+            self.document.document_folder
+            if self.id_
+            else self.document.project.get_document_by_id(self.document.copy_of_id).document_folder
+        )
+        self.image_path = os.path.join(document_folder, f'page_{self.number}.png')
+
+        self._category = self.document._category
+        self.category_annotations: List['CategoryAnnotation'] = []
+        self._human_chosen_category_annotation: Optional[CategoryAnnotation] = None
+        self._segmentation = None
+        self.is_first_page = None
+        self.is_first_page_confidence = None
+        if self.number == 1:
+            self.is_first_page = True
+            self.is_first_page_confidence = 1
+        else:
+            self.is_first_page = False
 
         check_page = True
         if self.index is None:
             logger.error(f'Page index is None of {self} in {self.document}.')
             check_page = False
         if self.height is None:  # todo why do we allow pages with height<=0?
             logger.error(f'Page Height is None of {self} in {self.document}.')
@@ -119,67 +183,97 @@
         if self.width is None:  # todo why do we allow pages with width<=0?
             logger.error(f'Page Width is None of {self} in {self.document}.')
             check_page = False
         assert check_page
 
     def __hash__(self):
         """Define that one Page per Document is unique."""
-        return (self.document, self.index)
+        return hash((self.document, self.index))
 
     def __eq__(self, other: 'Page') -> bool:
         """Define how one Page is identical."""
         return self.__hash__() == other.__hash__()
 
     def __repr__(self):
         """Return the name of the Document incl. the ID."""
-        return f"Page {self.index} in {self.document}"
+        return f'Page {self.index} in {self.document}'
+
+    def get_image(self, update: bool = False) -> Image.Image:
+        """
+        Get Page as a Pillow Image object.
+
+        The Page image is loaded from a PNG file at `Page.image_path`.
+        If the file is not present, or if `update` is True, it will be downloaded from the Konfuzio Host.
+        Alternatively, if you don't want to use a file, you can provide the image as bytes to `Page.image_bytes`. Then
+        call this method to convert the bytes into a Pillow Image.
+        In every case, the return value of this method and the attribute `Page.image` will be a Pillow Image.
+
+        :param update: Whether to force download the Page PNG file.
+        :return: A Pillow Image object for this Page's image.
+        """
+        if not self.image or update:
+            page_id = self.id_ if self.id_ else self.copy_of_id
+            if self.image_bytes:
+                try:
+                    self.image = Image.open(io.BytesIO(self.image_bytes))
+                except ValueError:
+                    self.image = Image.open(io.BytesIO(self.image_bytes)).convert('RGB')
+            elif is_file(self.image_path, raise_exception=False) and not update:
+                self.image = Image.open(self.image_path)
+            elif (not is_file(self.image_path, raise_exception=False) or update) and page_id:
+                document_id = self.document.id_ if self.document.id_ else self.document.copy_of_id
+                png_content = get_page_image(
+                    document_id=document_id, page_number=self.number, session=self.document.project.session
+                )
+                with open(self.image_path, 'wb') as f:
+                    f.write(png_content)
+                    self.image = Image.open(io.BytesIO(png_content))
 
-    def get_image(self, update: bool = False):
-        """Get Document Page as PNG."""
-        if self.document.status[0] == 2 and (not is_file(self.image_path, raise_exception=False) or update):
-            png_content = get_page_image(self.id_)
-            with open(self.image_path, "wb") as f:
-                f.write(png_content)
-                self.image = Image.open(io.BytesIO(png_content))
-        elif is_file(self.image_path, raise_exception=False):
-            self.image = Image.open(self.image_path)
         return self.image
 
-    def get_annotations_image(self, image: Image = None):
-        """Get Document Page as PNG with annotations shown."""
-        if image is None and self.document.id_ is not None:
-            image = self.get_image()
-        elif image is None and self.document.copy_of_id is not None:
-            original_doc = self.document.project.get_document_by_id(self.document.copy_of_id)
-            image = original_doc.get_page_by_index(self.index).get_image()
+    def get_annotations_image(self, display_all: bool = False) -> Image:
+        """Get Document Page as PNG with Annotations shown."""
+        image = self.get_image()
         image = image.convert('RGB')
-        # bbox information are based on a downscaled image
-        scale_mult = image.size[1] / self.height
 
-        anns = self.view_annotations()
+        draw = ImageDraw.Draw(image)
 
-        for ann in anns:
-            pos = [
-                scale_mult * ann.spans[0].bbox().x0,
-                scale_mult * (self.height - ann.spans[0].bbox().y0),
-                scale_mult * ann.spans[0].bbox().x1,
-                scale_mult * (self.height - ann.spans[0].bbox().y1),
-            ]
-            draw = ImageDraw.Draw(image)
-            draw.rectangle(pos, outline='blue', width=2)
+        try:
+            # We try to get a ttf font to be able to change bounding box label text size
+            font = ImageFont.truetype(
+                '/usr/share/fonts/truetype/liberation/LiberationSerif-Bold.ttf', 24, encoding='unic'
+            )
+        except OSError:
+            logger.warning('Font not found. Loading default.')
+            font = ImageFont.load_default()
 
-            try:
-                font = ImageFont.truetype(
-                    "/usr/share/fonts/truetype/liberation/LiberationSerif-Bold.ttf", 24, encoding="unic"
+        if not display_all:
+            annotations = self.view_annotations()
+        else:
+            annotations = self.annotations(use_correct=False)
+        for annotation in annotations:
+            annotation_image_bbox = (
+                annotation.bbox().x0_image,
+                annotation.bbox().y0_image,
+                annotation.bbox().x1_image,
+                annotation.bbox().y1_image,
+            )
+            draw.rectangle(annotation_image_bbox, outline='blue', width=2)
+            draw.text(
+                (annotation_image_bbox[0], annotation_image_bbox[1] - 24), annotation.label.name, fill='blue', font=font
+            )
+            for span in annotation.spans:
+                span_image_bbox = (
+                    span.bbox().x0_image,
+                    span.bbox().y0_image,
+                    span.bbox().x1_image,
+                    span.bbox().y1_image,
                 )
-            except OSError:
-                logger.warning('Font not found. Loading default.')
-                font = ImageFont.load_default()
+                draw.rectangle(span_image_bbox, outline='green', width=1)
 
-            draw.text((pos[0], pos[3] - 24), ann.label.name, fill='blue', font=font)
         return image
 
     @property
     def text(self):
         """Get Document text corresponding to the Page."""
         doc_text = self.document.text
         page_text = self.document.text[self.start_offset : self.end_offset]
@@ -208,18 +302,59 @@
         for annotation in annotations:
             for span in annotation.spans:
                 if span not in spans:
                     spans.append(span)
 
         return sorted(spans)
 
+    def lines(self) -> List['Span']:
+        """Return sorted list of Spans for each line in the Page."""
+        lines_spans = []
+        char_bboxes = self.get_bbox().values()
+        char_bboxes = sorted(char_bboxes, key=lambda x: x['char_index'])
+
+        # iterate over each line_number and all the character bboxes with that line number
+
+        # condition for backward compatibility that checks if bbox file structure includes 'line_number' or
+        # 'line_index' and parses the file accordingly.
+        if 'line_number' in [bbox.keys() for bbox in char_bboxes][0]:
+            for _, line_char_bboxes in itertools.groupby(char_bboxes, lambda x: x['line_number']):
+                # (a line should never start with a space char)
+                trimmed_line_char_bboxes = [char for char in line_char_bboxes if not char['text'].isspace()]
+
+                if len(trimmed_line_char_bboxes) == 0:
+                    continue
+
+                # create Span from the line characters bboxes
+                start_offset = min((char_bbox['char_index'] for char_bbox in trimmed_line_char_bboxes))
+                end_offset = max((char_bbox['char_index'] for char_bbox in trimmed_line_char_bboxes)) + 1
+                span = Span(start_offset=start_offset, end_offset=end_offset, document=self.document)
+
+                lines_spans.append(span)
+        elif 'line_index' in [bbox.keys() for bbox in char_bboxes][0]:
+            # line index is always less than line_index by 1, e.g. if line_index is 0, line_number is 1
+            for _, line_char_bboxes in itertools.groupby(char_bboxes, lambda x: x['line_index'] + 1):
+                # (a line should never start with a space char)
+                trimmed_line_char_bboxes = [char for char in line_char_bboxes if not char['text'].isspace()]
+
+                if len(trimmed_line_char_bboxes) == 0:
+                    continue
+
+                # create Span from the line characters bboxes
+                start_offset = min((char_bbox['char_index'] for char_bbox in trimmed_line_char_bboxes))
+                end_offset = max((char_bbox['char_index'] for char_bbox in trimmed_line_char_bboxes)) + 1
+                span = Span(start_offset=start_offset, end_offset=end_offset, document=self.document)
+
+                lines_spans.append(span)
+
+        return lines_spans
+
     def get_bbox(self):
         """Get bbox information per character of Page."""
-        doc_bbox = self.document.get_bbox()
-        page_bbox = {k: doc_bbox[k] for k in doc_bbox.keys() if doc_bbox[k]["page_number"] == self.number}
+        page_bbox = self.document.get_bbox_by_page(self.index)
         return page_bbox
 
     def annotations(
         self,
         label: 'Label' = None,
         use_correct: bool = True,
         ignore_below_threshold: bool = False,
@@ -244,100 +379,331 @@
         return page_annotations
 
     def view_annotations(self) -> List['Annotation']:
         """Get the best Annotations, where the Spans are not overlapping in Page."""
         page_view_anns = self.document.view_annotations(start_offset=self.start_offset, end_offset=self.end_offset)
         return page_view_anns
 
+    def add_category_annotation(self, category_annotation: 'CategoryAnnotation'):
+        """Annotate a Page with a Category and confidence information."""
+        if category_annotation.category != self.document.project.no_category:
+            duplicated = [x for x in self.category_annotations if x == category_annotation]
+            if duplicated:
+                raise ValueError(
+                    f'In {self} the {category_annotation} is a duplicate of {duplicated} and will not be added.'
+                )
+            self.category_annotations.append(category_annotation)
+
+    def get_category_annotation(self, category, add_if_not_present: bool = False) -> 'CategoryAnnotation':
+        """
+        Retrieve the Category Annotation associated with a specific Category within this Page.
+
+        If no Category Annotation is found for the provided Category, one can be created based on the
+        `add_if_not_present` argument.
+
+        :param category: The Category for which to retrieve the Category Annotation.
+        :type category: Category
+        :param add_if_not_present: If True, a Category Annotation will be added to the current Page if none is found. If
+                                False, a dummy Category Annotation will be created, not linked to any Document or Page.
+        :type add_if_not_present: bool
+
+        :return: The located or newly created Category Annotation.
+        :rtype: CategoryAnnotation
+        """
+        filtered_category_annotations = [
+            category_annotation
+            for category_annotation in self.category_annotations
+            if category_annotation.category == category
+            and category_annotation.category != self.document.project.no_category
+        ]
+        # if the list is not empty it means there is exactly one CategoryAnnotation with the assigned Category
+        # (see Page.add_category_annotation for duplicate checking)
+        if filtered_category_annotations:
+            return filtered_category_annotations[0]
+        else:  # otherwise a new one will be created
+            if add_if_not_present:
+                new_category_annotation = CategoryAnnotation(category=category, page=self)
+            else:
+                # dummy CategoryAnnotation (not associated to any Document or Page)
+                new_category_annotation = CategoryAnnotation(category=category)
+            return new_category_annotation
+
+    def set_category(self, category: 'Category') -> None:
+        """
+        Set the Category of the Page.
+
+        :param category: The Category to set for the Page.
+        """
+        if not category:
+            raise ValueError("We forbid setting a Page's Category to None.")
+        logger.info(f'Setting {self} Category to {category}.')
+        self._category = category
+        if category is self.document.project.no_category:
+            self.category_annotations = []
+            self._human_chosen_category_annotation = None
+            return
+        category_annotation = self.get_category_annotation(category, add_if_not_present=True)
+        self._human_chosen_category_annotation = category_annotation
+
+    @property
+    def maximum_confidence_category_annotation(self) -> Optional['CategoryAnnotation']:
+        """
+        Get the human revised Category Annotation of this Page, or the highest confidence one if not revised.
+
+        :return: The found Category Annotation, or None if not present.
+        """
+        if (
+            self._human_chosen_category_annotation is not None
+            and self._human_chosen_category_annotation.category != self.document.project.no_category
+        ):
+            return self._human_chosen_category_annotation
+        elif self.category_annotations:
+            # return the highest confidence CategoryAnnotation if no human revised it
+            return sorted(self.category_annotations, key=lambda x: x.confidence)[-1]
+        else:
+            return None
+
+    @property
+    def category(self) -> Optional['Category']:
+        """Get the Category of the Page, based on human revised Category Annotation, or on highest confidence."""
+        if self.maximum_confidence_category_annotation is not None:
+            return self.maximum_confidence_category_annotation.category
+        else:
+            return self._category
+
+    def get_original_page(self) -> 'Page':
+        """
+        Return an "original" Page in case the current Page is a copy without an ID.
+
+        An "original" Page is a Page from the Document that is not a copy and not a Virtual Document. This Page has an
+        ID.
+
+        The method is used in the File Splitting pipeline to retain the original Document's information in
+        the Sub-Documents that were created from its splitting. The original Document is a Document that has an ID and
+        is not a deepcopy.
+        """
+        if self.id_ and self.document.id_:
+            return self
+        elif self.copy_of_id:
+            if self.document.id_:
+                return self.document.get_page_by_id(self.copy_of_id)
+            else:
+                return self.document.project.get_document_by_id(self.document.copy_of_id).get_page_by_id(
+                    self.copy_of_id
+                )
+
+    def annotation_sets(self) -> List['AnnotationSet']:
+        """Show all Annotation Sets related to Annotations of the Page."""
+        page_annotations = self.annotations()
+        return list({annotation.annotation_set for annotation in page_annotations})
+
+
+class BboxValidationTypes(Enum):
+    """
+    Define validation strictness for Bounding Boxes.
+
+    For more details see the `Bbox` class.
+    """
+
+    STRICT = 'strict'
+    ALLOW_ZERO_SIZE = 'allow zero size'
+    DISABLED = 'disabled'
+
 
 class Bbox:
     """
     A bounding box relates to an area of a Document Page.
 
-    :param strict_validation: If False, it allows bounding boxes to have zero width or height. This option is available
-    and defaults to False for compatibility reasons since some OCR engines can sometimes return character level bboxes
-    with zero width or height.
+    For more details see https://dev.konfuzio.com/sdk/explanations.html#bbox-concept
+
+    What consistutes a valid Bbox changes depending on the value of the `validation` param.
+    If ALLOW_ZERO_SIZE (default), it allows bounding boxes to have zero width or height.
+    This option is available for compatibility reasons since some OCR engines can sometimes return character level
+    bboxes with zero width or height. If STRICT, it doesn't allow zero size bboxes. If DISABLED, it allows bboxes that
+    have negative size, or coordinates beyond the Page bounds.
+    For the default behaviour see https://dev.konfuzio.com/sdk/tutorials/data_validation/index.html
+
+    :param validation: One of ALLOW_ZERO_SIZE (default), STRICT, or DISABLED.
     """
 
-    def __init__(self, x0: int, x1: int, y0: int, y1: int, page: Page, strict_validation: bool = False):
+    def __init__(self, x0: int, x1: int, y0: int, y1: int, page: Page, validation=BboxValidationTypes.ALLOW_ZERO_SIZE):
         """Store information and validate."""
         self.x0: int = x0
         self.x1: int = x1
         self.y0: int = y0
         self.y1: int = y1
         self.angle: float = 0.0  # not yet used
         self.page: Page = page
-        self._valid(strict_validation)
+        self._label_name: Optional[str] = None  # used in detectron tokenizer
+        self._valid(validation)
+
+    @property
+    def document(self) -> 'Document':
+        """Get the Document the Bbox belongs to."""
+        return self.page.document
+
+    @property
+    def top(self):
+        """Calculate the distance to the top of the Page."""
+        if self.page:
+            return round(self.page.height - self.y1, 3)
 
     def __repr__(self):
         """Represent the Box."""
-        return f'{self.__class__.__name__}: {self.x0} {self.x1} {self.y0} {self.y1} on Page {self.page}'
+        return f'{self.__class__.__name__}: x0: {self.x0} x1: {self.x1} y0: {self.y0} y1: {self.y1} on Page {self.page}'
 
     def __hash__(self):
         """Return identical value for a Bounding Box."""
-        return (self.x0, self.x1, self.y0, self.y1, self.page)
+        return hash((self.x0, self.x1, self.y0, self.y1, self.page))
 
     def __eq__(self, other: 'Bbox') -> bool:
         """Define that one Bounding Box on the same page is identical."""
         return self.__hash__() == other.__hash__()
 
-    def _valid(self, strict: bool = False):
+    def _valid(self, validation=BboxValidationTypes.ALLOW_ZERO_SIZE, handler='sdk_validation'):
         """
-        Validate contained data.
+        Validate the coordinates of the Bounding Box contained in the Bbox, raising a ValueError exception in case.
 
-        :param strict: If False, it allows bounding boxes to have zero width or height. This option is available
-        and defaults to False for compatibility reasons since some OCR engines can sometimes return character level
-        bboxes with zero width or height.
+        :param validation: One of ALLOW_ZERO_SIZE (default), STRICT, or DISABLED. Also see the `Bbox` class.
         """
-        if self.x0 == self.x1:
-            if strict:
-                raise ValueError(f'{self} has no width in {self.page}.')
-            else:
-                # todo add link to documentation page relating to feature calculation for the RandomForest ExtractionAI
-                logger.error(
-                    f'{self} has no width in {self.page}. Some of our AIs use the area of bboxes as a feature'
-                    f'during training and prediction, which will be zero.'
-                )
+        round_decimals = 2
 
-        if self.x0 > self.x1:
-            raise ValueError(f'{self} has negative width in {self.page}.')
+        if round(self.x0, round_decimals) == round(self.x1, round_decimals):
+            logger.warning(f'{self} has no width in {self.page}.')
 
-        if self.y0 == self.y1:
-            if strict:
-                raise ValueError(f'{self} has no height in {self.page}.')
-            else:
-                # todo add link to documentation page relating to feature calculation for the RandomForest ExtractionAI
-                logger.error(
-                    f'{self} has no height in {self.page}. Some of our AIs use the area of bboxes as a feature'
-                    f'during training and prediction, which will be zero.'
-                )
+        if round(self.x0, round_decimals) > round(self.x1, round_decimals):
+            exception_or_log_error(
+                msg=f'{self} has negative width in {self.page}.',
+                fail_loudly=str(validation) != str(BboxValidationTypes.DISABLED),
+                exception_type=ValueError,
+                handler=handler,
+            )
+
+        if round(self.y0, round_decimals) == round(self.y1, round_decimals):
+            logger.warning(f'{self} has no height in {self.page}.')
 
-        if self.y0 > self.y1:
-            raise ValueError(f'{self} has negative height in {self.page}.')
+        if round(self.y0, round_decimals) > round(self.y1, round_decimals):
+            exception_or_log_error(
+                msg=f'{self} has negative height in {self.page}.',
+                fail_loudly=str(validation) != str(BboxValidationTypes.DISABLED),
+                exception_type=ValueError,
+                handler=handler,
+            )
 
-        if self.y1 > self.page.height:
-            raise ValueError(f'{self} exceeds height of {self.page}.')
+        if round(self.y1, round_decimals) > round(self.page.height, round_decimals):
+            exception_or_log_error(
+                msg=f'{self} exceeds height of {self.page} by '
+                f'{round(self.y1, round_decimals) - round(self.page.height, round_decimals)} '
+                f'with validation {validation}.',
+                fail_loudly=str(validation) != str(BboxValidationTypes.DISABLED),
+                exception_type=ValueError,
+                handler=handler,
+            )
 
-        if self.x1 > self.page.width:
-            raise ValueError(f'{self} exceeds width of {self.page}.')
+        if round(self.x1, round_decimals) > round(self.page.width, round_decimals):
+            exception_or_log_error(
+                msg=f'{self} exceeds width of {self.page} by '
+                f'{round(self.x1, round_decimals) - round(self.page.width, round_decimals)} '
+                f'with validation {validation}.',
+                fail_loudly=str(validation) != str(BboxValidationTypes.DISABLED),
+                exception_type=ValueError,
+                handler=handler,
+            )
+
+        if round(self.y0, round_decimals) < 0:
+            exception_or_log_error(
+                msg=f'{self} has negative y coordinate in {self.page}.',
+                fail_loudly=str(validation) != str(BboxValidationTypes.DISABLED),
+                exception_type=ValueError,
+                handler=handler,
+            )
 
-        if self.y0 < 0:
-            raise ValueError(f'{self} has negative y coordinate in {self.page}.')
+        if round(self.x0, round_decimals) < 0:
+            exception_or_log_error(
+                msg=f'{self} has negative x coordinate in {self.page}.',
+                fail_loudly=str(validation) != str(BboxValidationTypes.DISABLED),
+                exception_type=ValueError,
+                handler=handler,
+            )
 
-        if self.x0 < 0:
-            raise ValueError(f'{self} has negative x coordinate in {self.page}.')
+    def check_overlap(self, bbox: Union['Bbox', Dict]) -> bool:
+        """Verify if there's overlap between two Bboxes."""
+        if isinstance(bbox, dict) and (
+            bbox['x0'] <= self.x1 and bbox['x1'] >= self.x0 and bbox['y0'] <= self.y1 and bbox['y1'] >= self.y0
+        ):
+            return True
+        elif type(bbox) is type(self) and (
+            bbox.x0 <= self.x1 and bbox.x1 >= self.x0 and bbox.y0 <= self.y1 and bbox.y1 >= self.y0
+        ):
+            return True
+        else:
+            return False
 
     @property
     def area(self):
         """Return area covered by the Bbox."""
         return round(abs(self.x0 - self.x1) * abs(self.y0 - self.y1), 3)
 
+    @classmethod
+    def from_image_size(cls, x0, x1, y0, y1, page: Page) -> 'Bbox':
+        """
+        Create a Bbox from image dimensions, based on the scaling of character Bboxes within the Document.
+
+        This method computes the coordinates of the bottom-left and top-right corners in
+        a coordinate system where the y-axis is oriented from bottom to top, the x-axis is from left to right,
+        and the scale is based on the page.
+
+        :param x0: The x-coordinate of the top-left corner in an image-scaled system.
+        :param x1: The x-coordinate of the bottom-right corner in an image-scaled system.
+        :param y0: The y-coordinate of the top-left corner in an image-scaled system.
+        :param y1: The y-coordinate of the bottom-right corner in an image-scaled system.
+        :param page: The Page object for reference in scaling.
+
+        :return: A Bbox object with rescaled dimensions.
+        """
+        factor_y = page.height / page.image_height
+        factor_x = page.width / page.image_width
+        image_height = page.image_height
+
+        temp_y0 = (image_height - y0) * factor_y
+        temp_y1 = (image_height - y1) * factor_y
+        y0 = temp_y1
+        y1 = temp_y0
+        x0 = x0 * factor_x
+        x1 = x1 * factor_x
+
+        return cls(x0=x0, x1=x1, y0=y0, y1=y1, page=page)
+
+    @property
+    def x0_image(self):
+        """Get the x0 coordinate in the context of the Page image."""
+        return self.x0 * (self.page.image_width / self.page.width)
+
+    @property
+    def x1_image(self):
+        """Get the x1 coordinate in the context of the Page image."""
+        return self.x1 * (self.page.image_width / self.page.width)
+
+    @property
+    def y0_image(self):
+        """Get the y0 coordinate in the context of the Page image, in a top-down coordinate system."""
+        return self.page.image_height - self.y1 * (self.page.image_height / self.page.height)
+
+    @property
+    def y1_image(self):
+        """Get the y1 coordinate in the context of the Page image, in a top-down coordinate system."""
+        return self.page.image_height - self.y0 * (self.page.image_height / self.page.height)
+
 
 class AnnotationSet(Data):
-    """An Annotation Set is a group of Annotations. The Labels of those Annotations refer to the same Label Set."""
+    """
+    An Annotation Set is a group of Annotations. The Labels of those Annotations refer to the same Label Set.
+
+    For more details see https://dev.konfuzio.com/sdk/explanations.html#annotation-set-concept
+    """
 
     def __init__(self, document, label_set: 'LabelSet', id_: Union[int, None] = None, **kwargs):
         """
         Create an Annotation Set.
 
         :param id: ID of the Annotation Set
         :param document: Document where the Annotation Set belongs
@@ -350,50 +716,83 @@
         self.document: Document = document  # we don't add it to the Document as it's added via get_annotations
         self._force_offline = document._force_offline
         self._annotations = []
         document.add_annotation_set(self)
 
     def __repr__(self):
         """Return string representation of the Annotation Set."""
-        return f"{self.__class__.__name__}({self.id_}) of {self.label_set} in {self.document}."
+        return f'{self.__class__.__name__}({self.id_}) of {self.label_set} in {self.document}.'
+
+    def __lt__(self, other: 'AnnotationSet'):
+        """Sort AnnotationSets by their first Annotation."""
+        self_annotations = self.annotations(use_correct=False, ignore_below_threshold=True)
+        other_annotations = other.annotations(use_correct=False, ignore_below_threshold=True)
+        return self_annotations[0] < other_annotations[0]
 
     def annotations(self, use_correct: bool = True, ignore_below_threshold: bool = False):
         """All Annotations currently in this Annotation Set."""
         if not self._annotations:
             for annotation in self.document.annotations(use_correct=False, ignore_below_threshold=False):
                 if annotation.annotation_set == self:
                     self._annotations.append(annotation)
 
         annotations: List[Annotation] = []
         if use_correct:
             annotations = [ann for ann in self._annotations if ann.is_correct]
         elif ignore_below_threshold:
-            annotations = [ann for ann in self._annotations if ann.is_correct or ann.confidence >= ann.label.threshold]
+            annotations = [
+                ann
+                for ann in self._annotations
+                if ann.is_correct or (ann.confidence and ann.confidence >= ann.label.threshold)
+            ]
         else:
             annotations = self._annotations
         return annotations
 
     @property
-    def start_offset(self):
-        """Calculate the earliest start based on all Annotations currently in this Annotation Set."""
-        return min((s.start_offset for a in self.annotations() for s in a.spans), default=None)
+    def is_default(self) -> bool:
+        """Check if AnnotationSet is the default AnnotationSet of the Document."""
+        return self.label_set.is_default
 
     @property
-    def start_line_index(self):
+    def start_offset(self) -> Optional[int]:
+        """Calculate the earliest start based on all Annotations above detection threshold in this AnnotationSet."""
+        return min(
+            (s.start_offset for a in self.annotations(use_correct=False, ignore_below_threshold=True) for s in a.spans),
+            default=None,
+        )
+
+    @property
+    def start_line_index(self) -> Optional[int]:
         """Calculate starting line of this Annotation Set."""
+        if self.start_offset is None:
+            return None
         return self.document.text[0 : self.start_offset].count('\n')
 
     @property
-    def end_offset(self):
-        """Calculate the end based on all Annotations currently in this Annotation Set."""
-        return max((a.end_offset for a in self.annotations()), default=None)
+    def end_offset(self) -> Optional[int]:
+        """Calculate the end based on all Annotations above detection threshold currently in this AnnotationSet."""
+        return max(
+            (a.end_offset for a in self.annotations(use_correct=False, ignore_below_threshold=True)), default=None
+        )
+
+    @property
+    def end_line_index(self) -> Optional[int]:
+        """Calculate ending line of this Annotation Set."""
+        if self.end_offset is None:
+            return None
+        return self.document.text[0 : self.end_offset].count('\n')
 
 
 class LabelSet(Data):
-    """A Label Set is a group of labels."""
+    """
+    A Label Set is a group of Labels.
+
+    For more details see https://dev.konfuzio.com/sdk/explanations.html#label-set-concept
+    """
 
     def __init__(
         self,
         project,
         labels=None,
         id_: int = None,
         name: str = None,
@@ -421,60 +820,65 @@
             labels = []
         self.id_local = next(Data.id_iter)
         self.id_ = id_
         self.name = name
         self.name_clean = name_clean
         self.is_default = is_default
 
-        if not categories and "default_label_sets" in kwargs:
-            self._default_of_label_set_ids = kwargs["default_label_sets"]
+        if not categories and 'default_label_sets' in kwargs:
+            self._default_of_label_set_ids = kwargs['default_label_sets']
+            self.categories = []
+        elif not categories and 'default_section_labels' in kwargs:
+            self._default_of_label_set_ids = kwargs['default_section_labels']
             self.categories = []
-        elif not categories and "default_section_labels" in kwargs:
-            self._default_of_label_set_ids = kwargs["default_section_labels"]
+        elif isinstance(categories, list) and all(isinstance(category, dict) for category in categories):
+            self._default_of_label_set_ids = [category['id'] for category in categories]
             self.categories = []
         else:
             self._default_of_label_set_ids = []
             self.categories = categories
 
         self.has_multiple_annotation_sets = has_multiple_annotation_sets
 
-        if "has_multiple_sections" in kwargs:
-            self.has_multiple_annotation_sets = kwargs["has_multiple_sections"]
+        if 'has_multiple_sections' in kwargs:
+            self.has_multiple_annotation_sets = kwargs['has_multiple_sections']
 
         self.project: Project = project
         self._force_offline = project._force_offline
         self.labels: List[Label] = []
 
         # todo allow to create Labels either on Project or Label Set level, so they are (not) shared among Label Sets.
         for label in labels:
             if isinstance(label, int):
                 label = self.project.get_label_by_id(id_=label)
             self.add_label(label)
 
-        project.add_label_set(self)
+        if self not in project._label_sets:
+            project.add_label_set(self)
         for category in self.categories:
-            category.add_label_set(self)
+            if self not in category.label_sets:
+                category.add_label_set(self)
 
     def __lt__(self, other: 'LabelSet'):
         """Sort Label Sets by name."""
         try:
             return self.name < other.name
         except TypeError:
             logger.error(f'Cannot sort {self} and {other}.')
             return False
 
     def __repr__(self):
         """Return string representation of the Label Set."""
-        return f"{self.name} ({self.id_})"
+        return f'LabelSet: {self.name} ({self.id_})'
 
     def add_category(self, category: 'Category'):
         """
-        Add Category to Project, if it does not exist.
+        Add Category to the Label Set, if it does not exist.
 
-        :param category: Category to add in the Project
+        :param category: Category to add to the Label Set
         """
         if category not in self.categories:
             self.categories.append(category)
         else:
             raise ValueError(f'In {self} the {category} is a duplicate and will not be added.')
 
     def add_label(self, label):
@@ -498,44 +902,46 @@
                 targets.append(self.name + '__' + label.name)
             else:
                 targets.append(label.name)
         return targets
 
 
 class Category(Data):
-    """Group Documents in a Project."""
+    """
+    Group Documents in a Project.
+
+    For more details see https://dev.konfuzio.com/sdk/explanations.html#category-concept
+    """
 
     def __init__(self, project, id_: int = None, name: str = None, name_clean: str = None, *args, **kwargs):
         """Associate Label Sets to relate to Annotations."""
         self.id_local = next(Data.id_iter)
         self.id_ = id_
         self.name = name
         self.name_clean = name_clean
         self.project: Project = project
         self._force_offline = project._force_offline
         self.label_sets: List[LabelSet] = []
         self.project.add_category(category=self)
+        self._exclusive_first_page_strings = None
+        self._exclusive_span_tokenizer = None
 
     @property
     def labels(self):
-        """Return the Labels that belong to the Category and it's Label Sets."""
-        labels = []
-        # for label in self.project.labels:
-        #     if self in label.label_sets:
-        #         labels.append(label)
+        """Return the Labels that belong to the Category and its Label Sets."""
+        labels = set()
         for label_set in self.label_sets:
-            labels += label_set.labels
-
-        return list(set(labels))
+            labels.update(label_set.labels)
+        return list(labels)
 
     @property
     def fallback_name(self) -> str:
-        """Turn the category name to lowercase, remove parentheses along with their contents, and trim spaces."""
+        """Turn the Category name to lowercase, remove parentheses along with their contents, and trim spaces."""
         parentheses_removed = re.sub(r'\([^)]*\)', '', self.name.lower()).strip()
-        single_spaces = parentheses_removed.replace("  ", " ")
+        single_spaces = parentheses_removed.replace('  ', ' ')
         return single_spaces
 
     def documents(self):
         """Filter for Documents of this Category."""
         return [x for x in self.project.documents if x.category == self]
 
     def test_documents(self):
@@ -545,33 +951,184 @@
     def add_label_set(self, label_set):
         """Add Label Set to Category."""
         if label_set not in self.label_sets:
             self.label_sets.append(label_set)
         else:
             raise ValueError(f'In {self} the {label_set} is a duplicate and will not be added.')
 
+    @property
+    def default_label_set(self):
+        """Get the default Label Set of the Category."""
+        # Search for existing default LabelSet
+        default_label_set = next((label_set for label_set in self.label_sets if label_set.is_default), None)
+        # If not found, create a new default LabelSet
+        if not default_label_set:
+            default_label_set = LabelSet(
+                id_=self.id_,
+                project=self.project,
+                name=self.name,
+                name_clean=self.name_clean,
+                is_default=True,
+                categories=[self],
+                has_multiple_annotation_sets=False,
+            )
+        return default_label_set
+
+    def _collect_exclusive_first_page_strings(self, tokenizer):
+        """
+        Collect exclusive first-page string across the Documents within the Category.
+
+        :param tokenizer: A tokenizer to re-tokenize Documents within the Category before gathering the strings.
+        """
+        cur_first_page_strings = []
+        cur_non_first_page_strings = []
+        for doc in self.documents():
+            doc = deepcopy(doc)
+            doc = tokenizer.tokenize(doc)
+            for page in doc.pages():
+                if page.number == 1:
+                    cur_first_page_strings.append({span.offset_string for span in page.spans()})
+                else:
+                    cur_non_first_page_strings.append({span.offset_string for span in page.spans()})
+            doc.delete()
+        if cur_first_page_strings:
+            true_first_page_strings = set.intersection(*cur_first_page_strings)
+        else:
+            true_first_page_strings = set()
+        if cur_non_first_page_strings:
+            true_not_first_page_strings = set.intersection(*cur_non_first_page_strings)
+        else:
+            true_not_first_page_strings = set()
+        true_first_page_strings = true_first_page_strings - true_not_first_page_strings
+        self._exclusive_first_page_strings = true_first_page_strings
+
+    def exclusive_first_page_strings(self, tokenizer) -> set:
+        """
+        Return a set of strings exclusive for first Pages of Documents within the Category.
+
+        :param tokenizer: A tokenizer to process Documents before gathering strings.
+        """
+        if self._exclusive_span_tokenizer is not None:
+            if tokenizer != self._exclusive_span_tokenizer:
+                logger.warning(
+                    'Assigned tokenizer does not correspond to the one previously used within this instance.'
+                    'All previously found exclusive first-page strings within each Category will be removed '
+                    'and replaced with the newly generated ones.'
+                )
+                self._collect_exclusive_first_page_strings(tokenizer)
+        if not self._exclusive_first_page_strings:
+            self._collect_exclusive_first_page_strings(tokenizer)
+        return self._exclusive_first_page_strings
+
     def __lt__(self, other: 'Category'):
         """Sort Categories by name."""
         try:
             return self.name < other.name
         except TypeError:
             logger.error(f'Cannot sort {self} and {other}.')
             return False
 
     def __repr__(self):
         """Return string representation of the Category."""
-        return f"{self.name} ({self.id_})"
+        return f'Category: {self.name} ({self.id_})'
+
+
+class CategoryAnnotation(Data):
+    """
+    Annotate the Category of a Page.
+
+    For more details see https://dev.konfuzio.com/sdk/explanations.html#category-annotation-concept
+    """
+
+    def __init__(
+        self,
+        category: Category,
+        confidence: Optional[float] = None,
+        page: Optional[Page] = None,
+        document: Optional['Document'] = None,
+        id_: Optional[int] = None,
+    ):
+        """
+        Create a CategoryAnnotation and link it to a Document or to a specific Page in a Document.
+
+        :param id_: ID of the CategoryAnnotation.
+        :param category: The Category to annotate the Page with.
+        :param page: The Page to be annotated. Only use when not providing a Document.
+        :param document: The Document to be annotated. Only use when not providing a Page.
+        :param confidence: Predicted confidence of the CategoryAnnotation.
+        """
+        self.id_local = next(Data.id_iter)
+        self.id_ = id_
+        self.category = category
+        self.page = page
+        self.document = document
+        if page is not None:
+            if (document is not None) and (page.document != document):
+                raise ValueError(
+                    f'The provided {page} comes from {page.document} but the provided {document} does not correspond. '
+                    f'You can provide just the Document argument if this CategoryAnnotation is not linked to a Page, '
+                    f'otherwise only provide the Page argument; the corresponding Document will be found automatically.'
+                )
+            self.document = self.page.document
+        self._confidence = confidence
+        # Call add_category_annotation to Page at the end, so all attributes for duplicate checking are available.
+        if self.page is not None:
+            self.page.add_category_annotation(self)
+
+    def __repr__(self):
+        """Return string representation."""
+        return f'Category Annotation: ({self.category}, {self.confidence}) in {self.page or self.document}'
+
+    def __eq__(self, other):
+        """Define equality condition for CategoryAnnotations.
+
+        A CategoryAnnotation is equal to another if both the linked Page and the predicted Category are the same.
+        """
+        return (other is not None) and (self.page == other.page) and (self.category == other.category)
+
+    def set_revised(self) -> None:
+        """Set this Category Annotation as revised by human, and thus the correct one for the linked Page."""
+        if self.page is not None:
+            self.page.set_category(self.category)
+        elif self.document is not None:
+            self.document.set_category(self.category)
+
+    @property
+    def confidence(self) -> float:
+        """
+        Get the confidence of this Category Annotation.
+
+        If the confidence was not set, it means it was never predicted by an AI. Thus, the returned value will
+        be 0, unless it was set by a human, in which case it defaults to 1.
+
+        :return: Confidence between 0.0 and 1.0 included.
+        """
+        # if confidence is None it means it was never predicted by an AI
+        if self._confidence is None:
+            # if this CategoryAnnotation was added by a human then the confidence is 1
+            if (self.page is not None) and (self.page._human_chosen_category_annotation == self):
+                return 1.0
+            elif (self.document is not None) and (self.document._category == self.category):
+                return 1.0
+            else:
+                # otherwise there is no prediction and no human revision so the confidence is 0
+                return 0.0
+        return self._confidence
 
 
 class Label(Data):
-    """Group Annotations across Label Sets."""
+    """
+    Group Annotations across Label Sets.
+
+    For more details see https://dev.konfuzio.com/sdk/explanations.html#label-concept
+    """
 
     def __init__(
         self,
-        project,
+        project: 'Project',
         id_: Union[int, None] = None,
         text: str = None,
         get_data_type_display: str = 'Text',
         text_clean: str = None,
         description: str = None,
         label_sets=None,
         has_multiple_top_candidates: bool = False,
@@ -579,20 +1136,20 @@
         *initial_data,
         **kwargs,
     ):
         """
         Create a named Label.
 
         :param project: Project where the Label belongs
-        :param id_: ID of the label
-        :param text: Name of the label
-        :param get_data_type_display: Data type of the label
-        :param text_clean: Normalized name of the label
-        :param description: Description of the label
-        :param label_sets: Label sets that use this label
+        :param id_: ID of the Label
+        :param text: Name of the Label
+        :param get_data_type_display: Data type of the Label
+        :param text_clean: Normalized name of the Label
+        :param description: Description of the Label
+        :param label_sets: Label Sets that use this Label
         """
         self.id_local = next(Data.id_iter)
         self.id_ = id_
         self.name = text
         self.name_clean = text_clean
         self.data_type = get_data_type_display
         self.description = description
@@ -610,14 +1167,16 @@
         self._tokens = {}
         self.tokens_file_path = None
         self._regex = {}  # : List[str] = []
         # self._combined_tokens = None
         self.regex_file_path = os.path.join(self.project.regex_folder, f'{self.name_clean}.json5')
         self._evaluations = {}  # used to do the duplicate check on Annotation level
 
+        self._has_multiline_annotations = None
+
     def __repr__(self):
         """Return string representation."""
         return f'Label: {self.name}'
 
     def __lt__(self, other: 'Label'):
         """Sort Spans by start offset."""
         try:
@@ -639,51 +1198,67 @@
                     annotations.append(annotation)
 
         if not annotations:
             logger.warning(f'{self} has no correct annotations.')
 
         return annotations
 
-    def has_multiline_annotations(self, categories: List[Category]) -> bool:
+    def spans(self, categories: List[Category], use_correct=True, ignore_below_threshold=False) -> List['Span']:
+        """Return all Spans belonging to an Annotation of this Label."""
+        annotations = self.annotations(
+            categories=categories, use_correct=use_correct, ignore_below_threshold=ignore_below_threshold
+        )
+        spans = [span for annotation in annotations for span in annotation.spans]
+        return spans
+
+    def has_multiline_annotations(self, categories: List[Category] = None) -> bool:
         """Return if any Label annotations are multi-line."""
-        for category in categories:
-            for document in category.documents():
-                for annotation in document.annotations(label=self):
-                    if len(annotation.spans) > 1:
-                        return True
-        return False
+        if categories is None and self._has_multiline_annotations is None:
+            raise TypeError(
+                "This value has never been computed. Please provide a value for keyword argument: 'categories'"
+            )
+        elif isinstance(categories, list):
+            self._has_multiline_annotations = False
+            for category in categories:
+                for document in category.documents():
+                    for annotation in document.annotations(label=self):
+                        if len(annotation.spans) > 1:
+                            self._has_multiline_annotations = True
+                            return True
 
-    def add_label_set(self, label_set: "LabelSet"):
+        return self._has_multiline_annotations
+
+    def add_label_set(self, label_set: 'LabelSet'):
         """
         Add Label Set to label, if it does not exist.
 
-        :param label_set: Label set to add
+        :param label_set: Label Set to add
         """
         if label_set not in self.label_sets:
             self.label_sets.append(label_set)
         else:
             raise ValueError(f'In {self} the {label_set} is a duplicate and will not be added.')
 
     def evaluate_regex(self, regex, category: Category, annotations: List['Annotation'] = None, regex_quality=0):
         """
         Evaluate a regex on Categories.
 
         Type of regex allows you to group regex by generality
 
         Example:
             Three Annotations about the birthdate in two Documents and one regex to be evaluated
-            1.doc: "My was born at the 12th of December 1980, you could also say 12.12.1980." (2 Annotations)
-            2.doc: "My was born at 12.06.1997." (1 Annotations)
+            1.doc: "My was born on the 12th of December 1980, you could also say 12.12.1980." (2 Annotations)
+            2.doc: "My was born on 12.06.1997." (1 Annotations)
             regex: dd.dd.dddd (without escaped characters for easier reading)
             stats:
-                  total_correct_findings: 2
-                  correct_label_annotations: 3
-                  total_findings: 2 --> precision 100 %
-                  num_docs_matched: 2
-                  Project.documents: 2  --> Document recall 100%
+            - total_correct_findings: 2
+            - correct_label_annotations: 3
+            - total_findings: 2 --> precision 100 %
+            - num_docs_matched: 2
+            - Project.documents: 2  --> Document recall 100%
 
         """
         evaluations = []
         documents = category.documents()
 
         for document in documents:
             # todo: potential time saver: make sure we did a duplicate check for the regex before we run the evaluation
@@ -698,28 +1273,33 @@
 
         try:
             annotation_precision = total_correct_findings / total_findings
         except ZeroDivisionError:
             annotation_precision = 0
 
         try:
-            annotation_recall = total_correct_findings / len(self.annotations(categories=[category]))
+            annotation_recall = total_correct_findings / len(self.spans(categories=[category]))
         except ZeroDivisionError:
             annotation_recall = 0
 
         try:
             document_recall = num_docs_matched / len(documents)
         except ZeroDivisionError:
             document_recall = 0
 
         try:
             f_score = 2 * (annotation_precision * annotation_recall) / (annotation_precision + annotation_recall)
         except ZeroDivisionError:
             f_score = 0
 
+        assert 0 <= annotation_precision <= 1
+        assert 0 <= annotation_recall <= 1
+        assert 0 <= document_recall <= 1
+        assert 0 <= f_score <= 1
+
         if documents:
             evaluation = {
                 'regex': regex,
                 'regex_len': len(regex),  # the longer the regex the more conservative it is to use
                 'runtime': sum(processing_times) / len(processing_times),  # time to process the regex
                 'annotation_recall': annotation_recall,
                 'annotation_precision': annotation_precision,
@@ -743,15 +1323,15 @@
             return {}
 
     def base_regex(self, category: 'Category', annotations: List['Annotation'] = None) -> str:
         """Find the best combination of regex in the list of all regex proposed by Annotations."""
         if category.id_ in self._tokens:
             return self._tokens[category.id_]
 
-        logger.info(f"Beginning base regex search for Label {self.name}.")
+        logger.info(f'Beginning base regex search for Label {self.name}.')
 
         if annotations is None:
             all_annotations = self.annotations(categories=[category])  # default is use_correct = True
         else:
             all_annotations = annotations
 
         evaluated_proposals = []
@@ -769,32 +1349,26 @@
 
         label_regex_token = merge_regex(best_proposals)
 
         self._tokens[category.id_] = label_regex_token
 
         return label_regex_token
 
-    def find_regex(self, category: 'Category', max_findings_per_page=100) -> List[str]:
-        """Find the best combination of regex for Label with before and after context."""
-        all_annotations = self.annotations(categories=[category])  # default is use_correct = True
-        if all_annotations == []:
-            logger.error(f"We cannot find annotations for Label {self} and Category {category}.")
-            return []
-
-        label_regex_token = self.base_regex(category=category, annotations=all_annotations)
-
+    def _find_regexes(
+        self, annotations, label_regex_token, category: 'Category', max_findings_per_page=100
+    ) -> List[str]:
+        """Find regexes for the Label."""
         search = [1, 3, 5]
         regex_to_remove_groupnames = re.compile(r'<.*?>')
         regex_to_remove_groupnames_full = re.compile(r'\?P<.*?>')
 
-        naive_proposal = label_regex_token
         regex_made = []
         regex_found = set()
 
-        for annotation in all_annotations:
+        for annotation in annotations:
             new_proposals = []
             annotation.document.spans(fill=True)
             for span in annotation.spans:
                 before_reg_dict = {}
                 after_reg_dict = {}
                 for spacer in search:  # todo fix this search, so that we take regex token from other spans into account
                     before_regex = ''
@@ -844,52 +1418,60 @@
                             if max_findings_per_page:
                                 num_matches = len(regex_matches(regex=proposal, doctext=annotation.document.text))
                                 if num_matches / (annotation.document.number_of_pages) < max_findings_per_page:
                                     new_proposals.append(proposal)
                                 else:
                                     logger.info(
                                         f'Skip to evaluate regex {repr(proposal)} as it finds {num_matches} in\
-                                            {annotation.document}.'
+                                                    {annotation.document}.'
                                     )
                             else:
                                 new_proposals.append(proposal)
             for proposal in new_proposals:
                 new_regex = re.sub(regex_to_remove_groupnames, '', proposal)
                 if new_regex not in regex_found:
                     regex_made.append(proposal)
                     regex_found.add(new_regex)
 
         logger.info(
-            f'For Label {self.name} we found {len(regex_made)} regex proposals for {len(all_annotations)} annotations.'
+            f'For Label {self.name} we found {len(regex_made)} regex proposals for {len(annotations)} Annotations.'
         )
+        return regex_made
 
+    def find_regex(self, category: 'Category', max_findings_per_page=100) -> List[str]:
+        """Find the best combination of regex for Label with before and after context."""
+        all_annotations = self.annotations(categories=[category])  # default is use_correct = True
+        if all_annotations == []:
+            logger.error(f'We cannot find annotations for Label {self} and Category {category}.')
+            return []
+        label_regex_token = self.base_regex(category=category, annotations=all_annotations)
+        found_regex = self._find_regexes(all_annotations, label_regex_token, category, max_findings_per_page)
         # todo replace by compare
         evaluations = [
             self.evaluate_regex(_regex_made, category=category, annotations=all_annotations)
-            for _regex_made in regex_made
+            for _regex_made in found_regex
         ]
 
         logger.info(
-            f'We compare {len(evaluations)} regex for {len(all_annotations)} correct Annotations for Category '
-            f'{category}.'
+            f'We compare {len(evaluations)} regex for {len(all_annotations)} correct Annotations for {category}.'
         )
 
         try:
             logger.info(f'Evaluate {self} for best regex.')
             best_regex = get_best_regex(evaluations)
         except ValueError:
             logger.exception(f'We cannot find regex for {self} with a f_score > 0.')
             best_regex = []
 
         if best_regex == []:
-            best_regex = [naive_proposal]
+            best_regex = [label_regex_token]
 
         return best_regex
 
-    def regex(self, categories: List[Category], update=False) -> List:
+    def regex(self, categories: List[Category], update=False) -> Dict:
         """Calculate regex to be used in the Extraction AI."""
         # if not is_file(self.regex_file_path, raise_exception=False) or update:
         logger.info(f'Build regexes for Label {self.name}.')
         regex = {}
         for category in categories:
             if category.id_ not in self._regex or update:
                 regex_category_file_path = os.path.join(
@@ -928,14 +1510,218 @@
     def lose_weight(self):
         """Delete data of the instance."""
         super().lose_weight()
         self._evaluations = {}
         self._tokens = {}
         self._regex = {}
 
+    def get_probable_outliers_by_regex(
+        self, categories: List[Category], use_test_docs: bool = False, top_worst_percentage: float = 0.1
+    ) -> List['Annotation']:
+        """
+        Get a list of Annotations that are identified by the least precise regular expressions.
+
+        This method iterates over the list of Categories and Annotations within each Category, collecting all the
+        regexes associated with them. It then evaluates these regexes and collects the top worst ones (i.e., those with
+        the least True Positives). For each of these top worst regexes, it returns the Annotations found by them but
+        not by the best regex for that label, potentially identifying them as outliers.
+
+        To detect outlier Annotations with multi-Spans, the method iterates over all the multi-Span Annotations under
+        the Label and checks each Span that was not detected by the aforementioned worst regexes. If it is not found by
+        any other regex in the Project, the entire Annotation is considered a potential outlier.
+
+        :param categories: A list of Category objects under which the search is conducted.
+        :type categories: List[Category]
+        :param use_test_docs: Indicates whether the evaluation of the regular expressions occurs on test Documents or
+                            training Documents.
+        :type use_test_docs: bool
+        :param top_worst_percentage: A threshold for determining what percentage of the worst regexes' output to return.
+        :type top_worst_percentage: float
+
+        :return: A list of Annotation objects identified by the least precise regular expressions.
+        :rtype: List[Annotation]
+        """
+        if use_test_docs:
+            documents = self.project.test_documents
+        else:
+            documents = self.project.documents
+        outliers = set()
+        for category in categories:
+            true_positives = {}
+            all_annotations = [
+                annotation for annotation in self.annotations(categories=[category]) if annotation.is_correct
+            ]
+            found_regex = self.regex(categories)
+            for regex in found_regex[category.id_]:
+                for document in documents:
+                    if regex in true_positives.keys():
+                        true_positives[regex] += document.evaluate_regex(regex, self)['count_correct_annotations']
+                    else:
+                        true_positives[regex] = document.evaluate_regex(regex, self)['count_correct_annotations']
+            if not true_positives:
+                logger.warning(f'No regex was found for {self} in {category}.')
+            elif not sum(true_positives.values()):
+                logger.warning(f'No resultative regexes found for {self} in {category}.')
+            else:
+                regexes_with_percentages = {k: v / sum(true_positives.values()) for k, v in true_positives.items()}
+                sorted_regexes = dict(sorted(regexes_with_percentages.items(), key=lambda item: item[1]))
+                regexes_with_cumulative = {}
+                for cur_regex, pct in sorted_regexes.items():
+                    if not regexes_with_cumulative:
+                        regexes_with_cumulative[cur_regex] = pct
+                        previous_key = cur_regex
+                    else:
+                        regexes_with_cumulative[cur_regex] = sorted_regexes[cur_regex] + sorted_regexes[previous_key]
+                        previous_key = cur_regex
+                filtered_regexes = {k: v for k, v in regexes_with_cumulative.items() if v <= top_worst_percentage}
+                max_tps_regex = self.find_regex(category=category)[0]
+                detected_by_worst_spans = set()
+                detected_by_best_spans = set()
+                for regex in filtered_regexes:
+                    cur_annotations_worst = set()
+                    cur_annotations_best = set()
+                    for annotation in all_annotations:
+                        text = annotation.document.text
+                        matches = regex_matches(text, regex, keep_full_match=False)
+                        for span in annotation.spans:
+                            for span_match in matches:
+                                span_match_offsets = (span_match['start_offset'], span_match['end_offset'])
+                                if span_match_offsets == (span.start_offset, span.end_offset):
+                                    cur_annotations_worst.add(annotation)
+                                    detected_by_worst_spans.add(span)
+                        matches = regex_matches(text, max_tps_regex, keep_full_match=False)
+                        for span in annotation.spans:
+                            for span_match in matches:
+                                span_match_offsets = (span_match['start_offset'], span_match['end_offset'])
+                                if span_match_offsets == (span.start_offset, span.end_offset):
+                                    cur_annotations_best.add(annotation)
+                                    detected_by_best_spans.add(span)
+                    if len(cur_annotations_worst) not in range(
+                        round(len(cur_annotations_best) * 0.5), round(len(cur_annotations_best) * 1.5)
+                    ):
+                        outliers.update(cur_annotations_worst - cur_annotations_best)
+                    for annotation in cur_annotations_worst.union(cur_annotations_best):
+                        if len(annotation.spans) > 1:
+                            text = annotation.document.text
+                            for span in annotation.spans:
+                                if span not in detected_by_worst_spans.union(detected_by_best_spans):
+                                    cur_regex = None
+                                    if found_regex[category.id_]:
+                                        for top_regex in found_regex[category.id_]:
+                                            matches = regex_matches(
+                                                text,
+                                                top_regex,
+                                                keep_full_match=False,
+                                            )
+                                            if matches:
+                                                for match in matches:
+                                                    span_match_offsets = (
+                                                        match['start_offset'],
+                                                        match['end_offset'],
+                                                    )
+                                                    if span_match_offsets == (span.start_offset, span.end_offset):
+                                                        cur_regex = top_regex
+                                                break
+                                    if not cur_regex:
+                                        outliers.add(annotation)
+                                break
+        outliers = list(outliers)
+        return outliers
+
+    def get_probable_outliers_by_confidence(
+        self,
+        evaluation_data,
+        confidence: float = 0.5,
+    ) -> List['Annotation']:
+        """
+        Get a list of Annotations with the lowest confidence.
+
+        A method iterates over the list of Categories, returning the top N Annotations with the lowest confidence score.
+
+        :param evaluation_data: An instance of the ExtractionEvaluation class that contains predicted confidence scores.
+        :type evaluation_data: ExtractionEvaluation instance
+        :param confidence: A level of confidence below which the Annotations are returned.
+        :type confidence: float
+        """
+        outliers = []
+        all_annotations = evaluation_data.data[
+            (evaluation_data.data['label_id'] == self.id_)
+            & (evaluation_data.data['confidence_predicted'] < confidence)
+            & (evaluation_data.data['is_correct'])
+        ]
+        for idx, outlier in all_annotations.iterrows():
+            if outlier['id_']:
+                document_id = outlier['document_id']
+                cur_annotation = self.project.get_document_by_id(document_id).get_annotation_by_id(outlier['id_'])
+                outliers.append(cur_annotation)
+        return outliers
+
+    def get_probable_outliers_by_normalization(self, categories: List[Category]) -> List['Annotation']:
+        """
+        Get a list of Annotations that do not pass normalization by the data type.
+
+        A method iterates over the list of Categories, returning the Annotations that do not fit into the data type of
+        a Label (= have None returned in an attempt of the normalization by the Label's data type).
+
+        :param categories: Categories under which the search is done.
+        :type categories: List[Category]
+        """
+        outliers = set()
+        for category in categories:
+            for annotation in [
+                annotation for annotation in self.annotations(categories=[category]) if annotation.is_correct
+            ]:
+                for span in annotation.spans:
+                    normalized = normalize(span.offset_string, self.data_type)
+                    if not normalized:
+                        outliers.add(annotation)
+        outliers = list(outliers)
+        return outliers
+
+    def get_probable_outliers(
+        self,
+        categories: List[Category],
+        regex_search: bool = True,
+        regex_worst_percentage: float = 0.1,
+        confidence_search: bool = True,
+        evaluation_data=None,
+        normalization_search: bool = True,
+    ) -> List['Annotation']:
+        """
+        Get a list of Annotations that are outliers.
+
+        Outliers are determined by either of three logics or a combination of them applied: found by the worst regex,
+        have the lowest confidence and/or are not normalizeable by the data type of a given Label.
+
+        :param categories: Categories under which the search is done.
+        :type categories: List[Category]
+        :param regex_search: Enable search by top worst regexes.
+        :type regex_search: bool
+        :param regex_worst_percentage: A % of Annotations returned by the regexes.
+        :type regex_worst_percentage: float
+        :param confidence_search: Enable search by the lowest-confidence Annotations.
+        :type confidence_search: bool
+        :param normalization_search: Enable search by normalizing Annotations by the Label's data type.
+        :type normalization_search: bool
+        :raises ValueError: When all search options are disabled.
+        """
+        if not regex_search and not confidence_search and not normalization_search:
+            raise ValueError('All search modes disabled, search is impossible. Enable at least one search mode.')
+        results = []
+        if regex_search:
+            results.append(
+                set(self.get_probable_outliers_by_regex(categories, top_worst_percentage=regex_worst_percentage))
+            )
+        if confidence_search:
+            results.append(set(self.get_probable_outliers_by_confidence(evaluation_data)))
+        if normalization_search:
+            results.append(set(self.get_probable_outliers_by_normalization(categories)))
+        intersection_results = list(set.intersection(*results))
+        return intersection_results
+
     # def save(self) -> bool:
     #     """
     #     Save Label online.
     #
     #     If no Label Sets are specified, the Label is associated with the first default Label Set of the Project.
     #
     #     :return: True if the new Label was created.
@@ -954,94 +1740,150 @@
     #         label_sets=self.label_sets,
     #     )
     #
     #     return True
 
 
 class Span(Data):
-    """A Span is a sequence of characters or whitespaces without line break."""
+    """
+    A Span is a sequence of characters or whitespaces without line break.
+
+    For more details see https://dev.konfuzio.com/sdk/explanations.html#span-concept
+    """
 
-    def __init__(self, start_offset: int, end_offset: int, annotation=None):
+    def __init__(
+        self,
+        start_offset: int,
+        end_offset: int,
+        annotation: 'Annotation' = None,
+        document: 'Document' = None,
+        strict_validation: bool = True,
+    ):
         """
         Initialize the Span without bbox, to save storage.
 
         If Bbox should be calculated the bbox file of the Document will be automatically downloaded.
 
         :param start_offset: Start of the offset string (int)
         :param end_offset: Ending of the offset string (int)
-        :param annotation: The Annotation the Span belong to
+        :param annotation: The Annotation the Span belongs to. If not set, the Span is considered "virtual"
+        :param document: Document the Span belongs to. If not specified, the annotation document is used.
+        :param strict_validation: Whether to apply strict validation rules.
+        See https://dev.konfuzio.com/sdk/tutorials/data_validation/index.html
         """
         self.id_local = next(Data.id_iter)
+
+        self.document: Document = document
+        if annotation and document:
+            assert annotation.document is document
         self.annotation: Annotation = annotation
+        if annotation:
+            self.document = annotation.document
+
         self.start_offset = start_offset
         self.end_offset = end_offset
         self.top = None
         self.bottom = None
         self._line_index = None
         self._page: Union[Page, None] = None
         self._bbox: Union[Bbox, None] = None
         self.regex_matching = []
-        annotation and annotation.add_span(self)  # only add if Span has access to an Annotation
-        self._valid()
+        # check because we don't want to add a Span multiple times to the Annotation
+        if annotation and self not in annotation.spans:  # only add if Span has access to an Annotation
+            annotation.add_span(self)
+        self._valid(strict_validation)
 
-    def _valid(
-        self,
-    ):
-        """Validate containted data."""
+    def _valid(self, strict: bool = True, handler: str = 'sdk_validation'):
+        """
+        Validate containted data.
+
+        :param strict: If False, it allows Spans to have zero length, or span more than one visual line. For more
+        details see https://dev.konfuzio.com/sdk/tutorials/data_validation/index.html
+        """
         if self.end_offset == self.start_offset == 0:
-            logger.error(f'{self} is intentionally left empty.')
-        elif self.end_offset < 0:
-            raise ValueError(f'{self} must span text.')
+            logger.warning(f'{self} is intentionally left empty.')
+        elif self.start_offset < 0 or self.end_offset < 0:
+            exception_or_log_error(
+                msg=f'{self} must span text.',
+                fail_loudly=strict,
+                exception_type=ValueError,
+                handler=handler,
+            )
         elif self.start_offset == self.end_offset:
-            raise ValueError(f"{self} must span text: Start {self.start_offset} equals end.")
+            exception_or_log_error(
+                msg=f'{self} must span text: Start {self.start_offset} equals end.',
+                fail_loudly=strict,
+                exception_type=ValueError,
+                handler=handler,
+            )
         elif self.end_offset < self.start_offset:
-            raise ValueError(f"{self} length must be positive.")
+            exception_or_log_error(
+                msg=f'{self} length must be positive.',
+                fail_loudly=strict,
+                exception_type=ValueError,
+                handler=handler,
+            )
         elif self.offset_string and ('\n' in self.offset_string or '\f' in self.offset_string):
-            raise ValueError(f'{self} must not span more than one visual line.')
+            exception_or_log_error(
+                msg=f'{self} must not span more than one visual line.',
+                fail_loudly=strict,
+                exception_type=ValueError,
+                handler=handler,
+            )
         return True
 
     @property
     def page(self) -> Page:
         """Return Page of Span."""
-        if self.annotation is None or self.annotation.document is None:
+        if self.document is None:
             raise NotImplementedError
-        elif self.annotation.document.text is None:
-            logger.error(f'{self.annotation.document} does not provide text.')
+        elif self.document.text is None:
+            logger.error(f'{self.document} does not provide text.')
             pass
-        elif self._page is None and self.annotation.document.pages():
-            text = self.annotation.document.text[: self.start_offset]
+        elif self._page is None and self.document.pages():
+            text = self.document.text[: self.start_offset]
             page_index = len(text.split('\f')) - 1
-            self._page = self.annotation.document.get_page_by_index(page_index=page_index)
+            self._page = self.document.get_page_by_index(page_index=page_index)
         return self._page
 
     @property
     def line_index(self) -> int:
         """Return index of the line of the Span."""
         self._valid()
-        if self.annotation.document.text and self._line_index is None:
-            line_number = len(self.annotation.document.text[: self.start_offset].replace('\f', '\n').split('\n'))
+        if self.document.text and self._line_index is None:
+            line_number = len(self.document.text[: self.start_offset].replace('\f', '\n').split('\n'))
             self._line_index = line_number - 1
 
         return self._line_index
 
     def __eq__(self, other) -> bool:
-        """Compare any point of data with their position is equal."""
+        """Twp Spans are equal if their start_offset and end_offset are both equal."""
         return (
             type(self) == type(other)
             and self.start_offset == other.start_offset
             and self.end_offset == other.end_offset
         )
 
     def __lt__(self, other: 'Span'):
-        """If we sort spans we do so by start offset."""
-        return self.start_offset < other.start_offset
+        """We compare Spans by their start offset. If start offsets are equal, we use end offsets."""
+        return (self.start_offset, self.end_offset) < (other.start_offset, other.end_offset)
 
     def __repr__(self):
         """Return string representation."""
-        return f"{self.__class__.__name__} ({self.start_offset}, {self.end_offset})"
+        if self.offset_string and len(self.offset_string) < 16:
+            offset_string_repr = self.offset_string
+        elif self.offset_string:
+            offset_string_repr = f'{self.offset_string[:14]}[...]'
+        else:
+            offset_string_repr = ''
+
+        if not self.annotation:
+            return f'Virtual {self.__class__.__name__} ({self.start_offset}, {self.end_offset}): "{offset_string_repr}"'
+        else:
+            return f'{self.__class__.__name__} ({self.start_offset}, {self.end_offset}): "{offset_string_repr}"'
 
     def __hash__(self):
         """Make any online or local concept hashable. See https://stackoverflow.com/a/7152650."""
         if not self.annotation:
             raise NotImplementedError('Span without Annotation is not hashable.')
         else:
             return hash((self.annotation, self.start_offset, self.end_offset))
@@ -1053,159 +1895,252 @@
             full_replace = suggest_regex_for_string(self.offset_string, replace_characters=True, replace_numbers=True)
             return merge_regex([full_replace])
         else:
             raise NotImplementedError('A Span needs a Annotation and Document relation to suggest a Regex.')
 
     def bbox(self) -> Bbox:
         """Calculate the bounding box of a text sequence."""
-        if not self.annotation:
+        if not self.document:
             raise NotImplementedError
         if not self.page:
             logger.warning(f'{self} does not have a Page.')
             return None
-        if not self.annotation.document.bboxes_available:
-            logger.warning(f'{self.annotation.document} of {self} does not provide Bboxes.')
+        if not self.document.bboxes_available:
+            logger.warning(f'{self.document} of {self} does not provide Bboxes.')
             return None
         _ = self.line_index  # quick validate if start and end is in the same line of text
 
         if self._bbox is None:
-            warn('WIP: Modifications before the next stable release expected.', FutureWarning, stacklevel=2)
-            # todo: verify that one Span relates to Character in on line of text
             character_range = range(self.start_offset, self.end_offset)
-            document = self.annotation.document
+            document = self.document
             characters = {key: document.bboxes.get(key) for key in character_range if document.text[key] != ' '}
             if not all(characters.values()):
-                logger.error(
-                    f'{self} in {self.annotation.document} contains Characters that don\'t provide a Bounding Box.'
-                )
+                logger.error(f"{self} in {self.document} contains Characters that don't provide a Bounding Box.")
             self._bbox = Bbox(
                 x0=min([ch.x0 for c, ch in characters.items() if ch is not None]),
                 x1=max([ch.x1 for c, ch in characters.items() if ch is not None]),
-                y0=min([ch.y0 for c, ch in characters.items() if ch is not None]),
+                y0=max(0, min([ch.y0 for c, ch in characters.items() if ch is not None])),
                 y1=max([ch.y1 for c, ch in characters.items() if ch is not None]),
                 page=self.page,
+                validation=self.document._bbox_validation_type,
             )
         return self._bbox
 
+    def bbox_dict(self) -> Dict:
+        """Return Span Bbox info as a serializable Dict format for external integration with the Konfuzio Server."""
+        span_dict = {
+            'start_offset': self.start_offset,
+            'end_offset': self.end_offset,
+            'line_number': self.line_index + 1,
+            'offset_string': self.offset_string,
+            'offset_string_original': self.offset_string,
+            'page_index': self.bbox().page.index,
+            'top': self.bbox().page.height - self.bbox().y1,
+            'bottom': self.bbox().page.height - self.bbox().y0,
+            'x0': self.bbox().x0,
+            'x1': self.bbox().x1,
+            'y0': self.bbox().y0,
+            'y1': self.bbox().y1,
+        }
+        return span_dict
+
     @property
     def normalized(self):
         """Normalize the offset string."""
         return normalize(self.offset_string, self.annotation.label.data_type)
 
     @property
     def offset_string(self) -> Union[str, None]:
         """Calculate the offset string of a Span."""
-        if self.annotation and self.annotation.document and self.annotation.document.text:
-            return self.annotation.document.text[self.start_offset : self.end_offset]
+        if self.document and self.document.text:
+            return self.document.text[self.start_offset : self.end_offset]
         else:
             return None
 
     def eval_dict(self):
         """Return any information needed to evaluate the Span."""
         if self.start_offset == self.end_offset == 0:
             span_dict = {
-                "id_local": None,
-                "id_": None,
-                "confidence": None,
-                "offset_string": None,
-                "normalized": None,
-                "start_offset": 0,  # to support compare function to evaluate True and False
-                "end_offset": 0,  # to support compare function to evaluate True and False
-                "is_correct": None,
-                "created_by": None,
-                "revised_by": None,
-                "custom_offset_string": None,
-                "revised": None,
-                "label_threshold": None,
-                "label_id": None,
-                "label_set_id": None,
-                "annotation_id": None,
-                "annotation_set_id": 0,  # to allow grouping to compare boolean
-                "document_id": 0,
-                "document_id_local": 0,
-                "category_id": 0,
-                "x0": 0,
-                "x1": 0,
-                "y0": 0,
-                "y1": 0,
-                "line_index": 0,
-                "page_index": None,
-                "page_width": 0,
-                "page_height": 0,
-                "x0_relative": None,
-                "x1_relative": None,
-                "y0_relative": None,
-                "y1_relative": None,
-                "page_index_relative": None,
-                "area_quadrant_two": 0,
-                "area": 0,
-                "label_name": None,
-                "label_set_name": None,
-                "data_type": None,
+                'id_local': None,
+                'id_': None,
+                'confidence': None,
+                'offset_string': None,
+                'normalized': None,
+                'start_offset': 0,  # to support compare function to evaluate True and False
+                'end_offset': 0,  # to support compare function to evaluate True and False
+                'is_correct': None,
+                'created_by': None,
+                'revised_by': None,
+                'custom_offset_string': None,
+                'revised': None,
+                'label_threshold': None,
+                'label_id': 0,
+                'label_has_multiple_top_candidates': None,
+                'label_set_id': 0,
+                'annotation_id': None,
+                'annotation_set_id': 0,  # to allow grouping to compare boolean
+                'document_id': 0,
+                'document_id_local': 0,
+                'category_id': 0,
+                'x0': 0,
+                'x1': 0,
+                'y0': 0,
+                'y1': 0,
+                'line_index': 0,
+                'page_index': None,
+                'page_width': 0,
+                'page_height': 0,
+                'x0_relative': None,
+                'x1_relative': None,
+                'y0_relative': None,
+                'y1_relative': None,
+                'page_index_relative': None,
+                'area_quadrant_two': 0,
+                'area': 0,
+                'label_name': None,
+                'label_set_name': None,
+                'data_type': None,
             }
         else:
             span_dict = {
-                "id_local": self.annotation.id_local,
-                "id_": self.annotation.id_,
-                "confidence": self.annotation.confidence,
-                "offset_string": self.offset_string,
-                "normalized": self.normalized,
-                "start_offset": self.start_offset,  # to support multiline
-                "end_offset": self.end_offset,  # to support multiline
-                "is_correct": self.annotation.is_correct,
-                "created_by": self.annotation.created_by,
-                "revised_by": self.annotation.revised_by,
-                "custom_offset_string": self.annotation.custom_offset_string,
-                "revised": self.annotation.revised,
-                "label_threshold": self.annotation.label.threshold,  # todo: allow to optimize threshold
-                "label_id": self.annotation.label.id_,
-                "label_set_id": self.annotation.label_set.id_,
-                "annotation_id": self.annotation.id_,
-                "annotation_set_id": self.annotation.annotation_set.id_,
-                "document_id": self.annotation.document.id_,
-                "document_id_local": self.annotation.document.id_local,
-                "category_id": self.annotation.document.category.id_,
-                "line_index": self.line_index,
-                "data_type": self.annotation.label.data_type,
+                'id_local': self.annotation.id_local,
+                'id_': self.annotation.id_,
+                'confidence': self.annotation.confidence,
+                'offset_string': self.offset_string,
+                'normalized': self.normalized,
+                'start_offset': self.start_offset,  # to support multiline
+                'end_offset': self.end_offset,  # to support multiline
+                'is_correct': self.annotation.is_correct,
+                'created_by': self.annotation.created_by,
+                'revised_by': self.annotation.revised_by,
+                'custom_offset_string': self.annotation.custom_offset_string,
+                'revised': self.annotation.revised,
+                'label_threshold': self.annotation.label.threshold,  # todo: allow to optimize threshold
+                'label_id': self.annotation.label.id_,
+                'label_has_multiple_top_candidates': self.annotation.label.has_multiple_top_candidates,
+                'label_set_id': self.annotation.label_set.id_,
+                'annotation_id': self.annotation.id_,
+                'annotation_set_id': self.annotation.annotation_set.id_,
+                'document_id': self.document.id_ if self.document.id_ else self.document.copy_of_id,
+                'document_id_local': self.document.id_local,
+                'category_id': self.document.category.id_,
+                'line_index': self.line_index,
+                'data_type': self.annotation.label.data_type,
             }
 
             if self.bbox():
-                span_dict["x0"] = self.bbox().x0
-                span_dict["x1"] = self.bbox().x1
-                span_dict["y0"] = self.bbox().y0
-                span_dict["y1"] = self.bbox().y1
+                span_dict['x0'] = self.bbox().x0
+                span_dict['x1'] = self.bbox().x1
+                span_dict['y0'] = self.bbox().y0
+                span_dict['y1'] = self.bbox().y1
 
                 # https://www.cuemath.com/geometry/quadrant/
-                span_dict["area_quadrant_two"] = self.bbox().x0 * self.bbox().y0
-                span_dict["area"] = self.bbox().area
+                span_dict['area_quadrant_two'] = self.bbox().x0 * self.bbox().y0
+                span_dict['area'] = self.bbox().area
 
             if self.page:  # todo separate as eval_dict on Page level
-                span_dict["page_index"] = self.page.index
-                span_dict["page_width"] = self.page.width
-                span_dict["page_height"] = self.page.height
-                span_dict["x0_relative"] = self.bbox().x0 / self.page.width
-                span_dict["x1_relative"] = self.bbox().x1 / self.page.width
-                span_dict["y0_relative"] = self.bbox().y0 / self.page.height
-                span_dict["y1_relative"] = self.bbox().y1 / self.page.height
-                span_dict["page_index_relative"] = self.page.index / self.annotation.document.number_of_pages
-
-            document_id = (
-                self.annotation.document.id_
-                if self.annotation.document.id_ is not None
-                else self.annotation.document.copy_of_id
-            )
-            span_dict["document_id"] = document_id
-            span_dict["label_name"] = self.annotation.label.name if self.annotation.label else None
-            span_dict["label_set_name"] = self.annotation.label_set.name if self.annotation.label_set else None
+                span_dict['page_index'] = self.page.index
+                span_dict['page_width'] = self.page.width
+                span_dict['page_height'] = self.page.height
+                span_dict['x0_relative'] = self.bbox().x0 / self.page.width
+                span_dict['x1_relative'] = self.bbox().x1 / self.page.width
+                span_dict['y0_relative'] = self.bbox().y0 / self.page.height
+                span_dict['y1_relative'] = self.bbox().y1 / self.page.height
+                span_dict['page_index_relative'] = self.page.index / self.document.number_of_pages
+
+            document_id = self.document.id_ if self.document.id_ is not None else self.document.copy_of_id
+            span_dict['document_id'] = document_id
+            span_dict['label_name'] = self.annotation.label.name if self.annotation.label else None
+            span_dict['label_set_name'] = self.annotation.label_set.name if self.annotation.label_set else None
 
         return span_dict
 
+    @staticmethod
+    def get_sentence_from_spans(spans: Iterable['Span'], punctuation=None) -> List[List['Span']]:
+        """Return a list of Spans corresponding to Sentences separated by Punctuation."""
+        if punctuation is None:
+            punctuation = {'.', '!', '?'}
+
+        # get the sentence spans
+        sentence_spans: List[List[Span]] = [[]]
+        for span in spans:
+            # get the text of the span
+            span_text = span.offset_string
+
+            # find the start and end offsets of each sentence in the span
+            prev_sentence_start_offset = 0
+            for index, char in enumerate(span_text):
+                if char == ' ':
+                    continue
+                if char in punctuation:
+                    sentence_start_offset = span.start_offset + prev_sentence_start_offset
+                    sentence_end_offset = span.start_offset + index + 1
+                    sentence_spans[-1].append(
+                        Span(
+                            start_offset=sentence_start_offset,
+                            end_offset=sentence_end_offset,
+                            document=span.page.document,
+                        )
+                    )
+                    sentence_spans.append([])
+                    prev_sentence_start_offset = index + 1
+
+            if prev_sentence_start_offset < len(span_text):
+                sentence_start_offset = span.start_offset + prev_sentence_start_offset
+                sentence_end_offset = span.end_offset
+                sentence_spans[-1].append(
+                    Span(
+                        start_offset=sentence_start_offset,
+                        end_offset=sentence_end_offset,
+                        document=span.page.document,
+                    )
+                )
+
+        sentence_spans = [x for x in sentence_spans if len(x)]
+        return sentence_spans
+
+
+class AnnotationsContainer(dict):
+    """
+    Hold a collection of Annotations in an efficient way (dict of tuples).
+
+    Provides methods to interact with the AnnotationsContainer as if it was a list.
+    """
+
+    def remove(self, obj):
+        """Delete an Annotation from the container. Mimicks the similar method of the list."""
+        # obj._spans might be a list as it might come from a previous SDK version
+        if isinstance(obj._spans, list):
+            key = (
+                tuple(sorted((s.start_offset, s.end_offset) for s in obj._spans)),
+                obj.label.name,
+            )
+        else:
+            key = (tuple(sorted(obj._spans.keys())), obj.label.name)
+        del self[key]
+
+    def append(self, obj):
+        """Add an Annotation to the container. Mimicks the similar method of the list."""
+        # obj._spans might be a list as it might come from a previous SDK version
+        if isinstance(obj._spans, list):
+            key = (
+                tuple(sorted((s.start_offset, s.end_offset) for s in obj._spans)),
+                obj.label.name,
+            )
+        else:
+            key = (tuple(sorted(obj._spans.keys())), obj.label.name)
+        self[key] = obj
+
 
 class Annotation(Data):
-    """Hold information that a Label, Label Set and Annotation Set has been assigned to and combines Spans."""
+    """
+    Hold information that a Label, Label Set and Annotation Set has been assigned to and combines Spans.
+
+    For more details see https://dev.konfuzio.com/sdk/explanations.html#annotation-concept
+    """
 
     def __init__(
         self,
         document: 'Document',
         annotation_set_id: Union[int, None] = None,  # support to init from API output
         annotation_set: Union[AnnotationSet, None] = None,  # support to init from API output
         label: Union[int, Label, None] = None,
@@ -1218,15 +2153,15 @@
         spans=None,
         accuracy: float = None,
         confidence: float = None,
         created_by: int = None,
         revised_by: int = None,
         translated_string: str = None,
         custom_offset_string: bool = False,
-        offset_string: str = False,
+        offset_string: str = None,
         *args,
         **kwargs,
     ):
         """
         Initialize the Annotation.
 
         :param label: ID of the Annotation
@@ -1251,81 +2186,122 @@
         self.created_by = created_by
         self.revised_by = revised_by
         if custom_offset_string:
             self.custom_offset_string = offset_string
         else:
             self.custom_offset_string = None
         self.id_ = id_  # Annotations can have None id_, if they are not saved online and are only available locally
-        self._spans: List[Span] = []
+        self._spans: Dict = {}
+
+        self._bbox = None
 
-        if accuracy is not None:  # its a confidence
+        if accuracy is not None:  # it's a confidence
             self.confidence = accuracy
         elif confidence is not None:
             self.confidence = confidence
-        elif self.id_ is not None and accuracy is None:  # hotfix: it's an online annotation crated by a human
+        elif self.id_ is not None and accuracy is None:  # hotfix: it's an online Annotation crated by a human
             self.confidence = 1
         elif accuracy is None and confidence is None:
             self.confidence = None
         else:
             raise ValueError('Annotation has an id_ but does not provide a confidence.')
 
         if isinstance(label, int):
             self.label: Label = self.document.project.get_label_by_id(label)
         elif sdk_isinstance(label, Label):
             self.label: Label = label
+        elif isinstance(label, str):
+            self.label: Label = self.document.project.get_label_by_name(label)
+        elif label is None:
+            self.label = self.document.project.no_label
+            logger.warning(f'{self} in {self.document} initialized without Label information. Using NO_LABEL.')
         else:
-            raise ValueError(f'{self.__class__.__name__} {self.id_local} has no Label.')
-
-        # if no label_set_id we check if is passed by section_label_id
-        if label_set_id is None and kwargs.get("section_label_id") is not None:
-            label_set_id = kwargs.get("section_label_id")
-
-        # handles association to an Annotation Set if the Annotation belongs to a Category
-        if isinstance(label_set_id, int):
-            self.label_set: LabelSet = self.document.project.get_label_set_by_id(label_set_id)
-        elif sdk_isinstance(label_set, LabelSet):
-            self.label_set = label_set
-        else:
-            self.label_set = None
-            logger.info(f'{self.__class__.__name__} {self.id_local} has no Label Set.')
+            raise ValueError(f'Cannot initialize with {label=}. Must be int, str or Label.')
 
         # make sure an Annotation Set is available
         if isinstance(annotation_set_id, int):
             self.annotation_set: AnnotationSet = self.document.get_annotation_set_by_id(annotation_set_id)
         elif sdk_isinstance(annotation_set, AnnotationSet):
-            # it's a save way to look up the annotation set first. Otherwise users can add annotation sets which
-            # do not relate to the document
+            # it's a safe way to look up the Annotation Set first. Otherwise users can add Annotation Sets which
+            # do not relate to the Document
             self.annotation_set: AnnotationSet = self.document.get_annotation_set_by_id(annotation_set.id_)
         else:
+            # it will be set later, or an exception is raised at the end of the init
             self.annotation_set = None
-            logger.warning(f'{self} in {self.document} created but without Annotation Set information.')
+
+        # if no label_set_id we check if is passed by section_label_id
+        if label_set_id is None and kwargs.get('label_set_id') is not None:
+            label_set_id = kwargs.get('label_set_id')
+
+        # handles association to an Annotation Set if the Annotation belongs to a Category
+        if isinstance(label_set_id, int):
+            label_set: LabelSet = self.document.project.get_label_set_by_id(label_set_id)
+        elif label_set is None and label_set_id is None and len(self.label.label_sets) == 1:
+            label_set = self.label.label_sets[0]
+
+        if sdk_isinstance(label_set, LabelSet):
+            if self.annotation_set is not None:
+                assert label_set == self.annotation_set.label_set, f'Conflicting Label Set information provided\
+                    {label_set=} and {self.annotation_set.label_set=}'
+            elif label_set.has_multiple_annotation_sets:
+                raise ValueError(
+                    f'Cannot assign {self} to AnnotationSet. {label_set} can have multiple Annotation Sets. '
+                    f'Please provide the Annotation Set or AnnotationSet ID.'
+                )
+            else:
+                matching_annotation_sets = [
+                    ann_set for ann_set in self.document.annotation_sets() if ann_set.label_set == label_set
+                ]
+                if len(matching_annotation_sets) == 1:
+                    annotation_set = matching_annotation_sets[0]
+                elif len(matching_annotation_sets) == 0:
+                    annotation_set = AnnotationSet(label_set=label_set, document=self.document)
+                else:
+                    raise ValueError(
+                        f'Found multiple Annotation Sets for {label_set} in {self.document}. '
+                        f'This should not happen because {label_set.has_multiple_annotation_sets=}.'
+                    )
+                self.annotation_set = annotation_set
+
+        if self.annotation_set.label_set.id_:
+            # for legacy reasons, we allow all Annotations to be in the NO_LABEL_SET Annotation Set
+            assert (
+                self.label in self.annotation_set.label_set.labels
+            ), f'{self.label} is not in {self.annotation_set.label_set.labels} of {self.annotation_set}.'
 
         for span in spans or []:
             self.add_span(span)
 
-        self.selection_bbox = kwargs.get("selection_bbox", None)
+        self.selection_bbox = kwargs.get('selection_bbox', None)
+        if isinstance(self.selection_bbox, dict):
+            page = self.document.get_page_by_index(self.selection_bbox['page_index'])
+            x0, x1, y0, y1 = (
+                self.selection_bbox['x0'],
+                self.selection_bbox['x1'],
+                self.selection_bbox['y0'],
+                self.selection_bbox['y1'],
+            )
+            self.selection_bbox = Bbox(x0=x0, x1=x1, y0=y0, y1=y1, page=page)
 
         # TODO START LEGACY to support multiline Annotations
-        bboxes = kwargs.get("bboxes", None)
+        bboxes = kwargs.get('bboxes', None)
         if bboxes and len(bboxes) > 0:
             for bbox in bboxes:
-                if "start_offset" in bbox.keys() and "end_offset" in bbox.keys():
-                    Span(start_offset=bbox["start_offset"], end_offset=bbox["end_offset"], annotation=self)
+                if 'start_offset' in bbox.keys() and 'end_offset' in bbox.keys():
+                    Span(start_offset=bbox['start_offset'], end_offset=bbox['end_offset'], annotation=self)
                 else:
                     raise ValueError(f'SDK cannot read bbox of Annotation {self.id_} in {self.document}: {bbox}')
         elif (
             bboxes is None
-            and kwargs.get("start_offset", None) is not None
-            and kwargs.get("end_offset", None) is not None
+            and kwargs.get('start_offset', None) is not None
+            and kwargs.get('end_offset', None) is not None
         ):
             # Legacy support for creating Annotations with a single offset
             bbox = kwargs.get('bbox', {})
-            _ = Span(start_offset=kwargs.get("start_offset"), end_offset=kwargs.get("end_offset"), annotation=self)
-            # self.add_span(sa)
-
+            _ = Span(start_offset=kwargs.get('start_offset'), end_offset=kwargs.get('end_offset'), annotation=self)
             logger.warning(f'{self} is empty')
 
         self.top = None
         self.top = None
         self.x0 = None
         self.x1 = None
         self.y0 = None
@@ -1337,63 +2313,73 @@
             self.top = bbox.get('top')
             self.bottom = bbox.get('bottom')
             self.x0 = bbox.get('x0')
             self.x1 = bbox.get('x1')
             self.y0 = bbox.get('y0')
             self.y1 = bbox.get('y1')
 
-        self.bboxes = kwargs.get('bboxes', None)
-        self.selection_bbox = kwargs.get('selection_bbox', None)
         self.page_number = kwargs.get('page_number', None)
         # END LEGACY -
 
         # regex features
         self._tokens = []
         self._regex = None
 
         # Call add_annotation to document at the end, so all attributes for duplicate checking are available.
         self.document.add_annotation(self)
 
         if not self.document:
             raise NotImplementedError(f'{self} has no Document and cannot be created.')
         if not self.label_set:
             raise NotImplementedError(f'{self} has no Label Set and cannot be created.')
+        if not self.annotation_set:
+            raise NotImplementedError(f'{self} has no Annotation Set and cannot be created.')
         if not self.label:
             raise NotImplementedError(f'{self} has no Label and cannot be created.')
         if not self.spans:
-            raise NotImplementedError(f'{self} has no Spans and cannot be created.')
+            exception_or_log_error(
+                msg=f'{self} has no Spans and cannot be created.',
+                fail_loudly=self.document.project._strict_data_validation,
+                exception_type=NotImplementedError,
+            )
 
     def __repr__(self):
         """Return string representation."""
         if self.label and self.document:
-            span_str = ', '.join(f'{x.start_offset, x.end_offset}' for x in self._spans)
-            return f"Annotation ({self.get_link()}) {self.label.name} {span_str}"
+            span_str = ', '.join(f'{x.start_offset, x.end_offset}' for x in self.spans)
+            return f'Annotation ({self.get_link()}) {self.label.name} {span_str}'
         elif self.label:
-            return f"Annotation ({self.get_link()}) {self.label.name} ({self._spans})"
+            return f'Annotation ({self.get_link()}) {self.label.name} ({self.spans})'
         else:
-            return f"Annotation ({self.get_link()}) without Label ({self.start_offset}, {self.end_offset})"
+            return f'Annotation ({self.get_link()}) without Label ({self.start_offset}, {self.end_offset})'
 
     def __eq__(self, other):
         """We compare an Annotation based on it's Label, Label-Sets if it's online otherwise on the id_local."""
-        result = False
-        if self.document and other.document and self.document == other.document:  # same Document
-            # if self.is_correct and other.is_correct:  # for correct Annotations check if they are identical
-            if self.label and other.label and self.label == other.label:  # same Label
-                if self.spans == other.spans:  # logic changed from "one Span is identical" to "all Spans identical"
-                    return True
-
-        return result
+        return (
+            (self._spans.keys() == other._spans.keys())
+            and self.label
+            and other.label
+            and (self.label == other.label)
+            and self.document
+            and other.document
+            and (self.document == other.document)
+        )
 
     def __lt__(self, other):
         """If we sort Annotations we do so by start offset."""
-        return min([span.start_offset for span in self.spans]) < min([span.start_offset for span in other.spans])
+        return min(self._spans.keys()) < min(other._spans.keys())
 
     def __hash__(self):
         """Identity of Annotation that does not change over time."""
-        return hash((self.start_offset, self.end_offset, self.label_set, self.document, self.label))
+        return hash((self.id_local, self.document))
+
+    @property
+    def page(self) -> Page:
+        """Return Page of Annotation."""
+        return self.spans[0].page
 
     @property
     def is_multiline(self) -> int:
         """Calculate if Annotation spans multiple lines of text."""
         logger.error('We cannot calculate this. The indicator is unreliable.')
         return self.offset_string.count('\n')
 
@@ -1403,21 +2389,21 @@
         logger.warning('You use normalize on Annotation Level which is legacy.')
         return normalize(self.offset_string, self.label.data_type)
 
     @property
     def start_offset(self) -> int:
         """Legacy: One Annotation can have multiple start offsets."""
         logger.warning('You use start_offset on Annotation Level which is legacy.')
-        return min([sa.start_offset for sa in self._spans], default=None)
+        return min((sa[0] for sa in self._spans.keys()), default=None)
 
     @property
     def end_offset(self) -> int:
         """Legacy: One Annotation can have multiple end offsets."""
         logger.warning('You use end_offset on Annotation Level which is legacy.')
-        return max([sa.end_offset for sa in self._spans], default=None)
+        return max((sa[1] for sa in self._spans.keys()), default=None)
 
     @property
     def offset_string(self) -> List[str]:
         """View the string representation of the Annotation."""
         if len(self.spans) > 1:
             logger.warning(f'You use offset string on {self} level which is legacy.')
         if not self.custom_offset_string and self.document.text:
@@ -1429,122 +2415,128 @@
         return result
 
     @property
     def eval_dict(self) -> List[dict]:
         """Calculate the Span information to evaluate the Annotation."""
         return [span.eval_dict() for span in self.spans]
 
+    @property
+    def label_set(self) -> LabelSet:
+        """Return Label Set of Annotation."""
+        return self.annotation_set.label_set
+
     def add_span(self, span: Span):
         """Add a Span to an Annotation incl. a duplicate check per Annotation."""
-        if span not in self._spans:
+        if (span.start_offset, span.end_offset) not in self._spans:
             # add the Span first to make sure to bea able to do a duplicate check
-            self._spans.append(span)  # one Annotation can span multiple Spans
+            self._spans[(span.start_offset, span.end_offset)] = span  # one Annotation can span multiple Spans
             if span.annotation is not None and self != span.annotation:
                 raise ValueError(f'{span} should be added to {self} but relates to {span.annotation}.')
             else:
                 span.annotation = self  # todo feature to link one Span to many Annotations
+                span.document = self.document
         else:
             raise ValueError(f'In {self} the {span} is a duplicate and will not be added.')
         return self
 
     def get_link(self):
         """Get link to the Annotation in the SmartView."""
         if self.is_online:
             return get_annotation_view_url(self.id_)
         else:
             return None
 
-    def save(self, document_annotations: list = None) -> bool:
+    def save(self, label_set_id=None, annotation_set_id=None, document_annotations: list = None) -> bool:
         """
         Save Annotation online.
 
         If there is already an Annotation in the same place as the current one, we will not be able to save the current
         annotation.
 
         In that case, we get the id_ of the original one to be able to track it.
         The verification of the duplicates is done by checking if the offsets and Label match with any Annotations
         online.
         To be sure that we are comparing with the information online, we need to have the Document updated.
         The update can be done after the request (per annotation) or the updated Annotations can be passed as input
         of the function (advisable when dealing with big Documents or Documents with many Annotations).
 
+        Specify label_set_id if you want to create an Annotation belonging to a new Annotation Set. Specify
+        annotation_set_id if you want to add an Annotation to an existing Annotation Set. Do not specify both of them.
+
         :param document_annotations: Annotations in the Document (list)
         :return: True if new Annotation was created
         """
+        if self.label == self.document.project.no_label:
+            raise ValueError('You cannot save Annotations with Label NO_LABEL.')
+        if self.document.category == self.document.project.no_category:
+            raise ValueError(f'You cannot save Annotations of Documents with {self.document.category}.')
         new_annotation_added = False
-        if not self.label_set:
-            label_set_id = None
-        else:
-            label_set_id = self.label_set.id_
+
         if self.is_online:
-            raise ValueError(f"You cannot update Annotations once saved online: {self.get_link()}")
+            raise ValueError(f'You cannot update Annotations once saved online: {self.get_link()}')
             # update_annotation(id_=self.id_, document_id=self.document.id_, project_id=self.project.id_)
 
         if not self.is_online:
             response = post_document_annotation(
-                project_id=self.document.project.id_,
                 document_id=self.document.id_,
-                start_offset=self.start_offset,
-                end_offset=self.end_offset,
                 label_id=self.label.id_,
                 label_set_id=label_set_id,
                 confidence=self.confidence,
                 is_correct=self.is_correct,
                 revised=self.revised,
-                annotation_set=self.annotation_set,
-                # bboxes=self.bboxes,
-                # selection_bbox=self.selection_bbox,
-                page_number=self.page_number,
+                annotation_set_id=annotation_set_id,
+                session=self.document.project.session,
+                spans=self.spans,
             )
             if response.status_code == 201:
                 json_response = json.loads(response.text)
-                self.id_ = json_response["id"]
+                self.id_ = json_response['id']
                 new_annotation_added = True
             elif response.status_code == 403:
                 logger.error(response.text)
                 try:
-                    if "In one project you cannot label the same text twice." in response.text:
+                    if 'In one Project you cannot label the same text twice.' in response.text:
                         if document_annotations is None:
                             # get the Annotation
                             self.document.update()
                             document_annotations = self.document.annotations()
                         # get the id_ of the existing annotation
                         is_duplicated = False
                         for annotation in document_annotations:
                             if (
                                 annotation.start_offset == self.start_offset
                                 and annotation.end_offset == self.end_offset
                                 and annotation.label == self.label
                             ):
-                                logger.error(f"ID of annotation online: {annotation.id_}")
+                                logger.error(f'ID of annotation online: {annotation.id_}')
                                 self.id_ = annotation.id_
                                 is_duplicated = True
                                 break
 
                         # if there isn't a perfect match, the current Annotation is considered incorrect
                         if not is_duplicated:
                             self.is_correct = False
 
                         new_annotation_added = False
                     else:
-                        logger.exception(f"Unknown issue to create Annotation {self} in {self.document}")
+                        logger.exception(f'Unknown issue to create Annotation {self} in {self.document}')
                 except KeyError:
-                    logger.error(f"Not able to save annotation online: {response}")
+                    logger.error(f'Not able to save Annotation online: {response}')
         return new_annotation_added
 
     def regex_annotation_generator(self, regex_list) -> List[Span]:
         """
         Build Spans without Labels by regexes.
 
         :return: Return sorted list of Spans by start_offset
         """
         spans: List[Span] = []
         for regex in regex_list:
             dict_spans = regex_matches(doctext=self.document.text, regex=regex)
-            for offset in list(set((x['start_offset'], x['end_offset']) for x in dict_spans)):
+            for offset in list({(x['start_offset'], x['end_offset']) for x in dict_spans}):
                 try:
                     span = Span(start_offset=offset[0], end_offset=offset[1], annotation=self)
                     spans.append(span)
                 except ValueError as e:
                     logger.error(str(e))
         spans.sort()
         return spans
@@ -1581,162 +2573,456 @@
                 full_replacement = suggest_regex_for_string(span.offset_string, replace_characters=True)
                 regex_f = f'(?P<Label_{self.label.id_}_F_{self.id_}_{span.start_offset}>{full_replacement})'
                 self.token_append(new_regex=regex_f, regex_quality=2)
         return self._tokens
 
     # todo can we circumvent the combined tokens
     def regex(self):
-        """Return regex of this annotation."""
+        """Return regex of this Annotation."""
         return self.label.combined_tokens(categories=[self.document.category])
 
     def delete(self, delete_online: bool = True) -> None:
         """Delete Annotation.
 
         :param delete_online: Whether the Annotation is deleted online or only locally.
         """
         if self.document.is_online and delete_online:
-            delete_document_annotation(self.document.id_, self.id_, self.document.project.id_)
+            delete_document_annotation(
+                annotation_id=self.id_, session=self.document.project.session, delete_from_database=True
+            )
             self.document.update()
         else:
-            self.document._annotations.remove(self)
+            del self.document._annotations[(tuple(sorted(self._spans.keys())), self.label.name)]
+
+    def bbox(self) -> Bbox:
+        """Get Bbox encompassing all Annotation Spans."""
+        if self._bbox is None:
+            self._bbox = Bbox(
+                x0=min([span.bbox().x0 for span in self.spans]),
+                x1=max([span.bbox().x1 for span in self.spans]),
+                y0=min([span.bbox().y0 for span in self.spans]),
+                y1=max([span.bbox().y1 for span in self.spans]),
+                page=self.page,
+            )
+        return self._bbox
 
     @property
     def spans(self) -> List[Span]:
         """Return default entry to get all Spans of the Annotation."""
-        return sorted(self._spans)
+        return [self._spans[k] for k in sorted(self._spans.keys())]
+
+    @property
+    def bboxes(self) -> List[Dict]:
+        """Return the Bbox information for all Spans in serialized format.
+
+        This is useful for external integration (e.g. Konfuzio Server)."
+        """
+        return [span.bbox_dict() for span in self.spans]
 
     def lose_weight(self):
         """Delete data of the instance."""
         super().lose_weight()
         self._tokens = []
 
 
+class DocumentStatuses(Enum):
+    """
+    Define statuses of a Document's processing.
+
+    For more details see https://dev.konfuzio.com/sdk/explanations.html#document-concept
+    """
+
+    QUEUING_FOR_OCR = 0
+    OCR_IN_PROGRESS = 10
+    QUEUING_FOR_EXTRACTION = 1
+    EXTRACTION_IN_PROGRESS = 20
+    QUEUING_FOR_CATEGORIZATION = 3
+    CATEGORIZATION_IN_PROGRESS = 30
+    QUEUING_FOR_SPLITTING = 4
+    SPLITTING_IN_PROGRESS = 40
+    WAITING_FOR_SPLITTING_CONFIRMATION = 41
+    DONE = 2
+    COULD_NOT_BE_PROCESSED = 111
+
+
 class Document(Data):
-    """Access the information about one document, which is available online."""
+    """
+    Access the information about one Document, which is available online.
+
+    For more details see https://dev.konfuzio.com/sdk/explanations.html#document-concept
+    """
 
     def __init__(
         self,
         project: 'Project',
         id_: Union[int, None] = None,
         file_url: str = None,
-        status=None,
+        status: List[Union[int, str]] = None,
         data_file_name: str = None,
         is_dataset: bool = None,
         dataset_status: int = None,
         updated_at: str = None,
         assignee: int = None,
         category_template: int = None,  # fix for Konfuzio Server API, it's actually an ID of a Category
         category: Category = None,
+        category_confidence: Optional[float] = None,
+        category_is_revised: bool = False,
         text: str = None,
         bbox: dict = None,
-        strict_bbox_validation: bool = False,
+        bbox_validation_type=None,
         pages: list = None,
-        update: bool = None,
+        update: bool = False,
         copy_of_id: Union[int, None] = None,
         *args,
         **kwargs,
     ):
         """
         Create a Document and link it to its Project.
 
         :param id_: ID of the Document
         :param project: Project where the Document belongs to
-        :param file_url: URL of the document
-        :param status: Status of the document
-        :param data_file_name: File name of the document
+        :param file_url: URL of the Document
+        :param status: Status of the Document
+        :param data_file_name: File name of the Document
         :param is_dataset: Is dataset or not. (bool)
-        :param dataset_status: Dataset status of the Document (e.g. training)
+        :param dataset_status: Dataset status of the Document (e.g. Training)
         :param updated_at: Updated information
         :param assignee: Assignee of the Document
         :param bbox: Bounding box information per character in the PDF (dict)
-        :param strict_bbox_validation: If False, it allows bounding boxes to have zero width or height. This option is
-                        available and defaults to False for compatibility reasons since some OCR engines can sometimes
-                        return character level bboxes with zero width or height.
+        :param bbox_validation_type: One of ALLOW_ZERO_SIZE (default), STRICT, or DISABLED. Also see the `Bbox` class.
         :param pages: List of page sizes.
         :param update: Annotations, Annotation Sets will not be loaded by default. True will load it from the API.
                         False from local files
         :param copy_of_id: ID of the Document that originated the current Document
         """
         self._no_label_annotation_set = None
         self.id_local = next(Data.id_iter)
         self.id_ = id_
         self.assignee = assignee
-        self._annotations: List[Annotation] = None
+        self._annotations: {} = None
         self._annotation_sets: List[AnnotationSet] = None
         self.file_url = file_url
         self.is_dataset = is_dataset
         self.dataset_status = dataset_status
-        self.assignee = assignee
         self._update = update
         self.copy_of_id = copy_of_id
 
+        # The following variables come from the Server API
+        # self._category -> document level category from the "category" field
+        # self._category_confidence -> document level category confidence from the "category_confidence" field
+        # self.category_is_revised -> document level boolean flag from the "category_is_revised" field
         if project and category_template:
-            self.category = project.get_category_by_id(category_template)
+            self._category = project.get_category_by_id(category_template)
         elif category:
-            self.category = category
+            self._category = category
         else:
-            self.category = None
+            self._category = project.no_category
+        self._category_confidence = category_confidence
+        self.category_is_revised = category_is_revised
 
         if updated_at:
             self.updated_at = dateutil.parser.isoparse(updated_at)
         else:
             self.updated_at = None
 
         self.name = data_file_name
-        self.status = status  # status of document online
+        self.status = status  # status of Document online
         self.project = project
         self._force_offline = project._force_offline
         project.add_document(self)  # check for duplicates by ID before adding the Document to the project
 
         # use hidden variables to store low volume information in instance
         self._text: str = text
         self._text_hash = None
         self._characters: Dict[int, Bbox] = None
+        self._pages_char_bboxes = None
         self._bbox_hash = None
         self._bbox_json = bbox
-        self.bboxes_available: bool = True if (self.is_online or self._bbox_json) else False
-        self._strict_bbox_validation = strict_bbox_validation
-        self._hocr = None
+        self.bboxes_available: bool = bool(self.is_online or self._bbox_json)
+        self._bbox_validation_type = bbox_validation_type
+        if bbox_validation_type is None:
+            if self.project._strict_data_validation:
+                self._bbox_validation_type = BboxValidationTypes.ALLOW_ZERO_SIZE
+            else:
+                self._bbox_validation_type = BboxValidationTypes.DISABLED
         self._pages: List[Page] = []
         self._n_pages = None
+        self.text_encoded: List[int] = None
 
-        # prepare local setup for document
+        # prepare local setup for Document
         if self.is_online:
             pathlib.Path(self.document_folder).mkdir(parents=True, exist_ok=True)
-        self.annotation_file_path = os.path.join(self.document_folder, "annotations.json5")
-        self.annotation_set_file_path = os.path.join(self.document_folder, "annotation_sets.json5")
-        self.txt_file_path = os.path.join(self.document_folder, "document.txt")
-        self.hocr_file_path = os.path.join(self.document_folder, "document.hocr")
-        self.pages_file_path = os.path.join(self.document_folder, "pages.json5")
-        self.bbox_file_path = os.path.join(self.document_folder, "bbox.zip")
-        self.bio_scheme_file_path = os.path.join(self.document_folder, "bio_scheme.txt")
+        self.annotation_file_path = os.path.join(self.document_folder, 'annotations.json5')
+        self.annotation_set_file_path = os.path.join(self.document_folder, 'annotation_sets.json5')
+        self.txt_file_path = os.path.join(self.document_folder, 'document.txt')
+        self.pages_file_path = os.path.join(self.document_folder, 'pages.json5')
+        self.bbox_file_path = os.path.join(self.document_folder, 'bbox.zip')
+        self.bio_scheme_file_path = os.path.join(self.document_folder, 'bio_scheme.txt')
+
+        bbox_file_exists = is_file(self.bbox_file_path, raise_exception=False)
+        self.bboxes_available: bool = self.is_online or self._bbox_json or bbox_file_exists
 
         if pages:
-            self.pages()  # create page instances
+            self.pages()  # create Page instances
 
     def __repr__(self):
         """Return the name of the Document incl. the ID."""
-        if self.copy_of_id:
-            return f"Document {self.name} ({self.copy_of_id})"
+        if self.id_ is None:
+            return f'Virtual Document {self.name} ({self.copy_of_id})'
         else:
-            return f"Document {self.name} ({self.id_})"
+            return f'Document {self.name} ({self.id_})'
+
+    @property
+    def ocr_ready(self):
+        """Check if Document OCR is ready."""
+        return self.text is not None
+
+    def update_meta_data(
+        self,
+        assignee: int = None,
+        category_template: int = None,
+        category: Category = None,
+        data_file_name: str = None,
+        dataset_status: int = None,
+        status: List[Union[int, str]] = None,
+        **kwargs,
+    ):
+        """Update document metadata information."""
+        self.assignee = assignee
+
+        if self.project and category_template:
+            self._category = self.project.get_category_by_id(category_template)
+        elif category:
+            self._category = category
+        else:
+            self._category = None
+
+        self.name = data_file_name
+
+        self.status = status
+
+        self.dataset_status = dataset_status
+
+    def save_meta_data(self):
+        """Save local changes to Document metadata to server."""
+        update_document_konfuzio_api(
+            document_id=self.id_,
+            file_name=self.name,
+            dataset_status=self.dataset_status,
+            assignee=self.assignee,
+            session=self.project.session,
+        )
+
+    def save(self):
+        """Save all local changes to Document to server."""
+        self.save_meta_data()
+
+        for annotation in self.annotations(use_correct=False):
+            if not annotation.is_online:
+                try:
+                    annotation.save()
+                except HTTPError as e:
+                    logger.error(str(e))
+
+    @classmethod
+    def from_file(
+        self,
+        path: str,
+        project: 'Project',
+        dataset_status: int = 0,
+        category_id: Optional[int] = None,
+        callback_url: str = '',
+        timeout: Optional[int] = None,
+        sync: bool = True,
+    ) -> 'Document':
+        """
+        Initialize Document from file with synchronous API call.
+
+        This class method will wait for the document to be processed by the server
+        and then return the new Document. This may take a bit of time. When uploading
+        many Documents, it is advised to set the sync option to False method.
+
+        :param path: Path to file to be uploaded
+        :param project: If to filter by correct annotations
+        :param dataset_status: Dataset status of the Document (None: 0 Preparation: 1 Training: 2 Test: 3 Excluded: 4)
+        :param category_id: Category the Document belongs to (if unset, it will be assigned one by the server)
+        :param callback_url: Callback URL receiving POST call once extraction is done
+        :param timeout: Number of seconds to wait for response from the server
+        :param sync: Whether to wait for the file to be processed by the server
+        :return: New Document
+        """
+        get_file_type_and_extension(path)  # check if file is valid
+        response = upload_file_konfuzio_api(
+            path,
+            project_id=project.id_,
+            dataset_status=dataset_status,
+            category_id=category_id,
+            callback_url=callback_url,
+            sync=sync,
+            session=konfuzio_session(timeout=timeout),
+        )
+        response = response.json()
+        new_document_id = response['id']
+
+        if sync:
+            status = [
+                response['status_data'],
+                [status.name for status in DocumentStatuses if status.value == response['status_data']][0],
+            ]
+            if status[0] == 2:
+                logger.debug(f'Document status code {status[0]}: {status[1]}')
+            else:
+                logger.warning(f'Document status code {status[0]}: {status[1]}')
+            assert project.id_ == response['project'], 'Project id_ of uploaded file does not match'
+            document = Document(
+                id_=new_document_id,
+                project=project,
+                update=True,
+                category_template=category_id if category_id else response['category'],
+                text=response['text'],
+                status=status[0],  # we want a numeric representation of status, e.g. 2, not the textual, e.g. "Done"
+                data_file_name=response['data_file_name'],
+                file_url=response['file_url'],
+                dataset_status=dataset_status,
+            )
+        else:
+            document = Document(
+                id_=new_document_id,
+                project=project,
+                update=True,
+                category_template=category_id,
+                status=[0],  # numeric representation of a status that means "queueing for ocr"
+                data_file_name=response['data_file_name'],
+                dataset_status=dataset_status,
+            )
+
+        return document
 
     @property
     def file_path(self):
         """Return path to file."""
         return os.path.join(self.document_folder, amend_file_name(self.name))
 
     @property
+    def category_annotations(self) -> List[CategoryAnnotation]:
+        """
+        Collect Category Annotations and average confidence across all Pages.
+
+        :return: List of Category Annotations, one for each Category.
+        """
+        category_annotations = []
+        for category in self.project.categories:
+            if category != self.project.no_category:
+                confidence = 0
+                for page in self.pages():
+                    confidence += page.get_category_annotation(category).confidence
+                confidence /= self.number_of_pages
+                if (confidence == 0.0) and (category == self._category):
+                    confidence = self._category_confidence
+                category_annotation = CategoryAnnotation(category=category, document=self, confidence=confidence)
+                category_annotations.append(category_annotation)
+        return category_annotations
+
+    @property
+    def maximum_confidence_category_annotation(self) -> Optional[CategoryAnnotation]:
+        """
+        Get the human revised Category Annotation of this Document, or the highest confidence one if not revised.
+
+        :return: The found Category Annotation, or None if not present.
+        """
+        if self.category != self.project.no_category:
+            # there is a unique Category Annotation per Category associated to this Document
+            # by construction in Document.category_annotations
+            return [
+                category_annotation
+                for category_annotation in self.category_annotations
+                if category_annotation.category == self._category
+            ][0]
+        category_annotation = sorted(self.category_annotations, key=lambda x: x.confidence)[-1]
+        if category_annotation.confidence != 0.0:
+            return category_annotation
+        return None
+
+    @property
+    def maximum_confidence_category(self) -> Optional[Category]:
+        """
+        Get the human revised Category of this Document, or the highest confidence one if not revised.
+
+        :return: The found Category, or None if not present.
+        """
+        if self.maximum_confidence_category_annotation is not None:
+            return self.maximum_confidence_category_annotation.category
+        return self.project.no_category
+
+    @property
+    def category(self) -> Category:
+        """
+        Return the Category of the Document.
+
+        The Category of a Document is only defined as long as all Pages have the same Category. Otherwise, the Document
+        should probably be split into multiple Documents with a consistent Category assignment within their Pages, or
+        the Category for each Page should be manually revised.
+        """
+        if not self.pages():
+            return self._category
+        all_pages_have_same_category = len({page.category for page in self.pages()} - {self.project.no_category}) == 1
+        if all_pages_have_same_category:
+            self._category = self.pages()[0].category
+        else:
+            self._category = self.project.no_category
+        return self._category
+
+    def get_segmentation(self, timeout: Optional[int] = None, num_retries: Optional[int] = None) -> List:
+        """
+        Retrieve the segmentation results for the Document.
+
+        :param timeout: Number of seconds to wait for response from the server.
+        :param num_retries: Number of retries if the request fails.
+        :return: A list of segmentation results for each Page in the Document.
+        """
+        document = self.project.get_document_by_id(self.copy_of_id) if self.copy_of_id else self
+        if any(page._segmentation is None for page in document.pages()):
+            document_id = document.id_
+            detectron_document_results = get_results_from_segmentation(
+                document_id, self.project.id_, session=konfuzio_session(timeout=timeout, num_retries=num_retries)
+            )
+            assert len(detectron_document_results) == self.number_of_pages
+            for page_index, detectron_page_result in enumerate(detectron_document_results):
+                document.get_page_by_index(page_index)._segmentation = detectron_page_result
+        else:
+            detectron_document_results = [page._segmentation for page in document.pages()]
+
+        return detectron_document_results
+
+    def set_category(self, category: Category) -> None:
+        """Set the Category of the Document and the Category of all of its Pages as revised."""
+        if not category:
+            category = self.project.no_category
+        logger.info(f'Setting Category of {self} to {category}.')
+        if category not in [self._category, self.project.no_category] and (
+            self._category and self._category.name != self.project.no_category.name
+        ):
+            raise ValueError(
+                'We forbid changing Category when already existing, because this requires some validations that are '
+                'currently implemented in the Konfuzio Server. We recommend changing the Category of a Document via '
+                'the Konfuzio Server.'
+            )
+        for page in self.pages():
+            page.set_category(category)
+        self._category = category
+        self.category_is_revised = True
+
+    @property
     def ocr_file_path(self):
         """Return path to OCR PDF file."""
-        return os.path.join(self.document_folder, amend_file_name(self.name, append_text="ocr", new_extension=".pdf"))
+        return os.path.join(self.document_folder, amend_file_name(self.name, append_text='ocr', new_extension='.pdf'))
 
     @property
     def number_of_pages(self) -> int:
-        """Calculate the number of pages."""
+        """Calculate the number of Pages."""
         if self._n_pages is None:
             self._n_pages = len(self.text.split('\f'))
         return self._n_pages
 
     @property
     def number_of_lines(self) -> int:
         """Calculate the number of lines."""
@@ -1749,69 +3035,86 @@
 
         We need to load the Annotation Sets from Server first (call self.annotation_sets()).
         If we create the no_label_annotation_set in the first place, the data from the Server is not be loaded
         anymore because _annotation_sets will no longer be None.
         """
         if self._no_label_annotation_set is None:
             self.annotation_sets()
-            self._no_label_annotation_set = AnnotationSet(document=self, label_set=self.project.no_label_set)
+
+            # Find no label annotation set
+            self._no_label_annotation_set = next(
+                (
+                    annotation_set
+                    for annotation_set in self._annotation_sets
+                    if annotation_set.label_set == self.project.no_label_set
+                ),
+                None,
+            )
+
+            # Create no label annotation set if not found
+            if self._no_label_annotation_set is None:
+                self._no_label_annotation_set = AnnotationSet(document=self, label_set=self.project.no_label_set)
 
         return self._no_label_annotation_set
 
     def spans(
         self,
         label: Label = None,
         use_correct: bool = False,
         start_offset: int = 0,
         end_offset: int = None,
         fill: bool = False,
     ) -> List[Span]:
         """Return all Spans of the Document."""
-        spans = []
+        spans = {}
 
         annotations = self.annotations(
             label=label, use_correct=use_correct, start_offset=start_offset, end_offset=end_offset, fill=fill
         )
 
         for annotation in annotations:
             for span in annotation.spans:
-                if span not in spans:
-                    spans.append(span)
+                k = (span.start_offset, span.end_offset)
+                if k not in spans:
+                    spans[k] = span
 
         # if self.spans() == list(set(self.spans())):
-        #     # todo deduplicate Spans. One text offset in a document can ber referenced by many Spans of Annotations
+        #     # todo deduplicate Spans. One text offset in a Document can ber referenced by many Spans of Annotations
         #     raise NotImplementedError
 
-        return sorted(spans)
+        return [spans[k] for k in sorted(spans.keys())]
 
-    def eval_dict(self, use_correct=False) -> List[dict]:
+    def eval_dict(self, use_view_annotations=False, use_correct=False, ignore_below_threshold=False) -> List[dict]:
         """Use this dict to evaluate Documents. The speciality: For every Span of an Annotation create one entry."""
         result = []
-        annotations = self.annotations(use_correct=use_correct)
+        if use_view_annotations:
+            annotations = self.view_annotations()
+        else:
+            annotations = self.annotations(use_correct=use_correct, ignore_below_threshold=ignore_below_threshold)
         if not annotations:  # if there are no Annotations in this Documents
             result.append(Span(start_offset=0, end_offset=0).eval_dict())
         else:
             for annotation in annotations:
                 result += annotation.eval_dict
 
         return result
 
     def check_bbox(self) -> None:
         """
-        Run validation checks on the document text and bboxes.
+        Run validation checks on the Document text and bboxes.
 
-        This is run when the document is initialized, and usually it's not needed to be run again because a document's
+        This is run when the Document is initialized, and usually it's not needed to be run again because a Document's
         text and bboxes are not expected to change within the Konfuzio Server.
 
         You can run this manually instead if your pipeline allows changing the text or the bbox during the lifetime of
         a document. Will raise ValueError if the bboxes don't match with the text of the document, or if bboxes have
         invalid coordinates (outside page borders) or invalid size (negative width or height).
 
-        This check is usually slow, and it can be made faster by calling document.set_text_bbox_hashes() right after
-        initializing the document, which will enable running a hash comparison during this check.
+        This check is usually slow, and it can be made faster by calling Document.set_text_bbox_hashes() right after
+        initializing the Document, which will enable running a hash comparison during this check.
         """
         warn('WIP: Modifications before the next stable release expected.', FutureWarning, stacklevel=2)
         if self._check_text_or_bbox_modified():
             self._characters = None
             _ = self.bboxes
 
     def __deepcopy__(self, memo) -> 'Document':
@@ -1822,115 +3125,140 @@
             project=self.project,
             category=self.category,
             text=self.text,
             copy_of_id=copy_id,
             bbox=self.get_bbox(),
         )
         for page in self.pages():
+            copy_id = page.id_ if page.id_ else page.copy_of_id
             _ = Page(
                 id_=None,
                 document=document,
                 start_offset=page.start_offset,
                 end_offset=page.end_offset,
+                copy_of_id=copy_id,
                 number=page.number,
                 original_size=(page.width, page.height),
+                image_size=(page.image_width, page.image_height),
             )
+            _.image_bytes = page.image_bytes
         return document
 
     def check_annotations(self, update_document: bool = False) -> bool:
         """Check if Annotations are valid - no duplicates and correct Category."""
         valid = True
         assignee = None
 
         try:
             self.get_annotations()
 
         except ValueError as error_message:
             valid = False
 
-            if "is a duplicate of" in str(error_message):
+            if 'is a duplicate of' in str(error_message):
                 logger.error(f'{self} has duplicated Annotations.')
                 assignee = 1101  # duplicated-annotation@konfuzio.com
 
-            elif "related to" in str(error_message):
+            elif 'related to' in str(error_message):
                 logger.error(f'{self} has Annotations from an incorrect Category.')
                 assignee = 1118  # category-issue@konfuzio.com
 
             else:
                 raise ValueError('Error not expected.')
 
         if update_document and assignee is not None:
             # set the dataset status of the Document to Excluded
-            update_document_konfuzio_api(document_id=self.id_, file_name=self.name, dataset_status=4, assignee=assignee)
+            update_document_konfuzio_api(
+                document_id=self.id_,
+                file_name=self.name,
+                dataset_status=4,
+                assignee=assignee,
+                session=self.project.session,
+            )
 
         return valid
 
-    def annotation_sets(self):
-        """Return Annotation Sets of Documents."""
-        if self._annotation_sets is not None:
-            return self._annotation_sets
-        if self.is_online and not is_file(self.annotation_set_file_path, raise_exception=False):
-            self.download_document_details()
-        if is_file(self.annotation_set_file_path, raise_exception=False):
-            with open(self.annotation_set_file_path, "r") as f:
-                raw_annotation_sets = json.load(f)
-            # first load all Annotation Sets before we create Annotations
-            for raw_annotation_set in raw_annotation_sets:
-                _ = AnnotationSet(
-                    id_=raw_annotation_set["id"],
-                    document=self,
-                    label_set=self.project.get_label_set_by_id(raw_annotation_set["section_label"]),
-                )
-        elif self._annotation_sets is None:
-            self._annotation_sets = []  # Annotation sets cannot be loaded from Konfuzio Server
-        return self._annotation_sets
+    def annotation_sets(self, label_set: LabelSet = None) -> List[AnnotationSet]:
+        """
+        Return Annotation Sets of Documents.
+
+        :param label_set: Label Set for which to filter the Annotation Sets.
+        :return: Annotation Sets of Documents.
+        """
+        if self._annotation_sets is None:
+            if self.is_online and not is_file(self.annotation_set_file_path, raise_exception=False):
+                self.download_document_details()
+            if is_file(self.annotation_set_file_path, raise_exception=False):
+                with open(self.annotation_set_file_path, 'r') as f:
+                    raw_annotation_sets = json.load(f)
+                # first load all Annotation Sets before we create Annotations
+                for raw_annotation_set in raw_annotation_sets:
+                    # for backwards compatibility
+                    if 'label_set' in raw_annotation_set.keys():
+                        label_set_id = raw_annotation_set['label_set']['id']
+                    elif 'section_label' in raw_annotation_set.keys():
+                        label_set_id = raw_annotation_set['section_label']
+                    _ = AnnotationSet(
+                        id_=raw_annotation_set['id'],
+                        document=self,
+                        label_set=self.project.get_label_set_by_id(label_set_id),
+                    )
+            elif self._annotation_sets is None:
+                self._annotation_sets = []  # Annotation sets cannot be loaded from Konfuzio Server
+        annotation_sets = self._annotation_sets
+        if label_set:
+            # filter by Label Set given as argument
+            annotation_sets = [
+                annotation_set for annotation_set in annotation_sets if annotation_set.label_set == label_set
+            ]
+        return annotation_sets
 
     def annotations(
         self,
         label: Label = None,
         use_correct: bool = True,
         ignore_below_threshold: bool = False,
         start_offset: int = 0,
         end_offset: int = None,
         fill: bool = False,
     ) -> List[Annotation]:
         """
         Filter available annotations.
 
         :param label: Label for which to filter the Annotations.
-        :param use_correct: If to filter by correct annotations.
-        :param ignore_below_threshold: To filter out annotations with confidence below Label prediction threshold.
+        :param use_correct: If to filter by correct Annotations.
+        :param ignore_below_threshold: To filter out Annotations with confidence below Label prediction threshold.
         :return: Annotations in the document.
         """
         self.get_annotations()
         start_offset = max(start_offset, 0)
         if end_offset:
             end_offset = min(end_offset, len(self.text))
         annotations: List[Annotation] = []
         add = False
-        for annotation in self._annotations:
+        for annotation in self._annotations.values():
             # filter by correct information
             if not annotation.is_correct:
                 if ignore_below_threshold and (
                     not annotation.confidence or annotation.confidence < annotation.label.threshold
                 ):
                     continue
             for span in annotation.spans:
                 if (use_correct and annotation.is_correct) or not use_correct:
                     # todo: add option to filter for overruled Annotations where mult.=F
                     # todo: add option to filter for overlapping Annotations, `add_annotation` just checks for identical
-                    # filter by start and end offset, include annotations that extend into the offset
+                    # filter by start and end offset, include Annotations that extend into the offset
                     if start_offset is not None and end_offset is not None:  # if the start and end offset are specified
                         latest_start = max(span.start_offset, start_offset)
                         earliest_end = min(span.end_offset, end_offset)
                         is_overlapping = latest_start - earliest_end < 0
                     else:
                         is_overlapping = True
 
-                    if label is not None:  # filter by label
+                    if label is not None:  # filter by Label
                         if label == annotation.label and is_overlapping:
                             add = True
                     elif is_overlapping:
                         add = True
             # as multiline Annotations will be added twice
             if add:
                 annotations.append(annotation)
@@ -1983,54 +3311,56 @@
             key=lambda x: (
                 not x.is_correct,  # x.is_correct == True first
                 -x.confidence if x.confidence else 0,  # higher confidence first
                 min([span.start_offset for span in x.spans]),
             ),
         )
 
-        no_label_duplicates = set()  # for top annotation filter
+        no_label_duplicates = set()  # for top Annotation filter
         for annotation in priority_annotations:
             if annotation.confidence is not None and annotation.label.threshold > annotation.confidence:
                 continue
             if not annotation.is_correct and annotation.revised:  # if marked as incorrect by user
                 continue
             if annotation.label is self.project.no_label:
                 continue
             spans_num = 0
             for span in annotation.spans:
                 for i in range(span.start_offset, span.end_offset):
                     spans_num |= 1 << i
             if spans_num & filled:
                 # if there's overlap
                 continue
-            # if (
-            #     annotation.is_correct is False
-            #     and annotation.label.has_multiple_top_candidates is False
-            #     and annotation.label.id_ in no_label_duplicates
-            # ):
-            #     continue
+            if (
+                annotation.is_correct is False
+                and annotation.label.has_multiple_top_candidates is False
+                and (annotation.label.id_, annotation.annotation_set.id_) in no_label_duplicates
+            ):
+                continue
             annotations.append(annotation)
             filled |= spans_num
             if not annotation.label.has_multiple_top_candidates:
-                no_label_duplicates.add(annotation.label.id_)
+                no_label_duplicates.add((annotation.label.id_, annotation.annotation_set.id_))
 
         return sorted(annotations)
 
     def lose_weight(self):
         """Remove NO_LABEL, wrong and below threshold Annotations."""
         super().lose_weight()
+        self._bbox_json = None
+        self._characters = None
         for annotation in self.annotations(use_correct=False, ignore_below_threshold=False):
             if annotation.label is self.project.no_label:
-                logger.info("no_label")
-                annotation.delete()
+                annotation.delete(delete_online=False)
             elif not annotation.is_correct and (
                 not annotation.confidence or annotation.label.threshold > annotation.confidence or annotation.revised
             ):
-                logger.info(annotation.confidence)
-                annotation.delete()
+                annotation.delete(delete_online=False)
+            else:
+                annotation.lose_weight()
 
     @property
     def document_folder(self):
         """Get the path to the folder where all the Document information is cached locally."""
         return os.path.join(self.project.documents_folder, str(self.id_))
 
     def get_file(self, ocr_version: bool = True, update: bool = False):
@@ -2041,112 +3371,161 @@
         :param update: Update the downloaded file even if it is already available
         :return: Path to the selected file.
         """
         if ocr_version:
             file_path = self.ocr_file_path
         else:
             file_path = self.file_path
-
-        if self.status[0] == 2 and (not file_path or not is_file(file_path, raise_exception=False) or update):
-            pdf_content = download_file_konfuzio_api(self.id_, ocr=ocr_version, session=self.session)
-            with open(file_path, "wb") as f:
+        # backward compatibility check
+        if isinstance(self.status, int) or not self.status:
+            status = self.status
+        else:
+            status = self.status[0]
+        if status == DocumentStatuses.DONE.value and (
+            not file_path or not is_file(file_path, raise_exception=False) or update
+        ):
+            pdf_content = download_file_konfuzio_api(self.id_, ocr=ocr_version, session=self.project.session)
+            with open(file_path, 'wb') as f:
                 f.write(pdf_content)
 
         return file_path
 
     def get_images(self, update: bool = False):
         """
         Get Document Pages as PNG images.
 
         :param update: Update the downloaded images even they are already available
         :return: Path to PNG files.
         """
         return [page.get_image(update=update) for page in self.pages()]
 
     def download_document_details(self):
-        """Retrieve data from a Document online in case documented has finished processing."""
-        if self.is_online and self.status and self.status[0] == 2:
-            data = get_document_details(document_id=self.id_, project_id=self.project.id_, session=self.session)
+        """
+        Retrieve data from a Document online in case Document has finished processing.
 
+        Data includes Document's status, URL of its file, name of its file, date of
+        las update, its text and pagination, Annotations and Annotation Sets; optionally,
+        Category information.
+        """
+        if self.is_online:
+            data = get_document_details(document_id=self.id_, session=self.project.session)
+            self.status = data['status_data']
+            self.file_url = data['file_url']
+            self.name = data['data_file_name']
+            self.updated_at = dateutil.parser.isoparse(data['updated_at'])
+            if data['category']:
+                self._category = self.project.get_category_by_id(data['category'])
             # write a file, even there are no annotations to support offline work
-            with open(self.annotation_file_path, "w") as f:
-                json.dump(data["annotations"], f, indent=2, sort_keys=True)
-
-            with open(self.annotation_set_file_path, "w") as f:
-                json.dump(data["sections"], f, indent=2, sort_keys=True)
-
-            with open(self.txt_file_path, "w", encoding="utf-8") as f:
-                f.write(data["text"])
+            annotations = get_document_annotations(document_id=self.id_, session=self.project.session)['results']
+            with open(self.annotation_file_path, 'w') as f:
+                json.dump(annotations, f, indent=2, sort_keys=True)
+
+            with open(self.annotation_set_file_path, 'w') as f:
+                json.dump(data['annotation_sets'], f, indent=2, sort_keys=True)
+
+            with open(self.txt_file_path, 'w', encoding='utf-8') as f:
+                if data['text']:
+                    f.write(data['text'])
 
-            with open(self.pages_file_path, "w") as f:
-                json.dump(data["pages"], f, indent=2, sort_keys=True)
+            with open(self.pages_file_path, 'w') as f:
+                json.dump(data['pages'], f, indent=2, sort_keys=True)
         else:
             raise NotImplementedError
 
         return self
 
     def add_annotation(self, annotation: Annotation):
-        """Add an annotation to a document.
+        """Add an Annotation to a Document.
 
-        :param annotation: Annotation to add in the document
-        :return: Input annotation.
+        The Annotation is only added to the Document if the data validation tests are passing for this Annotation.
+        See https://dev.konfuzio.com/sdk/tutorials/data_validation/index.html
+
+        :param annotation: Annotation to add in the Document
+        :return: Input Annotation.
         """
         if self._annotations is None:
             self.annotations()
-        if annotation not in self._annotations:
+
+        # Keep compatibility with older AI versions that use lists for spans
+        if isinstance(annotation._spans, list):
+            ann_key = (
+                tuple(sorted((s.start_offset, s.end_offset) for s in annotation._spans)),
+                annotation.label.name,
+            )
+        else:
+            ann_key = (tuple(sorted(annotation._spans.keys())), annotation.label.name)
+
+        duplicated = self._annotations.get(ann_key, None)
+
+        if not duplicated:
             # Hotfix Text Annotation Server:
             #  Annotation belongs to a Label / Label Set that does not relate to the Category of the Document.
             # todo: add test that the Label and Label Set of an Annotation belong to the Category of the Document
-            if self.category is not None:
+            if self.category != self.project.no_category:
                 if annotation.label_set is not None:
                     if annotation.label_set.categories:
-                        if self.category in annotation.label_set.categories:
-                            self._annotations.append(annotation)
+                        if (self.category in annotation.label_set.categories) or (
+                            annotation.label is self.project.no_label
+                        ):
+                            self._annotations[ann_key] = annotation
                         else:
-                            raise ValueError(
-                                f'We cannot add {annotation} related to {annotation.label_set.categories} to {self} '
-                                f'as the document has {self.category}'
+                            exception_or_log_error(
+                                msg=f'We cannot add {annotation} related to {annotation.label_set.categories} to {self}'
+                                f' as the Document has {self.category}',
+                                fail_loudly=self.project._strict_data_validation,
+                                exception_type=ValueError,
                             )
                     else:
                         raise ValueError(f'{annotation} uses Label Set without Category, cannot be added to {self}.')
                 else:
                     raise ValueError(f'{annotation} has no Label Set, which cannot be added to {self}.')
             else:
-                raise ValueError(f'We cannot add {annotation} to {self} where the category is {self.category}')
+                if annotation.label is self.project.no_label and annotation.label_set is self.project.no_label_set:
+                    self._annotations[ann_key] = annotation
+                else:
+                    raise ValueError(f'We cannot add {annotation} to {self} where the Category is {self.category}')
         else:
-            duplicated = [x for x in self._annotations if x == annotation]
-            raise ValueError(f'In {self} the {annotation} is a duplicate of {duplicated} and will not be added.')
+            exception_or_log_error(
+                msg=f'In {self} the {annotation} is a duplicate of {duplicated} and will not be added.',
+                fail_loudly=self.project._strict_data_validation,
+                exception_type=ValueError,
+            )
 
         return self
 
     def get_annotation_by_id(self, annotation_id: int) -> Annotation:
         """
-        Return an Annotation by ID, searching within the document.
+        Return an Annotation by ID, searching within the Document.
 
-        :param id_: ID of the Annotation to get.
+        :param annotation_id: ID of the Annotation to get.
         """
         result = None
         if self._annotations is None:
             self.annotations()
-        for annotation in self._annotations:
+        for annotation in self._annotations.values():
             if annotation.id_ == annotation_id:
                 result = annotation
                 break
         if result:
             return result
         else:
-            raise IndexError(f"Annotation {annotation_id} is not part of {self}.")
+            raise IndexError(f'Annotation {annotation_id} is not part of {self}.')
 
     def add_annotation_set(self, annotation_set: AnnotationSet):
-        """Add the Annotation Sets to the document."""
+        """Add the Annotation Sets to the Document."""
         if annotation_set.document and annotation_set.document != self:
-            raise ValueError('One Annotation Set must only belong to one document.')
+            raise ValueError('One Annotation Set must only belong to one Document.')
         if self._annotation_sets is None:
             self._annotation_sets = []
         if annotation_set not in self._annotation_sets:
+            if annotation_set.label_set.has_multiple_annotation_sets is False:
+                # if the Label Set does not allow multiple Annotation Sets, check if there is already an Annotation Set
+                # with the same Label Set
+                if annotation_set.label_set in [x.label_set for x in self._annotation_sets]:
+                    logger.error(f'In {self} the {annotation_set.label_set} is already used by another Annotation Set.')
             self._annotation_sets.append(annotation_set)
         else:
             raise ValueError(f'In {self} the {annotation_set} is a duplicate and will not be added.')
         return self
 
     def get_annotation_set_by_id(self, id_: int) -> AnnotationSet:
         """
@@ -2159,136 +3538,169 @@
             self.annotation_sets()
         for annotation_set in self._annotation_sets:
             if annotation_set.id_ == id_:
                 result = annotation_set
         if result:
             return result
         else:
-            logger.error(f"Annotation Set {id_} is not part of Document {self.id_}.")
-            raise IndexError
+            raise IndexError(f'Annotation Set {id_} is not part of Document {self.id_}.')
+
+    @property
+    def default_annotation_set(self) -> AnnotationSet:
+        """Return the default Annotation Set of the Document."""
+        if self._annotation_sets is None:
+            self.annotation_sets()
+        for annotation_set in self._annotation_sets:
+            if annotation_set.is_default:
+                return annotation_set
+        default_label_set = self.category.default_label_set
+        default_annotation_set = AnnotationSet(
+            id_=next(Data.id_iter),
+            document=self,
+            label_set=default_label_set,
+        )
+        return default_annotation_set
 
     def get_text_in_bio_scheme(self, update=False) -> List[Tuple[str, str]]:
         """
         Get the text of the Document in the BIO scheme.
 
         :param update: Update the bio annotations even they are already available
         :return: list of tuples with each word in the text and the respective label
         """
         converted_text = []
         if not is_file(self.bio_scheme_file_path, raise_exception=False) or update:
             converted_text = convert_to_bio_scheme(self)
-            with open(self.bio_scheme_file_path, "w", encoding="utf-8") as f:
+            with open(self.bio_scheme_file_path, 'w', encoding='utf-8') as f:
                 for word, tag in converted_text:
-                    f.writelines(word + " " + tag + "\n")
-                f.writelines("\n")
+                    f.writelines(word + ' ' + tag + '\n')
+                f.writelines('\n')
         else:
-            with open(self.bio_scheme_file_path, "r", encoding="utf-8") as f:
+            with open(self.bio_scheme_file_path, 'r', encoding='utf-8') as f:
                 for line in f.readlines():
                     if not line.strip():
                         continue
                     split_line = line.strip().split(' ')
                     word = split_line[0]
                     tag = ' '.join(split_line[1:])  # tag allowed to have multiple words
                     converted_text.append((word, tag))
 
         return converted_text
 
     def get_bbox(self) -> Dict:
         """
         Get bbox information per character of file. We don't store bbox as an attribute to save memory.
 
-        :return: Bounding box information per character in the document.
+        :return: Bounding box information per character in the Document.
         """
         if self._bbox_json:
             bbox = self._bbox_json
         elif is_file(self.bbox_file_path, raise_exception=False):
-            with zipfile.ZipFile(self.bbox_file_path, "r") as archive:
+            with zipfile.ZipFile(self.bbox_file_path, 'r') as archive:
                 bbox = json.loads(archive.read('bbox.json5'))
-        elif self.is_online and self.status and self.status[0] == 2:
+        elif self.is_online and self.status and self.status == DocumentStatuses.DONE.value:
             # todo check for self.project.id_ and self.id_ and ?
-            logger.warning(f'Start downloading bbox files of {len(self.text)} characters for {self}.')
-            bbox = get_document_details(document_id=self.id_, project_id=self.project.id_, extra_fields="bbox")['bbox']
+            logger.info(f'Start downloading bbox files of {len(self.text)} characters for {self}.')
+            bbox = get_document_bbox(document_id=self.id_, session=self.project.session)['bbox']
             # Use the `zipfile` module: `compresslevel` was added in Python 3.7
             with zipfile.ZipFile(
-                self.bbox_file_path, mode="w", compression=zipfile.ZIP_DEFLATED, compresslevel=9
+                self.bbox_file_path, mode='w', compression=zipfile.ZIP_DEFLATED, compresslevel=9
             ) as zip_file:
                 # Dump JSON data
                 dumped: str = json.dumps(bbox, indent=2, sort_keys=True)
                 # Write the JSON data into `data.json` *inside* the ZIP file
                 zip_file.writestr('bbox.json5', data=dumped)
                 # Test integrity of compressed archive
                 zip_file.testzip()
         else:
             self.bboxes_available = False
             bbox = {}
 
         return bbox
 
+    def get_bbox_by_page(self, page_index: int) -> Dict[str, Dict]:
+        """Return list of all bboxes in a Page."""
+        if not self._pages_char_bboxes:
+            self._pages_char_bboxes: List[Dict[str, Dict]] = [{} for _ in self.pages()]
+            for char_index, bbox in self.get_bbox().items():
+                bbox['char_index'] = int(char_index)
+                # for backwards compatibility
+                if 'page_index' in bbox.keys():
+                    bbox_page_index = bbox['page_index']
+                else:
+                    bbox_page_index = bbox['page_number'] - 1
+                self._pages_char_bboxes[bbox_page_index][char_index] = bbox
+        return self._pages_char_bboxes[page_index]
+
     @property
     def _hashable_characters(self) -> Optional[frozenset]:
         """Convert bbox dict into a hashable type."""
         return frozenset(self._characters) if self._characters is not None else None
 
     def set_text_bbox_hashes(self) -> None:
-        """Update hashes of document text and bboxes. Can be used for checking later on if any changes happened."""
+        """Update hashes of Document text and bboxes. Can be used for checking later on if any changes happened."""
         self._text_hash = hash(self._text)
         self._bbox_hash = hash(self._hashable_characters)
 
     def _check_text_or_bbox_modified(self) -> bool:
-        """Check if either the document text or its bboxes have been modified in memory."""
+        """Check if either the Document text or its bboxes have been modified in memory."""
         text_modified = self._text_hash != hash(self._text)
         bbox_modified = self._bbox_hash != hash(self._hashable_characters)
         return text_modified or bbox_modified
 
     @property
     def bboxes(self) -> Dict[int, Bbox]:
         """Use the cached bbox version."""
-        warn('WIP: Modifications before the next stable release expected.', FutureWarning, stacklevel=2)
         if self.bboxes_available and self._characters is None:
             bbox = self.get_bbox()
             boxes = {}
             for character_index, box in bbox.items():
                 x0 = box.get('x0')
                 x1 = box.get('x1')
                 y0 = box.get('y0')
                 y1 = box.get('y1')
-                page_index = box.get('page_number') - 1
+                if 'page_index' in box.keys():
+                    page_index = box.get('page_index')
+                else:
+                    page_index = box.get('page_number') - 1
                 page = self.get_page_by_index(page_index=page_index)
                 box_character = box.get('text')
                 document_character = self.text[int(character_index)]
                 if box_character not in [' ', '\f', '\n'] and box_character != document_character:
-                    raise ValueError(
-                        f'{self} Bbox provides Character "{box_character}" document text refers to '
-                        f'"{document_character}" with ID "{character_index}".'
+                    exception_or_log_error(
+                        msg=f'{self} Bbox provides Character "{box_character}" Document text refers to '
+                        f'"{document_character}" with ID "{character_index}".',
+                        fail_loudly=self.project._strict_data_validation,
+                        exception_type=ValueError,
                     )
                 boxes[int(character_index)] = Bbox(
-                    x0=x0, x1=x1, y0=y0, y1=y1, page=page, strict_validation=self._strict_bbox_validation
+                    x0=x0, x1=x1, y0=y0, y1=y1, page=page, validation=self._bbox_validation_type
                 )
             self._characters = boxes
         return self._characters
 
     def set_bboxes(self, characters: Dict[int, Bbox]):
         """Set character Bbox dictionary."""
         characters = {int(key): bbox for key, bbox in characters.items()}
 
         for key, bbox in characters.items():
-            bbox._valid(self._strict_bbox_validation)
+            bbox._valid(self._bbox_validation_type)
 
         self._characters = characters
         self.bboxes_available = True
 
     @property
     def text(self):
         """Get Document text. Once loaded stored in memory."""
         if self._text is not None:
             return self._text
         if self.is_online and not is_file(self.txt_file_path, raise_exception=False):
             self.download_document_details()
         if is_file(self.txt_file_path, raise_exception=False):
-            with open(self.txt_file_path, "r", encoding="utf-8") as f:
+            with open(self.txt_file_path, 'r', encoding='utf-8') as f:
                 self._text = f.read()
         return self._text
 
     def add_page(self, page: Page):
         """Add a Page to a Document."""
         if page not in self._pages:
             self._pages.append(page)
@@ -2306,174 +3718,101 @@
         """Get Pages of Document."""
         if self._pages:
             return self._pages
         if self.is_online and not is_file(self.pages_file_path, raise_exception=False):
             self.download_document_details()
             is_file(self.pages_file_path)
         if is_file(self.pages_file_path, raise_exception=False):
-            with open(self.pages_file_path, "r") as f:
+            with open(self.pages_file_path, 'r') as f:
                 pages_data = json.loads(f.read())
 
             page_texts = self.text.split('\f')
             assert len(page_texts) == len(pages_data)
             start_offset = 0
             for page_index, page_data in enumerate(pages_data):
                 page_text = page_texts[page_index]
                 end_offset = start_offset + len(page_text)
                 _ = Page(
                     id_=page_data['id'],
                     document=self,
                     number=page_data['number'],
                     original_size=page_data['original_size'],
+                    image_size=page_data['size'],
                     start_offset=start_offset,
                     end_offset=end_offset,
                 )
                 start_offset = end_offset + 1
 
         return self._pages
 
-    @property
-    def hocr(self):
-        """Get HOCR of Document. Once loaded stored in memory."""
-        if self._hocr:
-            pass
-        elif is_file(self.hocr_file_path, raise_exception=False):
-            # hocr might not be available (depends on the Project settings)
-            with open(self.hocr_file_path, "r", encoding="utf-8") as f:
-                self._hocr = f.read()
-        else:
-            if self.status[0] == 2:
-                data = get_document_details(
-                    document_id=self.id_, project_id=self.project.id_, session=self.session, extra_fields="hocr"
-                )
-
-                if 'hocr' in data.keys() and data['hocr']:
-                    self._hocr = data['hocr']
-                    with open(self.hocr_file_path, "w", encoding="utf-8") as f:
-                        f.write(self._hocr)
-                else:
-                    logger.warning(f'Please enable HOCR in {self.project} and upload {self} again to create HOCR.')
-
-        return self._hocr
-
     def update(self):
-        """Update document information."""
-        self.delete()
+        """Update Document information."""
+        self.delete_document_details()
         self.download_document_details()
         return self
 
-    def delete(self):
-        """Delete all local information for the document."""
+    def delete_document_details(self):
+        """Delete all local content information for the Document."""
         try:
             shutil.rmtree(self.document_folder)
         except FileNotFoundError:
             pass
         pathlib.Path(self.document_folder).mkdir(parents=True, exist_ok=True)
         self._annotations = None
         self._annotation_sets = None
+        self._text = None
+        self._pages = []
 
-    def merge_vertical(self, only_multiline_labels=True):
-        """
-        Merge Annotations with the same Label.
-
-        :param only_multiline_labels: Only merge if multiline Label Annotation in category training set
-        """
-        logger.info("Vertical merging Annotations.")
-        labels_dict = {}
-        for label in self.project.labels:
-            if not only_multiline_labels or label.has_multiline_annotations(categories=[self.category]):
-                labels_dict[label.id_local] = []
-
-        for annotation in self.annotations(use_correct=False, ignore_below_threshold=True):
-            if annotation.label.id_local in labels_dict:
-                labels_dict[annotation.label.id_local].append(annotation)
-
-        for label_id in labels_dict:
-            buffer = []
-            for annotation in labels_dict[label_id]:
-                for span in annotation.spans:
-                    # remove all spans in buffer more than 1 line apart
-                    while buffer and span.line_index > buffer[0].line_index + 1:
-                        buffer.pop(0)
-
-                    if buffer and buffer[-1].page != span.page:
-                        buffer = [span]
-                        continue
-
-                    # Do not merge new Span if Annotation part of AnnotationSet with more than 1 Annotation
-                    # (except default annotationSet)
-                    if (
-                        span.annotation.annotation_set
-                        and not span.annotation.annotation_set.label_set.is_default
-                        and len(
-                            span.annotation.annotation_set.annotations(use_correct=False, ignore_below_threshold=True)
-                        )
-                        > 1
-                    ):
-                        buffer.append(span)
-                        continue
-                    if len(annotation.spans) > 1:
-                        buffer.append(span)
-                        continue
-
-                    for candidate in buffer:
-                        # only looking for elements in line above
-                        if candidate.line_index == span.line_index:
-                            break
-                        # overlap in x
-                        # or next line
-                        if (
-                            not (span.bbox().x0 > candidate.bbox().x1 or span.bbox().x1 < candidate.bbox().x0)
-                        ) or self.text[candidate.end_offset : span.start_offset].replace(' ', '').replace(
-                            '\n', ''
-                        ) == '':
-                            span.annotation.delete()
-                            span.annotation = None
-                            candidate.annotation.add_span(span)
-                            buffer.remove(candidate)
-                    buffer.append(span)
+    def delete(self, delete_online: bool = False):
+        """Delete Document."""
+        self.project.del_document_by_id(self.id_, delete_online=delete_online)
 
     def evaluate_regex(self, regex, label: Label, annotations: List['Annotation'] = None):
         """Evaluate a regex based on the Document."""
         start_time = time.time()
         findings_in_document = regex_matches(
             doctext=self.text,
             regex=regex,
             keep_full_match=False,
-            filtered_group=f'Label_{label.id_}'
-            # filter by name of label: one regex can match multiple labels
+            filtered_group=f'Label_{label.id_}',
+            # filter by name of Label: one regex can match multiple Labels
         )
         processing_time = time.time() - start_time
         correct_findings = []
 
         label_annotations = self.annotations(label=label)
 
-        label_annotations_offsets = {
+        label_spans_offsets = {
             (span.start_offset, span.end_offset): ann for ann in label_annotations for span in ann.spans
         }
 
         for finding in findings_in_document:
             key = (finding['start_offset'], finding['end_offset'])
-            if key in label_annotations_offsets:
-                correct_findings.append(label_annotations_offsets[key])
+            if key in label_spans_offsets:
+                correct_findings.append(label_spans_offsets[key])
 
         try:
             annotation_precision = len(correct_findings) / len(findings_in_document)
         except ZeroDivisionError:
             annotation_precision = 0
 
         try:
-            annotation_recall = len(correct_findings) / len(label_annotations)
+            annotation_recall = len(correct_findings) / len(label_spans_offsets)
         except ZeroDivisionError:
             annotation_recall = 0
 
         try:
             f1_score = 2 * (annotation_precision * annotation_recall) / (annotation_precision + annotation_recall)
         except ZeroDivisionError:
             f1_score = 0
+
+        assert 0 <= annotation_precision <= 1
+        assert 0 <= annotation_recall <= 1
+        assert 0 <= f1_score <= 1
+
         return {
             'id': self.id_local,
             'regex': regex,
             # processing_time time can vary slightly between runs, round to ms so that this variation does not affect
             # the choice of regexes when values are below ms and metrics are the same
             'runtime': round(processing_time, 3),
             'count_total_findings': len(findings_in_document),
@@ -2486,102 +3825,283 @@
             'annotation_recall': annotation_recall,
             'f1_score': f1_score,
             'correct_findings': correct_findings,
         }
 
     def get_annotations(self) -> List[Annotation]:
         """Get Annotations of the Document."""
-        if self.category is None:
-            raise ValueError(f'Document {self} without Category must not have Annotations')
+        # if self.category is None:
+        #    raise ValueError(f'Document {self} without Category must not have Annotations')
 
         annotation_file_exists = is_file(self.annotation_file_path, raise_exception=False)
         annotation_set_file_exists = is_file(self.annotation_set_file_path, raise_exception=False)
 
         if self._update or (self.is_online and (self._annotations is None or self._annotation_sets is None)):
-
             if self.is_online and (not annotation_file_exists or not annotation_set_file_exists or self._update):
                 self.update()  # delete the meta of the Document details and download them again
-                self._update = None  # Make sure we don't repeat to load once updated.
+                self._update = False  # Make sure we don't repeat to load once updated.
 
             self._annotation_sets = None  # clean Annotation Sets to not create duplicates
             self.annotation_sets()
 
-            self._annotations = []  # clean Annotations to not create duplicates
+            self._annotations = AnnotationsContainer()  # clean Annotations to not create duplicates
             # We read the annotation file that we just downloaded
             with open(self.annotation_file_path, 'r') as f:
                 raw_annotations = json.load(f)
 
-            for raw_annotation in raw_annotations:
-                raw_annotation['annotation_set_id'] = raw_annotation.pop('section')
-                raw_annotation['label_set_id'] = raw_annotation.pop('section_label_id')
-                _ = Annotation(document=self, id_=raw_annotation['id'], **raw_annotation)
-            self._update = None  # Make sure we don't repeat to load once loaded.
+            if self.category == self.project.no_category:
+                # for backwards compatibility
+                # todo: not send no_label label to the server / see how it is handled now
+                # they are ignored now
+                no_label_raw_annotations = []
+                for raw_annotation in raw_annotations:
+                    # we want to ensure that both label files of old structure that have 'label_text' field and label
+                    # files of a new structure that have 'label' field that is a dict with nested elements are properly
+                    # parsed
+                    if 'label_text' in raw_annotation.keys():
+                        if raw_annotation['label_text'] == 'NO_LABEL':
+                            no_label_raw_annotations.append(raw_annotation)
+                    elif isinstance(raw_annotation['label'], dict):
+                        if raw_annotation['label']['name'] == 'NO_LABEL':
+                            no_label_raw_annotations.append(raw_annotation)
+
+                raw_annotations = no_label_raw_annotations
+
+            if raw_annotations:
+                for raw_annotation in raw_annotations:
+                    # remove the 'annotation_set' because we specify its id explicitly when creating the Annotation
+                    # conditions for backward compatibility
+                    if 'annotation_set' in raw_annotation:
+                        raw_annotation['annotation_set_id'] = raw_annotation.pop('annotation_set')
+                    else:
+                        raw_annotation['annotation_set_id'] = raw_annotation.pop('section')
+                    # same with the 'label_set_id'
+                    if 'label_set' in raw_annotation:
+                        raw_annotation['label_set_id'] = raw_annotation.pop('label_set')['id']
+                    else:
+                        raw_annotation['label_set_id'] = raw_annotation.pop('section_label_id')
+                    # same with 'document'
+                    raw_annotation.pop('document', None)
+                    if isinstance(raw_annotation['label'], int):
+                        label = self.project.get_label_by_id(id_=raw_annotation['label'])
+                    else:
+                        label = self.project.get_label_by_id(id_=raw_annotation['label']['id'])
+                    # same with 'label'
+                    raw_annotation.pop('label', None)
+                    # same with 'span'/'bboxes'
+                    if 'span' in raw_annotation:
+                        raw_spans = raw_annotation['span']
+                        raw_annotation.pop('span', None)
+                    else:
+                        raw_spans = raw_annotation['bboxes']
+                    spans = [
+                        Span(start_offset=span['start_offset'], end_offset=span['end_offset']) for span in raw_spans
+                    ]
+                    # same with 'annotation_set'
+                    if (
+                        raw_annotation['annotation_set_id']
+                        and not self.project.get_label_set_by_id(
+                            raw_annotation['label_set_id']
+                        ).has_multiple_annotation_sets
+                    ):
+                        raw_annotation.pop('annotation_set_id', None)
+                    _ = Annotation(document=self, id_=raw_annotation['id'], label=label, spans=spans, **raw_annotation)
+                self._update = False  # Make sure we don't repeat to load once loaded.
 
         if self._annotations is None:
             self.annotation_sets()
-            self._annotations = []
+            self._annotations = AnnotationsContainer()
             # We load the annotation file if it exists
             if annotation_file_exists:
                 with open(self.annotation_file_path, 'r') as f:
                     raw_annotations = json.load(f)
 
-                for raw_annotation in raw_annotations:
-                    raw_annotation['annotation_set_id'] = raw_annotation.pop('section')
-                    raw_annotation['label_set_id'] = raw_annotation.pop('section_label_id')
-                    _ = Annotation(document=self, id_=raw_annotation['id'], **raw_annotation)
+                if self.category == self.project.no_category:
+                    # conditions for backward compatibility
+                    raw_annotations = [
+                        annotation
+                        for annotation in raw_annotations
+                        if (
+                            ('label_text' in annotation.keys() and annotation['label_text'] == 'NO_LABEL')
+                            or (
+                                'label' in annotation.keys()
+                                and isinstance(annotation['label'], dict)
+                                and annotation['label']['name'] == 'NO_LABEL'
+                            )
+                        )
+                    ]
+
+                if raw_annotations:
+                    for raw_annotation in raw_annotations:
+                        raw_annotation['annotation_set_id'] = raw_annotation.pop('section')
+                        raw_annotation['label_set_id'] = raw_annotation.pop('section_label_id')
+                        _ = Annotation(document=self, id_=raw_annotation['id'], **raw_annotation)
+
+        return self._annotations.values()
 
-        return self._annotations
+    def propose_splitting(self, splitting_ai) -> List:
+        """Propose splitting for a multi-file Document.
+
+        :param splitting_ai: An initialized SplittingAI class
+        """
+        proposed = splitting_ai.propose_split_documents(self)
+        return proposed
+
+    def create_subdocument_from_page_range(self, start_page: Page, end_page: Page, include=False):
+        """
+        Create a shorter Document from a Page range of an initial Document.
+
+        :param start_page: A Page that the new sub-Document starts with.
+        :type start_page: Page
+        :param end_page: A Page that the new sub-Document ends with, if include is True.
+        :type end_page: Page
+        :param include: Whether end_page is included into the new sub-Document.
+        :type include: bool
+        :returns: A new sub-Document.
+        """
+        if include:
+            pages_text = self.text[start_page.start_offset : end_page.end_offset]
+        else:
+            pages_text = self.text[start_page.start_offset : end_page.start_offset]
+        new_doc = Document(project=self.project, id_=None, text=pages_text, category=self.category)
+        i = 1
+        start_offset = 0
+        for page in self.pages():
+            end_offset = start_offset + len(page.text)
+            page_id = page.id_ if page.id_ else page.copy_of_id
+            if (include and page.number in range(start_page.number, end_page.number + 1)) or (
+                not include and page.number in range(start_page.number, end_page.number)
+            ):
+                new_page = Page(
+                    id_=None,
+                    original_size=(page.height, page.width),
+                    document=new_doc,
+                    start_offset=start_offset,
+                    end_offset=end_offset,
+                    copy_of_id=page_id,
+                    number=i,
+                )
+                for category_annotation in page.category_annotations:
+                    CategoryAnnotation(
+                        category=category_annotation.category,
+                        confidence=category_annotation.confidence,
+                        page=new_page,
+                    )
+                i += 1
+                start_offset = end_offset + 1
+        return new_doc
+
+    def get_page_by_id(self, page_id: int, original: bool = False) -> Page:
+        """
+        Get a Page by its ID.
+
+        :param page_id: An ID of the Page to fetch.
+        :type page_id: int
+        """
+        for page in self.pages():
+            if page.id_ == page_id:
+                return page
+            if original:
+                raise IndexError(f'Page id {page_id} was not found in {self}.')
+            else:
+                if not page.id_ and page.copy_of_id == page_id:
+                    logger.warning(f'Page id {page_id} was not found in {self}, only a Page copy.')
+                    return page
 
 
 class Project(Data):
-    """Access the information of a Project."""
+    """
+    Access the information of a Project.
 
-    def __init__(self, id_: Union[int, None], project_folder=None, update=False, max_ram=None, **kwargs):
+    For more details see https://dev.konfuzio.com/sdk/explanations.html#project-concept
+    """
+
+    def __init__(
+        self,
+        id_: Union[int, None],
+        project_folder=None,
+        update=False,
+        max_ram=None,
+        strict_data_validation: bool = True,
+        credentials: dict = {},
+        **kwargs,
+    ):
         """
         Set up the Data using the Konfuzio Host.
 
         :param id_: ID of the Project
         :param project_folder: Set a Project root folder, if empty "data_<id_>" will be used.
+        :param update: Whether to sync local files with the Project online.
         :param max_ram: Maximum RAM used by AI models trained on this Project.
+        :param strict_data_validation: Whether to apply strict data validation rules.
+        :param credentials: A dict of key/values that are available in the Project.
+        See https://dev.konfuzio.com/sdk/tutorials/data_validation/index.html
         """
         self.id_local = next(Data.id_iter)
         self.id_ = id_  # A Project with None ID is not retrieved from the HOST
+        if self.id_ is None:
+            self.set_offline()
         self._project_folder = project_folder
         self.categories: List[Category] = []
         self._label_sets: List[LabelSet] = []
         self._labels: List[Label] = []
         self._documents: List[Document] = []
         self._meta_data = []
         self._max_ram = max_ram
+        self._strict_data_validation = strict_data_validation
+        self.credentials = credentials
+
+        for key, value in kwargs.items():
+            setattr(self, key, value)
 
         # paths
-        self.meta_file_path = os.path.join(self.project_folder, "documents_meta.json5")
-        self.labels_file_path = os.path.join(self.project_folder, "labels.json5")
-        self.label_sets_file_path = os.path.join(self.project_folder, "label_sets.json5")
+        self.meta_file_path = os.path.join(self.project_folder, 'documents_meta.json5')
+        self.categories_and_label_data_file_path = os.path.join(self.project_folder, 'categories_and_label_data.json5')
+        # labels and label sets left for backwards compatibility
+        self.labels_file_path = os.path.join(self.project_folder, 'labels.json5')
+        self.label_sets_file_path = os.path.join(self.project_folder, 'label_sets.json5')
 
         if self.id_ or self._project_folder:
             self.get(update=update)
-
+        else:
+            self.no_category = Category(project=self, id_=0, name_clean='NO_CATEGORY', name='NO_CATEGORY')
         # todo: list of Categories related to NO LABEL SET can be outdated, i.e. if the number of Categories changes
-        self.no_label_set = LabelSet(project=self, categories=self.categories)
+        self.no_label_set = LabelSet(
+            project=self, id_=0, categories=self.categories, has_multiple_annotation_sets=False
+        )
         self.no_label_set.name_clean = 'NO_LABEL_SET'
         self.no_label_set.name = 'NO_LABEL_SET'
-        self.no_label = Label(project=self, text='NO_LABEL', label_sets=[self.no_label_set])
+        self.no_label = Label(project=self, id_=0, text='NO_LABEL', label_sets=[self.no_label_set])
+        if not self.no_category.label_sets:
+            self.no_category.add_label_set(self.no_label_set)
+        if not self.no_label_set.categories:
+            self.no_label_set.add_category(self.no_category)
         self.no_label.name_clean = 'NO_LABEL'
+        self._regexes = None
 
     def __repr__(self):
         """Return string representation."""
-        return f"Project {self.id_}"
+        return f'Project {self.id_}'
+
+    @property
+    def ai_models(self):
+        """Return all AIs."""
+        return get_all_project_ais(project_id=self.id_, session=self.session)
 
     @property
     def documents(self):
         """Return Documents with status training."""
         return [doc for doc in self._documents if doc.dataset_status == 2]
 
     @property
+    def online_documents_dict(self) -> Dict:
+        """Return a dictionary of online documents using their id as key."""
+        return {doc.id_: doc for doc in self._documents if isinstance(doc.id_, int)}
+
+    @property
     def virtual_documents(self):
         """Return Documents created virtually."""
         return [doc for doc in self._documents if doc.dataset_status is None or doc.id_ is None]
 
     @property
     def test_documents(self):
         """Return Documents with status test."""
@@ -2595,83 +4115,86 @@
     @property
     def preparation_documents(self):
         """Return Documents with status test."""
         return [doc for doc in self._documents if doc.dataset_status == 1]
 
     @property
     def no_status_documents(self):
-        """Return Documents with status test."""
+        """Return Documents with no status."""
         return [doc for doc in self._documents if doc.dataset_status == 0]
 
     @property
     def project_folder(self) -> str:
         """Calculate the data document_folder of the Project."""
         if self._project_folder is not None:
             return self._project_folder
         else:
-            return f"data_{self.id_}"
+            return f'data_{self.id_}'
 
     @property
     def regex_folder(self) -> str:
         """Calculate the regex folder of the Project."""
-        return os.path.join(self.project_folder, "regex")
+        return os.path.join(self.project_folder, 'regex')
 
     @property
     def documents_folder(self) -> str:
         """Calculate the regex folder of the Project."""
-        return os.path.join(self.project_folder, "documents")
+        return os.path.join(self.project_folder, 'documents')
 
     @property
     def model_folder(self) -> str:
         """Calculate the model folder of the Project."""
-        return os.path.join(self.project_folder, "models")
+        return os.path.join(self.project_folder, 'models')
 
     @property
     def max_ram(self):
         """Return maximum memory used by AI models."""
         return self._max_ram
 
     def write_project_files(self):
         """Overwrite files with Project, Label, Label Set information."""
-        data = get_project_details(project_id=self.id_)
-        with open(self.label_sets_file_path, "w") as f:
-            json.dump(data['section_labels'], f, indent=2, sort_keys=True)
-        with open(self.labels_file_path, "w") as f:
-            json.dump(data['labels'], f, indent=2, sort_keys=True)
+        categories_labels_label_sets = get_project_categories(project_id=self.id_, session=self.session)
+        with open(self.categories_and_label_data_file_path, 'w') as f:
+            json.dump(categories_labels_label_sets, f, indent=2, sort_keys=True)
+
+        self.write_meta_of_files()
+
+        return self
 
+    def write_meta_of_files(self):
+        """Overwrite meta-data of Documents in Project."""
         meta_data = get_meta_of_files(project_id=self.id_, session=self.session)
-        with open(self.meta_file_path, "w") as f:
+        with open(self.meta_file_path, 'w') as f:
             json.dump(meta_data, f, indent=2, sort_keys=True)
-        return self
 
     def get(self, update=False):
         """
         Access meta information of the Project.
 
         :param update: Update the downloaded information even it is already available
         """
-        if is_file(self.meta_file_path, raise_exception=False):
-            logger.debug("Keep your local information about Documents to be able to do a partial update.")
-            with open(self.meta_file_path, "r") as f:
-                self.old_meta_data = json.load(f)
-        else:
-            self.old_meta_data = []
-
         pathlib.Path(self.project_folder).mkdir(parents=True, exist_ok=True)
         pathlib.Path(self.documents_folder).mkdir(parents=True, exist_ok=True)
         pathlib.Path(self.regex_folder).mkdir(parents=True, exist_ok=True)
         pathlib.Path(self.model_folder).mkdir(parents=True, exist_ok=True)
 
+        # reload means re-add to the Project what is currently available in the Project's folder
+        # update means download information from server to keep up with the updates made online
         if self.id_ and (not is_file(self.meta_file_path, raise_exception=False) or update):
             self.write_project_files()
-        self.get_meta(reload=True)
+        # order of adding data into the project has changed after migration from v2 to v3 API - the endpoint used for
+        # fetching categories, labels and label sets returns them in a nested structure:
+        # Categories -> Label Sets -> Labels.
+        # order of methods is pertained for backward compatibility in case there is project information that is stored
+        # in an "old" way, with labels.json5 and label_sets.json5
         self.get_labels(reload=True)
         self.get_label_sets(reload=True)
-        self.get_categories()
-        self.init_or_update_document()
+        self.get_categories(reload=True)
+        self.get_meta(reload=True)
+        self.init_or_update_document(from_online=False)
         return self
 
     def add_label_set(self, label_set: LabelSet):
         """
         Add Label Set to Project, if it does not exist.
 
         :param label_set: Label Set to add in the Project
@@ -2683,18 +4206,19 @@
 
     def add_category(self, category: Category):
         """
         Add Category to Project, if it does not exist.
 
         :param category: Category to add in the Project
         """
-        if category not in self.categories:
-            self.categories.append(category)
-        else:
-            raise ValueError(f'In {self} the {category} is a duplicate and will not be added.')
+        if category.name != 'NO_CATEGORY':
+            if category not in self.categories:
+                self.categories.append(category)
+            else:
+                raise ValueError(f'In {self} the {category} is a duplicate and will not be added.')
 
     def add_label(self, label: Label):
         """
         Add Label to Project, if it does not exist.
 
         :param label: Label to add in the Project
         """
@@ -2713,114 +4237,249 @@
     def get_meta(self, reload=False):
         """
         Get the list of all Documents in the Project and their information.
 
         :return: Information of the Documents in the Project.
         """
         if not self._meta_data or reload:
-            with open(self.meta_file_path, "r") as f:
+            if self._meta_data:
+                self.old_meta_data = self._meta_data
+            with open(self.meta_file_path, 'r') as f:
                 self._meta_data = json.load(f)
+
         return self._meta_data
 
     @property
     def meta_data(self):
         """Return Project meta data."""
         if not self._meta_data:
             self.get_meta()
         return self._meta_data
 
-    def get_categories(self):
+    def get_categories(self, reload: bool = True):
         """Load Categories for all Label Sets in the Project."""
-        for label_set in self.label_sets:
-            if label_set.is_default:
-                # the _default_of_label_set_ids are the label sets used by the category
-                pass
-            else:
-                # the _default_of_label_set_ids are the categories the label set is used in
-                for label_set_id in label_set._default_of_label_set_ids:
-                    category = self.get_category_by_id(label_set_id)
-                    label_set.add_category(category)  # The Label Set is linked to a Category it created
-                    category.add_label_set(label_set)
 
-    def get_label_sets(self, reload=False):
-        """Get LabelSets in the Project."""
-        if not self._label_sets or reload:
-            with open(self.label_sets_file_path, "r") as f:
+        # backward compatibility loading
+        if is_file(self.label_sets_file_path, raise_exception=False):
+            with open(self.label_sets_file_path, 'r') as f:
                 label_sets_data = json.load(f)
 
-            self._label_sets = []  # clean up Label Sets to not create duplicates
             self.categories = []  # clean up Labels to not create duplicates
+
+            # adding a NO_CATEGORY at this step because we need to preserve it after Project is updated
+            if 'NO_CATEGORY' not in [category.name for category in self.categories]:
+                self.no_category = Category(project=self, id_=0, name_clean='NO_CATEGORY', name='NO_CATEGORY')
             for label_set_data in label_sets_data:
-                label_set = LabelSet(project=self, id_=label_set_data['id'], **label_set_data)
+                label_set = self.get_label_set_by_id(label_set_data['id'])
                 if label_set.is_default:
                     category = Category(project=self, id_=label_set_data['id'], **label_set_data)
                     category.label_sets.append(label_set)
                     label_set.categories.append(category)  # Konfuzio Server mixes the concepts, we use two instances
-                    # self.add_category(category)
+            for label_set in self.label_sets:
+                if label_set.is_default:
+                    # the _default_of_label_set_ids are the Label Sets used by the Category
+                    pass
+                else:
+                    # the _default_of_label_set_ids are the Categories the Label Set is used in
+                    for label_set_id in label_set._default_of_label_set_ids:
+                        category = self.get_category_by_id(label_set_id)
+                        if category not in label_set.categories:
+                            label_set.add_category(category)  # The Label Set is linked to a Category it created
+                        if label_set.name not in [cur_label_set.name for cur_label_set in category.label_sets]:
+                            category.add_label_set(label_set)
+
+        if reload and (
+            not is_file(self.labels_file_path, raise_exception=False)
+            and not is_file(self.label_sets_file_path, raise_exception=False)
+        ):
+            self.categories = []
+
+            if 'NO_CATEGORY' not in [category.name for category in self.categories]:
+                self.no_category = Category(project=self, id_=0, name_clean='NO_CATEGORY', name='NO_CATEGORY')
+            with open(self.categories_and_label_data_file_path, 'r') as f:
+                categories_and_label_data = json.load(f)
+            for category in categories_and_label_data:
+                cur_category = Category(project=self, id_=category['id'], name=category['name'])
+                for label_data in category['schema']:
+                    cur_labels = label_data['labels']
+                    label_data.pop('labels', None)
+                    label_set = LabelSet(project=self, id_=label_data['id'], **label_data)
+                    for cur_label in cur_labels:
+                        if cur_label['name'] not in [label.name for label in self.labels]:
+                            _ = Label(project=self, id_=cur_label['id'], text=cur_label['name'], **cur_label)
+                        else:
+                            _ = self.get_label_by_id(cur_label['id'])
+                        label_set.labels.append(_)
+                        _.label_sets.append(label_set)
+                    if label_set.id_ == cur_category.id_:
+                        label_set.is_default = True
+                    cur_category.label_sets.append(label_set)
+                    label_set.categories.append(cur_category)
 
+    def get_label_sets(self, reload=False):
+        """Get LabelSets in the Project."""
+        if not self._label_sets or reload:
+            self._label_sets = []  # clean up Label Sets to not create duplicates
+            if is_file(self.label_sets_file_path, raise_exception=False):
+                with open(self.label_sets_file_path, 'r') as f:
+                    label_sets_data = json.load(f)
+                for label_set_data in label_sets_data:
+                    _ = LabelSet(project=self, id_=label_set_data['id'], **label_set_data)
+                    if _.name not in [label_set.name for label_set in self._label_sets]:
+                        self._label_sets.append(_)
+            else:
+                for cur_label_set in [label_set for category in self.categories for label_set in category.label_sets]:
+                    self._label_sets.append(cur_label_set)
         return self._label_sets
 
     @property
     def label_sets(self):
         """Return Project LabelSets."""
         if not self._label_sets:
             self.get_label_sets()
         return self._label_sets
 
-    def get_labels(self, reload=False) -> Label:
+    def get_labels(self, reload=False) -> List[Label]:
         """Get ID and name of any Label in the Project."""
         if not self._labels or reload:
-            with open(self.labels_file_path, "r") as f:
-                labels_data = json.load(f)
             self._labels = []  # clean up Labels to not create duplicates
-            for label_data in labels_data:
-                # Remove the project from label_data
-                label_data.pop("project", None)
-                Label(project=self, id_=label_data['id'], **label_data)
-
+            if is_file(self.labels_file_path, raise_exception=False):
+                with open(self.labels_file_path, 'r') as f:
+                    labels_data = json.load(f)
+                for label_data in labels_data:
+                    # Remove the Project from label_data
+                    label_data.pop('project', None)
+                    Label(project=self, id_=label_data['id'], **label_data)
+            else:
+                for cur_label in [
+                    label
+                    for category in self.categories
+                    for label_set in category.label_sets
+                    for label in label_set.labels
+                ]:
+                    if cur_label not in self._labels:
+                        self._labels.append(cur_label)
         return self._labels
 
     @property
     def labels(self):
         """Return Project Labels."""
         if not self._labels:
             self.get_labels()
         return self._labels
 
-    def init_or_update_document(self):
-        """Initialize Document to then decide about full, incremental or no update."""
-        self._documents = []  # clean up Documents to not create duplicates
+    def init_or_update_document(self, from_online=False):
+        """
+        Initialize or update Documents from local files to then decide about full, incremental or no update.
+
+        :param from_online: If True, all Document metadata info is first reloaded with latest changes in the server
+        """
+        logger.info(f'Running init_or_update_document({from_online=}) on {self}')
+        local_docs_dict = self.online_documents_dict
+        if from_online:
+            self.write_meta_of_files()
+            self.get_meta(reload=True)
+        updated_docs_ids_set = set()  # delete all docs not in the list at the end
+        n_updated_documents = 0
+        n_new_documents = 0
+        n_unchanged_documents = 0
         for document_data in self.meta_data:
-            if document_data['status'][0] == 2:  # NOQA - hotfix for Text Annotation Server # todo add test
-                new_date = document_data["updated_at"]
-                new = True
-                updated = None
-                if self.old_meta_data:
-                    new = document_data["id"] not in [doc["id"] for doc in self.old_meta_data]
-                    if not new:
-                        last_date = [d["updated_at"] for d in self.old_meta_data if d['id'] == document_data["id"]][0]
-                        updated = dateutil.parser.isoparse(new_date) > dateutil.parser.isoparse(last_date)
-
-                if updated:
-                    doc = Document(project=self, update=True, id_=document_data['id'], **document_data)
-                    logger.info(f'{doc} was updated, we will download it again as soon you use it.')
-                elif new:
-                    doc = Document(project=self, update=True, id_=document_data['id'], **document_data)
-                    logger.info(f'{doc} is not available on your machine, we will download it as soon you use it.')
-                else:
-                    doc = Document(project=self, update=False, id_=document_data['id'], **document_data)
-                    logger.debug(f'Load local version of {doc} from {new_date}.')
+            updated_docs_ids_set.add(document_data['id'])
+            # if document_data['status'][0] == 2:  # - hotfix for Text Annotation Server # todo add test
+
+            new_date = document_data['updated_at']
+            updated = False
+            new = document_data['id'] not in local_docs_dict
+            if not new:
+                last_date = local_docs_dict[document_data['id']].updated_at
+                updated = dateutil.parser.isoparse(new_date) > last_date if last_date is not None else True
+            category_id = None
+            # backward compatibility
+            if 'category' in document_data.keys():
+                category_id = document_data['category']
+            elif 'category_template' in document_data.keys():
+                category_id = document_data['category_template']
+            doc_category = self.get_category_by_id(category_id) if category_id else self.no_category
+            document_data.pop('category', None)
+            # ensuring we store document status in a variable and don't pass it multiple times by not removing it from
+            # document_data
+            status = document_data['status_data']
+            document_data.pop('status_data', None)
+            if updated:
+                doc = local_docs_dict[document_data['id']]
+                doc.update_meta_data(category=doc_category, status=status, **document_data)
+                doc.update()
+                logger.debug(f'{doc} was updated, we will download it again as soon you use it.')
+                n_updated_documents += 1
+            elif new:
+                document_data.pop('project', None)
+                # ensuring we store dataset status in a variable and don't pass it multiple times by not removing it
+                # from document_data
+                if 'status' in document_data:
+                    status = document_data['status']
+                document_data.pop('status', None)
+                doc = Document(
+                    project=self,
+                    update=from_online,
+                    id_=document_data['id'],
+                    category=doc_category,
+                    status=status,
+                    **document_data,
+                )
+                logger.debug(f'{doc} is not available on your machine, we will download it as soon you use it.')
+                n_new_documents += 1
+            else:
+                doc = local_docs_dict[document_data['id']]
+                if 'status' in document_data:
+                    status = document_data['status']
+                document_data.pop('status', None)
+                doc.update_meta_data(
+                    category=doc_category, status=status, **document_data
+                )  # reset any Document level meta data changes
+                logger.debug(f'Unchanged local version of {doc} from {new_date}.')
+                n_unchanged_documents += 1
+            # else:
+            #    logger.debug(f"Not loading Document {[document_data['id']]} with status {document_data['status'][0]}.")
+
+        to_delete_ids = set(local_docs_dict.keys()) - updated_docs_ids_set
+        n_deleted_documents = len(to_delete_ids)
+        for to_del_id in to_delete_ids:
+            local_docs_dict[to_del_id].delete(delete_online=False)
+
+        logger.info(
+            f'{n_updated_documents} Documents were updated,'
+            f' {n_new_documents} Documents are new,'
+            f' {n_unchanged_documents} Documents are unchanged,'
+            f' and {n_deleted_documents} Documents were deleted.'
+        )
 
     def get_document_by_id(self, document_id: int) -> Document:
         """Return Document by its ID."""
         for document in self._documents:
             if document.id_ == document_id:
                 return document
         raise IndexError(f'Document id {document_id} was not found in {self}.')
 
+    def del_document_by_id(self, document_id: int, delete_online: bool = False) -> Document:
+        """Delete Document by its ID."""
+        document = self.get_document_by_id(document_id)
+
+        if delete_online:
+            delete_file_konfuzio_api(document_id, session=self.session)
+            self.write_meta_of_files()
+            self.get_meta(reload=True)
+            try:
+                shutil.rmtree(document.document_folder)
+            except FileNotFoundError:
+                pass
+
+        self._documents.remove(document)
+
+        return None
+
     def get_label_by_name(self, name: str) -> Label:
         """Return Label by its name."""
         for label in self.labels:
             if label.name == name:
                 return label
         raise IndexError(f'Label name {name} was not found in {self}.')
 
@@ -2860,14 +4519,32 @@
         :param id_: ID of the Category to get.
         """
         for category in self.categories:
             if category.id_ == id_:
                 return category
         raise IndexError(f'Category id {id_} was not found in {self}.')
 
+    def get_credentials(self, key):
+        """
+        Return the value of the key in the credentials dict or in the config file.
+
+        Returns None and emits a warning if the key is not found.
+
+        :param key: Key of the credential to get.
+        """
+        if key in self.credentials:
+            value = self.credentials[key]
+        else:
+            from .settings_importer import config
+
+            value = config(key, default=None)
+        if not value:
+            logger.warning(f'No value found for {key} in {self}.')
+        return value
+
     def delete(self):
         """Delete the Project folder."""
         shutil.rmtree(self.project_folder)
 
     def lose_weight(self):
         """Delete data of the instance."""
         super().lose_weight()
@@ -2877,28 +4554,50 @@
             label_set.lose_weight()
         for label in self.labels:
             label.lose_weight()
         self._documents = []
         self._meta_data = []
         return self
 
+    def download_training_and_test_data(self) -> None:
+        """
+        Migrate your Project to another HOST.
 
-def download_training_and_test_data(id_: int):
-    """
-    Migrate your project to another HOST.
+        See https://dev.konfuzio.com/web/migration-between-konfuzio-server-instances/index.html
 
-    See https://help.konfuzio.com/integrations/migration-between-konfuzio-server-instances/index.html
-        #migrate-projects-between-konfuzio-server-instances
-    """
-    prj = Project(id_=id_, update=True)
+        """
+        if len(self.documents + self.test_documents) == 0:
+            raise ValueError('No Documents in the training or test set. Please add them.')
+        for document in tqdm(self.documents + self.test_documents):
+            document.download_document_details()
+            document.get_file()
+            document.get_file(ocr_version=False)
+            document.get_bbox()
+            document.get_images()
 
-    if len(prj.documents + prj.test_documents) == 0:
-        raise ValueError("No Documents in the training or test set. Please add them.")
+        print('[SUCCESS] Data exporting finished successfully!')
 
-    for document in tqdm(prj.documents + prj.test_documents):
-        document.download_document_details()
-        document.get_file()
-        document.get_file(ocr_version=False)
-        document.get_bbox()
-        document.get_images()
+    def export_project_data(self, include_ais=False, training_and_test_documents=True) -> None:
+        """
+        "Export the Project data including Training, Test Documents and AI models.
 
-    print("[SUCCESS] Data downloading finished successfully!")
+        :include_ais: Whether to include AI models in the export
+        :training_and_test_documents: Whether to include training & test documents in the export.
+        """
+        if training_and_test_documents:
+            try:
+                print('[INFO] Starting Training and Test Document export!')
+                self.download_training_and_test_data()
+            except Exception as error:
+                print('[ERROR] Something went wrong while downloading Document data!')
+                raise error
+        if include_ais:
+            try:
+                print('[INFO] Starting AI Model file export!')
+                exported_ais = export_ai_models(self)
+                if exported_ais:
+                    print(f'[INFO] Export finished. {exported_ais} AIs were available for export.')
+                else:
+                    print('[INFO] No AIs available for export.')
+            except Exception as error:
+                print('[ERROR] Something went wrong while downloading AIs or AI metadata!')
+                raise error
```

### Comparing `konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk/normalize.py` & `konfuzio_sdk-0.3.0/konfuzio_sdk/normalize.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """Convert the Span according to the data_type of the Annotation."""
 import logging
-import numpy as np
 from typing import Dict, Optional
-import regex as re
 
+import numpy as np
+import regex as re
 
 logger = logging.getLogger(__name__)
 
 ROMAN_NUMS = {'M': 1000, 'D': 500, 'C': 100, 'L': 50, 'X': 10, 'V': 5, 'I': 1}
 
 
 def _get_is_negative(offset_string: str) -> bool:
     """Check if a string has a negative sign."""
     is_negative = False
     if offset_string.count('-') > 0 or offset_string.count('–'):
         if offset_string.count('-') == 1 or offset_string.count('–') == 1:
             is_negative = True
 
     if offset_string.count('S') > 0:
-        if offset_string.count('S') == 1 and offset_string[-1] == "S" and is_negative is False:
+        if offset_string.count('S') == 1 and offset_string[-1] == 'S' and is_negative is False:
             is_negative = True
 
     if (
         offset_string[0] == '*'
         and offset_string.count('*') == 1
         and offset_string.count('(') == 1
         and offset_string.count(')') == 1
@@ -58,14 +58,22 @@
 
 
 def normalize_to_positive_float(offset_string: str) -> Optional[float]:
     """Given an offset_string this function tries to translate the offset-string to an absolute number (ignores +/-)."""
     return _normalize_string_to_absolute_float(offset_string)
 
 
+def _normalize_to_float_safe(offset_string: str) -> Optional[float]:
+    """Given an offset_string this function tries to convert it to a float and returns None if failing."""
+    try:
+        return float(offset_string)
+    except ValueError:
+        return None
+
+
 def _normalize_string_to_absolute_float(offset_string: str) -> Optional[float]:
     """Given a string tries to translate that into an absolute float. SHOULD NOT BE CALLED DIRECTLY."""
     _float = None
     normalization = None
 
     if offset_string in ['-', '-,-', '-,--', '--,--', '--,-', '-.-', '-.--', '--.--', '--.-']:
         return 0.0
@@ -105,32 +113,65 @@
 
     if offset_string.lower() in ['elf', 'eleven']:
         return 11.0
 
     if offset_string.lower() in ['zwölf', 'twelve']:
         return 12.0
 
+    if 'Mio' in offset_string:
+        value = _normalize_string_to_absolute_float(offset_string.split('Mio')[0])
+        if value is None:
+            return None
+        else:
+            return 1000000 * value
+
+    if 'Million' in offset_string:
+        value = _normalize_string_to_absolute_float(offset_string.split('Million')[0])
+        if value is None:
+            return None
+        else:
+            return 1000000 * value
+
     # check for major spaces
     if re.search(r'(\d)[ ]{3,}(\d)', offset_string):
         return None
 
-    offset_string = re.sub(r"(\d)[ ]{1,2}(\d)", r'\1.\2', offset_string)
+    offset_string = re.sub(r'(\d)[ ]{1,2}(\d)', r'\1.\2', offset_string)
 
     if offset_string.count('*') > 1:
         return None
 
     if offset_string.count('*') == 1 and offset_string[0] == '*' and offset_string.count('(') == 0:
         return None
 
+    if offset_string.count('.') > 1:  # for cases like '0.22.1', '12.123.1111.3', '123.1.34'
+        split = offset_string.split('.')
+        # Check if middle parts have invalid length.
+        for chunk in split[1:-1]:
+            if len(chunk) != 3:
+                return None
+
+    if offset_string.count(',') > 1:  # for cases like '11111,12,3'
+        split = offset_string.split(',')
+        # Check if middle parts have invalid length.
+        for chunk in split[1:-1]:
+            if len(chunk.strip(' ')) != 3:
+                return None
+
+    # for cases like '0-3', '0,0-0,3
+    if offset_string.count('-') == 1 and offset_string[0] != '-' and offset_string[-1] != '-':
+        return None
+
     offset_string = (
         offset_string.replace('O', '0')
         .replace('°', '')
         .replace(':', '')
         .replace('“', '')
         .replace("'", '')
+        .replace('’', '')
         .replace('/', '')
         .replace('>', '')
         .replace('(', '')
         .replace(')', '')
         .replace('|', '')
         .replace(' ', '')
         .replace('"', '')
@@ -148,82 +189,99 @@
 
     ln = len(offset_string)
 
     # check for 1.234,56
     if '.' in offset_string and offset_string.count(',') == 1 and offset_string.index('.') < offset_string.index(','):
         offset_string = offset_string.replace('.', '').replace(',', '.')  # => 1234.56
         if all(x.isdecimal() for x in offset_string.split('.')):
-            _float = float(offset_string)
+            _float = _normalize_to_float_safe(offset_string)
     # check for 1,234.56
     elif '.' in offset_string and ',' in offset_string and offset_string.index(',') < offset_string.index('.'):
         offset_string = offset_string.replace(',', '')  # => 1234.56
-        if all(x.isdecimal() for x in offset_string.split('.')):
-            _float = float(offset_string)
+        if all(x.isdecimal() for x in offset_string.split('.')) and offset_string.count('.') < 2:
+            _float = _normalize_to_float_safe(offset_string)
     # check for 1,234,56
     elif (
         ln > 6
         and offset_string.count(',') == 2
         and offset_string.count('.') == 0
         and offset_string[-3] == ','
         and offset_string[-7] == ','
     ):
         offset_string = offset_string[:-3] + '.' + offset_string[-2:]  # => 1,234.56
         offset_string = offset_string.replace(',', '')  # => 1234.56
         if all(x.isdecimal() for x in offset_string.split('.')):
-            _float = float(offset_string)
+            _float = _normalize_to_float_safe(offset_string)
     # check for 1.234.56
     elif ln > 6 and offset_string.count('.') >= 2 and offset_string[-3] == '.' and offset_string[-7] == '.':
         offset_string = offset_string.replace('.', '')  # => 123456
         offset_string = offset_string[:-2] + '.' + offset_string[-2:]  # => 1234.56
         if all(x.isdecimal() for x in offset_string.split('.')):
-            _float = float(offset_string)
+            _float = _normalize_to_float_safe(offset_string)
     # check for 1.967.
     elif ln > 5 and offset_string.count('.') == 2 and offset_string[-1] == '.' and offset_string[-5] == '.':
         offset_string = offset_string.replace('.', '')  # => 123456
         if offset_string.isdecimal():
             _float = float(offset_string)
     # check for 1.234.567
     elif ln > 7 and offset_string.count('.') >= 2 and offset_string[-4] == '.' and offset_string[-8] == '.':
         offset_string = offset_string.replace('.', '')  # => 1234567
         if offset_string.isdecimal():
-            _float = float(offset_string)
+            _float = _normalize_to_float_safe(offset_string)
     # check for 3.456,814,75
     elif ln > 7 and offset_string.count(',') == 2 and offset_string[-3] == ',' and offset_string[-7] == ',':
         offset_string = offset_string.replace(',', '').replace('.', '')  # => 1234567
         if offset_string.isdecimal():
-            _float = float(offset_string) / 100.0
+            _float = _normalize_to_float_safe(offset_string) / 100.0
     # check for 1,234,567
     elif ln > 7 and offset_string.count(',') == 2 and offset_string[-4] == ',' and offset_string[-8] == ',':
         offset_string = offset_string.replace(',', '')  # => 1234567
         if offset_string.isdecimal():
-            _float = float(offset_string)
+            _float = _normalize_to_float_safe(offset_string)
     # check for 12,34 (comma is third last char).
     elif (
         ',' in offset_string
         and (len(offset_string) - offset_string.index(',')) == 3
         and offset_string.replace(',', '').isdecimal()
     ):
         offset_string = offset_string.replace(',', '.')  # => 12.34
         if all(x.isdecimal() for x in offset_string.split('.')):
-            _float = float(offset_string)
+            _float = _normalize_to_float_safe(offset_string)
     # check for 12.34 (dot is third last char).
     elif offset_string.count('.') == 1 and (len(offset_string) - offset_string.index('.')) == 3:
         if all(x.isdecimal() for x in offset_string.split('.')):
-            _float = float(offset_string)  # => 12.34
+            _float = _normalize_to_float_safe(offset_string)  # => 12.34
+    # check for 123,, or 2141,,,, (trailing commas that are not separators)
+    elif (
+        offset_string.count(',') > 1
+        and offset_string.replace(',', '').isdecimal()
+        and offset_string.endswith(',')
+        and '' in offset_string.split(',')
+    ):
+        _float = None
     # check for 12,3 (comma is second last char).
     elif (
         ',' in offset_string
         and (len(offset_string) - offset_string.index(',')) == 2
         and offset_string.replace(',', '').isdecimal()
     ):
         _float = float(offset_string.replace(',', '.'))  # => 12.3
+    # check for 123,4567 (comma and 4 decimals, no thousand separators).
+    elif (
+        ',' in offset_string
+        and (len(offset_string) - offset_string.index(',')) == 5
+        and offset_string.replace(',', '').isdecimal()
+    ):
+        offset_string = offset_string.replace(',', '.')  # => 123.4567
+        if all(x.isdecimal() for x in offset_string.split('.')):
+            _float = _normalize_to_float_safe(offset_string)
     # check for 12.3 (dot is second last char).
     elif offset_string.count('.') == 1 and (len(offset_string) - offset_string.index('.')) == 2:
         if all(x.isdecimal() for x in offset_string.split('.')):
-            _float = float(offset_string)  # => 12.3
+            _float = _normalize_to_float_safe(offset_string)  # => 12.3
     # check for 500,000 (comma is forth last char).
     elif (
         ln > 0
         and ',' in offset_string
         and (len(offset_string) - offset_string.index(',')) == 4
         and offset_string.replace(',', '').isdecimal()
         and not offset_string[0] == ','
@@ -239,40 +297,40 @@
         and offset_string[-4] == '.'
         and offset_string.replace('.', '').isdecimal()
         and offset_string.count('.') == 1
     ):
         normalization = abs(float(offset_string.replace('.', '')))
     # check for 5000 (only numbers)
     elif offset_string.isdecimal():
-        _float = float(offset_string)
+        _float = _normalize_to_float_safe(offset_string)
         _float = abs(_float)
         normalization = _float
     # check for 159,;03 (obscured edge case)
     elif (
         ln > 3
         and ';' in offset_string
         and ',' in offset_string
         and offset_string[-3] == ';'
         and offset_string[-4] == ','
     ):
         offset_string = offset_string.replace(',', '.').replace(';', '')  # => 159.03
         if all(x.isdecimal() for x in offset_string.split('.')):
-            _float = float(offset_string)
+            _float = _normalize_to_float_safe(offset_string)
     # # check for “71,90 (obscured edge case)
     # elif offset_string[0] == '“' and offset_string[-3] == ',':
     #     _float = float(offset_string.replace('“', '').replace(',','.'))  # => 71.90
     #     _float = abs(_float)
     #     normalization = _float
     # check for ,22,95 (obscured edge case)
     elif (
         ln > 2 and offset_string[0] == '‚' and offset_string[-3] == ','
     ):  # first comma is a very different comma ('‚' != ',')
         offset_string = offset_string[1:].replace(',', '.')  # => 22.95
         if all(x.isdecimal() for x in offset_string.split('.')):
-            _float = float(offset_string)
+            _float = _normalize_to_float_safe(offset_string)
     elif all(char in ROMAN_NUMS.keys() for char in offset_string):
         normalization = roman_to_float(offset_string)
     else:
         logger.debug(
             'Could not convert >>' + offset_string + '<< to positive/absolute float (no conversion case found)'
         )
 
@@ -455,14 +513,18 @@
     if len(offset_string) == 10 and offset_string[4] == '-' and offset_string[7] == '-':
         _date = f'{offset_string[8:10]}.{offset_string[5:7]}.{offset_string[0:4]}'
         translation = _date
     # check for 01.01.2001
     elif len(offset_string) == 10 and offset_string[2] == '.' and offset_string[5] == '.':
         _date = offset_string  # => 01.01.2001
         translation = _date
+    # check for 01.1.2001
+    elif len(offset_string) == 9 and offset_string[2] == '.' and offset_string[4] == '.':
+        _date = f'{offset_string[:2]}.0{offset_string[3]}.{offset_string[5:]}'
+        translation = _date  # => 01.01.2001
     # check for 01/01/2001
     elif len(offset_string) == 10 and offset_string[2] == '/' and offset_string[5] == '/':
         _date = offset_string.replace('/', '.')  # => 01.01.2001
         translation = _date
     # check for 01-01-2001
     elif len(offset_string) == 10 and offset_string[2] == '-' and offset_string[5] == '-':
         _date = offset_string.replace('-', '.')  # => 01.01.2001
@@ -607,22 +669,22 @@
             len(date_string) == 10
             and date_string[2] == '.'
             and date_string[5] == '.'
             and date_string[-4:].isdecimal()
             and date_string[:2].isdecimal()
             and date_string[3:5].isdecimal()
         ):
-            logger.info('Could not convert >>' + date_string + '<< to date (date contains letters)')
+            logger.debug('Could not convert >>' + date_string + '<< to date (date contains letters)')
             date_string = None
         elif (
             not ((1900 < int(date_string[-4:]) < 2100) or int(date_string[-4:]) == 0)
             or not (int(date_string[:2]) < 32)
             or not (int(date_string[3:5]) < 13)
         ):
-            logger.info('Could not convert >>' + date_string + '<< to date (invalid date)')
+            logger.debug('Could not convert >>' + date_string + '<< to date (invalid date)')
             date_string = None
     return date_string
 
 
 def normalize_to_bool(offset_string: str):
     """Given an offset_string this function tries to translate the offset-string to a bool."""
     offset_string = offset_string.upper()
@@ -644,23 +706,23 @@
             return None
     else:
         return None
 
 
 def roman_to_float(offset_string: str) -> Optional[float]:
     """Convert a Roman numeral to an integer."""
-    input = offset_string.upper()
+    input_string = offset_string.upper()
     if len(offset_string) == 0:
         return None
     roman_sum = 0
     for i, char in enumerate(offset_string):
         try:
-            value = ROMAN_NUMS[input[i]]
+            value = ROMAN_NUMS[input_string[i]]
             # If the next place holds a larger number, this value is negative
-            if i + 1 < len(input) and ROMAN_NUMS[input[i + 1]] > value:
+            if i + 1 < len(input_string) and ROMAN_NUMS[input_string[i + 1]] > value:
                 roman_sum -= value
             else:
                 roman_sum += value
         except KeyError:
             return None
     return float(roman_sum)
```

### Comparing `konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk/regex.py` & `konfuzio_sdk-0.3.0/konfuzio_sdk/regex.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Generic way to build regex from examples."""
 import logging
-import regex as re
-from typing import List, Dict
+from typing import Dict, List
 
 import pandas
+import regex as re
 from tabulate import tabulate
 
 logger = logging.getLogger(__name__)
 
 
 def merge_regex(regex_tokens: List[str]):
     """Merge a list of regex to one group."""
@@ -21,15 +21,15 @@
     suggestion = re.sub(r' {2,}', r'[ ]{2,}', single_whitespace_replaced)
     return suggestion
 
 
 def escape(string: str):
     """Escape a string, so that it can still be used to create a regex."""
     escaped_original = (
-        string.replace('\\', "\\\\")
+        string.replace('\\', '\\\\')
         .replace('[', r'\[')
         .replace(']', r'\]')
         .replace('+', r'[\+]')
         .replace('*', r'\*')
         .replace('|', r'\|')
         .replace('\n', '\n')
         .replace('-', '[-]')
@@ -117,15 +117,15 @@
             'regex_quality',
             'annotation_precision',
             'runtime',  # take the fastest regex
         ],
         ascending=[0, 0, 0, 0, 1],
     ).reset_index(drop=True)
 
-    df['correct_findings_id'] = df['correct_findings'].apply(lambda x: set(y.id_local for y in x))
+    df['correct_findings_id'] = df['correct_findings'].apply(lambda x: {y.id_local for y in x})
     df['all_matches_id'] = [set.union(*df.loc[0:i, 'correct_findings_id']) for i in range(len(df.index))]
     df['new_matches_id'] = df.all_matches_id - df.all_matches_id.shift(1)
     null_mask = df['new_matches_id'].isnull()
     df.loc[null_mask, 'new_matches_id'] = df.loc[null_mask]['correct_findings_id']
     df.insert(0, 'new_matches_count', df['new_matches_id'].str.len())
     df = df.drop(['correct_findings_id', 'correct_findings', 'all_matches_id', 'new_matches_id'], axis=1)
 
@@ -138,15 +138,15 @@
     # get the index of all good regex
     index_of_regex = df[df['new_matches_count'] > 0].index
 
     if log_stats:
         stats = df.loc[index_of_regex][
             ['regex', 'runtime', 'annotation_recall', 'annotation_precision', 'f1_score', 'new_matches_count']
         ]
-        logger.info(f'\n\n{tabulate(stats, floatfmt=".4f", headers="keys", tablefmt="pipe")}\n')
+        logger.debug(f'\n\n{tabulate(stats, floatfmt=".4f", headers="keys", tablefmt="pipe")}\n')
 
     # best_regex = df.loc[index_of_regex, 'regex'].to_list()
     best_regex = df.loc[df['new_matches_count'] > 0, 'regex'].to_list()
 
     return best_regex
 
 
@@ -181,15 +181,14 @@
         match = re.search(r'\?P<.*?>', regex)  # match the invalid group name
         group_name = match.group(0)  # get the string representation
         group_name = group_name.replace('?P<', '?P<_')  # add a leading underscore
         regex = re.sub(r'\?P<.*?>', group_name, regex)  # replace invalid group name with new one
         pattern = re.compile(regex, flags=flags)  # try the compile again
 
     for match in pattern.finditer(doctext, overlapped=overlapped):
-
         # hold results per match
         _results = []
 
         if match.groups():
             # parse named groups, if available
             for group_name, group_index in match.re.groupindex.items():
                 if match[group_index] is not None:
@@ -241,22 +240,23 @@
         # allow to use similar group names, you can use "Ort_" if the group name is "Ort_255_259"
         return [result for result in results if filtered_group in result['regex_group']]
     else:
         return results
 
 
 def generic_candidate_function(regex, flags=0, overlapped=False, filtered_group=None):
-    """Regex approach tob build a candidate function by one regex.
+    """Regex approach to build a candidate function by one regex.
 
     :param filtered_group: If a regex contains multiple named groups, you can filter the respective group by name
     :param overlapped: Indicate if regex matches can overlapp.
     :param regex: Regex to create a candidate_function.
     :param flags: Regex flag which should be considered.
     :return: An initialized candidate function.
     """
+
     # function to build candidates
     def candidate_function(doctext):
         """
         Split the text in candidates and other text chunks.
 
         :param doctext: Text of the candidate
         :return: Tuple of list of candidates and other text chunks
@@ -283,9 +283,9 @@
         for span in candidates_spans:
             other_text.append(doctext[previous : span[0]])
             previous = span[1]
         other_text.append(doctext[previous:])
 
         return candidates, other_text, candidates_spans
 
-    candidate_function.__name__ = f"regex_{regex}"
+    candidate_function.__name__ = f'regex_{regex}'
     return candidate_function
```

### Comparing `konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk/tokenizer/regex.py` & `konfuzio_sdk-0.3.0/konfuzio_sdk/tokenizer/regex.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Regex tokenizers."""
 import logging
 import time
 from typing import List
 
-
-from konfuzio_sdk.data import Annotation, Document, Category, Span
+from konfuzio_sdk.data import Annotation, Document, Span
 from konfuzio_sdk.regex import regex_matches
 from konfuzio_sdk.tokenizer.base import AbstractTokenizer, ProcessingStep
 from konfuzio_sdk.utils import sdk_isinstance
 
 logger = logging.getLogger(__name__)
 
 
@@ -18,54 +17,48 @@
     def __init__(self, regex: str):
         """Initialize the RegexTokenizer."""
         self.regex = regex
         self.processing_steps = []
 
     def __repr__(self):
         """Return string representation of the class."""
-        return f"{self.__class__.__name__}: {repr(self.regex)}"
+        return f'{self.__class__.__name__}: {repr(self.regex)}'
 
     def __hash__(self):
         """Get unique hash for RegexTokenizer."""
         return hash(repr(self.regex))
 
-    def __eq__(self, other) -> bool:
-        """Compare RegexTokenizer with another Tokenizer."""
-        return hash(self) == hash(other)
-
-    def fit(self, category: Category):
-        """Fit the tokenizer accordingly with the Documents of the Category."""
-        assert sdk_isinstance(category, Category)
-        return self
-
     def tokenize(self, document: Document) -> Document:
         """
         Create Annotations with 1 Span based on the result of the Tokenizer.
 
         :param document: Document to tokenize, can have been tokenized before
         :return: Document with Spans created by the Tokenizer.
         """
         assert sdk_isinstance(document, Document)
         if document.text is None:
             raise NotImplementedError(f'{document} cannot be tokenized when text is None.')
 
         before_none = len(document.annotations(use_correct=False, label=document.project.no_label))
 
         t0 = time.monotonic()
-        spans = []
+        spans = {}
         # do not keep the full regex match as we will see many matches whitespaces as pre or suffix
         for span_info in regex_matches(document.text, self.regex, keep_full_match=False):
             span = Span(start_offset=span_info['start_offset'], end_offset=span_info['end_offset'])
             span.regex_matching.append(self)
-            if span not in spans:  # do not use duplicated spans  # todo add test
-                spans.append(span)
+            if (
+                span_info['start_offset'],
+                span_info['end_offset'],
+            ) not in spans:  # do not use duplicated spans  # todo add test
+                spans[(span_info['start_offset'], span_info['end_offset'])] = span
 
         # Create a revised = False and is_correct = False (defaults) Annotation
         document_spans = {(span.start_offset, span.end_offset): span for span in document.spans()}
-        for span in spans:
+        for span in spans.values():
             span_key = (span.start_offset, span.end_offset)
             if span_key not in document_spans:  # (use_correct=False):
                 document_spans[span_key] = span
                 # todo this hides the fact, that Tokenizers of different quality can create the same Span
                 # todo we create an overlapping Annotation in case the Tokenizer finds a correct match
                 annotation = Annotation(
                     document=document,
@@ -83,15 +76,15 @@
                         # annotation.delete()  # todo we should skip Annotations that have no valide bbox
                     # except TypeError as e:
                     #   logger.error(f'Typeerror Bbox of {span} "{span.offset_string}": {repr(e)} - {span.eval_dict()}')
                     #   # annotation.delete()  # todo we should skip Annotations that have no valide bbox
             else:
                 if self not in document_spans[span_key].regex_matching:
                     document_spans[span_key].regex_matching.append(self)  # add tokenizer to Span.regex_matches:
-                logger.warning(f'{document} contains {span} already. It will not be added by the Tokenizer.')
+                logger.debug(f'{document} contains {span} already. It will not be added by the Tokenizer.')
         after_none = len(document.annotations(use_correct=False, label=document.project.no_label))
         logger.info(f'{after_none - before_none} new Annotations in {document} by {repr(self)}.')
 
         self.processing_steps.append(ProcessingStep(self, document, time.monotonic() - t0))
 
         return document
```

### Comparing `konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk/trainer/information_extraction.py` & `konfuzio_sdk-0.3.0/konfuzio_sdk/trainer/information_extraction.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,284 +1,64 @@
 """Extract information from Documents.
 
 Conventional template matching based approaches fail to generalize well to document images of unseen templates,
 and are not robust against text recognition errors.
 
-We follow the approach proposed by Sun et. al (2021) to encode both the visual and textual
+We follow the approach proposed by Sun et al. (2021) to encode both the visual and textual
 features of detected text regions, and edges of which represent the spatial relations between neighboring text
 regions. Their experiments validate that all information including visual features, textual
 features and spatial relations can benefit key information extraction.
 
 We reduce the hardware requirements from 1 NVIDIA Titan X GPUs with 12 GB memory to a 1 CPU and 16 GB memory by
 replacing the end-to-end pipeline into two parts.
 
 Sun, H., Kuang, Z., Yue, X., Lin, C., & Zhang, W. (2021). Spatial Dual-Modality Graph Reasoning for Key Information
 Extraction. arXiv. https://doi.org/10.48550/ARXIV.2103.14470
 """
-import bz2
 import collections
 import difflib
 import functools
-import itertools
 import logging
 import os
-import pathlib
-import shutil
-import sys
 import time
 import unicodedata
 from copy import deepcopy
 from heapq import nsmallest
-from typing import Tuple, Optional, List, Union, Callable, Dict
-from warnings import warn
+from inspect import signature
+from typing import Dict, List, Optional, Tuple, Union
 
 import numpy
 import pandas
-import cloudpickle
-from pympler import asizeof
 from sklearn.ensemble import RandomForestClassifier
 from sklearn.utils.validation import check_is_fitted
-from tabulate import tabulate
 
-from konfuzio_sdk.data import Data, Document, Annotation, Category, AnnotationSet, Label, LabelSet, Span
+from konfuzio_sdk.data import Annotation, AnnotationSet, Category, Document, Label, LabelSet, Span
+from konfuzio_sdk.evaluate import ExtractionEvaluation
 from konfuzio_sdk.normalize import (
-    normalize_to_float,
     normalize_to_date,
+    normalize_to_float,
     normalize_to_percentage,
     normalize_to_positive_float,
 )
 from konfuzio_sdk.regex import regex_matches
-from konfuzio_sdk.utils import get_timestamp, get_bbox, normalize_memory
-from konfuzio_sdk.evaluate import Evaluation
+from konfuzio_sdk.tokenizer.base import ListTokenizer
+from konfuzio_sdk.tokenizer.paragraph_and_sentence import ParagraphTokenizer, SentenceTokenizer
+from konfuzio_sdk.trainer.base import BaseModel
+from konfuzio_sdk.utils import (
+    get_bbox,
+    get_timestamp,
+    memory_size_of,
+    sdk_isinstance,
+)
 
 logger = logging.getLogger(__name__)
 
 """Multiclass classifier for document extraction."""
 CANDIDATES_CACHE_SIZE = 100
 
-warn('This module is WIP: https://gitlab.com/konfuzio/objectives/-/issues/9311', FutureWarning, stacklevel=2)
-
-
-def load_model(pickle_path: str, max_ram: Union[None, str] = None):
-    """
-    Load a pkl file.
-
-    :param pickle_path: Path to the pickled model.
-    :raises FileNotFoundError: If the path is invalid.
-    :raises OSError: When the data is corrupted or invalid and cannot be loaded.
-    :raises TypeError: When the loaded pickle isn't recognized as a Konfuzio AI model.
-    :return: Extraction AI model.
-    """
-    if not os.path.isfile(pickle_path):
-        raise FileNotFoundError("Invalid pickle file path:", pickle_path)
-
-    # The current local id iterator might otherwise be overriden
-    prev_local_id = next(Data.id_iter)
-
-    try:
-        with bz2.open(pickle_path, 'rb') as file:
-            model = cloudpickle.load(file)
-    except OSError:
-        raise OSError(f"Pickle file {pickle_path} data is invalid.")
-    except AttributeError as err:
-        if "__forward_module__" in str(err) and '3.9' in sys.version:
-            raise AttributeError("Pickle saved with incompatible Python version.") from err
-        elif "__forward_is_class__" in str(err) and '3.8' in sys.version:
-            raise AttributeError("Pickle saved with incompatible Python version.") from err
-        raise
-    except ValueError as err:
-        if "unsupported pickle protocol: 5" in str(err) and '3.7' in sys.version:
-            raise ValueError("Pickle saved with incompatible Python version.") from err
-        raise
-
-    max_ram = normalize_memory(max_ram)
-    if max_ram and asizeof.asizeof(model) > max_ram:
-        logger.error(f"Loaded model's memory use ({asizeof.asizeof(model)}) is greater than max_ram ({max_ram})")
-
-    if not hasattr(model, "name"):
-        raise TypeError("Saved model file needs to be a Konfuzio Trainer instance.")
-    elif model.name in {
-        "DocumentAnnotationMultiClassModel",
-        "DocumentEntityMulticlassModel",
-        "SeparateLabelsAnnotationMultiClassModel",
-        "SeparateLabelsEntityMultiClassModel",
-    }:
-        logger.warning(f"Loading legacy {model.name} AI model.")
-    else:
-        logger.info(f"Loading {model.name} AI model.")
-
-    curr_local_id = next(Data.id_iter)
-    Data.id_iter = itertools.count(max(prev_local_id, curr_local_id))
-
-    return model
-
-
-def get_offsets_per_page(doc_text: str) -> Dict:
-    """Get the first start and last end offsets per page."""
-    page_text = doc_text.split('\f')
-    start = 0
-    starts_ends_per_page = {}
-
-    for ind, page in enumerate(page_text):
-        len_page = len(page)
-        end = start + len_page
-        starts_ends_per_page[ind] = (start, end)
-        start = end + 1
-
-    return starts_ends_per_page
-
-
-def get_bboxes_by_coordinates(doc_bbox: Dict, selection_bboxes: List[Dict]) -> List[Dict]:
-    """
-    Get the bboxes of the characters contained in the selection bboxes.
-
-    todo: is this a duplicate of get_merged_bboxes in konfuzio_sdk.utils ?
-
-    Simplifies `get_bboxes`..
-
-    Returns a list of bboxes.
-    :param doc_bbox: Bboxes of the characters in the document.
-    :param selection_bboxes: Bboxes from which to get the info of the characters that they include.
-    :return: List of the bboxes of the characters included in selection_bboxes.
-    """
-    # initialize the list of bboxes that will later be returned
-    final_bboxes = []
-
-    # convert string indexes to int
-    doc_bbox = {int(index): char_bbox for index, char_bbox in doc_bbox.items()}
-
-    # iterate through every bbox of the selection
-    for selection_bbox in selection_bboxes:
-        selected_bboxes = [
-            # the index of the character is its offset, i.e. the number of chars before it in the document's text
-            {**char_bbox}
-            for index, char_bbox in doc_bbox.items()
-            if selection_bbox["page_index"] == char_bbox["page_number"] - 1
-            # filter the characters of the document according to their x/y values, so that we only include the
-            # characters that are inside the selection
-            and selection_bbox["x0"] <= char_bbox["x0"]
-            and selection_bbox["x1"] >= char_bbox["x1"]
-            and selection_bbox["y0"] <= char_bbox["y0"]
-            and selection_bbox["y1"] >= char_bbox["y1"]
-        ]
-
-        final_bboxes.extend(selected_bboxes)
-
-    return final_bboxes
-
-
-def is_valid_merge_vertical(
-    row: pandas.Series, buffer: List[pandas.Series], doc_bbox: Dict, offsets_per_page: Dict
-) -> bool:
-    """
-    Verify if the vertical merging that we are trying to do is valid.
-
-    To be valid, it has to respect 2 conditions:
-
-    1. There is an overlap in the x coordinates of the bbox that includes the entities in the buffer and the row x
-     coordinates.
-
-    2. The bbox that includes the entities in the buffer and the row does not include any other character of the
-    document.
-
-    To check the 2nd condition, we get the bboxes of the characters from the entities in the buffer and the entity in
-    the row:
-    a) based on their start and end offsets
-    b) based on the bounding box that includes all these entities
-
-    b should not include any character that is not in a.
-
-    :param row: Row candidate to be merged to what is already in the buffer.
-    :param buffer: Previous information.
-    :param doc_bbox: Bboxes of the characters in the document.
-    :param offsets_per_page: Start and end offset of each page in the document.
-    :return: If the merge is valid or not.
-    """
-    # Bbox formed by the entities in the buffer.
-    buffer_bbox = {
-        'x0': min([b['x0'] for b in buffer]),
-        'x1': max([b['x1'] for b in buffer]),
-        'y0': min([b['y0'] for b in buffer]),
-        'y1': max([b['y1'] for b in buffer]),
-    }
-
-    # 1. There is an overlap in x coordinates
-    is_overlap = (
-        buffer_bbox['x1'] >= row['x0'] >= buffer_bbox['x0']
-        or buffer_bbox['x1'] >= row['x1'] >= buffer_bbox['x0']
-        or (buffer_bbox['x0'] >= row['x0'] and row['x1'] >= buffer_bbox['x1'])
-    )  # NOQA
-
-    if not is_overlap:
-        return False
-
-    # 2. There is no other characters if the buffer bbox is updated with the current row
-    # update buffer with row
-    temp_buffer = buffer.copy()
-    temp_buffer.append(row)
-
-    # get page index (necessary to select the bboxes of the characters)
-    for buf in temp_buffer:
-        for page_index, offsets in offsets_per_page.items():
-            if buf['start_offset'] >= offsets[0] and buf['end_offset'] <= offsets[1]:
-                break
-
-        buf['page_index'] = page_index
-
-    if len(set([buf['page_index'] for buf in temp_buffer])) > 1:
-        logger.info('Merging annotations across pages is not possible.')
-        return False
-
-    # get bboxes by start and end offsets of each row in the temp buffer
-    bboxes_by_offset = []
-    for buf in temp_buffer:
-        char_bboxes = [
-            doc_bbox[str(char_bbox_id)]
-            for char_bbox_id in range(buf['start_offset'], buf['end_offset'] + 1)
-            if str(char_bbox_id) in doc_bbox
-        ]
-        bboxes_by_offset.extend(char_bboxes)
-
-    # get bboxes contained in the bbox of the temp buffer
-    buffer_row_bbox = {
-        'x0': min([buffer_bbox['x0'], row['x0']]),
-        'x1': max([buffer_bbox['x1'], row['x1']]),
-        'y0': min([buffer_bbox['y0'], row['y0']]),
-        'y1': max([buffer_bbox['y1'], row['y1']]),
-        'page_index': temp_buffer[0]['page_index'],
-    }
-
-    bboxes_by_coordinates = get_bboxes_by_coordinates(doc_bbox, [buffer_row_bbox])
-
-    # check if there are bboxes in the merged bbox that are not part of the ones obtained by the offsets
-    diff = [x for x in bboxes_by_coordinates if x not in bboxes_by_offset and x['text'] != ' ']
-    no_diffs = len(diff) == 0
-
-    return no_diffs
-
-
-def substring_count(list: list, substring: str) -> list:
-    """Given a list of strings returns the occurrence of a certain substring and returns the results as a list."""
-    r_list = [0] * len(list)
-
-    for index in range(len(list)):
-        r_list[index] = list[index].lower().count(substring)
-
-    return r_list
-
-
-def dict_to_dataframe(res_dict):
-    """Convert a Dict to Dataframe add label as column."""
-    df = pandas.DataFrame()
-    for name in res_dict.keys():
-        label_df = res_dict[name]
-        label_df['result_name'] = name
-        df = df.append(label_df, sort=True)
-    return df
-
 
 # # existent model classes
 # MODEL_CLASSES = {'LabelSectionModel': LabelSectionModel,
 #                  'DocumentModel': DocumentModel,
 #                  'ParagraphModel': ParagraphModel,
 #                  'CustomDocumentModel': CustomDocumentModel,
 #                  'SentenceModel': SentenceModel
@@ -446,94 +226,106 @@
 #                 file_data = dill.load(f)
 #
 #     return file_data
 
 
 def convert_to_feat(offset_string_list: list, ident_str: str = '') -> pandas.DataFrame:
     """Return a df containing all the features generated using the offset_string."""
-    df = pandas.DataFrame()
+    df = {}  # pandas.DataFrame()
 
     # strip all accents
     offset_string_list_accented = offset_string_list
     offset_string_list = [strip_accents(s) for s in offset_string_list]
 
     # gets the return lists for all the features
-    df[ident_str + "feat_vowel_len"] = [vowel_count(s) for s in offset_string_list]
-    df[ident_str + "feat_special_len"] = [special_count(s) for s in offset_string_list]
-    df[ident_str + "feat_space_len"] = [space_count(s) for s in offset_string_list]
-    df[ident_str + "feat_digit_len"] = [digit_count(s) for s in offset_string_list]
-    df[ident_str + "feat_len"] = [len(s) for s in offset_string_list]
-    df[ident_str + "feat_upper_len"] = [upper_count(s) for s in offset_string_list]
-    df[ident_str + "feat_date_count"] = [date_count(s) for s in offset_string_list]
-    df[ident_str + "feat_num_count"] = [num_count(s) for s in offset_string_list]
-    df[ident_str + "feat_as_float"] = [normalize_to_python_float(offset_string) for offset_string in offset_string_list]
-    df[ident_str + "feat_unique_char_count"] = [unique_char_count(s) for s in offset_string_list]
-    df[ident_str + "feat_duplicate_count"] = [duplicate_count(s) for s in offset_string_list]
-    df[ident_str + "accented_char_count"] = [
+    df[ident_str + 'feat_vowel_len'] = [vowel_count(s) for s in offset_string_list]
+    df[ident_str + 'feat_special_len'] = [special_count(s) for s in offset_string_list]
+    df[ident_str + 'feat_space_len'] = [space_count(s) for s in offset_string_list]
+    df[ident_str + 'feat_digit_len'] = [digit_count(s) for s in offset_string_list]
+    df[ident_str + 'feat_len'] = [len(s) for s in offset_string_list]
+    df[ident_str + 'feat_upper_len'] = [upper_count(s) for s in offset_string_list]
+    df[ident_str + 'feat_date_count'] = [date_count(s) for s in offset_string_list]
+    df[ident_str + 'feat_num_count'] = [num_count(s) for s in offset_string_list]
+    df[ident_str + 'feat_as_float'] = [normalize_to_python_float(offset_string) for offset_string in offset_string_list]
+    df[ident_str + 'feat_unique_char_count'] = [unique_char_count(s) for s in offset_string_list]
+    df[ident_str + 'feat_duplicate_count'] = [duplicate_count(s) for s in offset_string_list]
+    df[ident_str + 'accented_char_count'] = [
         count_string_differences(s1, s2) for s1, s2 in zip(offset_string_list, offset_string_list_accented)
     ]
 
     (
-        df[ident_str + "feat_year_count"],
-        df[ident_str + "feat_month_count"],
-        df[ident_str + "feat_day_count"],
+        df[ident_str + 'feat_year_count'],
+        df[ident_str + 'feat_month_count'],
+        df[ident_str + 'feat_day_count'],
     ) = year_month_day_count(offset_string_list)
 
-    df[ident_str + "feat_substring_count_slash"] = substring_count(offset_string_list, "/")
-    df[ident_str + "feat_substring_count_percent"] = substring_count(offset_string_list, "%")
-    df[ident_str + "feat_substring_count_e"] = substring_count(offset_string_list, "e")
-    df[ident_str + "feat_substring_count_g"] = substring_count(offset_string_list, "g")
-    df[ident_str + "feat_substring_count_a"] = substring_count(offset_string_list, "a")
-    df[ident_str + "feat_substring_count_u"] = substring_count(offset_string_list, "u")
-    df[ident_str + "feat_substring_count_i"] = substring_count(offset_string_list, "i")
-    df[ident_str + "feat_substring_count_f"] = substring_count(offset_string_list, "f")
-    df[ident_str + "feat_substring_count_s"] = substring_count(offset_string_list, "s")
-    df[ident_str + "feat_substring_count_oe"] = substring_count(offset_string_list, "ö")
-    df[ident_str + "feat_substring_count_ae"] = substring_count(offset_string_list, "ä")
-    df[ident_str + "feat_substring_count_ue"] = substring_count(offset_string_list, "ü")
-    df[ident_str + "feat_substring_count_er"] = substring_count(offset_string_list, "er")
-    df[ident_str + "feat_substring_count_str"] = substring_count(offset_string_list, "str")
-    df[ident_str + "feat_substring_count_k"] = substring_count(offset_string_list, "k")
-    df[ident_str + "feat_substring_count_r"] = substring_count(offset_string_list, "r")
-    df[ident_str + "feat_substring_count_y"] = substring_count(offset_string_list, "y")
-    df[ident_str + "feat_substring_count_en"] = substring_count(offset_string_list, "en")
-    df[ident_str + "feat_substring_count_g"] = substring_count(offset_string_list, "g")
-    df[ident_str + "feat_substring_count_ch"] = substring_count(offset_string_list, "ch")
-    df[ident_str + "feat_substring_count_sch"] = substring_count(offset_string_list, "sch")
-    df[ident_str + "feat_substring_count_c"] = substring_count(offset_string_list, "c")
-    df[ident_str + "feat_substring_count_ei"] = substring_count(offset_string_list, "ei")
-    df[ident_str + "feat_substring_count_on"] = substring_count(offset_string_list, "on")
-    df[ident_str + "feat_substring_count_ohn"] = substring_count(offset_string_list, "ohn")
-    df[ident_str + "feat_substring_count_n"] = substring_count(offset_string_list, "n")
-    df[ident_str + "feat_substring_count_m"] = substring_count(offset_string_list, "m")
-    df[ident_str + "feat_substring_count_j"] = substring_count(offset_string_list, "j")
-    df[ident_str + "feat_substring_count_h"] = substring_count(offset_string_list, "h")
-
-    df[ident_str + "feat_substring_count_plus"] = substring_count(offset_string_list, "+")
-    df[ident_str + "feat_substring_count_minus"] = substring_count(offset_string_list, "-")
-    df[ident_str + "feat_substring_count_period"] = substring_count(offset_string_list, ".")
-    df[ident_str + "feat_substring_count_comma"] = substring_count(offset_string_list, ",")
+    df[ident_str + 'feat_substring_count_slash'] = substring_count(offset_string_list, '/')
+    df[ident_str + 'feat_substring_count_percent'] = substring_count(offset_string_list, '%')
+    df[ident_str + 'feat_substring_count_e'] = substring_count(offset_string_list, 'e')
+    df[ident_str + 'feat_substring_count_g'] = substring_count(offset_string_list, 'g')
+    df[ident_str + 'feat_substring_count_a'] = substring_count(offset_string_list, 'a')
+    df[ident_str + 'feat_substring_count_u'] = substring_count(offset_string_list, 'u')
+    df[ident_str + 'feat_substring_count_i'] = substring_count(offset_string_list, 'i')
+    df[ident_str + 'feat_substring_count_f'] = substring_count(offset_string_list, 'f')
+    df[ident_str + 'feat_substring_count_s'] = substring_count(offset_string_list, 's')
+    df[ident_str + 'feat_substring_count_oe'] = substring_count(offset_string_list, 'ö')
+    df[ident_str + 'feat_substring_count_ae'] = substring_count(offset_string_list, 'ä')
+    df[ident_str + 'feat_substring_count_ue'] = substring_count(offset_string_list, 'ü')
+    df[ident_str + 'feat_substring_count_er'] = substring_count(offset_string_list, 'er')
+    df[ident_str + 'feat_substring_count_str'] = substring_count(offset_string_list, 'str')
+    df[ident_str + 'feat_substring_count_k'] = substring_count(offset_string_list, 'k')
+    df[ident_str + 'feat_substring_count_r'] = substring_count(offset_string_list, 'r')
+    df[ident_str + 'feat_substring_count_y'] = substring_count(offset_string_list, 'y')
+    df[ident_str + 'feat_substring_count_en'] = substring_count(offset_string_list, 'en')
+    df[ident_str + 'feat_substring_count_g'] = substring_count(offset_string_list, 'g')
+    df[ident_str + 'feat_substring_count_ch'] = substring_count(offset_string_list, 'ch')
+    df[ident_str + 'feat_substring_count_sch'] = substring_count(offset_string_list, 'sch')
+    df[ident_str + 'feat_substring_count_c'] = substring_count(offset_string_list, 'c')
+    df[ident_str + 'feat_substring_count_ei'] = substring_count(offset_string_list, 'ei')
+    df[ident_str + 'feat_substring_count_on'] = substring_count(offset_string_list, 'on')
+    df[ident_str + 'feat_substring_count_ohn'] = substring_count(offset_string_list, 'ohn')
+    df[ident_str + 'feat_substring_count_n'] = substring_count(offset_string_list, 'n')
+    df[ident_str + 'feat_substring_count_m'] = substring_count(offset_string_list, 'm')
+    df[ident_str + 'feat_substring_count_j'] = substring_count(offset_string_list, 'j')
+    df[ident_str + 'feat_substring_count_h'] = substring_count(offset_string_list, 'h')
+
+    df[ident_str + 'feat_substring_count_plus'] = substring_count(offset_string_list, '+')
+    df[ident_str + 'feat_substring_count_minus'] = substring_count(offset_string_list, '-')
+    df[ident_str + 'feat_substring_count_period'] = substring_count(offset_string_list, '.')
+    df[ident_str + 'feat_substring_count_comma'] = substring_count(offset_string_list, ',')
+
+    df[ident_str + 'feat_starts_with_plus'] = starts_with_substring(offset_string_list, '+')
+    df[ident_str + 'feat_starts_with_minus'] = starts_with_substring(offset_string_list, '-')
 
-    df[ident_str + "feat_starts_with_plus"] = starts_with_substring(offset_string_list, "+")
-    df[ident_str + "feat_starts_with_minus"] = starts_with_substring(offset_string_list, "-")
+    df[ident_str + 'feat_ends_with_plus'] = ends_with_substring(offset_string_list, '+')
+    df[ident_str + 'feat_ends_with_minus'] = ends_with_substring(offset_string_list, '-')
 
-    df[ident_str + "feat_ends_with_plus"] = ends_with_substring(offset_string_list, "+")
-    df[ident_str + "feat_ends_with_minus"] = ends_with_substring(offset_string_list, "-")
+    df = pandas.DataFrame(df)
 
     return df
 
 
-def starts_with_substring(list: list, substring: str) -> list:
+def substring_count(list_of_strings: list, substring: str) -> list:
+    """Given a list of strings returns the occurrence of a certain substring and returns the results as a list."""
+    r_list = [0] * len(list_of_strings)
+
+    for index in range(len(list_of_strings)):
+        r_list[index] = list_of_strings[index].lower().count(substring)
+
+    return r_list
+
+
+def starts_with_substring(list_of_strings: list, substring: str) -> list:
     """Given a list of strings return 1 if string starts with the given substring for each item."""
-    return [1 if s.lower().startswith(substring) else 0 for s in list]
+    return [1 if s.lower().startswith(substring) else 0 for s in list_of_strings]
 
 
-def ends_with_substring(list: list, substring: str) -> list:
+def ends_with_substring(list_of_strings: list, substring: str) -> list:
     """Given a list of strings return 1 if string starts with the given substring for each item."""
-    return [1 if s.lower().endswith(substring) else 0 for s in list]
+    return [1 if s.lower().endswith(substring) else 0 for s in list_of_strings]
 
 
 def digit_count(s: str) -> int:
     """Return the number of digits in a string."""
     return sum(c.isdigit() for c in s)
 
 
@@ -584,24 +376,26 @@
     Given a string this function tries to read it as a date (if not possible returns 0).
 
     If possible it returns the relative difference to 01.01.2010 in days.
     """
     # checks the format
     if len(s) > 5:
         if (s[2] == '.' and s[5] == '.') or (s[2] == '/' and s[5] == '/'):
-            date1 = pandas.to_datetime("01.01.2010")
-            date2 = pandas.to_datetime(s, errors='ignore')
+            date1 = pandas.to_datetime('01.01.2010', dayfirst=True)
+            date2 = normalize_to_date(s)
+            if not date2:
+                return 0
+            date2 = pandas.to_datetime(date2, errors='ignore')
             if date2 == s:
                 return 0
-
             else:
                 try:
                     diff = int((date2 - date1) / numpy.timedelta64(1, 'D'))
                 except TypeError as e:
-                    logger.error(f'Could not substract for string {s} because of >>{e}<<.')
+                    logger.debug(f'Could not substract for string {s} because of >>{e}<<.')
                     return 0
 
             if diff == 0:
                 return 1
             else:
                 return diff
 
@@ -678,86 +472,15 @@
             counter += count[key]
 
     return counter
 
 
 def unique_char_count(s: str) -> int:
     """Given a string returns the number of unique characters."""
-    return len(set(list(s)))
-
-
-def _convert_to_relative_dict(dict: dict):
-    """Convert a dict with absolute numbers as values to the same dict with the relative probabilities as values."""
-    return_dict = {}
-    abs_num = sum(dict.values())
-    for key, value in dict.items():
-        return_dict[key] = value / abs_num
-    return return_dict
-
-
-def plot_label_distribution(df_list: list, df_name_list=None) -> None:
-    """Plot the label-distribution of given DataFrames side-by-side."""
-    # check if any of the input df are empty
-    for df in df_list:
-        if df.empty:
-            logger.error('One of the Dataframes in df_list is empty.')
-            return None
-
-    # helper function
-    def Convert(tup, di):
-        for a, b in tup:
-            di.setdefault(a, []).append(b)
-        return di
-
-    # plot the relative distributions
-    logger.info('Percentage of total samples (per dataset) that have a certain label:')
-    rel_dict_list = []
-    for df in df_list:
-        rel_dict_list.append(_convert_to_relative_dict(collections.Counter(list(df['label_name']))))
-    logger.info(
-        '\n'
-        + tabulate(
-            pandas.DataFrame(rel_dict_list, index=df_name_list).transpose(),
-            floatfmt=".1%",
-            headers="keys",
-            tablefmt="pipe",
-        )
-        + '\n'
-    )
-
-    # print the number of documents in total and in the splits given
-    # total_count = 0
-    for index, df in enumerate(df_list):
-        doc_name = df_name_list[index] if df_name_list else str(index)
-        doc_count = len(set(df['document_id']))
-        logger.info(doc_name + ' contains ' + str(doc_count) + ' different documents.')
-        # total_count += doc_count
-    # logger.info(str(total_count) + ' documents in total.')
-
-    # plot the number of documents with at least one of a certain label
-    logger.info('Percentage of documents per split that contain a certain label at least once:')
-    doc_count_dict_list = []
-    for df in df_list:
-        doc_count_dict = {}
-        doc_count = len(set(df['document_id']))
-        toup_list = list(zip(list(df['label_name']), list(df['document_id'])))
-        list_dict = Convert(toup_list, {})
-        for key, value in list_dict.items():
-            doc_count_dict[key] = float(len(set(value)) / doc_count)
-        doc_count_dict_list.append(doc_count_dict)
-    logger.info(
-        '\n'
-        + tabulate(
-            pandas.DataFrame(doc_count_dict_list, index=df_name_list).transpose(),
-            floatfmt=".1%",
-            headers="keys",
-            tablefmt="pipe",
-        )
-        + '\n'
-    )
+    return len(set(s))
 
 
 def get_first_candidate(document_text, document_bbox, line_list):
     """Get the first candidate in a document."""
     # todo allow to have mult tokenizers?
     for line_num, _line in enumerate(line_list):
         line_start_offset = _line['start_offset']
@@ -806,17 +529,14 @@
 
 
 def process_document_data(
     document: Document,
     spans: List[Span],
     n_nearest: Union[int, List, Tuple] = 2,
     first_word: bool = True,
-    tokenize_fn: Optional[Callable] = None,
-    substring_features=None,
-    catchphrase_list=None,
     n_nearest_across_lines: bool = False,
 ) -> Tuple[pandas.DataFrame, List, pandas.DataFrame]:
     """
     Convert the json_data from one Document to a DataFrame that can be used for training or prediction.
 
     Additionally returns the fake negatives, errors and conflicting annotations as a DataFrames and of course the
     column_order for training
@@ -831,20 +551,20 @@
     if isinstance(n_nearest, int):
         n_left_nearest = n_nearest
         n_right_nearest = n_nearest
     else:
         assert isinstance(n_nearest, (tuple, list)) and len(n_nearest) == 2
         n_left_nearest, n_right_nearest = n_nearest
 
-    l_keys = ["l_dist" + str(x) for x in range(n_left_nearest)]
-    r_keys = ["r_dist" + str(x) for x in range(n_right_nearest)]
+    l_keys = ['l_dist' + str(x) for x in range(n_left_nearest)]
+    r_keys = ['r_dist' + str(x) for x in range(n_right_nearest)]
 
     if n_nearest_across_lines:
-        l_keys += ["l_pos" + str(x) for x in range(n_left_nearest)]
-        r_keys += ["r_pos" + str(x) for x in range(n_right_nearest)]
+        l_keys += ['l_pos' + str(x) for x in range(n_left_nearest)]
+        r_keys += ['r_pos' + str(x) for x in range(n_right_nearest)]
 
     document_bbox = document.get_bbox()
     document_text = document.text
     document_n_pages = document.number_of_pages
 
     if document_text is None or document_bbox == {} or len(spans) == 0:
         # if the document text is empty or if there are no ocr'd characters
@@ -854,46 +574,24 @@
     line_list: List[Dict] = []
     char_counter = 0
     for line_text in document_text.replace('\f', '\n').split('\n'):
         n_chars_on_line = len(line_text)
         line_list.append({'start_offset': char_counter, 'end_offset': char_counter + n_chars_on_line})
         char_counter += n_chars_on_line + 1
 
-    # generate the Catchphrase-Dataframe
-    if catchphrase_list is not None:
-        occurrence_dict = generate_catchphrase_occurrence_dict(line_list, catchphrase_list, document_text)
-
     if first_word:
         first_candidate = get_first_candidate(document_text, document_bbox, line_list)
         first_word_string = first_candidate['offset_string']
         first_word_x0 = first_candidate['x0']
         first_word_y0 = first_candidate['y0']
         first_word_x1 = first_candidate['x1']
         first_word_y1 = first_candidate['y1']
 
-    # todo document.annotations () should be sorted already - check or update this function
-    spans.sort(key=lambda x: x.start_offset)
-
-    # WIP: Word on page feature
-    page_text_list = document_text.split('\f')
-
-    # used to cache the catchphrase features
-    _line_num = -1
-    _catchphrase_dict = None
-    candidates_cache = dict()
+    candidates_cache = {}
     for span in spans:
-
-        word_on_page_feature_list = []
-        word_on_page_feature_name_list = []
-
-        # WIP: Word on page feature
-        if substring_features:
-            for index, substring_feature in enumerate(substring_features):
-                word_on_page_feature_list.append(substring_on_page(substring_feature, span, page_text_list))
-                word_on_page_feature_name_list.append(f'word_on_page_feat{index}')
         # if span.annotation.id_:
         #     # Annotation
         #     logger.error(f'{span}')
         #     if (
         #         span.annotation.is_correct
         #         or (not span.annotation.is_correct and span.annotation.revised)
         #         or (
@@ -908,32 +606,20 @@
 
         # find the line containing the annotation
         # tokenize that line to get all candidates
         # convert each candidate into a bbox
         # append to line candidates
         # store the line_start_offset so if the next annotation is on the same line then we use the same
         # line_candidiates list and therefore saves us tokenizing the same line again
-        for line_num, line in enumerate(line_list):
-            if line['start_offset'] <= span.end_offset and line['end_offset'] >= span.start_offset:
 
-                # get the catchphrase features
-                if catchphrase_list is not None and len(catchphrase_list) != 0:
-                    if line_num == _line_num:
-                        span.catchphrase_dict = _catchphrase_dict
-                    else:
-                        _catchphrase_dict = generate_feature_dict_from_occurence_dict(
-                            occurrence_dict, catchphrase_list, line_num
-                        )
-                        span.catchphrase_dict = _catchphrase_dict
-                        _line_num = line_num
+        line_num = span.line_index
 
-                line_candidates, candidates_cache = get_line_candidates(
-                    document_text, document_bbox, line_list, line_num, candidates_cache
-                )
-                break
+        line_candidates, candidates_cache = get_line_candidates(
+            document_text, document_bbox, line_list, line_num, candidates_cache
+        )
 
         l_list = []
         r_list = []
 
         # todo add way to calculate distance features between spans consistently
         # https://gitlab.com/konfuzio/objectives/-/issues/9688
         for candidate in line_candidates:
@@ -951,41 +637,49 @@
                 logger.error(f'{candidate}: {str(e)}')
 
         if n_nearest_across_lines:
             prev_line_candidates = []
             i = 1
             while (line_num - i) >= 0:
                 line_candidates, candidates_cache = get_line_candidates(
-                    document_text, document_bbox, line_list, line_num - i, tokenize_fn, candidates_cache
+                    document_text,
+                    document_bbox,
+                    line_list,
+                    line_num - i,
+                    candidates_cache,
                 )
                 for candidate in line_candidates:
                     candidate['dist'] = min(
-                        abs(span.x0 - candidate['x0']),
-                        abs(span.x0 - candidate['x1']),
-                        abs(span.x1 - candidate['x0']),
-                        abs(span.x1 - candidate['x1']),
+                        abs(span.bbox().x0 - candidate['x0']),
+                        abs(span.bbox().x0 - candidate['x1']),
+                        abs(span.bbox().x1 - candidate['x0']),
+                        abs(span.bbox().x1 - candidate['x1']),
                     )
                     candidate['pos'] = -i
                 prev_line_candidates.extend(line_candidates)
                 if len(prev_line_candidates) >= n_left_nearest - len(l_list):
                     break
                 i += 1
 
             next_line_candidates = []
             i = 1
             while line_num + i < len(line_list):
                 line_candidates, candidates_cache = get_line_candidates(
-                    document_text, document_bbox, line_list, line_num + i, tokenize_fn, candidates_cache
+                    document_text,
+                    document_bbox,
+                    line_list,
+                    line_num + i,
+                    candidates_cache,
                 )
                 for candidate in line_candidates:
                     candidate['dist'] = min(
-                        abs(span.x0 - candidate['x0']),
-                        abs(span.x0 - candidate['x1']),
-                        abs(span.x1 - candidate['x0']),
-                        abs(span.x1 - candidate['x1']),
+                        abs(span.bbox().x0 - candidate['x0']),
+                        abs(span.bbox().x0 - candidate['x1']),
+                        abs(span.bbox().x1 - candidate['x0']),
+                        abs(span.bbox().x1 - candidate['x1']),
                     )
                     candidate['pos'] = i
                 next_line_candidates.extend(line_candidates)
                 if len(next_line_candidates) >= n_right_nearest - len(r_list):
                     break
                 i += 1
 
@@ -1023,33 +717,20 @@
                 span_dict['l_pos' + str(index)] = item['pos']
         for index, item in enumerate(r_list):
             span_dict['r_dist' + str(index)] = item['dist']
             span_dict['r_offset_string' + str(index)] = item['offset_string']
             if n_nearest_across_lines:
                 span_dict['r_pos' + str(index)] = item['pos']
 
-        # WIP: word on page feature
-        for index, item in enumerate(word_on_page_feature_list):
-            span_dict['word_on_page_feat' + str(index)] = item
-
-        # if annotation.label and annotation.label.threshold:
-        #     annotation_dict["threshold"] = annotation.label.threshold
-        # else:
-        #     annotation_dict["threshold"] = 0.1
-
-        if _catchphrase_dict:
-            for catchphrase, dist in _catchphrase_dict.items():
-                span_dict['catchphrase_dist_' + catchphrase] = dist
-
         # checks for ERRORS
-        if span_dict["confidence"] is None and not (span_dict["revised"] is False and span_dict["is_correct"] is True):
+        if span_dict['confidence'] is None and not (span_dict['revised'] is False and span_dict['is_correct'] is True):
             file_error_data.append(span_dict)
 
         # adds the sample_data to the list
-        if span_dict["page_index"] is not None:
+        if span_dict['page_index'] is not None:
             file_data_raw.append(span_dict)
 
     # creates the dataframe
     df = pandas.DataFrame(file_data_raw)
     df_errors = pandas.DataFrame(file_error_data)
 
     # first word features
@@ -1057,246 +738,242 @@
         df['first_word_x0'] = first_word_x0
         df['first_word_x1'] = first_word_x1
         df['first_word_y0'] = first_word_y0
         df['first_word_y1'] = first_word_y1
         df['first_word_string'] = first_word_string
 
         # first word string features
-        df_string_features_first = convert_to_feat(list(df["first_word_string"]), "first_word_")
-        string_features_first_word = list(df_string_features_first.columns.values)  # NOQA
+        df_string_features_first = convert_to_feat(list(df['first_word_string']), 'first_word_')
+        string_features_first_word = list(df_string_features_first.columns.values)
         df = df.join(df_string_features_first, lsuffix='_caller', rsuffix='_other')
         first_word_features = ['first_word_x0', 'first_word_y0', 'first_word_x1', 'first_word_y1']
+        first_word_features += string_features_first_word
 
     # creates all the features from the offset string
-    df_string_features_real = convert_to_feat(list(df["offset_string"]))
+    df_string_features_real = convert_to_feat(list(df['offset_string']))
     string_feature_column_order = list(df_string_features_real.columns.values)
 
+    # joins it to the main DataFrame
+    df = df.join(df_string_features_real, lsuffix='_caller', rsuffix='_other')
     relative_string_feature_list = []
 
     for index in range(n_left_nearest):
         df_string_features_l = convert_to_feat(list(df['l_offset_string' + str(index)]), 'l' + str(index) + '_')
         relative_string_feature_list += list(df_string_features_l.columns.values)
         df = df.join(df_string_features_l, lsuffix='_caller', rsuffix='_other')
 
     for index in range(n_right_nearest):
         df_string_features_r = convert_to_feat(list(df['r_offset_string' + str(index)]), 'r' + str(index) + '_')
         relative_string_feature_list += list(df_string_features_r.columns.values)
         df = df.join(df_string_features_r, lsuffix='_caller', rsuffix='_other')
 
-    df["relative_position_in_page"] = df["page_index"] / document_n_pages
+    df['relative_position_in_page'] = df['page_index'] / document_n_pages
 
-    abs_pos_feature_list = ["x0", "y0", "x1", "y1", "page_index", "area_quadrant_two"]  # , "area"]
-    relative_pos_feature_list = ["relative_position_in_page"]
+    abs_pos_feature_list = ['x0', 'y0', 'x1', 'y1', 'page_index', 'area_quadrant_two', 'area']
+    relative_pos_feature_list = [
+        'x0_relative',
+        'x1_relative',
+        'y0_relative',
+        'y1_relative',
+        'relative_position_in_page',
+    ]
 
     feature_list = (
         string_feature_column_order
         + abs_pos_feature_list
         + l_keys
         + r_keys
         + relative_string_feature_list
         + relative_pos_feature_list
-        + word_on_page_feature_name_list
     )
     if first_word:
         feature_list += first_word_features
 
-    # append the catchphrase_features to the feature_list
-    if catchphrase_list is not None:
-        for catchphrase in catchphrase_list:
-            feature_list.append('catchphrase_dist_' + catchphrase)
-
-    # joins it to the main DataFrame
-    df = df.join(df_string_features_real, lsuffix='_caller', rsuffix='_other')
-
     return df, feature_list, df_errors
 
 
 def substring_on_page(substring, annotation, page_text_list) -> bool:
     """Check if there is an occurrence of the word on the according page."""
-    if not hasattr(annotation, "page_index"):
-        logger.warning("Annotation has no page_index!")
+    if not hasattr(annotation, 'page_index'):
+        logger.warning('Annotation has no page_index!')
         return False
     elif annotation.page_index > len(page_text_list) - 1:
         logger.warning("Annotation's page_index does not match given text.")
         return False
     else:
         return substring in page_text_list[annotation.page_index]
 
 
-def generate_catchphrase_occurrence_dict(line_list, catchphrase_list, document_text) -> Dict:
-    """Generate a dict that stores on which line certain catchphrases occurrence."""
-    _dict = {catchphrase: [] for catchphrase in catchphrase_list}
-
-    for line_num, _line in enumerate(line_list):
-        line_text = document_text[_line['start_offset'] : _line['end_offset']]
-        for catchphrase in catchphrase_list:
-            if catchphrase in line_text:
-                _dict[catchphrase].append(line_num)
-
-    return _dict
-
-
-def generate_feature_dict_from_occurence_dict(occurence_dict, catchphrase_list, line_num) -> Dict:
-    """Generate the fitting catchphrase features."""
-    _dict = {catchphrase: None for catchphrase in catchphrase_list}
-
-    for catchphrase in catchphrase_list:
-        _dict[catchphrase] = next((i - line_num for i in occurence_dict[catchphrase] if i < line_num), -1)
-
-    return _dict
-
-
-def add_extractions_as_annotations(
-    extractions: pandas.DataFrame, document: Document, label: Label, label_set: LabelSet, annotation_set: AnnotationSet
-) -> None:
-    """Add the extraction of a model to the document."""
-    if not isinstance(extractions, pandas.DataFrame):
-        raise TypeError(f'Provided extraction object should be a Dataframe, got a {type(extractions)} instead')
-    if not extractions.empty:
-        # TODO: define required fields
-        required_fields = ['start_offset', 'end_offset', 'confidence']
-        if not set(required_fields).issubset(extractions.columns):
-            raise ValueError(
-                f'Extraction do not contain all required fields: {required_fields}.'
-                f' Extraction columns: {extractions.columns.to_list()}'
-            )
+class AbstractExtractionAI(BaseModel):
+    """Parent class for all Extraction AIs, to extract information from unstructured human-readable text."""
 
-        extracted_spans = extractions[required_fields].sort_values(by='confidence', ascending=False)
+    requires_text = True
+    requires_images = False
 
-        for span in extracted_spans.to_dict('records'):  # todo: are start_offset and end_offset always ints?
-            if document.bboxes is not None:
-                start = span['start_offset']
-                end = span['end_offset']
-                offset_string = document.text[start:end]
-                bbox0 = document.bboxes[start]
-                bbox1 = document.bboxes[end - 1]
-                ann_bbox = {
-                    'bottom': bbox0.page.height - bbox0.y0,
-                    'end_offset': end,
-                    'line_number': len(document.text[:start].split('\n')),
-                    'offset_string': offset_string,
-                    'offset_string_original': offset_string,
-                    'page_index': bbox0.page.index,
-                    'start_offset': start,
-                    'top': bbox0.page.height - bbox0.y1,
-                    'x0': bbox0.x0,
-                    'x1': bbox1.x1,
-                    'y0': bbox0.y0,
-                    'y1': bbox1.y1,
-                }
-                annotation = Annotation(
-                    document=document,
-                    label=label,
-                    confidence=span['confidence'],
-                    label_set=label_set,
-                    annotation_set=annotation_set,
-                    bboxes=[ann_bbox],
-                )
-            else:
-                annotation = Annotation(
-                    document=document,
-                    label=label,
-                    confidence=span['confidence'],
-                    label_set=label_set,
-                    annotation_set=annotation_set,
-                    spans=[Span(start_offset=span['start_offset'], end_offset=span['end_offset'])],
-                )
-            if annotation.spans[0].offset_string is None:
-                raise NotImplementedError(
-                    f"Extracted {annotation} does not have a correspondence in the " f"text of {document}."
-                )
-
-
-class Trainer:
-    """Base Model to extract information from unstructured human readable text."""
-
-    def __init__(self, *args, **kwargs):
+    def __init__(self, category: Category, *args, **kwargs):
         """Initialize ExtractionModel."""
         # Go through keyword arguments, and either save their values to our
         # instance, or raise an error.
+        super().__init__()
+        self.category = category
         self.clf = None
-        self.name = self.__class__.__name__
         self.label_feature_list = None  # will be set later
 
         self.df_train = None
 
         self.evaluation = None
 
-    def name_lower(self):
-        """Convert class name to machine readable name."""
-        return f'{self.name.lower().strip()}'
+    @property
+    def project(self):
+        """Get RFExtractionAI Project."""
+        if not self.category:
+            raise AttributeError(f'{self} has no Category.')
+        return self.category.project
+
+    def check_is_ready(self):
+        """
+        Check if the ExtractionAI is ready for the inference.
+
+        It is assumed that the model is ready if a Category is set, and is ready for extraction.
+
+        :raises AttributeError: When no Category is specified.
+        """
+        logger.info(f'Checking if {self} is ready for extraction.')
+        if not self.category:
+            raise AttributeError(f'{self} requires a Category.')
 
     def fit(self):
-        """Use as placeholder Function."""
+        """Use as placeholder Function because the Abstract AI does not train a classifier."""
         logger.warning(f'{self} does not train a classifier.')
         pass
 
     def evaluate(self):
         """Use as placeholder Function."""
         logger.warning(f'{self} does not evaluate results.')
         pass
 
-    def extract(self):
-        """Use as placeholder Function."""
-        logger.warning(f'{self} does not extract.')
-        pass
+    def extract(self, document: Document) -> Document:
+        """Perform preliminary extraction steps."""
+        logger.info(f'Starting extraction of {document}.')
+
+        self.check_is_ready()  # check if the model is ready for extraction
+
+        document = deepcopy(document)  # to get a Virtual Document with no Annotations
+
+        # So that the Document belongs to the Category that is saved with the ExtractionAI
+        document._category = self.project.no_category
+        document.set_category(self.category)
+
+        return document
 
     def extraction_result_to_document(self, document: Document, extraction_result: dict) -> Document:
         """Return a virtual Document annotated with AI Model output."""
         virtual_doc = deepcopy(document)
         virtual_annotation_set_id = 1  # counter for across mult. Annotation Set groups of a Label Set
 
         # define Annotation Set for the Category Label Set: todo: this is unclear from API side
         # default Annotation Set will be always added even if there are no predictions for it
         category_label_set = self.category.project.get_label_set_by_id(self.category.id_)
         virtual_default_annotation_set = AnnotationSet(
             document=virtual_doc, label_set=category_label_set, id_=virtual_annotation_set_id
         )
-
+        virtual_annotation_set_id += 1
         for label_or_label_set_name, information in extraction_result.items():
-            if isinstance(information, pandas.DataFrame) and not information.empty:
+            if isinstance(information, pandas.DataFrame):
+                if information.empty:
+                    continue
+
                 # annotations belong to the default Annotation Set
                 label = self.category.project.get_label_by_name(label_or_label_set_name)
-                add_extractions_as_annotations(
+                self.add_extractions_as_annotations(
                     document=virtual_doc,
                     extractions=information,
                     label=label,
                     label_set=category_label_set,
                     annotation_set=virtual_default_annotation_set,
                 )
-
-            elif isinstance(information, list) or isinstance(information, dict):
-                # process multi Annotation Sets that are not part of the category Label Set
+            # process multi Annotation Sets that are not part of the category Label Set
+            else:
                 label_set = self.category.project.get_label_set_by_name(label_or_label_set_name)
 
                 if not isinstance(information, list):
                     information = [information]
 
                 for entry in information:  # represents one of pot. multiple annotation-sets belonging of one LabelSet
-                    virtual_annotation_set_id += 1
-                    virtual_annotation_set = AnnotationSet(
-                        document=virtual_doc, label_set=label_set, id_=virtual_annotation_set_id
-                    )
+                    if label_set is not category_label_set:
+                        virtual_annotation_set = AnnotationSet(
+                            document=virtual_doc, label_set=label_set, id_=virtual_annotation_set_id
+                        )
+                        virtual_annotation_set_id += 1
+                    else:
+                        virtual_annotation_set = virtual_default_annotation_set
 
                     for label_name, extractions in entry.items():
                         label = self.category.project.get_label_by_name(label_name)
-                        add_extractions_as_annotations(
+                        self.add_extractions_as_annotations(
                             document=virtual_doc,
                             extractions=extractions,
                             label=label,
                             label_set=label_set,
                             annotation_set=virtual_annotation_set,
                         )
+
         return virtual_doc
 
+    @staticmethod
+    def add_extractions_as_annotations(
+        extractions: pandas.DataFrame,
+        document: Document,
+        label: Label,
+        label_set: LabelSet,
+        annotation_set: AnnotationSet,
+    ) -> None:
+        """Add the extraction of a model to the document."""
+        if not isinstance(extractions, pandas.DataFrame):
+            raise TypeError(f'Provided extraction object should be a Dataframe, got a {type(extractions)} instead')
+        if not extractions.empty:
+            # TODO: define required fields
+            required_fields = ['start_offset', 'end_offset', 'confidence']
+            if not set(required_fields).issubset(extractions.columns):
+                raise ValueError(
+                    f'Extraction do not contain all required fields: {required_fields}.'
+                    f' Extraction columns: {extractions.columns.to_list()}'
+                )
+
+            extracted_spans = extractions[required_fields].sort_values(by='confidence', ascending=False)
+
+            for span in extracted_spans.to_dict('records'):
+                try:
+                    annotation = Annotation(
+                        document=document,
+                        label=label,
+                        confidence=span['confidence'],
+                        label_set=label_set,
+                        annotation_set=annotation_set,
+                        spans=[Span(start_offset=span['start_offset'], end_offset=span['end_offset'])],
+                    )
+                    if annotation.spans[0].offset_string is None:
+                        raise NotImplementedError(
+                            f'Extracted {annotation} does not have a correspondence in the ' f'text of {document}.'
+                        )
+                except ValueError as e:
+                    if 'is a duplicate of' in str(e):
+                        # Second duplicate Span is lower confidence since we sorted spans earlier, so we can ignore it
+                        logger.warning(f'Could not add duplicated {span}: {str(e)}')
+                    else:
+                        raise e
+
     @classmethod
     def merge_horizontal(cls, res_dict: Dict, doc_text: str) -> Dict:
-        """Merge contiguous spans with same predicted label."""
-        logger.info("Horizontal merge.")
-        merged_res_dict = dict()  # stores final results
+        """Merge contiguous spans with same predicted label.
+
+        See more details at https://dev.konfuzio.com/sdk/explanations.html#horizontal-merge
+        """
+        logger.info('Horizontal merge.')
+        merged_res_dict = {}  # stores final results
         for label, items in res_dict.items():
             res_dicts = []
             buffer = []
             end = None
 
             for _, row in items.iterrows():  # iterate over the rows in the DataFrame
                 # if they are valid merges then add to buffer
@@ -1331,15 +1008,15 @@
         assert 'label_name' in buffer[0]
         label = buffer[0]['label_name']
 
         starts = buffer[0]['start_offset']
         ends = buffer[-1]['end_offset']
         text = doc_text[starts:ends]
 
-        res_dict = dict()
+        res_dict = {}
         res_dict['start_offset'] = starts
         res_dict['end_offset'] = ends
         res_dict['label_name'] = label
         res_dict['offset_string'] = text
         res_dict['confidence'] = numpy.mean([b['confidence'] for b in buffer])
         return res_dict
 
@@ -1373,25 +1050,30 @@
 
         # sanity checks
         if buffer[-1]['label_name'] != row['label_name']:
             return False
         elif buffer[-1]['confidence'] < buffer[-1]['label_threshold']:
             return False
 
-        if not all([c == ' ' for c in doc_text[buffer[-1]['end_offset'] : row['start_offset']]]):
+        # Do not merge if any character in between the two Spans
+        if not all(c == ' ' for c in doc_text[buffer[-1]['end_offset'] : row['start_offset']]):
             return False
 
         # Do not merge if the difference in the offsets is bigger than the maximum offset distance
         if row['start_offset'] - buffer[-1]['end_offset'] > max_offset_distance:
             return False
 
         # only merge if text is on same line
         if '\n' in doc_text[buffer[0]['start_offset'] : row['end_offset']]:
             return False
 
+        # Do not merge overlapping spans
+        if row['start_offset'] < buffer[-1]['end_offset']:
+            return False
+
         data_type = row['data_type']
         # always merge if not one of these data types
         if data_type not in {'Number', 'Positive Number', 'Percentage', 'Date'}:
             return True
 
         merge = None
         text = doc_text[buffer[0]['start_offset'] : row['end_offset']]
@@ -1404,117 +1086,75 @@
         elif data_type == 'Number':
             merge = normalize_to_float(text)
         elif data_type == 'Positive Number':
             merge = normalize_to_positive_float(text)
 
         return merge is not None
 
-    def save(
-        self, output_dir: str = None, include_konfuzio=True, reduce_weight=True, keep_documents=False, max_ram=None
-    ):
+    @staticmethod
+    def has_compatible_interface(other) -> bool:
         """
-        Save the label model as bz2 compressed pickle object to the release directory.
+        Validate that an instance of an Extraction AI implements the same interface as AbstractExtractionAI.
 
-        Saving is done by: getting the serialized pickle object (via cloudpickle), "optimizing" the serialized object
-        with the built-in pickletools.optimize function (see: https://docs.python.org/3/library/pickletools.html),
-        saving the optimized serialized object.
+        An Extraction AI should implement methods with the same signature as:
+        - AbstractExtractionAI.__init__
+        - AbstractExtractionAI.fit
+        - AbstractExtractionAI.extract
+        - AbstractExtractionAI.check_is_ready
 
-        We then compress the pickle file with bz2 using shutil.copyfileobject which writes in chunks to avoid loading
-        the entire pickle file in memory.
-
-        Finally, we delete the cloudpickle file and are left with the bz2 file which has a .pkl extension.
-
-        :param output_dir: Folder to save AI model in.
-        :param include_konfuzio: Boolean whether to include konfuzio_sdk package in pickle file.
-        :param reduce_weight: Remove all non-strictly necessary parameters before saving.
-        :param max_ram: Specify maximum memory usage condition to save model.
-        :raises MemoryError: When the size of the model in memory is greater than the maximum value.
-        :return: Path of the saved model file.
+        :param other: An instance of an Extraction AI to compare with.
         """
-        logger.info('Saving model')
-
-        self.check_is_ready_for_extraction()
-
-        logger.info(f'{output_dir=}')
-        logger.info(f'{include_konfuzio=}')
-        logger.info(f'{reduce_weight=}')
-        logger.info(f'{keep_documents=}')
-        logger.info(f'{max_ram=}')
-
-        # if no argument passed, get project max_ram
-        if not max_ram and self.category is not None:
-            max_ram = self.category.project.max_ram
-            logger.info(f'project {max_ram=}')
-
-        if not output_dir:
-            output_dir = self.category.project.model_folder
-            logger.info(f'new {output_dir=}')
-
-        temp_pkl_file_path = os.path.join(output_dir, f'{get_timestamp()}_{self.category.name.lower()}.cloudpickle')
-        pkl_file_path = os.path.join(output_dir, f'{get_timestamp()}_{self.category.name.lower()}.pkl')
-
-        if reduce_weight:
-            logger.info('reducing weight before save')
-            self.df_train = None
-            self.category.project.lose_weight()
-            self.tokenizer.lose_weight()
-
-        if not keep_documents:
-            logger.info('removing documents before save')
-            restore_documents = self.documents
-            restore_test_documents = self.test_documents
-            self.documents = []
-            self.test_documents = []
-
-        logger.info(f'Model size: {asizeof.asizeof(self) / 1_000_000} MB')
-
-        max_ram = normalize_memory(max_ram)
-
-        if max_ram and asizeof.asizeof(self) > max_ram:
-            raise MemoryError(f"AI model memory use ({asizeof.asizeof(self)}) exceeds maximum ({max_ram=}).")
-
-        sys.setrecursionlimit(999999)  # ?
-
-        logger.info('Getting save paths')
-
-        if include_konfuzio:
-            import konfuzio_sdk
-
-            cloudpickle.register_pickle_by_value(konfuzio_sdk)
-            # todo register all dependencies?
-
-        # make sure output dir exists
-        pathlib.Path(output_dir).mkdir(parents=True, exist_ok=True)
-
-        logger.info('Saving model with cloudpickle')
-        # first save with cloudpickle
-        with open(temp_pkl_file_path, 'wb') as f:  # see: https://stackoverflow.com/a/9519016/5344492
-            cloudpickle.dump(self, f)
-
-        logger.info('Compressing model with bz2')
-
-        # then save to bz2 in chunks
-        with open(temp_pkl_file_path, 'rb') as input_f:
-            with bz2.open(pkl_file_path, 'wb') as output_f:
-                shutil.copyfileobj(input_f, output_f)
+        try:
+            return (
+                signature(other.__init__).parameters['category'].annotation.__name__ == 'Category'
+                and signature(other.extract).parameters['document'].annotation.__name__ == 'Document'
+                and signature(other.extract).return_annotation.__name__ == 'Document'
+                and signature(other.fit)
+                and signature(other.check_is_ready)
+            )
+        except KeyError:
+            return False
+        except AttributeError:
+            return False
 
-        logger.info('Deleting cloudpickle file')
-        # then delete cloudpickle file
-        os.remove(temp_pkl_file_path)
+    @property
+    def temp_pkl_file_path(self) -> str:
+        """Generate a path for temporary pickle file."""
+        temp_pkl_file_path = os.path.join(
+            self.output_dir, f'{get_timestamp()}_{self.category.name.lower()}_{self.name_lower()}_tmp.cloudpickle'
+        )
+        return temp_pkl_file_path
 
-        size_string = f'{os.path.getsize(pkl_file_path) / 1_000_000} MB'
-        logger.info(f'Model ({size_string}) {self.name_lower()} was saved to {pkl_file_path}')
+    @property
+    def pkl_file_path(self) -> str:
+        """Generate a path for a resulting pickle file."""
+        pkl_file_path = os.path.join(
+            self.output_dir, f'{get_timestamp()}_{self.category.name.lower()}_' f'{self.name_lower()}_.pkl'
+        )
+        return pkl_file_path
 
-        # restore Documents of the Category so that we can run the evaluation later
-        self.documents = restore_documents
-        self.test_documents = restore_test_documents
-        if reduce_weight:
-            self.category.project.init_or_update_document()
+    @staticmethod
+    def load_model(pickle_path: str, max_ram: Union[None, str] = None):
+        """
+        Load the model and check if it has the interface compatible with the class.
 
-        return pkl_file_path
+        :param pickle_path: Path to the pickled model.
+        :type pickle_path: str
+        :raises FileNotFoundError: If the path is invalid.
+        :raises OSError: When the data is corrupted or invalid and cannot be loaded.
+        :raises TypeError: When the loaded pickle isn't recognized as a Konfuzio AI model.
+        :return: Extraction AI model.
+        """
+        model = super(AbstractExtractionAI, AbstractExtractionAI).load_model(pickle_path, max_ram)
+        if not AbstractExtractionAI.has_compatible_interface(model):
+            raise TypeError(
+                "Loaded model's interface is not compatible with any AIs. Please provide a model that has all the "
+                'abstract methods implemented.'
+            )
+        return model
 
 
 class GroupAnnotationSets:
     """Groups Annotation into Annotation Sets."""
 
     def __init__(self):
         """Initialize TemplateClf."""
@@ -1527,45 +1167,46 @@
         """
         Fit classifier to predict start lines of Sections.
 
         :param documents:
         :return:
         """
         # Only train template clf is there are non default templates
+        logger.info('Start training of LabelSet Classifier.')
 
         LabelSetInfo = collections.namedtuple(
             'LabelSetInfo', ['is_default', 'name', 'has_multiple_annotation_sets', 'target_names']
         )
         self.label_sets_info = [
             LabelSetInfo(
-                **dict(
-                    is_default=label_set.is_default,
-                    name=label_set.name,
-                    has_multiple_annotation_sets=label_set.has_multiple_annotation_sets,
-                    target_names=label_set.get_target_names(self.use_separate_labels),
-                )
+                **{
+                    'is_default': label_set.is_default,
+                    'name': label_set.name,
+                    'has_multiple_annotation_sets': label_set.has_multiple_annotation_sets,
+                    'target_names': label_set.get_target_names(self.use_separate_labels),
+                }
             )
             for label_set in self.category.label_sets
         ]
 
         if not [lset for lset in self.category.label_sets if not lset.is_default]:
             # todo see https://gitlab.com/konfuzio/objectives/-/issues/2247
             # todo check for NO_LABEL_SET if we should keep it
-            return
+            return None
         logger.info('Start training of Multi-class Label Set Classifier.')
         # ignores the section count as it actually worsens results
         # todo check if no category labels should be ignored
         self.template_feature_list = list(self.clf.classes_)  # list of label classifier targets
         # logger.warning("template_feature_list:", self.template_feature_list)
         n_nearest = self.n_nearest_template  # if hasattr(self, 'n_nearest_template') else 0
 
         # Pretty long feature generation
         df_train_label = self.df_train
 
-        df_train_label_list = [(document_id, df_doc) for document_id, df_doc in df_train_label.groupby('document_id')]
+        df_train_label_list = list(df_train_label.groupby('document_id'))
 
         df_train_template_list = []
         df_train_ground_truth_list = []
         for document_id, df_doc in df_train_label_list:
             document = self.category.project.get_document_by_id(document_id)
             df_train_template_list.append(self.convert_label_features_to_template_features(df_doc, document.text))
             df_train_ground_truth_list.append(self.build_document_template_feature(document))
@@ -1678,15 +1319,17 @@
 
     def build_document_template_feature(self, document) -> pandas.DataFrame():
         """Build document feature for template classifier given ground truth."""
         df = pandas.DataFrame()
         char_count = 0
 
         document_annotations = [
-            annotation for annotation_set in document.annotation_sets() for annotation in annotation_set.annotations()
+            annotation
+            for annotation_set in document.annotation_sets()
+            for annotation in annotation_set.annotations(use_correct=True)
         ]
 
         # Loop over lines
         for i, line in enumerate(document.text.replace('\f', '\n').split('\n')):
             matched_annotation_set = None
             new_char_count = char_count + len(line)
             assert line == document.text[char_count:new_char_count]
@@ -1695,15 +1338,15 @@
                 if annotation_set.start_offset and char_count <= annotation_set.start_offset < new_char_count:
                     matched_annotation_set: AnnotationSet = annotation_set
                     break
 
             line_annotations = [
                 x for x in document_annotations if char_count <= x.spans[0].start_offset < new_char_count
             ]
-            annotations_dict = dict((x.label.name, True) for x in line_annotations)
+            annotations_dict = {x.label.name: True for x in line_annotations}
             counter_dict = dict(
                 collections.Counter(annotation.annotation_set.label_set.name for annotation in line_annotations)
             )
             y = matched_annotation_set.label_set.name if matched_annotation_set else 'No'
             tmp_df = pandas.DataFrame(
                 [{'line': i, 'y': y, 'document': document.id_, **annotations_dict, **counter_dict}]
             )
@@ -1716,55 +1359,69 @@
         """
         Calculate features for a document given the extraction results.
 
         :param text:
         :param df:
         :return:
         """
-        if self.category is None:
+        if self.category.name == 'NO_CATEGORY':
             raise AttributeError(f'{self} does not provide a Category.')
 
         global_df = pandas.DataFrame()
         char_count = 0
         # Using OptimalThreshold is a bad idea as it might defer between training (actual treshold from the label)
         # and runtime (default treshold.
 
         # df = df[df['confidence'] >= 0.1]  # df['OptimalThreshold']]
-        for i, line in enumerate(text.replace('\f', '\n').split('\n')):
+        lines = text.replace('\f', '\n').split('\n')
+        for i, line in enumerate(lines):
             new_char_count = char_count + len(line)
             assert line == text[char_count:new_char_count]
             line_df = df[(char_count <= df['start_offset']) & (df['end_offset'] <= new_char_count)]
             spans = [row for index, row in line_df.iterrows()]
-            spans_dict = dict((x['result_name'], True) for x in spans)
-            counter_dict = {}  # why?
+            spans_dict = {x['result_name']: True for x in spans}
+            # counter_dict = {}  # why?
             # annotations_accuracy_dict = defaultdict(lambda: 0)
             # for annotation in annotations:
             # annotations_accuracy_dict[f'{annotation["label"]}_accuracy'] += annotation['confidence']
             # try:
 
             #     label = next(x for x in self.category.project.labels if x.name == annotation['result_name'])
             # except StopIteration:
             #     continue
             # for label_set in self.label_sets:
             #     if label in label_set.labels:
             #         if label_set.name in counter_dict.keys():
             #             counter_dict[label_set.name] += 1
             #         else:
             #             counter_dict[label_set.name] = 1
-            tmp_df = pandas.DataFrame([{**spans_dict, **counter_dict}])
+            tmp_df = pandas.DataFrame([spans_dict])  # ([{**spans_dict, **counter_dict}])
             global_df = pandas.concat([global_df, tmp_df], ignore_index=True)
             char_count = new_char_count + 1
-        global_df['text'] = text.replace('\f', '\n').split('\n')
+        global_df['text'] = lines
         return global_df.fillna(0)
 
+    @classmethod
+    def dict_to_dataframe(cls, res_dict):
+        """Convert a Dict to Dataframe add label as column."""
+        df = pandas.DataFrame()
+        for name in res_dict.keys():
+            label_df = res_dict[name]
+            label_df['result_name'] = name
+            df = df.append(label_df, sort=True)
+        return df
+
     def extract_template_with_clf(self, text, res_dict):
-        """Run template classifier to calculate sections."""
-        logger.info('Extract sections.')
+        """Run LabelSet classifier to find AnnotationSets."""
+        logger.info('Extract AnnotationSets.')
+        if not res_dict:
+            logger.warning('res_dict is empty')
+            return res_dict
         n_nearest = self.n_nearest_template if hasattr(self, 'n_nearest_template') else 0
-        feature_df = self.build_document_template_feature_X(text, dict_to_dataframe(res_dict)).filter(
+        feature_df = self.build_document_template_feature_X(text, self.dict_to_dataframe(res_dict)).filter(
             self.template_feature_list, axis=1
         )
         feature_df = feature_df.reindex(columns=self.template_feature_list).fillna(0)
         feature_df = self.generate_relative_line_features(n_nearest, feature_df)
 
         res_series = self.label_set_clf.predict(feature_df)
         res_templates = pandas.DataFrame(res_series)
@@ -1787,15 +1444,14 @@
                     i = 0
                     # for each line of a certain section label
                     for line_number, section_name in detected_sections.iterrows():
                         section_dict = {}
                         # we try to find the labels that match that section
                         for target_label_name in label_set.target_names:
                             if target_label_name in res_dict.keys():
-
                                 label_df = res_dict[target_label_name]
                                 if label_df.empty:
                                     continue
                                 # todo: the next line is memory heavy
                                 #  https://gitlab.com/konfuzio/objectives/-/issues/9342
                                 label_df['line'] = (
                                     label_df['start_offset'].apply(lambda x: text_replaced[: int(x)]).str.count('\n')
@@ -1836,18 +1492,18 @@
                     new_res_dict[target_label_name] = res_dict[target_label_name]
                     del res_dict[target_label_name]  # ?
             continue
 
         return new_res_dict
 
 
-class RFExtractionAI(Trainer, GroupAnnotationSets):
+class RFExtractionAI(AbstractExtractionAI, GroupAnnotationSets):
     """Encode visual and textual features to extract text regions.
 
-    Fit a extraction pipeline to extract linked Annotations.
+    Fit an extraction pipeline to extract linked Annotations.
 
     Both Label and Label Set classifiers are using a RandomForestClassifier from scikit-learn to run in a low memory and
     single CPU environment. A random forest classifier is a group of decision trees classifiers, see:
     https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html
 
     The parameters of this class allow to select the Tokenizer, to configure the Label and Label Set classifiers and to
     select the type of features used by the Label and Label Set classifiers.
@@ -1887,114 +1543,125 @@
         self,
         n_nearest: int = 2,
         first_word: bool = True,
         n_estimators: int = 100,
         max_depth: int = 100,
         no_label_limit: Union[int, float, None] = None,
         n_nearest_across_lines: bool = False,
-        use_separate_labels: bool = False,
+        use_separate_labels: bool = True,
         category: Category = None,
         tokenizer=None,
         *args,
         **kwargs,
     ):
         """RFExtractionAI."""
-        logger.info("Initializing RFExtractionAI.")
-        super().__init__(*args, **kwargs)
+        logger.info('Initializing RFExtractionAI.')
+        super().__init__(category, *args, **kwargs)
         GroupAnnotationSets.__init__(self)
 
         self.label_feature_list = None
 
-        logger.info("RFExtractionAI settings:")
-        logger.info(f"{use_separate_labels=}")
-        logger.info(f"{category=}")
-        logger.info(f"{n_nearest=}")
-        logger.info(f"{first_word=}")
-        logger.info(f"{max_depth=}")
-        logger.info(f"{n_estimators=}")
-        logger.info(f"{no_label_limit=}")
-        logger.info(f"{n_nearest_across_lines=}")
+        logger.info('RFExtractionAI settings:')
+        logger.info(f'{use_separate_labels=}')
+        logger.info(f'{category=}')
+        logger.info(f'{n_nearest=}')
+        logger.info(f'{first_word=}')
+        logger.info(f'{max_depth=}')
+        logger.info(f'{n_estimators=}')
+        logger.info(f'{no_label_limit=}')
+        logger.info(f'{n_nearest_across_lines=}')
 
         self.use_separate_labels = use_separate_labels
-        self.category = category
         self.n_nearest = n_nearest
         self.first_word = first_word
         self.max_depth = max_depth
         self.n_estimators = n_estimators
         self.no_label_limit = no_label_limit
         self.n_nearest_across_lines = n_nearest_across_lines
 
-        self.substring_features = kwargs.get('substring_features', None)
-        self.catchphrase_features = kwargs.get('catchphrase_features', None)
-
         self.tokenizer = tokenizer
-        logger.info(f"{tokenizer=}")
+        logger.info(f'{tokenizer=}')
 
         self.clf = None
 
         self.no_label_set_name = None
         self.no_label_name = None
 
+        self.output_dir = None
+
+    @property
+    def requires_segmentation(self) -> bool:
+        """Return True if the Extraction AI requires detectron segmentation results to process Documents."""
+        if (
+            sdk_isinstance(self.tokenizer, ParagraphTokenizer) or sdk_isinstance(self.tokenizer, SentenceTokenizer)
+        ) and self.tokenizer.mode == 'detectron':
+            return True
+        elif self.tokenizer is None:
+            logger.warning('Tokenizer is not set. Assuming no segmentation results is required.')
+        return False
+
     def features(self, document: Document):
         """Calculate features using the best working default values that can be overwritten with self values."""
-        logger.info(f"Starting {document} feature calculation.")
+        logger.info(f'Starting {document} feature calculation.')
         if self.no_label_name is None or self.no_label_set_name is None:
             self.no_label_name = document.project.no_label.name_clean
             self.no_label_set_name = document.project.no_label_set.name_clean
         df, _feature_list, _temp_df_raw_errors = process_document_data(
             document=document,
             spans=document.spans(use_correct=False),
             n_nearest=self.n_nearest,
             first_word=self.first_word,
-            tokenize_fn=self.tokenizer.tokenize,  # todo: we are tokenizing the document multiple times
-            catchphrase_list=self.catchphrase_features,
-            substring_features=self.substring_features,
+            # tokenize_fn=self.tokenizer.tokenize,  # todo: we are tokenizing the document multiple times
+            # catchphrase_list=self.catchphrase_features,
+            # substring_features=self.substring_features,
             n_nearest_across_lines=self.n_nearest_across_lines,
         )
         if self.use_separate_labels:
             df['target'] = df['label_set_name'] + '__' + df['label_name']
         else:
             df['target'] = df['label_name']
         return df, _feature_list, _temp_df_raw_errors
 
-    def check_is_ready_for_extraction(self):
-        """Check if tokenizer is set and the classifiers set and trained."""
+    def check_is_ready(self):
+        """
+        Check if the ExtractionAI is ready for the inference.
+
+        It is assumed that the model is ready if a Tokenizer and a Category were set, Classifiers were set and trained.
+
+        :raises AttributeError: When no Tokenizer is specified.
+        :raises AttributeError: When no Category is specified.
+        :raises AttributeError: When no Label Classifier has been provided.
+        """
+        super().check_is_ready()
         if self.tokenizer is None:
             raise AttributeError(f'{self} missing Tokenizer.')
 
-        if not self.category:
-            raise AttributeError(f'{self} requires a Category.')
-
         if self.clf is None:
             raise AttributeError(f'{self} does not provide a Label Classifier. Please add it.')
         else:
             check_is_fitted(self.clf)
 
         if self.label_set_clf is None:
-            logger.warning('{self} does not provide a LabelSet Classfier.')
+            logger.warning(f'{self} does not provide a LabelSet Classfier.')
 
     def extract(self, document: Document) -> Document:
         """
         Infer information from a given Document.
 
         :param document: Document object
         :return: Document with predicted labels
 
         :raises:
          AttributeError: When missing a Tokenizer
          NotFittedError: When CLF is not fitted
 
         """
-        logger.info(f"Starting extraction of {document}.")
+        # 1. create Virtual inference Document with Category set to the Category of the ExtractionAI
+        inference_document = super().extract(document)
 
-        self.check_is_ready_for_extraction()
-
-        # Main Logic -------------------------
-        # 1. start inference with new document
-        inference_document = deepcopy(document)
         # 2. tokenize
         self.tokenizer.tokenize(inference_document)
         if not inference_document.spans():
             logger.error(f'{self.tokenizer} does not provide Spans for {document}')
             return inference_document
 
         # 3. preprocessing
@@ -2019,72 +1686,186 @@
         if self.no_label_set_name in results.columns:
             results = results.drop([self.no_label_set_name], axis=1)
 
         separate_no_label_target = self.no_label_set_name + '__' + self.no_label_name
         if separate_no_label_target in results.columns:
             results = results.drop([separate_no_label_target], axis=1)
 
-        df['result_name'] = results.idxmax(axis=1)
-        df['confidence'] = results.max(axis=1)
+        res_dict = {}
+        no_label_res_dict = {}
 
         # Main Logic -------------------------
+        if not results.empty:
+            df['result_name'] = results.idxmax(axis=1)
+            df['confidence'] = results.max(axis=1)
 
-        # Do column renaming to be compatible with text-annotation
-        # todo: how can multilines be created via SDK
-        # todo: why do we need to adjust the woring for Server?
-        # todo: which other attributes could be send in the extraction method?
-
-        # Convert DataFrame to Dict with labels as keys and label dataframes as value.
-        res_dict = {}
-        for result_name in set(df['result_name']):
-            result_df = df[(df['result_name'] == result_name) & (df['confidence'] >= df['label_threshold'])].copy()
+            # Convert DataFrame to Dict with labels as keys and label dataframes as value.
+            for result_name in set(df['result_name']):
+                result_df = df[(df['result_name'] == result_name) & (df['confidence'] >= df['label_threshold'])].copy()
 
-            if not result_df.empty:
-                res_dict[result_name] = result_df
+                if not result_df.empty:
+                    res_dict[result_name] = result_df
 
-        no_label_res_dict = {}
-        for result_name in set(df['result_name']):
-            result_df = df[(df['result_name'] == result_name) & (df['confidence'] < df['label_threshold'])].copy()
+            for result_name in set(df['result_name']):
+                result_df = df[(df['result_name'] == result_name) & (df['confidence'] < df['label_threshold'])].copy()
 
-            if not result_df.empty:
-                no_label_res_dict[result_name] = result_df
+                if not result_df.empty:
+                    no_label_res_dict[result_name] = result_df
 
         # Filter results that are bellow the extract threshold
         # (helpful to reduce the size in case of many predictions/ big documents)
 
         # if hasattr(self, 'extract_threshold') and self.extract_threshold is not None:
         #     logger.info('Filtering res_dict')
         #     for result_name, value in res_dict.items():
         #         if isinstance(value, pandas.DataFrame):
         #             res_dict[result_name] = value[value['confidence'] > self.extract_threshold]
 
         res_dict = self.remove_empty_dataframes_from_extraction(res_dict)
         no_label_res_dict = self.remove_empty_dataframes_from_extraction(no_label_res_dict)
 
         # res_dict = self.filter_low_confidence_extractions(res_dict)
-
-        res_dict = self.merge_horizontal(res_dict, inference_document.text)
+        if not sdk_isinstance(self.tokenizer, ParagraphTokenizer) and not sdk_isinstance(
+            self.tokenizer, SentenceTokenizer
+        ):
+            # We assume that Paragraph or Sentence tokenizers have correctly tokenized the Document
+            res_dict = self.merge_horizontal(res_dict, inference_document.text)
 
         # Try to calculate sections based on template classifier.
-        if self.label_set_clf is not None:  # todo smarter handling of multiple clf
+        if self.label_set_clf is not None and res_dict:  # todo smarter handling of multiple clf
             res_dict = self.extract_template_with_clf(inference_document.text, res_dict)
-            res_dict[self.no_label_set_name] = no_label_res_dict
+        res_dict[self.no_label_set_name] = no_label_res_dict
 
         if self.use_separate_labels:
             res_dict = self.separate_labels(res_dict)
 
         virtual_doc = self.extraction_result_to_document(inference_document, res_dict)
 
         self.tokenizer.found_spans(virtual_doc)
 
-        # join document Spans into multi-line Annotation
-        virtual_doc.merge_vertical()
+        if sdk_isinstance(self.tokenizer, ParagraphTokenizer) or sdk_isinstance(self.tokenizer, SentenceTokenizer):
+            # When using the Paragraph or Sentence tokenizer, we restore the multi-line Annotations they created.
+            virtual_doc = self.merge_vertical_like(virtual_doc, inference_document)
+        else:
+            # join document Spans into multi-line Annotation
+            virtual_doc = self.merge_vertical(virtual_doc)
 
         return virtual_doc
 
+    def merge_vertical(self, document: Document, only_multiline_labels=True):
+        """
+        Merge Annotations with the same Label.
+
+        See more details at https://dev.konfuzio.com/sdk/explanations.html#vertical-merge
+
+        :param document: Document whose Annotations should be merged vertically
+        :param only_multiline_labels: Only merge if a multiline Label Annotation is in the Category Training set
+        """
+        logger.info('Vertical merging Annotations.')
+        if not self.category:
+            raise AttributeError(f'{self} merge_vertical requires a Category.')
+        labels_dict = {}
+        for label in self.category.labels:
+            if not only_multiline_labels or label.has_multiline_annotations():
+                labels_dict[label.name] = []
+
+        for annotation in document.annotations(use_correct=False, ignore_below_threshold=True):
+            if annotation.label.name in labels_dict:
+                labels_dict[annotation.label.name].append(annotation)
+
+        for label_id in labels_dict:
+            buffer = []
+            for annotation in labels_dict[label_id]:
+                for span in annotation.spans:
+                    # remove all spans in buffer more than 1 line apart
+                    while buffer and span.line_index > buffer[0].line_index + 1:
+                        buffer.pop(0)
+
+                    if buffer and buffer[-1].page != span.page:
+                        buffer = [span]
+                        continue
+
+                    if len(annotation.spans) > 1:
+                        buffer.append(span)
+                        continue
+
+                    for candidate in buffer:
+                        # only looking for elements in line above
+                        if candidate.line_index == span.line_index:
+                            break
+
+                        # Merge if there is overlap in the horizontal direction or if only separated by a line break
+                        # AND if the AnnotationSets are the same or if the Annotation is alone in its AnnotationSet
+                        if (
+                            (not (span.bbox().x0 > candidate.bbox().x1 or span.bbox().x1 < candidate.bbox().x0))
+                            or document.text[candidate.end_offset : span.start_offset]
+                            .replace(' ', '')
+                            .replace('\n', '')
+                            == ''
+                        ) and (
+                            span.annotation.annotation_set is candidate.annotation.annotation_set
+                            or len(
+                                span.annotation.annotation_set.annotations(
+                                    use_correct=False, ignore_below_threshold=True
+                                )
+                            )
+                            == 1
+                        ):
+                            span.annotation.delete(delete_online=False)
+                            span.annotation = None
+                            candidate.annotation.add_span(span)
+                            buffer.remove(candidate)
+                    buffer.append(span)
+        return document
+
+    def merge_vertical_like(self, document: Document, template_document: Document):
+        """
+        Merge Annotations the same way as in another copy of the same Document.
+
+        All single-Span Annotations in the current Document (self) are matched with corresponding multi-line
+        Spans in the given Document and are merged in the same way.
+        The Label of the new multi-line Annotations is taken to be the most common Label among the original
+        single-line Annotations that are being merged.
+
+        :param document: Document with multi-line Annotations
+        """
+        logger.info(f'Vertical merging Annotations like {template_document}.')
+        assert (
+            document.text == template_document.text
+        ), f'{self} and {template_document} need to have the same ocr text.'
+        span_to_annotation = {
+            (span.start_offset, span.end_offset): hash(span.annotation)
+            for span in template_document.spans(use_correct=False)
+        }
+        ann_to_anns = collections.defaultdict(list)
+        for annotation in document.annotations(use_correct=False):
+            assert (
+                len(annotation.spans) == 1
+            ), f'Cannot use merge_verical_like in {document} with multi-span {annotation}.'
+            span_offset_key = (annotation.spans[0].start_offset, annotation.spans[0].end_offset)
+            if span_offset_key in span_to_annotation:
+                ann_to_anns[span_to_annotation[span_offset_key]].append(annotation)
+        for _, self_annotations in ann_to_anns.items():
+            if len(self_annotations) == 1:
+                continue
+            else:
+                self_annotations = sorted(self_annotations)
+                keep_annotation = self_annotations[0]
+                annotation_labels = [keep_annotation.label]
+                for to_merge_annotation in self_annotations[1:]:
+                    annotation_labels.append(to_merge_annotation.label)
+                    span = to_merge_annotation.spans[0]
+                    to_merge_annotation.delete(delete_online=False)
+                    span.annotation = None
+                    keep_annotation.add_span(span)
+                most_common_label = collections.Counter(annotation_labels).most_common(1)[0][0]
+                keep_annotation.label = most_common_label
+
+        return document
+
     def separate_labels(self, res_dict: 'Dict') -> 'Dict':
         """
         Undo the renaming of the labels.
 
         In this way we have the output of the extraction in the correct format.
         """
         new_res = {}
@@ -2213,74 +1994,68 @@
 
         :param df: Dataframe with extraction results
         :returns: Filtered dataframe
         """
         filtered = df[df['confidence'] >= df['label_threshold']]
         return filtered
 
-    def lose_weight(self):
-        """Lose weight before pickling."""
-        super().lose_weight()
-
-        # remove documents
-        self.documents = None
-        self.test_documents = None
-
     def label_train_document(self, virtual_document: Document, original_document: Document):
-        """Assign labels to Annotations in newly tokenized virtual training document."""
+        """Assign Labels to Annotations in newly tokenized virtual training Document."""
         doc_spans = original_document.spans(use_correct=True)
         s_i = 0
         for span in virtual_document.spans():
             while s_i < len(doc_spans) and span.start_offset > doc_spans[s_i].end_offset:
                 s_i += 1
             if s_i >= len(doc_spans):
                 break
             if span.end_offset < doc_spans[s_i].start_offset:
                 continue
 
             r = range(doc_spans[s_i].start_offset, doc_spans[s_i].end_offset + 1)
             if span.start_offset in r and span.end_offset in r:
                 span.annotation.label = doc_spans[s_i].annotation.label
-                span.annotation.label_set = doc_spans[s_i].annotation.label_set
                 span.annotation.annotation_set = doc_spans[s_i].annotation.annotation_set
 
     def feature_function(
         self,
         documents: List[Document],
-        no_label_limit=None,
-        retokenize=True,
-        require_revised_annotations=False,
+        no_label_limit: Union[None, int, float] = None,
+        retokenize: Optional[bool] = None,
+        require_revised_annotations: bool = False,
     ) -> Tuple[List[pandas.DataFrame], list]:
         """Calculate features per Span of Annotations.
 
-        :param documents: List of documents to extract features from.
-        :param no_label_limit: Int or Float to limit number of new annotations to create during tokenization.
-        :param retokenize: Bool for whether to recreate annotations from scratch or use already existing annotations.
+        :param documents: List of Documents to extract features from.
+        :param no_label_limit: Int or Float to limit number of new Annotations to create during tokenization.
+        :param retokenize: Bool for whether to recreate Annotations from scratch or use already existing Annotations.
+        :param require_revised_annotations: Only allow calculation of features if no unrevised Annotation present.
         :return: Dataframe of features and list of feature names.
         """
-        logger.info(f'Start generating features for {len(documents)} documents.')
+        logger.info(f'Start generating features for {len(documents)} Documents.')
         logger.info(f'{no_label_limit=}')
         logger.info(f'{retokenize=}')
         logger.info(f'{require_revised_annotations=}')
 
+        if retokenize is None:
+            if sdk_isinstance(self.tokenizer, ListTokenizer):
+                retokenize = False
+            else:
+                retokenize = True
+            logger.info(f'retokenize option set to {retokenize} with Tokenizer {self.tokenizer}')
+
         df_real_list = []
         df_raw_errors_list = []
         feature_list = []
 
-        # todo make regex Tokenizer optional as those will be saved by the Server
-        # if not hasattr(self, 'regexes'):  # Can be removed for models after 09.10.2020
-        #    self.regexes = [regex for label_model in self.labels for regex in label_model.label.regex()]
+        for label in self.category.labels:
+            label.has_multiline_annotations(categories=[self.category])
 
         for document in documents:
-            # todo check for tokenizer: self.tokenizer.tokenize(document)  # todo: do we need it?
-            # todo check removed  if x.x0 and x.y0
-            # todo: use NO_LABEL for any Annotation that has no Label, instead of keeping Label = None
             for span in document.spans(use_correct=False):
                 if span.annotation.id_:
-                    # Annotation
                     # we use "<" below because we don't want to have unconfirmed annotations in the training set,
                     # and the ones below threshold wouldn't be considered anyway
                     if (
                         span.annotation.is_correct
                         or (not span.annotation.is_correct and span.annotation.revised)
                         or (
                             span.annotation.confidence
@@ -2289,62 +2064,71 @@
                         )
                     ):
                         pass
                     else:
                         if require_revised_annotations:
                             raise ValueError(
                                 f"{span.annotation} is unrevised in this dataset and can't be used for training!"
-                                f"Please revise it manually by either confirming it, rejecting it, or modifying it."
+                                f'Please revise it manually by either confirming it, rejecting it, or modifying it.'
                             )
                         else:
                             logger.error(
-                                f"{span.annotation} is unrevised in this dataset and may impact model "
-                                f"performance! Please revise it manually by either confirming it, rejecting "
-                                f"it, or modifying it."
+                                f'{span.annotation} is unrevised in this dataset and may impact model '
+                                f'performance! Please revise it manually by either confirming it, rejecting '
+                                f'it, or modifying it.'
                             )
 
+            virtual_document = deepcopy(document)
             if retokenize:
-                virt_document = deepcopy(document)
-                self.tokenizer.tokenize(virt_document)
-                self.label_train_document(virt_document, document)
-                document = virt_document
+                # Retokenize the Document from scratch and add correct Label the new matching Annotations.
+                # This may not include exact matches for the training data, but will include all Annotations actually
+                # found by the Tokenizer
+                self.tokenizer.tokenize(virtual_document)
+                self.label_train_document(virtual_document, document)
             else:
-                virt_document = deepcopy(document)
-                for ann in document.annotations():
+                # Copy existing Annotations in training Document and then tokenize and add NO_LABEL Annotations to
+                # the virtual Document. This will include exact matches for the training data, but these might not
+                # actually be exactly found by the Tokenizer during inference.
+                for annotation in document.annotations():
                     new_spans = []
-                    for span in ann.spans:
+                    for span in annotation.spans:
                         new_span = Span(start_offset=span.start_offset, end_offset=span.end_offset)
                         new_spans.append(new_span)
 
-                    new_ann = Annotation(
-                        document=virt_document,
-                        annotation_set=virt_document.no_label_annotation_set,
-                        label=ann.label,
-                        label_set=virt_document.project.no_label_set,
+                    # Retrieve copy of AnnotationSet from virtual Document or create new one
+                    try:
+                        annotation_set = virtual_document.get_annotation_set_by_id(annotation.annotation_set.id_)
+                    except IndexError:
+                        annotation_set = AnnotationSet(
+                            document=virtual_document, label_set=annotation.label_set, id_=annotation.annotation_set.id_
+                        )
+                    _ = Annotation(
+                        document=virtual_document,
+                        annotation_set=annotation_set,
+                        label=annotation.label,
                         category=self.category,
                         spans=new_spans,
                     )
-                    new_ann.label_set = ann.label_set
-                    new_ann.annotation_set = ann.annotation_set
 
-                self.tokenizer.tokenize(virt_document)
-                document = virt_document
+                self.tokenizer.tokenize(virtual_document)
 
-            no_label_annotations = document.annotations(use_correct=False, label=document.project.no_label)
-            label_annotations = [x for x in document.annotations(use_correct=False) if x.label.id_ is not None]
+            no_label_annotations = virtual_document.annotations(
+                use_correct=False, label=virtual_document.project.no_label
+            )
+            label_annotations = [x for x in virtual_document.annotations(use_correct=False) if x.label.id_]
 
             # We calculate features of documents as long as they have IDs, even if they are offline.
             # The assumption is that if they have an ID, then the data came either from the API or from the DB.
-            if document.id_ is None and document.copy_of_id is None:
+            if virtual_document.id_ is None and virtual_document.copy_of_id is None:
                 # inference time todo reduce shuffled complexity
                 assert (
                     not label_annotations
                 ), "Documents that don't come from the server have no human revised Annotations."
                 raise NotImplementedError(
-                    f'{document} does not come from the server, please use process_document_data function.'
+                    f'{virtual_document} does not come from the server, please use process_document_data function.'
                 )
             else:
                 # training time: todo reduce shuffled complexity
                 if isinstance(no_label_limit, int):
                     n_no_labels = no_label_limit
                 elif isinstance(no_label_limit, float):
                     n_no_labels = int(len(label_annotations) * no_label_limit)
@@ -2352,91 +2136,101 @@
                     assert no_label_limit is None
 
                 if no_label_limit is not None:
                     no_label_annotations = self.get_best_no_label_annotations(
                         n_no_labels, label_annotations, no_label_annotations
                     )
                     logger.info(
-                        f'Document {document} NO_LABEL annotations has been reduced to {len(no_label_annotations)}'
+                        f'Document {virtual_document} NO_LABEL annotations reduced to {len(no_label_annotations)}'
                     )
 
-            logger.info(f'Document {document} has {len(label_annotations)} labeled annotations')
-            logger.info(f'Document {document} has {len(no_label_annotations)} NO_LABEL annotations')
+            logger.info(f'Document {virtual_document} has {len(label_annotations)} labeled annotations')
+            logger.info(f'Document {virtual_document} has {len(no_label_annotations)} NO_LABEL annotations')
 
             # todo: check if eq method of Annotation prevents duplicates
             # annotations = self._filter_annotations_for_duplicates(label_annotations + no_label_annotations)
 
             t0 = time.monotonic()
 
-            temp_df_real, _feature_list, temp_df_raw_errors = self.features(document)
+            temp_df_real, _feature_list, temp_df_raw_errors = self.features(virtual_document)
+
+            logger.info(f'Document {virtual_document} processed in {time.monotonic() - t0:.1f} seconds.')
 
-            logger.info(f'Document {document} processed in {time.monotonic() - t0:.1f} seconds.')
+            virtual_document.delete(delete_online=False)  # reduce memory from virtual doc
 
             feature_list += _feature_list
             df_real_list.append(temp_df_real)
             df_raw_errors_list.append(temp_df_raw_errors)
 
         feature_list = list(dict.fromkeys(feature_list))  # remove duplicates while maintaining order
 
         if df_real_list:
             df_real_list = pandas.concat(df_real_list).reset_index(drop=True)
         else:
-            raise NotImplementedError  # = pandas.DataFrame()
+            raise NotImplementedError
+
+        logger.info(f'Size of feature dict {memory_size_of(df_real_list)/1000} KB.')
 
         return df_real_list, feature_list
 
     def fit(self) -> RandomForestClassifier:
         """Given training data and the feature list this function returns the trained regression model."""
         logger.info('Start training of Multi-class Label Classifier.')
 
         # balanced gives every label the same weight so that the sample_number doesn't effect the results
         self.clf = RandomForestClassifier(
-            class_weight="balanced", n_estimators=self.n_estimators, max_depth=self.max_depth, random_state=420
+            class_weight='balanced', n_estimators=self.n_estimators, max_depth=self.max_depth, random_state=420
         )
 
         self.clf.fit(self.df_train[self.label_feature_list], self.df_train['target'])
 
+        logger.info(f'Size of Label classifier: {memory_size_of(self.clf)/1000} KB.')
+
         self.fit_label_set_clf()
 
+        logger.info(f'Size of LabelSet classifier: {memory_size_of(self.label_set_clf)/1000} KB.')
+
         return self.clf
 
-    def evaluate_full(self, strict: bool = True, use_training_docs: bool = False) -> Evaluation:
+    def evaluate_full(
+        self, strict: bool = True, use_training_docs: bool = False, use_view_annotations: bool = True
+    ) -> ExtractionEvaluation:
         """
         Evaluate the full pipeline on the pipeline's Test Documents.
 
-        :param strict: List of documents to extract features from.
+        :param strict: Evaluate on a Character exact level without any postprocessing.
         :param use_training_docs: Bool for whether to evaluate on the training documents instead of testing documents.
         :return: Evaluation object.
         """
         eval_list = []
         if not use_training_docs:
             eval_docs = self.test_documents
         else:
             eval_docs = self.documents
 
         for document in eval_docs:
             predicted_doc = self.extract(document=document)
             eval_list.append((document, predicted_doc))
 
-        self.full_evaluation = Evaluation(eval_list, strict=strict)
+        full_evaluation = ExtractionEvaluation(eval_list, strict=strict, use_view_annotations=use_view_annotations)
 
-        return self.full_evaluation
+        return full_evaluation
 
-    def evaluate_tokenizer(self, use_training_docs: bool = False) -> Evaluation:
+    def evaluate_tokenizer(self, use_training_docs: bool = False) -> ExtractionEvaluation:
         """Evaluate the tokenizer."""
         if not use_training_docs:
             eval_docs = self.test_documents
         else:
             eval_docs = self.documents
 
         evaluation = self.tokenizer.evaluate_dataset(eval_docs)
 
         return evaluation
 
-    def evaluate_clf(self, use_training_docs: bool = False) -> Evaluation:
+    def evaluate_clf(self, use_training_docs: bool = False) -> ExtractionEvaluation:
         """Evaluate the Label classifier."""
         eval_list = []
         if not use_training_docs:
             eval_docs = self.test_documents
         else:
             eval_docs = self.documents
 
@@ -2458,19 +2252,19 @@
                     spans=new_spans,
                 )
 
             feats_df, _, _ = self.features(virtual_doc)
             predicted_doc = self.extract_from_df(feats_df, virtual_doc)
             eval_list.append((document, predicted_doc))
 
-        clf_evaluation = Evaluation(eval_list)
+        clf_evaluation = ExtractionEvaluation(eval_list, use_view_annotations=False)
 
         return clf_evaluation
 
-    def evaluate_label_set_clf(self, use_training_docs: bool = False) -> Evaluation:
+    def evaluate_label_set_clf(self, use_training_docs: bool = False) -> ExtractionEvaluation:
         """Evaluate the LabelSet classifier."""
         if self.label_set_clf is None:
             raise AttributeError(f'{self} does not provide a LabelSet Classifier.')
         else:
             check_is_fitted(self.label_set_clf)
 
         eval_list = []
@@ -2497,10 +2291,15 @@
             if self.use_separate_labels:
                 res_dict = self.separate_labels(res_dict)
 
             predicted_doc = self.extraction_result_to_document(document, res_dict)
 
             eval_list.append((document, predicted_doc))
 
-        label_set_clf_evaluation = Evaluation(eval_list)
+        label_set_clf_evaluation = ExtractionEvaluation(eval_list, use_view_annotations=False)
 
         return label_set_clf_evaluation
+
+    def reduce_model_weight(self):
+        """Remove all non-strictly necessary parameters before saving."""
+        super().reduce_model_weight()
+        self.df_train = None
```

### Comparing `konfuzio_sdk-0.2.9.dev20230104175944/konfuzio_sdk/utils.py` & `konfuzio_sdk-0.3.0/konfuzio_sdk/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,59 +1,87 @@
 """Utils for the konfuzio sdk package."""
 import datetime
-import hashlib
 import itertools
 import logging
 import operator
 import os
-import regex as re
 import unicodedata
+import uuid
 import zipfile
 from contextlib import contextmanager
 from io import BytesIO
-from typing import Union, List, Tuple, Dict, Optional
+from typing import TYPE_CHECKING, Dict, List, Optional, Tuple, Type, Union
 from warnings import warn
 
 import filetype
+import pkg_resources
+import regex as re
 from PIL import Image
+from pympler import asizeof
 
-from konfuzio_sdk import IMAGE_FILE, PDF_FILE, OFFICE_FILE, SUPPORTED_FILE_TYPES
+from konfuzio_sdk import IMAGE_FILE, OFFICE_FILE, PDF_FILE, SUPPORTED_FILE_TYPES
 
 logger = logging.getLogger(__name__)
 
+if TYPE_CHECKING:  # only import when type checking to prevent circular import errors
+    from konfuzio_sdk.data import Bbox, Span
+
 
 def sdk_isinstance(instance, klass):
     """
     Implement a custom isinstance which is compatible with cloudpickle saving by value.
 
     When using cloudpickle with "register_pickle_by_value" the classes of "konfuzio.data" will be loaded in the
     "types" module. For this case the builtin method "isinstance" will return False because it tries to compare
     "types.Document" with "konfuzio_sdk.data.Document".
     """
     # TODO: Update test cases to use sdk_isinstance
     result = type(instance).__name__ == klass.__name__
     return result
 
 
-def get_id(a_string, include_time: bool = False) -> int:
+def exception_or_log_error(
+    msg: str,
+    handler: str = 'sdk',
+    fail_loudly: Optional[bool] = True,
+    exception_type: Optional[Type[Exception]] = ValueError,
+) -> None:
+    """
+    Log error or raise an exception.
+
+    This function is needed to control error handling in production. If `fail_loudly` is set to `True`, the function
+    raises an exception to type `exception_type` with a message and handler in the format `{"message" : msg,
+                                                                                            "handler" : handler}`.
+    If `fail_loudly` is set to `False`, the function logs an error with `msg` using the logger.
+
+    :param msg: (str): The error message to be logged or raised.
+    :param handler: (str): The handler associated with the error. Defaults to "sdk"
+    :param fail_loudly: A flag indicating whether to raise an exception or log the error. Defaults to `True`.
+    :param exception_type: The type of exception to be raised. Defaults to `ValueError`.
+    :return: None
+    """
+    # Raise whatever exception while specifying the handler
+    if fail_loudly:
+        raise exception_type({'message': msg, 'handler': handler})
+    else:
+        logger.error(msg)
+
+
+def get_id(include_time: bool = False) -> str:
     """
     Generate a unique ID.
 
-    :param a_string: String used to generating the unique ID
     :param include_time: Bool to include the time in the unique ID
     :return: Unique ID
     """
+    unique_id = str(uuid.uuid4())
     if include_time:
-        unique_string = a_string + get_timestamp(konfuzio_format='%Y-%m-%d-%H-%M-%S.%f')
+        return unique_id + get_timestamp(konfuzio_format='%Y-%m-%d-%H-%M-%S.%f')
     else:
-        unique_string = a_string
-    try:
-        return int(hashlib.md5(unique_string.encode()).hexdigest(), 16)
-    except (UnicodeDecodeError, AttributeError):  # duck typing for bytes like objects
-        return int(hashlib.md5(unique_string).hexdigest(), 16)
+        return unique_id
 
 
 def is_file(file_path, raise_exception=True, maximum_size=100000000, allow_empty=False) -> bool:
     """
     Check if file is available or raise error if it does not exist.
 
     :param file_path: Path to the file to be checked
@@ -63,43 +91,49 @@
     :return: True or false depending on the existence of the file
     """
     if os.path.isfile(file_path):
         file_size = os.path.getsize(file_path)
         if file_size > 0 or allow_empty:
             if file_size > maximum_size:
                 logger.warning(f'Please check your BIG file with size {file_size / 1000000:.2f} MB at {file_path}.')
-            with open(file_path, 'rb') as f:
-                logger.debug(f"File expected and found at {file_path} with ID {get_id(f.read())}")
+            with open(file_path, 'rb'):
+                logger.debug(f'File expected and found at {file_path} with ID {get_id()}')
             return True
         else:
             if raise_exception:
                 raise FileExistsError(f'Please check your file {file_path} with size {file_size} at {file_path}.')
             else:
                 return False
     else:
         if raise_exception:
             raise FileNotFoundError(f'File expected but not found at: {file_path}')
         else:
             return False
 
 
+def memory_size_of(obj) -> int:
+    """Return memory size of object in bytes."""
+    size = asizeof.asizeof(obj)
+    return size
+
+
 def normalize_memory(memory: Union[None, str]) -> Union[int, None]:
     """
-    Return memory size in human readable form to int of number of bytes.
+    Return memory size in human-readable form to int of number of bytes.
 
     :param memory: Memory size in human readable form (e.g. "50MB").
     :return: int of bytes if valid, else None
     """
     if memory is not None:
-        if type(memory) is int or memory.isdigit():
+        if isinstance(memory, int) or memory.isdigit():
             memory = int(memory)
         else:
             # Check if the first part of the string (before the unit) is numeric
             if not memory[:-3].isdigit() and not memory[:-2].isdigit():
-                logger.error(f"memory value {memory} invalid.")
+                logger.error(f'memory value {memory} invalid.')
                 return None
             else:
                 mem_val = int(memory[:-3] if memory[-3:].isalpha() else memory[:-2])
 
             # Check the unit and convert to bytes
             if memory[-2:].lower() == 'gb':
                 memory = mem_val * 1e9
@@ -110,15 +144,15 @@
             elif memory[-3:].lower() == 'gib':
                 memory = mem_val * 2**30
             elif memory[-3:].lower() == 'mib':
                 memory = mem_val * 2**20
             elif memory[-3:].lower() == 'kib':
                 memory = mem_val * 2**10
             else:
-                logger.error(f"memory value {memory} invalid.")
+                logger.error(f'memory value {memory} invalid.')
                 return None
     return memory
 
 
 def get_timestamp(konfuzio_format='%Y-%m-%d-%H-%M-%S') -> str:
     """
     Return formatted timestamp.
@@ -177,15 +211,15 @@
         file_path = 'bytes'
         extension = filetype.guess_extension(input_file)
     else:
         raise NotImplementedError(f'Unsupported type of argument file: {type(input_file)}.')
 
     def isdir(z, name):
         """Check zip file namelist."""
-        return any(x.startswith("%s/" % name.rstrip("/")) for x in z.namelist())
+        return any(x.startswith('%s/' % name.rstrip('/')) for x in z.namelist())
 
     def isfile(z, name):
         """Check zip file namelist."""
         return any(x.endswith(name) for x in z.namelist())
 
     if extension is None:
         if isinstance(input_file, str):
@@ -204,18 +238,18 @@
     if extension == 'pdf':
         file_type = PDF_FILE
     elif extension in ['png', 'tiff', 'tif', 'jpeg', 'jpg']:
         file_type = IMAGE_FILE
     elif extension == 'zip':
         r = zipfile.ZipFile(input_file)
         # check for office files
-        if isdir(r, "docProps") or isdir(r, "_rels"):
+        if isdir(r, 'docProps') or isdir(r, '_rels'):
             file_type = OFFICE_FILE
         # check for open office files
-        if isdir(r, "META-INF") and isfile(r, 'meta.xml') and isfile(r, 'settings.xml'):
+        if isdir(r, 'META-INF') and isfile(r, 'meta.xml') and isfile(r, 'settings.xml'):
             file_type = OFFICE_FILE
 
     if file_type not in [PDF_FILE, IMAGE_FILE, OFFICE_FILE]:
         error_message = f'We do not support file {file_name} with extension {extension} to get text: {file_path}'
         logger.error(error_message)
         raise NotImplementedError(error_message)
 
@@ -303,15 +337,17 @@
     """
     value = str(value)
     value = unicodedata.normalize('NFKD', value).encode('ascii', 'ignore').decode('ascii')
     value = re.sub(r'[^\:\.\w\s-]', '', value.lower())
     return re.sub(r'[-\s\:\.]+', '-', value).replace('-_', '_')
 
 
-def amend_file_name(file_name: str, append_text: str = '', new_extension: str = None) -> str:
+def amend_file_name(
+    file_name: str, append_text: str = '', append_separator: str = '_', new_extension: str = None
+) -> str:
     """
     Append text to a filename in front of extension.
 
     example found here: https://stackoverflow.com/a/37487898
 
     :param new_extension: Change the file extension
     :param file_path: Name of a file, e.g. file.pdf
@@ -326,145 +362,41 @@
 
         if new_extension == '':
             extension = ''
         elif new_extension:
             extension = new_extension
 
         if append_text:
-            append_text = f'_{append_text}'
+            append_text = f'{append_separator}{append_text}'
 
         return f'{path}{append_text}{extension}'
     else:
         raise ValueError(f'Name of file cannot be: {file_name}')
 
 
-def amend_file_path(file_path: str, append_text: str = '', new_extension: str = None):
+def amend_file_path(file_path: str, append_text: str = '', append_separator: str = '_', new_extension: str = None):
     """
     Similar to amend_file_name however the file_name is interpreted as a full path.
 
     :param new_extension: Change the file extension
     :param file_path: Name of a file, e.g. file.pdf
     :param append_text: Text you you want to append between file name ane extension
 
     :return: extended path to file
     """
     split_file_path, split_file_name = os.path.split(file_path)
-    new_filename = amend_file_name(split_file_name, append_text, new_extension)
+    new_filename = amend_file_name(
+        file_name=split_file_name,
+        append_text=append_text,
+        append_separator=append_separator,
+        new_extension=new_extension,
+    )
     return os.path.join(split_file_path, new_filename)
 
 
-# def get_paragraphs_by_line_space(
-#     bbox: dict,
-#     text: str,
-#     height: Union[float, int] = None,
-#     # return_dataframe: bool = False,
-#     line_height_ration: float = 0.8,
-# ) -> Union[List[List[List[dict]]], Tuple[List[List[List[dict]]]]]:
-#     """
-#     Split a text into paragraphs considering the space between the lines.
-#
-#     A paragraph consists in a list of lines. Each line corresponds to a dictionary.
-#
-#     :param bbox: Bounding boxes of the characters in the  Document
-#     :param text: Text of the document
-#     :param height: Threshold value for the distance between lines
-#     #:param return_dataframe: If to return a dataframe with the paragraph text and page number
-#     :param line_height_ration: Ratio of the result of median of the distance between lines as threshold
-#     :return: List of with the paragraph information per page of the document.
-#     """
-#     # Add start_offset and end_offset to every bbox item.
-#     from statistics import median
-#
-#     bbox = dict((k, dict(**v, start_offset=int(k), end_offset=int(k) + 1)) for (k, v) in bbox.items())
-#     page_numbers = set(int(box['page_number']) for box in bbox.values())
-#     document_structure = []
-#
-#     if height is not None:
-#         if not (isinstance(height, int) or isinstance(height, float)):
-#             raise Exception(f'Parameter must be of type int or float. It is {type(height)}.')
-#
-#     for page_number in page_numbers:
-#         previous_y0 = None
-#         paragraphs = []
-#
-#         if height is None:
-#             line_threshold = round(
-#                 line_height_ration
-#                 * median(box['y1'] - box['y0'] for box in bbox.values() if box['page_number'] == page_number),
-#                 6,
-#             )
-#         else:
-#             line_threshold = height
-#
-#         line_numbers = set(int(box['line_number']) for box in bbox.values() if box['page_number'] == page_number)
-#         for line_number in line_numbers:
-#             line_bboxes = list(
-#                 box for box in bbox.values()
-#                 if box['page_number'] == page_number and box['line_number'] == line_number
-#             )
-#             max_y1 = max([x['y1'] for x in line_bboxes])
-#             min_y0 = min([x['y0'] for x in line_bboxes])
-#
-#             max_x1 = max([x['x1'] for x in line_bboxes])
-#             min_x0 = min([x['x0'] for x in line_bboxes])
-#
-#             min_top = min([x['top'] for x in line_bboxes])
-#             max_bottom = max([x['bottom'] for x in line_bboxes])
-#
-#             start_offset = min(x['start_offset'] for x in line_bboxes)
-#             end_offset = max(x['end_offset'] for x in line_bboxes)
-#             _text = text[start_offset:end_offset]
-#
-#             # Do not create a paragraph for whitespaces.
-#             if _text.replace(' ', '') == '':
-#                 continue
-#
-#             paragraph = {
-#                 'start_offset': start_offset,
-#                 'end_offset': end_offset,
-#                 'text': _text,
-#                 'line_bbox': {
-#                     'x0': min_x0,
-#                     'x1': max_x1,
-#                     'y0': min_y0,
-#                     'y1': max_y1,
-#                     'top': min_top,
-#                     'bottom': max_bottom,
-#                     'page_index': page_number - 1,
-#                 },
-#             }
-#
-#             if previous_y0 is not None and previous_y0 - max_y1 < 0:
-#                 raise ValueError('Order of offsets does not match order y coordinate.')
-#
-#             if previous_y0 is not None and previous_y0 - max_y1 < line_threshold:
-#                 paragraphs[-1].append(paragraph)
-#             else:
-#                 paragraphs.append([paragraph])
-#
-#             previous_y0 = min_y0
-#
-#         document_structure.append(paragraphs)
-#
-#     return document_structure
-#
-#     #     for paragraph_ in paragraphs:
-#     #         paragraph_text = [line['text'] + "\n" for line in paragraph_]
-#     #         paragraph_text = ''.join(paragraph_text)
-#     #         data.append({"page_number": page_number, "paragraph_text": paragraph_text})
-#     #
-#     # dataframe = pd.DataFrame(data=data)
-#     #
-#     # if return_dataframe:
-#     #     return document_structure, dataframe
-#     #
-#     # else:
-#     #     return document_structure
-
-
 def get_sentences(text: str, offsets_map: Union[dict, None] = None, language: str = 'german') -> List[dict]:
     """
     Split a text into sentences using the sentence tokenizer from the package nltk.
 
     :param text: Text to split into sentences
     :param offsets_map: mapping between the position of the character in the input text and the offset in the text
     of the document
@@ -527,42 +459,44 @@
 
     :param characters_bboxes: Bounding boxes information of the characters.
     :returns: Mapping of the position of the characters and its offsets.
     """
     for character_bbox in characters_bboxes:
         character_bbox['string_offset'] = int(character_bbox['string_offset'])
     characters_bboxes.sort(key=lambda k: k['string_offset'])
-    offsets_map = dict((i, x['string_offset']) for i, x in enumerate(characters_bboxes))
+    offsets_map = {i: x['string_offset'] for i, x in enumerate(characters_bboxes)}
 
     return offsets_map
 
 
-def convert_segmentation_bbox(bbox: dict, page: dict) -> dict:
-    """
-    Convert bounding box from the segmentation result to the scale of the characters bboxes of the document.
+def detectron_get_paragraph_bboxes(detectron_document_results: List[List[Dict]], document) -> List[List['Bbox']]:
+    """Call detectron Bbox corresponding to each paragraph."""
+    from konfuzio_sdk.data import Bbox
+
+    assert len(detectron_document_results) == document.number_of_pages
+
+    paragraph_document_bboxes: List[List['Bbox']] = []
+
+    for page_index, detectron_page_results in enumerate(detectron_document_results):
+        paragraph_page_bboxes = []
+        for detectron_result in detectron_page_results:
+            paragraph_bbox = Bbox.from_image_size(
+                x0=detectron_result['x0'],
+                x1=detectron_result['x1'],
+                y1=detectron_result['y1'],
+                y0=detectron_result['y0'],
+                page=document.get_page_by_index(page_index=page_index),
+            )
+            label_name = detectron_result['label']
+            paragraph_bbox._label_name = label_name
+            paragraph_page_bboxes.append(paragraph_bbox)
+        paragraph_document_bboxes.append(paragraph_page_bboxes)
+    assert len(document.pages()) == len(paragraph_document_bboxes)
 
-    :param bbox: Bounding box from the segmentation result
-    :param page: Page information
-    :return: Converted bounding box.
-    """
-    warn('Method needs testing and revision. Please create a Ticket if you use it.', DeprecationWarning, stacklevel=2)
-    original_size = page['original_size']
-    image_size = page['size']
-    factor_y = original_size[1] / image_size[1]
-    factor_x = original_size[0] / image_size[0]
-    height = image_size[1]
-
-    temp_y0 = (height - bbox['y0']) * factor_y
-    temp_y1 = (height - bbox['y1']) * factor_y
-    bbox['y0'] = temp_y1
-    bbox['y1'] = temp_y0
-    bbox['x0'] = bbox['x0'] * factor_x
-    bbox['x1'] = bbox['x1'] * factor_x
-
-    return bbox
+    return paragraph_document_bboxes
 
 
 def select_bboxes(selection_bbox: dict, page_bboxes: list, tolerance: int = 10) -> list:
     """
     Filter the characters bboxes of the Document page according to their x/y values.
 
     The result only includes the characters that are inside the selection bbox.
@@ -572,102 +506,40 @@
     :param tolerance: Tolerance for the coordinates values.
     :return: Selected characters bboxes.
     """
     warn('Method needs testing and revision. Please create a Ticket if you use it.', DeprecationWarning, stacklevel=2)
     selected_char_bboxes = [
         char_bbox
         for char_bbox in page_bboxes
-        if int(selection_bbox["x0"]) - tolerance <= char_bbox["x0"]
-        and int(selection_bbox["x1"]) + tolerance >= char_bbox["x1"]
-        and int(selection_bbox["y0"]) - tolerance <= char_bbox["y0"]
-        and int(selection_bbox["y1"]) + tolerance >= char_bbox["y1"]
+        if int(selection_bbox['x0']) - tolerance <= char_bbox['x0']
+        and int(selection_bbox['x1']) + tolerance >= char_bbox['x1']
+        and int(selection_bbox['y0']) - tolerance <= char_bbox['y0']
+        and int(selection_bbox['y1']) + tolerance >= char_bbox['y1']
     ]
 
     return selected_char_bboxes
 
 
-def group_bboxes_per_line(char_bboxes: dict, page_index: int) -> list:
-    """
-    Group characters bounding boxes per line.
-
-    A line will have a single bounding box.
-
-    :param char_bboxes: Bounding boxes of the characters.
-    :param page_index: Index of the page in the document.
-    :return: List with 1 bounding box per line.
-    """
-    warn('Method needs testing and revision. Please create a Ticket if you use it.', DeprecationWarning, stacklevel=2)
-    lines_bboxes = []
-
-    # iterate over each line_number and all of the character bboxes with that line number
-    for line_number, line_char_bboxes in itertools.groupby(char_bboxes, lambda x: x['line_number']):
-        # set the default values which we overwrite with the actual character bbox values
-        x0 = 100000000
-        top = 10000000
-        y0 = 10000000
-        x1 = 0
-        y1 = 0
-        bottom = 0
-        start_offset = 100000000
-        end_offset = 0
-
-        # remove space chars from the line selection so they don't interfere with the merging of bboxes
-        # (a bbox should never start with a space char)
-        trimmed_line_char_bboxes = [char for char in line_char_bboxes if not char['text'].isspace()]
-
-        if len(trimmed_line_char_bboxes) == 0:
-            continue
-
-        # merge characters bounding boxes of the same line
-        for char_bbox in trimmed_line_char_bboxes:
-            x0 = min(char_bbox['x0'], x0)
-            top = min(char_bbox['top'], top)
-            y0 = min(char_bbox['y0'], y0)
-
-            x1 = max(char_bbox['x1'], x1)
-            bottom = max(char_bbox['bottom'], bottom)
-            y1 = max(char_bbox['y1'], y1)
-
-            start_offset = min(int(char_bbox['string_offset']), start_offset)
-            end_offset = max(int(char_bbox['string_offset']), end_offset)
-
-        line_bbox = {
-            'bottom': bottom,
-            'page_index': page_index,
-            'top': top,
-            'x0': x0,
-            'x1': x1,
-            'y0': y0,
-            'y1': y1,
-            'start_offset': start_offset,
-            'end_offset': end_offset + 1,
-            'line_number': line_number,
-        }
-
-        lines_bboxes.append(line_bbox)
-
-    return lines_bboxes
-
-
 def merge_bboxes(bboxes: list):
     """
     Merge bounding boxes.
 
     :param bboxes: Bounding boxes to be merged.
     :return: Merged bounding box.
     """
     warn('Method needs testing and revision. Please create a Ticket if you use it.', DeprecationWarning, stacklevel=2)
+    # the issue is there: https://git.konfuzio.com/konfuzio/objectives/-/issues/9333
     merge_bbox = {
-        "x0": min([b['x0'] for b in bboxes]),
-        "x1": max([b['x1'] for b in bboxes]),
-        "y0": min([b['y0'] for b in bboxes]),
-        "y1": max([b['y1'] for b in bboxes]),
-        "top": min([b['top'] for b in bboxes]),
-        "bottom": max([b['bottom'] for b in bboxes]),
-        "page_index": bboxes[0]['page_index'],
+        'x0': min([b['x0'] for b in bboxes]),
+        'x1': max([b['x1'] for b in bboxes]),
+        'y0': min([b['y0'] for b in bboxes]),
+        'y1': max([b['y1'] for b in bboxes]),
+        'top': min([b['top'] for b in bboxes]),
+        'bottom': max([b['bottom'] for b in bboxes]),
+        'page_index': bboxes[0]['page_index'],
     }
 
     return merge_bbox
 
 
 def get_bbox(bbox, start_offset: int, end_offset: int) -> Dict:
     """
@@ -682,48 +554,53 @@
     """
     warn('This method is deprecated. Please use Spans in Documents or Bbox in Pages.', DeprecationWarning, stacklevel=2)
     # get the index of every character bbox in the Document between the start and end offset
     char_bbox_ids = [str(char_bbox_id) for char_bbox_id in range(start_offset, end_offset) if str(char_bbox_id) in bbox]
 
     # exit early if no bboxes are found between the start/end offset
     if not char_bbox_ids:
-        logger.error(f"Between start {start_offset} and {end_offset} we do not find the bboxes of the characters.")
+        logger.error(f'Between start {start_offset} and {end_offset} we do not find the bboxes of the characters.')
         raise ValueError(f'Characters from {start_offset} to {end_offset} do not provide any bounding box.')
 
     # set the default values which we overwrite with the actual character bbox values
     x0 = 100000000
     top = 10000000
     y0 = 10000000
     x1 = 0
     y1 = 0
     bottom = 0
     pdf_page_index = None
     line_indexes = []  # todo create one bounding box per line.
 
-    # combine all of the found character bboxes and calculate their combined x0, x1, etc. values
+    # combine all the found character bboxes and calculate their combined x0, x1, etc. values
     for char_bbox_id in char_bbox_ids:
+        # conditions for backward compatibility
         x0 = min(bbox[char_bbox_id]['x0'], x0)
-        top = min(bbox[char_bbox_id]['top'], top)
+        if 'top' in bbox[char_bbox_id].keys():
+            top = min(bbox[char_bbox_id]['top'], top)
         y0 = min(bbox[char_bbox_id]['y0'], y0)
 
         x1 = max(bbox[char_bbox_id]['x1'], x1)
-        bottom = max(bbox[char_bbox_id]['bottom'], bottom)
+        if 'bottom' in bbox[char_bbox_id].keys():
+            bottom = max(bbox[char_bbox_id]['bottom'], bottom)
         y1 = max(bbox[char_bbox_id]['y1'], y1)
-        line_indexes.append(bbox[char_bbox_id]['page_number'])
+        if 'page_number' in bbox[char_bbox_id]:
+            line_indexes.append(bbox[char_bbox_id]['page_number'])
 
         if pdf_page_index is not None:
             try:
                 assert pdf_page_index == bbox[char_bbox_id]['page_number'] - 1
             except AssertionError:
                 logger.warning(
                     "We don't support bounding boxes over page breaks yet, and will return the bounding box"
-                    "on the first page of the match."
+                    'on the first page of the match.'
                 )
                 break
-        pdf_page_index = bbox[char_bbox_id]['page_number'] - 1
+        if 'page_number' in bbox[char_bbox_id]:
+            pdf_page_index = bbox[char_bbox_id]['page_number'] - 1
 
     res = {'bottom': bottom, 'page_index': pdf_page_index, 'top': top, 'x0': x0, 'x1': x1, 'y0': y0, 'y1': y1}
     if len(set(line_indexes)) == 1:
         res['line_index'] = line_indexes[0]
     return res
 
 
@@ -837,23 +714,23 @@
     # sort selected bboxes by y first, then x
     bboxes.sort(key=operator.itemgetter('y0', 'x0'))
 
     # iterate through every bbox of the selection
     for selection_bbox in bboxes:
         selected_bboxes = [
             # the index of the character is its offset, i.e. the number of chars before it in the document's text
-            {"string_offset": index, **char_bbox}
+            {'string_offset': index, **char_bbox}
             for index, char_bbox in doc_bbox.items()
-            if selection_bbox["page_index"] == char_bbox["page_number"] - 1
+            if selection_bbox['page_index'] == char_bbox['page_number'] - 1
             # filter the characters of the document according to their x/y values, so that we only include the
             # characters that are inside the selection
-            and selection_bbox["x0"] <= char_bbox["x0"]
-            and selection_bbox["x1"] >= char_bbox["x1"]
-            and selection_bbox["y0"] <= char_bbox["y0"]
-            and selection_bbox["y1"] >= char_bbox["y1"]
+            and selection_bbox['x0'] <= char_bbox['x0']
+            and selection_bbox['x1'] >= char_bbox['x1']
+            and selection_bbox['y0'] <= char_bbox['y0']
+            and selection_bbox['y1'] >= char_bbox['y1']
         ]
 
         # decide what we are going to group the character bboxes by in order to group those on the same line
         # either group by 'line_number' (if they all have a 'line_number' attribute) or 'bottom'
         if all('line_number' in selected_bbox.keys() for selected_bbox in selected_bboxes):
             group_by = 'line_number'
         else:
@@ -895,15 +772,15 @@
 
                 if pdf_page_index is not None:
                     try:
                         assert pdf_page_index == char_bbox['page_number'] - 1
                     except AssertionError:
                         logger.warning(
                             "We don't support bounding boxes over page breaks yet, and will return the bounding box"
-                            "on the first page of the match."
+                            'on the first page of the match.'
                         )
                         break
 
                 pdf_page_index = char_bbox['page_number'] - 1
 
             line_bbox = {
                 'bottom': bottom,
@@ -976,15 +853,15 @@
             merged_bboxes[-1]['bottom'] = max(merged_bboxes[-1]['bottom'], line_bbox['bottom'])
             merged_bboxes[-1]['y1'] = max(merged_bboxes[-1]['y1'], line_bbox['y1'])
             merged_bboxes[-1]['start_offset'] = min(merged_bboxes[-1]['start_offset'], line_bbox['start_offset'])
             merged_bboxes[-1]['end_offset'] = max(merged_bboxes[-1]['end_offset'], line_bbox['end_offset'])
 
             # if both bboxes have the offset string property, merge them
             if merged_bboxes[-1].get('offset_string') and line_bbox.get('offset_string'):
-                merged_bboxes[-1]['offset_string'] += " " * amount_of_spaces_in_between + line_bbox['offset_string']
+                merged_bboxes[-1]['offset_string'] += ' ' * amount_of_spaces_in_between + line_bbox['offset_string']
 
         # otherwise, just add the bbox to the list
         else:
             merged_bboxes.append(line_bbox)
 
     # if we're passed a doc_text, add an offset_string to each bbox
     if doc_text:
@@ -992,7 +869,44 @@
             offset_string = doc_text[bbox['start_offset'] : bbox['end_offset']]
             # don't override offset_string if already set
             if not bbox.get('offset_string'):
                 bbox['offset_string'] = offset_string
             bbox['offset_string_original'] = offset_string
 
     return merged_bboxes
+
+
+def get_sdk_version():
+    """Get a version of current Konfuzio SDK used."""
+    return pkg_resources.get_distribution('konfuzio-sdk').version
+
+
+def get_spans_from_bbox(selection_bbox: 'Bbox') -> List['Span']:
+    """Get a list of Spans for all the text contained within a Bbox."""
+    from konfuzio_sdk.data import Span
+
+    selected_bboxes = [
+        char_bbox for _, char_bbox in selection_bbox.page.get_bbox().items() if selection_bbox.check_overlap(char_bbox)
+    ]
+    selected_bboxes = sorted(selected_bboxes, key=lambda x: x['char_index'])
+
+    # iterate over each line_number (or bottom, depending on group_by) and all the character
+    # bboxes that have the same line_number (or bottom)
+    spans = []
+    if selected_bboxes:
+        # condition for backward compatibility
+        line_key = 'line_index' if 'line_index' in selected_bboxes[0].keys() else 'line_number'
+        for _, line_char_bboxes in itertools.groupby(selected_bboxes, lambda x: x[line_key]):
+            # remove space chars from the line selection, so they don't interfere with the merging of bboxes
+            # (a bbox should never start with a space char)
+            trimmed_line_char_bboxes = [char for char in line_char_bboxes if not char['text'].isspace()]
+
+            if len(trimmed_line_char_bboxes) == 0:
+                continue
+
+            # combine all the found character bboxes on a given line and calculate their combined x0, x1, etc. values
+            start_offset = min(char_bbox['char_index'] for char_bbox in trimmed_line_char_bboxes)
+            end_offset = max(char_bbox['char_index'] for char_bbox in trimmed_line_char_bboxes)
+            span = Span(start_offset=start_offset, end_offset=end_offset + 1, document=selection_bbox.page.document)
+            spans.append(span)
+
+    return spans
```

### Comparing `konfuzio_sdk-0.2.9.dev20230104175944/setup.py` & `konfuzio_sdk-0.3.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """Setup."""
 import subprocess
 import sys
 import textwrap
-from os import path, getenv
+from os import getenv, path
 
 import setuptools
 
+from extras_list import EXTRAS
 
 # Define version or calculate it for nightly build.
 #
 # PEP0440 compatible formatted version, see:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # Generic release markers:
@@ -32,17 +33,17 @@
 if getenv('NIGHTLY_BUILD'):
     # create a pre-release
     last_commit = (
         subprocess.check_output(['git', 'log', '-1', '--pretty=%cd', '--date=format:%Y%m%d%H%M%S'])
         .decode('ascii')
         .strip()
     )
-    version = f"{version_number}.dev{last_commit}"
+    version = f'{version_number}.dev{last_commit}'
 else:
-    version = f"{version_number}"
+    version = f'{version_number}'
 
 CURRENT_PYTHON = sys.version_info[:2]
 REQUIRED_PYTHON = (3, 7)
 
 if CURRENT_PYTHON < REQUIRED_PYTHON:
     sys.stderr.write(
         textwrap.dedent(
@@ -58,51 +59,39 @@
     sys.exit(1)
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
-    name="konfuzio_sdk",
+    name='konfuzio_sdk',
     version=version,
     author='Helm & Nagel GmbH',
-    author_email="info@helm-nagel.com",
-    description="Konfuzio Software Development Kit",
+    author_email='info@helm-nagel.com',
+    description='Konfuzio Software Development Kit',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    url="https://github.com/konfuzio-ai/konfuzio-sdk/",
+    url='https://github.com/konfuzio-ai/konfuzio-sdk/',
     packages=['konfuzio_sdk', 'konfuzio_sdk.tokenizer', 'konfuzio_sdk.trainer'],
     include_package_data=True,
     entry_points={'console_scripts': ['konfuzio_sdk=konfuzio_sdk.cli:main']},
     install_requires=[
-        'cloudpickle==2.0.0',  # Used to pickle objects
+        'certifi==2023.7.22',
+        'cloudpickle==2.2.1',  # Used to pickle objects
         'filetype==1.0.7',  # Used to check that files are in the correct format
-        'nltk',
-        'numpy>=1.21.6',
-        'pandas>=1.3.5',
-        'Pillow>=7.1.2',
-        'python-dateutil',
-        'python-decouple',  # todo add ==3.3 ?
-        'requests',  # todo add ==2.24.0 ?
+        'lz4>=4.3.2',  # Used to compress pickles
+        'matplotlib==3.7.1',
+        'nltk>=3.6.3',
+        'numpy>=1.22.4',
+        'pandas>=1.3.5,<2.0.0',
+        'Pillow>=8.4.0',
+        'python-dateutil>=2.8.2',
+        'python-decouple>=3.3',
+        'requests',
         'regex>=2020.6.8',  # re module but better
-        'tabulate==0.8.7',  # Used to pretty print DataFrames
-        'tqdm',
-        'pympler==1.0.1',  # Use to get pickle file size.
-        'scikit-learn==1.0.2',
+        'scikit-learn==1.2.2',
+        'tabulate>=0.9.0',  # Used to pretty print DataFrames
+        'tqdm>=4.64.0',
+        'pympler>=1.0.1',  # Use to get pickle file size.
     ],
-    extras_require={
-        'dev': [
-            'flake8',
-            'pydocstyle',
-            'pytest',
-            'pre-commit',
-            'parameterized',
-            'Sphinx==4.4.0',
-            'sphinx-reload==0.2.0',
-            'sphinx-notfound-page==0.8',
-            'm2r2==0.3.2',
-            'sphinx-sitemap==2.2.0',
-            'sphinx-rtd-theme==1.0.0',
-            'sphinxcontrib-mermaid==0.7.1',
-        ]
-    },
+    extras_require=EXTRAS,
 )
```

