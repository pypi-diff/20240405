# Comparing `tmp/dataspree-platform-sdk-1.9.5.tar.gz` & `tmp/dataspree-platform-sdk-1.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataspree-platform-sdk-1.9.5.tar", last modified: Mon Jan 29 16:30:16 2024, max compression
+gzip compressed data, was "dataspree-platform-sdk-1.9.6.tar", last modified: Fri Apr  5 14:11:45 2024, max compression
```

## Comparing `dataspree-platform-sdk-1.9.5.tar` & `dataspree-platform-sdk-1.9.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 x         (1000) x         (1000)        0 2024-01-29 16:30:16.965099 dataspree-platform-sdk-1.9.5/
--rw-r--r--   0 x         (1000) x         (1000)     9585 2023-09-16 12:25:47.000000 dataspree-platform-sdk-1.9.5/LICENSE
--rw-r--r--   0 x         (1000) x         (1000)       25 2023-09-16 12:25:47.000000 dataspree-platform-sdk-1.9.5/MANIFEST.in
--rw-rw-r--   0 x         (1000) x         (1000)     2759 2024-01-29 16:30:16.965099 dataspree-platform-sdk-1.9.5/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)     2228 2023-09-16 12:25:47.000000 dataspree-platform-sdk-1.9.5/README.md
-drwxrwxr-x   0 x         (1000) x         (1000)        0 2024-01-29 16:30:16.965099 dataspree-platform-sdk-1.9.5/dataspree/
-drwxrwxr-x   0 x         (1000) x         (1000)        0 2024-01-29 16:30:16.965099 dataspree-platform-sdk-1.9.5/dataspree/platform_sdk/
--rw-rw-r--   0 x         (1000) x         (1000)      613 2024-01-29 16:29:31.000000 dataspree-platform-sdk-1.9.5/dataspree/platform_sdk/__init__.py
--rw-r--r--   0 x         (1000) x         (1000)     9594 2023-09-16 12:25:47.000000 dataspree-platform-sdk-1.9.5/dataspree/platform_sdk/base_model.py
--rw-r--r--   0 x         (1000) x         (1000)    12174 2023-09-16 12:25:47.000000 dataspree-platform-sdk-1.9.5/dataspree/platform_sdk/cli.py
--rw-r--r--   0 x         (1000) x         (1000)    79663 2023-11-21 15:11:57.000000 dataspree-platform-sdk-1.9.5/dataspree/platform_sdk/client.py
--rw-r--r--   0 x         (1000) x         (1000)    20820 2023-09-16 12:25:47.000000 dataspree-platform-sdk-1.9.5/dataspree/platform_sdk/data_loader.py
-drwxrwxr-x   0 x         (1000) x         (1000)        0 2024-01-29 16:30:16.965099 dataspree-platform-sdk-1.9.5/dataspree/platform_sdk/decoder/
--rw-r--r--   0 x         (1000) x         (1000)      628 2023-09-16 12:25:47.000000 dataspree-platform-sdk-1.9.5/dataspree/platform_sdk/decoder/__init__.py
--rw-r--r--   0 x         (1000) x         (1000)     1354 2023-09-16 12:25:47.000000 dataspree-platform-sdk-1.9.5/dataspree/platform_sdk/decoder/base_decoder.py
--rw-rw-r--   0 x         (1000) x         (1000)     4236 2024-01-29 16:29:31.000000 dataspree-platform-sdk-1.9.5/dataspree/platform_sdk/decoder/opencv_decoder.py
--rw-r--r--   0 x         (1000) x         (1000)     1949 2023-09-16 12:25:47.000000 dataspree-platform-sdk-1.9.5/dataspree/platform_sdk/decoder/pcd_decoder.py
--rw-r--r--   0 x         (1000) x         (1000)     6731 2023-09-16 12:25:47.000000 dataspree-platform-sdk-1.9.5/dataspree/platform_sdk/decoder/serializer.py
--rw-r--r--   0 x         (1000) x         (1000)      946 2023-09-16 12:25:47.000000 dataspree-platform-sdk-1.9.5/dataspree/platform_sdk/http_token_authentication.py
--rw-r--r--   0 x         (1000) x         (1000)     4771 2023-09-16 12:25:47.000000 dataspree-platform-sdk-1.9.5/dataspree/platform_sdk/query.py
--rw-r--r--   0 x         (1000) x         (1000)    33032 2023-09-16 12:25:47.000000 dataspree-platform-sdk-1.9.5/dataspree/platform_sdk/worker.py
-drwxrwxr-x   0 x         (1000) x         (1000)        0 2024-01-29 16:30:16.965099 dataspree-platform-sdk-1.9.5/dataspree_platform_sdk.egg-info/
--rw-r--r--   0 x         (1000) x         (1000)     2759 2024-01-29 16:30:16.000000 dataspree-platform-sdk-1.9.5/dataspree_platform_sdk.egg-info/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)      874 2024-01-29 16:30:16.000000 dataspree-platform-sdk-1.9.5/dataspree_platform_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 x         (1000) x         (1000)        1 2024-01-29 16:30:16.000000 dataspree-platform-sdk-1.9.5/dataspree_platform_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 x         (1000) x         (1000)       54 2024-01-29 16:30:16.000000 dataspree-platform-sdk-1.9.5/dataspree_platform_sdk.egg-info/entry_points.txt
--rw-r--r--   0 x         (1000) x         (1000)      185 2024-01-29 16:30:16.000000 dataspree-platform-sdk-1.9.5/dataspree_platform_sdk.egg-info/requires.txt
--rw-r--r--   0 x         (1000) x         (1000)       10 2024-01-29 16:30:16.000000 dataspree-platform-sdk-1.9.5/dataspree_platform_sdk.egg-info/top_level.txt
--rw-r--r--   0 x         (1000) x         (1000)       63 2023-09-16 12:25:47.000000 dataspree-platform-sdk-1.9.5/requirements.txt
--rw-rw-r--   0 x         (1000) x         (1000)       38 2024-01-29 16:30:16.965099 dataspree-platform-sdk-1.9.5/setup.cfg
--rw-r--r--   0 x         (1000) x         (1000)     2510 2023-09-16 12:25:47.000000 dataspree-platform-sdk-1.9.5/setup.py
-drwxrwxr-x   0 x         (1000) x         (1000)        0 2024-01-29 16:30:16.965099 dataspree-platform-sdk-1.9.5/tests/
--rw-r--r--   0 x         (1000) x         (1000)     2853 2023-09-16 12:25:47.000000 dataspree-platform-sdk-1.9.5/tests/test_upload.py
+drwxrwxr-x   0 x         (1000) x         (1000)        0 2024-04-05 14:11:45.755936 dataspree-platform-sdk-1.9.6/
+-rw-r--r--   0 x         (1000) x         (1000)     9585 2023-09-16 12:25:47.000000 dataspree-platform-sdk-1.9.6/LICENSE
+-rw-r--r--   0 x         (1000) x         (1000)       25 2023-09-16 12:25:47.000000 dataspree-platform-sdk-1.9.6/MANIFEST.in
+-rw-rw-r--   0 x         (1000) x         (1000)     3272 2024-04-05 14:11:45.751936 dataspree-platform-sdk-1.9.6/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)     2228 2023-09-16 12:25:47.000000 dataspree-platform-sdk-1.9.6/README.md
+drwxrwxr-x   0 x         (1000) x         (1000)        0 2024-04-05 14:11:45.747936 dataspree-platform-sdk-1.9.6/dataspree/
+drwxrwxr-x   0 x         (1000) x         (1000)        0 2024-04-05 14:11:45.751936 dataspree-platform-sdk-1.9.6/dataspree/platform_sdk/
+-rw-rw-r--   0 x         (1000) x         (1000)      613 2024-04-05 14:08:25.000000 dataspree-platform-sdk-1.9.6/dataspree/platform_sdk/__init__.py
+-rw-r--r--   0 x         (1000) x         (1000)     9594 2023-09-16 12:25:47.000000 dataspree-platform-sdk-1.9.6/dataspree/platform_sdk/base_model.py
+-rw-r--r--   0 x         (1000) x         (1000)    12174 2023-09-16 12:25:47.000000 dataspree-platform-sdk-1.9.6/dataspree/platform_sdk/cli.py
+-rw-rw-r--   0 x         (1000) x         (1000)    79663 2024-04-05 14:08:25.000000 dataspree-platform-sdk-1.9.6/dataspree/platform_sdk/client.py
+-rw-r--r--   0 x         (1000) x         (1000)    20820 2023-09-16 12:25:47.000000 dataspree-platform-sdk-1.9.6/dataspree/platform_sdk/data_loader.py
+drwxrwxr-x   0 x         (1000) x         (1000)        0 2024-04-05 14:11:45.751936 dataspree-platform-sdk-1.9.6/dataspree/platform_sdk/decoder/
+-rw-r--r--   0 x         (1000) x         (1000)      628 2023-09-16 12:25:47.000000 dataspree-platform-sdk-1.9.6/dataspree/platform_sdk/decoder/__init__.py
+-rw-r--r--   0 x         (1000) x         (1000)     1354 2023-09-16 12:25:47.000000 dataspree-platform-sdk-1.9.6/dataspree/platform_sdk/decoder/base_decoder.py
+-rw-rw-r--   0 x         (1000) x         (1000)     4236 2024-01-29 16:29:31.000000 dataspree-platform-sdk-1.9.6/dataspree/platform_sdk/decoder/opencv_decoder.py
+-rw-r--r--   0 x         (1000) x         (1000)     1949 2023-09-16 12:25:47.000000 dataspree-platform-sdk-1.9.6/dataspree/platform_sdk/decoder/pcd_decoder.py
+-rw-rw-r--   0 x         (1000) x         (1000)     7421 2024-04-05 14:08:25.000000 dataspree-platform-sdk-1.9.6/dataspree/platform_sdk/decoder/serializer.py
+-rw-r--r--   0 x         (1000) x         (1000)      946 2023-09-16 12:25:47.000000 dataspree-platform-sdk-1.9.6/dataspree/platform_sdk/http_token_authentication.py
+-rw-r--r--   0 x         (1000) x         (1000)     4771 2023-09-16 12:25:47.000000 dataspree-platform-sdk-1.9.6/dataspree/platform_sdk/query.py
+-rw-r--r--   0 x         (1000) x         (1000)    33032 2023-09-16 12:25:47.000000 dataspree-platform-sdk-1.9.6/dataspree/platform_sdk/worker.py
+drwxrwxr-x   0 x         (1000) x         (1000)        0 2024-04-05 14:11:45.751936 dataspree-platform-sdk-1.9.6/dataspree_platform_sdk.egg-info/
+-rw-r--r--   0 x         (1000) x         (1000)     3272 2024-04-05 14:11:45.000000 dataspree-platform-sdk-1.9.6/dataspree_platform_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)      874 2024-04-05 14:11:45.000000 dataspree-platform-sdk-1.9.6/dataspree_platform_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 x         (1000) x         (1000)        1 2024-04-05 14:11:45.000000 dataspree-platform-sdk-1.9.6/dataspree_platform_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 x         (1000) x         (1000)       73 2024-04-05 14:11:45.000000 dataspree-platform-sdk-1.9.6/dataspree_platform_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 x         (1000) x         (1000)      185 2024-04-05 14:11:45.000000 dataspree-platform-sdk-1.9.6/dataspree_platform_sdk.egg-info/requires.txt
+-rw-r--r--   0 x         (1000) x         (1000)       10 2024-04-05 14:11:45.000000 dataspree-platform-sdk-1.9.6/dataspree_platform_sdk.egg-info/top_level.txt
+-rw-r--r--   0 x         (1000) x         (1000)       63 2023-09-16 12:25:47.000000 dataspree-platform-sdk-1.9.6/requirements.txt
+-rw-rw-r--   0 x         (1000) x         (1000)       38 2024-04-05 14:11:45.755936 dataspree-platform-sdk-1.9.6/setup.cfg
+-rw-r--r--   0 x         (1000) x         (1000)     2510 2023-09-16 12:25:47.000000 dataspree-platform-sdk-1.9.6/setup.py
+drwxrwxr-x   0 x         (1000) x         (1000)        0 2024-04-05 14:11:45.751936 dataspree-platform-sdk-1.9.6/tests/
+-rw-r--r--   0 x         (1000) x         (1000)     2853 2023-09-16 12:25:47.000000 dataspree-platform-sdk-1.9.6/tests/test_upload.py
```

### Comparing `dataspree-platform-sdk-1.9.5/LICENSE` & `dataspree-platform-sdk-1.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dataspree-platform-sdk-1.9.5/PKG-INFO` & `dataspree-platform-sdk-1.9.6/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: dataspree-platform-sdk
-Version: 1.9.5
-Summary: Python SDK Data Spree AI Platform
-Home-page: https://data-spree.com/ai
-Author: Data Spree GmbH
-Author-email: info@data-spree.com
-License: Apache-2.0
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: kitti
-Provides-Extra: worker
-Provides-Extra: build
-License-File: LICENSE
-
 # Data Spree AI Platform SDK
 The Platform SDK acts as an interface to the Data Spree AI Platform, contains all classes and functions to integrate
 custom models into the platform, and it provides a command-line tool for importing datasets of the following formats:
 * Data Spree
 * KITTI
 * COCO
