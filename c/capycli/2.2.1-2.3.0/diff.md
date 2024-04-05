# Comparing `tmp/capycli-2.2.1.tar.gz` & `tmp/capycli-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "capycli-2.2.1.tar", max compression
+gzip compressed data, was "capycli-2.3.0.tar", max compression
```

## Comparing `capycli-2.2.1.tar` & `capycli-2.3.0.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0     6267 2023-05-17 09:09:21.101912 capycli-2.2.1/capycli/__init__.py
--rw-r--r--   0        0        0      445 2023-05-17 09:09:21.102694 capycli-2.2.1/capycli/__main__.py
--rw-r--r--   0        0        0      376 2023-05-17 09:09:21.103422 capycli-2.2.1/capycli/bom/__init__.py
--rw-r--r--   0        0        0     7179 2024-01-28 14:53:16.289861 capycli-2.2.1/capycli/bom/bom_convert.py
--rw-r--r--   0        0        0     8410 2024-01-28 15:04:23.907189 capycli-2.2.1/capycli/bom/check_bom.py
--rw-r--r--   0        0        0     8986 2024-01-28 15:05:06.505097 capycli-2.2.1/capycli/bom/check_bom_item_status.py
--rw-r--r--   0        0        0    11158 2024-01-28 14:53:16.309388 capycli-2.2.1/capycli/bom/check_granularity.py
--rw-r--r--   0        0        0    30972 2024-01-28 15:05:23.289811 capycli-2.2.1/capycli/bom/create_components.py
--rw-r--r--   0        0        0     2337 2024-01-28 14:53:16.324753 capycli-2.2.1/capycli/bom/csv.py
--rw-r--r--   0        0        0    10969 2024-01-28 14:53:16.329827 capycli-2.2.1/capycli/bom/diff_bom.py
--rw-r--r--   0        0        0     8927 2024-01-28 14:53:16.329827 capycli-2.2.1/capycli/bom/download_sources.py
--rw-r--r--   0        0        0    13074 2024-01-28 14:53:16.339751 capycli-2.2.1/capycli/bom/filter_bom.py
--rw-r--r--   0        0        0    29044 2024-02-20 21:21:58.815954 capycli-2.2.1/capycli/bom/findsources.py
--rw-r--r--   0        0        0     4931 2024-01-28 14:53:16.354988 capycli-2.2.1/capycli/bom/handle_bom.py
--rw-r--r--   0        0        0     2423 2024-01-28 14:53:16.359544 capycli-2.2.1/capycli/bom/html.py
--rw-r--r--   0        0        0    12485 2024-01-28 14:53:16.359544 capycli-2.2.1/capycli/bom/legacy.py
--rw-r--r--   0        0        0     5878 2023-05-17 09:09:21.119771 capycli-2.2.1/capycli/bom/legacy_cx.py
--rw-r--r--   0        0        0    46924 2024-01-28 14:53:16.370105 capycli-2.2.1/capycli/bom/map_bom.py
--rw-r--r--   0        0        0     6219 2024-01-28 14:53:16.379638 capycli-2.2.1/capycli/bom/merge_bom.py
--rw-r--r--   0        0        0     2915 2024-01-28 14:53:16.379638 capycli-2.2.1/capycli/bom/plaintext.py
--rw-r--r--   0        0        0     3017 2024-01-28 14:53:16.389753 capycli-2.2.1/capycli/bom/show_bom.py
--rw-r--r--   0        0        0      350 2023-05-17 09:09:21.122947 capycli-2.2.1/capycli/common/__init__.py
--rw-r--r--   0        0        0    24813 2024-01-28 14:53:16.389753 capycli-2.2.1/capycli/common/capycli_bom_support.py
--rw-r--r--   0        0        0     6025 2024-01-28 14:53:16.403123 capycli-2.2.1/capycli/common/comparable_version.py
--rw-r--r--   0        0        0     9025 2024-01-28 14:53:16.409692 capycli-2.2.1/capycli/common/component_cache.py
--rw-r--r--   0        0        0     2097 2023-05-17 09:09:21.126220 capycli-2.2.1/capycli/common/dependencies_base.py
--rw-r--r--   0        0        0      741 2024-01-28 14:53:16.409692 capycli-2.2.1/capycli/common/file_support.py
--rw-r--r--   0        0        0     4063 2024-01-28 14:53:16.419864 capycli-2.2.1/capycli/common/html_support.py
--rw-r--r--   0        0        0     1192 2024-01-28 14:53:16.419864 capycli-2.2.1/capycli/common/json_support.py
--rw-r--r--   0        0        0     4266 2024-01-28 14:53:16.429366 capycli-2.2.1/capycli/common/map_result.py
--rw-r--r--   0        0        0     1732 2024-01-28 14:53:16.439635 capycli-2.2.1/capycli/common/print.py
--rw-r--r--   0        0        0     7613 2024-01-28 14:53:16.439635 capycli-2.2.1/capycli/common/purl_service.py
--rw-r--r--   0        0        0     3419 2024-01-28 21:52:10.032716 capycli-2.2.1/capycli/common/purl_store.py
--rw-r--r--   0        0        0     3310 2024-01-28 14:53:16.453230 capycli-2.2.1/capycli/common/purl_utils.py
--rw-r--r--   0        0        0     7012 2024-01-28 15:06:20.190107 capycli-2.2.1/capycli/common/script_base.py
--rw-r--r--   0        0        0     2971 2024-01-28 14:53:16.470534 capycli-2.2.1/capycli/common/script_support.py
--rw-r--r--   0        0        0      329 2023-05-17 09:09:21.130298 capycli-2.2.1/capycli/data/__init__.py
--rw-r--r--   0        0        0   240298 2023-07-30 14:38:15.453416 capycli-2.2.1/capycli/data/granularity_list.csv
--rw-r--r--   0        0        0      344 2023-05-17 09:09:21.130298 capycli-2.2.1/capycli/dependencies/__init__.py
--rw-r--r--   0        0        0     2752 2024-01-28 14:53:16.470534 capycli-2.2.1/capycli/dependencies/handle_dependencies.py
--rw-r--r--   0        0        0    12549 2024-01-28 17:43:25.157496 capycli-2.2.1/capycli/dependencies/javascript.py
--rw-r--r--   0        0        0    13907 2024-03-08 13:04:38.749772 capycli-2.2.1/capycli/dependencies/maven_list.py
--rw-r--r--   0        0        0     5385 2024-01-28 14:53:16.489438 capycli-2.2.1/capycli/dependencies/maven_pom.py
--rw-r--r--   0        0        0     7085 2024-01-28 14:53:16.503455 capycli-2.2.1/capycli/dependencies/nuget.py
--rw-r--r--   0        0        0    19145 2024-01-28 14:53:16.509561 capycli-2.2.1/capycli/dependencies/python.py
--rw-r--r--   0        0        0      363 2023-05-17 09:09:21.133323 capycli-2.2.1/capycli/main/__init__.py
--rw-r--r--   0        0        0     5904 2024-01-28 14:53:16.529337 capycli-2.2.1/capycli/main/application.py
--rw-r--r--   0        0        0     4061 2024-01-28 14:53:16.529337 capycli-2.2.1/capycli/main/argument_parser.py
--rw-r--r--   0        0        0      881 2024-01-28 14:53:16.539568 capycli-2.2.1/capycli/main/cli.py
--rw-r--r--   0        0        0      441 2023-05-17 09:09:21.135549 capycli-2.2.1/capycli/main/exceptions.py
--rw-r--r--   0        0        0    15118 2024-01-28 14:56:39.313238 capycli-2.2.1/capycli/main/options.py
--rw-r--r--   0        0        0     1576 2023-05-17 09:09:21.135787 capycli-2.2.1/capycli/main/result_codes.py
--rw-r--r--   0        0        0     1572 2024-01-28 14:53:16.553253 capycli-2.2.1/capycli/mapping/handle_mapping.py
--rw-r--r--   0        0        0     7200 2024-01-28 14:53:16.553253 capycli-2.2.1/capycli/mapping/mapping_to_html.py
--rw-r--r--   0        0        0     8347 2024-01-28 14:53:16.564831 capycli-2.2.1/capycli/mapping/mapping_to_xlsx.py
--rw-r--r--   0        0        0     1643 2024-01-28 14:53:16.570018 capycli-2.2.1/capycli/moverview/handle_moverview.py
--rw-r--r--   0        0        0     4840 2024-01-28 14:53:16.570018 capycli-2.2.1/capycli/moverview/moverview_to_html.py
--rw-r--r--   0        0        0     7224 2024-01-28 14:53:16.579565 capycli-2.2.1/capycli/moverview/moverview_to_xlsx.py
--rw-r--r--   0        0        0      330 2023-05-17 09:09:21.138795 capycli-2.2.1/capycli/project/__init__.py
--rw-r--r--   0        0        0    13486 2024-01-28 14:53:16.589401 capycli-2.2.1/capycli/project/check_prerequisites.py
--rw-r--r--   0        0        0     9756 2024-01-28 15:06:45.340845 capycli-2.2.1/capycli/project/create_bom.py
--rw-r--r--   0        0        0    16453 2024-03-08 14:28:16.162124 capycli-2.2.1/capycli/project/create_project.py
--rw-r--r--   0        0        0    23442 2024-01-28 14:53:16.609443 capycli-2.2.1/capycli/project/create_readme.py
--rw-r--r--   0        0        0     5605 2024-01-28 14:53:16.609443 capycli-2.2.1/capycli/project/find_project.py
--rw-r--r--   0        0        0    10478 2024-01-28 15:07:12.781127 capycli-2.2.1/capycli/project/get_license_info.py
--rw-r--r--   0        0        0     4454 2024-01-28 14:53:16.629590 capycli-2.2.1/capycli/project/handle_project.py
--rw-r--r--   0        0        0     9000 2024-01-28 15:02:03.962221 capycli-2.2.1/capycli/project/show_ecc.py
--rw-r--r--   0        0        0     8329 2024-01-28 14:53:16.639627 capycli-2.2.1/capycli/project/show_licenses.py
--rw-r--r--   0        0        0    10069 2024-01-28 14:53:16.639627 capycli-2.2.1/capycli/project/show_project.py
--rw-r--r--   0        0        0     9709 2024-01-28 15:07:26.594053 capycli-2.2.1/capycli/project/show_vulnerabilities.py
--rw-r--r--   0        0        0     1218 2024-01-28 14:56:39.309682 capycli-2.2.1/License.md
-drwxr-xr-x   0        0        0        0 2023-05-17 09:11:25.459479 capycli-2.2.1/LICENSES/
--rw-r--r--   0        0        0     3107 2024-03-08 12:16:33.093647 capycli-2.2.1/pyproject.toml
--rw-r--r--   0        0        0    12923 2024-01-28 14:56:39.309682 capycli-2.2.1/Readme.md
--rw-r--r--   0        0        0    14430 1970-01-01 00:00:00.000000 capycli-2.2.1/PKG-INFO
+-rw-r--r--   0        0        0     6267 2023-05-17 09:09:21.101912 capycli-2.3.0/capycli/__init__.py
+-rw-r--r--   0        0        0      445 2023-05-17 09:09:21.102694 capycli-2.3.0/capycli/__main__.py
+-rw-r--r--   0        0        0      376 2023-05-17 09:09:21.103422 capycli-2.3.0/capycli/bom/__init__.py
+-rw-r--r--   0        0        0     7179 2024-01-28 14:53:16.289861 capycli-2.3.0/capycli/bom/bom_convert.py
+-rw-r--r--   0        0        0     8410 2024-01-28 15:04:23.907189 capycli-2.3.0/capycli/bom/check_bom.py
+-rw-r--r--   0        0        0     8986 2024-01-28 15:05:06.505097 capycli-2.3.0/capycli/bom/check_bom_item_status.py
+-rw-r--r--   0        0        0    11158 2024-01-28 14:53:16.309388 capycli-2.3.0/capycli/bom/check_granularity.py
+-rw-r--r--   0        0        0    30972 2024-01-28 15:05:23.289811 capycli-2.3.0/capycli/bom/create_components.py
+-rw-r--r--   0        0        0     2337 2024-01-28 14:53:16.324753 capycli-2.3.0/capycli/bom/csv.py
+-rw-r--r--   0        0        0    10969 2024-01-28 14:53:16.329827 capycli-2.3.0/capycli/bom/diff_bom.py
+-rw-r--r--   0        0        0     8927 2024-01-28 14:53:16.329827 capycli-2.3.0/capycli/bom/download_sources.py
+-rw-r--r--   0        0        0    13074 2024-01-28 14:53:16.339751 capycli-2.3.0/capycli/bom/filter_bom.py
+-rw-r--r--   0        0        0    29044 2024-02-20 21:21:58.815954 capycli-2.3.0/capycli/bom/findsources.py
+-rw-r--r--   0        0        0     4931 2024-01-28 14:53:16.354988 capycli-2.3.0/capycli/bom/handle_bom.py
+-rw-r--r--   0        0        0     2423 2024-01-28 14:53:16.359544 capycli-2.3.0/capycli/bom/html.py
+-rw-r--r--   0        0        0    12485 2024-01-28 14:53:16.359544 capycli-2.3.0/capycli/bom/legacy.py
+-rw-r--r--   0        0        0     5878 2023-05-17 09:09:21.119771 capycli-2.3.0/capycli/bom/legacy_cx.py
+-rw-r--r--   0        0        0    46924 2024-01-28 14:53:16.370105 capycli-2.3.0/capycli/bom/map_bom.py
+-rw-r--r--   0        0        0     6219 2024-01-28 14:53:16.379638 capycli-2.3.0/capycli/bom/merge_bom.py
+-rw-r--r--   0        0        0     2915 2024-01-28 14:53:16.379638 capycli-2.3.0/capycli/bom/plaintext.py
+-rw-r--r--   0        0        0     3017 2024-01-28 14:53:16.389753 capycli-2.3.0/capycli/bom/show_bom.py
+-rw-r--r--   0        0        0      350 2023-05-17 09:09:21.122947 capycli-2.3.0/capycli/common/__init__.py
+-rw-r--r--   0        0        0    24813 2024-01-28 14:53:16.389753 capycli-2.3.0/capycli/common/capycli_bom_support.py
+-rw-r--r--   0        0        0     6025 2024-01-28 14:53:16.403123 capycli-2.3.0/capycli/common/comparable_version.py
+-rw-r--r--   0        0        0     9025 2024-01-28 14:53:16.409692 capycli-2.3.0/capycli/common/component_cache.py
+-rw-r--r--   0        0        0     2097 2023-05-17 09:09:21.126220 capycli-2.3.0/capycli/common/dependencies_base.py
+-rw-r--r--   0        0        0      741 2024-01-28 14:53:16.409692 capycli-2.3.0/capycli/common/file_support.py
+-rw-r--r--   0        0        0     4063 2024-01-28 14:53:16.419864 capycli-2.3.0/capycli/common/html_support.py
+-rw-r--r--   0        0        0     1192 2024-01-28 14:53:16.419864 capycli-2.3.0/capycli/common/json_support.py
+-rw-r--r--   0        0        0     4266 2024-01-28 14:53:16.429366 capycli-2.3.0/capycli/common/map_result.py
+-rw-r--r--   0        0        0     1732 2024-01-28 14:53:16.439635 capycli-2.3.0/capycli/common/print.py
+-rw-r--r--   0        0        0     7613 2024-01-28 14:53:16.439635 capycli-2.3.0/capycli/common/purl_service.py
+-rw-r--r--   0        0        0     3419 2024-01-28 21:52:10.032716 capycli-2.3.0/capycli/common/purl_store.py
+-rw-r--r--   0        0        0     3310 2024-01-28 14:53:16.453230 capycli-2.3.0/capycli/common/purl_utils.py
+-rw-r--r--   0        0        0     7012 2024-01-28 15:06:20.190107 capycli-2.3.0/capycli/common/script_base.py
+-rw-r--r--   0        0        0     2971 2024-01-28 14:53:16.470534 capycli-2.3.0/capycli/common/script_support.py
+-rw-r--r--   0        0        0      329 2023-05-17 09:09:21.130298 capycli-2.3.0/capycli/data/__init__.py
+-rw-r--r--   0        0        0   278377 2024-04-02 20:00:29.579607 capycli-2.3.0/capycli/data/granularity_list.csv
+-rw-r--r--   0        0        0      344 2023-05-17 09:09:21.130298 capycli-2.3.0/capycli/dependencies/__init__.py
+-rw-r--r--   0        0        0     2752 2024-01-28 14:53:16.470534 capycli-2.3.0/capycli/dependencies/handle_dependencies.py
+-rw-r--r--   0        0        0    12549 2024-01-28 17:43:25.157496 capycli-2.3.0/capycli/dependencies/javascript.py
+-rw-r--r--   0        0        0    13907 2024-03-08 13:04:38.749772 capycli-2.3.0/capycli/dependencies/maven_list.py
+-rw-r--r--   0        0        0     5385 2024-01-28 14:53:16.489438 capycli-2.3.0/capycli/dependencies/maven_pom.py
+-rw-r--r--   0        0        0     7085 2024-01-28 14:53:16.503455 capycli-2.3.0/capycli/dependencies/nuget.py
+-rw-r--r--   0        0        0    19145 2024-01-28 14:53:16.509561 capycli-2.3.0/capycli/dependencies/python.py
+-rw-r--r--   0        0        0      363 2023-05-17 09:09:21.133323 capycli-2.3.0/capycli/main/__init__.py
+-rw-r--r--   0        0        0     5904 2024-01-28 14:53:16.529337 capycli-2.3.0/capycli/main/application.py
+-rw-r--r--   0        0        0     4061 2024-01-28 14:53:16.529337 capycli-2.3.0/capycli/main/argument_parser.py
+-rw-r--r--   0        0        0      881 2024-01-28 14:53:16.539568 capycli-2.3.0/capycli/main/cli.py
+-rw-r--r--   0        0        0      441 2023-05-17 09:09:21.135549 capycli-2.3.0/capycli/main/exceptions.py
+-rw-r--r--   0        0        0    15371 2024-04-05 15:03:15.504828 capycli-2.3.0/capycli/main/options.py
+-rw-r--r--   0        0        0     1653 2024-04-05 15:03:15.504828 capycli-2.3.0/capycli/main/result_codes.py
+-rw-r--r--   0        0        0     1572 2024-01-28 14:53:16.553253 capycli-2.3.0/capycli/mapping/handle_mapping.py
+-rw-r--r--   0        0        0     7200 2024-01-28 14:53:16.553253 capycli-2.3.0/capycli/mapping/mapping_to_html.py
+-rw-r--r--   0        0        0     8347 2024-01-28 14:53:16.564831 capycli-2.3.0/capycli/mapping/mapping_to_xlsx.py
+-rw-r--r--   0        0        0     1643 2024-01-28 14:53:16.570018 capycli-2.3.0/capycli/moverview/handle_moverview.py
+-rw-r--r--   0        0        0     4840 2024-01-28 14:53:16.570018 capycli-2.3.0/capycli/moverview/moverview_to_html.py
+-rw-r--r--   0        0        0     7224 2024-01-28 14:53:16.579565 capycli-2.3.0/capycli/moverview/moverview_to_xlsx.py
+-rw-r--r--   0        0        0      330 2023-05-17 09:09:21.138795 capycli-2.3.0/capycli/project/__init__.py
+-rw-r--r--   0        0        0    13931 2024-04-05 15:03:15.504828 capycli-2.3.0/capycli/project/check_prerequisites.py
+-rw-r--r--   0        0        0     9756 2024-01-28 15:06:45.340845 capycli-2.3.0/capycli/project/create_bom.py
+-rw-r--r--   0        0        0    16458 2024-04-05 15:03:15.504828 capycli-2.3.0/capycli/project/create_project.py
+-rw-r--r--   0        0        0    23442 2024-04-05 14:37:40.708729 capycli-2.3.0/capycli/project/create_readme.py
+-rw-r--r--   0        0        0     5605 2024-01-28 14:53:16.609443 capycli-2.3.0/capycli/project/find_project.py
+-rw-r--r--   0        0        0    10955 2024-04-05 15:03:15.504828 capycli-2.3.0/capycli/project/get_license_info.py
+-rw-r--r--   0        0        0     4454 2024-01-28 14:53:16.629590 capycli-2.3.0/capycli/project/handle_project.py
+-rw-r--r--   0        0        0     9000 2024-01-28 15:02:03.962221 capycli-2.3.0/capycli/project/show_ecc.py
+-rw-r--r--   0        0        0     8329 2024-01-28 14:53:16.639627 capycli-2.3.0/capycli/project/show_licenses.py
+-rw-r--r--   0        0        0    10069 2024-01-28 14:53:16.639627 capycli-2.3.0/capycli/project/show_project.py
+-rw-r--r--   0        0        0     9709 2024-01-28 15:07:26.594053 capycli-2.3.0/capycli/project/show_vulnerabilities.py
+-rw-r--r--   0        0        0     1218 2024-01-28 14:56:39.309682 capycli-2.3.0/License.md
+drwxr-xr-x   0        0        0        0 2023-05-17 09:11:25.459479 capycli-2.3.0/LICENSES/
+-rw-r--r--   0        0        0     3107 2024-04-05 15:03:15.504828 capycli-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0    13026 2024-04-05 15:03:15.504828 capycli-2.3.0/Readme.md
+-rw-r--r--   0        0        0    14532 1970-01-01 00:00:00.000000 capycli-2.3.0/PKG-INFO
```

### Comparing `capycli-2.2.1/capycli/__init__.py` & `capycli-2.3.0/capycli/__init__.py`

 * *Files identical despite different names*

### Comparing `capycli-2.2.1/capycli/bom/bom_convert.py` & `capycli-2.3.0/capycli/bom/bom_convert.py`

 * *Files identical despite different names*

### Comparing `capycli-2.2.1/capycli/bom/check_bom.py` & `capycli-2.3.0/capycli/bom/check_bom.py`

 * *Files identical despite different names*

### Comparing `capycli-2.2.1/capycli/bom/check_bom_item_status.py` & `capycli-2.3.0/capycli/bom/check_bom_item_status.py`

 * *Files identical despite different names*

### Comparing `capycli-2.2.1/capycli/bom/check_granularity.py` & `capycli-2.3.0/capycli/bom/check_granularity.py`

 * *Files identical despite different names*

### Comparing `capycli-2.2.1/capycli/bom/create_components.py` & `capycli-2.3.0/capycli/bom/create_components.py`

 * *Files identical despite different names*

### Comparing `capycli-2.2.1/capycli/bom/csv.py` & `capycli-2.3.0/capycli/bom/csv.py`

 * *Files identical despite different names*

### Comparing `capycli-2.2.1/capycli/bom/diff_bom.py` & `capycli-2.3.0/capycli/bom/diff_bom.py`

 * *Files identical despite different names*

### Comparing `capycli-2.2.1/capycli/bom/download_sources.py` & `capycli-2.3.0/capycli/bom/download_sources.py`

 * *Files identical despite different names*

### Comparing `capycli-2.2.1/capycli/bom/filter_bom.py` & `capycli-2.3.0/capycli/bom/filter_bom.py`

 * *Files identical despite different names*

### Comparing `capycli-2.2.1/capycli/bom/findsources.py` & `capycli-2.3.0/capycli/bom/findsources.py`

 * *Files identical despite different names*

### Comparing `capycli-2.2.1/capycli/bom/handle_bom.py` & `capycli-2.3.0/capycli/bom/handle_bom.py`

 * *Files identical despite different names*

### Comparing `capycli-2.2.1/capycli/bom/html.py` & `capycli-2.3.0/capycli/bom/html.py`

 * *Files identical despite different names*

### Comparing `capycli-2.2.1/capycli/bom/legacy.py` & `capycli-2.3.0/capycli/bom/legacy.py`

 * *Files identical despite different names*

### Comparing `capycli-2.2.1/capycli/bom/legacy_cx.py` & `capycli-2.3.0/capycli/bom/legacy_cx.py`

 * *Files identical despite different names*

### Comparing `capycli-2.2.1/capycli/bom/map_bom.py` & `capycli-2.3.0/capycli/bom/map_bom.py`

 * *Files identical despite different names*

### Comparing `capycli-2.2.1/capycli/bom/merge_bom.py` & `capycli-2.3.0/capycli/bom/merge_bom.py`

 * *Files identical despite different names*

### Comparing `capycli-2.2.1/capycli/bom/plaintext.py` & `capycli-2.3.0/capycli/bom/plaintext.py`

 * *Files identical despite different names*

### Comparing `capycli-2.2.1/capycli/bom/show_bom.py` & `capycli-2.3.0/capycli/bom/show_bom.py`

 * *Files identical despite different names*

### Comparing `capycli-2.2.1/capycli/common/capycli_bom_support.py` & `capycli-2.3.0/capycli/common/capycli_bom_support.py`

 * *Files identical despite different names*

### Comparing `capycli-2.2.1/capycli/common/comparable_version.py` & `capycli-2.3.0/capycli/common/comparable_version.py`

 * *Files identical despite different names*

### Comparing `capycli-2.2.1/capycli/common/component_cache.py` & `capycli-2.3.0/capycli/common/component_cache.py`

 * *Files identical despite different names*

### Comparing `capycli-2.2.1/capycli/common/dependencies_base.py` & `capycli-2.3.0/capycli/common/dependencies_base.py`

 * *Files identical despite different names*

### Comparing `capycli-2.2.1/capycli/common/file_support.py` & `capycli-2.3.0/capycli/common/file_support.py`

 * *Files identical despite different names*

### Comparing `capycli-2.2.1/capycli/common/html_support.py` & `capycli-2.3.0/capycli/common/html_support.py`

 * *Files identical despite different names*

### Comparing `capycli-2.2.1/capycli/common/json_support.py` & `capycli-2.3.0/capycli/common/json_support.py`

 * *Files identical despite different names*

### Comparing `capycli-2.2.1/capycli/common/map_result.py` & `capycli-2.3.0/capycli/common/map_result.py`

 * *Files identical despite different names*

### Comparing `capycli-2.2.1/capycli/common/print.py` & `capycli-2.3.0/capycli/common/print.py`

 * *Files identical despite different names*

### Comparing `capycli-2.2.1/capycli/common/purl_service.py` & `capycli-2.3.0/capycli/common/purl_service.py`

 * *Files identical despite different names*

### Comparing `capycli-2.2.1/capycli/common/purl_store.py` & `capycli-2.3.0/capycli/common/purl_store.py`

 * *Files identical despite different names*

### Comparing `capycli-2.2.1/capycli/common/purl_utils.py` & `capycli-2.3.0/capycli/common/purl_utils.py`

 * *Files identical despite different names*

### Comparing `capycli-2.2.1/capycli/common/script_base.py` & `capycli-2.3.0/capycli/common/script_base.py`

 * *Files identical despite different names*

### Comparing `capycli-2.2.1/capycli/common/script_support.py` & `capycli-2.3.0/capycli/common/script_support.py`

 * *Files identical despite different names*

### Comparing `capycli-2.2.1/capycli/data/granularity_list.csv` & `capycli-2.3.0/capycli/data/granularity_list.csv`

 * *Files 7% similar despite different names*

```diff
@@ -1596,35 +1596,42 @@
 apache-mime4j-dom;Apache-mime4j;;https://github.com/apache/james-mime4j
 apache-mime4j-storage;Apache-mime4j;;https://github.com/apache/james-mime4j
 
 docker-java-api;Docker Java;;https://github.com/docker-java/docker-java
 docker-java-transport;Docker Java;;https://github.com/docker-java/docker-java
 docker-java-transport-httpclient5;Docker Java;;https://github.com/docker-java/docker-java
 docker-java-transport-zerodep;Docker Java;;https://github.com/docker-java/docker-java
