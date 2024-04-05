# Comparing `tmp/grrshell-20231227.tar.gz` & `tmp/grrshell-20240405.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grrshell-20231227.tar", max compression
+gzip compressed data, was "grrshell-20240405.tar", max compression
```

## Comparing `grrshell-20231227.tar` & `grrshell-20240405.tar`

### file list

```diff
@@ -1,66 +1,73 @@
--rw-r--r--   0        0        0    11358 2023-12-27 05:48:30.255668 grrshell-20231227/LICENSE
--rw-r--r--   0        0        0     7278 2023-12-27 05:48:30.255668 grrshell-20231227/README.md
--rw-r--r--   0        0        0     8698 2023-12-27 05:48:30.255668 grrshell-20231227/grrshell/cli/main.py
--rw-r--r--   0        0        0     4283 2023-12-27 05:48:30.259668 grrshell-20231227/grrshell/lib/client_monitors.py
--rw-r--r--   0        0        0     1272 2023-12-27 05:48:30.259668 grrshell-20231227/grrshell/lib/errors.py
--rw-r--r--   0        0        0     3840 2023-12-27 05:48:30.259668 grrshell-20231227/grrshell/lib/flow_args_parsers.py
--rw-r--r--   0        0        0     6804 2023-12-27 05:48:30.259668 grrshell-20231227/grrshell/lib/formatters.py
--rw-r--r--   0        0        0    33024 2023-12-27 05:48:30.259668 grrshell-20231227/grrshell/lib/grr_shell_client.py
--rw-r--r--   0        0        0    15655 2023-12-27 05:48:30.259668 grrshell-20231227/grrshell/lib/grr_shell_emulated_fs.py
--rw-r--r--   0        0        0    25503 2023-12-27 05:48:30.259668 grrshell-20231227/grrshell/lib/grr_shell_repl.py
--rw-r--r--   0        0        0     1092 2023-12-27 05:48:30.259668 grrshell-20231227/grrshell/lib/utils.py
--rw-r--r--   0        0        0     9132 2023-12-27 05:48:30.259668 grrshell-20231227/grrshell/tests/flow_args_parsers_test.py
--rw-r--r--   0        0        0    89442 2023-12-27 05:48:30.259668 grrshell-20231227/grrshell/tests/grr_shell_client_test.py
--rw-r--r--   0        0        0    24411 2023-12-27 05:48:30.259668 grrshell-20231227/grrshell/tests/grr_shell_emulated_fs_test.py
--rw-r--r--   0        0        0    31501 2023-12-27 05:48:30.259668 grrshell-20231227/grrshell/tests/grr_shell_repl_test.py
--rw-r--r--   0        0        0     1197 2023-12-27 05:48:30.259668 grrshell-20231227/grrshell/tests/testdata/artifact_collect_darwin.zip
--rw-r--r--   0        0        0     1190 2023-12-27 05:48:30.259668 grrshell-20231227/grrshell/tests/testdata/artifact_collect_linux.zip
--rw-r--r--   0        0        0     1257 2023-12-27 05:48:30.259668 grrshell-20231227/grrshell/tests/testdata/artifact_collect_windows.zip
--rw-r--r--   0        0        0     1125 2023-12-27 05:48:30.259668 grrshell-20231227/grrshell/tests/testdata/file_collect_darwin.zip
--rw-r--r--   0        0        0     1130 2023-12-27 05:48:30.259668 grrshell-20231227/grrshell/tests/testdata/file_collect_linux.zip
--rw-r--r--   0        0        0     1197 2023-12-27 05:48:30.259668 grrshell-20231227/grrshell/tests/testdata/file_collect_windows.zip
--rw-r--r--   0        0        0     1333 2023-12-27 05:48:30.259668 grrshell-20231227/grrshell/tests/testdata/getfile_ads.zip
--rw-r--r--   0        0        0      699 2023-12-27 05:48:30.259668 grrshell-20231227/grrshell/tests/testdata/getfile_ads_empty.zip
--rw-r--r--   0        0        0      422 2023-12-27 05:48:30.259668 grrshell-20231227/grrshell/tests/testdata/mock_apiflow_artifactcollector_allfile_running.textproto
--rw-r--r--   0        0        0      431 2023-12-27 05:48:30.259668 grrshell-20231227/grrshell/tests/testdata/mock_apiflow_artifactcollector_allfile_terminated.textproto
--rw-r--r--   0        0        0      451 2023-12-27 05:48:30.259668 grrshell-20231227/grrshell/tests/testdata/mock_apiflow_artifactcollector_multiple.textproto
--rw-r--r--   0        0        0      428 2023-12-27 05:48:30.259668 grrshell-20231227/grrshell/tests/testdata/mock_apiflow_artifactcollector_windowsregkey_running.textproto
--rw-r--r--   0        0        0      918 2023-12-27 05:48:30.259668 grrshell-20231227/grrshell/tests/testdata/mock_apiflow_clientfilefinder_download_error.textproto
--rw-r--r--   0        0        0      438 2023-12-27 05:48:30.259668 grrshell-20231227/grrshell/tests/testdata/mock_apiflow_clientfilefinder_download_running.textproto
--rw-r--r--   0        0        0      516 2023-12-27 05:48:30.259668 grrshell-20231227/grrshell/tests/testdata/mock_apiflow_clientfilefinder_download_terminated.textproto
--rw-r--r--   0        0        0      477 2023-12-27 05:48:30.259668 grrshell-20231227/grrshell/tests/testdata/mock_apiflow_clientfilefinder_hash_running.textproto
--rw-r--r--   0        0        0      526 2023-12-27 05:48:30.259668 grrshell-20231227/grrshell/tests/testdata/mock_apiflow_clientfilefinder_multiple.textproto
--rw-r--r--   0        0        0      453 2023-12-27 05:48:30.259668 grrshell-20231227/grrshell/tests/testdata/mock_apiflow_collectbrowserhistory.textproto
--rw-r--r--   0        0        0      547 2023-12-27 05:48:30.259668 grrshell-20231227/grrshell/tests/testdata/mock_apiflow_collectfilesbyknownpath_multiple.textproto
--rw-r--r--   0        0        0      467 2023-12-27 05:48:30.259668 grrshell-20231227/grrshell/tests/testdata/mock_apiflow_collectfilesbyknownpath_single.textproto
--rw-r--r--   0        0        0      465 2023-12-27 05:48:30.259668 grrshell-20231227/grrshell/tests/testdata/mock_apiflow_getfile_running.textproto
--rw-r--r--   0        0        0      322 2023-12-27 05:48:30.259668 grrshell-20231227/grrshell/tests/testdata/mock_apiflow_interrogate_running.textproto
--rw-r--r--   0        0        0     1492 2023-12-27 05:48:30.259668 grrshell-20231227/grrshell/tests/testdata/mock_apiflow_listflows.textproto
--rw-r--r--   0        0        0      449 2023-12-27 05:48:30.259668 grrshell-20231227/grrshell/tests/testdata/mock_apiflow_timeline_error.textproto
--rw-r--r--   0        0        0      397 2023-12-27 05:48:30.259668 grrshell-20231227/grrshell/tests/testdata/mock_apiflow_timeline_error_nomessage.textproto
--rw-r--r--   0        0        0      485 2023-12-27 05:48:30.259668 grrshell-20231227/grrshell/tests/testdata/mock_apiflow_timeline_error_stacktrace.textproto
--rw-r--r--   0        0        0      328 2023-12-27 05:48:30.259668 grrshell-20231227/grrshell/tests/testdata/mock_apiflow_timeline_running.textproto
--rw-r--r--   0        0        0      245 2023-12-27 05:48:30.259668 grrshell-20231227/grrshell/tests/testdata/mock_artifactdescriptor_all_artifactgroup.textproto
--rw-r--r--   0        0        0      226 2023-12-27 05:48:30.259668 grrshell-20231227/grrshell/tests/testdata/mock_artifactdescriptor_all_file.textproto
--rw-r--r--   0        0        0      196 2023-12-27 05:48:30.259668 grrshell-20231227/grrshell/tests/testdata/mock_artifactdescriptor_darwin_artifactfiles.textproto
--rw-r--r--   0        0        0      201 2023-12-27 05:48:30.259668 grrshell-20231227/grrshell/tests/testdata/mock_artifactdescriptor_darwin_grraction.textproto
--rw-r--r--   0        0        0      181 2023-12-27 05:48:30.263668 grrshell-20231227/grrshell/tests/testdata/mock_artifactdescriptor_linux_command.textproto
--rw-r--r--   0        0        0      175 2023-12-27 05:48:30.263668 grrshell-20231227/grrshell/tests/testdata/mock_artifactdescriptor_linux_path.textproto
--rw-r--r--   0        0        0      344 2023-12-27 05:48:30.263668 grrshell-20231227/grrshell/tests/testdata/mock_artifactdescriptor_mixed.textproto
--rw-r--r--   0        0        0      189 2023-12-27 05:48:30.263668 grrshell-20231227/grrshell/tests/testdata/mock_artifactdescriptor_windows_regkey.textproto
--rw-r--r--   0        0        0      193 2023-12-27 05:48:30.263668 grrshell-20231227/grrshell/tests/testdata/mock_artifactdescriptor_windows_regvalue.textproto
--rw-r--r--   0        0        0      488 2023-12-27 05:48:30.263668 grrshell-20231227/grrshell/tests/testdata/mock_client_darwin.textproto
--rw-r--r--   0        0        0      514 2023-12-27 05:48:30.263668 grrshell-20231227/grrshell/tests/testdata/mock_client_linux.textproto
--rw-r--r--   0        0        0      414 2023-12-27 05:48:30.263668 grrshell-20231227/grrshell/tests/testdata/mock_client_windows.textproto
--rw-r--r--   0        0        0      687 2023-12-27 05:48:30.263668 grrshell-20231227/grrshell/tests/testdata/mock_hash_linux.textproto
--rw-r--r--   0        0        0      819 2023-12-27 05:48:30.263668 grrshell-20231227/grrshell/tests/testdata/mock_hash_windows.textproto
--rw-r--r--   0        0        0      683 2023-12-27 05:48:30.263668 grrshell-20231227/grrshell/tests/testdata/mock_hash_windows_ads.textproto
--rw-r--r--   0        0        0      350 2023-12-27 05:48:30.263668 grrshell-20231227/grrshell/tests/testdata/mock_windows_registry_result.textproto
--rw-r--r--   0        0        0     6575 2023-12-27 05:48:30.263668 grrshell-20231227/grrshell/tests/testdata/sample_timeline_darwin
--rw-r--r--   0        0        0     3373 2023-12-27 05:48:30.263668 grrshell-20231227/grrshell/tests/testdata/sample_timeline_linux
--rw-r--r--   0        0        0      227 2023-12-27 05:48:30.263668 grrshell-20231227/grrshell/tests/testdata/sample_timeline_linux_overlay
--rw-r--r--   0        0        0     9691 2023-12-27 05:48:30.263668 grrshell-20231227/grrshell/tests/testdata/sample_timeline_windows
--rw-r--r--   0        0        0      827 2023-12-27 05:48:30.263668 grrshell-20231227/grrshell/tests/testdata/sample_timeline_windows_d_drive
--rw-r--r--   0        0        0     1378 2023-12-27 05:48:30.263668 grrshell-20231227/grrshell/tests/utils_test.py
--rw-r--r--   0        0        0      515 2023-12-27 05:48:30.263668 grrshell-20231227/pyproject.toml
--rw-r--r--   0        0        0     7890 1970-01-01 00:00:00.000000 grrshell-20231227/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-04-05 02:43:01.631924 grrshell-20240405/LICENSE
+-rw-r--r--   0        0        0     7278 2024-04-05 02:43:01.631924 grrshell-20240405/README.md
+-rw-r--r--   0        0        0    11492 2024-04-05 02:43:01.631924 grrshell-20240405/grrshell/cli/main.py
+-rw-r--r--   0        0        0     4802 2024-04-05 02:43:01.631924 grrshell-20240405/grrshell/lib/client_monitors.py
+-rw-r--r--   0        0        0     1272 2024-04-05 02:43:01.631924 grrshell-20240405/grrshell/lib/errors.py
+-rw-r--r--   0        0        0     4285 2024-04-05 02:43:01.631924 grrshell-20240405/grrshell/lib/flow_args_parsers.py
+-rw-r--r--   0        0        0     9830 2024-04-05 02:43:01.631924 grrshell-20240405/grrshell/lib/formatters.py
+-rw-r--r--   0        0        0    37171 2024-04-05 02:43:01.631924 grrshell-20240405/grrshell/lib/grr_shell_client.py
+-rw-r--r--   0        0        0    15713 2024-04-05 02:43:01.631924 grrshell-20240405/grrshell/lib/grr_shell_emulated_fs.py
+-rw-r--r--   0        0        0    26091 2024-04-05 02:43:01.631924 grrshell-20240405/grrshell/lib/grr_shell_repl.py
+-rw-r--r--   0        0        0     1092 2024-04-05 02:43:01.631924 grrshell-20240405/grrshell/lib/utils.py
+-rw-r--r--   0        0        0    10959 2024-04-05 02:43:01.631924 grrshell-20240405/grrshell/tests/flow_args_parsers_test.py
+-rw-r--r--   0        0        0   102434 2024-04-05 02:43:01.631924 grrshell-20240405/grrshell/tests/grr_shell_client_test.py
+-rw-r--r--   0        0        0    24532 2024-04-05 02:43:01.631924 grrshell-20240405/grrshell/tests/grr_shell_emulated_fs_test.py
+-rw-r--r--   0        0        0    32642 2024-04-05 02:43:01.631924 grrshell-20240405/grrshell/tests/grr_shell_repl_test.py
+-rw-r--r--   0        0        0    11440 2024-04-05 02:43:01.631924 grrshell-20240405/grrshell/tests/main_test.py
+-rw-r--r--   0        0        0     1197 2024-04-05 02:43:01.631924 grrshell-20240405/grrshell/tests/testdata/artifact_collect_darwin.zip
+-rw-r--r--   0        0        0     1190 2024-04-05 02:43:01.631924 grrshell-20240405/grrshell/tests/testdata/artifact_collect_linux.zip
+-rw-r--r--   0        0        0     1257 2024-04-05 02:43:01.631924 grrshell-20240405/grrshell/tests/testdata/artifact_collect_windows.zip
+-rw-r--r--   0        0        0     1125 2024-04-05 02:43:01.635924 grrshell-20240405/grrshell/tests/testdata/file_collect_darwin.zip
+-rw-r--r--   0        0        0     1130 2024-04-05 02:43:01.635924 grrshell-20240405/grrshell/tests/testdata/file_collect_linux.zip
+-rw-r--r--   0        0        0     1197 2024-04-05 02:43:01.635924 grrshell-20240405/grrshell/tests/testdata/file_collect_windows.zip
+-rw-r--r--   0        0        0      348 2024-04-05 02:43:01.635924 grrshell-20240405/grrshell/tests/testdata/file_collect_windows_fat32.zip
+-rw-r--r--   0        0        0     1333 2024-04-05 02:43:01.635924 grrshell-20240405/grrshell/tests/testdata/getfile_ads.zip
+-rw-r--r--   0        0        0      699 2024-04-05 02:43:01.635924 grrshell-20240405/grrshell/tests/testdata/getfile_ads_empty.zip
+-rw-r--r--   0        0        0      422 2024-04-05 02:43:01.635924 grrshell-20240405/grrshell/tests/testdata/mock_apiflow_artifactcollector_allfile_running.textproto
+-rw-r--r--   0        0        0      431 2024-04-05 02:43:01.635924 grrshell-20240405/grrshell/tests/testdata/mock_apiflow_artifactcollector_allfile_terminated.textproto
+-rw-r--r--   0        0        0      451 2024-04-05 02:43:01.635924 grrshell-20240405/grrshell/tests/testdata/mock_apiflow_artifactcollector_multiple.textproto
+-rw-r--r--   0        0        0      428 2024-04-05 02:43:01.635924 grrshell-20240405/grrshell/tests/testdata/mock_apiflow_artifactcollector_windowsregkey_running.textproto
+-rw-r--r--   0        0        0      429 2024-04-05 02:43:01.635924 grrshell-20240405/grrshell/tests/testdata/mock_apiflow_artifactcollector_wmilogicaldisks_running.textproto
+-rw-r--r--   0        0        0      918 2024-04-05 02:43:01.635924 grrshell-20240405/grrshell/tests/testdata/mock_apiflow_clientfilefinder_download_error.textproto
+-rw-r--r--   0        0        0      438 2024-04-05 02:43:01.635924 grrshell-20240405/grrshell/tests/testdata/mock_apiflow_clientfilefinder_download_running.textproto
+-rw-r--r--   0        0        0      516 2024-04-05 02:43:01.635924 grrshell-20240405/grrshell/tests/testdata/mock_apiflow_clientfilefinder_download_terminated.textproto
+-rw-r--r--   0        0        0      477 2024-04-05 02:43:01.635924 grrshell-20240405/grrshell/tests/testdata/mock_apiflow_clientfilefinder_hash_running.textproto
+-rw-r--r--   0        0        0      526 2024-04-05 02:43:01.635924 grrshell-20240405/grrshell/tests/testdata/mock_apiflow_clientfilefinder_multiple.textproto
+-rw-r--r--   0        0        0      453 2024-04-05 02:43:01.635924 grrshell-20240405/grrshell/tests/testdata/mock_apiflow_collectbrowserhistory.textproto
+-rw-r--r--   0        0        0      547 2024-04-05 02:43:01.635924 grrshell-20240405/grrshell/tests/testdata/mock_apiflow_collectfilesbyknownpath_multiple.textproto
+-rw-r--r--   0        0        0      467 2024-04-05 02:43:01.635924 grrshell-20240405/grrshell/tests/testdata/mock_apiflow_collectfilesbyknownpath_single.textproto
+-rw-r--r--   0        0        0      465 2024-04-05 02:43:01.635924 grrshell-20240405/grrshell/tests/testdata/mock_apiflow_getfile_running.textproto
+-rw-r--r--   0        0        0      322 2024-04-05 02:43:01.635924 grrshell-20240405/grrshell/tests/testdata/mock_apiflow_interrogate_running.textproto
+-rw-r--r--   0        0        0     2237 2024-04-05 02:43:01.635924 grrshell-20240405/grrshell/tests/testdata/mock_apiflow_listflows.textproto
+-rw-r--r--   0        0        0      629 2024-04-05 02:43:01.635924 grrshell-20240405/grrshell/tests/testdata/mock_apiflow_multigetfile_running_multiple.textproto
+-rw-r--r--   0        0        0      520 2024-04-05 02:43:01.635924 grrshell-20240405/grrshell/tests/testdata/mock_apiflow_multigetfile_running_single.textproto
+-rw-r--r--   0        0        0      449 2024-04-05 02:43:01.635924 grrshell-20240405/grrshell/tests/testdata/mock_apiflow_timeline_error.textproto
+-rw-r--r--   0        0        0      397 2024-04-05 02:43:01.635924 grrshell-20240405/grrshell/tests/testdata/mock_apiflow_timeline_error_nomessage.textproto
+-rw-r--r--   0        0        0      485 2024-04-05 02:43:01.635924 grrshell-20240405/grrshell/tests/testdata/mock_apiflow_timeline_error_stacktrace.textproto
+-rw-r--r--   0        0        0      328 2024-04-05 02:43:01.635924 grrshell-20240405/grrshell/tests/testdata/mock_apiflow_timeline_running.textproto
+-rw-r--r--   0        0        0      245 2024-04-05 02:43:01.635924 grrshell-20240405/grrshell/tests/testdata/mock_artifactdescriptor_all_artifactgroup.textproto
+-rw-r--r--   0        0        0      226 2024-04-05 02:43:01.635924 grrshell-20240405/grrshell/tests/testdata/mock_artifactdescriptor_all_file.textproto
+-rw-r--r--   0        0        0      196 2024-04-05 02:43:01.635924 grrshell-20240405/grrshell/tests/testdata/mock_artifactdescriptor_darwin_artifactfiles.textproto
+-rw-r--r--   0        0        0      201 2024-04-05 02:43:01.635924 grrshell-20240405/grrshell/tests/testdata/mock_artifactdescriptor_darwin_grraction.textproto
+-rw-r--r--   0        0        0      181 2024-04-05 02:43:01.635924 grrshell-20240405/grrshell/tests/testdata/mock_artifactdescriptor_linux_command.textproto
+-rw-r--r--   0        0        0      175 2024-04-05 02:43:01.635924 grrshell-20240405/grrshell/tests/testdata/mock_artifactdescriptor_linux_path.textproto
+-rw-r--r--   0        0        0      344 2024-04-05 02:43:01.635924 grrshell-20240405/grrshell/tests/testdata/mock_artifactdescriptor_mixed.textproto
+-rw-r--r--   0        0        0      189 2024-04-05 02:43:01.635924 grrshell-20240405/grrshell/tests/testdata/mock_artifactdescriptor_windows_regkey.textproto
+-rw-r--r--   0        0        0      193 2024-04-05 02:43:01.635924 grrshell-20240405/grrshell/tests/testdata/mock_artifactdescriptor_windows_regvalue.textproto
+-rw-r--r--   0        0        0      488 2024-04-05 02:43:01.635924 grrshell-20240405/grrshell/tests/testdata/mock_client_darwin.textproto
+-rw-r--r--   0        0        0      514 2024-04-05 02:43:01.635924 grrshell-20240405/grrshell/tests/testdata/mock_client_linux.textproto
+-rw-r--r--   0        0        0      414 2024-04-05 02:43:01.635924 grrshell-20240405/grrshell/tests/testdata/mock_client_windows.textproto
+-rw-r--r--   0        0        0      687 2024-04-05 02:43:01.635924 grrshell-20240405/grrshell/tests/testdata/mock_hash_linux.textproto
+-rw-r--r--   0        0        0      819 2024-04-05 02:43:01.635924 grrshell-20240405/grrshell/tests/testdata/mock_hash_windows.textproto
+-rw-r--r--   0        0        0      683 2024-04-05 02:43:01.635924 grrshell-20240405/grrshell/tests/testdata/mock_hash_windows_ads.textproto
+-rw-r--r--   0        0        0     1089 2024-04-05 02:43:01.639924 grrshell-20240405/grrshell/tests/testdata/mock_volume_windows_c.textproto
+-rw-r--r--   0        0        0     1085 2024-04-05 02:43:01.639924 grrshell-20240405/grrshell/tests/testdata/mock_volume_windows_d.textproto
+-rw-r--r--   0        0        0      350 2024-04-05 02:43:01.639924 grrshell-20240405/grrshell/tests/testdata/mock_windows_registry_result.textproto
+-rw-r--r--   0        0        0     6575 2024-04-05 02:43:01.639924 grrshell-20240405/grrshell/tests/testdata/sample_timeline_darwin
+-rw-r--r--   0        0        0     3373 2024-04-05 02:43:01.639924 grrshell-20240405/grrshell/tests/testdata/sample_timeline_linux
+-rw-r--r--   0        0        0      227 2024-04-05 02:43:01.639924 grrshell-20240405/grrshell/tests/testdata/sample_timeline_linux_overlay
+-rw-r--r--   0        0        0     9934 2024-04-05 02:43:01.639924 grrshell-20240405/grrshell/tests/testdata/sample_timeline_windows
+-rw-r--r--   0        0        0      827 2024-04-05 02:43:01.639924 grrshell-20240405/grrshell/tests/testdata/sample_timeline_windows_d_drive
+-rw-r--r--   0        0        0     1396 2024-04-05 02:43:01.639924 grrshell-20240405/grrshell/tests/utils_test.py
+-rw-r--r--   0        0        0      515 2024-04-05 02:43:01.639924 grrshell-20240405/pyproject.toml
+-rw-r--r--   0        0        0     7890 1970-01-01 00:00:00.000000 grrshell-20240405/PKG-INFO
```

### Comparing `grrshell-20231227/LICENSE` & `grrshell-20240405/LICENSE`

 * *Files identical despite different names*

### Comparing `grrshell-20231227/README.md` & `grrshell-20240405/README.md`

 * *Files identical despite different names*

### Comparing `grrshell-20231227/grrshell/lib/client_monitors.py` & `grrshell-20240405/grrshell/lib/client_monitors.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import time
 from typing import Iterator
 
 from absl import logging
 
 from grr_api_client import flow
 from grr_api_client import api as grr_api
