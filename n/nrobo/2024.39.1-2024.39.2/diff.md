# Comparing `tmp/nrobo-2024.39.1.tar.gz` & `tmp/nrobo-2024.39.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nrobo-2024.39.1.tar", last modified: Tue Apr  2 20:26:00 2024, max compression
+gzip compressed data, was "nrobo-2024.39.2.tar", last modified: Fri Apr  5 07:21:04 2024, max compression
```

## Comparing `nrobo-2024.39.1.tar` & `nrobo-2024.39.2.tar`

### file list

```diff
@@ -1,124 +1,124 @@
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-02 20:26:00.131354 nrobo-2024.39.1/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1079 2024-02-02 05:31:36.000000 nrobo-2024.39.1/LICENSE
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    18169 2024-04-02 20:26:00.130512 nrobo-2024.39.1/PKG-INFO
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    16531 2024-04-02 20:14:11.000000 nrobo-2024.39.1/README.rst
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-02 20:26:00.091713 nrobo-2024.39.1/nrobo/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     8668 2024-04-02 20:25:37.000000 nrobo-2024.39.1/nrobo/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-02 20:26:00.096652 nrobo-2024.39.1/nrobo/appium/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      716 2024-03-11 11:20:45.000000 nrobo-2024.39.1/nrobo/appium/__init__.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       72 2024-03-11 14:41:50.000000 nrobo-2024.39.1/nrobo/appium/android_capability.yaml
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       73 2024-03-11 12:05:03.000000 nrobo-2024.39.1/nrobo/appium/ios_capability.yaml
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-02 20:26:00.099183 nrobo-2024.39.1/nrobo/browserConfigs/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      452 2024-02-29 19:11:43.000000 nrobo-2024.39.1/nrobo/browserConfigs/__init__.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       35 2024-02-29 19:12:02.000000 nrobo-2024.39.1/nrobo/browserConfigs/capability.yaml
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       17 2024-02-19 15:42:30.000000 nrobo-2024.39.1/nrobo/browserConfigs/chrome_config.txt
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       39 2024-02-29 19:12:02.000000 nrobo-2024.39.1/nrobo/browserConfigs/chrome_prefs.yaml
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       63 2024-02-29 19:12:02.000000 nrobo-2024.39.1/nrobo/browserConfigs/markers.yaml
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-02 20:26:00.099683 nrobo-2024.39.1/nrobo/browsers/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      459 2024-02-15 02:56:21.000000 nrobo-2024.39.1/nrobo/browsers/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-02 20:26:00.100183 nrobo-2024.39.1/nrobo/browsers/chrome/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2168 2024-02-15 02:56:21.000000 nrobo-2024.39.1/nrobo/browsers/chrome/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-02 20:26:00.100696 nrobo-2024.39.1/nrobo/browsers/edge/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      468 2024-02-15 02:56:21.000000 nrobo-2024.39.1/nrobo/browsers/edge/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-02 20:26:00.101192 nrobo-2024.39.1/nrobo/browsers/firefox/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      472 2024-02-29 19:11:43.000000 nrobo-2024.39.1/nrobo/browsers/firefox/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-02 20:26:00.101681 nrobo-2024.39.1/nrobo/browsers/safari/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      477 2024-02-29 19:11:43.000000 nrobo-2024.39.1/nrobo/browsers/safari/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-02 20:26:00.104324 nrobo-2024.39.1/nrobo/cli/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2654 2024-03-23 16:37:25.000000 nrobo-2024.39.1/nrobo/cli/__init__.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2895 2024-03-11 13:01:11.000000 nrobo-2024.39.1/nrobo/cli/cli_constants.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       17 2024-02-15 02:56:21.000000 nrobo-2024.39.1/nrobo/cli/cli_version.yaml
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-02 20:26:00.104820 nrobo-2024.39.1/nrobo/cli/detection/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2585 2024-02-29 19:12:02.000000 nrobo-2024.39.1/nrobo/cli/detection/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-02 20:26:00.105325 nrobo-2024.39.1/nrobo/cli/formatting/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1226 2024-02-29 19:11:43.000000 nrobo-2024.39.1/nrobo/cli/formatting/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-02 20:26:00.106507 nrobo-2024.39.1/nrobo/cli/install/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    12266 2024-03-24 02:00:53.000000 nrobo-2024.39.1/nrobo/cli/install/__init__.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      987 2024-04-02 19:56:57.000000 nrobo-2024.39.1/nrobo/cli/install/requirements.txt
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    15058 2024-03-07 11:01:00.000000 nrobo-2024.39.1/nrobo/cli/launcher.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-02 20:26:00.106999 nrobo-2024.39.1/nrobo/cli/ncodes/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      594 2024-02-29 19:12:02.000000 nrobo-2024.39.1/nrobo/cli/ncodes/__init__.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1806 2024-03-01 03:35:55.000000 nrobo-2024.39.1/nrobo/cli/nglobals.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-02 20:26:00.107488 nrobo-2024.39.1/nrobo/cli/nrobo_args/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    25971 2024-03-11 13:04:58.000000 nrobo-2024.39.1/nrobo/cli/nrobo_args/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-02 20:26:00.108061 nrobo-2024.39.1/nrobo/cli/tools/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      813 2024-02-29 19:11:43.000000 nrobo-2024.39.1/nrobo/cli/tools/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-02 20:26:00.108564 nrobo-2024.39.1/nrobo/cli/upgrade/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     6308 2024-03-06 04:27:25.000000 nrobo-2024.39.1/nrobo/cli/upgrade/__init__.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    32339 2024-04-02 20:25:37.000000 nrobo-2024.39.1/nrobo/conftest.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-02 20:26:00.109068 nrobo-2024.39.1/nrobo/exceptions/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1937 2024-02-29 19:12:02.000000 nrobo-2024.39.1/nrobo/exceptions/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-02 20:26:00.111398 nrobo-2024.39.1/nrobo/framework/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        0 2024-02-05 04:31:26.000000 nrobo-2024.39.1/nrobo/framework/__init__.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      540 2024-02-16 15:47:33.000000 nrobo-2024.39.1/nrobo/framework/conftest-host.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      779 2024-03-07 13:19:52.000000 nrobo-2024.39.1/nrobo/framework/nrobo-config.yaml
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-02 20:26:00.112792 nrobo-2024.39.1/nrobo/framework/pages/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1506 2024-02-29 19:12:02.000000 nrobo-2024.39.1/nrobo/framework/pages/PagePyPiHome.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      485 2024-02-29 19:12:02.000000 nrobo-2024.39.1/nrobo/framework/pages/PageSearch.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2540 2024-02-29 19:12:02.000000 nrobo-2024.39.1/nrobo/framework/pages/__init__.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       26 2024-03-23 15:17:33.000000 nrobo-2024.39.1/nrobo/framework/requirements.txt
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        0 2024-03-30 08:56:49.000000 nrobo-2024.39.1/nrobo/framework/secrets.yaml
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-02 20:26:00.113322 nrobo-2024.39.1/nrobo/framework/tests/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        2 2024-02-07 04:51:13.000000 nrobo-2024.39.1/nrobo/framework/tests/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-02 20:26:00.083766 nrobo-2024.39.1/nrobo/framework/tests/mobile/
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-02 20:26:00.113830 nrobo-2024.39.1/nrobo/framework/tests/mobile/appium/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      383 2024-03-07 08:23:34.000000 nrobo-2024.39.1/nrobo/framework/tests/mobile/appium/test_appium.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-02 20:26:00.114361 nrobo-2024.39.1/nrobo/framework/tests/web/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1904 2024-02-29 19:12:02.000000 nrobo-2024.39.1/nrobo/framework/tests/web/PyPi_home_page_test.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-02 20:26:00.114874 nrobo-2024.39.1/nrobo/framework/tests/web/examples/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     6470 2024-02-29 19:12:02.000000 nrobo-2024.39.1/nrobo/framework/tests/web/examples/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-02 20:26:00.115885 nrobo-2024.39.1/nrobo/framework/tests/web/gui/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      723 2024-03-03 02:33:11.000000 nrobo-2024.39.1/nrobo/framework/tests/web/gui/PyPi_home_page_test.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        0 2024-02-06 09:49:32.000000 nrobo-2024.39.1/nrobo/framework/tests/web/gui/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-02 20:26:00.116504 nrobo-2024.39.1/nrobo/framework/tests/web/no_gui/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        0 2024-02-06 09:49:18.000000 nrobo-2024.39.1/nrobo/framework/tests/web/no_gui/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-02 20:26:00.120160 nrobo-2024.39.1/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        0 2024-02-29 19:12:02.000000 nrobo-2024.39.1/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/__init__.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      820 2024-02-29 19:12:02.000000 nrobo-2024.39.1/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_action_chain_methods.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2427 2024-02-29 19:12:02.000000 nrobo-2024.39.1/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_alert_methods.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     7583 2024-02-29 19:12:02.000000 nrobo-2024.39.1/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_element_wrapper_methods.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    19118 2024-02-29 19:12:02.000000 nrobo-2024.39.1/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_nrobo_methods.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1418 2024-02-29 19:12:02.000000 nrobo-2024.39.1/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_nrobo_wait_methods.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     6860 2024-02-29 19:12:02.000000 nrobo-2024.39.1/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_select.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-02 20:26:00.120665 nrobo-2024.39.1/nrobo/selenese/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    46611 2024-04-01 12:06:54.000000 nrobo-2024.39.1/nrobo/selenese/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-02 20:26:00.121276 nrobo-2024.39.1/nrobo/util/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      431 2024-02-15 02:56:21.000000 nrobo-2024.39.1/nrobo/util/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-02 20:26:00.121780 nrobo-2024.39.1/nrobo/util/commands/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      431 2024-02-15 02:56:21.000000 nrobo-2024.39.1/nrobo/util/commands/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-02 20:26:00.122278 nrobo-2024.39.1/nrobo/util/commands/ncommands/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2105 2024-03-06 18:41:46.000000 nrobo-2024.39.1/nrobo/util/commands/ncommands/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-02 20:26:00.122789 nrobo-2024.39.1/nrobo/util/commands/posix/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      533 2024-02-29 19:11:43.000000 nrobo-2024.39.1/nrobo/util/commands/posix/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-02 20:26:00.123288 nrobo-2024.39.1/nrobo/util/commands/windows/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      535 2024-02-29 19:11:43.000000 nrobo-2024.39.1/nrobo/util/commands/windows/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-02 20:26:00.123809 nrobo-2024.39.1/nrobo/util/common/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     7376 2024-03-18 10:49:47.000000 nrobo-2024.39.1/nrobo/util/common/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-02 20:26:00.124315 nrobo-2024.39.1/nrobo/util/constants/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1686 2024-02-29 19:11:43.000000 nrobo-2024.39.1/nrobo/util/constants/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-02 20:26:00.125183 nrobo-2024.39.1/nrobo/util/database/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        0 2024-03-30 08:55:53.000000 nrobo-2024.39.1/nrobo/util/database/__init__.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1992 2024-03-30 08:55:53.000000 nrobo-2024.39.1/nrobo/util/database/connectors.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-02 20:26:00.125671 nrobo-2024.39.1/nrobo/util/filesystem/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     6919 2024-02-29 19:12:02.000000 nrobo-2024.39.1/nrobo/util/filesystem/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-02 20:26:00.126174 nrobo-2024.39.1/nrobo/util/network/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      844 2024-02-29 19:12:02.000000 nrobo-2024.39.1/nrobo/util/network/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-02 20:26:00.126659 nrobo-2024.39.1/nrobo/util/platform/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      742 2024-02-29 19:11:43.000000 nrobo-2024.39.1/nrobo/util/platform/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-02 20:26:00.127141 nrobo-2024.39.1/nrobo/util/process/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     3322 2024-02-29 19:12:02.000000 nrobo-2024.39.1/nrobo/util/process/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-02 20:26:00.127625 nrobo-2024.39.1/nrobo/util/python/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2101 2024-02-29 19:11:43.000000 nrobo-2024.39.1/nrobo/util/python/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-02 20:26:00.128114 nrobo-2024.39.1/nrobo/util/regex/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      976 2024-02-29 19:11:43.000000 nrobo-2024.39.1/nrobo/util/regex/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-02 20:26:00.128609 nrobo-2024.39.1/nrobo/util/version/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     8316 2024-02-29 19:12:02.000000 nrobo-2024.39.1/nrobo/util/version/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-02 20:26:00.129414 nrobo-2024.39.1/nrobo.egg-info/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    18169 2024-04-02 20:26:00.000000 nrobo-2024.39.1/nrobo.egg-info/PKG-INFO
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2776 2024-04-02 20:26:00.000000 nrobo-2024.39.1/nrobo.egg-info/SOURCES.txt
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        1 2024-04-02 20:26:00.000000 nrobo-2024.39.1/nrobo.egg-info/dependency_links.txt
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       41 2024-04-02 20:26:00.000000 nrobo-2024.39.1/nrobo.egg-info/entry_points.txt
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       43 2024-04-02 20:26:00.000000 nrobo-2024.39.1/nrobo.egg-info/requires.txt
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        6 2024-04-02 20:26:00.000000 nrobo-2024.39.1/nrobo.egg-info/top_level.txt
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2545 2024-04-02 20:25:37.000000 nrobo-2024.39.1/pyproject.toml
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       38 2024-04-02 20:26:00.131500 nrobo-2024.39.1/setup.cfg
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:21:04.050386 nrobo-2024.39.2/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1079 2024-02-02 05:31:36.000000 nrobo-2024.39.2/LICENSE
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    18169 2024-04-05 07:21:04.049384 nrobo-2024.39.2/PKG-INFO
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    16531 2024-04-05 07:20:34.000000 nrobo-2024.39.2/README.rst
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:21:03.999951 nrobo-2024.39.2/nrobo/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     8668 2024-04-05 07:20:27.000000 nrobo-2024.39.2/nrobo/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:21:04.005781 nrobo-2024.39.2/nrobo/appium/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      716 2024-03-11 11:20:45.000000 nrobo-2024.39.2/nrobo/appium/__init__.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       72 2024-03-11 14:41:50.000000 nrobo-2024.39.2/nrobo/appium/android_capability.yaml
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       73 2024-03-11 12:05:03.000000 nrobo-2024.39.2/nrobo/appium/ios_capability.yaml
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:21:04.008932 nrobo-2024.39.2/nrobo/browserConfigs/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      452 2024-02-29 19:11:43.000000 nrobo-2024.39.2/nrobo/browserConfigs/__init__.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       35 2024-02-29 19:12:02.000000 nrobo-2024.39.2/nrobo/browserConfigs/capability.yaml
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       17 2024-02-19 15:42:30.000000 nrobo-2024.39.2/nrobo/browserConfigs/chrome_config.txt
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       39 2024-02-29 19:12:02.000000 nrobo-2024.39.2/nrobo/browserConfigs/chrome_prefs.yaml
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       63 2024-02-29 19:12:02.000000 nrobo-2024.39.2/nrobo/browserConfigs/markers.yaml
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:21:04.009553 nrobo-2024.39.2/nrobo/browsers/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      459 2024-02-15 02:56:21.000000 nrobo-2024.39.2/nrobo/browsers/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:21:04.010162 nrobo-2024.39.2/nrobo/browsers/chrome/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2168 2024-02-15 02:56:21.000000 nrobo-2024.39.2/nrobo/browsers/chrome/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:21:04.010784 nrobo-2024.39.2/nrobo/browsers/edge/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      468 2024-02-15 02:56:21.000000 nrobo-2024.39.2/nrobo/browsers/edge/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:21:04.011394 nrobo-2024.39.2/nrobo/browsers/firefox/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      472 2024-02-29 19:11:43.000000 nrobo-2024.39.2/nrobo/browsers/firefox/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:21:04.011999 nrobo-2024.39.2/nrobo/browsers/safari/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      477 2024-02-29 19:11:43.000000 nrobo-2024.39.2/nrobo/browsers/safari/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:21:04.015185 nrobo-2024.39.2/nrobo/cli/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2654 2024-03-23 16:37:25.000000 nrobo-2024.39.2/nrobo/cli/__init__.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2895 2024-03-11 13:01:11.000000 nrobo-2024.39.2/nrobo/cli/cli_constants.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       17 2024-02-15 02:56:21.000000 nrobo-2024.39.2/nrobo/cli/cli_version.yaml
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:21:04.015818 nrobo-2024.39.2/nrobo/cli/detection/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2585 2024-02-29 19:12:02.000000 nrobo-2024.39.2/nrobo/cli/detection/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:21:04.016428 nrobo-2024.39.2/nrobo/cli/formatting/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1226 2024-02-29 19:11:43.000000 nrobo-2024.39.2/nrobo/cli/formatting/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:21:04.017776 nrobo-2024.39.2/nrobo/cli/install/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    12266 2024-03-24 02:00:53.000000 nrobo-2024.39.2/nrobo/cli/install/__init__.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      987 2024-04-02 19:56:57.000000 nrobo-2024.39.2/nrobo/cli/install/requirements.txt
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    15058 2024-03-07 11:01:00.000000 nrobo-2024.39.2/nrobo/cli/launcher.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:21:04.018417 nrobo-2024.39.2/nrobo/cli/ncodes/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      594 2024-02-29 19:12:02.000000 nrobo-2024.39.2/nrobo/cli/ncodes/__init__.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1806 2024-03-01 03:35:55.000000 nrobo-2024.39.2/nrobo/cli/nglobals.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:21:04.019026 nrobo-2024.39.2/nrobo/cli/nrobo_args/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    25971 2024-03-11 13:04:58.000000 nrobo-2024.39.2/nrobo/cli/nrobo_args/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:21:04.019707 nrobo-2024.39.2/nrobo/cli/tools/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      813 2024-02-29 19:11:43.000000 nrobo-2024.39.2/nrobo/cli/tools/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:21:04.020351 nrobo-2024.39.2/nrobo/cli/upgrade/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     6308 2024-03-06 04:27:25.000000 nrobo-2024.39.2/nrobo/cli/upgrade/__init__.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    32195 2024-04-05 07:20:27.000000 nrobo-2024.39.2/nrobo/conftest.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:21:04.020959 nrobo-2024.39.2/nrobo/exceptions/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1937 2024-02-29 19:12:02.000000 nrobo-2024.39.2/nrobo/exceptions/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:21:04.024287 nrobo-2024.39.2/nrobo/framework/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        0 2024-02-05 04:31:26.000000 nrobo-2024.39.2/nrobo/framework/__init__.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      540 2024-02-16 15:47:33.000000 nrobo-2024.39.2/nrobo/framework/conftest-host.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      779 2024-03-07 13:19:52.000000 nrobo-2024.39.2/nrobo/framework/nrobo-config.yaml
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:21:04.026007 nrobo-2024.39.2/nrobo/framework/pages/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1506 2024-02-29 19:12:02.000000 nrobo-2024.39.2/nrobo/framework/pages/PagePyPiHome.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      485 2024-02-29 19:12:02.000000 nrobo-2024.39.2/nrobo/framework/pages/PageSearch.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2540 2024-02-29 19:12:02.000000 nrobo-2024.39.2/nrobo/framework/pages/__init__.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       26 2024-03-23 15:17:33.000000 nrobo-2024.39.2/nrobo/framework/requirements.txt
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        0 2024-03-30 08:56:49.000000 nrobo-2024.39.2/nrobo/framework/secrets.yaml
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:21:04.026626 nrobo-2024.39.2/nrobo/framework/tests/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        2 2024-02-07 04:51:13.000000 nrobo-2024.39.2/nrobo/framework/tests/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:21:03.990395 nrobo-2024.39.2/nrobo/framework/tests/mobile/
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:21:04.027244 nrobo-2024.39.2/nrobo/framework/tests/mobile/appium/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      383 2024-03-07 08:23:34.000000 nrobo-2024.39.2/nrobo/framework/tests/mobile/appium/test_appium.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:21:04.028308 nrobo-2024.39.2/nrobo/framework/tests/web/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1904 2024-02-29 19:12:02.000000 nrobo-2024.39.2/nrobo/framework/tests/web/PyPi_home_page_test.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:21:04.029123 nrobo-2024.39.2/nrobo/framework/tests/web/examples/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     6470 2024-02-29 19:12:02.000000 nrobo-2024.39.2/nrobo/framework/tests/web/examples/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:21:04.030919 nrobo-2024.39.2/nrobo/framework/tests/web/gui/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      723 2024-03-03 02:33:11.000000 nrobo-2024.39.2/nrobo/framework/tests/web/gui/PyPi_home_page_test.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        0 2024-02-06 09:49:32.000000 nrobo-2024.39.2/nrobo/framework/tests/web/gui/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:21:04.031429 nrobo-2024.39.2/nrobo/framework/tests/web/no_gui/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        0 2024-02-06 09:49:18.000000 nrobo-2024.39.2/nrobo/framework/tests/web/no_gui/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:21:04.036097 nrobo-2024.39.2/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        0 2024-02-29 19:12:02.000000 nrobo-2024.39.2/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/__init__.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      820 2024-02-29 19:12:02.000000 nrobo-2024.39.2/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_action_chain_methods.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2427 2024-02-29 19:12:02.000000 nrobo-2024.39.2/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_alert_methods.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     7583 2024-02-29 19:12:02.000000 nrobo-2024.39.2/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_element_wrapper_methods.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    19118 2024-02-29 19:12:02.000000 nrobo-2024.39.2/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_nrobo_methods.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1418 2024-02-29 19:12:02.000000 nrobo-2024.39.2/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_nrobo_wait_methods.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     6860 2024-02-29 19:12:02.000000 nrobo-2024.39.2/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_select.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:21:04.036796 nrobo-2024.39.2/nrobo/selenese/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    46611 2024-04-01 12:06:54.000000 nrobo-2024.39.2/nrobo/selenese/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:21:04.037545 nrobo-2024.39.2/nrobo/util/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      431 2024-02-15 02:56:21.000000 nrobo-2024.39.2/nrobo/util/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:21:04.038192 nrobo-2024.39.2/nrobo/util/commands/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      431 2024-02-15 02:56:21.000000 nrobo-2024.39.2/nrobo/util/commands/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:21:04.038859 nrobo-2024.39.2/nrobo/util/commands/ncommands/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2105 2024-03-06 18:41:46.000000 nrobo-2024.39.2/nrobo/util/commands/ncommands/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:21:04.039525 nrobo-2024.39.2/nrobo/util/commands/posix/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      533 2024-02-29 19:11:43.000000 nrobo-2024.39.2/nrobo/util/commands/posix/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:21:04.040194 nrobo-2024.39.2/nrobo/util/commands/windows/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      535 2024-02-29 19:11:43.000000 nrobo-2024.39.2/nrobo/util/commands/windows/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:21:04.040823 nrobo-2024.39.2/nrobo/util/common/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     7376 2024-03-18 10:49:47.000000 nrobo-2024.39.2/nrobo/util/common/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:21:04.041454 nrobo-2024.39.2/nrobo/util/constants/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1686 2024-02-29 19:11:43.000000 nrobo-2024.39.2/nrobo/util/constants/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:21:04.042557 nrobo-2024.39.2/nrobo/util/database/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        0 2024-03-30 08:55:53.000000 nrobo-2024.39.2/nrobo/util/database/__init__.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1992 2024-03-30 08:55:53.000000 nrobo-2024.39.2/nrobo/util/database/connectors.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:21:04.043205 nrobo-2024.39.2/nrobo/util/filesystem/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     6919 2024-02-29 19:12:02.000000 nrobo-2024.39.2/nrobo/util/filesystem/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:21:04.043841 nrobo-2024.39.2/nrobo/util/network/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      844 2024-02-29 19:12:02.000000 nrobo-2024.39.2/nrobo/util/network/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:21:04.044496 nrobo-2024.39.2/nrobo/util/platform/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      742 2024-02-29 19:11:43.000000 nrobo-2024.39.2/nrobo/util/platform/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:21:04.045139 nrobo-2024.39.2/nrobo/util/process/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     3322 2024-02-29 19:12:02.000000 nrobo-2024.39.2/nrobo/util/process/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:21:04.045771 nrobo-2024.39.2/nrobo/util/python/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2101 2024-02-29 19:11:43.000000 nrobo-2024.39.2/nrobo/util/python/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:21:04.046424 nrobo-2024.39.2/nrobo/util/regex/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      976 2024-02-29 19:11:43.000000 nrobo-2024.39.2/nrobo/util/regex/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:21:04.047090 nrobo-2024.39.2/nrobo/util/version/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     8316 2024-02-29 19:12:02.000000 nrobo-2024.39.2/nrobo/util/version/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:21:04.048007 nrobo-2024.39.2/nrobo.egg-info/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    18169 2024-04-05 07:21:03.000000 nrobo-2024.39.2/nrobo.egg-info/PKG-INFO
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2776 2024-04-05 07:21:03.000000 nrobo-2024.39.2/nrobo.egg-info/SOURCES.txt
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        1 2024-04-05 07:21:03.000000 nrobo-2024.39.2/nrobo.egg-info/dependency_links.txt
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       41 2024-04-05 07:21:03.000000 nrobo-2024.39.2/nrobo.egg-info/entry_points.txt
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       43 2024-04-05 07:21:03.000000 nrobo-2024.39.2/nrobo.egg-info/requires.txt
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        6 2024-04-05 07:21:03.000000 nrobo-2024.39.2/nrobo.egg-info/top_level.txt
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2545 2024-04-05 07:20:27.000000 nrobo-2024.39.2/pyproject.toml
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       38 2024-04-05 07:21:04.050576 nrobo-2024.39.2/setup.cfg
```

### Comparing `nrobo-2024.39.1/LICENSE` & `nrobo-2024.39.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nrobo-2024.39.1/PKG-INFO` & `nrobo-2024.39.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nrobo
-Version: 2024.39.1
+Version: 2024.39.2
 Summary: Powerful! Yet, Easy to USE! Automated Testing Framework
 Author-email: Panchdev Singh Chauhan <erpanchdev@gmail.com>
 Maintainer-email: Panchdev Singh Chauhan <erpanchdev@gmail.com>
 Project-URL: Homepage, https://pypi.org/project/nrobo/
 Project-URL: GitHub Repo, https://github.com/pancht/ngrobo
 Project-URL: Bug Tracker, https://github.com/pancht/ngrobo/issues
 Project-URL: changelog, https://github.com/pancht/ngrobo/blob/master/CHANGELOG.md
