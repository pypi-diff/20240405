# Comparing `tmp/copernicusmarine-1.0.8.tar.gz` & `tmp/copernicusmarine-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copernicusmarine-1.0.8.tar", max compression
+gzip compressed data, was "copernicusmarine-1.0.9.tar", max compression
```

## Comparing `copernicusmarine-1.0.8.tar` & `copernicusmarine-1.0.9.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0    13827 2024-03-20 08:25:03.643831 copernicusmarine-1.0.8/LICENSE.txt
--rw-r--r--   0        0        0    21758 2024-03-20 08:25:03.643831 copernicusmarine-1.0.8/README.md
--rw-r--r--   0        0        0      972 2024-03-20 08:25:03.643831 copernicusmarine-1.0.8/copernicusmarine/__init__.py
--rw-r--r--   0        0        0     1070 2024-03-22 14:56:19.033680 copernicusmarine-1.0.8/copernicusmarine/aioretry/LICENSE
--rw-r--r--   0        0        0      225 2024-03-22 14:56:19.033680 copernicusmarine-1.0.8/copernicusmarine/aioretry/__init__.py
--rw-r--r--   0        0        0     4152 2024-03-22 14:56:19.033680 copernicusmarine-1.0.8/copernicusmarine/aioretry/retry.py
--rw-r--r--   0        0        0       10 2024-03-20 08:25:03.643831 copernicusmarine-1.0.8/copernicusmarine/catalogue_parser/__init__.py
--rw-r--r--   0        0        0    48108 2024-03-22 14:56:19.033680 copernicusmarine-1.0.8/copernicusmarine/catalogue_parser/catalogue_parser.py
--rw-r--r--   0        0        0    11508 2024-03-20 08:25:03.647832 copernicusmarine-1.0.8/copernicusmarine/catalogue_parser/request_structure.py
--rw-r--r--   0        0        0       10 2024-03-20 08:25:03.647832 copernicusmarine-1.0.8/copernicusmarine/command_line_interface/__init__.py
--rw-r--r--   0        0        0      868 2024-03-20 08:25:03.647832 copernicusmarine-1.0.8/copernicusmarine/command_line_interface/copernicus_marine.py
--rw-r--r--   0        0        0     1766 2024-03-20 08:25:03.647832 copernicusmarine-1.0.8/copernicusmarine/command_line_interface/exception_handler.py
--rw-r--r--   0        0        0     3784 2024-03-20 08:25:03.647832 copernicusmarine-1.0.8/copernicusmarine/command_line_interface/group_describe.py
--rw-r--r--   0        0        0     9376 2024-03-20 08:25:03.647832 copernicusmarine-1.0.8/copernicusmarine/command_line_interface/group_get.py
--rw-r--r--   0        0        0     3040 2024-03-20 08:25:03.647832 copernicusmarine-1.0.8/copernicusmarine/command_line_interface/group_login.py
--rw-r--r--   0        0        0    12479 2024-03-20 08:25:03.647832 copernicusmarine-1.0.8/copernicusmarine/command_line_interface/group_subset.py
--rw-r--r--   0        0        0     2339 2024-03-20 08:25:03.647832 copernicusmarine-1.0.8/copernicusmarine/command_line_interface/utils.py
--rw-r--r--   0        0        0    13208 2024-03-20 08:25:03.647832 copernicusmarine-1.0.8/copernicusmarine/core_functions/credentials_utils.py
--rw-r--r--   0        0        0     4455 2024-03-22 14:16:13.464509 copernicusmarine-1.0.8/copernicusmarine/core_functions/custom_zarr_store.py
--rw-r--r--   0        0        0     2718 2024-03-20 08:25:03.647832 copernicusmarine-1.0.8/copernicusmarine/core_functions/deprecated.py
--rw-r--r--   0        0        0     2146 2024-03-20 08:25:03.647832 copernicusmarine-1.0.8/copernicusmarine/core_functions/deprecated_options.py
--rw-r--r--   0        0        0     2132 2024-03-20 08:25:03.647832 copernicusmarine-1.0.8/copernicusmarine/core_functions/describe.py
--rw-r--r--   0        0        0      603 2024-03-20 08:25:03.647832 copernicusmarine-1.0.8/copernicusmarine/core_functions/exceptions.py
--rw-r--r--   0        0        0     8108 2024-03-20 08:25:03.647832 copernicusmarine-1.0.8/copernicusmarine/core_functions/get.py
--rw-r--r--   0        0        0     1606 2024-03-20 08:25:03.647832 copernicusmarine-1.0.8/copernicusmarine/core_functions/login.py
--rw-r--r--   0        0        0      460 2024-03-20 08:25:03.647832 copernicusmarine-1.0.8/copernicusmarine/core_functions/models.py
--rw-r--r--   0        0        0    19524 2024-03-22 14:31:23.663772 copernicusmarine-1.0.8/copernicusmarine/core_functions/services_utils.py
--rw-r--r--   0        0        0     1665 2024-03-22 14:16:13.464509 copernicusmarine-1.0.8/copernicusmarine/core_functions/sessions.py
--rw-r--r--   0        0        0    10937 2024-03-20 08:25:03.647832 copernicusmarine-1.0.8/copernicusmarine/core_functions/subset.py
--rw-r--r--   0        0        0     5528 2024-03-22 14:30:17.326082 copernicusmarine-1.0.8/copernicusmarine/core_functions/utils.py
--rw-r--r--   0        0        0     2646 2024-03-20 08:25:03.647832 copernicusmarine-1.0.8/copernicusmarine/core_functions/versions_verifier.py
--rw-r--r--   0        0        0     2249 2024-03-20 08:25:03.647832 copernicusmarine-1.0.8/copernicusmarine/download_functions/common_download.py
--rw-r--r--   0        0        0     7889 2024-03-22 14:31:23.663772 copernicusmarine-1.0.8/copernicusmarine/download_functions/download_arco_series.py
--rw-r--r--   0        0        0    10499 2024-03-20 08:25:03.647832 copernicusmarine-1.0.8/copernicusmarine/download_functions/download_ftp.py
--rw-r--r--   0        0        0     1641 2024-03-20 08:25:03.647832 copernicusmarine-1.0.8/copernicusmarine/download_functions/download_get.py
--rw-r--r--   0        0        0     4098 2024-03-20 08:25:03.647832 copernicusmarine-1.0.8/copernicusmarine/download_functions/download_motu.py
--rw-r--r--   0        0        0    11305 2024-03-20 08:25:03.647832 copernicusmarine-1.0.8/copernicusmarine/download_functions/download_opendap.py
--rw-r--r--   0        0        0    14642 2024-03-22 14:16:13.464509 copernicusmarine-1.0.8/copernicusmarine/download_functions/download_original_files.py
--rw-r--r--   0        0        0      918 2024-03-20 08:25:03.647832 copernicusmarine-1.0.8/copernicusmarine/download_functions/subset_parameters.py
--rw-r--r--   0        0        0    18095 2024-03-22 14:31:23.663772 copernicusmarine-1.0.8/copernicusmarine/download_functions/subset_xarray.py
--rw-r--r--   0        0        0     5567 2024-03-20 08:25:03.647832 copernicusmarine-1.0.8/copernicusmarine/download_functions/utils.py
--rw-r--r--   0        0        0      863 2024-03-20 08:25:03.647832 copernicusmarine-1.0.8/copernicusmarine/logging_conf.json
--rw-r--r--   0        0        0     1961 2024-03-20 08:25:03.647832 copernicusmarine-1.0.8/copernicusmarine/python_interface/describe.py
--rw-r--r--   0        0        0      447 2024-03-20 08:25:03.647832 copernicusmarine-1.0.8/copernicusmarine/python_interface/exception_handler.py
--rw-r--r--   0        0        0     5421 2024-03-20 08:25:03.647832 copernicusmarine-1.0.8/copernicusmarine/python_interface/get.py
--rw-r--r--   0        0        0     4105 2024-03-22 14:31:23.663772 copernicusmarine-1.0.8/copernicusmarine/python_interface/load_utils.py
--rw-r--r--   0        0        0      731 2024-03-20 08:25:03.647832 copernicusmarine-1.0.8/copernicusmarine/python_interface/login.py
--rw-r--r--   0        0        0     6600 2024-03-20 08:25:03.647832 copernicusmarine-1.0.8/copernicusmarine/python_interface/open_dataset.py
--rw-r--r--   0        0        0     6289 2024-03-20 08:25:03.647832 copernicusmarine-1.0.8/copernicusmarine/python_interface/read_dataframe.py
--rw-r--r--   0        0        0     6331 2024-03-20 08:25:03.647832 copernicusmarine-1.0.8/copernicusmarine/python_interface/subset.py
--rw-r--r--   0        0        0      348 2024-03-20 08:25:03.647832 copernicusmarine-1.0.8/copernicusmarine/python_interface/utils.py
--rw-r--r--   0        0        0      942 2024-03-25 16:41:41.717356 copernicusmarine-1.0.8/pyproject.toml
--rw-r--r--   0        0        0    23536 1970-01-01 00:00:00.000000 copernicusmarine-1.0.8/setup.py
--rw-r--r--   0        0        0    22847 1970-01-01 00:00:00.000000 copernicusmarine-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0    13827 2024-03-20 08:25:03.643831 copernicusmarine-1.0.9/LICENSE.txt
+-rw-r--r--   0        0        0    21752 2024-03-26 09:34:05.299481 copernicusmarine-1.0.9/README.md
+-rw-r--r--   0        0        0      972 2024-03-20 08:25:03.643831 copernicusmarine-1.0.9/copernicusmarine/__init__.py
+-rw-r--r--   0        0        0     1070 2024-03-22 14:56:19.033680 copernicusmarine-1.0.9/copernicusmarine/aioretry/LICENSE
+-rw-r--r--   0        0        0      225 2024-03-22 14:56:19.033680 copernicusmarine-1.0.9/copernicusmarine/aioretry/__init__.py
+-rw-r--r--   0        0        0     4152 2024-03-22 14:56:19.033680 copernicusmarine-1.0.9/copernicusmarine/aioretry/retry.py
+-rw-r--r--   0        0        0       10 2024-03-20 08:25:03.643831 copernicusmarine-1.0.9/copernicusmarine/catalogue_parser/__init__.py
+-rw-r--r--   0        0        0    48108 2024-03-22 14:56:19.033680 copernicusmarine-1.0.9/copernicusmarine/catalogue_parser/catalogue_parser.py
+-rw-r--r--   0        0        0    11508 2024-03-20 08:25:03.647832 copernicusmarine-1.0.9/copernicusmarine/catalogue_parser/request_structure.py
+-rw-r--r--   0        0        0       10 2024-03-20 08:25:03.647832 copernicusmarine-1.0.9/copernicusmarine/command_line_interface/__init__.py
+-rw-r--r--   0        0        0      868 2024-03-20 08:25:03.647832 copernicusmarine-1.0.9/copernicusmarine/command_line_interface/copernicus_marine.py
+-rw-r--r--   0        0        0     1766 2024-03-20 08:25:03.647832 copernicusmarine-1.0.9/copernicusmarine/command_line_interface/exception_handler.py
+-rw-r--r--   0        0        0     3784 2024-03-20 08:25:03.647832 copernicusmarine-1.0.9/copernicusmarine/command_line_interface/group_describe.py
+-rw-r--r--   0        0        0     9376 2024-03-20 08:25:03.647832 copernicusmarine-1.0.9/copernicusmarine/command_line_interface/group_get.py
+-rw-r--r--   0        0        0     3040 2024-03-20 08:25:03.647832 copernicusmarine-1.0.9/copernicusmarine/command_line_interface/group_login.py
+-rw-r--r--   0        0        0    12479 2024-03-20 08:25:03.647832 copernicusmarine-1.0.9/copernicusmarine/command_line_interface/group_subset.py
+-rw-r--r--   0        0        0     2339 2024-03-20 08:25:03.647832 copernicusmarine-1.0.9/copernicusmarine/command_line_interface/utils.py
+-rw-r--r--   0        0        0    13208 2024-03-20 08:25:03.647832 copernicusmarine-1.0.9/copernicusmarine/core_functions/credentials_utils.py
+-rw-r--r--   0        0        0     4455 2024-03-22 14:16:13.464509 copernicusmarine-1.0.9/copernicusmarine/core_functions/custom_zarr_store.py
+-rw-r--r--   0        0        0     2718 2024-03-20 08:25:03.647832 copernicusmarine-1.0.9/copernicusmarine/core_functions/deprecated.py
+-rw-r--r--   0        0        0     2146 2024-03-20 08:25:03.647832 copernicusmarine-1.0.9/copernicusmarine/core_functions/deprecated_options.py
+-rw-r--r--   0        0        0     2132 2024-03-20 08:25:03.647832 copernicusmarine-1.0.9/copernicusmarine/core_functions/describe.py
+-rw-r--r--   0        0        0      603 2024-03-20 08:25:03.647832 copernicusmarine-1.0.9/copernicusmarine/core_functions/exceptions.py
+-rw-r--r--   0        0        0     8108 2024-03-20 08:25:03.647832 copernicusmarine-1.0.9/copernicusmarine/core_functions/get.py
+-rw-r--r--   0        0        0     1606 2024-03-20 08:25:03.647832 copernicusmarine-1.0.9/copernicusmarine/core_functions/login.py
+-rw-r--r--   0        0        0      460 2024-03-20 08:25:03.647832 copernicusmarine-1.0.9/copernicusmarine/core_functions/models.py
+-rw-r--r--   0        0        0    19524 2024-03-22 14:31:23.663772 copernicusmarine-1.0.9/copernicusmarine/core_functions/services_utils.py
+-rw-r--r--   0        0        0     1665 2024-03-22 14:16:13.464509 copernicusmarine-1.0.9/copernicusmarine/core_functions/sessions.py
+-rw-r--r--   0        0        0    10937 2024-03-20 08:25:03.647832 copernicusmarine-1.0.9/copernicusmarine/core_functions/subset.py
+-rw-r--r--   0        0        0     5528 2024-03-22 14:30:17.326082 copernicusmarine-1.0.9/copernicusmarine/core_functions/utils.py
+-rw-r--r--   0        0        0     2646 2024-03-20 08:25:03.647832 copernicusmarine-1.0.9/copernicusmarine/core_functions/versions_verifier.py
+-rw-r--r--   0        0        0     2249 2024-03-20 08:25:03.647832 copernicusmarine-1.0.9/copernicusmarine/download_functions/common_download.py
+-rw-r--r--   0        0        0     7889 2024-03-22 14:31:23.663772 copernicusmarine-1.0.9/copernicusmarine/download_functions/download_arco_series.py
+-rw-r--r--   0        0        0    10499 2024-03-20 08:25:03.647832 copernicusmarine-1.0.9/copernicusmarine/download_functions/download_ftp.py
+-rw-r--r--   0        0        0     1641 2024-03-20 08:25:03.647832 copernicusmarine-1.0.9/copernicusmarine/download_functions/download_get.py
+-rw-r--r--   0        0        0     4098 2024-03-20 08:25:03.647832 copernicusmarine-1.0.9/copernicusmarine/download_functions/download_motu.py
+-rw-r--r--   0        0        0    11305 2024-03-20 08:25:03.647832 copernicusmarine-1.0.9/copernicusmarine/download_functions/download_opendap.py
+-rw-r--r--   0        0        0    14642 2024-03-22 14:16:13.464509 copernicusmarine-1.0.9/copernicusmarine/download_functions/download_original_files.py
+-rw-r--r--   0        0        0      918 2024-03-20 08:25:03.647832 copernicusmarine-1.0.9/copernicusmarine/download_functions/subset_parameters.py
+-rw-r--r--   0        0        0    18095 2024-03-22 14:31:23.663772 copernicusmarine-1.0.9/copernicusmarine/download_functions/subset_xarray.py
+-rw-r--r--   0        0        0     5567 2024-03-20 08:25:03.647832 copernicusmarine-1.0.9/copernicusmarine/download_functions/utils.py
+-rw-r--r--   0        0        0      863 2024-03-20 08:25:03.647832 copernicusmarine-1.0.9/copernicusmarine/logging_conf.json
+-rw-r--r--   0        0        0     1961 2024-03-20 08:25:03.647832 copernicusmarine-1.0.9/copernicusmarine/python_interface/describe.py
+-rw-r--r--   0        0        0      447 2024-03-20 08:25:03.647832 copernicusmarine-1.0.9/copernicusmarine/python_interface/exception_handler.py
+-rw-r--r--   0        0        0     5421 2024-03-20 08:25:03.647832 copernicusmarine-1.0.9/copernicusmarine/python_interface/get.py
+-rw-r--r--   0        0        0     4105 2024-03-22 14:31:23.663772 copernicusmarine-1.0.9/copernicusmarine/python_interface/load_utils.py
+-rw-r--r--   0        0        0      731 2024-03-20 08:25:03.647832 copernicusmarine-1.0.9/copernicusmarine/python_interface/login.py
+-rw-r--r--   0        0        0     6600 2024-03-20 08:25:03.647832 copernicusmarine-1.0.9/copernicusmarine/python_interface/open_dataset.py
+-rw-r--r--   0        0        0     6289 2024-03-20 08:25:03.647832 copernicusmarine-1.0.9/copernicusmarine/python_interface/read_dataframe.py
+-rw-r--r--   0        0        0     6331 2024-03-20 08:25:03.647832 copernicusmarine-1.0.9/copernicusmarine/python_interface/subset.py
+-rw-r--r--   0        0        0      348 2024-03-20 08:25:03.647832 copernicusmarine-1.0.9/copernicusmarine/python_interface/utils.py
+-rw-r--r--   0        0        0      942 2024-03-26 09:35:31.669767 copernicusmarine-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0    23530 1970-01-01 00:00:00.000000 copernicusmarine-1.0.9/setup.py
+-rw-r--r--   0        0        0    22841 1970-01-01 00:00:00.000000 copernicusmarine-1.0.9/PKG-INFO
```

### Comparing `copernicusmarine-1.0.8/LICENSE.txt` & `copernicusmarine-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.0.8/README.md` & `copernicusmarine-1.0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 You can install it using conda though the conda-forge channel with the following command: `conda install copernicusmarine -c conda-forge`
 
 ### Docker
 
 A docker image is also available here: [https://hub.docker.com/r/copernicusmarine/copernicusmarine](https://hub.docker.com/r/copernicusmarine/copernicusmarine)
 
-Here is a basic command to run it: `docker run -it --rm copernicusmarine/copernicusmarine:1.0.5 --version`
+Here is a basic command to run it: `docker run -it --rm copernicusmarine/copernicusmarine --version`
 
 ### Pip
 Otherwise, if you already have an environment (safer to clone it), the package can be installed using the `pip` command:
 ```bash
 python -m pip install copernicusmarine
 ```
 
@@ -384,8 +384,8 @@
 - Create your [Copernicus Marine Account](https://data.marine.copernicus.eu/register)
 - [Log in](https://data.marine.copernicus.eu/login?redirect=%2Fproducts) and chat with us (bottom right corner of [Copernicus Marine Service](https://marine.copernicus.eu/))
 - Join our [training workshops](https://marine.copernicus.eu/services/user-learning-services)
 - Network y/our [Copernicus Stories](https://twitter.com/cmems_eu)
 - Watch [our videos](https://www.youtube.com/channel/UC71ceOVy7WtVC7F04BKoEew)
 
 ## Licence
-Licensed under the (EUPL)[https://joinup.ec.europa.eu/collection/eupl/eupl-text-eupl-12]
+Licensed under the [EUPL](https://joinup.ec.europa.eu/collection/eupl/eupl-text-eupl-12)
```

#### html2text {}

```diff
@@ -16,17 +16,17 @@
 been uploaded to the conda-forge channel. Here is the main web page of it:
 [https://anaconda.org/conda-forge/copernicusmarine](https://anaconda.org/conda-
 forge/copernicusmarine) You can install it using conda though the conda-forge
 channel with the following command: `conda install copernicusmarine -c conda-
 forge` ### Docker A docker image is also available here: [https://
 hub.docker.com/r/copernicusmarine/copernicusmarine](https://hub.docker.com/r/
 copernicusmarine/copernicusmarine) Here is a basic command to run it: `docker
-run -it --rm copernicusmarine/copernicusmarine:1.0.5 --version` ### Pip
-Otherwise, if you already have an environment (safer to clone it), the package
-can be installed using the `pip` command: ```bash python -m pip install
+run -it --rm copernicusmarine/copernicusmarine --version` ### Pip Otherwise, if
+you already have an environment (safer to clone it), the package can be
+installed using the `pip` command: ```bash python -m pip install
 copernicusmarine ``` And to **upgrade the package** to the newest available
 version, run: ```bash python -m pip install copernicusmarine --upgrade ``` ##
 User Guide For more comprehensive details on how to use the `copernicusmarine`,
 please refer to our [Help Center](https://help.marine.copernicus.eu/en/
 collections/4060068-copernicus-marine-toolbox). It ensures a smooth migration
 for existing users of legacy services such as MOTU, OPeNDAP, and FTP. ###
 General configuration #### Cache Usage Cachier library is used for caching part
@@ -276,9 +276,9 @@
 milestones). ## Join the community Get in touch! - Create your [Copernicus
 Marine Account](https://data.marine.copernicus.eu/register) - [Log in](https://
 data.marine.copernicus.eu/login?redirect=%2Fproducts) and chat with us (bottom
 right corner of [Copernicus Marine Service](https://marine.copernicus.eu/)) -
 Join our [training workshops](https://marine.copernicus.eu/services/user-
 learning-services) - Network y/our [Copernicus Stories](https://twitter.com/
 cmems_eu) - Watch [our videos](https://www.youtube.com/channel/
-UC71ceOVy7WtVC7F04BKoEew) ## Licence Licensed under the (EUPL)[https://
-joinup.ec.europa.eu/collection/eupl/eupl-text-eupl-12]
+UC71ceOVy7WtVC7F04BKoEew) ## Licence Licensed under the [EUPL](https://
+joinup.ec.europa.eu/collection/eupl/eupl-text-eupl-12)
```

### Comparing `copernicusmarine-1.0.8/copernicusmarine/__init__.py` & `copernicusmarine-1.0.9/copernicusmarine/__init__.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.0.8/copernicusmarine/aioretry/LICENSE` & `copernicusmarine-1.0.9/copernicusmarine/aioretry/LICENSE`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.0.8/copernicusmarine/aioretry/retry.py` & `copernicusmarine-1.0.9/copernicusmarine/aioretry/retry.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.0.8/copernicusmarine/catalogue_parser/catalogue_parser.py` & `copernicusmarine-1.0.9/copernicusmarine/catalogue_parser/catalogue_parser.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.0.8/copernicusmarine/catalogue_parser/request_structure.py` & `copernicusmarine-1.0.9/copernicusmarine/catalogue_parser/request_structure.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.0.8/copernicusmarine/command_line_interface/copernicus_marine.py` & `copernicusmarine-1.0.9/copernicusmarine/command_line_interface/copernicus_marine.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.0.8/copernicusmarine/command_line_interface/exception_handler.py` & `copernicusmarine-1.0.9/copernicusmarine/command_line_interface/exception_handler.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.0.8/copernicusmarine/command_line_interface/group_describe.py` & `copernicusmarine-1.0.9/copernicusmarine/command_line_interface/group_describe.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.0.8/copernicusmarine/command_line_interface/group_get.py` & `copernicusmarine-1.0.9/copernicusmarine/command_line_interface/group_get.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.0.8/copernicusmarine/command_line_interface/group_login.py` & `copernicusmarine-1.0.9/copernicusmarine/command_line_interface/group_login.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.0.8/copernicusmarine/command_line_interface/group_subset.py` & `copernicusmarine-1.0.9/copernicusmarine/command_line_interface/group_subset.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.0.8/copernicusmarine/command_line_interface/utils.py` & `copernicusmarine-1.0.9/copernicusmarine/command_line_interface/utils.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.0.8/copernicusmarine/core_functions/credentials_utils.py` & `copernicusmarine-1.0.9/copernicusmarine/core_functions/credentials_utils.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.0.8/copernicusmarine/core_functions/custom_zarr_store.py` & `copernicusmarine-1.0.9/copernicusmarine/core_functions/custom_zarr_store.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.0.8/copernicusmarine/core_functions/deprecated.py` & `copernicusmarine-1.0.9/copernicusmarine/core_functions/deprecated.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.0.8/copernicusmarine/core_functions/deprecated_options.py` & `copernicusmarine-1.0.9/copernicusmarine/core_functions/deprecated_options.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.0.8/copernicusmarine/core_functions/describe.py` & `copernicusmarine-1.0.9/copernicusmarine/core_functions/describe.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.0.8/copernicusmarine/core_functions/exceptions.py` & `copernicusmarine-1.0.9/copernicusmarine/core_functions/exceptions.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.0.8/copernicusmarine/core_functions/get.py` & `copernicusmarine-1.0.9/copernicusmarine/core_functions/get.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.0.8/copernicusmarine/core_functions/login.py` & `copernicusmarine-1.0.9/copernicusmarine/core_functions/login.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.0.8/copernicusmarine/core_functions/services_utils.py` & `copernicusmarine-1.0.9/copernicusmarine/core_functions/services_utils.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.0.8/copernicusmarine/core_functions/sessions.py` & `copernicusmarine-1.0.9/copernicusmarine/core_functions/sessions.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.0.8/copernicusmarine/core_functions/subset.py` & `copernicusmarine-1.0.9/copernicusmarine/core_functions/subset.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.0.8/copernicusmarine/core_functions/utils.py` & `copernicusmarine-1.0.9/copernicusmarine/core_functions/utils.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.0.8/copernicusmarine/core_functions/versions_verifier.py` & `copernicusmarine-1.0.9/copernicusmarine/core_functions/versions_verifier.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.0.8/copernicusmarine/download_functions/common_download.py` & `copernicusmarine-1.0.9/copernicusmarine/download_functions/common_download.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.0.8/copernicusmarine/download_functions/download_arco_series.py` & `copernicusmarine-1.0.9/copernicusmarine/download_functions/download_arco_series.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.0.8/copernicusmarine/download_functions/download_ftp.py` & `copernicusmarine-1.0.9/copernicusmarine/download_functions/download_ftp.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.0.8/copernicusmarine/download_functions/download_get.py` & `copernicusmarine-1.0.9/copernicusmarine/download_functions/download_get.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.0.8/copernicusmarine/download_functions/download_motu.py` & `copernicusmarine-1.0.9/copernicusmarine/download_functions/download_motu.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.0.8/copernicusmarine/download_functions/download_opendap.py` & `copernicusmarine-1.0.9/copernicusmarine/download_functions/download_opendap.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.0.8/copernicusmarine/download_functions/download_original_files.py` & `copernicusmarine-1.0.9/copernicusmarine/download_functions/download_original_files.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.0.8/copernicusmarine/download_functions/subset_parameters.py` & `copernicusmarine-1.0.9/copernicusmarine/download_functions/subset_parameters.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.0.8/copernicusmarine/download_functions/subset_xarray.py` & `copernicusmarine-1.0.9/copernicusmarine/download_functions/subset_xarray.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.0.8/copernicusmarine/download_functions/utils.py` & `copernicusmarine-1.0.9/copernicusmarine/download_functions/utils.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.0.8/copernicusmarine/logging_conf.json` & `copernicusmarine-1.0.9/copernicusmarine/logging_conf.json`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.0.8/copernicusmarine/python_interface/describe.py` & `copernicusmarine-1.0.9/copernicusmarine/python_interface/describe.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.0.8/copernicusmarine/python_interface/get.py` & `copernicusmarine-1.0.9/copernicusmarine/python_interface/get.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.0.8/copernicusmarine/python_interface/load_utils.py` & `copernicusmarine-1.0.9/copernicusmarine/python_interface/load_utils.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.0.8/copernicusmarine/python_interface/login.py` & `copernicusmarine-1.0.9/copernicusmarine/python_interface/login.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.0.8/copernicusmarine/python_interface/open_dataset.py` & `copernicusmarine-1.0.9/copernicusmarine/python_interface/open_dataset.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.0.8/copernicusmarine/python_interface/read_dataframe.py` & `copernicusmarine-1.0.9/copernicusmarine/python_interface/read_dataframe.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.0.8/copernicusmarine/python_interface/subset.py` & `copernicusmarine-1.0.9/copernicusmarine/python_interface/subset.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.0.8/pyproject.toml` & `copernicusmarine-1.0.9/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "copernicusmarine"
-version = "1.0.8"
+version = "1.0.9"
 description = ""
 authors = ["Copernicus Marine User Support <servicedesk.cmems@mercator-ocean.eu>"]
 readme = "README.md"
 packages = [{include = "copernicusmarine"}]
 license = "EUPL-1.2"
 
 [tool.poetry.dependencies]
```

### Comparing `copernicusmarine-1.0.8/setup.py` & `copernicusmarine-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,17 +34,17 @@
 
 entry_points = \
 {'console_scripts': ['copernicusmarine = '
                      'copernicusmarine.command_line_interface.copernicus_marine:command_line_interface']}
 
 setup_kwargs = {
     'name': 'copernicusmarine',
-    'version': '1.0.8',
+    'version': '1.0.9',
     'description': '',
-    'long_description': '\n<h1 align="center">Copernicus Marine Service toolbox (CLI & Python)</h1>\n<div align="center">\n  <a href="https://pypi.org/project/copernicusmarine/"><img src="https://img.shields.io/pypi/v/copernicusmarine.svg?style=flat-square" alt="PyPI" /></a>\n  <a href="https://pypi.org/project/copernicusmarine/"><img src="https://img.shields.io/pypi/pyversions/copernicusmarine.svg?style=flat-square" alt="PyPI Supported Versions" /></a>\n  <a href="https://pypi.org/project/copernicusmarine/"><img src="https://img.shields.io/badge/platform-windows | linux | macos-lightgrey?style=flat-square" alt="Supported Platforms" /></a>\n  <a href="https://joinup.ec.europa.eu/collection/eupl/eupl-text-eupl-12"><img src="https://img.shields.io/badge/licence-EUPL-lightblue?style=flat-square" alt="Licence" /></a>\n</div>\n\n![Copernicus Marine Service and Mercator Ocean international logos](https://www.mercator-ocean.eu/wp-content/uploads/2022/05/Cartouche_CMEMS_poisson_MOi.png)\n\n## Features\nThe `copernicusmarine` offers capabilities through both **Command Line Interface (CLI)** and **Python API**:\n- **Metadata Information**: List and retrieve metadata information on all variables, datasets, products, and their associated documentation.\n- **Subset Datasets**: Subset datasets to extract only the parts of interest, in preferred format, such as Analysis-Ready Cloud-Optimized (ARCO) Zarr or NetCDF file format.\n- **Advanced Filters**: Apply simple or advanced filters to get multiple files, in original formats like NetCDF/GeoTIFF, via direct Marine Data Store connections.\n- **No Quotas**: Enjoy no quotas, neither on volume size nor bandwidth.\n\n## Installation\nFor installation, multiple options are available depending on your setup:\n\n### Conda|Mamba\n\nA conda package is available and has been uploaded to the conda-forge channel.\n\nHere is the main web page of it: [https://anaconda.org/conda-forge/copernicusmarine](https://anaconda.org/conda-forge/copernicusmarine)\n\nYou can install it using conda though the conda-forge channel with the following command: `conda install copernicusmarine -c conda-forge`\n\n### Docker\n\nA docker image is also available here: [https://hub.docker.com/r/copernicusmarine/copernicusmarine](https://hub.docker.com/r/copernicusmarine/copernicusmarine)\n\nHere is a basic command to run it: `docker run -it --rm copernicusmarine/copernicusmarine:1.0.5 --version`\n\n### Pip\nOtherwise, if you already have an environment (safer to clone it), the package can be installed using the `pip` command:\n```bash\npython -m pip install copernicusmarine\n```\n\nAnd to **upgrade the package** to the newest available version, run:\n```bash\npython -m pip install copernicusmarine --upgrade\n```\n\n## User Guide\nFor more comprehensive details on how to use the `copernicusmarine`, please refer to our [Help Center](https://help.marine.copernicus.eu/en/collections/4060068-copernicus-marine-toolbox). It ensures a smooth migration for existing users of legacy services such as MOTU, OPeNDAP, and FTP.\n\n### General configuration\n\n#### Cache Usage\n\nCachier library is used for caching part of the requests (as describe result or login). By default, the cache will be located in the home folder. If you need to change the location of the cache, you can set the environment variable `COPERNICUSMARINE_CACHE_DIRECTORY` to point to the desired directory.\n\n#### Disable SSL\n\nA global SSL context is used when making HTTP calls using the `copernicusmarine` toolbox. For some reason, it can lead to unexpected behavior depending on your network configuration. You can set the `COPERNICUSMARINE_DISABLE_SSL_CONTEXT` environmnent variable to any value to globally disable the usage of SSL in the client (e.g. `COPERNICUSMARINE_DISABLE_SSL_CONTEXT=True`).\n\n## Command Line Interface (CLI)\n\n### The `--help` option\nTo discover commands and their available options, consider appending `--help` on any command line.\n\nExample:\n```bash\ncopernicusmarine --help\n```\nReturns:\n```bash\nUsage: copernicusmarine [OPTIONS] COMMAND [ARGS]...\n\nOptions:\n  -V, --version  Show the version and exit.\n  --help         Show this message and exit.\n\nCommands:\n  describe  Print Copernicus Marine catalog as JSON\n  login     This command check the copernicusmarine credentials provided...\n  get       Download originally produced data files\n  subset    Downloads subsets of datasets as NetCDF files or Zarr stores\n```\n\n### Command `describe`\nRetrieve metadata information about all products/datasets and display as JSON output:\n```bash\ncopernicusmarine describe --include-datasets\n```\n\nThe JSON output can also be saved like follows:\n```bash\ncopernicusmarine describe --include-datasets > all_datasets_copernicusmarine.json\n```\n\n### Command `login`\nCreate a single configuration file `.copernicusmarine-credentials` allowing to access all Marine Data Store data services. By default, it saves file in user\'s home directory.\n\nExample:\n```bash\n> copernicusmarine login\nusername : johndoe\npassword :\nINFO - Configuration files stored in /Users/foo/.copernicusmarine\n```\n\nIf `.copernicusmarine-credentials` already exists, the user is asked for confirmation to overwrite (`--overwrite`/`--overwrite-configuration-file`).\n\nYou can use the `--skip-if-user-logged-in` option to skip the configuration file overwrite if the user is already logged in.\n\n#### Access points migration and evolution\n\nIf you already have a configuration for current services (e.g. `~/motuclient/motuclient-python.ini`, `~/.netrc` or `~/_netrc`) in your home directory, it will automatically be taken into account with commands `get` and `subset` without the need for running the `login` command.\nIf the configuration files are already available in another directory, when running commands `subset` or `get`, you can use the `--credentials-file` option to point to the file.\n\n### Command `subset`\nRemotely subset a dataset, based on variable names, geographical and temporal parameters.\n\nExample:\n```bash\ncopernicusmarine subset --dataset-id cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m --variable thetao --variable so --start-datetime 2021-01-01 --end-datetime 2021-01-03 --minimum-longitude 0.0 --maximum-longitude 0.1 --minimum-latitude 28.0 --maximum-latitude 28.1\n```\nReturns:\n```bash\nINFO     - Download through S3\n<xarray.Dataset>\nDimensions:    (depth: 50, latitude: 2, longitude: 1, time: 1)\nCoordinates:\n  * depth      (depth) float32 0.5058 1.556 2.668 ... 5.292e+03 5.698e+03\n  * latitude   (latitude) float32 28.0 28.08\n  * longitude  (longitude) float32 0.08333\n  * time       (time) datetime64[ns] 2021-01-01\nData variables:\n    thetao     (time, depth, latitude, longitude) float32 dask.array<chunksize=(1, 50, 2, 1), meta=np.ndarray>\n    so         (time, depth, latitude, longitude) float32 dask.array<chunksize=(1, 50, 2, 1), meta=np.ndarray>\nAttributes: (12/19)\n    Conventions:    CF-1.0\n    bulletin_date:  2022-11-01\n    ...             ...\n    title:          CMEMS IBI REANALYSIS: YEARLY PHYSICAL PRODUCTS\nDo you want to proceed with download? [Y/n]:\n```\n\nBy default, after the display of the summary of the dataset subset, a download confirmation is asked. To skip this user\'s action, call option `--force-download`.\n\n#### Note about longitude range\nOptions `--minimum-longitude` and `--maximum-longitude` work as follows:\n- If the result of the substraction ( `--maximum-longitude` minus `--minimum-longitude` ) is superior or equal to 360, then return the full dataset.\n- If the requested longitude range:\n  - **does not cross** the antemeridian, then return the dataset between range -180° and 180°.\n  - **does cross** the antemeridian, then return the dataset between range 0° and 360°.\n\nNote that you can request any longitudes you want. A modulus is applied to bring the result between -180° and 360°. For example, if you request [530°, 560°], the result dataset will be in [170°, 200°].\n\n#### Access point migration and evolution\nThe copernicus marine toolbox will download the data in the most efficient way according to your request:\n- if the target dataset **is available** in ARCO version, then files are downloaded in a fresh new folder in the current working directory.\n- if the target dataset **is not yet available** in ARCO version, then a file is downloaded in the current working directory.\n> **_NOTE:_**  The filename will be with the following format `dataset_id-longitude_range-latitude_range-depth_range-date_range.[nc|zarr]`\n\nHowever, the output directory and filename can be specified using `-o`/`--output-directory` and `-f`/`--output-filename` respectively. If the later ends with `.nc`, it will be written as a NetCDF file.\n\nYou can force the use of a specific data access service with option `--service`.\n\n#### Note about netcdf-compression-enabled and --netcdf-compression-enabled options\nWhen subseting data, if you decide to write your data as a NetCDF file (which is the default behavior), then you can provide the extra option "--netcdf-compression-enabled". The downloaded file will be lighter but it will take you more time to write it (because of the compression task). If you don\'t provide it, the task will be faster, but the file heavier.\nFinally, if you decide to write your data in ZARR format (.zarr extension), then the original compression that is used in the Marine Data Store will be apply, which mean that the download task will be fast AND the file compressed. In that case, you cannot use the "netcdf-compression-enabled" as it has no sense.\n\nHere is the default options added to xarray in the background when using the option: {\'zlib\': True, \'complevel\': 1, \'contiguous\': False, \'shuffle\': True}\n\nIn addition to this option, you can also provide the `--netcdf-compression-enabled` option and customize the NetCDF compression level between 0 (no compression) and 9.\n\n### Command `get`\nDownload the dataset file(s) as originally produced, based on the datasetID or the path to files.\n\nExample:\n```bash\ncopernicusmarine get --dataset-url ftp://my.cmems-du.eu/Core/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m --service original-files\n```\nReturns:\n```bash\nINFO     - You forced selection of service: original-files\nINFO     - Downloading using service original-files...\nINFO     - You requested the download of the following files:\ns3://mdl-native/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_19930101_19931231_R20221101_RE01.nc - 8.83 MB\n[... truncated for brevity..]\ns3://mdl-native/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20120101_20121231_R20221101_RE01.nc - 8.62 MB\nPrinted 20 out of 29 files\n\nTotal size of the download: 252.94 MB\n\nDo you want to proceed with download? [Y/n]\n```\n\nYou can force the use of a specific data access service with option `--service`.\n\nBy default:\n- after the header displays a summary of the request, a download confirmation is asked. To skip this user\'s action, add option `--force-download`.\n- files are downloaded to the current directory applying the original folder structure. To avoid this behavior, add `--no-directories` and specify a destination with the `--output-directory` option.\n\nOption `--show-outputnames` displays the full paths of the output files, if required.\n\nOption `--download-file-list` only creates a file `files_to_download.txt` containing the names of the targeted files instead of downloading them. If specified, no other action will be performed.\n\n#### Note about sync option\n\nOption `--sync` allows to download original files only if not exist and not up to date. The toolbox checks the destination folder against the source folder. It can be combined with filters. Note that if set with `--overwrite-output-data`, the latter will be ignored.\nThe logic is largely inspired from [s5mp package sync command](https://github.com/peak/s5cmd#sync)\nOption `--sync-delete` will work as `--sync` with the added fonctionnality that it deletes any local file that has not been found on the remote server. Note that the files found on the server are also filtered. Hence, a file present locally might be deleted even if it is on the server because,  for example, the executed `get` command contains a filter that excludes this specific file.\nLimitations:\n- is not compatible with `--no-directories`.\n- Version needs to be set when using sync (with `--force-dataset-version` flag)\n- As for now, the sync functionality is not available for datasets with several parts (like INSITU or static datasets for example).\n\n#### Note about filtering options\nOption `--filter` allows to specify a Unix shell-style wildcard pattern (see [fnmatch — Unix filename pattern matching](https://docs.python.org/3/library/fnmatch.html)) and select specific files:\n```bash\ncopernicusmarine get --dataset-id cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m --filter "*01yav_200[0-2]*"\n```\nReturns:\n```bash\nINFO     - Downloading using service files...\nINFO     - You requested the download of the following files:\ns3://mdl-native/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20000101_20001231_R20221101_RE01.nc - 8.93 MB\ns3://mdl-native/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20010101_20011231_R20221101_RE01.nc - 8.91 MB\ns3://mdl-native/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20020101_20021231_R20221101_RE01.nc - 8.75 MB\n\nTotal size of the download: 26.59 MB\nDo you want to proceed with download? [Y/n]:\n```\n\nOption `--regex` allows to specify a regular expression for more advanced files selection:\n```bash\ncopernicusmarine get -i cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m --regex ".*01yav_20(00|01|02).*.nc"\n```\nReturns:\n```bash\nINFO     - Downloading using service files...\nINFO     - You requested the download of the following files:\ns3://mdl-native/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20000101_20001231_R20221101_RE01.nc - 8.93 MB\ns3://mdl-native/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20010101_20011231_R20221101_RE01.nc - 8.91 MB\ns3://mdl-native/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20020101_20021231_R20221101_RE01.nc - 8.75 MB\n\nTotal size of the download: 26.59 MB\nDo you want to proceed with download? [Y/n]:\n```\n\nOption `--file-list` allows to specify a list of files for more advanced files selection:\n\nAn example `file_list.txt` would look like this:\n```txt\nCMEMS_v5r1_IBI_PHY_MY_NL_01yav_20000101_20001231_R20221101_RE01.nc\nCMEMS_v5r1_IBI_PHY_MY_NL_01yav_20010101_20011231_R20221101_RE01.nc\nCMEMS_v5r1_IBI_PHY_MY_NL_01yav_20020101_20021231_R20221101_RE01.nc\n```\n> **_NOTE:_**  This option is compatible with the file generated by the `--download-file-list` option.\n\nThen the following command:\n```bash\ncopernicusmarine get -i cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m --file-list file_list.txt\n```\nReturns:\n```bash\nINFO     - Downloading using service files...\nINFO     - You requested the download of the following files:\ns3://mdl-native/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20000101_20001231_R20221101_RE01.nc - 8.93 MB\ns3://mdl-native/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20010101_20011231_R20221101_RE01.nc - 8.91 MB\ns3://mdl-native/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20020101_20021231_R20221101_RE01.nc - 8.75 MB\n\nTotal size of the download: 26.59 MB\nDo you want to proceed with download? [Y/n]:\n```\n\nAlso, there is a specific command `--index-part` to retrieve the index files of INSITU datasets (for index files example see [this link on Copernicus Marine Service](https://data.marine.copernicus.eu/product/INSITU_BLK_PHYBGCWAV_DISCRETE_MYNRT_013_034/files?subdataset=cmems_obs-ins_blk_phybgcwav_mynrt_na_irr_202311--ext--history&path=INSITU_BLK_PHYBGCWAV_DISCRETE_MYNRT_013_034%2Fcmems_obs-ins_blk_phybgcwav_mynrt_na_irr_202311%2F)). Note that in the future, we plan to have the index files for those datasets, directly available through the filter, regex and/or file-list options.\n\nThen the following command:\n```\ncopernicusmarine get --dataset-id cmems_obs-ins_blk_phybgcwav_mynrt_na_irr --index-parts\n```\n\nReturns:\n```\nINFO - 2024-03-13T08:08:12Z - Dataset version was not specified, the latest one was selected: "202311"\nINFO - 2024-03-13T08:08:12Z - Dataset part was not specified, the first one was selected: "history"\nINFO - 2024-03-13T08:08:12Z - You forced selection of service: original-files\nINFO - 2024-03-13T08:08:12Z - Downloading using service original-files...\nINFO - 2024-03-13T08:08:13Z - You requested the download of the following files:\ns3://mdl-native-08/native/INSITU_BLK_PHYBGCWAV_DISCRETE_MYNRT_013_034/cmems_obs-ins_blk_phybgcwav_mynrt_na_irr_202311/index_history.txt - 244.61 kB - 2023-11-30T17:01:25Z\ns3://mdl-native-08/native/INSITU_BLK_PHYBGCWAV_DISCRETE_MYNRT_013_034/cmems_obs-ins_blk_phybgcwav_mynrt_na_irr_202311/index_latest.txt - 572.09 kB - 2024-03-13T07:21:00Z\ns3://mdl-native-08/native/INSITU_BLK_PHYBGCWAV_DISCRETE_MYNRT_013_034/cmems_obs-ins_blk_phybgcwav_mynrt_na_irr_202311/index_monthly.txt - 1.51 MB - 2024-03-05T18:09:43Z\ns3://mdl-native-08/native/INSITU_BLK_PHYBGCWAV_DISCRETE_MYNRT_013_034/cmems_obs-ins_blk_phybgcwav_mynrt_na_irr_202311/index_platform.txt - 209.11 kB - 2024-03-13T07:21:00Z\n\nTotal size of the download: 2.53 MB\n\n\nDo you want to proceed with download? [Y/n]:\n```\n### Shared options\nBoth `subset` and `get` commands provide these options:\n\n#### Option `--overwrite-output-data`\n\nWhen specified, the existing files will be overwritten.\nOtherwise, if the files already exist on destination, new ones with a unique index will be created once the download has been accepted (or once `--force-download` is provided).\n\n#### Option `--request-file`\n\nThis option allows to specify CLI options but in a provided JSON file, useful for batch processing.\n\n- Template for `subset` data request:\n```json\n{\n\t"dataset_id": "cmems_mod_glo_phy-thetao_anfc_0.083deg_P1D-m",\n\t"start_datetime": "2022-04-11",\n\t"end_datetime": "2023-08-11",\n\t"minimum_longitude": -182.79,\n\t"maximum_longitude": -179.69,\n\t"minimum_latitude": -40,\n\t"maximum_latitude": -36,\n\t"minimum_depth": 0,\n\t"maximum_depth": 0,\n\t"variables": ["thetao"],\n\t"output_directory": "./data/",\n\t"output_filename": "temperature_small_pacific_2022208-202308.zarr",\n\t"force_download": false\n}\n```\n\nExample:\n```bash\ncopernicusmarine subset --request-file template_subset_data_request.json\n```\n\n- Template for `get` data request:\n```json\n{\n    "dataset_id": "cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m",\n    "filter": "*01yav_200[0-2]*",\n    "force_download": false,\n    "service": "files",\n    "log_level": "INFO",\n    "no_directories": false,\n    "no_metadata_cache": false,\n    "output_directory": "./data/",\n    "overwrite_output_data": false,\n    "overwrite_metadata_cache": false,\n    "show_outputnames": true\n}\n```\n\nExample:\n```bash\ncopernicusmarine get --request-file template_get_data_request.json\n```\n\n#### Option `--credentials-file`\nYou can use the `--credentials-file` option to point to a credentials file. The file can be either `.copernicusmarine-credentials`, `motuclient-python.ini`, `.netrc` or `_netrc`.\n\n\n#### Option `--dataset-version`\nYou can use the `--dataset-version` option to fetch a specific dataset version.\n\n#### Option `--dataset-part`\nYou can use the `--dataset-part` option to fecth a specific part for the chosen dataset version.\n\n\n## Python package (API)\nThe `copernicusmarine` exposes a Python interface to allow you to [call commands as functions](https://marine.copernicus.eu/python-interface).\n\n## Documentation\nSee the [Help Center](https://help.marine.copernicus.eu/en/collections/4060068-copernicus-marine-toolbox). A detailed standalone API documentation is under construction and will come at a later stage.\n\n## Contribution\nWe welcome contributions from the community to enhance this package. If you find any issues or have suggestions for improvements, please check out our [Report Template](https://help.marine.copernicus.eu/en/articles/8218546-how-to-report-a-bug-or-suggest-new-features).\n\n## Future improvements & Roadmap\n- [ ] Make available the currently not managed Analysis-Ready Cloud-Optimized (ARCO) versions of Ocean Monitoring Indicator (OMI), in situ and static datasets.\n- [ ] Allow to specify the compression level when downloading your subset as NetCDF file.\n- [ ] Allow to subset variables using their `standard_name(s)` and not only their `name(s)`.\n\nTo keep up to date with the most recent and planned advancements, including revisions, corrections, and feature requests generated from users\' feedback, please refer to our [Roadmap](https://help.marine.copernicus.eu/en/articles/8218641-what-are-the-next-milestones).\n\n## Join the community\nGet in touch!\n- Create your [Copernicus Marine Account](https://data.marine.copernicus.eu/register)\n- [Log in](https://data.marine.copernicus.eu/login?redirect=%2Fproducts) and chat with us (bottom right corner of [Copernicus Marine Service](https://marine.copernicus.eu/))\n- Join our [training workshops](https://marine.copernicus.eu/services/user-learning-services)\n- Network y/our [Copernicus Stories](https://twitter.com/cmems_eu)\n- Watch [our videos](https://www.youtube.com/channel/UC71ceOVy7WtVC7F04BKoEew)\n\n## Licence\nLicensed under the (EUPL)[https://joinup.ec.europa.eu/collection/eupl/eupl-text-eupl-12]\n',
+    'long_description': '\n<h1 align="center">Copernicus Marine Service toolbox (CLI & Python)</h1>\n<div align="center">\n  <a href="https://pypi.org/project/copernicusmarine/"><img src="https://img.shields.io/pypi/v/copernicusmarine.svg?style=flat-square" alt="PyPI" /></a>\n  <a href="https://pypi.org/project/copernicusmarine/"><img src="https://img.shields.io/pypi/pyversions/copernicusmarine.svg?style=flat-square" alt="PyPI Supported Versions" /></a>\n  <a href="https://pypi.org/project/copernicusmarine/"><img src="https://img.shields.io/badge/platform-windows | linux | macos-lightgrey?style=flat-square" alt="Supported Platforms" /></a>\n  <a href="https://joinup.ec.europa.eu/collection/eupl/eupl-text-eupl-12"><img src="https://img.shields.io/badge/licence-EUPL-lightblue?style=flat-square" alt="Licence" /></a>\n</div>\n\n![Copernicus Marine Service and Mercator Ocean international logos](https://www.mercator-ocean.eu/wp-content/uploads/2022/05/Cartouche_CMEMS_poisson_MOi.png)\n\n## Features\nThe `copernicusmarine` offers capabilities through both **Command Line Interface (CLI)** and **Python API**:\n- **Metadata Information**: List and retrieve metadata information on all variables, datasets, products, and their associated documentation.\n- **Subset Datasets**: Subset datasets to extract only the parts of interest, in preferred format, such as Analysis-Ready Cloud-Optimized (ARCO) Zarr or NetCDF file format.\n- **Advanced Filters**: Apply simple or advanced filters to get multiple files, in original formats like NetCDF/GeoTIFF, via direct Marine Data Store connections.\n- **No Quotas**: Enjoy no quotas, neither on volume size nor bandwidth.\n\n## Installation\nFor installation, multiple options are available depending on your setup:\n\n### Conda|Mamba\n\nA conda package is available and has been uploaded to the conda-forge channel.\n\nHere is the main web page of it: [https://anaconda.org/conda-forge/copernicusmarine](https://anaconda.org/conda-forge/copernicusmarine)\n\nYou can install it using conda though the conda-forge channel with the following command: `conda install copernicusmarine -c conda-forge`\n\n### Docker\n\nA docker image is also available here: [https://hub.docker.com/r/copernicusmarine/copernicusmarine](https://hub.docker.com/r/copernicusmarine/copernicusmarine)\n\nHere is a basic command to run it: `docker run -it --rm copernicusmarine/copernicusmarine --version`\n\n### Pip\nOtherwise, if you already have an environment (safer to clone it), the package can be installed using the `pip` command:\n```bash\npython -m pip install copernicusmarine\n```\n\nAnd to **upgrade the package** to the newest available version, run:\n```bash\npython -m pip install copernicusmarine --upgrade\n```\n\n## User Guide\nFor more comprehensive details on how to use the `copernicusmarine`, please refer to our [Help Center](https://help.marine.copernicus.eu/en/collections/4060068-copernicus-marine-toolbox). It ensures a smooth migration for existing users of legacy services such as MOTU, OPeNDAP, and FTP.\n\n### General configuration\n\n#### Cache Usage\n\nCachier library is used for caching part of the requests (as describe result or login). By default, the cache will be located in the home folder. If you need to change the location of the cache, you can set the environment variable `COPERNICUSMARINE_CACHE_DIRECTORY` to point to the desired directory.\n\n#### Disable SSL\n\nA global SSL context is used when making HTTP calls using the `copernicusmarine` toolbox. For some reason, it can lead to unexpected behavior depending on your network configuration. You can set the `COPERNICUSMARINE_DISABLE_SSL_CONTEXT` environmnent variable to any value to globally disable the usage of SSL in the client (e.g. `COPERNICUSMARINE_DISABLE_SSL_CONTEXT=True`).\n\n## Command Line Interface (CLI)\n\n### The `--help` option\nTo discover commands and their available options, consider appending `--help` on any command line.\n\nExample:\n```bash\ncopernicusmarine --help\n```\nReturns:\n```bash\nUsage: copernicusmarine [OPTIONS] COMMAND [ARGS]...\n\nOptions:\n  -V, --version  Show the version and exit.\n  --help         Show this message and exit.\n\nCommands:\n  describe  Print Copernicus Marine catalog as JSON\n  login     This command check the copernicusmarine credentials provided...\n  get       Download originally produced data files\n  subset    Downloads subsets of datasets as NetCDF files or Zarr stores\n```\n\n### Command `describe`\nRetrieve metadata information about all products/datasets and display as JSON output:\n```bash\ncopernicusmarine describe --include-datasets\n```\n\nThe JSON output can also be saved like follows:\n```bash\ncopernicusmarine describe --include-datasets > all_datasets_copernicusmarine.json\n```\n\n### Command `login`\nCreate a single configuration file `.copernicusmarine-credentials` allowing to access all Marine Data Store data services. By default, it saves file in user\'s home directory.\n\nExample:\n```bash\n> copernicusmarine login\nusername : johndoe\npassword :\nINFO - Configuration files stored in /Users/foo/.copernicusmarine\n```\n\nIf `.copernicusmarine-credentials` already exists, the user is asked for confirmation to overwrite (`--overwrite`/`--overwrite-configuration-file`).\n\nYou can use the `--skip-if-user-logged-in` option to skip the configuration file overwrite if the user is already logged in.\n\n#### Access points migration and evolution\n\nIf you already have a configuration for current services (e.g. `~/motuclient/motuclient-python.ini`, `~/.netrc` or `~/_netrc`) in your home directory, it will automatically be taken into account with commands `get` and `subset` without the need for running the `login` command.\nIf the configuration files are already available in another directory, when running commands `subset` or `get`, you can use the `--credentials-file` option to point to the file.\n\n### Command `subset`\nRemotely subset a dataset, based on variable names, geographical and temporal parameters.\n\nExample:\n```bash\ncopernicusmarine subset --dataset-id cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m --variable thetao --variable so --start-datetime 2021-01-01 --end-datetime 2021-01-03 --minimum-longitude 0.0 --maximum-longitude 0.1 --minimum-latitude 28.0 --maximum-latitude 28.1\n```\nReturns:\n```bash\nINFO     - Download through S3\n<xarray.Dataset>\nDimensions:    (depth: 50, latitude: 2, longitude: 1, time: 1)\nCoordinates:\n  * depth      (depth) float32 0.5058 1.556 2.668 ... 5.292e+03 5.698e+03\n  * latitude   (latitude) float32 28.0 28.08\n  * longitude  (longitude) float32 0.08333\n  * time       (time) datetime64[ns] 2021-01-01\nData variables:\n    thetao     (time, depth, latitude, longitude) float32 dask.array<chunksize=(1, 50, 2, 1), meta=np.ndarray>\n    so         (time, depth, latitude, longitude) float32 dask.array<chunksize=(1, 50, 2, 1), meta=np.ndarray>\nAttributes: (12/19)\n    Conventions:    CF-1.0\n    bulletin_date:  2022-11-01\n    ...             ...\n    title:          CMEMS IBI REANALYSIS: YEARLY PHYSICAL PRODUCTS\nDo you want to proceed with download? [Y/n]:\n```\n\nBy default, after the display of the summary of the dataset subset, a download confirmation is asked. To skip this user\'s action, call option `--force-download`.\n\n#### Note about longitude range\nOptions `--minimum-longitude` and `--maximum-longitude` work as follows:\n- If the result of the substraction ( `--maximum-longitude` minus `--minimum-longitude` ) is superior or equal to 360, then return the full dataset.\n- If the requested longitude range:\n  - **does not cross** the antemeridian, then return the dataset between range -180° and 180°.\n  - **does cross** the antemeridian, then return the dataset between range 0° and 360°.\n\nNote that you can request any longitudes you want. A modulus is applied to bring the result between -180° and 360°. For example, if you request [530°, 560°], the result dataset will be in [170°, 200°].\n\n#### Access point migration and evolution\nThe copernicus marine toolbox will download the data in the most efficient way according to your request:\n- if the target dataset **is available** in ARCO version, then files are downloaded in a fresh new folder in the current working directory.\n- if the target dataset **is not yet available** in ARCO version, then a file is downloaded in the current working directory.\n> **_NOTE:_**  The filename will be with the following format `dataset_id-longitude_range-latitude_range-depth_range-date_range.[nc|zarr]`\n\nHowever, the output directory and filename can be specified using `-o`/`--output-directory` and `-f`/`--output-filename` respectively. If the later ends with `.nc`, it will be written as a NetCDF file.\n\nYou can force the use of a specific data access service with option `--service`.\n\n#### Note about netcdf-compression-enabled and --netcdf-compression-enabled options\nWhen subseting data, if you decide to write your data as a NetCDF file (which is the default behavior), then you can provide the extra option "--netcdf-compression-enabled". The downloaded file will be lighter but it will take you more time to write it (because of the compression task). If you don\'t provide it, the task will be faster, but the file heavier.\nFinally, if you decide to write your data in ZARR format (.zarr extension), then the original compression that is used in the Marine Data Store will be apply, which mean that the download task will be fast AND the file compressed. In that case, you cannot use the "netcdf-compression-enabled" as it has no sense.\n\nHere is the default options added to xarray in the background when using the option: {\'zlib\': True, \'complevel\': 1, \'contiguous\': False, \'shuffle\': True}\n\nIn addition to this option, you can also provide the `--netcdf-compression-enabled` option and customize the NetCDF compression level between 0 (no compression) and 9.\n\n### Command `get`\nDownload the dataset file(s) as originally produced, based on the datasetID or the path to files.\n\nExample:\n```bash\ncopernicusmarine get --dataset-url ftp://my.cmems-du.eu/Core/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m --service original-files\n```\nReturns:\n```bash\nINFO     - You forced selection of service: original-files\nINFO     - Downloading using service original-files...\nINFO     - You requested the download of the following files:\ns3://mdl-native/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_19930101_19931231_R20221101_RE01.nc - 8.83 MB\n[... truncated for brevity..]\ns3://mdl-native/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20120101_20121231_R20221101_RE01.nc - 8.62 MB\nPrinted 20 out of 29 files\n\nTotal size of the download: 252.94 MB\n\nDo you want to proceed with download? [Y/n]\n```\n\nYou can force the use of a specific data access service with option `--service`.\n\nBy default:\n- after the header displays a summary of the request, a download confirmation is asked. To skip this user\'s action, add option `--force-download`.\n- files are downloaded to the current directory applying the original folder structure. To avoid this behavior, add `--no-directories` and specify a destination with the `--output-directory` option.\n\nOption `--show-outputnames` displays the full paths of the output files, if required.\n\nOption `--download-file-list` only creates a file `files_to_download.txt` containing the names of the targeted files instead of downloading them. If specified, no other action will be performed.\n\n#### Note about sync option\n\nOption `--sync` allows to download original files only if not exist and not up to date. The toolbox checks the destination folder against the source folder. It can be combined with filters. Note that if set with `--overwrite-output-data`, the latter will be ignored.\nThe logic is largely inspired from [s5mp package sync command](https://github.com/peak/s5cmd#sync)\nOption `--sync-delete` will work as `--sync` with the added fonctionnality that it deletes any local file that has not been found on the remote server. Note that the files found on the server are also filtered. Hence, a file present locally might be deleted even if it is on the server because,  for example, the executed `get` command contains a filter that excludes this specific file.\nLimitations:\n- is not compatible with `--no-directories`.\n- Version needs to be set when using sync (with `--force-dataset-version` flag)\n- As for now, the sync functionality is not available for datasets with several parts (like INSITU or static datasets for example).\n\n#### Note about filtering options\nOption `--filter` allows to specify a Unix shell-style wildcard pattern (see [fnmatch — Unix filename pattern matching](https://docs.python.org/3/library/fnmatch.html)) and select specific files:\n```bash\ncopernicusmarine get --dataset-id cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m --filter "*01yav_200[0-2]*"\n```\nReturns:\n```bash\nINFO     - Downloading using service files...\nINFO     - You requested the download of the following files:\ns3://mdl-native/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20000101_20001231_R20221101_RE01.nc - 8.93 MB\ns3://mdl-native/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20010101_20011231_R20221101_RE01.nc - 8.91 MB\ns3://mdl-native/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20020101_20021231_R20221101_RE01.nc - 8.75 MB\n\nTotal size of the download: 26.59 MB\nDo you want to proceed with download? [Y/n]:\n```\n\nOption `--regex` allows to specify a regular expression for more advanced files selection:\n```bash\ncopernicusmarine get -i cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m --regex ".*01yav_20(00|01|02).*.nc"\n```\nReturns:\n```bash\nINFO     - Downloading using service files...\nINFO     - You requested the download of the following files:\ns3://mdl-native/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20000101_20001231_R20221101_RE01.nc - 8.93 MB\ns3://mdl-native/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20010101_20011231_R20221101_RE01.nc - 8.91 MB\ns3://mdl-native/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20020101_20021231_R20221101_RE01.nc - 8.75 MB\n\nTotal size of the download: 26.59 MB\nDo you want to proceed with download? [Y/n]:\n```\n\nOption `--file-list` allows to specify a list of files for more advanced files selection:\n\nAn example `file_list.txt` would look like this:\n```txt\nCMEMS_v5r1_IBI_PHY_MY_NL_01yav_20000101_20001231_R20221101_RE01.nc\nCMEMS_v5r1_IBI_PHY_MY_NL_01yav_20010101_20011231_R20221101_RE01.nc\nCMEMS_v5r1_IBI_PHY_MY_NL_01yav_20020101_20021231_R20221101_RE01.nc\n```\n> **_NOTE:_**  This option is compatible with the file generated by the `--download-file-list` option.\n\nThen the following command:\n```bash\ncopernicusmarine get -i cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m --file-list file_list.txt\n```\nReturns:\n```bash\nINFO     - Downloading using service files...\nINFO     - You requested the download of the following files:\ns3://mdl-native/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20000101_20001231_R20221101_RE01.nc - 8.93 MB\ns3://mdl-native/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20010101_20011231_R20221101_RE01.nc - 8.91 MB\ns3://mdl-native/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20020101_20021231_R20221101_RE01.nc - 8.75 MB\n\nTotal size of the download: 26.59 MB\nDo you want to proceed with download? [Y/n]:\n```\n\nAlso, there is a specific command `--index-part` to retrieve the index files of INSITU datasets (for index files example see [this link on Copernicus Marine Service](https://data.marine.copernicus.eu/product/INSITU_BLK_PHYBGCWAV_DISCRETE_MYNRT_013_034/files?subdataset=cmems_obs-ins_blk_phybgcwav_mynrt_na_irr_202311--ext--history&path=INSITU_BLK_PHYBGCWAV_DISCRETE_MYNRT_013_034%2Fcmems_obs-ins_blk_phybgcwav_mynrt_na_irr_202311%2F)). Note that in the future, we plan to have the index files for those datasets, directly available through the filter, regex and/or file-list options.\n\nThen the following command:\n```\ncopernicusmarine get --dataset-id cmems_obs-ins_blk_phybgcwav_mynrt_na_irr --index-parts\n```\n\nReturns:\n```\nINFO - 2024-03-13T08:08:12Z - Dataset version was not specified, the latest one was selected: "202311"\nINFO - 2024-03-13T08:08:12Z - Dataset part was not specified, the first one was selected: "history"\nINFO - 2024-03-13T08:08:12Z - You forced selection of service: original-files\nINFO - 2024-03-13T08:08:12Z - Downloading using service original-files...\nINFO - 2024-03-13T08:08:13Z - You requested the download of the following files:\ns3://mdl-native-08/native/INSITU_BLK_PHYBGCWAV_DISCRETE_MYNRT_013_034/cmems_obs-ins_blk_phybgcwav_mynrt_na_irr_202311/index_history.txt - 244.61 kB - 2023-11-30T17:01:25Z\ns3://mdl-native-08/native/INSITU_BLK_PHYBGCWAV_DISCRETE_MYNRT_013_034/cmems_obs-ins_blk_phybgcwav_mynrt_na_irr_202311/index_latest.txt - 572.09 kB - 2024-03-13T07:21:00Z\ns3://mdl-native-08/native/INSITU_BLK_PHYBGCWAV_DISCRETE_MYNRT_013_034/cmems_obs-ins_blk_phybgcwav_mynrt_na_irr_202311/index_monthly.txt - 1.51 MB - 2024-03-05T18:09:43Z\ns3://mdl-native-08/native/INSITU_BLK_PHYBGCWAV_DISCRETE_MYNRT_013_034/cmems_obs-ins_blk_phybgcwav_mynrt_na_irr_202311/index_platform.txt - 209.11 kB - 2024-03-13T07:21:00Z\n\nTotal size of the download: 2.53 MB\n\n\nDo you want to proceed with download? [Y/n]:\n```\n### Shared options\nBoth `subset` and `get` commands provide these options:\n\n#### Option `--overwrite-output-data`\n\nWhen specified, the existing files will be overwritten.\nOtherwise, if the files already exist on destination, new ones with a unique index will be created once the download has been accepted (or once `--force-download` is provided).\n\n#### Option `--request-file`\n\nThis option allows to specify CLI options but in a provided JSON file, useful for batch processing.\n\n- Template for `subset` data request:\n```json\n{\n\t"dataset_id": "cmems_mod_glo_phy-thetao_anfc_0.083deg_P1D-m",\n\t"start_datetime": "2022-04-11",\n\t"end_datetime": "2023-08-11",\n\t"minimum_longitude": -182.79,\n\t"maximum_longitude": -179.69,\n\t"minimum_latitude": -40,\n\t"maximum_latitude": -36,\n\t"minimum_depth": 0,\n\t"maximum_depth": 0,\n\t"variables": ["thetao"],\n\t"output_directory": "./data/",\n\t"output_filename": "temperature_small_pacific_2022208-202308.zarr",\n\t"force_download": false\n}\n```\n\nExample:\n```bash\ncopernicusmarine subset --request-file template_subset_data_request.json\n```\n\n- Template for `get` data request:\n```json\n{\n    "dataset_id": "cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m",\n    "filter": "*01yav_200[0-2]*",\n    "force_download": false,\n    "service": "files",\n    "log_level": "INFO",\n    "no_directories": false,\n    "no_metadata_cache": false,\n    "output_directory": "./data/",\n    "overwrite_output_data": false,\n    "overwrite_metadata_cache": false,\n    "show_outputnames": true\n}\n```\n\nExample:\n```bash\ncopernicusmarine get --request-file template_get_data_request.json\n```\n\n#### Option `--credentials-file`\nYou can use the `--credentials-file` option to point to a credentials file. The file can be either `.copernicusmarine-credentials`, `motuclient-python.ini`, `.netrc` or `_netrc`.\n\n\n#### Option `--dataset-version`\nYou can use the `--dataset-version` option to fetch a specific dataset version.\n\n#### Option `--dataset-part`\nYou can use the `--dataset-part` option to fecth a specific part for the chosen dataset version.\n\n\n## Python package (API)\nThe `copernicusmarine` exposes a Python interface to allow you to [call commands as functions](https://marine.copernicus.eu/python-interface).\n\n## Documentation\nSee the [Help Center](https://help.marine.copernicus.eu/en/collections/4060068-copernicus-marine-toolbox). A detailed standalone API documentation is under construction and will come at a later stage.\n\n## Contribution\nWe welcome contributions from the community to enhance this package. If you find any issues or have suggestions for improvements, please check out our [Report Template](https://help.marine.copernicus.eu/en/articles/8218546-how-to-report-a-bug-or-suggest-new-features).\n\n## Future improvements & Roadmap\n- [ ] Make available the currently not managed Analysis-Ready Cloud-Optimized (ARCO) versions of Ocean Monitoring Indicator (OMI), in situ and static datasets.\n- [ ] Allow to specify the compression level when downloading your subset as NetCDF file.\n- [ ] Allow to subset variables using their `standard_name(s)` and not only their `name(s)`.\n\nTo keep up to date with the most recent and planned advancements, including revisions, corrections, and feature requests generated from users\' feedback, please refer to our [Roadmap](https://help.marine.copernicus.eu/en/articles/8218641-what-are-the-next-milestones).\n\n## Join the community\nGet in touch!\n- Create your [Copernicus Marine Account](https://data.marine.copernicus.eu/register)\n- [Log in](https://data.marine.copernicus.eu/login?redirect=%2Fproducts) and chat with us (bottom right corner of [Copernicus Marine Service](https://marine.copernicus.eu/))\n- Join our [training workshops](https://marine.copernicus.eu/services/user-learning-services)\n- Network y/our [Copernicus Stories](https://twitter.com/cmems_eu)\n- Watch [our videos](https://www.youtube.com/channel/UC71ceOVy7WtVC7F04BKoEew)\n\n## Licence\nLicensed under the [EUPL](https://joinup.ec.europa.eu/collection/eupl/eupl-text-eupl-12)\n',
     'author': 'Copernicus Marine User Support',
     'author_email': 'servicedesk.cmems@mercator-ocean.eu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 'click>=8.0.4', 'dask>=2022', 'lxml>=4.9.0', 'motuclient>=1.8.4', 'nest-
 asyncio>=1.5.8', 'netCDF4>=1.5.4', 'pydap>=3.2.2', 'pystac>=1.8.3',
 'requests>=2.27.1', 'semver>=3.0.2', 'setuptools>=68.2.2', 'tqdm>=4.65.0',
 'xarray>=2023.4.0', 'zarr>=2.13.3'] entry_points = \ {'console_scripts':
 ['copernicusmarine = '
 'copernicusmarine.command_line_interface.copernicus_marine:
 command_line_interface']} setup_kwargs = { 'name': 'copernicusmarine',
-'version': '1.0.8', 'description': '', 'long_description': '\n
+'version': '1.0.9', 'description': '', 'long_description': '\n
         ************ CCooppeerrnniiccuuss MMaarriinnee SSeerrvviiccee ttoooollbbooxx ((CCLLII && PPyytthhoonn)) ************
 \n
   \n _[_P_y_P_I_]\n _[_P_y_P_I_ _S_u_p_p_o_r_t_e_d_ _V_e_r_s_i_o_n_s_]\n _[_S_u_p_p_o_r_t_e_d_ _P_l_a_t_f_o_r_m_s_]\n _[_L_i_c_e_n_c_e_]\n
 \n\n![Copernicus Marine Service and Mercator Ocean international logos](https:/
 /www.mercator-ocean.eu/wp-content/uploads/2022/05/
 Cartouche_CMEMS_poisson_MOi.png)\n\n## Features\nThe `copernicusmarine` offers
 capabilities through both **Command Line Interface (CLI)** and **Python API**:
@@ -31,16 +31,16 @@
 available and has been uploaded to the conda-forge channel.\n\nHere is the main
 web page of it: [https://anaconda.org/conda-forge/copernicusmarine](https://
 anaconda.org/conda-forge/copernicusmarine)\n\nYou can install it using conda
 though the conda-forge channel with the following command: `conda install
 copernicusmarine -c conda-forge`\n\n### Docker\n\nA docker image is also
 available here: [https://hub.docker.com/r/copernicusmarine/copernicusmarine]
 (https://hub.docker.com/r/copernicusmarine/copernicusmarine)\n\nHere is a basic
-command to run it: `docker run -it --rm copernicusmarine/copernicusmarine:1.0.5
---version`\n\n### Pip\nOtherwise, if you already have an environment (safer to
+command to run it: `docker run -it --rm copernicusmarine/copernicusmarine --
+version`\n\n### Pip\nOtherwise, if you already have an environment (safer to
 clone it), the package can be installed using the `pip` command:
 \n```bash\npython -m pip install copernicusmarine\n```\n\nAnd to **upgrade the
 package** to the newest available version, run:\n```bash\npython -m pip install
 copernicusmarine --upgrade\n```\n\n## User Guide\nFor more comprehensive
 details on how to use the `copernicusmarine`, please refer to our [Help Center]
 (https://help.marine.copernicus.eu/en/collections/4060068-copernicus-marine-
 toolbox). It ensures a smooth migration for existing users of legacy services
@@ -301,14 +301,14 @@
 in touch!\n- Create your [Copernicus Marine Account](https://
 data.marine.copernicus.eu/register)\n- [Log in](https://
 data.marine.copernicus.eu/login?redirect=%2Fproducts) and chat with us (bottom
 right corner of [Copernicus Marine Service](https://marine.copernicus.eu/))\n-
 Join our [training workshops](https://marine.copernicus.eu/services/user-
 learning-services)\n- Network y/our [Copernicus Stories](https://twitter.com/
 cmems_eu)\n- Watch [our videos](https://www.youtube.com/channel/
-UC71ceOVy7WtVC7F04BKoEew)\n\n## Licence\nLicensed under the (EUPL)[https://
-joinup.ec.europa.eu/collection/eupl/eupl-text-eupl-12]\n', 'author':
+UC71ceOVy7WtVC7F04BKoEew)\n\n## Licence\nLicensed under the [EUPL](https://
+joinup.ec.europa.eu/collection/eupl/eupl-text-eupl-12)\n', 'author':
 'Copernicus Marine User Support', 'author_email': 'servicedesk.cmems@mercator-
 ocean.eu', 'maintainer': 'None', 'maintainer_email': 'None', 'url': 'None',
 'packages': packages, 'package_data': package_data, 'install_requires':
 install_requires, 'entry_points': entry_points, 'python_requires':
 '>=3.9,<3.13', } setup(**setup_kwargs)
```

### Comparing `copernicusmarine-1.0.8/PKG-INFO` & `copernicusmarine-1.0.9/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copernicusmarine
-Version: 1.0.8
+Version: 1.0.9
 Summary: 
 License: EUPL-1.2
 Author: Copernicus Marine User Support
 Author-email: servicedesk.cmems@mercator-ocean.eu
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 Classifier: Programming Language :: Python :: 3
@@ -59,15 +59,15 @@
 
 You can install it using conda though the conda-forge channel with the following command: `conda install copernicusmarine -c conda-forge`
 
 ### Docker
 
 A docker image is also available here: [https://hub.docker.com/r/copernicusmarine/copernicusmarine](https://hub.docker.com/r/copernicusmarine/copernicusmarine)
 
-Here is a basic command to run it: `docker run -it --rm copernicusmarine/copernicusmarine:1.0.5 --version`
+Here is a basic command to run it: `docker run -it --rm copernicusmarine/copernicusmarine --version`
 
 ### Pip
 Otherwise, if you already have an environment (safer to clone it), the package can be installed using the `pip` command:
 ```bash
 python -m pip install copernicusmarine
 ```
 
@@ -416,9 +416,9 @@
 - Create your [Copernicus Marine Account](https://data.marine.copernicus.eu/register)
 - [Log in](https://data.marine.copernicus.eu/login?redirect=%2Fproducts) and chat with us (bottom right corner of [Copernicus Marine Service](https://marine.copernicus.eu/))
 - Join our [training workshops](https://marine.copernicus.eu/services/user-learning-services)
 - Network y/our [Copernicus Stories](https://twitter.com/cmems_eu)
 - Watch [our videos](https://www.youtube.com/channel/UC71ceOVy7WtVC7F04BKoEew)
 
 ## Licence
-Licensed under the (EUPL)[https://joinup.ec.europa.eu/collection/eupl/eupl-text-eupl-12]
+Licensed under the [EUPL](https://joinup.ec.europa.eu/collection/eupl/eupl-text-eupl-12)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: copernicusmarine Version: 1.0.8 Summary: License:
+Metadata-Version: 2.1 Name: copernicusmarine Version: 1.0.9 Summary: License:
 EUPL-1.2 Author: Copernicus Marine User Support Author-email:
 servicedesk.cmems@mercator-ocean.eu Requires-Python: >=3.9,<3.13 Classifier:
 License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: aiohttp
 (>=3.8.5) Requires-Dist: boto3 (>=1.25) Requires-Dist: cachier (>=2.2.1)
@@ -31,17 +31,17 @@
 been uploaded to the conda-forge channel. Here is the main web page of it:
 [https://anaconda.org/conda-forge/copernicusmarine](https://anaconda.org/conda-
 forge/copernicusmarine) You can install it using conda though the conda-forge
 channel with the following command: `conda install copernicusmarine -c conda-
 forge` ### Docker A docker image is also available here: [https://
 hub.docker.com/r/copernicusmarine/copernicusmarine](https://hub.docker.com/r/
 copernicusmarine/copernicusmarine) Here is a basic command to run it: `docker
-run -it --rm copernicusmarine/copernicusmarine:1.0.5 --version` ### Pip
-Otherwise, if you already have an environment (safer to clone it), the package
-can be installed using the `pip` command: ```bash python -m pip install
+run -it --rm copernicusmarine/copernicusmarine --version` ### Pip Otherwise, if
+you already have an environment (safer to clone it), the package can be
+installed using the `pip` command: ```bash python -m pip install
 copernicusmarine ``` And to **upgrade the package** to the newest available
 version, run: ```bash python -m pip install copernicusmarine --upgrade ``` ##
 User Guide For more comprehensive details on how to use the `copernicusmarine`,
 please refer to our [Help Center](https://help.marine.copernicus.eu/en/
 collections/4060068-copernicus-marine-toolbox). It ensures a smooth migration
 for existing users of legacy services such as MOTU, OPeNDAP, and FTP. ###
 General configuration #### Cache Usage Cachier library is used for caching part
@@ -291,9 +291,9 @@
 milestones). ## Join the community Get in touch! - Create your [Copernicus
 Marine Account](https://data.marine.copernicus.eu/register) - [Log in](https://
 data.marine.copernicus.eu/login?redirect=%2Fproducts) and chat with us (bottom
 right corner of [Copernicus Marine Service](https://marine.copernicus.eu/)) -
 Join our [training workshops](https://marine.copernicus.eu/services/user-
 learning-services) - Network y/our [Copernicus Stories](https://twitter.com/
 cmems_eu) - Watch [our videos](https://www.youtube.com/channel/
-UC71ceOVy7WtVC7F04BKoEew) ## Licence Licensed under the (EUPL)[https://
-joinup.ec.europa.eu/collection/eupl/eupl-text-eupl-12]
+UC71ceOVy7WtVC7F04BKoEew) ## Licence Licensed under the [EUPL](https://
+joinup.ec.europa.eu/collection/eupl/eupl-text-eupl-12)
```