```

### Comparing `dataspree-platform-sdk-1.9.5/README.md` & `dataspree-platform-sdk-1.9.6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,63 +1,81 @@
-# Data Spree AI Platform SDK
-The Platform SDK acts as an interface to the Data Spree AI Platform, contains all classes and functions to integrate
-custom models into the platform, and it provides a command-line tool for importing datasets of the following formats:
-* Data Spree
-* KITTI
-* COCO
-
-Furthermore, it is possible to export datasets from the platform.
-
-## Usage
-
-### General Usage
-```
-Usage: ds [OPTIONS] COMMAND [ARGS]...
-
-Options:
-  --help  Show this message and exit.
-
-Commands:
-  export
-  import
-```
-
-### Dataset Import
-```
-Usage: ds import [OPTIONS]
-
-Options:
-  --format [dataspree|kitti|coco]  Dataset format to import
-  --dataset_name TEXT         Name of the newly created dataset.
-  --dataset_id INTEGER        ID of the dataset to which new items should be
-                              imported. If set to '-1', a new dataset will be
-                              created
-  --images PATH               Directory containing the images to import.
-                              [required]
-  --annotations PATH          Directory or file containing the annotations to
-                              import.  [required]
-  --http_retries INTEGER      Number of HTTP retries.  [default: 10]
-  --username TEXT             Username for data spree vision platform.
-  --password TEXT             Password for data spree vision platform.
-  --url TEXT                  URL to the API of the platform.
-  --help                      Show this message and exit.
-```
-
-### Dataset Export
-```
-Usage: ds export [OPTIONS]
-
-Options:
-  -o, --output_dir DIRECTORY   Output directory.  [required]
-  -i, --id INTEGER             ID of the dataset to download.
-  -n, --n_items INTEGER        Number of items to download. Download all
-                               items: '-1'  [default: -1]
-  --http_retries INTEGER       Number of HTTP retries.  [default: 10]
-  --parallel_requests INTEGER  Number of parallel requests.  [default: 16]
-  --username TEXT              Username for data spree vision platform.
-  --password TEXT              Password for data spree vision platform.
-  --url TEXT                   URL to the API of the platform.
-  --help                       Show this message and exit.
-```
-
-## License
-Apache License 2.0
+Metadata-Version: 2.1
+Name: dataspree-platform-sdk
+Version: 1.9.6
+Summary: Python SDK Data Spree AI Platform
+Home-page: https://data-spree.com/ai
+Author: Data Spree GmbH
+Author-email: info@data-spree.com
+License: Apache-2.0
+Description: # Data Spree AI Platform SDK
+        The Platform SDK acts as an interface to the Data Spree AI Platform, contains all classes and functions to integrate
+        custom models into the platform, and it provides a command-line tool for importing datasets of the following formats:
+        * Data Spree
+        * KITTI
+        * COCO
+        
+        Furthermore, it is possible to export datasets from the platform.
+        
+        ## Usage
+        
+        ### General Usage
+        ```
+        Usage: ds [OPTIONS] COMMAND [ARGS]...
+        
+        Options:
+          --help  Show this message and exit.
+        
+        Commands:
+          export
+          import
+        ```
+        
+        ### Dataset Import
+        ```
+        Usage: ds import [OPTIONS]
+        
+        Options:
+          --format [dataspree|kitti|coco]  Dataset format to import
+          --dataset_name TEXT         Name of the newly created dataset.
+          --dataset_id INTEGER        ID of the dataset to which new items should be
+                                      imported. If set to '-1', a new dataset will be
+                                      created
+          --images PATH               Directory containing the images to import.
+                                      [required]
+          --annotations PATH          Directory or file containing the annotations to
+                                      import.  [required]
+          --http_retries INTEGER      Number of HTTP retries.  [default: 10]
+          --username TEXT             Username for data spree vision platform.
+          --password TEXT             Password for data spree vision platform.
+          --url TEXT                  URL to the API of the platform.
+          --help                      Show this message and exit.
+        ```
+        
+        ### Dataset Export
+        ```
+        Usage: ds export [OPTIONS]
+        
+        Options:
+          -o, --output_dir DIRECTORY   Output directory.  [required]
+          -i, --id INTEGER             ID of the dataset to download.
+          -n, --n_items INTEGER        Number of items to download. Download all
+                                       items: '-1'  [default: -1]
+          --http_retries INTEGER       Number of HTTP retries.  [default: 10]
+          --parallel_requests INTEGER  Number of parallel requests.  [default: 16]
+          --username TEXT              Username for data spree vision platform.
+          --password TEXT              Password for data spree vision platform.
+          --url TEXT                   URL to the API of the platform.
+          --help                       Show this message and exit.
+        ```
+        
+        ## License
+        Apache License 2.0
+        
+Platform: UNKNOWN
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Provides-Extra: kitti
+Provides-Extra: worker
+Provides-Extra: build
```

### Comparing `dataspree-platform-sdk-1.9.5/dataspree/platform_sdk/__init__.py` & `dataspree-platform-sdk-1.9.6/dataspree/platform_sdk/decoder/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-__version__ = '1.9.5'
+from .base_decoder import BaseDecoder
```

### Comparing `dataspree-platform-sdk-1.9.5/dataspree/platform_sdk/base_model.py` & `dataspree-platform-sdk-1.9.6/dataspree/platform_sdk/base_model.py`

 * *Files identical despite different names*

### Comparing `dataspree-platform-sdk-1.9.5/dataspree/platform_sdk/cli.py` & `dataspree-platform-sdk-1.9.6/dataspree/platform_sdk/cli.py`

 * *Files identical despite different names*

### Comparing `dataspree-platform-sdk-1.9.5/dataspree/platform_sdk/client.py` & `dataspree-platform-sdk-1.9.6/dataspree/platform_sdk/client.py`

 * *Files identical despite different names*

### Comparing `dataspree-platform-sdk-1.9.5/dataspree/platform_sdk/data_loader.py` & `dataspree-platform-sdk-1.9.6/dataspree/platform_sdk/data_loader.py`

 * *Files identical despite different names*

### Comparing `dataspree-platform-sdk-1.9.5/dataspree/platform_sdk/decoder/base_decoder.py` & `dataspree-platform-sdk-1.9.6/dataspree/platform_sdk/decoder/base_decoder.py`

 * *Files identical despite different names*

### Comparing `dataspree-platform-sdk-1.9.5/dataspree/platform_sdk/decoder/opencv_decoder.py` & `dataspree-platform-sdk-1.9.6/dataspree/platform_sdk/decoder/opencv_decoder.py`

 * *Files identical despite different names*

### Comparing `dataspree-platform-sdk-1.9.5/dataspree/platform_sdk/decoder/pcd_decoder.py` & `dataspree-platform-sdk-1.9.6/dataspree/platform_sdk/decoder/pcd_decoder.py`

 * *Files identical despite different names*

### Comparing `dataspree-platform-sdk-1.9.5/dataspree/platform_sdk/decoder/serializer.py` & `dataspree-platform-sdk-1.9.6/dataspree/platform_sdk/decoder/serializer.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 import time
 import logging
 import numpy as np
 from typing import Any, Dict, Tuple, Optional, List, Iterator
 
 logger = logging.getLogger(__name__)
 