-from grr_response_proto import flows_pb2
+from grr_response_proto.api import flow_pb2
 
 
 logger = logging.logging.getLogger('grrshell')
 
 
 class _MonitorBase(metaclass=abc.ABCMeta):
   """Base class for background monitor classes."""
@@ -90,50 +90,67 @@
     super().__init__()
     self._grr_client = grr_client
     self._flows: dict[str, flow.Flow] = {}
 
   def _Monitor(self):
     """Repeatedly polls _SingleFetch()."""
     while True:
-      with self._mutex:
-        self._SingleFetch()
-
-      for flow_id in self._flows:
-        self._UpdateCachedFlow(flow_id)
+      try:
+        with self._mutex:
+          self._SingleFetch()
+
+        for flow_id in self._flows:
+          self._UpdateCachedFlow(flow_id)
+      except RuntimeError as error:
+        # b/321145259 - Ignore this exception
+        if str(error) != 'dictionary changed size during iteration':
+          raise error
 
       time.sleep(self.DELAY)
 
   def _SingleFetch(self):
     """Fetches all launched flows on the client."""
     logger.debug('Fetching launched flows')
     for flow_handle in self._grr_client.ListFlows():
       if flow_handle.flow_id not in self._flows:
         self._flows[flow_handle.flow_id] = flow_handle
 
   def GetFlowsInfoList(self, count: int = 50) -> Iterator[flow.Flow]:
     """Returns info on flows from the cache."""
-    with self._mutex:
-      values = list(self._flows.values())
-      values = sorted(values,
-                      key=lambda x: x.data.started_at, reverse=True)
-      for f in itertools.islice(values, 0, count):
-        yield f
+    values = list(self._flows.values())
+    values = sorted(values,
+                    key=lambda x: x.data.started_at, reverse=True)
+    for f in itertools.islice(values, 0, count):
+      yield f
 
   def GetFlow(self, flow_id: str) -> flow.Flow:
     """Returns cached info on a single flow."""
     self._UpdateCachedFlow(flow_id)
-    with self._mutex:
-      return self._flows[flow_id]
+    return self._flows[flow_id]
 
   def TrackFlow(self, flow_handle: flow.Flow) -> None:
     """Adds a launched flow to monitoring."""
     with self._mutex:
       self._flows[flow_handle.flow_id] = flow_handle
 
+  def IsFlowCached(self, flow_id: str) -> bool:
+    """Checks if flow information is currently cached.
+
+    Args:
+      flow_id: The ID of the flow to check.
+
+    Returns:
+      True if flow information is currently chached in the FlowMonitor, False
+          otherwise.
+    """
+    return (
+        flow_id in self._flows and
+        bool(self._flows[flow_id].data.args.TypeName()))
+
   def _UpdateCachedFlow(self, flow_id: str) -> None:
     """Fetches and caches info for a single flow."""
     if (flow_id not in self._flows or
         not self._flows[flow_id].data.args.TypeName() or
-        self._flows[flow_id].data.state == flows_pb2.FlowContext.State.RUNNING):
+        self._flows[flow_id].data.state == flow_pb2.ApiFlow.State.RUNNING):
       with self._mutex:
         flow_handle = self._grr_client.Flow(flow_id).Get()
         self._flows[flow_id] = flow_handle
```

### Comparing `grrshell-20231227/grrshell/lib/errors.py` & `grrshell-20240405/grrshell/lib/errors.py`

 * *Files identical despite different names*

### Comparing `grrshell-20231227/grrshell/lib/flow_args_parsers.py` & `grrshell-20240405/grrshell/lib/flow_args_parsers.py`

 * *Files 12% similar despite different names*

```diff
@@ -53,14 +53,27 @@
   args = flows_pb2.GetFileArgs.FromString(args.value)
   param = args.pathspec.path
   if args.pathspec.stream_name:
     param = f'{param}:{args.pathspec.stream_name}'
   return [param]
 
 
+def _MultiGetFileArgsParse(args: Any, multiline: bool) -> list[str]:
+  args = flows_pb2.MultiGetFileArgs.FromString(args.value)
+  lines: list[str] = []
+  for pathspec in args.pathspecs:
+    line = pathspec.path
+    if pathspec.stream_name:
+      line = f'{line}:{pathspec.stream_name}'
+    lines.append(line)
+  if multiline or len(lines) == 1:
+    return lines
+  return ['<MULTIPLE PATHS>']
+
+
 def _CollectFilesByKnownPathArgsParse(args: Any, multiline: bool) -> list[str]:
   args = flows_pb2.CollectFilesByKnownPathArgs.FromString(args.value)
   level = flows_pb2.CollectFilesByKnownPathArgs.CollectionLevel.Name(
       args.collection_level)
   if multiline:
     lines = [f'Collection Level: {level}']
     lines += [f'Path: {p}' for p in args.paths]
@@ -82,14 +95,15 @@
         _ArtifactCollectorFlowArgsParse,
     'grr.CollectBrowserHistoryArgs':
         _CollectBrowserHistoryArgsParse,
     'grr.CollectFilesByKnownPathArgs':
         _CollectFilesByKnownPathArgsParse,
     'grr.FileFinderArgs': _FileFinderArgsParse,
     'grr.GetFileArgs': _GetFileArgsParse,
+    'grr.MultiGetFileArgs': _MultiGetFileArgsParse,
     'grr.InterrogateArgs': lambda x, y: [''],
     'grr.TimelineArgs': _TimelineArgsParse,
 }
 
 
 def Parse(flow_handle: flow.Flow, multiline: bool = False) -> list[str]:
   """Parse out flow args from a flow object.
```

### Comparing `grrshell-20231227/grrshell/lib/formatters.py` & `grrshell-20240405/grrshell/lib/formatters.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,25 +19,41 @@
 import zipfile
 
 import humanize
 
 from grr_api_client import flow
 from grr_response_proto import flows_pb2
 from grr_response_proto import jobs_pb2
+from grr_response_proto import sysinfo_pb2
 from grrshell.lib import utils
 
 
+_WINDOWS_VOLUME_DESIRED_FIELDS_MAP = {
+    'Description': lambda x: x.string,
+    'DeviceID': lambda x: x.string,
+    'DriveType': lambda x: (
+        sysinfo_pb2.WindowsVolume.WindowsDriveTypeEnum.Name(x.integer)),
+    'FileSystem': lambda x: x.string,
+    'FreeSpace': lambda x: int(x.string),
+    'Name': lambda x: x.string,
+    'Size': lambda x: int(x.string),
+    'VolumeName': lambda x: x.string,
+    'VolumeSerialNumber': lambda x: x.string,
+}
+
+
 class GRRShellFormatter:
   """Handles formatting flow output."""
 
   def __init__(self):
     """Initialises a formatter object."""
     self._callback_map: dict[str, Callable[[Any, flow.Flow], list[str]]] = {
         'FileFinderResult': self._FormatFileFinderInfoResult,
         'StatEntry': self._FormatStatEntry,
+        'Dict': self._FormatDict
     }
 
   def FormatFlowResult(self, flow_handle: flow.Flow) -> list[str]:
     """Formats the result of a flow for display to an operator.
 
     Args:
       flow_handle: The Flow handle with which to extract results.
@@ -72,15 +88,16 @@
       A list of strings, one per line, of formatted output.
 
     Raises:
       RuntimeError: If the StatEntry type is unsupported.
     """
     args_typename = flow_handle.data.args.TypeName()
 
-    if args_typename == 'grr.GetFileArgs':
+    if args_typename in ('grr.GetFileArgs',
+                         'grr.MultiGetFileArgs'):
       return self._FormatADSResults(payload, flow_handle)
     if payload.pathspec.pathtype == jobs_pb2.PathSpec.PathType.REGISTRY:
       return self._FormatRegistryResult(payload)
     raise RuntimeError('Unsupported StatEntry type')
 
   def _FormatFileFinderInfoResult(self,
                                   payload: flows_pb2.FileFinderResult,
@@ -177,7 +194,69 @@
     """
     lines: list[str] = [
         f'    {payload.pathspec.path} '
         f'({jobs_pb2.StatEntry.RegistryType.Name(payload.registry_type)})']
     for descriptor, value in payload.registry_data.ListFields():
       lines.append(f'        {descriptor.name}: {value}')
     return lines
+
+  def _FormatDict(self,
+                  payload: jobs_pb2.Dict,
+                  flow_handle: flow.Flow) -> list[str]:
+    """Formats a Dict result type.
+
+    Currently supports the Dict returned from WMILogicalDisks artefact
+    collection only.
+
+    Args:
+      payload: The Dict payload to format.
+      flow_handle: The Flow the Dict entry originates from.
+
+    Returns:
+      A list of strings, one per line, of formatted output.
+
+    Raises:
+      RuntimeError: If the Dict type is unsupported.
+    """
+    args_typename = flow_handle.data.args.TypeName()
+    if args_typename == 'grr.ArtifactCollectorFlowArgs':
+      acf_args = flows_pb2.ArtifactCollectorFlowArgs.FromString(
+          flow_handle.data.args.value)
+      if len(acf_args.artifact_list) == 1:
+        if 'WMILogicalDisks' in acf_args.artifact_list:
+          return self._FormatWindowsVolumes(payload)
+    raise RuntimeError('Unsupported Dict type')
+
+  def _FormatWindowsVolumes(self, payload: jobs_pb2.Dict) -> list[str]:
+    """Formats the Dict response from a WMILogicalDisks artefact.
+
+    Args:
+      payload: The Dict payload to format.
+
+    Returns:
+      A list of strings, one per line, of formatted output.
+    """
+    fields: dict[str, Any] = {}
+    for dat in payload.dat:
+      if dat.k.string in _WINDOWS_VOLUME_DESIRED_FIELDS_MAP:
+        fields[dat.k.string] = (
+            _WINDOWS_VOLUME_DESIRED_FIELDS_MAP[dat.k.string](dat.v))
+
+    size_natural = humanize.naturalsize(
+        fields['Size'], binary=True, format='%.1f')
+    free_space_natural = humanize.naturalsize(
+        fields['FreeSpace'], binary=True, format='%.1f')
+    free_space_percentage = round(fields['FreeSpace'] / fields['Size'] * 100, 2)
+
+    lines: list[str] = []
+    lines.append(f'Device ID - {fields["DeviceID"]}')
+    lines.append(f'    Name:                 {fields["Name"]}')
+    lines.append(f'    Volume Name:          {fields["VolumeName"]}')
+    lines.append(f'    Volume Serial Number: {fields["VolumeSerialNumber"]}')
+    lines.append(f'    Description:          {fields["Description"]}')
+    lines.append(f'    Drive Type:           {fields["DriveType"]}')
+    lines.append(f'    File System:          {fields["FileSystem"]}')
+    lines.append(f'    Size:                 {fields["Size"]} ({size_natural})')
+    lines.append(f'    Free Space:           {fields["FreeSpace"]} '
+                 f'({free_space_natural}) - {free_space_percentage}%')
+
+    return lines
```

### Comparing `grrshell-20231227/grrshell/lib/grr_shell_client.py` & `grrshell-20240405/grrshell/lib/grr_shell_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,44 +18,48 @@
 import datetime
 import io
 import os
 import re
 import shutil
 import tempfile
 import threading
-import time
 import traceback
 from typing import Iterator, Optional
 import zipfile
 
 from absl import logging
 
 from grr_api_client import artifact as grr_artifact
 from grr_api_client import errors as grr_errors
 from grr_api_client import flow
 from grr_api_client import api as grr_api
 from grr_response_proto import artifact_pb2
 from grr_response_proto import flows_pb2
 from grr_response_proto import jobs_pb2
+from grr_response_proto import timeline_pb2
+from grr_response_proto.api import flow_pb2
 from grrshell.lib import client_monitors
 from grrshell.lib import errors
 from grrshell.lib import flow_args_parsers
 from grrshell.lib import formatters
 from grrshell.lib import utils
 
 
 _STALE_TIMELINE_THRESHOLD = datetime.timedelta(hours=12)