-
- infinispan-cachestore-remote;Infinispan;;https://github.com/infinispan/infinispan
- infinispan-client-hotrod;Infinispan;;https://github.com/infinispan/infinispan
- infinispan-clustered-counter;Infinispan;;https://github.com/infinispan/infinispan
- infinispan-commons;Infinispan;;https://github.com/infinispan/infinispan
- infinispan-core;Infinispan;;https://github.com/infinispan/infinispan
- infinispan-jb-marshalling;Infinispan;;https://github.com/infinispan/infinispan
- infinispan-multimap;Infinispan;;https://github.com/infinispan/infinispan
- infinispan-server-core;Infinispan;;https://github.com/infinispan/infinispan
- infinispan-server-hotrod;Infinispan;;https://github.com/infinispan/infinispan
- infinispan-tasks;Infinispan;;https://github.com/infinispan/infinispan
- infinispan-tasks-api;Infinispan;;https://github.com/infinispan/infinispan
-
- jansi-freebsd32;Jansi;;https://github.com/fusesource/jansi	
- jansi-freebsd64;Jansi;;https://github.com/fusesource/jansi	
- jansi-linux32;Jansi;;https://github.com/fusesource/jansi	
- jansi-linux64;Jansi;;https://github.com/fusesource/jansi	
- jansi-native;Jansi;;https://github.com/fusesource/jansi
- jansi-osx;Jansi;;https://github.com/fusesource/jansi
- jansi-windows32;Jansi;;https://github.com/fusesource/jansi
- jansi-windows64;Jansi;;https://github.com/fusesource/jansi
+docker-java-bom;Docker Java;;https://github.com/docker-java/docker-java
+docker-java-core;Docker Java;;https://github.com/docker-java/docker-java
+docker-java-transport-jersey;Docker Java;;https://github.com/docker-java/docker-java
+docker-java-transport-netty;Docker Java;;https://github.com/docker-java/docker-java
+docker-java-transport-okhttp;Docker Java;;https://github.com/docker-java/docker-java
+docker-java-transport-tck;Docker Java;;https://github.com/docker-java/docker-java
+docker-java;Docker Java;;https://github.com/docker-java/docker-java
+
+infinispan-cachestore-remote;Infinispan;;https://github.com/infinispan/infinispan
+infinispan-client-hotrod;Infinispan;;https://github.com/infinispan/infinispan
+infinispan-clustered-counter;Infinispan;;https://github.com/infinispan/infinispan
+infinispan-commons;Infinispan;;https://github.com/infinispan/infinispan
+infinispan-core;Infinispan;;https://github.com/infinispan/infinispan
+infinispan-jb-marshalling;Infinispan;;https://github.com/infinispan/infinispan
+infinispan-multimap;Infinispan;;https://github.com/infinispan/infinispan
+infinispan-server-core;Infinispan;;https://github.com/infinispan/infinispan
+infinispan-server-hotrod;Infinispan;;https://github.com/infinispan/infinispan
+infinispan-tasks;Infinispan;;https://github.com/infinispan/infinispan
+infinispan-tasks-api;Infinispan;;https://github.com/infinispan/infinispan
+
+jansi-freebsd32;Jansi;;https://github.com/fusesource/jansi	
+jansi-freebsd64;Jansi;;https://github.com/fusesource/jansi	
+jansi-linux32;Jansi;;https://github.com/fusesource/jansi	
+jansi-linux64;Jansi;;https://github.com/fusesource/jansi	
+jansi-native;Jansi;;https://github.com/fusesource/jansi
+jansi-osx;Jansi;;https://github.com/fusesource/jansi
+jansi-windows32;Jansi;;https://github.com/fusesource/jansi
+jansi-windows64;Jansi;;https://github.com/fusesource/jansi
 
 resteasy-client;Resteasy;;https://github.com/resteasy/resteasy
 resteasy-client-api;Resteasy;;https://github.com/resteasy/resteasy
 resteasy-core;Resteasy;;https://github.com/resteasy/resteasy
 resteasy-core-spi;Resteasy;;https://github.com/resteasy/resteasy
 resteasy-jackson2-provider;Resteasy;;https://github.com/resteasy/resteasy
 resteasy-jaxb-provider;Resteasy;;https://github.com/resteasy/resteasy