@@ -384,108 +384,108 @@
    :align: center
    :header-rows: 1
 
    * - Country
      - Percent
      - Download Count
    * - US
-     - 39.08%
-     - 22,848
+     - 38.96%
+     - 23,088
    * - CN
-     - 13.01%
-     - 7,606
+     - 13.06%
+     - 7,741
    * - DE
-     - 6.38%
-     - 3,731
+     - 6.48%
+     - 3,838
    * - SG
-     - 5.25%
-     - 3,070
+     - 5.58%
+     - 3,308
    * - RU
-     - 5.23%
-     - 3,059
+     - 5.17%
+     - 3,064
    * - HK
-     - 4.18%
-     - 2,443
+     - 4.13%
+     - 2,449
    * - JP
-     - 3.13%
-     - 1,830
+     - 3.10%
+     - 1,834
    * - FR
-     - 2.86%
-     - 1,673
+     - 2.83%
+     - 1,677
    * - KR
-     - 2.74%
-     - 1,599
+     - 2.72%
+     - 1,611
    * - CA
-     - 2.70%
-     - 1,579
+     - 2.67%
+     - 1,583
    * - NO
      - 2.00%
-     - 1,171
+     - 1,183
    * - GB
-     - 1.86%
-     - 1,088
+     - 1.84%
+     - 1,091
    * - AU