-_ROOT_TIMELINE_REGEX = r'/|(?:/?)[A-Z]:[/\\]'
+_WINDOWS_ROOT_TIMELINE_REGEX = r'^(?:/?)[A-Z]:[/\\]$'
+_LINUX_ROOT_TIMELINE_REGEX = r'^/$'
+
 
 _RESUMABLE_FLOW_TYPES = frozenset((
     'ClientFileFinder',
     'ArtifactCollectorFlow',
     'GetFile',
     'CollectFilesByKnownPath',
-    'CollectBrowserHistory'
+    'CollectBrowserHistory',
+    'MultiGetFile'
 ))
 
 _BACKGROUND_ARTEFACT_TYPES = frozenset((
     artifact_pb2.ArtifactSource.SourceType.ARTIFACT_FILES,
     artifact_pb2.ArtifactSource.SourceType.ARTIFACT_GROUP,
     artifact_pb2.ArtifactSource.SourceType.FILE,
     artifact_pb2.ArtifactSource.SourceType.PATH,
@@ -110,14 +114,15 @@
     self._grr_client_id = self._ResolveClientID(client_id)
     self._grr_client = self._grr_stubby.Client(self._grr_client_id)
     self._os: str = None
     self._max_collect_size = max_collect_size
     self._artefacts: dict[str, grr_artifact.Artifact] = {}
     self.last_timeline_time = 0
     self._formatter = formatters.GRRShellFormatter()
+    self._pathspec_mapper = _PathSpecMapper()
 
     self._artefact_list_mutex: threading.Lock = threading.Lock()
     threading.Thread(
         target=self._RetrieveSupportedArtefacts, daemon=True).start()
 
     self._flow_monitor = client_monitors.FlowMonitor(
         self._grr_stubby.Client(self._grr_client_id))
@@ -158,33 +163,43 @@
     """
     try:
       self._grr_client.VerifyAccess()
     except grr_errors.AccessForbiddenError:
       return False
     return True
 
-  def RequestAccess(self) -> None:
-    """Creates an access request and waits for the request to be granted."""
+  def RequestAccess(self) -> bool:
+    """Requests access to the client.
+
+    Prompts the user for access parameters and then waits for approval to be
+    granted.
+
+    Returns:
+      True is access was grented, False otherwise.
+    """
     reason = input('Enter access justification: ')
     approvers = input('Enter comma separated approvers: ').split(',')
 
     approval_req = self._grr_client.CreateApproval(
-        reason=reason, notified_users=approvers)
+        reason=reason,
+        notified_users=approvers)
 
     logger.debug('Approval request sent: %s', approval_req.data)
 
     print(
         f'Approval URL: {self._grr_endpoint}/v2/clients/'
         f'{self._grr_client_id}/users/{approval_req.data.requestor}/approvals/'
         f'{approval_req.data.id}\n<CTRL+C> to abandon session.')
 
     approval_req.WaitUntilValid()
 
     print('Approval received, proceeding.')
 
+    return True
+
   def StartBackgroundMonitors(self) -> None:
     """Starts background monitors."""
     self._flow_monitor.StartMonitor()
     self._last_seen_monitor.StartMonitor()
 
   def GetOS(self) -> str:
     """Gets the operating system of the client.
@@ -224,30 +239,34 @@
 
     Returns:
       The Flow ID of the most recent timeline that is not older than the
         staleness threshold.
     """
     flows = self._grr_client.ListFlows()
     latest_timeline = None
-    latest_timestamp = (
-        time.time() - _STALE_TIMELINE_THRESHOLD.total_seconds()
-    ) * 1000000
+    latest_timestamp = (datetime.datetime.now().timestamp()
+                        - _STALE_TIMELINE_THRESHOLD.total_seconds()) * 1000000
+
     for f in flows:
       if f.data.state != flows_pb2.FlowContext.TERMINATED:
         continue
       if f.data.name != 'TimelineFlow':
         continue
-      if not re.fullmatch(
-          _ROOT_TIMELINE_REGEX, str(f.Get().args.root, 'utf-8')
-      ):
+      if f.data.last_active_at < latest_timestamp:
+        continue
+
+      root = f.Get().args.root.decode('utf-8')
+      regex = (_WINDOWS_ROOT_TIMELINE_REGEX if self.GetOS() == utils.WINDOWS
+               else _LINUX_ROOT_TIMELINE_REGEX)
+      if not re.fullmatch(regex, root):
         continue
-      for result in f.ListResults():
-        if result.timestamp > latest_timestamp:
-          latest_timestamp = result.timestamp
-          latest_timeline = f.flow_id
+
+      # If we got this far, then we have found a more recent TimelineFlow
+      latest_timestamp = f.data.last_active_at
+      latest_timeline = f.flow_id
 
     return latest_timeline
 
   def CollectTimeline(self,
                       path: Optional[str] = None,
                       existing_timeline: Optional[str] = None) -> bytes:
     """Creates and waits for a GRR timeline flow.
@@ -281,23 +300,44 @@
       logger.debug('TimelineFlow Args:\n%s', flow_args)
 
     flow_handle.WaitUntilDone()
 
     logger.debug('Timeline flow complete, collecting and decoding')
 
     results = flow_handle.ListResults()
+    filesystem = 'UNKNOWN'
     for result in results:
+      payload: timeline_pb2.TimelineResult = result.payload  # pytype: disable=annotation-type-mismatch
+      filesystem = payload.filesystem_type
       self.last_timeline_time = result.timestamp
       break
 
     io_stream = io.BytesIO()
     body = flow_handle.GetCollectedTimelineBody()
     body.WriteToStream(io_stream)
+    timeline_bytes = io_stream.getvalue()
+
+    args: timeline_pb2.TimelineArgs = flow_handle.args  # pytype: disable=annotation-type-mismatch
+    timeline_root = args.root.decode('utf-8')
+
+    if self.GetOS() == utils.WINDOWS:
+      if timeline_root == '/':
+        # We're on windows, with a timeline root of '/' - We need to inspect the
+        # timeline result to get the true root: Probably 'C:' but that's not
+        # guaranteed. The timeline's first 6 bytes will tell us, eg: b'0|C:\\'
+        timeline_root = (timeline_bytes[0:6].decode('utf-8')
+                         .replace('0|', '').replace(r'\\', '/'))
+        logger.debug('Inspected timeline data to identify timeline root of %s',
+                     timeline_root)
+      if timeline_root[0] == '/':
+        timeline_root = timeline_root[1:]
+
+    self._TrackPathSpecForPath(timeline_root, filesystem)
 
-    return io_stream.getvalue()
+    return timeline_bytes
 
   def FileInfo(self, remote_path: str, collect_ads: bool = False) -> str:
     """Synchronously collects file info and hashes for remote files.
 
     Also attempts to collect the "Zone.Identifier" Alternate Data Stream for
     single files on windows. (Multiple files are not supported currently:
     b/288501445)
@@ -468,15 +508,15 @@
         bg_flow.flow = bg_flow.flow.Get()
       if bg_flow.flow.data.state == flows_pb2.FlowContext.TERMINATED:
         if running:
           state = 'DOWNLOADING'
         else:
           state = 'COMPLETE'
       else:
-        state = flows_pb2.FlowContext.State.Name(bg_flow.flow.data.state)
+        state = flow_pb2.ApiFlow.State.Name(bg_flow.flow.data.state)
 
       param = flow_args_parsers.Parse(bg_flow.flow)[0]
 
       error_msg = ''
       if not running and bg_flow.future.exception():
         error_msg = f' "{str(bg_flow.future.exception())}"'
         bg_flow.exception_displayed = True
@@ -518,19 +558,25 @@
     Returns:
       A string with details, one per line, of floaws launched on the client.
     """
     lines: list[str] = []
     flows = self._flow_monitor.GetFlowsInfoList(count=count)
 
     for flow_handle in flows:
+      if self._flow_monitor.IsFlowCached(flow_handle.flow_id):
+        flow_arg = flow_args_parsers.Parse(flow_handle)[0]
+      else:
+        flow_arg = '<UNCACHED FLOW ARGS>'
+
       lines.append(
           f'\t{flow_handle.flow_id} '
           f'{utils.UnixTSToReadable(flow_handle.data.started_at / 1000000)} '
-          f'{flow_handle.data.name} {flow_args_parsers.Parse(flow_handle)[0]} '
-          f'{flows_pb2.FlowContext.State.Name(flow_handle.data.state)}')
+          f'{flow_handle.data.name} {flow_arg} '
+          f'{flow_pb2.ApiFlow.State.Name(flow_handle.data.state)}')
+
     return '\n'.join(lines)
 
   def ReattachFlow(self,
                    flow_id: str,
                    local_path: Optional[str] = None) -> list[str]:
     """Resumes an existing flow, not attached to this GRRShell session.
 
@@ -603,15 +649,15 @@
 
     logger.debug('Flow args: %s', flow_handle.data)
 
     lines: list[str] = [
         flow_handle.data.name,
         f'\tCreator     {flow_handle.data.creator}',
         ('\tState       ' +
-         flows_pb2.FlowContext.State.Name(flow_handle.data.state)),
+         flow_pb2.ApiFlow.State.Name(flow_handle.data.state)),
         ('\tStarted     ' +
          utils.UnixTSToReadable(flow_handle.data.started_at / 1000000)),
         ('\tLast Active ' +
          utils.UnixTSToReadable(flow_handle.data.last_active_at / 1000000)),
         '\tArgs:']
 
     for l in flow_args_parsers.Parse(flow_handle, True):
@@ -637,14 +683,48 @@
         error_message = '\t\tMissing error message'
 
       lines.append('\tError Details')
       lines.append(error_message)
 
     return '\n'.join(lines)
 
+  def DescribeVolumes(self) -> str:
+    """Get information on volumes connected to the client."""
+    if self.GetOS() == utils.WINDOWS:
+      artefact = 'WMILogicalDisks'
+    elif self.GetOS() == utils.LINUX:
+      raise NotImplementedError('Linux volume information not yet supported')
+    elif self.GetOS() == utils.DARWIN:
+      raise NotImplementedError('Darwin volume information not yet supported')
+    else:
+      raise RuntimeError('Unknown OS')
+
+    ac_flow = self._CreateArtefactCollectorFlow(artefact)
+    ac_flow.WaitUntilDone()
+
+    logger.debug('Flow result: %s', ac_flow.data)
+
+    return '\n'.join(self._formatter.FormatFlowResult(ac_flow))
+
+  def _TrackPathSpecForPath(self, root: str, filesystem: str) -> None:
+    """Adds a path/pathspec to the client.
+
+    This mapping is used to determine which pathspec value should be used in
+    ClientFileFinder flows (`ntfs` for `ntfs`, `os` for all others.)
+
+    Args:
+      root: The timeline / mount point root
+      filesystem: The filesystem for the mount point
+    """
+    logger.debug('Setting root / filesystem map value: %s for %s',
+                 root, filesystem)
+    self._pathspec_mapper[root] = (
+        jobs_pb2.PathSpec.NTFS if filesystem.lower() == 'ntfs'
+        else jobs_pb2.PathSpec.OS)
+
   def _ResolveClientID(self, client_id: str) -> str:
     """Resolves a client id or hostname to a client id.
 
     Args:
       client_id: A FQDN or GRR client ID.
 
     Returns:
@@ -694,19 +774,17 @@
     """
     logger.debug('Launching a ClientFileFinder flow')
 
     flow_args: flows_pb2.FileFinderArgs = (
         self._grr_stubby.types.CreateFlowArgs('ClientFileFinder'))
 
     if self.GetOS() == utils.WINDOWS:
-      flow_args.pathtype = jobs_pb2.PathSpec.NTFS
       if remote_path.startswith('/'):
         remote_path = remote_path[1:]
-    else:
-      flow_args.pathtype = jobs_pb2.PathSpec.OS
+    flow_args.pathtype = self._pathspec_mapper[remote_path]
 
     flow_args.paths.append(remote_path)
     flow_args.action.action_type = action
     if self._max_collect_size:
       if action == flows_pb2.FileFinderAction.HASH:
         flow_args.action.hash.max_size = self._max_collect_size
       elif action == flows_pb2.FileFinderAction.DOWNLOAD:
@@ -718,19 +796,20 @@
     logger.debug('Launched flow %s', ff_flow.flow_id)
     logger.debug('Flow args: %s', ff_flow.data)
 
     return ff_flow
 
   def _CreateADSCollectionFlow(self, remote_path: str) -> flow.Flow:
     """Creates a GetFile flow for a Zone.Identifier ADS of a file."""
-    flow_args = flows_pb2.GetFileArgs(
-        pathspec=jobs_pb2.PathSpec(path=remote_path,
-                                   pathtype=jobs_pb2.PathSpec.NTFS,
-                                   stream_name='Zone.Identifier'))
-    ads_flow = self._grr_client.CreateFlow(name='GetFile',
+    flow_args = flows_pb2.MultiGetFileArgs(
+        pathspecs=[jobs_pb2.PathSpec(path=remote_path,
+                                     pathtype=jobs_pb2.PathSpec.NTFS,
+                                     stream_name='Zone.Identifier')])
+
+    ads_flow = self._grr_client.CreateFlow(name='MultiGetFile',
                                            args=flow_args)
 
     logger.debug('Launched flow %s', ads_flow.flow_id)
     logger.debug('Flow args: %s', ads_flow.data)
 
     return ads_flow
 
@@ -792,15 +871,14 @@
       ff_flow: The Flow to collect a result from.
       local_path: The local path to export the results to.
 
     Raises:
       InvalidRemotePathError: If the flow found no files at the remote path.
     """
     logger.debug('Exporting results for flow: %s', ff_flow.flow_id)
-    os_base = 'ntfs' if self.GetOS() == utils.WINDOWS else 'os'
 
     if not list(ff_flow.ListResults()):
       raise errors.InvalidRemotePathError(
           f'No FileFinder results for {ff_flow.flow_id}')
 
     with tempfile.NamedTemporaryFile(mode='wb+') as fp:
       logger.debug('Writing zip file for %s to %s', ff_flow.flow_id, fp.name)
@@ -818,25 +896,31 @@
               file_info.filename.endswith(
                   f'{self._grr_client.client_id}/client_info.yaml')):
             logger.debug('Skipping extraction of %s based on filename match',
                          file_info.filename)
             continue
           logger.debug('Extracting %s to %s', file_info.filename, local_path)
 
+          # 4th path component varies depending on collection pathtype
+          os_base = file_info.filename.split(os.path.sep)[3]
+
           nested_file_path = file_info.filename.replace(
               os.path.join(zip_root_dir, self._grr_client.client_id, 'fs',
                            os_base) + os.path.sep, '')
           dest_file_path = os.path.join(local_path, nested_file_path)
+          dest_file_path = dest_file_path.replace(':', '_')  # Windows volumes
           os.makedirs(os.path.dirname(dest_file_path), exist_ok=True)
 
           extracted_file = zip_file.extract(file_info, local_path)
           logger.debug('Moving %s to %s', extracted_file, dest_file_path)
           shutil.move(extracted_file, dest_file_path)
 
         try:
+          logger.debug('Removing zip root directory: %s',
+                       os.path.join(local_path, zip_root_dir))
           shutil.rmtree(os.path.join(local_path, zip_root_dir))
         except FileNotFoundError:
           # Failing to remove something that doesn't exist is fine.
           pass
 
   def _CreateOutputDir(self, local_path: str) -> None:
     """Creates a directory for collected file output.
@@ -864,15 +948,15 @@
       bool: True if resuming the flow should be synchronous, False for
         asynchronous.
 
     Raises:
       NotResumeableFlowTypeError: If the flow is not supported for resumption.
       RuntimeError: If an artefact is unsupported.
     """
-    if flow_handle.data.name == 'GetFile':
+    if flow_handle.data.name in ('GetFile', 'MultiGetFile'):
       return True
     if flow_handle.data.name in ('CollectFilesByKnownPath',
                                  'CollectBrowserHistory'):
       return False
     if flow_handle.data.name == 'ArtifactCollectorFlow':
       acf_args = flows_pb2.ArtifactCollectorFlowArgs.FromString(
           flow_handle.data.args.value)
@@ -929,7 +1013,34 @@
 
     if any(s.supported_os for s in sources):
       for s in sources:
         if self.GetOS() in s.supported_os:
           return s.type
 
     raise RuntimeError(f'Unsupported artefact "{artefact}"')
+
+
+class _PathSpecMapper:
+  """A helper class to manage mapping timeline roots to PathSpecs."""
+
+  def __init__(self) -> None:
+    """Initialise the object."""
+    self._path_ps_map: dict[str, jobs_pb2.PathSpec.PathType] = {}
+
+  def __getitem__(self, key: str) -> jobs_pb2.PathSpec.PathType:
+    """Override square bracket operator (fetch)."""
+    longest_match = 0
+    matching_key: str = None
+
+    for curr_key in self._path_ps_map:
+      curr_match_length = len(os.path.commonprefix([key, curr_key]))
+      if curr_match_length > longest_match:
+        longest_match = curr_match_length
+        matching_key = curr_key
+
+    if not matching_key:
+      return jobs_pb2.PathSpec.OS  # Default
+    return self._path_ps_map[matching_key]
+
+  def __setitem__(self, key: str, value: jobs_pb2.PathSpec.PathType) -> None:
+    """Override square bracket operator (assignment)."""
+    self._path_ps_map[key] = value
```

### Comparing `grrshell-20231227/grrshell/lib/grr_shell_emulated_fs.py` & `grrshell-20240405/grrshell/lib/grr_shell_emulated_fs.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 from grrshell.lib import errors
 from grrshell.lib import utils
 
 
 logger = logging.logging.getLogger('grrshell')
 
-_ENCODINGS = frozenset(('utf-8', 'cp1251'))
+_ENCODINGS = ['utf-8', 'cp1251']  # Order is important, so can't use a frozenset
 
 
 # GRR timelines use the Sleuthkit format
 # https://wiki.sleuthkit.org/index.php?title=Body_file
 # MD5|name|inode|mode_as_string|UID|GID|size|atime|mtime|ctime|crtime
 @dataclasses.dataclass(eq=True)
 class _TimelineRow:
@@ -358,15 +358,15 @@
       raise errors.InvalidRemotePathError(f'Invalid directory: {basedir}')
 
     directory = self._ResolveRemotePathToEmulatedFS(basedir)
     if not isinstance(directory, _EmulatedDirectory):
       raise errors.IsAFileError(
           f'Starting directory is actually a file: {basedir}')
 
-    matcher = re.compile(needle)
+    matcher = re.compile(needle, flags=re.IGNORECASE)
     results = self._GetFSTreeFromPath(directory)
     results = [r.stats.name for r in results if matcher.search(r.stats.name)]
 
     return sorted(results)
 
   def _AddRowToEmulatedFS(self,
                           row: _TimelineRow,
```

### Comparing `grrshell-20231227/grrshell/lib/grr_shell_repl.py` & `grrshell-20240405/grrshell/lib/grr_shell_repl.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,14 +94,16 @@
 _REFRESH_HELP_LONG = """\tOptionally provide a path to collect the TimelineFlow for a subdirectory."""
 _RESUME_HELP_LONG = """\tRequires a Flow ID argument. (Re)attaches the flow to the current GRRShell session.
 \tClientFileFinder, ArtifactCollectorFlow, and GetFile (Zone.Identifier ADS only) are supported.
 \tResuming an asynchronous flow will download the flow results in the background.
 \tSynchronous flows will display the flow result."""
 _SET_LONG_HELP = """\tCurrently supported shell env values:
 \t* max-file-size Specify a max file size for file collections. If not specified, the GRR default of 500MB is used."""
+_VOLUMES_LONG_HELP = """\t List volumes connected to the client.
+\tNon-root volumes do not have timelines collected. Use "refresh <volume> to browse the volume EFS."""
 # pylint: enable=line-too-long
 
 # go/keep-sorted start
 _ARTEFACT_HELP = _Help(
     '\tLaunch and download an ArtifactCollectorFlow (asynchronous)',
     _ARTEFACT_HELP_LONG)
 _CD_HELP = _Help('\tChange directory')
@@ -121,14 +123,16 @@
 _LS_HELP = _Help('\tList directory entries, with an optional path argument.',
                  _LS_HELP_LONG)
 _PWD_HELP = _Help('\tPrint current directory')
 _REFRESH_HELP = _Help('\tRefresh remote emulated FS (synchronous)',
                       _REFRESH_HELP_LONG)
 _RESUME_HELP = _Help('\tResume an existing flow', _RESUME_HELP_LONG)
 _SET_HELP = _Help('\tSet a shell value', _SET_LONG_HELP)
+_VOLUMES_HELP = _Help('\tList volumes connected to the client',
+                      _VOLUMES_LONG_HELP)
 # go/keep-sorted end
 
 
 class GRRShellREPL:
   """GRR Shell REPL driver."""
 
   def __init__(self,
@@ -215,15 +219,16 @@
         _Command('help', self._PrintHelp, _HELP_HELP),
         _Command('info', self._Info, _INFO_HELP, path_param=True),
         _Command('ls', self._Ls, _LS_HELP, path_param=True),
         _Command('pwd', self._Pwd, _PWD_HELP),
         _Command('quit', self._Exit, _EXIT_HELP, is_alias=True),
         _Command('refresh', self._Refresh, _REFRESH_HELP, path_param=True),
         _Command('resume', self._Resume, _RESUME_HELP),
-        _Command('set', self._Set, _SET_HELP)
+        _Command('set', self._Set, _SET_HELP),
+        _Command('volumes', self._Volumes, _VOLUMES_HELP),
         # go/keep-sorted end
     ]
     return {c.name: c for c in commands}
 
   def _GenerateHelp(self) -> str:
     """Generates the help string based of the available commands.
 
@@ -337,14 +342,16 @@
     windows_volume_root_regex = re.compile('^[A-Z]:$')
 
     if path == '.':
       path = self._emulated_fs.GetPWD()
     elif windows_volume_root_regex.match(path):
       path += '/'
 
+    logger.debug('Refreshing timeline for %s', path)
+
     timeline_data = self._grr_shell_client.CollectTimeline(
         path, existing_timeline)
     # Zero out the path we're refreshing.
     self._emulated_fs.ClearPath(path,
                                 self._grr_shell_client.last_timeline_time)
 
     self._emulated_fs.ParseTimelineFlow(
@@ -601,14 +608,19 @@
     if len(params) != 1:
       print('detail requires exactly 1 Flow ID argument. Usage:')
       print(self._commands['detail'].help)
       return
 
     print(self._grr_shell_client.FlowDetail(params[0]))
 
+  def _Volumes(self, params: Sequence[str]) -> None:
+    """Lists information for all voilumes attached to the client."""
+    del params  # unused
+    print(self._grr_shell_client.DescribeVolumes())
+
 
 class _GrrShellREPLPromptCompleter(prompt_toolkit.completion.Completer):
   """Implements autocomplete for the GRR Shell REPL.
 
   Uses the emulated FS for path completion, and also generates completions for
   commands.
   """
```

### Comparing `grrshell-20231227/grrshell/lib/utils.py` & `grrshell-20240405/grrshell/lib/utils.py`

 * *Files identical despite different names*

### Comparing `grrshell-20231227/grrshell/tests/flow_args_parsers_test.py` & `grrshell-20240405/grrshell/tests/flow_args_parsers_test.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Unit tests for GRR Flow Args parsing functions."""
 
-# pylint: disable=wrong-import-order
+# pylint: disable=wrong-import-order,ungrouped-imports
 from unittest import mock
 
 from google.protobuf import text_format
 from grr_api_client import flow
 from grr_response_proto.api import flow_pb2
 from grrshell.lib import flow_args_parsers
 from absl.testing import absltest
@@ -115,14 +115,35 @@
         _MOCK_APIFLOW_COLLECTBROWSERHIST_PROTO_FILE, 'rb').read(),
                            flow_pb2.ApiFlow()), context=mock.MagicMock())
 _MOCK_APIFLOW_COLLECTBROWSERHIST_EXPECTED_SINGLE = [
     'FIREFOX,CHROME,INTERNET_EXPLORER']
 _MOCK_APIFLOW_COLLECTBROWSERHIST_EXPECTED_MULTI = [
     'Browser: FIREFOX', 'Browser: CHROME', 'Browser: INTERNET_EXPLORER']
 