+try:
+    import lzma
+except Exception as e:
+    logger.warning('LZMA cannot be imported. LZMA compressed point clouds cannot be loaded')
+
+
 
 def load_pcd(data: bytes, width: Optional[int] = None, height: Optional[int] = None) \
         -> Tuple[np.ndarray, Dict[str, Any]]:
     """
     :brief: Load the entire content of the CPD file accessible via `filename` to the `item`.
             Retain types and dimensions indicated in PCD file.
     """
     times: List[Tuple[str, float]] = [('', time.time())]
 
     # Read header
     is_binary: bool
+    is_compressed_lzma: bool
     property_dict: Dict[str, List[str]] = dict()
     while True:
         line, data = read_line(data)
         if len(line) == 0:
             raise ValueError(f'Corrupted PCD data. The file does not contain a header.')
 
         current_line: List[str] = line.decode('utf-8')[:-1].split(' ')
@@ -27,15 +34,18 @@
         #       I don't think we have to treat the case line == " *" differently.
         # if current_line[0] == '':
         #     break
         if len(current_line):
             property_dict[current_line[0]] = current_line[1:]
 
             if current_line[0] == 'DATA':
-                is_binary = current_line[1] == 'binary'
+                is_binary = current_line[1].lower() != 'ascii'
+                is_compressed_lzma = current_line[1].lower() == 'binary_compressed_lzma'
+
+                #is_binary = current_line[1] == 'binary'
                 break
 
     # Acquire relevant information.
     def get_scalar(target_type: type, key_in_property_dict: str, default: Optional[Any] = None) -> Any:
         # return scalar value from `property_dict`, check that it is a scalar and cast to the desired type.
         default = None if default is None else [default]
         pd: List[str] = property_dict.get(key_in_property_dict, default)