-     - 1.78%
+     - 1.75%
      - 1,039
    * - IN
-     - 1.53%
-     - 895
+     - 1.52%
+     - 901
    * - SE
-     - 1.22%
-     - 712
+     - 1.21%
+     - 716
    * - TH
      - 0.79%
-     - 460
+     - 466
    * - HR
-     - 0.79%
-     - 460
+     - 0.78%
+     - 462
    * - DK
-     - 0.68%
+     - 0.67%
      - 395
    * - IE
      - 0.66%
-     - 385
+     - 389
    * - TW
-     - 0.62%
+     - 0.61%
      - 363
    * - IL
      - 0.58%
      - 341
    * - NL
-     - 0.51%
+     - 0.50%
      - 297
    * - ES
-     - 0.45%
+     - 0.44%
      - 262
    * - CH
-     - 0.43%
-     - 250
+     - 0.42%
+     - 251
    * - AE
      - 0.35%
      - 207
    * - CZ
-     - 0.25%
+     - 0.24%
      - 144
    * - FI
      - 0.16%
-     - 91
+     - 93
    * - ZA
      - 0.15%
      - 89
    * - BR
      - 0.13%
      - 77
    * - PL
      - 0.10%
      - 61
    * - TR
-     - 0.08%
+     - 0.07%
      - 44
    * - CW