+_MOCK_APIFLOW_MULTIGETFILE_SINGLE_PROTO_FILE = 'grrshell/tests/testdata/mock_apiflow_multigetfile_running_single.textproto'
+_MOCK_APIFLOW_MULTIGETFILE_SINGLE = flow.Flow(
+    data=text_format.Parse(open(
+        _MOCK_APIFLOW_MULTIGETFILE_SINGLE_PROTO_FILE, 'rb').read(),
+                           flow_pb2.ApiFlow()), context=mock.MagicMock())
+_MOCK_APIFLOW_MULTIGETFILE_SINGLE_EXPECTED_SINGLE = [
+    'C:/Users/username/Downloads/Firefox Installer.exe:Zone.Identifier']
+_MOCK_APIFLOW_MULTIGETFILE_SINGLE_EXPECTED_MULTIPLE = [
+    'C:/Users/username/Downloads/Firefox Installer.exe:Zone.Identifier']
+
+_MOCK_APIFLOW_MULTIGETFILE_MULTIPLE_PROTO_FILE = 'grrshell/tests/testdata/mock_apiflow_multigetfile_running_multiple.textproto'
+_MOCK_APIFLOW_MULTIGETFILE_MULTIPLE = flow.Flow(
+    data=text_format.Parse(open(
+        _MOCK_APIFLOW_MULTIGETFILE_MULTIPLE_PROTO_FILE, 'rb').read(),
+                           flow_pb2.ApiFlow()), context=mock.MagicMock())
+_MOCK_APIFLOW_MULTIGETFILE_MULTIPLE_EXPECTED_SINGLE = [
+    '<MULTIPLE PATHS>']
+_MOCK_APIFLOW_MULTIGETFILE_MULTIPLE_EXPECTED_MULTIPLE = [
+    'C:/Users/username/Downloads/Firefox Installer.exe:Zone.Identifier',
+    'C:/Users/username/Downloads/Safari Installer.exe']
+
 
 class FlowArgsParsersTest(parameterized.TestCase):
   """Unit tests for GRR Flow Args parsing functions."""
 
   @parameterized.named_parameters(
       ('artefact_single_singleline', _MOCK_APIFLOW_ARTEFACTCOLLECTOR_SINGLE,
        False, _MOCK_APIFLOW_ARTEFACT_SINGLE_EXPECTED_SINGLE),
@@ -160,14 +181,22 @@
        False, _MOCK_APIFLOW_COLLECTFILES_MULTIPLE_EXPECTED_SINGLE),
       ('collectfiles_multiple_multiline', _MOCK_APIFLOW_COLLECTFILES_MULTIPLE,
        True, _MOCK_APIFLOW_COLLECTFILES_MULTIPLE_EXPECTED_MULTI),
       ('collectbrowserhistory_singleline', _MOCK_APIFLOW_COLLECTBROWSERHIST,
        False, _MOCK_APIFLOW_COLLECTBROWSERHIST_EXPECTED_SINGLE),
       ('collectbrowserhistory_multiline', _MOCK_APIFLOW_COLLECTBROWSERHIST,
        True, _MOCK_APIFLOW_COLLECTBROWSERHIST_EXPECTED_MULTI),
+      ('multigetfiles_single_singleline', _MOCK_APIFLOW_MULTIGETFILE_SINGLE,
+       False, _MOCK_APIFLOW_MULTIGETFILE_SINGLE_EXPECTED_SINGLE),
+      ('multigetfiles_single_multiline', _MOCK_APIFLOW_MULTIGETFILE_SINGLE,
+       True, _MOCK_APIFLOW_MULTIGETFILE_SINGLE_EXPECTED_MULTIPLE),
+      ('multigetfiles_multiple_singleline', _MOCK_APIFLOW_MULTIGETFILE_MULTIPLE,
+       False, _MOCK_APIFLOW_MULTIGETFILE_MULTIPLE_EXPECTED_SINGLE),
+      ('multigetfiles_multiple_multiline', _MOCK_APIFLOW_MULTIGETFILE_MULTIPLE,
+       True, _MOCK_APIFLOW_MULTIGETFILE_MULTIPLE_EXPECTED_MULTIPLE),
   )
   def test_Parse(self,
                  flow_handle: flow.Flow,
                  multiline: bool,
                  expected_output: list[str]):
     """Tests the Parse function in flow_args_parsers."""
     output = flow_args_parsers.Parse(flow_handle, multiline)
