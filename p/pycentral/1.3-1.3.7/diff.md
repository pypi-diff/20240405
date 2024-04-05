# Comparing `tmp/pycentral-1.3.tar.gz` & `tmp/pycentral-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycentral-1.3.tar", last modified: Mon Oct 23 15:44:03 2023, max compression
+gzip compressed data, was "pycentral-1.3.7.tar", last modified: Fri Apr  5 14:18:54 2024, max compression
```

## Comparing `pycentral-1.3.tar` & `pycentral-1.3.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 satheesk   (501) staff       (20)        0 2023-10-23 15:44:03.915096 pycentral-1.3/
--rw-r--r--   0 satheesk   (501) staff       (20)     1100 2023-02-01 17:44:05.000000 pycentral-1.3/LICENSE
--rw-r--r--   0 satheesk   (501) staff       (20)     8450 2023-10-23 15:44:03.876959 pycentral-1.3/PKG-INFO
--rw-r--r--   0 satheesk   (501) staff       (20)     7709 2023-08-16 14:05:58.000000 pycentral-1.3/README.md
-drwxr-xr-x   0 satheesk   (501) staff       (20)        0 2023-10-23 15:44:03.848044 pycentral-1.3/pycentral/
--rw-r--r--   0 satheesk   (501) staff       (20)        0 2023-02-01 17:44:05.000000 pycentral-1.3/pycentral/__init__.py
--rw-r--r--   0 satheesk   (501) staff       (20)     8170 2023-09-11 18:13:12.000000 pycentral-1.3/pycentral/audit_logs.py
--rwxr-xr-x   0 satheesk   (501) staff       (20)    27319 2023-09-11 18:13:12.000000 pycentral-1.3/pycentral/base.py
--rwxr-xr-x   0 satheesk   (501) staff       (20)     6261 2023-09-11 18:13:12.000000 pycentral-1.3/pycentral/base_utils.py
--rw-r--r--   0 satheesk   (501) staff       (20)    47335 2023-09-11 18:13:12.000000 pycentral-1.3/pycentral/configuration.py
--rw-r--r--   0 satheesk   (501) staff       (20)     1205 2023-09-11 18:13:12.000000 pycentral-1.3/pycentral/constants.py
--rw-r--r--   0 satheesk   (501) staff       (20)    11268 2023-09-12 19:23:09.000000 pycentral-1.3/pycentral/device_inventory.py
--rw-r--r--   0 satheesk   (501) staff       (20)    12354 2023-09-11 18:13:12.000000 pycentral-1.3/pycentral/firmware_management.py
--rw-r--r--   0 satheesk   (501) staff       (20)    21314 2023-09-11 18:13:12.000000 pycentral-1.3/pycentral/licensing.py
--rw-r--r--   0 satheesk   (501) staff       (20)    12946 2023-09-11 18:13:12.000000 pycentral-1.3/pycentral/monitoring.py
--rw-r--r--   0 satheesk   (501) staff       (20)    38361 2023-10-23 14:39:48.000000 pycentral-1.3/pycentral/msp.py
--rw-r--r--   0 satheesk   (501) staff       (20)    23062 2023-09-11 18:13:12.000000 pycentral-1.3/pycentral/rapids.py
--rw-r--r--   0 satheesk   (501) staff       (20)     2815 2023-09-11 18:13:12.000000 pycentral-1.3/pycentral/refresh_api_token.py
--rw-r--r--   0 satheesk   (501) staff       (20)     5986 2023-09-11 18:13:12.000000 pycentral-1.3/pycentral/topology.py
--rw-r--r--   0 satheesk   (501) staff       (20)     8729 2023-10-23 10:10:40.000000 pycentral-1.3/pycentral/url_utils.py
--rw-r--r--   0 satheesk   (501) staff       (20)    17963 2023-09-11 18:13:12.000000 pycentral-1.3/pycentral/user_management.py
--rw-r--r--   0 satheesk   (501) staff       (20)    14313 2023-09-11 18:13:12.000000 pycentral-1.3/pycentral/visualrf.py
-drwxr-xr-x   0 satheesk   (501) staff       (20)        0 2023-10-23 15:44:03.870745 pycentral-1.3/pycentral/workflows/
--rw-r--r--   0 satheesk   (501) staff       (20)        0 2023-02-01 17:44:05.000000 pycentral-1.3/pycentral/workflows/__init__.py
--rw-r--r--   0 satheesk   (501) staff       (20)     6060 2023-09-11 18:13:12.000000 pycentral-1.3/pycentral/workflows/workflows_utils.py
-drwxr-xr-x   0 satheesk   (501) staff       (20)        0 2023-10-23 15:44:03.867684 pycentral-1.3/pycentral.egg-info/
--rw-r--r--   0 satheesk   (501) staff       (20)     8450 2023-10-23 15:44:03.000000 pycentral-1.3/pycentral.egg-info/PKG-INFO
--rw-r--r--   0 satheesk   (501) staff       (20)      673 2023-10-23 15:44:03.000000 pycentral-1.3/pycentral.egg-info/SOURCES.txt
--rw-r--r--   0 satheesk   (501) staff       (20)        1 2023-10-23 15:44:03.000000 pycentral-1.3/pycentral.egg-info/dependency_links.txt
--rw-r--r--   0 satheesk   (501) staff       (20)       53 2023-10-23 15:44:03.000000 pycentral-1.3/pycentral.egg-info/requires.txt
--rw-r--r--   0 satheesk   (501) staff       (20)       10 2023-10-23 15:44:03.000000 pycentral-1.3/pycentral.egg-info/top_level.txt
--rw-r--r--   0 satheesk   (501) staff       (20)       38 2023-10-23 15:44:03.915388 pycentral-1.3/setup.cfg
--rw-r--r--   0 satheesk   (501) staff       (20)     1122 2023-10-23 15:41:25.000000 pycentral-1.3/setup.py
+drwxr-xr-x   0 satheesk   (501) staff       (20)        0 2024-04-05 14:18:54.033451 pycentral-1.3.7/
+-rw-r--r--   0 satheesk   (501) staff       (20)     1100 2023-02-01 17:44:05.000000 pycentral-1.3.7/LICENSE
+-rw-r--r--   0 satheesk   (501) staff       (20)     9684 2024-04-05 14:18:54.032272 pycentral-1.3.7/PKG-INFO
+-rw-r--r--   0 satheesk   (501) staff       (20)     8941 2024-04-03 14:46:41.000000 pycentral-1.3.7/README.md
+drwxr-xr-x   0 satheesk   (501) staff       (20)        0 2024-04-05 14:18:54.020358 pycentral-1.3.7/pycentral/
+-rw-r--r--   0 satheesk   (501) staff       (20)        0 2023-02-01 17:44:05.000000 pycentral-1.3.7/pycentral/__init__.py
+-rw-r--r--   0 satheesk   (501) staff       (20)     8170 2023-09-11 18:13:12.000000 pycentral-1.3.7/pycentral/audit_logs.py
+-rwxr-xr-x   0 satheesk   (501) staff       (20)    27667 2024-04-03 14:41:41.000000 pycentral-1.3.7/pycentral/base.py
+-rwxr-xr-x   0 satheesk   (501) staff       (20)     9372 2024-04-01 08:40:02.000000 pycentral-1.3.7/pycentral/base_utils.py
+-rw-r--r--   0 satheesk   (501) staff       (20)    54134 2024-04-05 14:01:05.000000 pycentral-1.3.7/pycentral/configuration.py
+-rw-r--r--   0 satheesk   (501) staff       (20)     2165 2024-04-03 08:27:06.000000 pycentral-1.3.7/pycentral/constants.py
+-rw-r--r--   0 satheesk   (501) staff       (20)    11268 2023-09-12 19:23:09.000000 pycentral-1.3.7/pycentral/device_inventory.py
+-rw-r--r--   0 satheesk   (501) staff       (20)    12354 2023-09-11 18:13:12.000000 pycentral-1.3.7/pycentral/firmware_management.py
+-rw-r--r--   0 satheesk   (501) staff       (20)    21314 2023-09-11 18:13:12.000000 pycentral-1.3.7/pycentral/licensing.py
+-rw-r--r--   0 satheesk   (501) staff       (20)    12946 2023-09-11 18:13:12.000000 pycentral-1.3.7/pycentral/monitoring.py
+-rw-r--r--   0 satheesk   (501) staff       (20)    38361 2024-03-12 10:43:36.000000 pycentral-1.3.7/pycentral/msp.py
+-rw-r--r--   0 satheesk   (501) staff       (20)    23062 2023-09-11 18:13:12.000000 pycentral-1.3.7/pycentral/rapids.py
+-rw-r--r--   0 satheesk   (501) staff       (20)     2815 2023-09-11 18:13:12.000000 pycentral-1.3.7/pycentral/refresh_api_token.py
+-rw-r--r--   0 satheesk   (501) staff       (20)     5986 2023-09-11 18:13:12.000000 pycentral-1.3.7/pycentral/topology.py
+-rw-r--r--   0 satheesk   (501) staff       (20)     8729 2024-04-05 13:40:43.000000 pycentral-1.3.7/pycentral/url_utils.py
+-rw-r--r--   0 satheesk   (501) staff       (20)    17963 2023-09-11 18:13:12.000000 pycentral-1.3.7/pycentral/user_management.py
+-rw-r--r--   0 satheesk   (501) staff       (20)    14313 2023-09-11 18:13:12.000000 pycentral-1.3.7/pycentral/visualrf.py
+drwxr-xr-x   0 satheesk   (501) staff       (20)        0 2024-04-05 14:18:54.029584 pycentral-1.3.7/pycentral/workflows/
+-rw-r--r--   0 satheesk   (501) staff       (20)        0 2023-02-01 17:44:05.000000 pycentral-1.3.7/pycentral/workflows/__init__.py
+-rw-r--r--   0 satheesk   (501) staff       (20)     6060 2023-09-11 18:13:12.000000 pycentral-1.3.7/pycentral/workflows/workflows_utils.py
+drwxr-xr-x   0 satheesk   (501) staff       (20)        0 2024-04-05 14:18:54.031044 pycentral-1.3.7/pycentral.egg-info/
+-rw-r--r--   0 satheesk   (501) staff       (20)     9684 2024-04-05 14:18:53.000000 pycentral-1.3.7/pycentral.egg-info/PKG-INFO
+-rw-r--r--   0 satheesk   (501) staff       (20)      673 2024-04-05 14:18:53.000000 pycentral-1.3.7/pycentral.egg-info/SOURCES.txt
+-rw-r--r--   0 satheesk   (501) staff       (20)        1 2024-04-05 14:18:53.000000 pycentral-1.3.7/pycentral.egg-info/dependency_links.txt
+-rw-r--r--   0 satheesk   (501) staff       (20)       53 2024-04-05 14:18:53.000000 pycentral-1.3.7/pycentral.egg-info/requires.txt
+-rw-r--r--   0 satheesk   (501) staff       (20)       10 2024-04-05 14:18:53.000000 pycentral-1.3.7/pycentral.egg-info/top_level.txt
+-rw-r--r--   0 satheesk   (501) staff       (20)       38 2024-04-05 14:18:54.033661 pycentral-1.3.7/setup.cfg
+-rw-r--r--   0 satheesk   (501) staff       (20)     1124 2024-04-05 14:18:30.000000 pycentral-1.3.7/setup.py
```

### Comparing `pycentral-1.3/LICENSE` & `pycentral-1.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pycentral-1.3/PKG-INFO` & `pycentral-1.3.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: pycentral
-Version: 1.3
+Version: 1.3.7
 Summary: Aruba Central Python Package
 Home-page: https://github.com/aruba/pycentral
 Author: aruba-automation
 Author-email: aruba-automation@hpe.com
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: System Administrators
 Classifier: Topic :: System :: Networking
 Classifier: Development Status :: 4 - Beta
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: PyYAML
 Requires-Dist: urllib3
 Requires-Dist: certifi
 Provides-Extra: colorlog