-     - 0.08%
+     - 0.07%
      - 44
    * - OM
      - 0.07%
      - 42
    * - IS
      - 0.07%
      - 42
@@ -500,29 +500,29 @@
      - 8
    * - CY
      - 0.01%
      - 6
    * - DZ
      - 0.01%
      - 4
-   * - AR
+   * - EE
      - 0.01%
      - 3
-   * - EE
+   * - AR
      - 0.01%
      - 3
    * - SK
      - 0.00%
      - 2
-   * - PT
+   * - RS
      - 0.00%
      - 1
-   * - RS
+   * - PT
      - 0.00%
      - 1
    * - MX
      - 0.00%
      - 1
    * - **Total**
      - **100.00%**
-     - **58,460**
+     - **59,255**
```

### Comparing `nrobo-2024.39.1/README.rst` & `nrobo-2024.39.2/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -348,108 +348,108 @@
    :align: center
    :header-rows: 1
 
    * - Country
      - Percent
      - Download Count
    * - US
-     - 39.08%
-     - 22,848
+     - 38.96%
+     - 23,088
    * - CN
-     - 13.01%
-     - 7,606
+     - 13.06%
+     - 7,741
    * - DE
-     - 6.38%
-     - 3,731
+     - 6.48%
+     - 3,838
    * - SG