```

### Comparing `grrshell-20231227/grrshell/tests/grr_shell_client_test.py` & `grrshell-20240405/grrshell/tests/grr_shell_client_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,22 +9,23 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Unit tests for the Grr Shell client."""
 
-# pylint: disable=wrong-import-order
+# pylint: disable=wrong-import-order,ungrouped-imports
 from concurrent import futures
 import contextlib
 import datetime
 import io
 import os
 import sys
 from unittest import mock
+import unittest
 
 from google.protobuf import text_format
 from grr_api_client import api as grr_api
 from grr_api_client import artifact
 from grr_api_client import client
 from grr_api_client import errors as grr_errors
 from grr_api_client import flow
@@ -86,14 +87,20 @@
 
 _MOCK_APIFLOW_ARTEFACTCOLLECTOR_WINREGKEY_RUNNING_PROTO_FILE = 'grrshell/tests/testdata/mock_apiflow_artifactcollector_windowsregkey_running.textproto'
 _MOCK_APIFLOW_ARTEFACTCOLLECTOR_WINREGKEY_RUNNING = flow.Flow(
     data=text_format.Parse(open(
         _MOCK_APIFLOW_ARTEFACTCOLLECTOR_WINREGKEY_RUNNING_PROTO_FILE, 'rb').read(),
                            flow_pb2.ApiFlow()), context=mock.MagicMock())
 
+_MOCK_APIFLOW_ARTEFACTCOLLECTOR_WMILOGICALDISKS_RUNNING_PROTO_FILE = 'grrshell/tests/testdata/mock_apiflow_artifactcollector_wmilogicaldisks_running.textproto'
+_MOCK_APIFLOW_ARTEFACTCOLLECTOR_WMILOGICALDISKS_RUNNING = flow.Flow(
+    data=text_format.Parse(open(
+        _MOCK_APIFLOW_ARTEFACTCOLLECTOR_WMILOGICALDISKS_RUNNING_PROTO_FILE, 'rb').read(),
+                           flow_pb2.ApiFlow()), context=mock.MagicMock())
+
 _MOCK_APIFLOW_CFF_HASH_RUNNING_PROTO_FILE = 'grrshell/tests/testdata/mock_apiflow_clientfilefinder_hash_running.textproto'
 _MOCK_APIFLOW_CFF_HASH_RUNNING = flow.Flow(data=text_format.Parse(
     open(_MOCK_APIFLOW_CFF_HASH_RUNNING_PROTO_FILE, 'rb').read(),
     flow_pb2.ApiFlow()), context=mock.MagicMock())
 _MOCK_APIFLOW_CFF_DOWNLOAD_RUNNING_PROTO_FILE = 'grrshell/tests/testdata/mock_apiflow_clientfilefinder_download_running.textproto'
 _MOCK_APIFLOW_CFF_DOWNLOAD_RUNNING = flow.Flow(data=text_format.Parse(
     open(_MOCK_APIFLOW_CFF_DOWNLOAD_RUNNING_PROTO_FILE, 'rb').read(),
@@ -287,23 +294,55 @@
 _MOCK_WINDOWS_ARTEFACT_REGVALUE = flow.FlowResult(data=text_format.Parse(
     open(_MOCK_WINDOWS_ARTEFACT_REGVALUE_PROTO_FILE, 'rb').read(),
     flow_pb2.ApiFlowResult()))
 
 _EXPECTED_WINDOWS_REGVALUE_RESULT = """    /HKEY_LOCAL_MACHINE/SOFTWARE/Microsoft/Windows NT/CurrentVersion/InstallDate (REG_DWORD)
         integer: 12345"""
 
+_MOCK_WINDOWS_ARTEFACT_VOLUME_C_PROTO_FILE = 'grrshell/tests/testdata/mock_volume_windows_c.textproto'
+_MOCK_WINDOWS_ARTEFACT_VOLUME_C = flow.FlowResult(data=text_format.Parse(
+    open(_MOCK_WINDOWS_ARTEFACT_VOLUME_C_PROTO_FILE, 'rb').read(),
+    flow_pb2.ApiFlowResult()))
+
+_MOCK_WINDOWS_ARTEFACT_VOLUME_D_PROTO_FILE = 'grrshell/tests/testdata/mock_volume_windows_d.textproto'
+_MOCK_WINDOWS_ARTEFACT_VOLUME_D = flow.FlowResult(data=text_format.Parse(
+    open(_MOCK_WINDOWS_ARTEFACT_VOLUME_D_PROTO_FILE, 'rb').read(),
+    flow_pb2.ApiFlowResult()))
+
+_EXPECTED_WINDOWS_VOLUMES_RESULT = """Device ID - C:
+    Name:                 C:
+    Volume Name:          c_drive
+    Volume Serial Number: 01234567
+    Description:          Local Fixed Disk
+    Drive Type:           DRIVE_FIXED
+    File System:          NTFS
+    Size:                 2047370850304 (1.9 TiB)
+    Free Space:           1654566748160 (1.5 TiB) - 80.81%
+Device ID - D:
+    Name:                 D:
+    Volume Name:          THUMBDRIVE
+    Volume Serial Number: 98765432
+    Description:          Removable Disk
+    Drive Type:           DRIVE_REMOVABLE
+    File System:          FAT32
+    Size:                 8002781184 (7.5 GiB)
+    Free Space:           8002740224 (7.5 GiB) - 100.0%"""
+
 _MOCK_ZIP_DARWIN_CLIENTFILEFINDER_FILE = 'grrshell/tests/testdata/file_collect_darwin.zip'
 _MOCK_ZIP_DARWIN_CLIENTFILEFINDER_DATA = open(
     _MOCK_ZIP_DARWIN_CLIENTFILEFINDER_FILE, 'rb').read()
 _MOCK_ZIP_LINUX_CLIENTFILEFINDER_FILE = 'grrshell/tests/testdata/file_collect_linux.zip'
 _MOCK_ZIP_LINUX_CLIENTFILEFINDER_DATA = open(
     _MOCK_ZIP_LINUX_CLIENTFILEFINDER_FILE, 'rb').read()
 _MOCK_ZIP_WINDOWS_CLIENTFILEFINDER_FILE = 'grrshell/tests/testdata/file_collect_windows.zip'
 _MOCK_ZIP_WINDOWS_CLIENTFILEFINDER_DATA = open(
     _MOCK_ZIP_WINDOWS_CLIENTFILEFINDER_FILE, 'rb').read()
+_MOCK_ZIP_WINDOWS_CLIENTFILEFINDER_FAT32_FILE = 'grrshell/tests/testdata/file_collect_windows_fat32.zip'
+_MOCK_ZIP_WINDOWS_CLIENTFILEFINDER_FAT32_DATA = open(
+    _MOCK_ZIP_WINDOWS_CLIENTFILEFINDER_FAT32_FILE, 'rb').read()
 _MOCK_ZIP_DARWIN_ARTIFACTCOLLECTORFLOW_FILE = 'grrshell/tests/testdata/artifact_collect_darwin.zip'
 _MOCK_ZIP_DARWIN_ARTIFACTCOLLECTORFLOW_DATA = open(
     _MOCK_ZIP_DARWIN_ARTIFACTCOLLECTORFLOW_FILE, 'rb').read()
 _MOCK_ZIP_LINUX_ARTIFACTCOLLECTORFLOW_FILE = 'grrshell/tests/testdata/artifact_collect_linux.zip'
 _MOCK_ZIP_LINUX_ARTIFACTCOLLECTORFLOW_DATA = open(
     _MOCK_ZIP_LINUX_ARTIFACTCOLLECTORFLOW_FILE, 'rb').read()
 _MOCK_ZIP_WINDOWS_ARTIFACTCOLLECTORFLOW_FILE = 'grrshell/tests/testdata/artifact_collect_windows.zip'
@@ -312,14 +351,17 @@
 _MOCK_ZIP_WINDOWS_GETFILE_ADS_FILE = 'grrshell/tests/testdata/getfile_ads.zip'
 _MOCK_ZIP_WINDOWS_GETFILE_ADS_DATA = open(
     _MOCK_ZIP_WINDOWS_GETFILE_ADS_FILE, 'rb').read()
 _MOCK_ZIP_WINDOWS_GETFILE_ADS_EMPTY_FILE = 'grrshell/tests/testdata/getfile_ads_empty.zip'
 _MOCK_ZIP_WINDOWS_GETFILE_ADS_EMPTY_DATA = open(
     _MOCK_ZIP_WINDOWS_GETFILE_ADS_EMPTY_FILE, 'rb').read()
 
+_SAMPLE_TIMELINE_LINUX = 'grrshell/tests/testdata/sample_timeline_linux'
+_SAMPLE_TIMELINE_WINDOWS = 'grrshell/tests/testdata/sample_timeline_windows'
+
 _MAX_FILE_SIZE_1GB = 1024 * 1024 * 1024
 
 
 # pylint: enable=line-too-long
 def _BuildMockArtifactDescriptors() -> list[artifact.Artifact]:
   """Builds the mock artifact descriptors list, used by ListArtifacts."""
   artifactdescriptor_proto_files = (
@@ -339,14 +381,23 @@
   for proto_file in artifactdescriptor_proto_files:
     to_return.append(artifact.Artifact(data=text_format.Parse(
         open(proto_file, 'rb').read(),
         artifact_pb2.ArtifactDescriptor()), context=mock.MagicMock()))
   return to_return
 
 
+def _MockGetFromFlowList(self) -> flow.Flow:
+  """Based on the flows listed in _MOCK_APIFLOW_LISTFLOWS, return the one matching the Flow ID."""
+  # TODO(ramoj): Use this method for all mocked calls to Flow.Get()
+  for item in _MOCK_APIFLOW_LISTFLOWS_FLOWS.items:
+    if self.data.flow_id == item.flow_id:
+      return flow.Flow(data=item, context=mock.MagicMock())
+  raise RuntimeError('Failure in mocking of Flow.Get() - Flow not found.')
+
+
 # pylint: disable=protected-access
 # pylint: enable=line-too-long
 
 
 class GrrShellClientLinuxTest(parameterized.TestCase):
   """Unit tests for the Grr Shell client."""
 
@@ -363,14 +414,15 @@
     self.mock_grr_api.Client.return_value.Get.return_value = _MOCK_LINUX_CLIENT
     self.mock_grr_api.SearchClients.return_value = [_MOCK_LINUX_CLIENT]
     self.mock_grr_api.ListArtifacts.return_value = (
         _BuildMockArtifactDescriptors())
 
     self.client = grr_shell_client.GRRShellClient(
         _TEST_GRR_URL, _TEST_GRR_USER, _TEST_GRR_PASS, _TEST_CLIENT_FQDN, _MAX_FILE_SIZE_1GB)
+    self.client._pathspec_mapper['/'] = jobs_pb2.PathSpec.OS
 
   def test_Init(self):
     """Tests initialisation."""
     self.assertIsNotNone(self.client)
 
   def test_GetOS(self):
     """Tests the GetOS method."""
@@ -392,35 +444,68 @@
     self.assertFalse(result)
 
   def test_CheckAccess(self):
     """Tests the CheckAccess method."""
     result = self.client.CheckAccess()
     self.assertTrue(result)
 
-  def test_RequestAccess(self):
+  @parameterized.named_parameters(
+      ('no_duration', None, 0),
+      ('with_duration', '25', 25),
+  )
+  @unittest.skip('Expiration duration not available in current public GRR API library version')
+  def test_RequestAccessSuccess(self,
+                                duration_input: str,
+                                expected_duration: int):
     """Tests the RequestAccess method."""
     with (
         mock.patch('builtins.input') as mock_input,
         mock.patch.object(
             self.client._grr_client, 'CreateApproval') as mock_create_approval):
-      mock_input.side_effect = ['The reason', 'approver1,approver2']
+      mock_input.side_effect = ['reason', 'approver1,approver2', duration_input]
       mock_create_approval.return_value.data.requestor = 'requestor'
       mock_create_approval.return_value.data.id = 'request_id'
 
       with io.StringIO() as buf, contextlib.redirect_stdout(buf):
-        self.client.RequestAccess()
+        result = self.client.RequestAccess()
 
         self.assertIn(
             'Approval URL: grr-url/v2/clients/'
             'C.0000000000000001/users/requestor/approvals/request_id',
             buf.getvalue())
 
       mock_create_approval.assert_called_once_with(
-          reason='The reason', notified_users=['approver1', 'approver2'])
+          reason='reason',
+          notified_users=['approver1', 'approver2'],
+          expiration_duration_days=expected_duration)
       mock_create_approval.return_value.WaitUntilValid.assert_called_once()
+      self.assertTrue(result)
+
+  @parameterized.named_parameters(
+      ('negative_duration', '-5', 'Invalid duration: -5'),
+      ('non_int_duration', 'asdf', 'Invalid duration: asdf'),
+  )
+  @unittest.skip('Expiration duration not available in current public GRR API library version')
+  def test_RequestAccessFailure(self,
+                                duration_input: str,
+                                expected_message: str):
+    """Tests the RequestAccess method failure methods."""
+    with (
+        mock.patch('builtins.input') as mock_input,
+        mock.patch.object(
+            self.client._grr_client, 'CreateApproval') as mock_create_approval):
+      mock_input.side_effect = ['reason', 'approver1,approver2', duration_input]
+
+      with io.StringIO() as buf, contextlib.redirect_stdout(buf):
+        result = self.client.RequestAccess()
+
+        self.assertIn(expected_message, buf.getvalue())
+
+      mock_create_approval.assert_not_called()
+      self.assertFalse(result)
 
   def test_Cleanup(self):
     """Tests destructor."""
     with mock.patch.object(self.client._collection_threads,
                            'shutdown') as mock_shutdown:
       self.client.WaitForBackgroundCompletions()
       mock_shutdown.assert_called_once()
@@ -448,149 +533,134 @@
         self.client._grr_client, 'Get', return_value=_MOCK_LINUX_CLIENT):
       self.client.StartBackgroundMonitors()
       result = self.client.GetLastSeenTime()
       self.assertEqual(result,
                        datetime.datetime(2023, 5, 24, 1, 24, 23, 783055,
                                          tzinfo=datetime.timezone.utc))
 
-  @mock.patch.object(flow.Flow, 'Get', autospec=True)
-  def test_GetLastTimelineCorrect(self, mock_get):
+  @mock.patch('datetime.datetime', wraps=datetime.datetime)
+  def test_GetLastTimelineCorrect(self, mock_dt):
     """Tests the GetLastTimeline method when there is a recent one."""
-    with (
-        mock.patch.object(
-            self.client._grr_client,
-            'ListFlows',
-            return_value=_MOCK_APIFLOW_LISTFLOWS,
-        ),
-        mock.patch.object(
-            flow.Flow, 'ListResults', autospec=True
-        ) as mock_list_results
-    ):
-      mock_get.side_effect = _MOCK_APIFLOW_LISTFLOWS[2:]
-      mock_result = mock.Mock()
-      mock_result.timestamp = 9999999999999999999
-      mock_list_results.return_value = [mock_result]
+    with (mock.patch.object(self.client._grr_client,
+                            'ListFlows',
+                            return_value=_MOCK_APIFLOW_LISTFLOWS),
+          mock.patch.object(flow.Flow, 'Get', new=_MockGetFromFlowList)):
+      # "Now" is half of the staleness threshold past the epoch. All the flows
+      # returned are at 1 second past the epoch, so they are not stale.
+      mock_dt.now.return_value = datetime.datetime.fromtimestamp(
+          grr_shell_client._STALE_TIMELINE_THRESHOLD.total_seconds() / 2,
+          tz=datetime.timezone.utc)
+
       result = self.client.GetLastTimeline()
+
       self.assertStartsWith(result, 'CORRECT')
 
-  @mock.patch.object(flow.Flow, 'Get')
-  def test_GetLastTimelineNotFound(self, mock_get):
+  @mock.patch('datetime.datetime', wraps=datetime.datetime)
+  def test_GetLastTimelineNotFound(self, mock_dt):
     """Tests the GetLastTimeline method when there is no recent one."""
-    with (
-        mock.patch.object(
-            self.client._grr_client,
-            'ListFlows',
-            return_value=_MOCK_APIFLOW_LISTFLOWS,
-        ),
-        mock.patch.object(
-            flow.Flow, 'ListResults', autospec=True
-        ) as mock_list_results
-    ):
-      mock_get.side_effect = _MOCK_APIFLOW_LISTFLOWS[1:]
-      mock_result = mock.Mock()
-      mock_result.timestamp = 100
-      mock_list_results.return_value = [mock_result]
+    with (mock.patch.object(self.client._grr_client,
+                            'ListFlows',
+                            return_value=_MOCK_APIFLOW_LISTFLOWS),
+          mock.patch.object(flow.Flow, 'Get', new=_MockGetFromFlowList)):
+      # "Now" is twice the staleness threshold past the epoch. All the flows
+      # returned are at 1 second past the epoch, so they are stale.
+      mock_dt.now.return_value = datetime.datetime.fromtimestamp(
+          grr_shell_client._STALE_TIMELINE_THRESHOLD.total_seconds() * 2,
+          tz=datetime.timezone.utc)
+
       result = self.client.GetLastTimeline()
+
       self.assertIsNone(result)
 
-  @mock.patch.object(flow.Flow, 'Get')
-  def test_GetLastTimelineOldAndNew(self, mock_get):
+  @mock.patch('datetime.datetime', wraps=datetime.datetime)
+  def test_GetLastTimelineOldAndNew(self, mock_dt):
     """Tests the GetLastTimeline method when there is one old and one new one."""
-    with (
-        mock.patch.object(
-            self.client._grr_client,
-            'ListFlows',
-            return_value=_MOCK_APIFLOW_LISTFLOWS,
-        ),
-        mock.patch.object(
-            flow.Flow, 'ListResults', autospec=True
-        ) as mock_list_results
-    ):
-      mock_get.side_effect = _MOCK_APIFLOW_LISTFLOWS[2:]
-      mock_result_one = mock.Mock()
-      mock_result_one.timestamp = 9999999999999999999
-      mock_result_two = mock.Mock()
-      mock_result_two.timestamp = 100
-      mock_list_results.side_effect = [[mock_result_one], [mock_result_two]]
-      result = self.client.GetLastTimeline()
-      self.assertEqual(result, 'CORRECT_LIN')
+    with (mock.patch.object(self.client._grr_client,
+                            'ListFlows',
+                            return_value=_MOCK_APIFLOW_LISTFLOWS),
+          mock.patch.object(flow.Flow, 'Get', new=_MockGetFromFlowList)):
+      # "Now" is half of the staleness threshold past the epoch. All the flows
+      # returned are at 1 second past the epoch, so they are not stale.
+      mock_dt.now.return_value = datetime.datetime.fromtimestamp(
+          grr_shell_client._STALE_TIMELINE_THRESHOLD.total_seconds() / 2,
+          tz=datetime.timezone.utc)
 
-  @mock.patch.object(flow.Flow, 'Get')
-  def test_GetLastTimelineWindowsRoot(self, mock_get):
-    """Tests the GetLastTimeline method when there is a Windows root."""
-    with (
-        mock.patch.object(
-            self.client._grr_client,
-            'ListFlows',
-            return_value=_MOCK_APIFLOW_LISTFLOWS,
-        ),
-        mock.patch.object(
-            flow.Flow, 'ListResults', autospec=True
-        ) as mock_list_results
-    ):
-      mock_get.side_effect = _MOCK_APIFLOW_LISTFLOWS[2:]
-      mock_result_one = mock.Mock()
-      mock_result_one.timestamp = 100
-      mock_result_two = mock.Mock()
-      mock_result_two.timestamp = 9999999999999999999
-      mock_list_results.side_effect = [
-          [mock_result_one],
-          [mock_result_two]
-      ]
       result = self.client.GetLastTimeline()
-      self.assertEqual(result, 'CORRECT_WIN')
+
+      self.assertEqual(result, 'CORRECT_LIN_2_SECOND')
 
   def test_CollectTimelineNew(self):
     """Tests the CollectTimeline method with no existing timeline specified."""
     with (mock.patch.object(self.client._grr_stubby.types, 'CreateFlowArgs'
                             ) as mock_create_flow_args,
           mock.patch.object(self.client._grr_client, 'CreateFlow'
-                            ) as mock_create_flow):
+                            ) as mock_create_flow,
+          mock.patch('io.BytesIO') as mock_bytesio):
       mock_result_1 = mock.Mock()
       mock_result_1.timestamp = 1
       mock_result_2 = mock.Mock()
       mock_result_2.timestamp = 2
       mock_create_flow.return_value.ListResults.return_value = [mock_result_1]
+      mock_create_flow.return_value.args.root = b'/'
+      mock_bytesio.getvalue.return_value = open(
+          _SAMPLE_TIMELINE_LINUX, 'rb').read()
+
       self.client.CollectTimeline()
 
       mock_create_flow_args.assert_called_once_with('TimelineFlow')
       mock_create_flow.assert_called_once_with(
           name='TimelineFlow', args=mock_create_flow_args.return_value)
       mock_create_flow.return_value.WaitUntilDone.assert_called_once()
       mock_create_flow.return_value.GetCollectedTimelineBody.assert_called_once()
       self.assertEqual(self.client.last_timeline_time, 1)
+      self.assertDictEqual(self.client._pathspec_mapper._path_ps_map,
+                           {'/': jobs_pb2.PathSpec.OS})
 
   def test_CollectTimelineExisting(self):
     """Tests the CollectTimeline method with a specified existing timeline."""
-    with mock.patch.object(self.client._grr_client, 'Flow') as mock_flow:
+    with (mock.patch.object(self.client._grr_client, 'Flow') as mock_flow,
+          mock.patch('io.BytesIO') as mock_bytesio):
       mock_flow.return_value.Get.return_value.ListResults.return_value = []
+      mock_flow.return_value.Get.return_value.args.root = b'/'
+      mock_bytesio.getvalue.return_value = open(
+          _SAMPLE_TIMELINE_LINUX, 'rb').read()
+
       self.client.CollectTimeline(existing_timeline='ABCDE12345')
 
       mock_flow.assert_called_once_with('ABCDE12345')
       mock_flow.return_value.Get.assert_called_once()
       mock_flow.return_value.Get.return_value.WaitUntilDone.assert_called_once()
       mock_flow.return_value.Get.return_value.GetCollectedTimelineBody.assert_called_once()
+      self.assertDictEqual(self.client._pathspec_mapper._path_ps_map,
+                           {'/': jobs_pb2.PathSpec.OS})
 
   def test_CollectTimelinePath(self):
     """Tests the CollectTimeline method with a specified path."""
     with (mock.patch.object(self.client._grr_stubby.types, 'CreateFlowArgs',
                             return_value=mock.Mock()) as mock_create_flow_args,
           mock.patch.object(self.client._grr_client, 'CreateFlow',
-                            return_value=mock.Mock()) as mock_create_flow):
+                            return_value=mock.Mock()) as mock_create_flow,
+          mock.patch('io.BytesIO') as mock_bytesio):
       mock_create_flow.return_value.ListResults.return_value = []
+      mock_create_flow.return_value.args.root = b'/'
+      mock_bytesio.getvalue.return_value = open(
+          _SAMPLE_TIMELINE_LINUX, 'rb').read()
+
       self.client.CollectTimeline(path='/home/testuser/')
 
       mock_create_flow_args.assert_called_once_with('TimelineFlow')
       self.assertEqual(
           mock_create_flow_args.return_value.root, b'/home/testuser/'
       )
       mock_create_flow.assert_called_once_with(
           name='TimelineFlow', args=mock_create_flow_args.return_value)
       mock_create_flow.return_value.WaitUntilDone.assert_called_once()
       mock_create_flow.return_value.GetCollectedTimelineBody.assert_called_once()
+      self.assertDictEqual(self.client._pathspec_mapper._path_ps_map,
+                           {'/': jobs_pb2.PathSpec.OS})
 
   @mock.patch.object(_MOCK_APIFLOW_CFF_DOWNLOAD_RUNNING, 'WaitUntilDone')
   @mock.patch.object(_MOCK_APIFLOW_CFF_DOWNLOAD_RUNNING, 'ListResults')
   def test_FileInfo(self, mock_list_results, mock_wait_until_done):
     """Tests the FileInfo method."""
     mock_list_results.return_value = [_MOCK_HASH_LINUX_ENTRY]
 
@@ -1042,36 +1112,42 @@
           _MOCK_APIFLOW_GETFILE_RUNNING,
           _MOCK_APIFLOW_INTERROGATE_RUNNING,
           _MOCK_APIFLOW_TIMELINE_RUNNING]
 
       self.client._flow_monitor.StartMonitor()
       result = self.client.ListAllFlows(10)
 
+      expected = """\tARTIFACTCOLLECTORFLOWTERMINATEDFLOWID 1970-01-01T00:00:09Z ArtifactCollectorFlow AllOS_File TERMINATED
+\tARTIFACTCOLLECTORFLOWRUNNINGFLOWID 1970-01-01T00:00:08Z ArtifactCollectorFlow AllOS_File RUNNING
+\tGETFILERUNNINGFLOWID 1970-01-01T00:00:07Z GetFile C:/Users/username/Downloads/Firefox Installer.exe:Zone.Identifier RUNNING
+\tCLIENTFILEFINDERTERMINATEDFLOWID 1970-01-01T00:00:06Z ClientFileFinder DOWNLOAD /remote/path TERMINATED
+\tCLIENTFILEFINDERRUNNINGFLOWID 1970-01-01T00:00:05Z ClientFileFinder DOWNLOAD /remote/path RUNNING
+\tINTERROGATEFLOWID 1970-01-01T00:00:04Z Interrogate  RUNNING
+\tTIMELINEFLOWID 1970-01-01T00:00:03Z TimelineFlow root: / RUNNING"""
+
+      self.assertEqual(result, expected)
+
+  def test_ListAllFlowsUncached(self):
+    """Tests the ListAllFlows method when the flows are not yet cached."""
+    with (mock.patch.object(self.client._grr_client, 'ListFlows'
+                            ) as mock_listflows,
+          mock.patch.object(self.client._flow_monitor, 'IsFlowCached'
+                            ) as mock_isflowcached,
+          mock.patch.object(self.client._flow_monitor._grr_client, 'Flow'
+                            ) as mock_monitor_flow):
+      mock_listflows.return_value = [_MOCK_APIFLOW_CFF_DOWNLOAD_RUNNING]
+      mock_monitor_flow.side_effect = [_MOCK_APIFLOW_CFF_DOWNLOAD_RUNNING]
+      mock_isflowcached.return_value = False
+
+      self.client._flow_monitor.StartMonitor()
+      result = self.client.ListAllFlows(10)
+
       self.assertIn(
           '\tCLIENTFILEFINDERRUNNINGFLOWID 1970-01-01T00:00:05Z '
-          'ClientFileFinder DOWNLOAD /remote/path RUNNING', result)
-      self.assertIn(
-          '\tCLIENTFILEFINDERTERMINATEDFLOWID 1970-01-01T00:00:06Z '
-          'ClientFileFinder DOWNLOAD /remote/path TERMINATED', result)
-      self.assertIn(
-          '\tARTIFACTCOLLECTORFLOWRUNNINGFLOWID 1970-01-01T00:00:08Z '
-          'ArtifactCollectorFlow AllOS_File RUNNING', result)
-      self.assertIn(
-          '\tARTIFACTCOLLECTORFLOWTERMINATEDFLOWID 1970-01-01T00:00:09Z '
-          'ArtifactCollectorFlow AllOS_File TERMINATED', result)
-      self.assertIn(
-          '\tGETFILERUNNINGFLOWID 1970-01-01T00:00:07Z GetFile '
-          'C:/Users/username/Downloads/Firefox Installer.exe:Zone.Identifier '
-          'RUNNING', result)
-      self.assertIn(
-          '\tINTERROGATEFLOWID 1970-01-01T00:00:04Z Interrogate  RUNNING',
-          result)
-      self.assertIn(
-          '\tTIMELINEFLOWID 1970-01-01T00:00:03Z TimelineFlow root: / RUNNING',
-          result)
+          'ClientFileFinder <UNCACHED FLOW ARGS> RUNNING', result)
 
   @parameterized.named_parameters(
       ('cff_success', _MOCK_APIFLOW_CFF_DOWNLOAD_TERMINATED,
        _MOCK_CLIENTFILEFINDER_TERMINATED_DETAIL),
       ('cff_failure', _MOCK_APIFLOW_CFF_DOWNLOAD_ERROR,
        _MOCK_CLIENTFILEFINDER_ERROR_DETAIL),
       ('timeline_failure', _MOCK_APIFLOW_TIMELINE_ERROR,
@@ -1120,14 +1196,30 @@
     self.client = grr_shell_client.GRRShellClient(
         _TEST_GRR_URL, _TEST_GRR_USER, _TEST_GRR_PASS, _TEST_CLIENT_FQDN, _MAX_FILE_SIZE_1GB)
 
   def test_GetOS(self):
     """Tests the GetOS method."""
     self.assertEqual(self.client.GetOS(), 'Windows')
 
+  @mock.patch('datetime.datetime', wraps=datetime.datetime)
+  def test_GetLastTimelineWindowsRoot(self, mock_dt):
+    """Tests the GetLastTimeline method when there is a Windows root."""
+    with (mock.patch.object(self.client._grr_client,
+                            'ListFlows',
+                            return_value=_MOCK_APIFLOW_LISTFLOWS),
+          mock.patch.object(flow.Flow, 'Get', new=_MockGetFromFlowList)):
+      # "Now" is half of the staleness threshold past the epoch. All the flows
+      # returned are at 1 second past the epoch, so they are not stale.
+      mock_dt.now.return_value = datetime.datetime.fromtimestamp(
+          grr_shell_client._STALE_TIMELINE_THRESHOLD.total_seconds() / 2,
+          tz=datetime.timezone.utc)
+
+      result = self.client.GetLastTimeline()
+      self.assertEqual(result, 'CORRECT_WIN')
+
   @mock.patch.object(_MOCK_APIFLOW_CFF_DOWNLOAD_RUNNING, 'WaitUntilDone')
   @mock.patch.object(_MOCK_APIFLOW_CFF_DOWNLOAD_RUNNING, 'ListResults')
   @mock.patch.object(_MOCK_APIFLOW_GETFILE_RUNNING, 'WaitUntilDone')
   @mock.patch.object(_MOCK_APIFLOW_GETFILE_RUNNING, 'ListResults')
   def test_FileInfo_NoADS(self,
                           mock_gf_list_results,
                           mock_gf_wait_until_done,
@@ -1156,27 +1248,94 @@
           'C:/Users/username/Downloads/Firefox Installer.exe')
       self.assertEqual(mock_create_flow_args.return_value.action.action_type,
                        flows_pb2.FileFinderAction.HASH)
       mock_create_flow.assert_has_calls([
           mock.call(
               name='ClientFileFinder', args=mock_create_flow_args.return_value),
           mock.call(
-              name='GetFile',
-              args=flows_pb2.GetFileArgs(
-                  pathspec=jobs_pb2.PathSpec(
+              name='MultiGetFile',
+              args=flows_pb2.MultiGetFileArgs(
+                  pathspecs=[jobs_pb2.PathSpec(
                       path='C:/Users/username/Downloads/Firefox Installer.exe',
                       pathtype=jobs_pb2.PathSpec.NTFS,
-                      stream_name='Zone.Identifier')))])
+                      stream_name='Zone.Identifier')]))])
       mock_ff_wait_until_done.assert_called_once()
       mock_gf_wait_until_done.assert_called_once()
 
       self.assertEqual(result, _EXPECTED_HASH_WINDOWS_RESULT)
 
   @mock.patch.object(_MOCK_APIFLOW_CFF_DOWNLOAD_RUNNING, 'WaitUntilDone')
   @mock.patch.object(_MOCK_APIFLOW_CFF_DOWNLOAD_RUNNING, 'ListResults')
+  def test_FileInfo_D_Drive(self,
+                            mock_ff_list_results,
+                            mock_ff_wait_until_done):
+    """Tests CFF for a file on a Windows non-root drive uses OS PathSpec."""
+    mock_ff_list_results.return_value = [_MOCK_HASH_WINDOWS_ENTRY]
+
+    with (mock.patch.object(self.client._grr_stubby.types, 'CreateFlowArgs',
+                            ) as mock_create_flow_args,
+          mock.patch.object(self.client._grr_client, 'CreateFlow',
+                            ) as mock_create_flow):
+      mock_create_flow.side_effect = [_MOCK_APIFLOW_CFF_DOWNLOAD_RUNNING]
+
+      self.client.FileInfo('/D:/foo')
+
+      mock_create_flow_args.assert_called_once_with('ClientFileFinder')
+      mock_create_flow_args.return_value.paths.append.assert_called_once_with(
+          'D:/foo')
+      self.assertEqual(mock_create_flow_args.return_value.action.action_type,
+                       flows_pb2.FileFinderAction.HASH)
+      self.assertEqual(mock_create_flow_args.return_value.pathtype,
+                       jobs_pb2.PathSpec.OS)
+      mock_create_flow.assert_called_with(
+          name='ClientFileFinder', args=mock_create_flow_args.return_value)
+      mock_ff_wait_until_done.assert_called_once()
+
+  @mock.patch.object(flow.Flow, 'Get')
+  @mock.patch.object(_MOCK_APIFLOW_CFF_DOWNLOAD_RUNNING, 'WaitUntilDone')
+  @mock.patch.object(_MOCK_APIFLOW_CFF_DOWNLOAD_RUNNING, 'ListResults')
+  @mock.patch.object(_MOCK_APIFLOW_CFF_DOWNLOAD_RUNNING, 'GetFilesArchive')
+  def test_CollectFiles_D_Drive(self,
+                                mock_get_files_archive,
+                                mock_list_results,
+                                mock_wait_until_done,
+                                mock_get):
+    """Tests the CollectFile method for windows, non-NTFS volume, with a non-ascii directory name."""
+    mock_get.side_effect = [_MOCK_APIFLOW_CFF_DOWNLOAD_TERMINATED]
+    mock_list_results.return_value = [_MOCK_HASH_WINDOWS_ENTRY]
+    mock_get_files_archive.return_value = [
+        _MOCK_ZIP_WINDOWS_CLIENTFILEFINDER_FAT32_DATA]
+
+    with (mock.patch.object(self.client._grr_stubby.types, 'CreateFlowArgs'
+                            ) as mock_create_flow_args,
+          mock.patch.object(self.client._grr_client, 'CreateFlow'
+                            ) as mock_create_flow):
+      mock_create_flow.return_value = _MOCK_APIFLOW_CFF_DOWNLOAD_RUNNING
+      self.client._pathspec_mapper['D:/'] = jobs_pb2.PathSpec.OS
+
+      local_path = os.path.join(self.create_tempdir(), 'local_path')
+      self.client.CollectFiles('/D:/\xa0/bar', local_path)
+
+      mock_create_flow_args.assert_called_once_with('ClientFileFinder')
+      self.assertEqual(mock_create_flow_args.return_value.pathtype,
+                       jobs_pb2.PathSpec.OS)
+      self.assertTrue(
+          mock_create_flow_args.return_value.use_raw_filesystem_access)
+
+      mock_create_flow_args.return_value.paths.append.assert_called_once_with(
+          'D:/\xa0/bar')
+      mock_create_flow.assert_called_once_with(
+          name='ClientFileFinder', args=mock_create_flow_args.return_value)
+      mock_wait_until_done.assert_called_once()
+
+      self.assertTrue(os.path.exists(
+          os.path.join(local_path, 'D_', '\xa0', 'bar')))
+
+  @mock.patch.object(_MOCK_APIFLOW_CFF_DOWNLOAD_RUNNING, 'WaitUntilDone')
+  @mock.patch.object(_MOCK_APIFLOW_CFF_DOWNLOAD_RUNNING, 'ListResults')
   def test_FileInfo_wildcard(self, mock_list_results, mock_wait_until_done):
     """Tests the FileInfo method with a wildcard path."""
     mock_list_results.return_value = [_MOCK_HASH_WINDOWS_ENTRY]
 
     with (mock.patch.object(self.client._grr_stubby.types, 'CreateFlowArgs'
                             ) as mock_create_flow_args,
           mock.patch.object(self.client._grr_client, 'CreateFlow'
@@ -1235,20 +1394,20 @@
           'C:/Users/username/Downloads/Firefox Installer.exe')
       self.assertEqual(mock_create_flow_args.return_value.action.action_type,
                        flows_pb2.FileFinderAction.HASH)
       mock_create_flow.assert_has_calls([
           mock.call(
               name='ClientFileFinder', args=mock_create_flow_args.return_value),
           mock.call(
-              name='GetFile',
-              args=flows_pb2.GetFileArgs(
-                  pathspec=jobs_pb2.PathSpec(
+              name='MultiGetFile',
+              args=flows_pb2.MultiGetFileArgs(
+                  pathspecs=[jobs_pb2.PathSpec(
                       path='C:/Users/username/Downloads/Firefox Installer.exe',
                       pathtype=jobs_pb2.PathSpec.NTFS,
-                      stream_name='Zone.Identifier')))])
+                      stream_name='Zone.Identifier')]))])
       mock_ff_wait_until_done.assert_called_once()
       mock_gf_wait_until_done.assert_called_once()
       mock_gf_get_files_archive.assert_called_once()
 
       self.assertEqual(result, _EXPECTED_HASH_WINDOWS_WITH_ADS_RESULT)
 
   @mock.patch.object(_MOCK_APIFLOW_CFF_DOWNLOAD_RUNNING, 'WaitUntilDone')
@@ -1287,20 +1446,20 @@
           'C:/Users/username/Downloads/Firefox Installer.exe')
       self.assertEqual(mock_create_flow_args.return_value.action.action_type,
                        flows_pb2.FileFinderAction.HASH)
       mock_create_flow.assert_has_calls([
           mock.call(
               name='ClientFileFinder', args=mock_create_flow_args.return_value),
           mock.call(
-              name='GetFile',
-              args=flows_pb2.GetFileArgs(
-                  pathspec=jobs_pb2.PathSpec(
+              name='MultiGetFile',
+              args=flows_pb2.MultiGetFileArgs(
+                  pathspecs=[jobs_pb2.PathSpec(
                       path='C:/Users/username/Downloads/Firefox Installer.exe',
                       pathtype=jobs_pb2.PathSpec.NTFS,
-                      stream_name='Zone.Identifier')))])
+                      stream_name='Zone.Identifier')]))])
       mock_ff_wait_until_done.assert_called_once()
       mock_gf_wait_until_done.assert_called_once()
       mock_gf_get_files_archive.assert_called_once()
 
       self.assertEqual(result, _EXPECTED_HASH_WINDOWS_RESULT)
 
   @mock.patch.object(_MOCK_APIFLOW_CFF_DOWNLOAD_RUNNING, 'WaitUntilDone')
@@ -1374,14 +1533,15 @@
         _MOCK_ZIP_WINDOWS_CLIENTFILEFINDER_DATA]
 
     with (mock.patch.object(self.client._grr_stubby.types, 'CreateFlowArgs'
                             ) as mock_create_flow_args,
           mock.patch.object(self.client._grr_client, 'CreateFlow'
                             ) as mock_create_flow):
       mock_create_flow.return_value = _MOCK_APIFLOW_CFF_DOWNLOAD_RUNNING
+      self.client._pathspec_mapper['C:/'] = jobs_pb2.PathSpec.NTFS
 
       local_path = os.path.join(self.create_tempdir(), 'local_path')
       self.client.CollectFiles(
           '/C:/Users/username/Downloads/Firefox Installer.exe', local_path)
 
       mock_create_flow_args.assert_called_once_with('ClientFileFinder')
       self.assertEqual(mock_create_flow_args.return_value.pathtype,
@@ -1804,33 +1964,66 @@
       ('c_preceding_slash', '/C:/', b'C:/')
   )
   def test_CollectTimelinePath(self, in_path, expected_path):
     """Tests the CollectTimeline method with a specified path."""
     with (mock.patch.object(self.client._grr_stubby.types, 'CreateFlowArgs',
                             return_value=mock.Mock()) as mock_create_flow_args,
           mock.patch.object(self.client._grr_client, 'CreateFlow',
-                            return_value=mock.Mock()) as mock_create_flow):
-      mock_create_flow.return_value.ListResults.return_value = []
+                            return_value=mock.Mock()) as mock_create_flow,
+          mock.patch('io.BytesIO') as mock_bytesio):
+      mock_result = mock.Mock()
+      mock_result.payload.filesystem_type = 'NTFS'
+      mock_create_flow.return_value.ListResults.return_value = [mock_result]
+      mock_create_flow.return_value.args.root = in_path.encode('utf-8')
+      mock_bytesio.return_value.getvalue.return_value = open(
+          _SAMPLE_TIMELINE_WINDOWS, 'rb').read()
+
       self.client.CollectTimeline(path=in_path)
 
       mock_create_flow_args.assert_called_once_with('TimelineFlow')
       self.assertEqual(
           mock_create_flow_args.return_value.root, expected_path)
       mock_create_flow.assert_called_once_with(
           name='TimelineFlow', args=mock_create_flow_args.return_value)
       mock_create_flow.return_value.WaitUntilDone.assert_called_once()
       mock_create_flow.return_value.GetCollectedTimelineBody.assert_called_once()
+      self.assertDictEqual({'C:/': jobs_pb2.PathSpec.NTFS},
+                           self.client._pathspec_mapper._path_ps_map)
 
   def test_DetermineSourceForArtefact(self):
     """Tests determining the source type for a mixed type Artefact."""
     result = self.client._DetermineSourceForArtefact('Mixed')
 
     self.assertEqual(
         result, artifact_pb2.ArtifactSource.SourceType.REGISTRY_VALUE)
 
+  @mock.patch.object(
+      _MOCK_APIFLOW_ARTEFACTCOLLECTOR_WMILOGICALDISKS_RUNNING, 'WaitUntilDone')
+  @mock.patch.object(
+      _MOCK_APIFLOW_ARTEFACTCOLLECTOR_WMILOGICALDISKS_RUNNING, 'ListResults')
+  def test_DescribeVolumes(self,
+                           mock_list_results,
+                           mock_wait_until_done):
+    """Tests the DescribeVolumes method."""
+    with (mock.patch.object(self.client._grr_stubby.types, 'CreateFlowArgs'
+                            ) as mock_create_flow_args,
+          mock.patch.object(self.client._grr_client, 'CreateFlow'
+                            ) as mock_create_flow):
+      mock_create_flow.return_value = (
+          _MOCK_APIFLOW_ARTEFACTCOLLECTOR_WMILOGICALDISKS_RUNNING)
+      mock_list_results.return_value = [
+          _MOCK_WINDOWS_ARTEFACT_VOLUME_C,
+          _MOCK_WINDOWS_ARTEFACT_VOLUME_D]
+
+      result = self.client.DescribeVolumes()
+
+      mock_create_flow_args.assert_called_once_with('ArtifactCollectorFlow')
+      mock_wait_until_done.assert_called_once()
+      self.assertEqual(result, _EXPECTED_WINDOWS_VOLUMES_RESULT)
+
 
 class GrrShellClientDarwinTest(parameterized.TestCase):
   """Dawin/MacOS specific tests for the GRR Shell Client class."""
 
   mock_grr_api: mock.Mock
   client: grr_shell_client.GRRShellClient
 
@@ -1846,14 +2039,15 @@
         _MOCK_APIFLOW_LISTFLOWS)
     self.mock_grr_api.SearchClients.return_value = [_MOCK_DARWIN_CLIENT]
     self.mock_grr_api.ListArtifacts.return_value = (
         _BuildMockArtifactDescriptors())
 
     self.client = grr_shell_client.GRRShellClient(
         _TEST_GRR_URL, _TEST_GRR_USER, _TEST_GRR_PASS, _TEST_CLIENT_FQDN, _MAX_FILE_SIZE_1GB)
+    self.client._pathspec_mapper['/'] = jobs_pb2.PathSpec.OS
 
   def test_GetOS(self):
     """Tests the GetOS method."""
     self.assertEqual(self.client.GetOS(), 'Darwin')
 
   @mock.patch.object(flow.Flow, 'Get')
   @mock.patch.object(_MOCK_APIFLOW_CFF_DOWNLOAD_RUNNING, 'WaitUntilDone')
@@ -1948,9 +2142,58 @@
     """Tests determining the source type for a mixed type Artefact."""
     result = self.client._DetermineSourceForArtefact('Mixed')
 
     self.assertEqual(
         result, artifact_pb2.ArtifactSource.SourceType.FILE)
 
 
+class PathSpecMapperTest(parameterized.TestCase):
+  """Tests the _PathSpecMapper class."""
+
+  pathspecmapper_win = grr_shell_client._PathSpecMapper()
+  pathspecmapper_lin = grr_shell_client._PathSpecMapper()
+
+  def setUp(self):  # pylint: disable=arguments-differ
+    """Set up tests."""
+    super().setUp()
+    self.pathspecmapper_win['C:/'] = jobs_pb2.PathSpec.NTFS
+    self.pathspecmapper_win['D:/'] = jobs_pb2.PathSpec.OS
+
+    self.pathspecmapper_lin['/'] = jobs_pb2.PathSpec.OS
+    self.pathspecmapper_lin['/mnt/external'] = jobs_pb2.PathSpec.OS
+    self.pathspecmapper_lin['/mnt/external_ntfs'] = jobs_pb2.PathSpec.NTFS
+
+  def test_PathSpecMapper_SetItem(self):
+    """Tests adding mappings to _PathSpecMapper.
+
+    Mappings are added in setup(), this just tests they are as expected.
+    """
+    self.assertDictEqual(self.pathspecmapper_win._path_ps_map,
+                         {'C:/': jobs_pb2.PathSpec.NTFS,
+                          'D:/': jobs_pb2.PathSpec.OS})
+
+    self.assertDictEqual(self.pathspecmapper_lin._path_ps_map,
+                         {'/': jobs_pb2.PathSpec.OS,
+                          '/mnt/external': jobs_pb2.PathSpec.OS,
+                          '/mnt/external_ntfs': jobs_pb2.PathSpec.NTFS})
+
+  @parameterized.named_parameters(
+      ('c_drive', 'C:/file', jobs_pb2.PathSpec.NTFS),
+      ('d_drive', 'D:/file', jobs_pb2.PathSpec.OS),
+      ('e_drive', 'E:/file', jobs_pb2.PathSpec.OS),
+  )
+  def test_PathSpecmapper_win_GetItem(self, path, expected_value):
+    """Tests getting a mapping from _PathSpecMapper - windows edition."""
+    self.assertEqual(self.pathspecmapper_win[path], expected_value)
+
+  @parameterized.named_parameters(
+      ('root', '/home/file', jobs_pb2.PathSpec.OS),
+      ('mapped_ext', '/mnt/external/file', jobs_pb2.PathSpec.OS),
+      ('mapped_ntfs', '/mnt/external_ntfs/file', jobs_pb2.PathSpec.NTFS),
+  )
+  def test_PathSpecmapper_lin_GetItem(self, path, expected_value):
+    """Tests getting a mapping from _PathSpecMapper - linux edition."""
+    self.assertEqual(self.pathspecmapper_lin[path], expected_value)
+
+
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `grrshell-20231227/grrshell/tests/grr_shell_emulated_fs_test.py` & `grrshell-20240405/grrshell/tests/grr_shell_emulated_fs_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Unit tests for the Grr Shell Emulated FS class."""
 