@@ -1751,15 +1758,15 @@
 sundr-codegen-api;Sundrio;;https://github.com/sundrio/sundrio
 sundr-codegen-apt;Sundrio;;https://github.com/sundrio/sundrio
 sundr-core;Sundrio;;https://github.com/sundrio/sundrio
 sundr-model;Sundrio;;https://github.com/sundrio/sundrio
 sundr-model-base;Sundrio;;https://github.com/sundrio/sundrio
 sundr-model-repo;Sundrio;;https://github.com/sundrio/sundrio
 sundr-model-utils;Sundrio;;https://github.com/sundrio/sundrio
-;;;
+
 babel-jest;Jest;;https://github.com/facebook/jest
 babel-plugin-jest-hoist;Jest;;https://github.com/facebook/jest
 babel-preset-jest;Jest;;https://github.com/facebook/jest
 diff-sequences;Jest;;https://github.com/facebook/jest
 expect;Jest;;https://github.com/facebook/jest
 jest;Jest;;https://github.com/facebook/jest
 jest-changed-files;Jest;;https://github.com/facebook/jest
@@ -1852,14 +1859,17 @@
 keycloak-model-legacy-services;Keycloak;;https://github.com/keycloak/keycloak
 keycloak-crypto-default;Keycloak;;https://github.com/keycloak/keycloak
 keycloak-model-map-jpa;Keycloak;;https://github.com/keycloak/keycloak
 keycloak-model-map-hot-rod;Keycloak;;https://github.com/keycloak/keycloak
 keycloak-model-legacy-private;Keycloak;;https://github.com/keycloak/keycloak
 keycloak-config-api;Keycloak;;https://github.com/keycloak/keycloak
 keycloak-model-legacy;Keycloak;;https://github.com/keycloak/keycloak
