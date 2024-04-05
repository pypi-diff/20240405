# Comparing `tmp/ofxReaderBR-0.9.0.tar.gz` & `tmp/ofxReaderBR-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ofxReaderBR-0.9.0.tar", last modified: Fri Jan 31 17:43:25 2020, max compression
+gzip compressed data, was "dist/ofxReaderBR-0.9.1.tar", last modified: Mon Feb  3 16:09:22 2020, max compression
```

## Comparing `ofxReaderBR-0.9.0.tar` & `ofxReaderBR-0.9.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 silvino   (1001) silvino   (1001)        0 2020-01-31 17:43:25.000000 ofxReaderBR-0.9.0/
--rw-r--r--   0 silvino   (1001) silvino   (1001)       39 2019-11-05 20:00:45.000000 ofxReaderBR-0.9.0/setup.cfg
-drwxrwxr-x   0 silvino   (1001) silvino   (1001)        0 2020-01-31 17:43:25.000000 ofxReaderBR-0.9.0/ofxReaderBR/
-drwxrwxr-x   0 silvino   (1001) silvino   (1001)        0 2020-01-31 17:43:25.000000 ofxReaderBR-0.9.0/ofxReaderBR/reader/
--rw-rw-r--   0 silvino   (1001) silvino   (1001)     2318 2020-01-31 17:42:22.000000 ofxReaderBR-0.9.0/ofxReaderBR/reader/readercontroller.py
-drwxrwxr-x   0 silvino   (1001) silvino   (1001)        0 2020-01-31 17:43:25.000000 ofxReaderBR-0.9.0/ofxReaderBR/reader/pdf/
--rw-rw-r--   0 silvino   (1001) silvino   (1001)     1372 2020-01-31 17:42:22.000000 ofxReaderBR-0.9.0/ofxReaderBR/reader/pdf/pdfParser.py
--rw-rw-r--   0 silvino   (1001) silvino   (1001)     6243 2019-12-23 20:31:31.000000 ofxReaderBR-0.9.0/ofxReaderBR/reader/pdf/PDFParserSantander.py
--rw-rw-r--   0 silvino   (1001) silvino   (1001)      525 2020-01-31 17:42:22.000000 ofxReaderBR-0.9.0/ofxReaderBR/reader/pdf/pdfReader.py
--rw-rw-r--   0 silvino   (1001) silvino   (1001)     2987 2020-01-31 15:00:38.000000 ofxReaderBR-0.9.0/ofxReaderBR/reader/readercashflow.py
--rw-rw-r--   0 silvino   (1001) silvino   (1001)        0 2019-11-05 20:06:09.000000 ofxReaderBR-0.9.0/ofxReaderBR/reader/__init__.py
--rw-rw-r--   0 silvino   (1001) silvino   (1001)     3524 2020-01-31 17:42:22.000000 ofxReaderBR-0.9.0/ofxReaderBR/reader/OFXReaderController.py
--rw-rw-r--   0 silvino   (1001) silvino   (1001)     5431 2020-01-31 17:42:22.000000 ofxReaderBR-0.9.0/ofxReaderBR/reader/readerbankstatement.py
-drwxrwxr-x   0 silvino   (1001) silvino   (1001)        0 2020-01-31 17:43:25.000000 ofxReaderBR-0.9.0/ofxReaderBR/factory/
--rw-rw-r--   0 silvino   (1001) silvino   (1001)      640 2020-01-31 17:42:22.000000 ofxReaderBR-0.9.0/ofxReaderBR/factory/PDFReaderFactory.py
--rw-rw-r--   0 silvino   (1001) silvino   (1001)      640 2020-01-31 17:42:22.000000 ofxReaderBR-0.9.0/ofxReaderBR/factory/XLSReaderFactory.py
--rw-rw-r--   0 silvino   (1001) silvino   (1001)      643 2020-01-31 17:42:22.000000 ofxReaderBR-0.9.0/ofxReaderBR/factory/OFXReaderFactory.py
--rw-rw-r--   0 silvino   (1001) silvino   (1001)        0 2020-01-31 17:35:18.000000 ofxReaderBR-0.9.0/ofxReaderBR/factory/__init__.py
--rw-rw-r--   0 silvino   (1001) silvino   (1001)      640 2020-01-31 17:42:22.000000 ofxReaderBR-0.9.0/ofxReaderBR/factory/XMLReaderFactory.py
--rw-rw-r--   0 silvino   (1001) silvino   (1001)      334 2020-01-31 17:42:22.000000 ofxReaderBR-0.9.0/ofxReaderBR/factory/ReaderAbstractFactory.py
--rw-rw-r--   0 silvino   (1001) silvino   (1001)        0 2019-11-05 20:06:09.000000 ofxReaderBR-0.9.0/ofxReaderBR/__init__.py
-drwxrwxr-x   0 silvino   (1001) silvino   (1001)        0 2020-01-31 17:43:25.000000 ofxReaderBR-0.9.0/ofxReaderBR/model/
--rw-rw-r--   0 silvino   (1001) silvino   (1001)     2343 2020-01-31 17:42:22.000000 ofxReaderBR-0.9.0/ofxReaderBR/model/tests.py
--rw-rw-r--   0 silvino   (1001) silvino   (1001)      126 2020-01-31 17:42:22.000000 ofxReaderBR-0.9.0/ofxReaderBR/model/__init__.py
--rw-rw-r--   0 silvino   (1001) silvino   (1001)     1523 2020-01-30 17:39:32.000000 ofxReaderBR-0.9.0/ofxReaderBR/model/origin.py
--rw-rw-r--   0 silvino   (1001) silvino   (1001)      886 2020-01-31 17:42:22.000000 ofxReaderBR-0.9.0/ofxReaderBR/model/bankstatement.py
--rw-rw-r--   0 silvino   (1001) silvino   (1001)     2475 2020-01-31 15:00:38.000000 ofxReaderBR-0.9.0/ofxReaderBR/model/cashflow.py
--rw-rw-r--   0 silvino   (1001) silvino   (1001)     1971 2020-01-31 17:42:22.000000 ofxReaderBR-0.9.0/ofxReaderBR/OFXReaderBR.py
--rw-rw-r--   0 silvino   (1001) silvino   (1001)     1088 2020-01-31 17:42:31.000000 ofxReaderBR-0.9.0/setup.py
--rw-rw-r--   0 silvino   (1001) silvino   (1001)      593 2020-01-31 17:43:25.000000 ofxReaderBR-0.9.0/PKG-INFO
+drwxrwxr-x   0 silvino   (1001) silvino   (1001)        0 2020-02-03 16:09:22.000000 ofxReaderBR-0.9.1/
+-rw-r--r--   0 silvino   (1001) silvino   (1001)       39 2019-11-05 20:00:45.000000 ofxReaderBR-0.9.1/setup.cfg
+drwxrwxr-x   0 silvino   (1001) silvino   (1001)        0 2020-02-03 16:09:22.000000 ofxReaderBR-0.9.1/ofxReaderBR/
+drwxrwxr-x   0 silvino   (1001) silvino   (1001)        0 2020-02-03 16:09:22.000000 ofxReaderBR-0.9.1/ofxReaderBR/reader/
+-rw-rw-r--   0 silvino   (1001) silvino   (1001)     2318 2020-01-31 17:42:22.000000 ofxReaderBR-0.9.1/ofxReaderBR/reader/readercontroller.py
+drwxrwxr-x   0 silvino   (1001) silvino   (1001)        0 2020-02-03 16:09:22.000000 ofxReaderBR-0.9.1/ofxReaderBR/reader/pdf/
+-rw-rw-r--   0 silvino   (1001) silvino   (1001)     1372 2020-01-31 17:42:22.000000 ofxReaderBR-0.9.1/ofxReaderBR/reader/pdf/pdfParser.py
+-rw-rw-r--   0 silvino   (1001) silvino   (1001)     6243 2019-12-23 20:31:31.000000 ofxReaderBR-0.9.1/ofxReaderBR/reader/pdf/PDFParserSantander.py
+-rw-rw-r--   0 silvino   (1001) silvino   (1001)      525 2020-01-31 17:42:22.000000 ofxReaderBR-0.9.1/ofxReaderBR/reader/pdf/pdfReader.py
+-rw-rw-r--   0 silvino   (1001) silvino   (1001)     2955 2020-02-03 16:08:41.000000 ofxReaderBR-0.9.1/ofxReaderBR/reader/readercashflow.py
+-rw-rw-r--   0 silvino   (1001) silvino   (1001)        0 2019-11-05 20:06:09.000000 ofxReaderBR-0.9.1/ofxReaderBR/reader/__init__.py
+-rw-rw-r--   0 silvino   (1001) silvino   (1001)     3524 2020-01-31 17:42:22.000000 ofxReaderBR-0.9.1/ofxReaderBR/reader/OFXReaderController.py
+-rw-rw-r--   0 silvino   (1001) silvino   (1001)     5431 2020-01-31 17:42:22.000000 ofxReaderBR-0.9.1/ofxReaderBR/reader/readerbankstatement.py
+drwxrwxr-x   0 silvino   (1001) silvino   (1001)        0 2020-02-03 16:09:22.000000 ofxReaderBR-0.9.1/ofxReaderBR/factory/
+-rw-rw-r--   0 silvino   (1001) silvino   (1001)      640 2020-01-31 17:42:22.000000 ofxReaderBR-0.9.1/ofxReaderBR/factory/PDFReaderFactory.py
+-rw-rw-r--   0 silvino   (1001) silvino   (1001)      640 2020-01-31 17:42:22.000000 ofxReaderBR-0.9.1/ofxReaderBR/factory/XLSReaderFactory.py
+-rw-rw-r--   0 silvino   (1001) silvino   (1001)      643 2020-01-31 17:42:22.000000 ofxReaderBR-0.9.1/ofxReaderBR/factory/OFXReaderFactory.py
+-rw-rw-r--   0 silvino   (1001) silvino   (1001)        0 2020-01-31 17:35:18.000000 ofxReaderBR-0.9.1/ofxReaderBR/factory/__init__.py
+-rw-rw-r--   0 silvino   (1001) silvino   (1001)      640 2020-01-31 17:42:22.000000 ofxReaderBR-0.9.1/ofxReaderBR/factory/XMLReaderFactory.py
+-rw-rw-r--   0 silvino   (1001) silvino   (1001)      334 2020-01-31 17:42:22.000000 ofxReaderBR-0.9.1/ofxReaderBR/factory/ReaderAbstractFactory.py
+-rw-rw-r--   0 silvino   (1001) silvino   (1001)        0 2019-11-05 20:06:09.000000 ofxReaderBR-0.9.1/ofxReaderBR/__init__.py
+drwxrwxr-x   0 silvino   (1001) silvino   (1001)        0 2020-02-03 16:09:22.000000 ofxReaderBR-0.9.1/ofxReaderBR/model/
+-rw-rw-r--   0 silvino   (1001) silvino   (1001)     2343 2020-01-31 17:42:22.000000 ofxReaderBR-0.9.1/ofxReaderBR/model/tests.py
+-rw-rw-r--   0 silvino   (1001) silvino   (1001)      126 2020-01-31 17:42:22.000000 ofxReaderBR-0.9.1/ofxReaderBR/model/__init__.py
+-rw-rw-r--   0 silvino   (1001) silvino   (1001)     1523 2020-01-30 17:39:32.000000 ofxReaderBR-0.9.1/ofxReaderBR/model/origin.py
+-rw-rw-r--   0 silvino   (1001) silvino   (1001)      886 2020-01-31 17:42:22.000000 ofxReaderBR-0.9.1/ofxReaderBR/model/bankstatement.py
+-rw-rw-r--   0 silvino   (1001) silvino   (1001)     2475 2020-01-31 15:00:38.000000 ofxReaderBR-0.9.1/ofxReaderBR/model/cashflow.py
+-rw-rw-r--   0 silvino   (1001) silvino   (1001)     1971 2020-01-31 17:42:22.000000 ofxReaderBR-0.9.1/ofxReaderBR/OFXReaderBR.py
+-rw-rw-r--   0 silvino   (1001) silvino   (1001)     1088 2020-02-03 16:08:41.000000 ofxReaderBR-0.9.1/setup.py
+-rw-rw-r--   0 silvino   (1001) silvino   (1001)      593 2020-02-03 16:09:22.000000 ofxReaderBR-0.9.1/PKG-INFO
```

### Comparing `ofxReaderBR-0.9.0/ofxReaderBR/reader/readercontroller.py` & `ofxReaderBR-0.9.1/ofxReaderBR/reader/readercontroller.py`

 * *Files identical despite different names*

### Comparing `ofxReaderBR-0.9.0/ofxReaderBR/reader/pdf/pdfParser.py` & `ofxReaderBR-0.9.1/ofxReaderBR/reader/pdf/pdfParser.py`

 * *Files identical despite different names*

### Comparing `ofxReaderBR-0.9.0/ofxReaderBR/reader/pdf/PDFParserSantander.py` & `ofxReaderBR-0.9.1/ofxReaderBR/reader/pdf/PDFParserSantander.py`

 * *Files identical despite different names*

### Comparing `ofxReaderBR-0.9.0/ofxReaderBR/reader/pdf/pdfReader.py` & `ofxReaderBR-0.9.1/ofxReaderBR/reader/pdf/pdfReader.py`

 * *Files identical despite different names*

### Comparing `ofxReaderBR-0.9.0/ofxReaderBR/reader/readercashflow.py` & `ofxReaderBR-0.9.1/ofxReaderBR/reader/readercashflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,14 @@
         for cellValue in row:
             cell_values.append(cellValue)
 
         if len(cell_values) != 6:
             raise ValueError('XLS expected to have 6 columns.')
 
         if all([value is None for value in cell_values]):