@@ -52,15 +62,16 @@
     fields: List[str] = property_dict['FIELDS']
     dtypes: List[np.dtype] = [np.dtype(f'{t.lower()}{sizes[i]}') for i, t in enumerate(types)]
     if width * height != points:
         raise ValueError('The number of points in the PCD file does not match width * height. '
                          'Error deconding Point Cloud.')
     times.append(('read header       ', time.time()))
 
-    return read_point_cloud_data(data, is_binary=is_binary, width=width, height=height, sizes=sizes, dtypes=dtypes,
+    return read_point_cloud_data(data, is_binary=is_binary, is_compressed_lzma=is_compressed_lzma,
+                                 width=width, height=height, sizes=sizes, dtypes=dtypes,
                                  fields=fields, times=times), dict(viewpoint=viewpoint)
 
 
 def load_ply(data: bytes, width: int, height: int) -> Tuple[np.ndarray, Dict[str, Any]]:
     """
     :brief: Load the entire content of the PLY file accessible via `filename` to the `item`.
             Retain types and dimensions indicated in PCD file.
@@ -68,14 +79,15 @@
     times: List[Tuple[str, float]] = [('', time.time())]
 
     # Read header
     dtypes: List[np.dtype] = []
     sizes: List[int] = []
     fields: List[str] = []
     is_binary: bool = False
+    is_compressed_lzma: bool = False
 
     while True:
         line, data = read_line(data)
         current_line: List[str] = line.decode('utf-8')[:-1].split(' ')
         if len(current_line):
             if current_line[0] == 'property':
                 dtype_str, lookup_name = current_line[1:]
@@ -83,38 +95,44 @@
 
                 fields.append(lookup_name)
                 dtypes.append(field_dtype)
                 sizes.append(field_dtype.itemsize)
 
             elif current_line[0] == 'format':
                 is_binary = current_line[1] != 'ascii'
+                is_compressed_lzma = 'binary_compressed_lzma'
 
             elif current_line[0] == 'end_header':
                 break
     times.append(('read header       ', time.time()))
 
     # Read data payload
-    return read_point_cloud_data(data, is_binary=is_binary, width=width, height=height, sizes=sizes, dtypes=dtypes,
+    return read_point_cloud_data(data, is_binary=is_binary, is_compressed_lzma=is_compressed_lzma,
+                                 width=width, height=height, sizes=sizes, dtypes=dtypes,
                                  fields=fields, times=times), dict()
 
 
-def read_point_cloud_data(data: bytes, is_binary: bool, width: int, height, sizes: List[int], dtypes: List[np.dtype],
+def read_point_cloud_data(data: bytes, is_binary: bool, is_compressed_lzma: bool,
+                          width: int, height, sizes: List[int], dtypes: List[np.dtype],
                           fields: List[str], times) -> np.ndarray:
     npa: np.ndarray
 
     if is_binary:
         required_bytes: int = width * height * sum(sizes)
 
+        # Compose structured numpy array from arrays and target dtypes.
+        if is_compressed_lzma:
+            data = lzma.decompress(data)
+
         # Read data payload bytes
         if len(data) < required_bytes:
             missing_bytes: int = required_bytes - len(data)
             logger.warning(f'Reading corrupted Point Cloud File! Padding {missing_bytes} bytes with zeros.')
             data += bytes([0, ] * missing_bytes)
 
-        # Compose structured numpy array from arrays and target dtypes.
         npa = np.frombuffer(data, dtype=[(fields[i], dt) for i, dt in enumerate(dtypes)])
 
     else:
         lines = map(bytes.strip, read_lines(data))
 
         # lines = map(lambda a: a.decode('ASCII'), map(bytes.strip, file_handle.readlines())) # slows down proc.
         # npa = np.genfromtxt(lines, delimiter=' ', dtype=[(str(i), dt) for i, dt in enumerate(dtypes)]) # slow AF
```

### Comparing `dataspree-platform-sdk-1.9.5/dataspree/platform_sdk/http_token_authentication.py` & `dataspree-platform-sdk-1.9.6/dataspree/platform_sdk/http_token_authentication.py`

 * *Files identical despite different names*

### Comparing `dataspree-platform-sdk-1.9.5/dataspree/platform_sdk/query.py` & `dataspree-platform-sdk-1.9.6/dataspree/platform_sdk/query.py`

 * *Files identical despite different names*

### Comparing `dataspree-platform-sdk-1.9.5/dataspree/platform_sdk/worker.py` & `dataspree-platform-sdk-1.9.6/dataspree/platform_sdk/worker.py`

 * *Files identical despite different names*

### Comparing `dataspree-platform-sdk-1.9.5/dataspree_platform_sdk.egg-info/PKG-INFO` & `dataspree-platform-sdk-1.9.6/dataspree_platform_sdk.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,81 +1,81 @@
 Metadata-Version: 2.1
 Name: dataspree-platform-sdk
-Version: 1.9.5
+Version: 1.9.6
 Summary: Python SDK Data Spree AI Platform
 Home-page: https://data-spree.com/ai
 Author: Data Spree GmbH
 Author-email: info@data-spree.com
 License: Apache-2.0
+Description: # Data Spree AI Platform SDK
+        The Platform SDK acts as an interface to the Data Spree AI Platform, contains all classes and functions to integrate
+        custom models into the platform, and it provides a command-line tool for importing datasets of the following formats:
+        * Data Spree
+        * KITTI
+        * COCO
+        
+        Furthermore, it is possible to export datasets from the platform.
+        
+        ## Usage
+        
+        ### General Usage
+        ```
+        Usage: ds [OPTIONS] COMMAND [ARGS]...
+        
+        Options:
+          --help  Show this message and exit.
+        
+        Commands:
+          export
+          import
+        ```
+        
+        ### Dataset Import
+        ```
+        Usage: ds import [OPTIONS]
+        
+        Options:
+          --format [dataspree|kitti|coco]  Dataset format to import
+          --dataset_name TEXT         Name of the newly created dataset.
+          --dataset_id INTEGER        ID of the dataset to which new items should be
+                                      imported. If set to '-1', a new dataset will be
+                                      created
+          --images PATH               Directory containing the images to import.
+                                      [required]
+          --annotations PATH          Directory or file containing the annotations to
+                                      import.  [required]
+          --http_retries INTEGER      Number of HTTP retries.  [default: 10]
+          --username TEXT             Username for data spree vision platform.
+          --password TEXT             Password for data spree vision platform.
+          --url TEXT                  URL to the API of the platform.
+          --help                      Show this message and exit.
+        ```
+        
+        ### Dataset Export
+        ```
+        Usage: ds export [OPTIONS]
+        
+        Options:
+          -o, --output_dir DIRECTORY   Output directory.  [required]
+          -i, --id INTEGER             ID of the dataset to download.
+          -n, --n_items INTEGER        Number of items to download. Download all
+                                       items: '-1'  [default: -1]
+          --http_retries INTEGER       Number of HTTP retries.  [default: 10]
+          --parallel_requests INTEGER  Number of parallel requests.  [default: 16]
+          --username TEXT              Username for data spree vision platform.
+          --password TEXT              Password for data spree vision platform.
+          --url TEXT                   URL to the API of the platform.
+          --help                       Show this message and exit.
+        ```
+        
+        ## License
+        Apache License 2.0
+        
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: kitti
 Provides-Extra: worker
 Provides-Extra: build
-License-File: LICENSE
-
-# Data Spree AI Platform SDK
-The Platform SDK acts as an interface to the Data Spree AI Platform, contains all classes and functions to integrate
-custom models into the platform, and it provides a command-line tool for importing datasets of the following formats:
-* Data Spree
-* KITTI
-* COCO
-
-Furthermore, it is possible to export datasets from the platform.
-
-## Usage
-
-### General Usage
-```
-Usage: ds [OPTIONS] COMMAND [ARGS]...
-
-Options:
-  --help  Show this message and exit.
-
-Commands:
-  export
-  import
-```
-
-### Dataset Import
-```
-Usage: ds import [OPTIONS]
-
-Options:
-  --format [dataspree|kitti|coco]  Dataset format to import
-  --dataset_name TEXT         Name of the newly created dataset.
-  --dataset_id INTEGER        ID of the dataset to which new items should be
-                              imported. If set to '-1', a new dataset will be
-                              created
-  --images PATH               Directory containing the images to import.
-                              [required]
-  --annotations PATH          Directory or file containing the annotations to
-                              import.  [required]
-  --http_retries INTEGER      Number of HTTP retries.  [default: 10]
-  --username TEXT             Username for data spree vision platform.
-  --password TEXT             Password for data spree vision platform.
-  --url TEXT                  URL to the API of the platform.
-  --help                      Show this message and exit.
-```
-
-### Dataset Export
-```
-Usage: ds export [OPTIONS]
-
-Options:
-  -o, --output_dir DIRECTORY   Output directory.  [required]
-  -i, --id INTEGER             ID of the dataset to download.
-  -n, --n_items INTEGER        Number of items to download. Download all
-                               items: '-1'  [default: -1]
-  --http_retries INTEGER       Number of HTTP retries.  [default: 10]
-  --parallel_requests INTEGER  Number of parallel requests.  [default: 16]
-  --username TEXT              Username for data spree vision platform.
-  --password TEXT              Password for data spree vision platform.
-  --url TEXT                   URL to the API of the platform.
-  --help                       Show this message and exit.
-```
-
-## License
-Apache License 2.0
```

### Comparing `dataspree-platform-sdk-1.9.5/dataspree_platform_sdk.egg-info/SOURCES.txt` & `dataspree-platform-sdk-1.9.6/dataspree_platform_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dataspree-platform-sdk-1.9.5/setup.py` & `dataspree-platform-sdk-1.9.6/setup.py`

 * *Files identical despite different names*

### Comparing `dataspree-platform-sdk-1.9.5/tests/test_upload.py` & `dataspree-platform-sdk-1.9.6/tests/test_upload.py`

 * *Files identical despite different names*

