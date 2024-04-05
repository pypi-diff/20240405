# Comparing `tmp/drive_ibd-2.6.3.tar.gz` & `tmp/drive_ibd-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drive_ibd-2.6.3.tar", max compression
+gzip compressed data, was "drive_ibd-2.7.0.tar", max compression
```

## Comparing `drive_ibd-2.6.3.tar` & `drive_ibd-2.7.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0    11357 2023-10-09 16:10:09.111536 drive_ibd-2.6.3/LICENSE
--rw-r--r--   0        0        0     1614 2023-12-15 15:41:34.755994 drive_ibd-2.6.3/README.md
--rw-r--r--   0        0        0        0 2023-07-03 15:02:02.235740 drive_ibd-2.6.3/drive/__init__.py
--rwxr-xr-x   0        0        0    12233 2024-03-06 22:07:36.488162 drive_ibd-2.6.3/drive/__main__.py
--rw-r--r--   0        0        0       45 2023-08-03 19:43:34.428381 drive_ibd-2.6.3/drive/cluster/__init__.py
--rw-r--r--   0        0        0    20260 2024-03-06 22:07:36.488162 drive_ibd-2.6.3/drive/cluster/cluster.py
--rw-r--r--   0        0        0      205 2023-08-03 19:43:34.456380 drive_ibd-2.6.3/drive/config.json
--rwxr-xr-x   0        0        0    12405 2024-04-03 20:36:29.343561 drive_ibd-2.6.3/drive/drive.py
--rw-r--r--   0        0        0      129 2023-08-03 19:43:34.456380 drive_ibd-2.6.3/drive/factory/__init__.py
--rw-r--r--   0        0        0     1529 2023-08-03 19:43:34.524379 drive_ibd-2.6.3/drive/factory/factory.py
--rw-r--r--   0        0        0      784 2023-08-03 19:43:34.616376 drive_ibd-2.6.3/drive/factory/loader.py
--rw-r--r--   0        0        0       30 2023-08-03 19:43:34.664375 drive_ibd-2.6.3/drive/filters/__init__.py
--rw-r--r--   0        0        0    18392 2024-03-20 14:52:30.550275 drive_ibd-2.6.3/drive/filters/filter.py
--rw-r--r--   0        0        0       37 2023-04-03 17:12:25.006647 drive_ibd-2.6.3/drive/log/.git
--rw-r--r--   0        0        0       12 2023-04-03 17:12:25.030646 drive_ibd-2.6.3/drive/log/.gitignore
--rw-r--r--   0        0        0     4433 2023-04-03 17:12:25.050646 drive_ibd-2.6.3/drive/log/README.md
--rw-r--r--   0        0        0       33 2023-05-04 22:00:40.780404 drive_ibd-2.6.3/drive/log/__init__.py
--rw-r--r--   0        0        0      225 2023-05-04 22:01:13.999559 drive_ibd-2.6.3/drive/log/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      303 2023-04-07 13:55:36.577011 drive_ibd-2.6.3/drive/log/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     7199 2023-11-25 21:04:36.562604 drive_ibd-2.6.3/drive/log/__pycache__/logger.cpython-311.pyc
--rw-r--r--   0        0        0     2730 2023-04-14 16:19:44.018287 drive_ibd-2.6.3/drive/log/__pycache__/logger.cpython-39.pyc
--rw-r--r--   0        0        0     5031 2023-11-25 21:03:38.140112 drive_ibd-2.6.3/drive/log/logger.py
--rw-r--r--   0        0        0      189 2023-12-15 15:59:21.176736 drive_ibd-2.6.3/drive/models/__init__.py
--rw-r--r--   0        0        0      697 2024-03-19 14:02:55.531225 drive_ibd-2.6.3/drive/models/data_container.py
--rw-r--r--   0        0        0     4576 2024-03-06 22:07:36.492162 drive_ibd-2.6.3/drive/models/generate_indices.py
--rw-r--r--   0        0        0     2161 2023-08-03 19:43:34.884370 drive_ibd-2.6.3/drive/models/networks.py
--rw-r--r--   0        0        0      617 2023-08-03 19:43:34.908369 drive_ibd-2.6.3/drive/models/types.py
--rw-r--r--   0        0        0        0 2023-08-03 19:43:34.908369 drive_ibd-2.6.3/drive/plugins/__init__.py
--rw-r--r--   0        0        0     4435 2023-08-28 16:34:24.642658 drive_ibd-2.6.3/drive/plugins/network_writer.py
--rw-r--r--   0        0        0    11904 2024-04-03 20:36:18.799715 drive_ibd-2.6.3/drive/plugins/pvalues.py
--rw-r--r--   0        0        0        3 2024-03-06 22:07:36.516162 drive_ibd-2.6.3/drive/profile.json
--rw-r--r--   0        0        0       39 2023-12-15 15:59:21.224735 drive_ibd-2.6.3/drive/utilities/callbacks/__init__.py
--rw-r--r--   0        0        0     1821 2023-12-15 15:59:21.248734 drive_ibd-2.6.3/drive/utilities/callbacks/callbacks.py
--rw-r--r--   0        0        0     2263 2023-08-03 19:43:35.044366 drive_ibd-2.6.3/drive/utilities/load_phenotypes.py
--rw-r--r--   0        0        0      121 2023-08-03 19:43:35.076365 drive_ibd-2.6.3/drive/utilities/parser/__init__.py
--rw-r--r--   0        0        0     7763 2024-04-03 20:36:29.307561 drive_ibd-2.6.3/drive/utilities/parser/case_file_parser.py
--rw-r--r--   0        0        0      919 2023-08-03 19:43:35.156363 drive_ibd-2.6.3/drive/utilities/parser/phenotype_descriptions_parser.py
--rw-r--r--   0        0        0     2211 2024-04-03 20:05:55.639813 drive_ibd-2.6.3/pyproject.toml
--rw-r--r--   0        0        0     2868 1970-01-01 00:00:00.000000 drive_ibd-2.6.3/setup.py
--rw-r--r--   0        0        0     2828 1970-01-01 00:00:00.000000 drive_ibd-2.6.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-10-09 16:10:09.111536 drive_ibd-2.7.0/LICENSE
+-rw-r--r--   0        0        0     1614 2023-12-15 15:41:34.755994 drive_ibd-2.7.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-03 15:02:02.235740 drive_ibd-2.7.0/drive/__init__.py
+-rwxr-xr-x   0        0        0    12233 2024-04-05 15:53:53.695267 drive_ibd-2.7.0/drive/__main__.py
+-rw-r--r--   0        0        0       45 2023-08-03 19:43:34.428381 drive_ibd-2.7.0/drive/cluster/__init__.py
+-rw-r--r--   0        0        0    20260 2024-03-06 22:07:36.488162 drive_ibd-2.7.0/drive/cluster/cluster.py
+-rw-r--r--   0        0        0      205 2023-08-03 19:43:34.456380 drive_ibd-2.7.0/drive/config.json
+-rwxr-xr-x   0        0        0    12405 2024-04-05 15:53:53.699267 drive_ibd-2.7.0/drive/drive.py
+-rw-r--r--   0        0        0      129 2023-08-03 19:43:34.456380 drive_ibd-2.7.0/drive/factory/__init__.py
+-rw-r--r--   0        0        0     1529 2023-08-03 19:43:34.524379 drive_ibd-2.7.0/drive/factory/factory.py
+-rw-r--r--   0        0        0      784 2023-08-03 19:43:34.616376 drive_ibd-2.7.0/drive/factory/loader.py
+-rw-r--r--   0        0        0       30 2023-08-03 19:43:34.664375 drive_ibd-2.7.0/drive/filters/__init__.py
+-rw-r--r--   0        0        0    18393 2024-04-05 15:53:55.759238 drive_ibd-2.7.0/drive/filters/filter.py
+-rw-r--r--   0        0        0       37 2023-04-03 17:12:25.006647 drive_ibd-2.7.0/drive/log/.git
+-rw-r--r--   0        0        0       12 2023-04-03 17:12:25.030646 drive_ibd-2.7.0/drive/log/.gitignore
+-rw-r--r--   0        0        0     4433 2023-04-03 17:12:25.050646 drive_ibd-2.7.0/drive/log/README.md
+-rw-r--r--   0        0        0       33 2023-05-04 22:00:40.780404 drive_ibd-2.7.0/drive/log/__init__.py
+-rw-r--r--   0        0        0      225 2023-05-04 22:01:13.999559 drive_ibd-2.7.0/drive/log/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      303 2023-04-07 13:55:36.577011 drive_ibd-2.7.0/drive/log/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     7199 2023-11-25 21:04:36.562604 drive_ibd-2.7.0/drive/log/__pycache__/logger.cpython-311.pyc
+-rw-r--r--   0        0        0     2730 2023-04-14 16:19:44.018287 drive_ibd-2.7.0/drive/log/__pycache__/logger.cpython-39.pyc
+-rw-r--r--   0        0        0     5031 2024-04-05 15:53:55.955235 drive_ibd-2.7.0/drive/log/logger.py
+-rw-r--r--   0        0        0      189 2023-12-15 15:59:21.176736 drive_ibd-2.7.0/drive/models/__init__.py
+-rw-r--r--   0        0        0      697 2024-03-19 14:02:55.531225 drive_ibd-2.7.0/drive/models/data_container.py
+-rw-r--r--   0        0        0     4576 2024-03-06 22:07:36.492162 drive_ibd-2.7.0/drive/models/generate_indices.py
+-rw-r--r--   0        0        0     2161 2023-08-03 19:43:34.884370 drive_ibd-2.7.0/drive/models/networks.py
+-rw-r--r--   0        0        0      617 2023-08-03 19:43:34.908369 drive_ibd-2.7.0/drive/models/types.py
+-rw-r--r--   0        0        0        0 2023-08-03 19:43:34.908369 drive_ibd-2.7.0/drive/plugins/__init__.py
+-rw-r--r--   0        0        0     4475 2024-04-05 15:32:38.137080 drive_ibd-2.7.0/drive/plugins/network_writer.py
+-rw-r--r--   0        0        0    13389 2024-04-05 15:32:28.593218 drive_ibd-2.7.0/drive/plugins/pvalues.py
+-rw-r--r--   0        0        0        3 2024-03-06 22:07:36.516162 drive_ibd-2.7.0/drive/profile.json
+-rw-r--r--   0        0        0       39 2023-12-15 15:59:21.224735 drive_ibd-2.7.0/drive/utilities/callbacks/__init__.py
+-rw-r--r--   0        0        0     1821 2024-04-05 15:53:53.827265 drive_ibd-2.7.0/drive/utilities/callbacks/callbacks.py
+-rw-r--r--   0        0        0     2263 2023-08-03 19:43:35.044366 drive_ibd-2.7.0/drive/utilities/load_phenotypes.py
+-rw-r--r--   0        0        0      121 2023-08-03 19:43:35.076365 drive_ibd-2.7.0/drive/utilities/parser/__init__.py
+-rw-r--r--   0        0        0     7764 2024-04-05 15:53:53.739266 drive_ibd-2.7.0/drive/utilities/parser/case_file_parser.py
+-rw-r--r--   0        0        0      919 2023-08-03 19:43:35.156363 drive_ibd-2.7.0/drive/utilities/parser/phenotype_descriptions_parser.py
+-rw-r--r--   0        0        0     2211 2024-04-05 15:55:23.838003 drive_ibd-2.7.0/pyproject.toml
+-rw-r--r--   0        0        0     2868 1970-01-01 00:00:00.000000 drive_ibd-2.7.0/setup.py
+-rw-r--r--   0        0        0     2828 1970-01-01 00:00:00.000000 drive_ibd-2.7.0/PKG-INFO
```

### Comparing `drive_ibd-2.6.3/LICENSE` & `drive_ibd-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.6.3/README.md` & `drive_ibd-2.7.0/README.md`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.6.3/drive/__main__.py` & `drive_ibd-2.7.0/drive/__main__.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
+import argparse
 import json
 import re
 from datetime import datetime
 from pathlib import Path
-import argparse
-from rich_argparse import RichHelpFormatter
 
+from rich_argparse import RichHelpFormatter
 
 import drive.factory as factory
 from drive.cluster import ClusterHandler, cluster
 from drive.filters import IbdFilter
 from drive.log import CustomLogger
 from drive.models import Data, Genes, create_indices
 from drive.utilities.callbacks import CheckInputExist
```