@@ -52,27 +52,29 @@
 
 Now you can start making your script based on modules in pycentral or use different workflows from the subpackage `workflows`.
 
 ## Executing Scripts
 
 1. Gathering variables required for the package base class `ArubaCentralBase`.
 
-    * **base_url**: You can find the base URL of the Central account's API Gateway from the table <a href="https://www.arubanetworks.com/techdocs/central/latest/content/nms/api/domain_url.htm" target="_blank">here</a>. The base URL is based on the geographical Central cluster in which the account is registered.
-
-    * **client_id** and **client_secret**: Obtain client_id and client_secret variables by creating an API Gateway client in Aruba Central. Refer the following <a href="https://developer.arubanetworks.com/aruba-central/docs/api-gateway-creating-application-token" target="_blank">documentation</a> for more details.
+    * **base_url** OR **cluster_name**: You can find the base URL or cluster name of the Central account's API Gateway from the table <a href="https://www.arubanetworks.com/techdocs/central/latest/content/nms/api/domain_url.htm" target="_blank">here</a>. The base URL or cluster name is based on the geographical Central cluster in which the account is registered.
 
    * **access_token**: You can create an API access token for Aruba Central from -
       * <a href="https://developer.arubanetworks.com/aruba-central/docs/api-gateway-obtaining-access-tokens#obtain-access-token-via-web-ui" target="_blank">Aruba Central UI</a>
       * <a href="https://developer.arubanetworks.com/aruba-central/docs/api-oauth-access-token" target="_blank">OAuth APIs</a>
 
