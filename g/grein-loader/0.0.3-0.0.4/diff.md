# Comparing `tmp/grein_loader-0.0.3.tar.gz` & `tmp/grein_loader-0.0.4.tar.gz`

## Comparing `grein_loader-0.0.3.tar` & `grein_loader-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 grein_loader-0.0.3/requirements.txt
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 grein_loader-0.0.3/.github/workflows/deploy.yaml
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 grein_loader-0.0.3/.github/workflows/test.yaml
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 grein_loader-0.0.3/src/grein_loader/__init__.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 grein_loader-0.0.3/src/grein_loader/exceptions.py
--rw-r--r--   0        0        0    13121 2020-02-02 00:00:00.000000 grein_loader-0.0.3/src/grein_loader/load_dataset.py
--rwxr-xr-x   0        0        0     5598 2020-02-02 00:00:00.000000 grein_loader-0.0.3/src/grein_loader/load_overview.py
--rw-r--r--   0        0        0    25199 2020-02-02 00:00:00.000000 grein_loader-0.0.3/src/grein_loader/utils.py
--rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 grein_loader-0.0.3/tests/test_dataset.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 grein_loader-0.0.3/.gitignore
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 grein_loader-0.0.3/LICENSE
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 grein_loader-0.0.3/README.md
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 grein_loader-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 grein_loader-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 grein_loader-0.0.4/requirements.txt
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 grein_loader-0.0.4/.github/workflows/deploy.yaml
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 grein_loader-0.0.4/.github/workflows/test.yaml
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 grein_loader-0.0.4/src/grein_loader/__init__.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 grein_loader-0.0.4/src/grein_loader/exceptions.py
+-rw-r--r--   0        0        0    14301 2020-02-02 00:00:00.000000 grein_loader-0.0.4/src/grein_loader/load_dataset.py
+-rwxr-xr-x   0        0        0     5598 2020-02-02 00:00:00.000000 grein_loader-0.0.4/src/grein_loader/load_overview.py
+-rw-r--r--   0        0        0    25349 2020-02-02 00:00:00.000000 grein_loader-0.0.4/src/grein_loader/utils.py
+-rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 grein_loader-0.0.4/tests/test_dataset.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 grein_loader-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 grein_loader-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 grein_loader-0.0.4/README.md
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 grein_loader-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 grein_loader-0.0.4/PKG-INFO
```

### Comparing `grein_loader-0.0.3/.github/workflows/deploy.yaml` & `grein_loader-0.0.4/.github/workflows/deploy.yaml`

 * *Files identical despite different names*

### Comparing `grein_loader-0.0.3/.github/workflows/test.yaml` & `grein_loader-0.0.4/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `grein_loader-0.0.3/src/grein_loader/load_dataset.py` & `grein_loader-0.0.4/src/grein_loader/load_dataset.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,21 +15,25 @@
 from typing import Tuple
 from .exceptions import GreinLoaderException
 from . import utils
 
 LOGGER = logging.getLogger(__name__)
 
 
-def load_dataset(gse_id: str) -> Tuple[dict, dict, pandas.DataFrame]:
+def load_dataset(gse_id: str, download_type: str="RAW") -> Tuple[dict, dict, pandas.DataFrame]:
     """ Loads a dataset from GREIN.
-        :param: gse_id: The dataset's GSE id.
+        :param: gse_id: The dataset's GSE id, download_type: The type of data to download for expression value, either RAW or NORMALIZED
         :type: gse_id: str
         :return: description, metadata, count_matrix of the GREIN dataset
         :rtype: description:dict, metadata:dictionary, count_matrix:pandas dataframe
     """
+    if download_type != "RAW" and download_type != "NORMALIZED":
+        LOGGER.error("Invalid download_type passed. Value must either by 'RAW' or 'NORMALIZED'.")
+        raise ValueError("Invalid download_type passed. Value must either by 'RAW' or 'NORMALIZED'.")
+
     payloads = utils.GreinLoaderUtils(gse_id)
     # create the unique random string used later for nonce parameter in url
     n = utils.GreinLoaderUtils.get_random_url_string_parameter()
 
     # xhr_streaming_url will always be used for streaming requests in the code
     xhr_streaming_url = f"http://www.ilincs.org/apps/grein/__sockjs__/n={n}/xhr_streaming"
 
@@ -51,29 +55,31 @@
 
     # streaming request is necessary for connection parameters
     try:
         xhr_streaming_r = s.post(xhr_streaming_url, stream=True)
         lines = xhr_streaming_r.iter_lines()  # saves information provided by the streaming response
         xhr_streaming_r.raise_for_status()
     except requests.exceptions.HTTPError as err:
-        LOGGER.error("Streaming error: ", err)
+        LOGGER.error("Streaming error: ", str(err))
+        LOGGER.exception(err)
         raise GreinLoaderException("Streaming error: ", err)
 
     for line in lines:  # decodes content of provided by the streaming request
         line_content = line.decode()
         if ("hhhhhhhhhh" in line_content):  # streaming content for the request is done and the connection initialized
             LOGGER.debug("Connection initialized")
             break
 
     # streaming request for configs and sessionId
     try:
         xhr_send_r = s.post(xhr_send_url, data='["0#0|o|"]')
         xhr_send_r.raise_for_status()
     except requests.exceptions.HTTPError as err:
-        LOGGER.error("Streaming error: ", err)
+        LOGGER.error("Streaming error: ", str(err))
+        LOGGER.exception(err)
         raise GreinLoaderException("Streaming error: ", err)
 
     config = None
     ACK_flag = False
     for line in lines:
         line_content = line.decode()
         if line_content.startswith('a["0#0|m|'):  # search for config parameter to parse sessionId
@@ -92,47 +98,51 @@
 
     # streaming parameters of GREIN ui init for data set with gse_id
     try:
         xhr_send_summary_r = s.post(xhr_send_url,
                                     data=payloads.ui_init_parameter())  # data needs the gse_id in the payload str
         xhr_send_summary_r.raise_for_status()
     except requests.exceptions.HTTPError as err:
-        LOGGER.error("Streaming error with: ", err)
+        LOGGER.error("Streaming error with: ", str(err))
+        LOGGER.exception(err)
         raise GreinLoaderException("Streaming error: ", err)
 
     for line in lines:
         line_content = line.decode()  # decode content from GREIN
 
     LOGGER.debug("Opening new connection")
     try:
         xhr_streaming_r = s.post(xhr_streaming_url, stream=True)
         lines = xhr_streaming_r.iter_lines()
         xhr_streaming_r.raise_for_status()
     except requests.exceptions.HTTPError as err:
-        LOGGER.error("Streaming error with: ", err)
+        LOGGER.error("Streaming error with: ", str(err))
+        LOGGER.exception(err)
         raise GreinLoaderException("Streaming error: ", err)
 
     try:
         LOGGER.debug("Streaming parameter")
         xhr_send_r = s.post(xhr_send_url,
                             data=payloads.method_update_parameter())  # sets initial parameters for the dataset
     except requests.exceptions.HTTPError as err:
-        LOGGER.error("Streaming error with: ", err)
+        LOGGER.error("Streaming error with: ", str(err))
+        LOGGER.exception(err)
         raise GreinLoaderException("Streaming error: ", err)
 
     for line in lines:
         line_content = line.decode()
         if "ACK" in line_content:
             break
 
     try:
         LOGGER.debug("Streaming client parameter")
         xhr_send_r = s.post(xhr_send_url, data=payloads.client_parameter())  # sets client parameter for dataset
     except requests.exceptions.HTTPError as err:
-        LOGGER.error("Streaming error with: ", err)
+        LOGGER.error("Streaming error with: ", str(err))
+        LOGGER.exception(err)
         raise GreinLoaderException("Streaming error: ", err)
 
     try:
         LOGGER.debug("Streaming dataset")
         s.post(xhr_send_url, payloads.stream_dataset_parameter())  # sets parameter for streaming
     except requests.exceptions.HTTPError as err:
         LOGGER.error("Streaming error")
@@ -153,25 +163,27 @@
             f"http://www.ilincs.org/apps/grein/session/{session_id}/dataobj/geo_summary?w=&nonce={random_str}",
             headers={
                 "Content-Type": "application/x-www-form-urlencoded; charset=UTF-8",
                 "Accept": "application/json, text/javascript, */*; q=0.01",
                 "Origin": "http://www.ilincs.org",
                 "Referer": "http://www.ilincs.org/apps/grein/?gse=" + gse_id
             },
-            data=payloads.description_formdata(100))
+            data=payloads.description_formdata(100))  # Bruh wtf moment ??? 
         description_r.raise_for_status()
     except requests.exceptions.HTTPError as err:
-        LOGGER.error(f"Dataset description for {gse_id} not received: ", err)
+        LOGGER.error(f"Dataset description for {gse_id} not received")
+        LOGGER.exception(err)
         raise GreinLoaderException(f"Dataset description for {gse_id} not received: ", err)
 
     # request necessary for the metadata labels, provided in the ui via streaming
     try:
         metadata_labels_r = s.post(xhr_send_url, data=payloads.metadata_labels_parameter())
     except requests.exceptions.HTTPError as err:
-        LOGGER.error(f"Metadata labels for {gse_id} not received: ", err)
+        LOGGER.error(f"Metadata labels for {gse_id} not received.")
+        LOGGER.exception(err)
         raise GreinLoaderException(f"Metadata labels for {gse_id} not received: ", err)
 
     ui_content = []
     for line in lines:  # the streaming request provides elements elements from the ui
         line_content = line.decode()
         ui_content.append(line_content)
         if "ACK" in line_content:
@@ -194,34 +206,45 @@
             headers={
                 "Content-Type": "application/x-www-form-urlencoded; charset=UTF-8",
                 "Accept": "application/json, text/javascript, */*; q=0.01",
                 "Origin": "http://www.ilincs.org",
                 "Referer": "http://www.ilincs.org/apps/grein/?gse=" + gse_id
             }, data=metadata_formdata)
     except requests.exceptions.HTTPError as err:
-        LOGGER.error(f"Metadata for {gse_id} not received: ", err)
+        LOGGER.error(f"Metadata for {gse_id} not received.")
+        LOGGER.exception(err)
         raise GreinLoaderException(f"Metadata for {gse_id} not received: ", err)
 
     # method update for count_matrix
     try:
         xhr_send_r = s.post(xhr_send_url, data=payloads.count_matrix_parameter())
     except requests.exceptions.HTTPError as err:
-        LOGGER.error("Streaming error", err)
+        LOGGER.error("Streaming error")
+        LOGGER.exception(err)
         raise GreinLoaderException("Streaming error: ", err)
 
     for line in lines:
         line_content = line.decode()
         if "ACK" in line_content:
             break
+    
+    # in case method parameter is set to normalized, different request is send
+    if download_type == "NORMALIZED":
+        try: 
+            xhr_send_r = s.post(xhr_send_url, data=payloads.count_matrix_normalized())
+        except requests.exceptions.HTTPError as err:
+            LOGGER.error("Streaming error for normailzed count matrix", err)
+            raise GreinLoaderException("Streaming error for normailzed count matrix", err)
 
     # requesting count matrix
     try:
         count_matrix_r = s.post(f"http://www.ilincs.org/apps/grein/session/{session_id}/download/downloadcounts?w=")
     except requests.exceptions.HTTPError as err:
-        LOGGER.error(f"Count Matrix for {gse_id} not received ", err)
+        LOGGER.error(f"Count Matrix for {gse_id} not received")
+        LOGGER.exception(err)
         raise GreinLoaderException(f"Count Matrix for {gse_id} not received: ", err)
 
     LOGGER.debug("Count matrix received")
 
     # Before returning description, metadata and count_matrix is formatted,
     # before formatting all content from the requests must be decoded
 
@@ -319,8 +342,7 @@
     raw_form = raw_utils.raw_form_start()
     n = 1
     while n < n_columns-5:
         raw_form += raw_utils.raw_form_column(n)
         n = n+1
     raw_form += raw_utils.raw_form_end(no_samples)
     return raw_form
-
```