-# pylint: disable=wrong-import-order
+# pylint: disable=wrong-import-order,ungrouped-imports
 # pylint: disable=protected-access
 # pytype: disable=attribute-error
 
 from typing import Optional
 
 from grrshell.lib import errors
 from grrshell.lib import grr_shell_emulated_fs
@@ -189,14 +189,15 @@
     with self.assertRaisesRegex(errors.IsAFileError, '/root/.bashrc'):
       self.emulated_fs.GetChildrenOfPath('/root/.bashrc')
 
   @parameterized.named_parameters(
       ('slash_none_bash', '/', '', 'bash', ['/root/.bashrc']),
       ('root_none_bash', '/root', '', 'bash', ['/root/.bashrc']),
       ('slash_root_bash', '/', 'root', 'bash', ['/root/.bashrc']),
+      ('slash_root_bash_uppercase', '/', 'root', 'BASH', ['/root/.bashrc']),
       ('slash_none_regex', '/', '', '.*ca[cd].*', ['/root/.cache',
                                                    '/root/.cache/dconf',
                                                    '/root/.cache/dconf/user']),
   )
   def test_Find(self, starting_pwd, base_dir, needle, expected_results):
     """Tests the Find method."""
     self.emulated_fs.ParseTimelineFlow(self.timeline_data)
@@ -315,15 +316,15 @@
     self.assertEqual(result, expected_resuslt)
 
   @parameterized.named_parameters(
       ('no_path', None, ['.', 'C:']),
       ('c_drive', '/C:', ['.', '$Recycle.Bin', '$WinREAgent', 'Config.Msi',
                           'Documents and Settings', 'DumpStack.log.tmp',
                           'PerfLogs', 'Program Files', 'hiberfil.sys',
-                          'pagefile.sys']),
+                          'pagefile.sys', '\xa0']),
       ('file', '/C:/pagefile.sys', ['pagefile.sys']),
       ('glob_raw', '*', ['.', 'C:']),
       ('glob_c_star', 'C*', ['C:']),
       ('glob_subdir', 'C:/*e*', ['$Recycle.Bin', '$WinREAgent', 'hiberfil.sys',
                                  'Documents and Settings', 'pagefile.sys',
                                  'PerfLogs', 'Program Files'])
   )
@@ -334,19 +335,19 @@
     results = [r.name for r in self.emulated_fs.Ls(path)]
     self.assertCountEqual(results, expected_results)
 
   @parameterized.named_parameters(
       ('c_drive', '/C:', False, ['$Recycle.Bin/', '$WinREAgent/', 'Config.Msi/',
                                  'Documents and Settings/', 'DumpStack.log.tmp',
                                  'PerfLogs/', 'Program Files/', 'hiberfil.sys',
-                                 'pagefile.sys']),
+                                 'pagefile.sys', '\xa0/']),
       ('c_drive_dirs_only', '/C:', True, ['Config.Msi/', '$Recycle.Bin/',
                                           'Program Files/', '$WinREAgent/',
                                           'Documents and Settings/',
-                                          'PerfLogs/'])
+                                          'PerfLogs/', '\xa0/'])
   )
   def test_GetChildrenOfPath(self,
                              remote_path: str,
                              dirs_only: bool,
                              expected_results: list[str]):
     """Tests the GetChildrenOfPath method."""
     self.emulated_fs.ParseTimelineFlow(self.timeline_data)