-    * **customer_id**: Obtain the **customer_id** by clicking on the figure icon on top right corner of Aruba Central WebUI.
+    * Optional variables - You need to provide the below variables if you want to use PyCentral's ability to generate access tokens from Aruba Central with the help of OAuth APIs.
+      * **username** and **password**: Aruba Central user's *username* and *password*. The access token generated by the OAUTH APIs will have the same role/privileges as the provided Aruba Central user.
+  
+      * **client_id** and **client_secret**: Obtain client_id and client_secret variables by creating an API Gateway client in Aruba Central. Refer the following <a href="https://developer.arubanetworks.com/aruba-central/docs/api-gateway-creating-application-token" target="_blank">documentation</a> for more details.
+    
+      * **customer_id**: Obtain the **customer_id** by clicking on the figure icon on top right corner of Aruba Central WebUI.
 
     ![Customer ID](https://github.com/aruba/pycentral/raw/master/pictures/customer-id.png)
 
-    * **username** and **password**: Aruba Central user's *username* and *password*. The access token generated by the OAUTH APIs will have the same role/privileges as the provided Aruba Central user.
 
 2. Providing input variables to the Python scripts. One of the following options can be used.
     * Provide variables directly to Aruba Central Base class in dictionary format.
 
         Access token approach:
         ```python
         central_info = {
@@ -90,21 +92,25 @@
                 "password": "<aruba-central-account-password>",
                 "client_id": "<api-gateway-client-id>",
                 "client_secret": "<api-gateway-client-secret>",
                 "customer_id": "<aruba-central-customer-id>",
                 "base_url": "<api-gateway-domain-url>"
             }
         ```
-
+        Alternatively, you can use **cluster_name** instead of **base_url** in the above mentioned dictionaries. You can find the list of clusters that are supported in the <a href="https://github.com/aruba/pycentral/blob/master/pycentral/constants.py" target="_blank">constants.py file</a>. If you would like to add support for other Central clusters, you can do so by adding it in the constants.py. 
         Refer the sample scripts in *step3* and *step4* for examples.
 
-    * **OR** Provide the required variables using JSON/YAML file. Refer input files <a href="https://github.com/aruba/pycentral/blob/master/sample_scripts/input_token_only.yaml" target="_blank">sample_scripts/input_token_only.yaml</a> and <a href="https://github.com/aruba/pycentral/blob/master/sample_scripts/input_credentials.yaml" target="_blank">sample_scripts/input_credentials.yaml</a> for information.
+    * **OR** Provide the required variables using JSON/YAML file. Refer to the sample input files to understand how the files have to be structured -
+      * <a href="https://github.com/aruba/pycentral/blob/master/sample_scripts/input_token_only.yaml" target="_blank">sample_scripts/input_token_only.yaml</a>
+      * <a href="https://github.com/aruba/pycentral/blob/master/sample_scripts/input_credentials.yaml" target="_blank">sample_scripts/input_credentials.yaml</a> 
+      * <a href="https://github.com/aruba/pycentral/blob/master/sample_scripts/sample_scripts/input_token_only_cluster.yaml" target="_blank">sample_scripts/input_token_only_cluster_name.yaml</a>
+      * <a href="https://github.com/aruba/pycentral/blob/master/sample_scripts/sample_scripts/input_credentials_cluster_name.yaml" target="_blank">sample_scripts/input_credentials_cluster_name.yaml</a>
 
-        Use `pycentral.workflows_utils.get_conn_from_file()` function which accepts name of the file and returns
-        the `ArubaCentralBase` instance object. Refer the sample script in *step5* for example.
+        More sample input files can be found in the <a href="https://github.com/aruba/pycentral/blob/master/sample_scripts/sample_scripts/" target="_blank">sample_scripts folder</a>. Use `pycentral.workflows_utils.get_conn_from_file()` function which accepts name of the file and returns
+        the `ArubaCentralBase` instance object.
 
 3. **Making API call using pycentral base**: Using the base class `ArubaCentralBase`, any Aruba Central supported REST API calls can be made. Refer the following sample script <a href="https://github.com/aruba/pycentral/blob/master/sample_scripts/pycentral_base_sample.py" target="_blank">sample_scripts/pycentral_base_sample.py</a>
 
     Obtain the HTTP Request related information from Aruba Central Swagger documentation or <a href="https://developer.arubanetworks.com/aruba-central/reference" target="_blank">API references</a> page in Aruba Developer Hub.
 
 4. **Making API call using pycentral modules**: Some API endpoints supported by Aruba Central are implemented as modules in the Python package. Refer the following sample script using modules <a href="https://github.com/aruba/pycentral/blob/master/sample_scripts/pycentral_module_sample.py" target="_blank">sample_scripts/pycentral_module_sample.py</a>
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: pycentral Version: 1.3 Summary: Aruba Central
+Metadata-Version: 2.1 Name: pycentral Version: 1.3.7 Summary: Aruba Central
 Python Package Home-page: https://github.com/aruba/pycentral Author: aruba-
 automation Author-email: aruba-automation@hpe.com Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Classifier: Intended
 Audience :: System Administrators Classifier: Topic :: System :: Networking
-Classifier: Development Status :: 4 - Beta Requires-Python: >=3.6 Description-
+Classifier: Development Status :: 4 - Beta Requires-Python: >=3.8 Description-
 Content-Type: text/markdown License-File: LICENSE Requires-Dist: requests
 Requires-Dist: PyYAML Requires-Dist: urllib3 Requires-Dist: certifi Provides-
 Extra: colorlog Requires-Dist: colorlog; extra == "colorlog" # pycentral ####
 Aruba Central Python Package Index SDK Aruba Central is an unified cloud-based
 network management and configuration platform for campus, branch, remote and
 data center networks. There are various needs for automation and
 programmability like automating repetitive tasks, configuring multiple devices,
@@ -20,62 +20,72 @@
 $ source centralenv/bin/activate in Windows: $ centralenv/Scripts/activate.bat
 ``` 3. Install the **pycentral** package ``` (centralenv)$ pip3 install
 pycentral ``` To install package with *extras* `colorLog` which will display
 log in color ``` (centralenv)$ pip3 install pycentral[colorLog] ``` Now you can
 start making your script based on modules in pycentral or use different
 workflows from the subpackage `workflows`. ## Executing Scripts 1. Gathering
 variables required for the package base class `ArubaCentralBase`. *
-**base_url**: You can find the base URL of the Central account's API Gateway
-from the table _h_e_r_e. The base URL is based on the geographical Central cluster
-in which the account is registered. * **client_id** and **client_secret**:
+**base_url** OR **cluster_name**: You can find the base URL or cluster name of
+the Central account's API Gateway from the table _h_e_r_e. The base URL or cluster
+name is based on the geographical Central cluster in which the account is
+registered. * **access_token**: You can create an API access token for Aruba
+Central from - * _A_r_u_b_a_ _C_e_n_t_r_a_l_ _U_I * _O_A_u_t_h_ _A_P_I_s * Optional variables - You need
+to provide the below variables if you want to use PyCentral's ability to
+generate access tokens from Aruba Central with the help of OAuth APIs. *
+**username** and **password**: Aruba Central user's *username* and *password*.
+The access token generated by the OAUTH APIs will have the same role/privileges
+as the provided Aruba Central user. * **client_id** and **client_secret**:
 Obtain client_id and client_secret variables by creating an API Gateway client
 in Aruba Central. Refer the following _d_o_c_u_m_e_n_t_a_t_i_o_n for more details. *
-**access_token**: You can create an API access token for Aruba Central from - *
-_A_r_u_b_a_ _C_e_n_t_r_a_l_ _U_I * _O_A_u_t_h_ _A_P_I_s * **customer_id**: Obtain the **customer_id** by
-clicking on the figure icon on top right corner of Aruba Central WebUI. !
-[Customer ID](https://github.com/aruba/pycentral/raw/master/pictures/customer-
-id.png) * **username** and **password**: Aruba Central user's *username* and
-*password*. The access token generated by the OAUTH APIs will have the same
-role/privileges as the provided Aruba Central user. 2. Providing input
+**customer_id**: Obtain the **customer_id** by clicking on the figure icon on
+top right corner of Aruba Central WebUI. ![Customer ID](https://github.com/
+aruba/pycentral/raw/master/pictures/customer-id.png) 2. Providing input
 variables to the Python scripts. One of the following options can be used. *
 Provide variables directly to Aruba Central Base class in dictionary format.
 Access token approach: ```python central_info = { "base_url": "", "token":
 { "access_token": "" } } ``` OAUTH APIs approach with capability to generate
 new access token: ```python central_info = { "username": "", "password": "",
 "client_id": "", "client_secret": "", "customer_id": "", "base_url": "" } ```
-Refer the sample scripts in *step3* and *step4* for examples. * **OR** Provide
-the required variables using JSON/YAML file. Refer input files _s_a_m_p_l_e___s_c_r_i_p_t_s_/
-_i_n_p_u_t___t_o_k_e_n___o_n_l_y_._y_a_m_l and _s_a_m_p_l_e___s_c_r_i_p_t_s_/_i_n_p_u_t___c_r_e_d_e_n_t_i_a_l_s_._y_a_m_l for
-information. Use `pycentral.workflows_utils.get_conn_from_file()` function
-which accepts name of the file and returns the `ArubaCentralBase` instance
-object. Refer the sample script in *step5* for example. 3. **Making API call
-using pycentral base**: Using the base class `ArubaCentralBase`, any Aruba
-Central supported REST API calls can be made. Refer the following sample script
-_s_a_m_p_l_e___s_c_r_i_p_t_s_/_p_y_c_e_n_t_r_a_l___b_a_s_e___s_a_m_p_l_e_._p_y Obtain the HTTP Request related
-information from Aruba Central Swagger documentation or _A_P_I_ _r_e_f_e_r_e_n_c_e_s page in
-Aruba Developer Hub. 4. **Making API call using pycentral modules**: Some API
-endpoints supported by Aruba Central are implemented as modules in the Python
-package. Refer the following sample script using modules _s_a_m_p_l_e___s_c_r_i_p_t_s_/
-_p_y_c_e_n_t_r_a_l___m_o_d_u_l_e___s_a_m_p_l_e_._p_y To obtain a list of implemented modules and its
-documentation refer the _p_y_c_e_n_t_r_a_l_ _m_o_d_u_l_e_ _d_o_c_u_m_e_n_t_a_t_i_o_n 5. **Workflows**:
-Workflows are used to achieve an automation use-case which generally involves
-multiple API calls or dealing with scale and repetitive tasks with ease. Check
-out the _c_e_n_t_r_a_l_-_p_y_t_h_o_n_-_w_o_r_k_f_l_o_w_s_ repository to check out workflows that utilize
-the Pycentral library. ## Documentation: * **Python package documentation:** *
-_p_y_c_e_n_t_r_a_l_ _m_o_d_u_l_e_ _d_o_c_u_m_e_n_t_a_t_i_o_n * **Use-Cases and Workflows:** - _A_r_u_b_a_ _D_e_v_e_l_o_p_e_r
-_H_u_b - _c_e_n_t_r_a_l_-_p_y_t_h_o_n_-_w_o_r_k_f_l_o_w_s ## Note: The package takes one of the two
-approaches to gain access to Aruba Central APIs. * **OAUTH APIs:** By taking
-OAUTH approach to generate new access_token, the python package will cache the
-tokens locally for re-use. Caching tokens locally, helps preventing creation of
-new access_token every time the script is run. In addition, when the
-access_token is expired the script will attempt to use the supplied credentials
-and attempt to refresh the expired token. Override the
-`ArubaCentralBase.storeToken()` and `ArubaCentralBase.loadToken()` function
-definitions to change this behavior of caching in local file(JSON) and manage
-tokens more securely. * **Access Token**: This process is more secure. By
-providing only the *access_token* instead of credentials, the package will not
-cache the tokens. But loses the ability to handle expired token and to generate
-new access tokens. ## How to contribute Please see the accompanying
-_C_O_N_T_R_I_B_U_T_I_O_N_S_._m_d file for guidelines on how to contribute to this repository.
-## Troubleshooting Issues If you encounter module import errors, make sure that
-the package has been installed correctly. Additionally, please read the
-_R_E_L_E_A_S_E_-_N_O_T_E_S_._m_d file for the current release information and known issues.
+Alternatively, you can use **cluster_name** instead of **base_url** in the
+above mentioned dictionaries. You can find the list of clusters that are
+supported in the _c_o_n_s_t_a_n_t_s_._p_y_ _f_i_l_e. If you would like to add support for other
+Central clusters, you can do so by adding it in the constants.py. Refer the
+sample scripts in *step3* and *step4* for examples. * **OR** Provide the
+required variables using JSON/YAML file. Refer to the sample input files to
+understand how the files have to be structured - * _s_a_m_p_l_e___s_c_r_i_p_t_s_/
+_i_n_p_u_t___t_o_k_e_n___o_n_l_y_._y_a_m_l * _s_a_m_p_l_e___s_c_r_i_p_t_s_/_i_n_p_u_t___c_r_e_d_e_n_t_i_a_l_s_._y_a_m_l * _s_a_m_p_l_e___s_c_r_i_p_t_s_/
+_i_n_p_u_t___t_o_k_e_n___o_n_l_y___c_l_u_s_t_e_r___n_a_m_e_._y_a_m_l * _s_a_m_p_l_e___s_c_r_i_p_t_s_/
+_i_n_p_u_t___c_r_e_d_e_n_t_i_a_l_s___c_l_u_s_t_e_r___n_a_m_e_._y_a_m_l More sample input files can be found in the
+_s_a_m_p_l_e___s_c_r_i_p_t_s_ _f_o_l_d_e_r. Use `pycentral.workflows_utils.get_conn_from_file()`
+function which accepts name of the file and returns the `ArubaCentralBase`
+instance object. 3. **Making API call using pycentral base**: Using the base
+class `ArubaCentralBase`, any Aruba Central supported REST API calls can be
+made. Refer the following sample script _s_a_m_p_l_e___s_c_r_i_p_t_s_/_p_y_c_e_n_t_r_a_l___b_a_s_e___s_a_m_p_l_e_._p_y
+Obtain the HTTP Request related information from Aruba Central Swagger
+documentation or _A_P_I_ _r_e_f_e_r_e_n_c_e_s page in Aruba Developer Hub. 4. **Making API
+call using pycentral modules**: Some API endpoints supported by Aruba Central
+are implemented as modules in the Python package. Refer the following sample
+script using modules _s_a_m_p_l_e___s_c_r_i_p_t_s_/_p_y_c_e_n_t_r_a_l___m_o_d_u_l_e___s_a_m_p_l_e_._p_y To obtain a list
+of implemented modules and its documentation refer the _p_y_c_e_n_t_r_a_l_ _m_o_d_u_l_e
+_d_o_c_u_m_e_n_t_a_t_i_o_n 5. **Workflows**: Workflows are used to achieve an automation
+use-case which generally involves multiple API calls or dealing with scale and
+repetitive tasks with ease. Check out the _c_e_n_t_r_a_l_-_p_y_t_h_o_n_-_w_o_r_k_f_l_o_w_s_ repository
+to check out workflows that utilize the Pycentral library. ## Documentation: *
+**Python package documentation:** * _p_y_c_e_n_t_r_a_l_ _m_o_d_u_l_e_ _d_o_c_u_m_e_n_t_a_t_i_o_n * **Use-
+Cases and Workflows:** - _A_r_u_b_a_ _D_e_v_e_l_o_p_e_r_ _H_u_b - _c_e_n_t_r_a_l_-_p_y_t_h_o_n_-_w_o_r_k_f_l_o_w_s ##
+Note: The package takes one of the two approaches to gain access to Aruba
+Central APIs. * **OAUTH APIs:** By taking OAUTH approach to generate new
+access_token, the python package will cache the tokens locally for re-use.
+Caching tokens locally, helps preventing creation of new access_token every
+time the script is run. In addition, when the access_token is expired the
+script will attempt to use the supplied credentials and attempt to refresh the
+expired token. Override the `ArubaCentralBase.storeToken()` and
+`ArubaCentralBase.loadToken()` function definitions to change this behavior of
+caching in local file(JSON) and manage tokens more securely. * **Access
+Token**: This process is more secure. By providing only the *access_token*
+instead of credentials, the package will not cache the tokens. But loses the
+ability to handle expired token and to generate new access tokens. ## How to
+contribute Please see the accompanying _C_O_N_T_R_I_B_U_T_I_O_N_S_._m_d file for guidelines on
+how to contribute to this repository. ## Troubleshooting Issues If you
+encounter module import errors, make sure that the package has been installed
+correctly. Additionally, please read the _R_E_L_E_A_S_E_-_N_O_T_E_S_._m_d file for the current
+release information and known issues.
```

### Comparing `pycentral-1.3/README.md` & `pycentral-1.3.7/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -29,27 +29,29 @@
 
 Now you can start making your script based on modules in pycentral or use different workflows from the subpackage `workflows`.
 
 ## Executing Scripts
 
 1. Gathering variables required for the package base class `ArubaCentralBase`.
 
-    * **base_url**: You can find the base URL of the Central account's API Gateway from the table <a href="https://www.arubanetworks.com/techdocs/central/latest/content/nms/api/domain_url.htm" target="_blank">here</a>. The base URL is based on the geographical Central cluster in which the account is registered.
-
-    * **client_id** and **client_secret**: Obtain client_id and client_secret variables by creating an API Gateway client in Aruba Central. Refer the following <a href="https://developer.arubanetworks.com/aruba-central/docs/api-gateway-creating-application-token" target="_blank">documentation</a> for more details.
+    * **base_url** OR **cluster_name**: You can find the base URL or cluster name of the Central account's API Gateway from the table <a href="https://www.arubanetworks.com/techdocs/central/latest/content/nms/api/domain_url.htm" target="_blank">here</a>. The base URL or cluster name is based on the geographical Central cluster in which the account is registered.
 
    * **access_token**: You can create an API access token for Aruba Central from -
       * <a href="https://developer.arubanetworks.com/aruba-central/docs/api-gateway-obtaining-access-tokens#obtain-access-token-via-web-ui" target="_blank">Aruba Central UI</a>
       * <a href="https://developer.arubanetworks.com/aruba-central/docs/api-oauth-access-token" target="_blank">OAuth APIs</a>
 
-    * **customer_id**: Obtain the **customer_id** by clicking on the figure icon on top right corner of Aruba Central WebUI.
+    * Optional variables - You need to provide the below variables if you want to use PyCentral's ability to generate access tokens from Aruba Central with the help of OAuth APIs.
+      * **username** and **password**: Aruba Central user's *username* and *password*. The access token generated by the OAUTH APIs will have the same role/privileges as the provided Aruba Central user.
+  
+      * **client_id** and **client_secret**: Obtain client_id and client_secret variables by creating an API Gateway client in Aruba Central. Refer the following <a href="https://developer.arubanetworks.com/aruba-central/docs/api-gateway-creating-application-token" target="_blank">documentation</a> for more details.
+    
+      * **customer_id**: Obtain the **customer_id** by clicking on the figure icon on top right corner of Aruba Central WebUI.
 
     ![Customer ID](https://github.com/aruba/pycentral/raw/master/pictures/customer-id.png)
 
-    * **username** and **password**: Aruba Central user's *username* and *password*. The access token generated by the OAUTH APIs will have the same role/privileges as the provided Aruba Central user.
 
 2. Providing input variables to the Python scripts. One of the following options can be used.
     * Provide variables directly to Aruba Central Base class in dictionary format.
 
         Access token approach:
         ```python
         central_info = {
@@ -67,21 +69,25 @@
                 "password": "<aruba-central-account-password>",
                 "client_id": "<api-gateway-client-id>",
                 "client_secret": "<api-gateway-client-secret>",
                 "customer_id": "<aruba-central-customer-id>",
                 "base_url": "<api-gateway-domain-url>"
             }
         ```
-
+        Alternatively, you can use **cluster_name** instead of **base_url** in the above mentioned dictionaries. You can find the list of clusters that are supported in the <a href="https://github.com/aruba/pycentral/blob/master/pycentral/constants.py" target="_blank">constants.py file</a>. If you would like to add support for other Central clusters, you can do so by adding it in the constants.py. 
         Refer the sample scripts in *step3* and *step4* for examples.
 
-    * **OR** Provide the required variables using JSON/YAML file. Refer input files <a href="https://github.com/aruba/pycentral/blob/master/sample_scripts/input_token_only.yaml" target="_blank">sample_scripts/input_token_only.yaml</a> and <a href="https://github.com/aruba/pycentral/blob/master/sample_scripts/input_credentials.yaml" target="_blank">sample_scripts/input_credentials.yaml</a> for information.
+    * **OR** Provide the required variables using JSON/YAML file. Refer to the sample input files to understand how the files have to be structured -
+      * <a href="https://github.com/aruba/pycentral/blob/master/sample_scripts/input_token_only.yaml" target="_blank">sample_scripts/input_token_only.yaml</a>
+      * <a href="https://github.com/aruba/pycentral/blob/master/sample_scripts/input_credentials.yaml" target="_blank">sample_scripts/input_credentials.yaml</a> 
+      * <a href="https://github.com/aruba/pycentral/blob/master/sample_scripts/sample_scripts/input_token_only_cluster.yaml" target="_blank">sample_scripts/input_token_only_cluster_name.yaml</a>
+      * <a href="https://github.com/aruba/pycentral/blob/master/sample_scripts/sample_scripts/input_credentials_cluster_name.yaml" target="_blank">sample_scripts/input_credentials_cluster_name.yaml</a>
 
-        Use `pycentral.workflows_utils.get_conn_from_file()` function which accepts name of the file and returns
-        the `ArubaCentralBase` instance object. Refer the sample script in *step5* for example.
+        More sample input files can be found in the <a href="https://github.com/aruba/pycentral/blob/master/sample_scripts/sample_scripts/" target="_blank">sample_scripts folder</a>. Use `pycentral.workflows_utils.get_conn_from_file()` function which accepts name of the file and returns
+        the `ArubaCentralBase` instance object.
 
 3. **Making API call using pycentral base**: Using the base class `ArubaCentralBase`, any Aruba Central supported REST API calls can be made. Refer the following sample script <a href="https://github.com/aruba/pycentral/blob/master/sample_scripts/pycentral_base_sample.py" target="_blank">sample_scripts/pycentral_base_sample.py</a>
 
     Obtain the HTTP Request related information from Aruba Central Swagger documentation or <a href="https://developer.arubanetworks.com/aruba-central/reference" target="_blank">API references</a> page in Aruba Developer Hub.
 
 4. **Making API call using pycentral modules**: Some API endpoints supported by Aruba Central are implemented as modules in the Python package. Refer the following sample script using modules <a href="https://github.com/aruba/pycentral/blob/master/sample_scripts/pycentral_module_sample.py" target="_blank">sample_scripts/pycentral_module_sample.py</a>
```

#### html2text {}

```diff
@@ -10,62 +10,72 @@
 virtual env ``` $ source centralenv/bin/activate in Windows: $ centralenv/
 Scripts/activate.bat ``` 3. Install the **pycentral** package ``` (centralenv)$
 pip3 install pycentral ``` To install package with *extras* `colorLog` which
 will display log in color ``` (centralenv)$ pip3 install pycentral[colorLog]
 ``` Now you can start making your script based on modules in pycentral or use
 different workflows from the subpackage `workflows`. ## Executing Scripts 1.
 Gathering variables required for the package base class `ArubaCentralBase`. *
-**base_url**: You can find the base URL of the Central account's API Gateway
-from the table _h_e_r_e. The base URL is based on the geographical Central cluster
-in which the account is registered. * **client_id** and **client_secret**:
+**base_url** OR **cluster_name**: You can find the base URL or cluster name of
+the Central account's API Gateway from the table _h_e_r_e. The base URL or cluster
+name is based on the geographical Central cluster in which the account is
+registered. * **access_token**: You can create an API access token for Aruba
+Central from - * _A_r_u_b_a_ _C_e_n_t_r_a_l_ _U_I * _O_A_u_t_h_ _A_P_I_s * Optional variables - You need
+to provide the below variables if you want to use PyCentral's ability to
+generate access tokens from Aruba Central with the help of OAuth APIs. *
+**username** and **password**: Aruba Central user's *username* and *password*.
+The access token generated by the OAUTH APIs will have the same role/privileges
+as the provided Aruba Central user. * **client_id** and **client_secret**:
 Obtain client_id and client_secret variables by creating an API Gateway client
 in Aruba Central. Refer the following _d_o_c_u_m_e_n_t_a_t_i_o_n for more details. *
-**access_token**: You can create an API access token for Aruba Central from - *
-_A_r_u_b_a_ _C_e_n_t_r_a_l_ _U_I * _O_A_u_t_h_ _A_P_I_s * **customer_id**: Obtain the **customer_id** by
-clicking on the figure icon on top right corner of Aruba Central WebUI. !
-[Customer ID](https://github.com/aruba/pycentral/raw/master/pictures/customer-
-id.png) * **username** and **password**: Aruba Central user's *username* and
-*password*. The access token generated by the OAUTH APIs will have the same
-role/privileges as the provided Aruba Central user. 2. Providing input
+**customer_id**: Obtain the **customer_id** by clicking on the figure icon on
+top right corner of Aruba Central WebUI. ![Customer ID](https://github.com/
+aruba/pycentral/raw/master/pictures/customer-id.png) 2. Providing input
 variables to the Python scripts. One of the following options can be used. *
 Provide variables directly to Aruba Central Base class in dictionary format.
 Access token approach: ```python central_info = { "base_url": "", "token":
 { "access_token": "" } } ``` OAUTH APIs approach with capability to generate
 new access token: ```python central_info = { "username": "", "password": "",
 "client_id": "", "client_secret": "", "customer_id": "", "base_url": "" } ```
-Refer the sample scripts in *step3* and *step4* for examples. * **OR** Provide
-the required variables using JSON/YAML file. Refer input files _s_a_m_p_l_e___s_c_r_i_p_t_s_/
-_i_n_p_u_t___t_o_k_e_n___o_n_l_y_._y_a_m_l and _s_a_m_p_l_e___s_c_r_i_p_t_s_/_i_n_p_u_t___c_r_e_d_e_n_t_i_a_l_s_._y_a_m_l for
-information. Use `pycentral.workflows_utils.get_conn_from_file()` function
-which accepts name of the file and returns the `ArubaCentralBase` instance
-object. Refer the sample script in *step5* for example. 3. **Making API call
-using pycentral base**: Using the base class `ArubaCentralBase`, any Aruba
-Central supported REST API calls can be made. Refer the following sample script
-_s_a_m_p_l_e___s_c_r_i_p_t_s_/_p_y_c_e_n_t_r_a_l___b_a_s_e___s_a_m_p_l_e_._p_y Obtain the HTTP Request related
-information from Aruba Central Swagger documentation or _A_P_I_ _r_e_f_e_r_e_n_c_e_s page in
-Aruba Developer Hub. 4. **Making API call using pycentral modules**: Some API
-endpoints supported by Aruba Central are implemented as modules in the Python
-package. Refer the following sample script using modules _s_a_m_p_l_e___s_c_r_i_p_t_s_/
-_p_y_c_e_n_t_r_a_l___m_o_d_u_l_e___s_a_m_p_l_e_._p_y To obtain a list of implemented modules and its
-documentation refer the _p_y_c_e_n_t_r_a_l_ _m_o_d_u_l_e_ _d_o_c_u_m_e_n_t_a_t_i_o_n 5. **Workflows**:
-Workflows are used to achieve an automation use-case which generally involves
-multiple API calls or dealing with scale and repetitive tasks with ease. Check
-out the _c_e_n_t_r_a_l_-_p_y_t_h_o_n_-_w_o_r_k_f_l_o_w_s_ repository to check out workflows that utilize
-the Pycentral library. ## Documentation: * **Python package documentation:** *
-_p_y_c_e_n_t_r_a_l_ _m_o_d_u_l_e_ _d_o_c_u_m_e_n_t_a_t_i_o_n * **Use-Cases and Workflows:** - _A_r_u_b_a_ _D_e_v_e_l_o_p_e_r
-_H_u_b - _c_e_n_t_r_a_l_-_p_y_t_h_o_n_-_w_o_r_k_f_l_o_w_s ## Note: The package takes one of the two
-approaches to gain access to Aruba Central APIs. * **OAUTH APIs:** By taking
-OAUTH approach to generate new access_token, the python package will cache the
-tokens locally for re-use. Caching tokens locally, helps preventing creation of
-new access_token every time the script is run. In addition, when the
-access_token is expired the script will attempt to use the supplied credentials
-and attempt to refresh the expired token. Override the
-`ArubaCentralBase.storeToken()` and `ArubaCentralBase.loadToken()` function
-definitions to change this behavior of caching in local file(JSON) and manage
-tokens more securely. * **Access Token**: This process is more secure. By
-providing only the *access_token* instead of credentials, the package will not
-cache the tokens. But loses the ability to handle expired token and to generate
-new access tokens. ## How to contribute Please see the accompanying
-_C_O_N_T_R_I_B_U_T_I_O_N_S_._m_d file for guidelines on how to contribute to this repository.
-## Troubleshooting Issues If you encounter module import errors, make sure that
-the package has been installed correctly. Additionally, please read the
-_R_E_L_E_A_S_E_-_N_O_T_E_S_._m_d file for the current release information and known issues.
+Alternatively, you can use **cluster_name** instead of **base_url** in the
+above mentioned dictionaries. You can find the list of clusters that are
+supported in the _c_o_n_s_t_a_n_t_s_._p_y_ _f_i_l_e. If you would like to add support for other
+Central clusters, you can do so by adding it in the constants.py. Refer the
+sample scripts in *step3* and *step4* for examples. * **OR** Provide the
+required variables using JSON/YAML file. Refer to the sample input files to
+understand how the files have to be structured - * _s_a_m_p_l_e___s_c_r_i_p_t_s_/
+_i_n_p_u_t___t_o_k_e_n___o_n_l_y_._y_a_m_l * _s_a_m_p_l_e___s_c_r_i_p_t_s_/_i_n_p_u_t___c_r_e_d_e_n_t_i_a_l_s_._y_a_m_l * _s_a_m_p_l_e___s_c_r_i_p_t_s_/
+_i_n_p_u_t___t_o_k_e_n___o_n_l_y___c_l_u_s_t_e_r___n_a_m_e_._y_a_m_l * _s_a_m_p_l_e___s_c_r_i_p_t_s_/
+_i_n_p_u_t___c_r_e_d_e_n_t_i_a_l_s___c_l_u_s_t_e_r___n_a_m_e_._y_a_m_l More sample input files can be found in the
+_s_a_m_p_l_e___s_c_r_i_p_t_s_ _f_o_l_d_e_r. Use `pycentral.workflows_utils.get_conn_from_file()`
+function which accepts name of the file and returns the `ArubaCentralBase`
+instance object. 3. **Making API call using pycentral base**: Using the base
+class `ArubaCentralBase`, any Aruba Central supported REST API calls can be
+made. Refer the following sample script _s_a_m_p_l_e___s_c_r_i_p_t_s_/_p_y_c_e_n_t_r_a_l___b_a_s_e___s_a_m_p_l_e_._p_y
+Obtain the HTTP Request related information from Aruba Central Swagger
+documentation or _A_P_I_ _r_e_f_e_r_e_n_c_e_s page in Aruba Developer Hub. 4. **Making API
+call using pycentral modules**: Some API endpoints supported by Aruba Central
+are implemented as modules in the Python package. Refer the following sample
+script using modules _s_a_m_p_l_e___s_c_r_i_p_t_s_/_p_y_c_e_n_t_r_a_l___m_o_d_u_l_e___s_a_m_p_l_e_._p_y To obtain a list
+of implemented modules and its documentation refer the _p_y_c_e_n_t_r_a_l_ _m_o_d_u_l_e
+_d_o_c_u_m_e_n_t_a_t_i_o_n 5. **Workflows**: Workflows are used to achieve an automation
+use-case which generally involves multiple API calls or dealing with scale and
+repetitive tasks with ease. Check out the _c_e_n_t_r_a_l_-_p_y_t_h_o_n_-_w_o_r_k_f_l_o_w_s_ repository
+to check out workflows that utilize the Pycentral library. ## Documentation: *
+**Python package documentation:** * _p_y_c_e_n_t_r_a_l_ _m_o_d_u_l_e_ _d_o_c_u_m_e_n_t_a_t_i_o_n * **Use-
+Cases and Workflows:** - _A_r_u_b_a_ _D_e_v_e_l_o_p_e_r_ _H_u_b - _c_e_n_t_r_a_l_-_p_y_t_h_o_n_-_w_o_r_k_f_l_o_w_s ##
+Note: The package takes one of the two approaches to gain access to Aruba
+Central APIs. * **OAUTH APIs:** By taking OAUTH approach to generate new
+access_token, the python package will cache the tokens locally for re-use.
+Caching tokens locally, helps preventing creation of new access_token every
+time the script is run. In addition, when the access_token is expired the
+script will attempt to use the supplied credentials and attempt to refresh the
+expired token. Override the `ArubaCentralBase.storeToken()` and
+`ArubaCentralBase.loadToken()` function definitions to change this behavior of
+caching in local file(JSON) and manage tokens more securely. * **Access
+Token**: This process is more secure. By providing only the *access_token*
+instead of credentials, the package will not cache the tokens. But loses the
+ability to handle expired token and to generate new access tokens. ## How to
+contribute Please see the accompanying _C_O_N_T_R_I_B_U_T_I_O_N_S_._m_d file for guidelines on
+how to contribute to this repository. ## Troubleshooting Issues If you
+encounter module import errors, make sure that the package has been installed
+correctly. Additionally, please read the _R_E_L_E_A_S_E_-_N_O_T_E_S_._m_d file for the current
+release information and known issues.
```

### Comparing `pycentral-1.3/pycentral/audit_logs.py` & `pycentral-1.3.7/pycentral/audit_logs.py`

 * *Files identical despite different names*

### Comparing `pycentral-1.3/pycentral/base.py` & `pycentral-1.3.7/pycentral/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,20 @@
         * keyword client_id: (Optional) API Gateway client_id string, Provide\
             for OAUTH2.0 and refresh token API. \n
         * keyword client_secret: (Optional) API Gateway client_secret string,\
             Provide for OAUTH2.0 and refresh token API. \n
         * keyword customer_id: (Optional) API Gateway client_secret string,\
             Provide for OAUTH2.0 and refresh token API. \n
         * keyword base_url: Provide the API Gateway string base FQDN in format\
-            `https://<Aruba-Central-API-Gateway-Domain-Name>` \n
+            `https://<Aruba-Central-API-Gateway-Domain-Name>` You need to \
+            provide either a base_url or cluster_name. \n
+        * keyword cluster_name: Provide the name of the cluster where the\
+            Aruba Central account is provisioned. You need to provide either a\
+            base_url or cluster_name. You can find the list of supported\
+            clusters in the constants.py file. \n
         * keyword token: (Optional) The token dict is mutually excluive with\
             OAUTH2.0 parameters. token dict should consist of the following\
             key-value pairs - \n
                 {"access_token": "xxxx", "refresh_token": "XXYY"}\n
     :type central_info: dict
     :param token_store: Placeholder for future development which provides\
         options to secrely cache and reuse access tokens. defaults to None
```

### Comparing `pycentral-1.3/pycentral/base_utils.py` & `pycentral-1.3.7/pycentral/workflows/workflows_utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -16,156 +16,139 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-import logging
+import sys
 import os
-from urllib.parse import urlencode, urlparse, urlunparse
-try:
-    import colorlog  # type: ignore
-    COLOR = True
-except (ImportError, ModuleNotFoundError):
-    COLOR = False
-
-C_LOG_LEVEL = {
-    "CRITICAL": 50,
-    "ERROR": 40,
-    "WARNING": 30,
-    "INFO": 20,
-    "DEBUG": 10,
-    "NOTSET": 0
-}
-
-C_DEFAULT_ARGS = {
-    "base_url": None,
-    "client_id": None,
-    "client_secret": None,
-    "customer_id": None,
-    "username": None,
-    "password": None,
-    "token": None
-}
-
-
-def parseInputArgs(central_info):
-    """This method parses user input, checks for the availability of mandatory\
-        arguments. Optional missing parameters in central_info variable is\
-        initialized as defined in C_DEFAULT_ARGS.
-
-    :param central_info: central_info dictionary as read from user's input\
-        file.
-    :type central_info: dict
-    :return: parsed central_info dict with missing optional params set to\
-        default values.
-    :rtype: dict
+import json
+import yaml
+import csv
+
+from pycentral.base import ArubaCentralBase
+
+
+def get_file_contents(filename, logger=None):
+    """Function to open a JSON/YAML/CSV file and return the contents of the\
+        file in dict format. (A list of dict is returned for a CSV file.)
+
+    :param filename: Name of an existing JSON/YAML/CSV file.
+    :type filename: str
+    :param logger: Provide an instance of class:`logging.logger`.
+    :type logger: class:`logging.logger`, optional
+    :raises UserWarning: Raises warning when supported filetypes are not\
+        provided.
+    :return: Data loaded from JSON/YAML/CSV file
+    :rtype: dict (a list of dict for CSV)
     """
-    if not central_info:
-        exit("Error: Invalid Input!")
-
-    # Mandatory input arg
-    if "base_url" not in central_info:
-        exit("Error: Provide base_url for API Gateway!")
-
-    default_dict = dict(C_DEFAULT_ARGS)
-    for key in default_dict.keys():
-        if key in central_info:
-            default_dict[key] = central_info[key]
-
-    return default_dict
-
-
-def tokenLocalStoreUtil(token_store, customer_id="customer",
-                        client_id="client"):
-    """Utility function for storeToken and loadToken default access token\
-        storage/cache method. This function generates unique file name for a\
-        customer and API gateway client to store and load access token in the\
-        local machine for reuse. The format of the file name is\
-        tok_<customer_id>_<client_id>.json. If customer_id or client_id is not\
-        provided, default values mentioned in args will be used.
-
-    :param token_store: Placeholder to support different token storage\
-        mechanism. \n
-        * keyword type: Place holder for different token storage mechanism.\
-            Defaults to local storage. \n
-        * keyword path: path where temp folder is created to store token JSON\
-            file. \n
-    :type token_store: dict
-    :param customer_id: Aruba Central customer id, defaults to "customer"
-    :type customer_id: str, optional
-    :param client_id: API Gateway client id, defaults to "client"
-    :type client_id: str, optional
-    :return: Filename for access token storage.
-    :rtype: str
-    """
-    fileName = "tok_" + str(customer_id)
-    fileName = fileName + "_" + str(client_id) + ".json"
-    filePath = os.path.join(os.getcwd(), "temp")
-    if token_store and "path" in token_store:
-        filePath = os.path.join(token_store["path"])
-    fullName = os.path.join(filePath, fileName)
-    return fullName
-
-
-def get_url(base_url, path='', params='', query={}, fragment=''):
-    """This method constructs complete URL based on multiple parts of URL.
-
-    :param base_url: base url for a HTTP request
-    :type base_url: str
-    :param path: API endpoint path, defaults to ''
-    :type path: str, optional
-    :param params: API endpoint path parameters, defaults to ''
-    :type params: str, optional
-    :param query: HTTP request url query parameters, defaults to {}
-    :type query: dict, optional
-    :param fragment: URL fragment identifier, defaults to ''
-    :type fragment: str, optional
-    :return: Parsed URL
-    :rtype: class:`urllib.parse.ParseResult`
-    """
-    parsed_baseurl = urlparse(base_url)
-    scheme = parsed_baseurl.scheme
-    netloc = parsed_baseurl.netloc
-    query = urlencode(query)
-    url = urlunparse((scheme, netloc, path, params, query, fragment))
-    return url
-
-
-def console_logger(name, level="DEBUG"):
-    """This method create an instance of python logging and sets the following\
-        format for log messages.\n<date> <time> - <name> - <level> - <message>
-
-    :param name: String displayed after data and time. Define it to identify\
-        from which part of the code, log message is generated.
-    :type name: str
-    :param level: Loggin level set to display messages from a certain logging\
-        level. Refer Python logging library man page, defaults to "DEBUG"
-    :type level: str, optional
-    :return: An instance of class logging
-    :rtype: class:`logging.Logger`
+    read_data = {}
+    try:
+        with open(filename, "r") as fp:
+            file_dummy, file_ext = os.path.splitext(filename)
+            if ".json" in file_ext:
+                read_data = json.loads(fp.read())
+            elif file_ext in ['.yaml', '.yml']:
+                read_data = yaml.safe_load(fp.read())
+            elif ".csv" in file_ext:
+                read_data = list(csv.DictReader(open(filename)))
+            else:
+                raise UserWarning("Provide valid file with"
+                                  "format/extension [.json/.yaml/.yml/.csv]!")
+        return read_data
+    except FileNotFoundError:
+        if logger:
+            logger.error("File %s not found.." % filename)
+        else:
+            print("File %s Not Found!" % filename)
+    except Exception as err:
+        if logger:
+            logger.error("Error reading file %s: %s" % (filename, str(err)))
+        else:
+            print(str(err))
+
+
+def dict_list_to_csv(filename, csv_data_list, logger=None):
+    """Write list of dictionaries into a CSV File via csv.DictWriter()
+
+    :param filename: Name of the file to be created or overwritten
+    :type filename: str
+    :param csv_data_list: A list of dictionaries, where each dict is a row in\
+        CSV file
+    :type csv_data_list: list
+    :param logger: Provide an instance of class:`logging.logger`.
+    :type logger: class:`logging.logger`, optional
     """
-    channel_handler = logging.StreamHandler()
-    format = "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
-    date_format = '%Y-%m-%d %H:%M:%S'
-    f = format
-    if COLOR:
-        cformat = '%(log_color)s' + format
-        f = colorlog.ColoredFormatter(
-            cformat,
-            date_format,
-            log_colors={
-                'DEBUG': 'bold_cyan',
-                'INFO': 'blue',
-                'WARNING': 'yellow',
-                'ERROR': 'red',
-                'CRITICAL': 'bold_red'})
+    csv_columns = []
+    if csv_data_list and csv_data_list[0]:
+        csv_columns = list(csv_data_list[0].keys())
     else:
-        f = logging.Formatter(format, date_format)
-    channel_handler.setFormatter(f)
-
-    logger = logging.getLogger(name)
-    logger.setLevel(C_LOG_LEVEL[level])
-    logger.addHandler(channel_handler)
-
-    return logger
+        if logger:
+            logger.warning("No data to write to a CSV file...")
+        return
+    try:
+        with open(filename, 'w') as csvfile:
+            writer = csv.DictWriter(csvfile, fieldnames=csv_columns)
+            writer.writeheader()
+            for data in csv_data_list:
+                writer.writerow(data)
+        if logger:
+            logger.info(
+                "Creating a new csv file '%s' with failed APs..." %
+                filename)
+    except IOError:
+        print("I/O error")
+    except Exception as err:
+        if logger:
+            logger.error("Error writing to file %s: %s" % (filename, str(err)))
+        else:
+            print(str(err))
+
+
+def get_conn_from_file(filename, account=None, logger=None):
+    """Creates an instance of class`pycentral.ArubaCentralBase` based on the\
+        information
+    provided in the YAML/JSON file. \n
+        * keyword central_info: A dict containing arguments as accepted by\
+            class`pycentral.ArubaCentralBase` \n
+        * keyword ssl_verify: A boolean when set to True, the python client\
+            validates Aruba Central's SSL certs. \n
+        * keyword token_store: Optional. Defaults to None. \n
+
+    :param filename: Name of a JSON/YAML file containing the keywords required\
+        for class:`pycentral.ArubaCentralBase`
+    :type filename: str
+    :param logger: Provide an instance of class:`logging.logger`, defaults to\
+        logger class with name "ARUBA_BASE".
+    :type logger: class:`logging.logger`, optional
+    :return: An instance of class:`pycentral.ArubaCentralBase` to make API\
+        calls and manage access tokens.
+    :rtype: class:`pycentral.ArubaCentralBase`
+    """
+    conn = None
+    token_store = None
+    ssl_verify = True
+
+    input_args = get_file_contents(filename=filename, logger=logger)
+    if not input_args:
+        sys.exit("Unable to get the file content... exiting!")
+    # if "central_info" not in input_args:
+    #     sys.exit("exiting... Provide central_info in the file %s" % filename)
+    # central_info = input_args["central_info"]
+
+    if account is None:
+        account = "central_info"
+    if account not in input_args:
+        sys.exit("exiting... Provide %s in the file %s" % (account, filename))
+    central_info = input_args[account]
+
+    if "token_store" in input_args:
+        token_store = input_args["token_store"]
+    if "ssl_verify" in input_args:
+        ssl_verify = input_args["ssl_verify"]
+
+    conn = ArubaCentralBase(central_info=central_info,
+                            token_store=token_store,
+                            ssl_verify=ssl_verify,
+                            logger=logger)
+    return conn
```

### Comparing `pycentral-1.3/pycentral/configuration.py` & `pycentral-1.3.7/pycentral/configuration.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-import sys
 from pycentral.url_utils import ConfigurationUrl, urlJoin
 from pycentral.base_utils import console_logger
 
 urls = ConfigurationUrl()
 DEVICE_TYPES = ["IAP", "ArubaSwitch", "CX", "MobilityController"]
 logger = console_logger("CONFIGURATION")
 
@@ -1048,20 +1047,149 @@
         :rtype: dict
         """
         path = urlJoin(urls.AP_CONFIGURATION["REPLACE"], group_name)
         resp = conn.command(apiMethod="POST", apiPath=path, apiData=data)
 
         return resp
 
+    def change_wlan_status(self, conn, group_name, wlan_name, new_wlan_status):
+        """
+        This function lets you enable or disable the specified WLAN in a UI \
+        group. 
+
+        :param conn: Instance of class:`pycentral.ArubaCentralBase` to make an
+            API call.
+        :type conn: class:`pycentral.ArubaCentralBase`
+        :param group_name: Name of Aruba Central group which has the WLAN
+        :type group_name: str
+        :param wlan_name: Name of WLAN whose status has to be changed
+        :type wlan_name: str
+        :param new_wlan_status: Status of WLAN - True => Enable WLAN, \
+        False => Disable WLAN
+        :type new_wlan_status: bool
+
+        :return: True when WLAN status was updated successfully. Otherwise, it\
+            will return False
+        :rtype: bool
+        """
+        wlan_action = "enable" if new_wlan_status else "disable"
+        ap_config_resp = self.get_ap_config(conn, group_name)
+        if ap_config_resp['code'] != 200:
+            resp = ap_config_resp
+            logger.error(
+                f'Unable to {wlan_action} WLAN {wlan_name}. \nError code {resp["code"]}. Error Message - {resp["msg"]}')
+            return False
+
+        ap_config = ap_config_resp['msg']
+        wlan_list = self._parse_wlans_from_ap_config(ap_config)
+        if wlan_name not in wlan_list.keys():
+            logger.error(
+                f'Unable to find WLAN {wlan_name} in group {group_name}.\n Please provide a valid WLAN to {wlan_action}')
+            return False
+
+        new_wlan_config = self._update_wlan_status_ap_config(
+            wlan_list[wlan_name]['config'], wlan_action)
+        wlan_config_index = wlan_list[wlan_name]['config_start_index']
+        new_ap_config = self._update_wlan_in_ap_cli_config(
+            ap_config, new_wlan_config, wlan_config_index)
+        ap_config_resp = self.replace_ap(
+            conn, group_name=group_name, data={"clis": new_ap_config})
+        if ap_config_resp['code'] == 200 and ap_config_resp['msg'] == group_name:
+            logger.info(f'Successfully {wlan_action}d WLAN {wlan_name}')
+            return True
+        else:
+            logger.error(
+                f'Unable to {wlan_action} WLAN {wlan_name}. \nError code {ap_config_resp["code"]}. Error Message - {ap_config_resp["msg"]}')
+            return False
+
+    def _parse_wlans_from_ap_config(self, ap_config):
+        """
+        This function lets you parse out WLANs from a given AP configuration
+
+        :param ap_config: Whole configuration in CLI format of an UI group
+        :type ap_config: list
+
+        :return: Dictionary of WLAN with WLAN Configuration in CLI format & \
+            index of WLAN CLI Configuration
+        :rtype: dict
+        """
+        empty_space = '  '
+        wlans = {}
+        current_wlan = None
+        wlan_prefix = 'wlan ssid-profile '
+        for index, config_line in enumerate(ap_config):
+            if config_line.startswith(wlan_prefix):
+                wlan_name = config_line[len(wlan_prefix):]
+                current_wlan = wlan_name
+                wlans[wlan_name] = {
+                    'config': [config_line],
+                    'config_start_index': index
+                }
+            elif config_line.startswith(empty_space) and current_wlan:
+                wlans[current_wlan]['config'].append(config_line)
+            elif current_wlan:
+                current_wlan = None
+        return wlans
+
+    def _update_wlan_status_ap_config(self, ap_wlan_config, wlan_action):
+        """
+        This function updates the status of WLAN in WLAN configuration in CLI\
+        format.
+
+        :param ap_wlan_config: WLAN Configuration in CLI format
+        :type ap_wlan_config: list
+        :param wlan_action: Status that WLAN will be updated to. The action \
+            can either be enable or disable
+        :type wlan_action: str
+
+        :return: Updated WLAN Configuration in CLI format
+        :rtype: list
+        """
+        wlan_actions = ["enable", "disable"]
+        wlan_opp_action = list(
+            filter(lambda x: x != wlan_action, wlan_actions))[0]
+        empty_space = '  '
+        for index, config_line in enumerate(ap_wlan_config):
+            if (config_line == (empty_space + wlan_action)):
+                return ap_wlan_config
+            elif (config_line == (empty_space + wlan_opp_action)):
+                ap_wlan_config[index] = (empty_space + wlan_action)
+                return ap_wlan_config
+
+    def _update_wlan_in_ap_cli_config(self, old_ap_config, new_wlan_config, wlan_start_index):
+        """
+        This function changes the WLAN configuration in the group\
+        configuration in CLI format.
+
+        :param old_ap_config: AP Configuration in CLI format
+        :type old_ap_config: list
+        :param new_wlan_config: WLAN Configuration in CLI format
+        :type new_wlan_config: list
+        :param wlan_start_index: Index of WLAN Configuration Status that WLAN\
+            will be updated to. The action can either be enable or disable
+        :type wlan_start_index: int
+
+        :return: Updated WLAN Configuration in CLI format
+        :rtype: list
+        """
+        endIndex = wlan_start_index + len(new_wlan_config)
+        old_ap_config[wlan_start_index:endIndex] = new_wlan_config
+        return old_ap_config
+
 
 class Wlan(object):
     """A python class consisting of functions to manage Aruba Central WLANs
-    via REST API.
+    via REST API. This class uses WLAN APIs that have to be allowlisted for
+    the Aruba Central account
     """
 
+    def __init__(self):
+        logger.info(
+            'The WLAN class\'s APIs have to be allowlisted for the Aruba Central account.')
+
     def create_wlan(self, conn, group_name, wlan_name, wlan_data):
         """
         Create new WLAN.
 
         :param conn: Instance of class:`pycentral.ArubaCentralBase` to make an
             API call.
         :type conn: class:`pycentral.ArubaCentralBase`
@@ -1188,15 +1316,15 @@
         """
         path = urlJoin(urls.WLAN["UPDATE_FULL"], group_name, wlan_name)
         resp = conn.command(apiMethod="PUT", apiPath=path, apiData=wlan_data)
         return resp
 
     def get_wlan(self, conn, group_name, wlan_name):
         """
-        Gets full configuration of a WLAN in a Central group.
+        Gets configuration of a WLAN in a Central group.
 
         :param conn: Instance of class:`pycentral.ArubaCentralBase` to make an
             API call.
         :type conn: class:`pycentral.ArubaCentralBase`
         :param group_name: Group name of the group or guid of the swarm.
         :type group_name: str
         :param wlan_name: Name string for wlan to get.
@@ -1224,7 +1352,38 @@
         :return: Response as provided by 'command' function in class:
             `pycentral.ArubaCentralBase`.
         :rtype: dict
         """
         path = urlJoin(urls.WLAN["GET_ALL"], group_name)
         resp = conn.command(apiMethod="GET", apiPath=path)
         return resp
+
+    def enable_wlan(self, conn, group_name, wlan_name):
+        """
+        This function will enable the WLAN for client connections.
+
+        :param conn: Instance of class:`pycentral.ArubaCentralBase` to make an
+            API call.
+        :type conn: class:`pycentral.ArubaCentralBase`
+        :param group_name: Name of Aruba Central UI group which has the WLAN
+        :type group_name: str
+        :param wlan_name: Name of WLAN which has to be enabled
+        :type wlan_name: str
+        """
+        a = ApConfiguration()
+        a.change_wlan_status(conn, group_name, wlan_name, True)
+
+    def disable_wlan(self, conn, group_name, wlan_name):
+        """
+        This function will disable the WLAN for client connections. Current 
+        connected clients will be disconnected from this WLAN.
+
+        :param conn: Instance of class:`pycentral.ArubaCentralBase` to make an
+            API call.
+        :type conn: class:`pycentral.ArubaCentralBase`
+        :param group_name: Name of Aruba Central UI group which has the WLAN
+        :type group_name: str
+        :param wlan_name: Name of WLAN which has to be disabled
+        :type wlan_name: str
+        """
+        a = ApConfiguration()
+        a.change_wlan_status(conn, group_name, wlan_name, False)
```

### Comparing `pycentral-1.3/pycentral/device_inventory.py` & `pycentral-1.3.7/pycentral/device_inventory.py`

 * *Files identical despite different names*

### Comparing `pycentral-1.3/pycentral/firmware_management.py` & `pycentral-1.3.7/pycentral/firmware_management.py`

 * *Files identical despite different names*

### Comparing `pycentral-1.3/pycentral/licensing.py` & `pycentral-1.3.7/pycentral/licensing.py`

 * *Files identical despite different names*

### Comparing `pycentral-1.3/pycentral/monitoring.py` & `pycentral-1.3.7/pycentral/monitoring.py`

 * *Files identical despite different names*

### Comparing `pycentral-1.3/pycentral/msp.py` & `pycentral-1.3.7/pycentral/msp.py`

 * *Files identical despite different names*

### Comparing `pycentral-1.3/pycentral/rapids.py` & `pycentral-1.3.7/pycentral/rapids.py`

 * *Files identical despite different names*

### Comparing `pycentral-1.3/pycentral/refresh_api_token.py` & `pycentral-1.3.7/pycentral/refresh_api_token.py`

 * *Files identical despite different names*

### Comparing `pycentral-1.3/pycentral/topology.py` & `pycentral-1.3.7/pycentral/topology.py`

 * *Files identical despite different names*

### Comparing `pycentral-1.3/pycentral/url_utils.py` & `pycentral-1.3.7/pycentral/url_utils.py`

 * *Files identical despite different names*

### Comparing `pycentral-1.3/pycentral/user_management.py` & `pycentral-1.3.7/pycentral/user_management.py`

 * *Files identical despite different names*

### Comparing `pycentral-1.3/pycentral/visualrf.py` & `pycentral-1.3.7/pycentral/visualrf.py`

 * *Files identical despite different names*

### Comparing `pycentral-1.3/pycentral.egg-info/PKG-INFO` & `pycentral-1.3.7/pycentral.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: pycentral
-Version: 1.3
+Version: 1.3.7
 Summary: Aruba Central Python Package
 Home-page: https://github.com/aruba/pycentral
 Author: aruba-automation
 Author-email: aruba-automation@hpe.com
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: System Administrators
 Classifier: Topic :: System :: Networking
 Classifier: Development Status :: 4 - Beta
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: PyYAML
 Requires-Dist: urllib3
 Requires-Dist: certifi
 Provides-Extra: colorlog
@@ -52,27 +52,29 @@
 
 Now you can start making your script based on modules in pycentral or use different workflows from the subpackage `workflows`.
 
 ## Executing Scripts
 
 1. Gathering variables required for the package base class `ArubaCentralBase`.
 
-    * **base_url**: You can find the base URL of the Central account's API Gateway from the table <a href="https://www.arubanetworks.com/techdocs/central/latest/content/nms/api/domain_url.htm" target="_blank">here</a>. The base URL is based on the geographical Central cluster in which the account is registered.
-
-    * **client_id** and **client_secret**: Obtain client_id and client_secret variables by creating an API Gateway client in Aruba Central. Refer the following <a href="https://developer.arubanetworks.com/aruba-central/docs/api-gateway-creating-application-token" target="_blank">documentation</a> for more details.
+    * **base_url** OR **cluster_name**: You can find the base URL or cluster name of the Central account's API Gateway from the table <a href="https://www.arubanetworks.com/techdocs/central/latest/content/nms/api/domain_url.htm" target="_blank">here</a>. The base URL or cluster name is based on the geographical Central cluster in which the account is registered.
 
    * **access_token**: You can create an API access token for Aruba Central from -
       * <a href="https://developer.arubanetworks.com/aruba-central/docs/api-gateway-obtaining-access-tokens#obtain-access-token-via-web-ui" target="_blank">Aruba Central UI</a>
       * <a href="https://developer.arubanetworks.com/aruba-central/docs/api-oauth-access-token" target="_blank">OAuth APIs</a>
 
-    * **customer_id**: Obtain the **customer_id** by clicking on the figure icon on top right corner of Aruba Central WebUI.
+    * Optional variables - You need to provide the below variables if you want to use PyCentral's ability to generate access tokens from Aruba Central with the help of OAuth APIs.
+      * **username** and **password**: Aruba Central user's *username* and *password*. The access token generated by the OAUTH APIs will have the same role/privileges as the provided Aruba Central user.
+  
+      * **client_id** and **client_secret**: Obtain client_id and client_secret variables by creating an API Gateway client in Aruba Central. Refer the following <a href="https://developer.arubanetworks.com/aruba-central/docs/api-gateway-creating-application-token" target="_blank">documentation</a> for more details.
+    
+      * **customer_id**: Obtain the **customer_id** by clicking on the figure icon on top right corner of Aruba Central WebUI.
 
     ![Customer ID](https://github.com/aruba/pycentral/raw/master/pictures/customer-id.png)
 
-    * **username** and **password**: Aruba Central user's *username* and *password*. The access token generated by the OAUTH APIs will have the same role/privileges as the provided Aruba Central user.
 
 2. Providing input variables to the Python scripts. One of the following options can be used.
     * Provide variables directly to Aruba Central Base class in dictionary format.
 
         Access token approach:
         ```python
         central_info = {
@@ -90,21 +92,25 @@
                 "password": "<aruba-central-account-password>",
                 "client_id": "<api-gateway-client-id>",
                 "client_secret": "<api-gateway-client-secret>",
                 "customer_id": "<aruba-central-customer-id>",
                 "base_url": "<api-gateway-domain-url>"
             }
         ```
-
+        Alternatively, you can use **cluster_name** instead of **base_url** in the above mentioned dictionaries. You can find the list of clusters that are supported in the <a href="https://github.com/aruba/pycentral/blob/master/pycentral/constants.py" target="_blank">constants.py file</a>. If you would like to add support for other Central clusters, you can do so by adding it in the constants.py. 
         Refer the sample scripts in *step3* and *step4* for examples.
 
-    * **OR** Provide the required variables using JSON/YAML file. Refer input files <a href="https://github.com/aruba/pycentral/blob/master/sample_scripts/input_token_only.yaml" target="_blank">sample_scripts/input_token_only.yaml</a> and <a href="https://github.com/aruba/pycentral/blob/master/sample_scripts/input_credentials.yaml" target="_blank">sample_scripts/input_credentials.yaml</a> for information.
+    * **OR** Provide the required variables using JSON/YAML file. Refer to the sample input files to understand how the files have to be structured -
+      * <a href="https://github.com/aruba/pycentral/blob/master/sample_scripts/input_token_only.yaml" target="_blank">sample_scripts/input_token_only.yaml</a>
+      * <a href="https://github.com/aruba/pycentral/blob/master/sample_scripts/input_credentials.yaml" target="_blank">sample_scripts/input_credentials.yaml</a> 
+      * <a href="https://github.com/aruba/pycentral/blob/master/sample_scripts/sample_scripts/input_token_only_cluster.yaml" target="_blank">sample_scripts/input_token_only_cluster_name.yaml</a>
+      * <a href="https://github.com/aruba/pycentral/blob/master/sample_scripts/sample_scripts/input_credentials_cluster_name.yaml" target="_blank">sample_scripts/input_credentials_cluster_name.yaml</a>
 
-        Use `pycentral.workflows_utils.get_conn_from_file()` function which accepts name of the file and returns
-        the `ArubaCentralBase` instance object. Refer the sample script in *step5* for example.
+        More sample input files can be found in the <a href="https://github.com/aruba/pycentral/blob/master/sample_scripts/sample_scripts/" target="_blank">sample_scripts folder</a>. Use `pycentral.workflows_utils.get_conn_from_file()` function which accepts name of the file and returns
+        the `ArubaCentralBase` instance object.
 
 3. **Making API call using pycentral base**: Using the base class `ArubaCentralBase`, any Aruba Central supported REST API calls can be made. Refer the following sample script <a href="https://github.com/aruba/pycentral/blob/master/sample_scripts/pycentral_base_sample.py" target="_blank">sample_scripts/pycentral_base_sample.py</a>
 
     Obtain the HTTP Request related information from Aruba Central Swagger documentation or <a href="https://developer.arubanetworks.com/aruba-central/reference" target="_blank">API references</a> page in Aruba Developer Hub.
 
 4. **Making API call using pycentral modules**: Some API endpoints supported by Aruba Central are implemented as modules in the Python package. Refer the following sample script using modules <a href="https://github.com/aruba/pycentral/blob/master/sample_scripts/pycentral_module_sample.py" target="_blank">sample_scripts/pycentral_module_sample.py</a>
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: pycentral Version: 1.3 Summary: Aruba Central
+Metadata-Version: 2.1 Name: pycentral Version: 1.3.7 Summary: Aruba Central
 Python Package Home-page: https://github.com/aruba/pycentral Author: aruba-
 automation Author-email: aruba-automation@hpe.com Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Classifier: Intended
 Audience :: System Administrators Classifier: Topic :: System :: Networking
-Classifier: Development Status :: 4 - Beta Requires-Python: >=3.6 Description-
+Classifier: Development Status :: 4 - Beta Requires-Python: >=3.8 Description-
 Content-Type: text/markdown License-File: LICENSE Requires-Dist: requests
 Requires-Dist: PyYAML Requires-Dist: urllib3 Requires-Dist: certifi Provides-
 Extra: colorlog Requires-Dist: colorlog; extra == "colorlog" # pycentral ####
 Aruba Central Python Package Index SDK Aruba Central is an unified cloud-based
 network management and configuration platform for campus, branch, remote and
 data center networks. There are various needs for automation and
 programmability like automating repetitive tasks, configuring multiple devices,
@@ -20,62 +20,72 @@
 $ source centralenv/bin/activate in Windows: $ centralenv/Scripts/activate.bat
 ``` 3. Install the **pycentral** package ``` (centralenv)$ pip3 install
 pycentral ``` To install package with *extras* `colorLog` which will display
 log in color ``` (centralenv)$ pip3 install pycentral[colorLog] ``` Now you can
 start making your script based on modules in pycentral or use different
 workflows from the subpackage `workflows`. ## Executing Scripts 1. Gathering
 variables required for the package base class `ArubaCentralBase`. *
-**base_url**: You can find the base URL of the Central account's API Gateway
-from the table _h_e_r_e. The base URL is based on the geographical Central cluster
-in which the account is registered. * **client_id** and **client_secret**:
+**base_url** OR **cluster_name**: You can find the base URL or cluster name of
+the Central account's API Gateway from the table _h_e_r_e. The base URL or cluster
+name is based on the geographical Central cluster in which the account is
+registered. * **access_token**: You can create an API access token for Aruba
+Central from - * _A_r_u_b_a_ _C_e_n_t_r_a_l_ _U_I * _O_A_u_t_h_ _A_P_I_s * Optional variables - You need
+to provide the below variables if you want to use PyCentral's ability to
+generate access tokens from Aruba Central with the help of OAuth APIs. *
+**username** and **password**: Aruba Central user's *username* and *password*.
+The access token generated by the OAUTH APIs will have the same role/privileges
+as the provided Aruba Central user. * **client_id** and **client_secret**:
 Obtain client_id and client_secret variables by creating an API Gateway client
 in Aruba Central. Refer the following _d_o_c_u_m_e_n_t_a_t_i_o_n for more details. *
-**access_token**: You can create an API access token for Aruba Central from - *
-_A_r_u_b_a_ _C_e_n_t_r_a_l_ _U_I * _O_A_u_t_h_ _A_P_I_s * **customer_id**: Obtain the **customer_id** by
-clicking on the figure icon on top right corner of Aruba Central WebUI. !
-[Customer ID](https://github.com/aruba/pycentral/raw/master/pictures/customer-
-id.png) * **username** and **password**: Aruba Central user's *username* and
-*password*. The access token generated by the OAUTH APIs will have the same
-role/privileges as the provided Aruba Central user. 2. Providing input
+**customer_id**: Obtain the **customer_id** by clicking on the figure icon on
+top right corner of Aruba Central WebUI. ![Customer ID](https://github.com/
+aruba/pycentral/raw/master/pictures/customer-id.png) 2. Providing input
 variables to the Python scripts. One of the following options can be used. *
 Provide variables directly to Aruba Central Base class in dictionary format.
 Access token approach: ```python central_info = { "base_url": "", "token":
 { "access_token": "" } } ``` OAUTH APIs approach with capability to generate
 new access token: ```python central_info = { "username": "", "password": "",
 "client_id": "", "client_secret": "", "customer_id": "", "base_url": "" } ```
-Refer the sample scripts in *step3* and *step4* for examples. * **OR** Provide
-the required variables using JSON/YAML file. Refer input files _s_a_m_p_l_e___s_c_r_i_p_t_s_/
-_i_n_p_u_t___t_o_k_e_n___o_n_l_y_._y_a_m_l and _s_a_m_p_l_e___s_c_r_i_p_t_s_/_i_n_p_u_t___c_r_e_d_e_n_t_i_a_l_s_._y_a_m_l for
-information. Use `pycentral.workflows_utils.get_conn_from_file()` function
-which accepts name of the file and returns the `ArubaCentralBase` instance
-object. Refer the sample script in *step5* for example. 3. **Making API call
-using pycentral base**: Using the base class `ArubaCentralBase`, any Aruba
-Central supported REST API calls can be made. Refer the following sample script
-_s_a_m_p_l_e___s_c_r_i_p_t_s_/_p_y_c_e_n_t_r_a_l___b_a_s_e___s_a_m_p_l_e_._p_y Obtain the HTTP Request related
-information from Aruba Central Swagger documentation or _A_P_I_ _r_e_f_e_r_e_n_c_e_s page in
-Aruba Developer Hub. 4. **Making API call using pycentral modules**: Some API
-endpoints supported by Aruba Central are implemented as modules in the Python
-package. Refer the following sample script using modules _s_a_m_p_l_e___s_c_r_i_p_t_s_/
-_p_y_c_e_n_t_r_a_l___m_o_d_u_l_e___s_a_m_p_l_e_._p_y To obtain a list of implemented modules and its
-documentation refer the _p_y_c_e_n_t_r_a_l_ _m_o_d_u_l_e_ _d_o_c_u_m_e_n_t_a_t_i_o_n 5. **Workflows**:
-Workflows are used to achieve an automation use-case which generally involves
-multiple API calls or dealing with scale and repetitive tasks with ease. Check
-out the _c_e_n_t_r_a_l_-_p_y_t_h_o_n_-_w_o_r_k_f_l_o_w_s_ repository to check out workflows that utilize
-the Pycentral library. ## Documentation: * **Python package documentation:** *
-_p_y_c_e_n_t_r_a_l_ _m_o_d_u_l_e_ _d_o_c_u_m_e_n_t_a_t_i_o_n * **Use-Cases and Workflows:** - _A_r_u_b_a_ _D_e_v_e_l_o_p_e_r
-_H_u_b - _c_e_n_t_r_a_l_-_p_y_t_h_o_n_-_w_o_r_k_f_l_o_w_s ## Note: The package takes one of the two
-approaches to gain access to Aruba Central APIs. * **OAUTH APIs:** By taking
-OAUTH approach to generate new access_token, the python package will cache the
-tokens locally for re-use. Caching tokens locally, helps preventing creation of
-new access_token every time the script is run. In addition, when the
-access_token is expired the script will attempt to use the supplied credentials
-and attempt to refresh the expired token. Override the
-`ArubaCentralBase.storeToken()` and `ArubaCentralBase.loadToken()` function
-definitions to change this behavior of caching in local file(JSON) and manage
-tokens more securely. * **Access Token**: This process is more secure. By
-providing only the *access_token* instead of credentials, the package will not
-cache the tokens. But loses the ability to handle expired token and to generate
-new access tokens. ## How to contribute Please see the accompanying
-_C_O_N_T_R_I_B_U_T_I_O_N_S_._m_d file for guidelines on how to contribute to this repository.
-## Troubleshooting Issues If you encounter module import errors, make sure that
-the package has been installed correctly. Additionally, please read the
-_R_E_L_E_A_S_E_-_N_O_T_E_S_._m_d file for the current release information and known issues.
+Alternatively, you can use **cluster_name** instead of **base_url** in the
+above mentioned dictionaries. You can find the list of clusters that are
+supported in the _c_o_n_s_t_a_n_t_s_._p_y_ _f_i_l_e. If you would like to add support for other
+Central clusters, you can do so by adding it in the constants.py. Refer the
+sample scripts in *step3* and *step4* for examples. * **OR** Provide the
+required variables using JSON/YAML file. Refer to the sample input files to
+understand how the files have to be structured - * _s_a_m_p_l_e___s_c_r_i_p_t_s_/
+_i_n_p_u_t___t_o_k_e_n___o_n_l_y_._y_a_m_l * _s_a_m_p_l_e___s_c_r_i_p_t_s_/_i_n_p_u_t___c_r_e_d_e_n_t_i_a_l_s_._y_a_m_l * _s_a_m_p_l_e___s_c_r_i_p_t_s_/
+_i_n_p_u_t___t_o_k_e_n___o_n_l_y___c_l_u_s_t_e_r___n_a_m_e_._y_a_m_l * _s_a_m_p_l_e___s_c_r_i_p_t_s_/
+_i_n_p_u_t___c_r_e_d_e_n_t_i_a_l_s___c_l_u_s_t_e_r___n_a_m_e_._y_a_m_l More sample input files can be found in the
+_s_a_m_p_l_e___s_c_r_i_p_t_s_ _f_o_l_d_e_r. Use `pycentral.workflows_utils.get_conn_from_file()`
+function which accepts name of the file and returns the `ArubaCentralBase`
+instance object. 3. **Making API call using pycentral base**: Using the base
+class `ArubaCentralBase`, any Aruba Central supported REST API calls can be
+made. Refer the following sample script _s_a_m_p_l_e___s_c_r_i_p_t_s_/_p_y_c_e_n_t_r_a_l___b_a_s_e___s_a_m_p_l_e_._p_y
+Obtain the HTTP Request related information from Aruba Central Swagger
+documentation or _A_P_I_ _r_e_f_e_r_e_n_c_e_s page in Aruba Developer Hub. 4. **Making API
+call using pycentral modules**: Some API endpoints supported by Aruba Central
+are implemented as modules in the Python package. Refer the following sample
+script using modules _s_a_m_p_l_e___s_c_r_i_p_t_s_/_p_y_c_e_n_t_r_a_l___m_o_d_u_l_e___s_a_m_p_l_e_._p_y To obtain a list
+of implemented modules and its documentation refer the _p_y_c_e_n_t_r_a_l_ _m_o_d_u_l_e
+_d_o_c_u_m_e_n_t_a_t_i_o_n 5. **Workflows**: Workflows are used to achieve an automation
+use-case which generally involves multiple API calls or dealing with scale and
+repetitive tasks with ease. Check out the _c_e_n_t_r_a_l_-_p_y_t_h_o_n_-_w_o_r_k_f_l_o_w_s_ repository
+to check out workflows that utilize the Pycentral library. ## Documentation: *
+**Python package documentation:** * _p_y_c_e_n_t_r_a_l_ _m_o_d_u_l_e_ _d_o_c_u_m_e_n_t_a_t_i_o_n * **Use-
+Cases and Workflows:** - _A_r_u_b_a_ _D_e_v_e_l_o_p_e_r_ _H_u_b - _c_e_n_t_r_a_l_-_p_y_t_h_o_n_-_w_o_r_k_f_l_o_w_s ##
+Note: The package takes one of the two approaches to gain access to Aruba
+Central APIs. * **OAUTH APIs:** By taking OAUTH approach to generate new
+access_token, the python package will cache the tokens locally for re-use.
+Caching tokens locally, helps preventing creation of new access_token every
+time the script is run. In addition, when the access_token is expired the
+script will attempt to use the supplied credentials and attempt to refresh the
+expired token. Override the `ArubaCentralBase.storeToken()` and
+`ArubaCentralBase.loadToken()` function definitions to change this behavior of
+caching in local file(JSON) and manage tokens more securely. * **Access
+Token**: This process is more secure. By providing only the *access_token*
+instead of credentials, the package will not cache the tokens. But loses the
+ability to handle expired token and to generate new access tokens. ## How to
+contribute Please see the accompanying _C_O_N_T_R_I_B_U_T_I_O_N_S_._m_d file for guidelines on
+how to contribute to this repository. ## Troubleshooting Issues If you
+encounter module import errors, make sure that the package has been installed
+correctly. Additionally, please read the _R_E_L_E_A_S_E_-_N_O_T_E_S_._m_d file for the current
+release information and known issues.
```

### Comparing `pycentral-1.3/pycentral.egg-info/SOURCES.txt` & `pycentral-1.3.7/pycentral.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycentral-1.3/setup.py` & `pycentral-1.3.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pycentral",
-    version="1.3",
+    version="1.3.7",
     author="aruba-automation",
     author_email="aruba-automation@hpe.com",
     description="Aruba Central Python Package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/aruba/pycentral",
     packages=setuptools.find_packages(exclude=['docs', 'tests',
@@ -20,13 +20,13 @@
         "Programming Language :: Python :: 3 :: Only",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         'Intended Audience :: System Administrators',
         'Topic :: System :: Networking',
         'Development Status :: 4 - Beta'
     ],
-    python_requires='>=3.6',
+    python_requires='>=3.8',
     install_requires=['requests', 'PyYAML', 'urllib3', 'certifi'],
     extras_require={
         'colorLog': ["colorlog"]
     }
 )
```