### Comparing `grein_loader-0.0.3/src/grein_loader/load_overview.py` & `grein_loader-0.0.4/src/grein_loader/load_overview.py`

 * *Files identical despite different names*

### Comparing `grein_loader-0.0.3/src/grein_loader/utils.py` & `grein_loader-0.0.4/src/grein_loader/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,17 @@
 
     def metadata_labels_parameter(self):
         return '["B#0|m|{\\"method\\":\\"update\\",\\"data\\":{\\"tab2\\":\\"metadata\\",\\".clientdata_output_geo_summary_hidden\\":true,\\".clientdata_output_metadata_hidden\\":false,\\".clientdata_output_metadata_full_hidden\\":false,\\".clientdata_output_ontology_hidden\\":false}}"]'
 
     def count_matrix_parameter(self):
         return '["18#0|m|{\\"method\\":\\"update\\",\\"data\\":{\\"counts_rows_selected\\":[],\\"counts_rows_current\\":[],\\"counts_rows_all\\":[],\\"counts_state\\":null,\\"counts_search\\":\\"\\",\\"counts_cell_clicked\\":{},\\".clientdata_output_downloadcounts_hidden\\":false}}"]'
 
+    def count_matrix_normalized(self):
+        return '["19#0|m|{\\"method\\":\\"update\\",\\"data\\":{\\"counts_choice\\":\\"Normalized\\"}}"]'
+    
     def raw_form_start(self):
         return "draw=1&columns%5B0%5D%5Bdata%5D=0&columns%5B0%5D%5Bname%5D=&columns%5B0%5D%5Bsearchable%5D=true&columns%5B0%5D%5Borderable%5D=false&columns%5B0%5D%5Bsearch%5D%5Bvalue%5D=&columns%5B0%5D%5Bsearch%5D%5Bregex%5D=false"
 
     def raw_form_end(self, no_samples = 100):
         return f"start=0&length={no_samples}&search%5Bvalue%5D=&search%5Bregex%5D=false&search%5BcaseInsensitive%5D=true&search%5Bsmart%5D=true&escape=true"
 
     def raw_form_column(self, n):
```

### Comparing `grein_loader-0.0.3/tests/test_dataset.py` & `grein_loader-0.0.4/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `grein_loader-0.0.3/LICENSE` & `grein_loader-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `grein_loader-0.0.3/README.md` & `grein_loader-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `grein_loader-0.0.3/pyproject.toml` & `grein_loader-0.0.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "hatch-requirements-txt"]
 build-backend = "hatchling.build"
 
 [project]
 name = "grein_loader"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   {name="Griss Lab", email="johannes.griss@meduniwien.ac.at"},
   {name="Alexander Grentner", email="alexander.grentner@meduniwien.ac.at"}
 ]
 description = "Package for loading datasets from GREIN"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `grein_loader-0.0.3/PKG-INFO` & `grein_loader-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: grein_loader
-Version: 0.0.3
+Version: 0.0.4
 Summary: Package for loading datasets from GREIN
 Project-URL: Homepage, https://github.com/grisslab/grein_loader
 Project-URL: Bug Tracker, https://github.com/grisslab/grein_loader/issues
 Author-email: Griss Lab <johannes.griss@meduniwien.ac.at>, Alexander Grentner <alexander.grentner@meduniwien.ac.at>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