-     - 5.25%
-     - 3,070
+     - 5.58%
+     - 3,308
    * - RU
-     - 5.23%
-     - 3,059
+     - 5.17%
+     - 3,064
    * - HK
-     - 4.18%
-     - 2,443
+     - 4.13%
+     - 2,449
    * - JP
-     - 3.13%
-     - 1,830
+     - 3.10%
+     - 1,834
    * - FR
-     - 2.86%
-     - 1,673
+     - 2.83%
+     - 1,677
    * - KR
-     - 2.74%
-     - 1,599
+     - 2.72%
+     - 1,611
    * - CA
-     - 2.70%
-     - 1,579
+     - 2.67%
+     - 1,583
    * - NO
      - 2.00%
-     - 1,171
+     - 1,183
    * - GB
-     - 1.86%
-     - 1,088
+     - 1.84%
+     - 1,091
    * - AU
-     - 1.78%
+     - 1.75%
      - 1,039
    * - IN
-     - 1.53%
-     - 895
+     - 1.52%
+     - 901
    * - SE
-     - 1.22%
-     - 712
+     - 1.21%
+     - 716
    * - TH
      - 0.79%
-     - 460
+     - 466
    * - HR
-     - 0.79%
-     - 460
+     - 0.78%
+     - 462
    * - DK
