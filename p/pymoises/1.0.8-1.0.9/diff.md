# Comparing `tmp/pymoises-1.0.8.tar.gz` & `tmp/pymoises-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymoises-1.0.8.tar", last modified: Thu Dec  7 00:07:40 2023, max compression
+gzip compressed data, was "pymoises-1.0.9.tar", last modified: Thu Dec  7 00:31:56 2023, max compression
```

## Comparing `pymoises-1.0.8.tar` & `pymoises-1.0.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-12-07 00:07:40.407961 pymoises-1.0.8/
--rw-rw-rw-   0        0        0      187 2023-12-07 00:07:40.405962 pymoises-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       12 2023-12-06 15:35:18.000000 pymoises-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-12-07 00:07:40.352962 pymoises-1.0.8/pymoises/
--rw-rw-rw-   0        0        0     5226 2023-12-06 15:35:18.000000 pymoises-1.0.8/pymoises/Transactions.py
--rw-rw-rw-   0        0        0      135 2023-12-06 15:35:18.000000 pymoises-1.0.8/pymoises/__init__.py
--rw-rw-rw-   0        0        0     1705 2023-12-06 15:35:18.000000 pymoises-1.0.8/pymoises/bussinesUnits.py
--rw-rw-rw-   0        0        0    10329 2023-12-06 15:35:18.000000 pymoises-1.0.8/pymoises/customer.py
-drwxrwxrwx   0        0        0        0 2023-12-07 00:07:40.373963 pymoises-1.0.8/pymoises/dto/
--rw-rw-rw-   0        0        0       43 2023-12-06 15:35:18.000000 pymoises-1.0.8/pymoises/dto/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-07 00:07:40.374964 pymoises-1.0.8/pymoises/dto/input/
--rw-rw-rw-   0        0        0       52 2023-12-06 15:35:18.000000 pymoises-1.0.8/pymoises/dto/input/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-07 00:07:40.380961 pymoises-1.0.8/pymoises/dto/input/customer/
--rw-rw-rw-   0        0        0       86 2023-12-06 15:35:18.000000 pymoises-1.0.8/pymoises/dto/input/customer/__init__.py
--rw-rw-rw-   0        0        0      530 2023-12-06 15:35:18.000000 pymoises-1.0.8/pymoises/dto/input/customer/checkEmailPhone_customer_input_dto.py
--rw-rw-rw-   0        0        0     1570 2023-12-06 15:35:18.000000 pymoises-1.0.8/pymoises/dto/input/customer/createLead_input_dto.py
-drwxrwxrwx   0        0        0        0 2023-12-07 00:07:40.385963 pymoises-1.0.8/pymoises/dto/input/transaction/
--rw-rw-rw-   0        0        0       43 2023-12-06 15:35:18.000000 pymoises-1.0.8/pymoises/dto/input/transaction/__init__.py
--rw-rw-rw-   0        0        0      524 2023-12-06 15:35:18.000000 pymoises-1.0.8/pymoises/dto/input/transaction/create_transaction_input_dto.py
-drwxrwxrwx   0        0        0        0 2023-12-07 00:07:40.387961 pymoises-1.0.8/pymoises/dto/output/
--rw-rw-rw-   0        0        0       51 2023-12-06 15:35:18.000000 pymoises-1.0.8/pymoises/dto/output/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-07 00:07:40.396968 pymoises-1.0.8/pymoises/dto/output/customer/
--rw-rw-rw-   0        0        0      108 2023-12-06 15:35:18.000000 pymoises-1.0.8/pymoises/dto/output/customer/__init__.py
--rw-rw-rw-   0        0        0      758 2023-12-06 15:35:18.000000 pymoises-1.0.8/pymoises/dto/output/customer/createLead_output_dto.py
--rw-rw-rw-   0        0        0     1351 2023-12-06 15:35:18.000000 pymoises-1.0.8/pymoises/dto/output/customer/customer_output_dto.py
--rw-rw-rw-   0        0        0      930 2023-12-06 15:35:18.000000 pymoises-1.0.8/pymoises/dto/output/customer/moveLead_output_dto.py
-drwxrwxrwx   0        0        0        0 2023-12-07 00:07:40.399962 pymoises-1.0.8/pymoises/dto/output/psps/
--rw-rw-rw-   0        0        0        0 2023-12-06 15:35:18.000000 pymoises-1.0.8/pymoises/dto/output/psps/__init__.py
--rw-rw-rw-   0        0        0     1602 2023-12-06 15:35:18.000000 pymoises-1.0.8/pymoises/dto/output/psps/get_info_psp_output_dto.py
-drwxrwxrwx   0        0        0        0 2023-12-07 00:07:40.403962 pymoises-1.0.8/pymoises/dto/output/transaction/
--rw-rw-rw-   0        0        0       37 2023-12-06 15:35:18.000000 pymoises-1.0.8/pymoises/dto/output/transaction/__init__.py
--rw-rw-rw-   0        0        0      552 2023-12-06 15:35:18.000000 pymoises-1.0.8/pymoises/dto/output/transaction/transaction_output_dto.py
--rw-rw-rw-   0        0        0     3613 2023-12-06 20:22:45.000000 pymoises-1.0.8/pymoises/psps.py
-drwxrwxrwx   0        0        0        0 2023-12-07 00:07:40.371963 pymoises-1.0.8/pymoises.egg-info/
--rw-rw-rw-   0        0        0      187 2023-12-07 00:07:40.000000 pymoises-1.0.8/pymoises.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1029 2023-12-07 00:07:40.000000 pymoises-1.0.8/pymoises.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-07 00:07:40.000000 pymoises-1.0.8/pymoises.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-12-07 00:07:40.000000 pymoises-1.0.8/pymoises.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-12-07 00:07:40.000000 pymoises-1.0.8/pymoises.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-12-07 00:07:40.407961 pymoises-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      558 2023-12-07 00:06:30.000000 pymoises-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-12-07 00:31:56.585068 pymoises-1.0.9/
+-rw-rw-rw-   0        0        0      187 2023-12-07 00:31:56.584064 pymoises-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       12 2023-12-06 15:35:18.000000 pymoises-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-12-07 00:31:56.523066 pymoises-1.0.9/pymoises/
+-rw-rw-rw-   0        0        0     5226 2023-12-06 15:35:18.000000 pymoises-1.0.9/pymoises/Transactions.py
+-rw-rw-rw-   0        0        0      135 2023-12-06 15:35:18.000000 pymoises-1.0.9/pymoises/__init__.py
+-rw-rw-rw-   0        0        0     1705 2023-12-06 15:35:18.000000 pymoises-1.0.9/pymoises/bussinesUnits.py
+-rw-rw-rw-   0        0        0    10329 2023-12-06 15:35:18.000000 pymoises-1.0.9/pymoises/customer.py
+drwxrwxrwx   0        0        0        0 2023-12-07 00:31:56.553068 pymoises-1.0.9/pymoises/dto/
+-rw-rw-rw-   0        0        0       43 2023-12-06 15:35:18.000000 pymoises-1.0.9/pymoises/dto/__init__.py
+drwxrwxrwx   0        0        0        0 2023-12-07 00:31:56.555068 pymoises-1.0.9/pymoises/dto/input/
+-rw-rw-rw-   0        0        0       52 2023-12-06 15:35:18.000000 pymoises-1.0.9/pymoises/dto/input/__init__.py
+drwxrwxrwx   0        0        0        0 2023-12-07 00:31:56.562067 pymoises-1.0.9/pymoises/dto/input/customer/
+-rw-rw-rw-   0        0        0       86 2023-12-06 15:35:18.000000 pymoises-1.0.9/pymoises/dto/input/customer/__init__.py
+-rw-rw-rw-   0        0        0      530 2023-12-06 15:35:18.000000 pymoises-1.0.9/pymoises/dto/input/customer/checkEmailPhone_customer_input_dto.py
+-rw-rw-rw-   0        0        0     1570 2023-12-06 15:35:18.000000 pymoises-1.0.9/pymoises/dto/input/customer/createLead_input_dto.py
+drwxrwxrwx   0        0        0        0 2023-12-07 00:31:56.565067 pymoises-1.0.9/pymoises/dto/input/transaction/
+-rw-rw-rw-   0        0        0       43 2023-12-06 15:35:18.000000 pymoises-1.0.9/pymoises/dto/input/transaction/__init__.py
+-rw-rw-rw-   0        0        0      524 2023-12-06 15:35:18.000000 pymoises-1.0.9/pymoises/dto/input/transaction/create_transaction_input_dto.py
+drwxrwxrwx   0        0        0        0 2023-12-07 00:31:56.567066 pymoises-1.0.9/pymoises/dto/output/
+-rw-rw-rw-   0        0        0       51 2023-12-06 15:35:18.000000 pymoises-1.0.9/pymoises/dto/output/__init__.py
+drwxrwxrwx   0        0        0        0 2023-12-07 00:31:56.575068 pymoises-1.0.9/pymoises/dto/output/customer/
+-rw-rw-rw-   0        0        0      108 2023-12-06 15:35:18.000000 pymoises-1.0.9/pymoises/dto/output/customer/__init__.py
+-rw-rw-rw-   0        0        0      758 2023-12-06 15:35:18.000000 pymoises-1.0.9/pymoises/dto/output/customer/createLead_output_dto.py
+-rw-rw-rw-   0        0        0     1351 2023-12-06 15:35:18.000000 pymoises-1.0.9/pymoises/dto/output/customer/customer_output_dto.py
+-rw-rw-rw-   0        0        0      930 2023-12-06 15:35:18.000000 pymoises-1.0.9/pymoises/dto/output/customer/moveLead_output_dto.py
+drwxrwxrwx   0        0        0        0 2023-12-07 00:31:56.578066 pymoises-1.0.9/pymoises/dto/output/psps/
+-rw-rw-rw-   0        0        0        0 2023-12-06 15:35:18.000000 pymoises-1.0.9/pymoises/dto/output/psps/__init__.py
+-rw-rw-rw-   0        0        0     1602 2023-12-06 15:35:18.000000 pymoises-1.0.9/pymoises/dto/output/psps/get_info_psp_output_dto.py
+drwxrwxrwx   0        0        0        0 2023-12-07 00:31:56.582074 pymoises-1.0.9/pymoises/dto/output/transaction/
+-rw-rw-rw-   0        0        0       37 2023-12-06 15:35:18.000000 pymoises-1.0.9/pymoises/dto/output/transaction/__init__.py
+-rw-rw-rw-   0        0        0      552 2023-12-06 15:35:18.000000 pymoises-1.0.9/pymoises/dto/output/transaction/transaction_output_dto.py
+-rw-rw-rw-   0        0        0     3626 2023-12-07 00:19:28.000000 pymoises-1.0.9/pymoises/psps.py
+drwxrwxrwx   0        0        0        0 2023-12-07 00:31:56.551067 pymoises-1.0.9/pymoises.egg-info/
+-rw-rw-rw-   0        0        0      187 2023-12-07 00:31:56.000000 pymoises-1.0.9/pymoises.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1029 2023-12-07 00:31:56.000000 pymoises-1.0.9/pymoises.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-12-07 00:31:56.000000 pymoises-1.0.9/pymoises.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-12-07 00:31:56.000000 pymoises-1.0.9/pymoises.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-12-07 00:31:56.000000 pymoises-1.0.9/pymoises.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-12-07 00:31:56.585068 pymoises-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      558 2023-12-07 00:31:37.000000 pymoises-1.0.9/setup.py
```

### Comparing `pymoises-1.0.8/pymoises/Transactions.py` & `pymoises-1.0.9/pymoises/Transactions.py`

 * *Files identical despite different names*

### Comparing `pymoises-1.0.8/pymoises/bussinesUnits.py` & `pymoises-1.0.9/pymoises/bussinesUnits.py`

 * *Files identical despite different names*

### Comparing `pymoises-1.0.8/pymoises/customer.py` & `pymoises-1.0.9/pymoises/customer.py`

 * *Files identical despite different names*

### Comparing `pymoises-1.0.8/pymoises/dto/input/customer/checkEmailPhone_customer_input_dto.py` & `pymoises-1.0.9/pymoises/dto/input/customer/checkEmailPhone_customer_input_dto.py`

 * *Files identical despite different names*

### Comparing `pymoises-1.0.8/pymoises/dto/input/customer/createLead_input_dto.py` & `pymoises-1.0.9/pymoises/dto/input/customer/createLead_input_dto.py`

 * *Files identical despite different names*

### Comparing `pymoises-1.0.8/pymoises/dto/input/transaction/create_transaction_input_dto.py` & `pymoises-1.0.9/pymoises/dto/input/transaction/create_transaction_input_dto.py`

 * *Files identical despite different names*

### Comparing `pymoises-1.0.8/pymoises/dto/output/customer/createLead_output_dto.py` & `pymoises-1.0.9/pymoises/dto/output/customer/createLead_output_dto.py`

 * *Files identical despite different names*

### Comparing `pymoises-1.0.8/pymoises/dto/output/customer/customer_output_dto.py` & `pymoises-1.0.9/pymoises/dto/output/customer/customer_output_dto.py`

 * *Files identical despite different names*

### Comparing `pymoises-1.0.8/pymoises/dto/output/customer/moveLead_output_dto.py` & `pymoises-1.0.9/pymoises/dto/output/customer/moveLead_output_dto.py`

 * *Files identical despite different names*

### Comparing `pymoises-1.0.8/pymoises/dto/output/psps/get_info_psp_output_dto.py` & `pymoises-1.0.9/pymoises/dto/output/psps/get_info_psp_output_dto.py`

 * *Files identical despite different names*

### Comparing `pymoises-1.0.8/pymoises/dto/output/transaction/transaction_output_dto.py` & `pymoises-1.0.9/pymoises/dto/output/transaction/transaction_output_dto.py`

 * *Files identical despite different names*

### Comparing `pymoises-1.0.8/pymoises/psps.py` & `pymoises-1.0.9/pymoises/psps.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,17 +69,17 @@
         """
         Activate the psp and set 'active' in both the visibility and active fields.
 
         Params:
             idPsp (int): psps ids in moises  
 
         Return:
-            result (int): success function
-            error (string): result of function
-            data (dict) : result message
+            success (boolean): success function
+            message (string): result of function
+            payload (dict) : result message
 
         """
         
         url = "http://webservicesnt.org:5050/update/cat-psp-active"
     
         
         payload = {}
@@ -88,15 +88,15 @@
 
         headers = {}
         headers['Content-Type'] = 'application/json'
         
         try:
 
             response = requests.request("POST", url, headers=headers, json=payload)
-            logging.warning('response active cat psp'.format(response.text))
+            logging.warning('response active cat psp {}'.format(response.text))
             response = response.json()
 
             if not response['result'] == 1:
                 response_psp = {}
                 response_psp['success'] = False
                 response_psp['message'] = "psp not updated"
                 response_psp['payload'] = {}
```

### Comparing `pymoises-1.0.8/pymoises.egg-info/SOURCES.txt` & `pymoises-1.0.9/pymoises.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymoises-1.0.8/setup.py` & `pymoises-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="pymoises",
-    version="1.0.8",
+    version="1.0.9",
     description="Callings from moises endpoints...",
     author="Platimex",
     packages=[
         "pymoises", 
         "pymoises.dto", 
         "pymoises.dto.input", 
         "pymoises.dto.input.customer",
```