### Comparing `drive_ibd-2.6.3/drive/cluster/cluster.py` & `drive_ibd-2.7.0/drive/cluster/cluster.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.6.3/drive/drive.py` & `drive_ibd-2.7.0/drive/drive.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
+import argparse
 import json
 import re
 from datetime import datetime
-from pathlib import Path
-import argparse
-from rich_argparse import RichHelpFormatter
 from importlib.metadata import version
+from pathlib import Path
 
+from rich_argparse import RichHelpFormatter
 
 import drive.factory as factory
 from drive.cluster import ClusterHandler, cluster
 from drive.filters import IbdFilter
 from drive.log import CustomLogger
 from drive.models import Data, Genes, create_indices
 from drive.utilities.callbacks import CheckInputExist
```

### Comparing `drive_ibd-2.6.3/drive/factory/factory.py` & `drive_ibd-2.7.0/drive/factory/factory.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.6.3/drive/factory/loader.py` & `drive_ibd-2.7.0/drive/factory/loader.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.6.3/drive/filters/filter.py` & `drive_ibd-2.7.0/drive/filters/filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import sys
 from dataclasses import dataclass, field
+from datetime import datetime
 from pathlib import Path
 from typing import Callable, Dict, Iterator, List, Optional, TypeVar
+
 from pandas import DataFrame, concat, read_csv