+Keycloak;KEYCLOAK;;https://github.com/keycloak/keycloak
+keycloak-admin-client;KEYCLOAK;;https://github.com/keycloak/keycloak
+keycloak-core;KEYCLOAK;;https://github.com/keycloak/keycloak
 
 jboss-marshalling-river;Jboss-marshalling;;https://github.com/jboss-remoting/jboss-marshalling
 jboss-marshalling-osgi;Jboss-marshalling;;https://github.com/jboss-remoting/jboss-marshalling
 jboss-marshalling-serial;Jboss-marshalling;;https://github.com/jboss-remoting/jboss-marshalling
 
 txoj;Narayana;;https://github.com/jbosstm/narayana
 arjuna;Narayana;;https://github.com/jbosstm/narayana
@@ -1867,19 +1877,19 @@
 narayana-jta;Narayana;;https://github.com/jbosstm/narayana
 COMMON;Narayana;;https://github.com/jbosstm/narayana
 jta;Narayana;;https://github.com/jbosstm/narayana
 cdi;Narayana;;https://github.com/jbosstm/narayana
 narayana-jts-integration;Narayana;;https://github.com/jbosstm/narayana
 jms;Narayana;;https://github.com/jbosstm/narayana
 
- quarkus-logging-gelf-deployment ;Quarkus;;https://github.com/quarkusio/quarkus
- quarkus-security;Quarkus;;https://github.com/quarkusio/quarkus
- quarkus-vault;Quarkus;;https://github.com/quarkusio/quarkus
- quarkus-vault-deployment;Quarkus;;https://github.com/quarkusio/quarkus
- quarkus-vault-model;Quarkus;;https://github.com/quarkusio/quarkus
+quarkus-logging-gelf-deployment;Quarkus;;https://github.com/quarkusio/quarkus
+quarkus-security;Quarkus;;https://github.com/quarkusio/quarkus
+quarkus-vault;Quarkus;;https://github.com/quarkusio/quarkus
+quarkus-vault-deployment;Quarkus;;https://github.com/quarkusio/quarkus
+quarkus-vault-model;Quarkus;;https://github.com/quarkusio/quarkus
 quarkus-agroal;Quarkus;;https://github.com/quarkusio/quarkus
 quarkus-agroal-deployment;Quarkus;;https://github.com/quarkusio/quarkus
 quarkus-agroal-spi;Quarkus;;https://github.com/quarkusio/quarkus
 quarkus-amazon-dynamodb;Quarkus;;https://github.com/quarkusio/quarkus
 quarkus-apache-httpclient;Quarkus;;https://github.com/quarkusio/quarkus
 quarkus-arc;Quarkus;;https://github.com/quarkusio/quarkus
 quarkus-arc-deployment;Quarkus;;https://github.com/quarkusio/quarkus
@@ -2289,19 +2299,24 @@
 opentelemetry-api-logs;opentelemetry-java;;https://github.com/open-telemetry/opentelemetry-java
 opentelemetry-context;opentelemetry-java;;https://github.com/open-telemetry/opentelemetry-java
 opentelemetry-extension-aws;opentelemetry-java;;https://github.com/open-telemetry/opentelemetry-java
 opentelemetry-extension-trace-propagators;opentelemetry-java;;https://github.com/open-telemetry/opentelemetry-java
 opentelemetry-sdk;opentelemetry-java;;https://github.com/open-telemetry/opentelemetry-java
 opentelemetry-sdk-common;opentelemetry-java;;https://github.com/open-telemetry/opentelemetry-java
 opentelemetry-sdk-extension-autoconfigure-spi;opentelemetry-java;;https://github.com/open-telemetry/opentelemetry-java
+opentelemetry-sdk-extension-autoconfigure;opentelemetry-java;;https://github.com/open-telemetry/opentelemetry-java
 opentelemetry-sdk-logs;opentelemetry-java;;https://github.com/open-telemetry/opentelemetry-java
 opentelemetry-sdk-metrics;opentelemetry-java;;https://github.com/open-telemetry/opentelemetry-java
 opentelemetry-sdk-trace;opentelemetry-java;;https://github.com/open-telemetry/opentelemetry-java
 opentelemetry-semconv;opentelemetry-java;;https://github.com/open-telemetry/opentelemetry-java
