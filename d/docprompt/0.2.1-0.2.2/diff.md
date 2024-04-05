# Comparing `tmp/docprompt-0.2.1.tar.gz` & `tmp/docprompt-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docprompt-0.2.1.tar", max compression
+gzip compressed data, was "docprompt-0.2.2.tar", max compression
```

## Comparing `docprompt-0.2.1.tar` & `docprompt-0.2.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0      585 2023-10-19 02:11:11.194822 docprompt-0.2.1/LICENSE
--rw-r--r--   0        0        0     4917 2024-03-19 03:22:18.145677 docprompt-0.2.1/README.md
--rw-r--r--   0        0        0      593 2024-03-21 01:44:38.876965 docprompt-0.2.1/docprompt/__init__.py
--rw-r--r--   0        0        0        0 2024-03-18 16:11:05.761315 docprompt-0.2.1/docprompt/_exec/__init__.py
--rw-r--r--   0        0        0     2395 2024-03-19 02:54:19.707704 docprompt-0.2.1/docprompt/_exec/ghostscript.py
--rw-r--r--   0        0        0        0 2024-03-18 23:40:35.967506 docprompt-0.2.1/docprompt/provenance/__init__.py
--rw-r--r--   0        0        0     9850 2024-03-19 01:27:56.655646 docprompt-0.2.1/docprompt/provenance/search.py
--rw-r--r--   0        0        0     1357 2024-03-19 01:25:52.543395 docprompt-0.2.1/docprompt/provenance/source.py
--rw-r--r--   0        0        0     6054 2024-03-19 01:25:52.543395 docprompt-0.2.1/docprompt/provenance/util.py
--rw-r--r--   0        0        0        0 2024-01-07 23:02:33.076362 docprompt-0.2.1/docprompt/schema/__init__.py
--rw-r--r--   0        0        0     8355 2024-03-18 16:11:18.725305 docprompt-0.2.1/docprompt/schema/document.py
--rw-r--r--   0        0        0     6356 2024-03-14 22:46:13.968446 docprompt-0.2.1/docprompt/schema/layout.py
--rw-r--r--   0        0        0     3758 2024-03-19 01:25:52.543395 docprompt-0.2.1/docprompt/schema/pipeline.py
--rw-r--r--   0        0        0        0 2024-03-12 20:38:52.149979 docprompt-0.2.1/docprompt/tasks/__init__.py
--rw-r--r--   0        0        0     5097 2024-03-17 22:06:10.239019 docprompt-0.2.1/docprompt/tasks/base.py
--rw-r--r--   0        0        0        0 2024-03-12 20:43:10.168189 docprompt-0.2.1/docprompt/tasks/classification/__init__.py
--rw-r--r--   0        0        0     2516 2024-03-17 22:03:09.947425 docprompt-0.2.1/docprompt/tasks/message.py
--rw-r--r--   0        0        0        0 2024-03-14 22:11:01.166853 docprompt-0.2.1/docprompt/tasks/ocr/__init__.py
--rw-r--r--   0        0        0    18321 2024-03-17 05:05:54.360075 docprompt-0.2.1/docprompt/tasks/ocr/gcp.py
--rw-r--r--   0        0        0     1164 2024-03-19 01:25:52.543395 docprompt-0.2.1/docprompt/tasks/ocr/result.py
--rw-r--r--   0        0        0        0 2024-03-17 06:03:50.676445 docprompt-0.2.1/docprompt/tasks/table_extraction/__init__.py
--rw-r--r--   0        0        0      722 2024-03-17 22:04:31.923231 docprompt-0.2.1/docprompt/tasks/table_extraction/base.py
--rw-r--r--   0        0        0        0 2024-03-17 06:15:55.636068 docprompt-0.2.1/docprompt/tasks/table_extraction/providers/__init__.py
--rw-r--r--   0        0        0     3392 2024-03-18 16:00:17.433830 docprompt-0.2.1/docprompt/tasks/table_extraction/providers/claude.py
--rw-r--r--   0        0        0      777 2024-03-17 22:03:09.947425 docprompt-0.2.1/docprompt/tasks/table_extraction/result.py
--rw-r--r--   0        0        0      351 2024-03-14 21:45:48.927780 docprompt-0.2.1/docprompt/utils/__init__.py
--rw-r--r--   0        0        0      421 2023-10-19 04:28:21.331934 docprompt-0.2.1/docprompt/utils/compressor.py
--rw-r--r--   0        0        0     4884 2024-03-14 22:46:13.968446 docprompt-0.2.1/docprompt/utils/date_extraction.py
--rw-r--r--   0        0        0        0 2024-03-18 15:46:16.978297 docprompt-0.2.1/docprompt/utils/raster.py
--rw-r--r--   0        0        0     3417 2024-03-18 15:40:58.846295 docprompt-0.2.1/docprompt/utils/splitter.py
--rw-r--r--   0        0        0     3947 2024-03-18 16:00:17.433830 docprompt-0.2.1/docprompt/utils/util.py
--rw-r--r--   0        0        0     3643 2024-03-21 01:45:15.221149 docprompt-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       39 2023-10-19 02:11:11.222822 docprompt-0.2.1/tests/__init__.py
--rw-r--r--   0        0        0   123638 2024-03-18 16:06:46.485527 docprompt-0.2.1/tests/fixtures/1.pdf
--rw-r--r--   0        0        0  2788655 2024-03-19 01:25:52.543395 docprompt-0.2.1/tests/fixtures/1_ocr.json
--rw-r--r--   0        0        0      202 2024-03-19 01:25:52.543395 docprompt-0.2.1/tests/fixtures.py
--rw-r--r--   0        0        0      830 2024-03-19 02:48:57.067976 docprompt-0.2.1/tests/test_date_extraction.py
--rw-r--r--   0        0        0      971 2024-03-19 02:48:57.067976 docprompt-0.2.1/tests/test_document.py
--rw-r--r--   0        0        0      941 2024-03-19 01:25:52.547395 docprompt-0.2.1/tests/test_search.py
--rw-r--r--   0        0        0     1003 2024-03-19 01:25:52.547395 docprompt-0.2.1/tests/util.py
--rw-r--r--   0        0        0     7794 1970-01-01 00:00:00.000000 docprompt-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      585 2023-10-19 02:11:11.194822 docprompt-0.2.2/LICENSE
+-rw-r--r--   0        0        0     4917 2024-03-19 03:22:18.145677 docprompt-0.2.2/README.md
+-rw-r--r--   0        0        0      593 2024-03-21 01:44:38.876965 docprompt-0.2.2/docprompt/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-18 16:11:05.761315 docprompt-0.2.2/docprompt/_exec/__init__.py
+-rw-r--r--   0        0        0     2395 2024-03-19 02:54:19.707704 docprompt-0.2.2/docprompt/_exec/ghostscript.py
+-rw-r--r--   0        0        0        0 2024-03-18 23:40:35.967506 docprompt-0.2.2/docprompt/provenance/__init__.py
+-rw-r--r--   0        0        0     9850 2024-03-19 01:27:56.655646 docprompt-0.2.2/docprompt/provenance/search.py
+-rw-r--r--   0        0        0     1357 2024-03-19 01:25:52.543395 docprompt-0.2.2/docprompt/provenance/source.py
+-rw-r--r--   0        0        0     6054 2024-03-19 01:25:52.543395 docprompt-0.2.2/docprompt/provenance/util.py
+-rw-r--r--   0        0        0        0 2024-01-07 23:02:33.076362 docprompt-0.2.2/docprompt/schema/__init__.py
+-rw-r--r--   0        0        0     8355 2024-03-18 16:11:18.725305 docprompt-0.2.2/docprompt/schema/document.py
+-rw-r--r--   0        0        0     6356 2024-03-14 22:46:13.968446 docprompt-0.2.2/docprompt/schema/layout.py
+-rw-r--r--   0        0        0     3758 2024-03-19 01:25:52.543395 docprompt-0.2.2/docprompt/schema/pipeline.py
+-rw-r--r--   0        0        0        0 2024-03-12 20:38:52.149979 docprompt-0.2.2/docprompt/tasks/__init__.py
+-rw-r--r--   0        0        0     5097 2024-03-17 22:06:10.239019 docprompt-0.2.2/docprompt/tasks/base.py
+-rw-r--r--   0        0        0        0 2024-03-12 20:43:10.168189 docprompt-0.2.2/docprompt/tasks/classification/__init__.py
+-rw-r--r--   0        0        0     2516 2024-03-17 22:03:09.947425 docprompt-0.2.2/docprompt/tasks/message.py
+-rw-r--r--   0        0        0        0 2024-03-14 22:11:01.166853 docprompt-0.2.2/docprompt/tasks/ocr/__init__.py
+-rw-r--r--   0        0        0    18321 2024-03-17 05:05:54.360075 docprompt-0.2.2/docprompt/tasks/ocr/gcp.py
+-rw-r--r--   0        0        0     1164 2024-03-19 01:25:52.543395 docprompt-0.2.2/docprompt/tasks/ocr/result.py
+-rw-r--r--   0        0        0        0 2024-03-17 06:03:50.676445 docprompt-0.2.2/docprompt/tasks/table_extraction/__init__.py
+-rw-r--r--   0        0        0      722 2024-03-17 22:04:31.923231 docprompt-0.2.2/docprompt/tasks/table_extraction/base.py
+-rw-r--r--   0        0        0        0 2024-03-17 06:15:55.636068 docprompt-0.2.2/docprompt/tasks/table_extraction/providers/__init__.py
+-rw-r--r--   0        0        0     3392 2024-03-18 16:00:17.433830 docprompt-0.2.2/docprompt/tasks/table_extraction/providers/claude.py
+-rw-r--r--   0        0        0      777 2024-03-17 22:03:09.947425 docprompt-0.2.2/docprompt/tasks/table_extraction/result.py
+-rw-r--r--   0        0        0      351 2024-03-14 21:45:48.927780 docprompt-0.2.2/docprompt/utils/__init__.py
+-rw-r--r--   0        0        0      421 2023-10-19 04:28:21.331934 docprompt-0.2.2/docprompt/utils/compressor.py
+-rw-r--r--   0        0        0     4884 2024-03-14 22:46:13.968446 docprompt-0.2.2/docprompt/utils/date_extraction.py
+-rw-r--r--   0        0        0        0 2024-03-18 15:46:16.978297 docprompt-0.2.2/docprompt/utils/raster.py
+-rw-r--r--   0        0        0     3655 2024-04-05 21:23:49.921077 docprompt-0.2.2/docprompt/utils/splitter.py
+-rw-r--r--   0        0        0     3947 2024-04-05 20:16:08.417755 docprompt-0.2.2/docprompt/utils/util.py
+-rw-r--r--   0        0        0     3643 2024-04-05 21:23:37.448987 docprompt-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0       39 2023-10-19 02:11:11.222822 docprompt-0.2.2/tests/__init__.py
+-rw-r--r--   0        0        0   123638 2024-03-18 16:06:46.485527 docprompt-0.2.2/tests/fixtures/1.pdf
+-rw-r--r--   0        0        0  2788655 2024-03-19 01:25:52.543395 docprompt-0.2.2/tests/fixtures/1_ocr.json
+-rw-r--r--   0        0        0      202 2024-03-19 01:25:52.543395 docprompt-0.2.2/tests/fixtures.py
+-rw-r--r--   0        0        0      830 2024-03-19 02:48:57.067976 docprompt-0.2.2/tests/test_date_extraction.py
+-rw-r--r--   0        0        0      971 2024-03-19 02:48:57.067976 docprompt-0.2.2/tests/test_document.py
+-rw-r--r--   0        0        0      941 2024-03-19 01:25:52.547395 docprompt-0.2.2/tests/test_search.py
+-rw-r--r--   0        0        0     1003 2024-03-19 01:25:52.547395 docprompt-0.2.2/tests/util.py
+-rw-r--r--   0        0        0     7743 1970-01-01 00:00:00.000000 docprompt-0.2.2/PKG-INFO
```

### Comparing `docprompt-0.2.1/LICENSE` & `docprompt-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.1/README.md` & `docprompt-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.1/docprompt/__init__.py` & `docprompt-0.2.2/docprompt/__init__.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.1/docprompt/_exec/ghostscript.py` & `docprompt-0.2.2/docprompt/_exec/ghostscript.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.1/docprompt/provenance/search.py` & `docprompt-0.2.2/docprompt/provenance/search.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.1/docprompt/provenance/source.py` & `docprompt-0.2.2/docprompt/provenance/source.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.1/docprompt/provenance/util.py` & `docprompt-0.2.2/docprompt/provenance/util.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.1/docprompt/schema/document.py` & `docprompt-0.2.2/docprompt/schema/document.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.1/docprompt/schema/layout.py` & `docprompt-0.2.2/docprompt/schema/layout.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.1/docprompt/schema/pipeline.py` & `docprompt-0.2.2/docprompt/schema/pipeline.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.1/docprompt/tasks/base.py` & `docprompt-0.2.2/docprompt/tasks/base.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.1/docprompt/tasks/message.py` & `docprompt-0.2.2/docprompt/tasks/message.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.1/docprompt/tasks/ocr/gcp.py` & `docprompt-0.2.2/docprompt/tasks/ocr/gcp.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.1/docprompt/tasks/ocr/result.py` & `docprompt-0.2.2/docprompt/tasks/ocr/result.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.1/docprompt/tasks/table_extraction/base.py` & `docprompt-0.2.2/docprompt/tasks/table_extraction/base.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.1/docprompt/tasks/table_extraction/providers/claude.py` & `docprompt-0.2.2/docprompt/tasks/table_extraction/providers/claude.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.1/docprompt/tasks/table_extraction/result.py` & `docprompt-0.2.2/docprompt/tasks/table_extraction/result.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.1/docprompt/utils/date_extraction.py` & `docprompt-0.2.2/docprompt/utils/date_extraction.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.1/docprompt/utils/splitter.py` & `docprompt-0.2.2/docprompt/utils/splitter.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,21 @@
 import tempfile
 from typing import Iterator, Optional
 
 import pypdfium2 as pdfium
 
 from docprompt._exec.ghostscript import compress_pdf_to_bytes
 from docprompt.utils import get_page_count