-from datetime import datetime
 
 from drive.log import CustomLogger
 from drive.models import FileIndices, Genes
 
 logger = CustomLogger.get_logger(__name__)
 
 # we are going to create two exception class for the vertex
```

### Comparing `drive_ibd-2.6.3/drive/log/README.md` & `drive_ibd-2.7.0/drive/log/README.md`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.6.3/drive/log/__pycache__/logger.cpython-311.pyc` & `drive_ibd-2.7.0/drive/log/__pycache__/logger.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.6.3/drive/log/__pycache__/logger.cpython-39.pyc` & `drive_ibd-2.7.0/drive/log/__pycache__/logger.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.6.3/drive/log/logger.py` & `drive_ibd-2.7.0/drive/log/logger.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
+from argparse import Namespace
 from pathlib import Path
 from typing import Any, Dict
-from argparse import Namespace
 
 # We are going to configure a specific logging level for
 # VERBOSE versus INFO
 logging.VERBOSE = logging.INFO - 5
 
 
 class CustomLogger(logging.getLoggerClass()):
```

### Comparing `drive_ibd-2.6.3/drive/models/data_container.py` & `drive_ibd-2.7.0/drive/models/data_container.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.6.3/drive/models/generate_indices.py` & `drive_ibd-2.7.0/drive/models/generate_indices.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.6.3/drive/models/networks.py` & `drive_ibd-2.7.0/drive/models/networks.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.6.3/drive/models/types.py` & `drive_ibd-2.7.0/drive/models/types.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.6.3/drive/plugins/network_writer.py` & `drive_ibd-2.7.0/drive/plugins/network_writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         else:
             # We need to add columns for the min pvalue descriptions
             header_str += "\tmin_pvalue\tmin_phenotype\tmin_phenotype_description"
             # for each phenotype we are going to create 4 columns for the number
             # of cases in the network, The case ids in the network the number of
             # excluded individuals in the network, and the pvalue for the phenotype
             for column in phenotypes:
-                header_str += f"\t{column + '_case_count_in_network'}\t{column + 'cases_in_network'}\t{column + '_excluded_in_network'}\t{column + '_pvalue'}"  # noqa: E501
+                header_str += f"\t{column + '_case_count_in_network'}\t{column + 'cases_in_network'}\t{column + '_excluded_count_in_network'}\t{column + 'excluded_in_network'}\t{column + '_pvalue'}"  # noqa: E501
 
             return header_str + "\n"
 
     @staticmethod
     def _create_network_info_str(
         network: Network_Interface, phenotypes: List[str]
     ) -> str:
```

### Comparing `drive_ibd-2.6.3/drive/plugins/pvalues.py` & `drive_ibd-2.7.0/drive/plugins/pvalues.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass
-from typing import Dict, List, Set, Tuple
+from typing import Dict, List, Optional, Set, Tuple
 
 from numpy import float64
 from scipy.stats import binomtest
 
 from drive.factory import factory_register
 from drive.log import CustomLogger
 from drive.models import Data_Interface, Network_Interface
@@ -117,36 +117,78 @@
         # determine the number of carriers in the network
 
         return len(network.members.intersection(phenotype_counts.get("cases")))
 
     @staticmethod
     def _get_carriers_in_network(
         phenotype_counts: Dict[str, List[str]], network: Network_Interface
-    ) -> Set[str]:
+    ) -> str:
         """Generate a set of cases that are in the network
 
         Parameters
         ----------
         phenotype_counts : Dict[str, List[str]]
             Dictionary that has list for individuals who are
             cases, controls, or exclusions.
 
         network : Network_Interface
             Network object with information about members of
             the networks and what haplotypes are in the network
 
         Returns
         -------
-        Set[str]
-            returns a set of individuals that are in both the phenotype_counts
-            case set and the network members set
+        str
+            returns a string of individuals that are in both the phenotype_counts
+            case set and the network members set. If this interection is empty
+            then it returns a str "N/A"
         """
         # determine the number of carriers in the network