-
+opentelemetry-api-events;opentelemetry-java;;https://github.com/open-telemetry/opentelemetry-java
+opentelemetry-exporter-logging;opentelemetry-java;;https://github.com/open-telemetry/opentelemetry-java
+opentelemetry-extension-incubator;opentelemetry-java;;https://github.com/open-telemetry/opentelemetry-java
+opentelemetry-java;opentelemetry-java;;https://github.com/open-telemetry/opentelemetry-java
+opentelemetry-java-instrumentation;opentelemetry-java-instrumentation;;https://github.com/open-telemetry/opentelemetry-java-instrumentation
 opentelemetry-instrumentation-api;opentelemetry-java-instrumentation;;https://github.com/open-telemetry/opentelemetry-java-instrumentation
 opentelemetry-instrumentation-api-semconv;opentelemetry-java-instrumentation;;https://github.com/open-telemetry/opentelemetry-java-instrumentation
 opentelemetry-logback-mdc-1.0;opentelemetry-java-instrumentation;;https://github.com/open-telemetry/opentelemetry-java-instrumentation
 
 @material/animation;material-components-web;;https://github.com/material-components/material-components-web
 @material/auto-init;material-components-web;;https://github.com/material-components/material-components-web
 @material/banner;material-components-web;;https://github.com/material-components/material-components-web
@@ -2350,19 +2365,14 @@
 @material/tokens;material-components-web;;https://github.com/material-components/material-components-web
 @material/tooltip;material-components-web;;https://github.com/material-components/material-components-web
 @material/top-app-bar;material-components-web;;https://github.com/material-components/material-components-web
 @material/touch-target;material-components-web;;https://github.com/material-components/material-components-web
 @material/typography;material-components-web;;https://github.com/material-components/material-components-web
 
 
-aws-java-sdk-core;aws-java-sdk;;https://github.com/aws/aws-sdk-java
-aws-java-sdk-s3;aws-java-sdk;;https://github.com/aws/aws-sdk-java
-aws-java-sdk-sts;aws-java-sdk;;https://github.com/aws/aws-sdk-java
-jmespath-java;aws-java-sdk;;https://github.com/aws/aws-sdk-java
-
 google-http-client-appengine;google-http-client;;https://github.com/googleapis/google-http-java-client
 google-http-client-gson;google-http-client;;https://github.com/googleapis/google-http-java-client
 google-http-client-jackson2;google-http-client;;https://github.com/googleapis/google-http-java-client
 
 tika-core;Tika;;https://github.com/apache/tika
 tika-langdetect-tika;Tika;;https://github.com/apache/tika
 tika-parser-apple-module;Tika;;https://github.com/apache/tika
@@ -2684,14 +2694,490 @@
 @turf/transform-translate;Turf;;https://github.com/Turfjs/turf
 @turf/triangle-grid;Turf;;https://github.com/Turfjs/turf
 @turf/truncate;Turf;;https://github.com/Turfjs/turf
 @turf/union;Turf;;https://github.com/Turfjs/turf
 @turf/unkink-polygon;Turf;;https://github.com/Turfjs/turf
 @turf/voronoi;Turf;;https://github.com/Turfjs/turf
 