-     - 0.68%
+     - 0.67%
      - 395
    * - IE
      - 0.66%
-     - 385
+     - 389
    * - TW
-     - 0.62%
+     - 0.61%
      - 363
    * - IL
      - 0.58%
      - 341
    * - NL
-     - 0.51%
+     - 0.50%
      - 297
    * - ES
-     - 0.45%
+     - 0.44%
      - 262
    * - CH
-     - 0.43%
-     - 250
+     - 0.42%
+     - 251
    * - AE
      - 0.35%
      - 207
    * - CZ
-     - 0.25%
+     - 0.24%
      - 144
    * - FI
      - 0.16%
-     - 91
+     - 93
    * - ZA
      - 0.15%
      - 89
    * - BR
      - 0.13%
      - 77
    * - PL
      - 0.10%
      - 61
    * - TR
-     - 0.08%
+     - 0.07%
      - 44
    * - CW
-     - 0.08%
+     - 0.07%
      - 44
    * - OM
      - 0.07%
      - 42
    * - IS
      - 0.07%
      - 42
@@ -464,29 +464,29 @@
      - 8
    * - CY
      - 0.01%
      - 6
    * - DZ
      - 0.01%
      - 4
-   * - AR
+   * - EE
      - 0.01%
      - 3
-   * - EE
+   * - AR
      - 0.01%
      - 3
    * - SK
      - 0.00%
      - 2
-   * - PT
+   * - RS
      - 0.00%
      - 1
-   * - RS
+   * - PT
      - 0.00%
      - 1
    * - MX
      - 0.00%
      - 1
    * - **Total**
      - **100.00%**