-            cs.date = 'invalid'
             logger.info('Row with blank columns. Made cash flow invalid.')
             return cs
 
         if None in cell_values:
             raise ValueError(f'Row does not have all values: {row}')
 
         Account = namedtuple('Account', 'acctid')
```

### Comparing `ofxReaderBR-0.9.0/ofxReaderBR/reader/OFXReaderController.py` & `ofxReaderBR-0.9.1/ofxReaderBR/reader/OFXReaderController.py`

 * *Files identical despite different names*

### Comparing `ofxReaderBR-0.9.0/ofxReaderBR/reader/readerbankstatement.py` & `ofxReaderBR-0.9.1/ofxReaderBR/reader/readerbankstatement.py`

 * *Files identical despite different names*

### Comparing `ofxReaderBR-0.9.0/ofxReaderBR/factory/PDFReaderFactory.py` & `ofxReaderBR-0.9.1/ofxReaderBR/factory/PDFReaderFactory.py`

 * *Files identical despite different names*

### Comparing `ofxReaderBR-0.9.0/ofxReaderBR/factory/XLSReaderFactory.py` & `ofxReaderBR-0.9.1/ofxReaderBR/factory/XLSReaderFactory.py`

 * *Files identical despite different names*

### Comparing `ofxReaderBR-0.9.0/ofxReaderBR/factory/OFXReaderFactory.py` & `ofxReaderBR-0.9.1/ofxReaderBR/factory/OFXReaderFactory.py`

 * *Files identical despite different names*

### Comparing `ofxReaderBR-0.9.0/ofxReaderBR/factory/XMLReaderFactory.py` & `ofxReaderBR-0.9.1/ofxReaderBR/factory/XMLReaderFactory.py`

 * *Files identical despite different names*

### Comparing `ofxReaderBR-0.9.0/ofxReaderBR/model/tests.py` & `ofxReaderBR-0.9.1/ofxReaderBR/model/tests.py`

 * *Files identical despite different names*

### Comparing `ofxReaderBR-0.9.0/ofxReaderBR/model/origin.py` & `ofxReaderBR-0.9.1/ofxReaderBR/model/origin.py`

 * *Files identical despite different names*

### Comparing `ofxReaderBR-0.9.0/ofxReaderBR/model/bankstatement.py` & `ofxReaderBR-0.9.1/ofxReaderBR/model/bankstatement.py`

 * *Files identical despite different names*

### Comparing `ofxReaderBR-0.9.0/ofxReaderBR/model/cashflow.py` & `ofxReaderBR-0.9.1/ofxReaderBR/model/cashflow.py`

 * *Files identical despite different names*

### Comparing `ofxReaderBR-0.9.0/ofxReaderBR/OFXReaderBR.py` & `ofxReaderBR-0.9.1/ofxReaderBR/OFXReaderBR.py`

 * *Files identical despite different names*

### Comparing `ofxReaderBR-0.9.0/setup.py` & `ofxReaderBR-0.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 setup(
     name='ofxReaderBR',
     packages=['ofxReaderBR',
               'ofxReaderBR.factory',
               'ofxReaderBR.model',
               'ofxReaderBR.reader',
               'ofxReaderBR.reader.pdf'],
-    version='0.9.0',
+    version='0.9.1',
     license='MIT',
     description='Convert ofx + xlsx to xlsx - pt_BR',
     author='Fintask',
     author_email='admin@fintask.com.br',
     url='https://github.com/Fintask/ofxReaderBR/',
-    download_url='https://github.com/Fintask/ofxReaderBR/archive/v0.9.0.tar.gz',
+    download_url='https://github.com/Fintask/ofxReaderBR/archive/v0.9.1.tar.gz',
     keywords=['ofx', 'xlsx'],
     install_requires=[
         'et-xmlfile',
         'jdcal',
         'openpyxl',
         'ofxtoolslambda',
         'pytz',
```

### Comparing `ofxReaderBR-0.9.0/PKG-INFO` & `ofxReaderBR-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: ofxReaderBR
-Version: 0.9.0
+Version: 0.9.1
 Summary: Convert ofx + xlsx to xlsx - pt_BR
 Home-page: https://github.com/Fintask/ofxReaderBR/
 Author: Fintask
 Author-email: admin@fintask.com.br
 License: MIT
-Download-URL: https://github.com/Fintask/ofxReaderBR/archive/v0.9.0.tar.gz
+Download-URL: https://github.com/Fintask/ofxReaderBR/archive/v0.9.1.tar.gz
 Description: UNKNOWN
 Keywords: ofx,xlsx
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