+selenium-api;Selenium;;https://github.com/SeleniumHQ/selenium
+selenium-chrome-driver;Selenium;;https://github.com/SeleniumHQ/selenium
+selenium-chromium-driver;Selenium;;https://github.com/SeleniumHQ/selenium
+selenium-devtools-v116;Selenium;;https://github.com/SeleniumHQ/selenium
+selenium-devtools-v117;Selenium;;https://github.com/SeleniumHQ/selenium
+selenium-devtools-v118;Selenium;;https://github.com/SeleniumHQ/selenium
+selenium-devtools-v85;Selenium;;https://github.com/SeleniumHQ/selenium
+selenium-edge-driver;Selenium;;https://github.com/SeleniumHQ/selenium
+selenium-firefox-driver;Selenium;;https://github.com/SeleniumHQ/selenium
+selenium-http;Selenium;;https://github.com/SeleniumHQ/selenium
+selenium-ie-driver;Selenium;;https://github.com/SeleniumHQ/selenium
+selenium-java;Selenium;;https://github.com/SeleniumHQ/selenium
+selenium-json;Selenium;;https://github.com/SeleniumHQ/selenium
+selenium-manager;Selenium;;https://github.com/SeleniumHQ/selenium
+selenium-os;Selenium;;https://github.com/SeleniumHQ/selenium
+selenium-remote-driver;Selenium;;https://github.com/SeleniumHQ/selenium
+selenium-safari-driver;Selenium;;https://github.com/SeleniumHQ/selenium
+selenium-support;Selenium;;https://github.com/SeleniumHQ/selenium
+
+camunda-bpm-platform;Camunda Platform;;https://github.com/camunda/camunda-bpm-platform
+camunda-bpm-spring-boot-starter-external-task-client;Camunda Platform;;https://github.com/camunda/camunda-bpm-platform
+camunda-engine-rest-client-openapi-java;Camunda Platform;;https://github.com/camunda/camunda-bpm-platform
+camunda-engine-rest-client-openapi-springboot;Camunda Platform;;https://github.com/camunda/camunda-bpm-platform
+camunda-external-task-client;Camunda Platform;;https://github.com/camunda/camunda-bpm-platform
+camunda-external-task-client-spring;Camunda Platform;;https://github.com/camunda/camunda-bpm-platform
+
+org.jacoco.agent;JaCoCo;;https://github.com/jacoco/jacoco
+org.jacoco.core;JaCoCo;;https://github.com/jacoco/jacoco
+org.jacoco.report;JaCoCo;;https://github.com/jacoco/jacoco
+org.jacoco.tests;JaCoCo;;https://github.com/jacoco/jacoco
+org.jacoco.test;JaCoCo;;https://github.com/jacoco/jacoco
+org.jacoco.cli;JaCoCo;;https://github.com/jacoco/jacoco
+org.jacoco.build;JaCoCo;;https://github.com/jacoco/jacoco
+org.jacoco.ant;JaCoCo;;https://github.com/jacoco/jacoco
+
+micrometer;Micrometer Application Metrics;;https://github.com/micrometer-metrics/micrometer
+micrometer-commons;Micrometer Application Metrics;;https://github.com/micrometer-metrics/micrometer
+micrometer-core;Micrometer Application Metrics;;https://github.com/micrometer-metrics/micrometer
+micrometer-jakarta9;Micrometer Application Metrics;;https://github.com/micrometer-metrics/micrometer
+micrometer-observation;Micrometer Application Metrics;;https://github.com/micrometer-metrics/micrometer
+micrometer-registry-prometheus;Micrometer Application Metrics;;https://github.com/micrometer-metrics/micrometer
+micrometer-tracing;Micrometer Tracing Facade;;https://github.com/micrometer-metrics/tracing
+micrometer-tracing-bridge-otel;Micrometer Tracing Facade;;https://github.com/micrometer-metrics/tracing
+
+kotlin-stdlib;Kotlin;;https://github.com/JetBrains/kotlin
+kotlin-stdlib-common;Kotlin;;https://github.com/JetBrains/kotlin
+kotlin-stdlib-jdk7;Kotlin;;https://github.com/JetBrains/kotlin
+kotlin-stdlib-jdk8;Kotlin;;https://github.com/JetBrains/kotlin
+
+ASM;ASM;;https://gitlab.ow2.org/asm/asm
+asm-commons;ASM;;https://gitlab.ow2.org/asm/asm
+asm-tree;ASM;;https://gitlab.ow2.org/asm/asm
+
+aws-java-sdk-kms;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-accessanalyzer;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-account;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-acm;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-acmpca;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-alexaforbusiness;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-amplify;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-amplifybackend;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-amplifyuibuilder;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-api-gateway;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-apigatewaymanagementapi;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-apigatewayv2;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-appconfig;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-appconfigdata;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-appfabric;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-appflow;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-appintegrations;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-applicationautoscaling;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-applicationcostprofiler;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-applicationinsights;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-appmesh;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-appregistry;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-apprunner;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-appstream;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-appsync;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-arczonalshift;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-artifact;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-athena;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-auditmanager;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-augmentedairuntime;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-autoscaling;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-autoscalingplans;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-b2bi;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-backup;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-backupgateway;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-backupstorage;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-batch;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-bcmdataexports;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-bedrock;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-bedrockagent;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-bedrockagentruntime;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-bedrockruntime;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-billingconductor;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-bom;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-braket;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-budgets;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-bundle;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-chatbot;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-chime;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-chimesdkidentity;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-chimesdkmediapipelines;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-chimesdkmeetings;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-chimesdkmessaging;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-chimesdkvoice;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-cleanrooms;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-cleanroomsml;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-cloud9;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-cloudcontrolapi;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-clouddirectory;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-cloudformation;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-cloudfront;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-cloudhsm;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-cloudhsmv2;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-cloudsearch;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-cloudtrail;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-cloudtraildata;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-cloudwatch;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-cloudwatchevidently;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-cloudwatchmetrics;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-cloudwatchrum;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-code-generator;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-codeartifact;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-codebuild;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-codecommit;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-codeconnections;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-codedeploy;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-codegen-maven-plugin;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-codeguruprofiler;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-codegurureviewer;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-codegurusecurity;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-codepipeline;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-codestar;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-codestarconnections;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-codestarnotifications;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-cognitoidentity;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-cognitoidp;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-cognitosync;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-comprehend;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-comprehendmedical;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-computeoptimizer;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-config;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-connect;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-connectcampaign;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-connectcases;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-connectcontactlens;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-connectparticipant;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-connectwisdom;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-controltower;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-core;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-costandusagereport;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-costexplorer;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-costoptimizationhub;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-customerprofiles;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-dataexchange;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-datapipeline;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-datasync;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-datazoneexternal;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-dax;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-detective;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-devicefarm;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-devopsguru;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-directconnect;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-directory;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-discovery;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-dlm;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-dms;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-docdb;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-docdbelastic;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-drs;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-dynamodb;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-ebs;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-ec2;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-ec2instanceconnect;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-ecr;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-ecrpublic;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-ecs;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-efs;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-eks;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-eksauth;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-elasticache;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-elasticbeanstalk;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-elasticinference;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-elasticloadbalancing;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-elasticloadbalancingv2;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-elasticsearch;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-elastictranscoder;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-emr;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-emrcontainers;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-emrserverless;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-entityresolution;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-eventbridge;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-events;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-finspace;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-finspacedata;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-fis;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-fms;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-forecast;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-forecastquery;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-frauddetector;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-freetier;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-fsx;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-gamelift;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-glacier;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-globalaccelerator;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-glue;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-gluedatabrew;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-greengrass;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-greengrassv2;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-groundstation;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-guardduty;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-health;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-healthlake;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-honeycode;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-iam;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-iamrolesanywhere;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-identitystore;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-imagebuilder;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-importexport;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-inspector;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-inspector2;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-inspectorscan;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-internetmonitor;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-iot;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-iot1clickdevices;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-iot1clickprojects;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-iotanalytics;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-iotdeviceadvisor;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-iotevents;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-ioteventsdata;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-iotfleethub;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-iotfleetwise;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-iotjobsdataplane;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-iotsecuretunneling;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-iotsitewise;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-iotthingsgraph;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-iottwinmaker;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-iotwireless;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-ivs;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-ivschat;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-ivsrealtime;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-kafka;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-kafkaconnect;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-kendra;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-kendraranking;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-keyspaces;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-kinesis;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-kinesisanalyticsv2;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-kinesisvideo;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-kinesisvideosignalingchannels;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-kinesisvideowebrtcstorage;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-kms;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-lakeformation;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-lambda;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-launchwizard;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-lex;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-lexmodelbuilding;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-lexmodelsv2;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-lexruntimev2;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-licensemanager;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-licensemanagerlinuxsubscriptions;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-licensemanagerusersubscriptions;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-lightsail;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-location;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-logs;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-lookoutequipment;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-lookoutforvision;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-lookoutmetrics;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-machinelearning;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-macie2;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-mainframemodernization;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-managedblockchain;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-managedblockchainquery;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-managedgrafana;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-marketplaceagreement;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-marketplacecatalog;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-marketplacecommerceanalytics;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-marketplacedeployment;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-marketplaceentitlement;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-marketplacemeteringservice;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-mechanicalturkrequester;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-mediaconnect;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-mediaconvert;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-medialive;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-mediapackage;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-mediapackagev2;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-mediapackagevod;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-mediastore;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-mediastoredata;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-mediatailor;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-medicalimaging;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-memorydb;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-mgn;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-migrationhub;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-migrationhubconfig;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-migrationhuborchestrator;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-migrationhubrefactorspaces;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-migrationhubstrategyrecommendations;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-mobile;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-models;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-mq;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-mwaa;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-neptune;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-neptunedata;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-networkfirewall;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-networkmanager;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-networkmonitor;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-nimblestudio;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-oam;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-omics;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-opensdk;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-opensearch;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-opensearchserverless;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-opsworks;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-opsworkscm;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-organizations;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-osgi;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-osis;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-outposts;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-panorama;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-paymentcryptography;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-paymentcryptographydata;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-pcaconnectorad;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-personalize;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-personalizeevents;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-personalizeruntime;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-pi;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-pinpoint;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-pinpointemail;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-pinpointsmsvoice;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-pinpointsmsvoicev2;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-pipes;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-polly;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-pricing;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-private5g;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-prometheus;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-proton;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-qbusiness;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-qconnect;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-qldb;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-qldbsession;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-quicksight;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-ram;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-rds;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-rdsdata;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-recyclebin;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-redshift;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-redshiftdataapi;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-redshiftserverless;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-rekognition;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-repostspace;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-resiliencehub;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-resourceexplorer2;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-resourcegroups;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-resourcegroupstaggingapi;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-robomaker;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-route53;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-route53recoverycluster;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-route53recoverycontrolconfig;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-route53recoveryreadiness;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-route53resolver;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-s3;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-s3control;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-s3outposts;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-sagemaker;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-sagemakeredgemanager;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-sagemakerfeaturestoreruntime;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-sagemakergeospatial;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-sagemakermetrics;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-sagemakerruntime;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-savingsplans;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-scheduler;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-schemas;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-secretsmanager;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-securityhub;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-securitylake;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-serverlessapplicationrepository;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-servermigration;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-servicecatalog;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-servicediscovery;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-servicequotas;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-ses;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-sesv2;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-shield;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-signer;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-simpledb;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-simpleworkflow;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-simspaceweaver;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-snowball;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-snowdevicemanagement;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-sns;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-sqs;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-ssm;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-ssmcontacts;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-ssmincidents;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-ssmsap;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-sso;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-ssoadmin;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-ssooidc;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-stepfunctions;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-storagegateway;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-sts;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-supplychain;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-support;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-supportapp;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-synthetics;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-test-utils;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-textract;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-timestreaminfluxdb;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-timestreamquery;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-timestreamwrite;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-tnb;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-transcribe;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-transfer;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-translate;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-trustedadvisor;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-verifiedpermissions;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-voiceid;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-vpclattice;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-waf;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-wafv2;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-wellarchitected;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-workdocs;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-worklink;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-workmail;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-workmailmessageflow;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-workspaces;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-workspacesthinclient;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-workspacesweb;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk-xray;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+aws-java-sdk;;;https://github.com/aws/aws-sdk-java
+jmespath-java;AWS SDK for Java;;https://github.com/aws/aws-sdk-java
+
+Byte Buddy;Byte Buddy;;https://github.com/raphw/byte-buddy
+byte-buddy-agent;Byte Buddy;;https://github.com/raphw/byte-buddy
+byte-buddy-benchmark;Byte Buddy;;https://github.com/raphw/byte-buddy
+byte-buddy-dep;Byte Buddy;;https://github.com/raphw/byte-buddy
+byte-buddy-gradle-plugin;Byte Buddy;;https://github.com/raphw/byte-buddy
+byte-buddy-maven-plugin;Byte Buddy;;https://github.com/raphw/byte-buddy
+byte-buddy;Byte Buddy;;https://github.com/raphw/byte-buddy
+
+httpcore5;Apache HttpComponents Core;;https://github.com/apache/httpcomponents-core
+httpcore5-h2;Apache HttpComponents Core;;https://github.com/apache/httpcomponents-core
+httpcore5-reactive;Apache HttpComponents Core;;https://github.com/apache/httpcomponents-core
+httpcore5-testing;Apache HttpComponents Core;;https://github.com/apache/httpcomponents-core
+
+Netty;Netty Project;;https://github.com/netty/netty
+netty-resolver-dns;Netty Project;;https://github.com/netty/netty
+netty-resolver-dns-classes-macos;Netty Project;;https://github.com/netty/netty
+netyy-resolver-dns-native-macos;Netty Project;;https://github.com/netty/netty
+netty-transport-blockhound-tests;Netty Project;;https://github.com/netty/netty
+netty-transport-classes-epoll;Netty Project;;https://github.com/netty/netty
+netty-transport-classes-kqueue;Netty Project;;https://github.com/netty/netty
+netty-transport-native-epoll;Netty Project;;https://github.com/netty/netty
+netty-transport-native-kqueue;Netty Project;;https://github.com/netty/netty
+netty-transport-native-unix-common-tests;Netty Project;;https://github.com/netty/netty
+netty-transport-native-unix-common;Netty Project;;https://github.com/netty/netty
+netty-transport-rxtx;Netty Project;;https://github.com/netty/netty
+netty-transport-sctp;Netty Project;;https://github.com/netty/netty
+netty-4transport-udt;Netty Project;;https://github.com/netty/netty
+netty-transport;Netty Project;;https://github.com/netty/netty
+netty-codec-dns;Netty Project;;https://github.com/netty/netty
+netty-codec-haproxy;Netty Project;;https://github.com/netty/netty
+netty-codec-http;Netty Project;;https://github.com/netty/netty
+netty-codec-http2;Netty Project;;https://github.com/netty/netty
+netty-codec-memcache;Netty Project;;https://github.com/netty/netty
+netty-codec-mqtt;Netty Project;;https://github.com/netty/netty
+netty-codec-redis;Netty Project;;https://github.com/netty/netty
+netty-codec-smtp;Netty Project;;https://github.com/netty/netty
+netty-codec-socks;Netty Project;;https://github.com/netty/netty
+netty-codec-stomp;Netty Project;;https://github.com/netty/netty
+netty-codec-xml;Netty Project;;https://github.com/netty/netty
+netty-codec;Netty Project;;https://github.com/netty/netty
+
 @nestjs/common;Nest;;https://github.com/nestjs/nest
 @nestjs/core;Nest;;https://github.com/nestjs/nest
 @nestjs/microservices;Nest;;https://github.com/nestjs/nest
 @nestjs/platform-express;Nest;;https://github.com/nestjs/nest
 @nestjs/platform-fastify;Nest;;https://github.com/nestjs/nest
 @nestjs/platform-socket.io;Nest;;https://github.com/nestjs/nest
 @nestjs/platform-ws;Nest;;https://github.com/nestjs/nest