-     - **58,460**
+     - **59,255**
```

### Comparing `nrobo-2024.39.1/nrobo/__init__.py` & `nrobo-2024.39.2/nrobo/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 nrobo module loads nRoBo globals.
 
 
 @author: Panchdev Singh Chauhan
 @email: erpanchdev@gmail.com
 """
 
-__version__ = '2024.39.1'
+__version__ = '2024.39.2'
 
 # install rich library
 import os
 from pathlib import Path
 
 
 class DB_CONNECTOR_TYPE:
```

### Comparing `nrobo-2024.39.1/nrobo/appium/__init__.py` & `nrobo-2024.39.2/nrobo/appium/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.39.1/nrobo/browsers/chrome/__init__.py` & `nrobo-2024.39.2/nrobo/browsers/chrome/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.39.1/nrobo/cli/__init__.py` & `nrobo-2024.39.2/nrobo/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.39.1/nrobo/cli/cli_constants.py` & `nrobo-2024.39.2/nrobo/cli/cli_constants.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.39.1/nrobo/cli/detection/__init__.py` & `nrobo-2024.39.2/nrobo/cli/detection/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.39.1/nrobo/cli/formatting/__init__.py` & `nrobo-2024.39.2/nrobo/cli/formatting/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.39.1/nrobo/cli/install/__init__.py` & `nrobo-2024.39.2/nrobo/cli/install/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.39.1/nrobo/cli/install/requirements.txt` & `nrobo-2024.39.2/nrobo/cli/install/requirements.txt`

 * *Files identical despite different names*

### Comparing `nrobo-2024.39.1/nrobo/cli/launcher.py` & `nrobo-2024.39.2/nrobo/cli/launcher.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.39.1/nrobo/cli/ncodes/__init__.py` & `nrobo-2024.39.2/nrobo/cli/ncodes/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.39.1/nrobo/cli/nglobals.py` & `nrobo-2024.39.2/nrobo/cli/nglobals.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.39.1/nrobo/cli/nrobo_args/__init__.py` & `nrobo-2024.39.2/nrobo/cli/nrobo_args/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.39.1/nrobo/cli/tools/__init__.py` & `nrobo-2024.39.2/nrobo/cli/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.39.1/nrobo/cli/upgrade/__init__.py` & `nrobo-2024.39.2/nrobo/cli/upgrade/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.39.1/nrobo/conftest.py` & `nrobo-2024.39.2/nrobo/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -262,14 +262,33 @@
 
     update_pytest_life_cycle_log("password")
     # Global fixture returning admin password
     # Access pytest command line options
     return request.config.getoption(f"--{nCLI.PASSWORD}")
 
 
+def get_fake_user_agents():
+    """
+    Get fake user agents at random
+    """
+    from fake_useragent import UserAgent
+
+    _browsers = ['chrome', 'edge', 'firefox', 'safari']
+    _os = ["windows", "macos", "linux", "android", "ios"]
+    _platform = ["pc", "mobile", "tablet"]
+
+    _browser_name = [_browsers[Common.generate_random_numbers(0, 3)]]
+    _os_name = [_os[Common.generate_random_numbers(0, 4)]]
+    _platform_name = [_platform[Common.generate_random_numbers(0, 2)]]
+
+    return UserAgent(browsers=_browser_name,
+                     os=_os_name,
+                     platforms=_platform_name).random
+
+
 @pytest.fixture(autouse=True, scope='function')
 def driver(request):
     """
     Instantiating driver for given browser.
     """
 
     update_pytest_life_cycle_log("driver")
@@ -360,28 +379,15 @@
                                            ChromeDriverManager().install(),
                                            log_output=_driver_log_path))
 
         # Anti Bot Detection logic by ZenRows
         # URL: https://www.zenrows.com/blog/selenium-avoid-bot-detection#how-anti-bots-work
         _driver.execute_script("Object.defineProperty(navigator, 'webdriver', {get: () => undefined})")
 
-        # Initializing a list with two Useragents
-        # useragentarray = [
-        #     "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/108.0.0.0 Safari/537.36",
-        #     "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/107.0.0.0 Safari/537.36",
-        # ]
-        #
-        # for i in range(len(useragentarray)):
-        #     # Setting user agent iteratively as Chrome 108 and 107
-        #     _driver.execute_cdp_cmd("Network.setUserAgentOverride", {"userAgent": useragentarray[i]})
-        #     print(_driver.execute_script("return navigator.userAgent;"))
-        #     # _driver.get("https://www.httpbin.org/headers")
-
-        from fake_useragent import UserAgent
-        _driver.execute_cdp_cmd("Network.setUserAgentOverride", {"userAgent": UserAgent().random})
+        _driver.execute_cdp_cmd("Network.setUserAgentOverride", {"userAgent": get_fake_user_agents()})
 
     elif browser == Browsers.CHROME_HEADLESS:
         """if browser requested is chrome"""
 
         options = webdriver.ChromeOptions()
         options.add_argument('--headless=new')
         options = add_capabilities_from_file(options)
```

### Comparing `nrobo-2024.39.1/nrobo/exceptions/__init__.py` & `nrobo-2024.39.2/nrobo/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.39.1/nrobo/framework/conftest-host.py` & `nrobo-2024.39.2/nrobo/framework/conftest-host.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.39.1/nrobo/framework/nrobo-config.yaml` & `nrobo-2024.39.2/nrobo/framework/nrobo-config.yaml`

 * *Files identical despite different names*

### Comparing `nrobo-2024.39.1/nrobo/framework/pages/PagePyPiHome.py` & `nrobo-2024.39.2/nrobo/framework/pages/PagePyPiHome.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.39.1/nrobo/framework/pages/__init__.py` & `nrobo-2024.39.2/nrobo/framework/pages/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.39.1/nrobo/framework/tests/web/PyPi_home_page_test.py` & `nrobo-2024.39.2/nrobo/framework/tests/web/PyPi_home_page_test.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.39.1/nrobo/framework/tests/web/examples/__init__.py` & `nrobo-2024.39.2/nrobo/framework/tests/web/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.39.1/nrobo/framework/tests/web/gui/PyPi_home_page_test.py` & `nrobo-2024.39.2/nrobo/framework/tests/web/gui/PyPi_home_page_test.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.39.1/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_action_chain_methods.py` & `nrobo-2024.39.2/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_action_chain_methods.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.39.1/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_alert_methods.py` & `nrobo-2024.39.2/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_alert_methods.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.39.1/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_element_wrapper_methods.py` & `nrobo-2024.39.2/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_element_wrapper_methods.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.39.1/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_nrobo_methods.py` & `nrobo-2024.39.2/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_nrobo_methods.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.39.1/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_nrobo_wait_methods.py` & `nrobo-2024.39.2/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_nrobo_wait_methods.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.39.1/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_select.py` & `nrobo-2024.39.2/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_select.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.39.1/nrobo/selenese/__init__.py` & `nrobo-2024.39.2/nrobo/selenese/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.39.1/nrobo/util/commands/ncommands/__init__.py` & `nrobo-2024.39.2/nrobo/util/commands/ncommands/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.39.1/nrobo/util/commands/posix/__init__.py` & `nrobo-2024.39.2/nrobo/util/commands/posix/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.39.1/nrobo/util/commands/windows/__init__.py` & `nrobo-2024.39.2/nrobo/util/commands/windows/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.39.1/nrobo/util/common/__init__.py` & `nrobo-2024.39.2/nrobo/util/common/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.39.1/nrobo/util/constants/__init__.py` & `nrobo-2024.39.2/nrobo/util/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.39.1/nrobo/util/database/connectors.py` & `nrobo-2024.39.2/nrobo/util/database/connectors.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.39.1/nrobo/util/filesystem/__init__.py` & `nrobo-2024.39.2/nrobo/util/filesystem/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.39.1/nrobo/util/network/__init__.py` & `nrobo-2024.39.2/nrobo/util/network/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.39.1/nrobo/util/platform/__init__.py` & `nrobo-2024.39.2/nrobo/util/platform/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.39.1/nrobo/util/process/__init__.py` & `nrobo-2024.39.2/nrobo/util/process/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.39.1/nrobo/util/python/__init__.py` & `nrobo-2024.39.2/nrobo/util/python/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.39.1/nrobo/util/regex/__init__.py` & `nrobo-2024.39.2/nrobo/util/regex/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.39.1/nrobo/util/version/__init__.py` & `nrobo-2024.39.2/nrobo/util/version/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.39.1/nrobo.egg-info/PKG-INFO` & `nrobo-2024.39.2/nrobo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nrobo
-Version: 2024.39.1
+Version: 2024.39.2
 Summary: Powerful! Yet, Easy to USE! Automated Testing Framework
 Author-email: Panchdev Singh Chauhan <erpanchdev@gmail.com>
 Maintainer-email: Panchdev Singh Chauhan <erpanchdev@gmail.com>
 Project-URL: Homepage, https://pypi.org/project/nrobo/
 Project-URL: GitHub Repo, https://github.com/pancht/ngrobo
 Project-URL: Bug Tracker, https://github.com/pancht/ngrobo/issues
 Project-URL: changelog, https://github.com/pancht/ngrobo/blob/master/CHANGELOG.md
@@ -384,108 +384,108 @@
    :align: center
    :header-rows: 1
 
    * - Country
      - Percent
      - Download Count
    * - US
-     - 39.08%
-     - 22,848
+     - 38.96%
+     - 23,088
    * - CN
-     - 13.01%
-     - 7,606
+     - 13.06%
+     - 7,741
    * - DE
-     - 6.38%
-     - 3,731
+     - 6.48%
+     - 3,838
    * - SG
-     - 5.25%
-     - 3,070
+     - 5.58%
+     - 3,308
    * - RU
-     - 5.23%
-     - 3,059
+     - 5.17%
+     - 3,064
    * - HK
-     - 4.18%
-     - 2,443
+     - 4.13%
+     - 2,449
    * - JP
-     - 3.13%
-     - 1,830
+     - 3.10%
+     - 1,834
    * - FR
-     - 2.86%
-     - 1,673
+     - 2.83%
+     - 1,677
    * - KR
-     - 2.74%
-     - 1,599
+     - 2.72%
+     - 1,611
    * - CA
-     - 2.70%
-     - 1,579
+     - 2.67%
+     - 1,583
    * - NO
      - 2.00%
-     - 1,171
+     - 1,183
    * - GB
-     - 1.86%
-     - 1,088
+     - 1.84%
+     - 1,091
    * - AU
-     - 1.78%
+     - 1.75%
      - 1,039
    * - IN
-     - 1.53%
-     - 895
+     - 1.52%
+     - 901
    * - SE
-     - 1.22%
-     - 712
+     - 1.21%
+     - 716
    * - TH
      - 0.79%
-     - 460
+     - 466
    * - HR
-     - 0.79%
-     - 460
+     - 0.78%
+     - 462
    * - DK
-     - 0.68%
+     - 0.67%
      - 395
    * - IE
      - 0.66%
-     - 385
+     - 389
    * - TW
-     - 0.62%
+     - 0.61%
      - 363
    * - IL
      - 0.58%
      - 341
    * - NL
-     - 0.51%
+     - 0.50%
      - 297
    * - ES
-     - 0.45%
+     - 0.44%
      - 262
    * - CH
-     - 0.43%
-     - 250
+     - 0.42%
+     - 251
    * - AE
      - 0.35%
      - 207
    * - CZ
-     - 0.25%
+     - 0.24%
      - 144
    * - FI
      - 0.16%
-     - 91
+     - 93
    * - ZA
      - 0.15%
      - 89
    * - BR
      - 0.13%
      - 77
    * - PL
      - 0.10%
      - 61
    * - TR
-     - 0.08%
+     - 0.07%
      - 44
    * - CW
-     - 0.08%
+     - 0.07%
      - 44
    * - OM
      - 0.07%
      - 42
    * - IS
      - 0.07%
      - 42
@@ -500,29 +500,29 @@
      - 8
    * - CY
      - 0.01%
      - 6
    * - DZ
      - 0.01%
      - 4
-   * - AR
+   * - EE
      - 0.01%
      - 3
-   * - EE
+   * - AR
      - 0.01%
      - 3
    * - SK
      - 0.00%
      - 2
-   * - PT
+   * - RS
      - 0.00%
      - 1
-   * - RS
+   * - PT
      - 0.00%
      - 1
    * - MX
      - 0.00%
      - 1
    * - **Total**
      - **100.00%**
-     - **58,460**
+     - **59,255**
```

### Comparing `nrobo-2024.39.1/nrobo.egg-info/SOURCES.txt` & `nrobo-2024.39.2/nrobo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nrobo-2024.39.1/pyproject.toml` & `nrobo-2024.39.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [build-system]
 requires = ["setuptools >= 40.7.0",]
 build-backend = "setuptools.build_meta"
 
 # Project details
 [project]
 name = "nrobo"
-version = "2024.39.1"
+version = "2024.39.2"
 authors = [{name="Panchdev Singh Chauhan", email="erpanchdev@gmail.com"}]
 maintainers = [{name="Panchdev Singh Chauhan", email="erpanchdev@gmail.com"}]
 description = "Powerful! Yet, Easy to USE! Automated Testing Framework"
 readme = "README.rst"
 keywords = ["test automation", "test automation framework", "automated testing", "automation testing", "testing", "qa", "acceptance test", "automation"]
 classifiers = [
     "Programming Language :: Python :: 3 :: Only",
```

