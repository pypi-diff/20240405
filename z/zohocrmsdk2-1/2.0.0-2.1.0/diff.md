# Comparing `tmp/zohocrmsdk2_1-2.0.0.tar.gz` & `tmp/zohocrmsdk2_1-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zohocrmsdk2_1-2.0.0.tar", last modified: Mon Mar 13 11:32:39 2023, max compression
+gzip compressed data, was "dist/zohocrmsdk2_1-2.1.0.tar", last modified: Fri Apr  5 08:20:01 2024, max compression
```

## Comparing `zohocrmsdk2_1-2.0.0.tar` & `zohocrmsdk2_1-2.1.0.tar`

### file list

```diff
@@ -1,572 +1,572 @@
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-03-13 11:32:39.915367 zohocrmsdk2_1-2.0.0/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    11358 2023-02-28 12:06:06.000000 zohocrmsdk2_1-2.0.0/LICENSE
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      103 2023-02-28 12:06:06.000000 zohocrmsdk2_1-2.0.0/MANIFEST.in
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    43029 2023-03-13 11:32:39.915367 zohocrmsdk2_1-2.0.0/PKG-INFO
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    42023 2023-02-28 12:06:06.000000 zohocrmsdk2_1-2.0.0/README.md
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)       67 2023-03-13 11:32:39.915367 zohocrmsdk2_1-2.0.0/setup.cfg
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1584 2023-03-08 05:45:19.000000 zohocrmsdk2_1-2.0.0/setup.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-03-13 11:32:39.871353 zohocrmsdk2_1-2.0.0/zcrmsdk/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)       17 2023-02-28 12:06:06.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/__init__.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-03-13 11:32:39.871353 zohocrmsdk2_1-2.0.0/zcrmsdk/src/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)       17 2023-02-28 12:06:06.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/__init__.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-03-13 11:32:39.871353 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)       18 2023-02-28 12:06:06.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/__init__.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-03-13 11:32:39.871353 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)       35 2023-02-28 12:06:06.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/__init__.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-03-13 11:32:39.871353 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/api/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)       49 2023-02-28 12:06:06.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/api/__init__.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-03-13 11:32:39.871353 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/api/authenticator/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)       81 2023-02-28 12:06:06.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/api/authenticator/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    12690 2023-02-28 12:06:06.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/api/authenticator/oauth_token.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-03-13 11:32:39.875354 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/api/authenticator/store/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      100 2023-02-28 12:06:06.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/api/authenticator/store/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    11433 2023-02-28 12:06:06.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/api/authenticator/store/db_store.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     8998 2023-02-28 12:06:06.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/api/authenticator/store/file_store.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1969 2023-02-28 12:06:06.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/api/authenticator/store/token_store.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      665 2023-02-28 12:06:06.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/api/authenticator/token.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-03-13 11:32:39.875354 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/api/logger/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)       39 2023-02-28 12:06:06.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/api/logger/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2813 2023-02-28 12:06:06.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/api/logger/logger.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-03-13 11:32:39.875354 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)       17 2023-02-28 12:06:06.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/__init__.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-03-13 11:32:39.875354 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1203 2023-02-28 12:24:33.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/__init__.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-03-13 11:32:39.875354 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/assignment_rules/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      305 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/assignment_rules/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3666 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/assignment_rules/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     7179 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/assignment_rules/assignment_rule.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2745 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/assignment_rules/assignment_rules_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2379 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/assignment_rules/default_user.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/assignment_rules/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2224 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/assignment_rules/response_wrapper.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-03-13 11:32:39.875354 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/attachments/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      518 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/attachments/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/attachments/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/attachments/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2037 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/attachments/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3948 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/attachments/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    12859 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/attachments/attachment.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     8819 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/attachments/attachments_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2135 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/attachments/file_body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/attachments/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2648 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/attachments/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3662 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/attachments/success_response.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-03-13 11:32:39.875354 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/blue_print/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      572 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/blue_print/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/blue_print/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3805 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/blue_print/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4015 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/blue_print/blue_print.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3181 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/blue_print/blue_print_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1949 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/blue_print/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2431 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/blue_print/escalation.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    38610 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/blue_print/field.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3577 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/blue_print/next_transition.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     7968 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/blue_print/process_info.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/blue_print/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2291 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/blue_print/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3661 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/blue_print/success_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     9036 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/blue_print/transition.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4365 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/blue_print/validation_error.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-03-13 11:32:39.879355 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      599 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2519 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3942 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3550 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/bulk_read_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2421 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/call_back.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4682 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/criteria.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2133 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/file_body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     6167 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/job_detail.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4242 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/query.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3309 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/request_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2049 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4225 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/result.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3660 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/success_response.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-03-13 11:32:39.879355 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      590 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     7349 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     5554 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/bulk_write_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     7120 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/bulk_write_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2421 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/call_back.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4729 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/field_mapping.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4933 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/file.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2134 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/file_body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3956 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/request_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     6545 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/resource.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2021 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/result.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3661 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/success_response.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-03-13 11:32:39.879355 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/cancel_meetings/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      344 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/cancel_meetings/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/cancel_meetings/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/cancel_meetings/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2041 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/cancel_meetings/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3805 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/cancel_meetings/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1879 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/cancel_meetings/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1940 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/cancel_meetings/cancel_meetings_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2143 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/cancel_meetings/notify.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3666 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/cancel_meetings/success_response.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-03-13 11:32:39.883357 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      831 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2165 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4314 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2005 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3043 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/contact_role.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2045 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/contact_role_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    14189 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/contact_roles_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      150 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/record_action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2083 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/record_action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1891 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/record_body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      154 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/record_response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2694 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/record_response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2179 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3664 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/success_response.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-03-13 11:32:39.883357 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/currencies/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      649 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/currencies/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/currencies/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/currencies/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2120 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/currencies/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4149 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/currencies/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      162 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/currencies/base_currency_action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2471 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/currencies/base_currency_action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2180 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/currencies/base_currency_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1963 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/currencies/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     8586 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/currencies/currencies_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     9248 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/currencies/currency.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3407 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/currencies/format.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/currencies/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2134 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/currencies/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3661 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/currencies/success_response.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-03-13 11:32:39.883357 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/custom_views/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      416 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/custom_views/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3662 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/custom_views/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4110 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/custom_views/criteria.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    12961 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/custom_views/custom_view.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3292 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/custom_views/custom_views_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4914 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/custom_views/info.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2369 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/custom_views/range.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/custom_views/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2769 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/custom_views/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3501 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/custom_views/shared_to.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4067 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/custom_views/translation.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-03-13 11:32:39.883357 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/dc/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      282 2023-02-28 12:06:06.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/dc/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1408 2023-02-28 12:06:06.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/dc/au_data_center.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1399 2023-02-28 12:06:06.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/dc/cn_data_center.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1125 2023-02-28 12:06:06.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/dc/data_center.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1381 2023-02-28 12:06:06.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/dc/eu_data_center.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1379 2023-02-28 12:06:06.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/dc/in_data_center.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1402 2023-02-28 12:06:06.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/dc/jp_data_center.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1384 2023-02-28 12:06:06.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/dc/us_data_center.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-03-13 11:32:39.883357 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/email_templates/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      298 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/email_templates/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3665 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/email_templates/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3501 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/email_templates/attachment.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    12517 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/email_templates/email_template.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2709 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/email_templates/email_templates_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/email_templates/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2806 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/email_templates/response_wrapper.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-03-13 11:32:39.883357 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/exception/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)       40 2023-02-28 12:06:06.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/exception/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1157 2023-02-28 12:06:06.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/exception/sdk_exception.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-03-13 11:32:39.887358 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/field_attachments/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      266 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/field_attachments/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3667 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/field_attachments/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1909 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/field_attachments/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2486 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/field_attachments/field_attachments_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2141 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/field_attachments/file_body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/field_attachments/response_handler.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-03-13 11:32:39.887358 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/fields/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      928 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/fields/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3656 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/fields/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2989 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/fields/association_details.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3099 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/fields/auto_number.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4579 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/fields/crypt.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2651 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/fields/currency.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3173 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/fields/external.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    39525 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/fields/field.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3112 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/fields/fields_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2611 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/fields/formula.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2953 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/fields/history_tracking.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2369 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/fields/lookup_field.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2605 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/fields/maps.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4878 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/fields/module.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3028 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/fields/multi_module_lookup.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     5945 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/fields/multi_select_lookup.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     5941 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/fields/multi_user_lookup.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     8155 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/fields/pick_list_value.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3027 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/fields/private.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4867 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/fields/related_details.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/fields/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2074 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/fields/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2419 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/fields/tool_tip.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2037 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/fields/unique.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3557 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/fields/view_type.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-03-13 11:32:39.887358 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/file/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      421 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/file/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/file/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/file/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2030 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/file/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3927 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/file/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1909 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/file/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2128 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/file/file_body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3292 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/file/file_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/file/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3655 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/file/success_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      447 2023-02-28 12:06:06.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/header.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1796 2023-02-28 12:06:06.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/header_map.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    11164 2023-02-28 12:06:06.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/initializer.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-03-13 11:32:39.887358 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/inventory_templates/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      314 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/inventory_templates/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3669 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/inventory_templates/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    11325 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/inventory_templates/inventory_template.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4452 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/inventory_templates/inventory_templates_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/inventory_templates/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2866 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/inventory_templates/response_wrapper.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-03-13 11:32:39.887358 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/layouts/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      306 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/layouts/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3657 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/layouts/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     9894 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/layouts/layout.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2618 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/layouts/layouts_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3312 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/layouts/properties.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/layouts/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2089 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/layouts/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     8187 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/layouts/section.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-03-13 11:32:39.891359 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/modules/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      562 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/modules/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/modules/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/modules/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2075 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/modules/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3936 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/modules/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2421 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/modules/argument.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1921 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/modules/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    32535 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/modules/module.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     5472 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/modules/modules_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3087 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/modules/related_list_properties.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/modules/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2089 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/modules/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3658 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/modules/success_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2995 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/modules/territory.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-03-13 11:32:39.891359 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/notes/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      514 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/notes/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/notes/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/notes/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2031 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/notes/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3930 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/notes/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1879 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/notes/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3585 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/notes/info.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    11919 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/notes/note.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    10048 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/notes/notes_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/notes/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2643 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/notes/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3656 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/notes/success_response.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-03-13 11:32:39.891359 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/notification/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      522 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/notification/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/notification/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/notification/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2052 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/notification/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3951 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/notification/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1893 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/notification/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3585 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/notification/info.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     8186 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/notification/notification.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     8168 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/notification/notification_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/notification/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2671 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/notification/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3663 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/notification/success_response.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-03-13 11:32:39.891359 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/org/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      430 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/org/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/org/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3791 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/org/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1971 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/org/file_body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1919 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/org/hierarchy_preference.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     5172 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/org/license_details.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    21725 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/org/org.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2321 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/org/org_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/org/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2029 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/org/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3654 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/org/success_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      454 2023-02-28 12:06:06.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/param.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1817 2023-02-28 12:06:06.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/parameter_map.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-03-13 11:32:39.895360 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/pipeline/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      963 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/pipeline/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/pipeline/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/pipeline/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2090 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/pipeline/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4304 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/pipeline/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1935 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/pipeline/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2379 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/pipeline/forecast_category.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     5919 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/pipeline/pick_list_value.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     6510 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/pipeline/pipeline.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     8659 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/pipeline/pipeline_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/pipeline/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2104 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/pipeline/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2369 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/pipeline/stage.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3844 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/pipeline/success_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      154 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/pipeline/transfer_action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      156 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/pipeline/transfer_action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2274 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/pipeline/transfer_action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2087 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/pipeline/transfer_and_delete_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2614 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/pipeline/transfer_pipe_line.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-03-13 11:32:39.895360 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/profiles/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      396 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/profiles/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3658 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/profiles/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3783 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/profiles/category.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2877 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/profiles/default_view.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4121 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/profiles/permission_detail.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    10635 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/profiles/profile.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2803 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/profiles/profiles_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/profiles/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2104 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/profiles/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2463 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/profiles/section.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-03-13 11:32:39.895360 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/query/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      216 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/query/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3655 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/query/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2031 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/query/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1591 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/query/query_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/query/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2642 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/query/response_wrapper.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-03-13 11:32:39.899362 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3107 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2032 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     5613 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1923 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/apply_feature_execution.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     5561 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2977 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/carry_over_tags.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3854 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/comment.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     7057 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/consent.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      152 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/convert_action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      154 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/convert_action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2083 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/convert_action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1893 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/convert_body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      136 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/count_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2055 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/count_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4015 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/criteria.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     5020 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/deleted_record.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      154 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/deleted_records_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2689 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/deleted_records_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/download_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    36450 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/field.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2276 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/file_body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    10456 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/file_details.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      134 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/file_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     6561 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/image_upload.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3585 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/info.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     6709 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/lead_converter.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2041 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/line_item_product.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4125 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/line_tax.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4693 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/mass_update.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      158 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/mass_update_action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      160 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/mass_update_action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2106 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/mass_update_action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4838 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/mass_update_body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      148 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/mass_update_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      162 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/mass_update_response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2120 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/mass_update_response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3731 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/mass_update_success_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2523 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/mass_update_territory.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2968 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/multi_select_lookup.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2431 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/multi_select_picklist.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      306 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/options.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3489 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/participants.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      897 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/price_book.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2067 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/pricing_details.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     6385 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/record.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    49696 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/record_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1931 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/recurring_activity.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1913 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/remind_at.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2437 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/reminder.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2645 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4991 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/success_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3266 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/successful_convert.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2369 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/tax.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4300 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/territory.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2359 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/widget.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2359 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/wizard.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-03-13 11:32:39.899362 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/related_lists/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      274 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/related_lists/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3663 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/related_lists/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     7709 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/related_lists/related_list.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2706 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/related_lists/related_lists_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/related_lists/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2179 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/related_lists/response_wrapper.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-03-13 11:32:39.899362 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/related_records/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      975 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/related_records/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/related_records/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/related_records/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2041 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/related_records/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3960 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/related_records/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1879 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/related_records/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2139 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/related_records/file_body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    26554 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/related_records/related_records_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/related_records/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2652 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/related_records/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3666 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/related_records/success_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1858 2023-02-28 12:06:06.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/request_proxy.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-03-13 11:32:39.903363 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/roles/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      201 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/roles/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3655 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/roles/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/roles/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2059 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/roles/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     6389 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/roles/role.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1942 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/roles/roles_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1753 2023-02-28 12:06:06.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/sdk_config.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-03-13 11:32:39.903363 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/send_mail/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      590 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/send_mail/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/send_mail/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/send_mail/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2035 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/send_mail/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3942 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/send_mail/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1879 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/send_mail/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2383 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/send_mail/data_subject_request.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3519 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/send_mail/inventory_details.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    13774 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/send_mail/mail.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/send_mail/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2189 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/send_mail/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2907 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/send_mail/send_mail_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3660 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/send_mail/success_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      128 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/send_mail/template.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4031 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/send_mail/user_address.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-03-13 11:32:39.903363 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/share_records/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      681 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/share_records/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/share_records/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/share_records/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2053 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/share_records/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4309 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/share_records/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1893 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/share_records/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      150 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/share_records/delete_action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      152 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/share_records/delete_action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2383 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/share_records/delete_action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/share_records/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2691 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/share_records/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     5510 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/share_records/share_record.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     6234 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/share_records/share_records_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3128 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/share_records/shared_through.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3844 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/share_records/success_response.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-03-13 11:32:39.907364 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/tags/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      972 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/tags/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/tags/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/tags/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2030 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/tags/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4393 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/tags/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1879 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/tags/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2023 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/tags/conflict_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      136 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/tags/count_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2063 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/tags/count_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2537 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/tags/info.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1881 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/tags/merge_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      150 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/tags/record_action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      152 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/tags/record_action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3982 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/tags/record_action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/tags/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2641 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/tags/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3826 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/tags/success_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     5649 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/tags/tag.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    17633 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/tags/tags_operations.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-03-13 11:32:39.907364 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/taxes/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      464 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/taxes/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/taxes/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/taxes/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2045 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/taxes/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3930 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/taxes/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1893 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/taxes/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2797 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/taxes/preference.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/taxes/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2801 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/taxes/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3656 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/taxes/success_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4203 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/taxes/tax.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     6514 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/taxes/taxes_operations.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-03-13 11:32:39.907364 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/territories/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      223 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/territories/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3661 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/territories/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/territories/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2746 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/territories/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2000 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/territories/territories_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     9478 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/territories/territory.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1145 2023-02-28 12:06:06.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/user_signature.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-03-13 11:32:39.907364 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/users/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      683 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/users/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/users/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/users/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2045 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/users/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3930 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/users/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1893 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/users/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     5245 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/users/customize_info.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3585 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/users/info.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1899 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/users/request_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/users/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2657 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/users/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2357 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/users/shift.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3656 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/users/success_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2597 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/users/tab_theme.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2915 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/users/territory.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     5179 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/users/theme.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    24295 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/users/user.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     8403 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/users/users_operations.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-03-13 11:32:39.911365 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/util/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      630 2023-02-28 12:06:06.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/util/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     6709 2023-02-28 12:06:06.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/util/api_http_connector.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1348 2023-02-28 12:06:06.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/util/api_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      245 2023-02-28 12:06:06.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/util/choice.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    15447 2023-02-28 12:06:06.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/util/common_api_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    15655 2023-03-08 05:45:26.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/util/constants.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    10600 2023-02-28 12:06:06.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/util/converter.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4275 2023-02-28 12:06:06.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/util/datatype_converter.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3370 2023-02-28 12:06:06.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/util/downloader.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     7860 2023-02-28 12:06:06.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/util/form_data_converter.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3468 2023-02-28 12:06:06.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/util/header_param_validator.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    31813 2023-02-28 12:06:06.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/util/json_converter.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     5689 2023-03-13 10:16:55.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/util/module_fields_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1531 2023-02-28 12:06:06.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/util/stream_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    40824 2023-03-01 06:43:59.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/util/utility.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      972 2023-02-28 12:06:06.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/util/xml_converter.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-03-13 11:32:39.911365 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/variable_groups/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      239 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/variable_groups/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3665 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/variable_groups/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/variable_groups/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2209 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/variable_groups/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4217 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/variable_groups/variable_group.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3044 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/variable_groups/variable_groups_operations.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-03-13 11:32:39.911365 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/variables/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      520 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/variables/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/variables/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/variables/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2105 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/variables/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3942 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/variables/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1949 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/variables/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/variables/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2119 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/variables/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3660 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/variables/success_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     5801 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/variables/variable.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    11833 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/variables/variables_operations.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-03-13 11:32:39.911365 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/wizards/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      472 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/wizards/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3657 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/wizards/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     8223 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/wizards/button.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3739 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/wizards/chart_data.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2885 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/wizards/connection.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3762 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/wizards/container.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3655 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/wizards/node.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/wizards/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2089 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/wizards/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3043 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/wizards/screen.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     5351 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/wizards/segment.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2367 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/wizards/transition.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     8600 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/wizards/wizard.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2649 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/wizards/wizards_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)   195128 2023-03-07 11:26:41.000000 zohocrmsdk2_1-2.0.0/zcrmsdk/src/json_details.json
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-03-13 11:32:39.915367 zohocrmsdk2_1-2.0.0/zohocrmsdk2_1.egg-info/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    43029 2023-03-13 11:32:39.000000 zohocrmsdk2_1-2.0.0/zohocrmsdk2_1.egg-info/PKG-INFO
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    28648 2023-03-13 11:32:39.000000 zohocrmsdk2_1-2.0.0/zohocrmsdk2_1.egg-info/SOURCES.txt
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)        1 2023-03-13 11:32:39.000000 zohocrmsdk2_1-2.0.0/zohocrmsdk2_1.egg-info/dependency_links.txt
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)       33 2023-03-13 11:32:39.000000 zohocrmsdk2_1-2.0.0/zohocrmsdk2_1.egg-info/requires.txt
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)        8 2023-03-13 11:32:39.000000 zohocrmsdk2_1-2.0.0/zohocrmsdk2_1.egg-info/top_level.txt
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-05 08:20:01.000000 zohocrmsdk2_1-2.1.0/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    51726 2024-04-05 08:20:01.000000 zohocrmsdk2_1-2.1.0/PKG-INFO
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    11358 2021-12-23 08:38:55.000000 zohocrmsdk2_1-2.1.0/LICENSE
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-05 08:20:01.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)       17 2021-11-19 11:38:03.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/__init__.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-05 08:20:01.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)       17 2021-11-19 11:38:03.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)   195184 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/json_details.json
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-05 08:20:01.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-05 08:20:01.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-05 08:20:01.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)       17 2021-11-19 11:38:03.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/__init__.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-05 08:20:01.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-05 08:20:01.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/pipeline/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3844 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/pipeline/success_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/pipeline/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/pipeline/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2104 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/pipeline/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4304 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/pipeline/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2614 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/pipeline/transfer_pipe_line.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      963 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/pipeline/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2379 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/pipeline/forecast_category.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2087 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/pipeline/transfer_and_delete_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2090 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/pipeline/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     5919 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/pipeline/pick_list_value.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/pipeline/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     6510 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/pipeline/pipeline.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     8659 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/pipeline/pipeline_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      156 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/pipeline/transfer_action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2369 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/pipeline/stage.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2274 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/pipeline/transfer_action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1935 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/pipeline/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      154 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/pipeline/transfer_action_handler.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-05 08:20:01.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/currencies/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3661 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/currencies/success_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/currencies/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/currencies/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2134 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/currencies/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4149 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/currencies/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2471 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/currencies/base_currency_action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      162 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/currencies/base_currency_action_handler.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      649 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/currencies/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3407 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/currencies/format.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2180 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/currencies/base_currency_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2120 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/currencies/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/currencies/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     8586 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/currencies/currencies_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     9248 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/currencies/currency.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1963 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/currencies/body_wrapper.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-05 08:20:01.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/territories/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/territories/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2746 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/territories/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3661 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/territories/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     9478 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/territories/territory.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2000 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/territories/territories_operations.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      223 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/territories/__init__.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1817 2021-11-19 13:58:05.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/parameter_map.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-05 08:20:01.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2120 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/mass_update_response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4015 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/criteria.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4991 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/success_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2055 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/count_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      306 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/options.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    36450 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/field.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2369 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/tax.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     6561 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/image_upload.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1931 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/recurring_activity.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2106 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/mass_update_action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3266 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/successful_convert.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2041 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/line_item_product.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2067 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/pricing_details.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      158 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/mass_update_action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2276 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/file_body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3854 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/comment.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      134 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/file_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2359 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/widget.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4838 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/mass_update_body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3731 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/mass_update_success_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      148 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/mass_update_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2645 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      162 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/mass_update_response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      136 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/count_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     5613 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2431 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/multi_select_picklist.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2083 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/convert_action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     5020 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/deleted_record.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4300 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/territory.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4693 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/mass_update.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      160 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/mass_update_action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      152 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/convert_action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3107 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2523 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/mass_update_territory.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2968 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/multi_select_lookup.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2359 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/wizard.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2032 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      154 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/deleted_records_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1893 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/convert_body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      897 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/price_book.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    10456 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/file_details.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     6709 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/lead_converter.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2689 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/deleted_records_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      154 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/convert_action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/download_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     6385 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/record.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1913 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/remind_at.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3489 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/participants.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    49696 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/record_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2977 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/carry_over_tags.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1923 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/apply_feature_execution.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     5561 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3585 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/info.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     7057 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/consent.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4125 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/line_tax.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2437 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/reminder.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-05 08:20:01.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/field_attachments/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2486 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/field_attachments/field_attachments_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/field_attachments/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2141 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/field_attachments/file_body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3667 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/field_attachments/api_exception.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      266 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/field_attachments/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1909 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/field_attachments/body_wrapper.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      447 2021-11-19 13:57:43.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/header.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-05 08:20:01.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/util/
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3370 2021-11-22 12:15:25.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/util/downloader.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    40824 2023-06-28 11:15:29.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/util/utility.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    15655 2024-04-05 08:18:43.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/util/constants.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      245 2021-11-19 13:57:00.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/util/choice.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    10600 2021-11-22 12:09:24.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/util/converter.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      630 2021-11-19 11:38:03.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/util/__init__.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3468 2021-11-19 13:57:00.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/util/header_param_validator.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     5689 2023-06-28 11:15:29.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/util/module_fields_handler.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    31813 2021-11-24 06:16:14.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/util/json_converter.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      972 2021-11-19 13:57:00.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/util/xml_converter.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1348 2021-11-19 13:56:10.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/util/api_response.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1531 2021-11-19 13:57:00.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/util/stream_wrapper.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     6709 2021-11-22 09:46:50.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/util/api_http_connector.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    15447 2021-11-22 10:42:07.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/util/common_api_handler.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     7860 2021-11-22 12:34:41.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/util/form_data_converter.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4275 2021-11-19 13:57:00.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/util/datatype_converter.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-05 08:20:01.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/file/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3655 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/file/success_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/file/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/file/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2128 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/file/file_body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3927 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/file/api_exception.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      421 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/file/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2030 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/file/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/file/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1909 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/file/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3292 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/file/file_operations.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-05 08:20:01.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/related_lists/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/related_lists/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2179 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/related_lists/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3663 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/related_lists/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     7709 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/related_lists/related_list.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      274 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/related_lists/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2706 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/related_lists/related_lists_operations.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-05 08:20:01.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/notification/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3663 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/notification/success_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/notification/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/notification/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2671 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/notification/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3951 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/notification/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     8186 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/notification/notification.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      522 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/notification/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2052 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/notification/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/notification/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1893 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/notification/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3585 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/notification/info.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     8168 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/notification/notification_operations.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-05 08:20:01.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/org/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3654 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/org/success_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/org/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/org/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    21725 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/org/org.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1971 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/org/file_body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2029 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/org/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3791 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/org/api_exception.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      430 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/org/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     5172 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/org/license_details.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1919 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/org/hierarchy_preference.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2321 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/org/org_operations.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-05 08:20:01.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/inventory_templates/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/inventory_templates/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2866 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/inventory_templates/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3669 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/inventory_templates/api_exception.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      314 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/inventory_templates/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4452 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/inventory_templates/inventory_templates_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    11325 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/inventory_templates/inventory_template.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-05 08:20:01.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/blue_print/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3661 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/blue_print/success_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/blue_print/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    38610 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/blue_print/field.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/blue_print/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2291 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/blue_print/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4365 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/blue_print/validation_error.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3805 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/blue_print/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     9036 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/blue_print/transition.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4015 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/blue_print/blue_print.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      572 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/blue_print/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2431 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/blue_print/escalation.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     7968 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/blue_print/process_info.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3577 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/blue_print/next_transition.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3181 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/blue_print/blue_print_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1949 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/blue_print/body_wrapper.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-05 08:20:01.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/email_templates/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/email_templates/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2709 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/email_templates/email_templates_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2806 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/email_templates/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3665 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/email_templates/api_exception.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      298 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/email_templates/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3501 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/email_templates/attachment.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    12517 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/email_templates/email_template.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-05 08:20:01.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/related_records/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3666 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/related_records/success_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/related_records/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/related_records/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2139 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/related_records/file_body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2652 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/related_records/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3960 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/related_records/api_exception.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      975 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/related_records/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2041 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/related_records/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/related_records/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    26554 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/related_records/related_records_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1879 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/related_records/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1203 2024-04-05 08:05:48.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/__init__.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-05 08:20:01.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/roles/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/roles/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2059 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/roles/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3655 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/roles/api_exception.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      201 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/roles/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     6389 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/roles/role.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1942 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/roles/roles_operations.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      454 2021-11-19 13:57:57.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/param.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1796 2021-11-19 13:57:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/header_map.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-05 08:20:01.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/cancel_meetings/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3666 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/cancel_meetings/success_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/cancel_meetings/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1940 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/cancel_meetings/cancel_meetings_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3805 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/cancel_meetings/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      344 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/cancel_meetings/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2143 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/cancel_meetings/notify.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2041 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/cancel_meetings/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/cancel_meetings/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1879 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/cancel_meetings/body_wrapper.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-05 08:20:01.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/tags/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3826 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/tags/success_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/tags/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2063 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/tags/count_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    17633 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/tags/tags_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1881 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/tags/merge_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/tags/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      152 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/tags/record_action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2641 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/tags/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      136 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/tags/count_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4393 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/tags/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3982 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/tags/record_action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2023 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/tags/conflict_wrapper.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      972 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/tags/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      150 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/tags/record_action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2030 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/tags/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/tags/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1879 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/tags/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2537 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/tags/info.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     5649 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/tags/tag.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    11164 2021-12-23 08:40:15.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/initializer.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-05 08:20:01.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/custom_views/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4110 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/custom_views/criteria.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3292 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/custom_views/custom_views_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/custom_views/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2769 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/custom_views/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3662 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/custom_views/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2369 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/custom_views/range.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      416 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/custom_views/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    12961 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/custom_views/custom_view.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4067 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/custom_views/translation.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3501 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/custom_views/shared_to.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4914 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/custom_views/info.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1145 2021-11-19 13:58:25.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/user_signature.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-05 08:20:01.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4682 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/criteria.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3660 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/success_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2133 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/file_body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2049 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4242 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/query.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3942 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/api_exception.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      599 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     6167 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/job_detail.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2421 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/call_back.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4225 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/result.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2519 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3309 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/request_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3550 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/bulk_read_operations.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-05 08:20:01.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/notes/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3656 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/notes/success_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/notes/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/notes/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2643 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/notes/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    10048 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/notes/notes_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3930 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/notes/api_exception.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      514 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/notes/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2031 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/notes/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/notes/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1879 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/notes/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3585 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/notes/info.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    11919 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/notes/note.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-05 08:20:01.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/variable_groups/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/variable_groups/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2209 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/variable_groups/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3665 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/variable_groups/api_exception.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      239 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/variable_groups/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4217 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/variable_groups/variable_group.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3044 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/variable_groups/variable_groups_operations.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-05 08:20:01.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3664 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/success_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    14189 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/contact_roles_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2045 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/contact_role_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2179 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4314 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1891 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/record_body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2694 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/record_response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2083 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/record_action_wrapper.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      831 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      154 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/record_response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      150 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/record_action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2165 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2005 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3043 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/contact_role.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-05 08:20:01.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/layouts/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/layouts/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2089 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/layouts/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3657 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/layouts/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3312 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/layouts/properties.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     9894 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/layouts/layout.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      306 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/layouts/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     8187 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/layouts/section.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2618 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/layouts/layouts_operations.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-05 08:20:01.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/variables/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3660 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/variables/success_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/variables/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/variables/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2119 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/variables/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3942 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/variables/api_exception.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      520 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/variables/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     5801 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/variables/variable.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2105 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/variables/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    11833 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/variables/variables_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/variables/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1949 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/variables/body_wrapper.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-05 08:20:01.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/taxes/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3656 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/taxes/success_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/taxes/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4203 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/taxes/tax.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2797 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/taxes/preference.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/taxes/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2801 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/taxes/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3930 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/taxes/api_exception.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      464 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/taxes/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2045 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/taxes/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/taxes/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1893 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/taxes/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     6514 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/taxes/taxes_operations.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-05 08:20:01.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/users/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3656 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/users/success_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/users/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    24295 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/users/user.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/users/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2657 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/users/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     5179 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/users/theme.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2597 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/users/tab_theme.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3930 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/users/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2915 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/users/territory.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      683 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/users/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     5245 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/users/customize_info.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2045 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/users/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2357 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/users/shift.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/users/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1899 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/users/request_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     8403 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/users/users_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1893 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/users/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3585 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/users/info.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-05 08:20:01.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/dc/
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1399 2021-11-22 09:35:43.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/dc/cn_data_center.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1408 2021-11-22 09:35:32.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/dc/au_data_center.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      282 2022-04-01 06:14:32.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/dc/__init__.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1384 2021-11-22 09:36:52.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/dc/us_data_center.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1125 2021-11-22 09:36:20.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/dc/data_center.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1381 2021-11-22 09:36:26.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/dc/eu_data_center.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1402 2022-04-01 06:14:19.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/dc/jp_data_center.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1379 2021-11-22 09:36:31.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/dc/in_data_center.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-05 08:20:01.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/assignment_rules/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/assignment_rules/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2224 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/assignment_rules/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2379 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/assignment_rules/default_user.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3666 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/assignment_rules/api_exception.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      305 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/assignment_rules/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     7179 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/assignment_rules/assignment_rule.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2745 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/assignment_rules/assignment_rules_operations.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-05 08:20:01.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3661 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/success_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2134 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/file_body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     7349 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     6545 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/resource.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      590 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2421 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/call_back.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2021 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/result.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4933 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/file.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4586 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/request_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4729 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/field_mapping.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     5554 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/bulk_write_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     7120 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/bulk_write_response.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-05 08:20:01.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/fields/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4579 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/fields/crypt.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    39525 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/fields/field.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2953 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/fields/history_tracking.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2605 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/fields/maps.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2419 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/fields/tool_tip.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/fields/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3112 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/fields/fields_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2074 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/fields/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4867 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/fields/related_details.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2611 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/fields/formula.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3656 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/fields/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3099 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/fields/auto_number.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2037 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/fields/unique.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      928 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/fields/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2369 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/fields/lookup_field.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     5945 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/fields/multi_select_lookup.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     5941 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/fields/multi_user_lookup.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3557 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/fields/view_type.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     8155 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/fields/pick_list_value.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3028 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/fields/multi_module_lookup.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4878 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/fields/module.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2989 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/fields/association_details.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2651 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/fields/currency.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3173 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/fields/external.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3027 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/fields/private.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-05 08:20:01.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/profiles/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/profiles/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2104 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/profiles/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2803 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/profiles/profiles_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3658 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/profiles/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    10635 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/profiles/profile.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      396 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/profiles/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2463 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/profiles/section.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2877 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/profiles/default_view.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4121 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/profiles/permission_detail.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3783 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/profiles/category.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-05 08:20:01.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/share_records/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3844 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/share_records/success_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/share_records/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/share_records/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     5510 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/share_records/share_record.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2691 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/share_records/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4309 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/share_records/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      152 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/share_records/delete_action_response.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      681 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/share_records/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      150 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/share_records/delete_action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2053 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/share_records/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/share_records/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3128 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/share_records/shared_through.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2383 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/share_records/delete_action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     6234 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/share_records/share_records_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1893 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/share_records/body_wrapper.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-05 08:20:01.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/send_mail/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3660 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/send_mail/success_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    13774 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/send_mail/mail.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/send_mail/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/send_mail/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2189 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/send_mail/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3942 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/send_mail/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2907 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/send_mail/send_mail_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2383 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/send_mail/data_subject_request.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      590 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/send_mail/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2035 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/send_mail/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/send_mail/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4031 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/send_mail/user_address.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3519 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/send_mail/inventory_details.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      128 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/send_mail/template.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1879 2024-04-05 08:05:37.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/send_mail/body_wrapper.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-05 08:20:01.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/wizards/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3043 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/wizards/screen.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/wizards/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2089 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/wizards/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3657 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/wizards/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2649 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/wizards/wizards_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2367 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/wizards/transition.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      472 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/wizards/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3762 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/wizards/container.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2885 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/wizards/connection.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     8600 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/wizards/wizard.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     8223 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/wizards/button.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3739 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/wizards/chart_data.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     5351 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/wizards/segment.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3655 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/wizards/node.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1753 2021-11-19 13:58:19.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/sdk_config.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-05 08:20:01.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/query/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/query/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1591 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/query/query_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2642 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/query/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3655 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/query/api_exception.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      216 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/query/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2031 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/query/body_wrapper.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-05 08:20:01.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/attachments/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3662 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/attachments/success_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/attachments/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/attachments/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2135 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/attachments/file_body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2648 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/attachments/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3948 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/attachments/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     8819 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/attachments/attachments_operations.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      518 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/attachments/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    12859 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/attachments/attachment.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2037 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/attachments/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-05 08:05:36.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/attachments/action_handler.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-05 08:20:01.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/modules/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3658 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/modules/success_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/modules/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2421 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/modules/argument.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/modules/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2089 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/modules/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3936 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/modules/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2995 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/modules/territory.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3087 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/modules/related_list_properties.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      562 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/modules/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2075 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/modules/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/modules/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    32535 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/modules/module.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     5472 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/modules/modules_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1921 2024-04-05 08:05:38.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/modules/body_wrapper.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1858 2021-11-19 13:58:12.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/request_proxy.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-05 08:20:01.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/exception/
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)       40 2021-11-19 11:38:03.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/exception/__init__.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1157 2021-11-22 09:44:50.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/exception/sdk_exception.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)       35 2021-11-19 11:38:03.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/__init__.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-05 08:20:01.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/api/
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-05 08:20:01.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/api/logger/
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)       39 2021-11-19 11:38:03.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/api/logger/__init__.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2813 2021-11-22 09:35:19.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/api/logger/logger.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)       49 2021-11-19 11:38:03.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/api/__init__.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-05 08:20:01.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/api/authenticator/
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      665 2021-11-19 13:54:30.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/api/authenticator/token.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)       81 2021-11-19 11:38:03.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/api/authenticator/__init__.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    12690 2021-11-22 09:34:50.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/api/authenticator/oauth_token.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-05 08:20:01.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/api/authenticator/store/
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     8998 2021-11-22 09:34:40.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/api/authenticator/store/file_store.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    11433 2021-11-22 05:52:47.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/api/authenticator/store/db_store.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1969 2021-11-19 13:54:05.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/api/authenticator/store/token_store.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      100 2021-11-19 11:38:03.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/api/authenticator/store/__init__.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)       18 2021-11-19 11:38:03.000000 zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/__init__.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      103 2022-04-01 06:13:57.000000 zohocrmsdk2_1-2.1.0/MANIFEST.in
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    42023 2021-12-23 08:38:50.000000 zohocrmsdk2_1-2.1.0/README.md
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1584 2024-04-05 08:18:39.000000 zohocrmsdk2_1-2.1.0/setup.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)       67 2024-04-05 08:20:01.000000 zohocrmsdk2_1-2.1.0/setup.cfg
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-05 08:20:01.000000 zohocrmsdk2_1-2.1.0/zohocrmsdk2_1.egg-info/
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    51726 2024-04-05 08:20:00.000000 zohocrmsdk2_1-2.1.0/zohocrmsdk2_1.egg-info/PKG-INFO
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    28648 2024-04-05 08:20:01.000000 zohocrmsdk2_1-2.1.0/zohocrmsdk2_1.egg-info/SOURCES.txt
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)       33 2024-04-05 08:20:00.000000 zohocrmsdk2_1-2.1.0/zohocrmsdk2_1.egg-info/requires.txt
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        8 2024-04-05 08:20:00.000000 zohocrmsdk2_1-2.1.0/zohocrmsdk2_1.egg-info/top_level.txt
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        1 2024-04-05 08:20:00.000000 zohocrmsdk2_1-2.1.0/zohocrmsdk2_1.egg-info/dependency_links.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `zohocrmsdk2_1-2.0.0/LICENSE` & `zohocrmsdk2_1-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/PKG-INFO` & `zohocrmsdk2_1-2.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: zohocrmsdk2_1
-Version: 2.0.0
-Summary: Zoho CRM SDK for ZOHO CRM 2.1 APIs
-Home-page: https://github.com/zoho/zohocrm-python-sdk-2.1
-Author: Zoho CRM API Team
-Author-email: support@zohocrm.com
-License: Apache Software License, Version 2.0, http://www.apache.org/licenses/LICENSE-2.0
-Keywords: development,zoho,crm,api,zcrmsdk,sdk,zcrm,zohocrmsdk2_1
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 License
 =======
 
     Copyright (c) 2021, ZOHO CORPORATION PRIVATE LIMITED 
     All rights reserved. 
 
     Licensed under the Apache License, Version 2.0 (the "License");
```