```

### Comparing `capycli-2.2.1/capycli/dependencies/handle_dependencies.py` & `capycli-2.3.0/capycli/dependencies/handle_dependencies.py`

 * *Files identical despite different names*

### Comparing `capycli-2.2.1/capycli/dependencies/javascript.py` & `capycli-2.3.0/capycli/dependencies/javascript.py`

 * *Files identical despite different names*

### Comparing `capycli-2.2.1/capycli/dependencies/maven_list.py` & `capycli-2.3.0/capycli/dependencies/maven_list.py`

 * *Files identical despite different names*

### Comparing `capycli-2.2.1/capycli/dependencies/maven_pom.py` & `capycli-2.3.0/capycli/dependencies/maven_pom.py`

 * *Files identical despite different names*

### Comparing `capycli-2.2.1/capycli/dependencies/nuget.py` & `capycli-2.3.0/capycli/dependencies/nuget.py`

 * *Files identical despite different names*

### Comparing `capycli-2.2.1/capycli/dependencies/python.py` & `capycli-2.3.0/capycli/dependencies/python.py`

 * *Files identical despite different names*

### Comparing `capycli-2.2.1/capycli/main/application.py` & `capycli-2.3.0/capycli/main/application.py`

 * *Files identical despite different names*

### Comparing `capycli-2.2.1/capycli/main/argument_parser.py` & `capycli-2.3.0/capycli/main/argument_parser.py`

 * *Files identical despite different names*

### Comparing `capycli-2.2.1/capycli/main/cli.py` & `capycli-2.3.0/capycli/main/cli.py`

 * *Files identical despite different names*

### Comparing `capycli-2.2.1/capycli/main/options.py` & `capycli-2.3.0/capycli/main/options.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -------------------------------------------------------------------------------
-# Copyright (c) 2019-23 Siemens
+# Copyright (c) 2019-24 Siemens
 # All Rights Reserved.
 # Author: thomas.graf@siemens.com
 #
 # SPDX-License-Identifier: MIT
 # -------------------------------------------------------------------------------
 
 """Contains the logic for all of the default options for CaPyCli."""
@@ -388,14 +388,22 @@
         )
 
         self.parser.add_argument(
             "-X",
             dest="debug", action="store_true",
             help="Enable debug output")
 
+        # used by CheckPrerequisites
+        self.parser.add_argument(
+            "--forceerror",
+            dest="force_error",
+            action="store_true",
+            help="force an error exit code in case of visual errors",
+        )
+
     def read_config(self, filename: str = "", config_string: str = "") -> Dict[str, Any]:
         """
         Read configuration from string or config file.
         """
 
         toml_dict = None
         try:
```

### Comparing `capycli-2.2.1/capycli/main/result_codes.py` & `capycli-2.3.0/capycli/main/result_codes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -------------------------------------------------------------------------------
-# Copyright 2023 Siemens
+# Copyright 2023-2024 Siemens
 # All Rights Reserved.
 # Author: thomas.graf@siemens.com
 #
 # SPDX-License-Identifier: MIT
 # -------------------------------------------------------------------------------
 
 class ResultCode(object):
@@ -35,7 +35,9 @@
     RESULT_ERROR_CREATING_COMPONENT = 90
     RESULT_ERROR_CREATING_RELEASE = 91
     RESULT_ERROR_CREATING_ITEM = 92
     RESULT_NO_CACHED_RELEASES = 93
     RESULT_PROJECT_NOT_FOUND = 94
     RESULT_ERROR_ACCESSING_SW360 = 95
     RESULT_FILTER_ERROR = 96
+    RESULT_PREREQUISITE_ERROR = 97
+    RESULT_LICENSE_INFO_ERROR = 98
```

### Comparing `capycli-2.2.1/capycli/mapping/handle_mapping.py` & `capycli-2.3.0/capycli/mapping/handle_mapping.py`

 * *Files identical despite different names*

### Comparing `capycli-2.2.1/capycli/mapping/mapping_to_html.py` & `capycli-2.3.0/capycli/mapping/mapping_to_html.py`

 * *Files identical despite different names*

### Comparing `capycli-2.2.1/capycli/mapping/mapping_to_xlsx.py` & `capycli-2.3.0/capycli/mapping/mapping_to_xlsx.py`

 * *Files identical despite different names*

### Comparing `capycli-2.2.1/capycli/moverview/handle_moverview.py` & `capycli-2.3.0/capycli/moverview/handle_moverview.py`

 * *Files identical despite different names*

### Comparing `capycli-2.2.1/capycli/moverview/moverview_to_html.py` & `capycli-2.3.0/capycli/moverview/moverview_to_html.py`

 * *Files identical despite different names*

### Comparing `capycli-2.2.1/capycli/moverview/moverview_to_xlsx.py` & `capycli-2.3.0/capycli/moverview/moverview_to_xlsx.py`

 * *Files identical despite different names*

### Comparing `capycli-2.2.1/capycli/project/check_prerequisites.py` & `capycli-2.3.0/capycli/project/check_prerequisites.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ﻿# -------------------------------------------------------------------------------
-# Copyright (c) 2019-23 Siemens
+# Copyright (c) 2019-24 Siemens
 # All Rights Reserved.
 # Author: thomas.graf@siemens.com
 #
 # SPDX-License-Identifier: MIT
 # -------------------------------------------------------------------------------
 
 import logging