+        case_individuals = network.members.intersection(phenotype_counts.get("cases"))
 
-        return network.members.intersection(phenotype_counts.get("cases"))
+        if case_individuals:
+            return ", ".join(
+                network.members.intersection(phenotype_counts.get("cases"))
+            )  # noqa: E501
+        else:
+            return "N/A"
+
+    @staticmethod
+    def _get_exclusions_in_network(
+        phenotype_counts: Dict[str, List[str]], network: Network_Interface
+    ) -> str:
+        """Generate a set of cases that are in the network
+
+        Parameters
+        ----------
+        phenotype_counts : Dict[str, List[str]]
+            Dictionary that has list for individuals who are
+            cases, controls, or exclusions.
+
+        network : Network_Interface
+            Network object with information about members of
+            the networks and what haplotypes are in the network
+
+        Returns
+        -------
+        str
+            returns a string of individuals that are in both the phenotype_counts
+            exclusion set and the network members set. If this interection is
+            empty then it returns a str "N/A"
+        """
+        # determine the number of carriers in the network
+        excluded_individuals = network.members.intersection(
+            phenotype_counts.get("excluded")
+        )  # noqa: E501
+
+        if excluded_individuals:
+            return ", ".join(
+                network.members.intersection(phenotype_counts.get("excluded"))
+            )  # noqa: E501
+        else:
+            "N/A"
 
     def _remove_exclusions(
         phenotype_counts: Dict[str, List[str]], network: Network_Interface
     ) -> Tuple[int, int]:
         """determine size of network after removing excluded
         individuals
 
@@ -162,15 +204,15 @@
 
         Returns
         -------
         Tuple[int, int]
             returns the number of individuals in the network,
             not counting those individuals classified as
             excluded in the phenotype_counts dictionary. Also
-            returns the number of individuals excluded.
+            returns the number of individuals excluded. Also returns the
         """
 
         return (
             len(network.members.difference(phenotype_counts.get("excluded"))),
             len(network.members.intersection(phenotype_counts.get("excluded"))),
         )
 
@@ -225,15 +267,19 @@
                     phenotype, phenotype_counts
                 )
 
                 num_carriers_in_network = Pvalues._get_carrier_count_in_network(
                     phenotype_counts, network
                 )
 
-                carrier_set = Pvalues._get_carriers_in_network(
+                carrier_str = Pvalues._get_carriers_in_network(
+                    phenotype_counts, network
+                )
+
+                exclusion_str = Pvalues._get_exclusions_in_network(
                     phenotype_counts, network
                 )
 
                 (
                     network_size_after_exclusions,
                     excluded_count,
                 ) = Pvalues._remove_exclusions(phenotype_counts, network)
@@ -243,18 +289,16 @@
                     phenotype,
                     phenotype_freq,
                     num_carriers_in_network,
                     network_size_after_exclusions,
                 )
 
                 # Next two lines create the string and then concats it to the output_str
-                if carrier_set:
-                    phenotype_str = f"{num_carriers_in_network}\t{', '.join(carrier_set)}\t{excluded_count}\t{pvalue}"  # noqa: E501
-                else:
-                    phenotype_str = f"{num_carriers_in_network}\tN/A\t{excluded_count}\t{pvalue}"  # noqa: E501
+
+                phenotype_str = f"{num_carriers_in_network}\t{carrier_str}\t{excluded_count}\t{exclusion_str}\t{pvalue}"  # noqa: E501
 
                 phenotype_pvalues[phenotype] = phenotype_str
 
                 # Now we will see if the phecode is lower then the cur_min_pvalue.
                 # If it is then we will change the cur_min_pvalue and we will
                 # update the cur_min_phecode
                 if pvalue < cur_min_pvalue and pvalue != 0:
```

### Comparing `drive_ibd-2.6.3/drive/utilities/callbacks/callbacks.py` & `drive_ibd-2.7.0/drive/utilities/callbacks/callbacks.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from pathlib import Path
 import argparse
 import sys
+from pathlib import Path
 
 
 class CheckInputExist(argparse.Action):
     def __init__(self, option_strings, dest, nargs=None, **kwargs) -> None:
         if nargs is not None:
             raise ValueError("nargs not allowed")
         super(CheckInputExist, self).__init__(option_strings, dest, **kwargs)