+from threading import Lock
+import time
 
 logger = logging.getLogger(__name__)
 
+PDFIUM_SPLIT_LOCK = Lock()
+
 
 class UnsupportedDocumentType(ValueError):
     pass
 
 
 def split_pdf_to_bytes(
     file_bytes: bytes,
@@ -51,38 +55,45 @@
 
 
 def pdf_split_iter_fast(file_bytes: bytes, max_page_count: int) -> Iterator[bytes]:
     """
     Splits a PDF into batches of pages up to `max_page_count` pages quickly.
     """
     # Load the PDF from bytes
-    src_pdf = pdfium.PdfDocument(io.BytesIO(file_bytes))
+    with PDFIUM_SPLIT_LOCK:
+        src_pdf = pdfium.PdfDocument(io.BytesIO(file_bytes))
+
+        current_page = 0
+        total_pages = len(src_pdf)
+
+        while current_page < total_pages:
+            # Determine the last page for the current batch
+            last_page = min(current_page + max_page_count, total_pages)
+
+            dst_pdf = pdfium.PdfDocument.new()
 
-    current_page = 0
-    total_pages = len(src_pdf)
+            # Append pages to the batch
+            dst_pdf.import_pages(src_pdf, list(range(current_page, last_page)))
 
-    while current_page < total_pages:
-        # Determine the last page for the current batch
-        last_page = min(current_page + max_page_count, total_pages)
+            # Save the batch PDF to a bytes buffer
+            pdf_bytes_buffer = io.BytesIO()
+            dst_pdf.save(pdf_bytes_buffer)
+            pdf_bytes_buffer.seek(0)  # Reset buffer pointer to the beginning
 
-        dst_pdf = pdfium.PdfDocument.new()
+            dst_pdf.close()
 
-        # Append pages to the batch
-        dst_pdf.import_pages(src_pdf, list(range(current_page, last_page)))
+            # Yield the bytes of the batch PDF
+            yield pdf_bytes_buffer.getvalue()
 
-        # Save the batch PDF to a bytes buffer
-        pdf_bytes_buffer = io.BytesIO()
-        dst_pdf.save(pdf_bytes_buffer)
-        pdf_bytes_buffer.seek(0)  # Reset buffer pointer to the beginning
+            # Update the current page for the next batch
+            current_page += max_page_count
 
-        # Yield the bytes of the batch PDF
-        yield pdf_bytes_buffer.getvalue()
+        src_pdf.close()
 
-        # Update the current page for the next batch
-        current_page += max_page_count
+    time.sleep(0.1)
 
 
 def pdf_split_iter_with_max_bytes(
     file_bytes: bytes, max_page_count: int, max_bytes: int
 ) -> Iterator[bytes]:
     """
     Splits a PDF into batches of pages up to `max_page_count` pages and `max_bytes` bytes.
```

### Comparing `docprompt-0.2.1/docprompt/utils/util.py` & `docprompt-0.2.2/docprompt/utils/util.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.1/pyproject.toml` & `docprompt-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "docprompt"
-version = "0.2.1"
+version = "0.2.2"
 homepage = "https://github.com/Page-Leaf/docprompt"
 description = "Documents and large language models."
 authors = ["Frankie Colson <frank@pageleaf.io>"]
 readme = "README.md"
 license =  "Apache-2.0"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
```

### Comparing `docprompt-0.2.1/tests/fixtures/1.pdf` & `docprompt-0.2.2/tests/fixtures/1.pdf`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.1/tests/fixtures/1_ocr.json` & `docprompt-0.2.2/tests/fixtures/1_ocr.json`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.1/tests/test_date_extraction.py` & `docprompt-0.2.2/tests/test_date_extraction.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.1/tests/test_document.py` & `docprompt-0.2.2/tests/test_document.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.1/tests/test_search.py` & `docprompt-0.2.2/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.1/tests/util.py` & `docprompt-0.2.2/tests/util.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.1/PKG-INFO` & `docprompt-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: docprompt
-Version: 0.2.1
+Version: 0.2.2
 Summary: Documents and large language models.
 Home-page: https://github.com/Page-Leaf/docprompt
 License: Apache-2.0
 Author: Frankie Colson
 Author-email: frank@pageleaf.io
 Requires-Python: >=3.9,<3.13
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.8
 Provides-Extra: azure
 Provides-Extra: dev
 Provides-Extra: doc
 Provides-Extra: google
 Provides-Extra: search
 Provides-Extra: test
```

#### html2text {}

```diff
@@ -1,43 +1,43 @@
-Metadata-Version: 2.1 Name: docprompt Version: 0.2.1 Summary: Documents and
+Metadata-Version: 2.1 Name: docprompt Version: 0.2.2 Summary: Documents and
 large language models. Home-page: https://github.com/Page-Leaf/docprompt
 License: Apache-2.0 Author: Frankie Colson Author-email: frank@pageleaf.io
 Requires-Python: >=3.9,<3.13 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Natural Language :: English Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: 3.12 Classifier: Programming Language :: Python :: 3.8 Provides-
-Extra: azure Provides-Extra: dev Provides-Extra: doc Provides-Extra: google
-Provides-Extra: search Provides-Extra: test Requires-Dist: azure-ai-
-formrecognizer (>=3.3.0) ; extra == "azure" Requires-Dist: bump2version
-(>=1.0.1,<2.0.0) ; extra == "dev" Requires-Dist: flake8 (>=6.1.0,<7.0.0) ;
-extra == "test" Requires-Dist: flake8-docstrings (>=1.7.0,<2.0.0) ; extra ==
-"test" Requires-Dist: fsspec (>=2023.10.0,<2024.0.0) Requires-Dist: google-
-cloud-documentai (>=2.20.0) ; extra == "google" Requires-Dist: isort
-(>=5.12.0,<6.0.0) ; extra == "test" Requires-Dist: mkdocs (>=1.1.2,<2.0.0) ;
-extra == "doc" Requires-Dist: mkdocs-autorefs (>=0.2.1,<0.3.0) ; extra == "doc"
-Requires-Dist: mkdocs-include-markdown-plugin (>=1.0.0,<2.0.0) ; extra == "doc"
-Requires-Dist: mkdocs-material (>=6.1.7,<7.0.0) ; extra == "doc" Requires-Dist:
-mkdocs-material-extensions (>=1.0.1,<2.0.0) Requires-Dist: mkdocstrings
-(>=0.15.2,<0.16.0) ; extra == "doc" Requires-Dist: mypy (>=1.6.1,<2.0.0) ;
-extra == "test" Requires-Dist: networkx (>=3.2.1,<4.0.0) ; extra == "search"
-Requires-Dist: numpy (>=1.26.1,<2.0.0) Requires-Dist: pillow (>=9.0.1)
-Requires-Dist: pip (>=20.3.1,<21.0.0) ; extra == "dev" Requires-Dist: pre-
-commit (>=2.12.0,<3.0.0) ; extra == "dev" Requires-Dist: pydantic (>=2.1.0)
-Requires-Dist: pypdf (>=3.16.4,<4.0.0) Requires-Dist: pypdfium2
-(>=4.28.0,<5.0.0) Requires-Dist: pytest (>=7.4.2,<8.0.0) ; extra == "test"
-Requires-Dist: pytest-cov (>=4.1.0,<5.0.0) ; extra == "test" Requires-Dist:
-python-dateutil (>=2.8.2,<3.0.0) Requires-Dist: python-magic (>=0.4.24)
-Requires-Dist: rapidfuzz (>=3.6.2,<4.0.0) Requires-Dist: rtree (>=1.2.0,<2.0.0)
-; extra == "search" Requires-Dist: ruff (>=0.3.3,<0.4.0) ; extra == "test"
-Requires-Dist: tantivy (>=0.21.0,<0.22.0) ; extra == "search" Requires-Dist:
-tenacity (>=8.2.3,<9.0.0) Requires-Dist: toml (>=0.10.2,<0.11.0) ; extra ==
-"dev" Requires-Dist: tox (>=3.20.1,<4.0.0) ; extra == "dev" Requires-Dist: tqdm
+Python :: 3.8 Provides-Extra: azure Provides-Extra: dev Provides-Extra: doc
+Provides-Extra: google Provides-Extra: search Provides-Extra: test Requires-
+Dist: azure-ai-formrecognizer (>=3.3.0) ; extra == "azure" Requires-Dist:
+bump2version (>=1.0.1,<2.0.0) ; extra == "dev" Requires-Dist: flake8
+(>=6.1.0,<7.0.0) ; extra == "test" Requires-Dist: flake8-docstrings
+(>=1.7.0,<2.0.0) ; extra == "test" Requires-Dist: fsspec
+(>=2023.10.0,<2024.0.0) Requires-Dist: google-cloud-documentai (>=2.20.0) ;
+extra == "google" Requires-Dist: isort (>=5.12.0,<6.0.0) ; extra == "test"
+Requires-Dist: mkdocs (>=1.1.2,<2.0.0) ; extra == "doc" Requires-Dist: mkdocs-
+autorefs (>=0.2.1,<0.3.0) ; extra == "doc" Requires-Dist: mkdocs-include-
+markdown-plugin (>=1.0.0,<2.0.0) ; extra == "doc" Requires-Dist: mkdocs-
+material (>=6.1.7,<7.0.0) ; extra == "doc" Requires-Dist: mkdocs-material-
+extensions (>=1.0.1,<2.0.0) Requires-Dist: mkdocstrings (>=0.15.2,<0.16.0) ;
+extra == "doc" Requires-Dist: mypy (>=1.6.1,<2.0.0) ; extra == "test" Requires-
+Dist: networkx (>=3.2.1,<4.0.0) ; extra == "search" Requires-Dist: numpy
+(>=1.26.1,<2.0.0) Requires-Dist: pillow (>=9.0.1) Requires-Dist: pip
+(>=20.3.1,<21.0.0) ; extra == "dev" Requires-Dist: pre-commit (>=2.12.0,<3.0.0)
+; extra == "dev" Requires-Dist: pydantic (>=2.1.0) Requires-Dist: pypdf
+(>=3.16.4,<4.0.0) Requires-Dist: pypdfium2 (>=4.28.0,<5.0.0) Requires-Dist:
+pytest (>=7.4.2,<8.0.0) ; extra == "test" Requires-Dist: pytest-cov
+(>=4.1.0,<5.0.0) ; extra == "test" Requires-Dist: python-dateutil
+(>=2.8.2,<3.0.0) Requires-Dist: python-magic (>=0.4.24) Requires-Dist:
+rapidfuzz (>=3.6.2,<4.0.0) Requires-Dist: rtree (>=1.2.0,<2.0.0) ; extra ==
+"search" Requires-Dist: ruff (>=0.3.3,<0.4.0) ; extra == "test" Requires-Dist:
+tantivy (>=0.21.0,<0.22.0) ; extra == "search" Requires-Dist: tenacity
+(>=8.2.3,<9.0.0) Requires-Dist: toml (>=0.10.2,<0.11.0) ; extra == "dev"
+Requires-Dist: tox (>=3.20.1,<4.0.0) ; extra == "dev" Requires-Dist: tqdm
 (>=4.61.0) Requires-Dist: twine (>=3.3.0,<4.0.0) ; extra == "dev" Requires-
 Dist: virtualenv (>=20.2.2,<21.0.0) ; extra == "dev" Description-Content-Type:
 text/markdown [![pypi](https://img.shields.io/pypi/v/docprompt.svg)](https://
 pypi.org/project/docprompt/) [![python](https://img.shields.io/pypi/pyversions/
 docprompt.svg)](https://pypi.org/project/docprompt/) [![Build Status](https://
 github.com/Page-Leaf/Docprompt/actions/workflows/dev.yml/badge.svg)](https://
 github.com/Page-Leaf/docprompt/actions/workflows/dev.yml) [![codecov](https://
```