### Comparing `zohocrmsdk2_1-2.0.0/README.md` & `zohocrmsdk2_1-2.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,1086 +1,1109 @@
-License
-=======
-
-    Copyright (c) 2021, ZOHO CORPORATION PRIVATE LIMITED 
-    All rights reserved. 
-
-    Licensed under the Apache License, Version 2.0 (the "License"); 
-    you may not use this file except in compliance with the License. 
-    You may obtain a copy of the License at 
-    
-        http://www.apache.org/licenses/LICENSE-2.0 
-    
-    Unless required by applicable law or agreed to in writing, software 
-    distributed under the License is distributed on an "AS IS" BASIS, 
-    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. 
-    See the License for the specific language governing permissions and 
-    limitations under the License.
-
-# ZOHO CRM PYTHON SDK 2.1 for API version 2.1
-
-## Table Of Contents
-
-* [Overview](#overview)
-* [Registering a Zoho Client](#registering-a-zoho-client)
-* [Environmental Setup](#environmental-setup)
-* [Including the SDK in your project](#including-the-sdk-in-your-project)
-* [Persistence](#token-persistence)
-  * [DataBase Persistence](#database-persistence)
-  * [File Persistence](#file-persistence)
-  * [Custom Persistence](#custom-persistence)
-* [Configuration](#configuration)
-* [Initialization](#initializing-the-application)
-* [Class Hierarchy](#class-hierarchy)
-* [Responses And Exceptions](#responses-and-exceptions)
-* [Threading](#threading-in-the-python-sdk)
-  * [Multithreading in a Multi-User App](#multithreading-in-a-multi-user-app)
-  * [Multi-threading in a Single User App](#multi-threading-in-a-single-user-app)
-* [Sample Code](#sdk-sample-code)
-## Overview
-
-Zoho CRM PYTHON SDK offers a way to create client Python applications that can be integrated with Zoho CRM.
-
-## Registering a Zoho Client
-
-Since Zoho CRM APIs are authenticated with OAuth2 standards, you should register your client app with Zoho. To register your app:
-
-- Visit this page [https://api-console.zoho.com](https://api-console.zoho.com)
-
-- Click on `ADD CLIENT`.
-
-- Choose the `Client Type`.
-
-- Enter **Client Name**, **Client Domain** or **Homepage URL** and **Authorized Redirect URIs** then click `CREATE`.
-
-- Your Client app will be created.
-
-- Select the created OAuth client.
-
-- Generate grant token by providing the necessary scopes, time duration (the duration for which the generated token is valid) and Scope Description.
-
-## Environmental Setup
-
-Python SDK is installable through **pip**. **pip** is a tool for dependency management in Python. SDK expects the following from the client app.
-
-- Client app must have Python(version 3 and above)
-
-- Python SDK must be installed into client app through **pip**.
-
-## Including the SDK in your project
-
-- Install **Python** from [python.org](https://www.python.org/downloads/) (if not installed).
-
-- Install **Python SDK**
-    - Navigate to the workspace of your client app.
-    - Run the command below:
-
-    ```sh
-    pip install zohocrmsdk2_1==1.x.x
-    ```
-- The Python SDK will be installed in your client application.
-
-## Token Persistence
-
-Token persistence refers to storing and utilizing the authentication tokens that are provided by Zoho. There are three ways provided by the SDK in which persistence can be utilized. They are DataBase Persistence, File Persistence and Custom Persistence.
-
-### Table of Contents
-
-- [DataBase Persistence](#database-persistence)
-
-- [File Persistence](#file-persistence)
-
-- [Custom Persistence](#custom-persistence)
-
-### Implementing OAuth Persistence
-
-Once the application is authorized, OAuth access and refresh tokens can be used for subsequent user data requests to Zoho CRM. Hence, they need to be persisted by the client app.
-
-The persistence is achieved by writing an implementation of the inbuilt Abstract Base Class **[TokenStore](zcrmsdk/src/com/zoho/api/authenticator/store/token_store.py)**, which has the following callback methods.
-
-- **get_token(self, user, [token](zcrmsdk/src/com/zoho/api/authenticator/token.py))** - invoked before firing a request to fetch the saved tokens. This method should return implementation of inbuilt **Token Class** object for the library to process it.
-
-- **save_token(self, user, [token](zcrmsdk/src/com/zoho/api/authenticator/token.py))** - invoked after fetching access and refresh tokens from Zoho.
-
-- **delete_token(self, [token](zcrmsdk/src/com/zoho/api/authenticator/token.py))** - invoked before saving the latest tokens.
-
-- **get_tokens(self)** - The method to get the all the stored tokens.
-
-- **delete_tokens(self)** - The method to delete all the stored tokens.
-
-- **get_token_by_id(self, id, token)** - The method to retrieve the user's token details based on unique ID.
-
-Note:
-
-- user is an instance of UserSignature Class.
-
-- token is an instance of Token Class.
-
-### DataBase Persistence
-
-In case the user prefers to use default DataBase persistence, **MySQL** can be used.
-
-- The database name should be **zohooauth**.
-
-- There must be a table name **oauthtoken** with the following columns.
-
-  - id int(11)
-
-  - user_mail varchar(255)
-  
-  - client_id varchar(255)
-  
-  - client_secret varchar(255)
-
-  - refresh_token varchar(255)
-
-  - access_token varchar(255)
-
-  - grant_token varchar(255)
-
-  - expiry_time varchar(20)
-  
-  - redirect_url varchar(255)
-
-Note:
-- Custom database name and table name can be set in DBStore instance.
-
-#### MySQL Query
-
-```sql
-CREATE TABLE  oauthtoken (
-  id varchar(255) NOT NULL,
-  user_mail varchar(255) NOT NULL,
-  client_id varchar(255),
-  client_secret varchar(255),
-  refresh_token varchar(255),
-  access_token varchar(255),
-  grant_token varchar(255),
-  expiry_time varchar(20),
-  redirect_url varchar(255),
-  primary key (id)
-)
-```
-
-#### Create DBStore object
-
-```python
-from zcrmsdk.src.com.zoho.api.authenticator.store import DBStore
-"""
-DBStore takes the following parameters
-1 -> DataBase host name. Default value "localhost"
-2 -> DataBase name. Default value "zohooauth"
-3 -> DataBase user name. Default value "root"
-4 -> DataBase password. Default value ""
-5 -> DataBase port number. Default value "3306"
-6->  DataBase table name . Default value "oauthtoken"
-"""
-store = DBStore()
-
-store = DBStore(host='host_name', database_name='database_name', user_name='user_name', password='password', port_number='port_number', table_name = "table_name")
-```
-
-### File Persistence
-
-In case of File Persistence, the user can persist tokens in the local drive, by providing the absolute file path to the FileStore object.
-
-- The File contains
-    - id 
-    
-    - user_mail
-
-    - client_id
-    
-    - client_secret
-
-    - refresh_token
-
-    - access_token
-
-    - grant_token
-
-    - expiry_time
-    
-    - redirect_url
-
-#### Create FileStore object
-
-```python
-from zcrmsdk.src.com.zoho.api.authenticator.store import FileStore
-"""
-FileStore takes the following parameter
-1 -> Absolute file path of the file to persist tokens
-"""
-store = FileStore(file_path='/Users/username/Documents/python_sdk_token.txt')
-```
-
-### Custom Persistence
-To use Custom Persistence, you must implement **[TokenStore](zcrmsdk/src/com/zoho/api/authenticator/store/token_store.py)** and override the methods.
-
-```python
-from zcrmsdk.src.com.zoho.api.authenticator.store import TokenStore
-
-
-class CustomStore(TokenStore):
-
-    def __init__(self):
-        pass
-
-    def get_token(self, user, token):
-
-        """
-        Parameters:
-            user (UserSignature) : A UserSignature class instance.
-            token (Token) : A Token (zcrmsdk.src.com.zoho.api.authenticator.OAuthToken) class instance
-        """
-
-        # Add code to get the token
-        return None
-
-    def save_token(self, user, token):
-
-        """
-        Parameters:
-            user (UserSignature) : A UserSignature class instance.
-            token (Token) : A Token (zcrmsdk.src.com.zoho.api.authenticator.OAuthToken) class instance
-        """
-
-        # Add code to save the token
-
-    def delete_token(self, token):
-
-        """
-        Parameters:
-            token (Token) : A Token (zcrmsdk.src.com.zoho.api.authenticator.OAuthToken) class instance
-        """
-
-        # Add code to delete the token
-    
-    def get_tokens(self):
-
-        """
-        Returns:
-            list: List of stored tokens
-        """
-
-        # Add code to get all the stored tokens
-    
-    def delete_tokens(self):
-
-        # Add code to delete all the stored tokens
-    
-    def get_token_by_id(id, token):
+Metadata-Version: 2.1
+Name: zohocrmsdk2_1
+Version: 2.1.0
+Summary: Zoho CRM SDK for ZOHO CRM 2.1 APIs
+Home-page: https://github.com/zoho/zohocrm-python-sdk-2.1
+Author: Zoho CRM API Team
+Author-email: support@zohocrm.com
+License: Apache Software License, Version 2.0, http://www.apache.org/licenses/LICENSE-2.0
+Description: License
+        =======
         
-        """
-        The method to get id token details.
-
-        Parameters:
-            id (String) : A String id.
-            token (Token) : A Token class instance.
-
-        Returns:
-            Token : A Token class instance representing the id token details.
-        """
-```
-
-## Configuration
-
-Before you get started with creating your Python application, you need to register your client and authenticate the app with Zoho.
-
-| Mandatory Keys    | Optional Keys |
-| :---------------- | :------------ |
-| user              | logger        |
-| environment       | store         |
-| token             | sdk_config    |
-|                   | proxy         |
-|                   | resource_path |
-----
-
-- Create an instance of **UserSignature** Class that identifies the current user.
-  ```python
-  from zcrmsdk.src.com.zoho.crm.api.user_signature import UserSignature
-
-  # Create an UserSignature instance that takes user Email as parameter
-  user = UserSignature(email='abc@zoho.com')
-  ```
-
-- Configure the API environment which decides the domain and the URL to make API calls.
-  ```python
-  from zcrmsdk.src.com.zoho.crm.api.dc import USDataCenter
-
-  """
-  Configure the environment
-  which is of the pattern Domain.Environment
-  Available Domains: USDataCenter, EUDataCenter, INDataCenter, CNDataCenter, AUDataCenter
-  Available Environments: PRODUCTION(), DEVELOPER(), SANDBOX()
-  """
-  environment = USDataCenter.PRODUCTION()
-  ```
-
-- Create an instance of **OAuthToken** with the information that you get after registering your Zoho client.
-  ```python
-  from zcrmsdk.src.com.zoho.api.authenticator.oauth_token import OAuthToken
-
-  """
-  Create a Token instance that takes the following parameters
-  1 -> OAuth client id.
-  2 -> OAuth client secret.
-  3 -> Grant token.
-  4 -> Refresh token.
-  5 -> OAuth redirect URL. Default value is None
-  6 -> id
-  7 -> Access token
-  """
-  token = OAuthToken(client_id='clientId', client_secret='clientSecret', grant_token='grant_token', refresh_token="refresh_token", redirect_url='redirectURL', id="id", access_token="access_token")
-  ```
-
-- Create an instance of **Logger** Class to log exception and API information. By default, the SDK constructs a Logger instance with level - INFO and file_path - (sdk_logs.log, created in the current working directory)
-  ```python
-    from zcrmsdk.src.com.zoho.api.logger import Logger
-  
-    """
-    Create an instance of Logger Class that takes two parameters
-    1 -> Level of the log messages to be logged. Can be configured by typing Logger.Levels "." and choose any level from the list displayed.
-    2 -> Absolute file path, where messages need to be logged.
-    """
-    logger = Logger.get_instance(level=Logger.Levels.INFO, file_path="/Users/user_name/Documents/python_sdk_log.log")
-    ```
-
-- Create an instance of **TokenStore** to persist tokens, used for authenticating all the requests. By default, the SDK creates the sdk_tokens.txt created in the current working directory) to persist the tokens.
-  ```python
-  from zcrmsdk.src.com.zoho.api.authenticator.store import DBStore, FileStore
-
-  """
-  DBStore takes the following parameters
-  1 -> DataBase host name. Default value "localhost"
-  2 -> DataBase name. Default value "zohooauth"
-  3 -> DataBase user name. Default value "root"
-  4 -> DataBase password. Default value ""
-  5 -> DataBase port number. Default value "3306"
-  6 -> DataBase table name. Default value "oauthtoken"
-  """
-  store = DBStore()
-
-  #store = DBStore(host='host_name', database_name='database_name', user_name='user_name', password='password', port_number='port_number', table_name = "table_name")
-
-  """
-  FileStore takes the following parameter
-  1 -> Absolute file path of the file to persist tokens
-  """
-  #store = FileStore(file_path='/Users/username/Documents/python_sdk_tokens.txt')
-  ```
-
-- Create an instance of SDKConfig containing SDK configurations.
-  ```python
-  from zcrmsdk.src.com.zoho.crm.api.sdk_config import SDKConfig
-
-  """
-  By default, the SDK creates the SDKConfig instance
-  auto_refresh_fields (Default value is False)
-    if True - all the modules' fields will be auto-refreshed in the background, every hour.
-    if False - the fields will not be auto-refreshed in the background. The user can manually delete the file(s) or refresh the fields using methods from ModuleFieldsHandler(zcrmsdk/src/com/zoho/crm/api/util/module_fields_handler.py)
-
-  pick_list_validation (Default value is True)
-    A boolean field that validates user input for a pick list field and allows or disallows the addition of a new value to the list.
-    if True - the SDK validates the input. If the value does not exist in the pick list, the SDK throws an error.
-    if False - the SDK does not validate the input and makes the API request with the user’s input to the pick list
-  
-  connect_timeout (Default value is None) 
-    A  Float field to set connect timeout
-  
-  read_timeout (Default value is None) 
-    A  Float field to set read timeout
-  """
-  config = SDKConfig(auto_refresh_fields=True, pick_list_validation=False, connect_timeout=None, read_timeout=None)
-  ```
-
-- The path containing the absolute directory path to store user specific files containing module fields information. By default, the SDK stores the user-specific files within a folder in the current working directory.
-  ```python
-  resource_path = '/Users/user_name/Documents/python-app'
-  ```
-
-- Create an instance of RequestProxy containing the proxy properties of the user.
-    ```python
-    from zcrmsdk.src.com.zoho.crm.api.request_proxy import RequestProxy
-
-    """
-    RequestProxy takes the following parameters
-    1 -> Host
-    2 -> Port Number
-    3 -> User Name. Default value is None
-    4 -> Password. Default value is an empty string
-    """
-    request_proxy = RequestProxy(host='proxyHost', port=80)
-    request_proxy = RequestProxy(host='proxyHost', port=80, user='userName', password='password')
-    ```
-
-## Initializing the Application
-
-Initialize the SDK using the following code.
-
-```python
-from zcrmsdk.src.com.zoho.crm.api.user_signature import UserSignature
-from zcrmsdk.src.com.zoho.crm.api.dc import USDataCenter
-from zcrmsdk.src.com.zoho.api.authenticator.store import DBStore, FileStore
-from zcrmsdk.src.com.zoho.api.logger import Logger
-from zcrmsdk.src.com.zoho.crm.api.initializer import Initializer
-from zcrmsdk.src.com.zoho.api.authenticator.oauth_token import OAuthToken
-from zcrmsdk.src.com.zoho.crm.api.sdk_config import SDKConfig
-
-
-class SDKInitializer(object):
-
-    @staticmethod
-    def initialize():
-
-        """
-        Create an instance of Logger Class that takes two parameters
-        1 -> Level of the log messages to be logged. Can be configured by typing Logger.Levels "." and choose any level from the list displayed.
-        2 -> Absolute file path, where messages need to be logged.
-        """
-        logger = Logger.get_instance(level=Logger.Levels.INFO, file_path='/Users/user_name/Documents/python_sdk_log.log')
-
-        # Create an UserSignature instance that takes user Email as parameter
-        user = UserSignature(email='abc@zoho.com')
-
-        """
-        Configure the environment
-        which is of the pattern Domain.Environment
-        Available Domains: USDataCenter, EUDataCenter, INDataCenter, CNDataCenter, AUDataCenter
-        Available Environments: PRODUCTION(), DEVELOPER(), SANDBOX()
-        """
-        environment = USDataCenter.PRODUCTION()
-
-        """
-        Create a Token instance that takes the following parameters
-        1 -> OAuth client id.
-        2 -> OAuth client secret.
-        3 -> Grant token.
-        4 -> Refresh token.
-        5 -> OAuth redirect URL.
-        6 -> id
-        """
-        token = OAuthToken(client_id='clientId', client_secret='clientSecret', grant_token='grant_token', refresh_token="refresh_token", redirect_url='redirectURL', id="id")
-
-        """
-        Create an instance of TokenStore
-        1 -> Absolute file path of the file to persist tokens
-        """
-        store = FileStore(file_path='/Users/username/Documents/python_sdk_tokens.txt')
-
-        """
-        Create an instance of TokenStore
-        1 -> DataBase host name. Default value "localhost"
-        2 -> DataBase name. Default value "zohooauth"
-        3 -> DataBase user name. Default value "root"
-        4 -> DataBase password. Default value ""
-        5 -> DataBase port number. Default value "3306"
-        6->  DataBase table name . Default value "oauthtoken"
-        """
-        store = DBStore()
-        store = DBStore(host='host_name', database_name='database_name', user_name='user_name', password='password',port_number='port_number', table_name = "table_name")
-
-        """
-        auto_refresh_fields (Default value is False)
-            if True - all the modules' fields will be auto-refreshed in the background, every hour.
-            if False - the fields will not be auto-refreshed in the background. The user can manually delete the file(s) or refresh the fields using methods from ModuleFieldsHandler(zcrmsdk/src/com/zoho/crm/api/util/module_fields_handler.py)
-
-        pick_list_validation (Default value is True)
-        A boolean field that validates user input for a pick list field and allows or disallows the addition of a new value to the list.
-            if True - the SDK validates the input. If the value does not exist in the pick list, the SDK throws an error.
-            if False - the SDK does not validate the input and makes the API request with the user’s input to the pick list
-
-        connect_timeout (Default value is None) 
-            A  Float field to set connect timeout
+            Copyright (c) 2021, ZOHO CORPORATION PRIVATE LIMITED 
+            All rights reserved. 
+        
+            Licensed under the Apache License, Version 2.0 (the "License"); 
+            you may not use this file except in compliance with the License. 
+            You may obtain a copy of the License at 
+            
+                http://www.apache.org/licenses/LICENSE-2.0 
+            
+            Unless required by applicable law or agreed to in writing, software 
+            distributed under the License is distributed on an "AS IS" BASIS, 
+            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. 
+            See the License for the specific language governing permissions and 
+            limitations under the License.
+        
+        # ZOHO CRM PYTHON SDK 2.1 for API version 2.1
+        
+        ## Table Of Contents
+        
+        * [Overview](#overview)
+        * [Registering a Zoho Client](#registering-a-zoho-client)
+        * [Environmental Setup](#environmental-setup)
+        * [Including the SDK in your project](#including-the-sdk-in-your-project)
+        * [Persistence](#token-persistence)
+          * [DataBase Persistence](#database-persistence)
+          * [File Persistence](#file-persistence)
+          * [Custom Persistence](#custom-persistence)
+        * [Configuration](#configuration)
+        * [Initialization](#initializing-the-application)
+        * [Class Hierarchy](#class-hierarchy)
+        * [Responses And Exceptions](#responses-and-exceptions)
+        * [Threading](#threading-in-the-python-sdk)
+          * [Multithreading in a Multi-User App](#multithreading-in-a-multi-user-app)
+          * [Multi-threading in a Single User App](#multi-threading-in-a-single-user-app)
+        * [Sample Code](#sdk-sample-code)
+        ## Overview
+        
+        Zoho CRM PYTHON SDK offers a way to create client Python applications that can be integrated with Zoho CRM.
+        
+        ## Registering a Zoho Client
+        
+        Since Zoho CRM APIs are authenticated with OAuth2 standards, you should register your client app with Zoho. To register your app:
+        
+        - Visit this page [https://api-console.zoho.com](https://api-console.zoho.com)
+        
+        - Click on `ADD CLIENT`.
+        
+        - Choose the `Client Type`.
+        
+        - Enter **Client Name**, **Client Domain** or **Homepage URL** and **Authorized Redirect URIs** then click `CREATE`.
+        
+        - Your Client app will be created.
+        
+        - Select the created OAuth client.
+        
+        - Generate grant token by providing the necessary scopes, time duration (the duration for which the generated token is valid) and Scope Description.
+        
+        ## Environmental Setup
+        
+        Python SDK is installable through **pip**. **pip** is a tool for dependency management in Python. SDK expects the following from the client app.
+        
+        - Client app must have Python(version 3 and above)
+        
+        - Python SDK must be installed into client app through **pip**.
+        
+        ## Including the SDK in your project
+        
+        - Install **Python** from [python.org](https://www.python.org/downloads/) (if not installed).
+        
+        - Install **Python SDK**
+            - Navigate to the workspace of your client app.
+            - Run the command below:
+        
+            ```sh
+            pip install zohocrmsdk2_1==1.x.x
+            ```
+        - The Python SDK will be installed in your client application.
+        
+        ## Token Persistence
+        
+        Token persistence refers to storing and utilizing the authentication tokens that are provided by Zoho. There are three ways provided by the SDK in which persistence can be utilized. They are DataBase Persistence, File Persistence and Custom Persistence.
+        
+        ### Table of Contents
+        
+        - [DataBase Persistence](#database-persistence)
+        
+        - [File Persistence](#file-persistence)
+        
+        - [Custom Persistence](#custom-persistence)
+        
+        ### Implementing OAuth Persistence
+        
+        Once the application is authorized, OAuth access and refresh tokens can be used for subsequent user data requests to Zoho CRM. Hence, they need to be persisted by the client app.
+        
+        The persistence is achieved by writing an implementation of the inbuilt Abstract Base Class **[TokenStore](zcrmsdk/src/com/zoho/api/authenticator/store/token_store.py)**, which has the following callback methods.
+        
+        - **get_token(self, user, [token](zcrmsdk/src/com/zoho/api/authenticator/token.py))** - invoked before firing a request to fetch the saved tokens. This method should return implementation of inbuilt **Token Class** object for the library to process it.
+        
+        - **save_token(self, user, [token](zcrmsdk/src/com/zoho/api/authenticator/token.py))** - invoked after fetching access and refresh tokens from Zoho.
+        
+        - **delete_token(self, [token](zcrmsdk/src/com/zoho/api/authenticator/token.py))** - invoked before saving the latest tokens.
+        
+        - **get_tokens(self)** - The method to get the all the stored tokens.
+        
+        - **delete_tokens(self)** - The method to delete all the stored tokens.
+        
+        - **get_token_by_id(self, id, token)** - The method to retrieve the user's token details based on unique ID.
+        
+        Note:
+        
+        - user is an instance of UserSignature Class.
+        
+        - token is an instance of Token Class.
+        
+        ### DataBase Persistence
+        
+        In case the user prefers to use default DataBase persistence, **MySQL** can be used.
+        
+        - The database name should be **zohooauth**.
+        
+        - There must be a table name **oauthtoken** with the following columns.
+        
+          - id int(11)
+        
+          - user_mail varchar(255)
           
-        read_timeout (Default value is None) 
-            A  Float field to set read timeout
-        """
-        config = SDKConfig(auto_refresh_fields=True, pick_list_validation=False, connect_timeout=None, read_timeout=None)
-
-        """
-        The path containing the absolute directory path (in the key resource_path) to store user-specific files containing information about fields in modules. 
-        """
-        resource_path = '/Users/user_name/Documents/python-app'
-
-        """
-        Create an instance of RequestProxy class that takes the following parameters
-        1 -> Host
-        2 -> Port Number
-        3 -> User Name. Default value is None
-        4 -> Password. Default value is None
-        """
-        request_proxy = RequestProxy(host='host', port=8080)
-
-        request_proxy = RequestProxy(host='host', port=8080, user='user', password='password')
-
-        """
-        Call the static initialize method of Initializer class that takes the following arguments
-        1 -> UserSignature instance
-        2 -> Environment instance
-        3 -> Token instance
-        4 -> TokenStore instance
-        5 -> SDKConfig instance
-        6 -> resource_path
-        7 -> Logger instance. Default value is None
-        8 -> RequestProxy instance. Default value is None
-        """
-        Initializer.initialize(user=user, environment=environment, token=token, store=store, sdk_config=config, resource_path=resource_path, logger=logger, proxy=request_proxy)
-
-
-SDKInitializer.initialize()
-
-```
-
-- You can now access the functionalities of the SDK. Refer to the sample codes to make various API calls through the SDK.
-
-## Class Hierarchy
-
-![classdiagram](class_hierarchy.png)
-
-## Responses and Exceptions
-
-All SDK methods return an instance of the APIResponse class.
-
-After a successful API request, the **get_object()** method returns an instance of the **ResponseWrapper** (for **GET**) or the **ActionWrapper** (for **POST, PUT, DELETE**)
-
-Whenever the API returns an error response, the **get_object()** returns an instance of **APIException** class.
-
-**ResponseWrapper** (for **GET** requests) and **ActionWrapper** (for **POST, PUT, DELETE** requests) are the expected objects for Zoho CRM APIs’ responses
-
-However, some specific operations have different expected objects, such as the following:
-
-- Operations involving records in Tags
-    - **RecordActionWrapper**
-
-- Getting Record Count for a specific Tag operation
-    - **CountWrapper**
-
-- Operations involving BaseCurrency
-    - **BaseCurrencyActionWrapper**
-
-- Lead convert operation
-    - **ConvertActionWrapper**
-
-- Retrieving Deleted records operation
-    - **DeletedRecordsWrapper**
-
-- Record image download operation
-    - **FileBodyWrapper**
-
-- MassUpdate record operations
-    - **MassUpdateActionWrapper**
-    - **MassUpdateResponseWrapper**
-  
-### GET Requests
-
-- The **get_object()** returns an instance of one of the following classes, based on the return type.
-
-    - For  **application/json** responses
-        - **ResponseWrapper**
-        - **CountWrapper**
-        - **DeletedRecordsWrapper**
-        - **MassUpdateResponseWrapper**
-        - **APIException**
-
-    - For **file download** responses
-        - **FileBodyWrapper**
-        - **APIException**
-
-### POST, PUT, DELETE Requests
-
-- The **getObject()** returns an instance of one of the following classes
-    - **ActionWrapper**
-    - **RecordActionWrapper**
-    - **BaseCurrencyActionWrapper**
-    - **MassUpdateActionWrapper**
-    - **ConvertActionWrapper**
-    - **APIException**
-
-- These wrapper classes may contain one or a list of instances of the following classes, depending on the response.
-    - **SuccessResponse Class**, if the request was successful.
-    - **APIException Class**, if the request was erroneous.
-
-For example, when you insert two records, and one of them was inserted successfully while the other one failed, the ActionWrapper will contain one instance each of the SuccessResponse and APIException classes.
-
-All other exceptions such as SDK anomalies and other unexpected behaviours are thrown under the SDKException class.
-
-## Threading in the Python SDK
-
-Threads in a Python program help you achieve parallelism. By using multiple threads, you can make a Python program run faster and do multiple things simultaneously.
-
-The **Python SDK** (from version 3.x.x) supports both single-user and multi-user app.
-
-### Multithreading in a Multi-user App
-
-Multi-threading for multi-users is achieved using Initializer's static **switch_user()** method.
-switch_user() takes the value initialized previously for user, enviroment, token and sdk_config incase None is passed (or default value is passed). In case of request_proxy, if intended, the value has to be passed again else None(default value) will be taken.
-
-```python
-# without proxy
-Initializer.switch_user(user=user, environment=environment, token=token, sdk_config=sdk_config_instance)
-
-# with proxy
-Initializer.switch_user(user=user, environment=environment, token=token, sdk_config=sdk_config_instance, proxy=request_proxy)
-```
-
-Here is a sample code to depict multi-threading for a multi-user app.
-
-```python
-import threading
-from zcrmsdk.src.com.zoho.crm.api.user_signature import UserSignature
-from zcrmsdk.src.com.zoho.crm.api.dc import USDataCenter, EUDataCenter
-from zcrmsdk.src.com.zoho.api.authenticator.store import DBStore
-from zcrmsdk.src.com.zoho.api.logger import Logger
-from zcrmsdk.src.com.zoho.crm.api.initializer import Initializer
-from zcrmsdk.src.com.zoho.api.authenticator.oauth_token import OAuthToken
-from zcrmsdk.src.com.zoho.crm.api.record import *
-from zcrmsdk.src.com.zoho.crm.api.request_proxy import RequestProxy
-from zcrmsdk.src.com.zoho.crm.api.sdk_config import SDKConfig
-
-
-class MultiThread(threading.Thread):
-
-    def __init__(self, environment, token, user, module_api_name, sdk_config, proxy=None):
-        super().__init__()
-        self.environment = environment
-        self.token = token
-        self.user = user
-        self.module_api_name = module_api_name
-        self.sdk_config = sdk_config
-        self.proxy = proxy
-
-    def run(self):
-        try:
-            Initializer.switch_user(user=self.user, environment=self.environment, token=self.token, sdk_config=self.sdk_config, proxy=self.proxy)
-
-            print('Getting records for User: ' + Initializer.get_initializer().user.get_email())
-
-            response = RecordOperations().get_records(self.module_api_name)
-
-            if response is not None:
-
-                # Get the status code from response
-                print('Status Code: ' + str(response.get_status_code()))
-
-                if response.get_status_code() in [204, 304]:
-                    print('No Content' if response.get_status_code() == 204 else 'Not Modified')
-                    return
-
-                # Get object from response
-                response_object = response.get_object()
-
-                if response_object is not None:
-
-                    # Check if expected ResponseWrapper instance is received.
-                    if isinstance(response_object, ResponseWrapper):
-                        # Get the list of obtained Record instances
-                        record_list = response_object.get_data()
-
-                        for record in record_list:
-                            for key, value in record.get_key_values().items():
-                                print(key + " : " + str(value))
-
-                    # Check if the request returned an exception
-                    elif isinstance(response_object, APIException):
-                        # Get the Status
-                        print("Status: " + response_object.get_status().get_value())
-
-                        # Get the Code
-                        print("Code: " + response_object.get_code().get_value())
-
-                        print("Details")
-
-                        # Get the details dict
-                        details = response_object.get_details()
-
-                        for key, value in details.items():
-                            print(key + ' : ' + str(value))
-
-                        # Get the Message
-                        print("Message: " + response_object.get_message().get_value())
-
-        except Exception as e:
-            print(e)
-
-    @staticmethod
-    def call():
-        logger = Logger.get_instance(level=Logger.Levels.INFO, file_path="/Users/user_name/Documents/python_sdk_log.log")
-
-        user1 = UserSignature(email="abc@zoho.com")
-
-        token1 = OAuthToken(client_id="clientId1", client_secret="clientSecret1", grant_token="Grant Token", refresh_token="refresh_token", id="id")
-
-        environment1 = USDataCenter.PRODUCTION()
-
-        store = DBStore()
-
-        sdk_config_1 = SDKConfig(auto_refresh_fields=True, pick_list_validation=False)
-
-        resource_path = '/Users/user_name/Documents/python-app'
-
-        user1_module_api_name = 'Leads'
-
-        user2_module_api_name = 'Contacts'
-
-        environment2 = EUDataCenter.SANDBOX()
-
-        user2 = UserSignature(email="abc@zoho.eu")
-
-        sdk_config_2 = SDKConfig(auto_refresh_fields=False, pick_list_validation=True)
-
-        token2 = OAuthToken(client_id="clientId2", client_secret="clientSecret2",grant_token="GRANT Token", refresh_token="refresh_token", redirect_url="redirectURL", id="id")
-
-        request_proxy_user_2 = RequestProxy("host", 8080)
-
-        Initializer.initialize(user=user1, environment=environment1, token=token1, store=store, sdk_config=sdk_config_1, resource_path=resource_path, logger=logger)
-
-        t1 = MultiThread(environment1, token1, user1, user1_module_api_name, sdk_config_1)
-        t2 = MultiThread(environment2, token2, user2, user2_module_api_name, sdk_config_2, request_proxy_user_2)
-
-        t1.start()
-        t2.start()
-
-        t1.join()
-        t2.join()
-
-
-MultiThread.call()
-
-```
-
-- The program execution starts from **call()**.
-
-- The details of **user1** are given in the variables user1, token1, environment1.
-
-- Similarly, the details of another user **user2** are given in the variables user2, token2, environment2.
-
-- For each user, an instance of **MultiThread class** is created.
-
-- When the **start()** is called which in-turn invokes the **run()**,  the details of user1 are passed to the **switch_user** method through the **MultiThread object**. Therefore, this creates a thread for user1.
-
-- Similarly, When the **start()** is invoked again,  the details of user2 are passed to the **switch_user** function through the **MultiThread object**. Therefore, this creates a thread for user2.
-
-### Multi-threading in a Single User App
-
-Here is a sample code to depict multi-threading for a single-user app.
-
-```python
-import threading
-from zcrmsdk.src.com.zoho.crm.api.user_signature import UserSignature
-from zcrmsdk.src.com.zoho.crm.api.dc import USDataCenter
-from zcrmsdk.src.com.zoho.api.authenticator.store import DBStore
-from zcrmsdk.src.com.zoho.api.logger import Logger
-from zcrmsdk.src.com.zoho.crm.api.initializer import Initializer
-from zcrmsdk.src.com.zoho.api.authenticator.oauth_token import OAuthToken
-from zcrmsdk.src.com.zoho.crm.api.sdk_config import SDKConfig
-from zcrmsdk.src.com.zoho.crm.api.record import *
-
-
-class MultiThread(threading.Thread):
-
-    def __init__(self, module_api_name):
-        super().__init__()
-        self.module_api_name = module_api_name
-
-    def run(self):
-        try:
-            print("Calling Get Records for module: " + self.module_api_name)
-
-            response = RecordOperations().get_records(self.module_api_name)
-
-            if response is not None:
-
-                # Get the status code from response
-                print('Status Code: ' + str(response.get_status_code()))
-
-                if response.get_status_code() in [204, 304]:
-                    print('No Content' if response.get_status_code() == 204 else 'Not Modified')
-                    return
-
-                # Get object from response
-                response_object = response.get_object()
-
-                if response_object is not None:
-
-                    # Check if expected ResponseWrapper instance is received.
-                    if isinstance(response_object, ResponseWrapper):
-                        # Get the list of obtained Record instances
-                        record_list = response_object.get_data()
-
-                        for record in record_list:
-                            for key, value in record.get_key_values().items():
-                                print(key + " : " + str(value))
-
-                    # Check if the request returned an exception
-                    elif isinstance(response_object, APIException):
-                        # Get the Status
-                        print("Status: " + response_object.get_status().get_value())
-
-                        # Get the Code
-                        print("Code: " + response_object.get_code().get_value())
-
-                        print("Details")
-
-                        # Get the details dict
-                        details = response_object.get_details()
-
-                        for key, value in details.items():
-                            print(key + ' : ' + str(value))
-
-                        # Get the Message
-                        print("Message: " + response_object.get_message().get_value())
-
-        except Exception as e:
-            print(e)
-
-    @staticmethod
-    def call():
-        logger = Logger.get_instance(level=Logger.Levels.INFO, file_path="/Users/user_name/Documents/python_sdk_log.log")
-
-        user = UserSignature(email="abc@zoho.com")
-
-        token = OAuthToken(client_id="clientId", client_secret="clientSecret", grant_token="grant_token", refresh_token="refresh_token", redirect_url="redirectURL", id="id")
-
-        environment = USDataCenter.PRODUCTION()
-
-        store = DBStore()
-
-        sdk_config = SDKConfig()
-
-        resource_path = '/Users/user_name/Documents/python-app'
-
-        Initializer.initialize(user=user, environment=environment, token=token, store=store, sdk_config=sdk_config, resource_path=resource_path, logger=logger)
-
-        t1 = MultiThread('Leads')
-        t2 = MultiThread('Quotes')
-
-        t1.start()
-        t2.start()
-
-        t1.join()
-        t2.join()
-
-
-MultiThread.call()
-```
-
-- The program execution starts from **call()** where the SDK is initialized with the details of the user.
-
-- When the **start()** is called which in-turn invokes the run(),  the module_api_name is switched through the MultiThread object. Therefore, this creates a thread for the particular MultiThread instance.
-
-## SDK Sample code
-
-```python
-from datetime import datetime
-from zcrmsdk.src.com.zoho.crm.api.user_signature import UserSignature
-from zcrmsdk.src.com.zoho.crm.api.dc import USDataCenter
-from zcrmsdk.src.com.zoho.api.authenticator.store import DBStore
-from zcrmsdk.src.com.zoho.api.logger import Logger
-from zcrmsdk.src.com.zoho.crm.api.initializer import Initializer
-from zcrmsdk.src.com.zoho.api.authenticator.oauth_token import OAuthToken
-from zcrmsdk.src.com.zoho.crm.api.record import *
-from zcrmsdk.src.com.zoho.crm.api import HeaderMap, ParameterMap
-from zcrmsdk.src.com.zoho.crm.api.sdk_config import SDKConfig
-
-
-class Record(object):
-
-    def __init__(self):
-        pass
-
-    @staticmethod
-    def get_records():
-
-        """
-        Create an instance of Logger Class that takes two parameters
-        1 -> Level of the log messages to be logged. Can be configured by typing Logger.Levels "." and choose any level from the list displayed.
-        2 -> Absolute file path, where messages need to be logged.
-        """
-        logger = Logger.get_instance(level=Logger.Levels.INFO,
-                                     file_path="/Users/user_name/Documents/python_sdk_log.log")
-
-        # Create an UserSignature instance that takes user Email as parameter
-        user = UserSignature(email="abc@zoho.com")
-
-        """
-        Configure the environment
-        which is of the pattern Domain.Environment
-        Available Domains: USDataCenter, EUDataCenter, INDataCenter, CNDataCenter, AUDataCenter
-        Available Environments: PRODUCTION(), DEVELOPER(), SANDBOX()
-        """
-        environment = USDataCenter.PRODUCTION()
-
-        """
-        Create a Token instance that takes the following parameters
-        1 -> OAuth client id.
-        2 -> OAuth client secret.
-        3 -> Grant token.
-        4 -> Refresh token.
-        5 -> OAuth redirect URL.
-        6 -> id
-        """
-        token = OAuthToken(client_id="clientId", client_secret="clientSecret", grant_token="grant_token", refresh_token="refresh_token", redirect_url="redirectURL", id="id")
-
+          - client_id varchar(255)
+          
+          - client_secret varchar(255)
+        
+          - refresh_token varchar(255)
+        
+          - access_token varchar(255)
+        
+          - grant_token varchar(255)
+        
+          - expiry_time varchar(20)
+          
+          - redirect_url varchar(255)
+        
+        Note:
+        - Custom database name and table name can be set in DBStore instance.
+        
+        #### MySQL Query
+        
+        ```sql
+        CREATE TABLE  oauthtoken (
+          id varchar(255) NOT NULL,
+          user_mail varchar(255) NOT NULL,
+          client_id varchar(255),
+          client_secret varchar(255),
+          refresh_token varchar(255),
+          access_token varchar(255),
+          grant_token varchar(255),
+          expiry_time varchar(20),
+          redirect_url varchar(255),
+          primary key (id)
+        )
+        ```
+        
+        #### Create DBStore object
+        
+        ```python
+        from zcrmsdk.src.com.zoho.api.authenticator.store import DBStore
         """
-        Create an instance of TokenStore
+        DBStore takes the following parameters
         1 -> DataBase host name. Default value "localhost"
         2 -> DataBase name. Default value "zohooauth"
         3 -> DataBase user name. Default value "root"
         4 -> DataBase password. Default value ""
         5 -> DataBase port number. Default value "3306"
         6->  DataBase table name . Default value "oauthtoken"
         """
         store = DBStore()
-
+        
+        store = DBStore(host='host_name', database_name='database_name', user_name='user_name', password='password', port_number='port_number', table_name = "table_name")
+        ```
+        
+        ### File Persistence
+        
+        In case of File Persistence, the user can persist tokens in the local drive, by providing the absolute file path to the FileStore object.
+        
+        - The File contains
+            - id 
+            
+            - user_mail
+        
+            - client_id
+            
+            - client_secret
+        
+            - refresh_token
+        
+            - access_token
+        
+            - grant_token
+        
+            - expiry_time
+            
+            - redirect_url
+        
+        #### Create FileStore object
+        
+        ```python
+        from zcrmsdk.src.com.zoho.api.authenticator.store import FileStore
+        """
+        FileStore takes the following parameter
+        1 -> Absolute file path of the file to persist tokens
         """
-        auto_refresh_fields (Default value is False)
+        store = FileStore(file_path='/Users/username/Documents/python_sdk_token.txt')
+        ```
+        
+        ### Custom Persistence
+        To use Custom Persistence, you must implement **[TokenStore](zcrmsdk/src/com/zoho/api/authenticator/store/token_store.py)** and override the methods.
+        
+        ```python
+        from zcrmsdk.src.com.zoho.api.authenticator.store import TokenStore
+        
+        
+        class CustomStore(TokenStore):
+        
+            def __init__(self):
+                pass
+        
+            def get_token(self, user, token):
+        
+                """
+                Parameters:
+                    user (UserSignature) : A UserSignature class instance.
+                    token (Token) : A Token (zcrmsdk.src.com.zoho.api.authenticator.OAuthToken) class instance
+                """
+        
+                # Add code to get the token
+                return None
+        
+            def save_token(self, user, token):
+        
+                """
+                Parameters:
+                    user (UserSignature) : A UserSignature class instance.
+                    token (Token) : A Token (zcrmsdk.src.com.zoho.api.authenticator.OAuthToken) class instance
+                """
+        
+                # Add code to save the token
+        
+            def delete_token(self, token):
+        
+                """
+                Parameters:
+                    token (Token) : A Token (zcrmsdk.src.com.zoho.api.authenticator.OAuthToken) class instance
+                """
+        
+                # Add code to delete the token
+            
+            def get_tokens(self):
+        
+                """
+                Returns:
+                    list: List of stored tokens
+                """
+        
+                # Add code to get all the stored tokens
+            
+            def delete_tokens(self):
+        
+                # Add code to delete all the stored tokens
+            
+            def get_token_by_id(id, token):
+                
+                """
+                The method to get id token details.
+        
+                Parameters:
+                    id (String) : A String id.
+                    token (Token) : A Token class instance.
+        
+                Returns:
+                    Token : A Token class instance representing the id token details.
+                """
+        ```
+        
+        ## Configuration
+        
+        Before you get started with creating your Python application, you need to register your client and authenticate the app with Zoho.
+        
+        | Mandatory Keys    | Optional Keys |
+        | :---------------- | :------------ |
+        | user              | logger        |
+        | environment       | store         |
+        | token             | sdk_config    |
+        |                   | proxy         |
+        |                   | resource_path |
+        ----
+        
+        - Create an instance of **UserSignature** Class that identifies the current user.
+          ```python
+          from zcrmsdk.src.com.zoho.crm.api.user_signature import UserSignature
+        
+          # Create an UserSignature instance that takes user Email as parameter
+          user = UserSignature(email='abc@zoho.com')
+          ```
+        
+        - Configure the API environment which decides the domain and the URL to make API calls.
+          ```python
+          from zcrmsdk.src.com.zoho.crm.api.dc import USDataCenter
+        
+          """
+          Configure the environment
+          which is of the pattern Domain.Environment
+          Available Domains: USDataCenter, EUDataCenter, INDataCenter, CNDataCenter, AUDataCenter
+          Available Environments: PRODUCTION(), DEVELOPER(), SANDBOX()
+          """
+          environment = USDataCenter.PRODUCTION()
+          ```
+        
+        - Create an instance of **OAuthToken** with the information that you get after registering your Zoho client.
+          ```python
+          from zcrmsdk.src.com.zoho.api.authenticator.oauth_token import OAuthToken
+        
+          """
+          Create a Token instance that takes the following parameters
+          1 -> OAuth client id.
+          2 -> OAuth client secret.
+          3 -> Grant token.
+          4 -> Refresh token.
+          5 -> OAuth redirect URL. Default value is None
+          6 -> id
+          7 -> Access token
+          """
+          token = OAuthToken(client_id='clientId', client_secret='clientSecret', grant_token='grant_token', refresh_token="refresh_token", redirect_url='redirectURL', id="id", access_token="access_token")
+          ```
+        
+        - Create an instance of **Logger** Class to log exception and API information. By default, the SDK constructs a Logger instance with level - INFO and file_path - (sdk_logs.log, created in the current working directory)
+          ```python
+            from zcrmsdk.src.com.zoho.api.logger import Logger
+          
+            """
+            Create an instance of Logger Class that takes two parameters
+            1 -> Level of the log messages to be logged. Can be configured by typing Logger.Levels "." and choose any level from the list displayed.
+            2 -> Absolute file path, where messages need to be logged.
+            """
+            logger = Logger.get_instance(level=Logger.Levels.INFO, file_path="/Users/user_name/Documents/python_sdk_log.log")
+            ```
+        
+        - Create an instance of **TokenStore** to persist tokens, used for authenticating all the requests. By default, the SDK creates the sdk_tokens.txt created in the current working directory) to persist the tokens.
+          ```python
+          from zcrmsdk.src.com.zoho.api.authenticator.store import DBStore, FileStore
+        
+          """
+          DBStore takes the following parameters
+          1 -> DataBase host name. Default value "localhost"
+          2 -> DataBase name. Default value "zohooauth"
+          3 -> DataBase user name. Default value "root"
+          4 -> DataBase password. Default value ""
+          5 -> DataBase port number. Default value "3306"
+          6 -> DataBase table name. Default value "oauthtoken"
+          """
+          store = DBStore()
+        
+          #store = DBStore(host='host_name', database_name='database_name', user_name='user_name', password='password', port_number='port_number', table_name = "table_name")
+        
+          """
+          FileStore takes the following parameter
+          1 -> Absolute file path of the file to persist tokens
+          """
+          #store = FileStore(file_path='/Users/username/Documents/python_sdk_tokens.txt')
+          ```
+        
+        - Create an instance of SDKConfig containing SDK configurations.
+          ```python
+          from zcrmsdk.src.com.zoho.crm.api.sdk_config import SDKConfig
+        
+          """
+          By default, the SDK creates the SDKConfig instance
+          auto_refresh_fields (Default value is False)
             if True - all the modules' fields will be auto-refreshed in the background, every hour.
             if False - the fields will not be auto-refreshed in the background. The user can manually delete the file(s) or refresh the fields using methods from ModuleFieldsHandler(zcrmsdk/src/com/zoho/crm/api/util/module_fields_handler.py)
-
-        pick_list_validation (Default value is True)
+        
+          pick_list_validation (Default value is True)
             A boolean field that validates user input for a pick list field and allows or disallows the addition of a new value to the list.
             if True - the SDK validates the input. If the value does not exist in the pick list, the SDK throws an error.
             if False - the SDK does not validate the input and makes the API request with the user’s input to the pick list
-         connect_timeout (Default value is None) 
+          
+          connect_timeout (Default value is None) 
             A  Float field to set connect timeout
-  
-         read_timeout (Default value is None) 
+          
+          read_timeout (Default value is None) 
             A  Float field to set read timeout
-         """
-        config = SDKConfig(auto_refresh_fields=True, pick_list_validation=False, connect_timeout=None, read_timeout=None)
-
-        """
-        The path containing the absolute directory path (in the key resource_path) to store user-specific files containing information about fields in modules. 
-        """
-        resource_path = '/Users/user_name/Documents/python-app'
-
-        """
-        Call the static initialize method of Initializer class that takes the following arguments
-        1 -> UserSignature instance
-        2 -> Environment instance
-        3 -> Token instance
-        4 -> TokenStore instance
-        5 -> SDKConfig instance
-        6 -> resource_path
-        7 -> Logger instance
-        """
-        Initializer.initialize(user=user, environment=environment, token=token, store=store, sdk_config=config, resource_path=resource_path, logger=logger)
-
-        try:
-            module_api_name = 'Leads'
-
-            param_instance = ParameterMap()
-
-            param_instance.add(GetRecordsParam.converted, 'both')
-
-            param_instance.add(GetRecordsParam.cvid, '12712717217218')
-
-            header_instance = HeaderMap()
-
-            header_instance.add(GetRecordsHeader.if_modified_since, datetime.now())
-
-            response = RecordOperations().get_records(module_api_name, param_instance, header_instance)
-
-            if response is not None:
-
-                # Get the status code from response
-                print('Status Code: ' + str(response.get_status_code()))
-
-                if response.get_status_code() in [204, 304]:
-                    print('No Content' if response.get_status_code() == 204 else 'Not Modified')
-                    return
-
-                # Get object from response
-                response_object = response.get_object()
-
-                if response_object is not None:
-
-                    # Check if expected ResponseWrapper instance is received.
-                    if isinstance(response_object, ResponseWrapper):
-                        # Get the list of obtained Record instances
-                        record_list = response_object.get_data()
-
-                        for record in record_list:
-
-                            # Get the ID of each Record
-                            print("Record ID: " + record.get_id())
-
-                            # Get the createdBy User instance of each Record
-                            created_by = record.get_created_by()
-
-                            # Check if created_by is not None
-                            if created_by is not None:
-                                # Get the Name of the created_by User
-                                print("Record Created By - Name: " + created_by.get_name())
-
-                                # Get the ID of the created_by User
-                                print("Record Created By - ID: " + created_by.get_id())
-
-                                # Get the Email of the created_by User
-                                print("Record Created By - Email: " + created_by.get_email())
-
-                            # Get the CreatedTime of each Record
-                            print("Record CreatedTime: " + str(record.get_created_time()))
-
-                            if record.get_modified_time() is not None:
-                                # Get the ModifiedTime of each Record
-                                print("Record ModifiedTime: " + str(record.get_modified_time()))
-
-                            # Get the modified_by User instance of each Record
-                            modified_by = record.get_modified_by()
-
-                            # Check if modified_by is not None
-                            if modified_by is not None:
-                                # Get the Name of the modified_by User
-                                print("Record Modified By - Name: " + modified_by.get_name())
-
-                                # Get the ID of the modified_by User
-                                print("Record Modified By - ID: " + modified_by.get_id())
-
-                                # Get the Email of the modified_by User
-                                print("Record Modified By - Email: " + modified_by.get_email())
-
-                            # Get the list of obtained Tag instance of each Record
-                            tags = record.get_tag()
-
-                            if tags is not None:
-                                for tag in tags:
-                                    # Get the Name of each Tag
-                                    print("Record Tag Name: " + tag.get_name())
-
-                                    # Get the Id of each Tag
-                                    print("Record Tag ID: " + tag.get_id())
-
-                            # To get particular field value
-                            print("Record Field Value: " + str(record.get_key_value('Last_Name')))
-
-                            print('Record KeyValues: ')
-
-                            for key, value in record.get_key_values().items():
-                                print(key + " : " + str(value))
-
-                    # Check if the request returned an exception
-                    elif isinstance(response_object, APIException):
-                        # Get the Status
-                        print("Status: " + response_object.get_status().get_value())
-
-                        # Get the Code
-                        print("Code: " + response_object.get_code().get_value())
-
-                        print("Details")
-
-                        # Get the details dict
-                        details = response_object.get_details()
-
-                        for key, value in details.items():
-                            print(key + ' : ' + str(value))
-
-                        # Get the Message
-                        print("Message: " + response_object.get_message().get_value())
-
-        except Exception as e:
-            print(e)
-
-
-Record.get_records()
-```
+          """
+          config = SDKConfig(auto_refresh_fields=True, pick_list_validation=False, connect_timeout=None, read_timeout=None)
+          ```
+        
+        - The path containing the absolute directory path to store user specific files containing module fields information. By default, the SDK stores the user-specific files within a folder in the current working directory.
+          ```python
+          resource_path = '/Users/user_name/Documents/python-app'
+          ```
+        
+        - Create an instance of RequestProxy containing the proxy properties of the user.
+            ```python
+            from zcrmsdk.src.com.zoho.crm.api.request_proxy import RequestProxy
+        
+            """
+            RequestProxy takes the following parameters
+            1 -> Host
+            2 -> Port Number
+            3 -> User Name. Default value is None
+            4 -> Password. Default value is an empty string
+            """
+            request_proxy = RequestProxy(host='proxyHost', port=80)
+            request_proxy = RequestProxy(host='proxyHost', port=80, user='userName', password='password')
+            ```
+        
+        ## Initializing the Application
+        
+        Initialize the SDK using the following code.
+        
+        ```python
+        from zcrmsdk.src.com.zoho.crm.api.user_signature import UserSignature
+        from zcrmsdk.src.com.zoho.crm.api.dc import USDataCenter
+        from zcrmsdk.src.com.zoho.api.authenticator.store import DBStore, FileStore
+        from zcrmsdk.src.com.zoho.api.logger import Logger
+        from zcrmsdk.src.com.zoho.crm.api.initializer import Initializer
+        from zcrmsdk.src.com.zoho.api.authenticator.oauth_token import OAuthToken
+        from zcrmsdk.src.com.zoho.crm.api.sdk_config import SDKConfig
+        
+        
+        class SDKInitializer(object):
+        
+            @staticmethod
+            def initialize():
+        
+                """
+                Create an instance of Logger Class that takes two parameters
+                1 -> Level of the log messages to be logged. Can be configured by typing Logger.Levels "." and choose any level from the list displayed.
+                2 -> Absolute file path, where messages need to be logged.
+                """
+                logger = Logger.get_instance(level=Logger.Levels.INFO, file_path='/Users/user_name/Documents/python_sdk_log.log')
+        
+                # Create an UserSignature instance that takes user Email as parameter
+                user = UserSignature(email='abc@zoho.com')
+        
+                """
+                Configure the environment
+                which is of the pattern Domain.Environment
+                Available Domains: USDataCenter, EUDataCenter, INDataCenter, CNDataCenter, AUDataCenter
+                Available Environments: PRODUCTION(), DEVELOPER(), SANDBOX()
+                """
+                environment = USDataCenter.PRODUCTION()
+        
+                """
+                Create a Token instance that takes the following parameters
+                1 -> OAuth client id.
+                2 -> OAuth client secret.
+                3 -> Grant token.
+                4 -> Refresh token.
+                5 -> OAuth redirect URL.
+                6 -> id
+                """
+                token = OAuthToken(client_id='clientId', client_secret='clientSecret', grant_token='grant_token', refresh_token="refresh_token", redirect_url='redirectURL', id="id")
+        
+                """
+                Create an instance of TokenStore
+                1 -> Absolute file path of the file to persist tokens
+                """
+                store = FileStore(file_path='/Users/username/Documents/python_sdk_tokens.txt')
+        
+                """
+                Create an instance of TokenStore
+                1 -> DataBase host name. Default value "localhost"
+                2 -> DataBase name. Default value "zohooauth"
+                3 -> DataBase user name. Default value "root"
+                4 -> DataBase password. Default value ""
+                5 -> DataBase port number. Default value "3306"
+                6->  DataBase table name . Default value "oauthtoken"
+                """
+                store = DBStore()
+                store = DBStore(host='host_name', database_name='database_name', user_name='user_name', password='password',port_number='port_number', table_name = "table_name")
+        
+                """
+                auto_refresh_fields (Default value is False)
+                    if True - all the modules' fields will be auto-refreshed in the background, every hour.
+                    if False - the fields will not be auto-refreshed in the background. The user can manually delete the file(s) or refresh the fields using methods from ModuleFieldsHandler(zcrmsdk/src/com/zoho/crm/api/util/module_fields_handler.py)
+        
+                pick_list_validation (Default value is True)
+                A boolean field that validates user input for a pick list field and allows or disallows the addition of a new value to the list.
+                    if True - the SDK validates the input. If the value does not exist in the pick list, the SDK throws an error.
+                    if False - the SDK does not validate the input and makes the API request with the user’s input to the pick list
+        
+                connect_timeout (Default value is None) 
+                    A  Float field to set connect timeout
+                  
+                read_timeout (Default value is None) 
+                    A  Float field to set read timeout
+                """
+                config = SDKConfig(auto_refresh_fields=True, pick_list_validation=False, connect_timeout=None, read_timeout=None)
+        
+                """
+                The path containing the absolute directory path (in the key resource_path) to store user-specific files containing information about fields in modules. 
+                """
+                resource_path = '/Users/user_name/Documents/python-app'
+        
+                """
+                Create an instance of RequestProxy class that takes the following parameters
+                1 -> Host
+                2 -> Port Number
+                3 -> User Name. Default value is None
+                4 -> Password. Default value is None
+                """
+                request_proxy = RequestProxy(host='host', port=8080)
+        
+                request_proxy = RequestProxy(host='host', port=8080, user='user', password='password')
+        
+                """
+                Call the static initialize method of Initializer class that takes the following arguments
+                1 -> UserSignature instance
+                2 -> Environment instance
+                3 -> Token instance
+                4 -> TokenStore instance
+                5 -> SDKConfig instance
+                6 -> resource_path
+                7 -> Logger instance. Default value is None
+                8 -> RequestProxy instance. Default value is None
+                """
+                Initializer.initialize(user=user, environment=environment, token=token, store=store, sdk_config=config, resource_path=resource_path, logger=logger, proxy=request_proxy)
+        
+        
+        SDKInitializer.initialize()
+        
+        ```
+        
+        - You can now access the functionalities of the SDK. Refer to the sample codes to make various API calls through the SDK.
+        
+        ## Class Hierarchy
+        
+        ![classdiagram](class_hierarchy.png)
+        
+        ## Responses and Exceptions
+        
+        All SDK methods return an instance of the APIResponse class.
+        
+        After a successful API request, the **get_object()** method returns an instance of the **ResponseWrapper** (for **GET**) or the **ActionWrapper** (for **POST, PUT, DELETE**)
+        
+        Whenever the API returns an error response, the **get_object()** returns an instance of **APIException** class.
+        
+        **ResponseWrapper** (for **GET** requests) and **ActionWrapper** (for **POST, PUT, DELETE** requests) are the expected objects for Zoho CRM APIs’ responses
+        
+        However, some specific operations have different expected objects, such as the following:
+        
+        - Operations involving records in Tags
+            - **RecordActionWrapper**
+        
+        - Getting Record Count for a specific Tag operation
+            - **CountWrapper**
+        
+        - Operations involving BaseCurrency
+            - **BaseCurrencyActionWrapper**
+        
+        - Lead convert operation
+            - **ConvertActionWrapper**
+        
+        - Retrieving Deleted records operation
+            - **DeletedRecordsWrapper**
+        
+        - Record image download operation
+            - **FileBodyWrapper**
+        
+        - MassUpdate record operations
+            - **MassUpdateActionWrapper**
+            - **MassUpdateResponseWrapper**
+          
+        ### GET Requests
+        
+        - The **get_object()** returns an instance of one of the following classes, based on the return type.
+        
+            - For  **application/json** responses
+                - **ResponseWrapper**
+                - **CountWrapper**
+                - **DeletedRecordsWrapper**
+                - **MassUpdateResponseWrapper**
+                - **APIException**
+        
+            - For **file download** responses
+                - **FileBodyWrapper**
+                - **APIException**
+        
+        ### POST, PUT, DELETE Requests
+        
+        - The **getObject()** returns an instance of one of the following classes
+            - **ActionWrapper**
+            - **RecordActionWrapper**
+            - **BaseCurrencyActionWrapper**
+            - **MassUpdateActionWrapper**
+            - **ConvertActionWrapper**
+            - **APIException**
+        
+        - These wrapper classes may contain one or a list of instances of the following classes, depending on the response.
+            - **SuccessResponse Class**, if the request was successful.
+            - **APIException Class**, if the request was erroneous.
+        
+        For example, when you insert two records, and one of them was inserted successfully while the other one failed, the ActionWrapper will contain one instance each of the SuccessResponse and APIException classes.
+        
+        All other exceptions such as SDK anomalies and other unexpected behaviours are thrown under the SDKException class.
+        
+        ## Threading in the Python SDK
+        
+        Threads in a Python program help you achieve parallelism. By using multiple threads, you can make a Python program run faster and do multiple things simultaneously.
+        
+        The **Python SDK** (from version 3.x.x) supports both single-user and multi-user app.
+        
+        ### Multithreading in a Multi-user App
+        
+        Multi-threading for multi-users is achieved using Initializer's static **switch_user()** method.
+        switch_user() takes the value initialized previously for user, enviroment, token and sdk_config incase None is passed (or default value is passed). In case of request_proxy, if intended, the value has to be passed again else None(default value) will be taken.
+        
+        ```python
+        # without proxy
+        Initializer.switch_user(user=user, environment=environment, token=token, sdk_config=sdk_config_instance)
+        
+        # with proxy
+        Initializer.switch_user(user=user, environment=environment, token=token, sdk_config=sdk_config_instance, proxy=request_proxy)
+        ```
+        
+        Here is a sample code to depict multi-threading for a multi-user app.
+        
+        ```python
+        import threading
+        from zcrmsdk.src.com.zoho.crm.api.user_signature import UserSignature
+        from zcrmsdk.src.com.zoho.crm.api.dc import USDataCenter, EUDataCenter
+        from zcrmsdk.src.com.zoho.api.authenticator.store import DBStore
+        from zcrmsdk.src.com.zoho.api.logger import Logger
+        from zcrmsdk.src.com.zoho.crm.api.initializer import Initializer
+        from zcrmsdk.src.com.zoho.api.authenticator.oauth_token import OAuthToken
+        from zcrmsdk.src.com.zoho.crm.api.record import *
+        from zcrmsdk.src.com.zoho.crm.api.request_proxy import RequestProxy
+        from zcrmsdk.src.com.zoho.crm.api.sdk_config import SDKConfig
+        
+        
+        class MultiThread(threading.Thread):
+        
+            def __init__(self, environment, token, user, module_api_name, sdk_config, proxy=None):
+                super().__init__()
+                self.environment = environment
+                self.token = token
+                self.user = user
+                self.module_api_name = module_api_name
+                self.sdk_config = sdk_config
+                self.proxy = proxy
+        
+            def run(self):
+                try:
+                    Initializer.switch_user(user=self.user, environment=self.environment, token=self.token, sdk_config=self.sdk_config, proxy=self.proxy)
+        
+                    print('Getting records for User: ' + Initializer.get_initializer().user.get_email())
+        
+                    response = RecordOperations().get_records(self.module_api_name)
+        
+                    if response is not None:
+        
+                        # Get the status code from response
+                        print('Status Code: ' + str(response.get_status_code()))
+        
+                        if response.get_status_code() in [204, 304]:
+                            print('No Content' if response.get_status_code() == 204 else 'Not Modified')
+                            return
+        
+                        # Get object from response
+                        response_object = response.get_object()
+        
+                        if response_object is not None:
+        
+                            # Check if expected ResponseWrapper instance is received.
+                            if isinstance(response_object, ResponseWrapper):
+                                # Get the list of obtained Record instances
+                                record_list = response_object.get_data()
+        
+                                for record in record_list:
+                                    for key, value in record.get_key_values().items():
+                                        print(key + " : " + str(value))
+        
+                            # Check if the request returned an exception
+                            elif isinstance(response_object, APIException):
+                                # Get the Status
+                                print("Status: " + response_object.get_status().get_value())
+        
+                                # Get the Code
+                                print("Code: " + response_object.get_code().get_value())
+        
+                                print("Details")
+        
+                                # Get the details dict
+                                details = response_object.get_details()
+        
+                                for key, value in details.items():
+                                    print(key + ' : ' + str(value))
+        
+                                # Get the Message
+                                print("Message: " + response_object.get_message().get_value())
+        
+                except Exception as e:
+                    print(e)
+        
+            @staticmethod
+            def call():
+                logger = Logger.get_instance(level=Logger.Levels.INFO, file_path="/Users/user_name/Documents/python_sdk_log.log")
+        
+                user1 = UserSignature(email="abc@zoho.com")
+        
+                token1 = OAuthToken(client_id="clientId1", client_secret="clientSecret1", grant_token="Grant Token", refresh_token="refresh_token", id="id")
+        
+                environment1 = USDataCenter.PRODUCTION()
+        
+                store = DBStore()
+        
+                sdk_config_1 = SDKConfig(auto_refresh_fields=True, pick_list_validation=False)
+        
+                resource_path = '/Users/user_name/Documents/python-app'
+        
+                user1_module_api_name = 'Leads'
+        
+                user2_module_api_name = 'Contacts'
+        
+                environment2 = EUDataCenter.SANDBOX()
+        
+                user2 = UserSignature(email="abc@zoho.eu")
+        
+                sdk_config_2 = SDKConfig(auto_refresh_fields=False, pick_list_validation=True)
+        
+                token2 = OAuthToken(client_id="clientId2", client_secret="clientSecret2",grant_token="GRANT Token", refresh_token="refresh_token", redirect_url="redirectURL", id="id")
+        
+                request_proxy_user_2 = RequestProxy("host", 8080)
+        
+                Initializer.initialize(user=user1, environment=environment1, token=token1, store=store, sdk_config=sdk_config_1, resource_path=resource_path, logger=logger)
+        
+                t1 = MultiThread(environment1, token1, user1, user1_module_api_name, sdk_config_1)
+                t2 = MultiThread(environment2, token2, user2, user2_module_api_name, sdk_config_2, request_proxy_user_2)
+        
+                t1.start()
+                t2.start()
+        
+                t1.join()
+                t2.join()
+        
+        
+        MultiThread.call()
+        
+        ```
+        
+        - The program execution starts from **call()**.
+        
+        - The details of **user1** are given in the variables user1, token1, environment1.
+        
+        - Similarly, the details of another user **user2** are given in the variables user2, token2, environment2.
+        
+        - For each user, an instance of **MultiThread class** is created.
+        
+        - When the **start()** is called which in-turn invokes the **run()**,  the details of user1 are passed to the **switch_user** method through the **MultiThread object**. Therefore, this creates a thread for user1.
+        
+        - Similarly, When the **start()** is invoked again,  the details of user2 are passed to the **switch_user** function through the **MultiThread object**. Therefore, this creates a thread for user2.
+        
+        ### Multi-threading in a Single User App
+        
+        Here is a sample code to depict multi-threading for a single-user app.
+        
+        ```python
+        import threading
+        from zcrmsdk.src.com.zoho.crm.api.user_signature import UserSignature
+        from zcrmsdk.src.com.zoho.crm.api.dc import USDataCenter
+        from zcrmsdk.src.com.zoho.api.authenticator.store import DBStore
+        from zcrmsdk.src.com.zoho.api.logger import Logger
+        from zcrmsdk.src.com.zoho.crm.api.initializer import Initializer
+        from zcrmsdk.src.com.zoho.api.authenticator.oauth_token import OAuthToken
+        from zcrmsdk.src.com.zoho.crm.api.sdk_config import SDKConfig
+        from zcrmsdk.src.com.zoho.crm.api.record import *
+        
+        
+        class MultiThread(threading.Thread):
+        
+            def __init__(self, module_api_name):
+                super().__init__()
+                self.module_api_name = module_api_name
+        
+            def run(self):
+                try:
+                    print("Calling Get Records for module: " + self.module_api_name)
+        
+                    response = RecordOperations().get_records(self.module_api_name)
+        
+                    if response is not None:
+        
+                        # Get the status code from response
+                        print('Status Code: ' + str(response.get_status_code()))
+        
+                        if response.get_status_code() in [204, 304]:
+                            print('No Content' if response.get_status_code() == 204 else 'Not Modified')
+                            return
+        
+                        # Get object from response
+                        response_object = response.get_object()
+        
+                        if response_object is not None:
+        
+                            # Check if expected ResponseWrapper instance is received.
+                            if isinstance(response_object, ResponseWrapper):
+                                # Get the list of obtained Record instances
+                                record_list = response_object.get_data()
+        
+                                for record in record_list:
+                                    for key, value in record.get_key_values().items():
+                                        print(key + " : " + str(value))
+        
+                            # Check if the request returned an exception
+                            elif isinstance(response_object, APIException):
+                                # Get the Status
+                                print("Status: " + response_object.get_status().get_value())
+        
+                                # Get the Code
+                                print("Code: " + response_object.get_code().get_value())
+        
+                                print("Details")
+        
+                                # Get the details dict
+                                details = response_object.get_details()
+        
+                                for key, value in details.items():
+                                    print(key + ' : ' + str(value))
+        
+                                # Get the Message
+                                print("Message: " + response_object.get_message().get_value())
+        
+                except Exception as e:
+                    print(e)
+        
+            @staticmethod
+            def call():
+                logger = Logger.get_instance(level=Logger.Levels.INFO, file_path="/Users/user_name/Documents/python_sdk_log.log")
+        
+                user = UserSignature(email="abc@zoho.com")
+        
+                token = OAuthToken(client_id="clientId", client_secret="clientSecret", grant_token="grant_token", refresh_token="refresh_token", redirect_url="redirectURL", id="id")
+        
+                environment = USDataCenter.PRODUCTION()
+        
+                store = DBStore()
+        
+                sdk_config = SDKConfig()
+        
+                resource_path = '/Users/user_name/Documents/python-app'
+        
+                Initializer.initialize(user=user, environment=environment, token=token, store=store, sdk_config=sdk_config, resource_path=resource_path, logger=logger)
+        
+                t1 = MultiThread('Leads')
+                t2 = MultiThread('Quotes')
+        
+                t1.start()
+                t2.start()
+        
+                t1.join()
+                t2.join()
+        
+        
+        MultiThread.call()
+        ```
+        
+        - The program execution starts from **call()** where the SDK is initialized with the details of the user.
+        
+        - When the **start()** is called which in-turn invokes the run(),  the module_api_name is switched through the MultiThread object. Therefore, this creates a thread for the particular MultiThread instance.
+        
+        ## SDK Sample code
+        
+        ```python
+        from datetime import datetime
+        from zcrmsdk.src.com.zoho.crm.api.user_signature import UserSignature
+        from zcrmsdk.src.com.zoho.crm.api.dc import USDataCenter
+        from zcrmsdk.src.com.zoho.api.authenticator.store import DBStore
+        from zcrmsdk.src.com.zoho.api.logger import Logger
+        from zcrmsdk.src.com.zoho.crm.api.initializer import Initializer
+        from zcrmsdk.src.com.zoho.api.authenticator.oauth_token import OAuthToken
+        from zcrmsdk.src.com.zoho.crm.api.record import *
+        from zcrmsdk.src.com.zoho.crm.api import HeaderMap, ParameterMap
+        from zcrmsdk.src.com.zoho.crm.api.sdk_config import SDKConfig
+        
+        
+        class Record(object):
+        
+            def __init__(self):
+                pass
+        
+            @staticmethod
+            def get_records():
+        
+                """
+                Create an instance of Logger Class that takes two parameters
+                1 -> Level of the log messages to be logged. Can be configured by typing Logger.Levels "." and choose any level from the list displayed.
+                2 -> Absolute file path, where messages need to be logged.
+                """
+                logger = Logger.get_instance(level=Logger.Levels.INFO,
+                                             file_path="/Users/user_name/Documents/python_sdk_log.log")
+        
+                # Create an UserSignature instance that takes user Email as parameter
+                user = UserSignature(email="abc@zoho.com")
+        
+                """
+                Configure the environment
+                which is of the pattern Domain.Environment
+                Available Domains: USDataCenter, EUDataCenter, INDataCenter, CNDataCenter, AUDataCenter
+                Available Environments: PRODUCTION(), DEVELOPER(), SANDBOX()
+                """
+                environment = USDataCenter.PRODUCTION()
+        
+                """
+                Create a Token instance that takes the following parameters
+                1 -> OAuth client id.
+                2 -> OAuth client secret.
+                3 -> Grant token.
+                4 -> Refresh token.
+                5 -> OAuth redirect URL.
+                6 -> id
+                """
+                token = OAuthToken(client_id="clientId", client_secret="clientSecret", grant_token="grant_token", refresh_token="refresh_token", redirect_url="redirectURL", id="id")
+        
+                """
+                Create an instance of TokenStore
+                1 -> DataBase host name. Default value "localhost"
+                2 -> DataBase name. Default value "zohooauth"
+                3 -> DataBase user name. Default value "root"
+                4 -> DataBase password. Default value ""
+                5 -> DataBase port number. Default value "3306"
+                6->  DataBase table name . Default value "oauthtoken"
+                """
+                store = DBStore()
+        
+                """
+                auto_refresh_fields (Default value is False)
+                    if True - all the modules' fields will be auto-refreshed in the background, every hour.
+                    if False - the fields will not be auto-refreshed in the background. The user can manually delete the file(s) or refresh the fields using methods from ModuleFieldsHandler(zcrmsdk/src/com/zoho/crm/api/util/module_fields_handler.py)
+        
+                pick_list_validation (Default value is True)
+                    A boolean field that validates user input for a pick list field and allows or disallows the addition of a new value to the list.
+                    if True - the SDK validates the input. If the value does not exist in the pick list, the SDK throws an error.
+                    if False - the SDK does not validate the input and makes the API request with the user’s input to the pick list
+                 connect_timeout (Default value is None) 
+                    A  Float field to set connect timeout
+          
+                 read_timeout (Default value is None) 
+                    A  Float field to set read timeout
+                 """
+                config = SDKConfig(auto_refresh_fields=True, pick_list_validation=False, connect_timeout=None, read_timeout=None)
+        
+                """
+                The path containing the absolute directory path (in the key resource_path) to store user-specific files containing information about fields in modules. 
+                """
+                resource_path = '/Users/user_name/Documents/python-app'
+        
+                """
+                Call the static initialize method of Initializer class that takes the following arguments
+                1 -> UserSignature instance
+                2 -> Environment instance
+                3 -> Token instance
+                4 -> TokenStore instance
+                5 -> SDKConfig instance
+                6 -> resource_path
+                7 -> Logger instance
+                """
+                Initializer.initialize(user=user, environment=environment, token=token, store=store, sdk_config=config, resource_path=resource_path, logger=logger)
+        
+                try:
+                    module_api_name = 'Leads'
+        
+                    param_instance = ParameterMap()
+        
+                    param_instance.add(GetRecordsParam.converted, 'both')
+        
+                    param_instance.add(GetRecordsParam.cvid, '12712717217218')
+        
+                    header_instance = HeaderMap()
+        
+                    header_instance.add(GetRecordsHeader.if_modified_since, datetime.now())
+        
+                    response = RecordOperations().get_records(module_api_name, param_instance, header_instance)
+        
+                    if response is not None:
+        
+                        # Get the status code from response
+                        print('Status Code: ' + str(response.get_status_code()))
+        
+                        if response.get_status_code() in [204, 304]:
+                            print('No Content' if response.get_status_code() == 204 else 'Not Modified')
+                            return
+        
+                        # Get object from response
+                        response_object = response.get_object()
+        
+                        if response_object is not None:
+        
+                            # Check if expected ResponseWrapper instance is received.
+                            if isinstance(response_object, ResponseWrapper):
+                                # Get the list of obtained Record instances
+                                record_list = response_object.get_data()
+        
+                                for record in record_list:
+        
+                                    # Get the ID of each Record
+                                    print("Record ID: " + record.get_id())
+        
+                                    # Get the createdBy User instance of each Record
+                                    created_by = record.get_created_by()
+        
+                                    # Check if created_by is not None
+                                    if created_by is not None:
+                                        # Get the Name of the created_by User
+                                        print("Record Created By - Name: " + created_by.get_name())
+        
+                                        # Get the ID of the created_by User
+                                        print("Record Created By - ID: " + created_by.get_id())
+        
+                                        # Get the Email of the created_by User
+                                        print("Record Created By - Email: " + created_by.get_email())
+        
+                                    # Get the CreatedTime of each Record
+                                    print("Record CreatedTime: " + str(record.get_created_time()))
+        
+                                    if record.get_modified_time() is not None:
+                                        # Get the ModifiedTime of each Record
+                                        print("Record ModifiedTime: " + str(record.get_modified_time()))
+        
+                                    # Get the modified_by User instance of each Record
+                                    modified_by = record.get_modified_by()
+        
+                                    # Check if modified_by is not None
+                                    if modified_by is not None:
+                                        # Get the Name of the modified_by User
+                                        print("Record Modified By - Name: " + modified_by.get_name())
+        
+                                        # Get the ID of the modified_by User
+                                        print("Record Modified By - ID: " + modified_by.get_id())
+        
+                                        # Get the Email of the modified_by User
+                                        print("Record Modified By - Email: " + modified_by.get_email())
+        
+                                    # Get the list of obtained Tag instance of each Record
+                                    tags = record.get_tag()
+        
+                                    if tags is not None:
+                                        for tag in tags:
+                                            # Get the Name of each Tag
+                                            print("Record Tag Name: " + tag.get_name())
+        
+                                            # Get the Id of each Tag
+                                            print("Record Tag ID: " + tag.get_id())
+        
+                                    # To get particular field value
+                                    print("Record Field Value: " + str(record.get_key_value('Last_Name')))
+        
+                                    print('Record KeyValues: ')
+        
+                                    for key, value in record.get_key_values().items():
+                                        print(key + " : " + str(value))
+        
+                            # Check if the request returned an exception
+                            elif isinstance(response_object, APIException):
+                                # Get the Status
+                                print("Status: " + response_object.get_status().get_value())
+        
+                                # Get the Code
+                                print("Code: " + response_object.get_code().get_value())
+        
+                                print("Details")
+        
+                                # Get the details dict
+                                details = response_object.get_details()
+        
+                                for key, value in details.items():
+                                    print(key + ' : ' + str(value))
+        
+                                # Get the Message
+                                print("Message: " + response_object.get_message().get_value())
+        
+                except Exception as e:
+                    print(e)
+        
+        
+        Record.get_records()
+        ```
+        
+Keywords: development,zoho,crm,api,zcrmsdk,sdk,zcrm,zohocrmsdk2_1
+Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Description-Content-Type: text/markdown
```

### Comparing `zohocrmsdk2_1-2.0.0/setup.py` & `zohocrmsdk2_1-2.1.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='zohocrmsdk2_1',
-    version='2.0.0',
+    version='2.1.0',
     description='Zoho CRM SDK for ZOHO CRM 2.1 APIs',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/zoho/zohocrm-python-sdk-2.1',
     author='Zoho CRM API Team',
     author_email='support@zohocrm.com',
     scripts=[],
```

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/api/authenticator/oauth_token.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/api/authenticator/oauth_token.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/api/authenticator/store/db_store.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/api/authenticator/store/db_store.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/api/authenticator/store/file_store.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/api/authenticator/store/file_store.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/api/authenticator/store/token_store.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/api/authenticator/store/token_store.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/api/authenticator/token.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/api/authenticator/token.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/api/logger/logger.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/api/logger/logger.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/__init__.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/assignment_rules/api_exception.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/assignment_rules/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/assignment_rules/assignment_rule.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/assignment_rules/assignment_rule.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/assignment_rules/assignment_rules_operations.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/assignment_rules/assignment_rules_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/assignment_rules/default_user.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/assignment_rules/default_user.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/assignment_rules/response_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/assignment_rules/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/attachments/__init__.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/attachments/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/attachments/action_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/attachments/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/attachments/api_exception.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/attachments/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/attachments/attachment.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/attachments/attachment.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/attachments/attachments_operations.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/attachments/attachments_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/attachments/file_body_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/attachments/file_body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/attachments/response_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/attachments/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/attachments/success_response.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/attachments/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/blue_print/__init__.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/blue_print/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/blue_print/api_exception.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/blue_print/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/blue_print/blue_print.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/blue_print/blue_print.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/blue_print/blue_print_operations.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/blue_print/blue_print_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/blue_print/body_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/blue_print/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/blue_print/escalation.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/blue_print/escalation.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/blue_print/field.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/blue_print/field.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/blue_print/next_transition.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/blue_print/next_transition.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/blue_print/process_info.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/blue_print/process_info.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/blue_print/response_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/blue_print/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/blue_print/success_response.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/blue_print/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/blue_print/transition.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/blue_print/transition.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/blue_print/validation_error.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/blue_print/validation_error.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/__init__.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/action_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/api_exception.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/bulk_read_operations.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/bulk_read_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/call_back.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/call_back.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/criteria.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/criteria.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/file_body_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/file_body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/job_detail.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/job_detail.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/query.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/query.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/request_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/request_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/response_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/result.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/result.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/success_response.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/__init__.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/api_exception.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/bulk_write_operations.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/bulk_write_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/bulk_write_response.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/bulk_write_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/call_back.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/call_back.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/field_mapping.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/field_mapping.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/file.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/file.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/file_body_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/file_body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/request_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/request_wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 	def __init__(self):
 		"""Creates an instance of RequestWrapper"""
 
 		self.__character_encoding = None
 		self.__operation = None
 		self.__callback = None
 		self.__resource = None
+		self.__ignore_empty = None
 		self.__key_modified = dict()
 
 	def get_character_encoding(self):
 		"""
 		The method to get the character_encoding
 
 		Returns:
@@ -113,14 +114,38 @@
 
 		if resource is not None and not isinstance(resource, list):
 			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: resource EXPECTED TYPE: list', None, None)
 		
 		self.__resource = resource
 		self.__key_modified['resource'] = 1
 
+	def get_ignore_empty(self):
+		"""
+		The method to get the ignore_empty
+
+		Returns:
+			bool: A bool representing the ignore_empty
+		"""
+
+		return self.__ignore_empty
+
+	def set_ignore_empty(self, ignore_empty):
+		"""
+		The method to set the value to ignore_empty
+
+		Parameters:
+			ignore_empty (bool) : A bool representing the ignore_empty
+		"""
+
+		if ignore_empty is not None and not isinstance(ignore_empty, bool):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: ignore_empty EXPECTED TYPE: bool', None, None)
+		
+		self.__ignore_empty = ignore_empty
+		self.__key_modified['ignore_empty'] = 1
+
 	def is_key_modified(self, key):
 		"""
 		The method to check if the user has modified the given key
 
 		Parameters:
 			key (string) : A string representing the key
```

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/resource.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/resource.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/result.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/result.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/success_response.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/cancel_meetings/action_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/cancel_meetings/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/cancel_meetings/api_exception.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/cancel_meetings/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/cancel_meetings/body_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/related_records/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/cancel_meetings/cancel_meetings_operations.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/cancel_meetings/cancel_meetings_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/cancel_meetings/notify.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/cancel_meetings/notify.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/cancel_meetings/success_response.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/cancel_meetings/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/__init__.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/action_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/api_exception.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/body_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/contact_role.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/contact_role.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/contact_role_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/contact_role_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/contact_roles_operations.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/contact_roles_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/record_action_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/record_action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/record_body_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/record_body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/record_response_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/record_response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/response_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/success_response.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/currencies/__init__.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/currencies/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/currencies/action_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/currencies/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/currencies/api_exception.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/currencies/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/currencies/base_currency_action_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/currencies/base_currency_action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/currencies/base_currency_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/currencies/base_currency_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/currencies/body_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/currencies/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/currencies/currencies_operations.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/currencies/currencies_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/currencies/currency.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/currencies/currency.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/currencies/format.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/currencies/format.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/currencies/response_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/currencies/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/currencies/success_response.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/currencies/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/custom_views/api_exception.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/custom_views/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/custom_views/criteria.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/custom_views/criteria.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/custom_views/custom_view.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/custom_views/custom_view.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/custom_views/custom_views_operations.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/custom_views/custom_views_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/custom_views/info.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/custom_views/info.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/custom_views/range.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/custom_views/range.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/custom_views/response_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/custom_views/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/custom_views/shared_to.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/custom_views/shared_to.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/custom_views/translation.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/custom_views/translation.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/dc/au_data_center.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/dc/au_data_center.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/dc/cn_data_center.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/dc/cn_data_center.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/dc/data_center.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/dc/data_center.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/dc/eu_data_center.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/dc/eu_data_center.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/dc/in_data_center.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/dc/in_data_center.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/dc/jp_data_center.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/dc/jp_data_center.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/dc/us_data_center.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/dc/us_data_center.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/email_templates/api_exception.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/email_templates/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/email_templates/attachment.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/email_templates/attachment.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/email_templates/email_template.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/email_templates/email_template.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/email_templates/email_templates_operations.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/email_templates/email_templates_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/email_templates/response_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/email_templates/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/exception/sdk_exception.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/exception/sdk_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/field_attachments/api_exception.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/field_attachments/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/field_attachments/body_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/field_attachments/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/field_attachments/field_attachments_operations.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/field_attachments/field_attachments_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/field_attachments/file_body_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/field_attachments/file_body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/fields/__init__.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/fields/api_exception.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/fields/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/fields/association_details.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/fields/association_details.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/fields/auto_number.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/fields/auto_number.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/fields/crypt.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/fields/crypt.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/fields/currency.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/fields/currency.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/fields/external.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/fields/external.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/fields/field.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/fields/field.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/fields/fields_operations.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/fields/fields_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/fields/formula.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/fields/formula.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/fields/history_tracking.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/fields/history_tracking.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/fields/lookup_field.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/fields/lookup_field.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/fields/maps.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/fields/maps.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/fields/module.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/fields/module.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/fields/multi_module_lookup.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/fields/multi_module_lookup.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/fields/multi_select_lookup.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/fields/multi_select_lookup.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/fields/multi_user_lookup.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/fields/multi_user_lookup.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/fields/pick_list_value.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/fields/pick_list_value.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/fields/private.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/fields/private.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/fields/related_details.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/fields/related_details.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/fields/response_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/fields/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/fields/tool_tip.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/fields/tool_tip.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/fields/unique.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/fields/unique.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/fields/view_type.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/fields/view_type.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/file/action_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/file/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/file/api_exception.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/file/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/file/body_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/file/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/file/file_body_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/file/file_body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/file/file_operations.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/file/file_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/file/success_response.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/file/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/header_map.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/header_map.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/initializer.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/initializer.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/inventory_templates/api_exception.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/inventory_templates/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/inventory_templates/inventory_template.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/inventory_templates/inventory_template.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/inventory_templates/inventory_templates_operations.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/inventory_templates/inventory_templates_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/inventory_templates/response_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/inventory_templates/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/layouts/api_exception.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/layouts/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/layouts/layout.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/layouts/layout.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/layouts/layouts_operations.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/layouts/layouts_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/layouts/properties.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/layouts/properties.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/layouts/response_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/layouts/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/layouts/section.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/layouts/section.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/modules/__init__.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/modules/action_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/modules/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/modules/api_exception.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/modules/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/modules/argument.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/modules/argument.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/modules/body_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/modules/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/modules/module.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/modules/module.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/modules/modules_operations.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/modules/modules_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/modules/related_list_properties.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/modules/related_list_properties.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/modules/response_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/modules/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/modules/success_response.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/modules/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/modules/territory.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/modules/territory.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/notes/__init__.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/notes/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/notes/action_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/notes/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/notes/api_exception.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/notes/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/notes/body_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/cancel_meetings/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/notes/info.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/info.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/notes/note.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/notes/note.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/notes/notes_operations.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/notes/notes_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/notes/response_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/notes/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/notes/success_response.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/notes/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/notification/__init__.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/notification/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/notification/action_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/notification/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/notification/api_exception.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/notification/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/notification/body_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/notification/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/notification/info.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/notification/info.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/notification/notification.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/notification/notification.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/notification/notification_operations.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/notification/notification_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/notification/response_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/notification/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/notification/success_response.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/notification/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/org/api_exception.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/org/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/org/file_body_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/org/file_body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/org/hierarchy_preference.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/org/hierarchy_preference.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/org/license_details.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/org/license_details.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/org/org.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/org/org.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/org/org_operations.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/org/org_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/org/response_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/org/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/org/success_response.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/org/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/parameter_map.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/parameter_map.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/pipeline/__init__.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/pipeline/action_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/pipeline/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/pipeline/api_exception.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/pipeline/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/pipeline/body_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/pipeline/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/pipeline/forecast_category.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/pipeline/forecast_category.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/pipeline/pick_list_value.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/pipeline/pick_list_value.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/pipeline/pipeline.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/pipeline/pipeline_operations.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/pipeline/pipeline_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/pipeline/response_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/pipeline/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/pipeline/stage.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/pipeline/stage.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/pipeline/success_response.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/pipeline/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/pipeline/transfer_action_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/pipeline/transfer_action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/pipeline/transfer_and_delete_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/pipeline/transfer_and_delete_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/pipeline/transfer_pipe_line.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/pipeline/transfer_pipe_line.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/profiles/api_exception.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/profiles/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/profiles/category.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/profiles/category.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/profiles/default_view.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/profiles/default_view.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/profiles/permission_detail.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/profiles/permission_detail.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/profiles/profile.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/profiles/profile.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/profiles/profiles_operations.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/profiles/profiles_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/profiles/response_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/profiles/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/profiles/section.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/profiles/section.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/query/api_exception.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/query/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/query/body_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/query/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/query/query_operations.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/query/query_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/query/response_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/query/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/__init__.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/action_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/api_exception.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/apply_feature_execution.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/apply_feature_execution.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/body_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/carry_over_tags.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/carry_over_tags.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/comment.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/comment.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/consent.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/consent.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/convert_action_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/convert_action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/convert_body_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/convert_body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/count_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/count_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/criteria.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/criteria.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/deleted_record.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/deleted_record.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/deleted_records_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/deleted_records_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/field.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/field.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/file_body_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/file_body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/file_details.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/file_details.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/image_upload.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/image_upload.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/info.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/notes/info.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/lead_converter.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/lead_converter.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/line_item_product.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/line_item_product.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/line_tax.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/line_tax.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/mass_update.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/mass_update.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/mass_update_action_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/mass_update_action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/mass_update_body_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/mass_update_body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/mass_update_response_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/mass_update_response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/mass_update_success_response.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/mass_update_success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/mass_update_territory.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/mass_update_territory.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/multi_select_lookup.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/multi_select_lookup.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/multi_select_picklist.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/multi_select_picklist.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/participants.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/participants.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/price_book.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/price_book.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/pricing_details.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/pricing_details.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/record.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/record.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/record_operations.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/record_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/recurring_activity.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/recurring_activity.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/remind_at.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/remind_at.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/reminder.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/reminder.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/response_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/success_response.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/successful_convert.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/successful_convert.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/tax.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/tax.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/territory.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/territory.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/widget.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/widget.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/record/wizard.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/record/wizard.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/related_lists/api_exception.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/related_lists/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/related_lists/related_list.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/related_lists/related_list.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/related_lists/related_lists_operations.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/related_lists/related_lists_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/related_lists/response_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/related_lists/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/related_records/__init__.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/related_records/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/related_records/action_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/related_records/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/related_records/api_exception.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/related_records/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/related_records/body_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/notes/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/related_records/file_body_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/related_records/file_body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/related_records/related_records_operations.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/related_records/related_records_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/related_records/response_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/related_records/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/related_records/success_response.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/related_records/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/request_proxy.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/request_proxy.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/roles/api_exception.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/roles/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/roles/response_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/roles/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/roles/role.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/roles/role.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/roles/roles_operations.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/roles/roles_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/sdk_config.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/sdk_config.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/send_mail/__init__.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/send_mail/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/send_mail/action_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/send_mail/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/send_mail/api_exception.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/send_mail/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/send_mail/body_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/send_mail/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/send_mail/data_subject_request.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/send_mail/data_subject_request.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/send_mail/inventory_details.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/send_mail/inventory_details.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/send_mail/mail.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/send_mail/mail.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/send_mail/response_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/send_mail/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/send_mail/send_mail_operations.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/send_mail/send_mail_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/send_mail/success_response.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/send_mail/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/send_mail/user_address.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/send_mail/user_address.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/share_records/__init__.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/share_records/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/share_records/action_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/share_records/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/share_records/api_exception.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/share_records/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/share_records/body_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/share_records/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/share_records/delete_action_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/share_records/delete_action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/share_records/response_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/share_records/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/share_records/share_record.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/share_records/share_record.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/share_records/share_records_operations.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/share_records/share_records_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/share_records/shared_through.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/share_records/shared_through.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/share_records/success_response.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/share_records/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/tags/__init__.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/tags/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/tags/action_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/tags/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/tags/api_exception.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/tags/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/tags/body_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/tags/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/tags/conflict_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/tags/conflict_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/tags/count_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/tags/count_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/tags/info.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/tags/info.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/tags/merge_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/tags/merge_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/tags/record_action_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/tags/record_action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/tags/response_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/tags/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/tags/success_response.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/tags/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/tags/tag.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/tags/tag.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/tags/tags_operations.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/tags/tags_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/taxes/action_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/taxes/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/taxes/api_exception.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/taxes/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/taxes/body_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/taxes/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/taxes/preference.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/taxes/preference.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/taxes/response_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/taxes/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/taxes/success_response.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/taxes/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/taxes/tax.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/taxes/tax.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/taxes/taxes_operations.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/taxes/taxes_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/territories/api_exception.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/territories/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/territories/response_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/territories/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/territories/territories_operations.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/territories/territories_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/territories/territory.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/territories/territory.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/user_signature.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/user_signature.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/users/__init__.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/users/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/users/action_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/users/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/users/api_exception.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/users/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/users/body_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/users/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/users/customize_info.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/users/customize_info.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/users/info.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/users/info.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/users/request_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/users/request_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/users/response_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/users/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/users/shift.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/users/shift.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/users/success_response.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/users/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/users/tab_theme.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/users/tab_theme.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/users/territory.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/users/territory.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/users/theme.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/users/theme.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/users/user.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/users/user.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/users/users_operations.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/users/users_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/util/__init__.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/util/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/util/api_http_connector.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/util/api_http_connector.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/util/api_response.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/util/api_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/util/common_api_handler.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/util/common_api_handler.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/util/constants.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/util/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,15 +170,15 @@
 
     PHOTO_SUPPORTED_MODULES = ["leads", "contacts", "accounts", "products", "vendors"]
 
     GIVEN_LENGTH = "given-length"
 
     ZOHO_SDK = "X-ZOHO-SDK"
 
-    SDK_VERSION = "2.0.0"
+    SDK_VERSION = "2.1.0"
 
     CONTENT_DISPOSITION = "Content-Disposition"
 
     TOKEN_ERROR = "TOKEN ERROR"
 
     SAVE_TOKEN_ERROR = "Exception in saving tokens"
```

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/util/converter.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/util/converter.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/util/datatype_converter.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/util/datatype_converter.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/util/downloader.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/util/downloader.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/util/form_data_converter.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/util/form_data_converter.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/util/header_param_validator.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/util/header_param_validator.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/util/json_converter.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/util/json_converter.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/util/module_fields_handler.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/util/module_fields_handler.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/util/stream_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/util/stream_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/util/utility.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/util/utility.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/util/xml_converter.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/util/xml_converter.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/variable_groups/api_exception.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/variable_groups/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/variable_groups/response_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/variable_groups/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/variable_groups/variable_group.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/variable_groups/variable_group.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/variable_groups/variable_groups_operations.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/variable_groups/variable_groups_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/variables/__init__.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/variables/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/variables/action_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/variables/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/variables/api_exception.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/variables/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/variables/body_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/variables/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/variables/response_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/variables/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/variables/success_response.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/variables/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/variables/variable.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/variables/variable.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/variables/variables_operations.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/variables/variables_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/wizards/api_exception.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/wizards/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/wizards/button.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/wizards/button.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/wizards/chart_data.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/wizards/chart_data.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/wizards/connection.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/wizards/connection.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/wizards/container.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/wizards/container.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/wizards/node.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/wizards/node.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/wizards/response_wrapper.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/wizards/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/wizards/screen.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/wizards/screen.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/wizards/segment.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/wizards/segment.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/wizards/transition.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/wizards/transition.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/wizards/wizard.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/wizards/wizard.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/com/zoho/crm/api/wizards/wizards_operations.py` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/com/zoho/crm/api/wizards/wizards_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_1-2.0.0/zcrmsdk/src/json_details.json` & `zohocrmsdk2_1-2.1.0/zcrmsdk/src/json_details.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997929606625259%*

 * *Differences: {"'zcrmsdk.src.com.zoho.crm.api.bulk_write.RequestWrapper'": "{'ignore_empty': "*

 * *                                                             "OrderedDict([('name', "*

 * *                                                             "'ignore_empty'), ('type', "*

 * *                                                             "'Boolean')])}"}*

```diff
@@ -1642,14 +1642,18 @@
             "structure_name": "zcrmsdk.src.com.zoho.crm.api.bulk_write.CallBack",
             "type": "zcrmsdk.src.com.zoho.crm.api.bulk_write.CallBack"
         },
         "character_encoding": {
             "name": "character_encoding",
             "type": "String"
         },
+        "ignore_empty": {
+            "name": "ignore_empty",
+            "type": "Boolean"
+        },
         "operation": {
             "name": "operation",
             "required": true,
             "type": "zcrmsdk.src.com.zoho.crm.api.util.Choice",
             "values": [
                 "insert",
                 "update",
```

### Comparing `zohocrmsdk2_1-2.0.0/zohocrmsdk2_1.egg-info/PKG-INFO` & `zohocrmsdk2_1-2.1.0/zohocrmsdk2_1.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,1109 +1,1109 @@
 Metadata-Version: 2.1
 Name: zohocrmsdk2-1
-Version: 2.0.0
+Version: 2.1.0
 Summary: Zoho CRM SDK for ZOHO CRM 2.1 APIs
 Home-page: https://github.com/zoho/zohocrm-python-sdk-2.1
 Author: Zoho CRM API Team
 Author-email: support@zohocrm.com
 License: Apache Software License, Version 2.0, http://www.apache.org/licenses/LICENSE-2.0
-Keywords: development,zoho,crm,api,zcrmsdk,sdk,zcrm,zohocrmsdk2_1
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-License
-=======
-
-    Copyright (c) 2021, ZOHO CORPORATION PRIVATE LIMITED 
-    All rights reserved. 
-
-    Licensed under the Apache License, Version 2.0 (the "License"); 
-    you may not use this file except in compliance with the License. 
-    You may obtain a copy of the License at 
-    
-        http://www.apache.org/licenses/LICENSE-2.0 
-    
-    Unless required by applicable law or agreed to in writing, software 
-    distributed under the License is distributed on an "AS IS" BASIS, 
-    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. 
-    See the License for the specific language governing permissions and 
-    limitations under the License.
-
-# ZOHO CRM PYTHON SDK 2.1 for API version 2.1
-
-## Table Of Contents
-
-* [Overview](#overview)
-* [Registering a Zoho Client](#registering-a-zoho-client)
-* [Environmental Setup](#environmental-setup)
-* [Including the SDK in your project](#including-the-sdk-in-your-project)
-* [Persistence](#token-persistence)
-  * [DataBase Persistence](#database-persistence)
-  * [File Persistence](#file-persistence)
-  * [Custom Persistence](#custom-persistence)
-* [Configuration](#configuration)
-* [Initialization](#initializing-the-application)
-* [Class Hierarchy](#class-hierarchy)
-* [Responses And Exceptions](#responses-and-exceptions)
-* [Threading](#threading-in-the-python-sdk)
-  * [Multithreading in a Multi-User App](#multithreading-in-a-multi-user-app)
-  * [Multi-threading in a Single User App](#multi-threading-in-a-single-user-app)
-* [Sample Code](#sdk-sample-code)
-## Overview
-
-Zoho CRM PYTHON SDK offers a way to create client Python applications that can be integrated with Zoho CRM.
-
-## Registering a Zoho Client
-
-Since Zoho CRM APIs are authenticated with OAuth2 standards, you should register your client app with Zoho. To register your app:
-
-- Visit this page [https://api-console.zoho.com](https://api-console.zoho.com)
-
-- Click on `ADD CLIENT`.
-
-- Choose the `Client Type`.
-
-- Enter **Client Name**, **Client Domain** or **Homepage URL** and **Authorized Redirect URIs** then click `CREATE`.
-
-- Your Client app will be created.
-
-- Select the created OAuth client.
-
-- Generate grant token by providing the necessary scopes, time duration (the duration for which the generated token is valid) and Scope Description.
-
-## Environmental Setup
-
-Python SDK is installable through **pip**. **pip** is a tool for dependency management in Python. SDK expects the following from the client app.
-
-- Client app must have Python(version 3 and above)
-
-- Python SDK must be installed into client app through **pip**.
-
-## Including the SDK in your project
-
-- Install **Python** from [python.org](https://www.python.org/downloads/) (if not installed).
-
-- Install **Python SDK**
-    - Navigate to the workspace of your client app.
-    - Run the command below:
-
-    ```sh
-    pip install zohocrmsdk2_1==1.x.x
-    ```
-- The Python SDK will be installed in your client application.
-
-## Token Persistence
-
-Token persistence refers to storing and utilizing the authentication tokens that are provided by Zoho. There are three ways provided by the SDK in which persistence can be utilized. They are DataBase Persistence, File Persistence and Custom Persistence.
-
-### Table of Contents
-
-- [DataBase Persistence](#database-persistence)
-
-- [File Persistence](#file-persistence)
-
-- [Custom Persistence](#custom-persistence)
-
-### Implementing OAuth Persistence
-
-Once the application is authorized, OAuth access and refresh tokens can be used for subsequent user data requests to Zoho CRM. Hence, they need to be persisted by the client app.
-
-The persistence is achieved by writing an implementation of the inbuilt Abstract Base Class **[TokenStore](zcrmsdk/src/com/zoho/api/authenticator/store/token_store.py)**, which has the following callback methods.
-
-- **get_token(self, user, [token](zcrmsdk/src/com/zoho/api/authenticator/token.py))** - invoked before firing a request to fetch the saved tokens. This method should return implementation of inbuilt **Token Class** object for the library to process it.
-
-- **save_token(self, user, [token](zcrmsdk/src/com/zoho/api/authenticator/token.py))** - invoked after fetching access and refresh tokens from Zoho.
-
-- **delete_token(self, [token](zcrmsdk/src/com/zoho/api/authenticator/token.py))** - invoked before saving the latest tokens.
-
-- **get_tokens(self)** - The method to get the all the stored tokens.
-
-- **delete_tokens(self)** - The method to delete all the stored tokens.
-
-- **get_token_by_id(self, id, token)** - The method to retrieve the user's token details based on unique ID.
-
-Note:
-
-- user is an instance of UserSignature Class.
-
-- token is an instance of Token Class.
-
-### DataBase Persistence
-
-In case the user prefers to use default DataBase persistence, **MySQL** can be used.
-
-- The database name should be **zohooauth**.
-
-- There must be a table name **oauthtoken** with the following columns.
-
-  - id int(11)
-
-  - user_mail varchar(255)
-  
-  - client_id varchar(255)
-  
-  - client_secret varchar(255)
-
-  - refresh_token varchar(255)
-
-  - access_token varchar(255)
-
-  - grant_token varchar(255)
-
-  - expiry_time varchar(20)
-  
-  - redirect_url varchar(255)
-
-Note:
-- Custom database name and table name can be set in DBStore instance.
-
-#### MySQL Query
-
-```sql
-CREATE TABLE  oauthtoken (
-  id varchar(255) NOT NULL,
-  user_mail varchar(255) NOT NULL,
-  client_id varchar(255),
-  client_secret varchar(255),
-  refresh_token varchar(255),
-  access_token varchar(255),
-  grant_token varchar(255),
-  expiry_time varchar(20),
-  redirect_url varchar(255),
-  primary key (id)
-)
-```
-
-#### Create DBStore object
-
-```python
-from zcrmsdk.src.com.zoho.api.authenticator.store import DBStore
-"""
-DBStore takes the following parameters
-1 -> DataBase host name. Default value "localhost"
-2 -> DataBase name. Default value "zohooauth"
-3 -> DataBase user name. Default value "root"
-4 -> DataBase password. Default value ""
-5 -> DataBase port number. Default value "3306"
-6->  DataBase table name . Default value "oauthtoken"
-"""
-store = DBStore()
-
-store = DBStore(host='host_name', database_name='database_name', user_name='user_name', password='password', port_number='port_number', table_name = "table_name")
-```
-
-### File Persistence
-
-In case of File Persistence, the user can persist tokens in the local drive, by providing the absolute file path to the FileStore object.
-
-- The File contains
-    - id 
-    
-    - user_mail
-
-    - client_id
-    
-    - client_secret
-
-    - refresh_token
-
-    - access_token
-
-    - grant_token
-
-    - expiry_time
-    
-    - redirect_url
-
-#### Create FileStore object
-
-```python
-from zcrmsdk.src.com.zoho.api.authenticator.store import FileStore
-"""
-FileStore takes the following parameter
-1 -> Absolute file path of the file to persist tokens
-"""
-store = FileStore(file_path='/Users/username/Documents/python_sdk_token.txt')
-```
-
-### Custom Persistence
-To use Custom Persistence, you must implement **[TokenStore](zcrmsdk/src/com/zoho/api/authenticator/store/token_store.py)** and override the methods.
-
-```python
-from zcrmsdk.src.com.zoho.api.authenticator.store import TokenStore
-
-
-class CustomStore(TokenStore):
-
-    def __init__(self):
-        pass
-
-    def get_token(self, user, token):
-
-        """
-        Parameters:
-            user (UserSignature) : A UserSignature class instance.
-            token (Token) : A Token (zcrmsdk.src.com.zoho.api.authenticator.OAuthToken) class instance
-        """
-
-        # Add code to get the token
-        return None
-
-    def save_token(self, user, token):
-
-        """
-        Parameters:
-            user (UserSignature) : A UserSignature class instance.
-            token (Token) : A Token (zcrmsdk.src.com.zoho.api.authenticator.OAuthToken) class instance
-        """
-
-        # Add code to save the token
-
-    def delete_token(self, token):
-
-        """
-        Parameters:
-            token (Token) : A Token (zcrmsdk.src.com.zoho.api.authenticator.OAuthToken) class instance
-        """
-
-        # Add code to delete the token
-    
-    def get_tokens(self):
-
-        """
-        Returns:
-            list: List of stored tokens
-        """
-
-        # Add code to get all the stored tokens
-    
-    def delete_tokens(self):
-
-        # Add code to delete all the stored tokens
-    
-    def get_token_by_id(id, token):
+Description: License
+        =======
         
-        """
-        The method to get id token details.
-
-        Parameters:
-            id (String) : A String id.
-            token (Token) : A Token class instance.
-
-        Returns:
-            Token : A Token class instance representing the id token details.
-        """
-```
-
-## Configuration
-
-Before you get started with creating your Python application, you need to register your client and authenticate the app with Zoho.
-
-| Mandatory Keys    | Optional Keys |
-| :---------------- | :------------ |
-| user              | logger        |
-| environment       | store         |
-| token             | sdk_config    |
-|                   | proxy         |
-|                   | resource_path |
-----
-
-- Create an instance of **UserSignature** Class that identifies the current user.
-  ```python
-  from zcrmsdk.src.com.zoho.crm.api.user_signature import UserSignature
-
-  # Create an UserSignature instance that takes user Email as parameter
-  user = UserSignature(email='abc@zoho.com')
-  ```
-
-- Configure the API environment which decides the domain and the URL to make API calls.
-  ```python
-  from zcrmsdk.src.com.zoho.crm.api.dc import USDataCenter
-
-  """
-  Configure the environment
-  which is of the pattern Domain.Environment
-  Available Domains: USDataCenter, EUDataCenter, INDataCenter, CNDataCenter, AUDataCenter
-  Available Environments: PRODUCTION(), DEVELOPER(), SANDBOX()
-  """
-  environment = USDataCenter.PRODUCTION()
-  ```
-
-- Create an instance of **OAuthToken** with the information that you get after registering your Zoho client.
-  ```python
-  from zcrmsdk.src.com.zoho.api.authenticator.oauth_token import OAuthToken
-
-  """
-  Create a Token instance that takes the following parameters
-  1 -> OAuth client id.
-  2 -> OAuth client secret.
-  3 -> Grant token.
-  4 -> Refresh token.
-  5 -> OAuth redirect URL. Default value is None
-  6 -> id
-  7 -> Access token
-  """
-  token = OAuthToken(client_id='clientId', client_secret='clientSecret', grant_token='grant_token', refresh_token="refresh_token", redirect_url='redirectURL', id="id", access_token="access_token")
-  ```
-
-- Create an instance of **Logger** Class to log exception and API information. By default, the SDK constructs a Logger instance with level - INFO and file_path - (sdk_logs.log, created in the current working directory)
-  ```python
-    from zcrmsdk.src.com.zoho.api.logger import Logger
-  
-    """
-    Create an instance of Logger Class that takes two parameters
-    1 -> Level of the log messages to be logged. Can be configured by typing Logger.Levels "." and choose any level from the list displayed.
-    2 -> Absolute file path, where messages need to be logged.
-    """
-    logger = Logger.get_instance(level=Logger.Levels.INFO, file_path="/Users/user_name/Documents/python_sdk_log.log")
-    ```
-
-- Create an instance of **TokenStore** to persist tokens, used for authenticating all the requests. By default, the SDK creates the sdk_tokens.txt created in the current working directory) to persist the tokens.
-  ```python
-  from zcrmsdk.src.com.zoho.api.authenticator.store import DBStore, FileStore
-
-  """
-  DBStore takes the following parameters
-  1 -> DataBase host name. Default value "localhost"
-  2 -> DataBase name. Default value "zohooauth"
-  3 -> DataBase user name. Default value "root"
-  4 -> DataBase password. Default value ""
-  5 -> DataBase port number. Default value "3306"
-  6 -> DataBase table name. Default value "oauthtoken"
-  """
-  store = DBStore()
-
-  #store = DBStore(host='host_name', database_name='database_name', user_name='user_name', password='password', port_number='port_number', table_name = "table_name")
-
-  """
-  FileStore takes the following parameter
-  1 -> Absolute file path of the file to persist tokens
-  """
-  #store = FileStore(file_path='/Users/username/Documents/python_sdk_tokens.txt')
-  ```
-
-- Create an instance of SDKConfig containing SDK configurations.
-  ```python
-  from zcrmsdk.src.com.zoho.crm.api.sdk_config import SDKConfig
-
-  """
-  By default, the SDK creates the SDKConfig instance
-  auto_refresh_fields (Default value is False)
-    if True - all the modules' fields will be auto-refreshed in the background, every hour.
-    if False - the fields will not be auto-refreshed in the background. The user can manually delete the file(s) or refresh the fields using methods from ModuleFieldsHandler(zcrmsdk/src/com/zoho/crm/api/util/module_fields_handler.py)
-
-  pick_list_validation (Default value is True)
-    A boolean field that validates user input for a pick list field and allows or disallows the addition of a new value to the list.
-    if True - the SDK validates the input. If the value does not exist in the pick list, the SDK throws an error.
-    if False - the SDK does not validate the input and makes the API request with the user’s input to the pick list
-  
-  connect_timeout (Default value is None) 
-    A  Float field to set connect timeout
-  
-  read_timeout (Default value is None) 
-    A  Float field to set read timeout
-  """
-  config = SDKConfig(auto_refresh_fields=True, pick_list_validation=False, connect_timeout=None, read_timeout=None)
-  ```
-
-- The path containing the absolute directory path to store user specific files containing module fields information. By default, the SDK stores the user-specific files within a folder in the current working directory.
-  ```python
-  resource_path = '/Users/user_name/Documents/python-app'
-  ```
-
-- Create an instance of RequestProxy containing the proxy properties of the user.
-    ```python
-    from zcrmsdk.src.com.zoho.crm.api.request_proxy import RequestProxy
-
-    """
-    RequestProxy takes the following parameters
-    1 -> Host
-    2 -> Port Number
-    3 -> User Name. Default value is None
-    4 -> Password. Default value is an empty string
-    """
-    request_proxy = RequestProxy(host='proxyHost', port=80)
-    request_proxy = RequestProxy(host='proxyHost', port=80, user='userName', password='password')
-    ```
-
-## Initializing the Application
-
-Initialize the SDK using the following code.
-
-```python
-from zcrmsdk.src.com.zoho.crm.api.user_signature import UserSignature
-from zcrmsdk.src.com.zoho.crm.api.dc import USDataCenter
-from zcrmsdk.src.com.zoho.api.authenticator.store import DBStore, FileStore
-from zcrmsdk.src.com.zoho.api.logger import Logger
-from zcrmsdk.src.com.zoho.crm.api.initializer import Initializer
-from zcrmsdk.src.com.zoho.api.authenticator.oauth_token import OAuthToken
-from zcrmsdk.src.com.zoho.crm.api.sdk_config import SDKConfig
-
-
-class SDKInitializer(object):
-
-    @staticmethod
-    def initialize():
-
-        """
-        Create an instance of Logger Class that takes two parameters
-        1 -> Level of the log messages to be logged. Can be configured by typing Logger.Levels "." and choose any level from the list displayed.
-        2 -> Absolute file path, where messages need to be logged.
-        """
-        logger = Logger.get_instance(level=Logger.Levels.INFO, file_path='/Users/user_name/Documents/python_sdk_log.log')
-
-        # Create an UserSignature instance that takes user Email as parameter
-        user = UserSignature(email='abc@zoho.com')
-
-        """
-        Configure the environment
-        which is of the pattern Domain.Environment
-        Available Domains: USDataCenter, EUDataCenter, INDataCenter, CNDataCenter, AUDataCenter
-        Available Environments: PRODUCTION(), DEVELOPER(), SANDBOX()
-        """
-        environment = USDataCenter.PRODUCTION()
-
-        """
-        Create a Token instance that takes the following parameters
-        1 -> OAuth client id.
-        2 -> OAuth client secret.
-        3 -> Grant token.
-        4 -> Refresh token.
-        5 -> OAuth redirect URL.
-        6 -> id
-        """
-        token = OAuthToken(client_id='clientId', client_secret='clientSecret', grant_token='grant_token', refresh_token="refresh_token", redirect_url='redirectURL', id="id")
-
-        """
-        Create an instance of TokenStore
-        1 -> Absolute file path of the file to persist tokens
-        """
-        store = FileStore(file_path='/Users/username/Documents/python_sdk_tokens.txt')
-
-        """
-        Create an instance of TokenStore
-        1 -> DataBase host name. Default value "localhost"
-        2 -> DataBase name. Default value "zohooauth"
-        3 -> DataBase user name. Default value "root"
-        4 -> DataBase password. Default value ""
-        5 -> DataBase port number. Default value "3306"
-        6->  DataBase table name . Default value "oauthtoken"
-        """
-        store = DBStore()
-        store = DBStore(host='host_name', database_name='database_name', user_name='user_name', password='password',port_number='port_number', table_name = "table_name")
-
-        """
-        auto_refresh_fields (Default value is False)
-            if True - all the modules' fields will be auto-refreshed in the background, every hour.
-            if False - the fields will not be auto-refreshed in the background. The user can manually delete the file(s) or refresh the fields using methods from ModuleFieldsHandler(zcrmsdk/src/com/zoho/crm/api/util/module_fields_handler.py)
-
-        pick_list_validation (Default value is True)
-        A boolean field that validates user input for a pick list field and allows or disallows the addition of a new value to the list.
-            if True - the SDK validates the input. If the value does not exist in the pick list, the SDK throws an error.
-            if False - the SDK does not validate the input and makes the API request with the user’s input to the pick list
-
-        connect_timeout (Default value is None) 
-            A  Float field to set connect timeout
+            Copyright (c) 2021, ZOHO CORPORATION PRIVATE LIMITED 
+            All rights reserved. 
+        
+            Licensed under the Apache License, Version 2.0 (the "License"); 
+            you may not use this file except in compliance with the License. 
+            You may obtain a copy of the License at 
+            
+                http://www.apache.org/licenses/LICENSE-2.0 
+            
+            Unless required by applicable law or agreed to in writing, software 
+            distributed under the License is distributed on an "AS IS" BASIS, 
+            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. 
+            See the License for the specific language governing permissions and 
+            limitations under the License.
+        
+        # ZOHO CRM PYTHON SDK 2.1 for API version 2.1
+        
+        ## Table Of Contents
+        
+        * [Overview](#overview)
+        * [Registering a Zoho Client](#registering-a-zoho-client)
+        * [Environmental Setup](#environmental-setup)
+        * [Including the SDK in your project](#including-the-sdk-in-your-project)
+        * [Persistence](#token-persistence)
+          * [DataBase Persistence](#database-persistence)
+          * [File Persistence](#file-persistence)
+          * [Custom Persistence](#custom-persistence)
+        * [Configuration](#configuration)
+        * [Initialization](#initializing-the-application)
+        * [Class Hierarchy](#class-hierarchy)
+        * [Responses And Exceptions](#responses-and-exceptions)
+        * [Threading](#threading-in-the-python-sdk)
+          * [Multithreading in a Multi-User App](#multithreading-in-a-multi-user-app)
+          * [Multi-threading in a Single User App](#multi-threading-in-a-single-user-app)
+        * [Sample Code](#sdk-sample-code)
+        ## Overview
+        
+        Zoho CRM PYTHON SDK offers a way to create client Python applications that can be integrated with Zoho CRM.
+        
+        ## Registering a Zoho Client
+        
+        Since Zoho CRM APIs are authenticated with OAuth2 standards, you should register your client app with Zoho. To register your app:
+        
+        - Visit this page [https://api-console.zoho.com](https://api-console.zoho.com)
+        
+        - Click on `ADD CLIENT`.
+        
+        - Choose the `Client Type`.
+        
+        - Enter **Client Name**, **Client Domain** or **Homepage URL** and **Authorized Redirect URIs** then click `CREATE`.
+        
+        - Your Client app will be created.
+        
+        - Select the created OAuth client.
+        
+        - Generate grant token by providing the necessary scopes, time duration (the duration for which the generated token is valid) and Scope Description.
+        
+        ## Environmental Setup
+        
+        Python SDK is installable through **pip**. **pip** is a tool for dependency management in Python. SDK expects the following from the client app.
+        
+        - Client app must have Python(version 3 and above)
+        
+        - Python SDK must be installed into client app through **pip**.
+        
+        ## Including the SDK in your project
+        
+        - Install **Python** from [python.org](https://www.python.org/downloads/) (if not installed).
+        
+        - Install **Python SDK**
+            - Navigate to the workspace of your client app.
+            - Run the command below:
+        
+            ```sh
+            pip install zohocrmsdk2_1==1.x.x
+            ```
+        - The Python SDK will be installed in your client application.
+        
+        ## Token Persistence
+        
+        Token persistence refers to storing and utilizing the authentication tokens that are provided by Zoho. There are three ways provided by the SDK in which persistence can be utilized. They are DataBase Persistence, File Persistence and Custom Persistence.
+        
+        ### Table of Contents
+        
+        - [DataBase Persistence](#database-persistence)
+        
+        - [File Persistence](#file-persistence)
+        
+        - [Custom Persistence](#custom-persistence)
+        
+        ### Implementing OAuth Persistence
+        
+        Once the application is authorized, OAuth access and refresh tokens can be used for subsequent user data requests to Zoho CRM. Hence, they need to be persisted by the client app.
+        
+        The persistence is achieved by writing an implementation of the inbuilt Abstract Base Class **[TokenStore](zcrmsdk/src/com/zoho/api/authenticator/store/token_store.py)**, which has the following callback methods.
+        
+        - **get_token(self, user, [token](zcrmsdk/src/com/zoho/api/authenticator/token.py))** - invoked before firing a request to fetch the saved tokens. This method should return implementation of inbuilt **Token Class** object for the library to process it.
+        
+        - **save_token(self, user, [token](zcrmsdk/src/com/zoho/api/authenticator/token.py))** - invoked after fetching access and refresh tokens from Zoho.
+        
+        - **delete_token(self, [token](zcrmsdk/src/com/zoho/api/authenticator/token.py))** - invoked before saving the latest tokens.
+        
+        - **get_tokens(self)** - The method to get the all the stored tokens.
+        
+        - **delete_tokens(self)** - The method to delete all the stored tokens.
+        
+        - **get_token_by_id(self, id, token)** - The method to retrieve the user's token details based on unique ID.
+        
+        Note:
+        
+        - user is an instance of UserSignature Class.
+        
+        - token is an instance of Token Class.
+        
+        ### DataBase Persistence
+        
+        In case the user prefers to use default DataBase persistence, **MySQL** can be used.
+        
+        - The database name should be **zohooauth**.
+        
+        - There must be a table name **oauthtoken** with the following columns.
+        
+          - id int(11)
+        
+          - user_mail varchar(255)
           
-        read_timeout (Default value is None) 
-            A  Float field to set read timeout
-        """
-        config = SDKConfig(auto_refresh_fields=True, pick_list_validation=False, connect_timeout=None, read_timeout=None)
-
-        """
-        The path containing the absolute directory path (in the key resource_path) to store user-specific files containing information about fields in modules. 
-        """
-        resource_path = '/Users/user_name/Documents/python-app'
-
-        """
-        Create an instance of RequestProxy class that takes the following parameters
-        1 -> Host
-        2 -> Port Number
-        3 -> User Name. Default value is None
-        4 -> Password. Default value is None
-        """
-        request_proxy = RequestProxy(host='host', port=8080)
-
-        request_proxy = RequestProxy(host='host', port=8080, user='user', password='password')
-
-        """
-        Call the static initialize method of Initializer class that takes the following arguments
-        1 -> UserSignature instance
-        2 -> Environment instance
-        3 -> Token instance
-        4 -> TokenStore instance
-        5 -> SDKConfig instance
-        6 -> resource_path
-        7 -> Logger instance. Default value is None
-        8 -> RequestProxy instance. Default value is None
-        """
-        Initializer.initialize(user=user, environment=environment, token=token, store=store, sdk_config=config, resource_path=resource_path, logger=logger, proxy=request_proxy)
-
-
-SDKInitializer.initialize()
-
-```
-
-- You can now access the functionalities of the SDK. Refer to the sample codes to make various API calls through the SDK.
-
-## Class Hierarchy
-
-![classdiagram](class_hierarchy.png)
-
-## Responses and Exceptions
-
-All SDK methods return an instance of the APIResponse class.
-
-After a successful API request, the **get_object()** method returns an instance of the **ResponseWrapper** (for **GET**) or the **ActionWrapper** (for **POST, PUT, DELETE**)
-
-Whenever the API returns an error response, the **get_object()** returns an instance of **APIException** class.
-
-**ResponseWrapper** (for **GET** requests) and **ActionWrapper** (for **POST, PUT, DELETE** requests) are the expected objects for Zoho CRM APIs’ responses
-
-However, some specific operations have different expected objects, such as the following:
-
-- Operations involving records in Tags
-    - **RecordActionWrapper**
-
-- Getting Record Count for a specific Tag operation
-    - **CountWrapper**
-
-- Operations involving BaseCurrency
-    - **BaseCurrencyActionWrapper**
-
-- Lead convert operation
-    - **ConvertActionWrapper**
-
-- Retrieving Deleted records operation
-    - **DeletedRecordsWrapper**
-
-- Record image download operation
-    - **FileBodyWrapper**
-
-- MassUpdate record operations
-    - **MassUpdateActionWrapper**
-    - **MassUpdateResponseWrapper**
-  
-### GET Requests
-
-- The **get_object()** returns an instance of one of the following classes, based on the return type.
-
-    - For  **application/json** responses
-        - **ResponseWrapper**
-        - **CountWrapper**
-        - **DeletedRecordsWrapper**
-        - **MassUpdateResponseWrapper**
-        - **APIException**
-
-    - For **file download** responses
-        - **FileBodyWrapper**
-        - **APIException**
-
-### POST, PUT, DELETE Requests
-
-- The **getObject()** returns an instance of one of the following classes
-    - **ActionWrapper**
-    - **RecordActionWrapper**
-    - **BaseCurrencyActionWrapper**
-    - **MassUpdateActionWrapper**
-    - **ConvertActionWrapper**
-    - **APIException**
-
-- These wrapper classes may contain one or a list of instances of the following classes, depending on the response.
-    - **SuccessResponse Class**, if the request was successful.
-    - **APIException Class**, if the request was erroneous.
-
-For example, when you insert two records, and one of them was inserted successfully while the other one failed, the ActionWrapper will contain one instance each of the SuccessResponse and APIException classes.
-
-All other exceptions such as SDK anomalies and other unexpected behaviours are thrown under the SDKException class.
-
-## Threading in the Python SDK
-
-Threads in a Python program help you achieve parallelism. By using multiple threads, you can make a Python program run faster and do multiple things simultaneously.
-
-The **Python SDK** (from version 3.x.x) supports both single-user and multi-user app.
-
-### Multithreading in a Multi-user App
-
-Multi-threading for multi-users is achieved using Initializer's static **switch_user()** method.
-switch_user() takes the value initialized previously for user, enviroment, token and sdk_config incase None is passed (or default value is passed). In case of request_proxy, if intended, the value has to be passed again else None(default value) will be taken.
-
-```python
-# without proxy
-Initializer.switch_user(user=user, environment=environment, token=token, sdk_config=sdk_config_instance)
-
-# with proxy
-Initializer.switch_user(user=user, environment=environment, token=token, sdk_config=sdk_config_instance, proxy=request_proxy)
-```
-
-Here is a sample code to depict multi-threading for a multi-user app.
-
-```python
-import threading
-from zcrmsdk.src.com.zoho.crm.api.user_signature import UserSignature
-from zcrmsdk.src.com.zoho.crm.api.dc import USDataCenter, EUDataCenter
-from zcrmsdk.src.com.zoho.api.authenticator.store import DBStore
-from zcrmsdk.src.com.zoho.api.logger import Logger
-from zcrmsdk.src.com.zoho.crm.api.initializer import Initializer
-from zcrmsdk.src.com.zoho.api.authenticator.oauth_token import OAuthToken
-from zcrmsdk.src.com.zoho.crm.api.record import *
-from zcrmsdk.src.com.zoho.crm.api.request_proxy import RequestProxy
-from zcrmsdk.src.com.zoho.crm.api.sdk_config import SDKConfig
-
-
-class MultiThread(threading.Thread):
-
-    def __init__(self, environment, token, user, module_api_name, sdk_config, proxy=None):
-        super().__init__()
-        self.environment = environment
-        self.token = token
-        self.user = user
-        self.module_api_name = module_api_name
-        self.sdk_config = sdk_config
-        self.proxy = proxy
-
-    def run(self):
-        try:
-            Initializer.switch_user(user=self.user, environment=self.environment, token=self.token, sdk_config=self.sdk_config, proxy=self.proxy)
-
-            print('Getting records for User: ' + Initializer.get_initializer().user.get_email())
-
-            response = RecordOperations().get_records(self.module_api_name)
-
-            if response is not None:
-
-                # Get the status code from response
-                print('Status Code: ' + str(response.get_status_code()))
-
-                if response.get_status_code() in [204, 304]:
-                    print('No Content' if response.get_status_code() == 204 else 'Not Modified')
-                    return
-
-                # Get object from response
-                response_object = response.get_object()
-
-                if response_object is not None:
-
-                    # Check if expected ResponseWrapper instance is received.
-                    if isinstance(response_object, ResponseWrapper):
-                        # Get the list of obtained Record instances
-                        record_list = response_object.get_data()
-
-                        for record in record_list:
-                            for key, value in record.get_key_values().items():
-                                print(key + " : " + str(value))
-
-                    # Check if the request returned an exception
-                    elif isinstance(response_object, APIException):
-                        # Get the Status
-                        print("Status: " + response_object.get_status().get_value())
-
-                        # Get the Code
-                        print("Code: " + response_object.get_code().get_value())
-
-                        print("Details")
-
-                        # Get the details dict
-                        details = response_object.get_details()
-
-                        for key, value in details.items():
-                            print(key + ' : ' + str(value))
-
-                        # Get the Message
-                        print("Message: " + response_object.get_message().get_value())
-
-        except Exception as e:
-            print(e)
-
-    @staticmethod
-    def call():
-        logger = Logger.get_instance(level=Logger.Levels.INFO, file_path="/Users/user_name/Documents/python_sdk_log.log")
-
-        user1 = UserSignature(email="abc@zoho.com")
-
-        token1 = OAuthToken(client_id="clientId1", client_secret="clientSecret1", grant_token="Grant Token", refresh_token="refresh_token", id="id")
-
-        environment1 = USDataCenter.PRODUCTION()
-
-        store = DBStore()
-
-        sdk_config_1 = SDKConfig(auto_refresh_fields=True, pick_list_validation=False)
-
-        resource_path = '/Users/user_name/Documents/python-app'
-
-        user1_module_api_name = 'Leads'
-
-        user2_module_api_name = 'Contacts'
-
-        environment2 = EUDataCenter.SANDBOX()
-
-        user2 = UserSignature(email="abc@zoho.eu")
-
-        sdk_config_2 = SDKConfig(auto_refresh_fields=False, pick_list_validation=True)
-
-        token2 = OAuthToken(client_id="clientId2", client_secret="clientSecret2",grant_token="GRANT Token", refresh_token="refresh_token", redirect_url="redirectURL", id="id")
-
-        request_proxy_user_2 = RequestProxy("host", 8080)
-
-        Initializer.initialize(user=user1, environment=environment1, token=token1, store=store, sdk_config=sdk_config_1, resource_path=resource_path, logger=logger)
-
-        t1 = MultiThread(environment1, token1, user1, user1_module_api_name, sdk_config_1)
-        t2 = MultiThread(environment2, token2, user2, user2_module_api_name, sdk_config_2, request_proxy_user_2)
-
-        t1.start()
-        t2.start()
-
-        t1.join()
-        t2.join()
-
-
-MultiThread.call()
-
-```
-
-- The program execution starts from **call()**.
-
-- The details of **user1** are given in the variables user1, token1, environment1.
-
-- Similarly, the details of another user **user2** are given in the variables user2, token2, environment2.
-
-- For each user, an instance of **MultiThread class** is created.
-
-- When the **start()** is called which in-turn invokes the **run()**,  the details of user1 are passed to the **switch_user** method through the **MultiThread object**. Therefore, this creates a thread for user1.
-
-- Similarly, When the **start()** is invoked again,  the details of user2 are passed to the **switch_user** function through the **MultiThread object**. Therefore, this creates a thread for user2.
-
-### Multi-threading in a Single User App
-
-Here is a sample code to depict multi-threading for a single-user app.
-
-```python
-import threading
-from zcrmsdk.src.com.zoho.crm.api.user_signature import UserSignature
-from zcrmsdk.src.com.zoho.crm.api.dc import USDataCenter
-from zcrmsdk.src.com.zoho.api.authenticator.store import DBStore
-from zcrmsdk.src.com.zoho.api.logger import Logger
-from zcrmsdk.src.com.zoho.crm.api.initializer import Initializer
-from zcrmsdk.src.com.zoho.api.authenticator.oauth_token import OAuthToken
-from zcrmsdk.src.com.zoho.crm.api.sdk_config import SDKConfig
-from zcrmsdk.src.com.zoho.crm.api.record import *
-
-
-class MultiThread(threading.Thread):
-
-    def __init__(self, module_api_name):
-        super().__init__()
-        self.module_api_name = module_api_name
-
-    def run(self):
-        try:
-            print("Calling Get Records for module: " + self.module_api_name)
-
-            response = RecordOperations().get_records(self.module_api_name)
-
-            if response is not None:
-
-                # Get the status code from response
-                print('Status Code: ' + str(response.get_status_code()))
-
-                if response.get_status_code() in [204, 304]:
-                    print('No Content' if response.get_status_code() == 204 else 'Not Modified')
-                    return
-
-                # Get object from response
-                response_object = response.get_object()
-
-                if response_object is not None:
-
-                    # Check if expected ResponseWrapper instance is received.
-                    if isinstance(response_object, ResponseWrapper):
-                        # Get the list of obtained Record instances
-                        record_list = response_object.get_data()
-
-                        for record in record_list:
-                            for key, value in record.get_key_values().items():
-                                print(key + " : " + str(value))
-
-                    # Check if the request returned an exception
-                    elif isinstance(response_object, APIException):
-                        # Get the Status
-                        print("Status: " + response_object.get_status().get_value())
-
-                        # Get the Code
-                        print("Code: " + response_object.get_code().get_value())
-
-                        print("Details")
-
-                        # Get the details dict
-                        details = response_object.get_details()
-
-                        for key, value in details.items():
-                            print(key + ' : ' + str(value))
-
-                        # Get the Message
-                        print("Message: " + response_object.get_message().get_value())
-
-        except Exception as e:
-            print(e)
-
-    @staticmethod
-    def call():
-        logger = Logger.get_instance(level=Logger.Levels.INFO, file_path="/Users/user_name/Documents/python_sdk_log.log")
-
-        user = UserSignature(email="abc@zoho.com")
-
-        token = OAuthToken(client_id="clientId", client_secret="clientSecret", grant_token="grant_token", refresh_token="refresh_token", redirect_url="redirectURL", id="id")
-
-        environment = USDataCenter.PRODUCTION()
-
-        store = DBStore()
-
-        sdk_config = SDKConfig()
-
-        resource_path = '/Users/user_name/Documents/python-app'
-
-        Initializer.initialize(user=user, environment=environment, token=token, store=store, sdk_config=sdk_config, resource_path=resource_path, logger=logger)
-
-        t1 = MultiThread('Leads')
-        t2 = MultiThread('Quotes')
-
-        t1.start()
-        t2.start()
-
-        t1.join()
-        t2.join()
-
-
-MultiThread.call()
-```
-
-- The program execution starts from **call()** where the SDK is initialized with the details of the user.
-
-- When the **start()** is called which in-turn invokes the run(),  the module_api_name is switched through the MultiThread object. Therefore, this creates a thread for the particular MultiThread instance.
-
-## SDK Sample code
-
-```python
-from datetime import datetime
-from zcrmsdk.src.com.zoho.crm.api.user_signature import UserSignature
-from zcrmsdk.src.com.zoho.crm.api.dc import USDataCenter
-from zcrmsdk.src.com.zoho.api.authenticator.store import DBStore
-from zcrmsdk.src.com.zoho.api.logger import Logger
-from zcrmsdk.src.com.zoho.crm.api.initializer import Initializer
-from zcrmsdk.src.com.zoho.api.authenticator.oauth_token import OAuthToken
-from zcrmsdk.src.com.zoho.crm.api.record import *
-from zcrmsdk.src.com.zoho.crm.api import HeaderMap, ParameterMap
-from zcrmsdk.src.com.zoho.crm.api.sdk_config import SDKConfig
-
-
-class Record(object):
-
-    def __init__(self):
-        pass
-
-    @staticmethod
-    def get_records():
-
-        """
-        Create an instance of Logger Class that takes two parameters
-        1 -> Level of the log messages to be logged. Can be configured by typing Logger.Levels "." and choose any level from the list displayed.
-        2 -> Absolute file path, where messages need to be logged.
-        """
-        logger = Logger.get_instance(level=Logger.Levels.INFO,
-                                     file_path="/Users/user_name/Documents/python_sdk_log.log")
-
-        # Create an UserSignature instance that takes user Email as parameter
-        user = UserSignature(email="abc@zoho.com")
-
-        """
-        Configure the environment
-        which is of the pattern Domain.Environment
-        Available Domains: USDataCenter, EUDataCenter, INDataCenter, CNDataCenter, AUDataCenter
-        Available Environments: PRODUCTION(), DEVELOPER(), SANDBOX()
-        """
-        environment = USDataCenter.PRODUCTION()
-
-        """
-        Create a Token instance that takes the following parameters
-        1 -> OAuth client id.
-        2 -> OAuth client secret.
-        3 -> Grant token.
-        4 -> Refresh token.
-        5 -> OAuth redirect URL.
-        6 -> id
-        """
-        token = OAuthToken(client_id="clientId", client_secret="clientSecret", grant_token="grant_token", refresh_token="refresh_token", redirect_url="redirectURL", id="id")
-
+          - client_id varchar(255)
+          
+          - client_secret varchar(255)
+        
+          - refresh_token varchar(255)
+        
+          - access_token varchar(255)
+        
+          - grant_token varchar(255)
+        
+          - expiry_time varchar(20)
+          
+          - redirect_url varchar(255)
+        
+        Note:
+        - Custom database name and table name can be set in DBStore instance.
+        
+        #### MySQL Query
+        
+        ```sql
+        CREATE TABLE  oauthtoken (
+          id varchar(255) NOT NULL,
+          user_mail varchar(255) NOT NULL,
+          client_id varchar(255),
+          client_secret varchar(255),
+          refresh_token varchar(255),
+          access_token varchar(255),
+          grant_token varchar(255),
+          expiry_time varchar(20),
+          redirect_url varchar(255),
+          primary key (id)
+        )
+        ```
+        
+        #### Create DBStore object
+        
+        ```python
+        from zcrmsdk.src.com.zoho.api.authenticator.store import DBStore
         """
-        Create an instance of TokenStore
+        DBStore takes the following parameters
         1 -> DataBase host name. Default value "localhost"
         2 -> DataBase name. Default value "zohooauth"
         3 -> DataBase user name. Default value "root"
         4 -> DataBase password. Default value ""
         5 -> DataBase port number. Default value "3306"
         6->  DataBase table name . Default value "oauthtoken"
         """
         store = DBStore()
-
+        
+        store = DBStore(host='host_name', database_name='database_name', user_name='user_name', password='password', port_number='port_number', table_name = "table_name")
+        ```
+        
+        ### File Persistence
+        
+        In case of File Persistence, the user can persist tokens in the local drive, by providing the absolute file path to the FileStore object.
+        
+        - The File contains
+            - id 
+            
+            - user_mail
+        
+            - client_id
+            
+            - client_secret
+        
+            - refresh_token
+        
+            - access_token
+        
+            - grant_token
+        
+            - expiry_time
+            
+            - redirect_url
+        
+        #### Create FileStore object
+        
+        ```python
+        from zcrmsdk.src.com.zoho.api.authenticator.store import FileStore
+        """
+        FileStore takes the following parameter
+        1 -> Absolute file path of the file to persist tokens
         """
-        auto_refresh_fields (Default value is False)
+        store = FileStore(file_path='/Users/username/Documents/python_sdk_token.txt')
+        ```
+        
+        ### Custom Persistence
+        To use Custom Persistence, you must implement **[TokenStore](zcrmsdk/src/com/zoho/api/authenticator/store/token_store.py)** and override the methods.
+        
+        ```python
+        from zcrmsdk.src.com.zoho.api.authenticator.store import TokenStore
+        
+        
+        class CustomStore(TokenStore):
+        
+            def __init__(self):
+                pass
+        
+            def get_token(self, user, token):
+        
+                """
+                Parameters:
+                    user (UserSignature) : A UserSignature class instance.
+                    token (Token) : A Token (zcrmsdk.src.com.zoho.api.authenticator.OAuthToken) class instance
+                """
+        
+                # Add code to get the token
+                return None
+        
+            def save_token(self, user, token):
+        
+                """
+                Parameters:
+                    user (UserSignature) : A UserSignature class instance.
+                    token (Token) : A Token (zcrmsdk.src.com.zoho.api.authenticator.OAuthToken) class instance
+                """
+        
+                # Add code to save the token
+        
+            def delete_token(self, token):
+        
+                """
+                Parameters:
+                    token (Token) : A Token (zcrmsdk.src.com.zoho.api.authenticator.OAuthToken) class instance
+                """
+        
+                # Add code to delete the token
+            
+            def get_tokens(self):
+        
+                """
+                Returns:
+                    list: List of stored tokens
+                """
+        
+                # Add code to get all the stored tokens
+            
+            def delete_tokens(self):
+        
+                # Add code to delete all the stored tokens
+            
+            def get_token_by_id(id, token):
+                
+                """
+                The method to get id token details.
+        
+                Parameters:
+                    id (String) : A String id.
+                    token (Token) : A Token class instance.
+        
+                Returns:
+                    Token : A Token class instance representing the id token details.
+                """
+        ```
+        
+        ## Configuration
+        
+        Before you get started with creating your Python application, you need to register your client and authenticate the app with Zoho.
+        
+        | Mandatory Keys    | Optional Keys |
+        | :---------------- | :------------ |
+        | user              | logger        |
+        | environment       | store         |
+        | token             | sdk_config    |
+        |                   | proxy         |
+        |                   | resource_path |
+        ----
+        
+        - Create an instance of **UserSignature** Class that identifies the current user.
+          ```python
+          from zcrmsdk.src.com.zoho.crm.api.user_signature import UserSignature
+        
+          # Create an UserSignature instance that takes user Email as parameter
+          user = UserSignature(email='abc@zoho.com')
+          ```
+        
+        - Configure the API environment which decides the domain and the URL to make API calls.
+          ```python
+          from zcrmsdk.src.com.zoho.crm.api.dc import USDataCenter
+        
+          """
+          Configure the environment
+          which is of the pattern Domain.Environment
+          Available Domains: USDataCenter, EUDataCenter, INDataCenter, CNDataCenter, AUDataCenter
+          Available Environments: PRODUCTION(), DEVELOPER(), SANDBOX()
+          """
+          environment = USDataCenter.PRODUCTION()
+          ```
+        
+        - Create an instance of **OAuthToken** with the information that you get after registering your Zoho client.
+          ```python
+          from zcrmsdk.src.com.zoho.api.authenticator.oauth_token import OAuthToken
+        
+          """
+          Create a Token instance that takes the following parameters
+          1 -> OAuth client id.
+          2 -> OAuth client secret.
+          3 -> Grant token.
+          4 -> Refresh token.
+          5 -> OAuth redirect URL. Default value is None
+          6 -> id
+          7 -> Access token
+          """
+          token = OAuthToken(client_id='clientId', client_secret='clientSecret', grant_token='grant_token', refresh_token="refresh_token", redirect_url='redirectURL', id="id", access_token="access_token")
+          ```
+        
+        - Create an instance of **Logger** Class to log exception and API information. By default, the SDK constructs a Logger instance with level - INFO and file_path - (sdk_logs.log, created in the current working directory)
+          ```python
+            from zcrmsdk.src.com.zoho.api.logger import Logger
+          
+            """
+            Create an instance of Logger Class that takes two parameters
+            1 -> Level of the log messages to be logged. Can be configured by typing Logger.Levels "." and choose any level from the list displayed.
+            2 -> Absolute file path, where messages need to be logged.
+            """
+            logger = Logger.get_instance(level=Logger.Levels.INFO, file_path="/Users/user_name/Documents/python_sdk_log.log")
+            ```
+        
+        - Create an instance of **TokenStore** to persist tokens, used for authenticating all the requests. By default, the SDK creates the sdk_tokens.txt created in the current working directory) to persist the tokens.
+          ```python
+          from zcrmsdk.src.com.zoho.api.authenticator.store import DBStore, FileStore
+        
+          """
+          DBStore takes the following parameters
+          1 -> DataBase host name. Default value "localhost"
+          2 -> DataBase name. Default value "zohooauth"
+          3 -> DataBase user name. Default value "root"
+          4 -> DataBase password. Default value ""
+          5 -> DataBase port number. Default value "3306"
+          6 -> DataBase table name. Default value "oauthtoken"
+          """
+          store = DBStore()
+        
+          #store = DBStore(host='host_name', database_name='database_name', user_name='user_name', password='password', port_number='port_number', table_name = "table_name")
+        
+          """
+          FileStore takes the following parameter
+          1 -> Absolute file path of the file to persist tokens
+          """
+          #store = FileStore(file_path='/Users/username/Documents/python_sdk_tokens.txt')
+          ```
+        
+        - Create an instance of SDKConfig containing SDK configurations.
+          ```python
+          from zcrmsdk.src.com.zoho.crm.api.sdk_config import SDKConfig
+        
+          """
+          By default, the SDK creates the SDKConfig instance
+          auto_refresh_fields (Default value is False)
             if True - all the modules' fields will be auto-refreshed in the background, every hour.
             if False - the fields will not be auto-refreshed in the background. The user can manually delete the file(s) or refresh the fields using methods from ModuleFieldsHandler(zcrmsdk/src/com/zoho/crm/api/util/module_fields_handler.py)
-
-        pick_list_validation (Default value is True)
+        
+          pick_list_validation (Default value is True)
             A boolean field that validates user input for a pick list field and allows or disallows the addition of a new value to the list.
             if True - the SDK validates the input. If the value does not exist in the pick list, the SDK throws an error.
             if False - the SDK does not validate the input and makes the API request with the user’s input to the pick list
-         connect_timeout (Default value is None) 
+          
+          connect_timeout (Default value is None) 
             A  Float field to set connect timeout
-  
-         read_timeout (Default value is None) 
+          
+          read_timeout (Default value is None) 
             A  Float field to set read timeout
-         """
-        config = SDKConfig(auto_refresh_fields=True, pick_list_validation=False, connect_timeout=None, read_timeout=None)
-
-        """
-        The path containing the absolute directory path (in the key resource_path) to store user-specific files containing information about fields in modules. 
-        """
-        resource_path = '/Users/user_name/Documents/python-app'
-
-        """
-        Call the static initialize method of Initializer class that takes the following arguments
-        1 -> UserSignature instance
-        2 -> Environment instance
-        3 -> Token instance
-        4 -> TokenStore instance
-        5 -> SDKConfig instance
-        6 -> resource_path
-        7 -> Logger instance
-        """
-        Initializer.initialize(user=user, environment=environment, token=token, store=store, sdk_config=config, resource_path=resource_path, logger=logger)
-
-        try:
-            module_api_name = 'Leads'
-
-            param_instance = ParameterMap()
-
-            param_instance.add(GetRecordsParam.converted, 'both')
-
-            param_instance.add(GetRecordsParam.cvid, '12712717217218')
-
-            header_instance = HeaderMap()
-
-            header_instance.add(GetRecordsHeader.if_modified_since, datetime.now())
-
-            response = RecordOperations().get_records(module_api_name, param_instance, header_instance)
-
-            if response is not None:
-
-                # Get the status code from response
-                print('Status Code: ' + str(response.get_status_code()))
-
-                if response.get_status_code() in [204, 304]:
-                    print('No Content' if response.get_status_code() == 204 else 'Not Modified')
-                    return
-
-                # Get object from response
-                response_object = response.get_object()
-
-                if response_object is not None:
-
-                    # Check if expected ResponseWrapper instance is received.
-                    if isinstance(response_object, ResponseWrapper):
-                        # Get the list of obtained Record instances
-                        record_list = response_object.get_data()
-
-                        for record in record_list:
-
-                            # Get the ID of each Record
-                            print("Record ID: " + record.get_id())
-
-                            # Get the createdBy User instance of each Record
-                            created_by = record.get_created_by()
-
-                            # Check if created_by is not None
-                            if created_by is not None:
-                                # Get the Name of the created_by User
-                                print("Record Created By - Name: " + created_by.get_name())
-
-                                # Get the ID of the created_by User
-                                print("Record Created By - ID: " + created_by.get_id())
-
-                                # Get the Email of the created_by User
-                                print("Record Created By - Email: " + created_by.get_email())
-
-                            # Get the CreatedTime of each Record
-                            print("Record CreatedTime: " + str(record.get_created_time()))
-
-                            if record.get_modified_time() is not None:
-                                # Get the ModifiedTime of each Record
-                                print("Record ModifiedTime: " + str(record.get_modified_time()))
-
-                            # Get the modified_by User instance of each Record
-                            modified_by = record.get_modified_by()
-
-                            # Check if modified_by is not None
-                            if modified_by is not None:
-                                # Get the Name of the modified_by User
-                                print("Record Modified By - Name: " + modified_by.get_name())
-
-                                # Get the ID of the modified_by User
-                                print("Record Modified By - ID: " + modified_by.get_id())
-
-                                # Get the Email of the modified_by User
-                                print("Record Modified By - Email: " + modified_by.get_email())
-
-                            # Get the list of obtained Tag instance of each Record
-                            tags = record.get_tag()
-
-                            if tags is not None:
-                                for tag in tags:
-                                    # Get the Name of each Tag
-                                    print("Record Tag Name: " + tag.get_name())
-
-                                    # Get the Id of each Tag
-                                    print("Record Tag ID: " + tag.get_id())
-
-                            # To get particular field value
-                            print("Record Field Value: " + str(record.get_key_value('Last_Name')))
-
-                            print('Record KeyValues: ')
-
-                            for key, value in record.get_key_values().items():
-                                print(key + " : " + str(value))
-
-                    # Check if the request returned an exception
-                    elif isinstance(response_object, APIException):
-                        # Get the Status
-                        print("Status: " + response_object.get_status().get_value())
-
-                        # Get the Code
-                        print("Code: " + response_object.get_code().get_value())
-
-                        print("Details")
-
-                        # Get the details dict
-                        details = response_object.get_details()
-
-                        for key, value in details.items():
-                            print(key + ' : ' + str(value))
-
-                        # Get the Message
-                        print("Message: " + response_object.get_message().get_value())
-
-        except Exception as e:
-            print(e)
-
-
-Record.get_records()
-```
+          """
+          config = SDKConfig(auto_refresh_fields=True, pick_list_validation=False, connect_timeout=None, read_timeout=None)
+          ```
+        
+        - The path containing the absolute directory path to store user specific files containing module fields information. By default, the SDK stores the user-specific files within a folder in the current working directory.
+          ```python
+          resource_path = '/Users/user_name/Documents/python-app'
+          ```
+        
+        - Create an instance of RequestProxy containing the proxy properties of the user.
+            ```python
+            from zcrmsdk.src.com.zoho.crm.api.request_proxy import RequestProxy
+        
+            """
+            RequestProxy takes the following parameters
+            1 -> Host
+            2 -> Port Number
+            3 -> User Name. Default value is None
+            4 -> Password. Default value is an empty string
+            """
+            request_proxy = RequestProxy(host='proxyHost', port=80)
+            request_proxy = RequestProxy(host='proxyHost', port=80, user='userName', password='password')
+            ```
+        
+        ## Initializing the Application
+        
+        Initialize the SDK using the following code.
+        
+        ```python
+        from zcrmsdk.src.com.zoho.crm.api.user_signature import UserSignature
+        from zcrmsdk.src.com.zoho.crm.api.dc import USDataCenter
+        from zcrmsdk.src.com.zoho.api.authenticator.store import DBStore, FileStore
+        from zcrmsdk.src.com.zoho.api.logger import Logger
+        from zcrmsdk.src.com.zoho.crm.api.initializer import Initializer
+        from zcrmsdk.src.com.zoho.api.authenticator.oauth_token import OAuthToken
+        from zcrmsdk.src.com.zoho.crm.api.sdk_config import SDKConfig
+        
+        
+        class SDKInitializer(object):
+        
+            @staticmethod
+            def initialize():
+        
+                """
+                Create an instance of Logger Class that takes two parameters
+                1 -> Level of the log messages to be logged. Can be configured by typing Logger.Levels "." and choose any level from the list displayed.
+                2 -> Absolute file path, where messages need to be logged.
+                """
+                logger = Logger.get_instance(level=Logger.Levels.INFO, file_path='/Users/user_name/Documents/python_sdk_log.log')
+        
+                # Create an UserSignature instance that takes user Email as parameter
+                user = UserSignature(email='abc@zoho.com')
+        
+                """
+                Configure the environment
+                which is of the pattern Domain.Environment
+                Available Domains: USDataCenter, EUDataCenter, INDataCenter, CNDataCenter, AUDataCenter
+                Available Environments: PRODUCTION(), DEVELOPER(), SANDBOX()
+                """
+                environment = USDataCenter.PRODUCTION()
+        
+                """
+                Create a Token instance that takes the following parameters
+                1 -> OAuth client id.
+                2 -> OAuth client secret.
+                3 -> Grant token.
+                4 -> Refresh token.
+                5 -> OAuth redirect URL.
+                6 -> id
+                """
+                token = OAuthToken(client_id='clientId', client_secret='clientSecret', grant_token='grant_token', refresh_token="refresh_token", redirect_url='redirectURL', id="id")
+        
+                """
+                Create an instance of TokenStore
+                1 -> Absolute file path of the file to persist tokens
+                """
+                store = FileStore(file_path='/Users/username/Documents/python_sdk_tokens.txt')
+        
+                """
+                Create an instance of TokenStore
+                1 -> DataBase host name. Default value "localhost"
+                2 -> DataBase name. Default value "zohooauth"
+                3 -> DataBase user name. Default value "root"
+                4 -> DataBase password. Default value ""
+                5 -> DataBase port number. Default value "3306"
+                6->  DataBase table name . Default value "oauthtoken"
+                """
+                store = DBStore()
+                store = DBStore(host='host_name', database_name='database_name', user_name='user_name', password='password',port_number='port_number', table_name = "table_name")
+        
+                """
+                auto_refresh_fields (Default value is False)
+                    if True - all the modules' fields will be auto-refreshed in the background, every hour.
+                    if False - the fields will not be auto-refreshed in the background. The user can manually delete the file(s) or refresh the fields using methods from ModuleFieldsHandler(zcrmsdk/src/com/zoho/crm/api/util/module_fields_handler.py)
+        
+                pick_list_validation (Default value is True)
+                A boolean field that validates user input for a pick list field and allows or disallows the addition of a new value to the list.
+                    if True - the SDK validates the input. If the value does not exist in the pick list, the SDK throws an error.
+                    if False - the SDK does not validate the input and makes the API request with the user’s input to the pick list
+        
+                connect_timeout (Default value is None) 
+                    A  Float field to set connect timeout
+                  
+                read_timeout (Default value is None) 
+                    A  Float field to set read timeout
+                """
+                config = SDKConfig(auto_refresh_fields=True, pick_list_validation=False, connect_timeout=None, read_timeout=None)
+        
+                """
+                The path containing the absolute directory path (in the key resource_path) to store user-specific files containing information about fields in modules. 
+                """
+                resource_path = '/Users/user_name/Documents/python-app'
+        
+                """
+                Create an instance of RequestProxy class that takes the following parameters
+                1 -> Host
+                2 -> Port Number
+                3 -> User Name. Default value is None
+                4 -> Password. Default value is None
+                """
+                request_proxy = RequestProxy(host='host', port=8080)
+        
+                request_proxy = RequestProxy(host='host', port=8080, user='user', password='password')
+        
+                """
+                Call the static initialize method of Initializer class that takes the following arguments
+                1 -> UserSignature instance
+                2 -> Environment instance
+                3 -> Token instance
+                4 -> TokenStore instance
+                5 -> SDKConfig instance
+                6 -> resource_path
+                7 -> Logger instance. Default value is None
+                8 -> RequestProxy instance. Default value is None
+                """
+                Initializer.initialize(user=user, environment=environment, token=token, store=store, sdk_config=config, resource_path=resource_path, logger=logger, proxy=request_proxy)
+        
+        
+        SDKInitializer.initialize()
+        
+        ```
+        
+        - You can now access the functionalities of the SDK. Refer to the sample codes to make various API calls through the SDK.
+        
+        ## Class Hierarchy
+        
+        ![classdiagram](class_hierarchy.png)
+        
+        ## Responses and Exceptions
+        
+        All SDK methods return an instance of the APIResponse class.
+        
+        After a successful API request, the **get_object()** method returns an instance of the **ResponseWrapper** (for **GET**) or the **ActionWrapper** (for **POST, PUT, DELETE**)
+        
+        Whenever the API returns an error response, the **get_object()** returns an instance of **APIException** class.
+        
+        **ResponseWrapper** (for **GET** requests) and **ActionWrapper** (for **POST, PUT, DELETE** requests) are the expected objects for Zoho CRM APIs’ responses
+        
+        However, some specific operations have different expected objects, such as the following:
+        
+        - Operations involving records in Tags
+            - **RecordActionWrapper**
+        
+        - Getting Record Count for a specific Tag operation
+            - **CountWrapper**
+        
+        - Operations involving BaseCurrency
+            - **BaseCurrencyActionWrapper**
+        
+        - Lead convert operation
+            - **ConvertActionWrapper**
+        
+        - Retrieving Deleted records operation
+            - **DeletedRecordsWrapper**
+        
+        - Record image download operation
+            - **FileBodyWrapper**
+        
+        - MassUpdate record operations
+            - **MassUpdateActionWrapper**
+            - **MassUpdateResponseWrapper**
+          
+        ### GET Requests
+        
+        - The **get_object()** returns an instance of one of the following classes, based on the return type.
+        
+            - For  **application/json** responses
+                - **ResponseWrapper**
+                - **CountWrapper**
+                - **DeletedRecordsWrapper**
+                - **MassUpdateResponseWrapper**
+                - **APIException**
+        
+            - For **file download** responses
+                - **FileBodyWrapper**
+                - **APIException**
+        
+        ### POST, PUT, DELETE Requests
+        
+        - The **getObject()** returns an instance of one of the following classes
+            - **ActionWrapper**
+            - **RecordActionWrapper**
+            - **BaseCurrencyActionWrapper**
+            - **MassUpdateActionWrapper**
+            - **ConvertActionWrapper**
+            - **APIException**
+        
+        - These wrapper classes may contain one or a list of instances of the following classes, depending on the response.
+            - **SuccessResponse Class**, if the request was successful.
+            - **APIException Class**, if the request was erroneous.
+        
+        For example, when you insert two records, and one of them was inserted successfully while the other one failed, the ActionWrapper will contain one instance each of the SuccessResponse and APIException classes.
+        
+        All other exceptions such as SDK anomalies and other unexpected behaviours are thrown under the SDKException class.
+        
+        ## Threading in the Python SDK
+        
+        Threads in a Python program help you achieve parallelism. By using multiple threads, you can make a Python program run faster and do multiple things simultaneously.
+        
+        The **Python SDK** (from version 3.x.x) supports both single-user and multi-user app.
+        
+        ### Multithreading in a Multi-user App
+        
+        Multi-threading for multi-users is achieved using Initializer's static **switch_user()** method.
+        switch_user() takes the value initialized previously for user, enviroment, token and sdk_config incase None is passed (or default value is passed). In case of request_proxy, if intended, the value has to be passed again else None(default value) will be taken.
+        
+        ```python
+        # without proxy
+        Initializer.switch_user(user=user, environment=environment, token=token, sdk_config=sdk_config_instance)
+        
+        # with proxy
+        Initializer.switch_user(user=user, environment=environment, token=token, sdk_config=sdk_config_instance, proxy=request_proxy)
+        ```
+        
+        Here is a sample code to depict multi-threading for a multi-user app.
+        
+        ```python
+        import threading
+        from zcrmsdk.src.com.zoho.crm.api.user_signature import UserSignature
+        from zcrmsdk.src.com.zoho.crm.api.dc import USDataCenter, EUDataCenter
+        from zcrmsdk.src.com.zoho.api.authenticator.store import DBStore
+        from zcrmsdk.src.com.zoho.api.logger import Logger
+        from zcrmsdk.src.com.zoho.crm.api.initializer import Initializer
+        from zcrmsdk.src.com.zoho.api.authenticator.oauth_token import OAuthToken
+        from zcrmsdk.src.com.zoho.crm.api.record import *
+        from zcrmsdk.src.com.zoho.crm.api.request_proxy import RequestProxy
+        from zcrmsdk.src.com.zoho.crm.api.sdk_config import SDKConfig
+        
+        
+        class MultiThread(threading.Thread):
+        
+            def __init__(self, environment, token, user, module_api_name, sdk_config, proxy=None):
+                super().__init__()
+                self.environment = environment
+                self.token = token
+                self.user = user
+                self.module_api_name = module_api_name
+                self.sdk_config = sdk_config
+                self.proxy = proxy
+        
+            def run(self):
+                try:
+                    Initializer.switch_user(user=self.user, environment=self.environment, token=self.token, sdk_config=self.sdk_config, proxy=self.proxy)
+        
+                    print('Getting records for User: ' + Initializer.get_initializer().user.get_email())
+        
+                    response = RecordOperations().get_records(self.module_api_name)
+        
+                    if response is not None:
+        
+                        # Get the status code from response
+                        print('Status Code: ' + str(response.get_status_code()))
+        
+                        if response.get_status_code() in [204, 304]:
+                            print('No Content' if response.get_status_code() == 204 else 'Not Modified')
+                            return
+        
+                        # Get object from response
+                        response_object = response.get_object()
+        
+                        if response_object is not None:
+        
+                            # Check if expected ResponseWrapper instance is received.
+                            if isinstance(response_object, ResponseWrapper):
+                                # Get the list of obtained Record instances
+                                record_list = response_object.get_data()
+        
+                                for record in record_list:
+                                    for key, value in record.get_key_values().items():
+                                        print(key + " : " + str(value))
+        
+                            # Check if the request returned an exception
+                            elif isinstance(response_object, APIException):
+                                # Get the Status
+                                print("Status: " + response_object.get_status().get_value())
+        
+                                # Get the Code
+                                print("Code: " + response_object.get_code().get_value())
+        
+                                print("Details")
+        
+                                # Get the details dict
+                                details = response_object.get_details()
+        
+                                for key, value in details.items():
+                                    print(key + ' : ' + str(value))
+        
+                                # Get the Message
+                                print("Message: " + response_object.get_message().get_value())
+        
+                except Exception as e:
+                    print(e)
+        
+            @staticmethod
+            def call():
+                logger = Logger.get_instance(level=Logger.Levels.INFO, file_path="/Users/user_name/Documents/python_sdk_log.log")
+        
+                user1 = UserSignature(email="abc@zoho.com")
+        
+                token1 = OAuthToken(client_id="clientId1", client_secret="clientSecret1", grant_token="Grant Token", refresh_token="refresh_token", id="id")
+        
+                environment1 = USDataCenter.PRODUCTION()
+        
+                store = DBStore()
+        
+                sdk_config_1 = SDKConfig(auto_refresh_fields=True, pick_list_validation=False)
+        
+                resource_path = '/Users/user_name/Documents/python-app'
+        
+                user1_module_api_name = 'Leads'
+        
+                user2_module_api_name = 'Contacts'
+        
+                environment2 = EUDataCenter.SANDBOX()
+        
+                user2 = UserSignature(email="abc@zoho.eu")
+        
+                sdk_config_2 = SDKConfig(auto_refresh_fields=False, pick_list_validation=True)
+        
+                token2 = OAuthToken(client_id="clientId2", client_secret="clientSecret2",grant_token="GRANT Token", refresh_token="refresh_token", redirect_url="redirectURL", id="id")
+        
+                request_proxy_user_2 = RequestProxy("host", 8080)
+        
+                Initializer.initialize(user=user1, environment=environment1, token=token1, store=store, sdk_config=sdk_config_1, resource_path=resource_path, logger=logger)
+        
+                t1 = MultiThread(environment1, token1, user1, user1_module_api_name, sdk_config_1)
+                t2 = MultiThread(environment2, token2, user2, user2_module_api_name, sdk_config_2, request_proxy_user_2)
+        
+                t1.start()
+                t2.start()
+        
+                t1.join()
+                t2.join()
+        
+        
+        MultiThread.call()
+        
+        ```
+        
+        - The program execution starts from **call()**.
+        
+        - The details of **user1** are given in the variables user1, token1, environment1.
+        
+        - Similarly, the details of another user **user2** are given in the variables user2, token2, environment2.
+        
+        - For each user, an instance of **MultiThread class** is created.
+        
+        - When the **start()** is called which in-turn invokes the **run()**,  the details of user1 are passed to the **switch_user** method through the **MultiThread object**. Therefore, this creates a thread for user1.
+        
+        - Similarly, When the **start()** is invoked again,  the details of user2 are passed to the **switch_user** function through the **MultiThread object**. Therefore, this creates a thread for user2.
+        
+        ### Multi-threading in a Single User App
+        
+        Here is a sample code to depict multi-threading for a single-user app.
+        
+        ```python
+        import threading
+        from zcrmsdk.src.com.zoho.crm.api.user_signature import UserSignature
+        from zcrmsdk.src.com.zoho.crm.api.dc import USDataCenter
+        from zcrmsdk.src.com.zoho.api.authenticator.store import DBStore
+        from zcrmsdk.src.com.zoho.api.logger import Logger
+        from zcrmsdk.src.com.zoho.crm.api.initializer import Initializer
+        from zcrmsdk.src.com.zoho.api.authenticator.oauth_token import OAuthToken
+        from zcrmsdk.src.com.zoho.crm.api.sdk_config import SDKConfig
+        from zcrmsdk.src.com.zoho.crm.api.record import *
+        
+        
+        class MultiThread(threading.Thread):
+        
+            def __init__(self, module_api_name):
+                super().__init__()
+                self.module_api_name = module_api_name
+        
+            def run(self):
+                try:
+                    print("Calling Get Records for module: " + self.module_api_name)
+        
+                    response = RecordOperations().get_records(self.module_api_name)
+        
+                    if response is not None:
+        
+                        # Get the status code from response
+                        print('Status Code: ' + str(response.get_status_code()))
+        
+                        if response.get_status_code() in [204, 304]:
+                            print('No Content' if response.get_status_code() == 204 else 'Not Modified')
+                            return
+        
+                        # Get object from response
+                        response_object = response.get_object()
+        
+                        if response_object is not None:
+        
+                            # Check if expected ResponseWrapper instance is received.
+                            if isinstance(response_object, ResponseWrapper):
+                                # Get the list of obtained Record instances
+                                record_list = response_object.get_data()
+        
+                                for record in record_list:
+                                    for key, value in record.get_key_values().items():
+                                        print(key + " : " + str(value))
+        
+                            # Check if the request returned an exception
+                            elif isinstance(response_object, APIException):
+                                # Get the Status
+                                print("Status: " + response_object.get_status().get_value())
+        
+                                # Get the Code
+                                print("Code: " + response_object.get_code().get_value())
+        
+                                print("Details")
+        
+                                # Get the details dict
+                                details = response_object.get_details()
+        
+                                for key, value in details.items():
+                                    print(key + ' : ' + str(value))
+        
+                                # Get the Message
+                                print("Message: " + response_object.get_message().get_value())
+        
+                except Exception as e:
+                    print(e)
+        
+            @staticmethod
+            def call():
+                logger = Logger.get_instance(level=Logger.Levels.INFO, file_path="/Users/user_name/Documents/python_sdk_log.log")
+        
+                user = UserSignature(email="abc@zoho.com")
+        
+                token = OAuthToken(client_id="clientId", client_secret="clientSecret", grant_token="grant_token", refresh_token="refresh_token", redirect_url="redirectURL", id="id")
+        
+                environment = USDataCenter.PRODUCTION()
+        
+                store = DBStore()
+        
+                sdk_config = SDKConfig()
+        
+                resource_path = '/Users/user_name/Documents/python-app'
+        
+                Initializer.initialize(user=user, environment=environment, token=token, store=store, sdk_config=sdk_config, resource_path=resource_path, logger=logger)
+        
+                t1 = MultiThread('Leads')
+                t2 = MultiThread('Quotes')
+        
+                t1.start()
+                t2.start()
+        
+                t1.join()
+                t2.join()
+        
+        
+        MultiThread.call()
+        ```
+        
+        - The program execution starts from **call()** where the SDK is initialized with the details of the user.
+        
+        - When the **start()** is called which in-turn invokes the run(),  the module_api_name is switched through the MultiThread object. Therefore, this creates a thread for the particular MultiThread instance.
+        
+        ## SDK Sample code
+        
+        ```python
+        from datetime import datetime
+        from zcrmsdk.src.com.zoho.crm.api.user_signature import UserSignature
+        from zcrmsdk.src.com.zoho.crm.api.dc import USDataCenter
+        from zcrmsdk.src.com.zoho.api.authenticator.store import DBStore
+        from zcrmsdk.src.com.zoho.api.logger import Logger
+        from zcrmsdk.src.com.zoho.crm.api.initializer import Initializer
+        from zcrmsdk.src.com.zoho.api.authenticator.oauth_token import OAuthToken
+        from zcrmsdk.src.com.zoho.crm.api.record import *
+        from zcrmsdk.src.com.zoho.crm.api import HeaderMap, ParameterMap
+        from zcrmsdk.src.com.zoho.crm.api.sdk_config import SDKConfig
+        
+        
+        class Record(object):
+        
+            def __init__(self):
+                pass
+        
+            @staticmethod
+            def get_records():
+        
+                """
+                Create an instance of Logger Class that takes two parameters
+                1 -> Level of the log messages to be logged. Can be configured by typing Logger.Levels "." and choose any level from the list displayed.
+                2 -> Absolute file path, where messages need to be logged.
+                """
+                logger = Logger.get_instance(level=Logger.Levels.INFO,
+                                             file_path="/Users/user_name/Documents/python_sdk_log.log")
+        
+                # Create an UserSignature instance that takes user Email as parameter
+                user = UserSignature(email="abc@zoho.com")
+        
+                """
+                Configure the environment
+                which is of the pattern Domain.Environment
+                Available Domains: USDataCenter, EUDataCenter, INDataCenter, CNDataCenter, AUDataCenter
+                Available Environments: PRODUCTION(), DEVELOPER(), SANDBOX()
+                """
+                environment = USDataCenter.PRODUCTION()
+        
+                """
+                Create a Token instance that takes the following parameters
+                1 -> OAuth client id.
+                2 -> OAuth client secret.
+                3 -> Grant token.
+                4 -> Refresh token.
+                5 -> OAuth redirect URL.
+                6 -> id
+                """
+                token = OAuthToken(client_id="clientId", client_secret="clientSecret", grant_token="grant_token", refresh_token="refresh_token", redirect_url="redirectURL", id="id")
+        
+                """
+                Create an instance of TokenStore
+                1 -> DataBase host name. Default value "localhost"
+                2 -> DataBase name. Default value "zohooauth"
+                3 -> DataBase user name. Default value "root"
+                4 -> DataBase password. Default value ""
+                5 -> DataBase port number. Default value "3306"
+                6->  DataBase table name . Default value "oauthtoken"
+                """
+                store = DBStore()
+        
+                """
+                auto_refresh_fields (Default value is False)
+                    if True - all the modules' fields will be auto-refreshed in the background, every hour.
+                    if False - the fields will not be auto-refreshed in the background. The user can manually delete the file(s) or refresh the fields using methods from ModuleFieldsHandler(zcrmsdk/src/com/zoho/crm/api/util/module_fields_handler.py)
+        
+                pick_list_validation (Default value is True)
+                    A boolean field that validates user input for a pick list field and allows or disallows the addition of a new value to the list.
+                    if True - the SDK validates the input. If the value does not exist in the pick list, the SDK throws an error.
+                    if False - the SDK does not validate the input and makes the API request with the user’s input to the pick list
+                 connect_timeout (Default value is None) 
+                    A  Float field to set connect timeout
+          
+                 read_timeout (Default value is None) 
+                    A  Float field to set read timeout
+                 """
+                config = SDKConfig(auto_refresh_fields=True, pick_list_validation=False, connect_timeout=None, read_timeout=None)
+        
+                """
+                The path containing the absolute directory path (in the key resource_path) to store user-specific files containing information about fields in modules. 
+                """
+                resource_path = '/Users/user_name/Documents/python-app'
+        
+                """
+                Call the static initialize method of Initializer class that takes the following arguments
+                1 -> UserSignature instance
+                2 -> Environment instance
+                3 -> Token instance
+                4 -> TokenStore instance
+                5 -> SDKConfig instance
+                6 -> resource_path
+                7 -> Logger instance
+                """
+                Initializer.initialize(user=user, environment=environment, token=token, store=store, sdk_config=config, resource_path=resource_path, logger=logger)
+        
+                try:
+                    module_api_name = 'Leads'
+        
+                    param_instance = ParameterMap()
+        
+                    param_instance.add(GetRecordsParam.converted, 'both')
+        
+                    param_instance.add(GetRecordsParam.cvid, '12712717217218')
+        
+                    header_instance = HeaderMap()
+        
+                    header_instance.add(GetRecordsHeader.if_modified_since, datetime.now())
+        
+                    response = RecordOperations().get_records(module_api_name, param_instance, header_instance)
+        
+                    if response is not None:
+        
+                        # Get the status code from response
+                        print('Status Code: ' + str(response.get_status_code()))
+        
+                        if response.get_status_code() in [204, 304]:
+                            print('No Content' if response.get_status_code() == 204 else 'Not Modified')
+                            return
+        
+                        # Get object from response
+                        response_object = response.get_object()
+        
+                        if response_object is not None:
+        
+                            # Check if expected ResponseWrapper instance is received.
+                            if isinstance(response_object, ResponseWrapper):
+                                # Get the list of obtained Record instances
+                                record_list = response_object.get_data()
+        
+                                for record in record_list:
+        
+                                    # Get the ID of each Record
+                                    print("Record ID: " + record.get_id())
+        
+                                    # Get the createdBy User instance of each Record
+                                    created_by = record.get_created_by()
+        
+                                    # Check if created_by is not None
+                                    if created_by is not None:
+                                        # Get the Name of the created_by User
+                                        print("Record Created By - Name: " + created_by.get_name())
+        
+                                        # Get the ID of the created_by User
+                                        print("Record Created By - ID: " + created_by.get_id())
+        
+                                        # Get the Email of the created_by User
+                                        print("Record Created By - Email: " + created_by.get_email())
+        
+                                    # Get the CreatedTime of each Record
+                                    print("Record CreatedTime: " + str(record.get_created_time()))
+        
+                                    if record.get_modified_time() is not None:
+                                        # Get the ModifiedTime of each Record
+                                        print("Record ModifiedTime: " + str(record.get_modified_time()))
+        
+                                    # Get the modified_by User instance of each Record
+                                    modified_by = record.get_modified_by()
+        
+                                    # Check if modified_by is not None
+                                    if modified_by is not None:
+                                        # Get the Name of the modified_by User
+                                        print("Record Modified By - Name: " + modified_by.get_name())
+        
+                                        # Get the ID of the modified_by User
+                                        print("Record Modified By - ID: " + modified_by.get_id())
+        
+                                        # Get the Email of the modified_by User
+                                        print("Record Modified By - Email: " + modified_by.get_email())
+        
+                                    # Get the list of obtained Tag instance of each Record
+                                    tags = record.get_tag()
+        
+                                    if tags is not None:
+                                        for tag in tags:
+                                            # Get the Name of each Tag
+                                            print("Record Tag Name: " + tag.get_name())
+        
+                                            # Get the Id of each Tag
+                                            print("Record Tag ID: " + tag.get_id())
+        
+                                    # To get particular field value
+                                    print("Record Field Value: " + str(record.get_key_value('Last_Name')))
+        
+                                    print('Record KeyValues: ')
+        
+                                    for key, value in record.get_key_values().items():
+                                        print(key + " : " + str(value))
+        
+                            # Check if the request returned an exception
+                            elif isinstance(response_object, APIException):
+                                # Get the Status
+                                print("Status: " + response_object.get_status().get_value())
+        
+                                # Get the Code
+                                print("Code: " + response_object.get_code().get_value())
+        
+                                print("Details")
+        
+                                # Get the details dict
+                                details = response_object.get_details()
+        
+                                for key, value in details.items():
+                                    print(key + ' : ' + str(value))
+        
+                                # Get the Message
+                                print("Message: " + response_object.get_message().get_value())
+        
+                except Exception as e:
+                    print(e)
+        
+        
+        Record.get_records()
+        ```
+        
+Keywords: development,zoho,crm,api,zcrmsdk,sdk,zcrm,zohocrmsdk2_1
+Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Description-Content-Type: text/markdown
```

### Comparing `zohocrmsdk2_1-2.0.0/zohocrmsdk2_1.egg-info/SOURCES.txt` & `zohocrmsdk2_1-2.1.0/zohocrmsdk2_1.egg-info/SOURCES.txt`

 * *Files identical despite different names*