```

### Comparing `drive_ibd-2.6.3/drive/utilities/load_phenotypes.py` & `drive_ibd-2.7.0/drive/utilities/load_phenotypes.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.6.3/drive/utilities/parser/case_file_parser.py` & `drive_ibd-2.7.0/drive/utilities/parser/case_file_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Module to faciliate the user in parsing the phenotype file by incorporating multiple 
 ecodings, separators, and by handling multiple errors."""
 
 from logging import Logger
 from pathlib import Path
 from typing import Dict, List, Optional, Set, Tuple, TypeVar, Union
+
 import pandas as pd
 
 from drive.log import CustomLogger
 
 logger: Logger = CustomLogger.get_logger(__name__)
 
 # creating a type annotation for the PhenotypeFileParser class
```

### Comparing `drive_ibd-2.6.3/drive/utilities/parser/phenotype_descriptions_parser.py` & `drive_ibd-2.7.0/drive/utilities/parser/phenotype_descriptions_parser.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.6.3/pyproject.toml` & `drive_ibd-2.7.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "drive-ibd"
 
-version = "2.6.3"
+version = "2.7.0"
 description = "cli tool to identify networks of individuals who share IBD segments overlapping loci of interest"
 authors = ["James Baker <james.baker@vanderbilt.edu>", "Hung-Hsin Chen <hung-hsin.chen.1@vumc.org>", "Jennifer E. Below <jennifer.e.below@vumc.org>"]
 maintainers = ["James Baker <james.baker@vanderbilt.edu>", "Hung-Hsin Chen <hung-hsin.chen.1@vumc.org>"]
 repository = "https://github.com/belowlab/drive"
 homepage = "https://drive-ibd.readthedocs.io/en/latest/"
 readme = "README.md"
 keywords = ["python", "genetics", "identity by descent", "relatedness"]
```

### Comparing `drive_ibd-2.6.3/setup.py` & `drive_ibd-2.7.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
  'scipy>=1.10.1,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['drive = drive.drive:main']}
 
 setup_kwargs = {
     'name': 'drive-ibd',
-    'version': '2.6.3',
+    'version': '2.7.0',
     'description': 'cli tool to identify networks of individuals who share IBD segments overlapping loci of interest',
     'long_description': '[![Documentation Status](https://readthedocs.org/projects/drive-ibd/badge/?version=latest)](https://drive-ibd.readthedocs.io/en/latest/?badge=latest)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![PyPI version](https://badge.fury.io/py/drive-ibd.svg)](https://badge.fury.io/py/drive-ibd)\n\n# DRIVE:\n\nThis repository contains the source code for the tool DRIVE (Distant Relatedness for Identification and Variant Evaluation) is a novel approach to IBD-based genotype inference used to identify shared chromosomal segments in dense genetic arrays. DRIVE implements a random walk algorithm that identifies clusters of individuals who pairwise share an IBD segment overlapping a locus of interest. This tool was developed in python by the Below Lab at Vanderbilt University. The documentation for how to use this tool can be found here [DRIVE documentation](https://drive-ibd.readthedocs.io/en/latest/)\n\n## Installing DRIVE:\nDRIVE is available on PYPI and can easily be installed using the following command:\n\n```bash\npip install drive-ibd\n```\nIt is recommended to install DRIVE within a virtual environment such as venv, or conda. More information about this process can be found within the documentation.\n\nIf the user wishes to develop DRIVE or install the program from source then they can clone the repository. This process is described under the section called "Github Installation" in the documentation.\n\n### Reporting issues:\nIf you wish to report a bug or propose a feature you can find templates under the .github/ISSUE_TEMPLATE directory.\n\n',
     'author': 'James Baker',
     'author_email': 'james.baker@vanderbilt.edu',
     'maintainer': 'James Baker',
     'maintainer_email': 'james.baker@vanderbilt.edu',
     'url': 'https://drive-ibd.readthedocs.io/en/latest/',
```

### Comparing `drive_ibd-2.6.3/PKG-INFO` & `drive_ibd-2.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drive-ibd
-Version: 2.6.3
+Version: 2.7.0
 Summary: cli tool to identify networks of individuals who share IBD segments overlapping loci of interest
 Home-page: https://drive-ibd.readthedocs.io/en/latest/
 Keywords: python,genetics,identity by descent,relatedness
 Author: James Baker
 Author-email: james.baker@vanderbilt.edu
 Maintainer: James Baker
 Maintainer-email: james.baker@vanderbilt.edu
```