@@ -94,39 +94,42 @@
          search for them."""
         for cx_comp in sbom.components:
             if CycloneDxSupport.get_property_value(cx_comp, CycloneDxSupport.CDX_PROP_SW360ID):
                 return True
 
         return False
 
-    def check_project_prerequisites(self, id: str, sbom: Optional[Bom]) -> None:
+    def check_project_prerequisites(self, id: str, sbom: Optional[Bom]) -> bool:
         if not self.client:
             print_red("  No client!")
             sys.exit(ResultCode.RESULT_ERROR_ACCESSING_SW360)
 
         try:
             project = self.client.get_project(id)
         except Exception as ex:
             print_red("Error retrieving project details: \n" + repr(ex))
             sys.exit(ResultCode.RESULT_ERROR_ACCESSING_SW360)
 
         if not project:
             print_red("Error retrieving project details")
             sys.exit(ResultCode.RESULT_ERROR_ACCESSING_SW360)
 
+        has_errors = False
         print_text("  Project name: " + project["name"] + ", " + project["version"])
         print_text("  Clearing state: " + project.get("clearingState", "UNKNOWN"))
 
         if not project.get("projectOwner", None):
             print_yellow("  No project owner specified!")
+            has_errors = True
         else:
             print_green("  Project owner: " + project["projectOwner"])
 
         if not project.get("projectResponsible", None):
             print_yellow("  No project responsible specified!")
+            has_errors = True
         else:
             print_green(
                 "  Project responsible: "
                 + project["projectResponsible"])
 
         if len(project.get("securityResponsibles", [])) < 1:
             print_yellow("  No security responsibles specified!")
@@ -153,14 +156,15 @@
             print_text("\n  Components: ")
             releases = project["_embedded"]["sw360:releases"]
             for key in releases:
                 href = key["_links"]["self"]["href"]
                 release = self.client.get_release_by_url(href)
                 if not release:
                     print_red("Error accessign release " + href)
+                    has_errors = True
                     continue
 
                 state = self.get_clearing_state(project, href)
 
                 print_text("    " + key["name"] + ", " + key["version"] + ": " + state)
 
                 if not release.get("sourceCodeDownloadurl", ""):
@@ -181,14 +185,15 @@
                 if sbom and self.any_sw360id_in_bom(sbom):
                     release_id = self.client.get_id_from_href(href)
                     bom_item = [cx_comp for cx_comp in sbom.components
                                 if CycloneDxSupport.get_property_value(
                                     cx_comp, CycloneDxSupport.CDX_PROP_SW360ID) == release_id]
                     if len(bom_item) == 0:
                         print_red("      Item not in specified SBOM!")
+                        has_errors = True
                     else:
                         assert len(bom_item) == 1
                         bom_sha1 = CycloneDxSupport.get_source_file_hash(bom_item[0])
 
                 source = self.get_source_code(release)
                 for source_info in source:
                     source_name = source_info["filename"]
@@ -209,14 +214,15 @@
                                 "      SHA1 for source" +
                                 source_name +
                                 " matches!")
 
                 if len(source) != 1:
                     if state == "OPEN":
                         print(Fore.LIGHTRED_EX, end="")
+                        has_errors = True
                     else:
                         print(Fore.LIGHTYELLOW_EX, end="")
                 else:
                     print(Fore.LIGHTGREEN_EX, end="")
                 print("     ", len(source), "source file(s) available." + Fore.RESET)
 
                 ids = self.get_component_management_id(release)
@@ -246,14 +252,16 @@
                 print_text("      Check finished.")
             else:
                 print_yellow("      No SBOM specified, skipping release comparison!")
 
         else:
             print_text("    No linked releases")
 
+        return has_errors
+
     def run(self, args: Any) -> None:
         """Main method()"""
         if args.debug:
             global LOG
             LOG = capycli.get_logger(__name__)
         else:
             # suppress (debug) log output from requests and urllib
@@ -276,14 +284,15 @@
             print("    -n NAME, --name NAME    name of the project")
             print("    -v VERSION,             version of the project")
             print("    -id PROJECT_ID          SW360 id of the project, supersedes name and version parameters")
             print("    -i INPUTFILE            SBOM input file to read from (JSON)")
             print("    -t SW360_TOKEN,         use this token for access to SW360")
             print("    -oa, --oauth2           this is an oauth2 token")
             print("    -url SW360_URL          use this URL for access to SW360")
+            print("    --forceerror            force an error exit code in case of prerequisite errors")
             return
 
         if not self.login(token=args.sw360_token, url=args.sw360_url, oauth2=args.oauth2):
             print_red("ERROR: login failed!")
             sys.exit(ResultCode.RESULT_AUTH_ERROR)
 
         sbom = None
@@ -309,13 +318,14 @@
 
         if args.id:
             self.check_project_prerequisites(args.id, sbom)
         elif (args.name and args.version):
             # find_project() is part of script_base.py
             pid = self.find_project(name, version)
             if pid:
-                self.check_project_prerequisites(pid, sbom)
+                if (self.check_project_prerequisites(pid, sbom) and args.force_error):
+                    sys.exit(ResultCode.RESULT_PREREQUISITE_ERROR)
             else:
                 print_yellow("  No matching project found")
         else:
             print_red("Neither name and version nor project id specified!")
             sys.exit(ResultCode.RESULT_COMMAND_ERROR)
```

### Comparing `capycli-2.2.1/capycli/project/create_bom.py` & `capycli-2.3.0/capycli/project/create_bom.py`

 * *Files identical despite different names*

### Comparing `capycli-2.2.1/capycli/project/create_project.py` & `capycli-2.3.0/capycli/project/create_project.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
             if swex.response.status_code == requests.codes["unauthorized"]:
                 print_red("  You are not authorized!")
                 sys.exit(ResultCode.RESULT_AUTH_ERROR)
             if swex.response.status_code == requests.codes["forbidden"]:
                 print_red("  You are not authorized - do you have a valid write token?")
                 sys.exit(ResultCode.RESULT_AUTH_ERROR)
             if swex.response:
-                print_red("  " + swex.response.status_code + ": " + swex.response.text)
+                print_red("  " + str(swex.response.status_code) + ": " + swex.response.text)
                 sys.exit(ResultCode.RESULT_ERROR_ACCESSING_SW360)
             if swex.details:
                 print_red("  " + swex.details.get("error", "") + ": " + swex.details.get("message", ""))
                 sys.exit(ResultCode.RESULT_ERROR_ACCESSING_SW360)
 
             print_red("  Unknown error updating project: " + repr(swex))
             sys.exit(ResultCode.RESULT_ERROR_ACCESSING_SW360)
```

### Comparing `capycli-2.2.1/capycli/project/create_readme.py` & `capycli-2.3.0/capycli/project/create_readme.py`

 * *Files identical despite different names*

### Comparing `capycli-2.2.1/capycli/project/find_project.py` & `capycli-2.3.0/capycli/project/find_project.py`

 * *Files identical despite different names*

### Comparing `capycli-2.2.1/capycli/project/get_license_info.py` & `capycli-2.3.0/capycli/project/get_license_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,17 @@
 from capycli.common.script_support import ScriptSupport
 from capycli.main.result_codes import ResultCode
 
 LOG = capycli.get_logger(__name__)
 
 
 class GetLicenseInfo(capycli.common.script_base.ScriptBase):
+    def __init__(self) -> None:
+        self.has_error = False
+
     """
     Get license info on all project components.
     """
     def get_cli_files_for_release(self, release: Dict[str, Any],
                                   folder: str, no_overwrite: bool) -> List[Dict[str, Any]]:
         """Find all CLI file attachments for the given release, download them and return
         a list with the file information."""
@@ -127,14 +130,15 @@
                 os.mkdir(target_folder)
 
             for key in releases:
                 href = key["_links"]["self"]["href"]
                 release = self.client.get_release_by_url(href)
                 if not release:
                     print_red("  ERROR: unable to access release")
+                    self.has_error = True
                     continue
 
                 component_name = release["name"]
                 if "version" in release:
                     component_name = (
                         component_name + " " + release["version"]
                     )
@@ -162,14 +166,18 @@
                         if not warning_shown:
                             print_yellow("        Multiple CLI files exist for the same component"
                                          + " - manual review needed!")
                             warning_shown = True
 
                     complist.append(comp)
 
+                if len(cli_files) == 0:
+                    print_red("        No CLI file exist for this component!")
+                    self.has_error = True
+
             complist.sort(key=lambda s: s["ComponentName"].lower())
 
             rdm_info["Components"] = complist
 
         return rdm_info
 
     def show_command_help(self) -> None:
@@ -184,14 +192,15 @@
   -version                       version of the project
   -i INPUTFILE                   existing configuration file to read from (optional)
   -o OUTPUTFILE                  write config file for "project CreateReadme"
   -dest DESTINATION              destination folder
   -ncli, --no-overwrite-cli      do not overwrite existing CLI files
   -nconf, --no-overwrite-config  do not overwrite an existing configuration file
   -all                           add all available CLI files of a component
+  --forceerror                   force an error exit code in case of missing information
         """)
 
         print()
 
     @classmethod
     def write_result(cls, result: Dict[str, Any], filename: str, no_overwrite: bool) -> None:
         """Write the Readme_OSS configuration to a JSON file"""
@@ -256,7 +265,10 @@
         print("")
 
         if args.outputfile:
             print_text("  Writing Readme_OSS config file " + args.outputfile)
             self.write_result(rdm_info, args.outputfile, args.nconf)
 
         print_text("\ndone.")
+
+        if args.force_error and self.has_error:
+            sys.exit(ResultCode.RESULT_LICENSE_INFO_ERROR)
```

### Comparing `capycli-2.2.1/capycli/project/handle_project.py` & `capycli-2.3.0/capycli/project/handle_project.py`

 * *Files identical despite different names*

### Comparing `capycli-2.2.1/capycli/project/show_ecc.py` & `capycli-2.3.0/capycli/project/show_ecc.py`

 * *Files identical despite different names*

### Comparing `capycli-2.2.1/capycli/project/show_licenses.py` & `capycli-2.3.0/capycli/project/show_licenses.py`

 * *Files identical despite different names*

### Comparing `capycli-2.2.1/capycli/project/show_project.py` & `capycli-2.3.0/capycli/project/show_project.py`

 * *Files identical despite different names*

### Comparing `capycli-2.2.1/capycli/project/show_vulnerabilities.py` & `capycli-2.3.0/capycli/project/show_vulnerabilities.py`

 * *Files identical despite different names*

### Comparing `capycli-2.2.1/License.md` & `capycli-2.3.0/License.md`

 * *Files identical despite different names*

### Comparing `capycli-2.2.1/pyproject.toml` & `capycli-2.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # SPDX-FileCopyrightText: (c) 2018-2024 Siemens
 # SPDX-License-Identifier: MIT
 
 [tool.poetry]
 name = "capycli"
-version = "2.2.1"
+version = "2.3.0"
 description = "CaPyCli - Clearing Automation Python Command Line Interface for SW360"
 authors = ["Thomas Graf <thomas.graf@siemens.com>"]
 license = "MIT"
 readme="Readme.md"
 repository = "https://github.com/sw360/capycli"
 homepage = "https://github.com/sw360/capycli"
 keywords = ["sw360", "cli, automation", "license", "compliance", "clearing"]
```

### Comparing `capycli-2.2.1/Readme.md` & `capycli-2.3.0/Readme.md`

 * *Files 2% similar despite different names*

```diff
@@ -134,14 +134,15 @@
   -all                                              show/use all items
   -format FORMAT                                    format to use (text, json, xml)
   -fe FORCE_EXIT, --forceexit FORCE_EXIT            force a specific exit code
   -m MODE, --mode MODE                              specific mode for some commands
   -if INPUTFORMAT                                   Specify input file format
   -of OUTPUTFORMAT                                  Specify output file format
   -X DEBUG                                          Enable debug output
+  --forceerror FORCE_ERROR                          force an error exit code in case of visual errors
 ```
 
 ## Use Cases
 
 Over the time we implemented more and more commands with more and more parameters.  
 We understand that it is hard for beginners to find the right command for the task
 they want to do. Have a look at our [Use Case Overview](UseCaseOverview.md).
```

### Comparing `capycli-2.2.1/PKG-INFO` & `capycli-2.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capycli
-Version: 2.2.1
+Version: 2.3.0
 Summary: CaPyCli - Clearing Automation Python Command Line Interface for SW360
 Home-page: https://github.com/sw360/capycli
 License: MIT
 Keywords: sw360,cli, automation,license,compliance,clearing
 Author: Thomas Graf
 Author-email: thomas.graf@siemens.com
 Requires-Python: >=3.8,<4.0
@@ -177,14 +177,15 @@
   -all                                              show/use all items
   -format FORMAT                                    format to use (text, json, xml)
   -fe FORCE_EXIT, --forceexit FORCE_EXIT            force a specific exit code
   -m MODE, --mode MODE                              specific mode for some commands
   -if INPUTFORMAT                                   Specify input file format
   -of OUTPUTFORMAT                                  Specify output file format
   -X DEBUG                                          Enable debug output
+  --forceerror FORCE_ERROR                          force an error exit code in case of visual errors
 ```
 
 ## Use Cases
 
 Over the time we implemented more and more commands with more and more parameters.  
 We understand that it is hard for beginners to find the right command for the task
 they want to do. Have a look at our [Use Case Overview](UseCaseOverview.md).
```