```

### Comparing `grrshell-20231227/grrshell/tests/grr_shell_repl_test.py` & `grrshell-20240405/grrshell/tests/grr_shell_repl_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Unit tests for the Grr Shell REPL driver."""
 
-# pylint: disable=wrong-import-order
+# pylint: disable=wrong-import-order,ungrouped-imports
 import contextlib
 import datetime
 import io
 import sys
 from unittest import mock
 
 import prompt_toolkit
@@ -30,30 +30,38 @@
 from absl.testing import absltest
 from absl.testing import parameterized
 
 
 _SAMPLE_TIMELINE_LINUX = 'grrshell/tests/testdata/sample_timeline_linux'
 _SAMPLE_TIMELINE_WINDOWS = 'grrshell/tests/testdata/sample_timeline_windows'
 
-_COMMANDS = ('help', 'ls', 'pwd', 'cd', 'refresh', 'info', 'collect', 'find',
-             'flows', 'exit', 'set', 'artefact', 'clear', 'resume', 'detail')
-_ALIASES = ('h', '?', 'hash', 'quit')
+_COMMANDS = ['help', 'ls', 'pwd', 'cd', 'refresh', 'info', 'collect', 'find',
+             'flows', 'exit', 'set', 'artefact', 'clear', 'resume', 'detail',
+             'volumes']
+_ALIASES = ['h', '?', 'hash', 'quit']
 _ARTIFACT_NAMES = ['first', 'second', 'third', 'fourth']
 
 _CLIENT_ID = 'C.0000000000000001'
 
 
 # pylint: disable=protected-access
 # pylint: disable=consider-using-with
 
 
 class GRRShellREPLTest(parameterized.TestCase):
   """Unit tests for the Grr Shell REPL driver."""
 
-  shell: grr_shell_repl.GRRShellREPL
+  shell_repl: grr_shell_repl.GRRShellREPL
+
+  @classmethod
+  def _CreateGrrShellRepl(cls,
+                          client: grr_shell_client.GRRShellClient
+                          ) -> grr_shell_repl.GRRShellREPL:
+    """Create the GRRShellRepl object. Exists to be overridden by subclasses."""
+    return grr_shell_repl.GRRShellREPL(client)
 
   @mock.patch.object(grr_api, 'InitHttp', autospec=True)
   @mock.patch.object(grr_shell_client.GRRShellClient, '_ResolveClientID')
   @mock.patch.object(grr_shell_client.GRRShellClient, 'GetOS')
   @mock.patch.object(grr_shell_client.GRRShellClient, 'CollectTimeline')
   def setUp(self,  # pylint: disable=arguments-differ
             mock_collect_timeline,
@@ -66,23 +74,23 @@
     mock_collect_timeline.return_value = open(
         _SAMPLE_TIMELINE_LINUX, 'rb').read()
     mock_get_os.return_value = 'Linux'
     mock_resolve_client_id.return_value = _CLIENT_ID
 
     shell_client = grr_shell_client.GRRShellClient('url', 'user', 'pass', 'host.domain.com')
     shell_client.StartBackgroundMonitors()
-    self.shell = grr_shell_repl.GRRShellREPL(shell_client)
+    self.shell_repl = self._CreateGrrShellRepl(shell_client)
 
   def test_Init(self):
     """Tests initialisation."""
-    self.assertIsNotNone(self.shell)
+    self.assertIsNotNone(self.shell_repl)
 
   def test_GeneratePrompt(self):
     """Tests the _GeneratePrompt method."""
-    result = self.shell._GeneratePrompt()
+    result = self.shell_repl._GeneratePrompt()
     self.assertEqual(result, f'{_CLIENT_ID}:/ $ ')
 
   @parameterized.named_parameters(
       ('online', 300, 'class:online', '3 minutes', '4 minutes'),
       ('stale', 1000, 'class:stale', '15 minutes', '16 minutes'),
       ('offline', 30000, 'class:offline', '8 hours', '8 hours'),
   )
@@ -90,52 +98,52 @@
   def test_GenerateBottomBar(self,
                              now,
                              expected_format_class,
                              expected_relative_lastseen,
                              expected_relative_timeline,
                              mock_dt):
     """Tests generating the status bar content."""
-    def mock_isinstance_method(obj, classinfo):  # pylint: disable=invalid-name
+    def mock_isinstance_method(obj, classinfo):  # pylint: disable=invalid-name  # pylint: disable=invalid-name
       """Mocked version of isinstance needed due to the wrapping of datetime."""
       if hasattr(classinfo, '_mock_wraps'):
         return isinstance(obj, classinfo._mock_wraps)
       return isinstance(obj, classinfo)
 
     mock_dt.now.return_value = datetime.datetime.fromtimestamp(
         now, tz=datetime.timezone.utc)
 
-    with (mock.patch.object(self.shell._grr_shell_client, 'GetRunningFlowCount'
-                            ) as mock_get_flow_count,
-          mock.patch.object(self.shell._grr_shell_client, 'GetLastSeenTime'
-                            ) as mock_get_last_seen,
-          mock.patch.object(self.shell._emulated_fs, 'GetTimelineTime'
-                            ) as mock_get_timeline_time,
+    with (mock.patch.object(self.shell_repl._grr_shell_client,
+                            'GetRunningFlowCount') as mock_get_flow_count,
+          mock.patch.object(self.shell_repl._grr_shell_client,
+                            'GetLastSeenTime') as mock_get_last_seen,
+          mock.patch.object(self.shell_repl._emulated_fs,
+                            'GetTimelineTime') as mock_get_timeline_time,
           mock.patch('humanize.time.isinstance') as mock_isinstance):
       mock_get_flow_count.return_value = 4, 8
       mock_get_last_seen.return_value = datetime.datetime.fromtimestamp(
           75, tz=datetime.timezone.utc)
       mock_get_timeline_time.return_value = 1000000  # microseconds past epoch
       mock_isinstance.side_effect = mock_isinstance_method
 
-      result = self.shell._GenerateBottomBar()
+      result = self.shell_repl._GenerateBottomBar()
       self.assertEqual(
           result,
           [(expected_format_class, ' Last seen: 1970-01-01 00:01:15 '
                                    f'({expected_relative_lastseen} ago) '),
            ('class:bottom-toolbar', ' 4/8 flows running '),
            (expected_format_class, ' Timeline freshness: 1970-01-01 00:00:01'
                                    f' ({expected_relative_timeline} ago) ')])
 
   @mock.patch.object(prompt_toolkit.PromptSession, 'prompt', autospec=True)
   def test_RunShell_help(self, mock_prompt):
     """Tests printing help text, and its content."""
     mock_prompt.side_effect = ['help', EOFError]
 
     with io.StringIO() as buf, contextlib.redirect_stdout(buf):
-      self.shell.RunShell()
+      self.shell_repl.RunShell()
 
       for c in _COMMANDS:
         self.assertIn(f'\t{c} ', buf.getvalue())
       for c in _ALIASES:
         self.assertNotIn(f'\t{c} ', buf.getvalue())
 
   @parameterized.named_parameters(
@@ -152,16 +160,16 @@
                        expected_path,
                        expected_sort_key,
                        expected_reversed,
                        mock_prompt):
     """Tests entering ls at the prompt correctly calls ls for the emulated_fs."""
     mock_prompt.side_effect = [in_text, EOFError]
 
-    with mock.patch.object(self.shell._emulated_fs, 'Ls') as mock_ls:
-      self.shell.RunShell()
+    with mock.patch.object(self.shell_repl._emulated_fs, 'Ls') as mock_ls:
+      self.shell_repl.RunShell()
       mock_ls.assert_called_once_with(expected_path,
                                       expected_sort_key,
                                       expected_reversed)
 
   @parameterized.named_parameters(
       ('nonexistent', 'ls /nonexist', 'No such file or directory: /nonexist'),
       ('bad_glob', 'ls /tm*/file',
@@ -172,92 +180,92 @@
   )
   @mock.patch.object(prompt_toolkit.PromptSession, 'prompt', autospec=True)
   def test_RunShell_ls_error(self, in_text, expected_error, mock_prompt):
     """Tests ls failure modes."""
     mock_prompt.side_effect = [in_text, EOFError]
 
     with io.StringIO() as buf, contextlib.redirect_stdout(buf):
-      self.shell.RunShell()
+      self.shell_repl.RunShell()
       self.assertIn(expected_error, buf.getvalue())
 
   def test_LS_Colours(self):
     """Tests the colouring of LS results."""
-    with mock.patch.object(self.shell._emulated_fs, 'Ls') as mock_ls:
+    with mock.patch.object(self.shell_repl._emulated_fs, 'Ls') as mock_ls:
       mock_ls.return_value = [
           grr_shell_emulated_fs._LSEntry('d------', 1, 2, 3, '4', 'directory'),
           grr_shell_emulated_fs._LSEntry('l------', 5, 6, 7, '8', 'symlink'),
           grr_shell_emulated_fs._LSEntry('-------', 9, 10, 11, '12', 'file')
       ]
 
       with io.StringIO() as buf, contextlib.redirect_stdout(buf):
-        self.shell._Ls(['/path'])
+        self.shell_repl._Ls(['/path'])
 
         output = buf.getvalue()
 
         self.assertIn(' \x1b[94mdirectory\x1b[0m', output)
         self.assertIn(' \x1b[93msymlink\x1b[0m', output)
         self.assertIn(' file', output)
 
   @mock.patch.object(prompt_toolkit.PromptSession, 'prompt', autospec=True)
   def test_RunShell_cd(self, mock_prompt):
     """Tests entering cd at the prompt correctly calls cd for the emulated_fs."""
     mock_prompt.side_effect = ['cd path', EOFError]
 
-    with mock.patch.object(self.shell._emulated_fs, 'Cd') as mock_cd:
-      self.shell.RunShell()
+    with mock.patch.object(self.shell_repl._emulated_fs, 'Cd') as mock_cd:
+      self.shell_repl.RunShell()
       mock_cd.assert_called_once_with('path')
 
   @parameterized.named_parameters(
       ('nonexistent', 'cd /nonexistent',
        'No such file or directory: /nonexistent'),
       ('file', 'cd /root/.bashrc', 'Not a directory: /root/.bashrc'),
   )
   @mock.patch.object(prompt_toolkit.PromptSession, 'prompt', autospec=True)
   def test_RunShell_cd_error(self, in_text, expected, mock_prompt):
     """Tests invalid cd arguments."""
     mock_prompt.side_effect = [in_text, EOFError]
 
     with io.StringIO() as buf, contextlib.redirect_stdout(buf):
-      self.shell.RunShell()
+      self.shell_repl.RunShell()
       self.assertIn(expected, buf.getvalue())
 
   @mock.patch.object(prompt_toolkit.PromptSession, 'prompt', autospec=True)
   def test_RunShell_pwd(self, mock_prompt):
     """Tests entering pwd at the prompt correctly calls GetPWD for the emulated_fs."""
     mock_prompt.side_effect = ['pwd', EOFError]
 
-    with mock.patch.object(self.shell._emulated_fs, 'GetPWD') as mock_pwd:
-      self.shell.RunShell()
+    with mock.patch.object(self.shell_repl._emulated_fs, 'GetPWD') as mock_pwd:
+      self.shell_repl.RunShell()
 
       # 3 because PWD gets called in prompt generation, which happens twice, and
       # once more because we've ran the shell command.
       self.assertEqual(mock_pwd.call_count, 3)
 
   @mock.patch.object(prompt_toolkit.PromptSession, 'prompt', autospec=True)
   def test_RunShell_refresh(self, mock_prompt):
     """Tests entering refresh at the prompt correctly collects and parses a timeline."""
     mock_prompt.side_effect = ['refresh', EOFError]
 
-    with (mock.patch.object(self.shell._grr_shell_client,
+    with (mock.patch.object(self.shell_repl._grr_shell_client,
                             'CollectTimeline') as mock_collect_timeline,
-          mock.patch.object(self.shell._emulated_fs,
+          mock.patch.object(self.shell_repl._emulated_fs,
                             'ParseTimelineFlow') as mock_parse_timeline):
-      self.shell.RunShell()
+      self.shell_repl.RunShell()
       mock_collect_timeline.assert_called_once()
       mock_parse_timeline.assert_called_once_with(
           mock_collect_timeline.return_value, 0)
 
   def test_Refresh_cwd(self):
     """Tests running refresh manually on the current working dir."""
-    with (mock.patch.object(self.shell._grr_shell_client,
+    with (mock.patch.object(self.shell_repl._grr_shell_client,
                             'CollectTimeline') as mock_collect_timeline,
-          mock.patch.object(self.shell._emulated_fs,
+          mock.patch.object(self.shell_repl._emulated_fs,
                             'ParseTimelineFlow') as mock_parse_timeline):
-      self.shell._Cd(['/root'])
-      self.shell._Refresh(['.'])
+      self.shell_repl._Cd(['/root'])
+      self.shell_repl._Refresh(['.'])
       mock_collect_timeline.assert_called_once()
       mock_parse_timeline.assert_called_once_with(
           mock_collect_timeline.return_value, 0)
 
   @parameterized.named_parameters(
       ('basic', 'collect path', '/path'),
       ('directory', 'collect root', '/root/*'),
@@ -265,245 +273,256 @@
       ('file', 'collect root/.bashrc', '/root/.bashrc'),
   )
   @mock.patch.object(prompt_toolkit.PromptSession, 'prompt', autospec=True)
   def test_RunShell_collect(self, in_text, expected_param, mock_prompt):
     """Tests entering collect at the prompt correctly calls CollectFilesInBackground."""
     mock_prompt.side_effect = [in_text, EOFError]
 
-    with (mock.patch.object(self.shell._grr_shell_client,
+    with (mock.patch.object(self.shell_repl._grr_shell_client,
                             'CollectFilesInBackground') as mock_collect):
-      self.shell.RunShell()
+      self.shell_repl.RunShell()
       mock_collect.assert_called_once_with(expected_param, './')
 
   @mock.patch.object(prompt_toolkit.PromptSession, 'prompt', autospec=True)
   def test_RunShell_info(self, mock_prompt):
     """Tests entering stat at the prompt correctly calls StatFile."""
     mock_prompt.side_effect = ['info /path', EOFError]
 
-    with (mock.patch.object(self.shell._grr_shell_client,
+    with (mock.patch.object(self.shell_repl._grr_shell_client,
                             'FileInfo') as mock_fileinfo):
-      self.shell.RunShell()
+      self.shell_repl.RunShell()
       mock_fileinfo.assert_called_once_with('/path', False)
 
   @mock.patch.object(prompt_toolkit.PromptSession, 'prompt', autospec=True)
   def test_RunShell_info_offline(self, mock_prompt):
     """Tests entering stat at the prompt correctly calls StatFile."""
     mock_prompt.side_effect = ['info /path --offline', EOFError]
 
-    with (mock.patch.object(self.shell._emulated_fs,
+    with (mock.patch.object(self.shell_repl._emulated_fs,
                             'OfflineFileInfo') as mock_fileinfo):
-      self.shell.RunShell()
+      self.shell_repl.RunShell()
       mock_fileinfo.assert_called_once_with('/path')
 
   @mock.patch.object(prompt_toolkit.PromptSession, 'prompt', autospec=True)
   def test_RunShell_flows(self, mock_prompt):
     """Tests entering flows at the prompt correctly calls GetBackgroundFlowsState."""
     mock_prompt.side_effect = ['flows', EOFError]
 
-    with (mock.patch.object(self.shell._grr_shell_client,
+    with (mock.patch.object(self.shell_repl._grr_shell_client,
                             'GetBackgroundFlowsState') as mock_flows):
-      self.shell.RunShell()
+      self.shell_repl.RunShell()
       mock_flows.assert_called_once()
 
   @parameterized.named_parameters(
       ('default', 'flows --all', 50),
       ('with_count', 'flows --all 30', 30),
       ('invalid_count', 'flows --all asdf', 50)
   )
   @mock.patch.object(prompt_toolkit.PromptSession, 'prompt', autospec=True)
   def test_RunShell_flows_all(self, in_text, expected_count, mock_prompt):
     """Tests entering flows --all at the prompt correctly calls ListAllFlows."""
     mock_prompt.side_effect = [in_text, EOFError]
 
-    with (mock.patch.object(self.shell._grr_shell_client,
+    with (mock.patch.object(self.shell_repl._grr_shell_client,
                             'ListAllFlows') as mock_list_all):
-      self.shell.RunShell()
+      self.shell_repl.RunShell()
       mock_list_all.assert_called_once_with(count=expected_count)
 
   @parameterized.named_parameters(
       ('one_param', 'find a', './', 'a'),
       ('two_param', 'find a b', 'a', 'b'),
   )
   @mock.patch.object(prompt_toolkit.PromptSession, 'prompt', autospec=True)
   def test_RunShell_find(
       self, in_text, expected_param1, expected_param2, mock_prompt):
     """Tests entering find at the prompt correctly calls find for the emaulated fs."""
     mock_prompt.side_effect = [in_text, EOFError]
 
-    with mock.patch.object(self.shell._emulated_fs, 'Find') as mock_find:
-      self.shell.RunShell()
+    with mock.patch.object(self.shell_repl._emulated_fs, 'Find') as mock_find:
+      self.shell_repl.RunShell()
       mock_find.assert_called_once_with(expected_param1, expected_param2)
 
   @parameterized.named_parameters(
       ('bare', 'set', 'Valid properties: max-file-size'),
       ('invalid_name', 'set invalid', 'Valid properties: max-file-size'),
       ('no_value', 'set max-file-size', 'set requires two parameters'),
   )
   @mock.patch.object(prompt_toolkit.PromptSession, 'prompt', autospec=True)
   def test_RunShell_set_invalid(self, in_text, expected_out, mock_prompt):
     """Tests entinering set with invalid params at the prompt."""
     mock_prompt.side_effect = [in_text, EOFError]
 
     with io.StringIO() as buf, contextlib.redirect_stdout(buf):
-      self.shell.RunShell()
+      self.shell_repl.RunShell()
       self.assertIn(expected_out, buf.getvalue())
 
   @parameterized.named_parameters(
       ('zero', 'set max-file-size 0', 0),
       ('10', 'set max-file-size 10', 10),
   )
   @mock.patch.object(prompt_toolkit.PromptSession, 'prompt', autospec=True)
   def test_RunShell_set_maxfilesize(self, in_text, expected_param, mock_prompt):
     """Tests setting the max file size."""
     mock_prompt.side_effect = [in_text, EOFError]
 
-    with (mock.patch.object(self.shell._grr_shell_client,
+    with (mock.patch.object(self.shell_repl._grr_shell_client,
                             'SetMaxFilesize') as mock_set_file_size):
-      self.shell.RunShell()
+      self.shell_repl.RunShell()
       mock_set_file_size.assert_called_once_with(expected_param)
 
   @mock.patch.object(prompt_toolkit.PromptSession, 'prompt', autospec=True)
   @mock.patch.object(sys, 'exit')
   def test_RunShell_exit(self, mock_exit, mock_prompt):
     """Tests entering exit at the prompt correctly exits."""
     mock_prompt.side_effect = ['exit', EOFError]
 
-    self.shell.RunShell()
+    self.shell_repl.RunShell()
     mock_exit.assert_called_once()
 
   @mock.patch.object(prompt_toolkit.PromptSession, 'prompt', autospec=True)
   @mock.patch.object(prompt_toolkit.shortcuts, 'clear')
   def test_RunShell_clear(self, mock_clear, mock_prompt):
     """Tests entering clear at the prompt correctly calls the clear method."""
     mock_prompt.side_effect = ['clear', EOFError]
 
-    self.shell.RunShell()
+    self.shell_repl.RunShell()
     mock_clear.assert_called_once()
 
   @mock.patch.object(prompt_toolkit.PromptSession, 'prompt', autospec=True)
   @mock.patch.object(prompt_toolkit.shortcuts, 'clear', autospec=True)
   @mock.patch.object(sys, 'exit', autospec=True)
   def test_RunShell_multiple(self, mock_exit, mock_clear, mock_prompt):
     """Tests entering multiple commands works correctly."""
     mock_prompt.side_effect = ['clear', 'exit', EOFError]
-    self.shell.RunShell()
+    self.shell_repl.RunShell()
     mock_clear.assert_called_once()
     mock_exit.assert_called_once()
 
   @mock.patch.object(prompt_toolkit.PromptSession, 'prompt', autospec=True)
   def test_RunShell_invalid_command(self, mock_prompt):
     """Tests an invalid command only complains (ie, no exceptions thrown.)"""
     mock_prompt.side_effect = ['invalid', EOFError]
 
     with io.StringIO() as buf, contextlib.redirect_stdout(buf):
-      self.shell.RunShell()
+      self.shell_repl.RunShell()
       self.assertIn('Unrecognised command', buf.getvalue())
 
   @mock.patch.object(prompt_toolkit.PromptSession, 'prompt', autospec=True)
   def test_RunShell_empty(self, mock_prompt):
     """Tests an empty command (ie, no exceptions thrown.)"""
     mock_prompt.side_effect = ['', EOFError]
 
     with io.StringIO() as buf, contextlib.redirect_stdout(buf):
-      self.shell.RunShell()
+      self.shell_repl.RunShell()
       self.assertEqual('Exiting\n', buf.getvalue())
 
   @parameterized.named_parameters(
       ('american_spelling', 'artifact name'),
       ('correct_spelling', 'artefact name'),
   )
   @mock.patch.object(prompt_toolkit.PromptSession, 'prompt', autospec=True)
   def test_RunShell_artifact(self, in_text, mock_prompt):
     """Tests 'artifact' at the prompt calls CollectArtifactsInBackground."""
-    with mock.patch.object(self.shell._grr_shell_client,
+    with mock.patch.object(self.shell_repl._grr_shell_client,
                            'CollectArtefact') as mock_collect:
       mock_prompt.side_effect = [in_text, EOFError]
-      self.shell.RunShell()
+      self.shell_repl.RunShell()
       mock_collect.assert_called_once_with('name', './')
 
   @mock.patch.object(prompt_toolkit.PromptSession, 'prompt', autospec=True)
   @mock.patch.object(sys, 'exit')
   def test_RunShell_CTRLC(self, mock_exit, mock_prompt):
     """Tests that if the user hits CTRL+C, they are returned to the prompt."""
     mock_prompt.side_effect = ['info path', KeyboardInterrupt, 'exit', EOFError]
 
     with mock.patch.object(
-        self.shell._grr_shell_client, 'FileInfo') as mock_stat:
+        self.shell_repl._grr_shell_client, 'FileInfo') as mock_stat:
       mock_stat.side_effect = [KeyboardInterrupt]
 
-      self.shell.RunShell()
+      self.shell_repl.RunShell()
       mock_exit.assert_called_once()
 
   @mock.patch.object(prompt_toolkit.PromptSession, 'prompt', autospec=True)
   @mock.patch.object(sys, 'exit')
   def test_RunShell_UnknownException(self, mock_exit, mock_prompt):
     """Tests that if the user hits CTRL+C, they are returned to the prompt."""
     mock_prompt.side_effect = ['info path', 'exit', EOFError]
 
     with mock.patch.object(
-        self.shell._grr_shell_client, 'FileInfo') as mock_info:
+        self.shell_repl._grr_shell_client, 'FileInfo') as mock_info:
       mock_info.side_effect = [RuntimeError('Test RuntimeError')]
 
       with io.StringIO() as buf, contextlib.redirect_stdout(buf):
-        self.shell.RunShell()
+        self.shell_repl.RunShell()
         self.assertIn(
             "Unknown exception: <class 'RuntimeError'> - Test RuntimeError",
             buf.getvalue())
         mock_exit.assert_called_once()
 
   @mock.patch.object(prompt_toolkit.PromptSession, 'prompt', autospec=True)
   def test_RunShell_resume(self, mock_prompt):
     """Tests resuming a flow works as expected."""
     mock_prompt.side_effect = ['resume flowid', EOFError]
 
     with mock.patch.object(
-        self.shell._grr_shell_client, 'ReattachFlow') as mock_resume:
+        self.shell_repl._grr_shell_client, 'ReattachFlow') as mock_resume:
 
-      self.shell.RunShell()
+      self.shell_repl.RunShell()
       mock_resume.assert_called_once_with('flowid', './')
 
   @mock.patch.object(prompt_toolkit.PromptSession, 'prompt', autospec=True)
   def test_RunShell_resume_error(self, mock_prompt):
     """Tests resuming an invalid flow is correctly handled."""
     mock_prompt.side_effect = ['resume flowid', EOFError]
 
     with mock.patch.object(
-        self.shell._grr_shell_client, 'ReattachFlow') as mock_resume:
+        self.shell_repl._grr_shell_client, 'ReattachFlow') as mock_resume:
       mock_resume.side_effect = errors.NotResumeableFlowTypeError('test error')
 
       with io.StringIO() as buf, contextlib.redirect_stdout(buf):
-        self.shell.RunShell()
+        self.shell_repl.RunShell()
 
         mock_resume.assert_called_once_with('flowid', './')
         self.assertIn('test error', buf.getvalue())
 
   @mock.patch.object(prompt_toolkit.PromptSession, 'prompt', autospec=True)
   def test_RunShell_detail(self, mock_prompt):
     """Tests entering detail at the prompt calls the correct method."""
     mock_prompt.side_effect = ['detail flowid', EOFError]
 
     with mock.patch.object(
-        self.shell._grr_shell_client, 'FlowDetail') as mock_detail:
+        self.shell_repl._grr_shell_client, 'FlowDetail') as mock_detail:
 
-      self.shell.RunShell()
+      self.shell_repl.RunShell()
       mock_detail.assert_called_once_with('flowid')
 
+  @mock.patch.object(prompt_toolkit.PromptSession, 'prompt', autospec=True)
+  def test_RunShell_volumes(self, mock_prompt):
+    """Tests entering volumes at the prompt calls the correct method."""
+    mock_prompt.side_effect = ['volumes', EOFError]
+
+    with mock.patch.object(
+        self.shell_repl._grr_shell_client, 'DescribeVolumes') as mock_volumes:
+
+      self.shell_repl.RunShell()
+      mock_volumes.assert_called_once()
+
   @parameterized.named_parameters(
       ('short_only', 'help ls', grr_shell_repl._LS_HELP.short),
       ('long_check_short', 'help find', grr_shell_repl._FIND_HELP.short),
       ('long_check_long', 'help find', grr_shell_repl._FIND_HELP_LONG),
       ('invalid', 'help foobar', 'Unknown command'),
   )
   @mock.patch.object(prompt_toolkit.PromptSession, 'prompt', autospec=True)
   def test_RunShell_extended_help(self, in_text, expected, mock_prompt):
     """Tests fetching extended help text for a command."""
     mock_prompt.side_effect = [in_text, EOFError]
 
     with io.StringIO() as buf, contextlib.redirect_stdout(buf):
-      self.shell.RunShell()
+      self.shell_repl.RunShell()
 
       self.assertIn(expected, buf.getvalue())
 
   @parameterized.named_parameters(
       ('help', 'help one two', grr_shell_repl._HELP_HELP.short),
       ('ls', 'ls one two', grr_shell_repl._LS_HELP.short),
       ('cd', 'cd one two', grr_shell_repl._CD_HELP.short),
@@ -519,15 +538,15 @@
   )
   @mock.patch.object(prompt_toolkit.PromptSession, 'prompt', autospec=True)
   def test_RunShell_malformed_command(self, in_text, expected, mock_prompt):
     """Tests output when command syntax is incorrect."""
     mock_prompt.side_effect = [in_text, EOFError]
 
     with io.StringIO() as buf, contextlib.redirect_stdout(buf):
-      self.shell.RunShell()
+      self.shell_repl.RunShell()
 
       self.assertIn(expected, buf.getvalue())
 
 
 class GRRShellREPLTestWindows(parameterized.TestCase):
   """Windows specific unit tests for the Grr Shell REPL driver."""
 
@@ -635,15 +654,15 @@
       ('cd_root', 'cd root/', ['..', '.pki/', '.cache/', '.local/', '.ssh/',
                                '.augeas/', r'directory\ with\ spaces/']),
       ('cd_space_only', 'cd ', ['..', 'root/', 'odd/']),
       ('cd_spaces', 'cd root/dir', [r'directory\ with\ spaces/'], -3),
       ('collect_space_only', 'collect ', ['..', 'root/', 'odd/', 'root_file']),
       ('empty', '', ['help', 'ls', 'pwd', 'cd', 'info', 'refresh', 'collect',
                      'exit', 'flows', 'find', 'set', 'artefact', 'clear',
-                     'resume', 'detail']),
+                     'resume', 'detail', 'volumes']),
       ('find_space_only', 'find ', []),
       ('hash_space_only', 'hash ', ['..', 'root/', 'odd/', 'root_file']),
       ('help_c', 'help c', ['cd', 'clear', 'collect'], -1),
       ('info_space_only', 'info ', ['..', 'root/', 'odd/', 'root_file']),
       ('ls_bare', 'ls', ['ls'], -2),
       ('ls_r', 'ls r', ['root/', 'root_file'], -1),
       ('ls_root', 'ls root/', ['..', '.pki/', '.cache/', '.local/', '.ssh/',
@@ -702,25 +721,25 @@
   def test_Init(self):
     """Tests initialisation."""
     self.assertIsNotNone(self.completer)
 
   @parameterized.named_parameters(
       ('empty', '', ['help', 'ls', 'pwd', 'cd', 'info', 'refresh', 'collect',
                      'exit', 'flows', 'find', 'set', 'artefact', 'clear',
-                     'resume', 'detail']),
+                     'resume', 'detail', 'volumes']),
       ('single_char', 'c', ['cd', 'collect', 'clear']),
       ('cd_only', 'cd', ['cd']),
       ('cd_error', 'cd /nonexist', []),
       ('cd_root', 'cd C:/', ['$Recycle.Bin/', '$WinREAgent/', 'Config.Msi/',
                              r'Documents\ and\ Settings/', 'PerfLogs/',
-                             r'Program\ Files/', '..']),
+                             r'Program\ Files/', '..', '\xa0/']),
       ('ls_root', 'ls C:/', ['$Recycle.Bin/', '$WinREAgent/', 'Config.Msi/',
                              r'Documents\ and\ Settings/', 'DumpStack.log.tmp',
                              'hiberfil.sys', 'pagefile.sys', 'PerfLogs/',
-                             r'Program\ Files/', '..'])
+                             r'Program\ Files/', '..', '\xa0/'])
   )
   def test_GetCompletion(self, in_text, expected_suggestions):
     """Tests the get_completion method."""
     document = prompt_toolkit.document.Document(in_text, len(in_text))
 
     results = (c.text for c in self.completer.get_completions(document, None))
     self.assertCountEqual(expected_suggestions, results)
```

### Comparing `grrshell-20231227/grrshell/tests/testdata/artifact_collect_darwin.zip` & `grrshell-20240405/grrshell/tests/testdata/artifact_collect_darwin.zip`

 * *Files identical despite different names*

### Comparing `grrshell-20231227/grrshell/tests/testdata/artifact_collect_linux.zip` & `grrshell-20240405/grrshell/tests/testdata/artifact_collect_linux.zip`

 * *Files identical despite different names*

### Comparing `grrshell-20231227/grrshell/tests/testdata/artifact_collect_windows.zip` & `grrshell-20240405/grrshell/tests/testdata/artifact_collect_windows.zip`

 * *Files identical despite different names*

### Comparing `grrshell-20231227/grrshell/tests/testdata/file_collect_darwin.zip` & `grrshell-20240405/grrshell/tests/testdata/file_collect_darwin.zip`

 * *Files identical despite different names*

### Comparing `grrshell-20231227/grrshell/tests/testdata/file_collect_linux.zip` & `grrshell-20240405/grrshell/tests/testdata/file_collect_linux.zip`

 * *Files identical despite different names*

### Comparing `grrshell-20231227/grrshell/tests/testdata/file_collect_windows.zip` & `grrshell-20240405/grrshell/tests/testdata/file_collect_windows.zip`

 * *Files identical despite different names*

### Comparing `grrshell-20231227/grrshell/tests/testdata/getfile_ads.zip` & `grrshell-20240405/grrshell/tests/testdata/getfile_ads.zip`

 * *Files identical despite different names*

### Comparing `grrshell-20231227/grrshell/tests/testdata/getfile_ads_empty.zip` & `grrshell-20240405/grrshell/tests/testdata/getfile_ads_empty.zip`

 * *Files identical despite different names*

### Comparing `grrshell-20231227/grrshell/tests/testdata/mock_apiflow_clientfilefinder_download_error.textproto` & `grrshell-20240405/grrshell/tests/testdata/mock_apiflow_clientfilefinder_download_error.textproto`

 * *Files identical despite different names*

### Comparing `grrshell-20231227/grrshell/tests/testdata/mock_apiflow_clientfilefinder_download_terminated.textproto` & `grrshell-20240405/grrshell/tests/testdata/mock_apiflow_clientfilefinder_download_terminated.textproto`

 * *Files identical despite different names*

### Comparing `grrshell-20231227/grrshell/tests/testdata/mock_apiflow_clientfilefinder_multiple.textproto` & `grrshell-20240405/grrshell/tests/testdata/mock_apiflow_clientfilefinder_multiple.textproto`

 * *Files identical despite different names*

### Comparing `grrshell-20231227/grrshell/tests/testdata/mock_apiflow_collectfilesbyknownpath_multiple.textproto` & `grrshell-20240405/grrshell/tests/testdata/mock_apiflow_collectfilesbyknownpath_multiple.textproto`

 * *Files identical despite different names*

### Comparing `grrshell-20231227/grrshell/tests/testdata/mock_apiflow_listflows.textproto` & `grrshell-20240405/grrshell/tests/testdata/mock_apiflow_listflows.textproto`

 * *Files 27% similar despite different names*

```diff
@@ -1,76 +1,94 @@
 # proto-file: grr_response_proto/api/flow.proto
 # proto-message: ApiListFlowsResult
 items: [
   {
     urn: "aff4:/C.0000000000000001/A1B2C3D4E5F6A1B2"
     name: "ClientFileFinder"
-    state: 0
+    state: RUNNING
     args {
       [type.googleapis.com/grr.FileFinderArgs] {
         action: {
           action_type: DOWNLOAD
         }
         paths: [
           "/remote/path"
         ]
       }
     }
     flow_id: "A1B2C3D4E5F6A1B2"
     client_id: "C.0000000000000001"
+    last_active_at: 1000000  # 1 second past epoch in microseconds
   },
   {
     urn: "aff4:/C.0000000000000001"
     flow_id: "ERRORED_BUT_CORRECT",
     name: "TimelineFlow",
-    state: 3,
+    state: ERROR,
     args: {
       [type.googleapis.com/grr.TimelineArgs] {
         root: "/"
       }
     }
+    last_active_at: 1000000  # 1 second past epoch in microseconds
   },
   {
     urn: "aff4:/C.0000000000000001"
     flow_id: "INCORRECT"
     name: "TimelineFlow"
-    state: 1
+    state: TERMINATED
     args: {
       [type.googleapis.com/grr.TimelineArgs] {
         root: "/root"
       }
     }
+    last_active_at: 1000000  # 1 second past epoch in microseconds
   },
   {
     urn: "aff4:/C.0000000000000001"
-    flow_id: "CORRECT_LIN",
+    flow_id: "CORRECT_LIN_1_SECOND",
     name: "TimelineFlow",
-    state: 1
+    state: TERMINATED
     args: {
       [type.googleapis.com/grr.TimelineArgs] {
         root: "/"
       }
     }
+    last_active_at: 1000000  # 1 second past epoch in microseconds
+  },
+  {
+    urn: "aff4:/C.0000000000000001"
+    flow_id: "CORRECT_LIN_2_SECOND",
+    name: "TimelineFlow",
+    state: TERMINATED
+    args: {
+      [type.googleapis.com/grr.TimelineArgs] {
+        root: "/"
+      }
+    }
+    last_active_at: 2000000  # 1 second past epoch in microseconds
   },
   {
     urn: "aff4:/C.0000000000000001"
     flow_id: "INCORRECT_WIN",
     name: "TimelineFlow",
-    state: 1
+    state: TERMINATED
     args: {
       [type.googleapis.com/grr.TimelineArgs] {
         root: "C:/Users/test"
       }
     }
+    last_active_at: 1000000  # 1 second past epoch in microseconds
   },
   {
     urn: "aff4:/C.0000000000000001"
     flow_id: "CORRECT_WIN",
     name: "TimelineFlow",
-    state: 1
+    state: TERMINATED
     args: {
       [type.googleapis.com/grr.TimelineArgs] {
         root: "C:/"
       }
     }
+    last_active_at: 1000000  # 1 second past epoch in microseconds
   }
 ]
```

### Comparing `grrshell-20231227/grrshell/tests/testdata/mock_client_linux.textproto` & `grrshell-20240405/grrshell/tests/testdata/mock_client_linux.textproto`

 * *Files identical despite different names*

### Comparing `grrshell-20231227/grrshell/tests/testdata/mock_hash_linux.textproto` & `grrshell-20240405/grrshell/tests/testdata/mock_hash_linux.textproto`

 * *Files identical despite different names*

### Comparing `grrshell-20231227/grrshell/tests/testdata/mock_hash_windows.textproto` & `grrshell-20240405/grrshell/tests/testdata/mock_hash_windows.textproto`

 * *Files identical despite different names*

### Comparing `grrshell-20231227/grrshell/tests/testdata/mock_hash_windows_ads.textproto` & `grrshell-20240405/grrshell/tests/testdata/mock_hash_windows_ads.textproto`

 * *Files identical despite different names*

### Comparing `grrshell-20231227/grrshell/tests/testdata/sample_timeline_darwin` & `grrshell-20240405/grrshell/tests/testdata/sample_timeline_darwin`

 * *Files identical despite different names*

### Comparing `grrshell-20231227/grrshell/tests/testdata/sample_timeline_linux` & `grrshell-20240405/grrshell/tests/testdata/sample_timeline_linux`

 * *Files identical despite different names*

### Comparing `grrshell-20231227/grrshell/tests/testdata/sample_timeline_windows` & `grrshell-20240405/grrshell/tests/testdata/sample_timeline_windows`

 * *Files 2% similar despite different names*

```diff
@@ -65,7 +65,10 @@
 0|C:\\Program Files\\7-Zip\\Lang\\hu.txt|281474976832288|-rw-rw-rw-|0|0|9601|1684112741.8820622|1636452000.0|1636452000.0|1636452000.0
 0|C:\\Program Files\\7-Zip\\Lang\\hy.txt|281474976832289|-rw-rw-rw-|0|0|14158|1684112741.8830771|1517112000.0|1517112000.0|1517112000.0
 0|C:\\Program Files\\7-Zip\\Lang\\id.txt|281474976832290|-rw-rw-rw-|0|0|8344|1684112741.884097|1581998400.0|1581998400.0|1581998400.0
 0|C:\\Program Files\\7-Zip\\Lang\\io.txt|281474976832291|-rw-rw-rw-|0|0|5074|1684112741.8850777|1517112000.0|1517112000.0|1517112000.0
 0|C:\\Program Files\\7-Zip\\Lang\\is.txt|281474976832292|-rw-rw-rw-|0|0|8746|1684112741.886078|1573650000.0|1573650000.0|1573650000.0
 0|C:\\Program Files\\7-Zip\\Lang\\it.txt|281474976832293|-rw-rw-rw-|0|0|9880|1684112741.887078|1657623600.0|1657623600.0|1657623600.0
 0|C:\\Program Files\\7-Zip\\Lang\\ja.txt|281474976832294|-rw-rw-rw-|0|0|12217|1684112741.887078|1657623600.0|1657623600.0|1657623600.0
+# b/319755600 - Directory name is '0xC2 0xA0'
+0|C:\\ |15655264|drwxrwxrwx|0|0|0|1705582800.0|1705596148.0|1705596090.74|1705596090.74
+0|C:\\ \\file_in_dodgy_dir|15687808|-rw-rw-rw-|0|0|5|1705582800.0|1705596148.0|1705596148.17|1705596148.17
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `grrshell-20231227/grrshell/tests/testdata/sample_timeline_windows_d_drive` & `grrshell-20240405/grrshell/tests/testdata/sample_timeline_windows_d_drive`

 * *Files identical despite different names*

### Comparing `grrshell-20231227/grrshell/tests/utils_test.py` & `grrshell-20240405/grrshell/tests/utils_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Unit tests for util methods."""
 
-# pylint: disable=wrong-import-order
+# pylint: disable=wrong-import-order,ungrouped-imports
 from typing import Union
 
 from absl.testing import absltest
 from absl.testing import parameterized
 from grrshell.lib import utils
```

### Comparing `grrshell-20231227/PKG-INFO` & `grrshell-20240405/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grrshell
-Version: 20231227
+Version: 20240405
 Summary: 
 Author: Ramo
 Author-email: ramoj@google.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

