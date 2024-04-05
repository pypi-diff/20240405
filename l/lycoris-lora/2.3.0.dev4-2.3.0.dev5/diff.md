# Comparing `tmp/lycoris_lora-2.3.0.dev4.tar.gz` & `tmp/lycoris_lora-2.3.0.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lycoris_lora-2.3.0.dev4.tar", last modified: Sun Mar 31 11:28:22 2024, max compression
+gzip compressed data, was "lycoris_lora-2.3.0.dev5.tar", last modified: Fri Apr  5 10:25:53 2024, max compression
```

## Comparing `lycoris_lora-2.3.0.dev4.tar` & `lycoris_lora-2.3.0.dev5.tar`

### file list

```diff
@@ -1,59 +1,57 @@
-drwxrwxrwx   0        0        0        0 2024-03-31 11:28:22.215857 lycoris_lora-2.3.0.dev4/
--rw-rw-rw-   0        0        0    11545 2023-03-09 05:37:07.000000 lycoris_lora-2.3.0.dev4/LICENSE.md
--rw-rw-rw-   0        0        0      527 2024-03-31 11:28:22.215857 lycoris_lora-2.3.0.dev4/PKG-INFO
--rw-rw-rw-   0        0        0    11988 2024-03-15 08:57:27.000000 lycoris_lora-2.3.0.dev4/README.md
-drwxrwxrwx   0        0        0        0 2024-03-31 11:28:22.184098 lycoris_lora-2.3.0.dev4/lycoris/
--rw-rw-rw-   0        0        0      550 2024-02-05 11:33:28.000000 lycoris_lora-2.3.0.dev4/lycoris/__init__.py
--rw-rw-rw-   0        0        0     2537 2023-12-02 03:39:50.000000 lycoris_lora-2.3.0.dev4/lycoris/config.py
-drwxrwxrwx   0        0        0        0 2024-03-31 11:28:22.187602 lycoris_lora-2.3.0.dev4/lycoris/hcp/
--rw-rw-rw-   0        0        0      156 2023-12-02 03:39:50.000000 lycoris_lora-2.3.0.dev4/lycoris/hcp/__init__.py
--rw-rw-rw-   0        0        0     5329 2023-12-02 03:39:50.000000 lycoris_lora-2.3.0.dev4/lycoris/hcp/base.py
--rw-rw-rw-   0        0        0     2281 2024-02-12 10:32:01.000000 lycoris_lora-2.3.0.dev4/lycoris/hcp/diag_oft.py
--rw-rw-rw-   0        0        0     3391 2024-03-04 15:01:10.000000 lycoris_lora-2.3.0.dev4/lycoris/hcp/loha.py
--rw-rw-rw-   0        0        0     5643 2024-03-04 15:01:21.000000 lycoris_lora-2.3.0.dev4/lycoris/hcp/lokr.py
-drwxrwxrwx   0        0        0        0 2024-03-31 11:28:22.191602 lycoris_lora-2.3.0.dev4/lycoris/kohya/
--rw-rw-rw-   0        0        0    31700 2024-03-16 16:01:01.000000 lycoris_lora-2.3.0.dev4/lycoris/kohya/__init__.py
--rw-rw-rw-   0        0        0    59991 2024-02-18 06:15:40.000000 lycoris_lora-2.3.0.dev4/lycoris/kohya/model_utils.py
--rw-rw-rw-   0        0        0    61070 2023-12-02 03:39:51.000000 lycoris_lora-2.3.0.dev4/lycoris/kohya/original_unet.py
--rw-rw-rw-   0        0        0    21297 2024-02-18 06:15:40.000000 lycoris_lora-2.3.0.dev4/lycoris/kohya/sdxl_model_util.py
--rw-rw-rw-   0        0        0    42690 2023-12-02 03:39:51.000000 lycoris_lora-2.3.0.dev4/lycoris/kohya/sdxl_original_unet.py
--rw-rw-rw-   0        0        0    19901 2024-03-11 06:16:36.000000 lycoris_lora-2.3.0.dev4/lycoris/kohya/test_hyperdream.py
--rw-rw-rw-   0        0        0     1514 2023-12-02 03:39:50.000000 lycoris_lora-2.3.0.dev4/lycoris/kohya/utils.py
--rw-rw-rw-   0        0        0     1053 2024-02-05 11:33:20.000000 lycoris_lora-2.3.0.dev4/lycoris/logging.py
-drwxrwxrwx   0        0        0        0 2024-03-31 11:28:22.198070 lycoris_lora-2.3.0.dev4/lycoris/modules/
--rw-rw-rw-   0        0        0     3998 2024-03-31 02:52:53.000000 lycoris_lora-2.3.0.dev4/lycoris/modules/__init__.py
--rw-rw-rw-   0        0        0     8185 2023-12-02 03:39:50.000000 lycoris_lora-2.3.0.dev4/lycoris/modules/attention.py
--rw-rw-rw-   0        0        0     1774 2024-03-11 06:14:14.000000 lycoris_lora-2.3.0.dev4/lycoris/modules/base.py
--rw-rw-rw-   0        0        0     8339 2024-03-14 17:55:35.000000 lycoris_lora-2.3.0.dev4/lycoris/modules/boft.py
--rw-rw-rw-   0        0        0     7050 2024-03-14 17:47:31.000000 lycoris_lora-2.3.0.dev4/lycoris/modules/diag_oft.py
--rw-rw-rw-   0        0        0     4395 2024-01-15 10:23:42.000000 lycoris_lora-2.3.0.dev4/lycoris/modules/dylora.py
--rw-rw-rw-   0        0        0     4622 2024-03-11 06:14:35.000000 lycoris_lora-2.3.0.dev4/lycoris/modules/full.py
--rw-rw-rw-   0        0        0    11617 2024-03-11 01:31:10.000000 lycoris_lora-2.3.0.dev4/lycoris/modules/glokr.py
--rw-rw-rw-   0        0        0     4822 2024-03-11 06:14:42.000000 lycoris_lora-2.3.0.dev4/lycoris/modules/glora.py
-drwxrwxrwx   0        0        0        0 2024-03-31 11:28:22.199814 lycoris_lora-2.3.0.dev4/lycoris/modules/hypernet/
--rw-rw-rw-   0        0        0       79 2023-12-02 03:39:50.000000 lycoris_lora-2.3.0.dev4/lycoris/modules/hypernet/__init__.py
--rw-rw-rw-   0        0        0     8302 2023-12-02 03:39:50.000000 lycoris_lora-2.3.0.dev4/lycoris/modules/hypernet/generater.py
--rw-rw-rw-   0        0        0     8339 2024-02-18 06:15:40.000000 lycoris_lora-2.3.0.dev4/lycoris/modules/hypernet/text_encoder.py
--rw-rw-rw-   0        0        0     2078 2024-03-11 06:14:46.000000 lycoris_lora-2.3.0.dev4/lycoris/modules/ia3.py
--rw-rw-rw-   0        0        0    12386 2024-03-13 16:44:41.000000 lycoris_lora-2.3.0.dev4/lycoris/modules/lilora.py
--rw-rw-rw-   0        0        0    10997 2024-03-16 18:06:05.000000 lycoris_lora-2.3.0.dev4/lycoris/modules/locon.py
--rw-rw-rw-   0        0        0    13275 2024-03-16 18:10:02.000000 lycoris_lora-2.3.0.dev4/lycoris/modules/loha.py
--rw-rw-rw-   0        0        0    18710 2024-03-16 18:10:12.000000 lycoris_lora-2.3.0.dev4/lycoris/modules/lokr.py
--rw-rw-rw-   0        0        0     3244 2024-03-14 14:32:39.000000 lycoris_lora-2.3.0.dev4/lycoris/modules/norms.py
-drwxrwxrwx   0        0        0        0 2024-03-31 11:28:22.201818 lycoris_lora-2.3.0.dev4/lycoris/utils/
--rw-rw-rw-   0        0        0    23287 2024-03-23 07:38:25.000000 lycoris_lora-2.3.0.dev4/lycoris/utils/__init__.py
--rw-rw-rw-   0        0        0      497 2024-03-13 17:06:13.000000 lycoris_lora-2.3.0.dev4/lycoris/utils/bnb.py
--rw-rw-rw-   0        0        0     1078 2023-12-02 03:39:50.000000 lycoris_lora-2.3.0.dev4/lycoris/utils/logger.py
--rw-rw-rw-   0        0        0      190 2023-12-02 03:39:50.000000 lycoris_lora-2.3.0.dev4/lycoris/utils/preset.py
--rw-rw-rw-   0        0        0      196 2024-03-16 16:01:30.000000 lycoris_lora-2.3.0.dev4/lycoris/utils/tensor_norm.py
--rw-rw-rw-   0        0        0      251 2023-12-02 03:39:50.000000 lycoris_lora-2.3.0.dev4/lycoris/utils/xformers_utils.py
--rw-rw-rw-   0        0        0    18706 2024-03-16 16:01:01.000000 lycoris_lora-2.3.0.dev4/lycoris/wrapper.py
-drwxrwxrwx   0        0        0        0 2024-03-31 11:28:22.214355 lycoris_lora-2.3.0.dev4/lycoris_lora.egg-info/
--rw-rw-rw-   0        0        0      527 2024-03-31 11:28:22.000000 lycoris_lora-2.3.0.dev4/lycoris_lora.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1290 2024-03-31 11:28:22.000000 lycoris_lora-2.3.0.dev4/lycoris_lora.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-31 11:28:22.000000 lycoris_lora-2.3.0.dev4/lycoris_lora.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-11-06 13:42:23.000000 lycoris_lora-2.3.0.dev4/lycoris_lora.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       53 2024-03-31 11:28:22.000000 lycoris_lora-2.3.0.dev4/lycoris_lora.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-03-31 11:28:22.000000 lycoris_lora-2.3.0.dev4/lycoris_lora.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-31 11:28:22.216863 lycoris_lora-2.3.0.dev4/setup.cfg
--rw-rw-rw-   0        0        0      638 2024-03-31 11:28:14.000000 lycoris_lora-2.3.0.dev4/setup.py
+drwxr-xr-x   0 kblueleaf   (501) staff       (20)        0 2024-04-05 10:25:53.340557 lycoris_lora-2.3.0.dev5/
+-rw-r--r--   0 kblueleaf   (501) staff       (20)    11344 2023-03-09 06:17:28.000000 lycoris_lora-2.3.0.dev5/LICENSE.md
+-rw-r--r--   0 kblueleaf   (501) staff       (20)      512 2024-04-05 10:25:53.340260 lycoris_lora-2.3.0.dev5/PKG-INFO
+-rw-r--r--   0 kblueleaf   (501) staff       (20)    11695 2024-04-05 10:23:00.000000 lycoris_lora-2.3.0.dev5/README.md
+drwxr-xr-x   0 kblueleaf   (501) staff       (20)        0 2024-04-05 10:25:53.332560 lycoris_lora-2.3.0.dev5/lycoris/
+-rw-r--r--   0 kblueleaf   (501) staff       (20)      527 2024-03-14 02:11:08.000000 lycoris_lora-2.3.0.dev5/lycoris/__init__.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)     2451 2023-12-11 07:32:33.000000 lycoris_lora-2.3.0.dev5/lycoris/config.py
+drwxr-xr-x   0 kblueleaf   (501) staff       (20)        0 2024-04-05 10:25:53.333382 lycoris_lora-2.3.0.dev5/lycoris/hcp/
+-rw-r--r--   0 kblueleaf   (501) staff       (20)      152 2023-12-11 07:32:33.000000 lycoris_lora-2.3.0.dev5/lycoris/hcp/__init__.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)     5176 2023-12-11 07:32:33.000000 lycoris_lora-2.3.0.dev5/lycoris/hcp/base.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)     2219 2024-03-14 02:11:08.000000 lycoris_lora-2.3.0.dev5/lycoris/hcp/diag_oft.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)     3306 2024-03-14 02:11:08.000000 lycoris_lora-2.3.0.dev5/lycoris/hcp/loha.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)     5512 2024-03-14 02:11:08.000000 lycoris_lora-2.3.0.dev5/lycoris/hcp/lokr.py
+drwxr-xr-x   0 kblueleaf   (501) staff       (20)        0 2024-04-05 10:25:53.334418 lycoris_lora-2.3.0.dev5/lycoris/kohya/
+-rw-r--r--   0 kblueleaf   (501) staff       (20)    30917 2024-04-05 10:23:01.000000 lycoris_lora-2.3.0.dev5/lycoris/kohya/__init__.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)    58358 2024-03-14 02:11:08.000000 lycoris_lora-2.3.0.dev5/lycoris/kohya/model_utils.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)    59310 2023-12-11 07:32:33.000000 lycoris_lora-2.3.0.dev5/lycoris/kohya/original_unet.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)    20716 2024-03-14 02:11:08.000000 lycoris_lora-2.3.0.dev5/lycoris/kohya/sdxl_model_util.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)    41447 2023-12-11 07:32:33.000000 lycoris_lora-2.3.0.dev5/lycoris/kohya/sdxl_original_unet.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)     1466 2023-12-11 07:32:33.000000 lycoris_lora-2.3.0.dev5/lycoris/kohya/utils.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)     1017 2024-03-14 02:11:08.000000 lycoris_lora-2.3.0.dev5/lycoris/logging.py
+drwxr-xr-x   0 kblueleaf   (501) staff       (20)        0 2024-04-05 10:25:53.337391 lycoris_lora-2.3.0.dev5/lycoris/modules/
+-rw-r--r--   0 kblueleaf   (501) staff       (20)     3865 2024-04-05 10:23:01.000000 lycoris_lora-2.3.0.dev5/lycoris/modules/__init__.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)     7926 2023-12-11 07:32:33.000000 lycoris_lora-2.3.0.dev5/lycoris/modules/attention.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)     1719 2024-03-14 02:11:08.000000 lycoris_lora-2.3.0.dev5/lycoris/modules/base.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)     8085 2024-04-05 10:23:01.000000 lycoris_lora-2.3.0.dev5/lycoris/modules/boft.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)     6832 2024-04-05 10:23:01.000000 lycoris_lora-2.3.0.dev5/lycoris/modules/diag_oft.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)     4263 2024-03-14 02:11:08.000000 lycoris_lora-2.3.0.dev5/lycoris/modules/dylora.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)     4489 2024-03-14 02:11:08.000000 lycoris_lora-2.3.0.dev5/lycoris/modules/full.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)    11486 2024-04-05 10:23:01.000000 lycoris_lora-2.3.0.dev5/lycoris/modules/glokr.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)     4846 2024-04-05 10:23:01.000000 lycoris_lora-2.3.0.dev5/lycoris/modules/glora.py
+drwxr-xr-x   0 kblueleaf   (501) staff       (20)        0 2024-04-05 10:25:53.337865 lycoris_lora-2.3.0.dev5/lycoris/modules/hypernet/
+-rw-r--r--   0 kblueleaf   (501) staff       (20)       78 2023-12-11 07:32:33.000000 lycoris_lora-2.3.0.dev5/lycoris/modules/hypernet/__init__.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)     8079 2023-12-11 07:32:33.000000 lycoris_lora-2.3.0.dev5/lycoris/modules/hypernet/generater.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)     8073 2024-03-14 02:11:08.000000 lycoris_lora-2.3.0.dev5/lycoris/modules/hypernet/text_encoder.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)     2011 2024-03-14 02:11:08.000000 lycoris_lora-2.3.0.dev5/lycoris/modules/ia3.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)    12332 2024-04-05 10:25:13.000000 lycoris_lora-2.3.0.dev5/lycoris/modules/lilora.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)    10996 2024-04-05 10:25:02.000000 lycoris_lora-2.3.0.dev5/lycoris/modules/locon.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)    13226 2024-04-05 10:24:56.000000 lycoris_lora-2.3.0.dev5/lycoris/modules/loha.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)    18504 2024-04-05 10:24:45.000000 lycoris_lora-2.3.0.dev5/lycoris/modules/lokr.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)     3152 2024-03-14 02:11:08.000000 lycoris_lora-2.3.0.dev5/lycoris/modules/norms.py
+drwxr-xr-x   0 kblueleaf   (501) staff       (20)        0 2024-04-05 10:25:53.338582 lycoris_lora-2.3.0.dev5/lycoris/utils/
+-rw-r--r--   0 kblueleaf   (501) staff       (20)    22647 2024-04-05 10:23:01.000000 lycoris_lora-2.3.0.dev5/lycoris/utils/__init__.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)      471 2024-03-14 02:11:08.000000 lycoris_lora-2.3.0.dev5/lycoris/utils/bnb.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)     1043 2023-12-11 07:32:33.000000 lycoris_lora-2.3.0.dev5/lycoris/utils/logger.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)      181 2023-12-11 07:32:33.000000 lycoris_lora-2.3.0.dev5/lycoris/utils/preset.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)      238 2023-12-11 07:32:33.000000 lycoris_lora-2.3.0.dev5/lycoris/utils/xformers_utils.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)    18172 2024-04-05 10:23:01.000000 lycoris_lora-2.3.0.dev5/lycoris/wrapper.py
+drwxr-xr-x   0 kblueleaf   (501) staff       (20)        0 2024-04-05 10:25:53.339921 lycoris_lora-2.3.0.dev5/lycoris_lora.egg-info/
+-rw-r--r--   0 kblueleaf   (501) staff       (20)      512 2024-04-05 10:25:53.000000 lycoris_lora-2.3.0.dev5/lycoris_lora.egg-info/PKG-INFO
+-rw-r--r--   0 kblueleaf   (501) staff       (20)     1228 2024-04-05 10:25:53.000000 lycoris_lora-2.3.0.dev5/lycoris_lora.egg-info/SOURCES.txt
+-rw-r--r--   0 kblueleaf   (501) staff       (20)        1 2024-04-05 10:25:53.000000 lycoris_lora-2.3.0.dev5/lycoris_lora.egg-info/dependency_links.txt
+-rw-r--r--   0 kblueleaf   (501) staff       (20)        1 2023-03-09 06:17:38.000000 lycoris_lora-2.3.0.dev5/lycoris_lora.egg-info/not-zip-safe
+-rw-r--r--   0 kblueleaf   (501) staff       (20)       53 2024-04-05 10:25:53.000000 lycoris_lora-2.3.0.dev5/lycoris_lora.egg-info/requires.txt
+-rw-r--r--   0 kblueleaf   (501) staff       (20)        8 2024-04-05 10:25:53.000000 lycoris_lora-2.3.0.dev5/lycoris_lora.egg-info/top_level.txt
+-rw-r--r--   0 kblueleaf   (501) staff       (20)       38 2024-04-05 10:25:53.340611 lycoris_lora-2.3.0.dev5/setup.cfg
+-rw-r--r--   0 kblueleaf   (501) staff       (20)      616 2024-04-05 10:25:46.000000 lycoris_lora-2.3.0.dev5/setup.py
```

### Comparing `lycoris_lora-2.3.0.dev4/LICENSE.md` & `lycoris_lora-2.3.0.dev5/LICENSE.md`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright 2023 KohakuBlueLeaf
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright 2023 KohakuBlueLeaf
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `lycoris_lora-2.3.0.dev4/PKG-INFO` & `lycoris_lora-2.3.0.dev5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1
-Name: lycoris_lora
-Version: 2.3.0.dev4
-Summary: Lora beYond Conventional methods, Other Rank adaptation Implementations for Stable diffusion
-Home-page: https://github.com/KohakuBlueleaf/LyCORIS
-Author: Shih-Ying Yeh(KohakuBlueLeaf), Yu-Guan Hsieh, Zhidong Gao
-Author-email: apolloyeh0123@gmail.com
-Requires-Python: >=3.10
-License-File: LICENSE.md
-Requires-Dist: torch
-Requires-Dist: safetensors
-Requires-Dist: diffusers
-Requires-Dist: transformers
-Requires-Dist: einops
-Requires-Dist: toml
+Metadata-Version: 2.1
+Name: lycoris_lora
+Version: 2.3.0.dev5
+Summary: Lora beYond Conventional methods, Other Rank adaptation Implementations for Stable diffusion
+Home-page: https://github.com/KohakuBlueleaf/LyCORIS
+Author: Shih-Ying Yeh(KohakuBlueLeaf), Yu-Guan Hsieh, Zhidong Gao
+Author-email: apolloyeh0123@gmail.com
+Requires-Python: >=3.10
+License-File: LICENSE.md
+Requires-Dist: torch
+Requires-Dist: safetensors
+Requires-Dist: diffusers
+Requires-Dist: transformers
+Requires-Dist: einops
+Requires-Dist: toml
```

### Comparing `lycoris_lora-2.3.0.dev4/README.md` & `lycoris_lora-2.3.0.dev5/README.md`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,293 +1,293 @@
-# LyCORIS - Lora beYond Conventional methods, Other Rank adaptation Implementations for Stable diffusion.
-
-![banner image](docs/images/banner.png)
-
-A project that implements different parameter-efficient fine-tuning algorithms for Stable Diffusion.
-
-This project originated from LoCon (see archive branch).
-
-**If you are interested in discussing more details, you can join [our Discord server](https://discord.gg/VtTFKrj9gJ)**
-
-[![Discord!](https://i.imgur.com/A8tOvFS.jpg)](https://discord.gg/VtTFKrj9gJ)
-
-**If you want to check more in-depth experiment results and discussions for LyCORIS, you can check our [paper](https://arxiv.org/abs/2309.14859)**
-
-## Algorithm Overview
-
-LyCORIS currently contains LoRA (LoCon), LoHa, LoKr, (IA)^3, DyLoRA, Native fine-tuning (aka dreambooth).
-GLoRA and GLoKr are coming soon.
-Please check [List of Implemented Algorithms](docs/Algo-List.md) and [Guidelines](docs/Guidelines.md) for more details.
-
-A simple comparison of some of these methods are provided below (to be taken with a grain of salt)
-
-|                       | Full | LoRA | LoHa | LoKr low factor | LoKr high factor |
-| --------------------- | ---- | ---- | ---- | --------------- | ---------------- |
-| Fidelity              | ★   | ●   | ▲   | ◉              | ▲               |
-| Flexibility$^*$     | ★   | ●   | ◉   | ▲              | ●$^†$        |
-| Diversity             | ▲   | ◉   | ★   | ●              | ★               |
-| Size                  | ▲   | ●   | ●   | ●              | ★               |
-| Training Speed Linear | ★   | ●   | ●   | ★              | ★               |
-| Training Speed Conv   | ●   | ★   | ▲   | ●              | ●               |
-
-★ > ◉ > ● > ▲
-[> means better and smaller size is better]
-
-$^*$ Flexibility means anything related to generating images not similar to those in the training set, and combination of multiple concepts, whether they are trained together or not
-$^†$ It may become more difficult to switch base model or combine multiple concepts in this situation
-
-## Usage
-
-### Image Generation
-
-#### [a1111/sd-webui](https://github.com/AUTOMATIC1111/stable-diffusion-webui)
-
-After sd-webui 1.5.0, LyCORIS models are officially supported by the built-in LoRA system. You can put them in either `models/Lora` or `models/LyCORIS` and use the default syntax `<lora:filename:multiplier>` to trigger it.
-
-When we add new model types, we will always make sure they can be used with the newest version of sd-webui.
-
-As for sd-webui with version < 1.5.0 or sd-webui-forge, please check this [extension](https://github.com/KohakuBlueleaf/a1111-sd-webui-lycoris).
-
-#### Others
-
-As far as we are aware, LyCORIS models are also supported in the following interfaces / online generation services (please help us complete the list!)
-
-- [ComfyUI](https://github.com/comfyanonymous/ComfyUI)
-- [InvokeAI](https://github.com/invoke-ai/InvokeAI)
-- [CivitAI](https://civitai.com/)
-- [Tensor.Art](https://tensor.art/)
-
-However, newer model types may not always be supported. If you encounter this issue, consider requesting the developers of the corresponding interface or website to include support for the new type.
-
-### Training
-
-There are three different ways to train LyCORIS models.
-
-- With [kohya-ss/sd-scripts](https://github.com/kohya-ss/sd-scripts) (see a list of compatible graphical interfaces and colabs at the end of the section)
-- With [HCP-Diffusion](https://github.com/IrisRainbowNeko/HCP-Diffusion)
-- With your own script by using LyCORIS as standalone wrappers for **ANY** pytorch modules.
-
-In any case, please install this package in the corresponding virtual environment. You can either install it
-
-- through pip
-
-  ```bash
-  pip install lycoris_lora
-  ```
-- or from source
-
-  ```bash
-  git clone https://github.com/KohakuBlueleaf/LyCORIS
-  cd LyCORIS
-  pip install .
-  ```
-
-A detilaed description of the network arguments is provided in [docs/Network-Args.md](docs/Network-Args.md).
-
-#### kohya script
-
-You can use this package's kohya module to run kohya's training script to train lycoris module for SD models
-
-- with command line arguments
-
-  ```bash
-  accelerate launch train_network.py \
-    --network_module lycoris.kohya \
-    --network_dim "DIM_FOR_LINEAR" --network_alpha "ALPHA_FOR_LINEAR"\
-    --network_args "conv_dim=DIM_FOR_CONV" "conv_alpha=ALPHA_FOR_CONV" \
-    "dropout=DROPOUT_RATE" "algo=locon" \
-  ```
-- with `toml` files
-
-  ```bash
-  accelerate launch train_network.py \
-    --config_file example_configs/training_configs/kohya/loha_config.toml \
-    --dataset_config example_configs/training_configs/kohya/dataset_config.toml
-  ```
-
-  For your convenience, some example `toml` files for kohya LyCORIS training are provided in [example/training_configs/kohya](example_configs/training_configs/kohya).
-
-#### HCP-Diffusion
-
-You can use this package's hcp module to run HCP-Diffusion's training script to train lycoris module for SD models
-
-```bash
-accelerate launch -m hcpdiff.train_ac_single \
-  --cfg example_configs/training_configs/hcp/hcp_diag_oft.yaml
-```
-
-For your convenience, some example `yaml` files for HCP LyCORIS training are provided in [example/training_configs/hcp](example_configs/training_configs/hcp).
-
-For the moment being the outputs of HCP-Diffusion are not directly compatible with a1111/sdwebui.
-You can perform conversion with [tools/batch_hcp_convert.py](tools/batch_hcp_convert.py).
-
-In the case of pivotal tuning, [tools/batch_bundle_convert.py](tools/batch_bundle_convert.py) can be further used to convert to and from bundle formats.
-Check [docs/Conversion-scripts.md](docs/Conversion-scripts.md) for more information.
-
-#### As standalone wrappers
-
-See [standalone_example.py](standalone_example.py) for full example.
-
-Import `create_lycoris` and `LycorisNetwork` from `lycoris` library, put your preset to `LycorisNetwork` and then use `create_lycoris` to create LyCORIS module for your pytorch module.
-
-For example:
-
-```py
-from lycoris import create_lycoris, LycorisNetwork
-
-LycorisNetwork.apply_preset(
-    {"target_name": [".*attn.*"]}
-)
-lycoris_net = create_lycoris(
-    your_model, 
-    1.0, 
-    linear_dim=16, 
-    linear_alpha=2.0, 
-    algo="lokr"
-)
-lycoris_net.apply_to()
-
-# after apply_to(), your_model() will run with LyCORIS net
-lycoris_param = lycoris_net.parameters()
-forward_with_lyco = your_model(x)
-```
-
-You can check my [HakuPhi](https://github.com/KohakuBlueleaf/HakuPhi) project to see how I utilize LyCORIS to finetune the Phi-1.5 models.
-
-#### Bitsandbytes support
-
-See [bnb_example.py](bnb_example.py) for example. Basically as same as standalone wrapper.
-
-#### Graphical interfaces and Colabs (via kohya trainer)
-
-You can also train LyCORIS with the following graphical interfaces
-
-* [bmaltais/kohya_ss](https://github.com/bmaltais/kohya_ss)
-* [derrian-distro/LoRA_Easy_Training_Scripts](https://github.com/derrian-distro/LoRA_Easy_Training_Scripts)
-* [Akegarasu/lora-scripts](https://github.com/Akegarasu/lora-scripts)
-
-and colabs (please help us complete the list!)
-
-* [hollowstrawberry/kohya-colab](https://github.com/hollowstrawberry/kohya-colab)
-* [Linaqruf/kohya-trainer](https://github.com/Linaqruf/kohya-trainer)
-
-However, they are not guaranteed to be up-to-date. In particular, newer types may not be supported. Consider requesting the developers for support or simply use the original kohya script in this case.
-
-## Utilities
-
-### Extract LoCon
-
-You can extract LoCon from a dreambooth model with its base model.
-
-```bash
-python3 extract_locon.py <settings> <base_model> <db_model> <output>
-```
-
-Use --help to get more info
-
-```
-$ python3 extract_locon.py --help
-usage: extract_locon.py [-h] [--is_v2] [--is_sdxl] [--device DEVICE] [--mode MODE] [--safetensors] [--linear_dim LINEAR_DIM]
-                        [--conv_dim CONV_DIM] [--linear_threshold LINEAR_THRESHOLD] [--conv_threshold CONV_THRESHOLD]
-                        [--linear_ratio LINEAR_RATIO] [--conv_ratio CONV_RATIO] [--linear_quantile LINEAR_QUANTILE]
-                        [--conv_quantile CONV_QUANTILE] [--use_sparse_bias] [--sparsity SPARSITY] [--disable_cp]
-                        base_model db_model output_name
-```
-
-### Merge LyCORIS back to model
-
-You can merge your LyCORIS model back to your checkpoint (base model).
-
-```bash
-python3 merge.py <settings> <base_model> <lycoris_model> <output>
-```
-
-Use --help to get more info
-
-```
-$ python3 merge.py --help
-usage: merge.py [-h] [--is_v2] [--is_sdxl] [--device DEVICE] [--dtype DTYPE] [--weight WEIGHT] base_model lycoris_model output_name
-```
-
-### Conversion of LoRA, LyCORIS and full models between HCP and sd-webui format
-
-This script allows you to use the LyCORIS models trained with HCP-Diffusion in sd-webui.
-
-```bash
-python3 batch_hcp_convert.py \
-  --network_path /path/to/ckpts \
-  --dst_dir /path/to/stable-diffusion-webui/models/Lora \
-  --output_prefix something \
-  --auto_scale_alpha --to_webui
-```
-
-See [docs/Conversion-scripts.md](docs/Conversion-scripts.md) for more information.
-
-### Conversion from and to bundle format
-
-This script is particularly useful in the case of pivotal tuning.
-
-```bash
-python3 batch_bundle_convert.py \
-  --network_path /path/to/sd-webui-ssd/models/Lora  \
-  --emb_path /path/to/ckpts \
-  --dst_dir /path/to/sd-webui-ssd/models/Lora/bundle \
-  --to_bundle --verbose 2 
-```
-
-See [docs/Conversion-scripts.md](docs/Conversion-scripts.md) for more information.
-
-## Change Log
-
-For full log, please see [Change.md](Change.md)
-
-## 2024/03/15 update to 2.2.0 - QLyCORIS and DoRA
-
-#### New Algo
-
-* DoRA
-  * Ref: [DoRA: Weight-Decomposed Low-Rank Adaptation](https://github.com/KohakuBlueleaf/LyCORIS)
-* Weight decompose for LoHa and LoKr. (A.K.A DoHa/DoKr)
-  * DoRA/DoHa/DoKr will require smaller Learning rate!
-
-#### New Features
-
-* Support "bypass" (a.k.a. adapter) mode for LoHa/LoKr/OFT/BOFT
-  * LoHa will require 2xFLOPs since we rebuild full diff weight and then do one more forward.
-  * LoKr, OFT, BOFT should be more efficient than LoHa in bypass mode.
-* Support [bnb 8bit/4bit Linear layer](https://github.com/TimDettmers/bitsandbytes) (a.k.a. QLyCORIS) with LoHa/LoKr/OFT/BOFT.
-  * This will force module to enable bypass mode.
-
-#### Fixes, slight changes
-
-* Refine some details about code quality. Based on the report from GitRoll. (Thx you gitroll!)
-* Remove redundant calculation in BOFT
-* rank_dropout has been removed from OFT/BOFT temporarily untill we ensure how to apply it.
-* Fix bugs in lokr when `lokr_w1_a` not exist.
-* Fix bugs in conversion scritps.
-
-## Todo list
-
-- [X] Module and Document for using LyCORIS in any other model, Not only SD.
-- [X] Proposition3 in [FedPara](https://arxiv.org/abs/2108.06098)
-  * also need custom backward to save the vram
-- [ ] Low rank + sparse representation
-  - [X] For extraction
-  - [ ] For training
-- [ ] Support more operation, not only linear and conv2d.
-- [X] Configure varying ranks or dimensions for specific modules as needed.
-- [ ] Automatically selecting an algorithm based on the specific rank requirement.
-- [ ] Explore other low-rank representations or parameter-efficient methods to fine-tune either the entire model or specific parts of it.
-- [ ] More experiments for different task, not only diffusion models.
-
-## Citation
-
-```bibtex
-@inproceedings{
-  yeh2024navigating,
-  title={Navigating Text-To-Image Customization: From Ly{CORIS} Fine-Tuning to Model Evaluation},
-  author={SHIH-YING YEH and Yu-Guan Hsieh and Zhidong Gao and Bernard B W Yang and Giyeong Oh and Yanmin Gong},
-  booktitle={The Twelfth International Conference on Learning Representations},
-  year={2024},
-  url={https://openreview.net/forum?id=wfzXa8e783}
-}
-```
+# LyCORIS - Lora beYond Conventional methods, Other Rank adaptation Implementations for Stable diffusion.
+
+![banner image](docs/images/banner.png)
+
+A project that implements different parameter-efficient fine-tuning algorithms for Stable Diffusion.
+
+This project originated from LoCon (see archive branch).
+
+**If you are interested in discussing more details, you can join [our Discord server](https://discord.gg/VtTFKrj9gJ)**
+
+[![Discord!](https://i.imgur.com/A8tOvFS.jpg)](https://discord.gg/VtTFKrj9gJ)
+
+**If you want to check more in-depth experiment results and discussions for LyCORIS, you can check our [paper](https://arxiv.org/abs/2309.14859)**
+
+## Algorithm Overview
+
+LyCORIS currently contains LoRA (LoCon), LoHa, LoKr, (IA)^3, DyLoRA, Native fine-tuning (aka dreambooth).
+GLoRA and GLoKr are coming soon.
+Please check [List of Implemented Algorithms](docs/Algo-List.md) and [Guidelines](docs/Guidelines.md) for more details.
+
+A simple comparison of some of these methods are provided below (to be taken with a grain of salt)
+
+|                       | Full | LoRA | LoHa | LoKr low factor | LoKr high factor |
+| --------------------- | ---- | ---- | ---- | --------------- | ---------------- |
+| Fidelity              | ★   | ●   | ▲   | ◉              | ▲               |
+| Flexibility$^*$     | ★   | ●   | ◉   | ▲              | ●$^†$        |
+| Diversity             | ▲   | ◉   | ★   | ●              | ★               |
+| Size                  | ▲   | ●   | ●   | ●              | ★               |
+| Training Speed Linear | ★   | ●   | ●   | ★              | ★               |
+| Training Speed Conv   | ●   | ★   | ▲   | ●              | ●               |
+
+★ > ◉ > ● > ▲
+[> means better and smaller size is better]
+
+$^*$ Flexibility means anything related to generating images not similar to those in the training set, and combination of multiple concepts, whether they are trained together or not
+$^†$ It may become more difficult to switch base model or combine multiple concepts in this situation
+
+## Usage
+
+### Image Generation
+
+#### [a1111/sd-webui](https://github.com/AUTOMATIC1111/stable-diffusion-webui)
+
+After sd-webui 1.5.0, LyCORIS models are officially supported by the built-in LoRA system. You can put them in either `models/Lora` or `models/LyCORIS` and use the default syntax `<lora:filename:multiplier>` to trigger it.
+
+When we add new model types, we will always make sure they can be used with the newest version of sd-webui.
+
+As for sd-webui with version < 1.5.0 or sd-webui-forge, please check this [extension](https://github.com/KohakuBlueleaf/a1111-sd-webui-lycoris).
+
+#### Others
+
+As far as we are aware, LyCORIS models are also supported in the following interfaces / online generation services (please help us complete the list!)
+
+- [ComfyUI](https://github.com/comfyanonymous/ComfyUI)
+- [InvokeAI](https://github.com/invoke-ai/InvokeAI)
+- [CivitAI](https://civitai.com/)
+- [Tensor.Art](https://tensor.art/)
+
+However, newer model types may not always be supported. If you encounter this issue, consider requesting the developers of the corresponding interface or website to include support for the new type.
+
+### Training
+
+There are three different ways to train LyCORIS models.
+
+- With [kohya-ss/sd-scripts](https://github.com/kohya-ss/sd-scripts) (see a list of compatible graphical interfaces and colabs at the end of the section)
+- With [HCP-Diffusion](https://github.com/IrisRainbowNeko/HCP-Diffusion)
+- With your own script by using LyCORIS as standalone wrappers for **ANY** pytorch modules.
+
+In any case, please install this package in the corresponding virtual environment. You can either install it
+
+- through pip
+
+  ```bash
+  pip install lycoris_lora
+  ```
+- or from source
+
+  ```bash
+  git clone https://github.com/KohakuBlueleaf/LyCORIS
+  cd LyCORIS
+  pip install .
+  ```
+
+A detilaed description of the network arguments is provided in [docs/Network-Args.md](docs/Network-Args.md).
+
+#### kohya script
+
+You can use this package's kohya module to run kohya's training script to train lycoris module for SD models
+
+- with command line arguments
+
+  ```bash
+  accelerate launch train_network.py \
+    --network_module lycoris.kohya \
+    --network_dim "DIM_FOR_LINEAR" --network_alpha "ALPHA_FOR_LINEAR"\
+    --network_args "conv_dim=DIM_FOR_CONV" "conv_alpha=ALPHA_FOR_CONV" \
+    "dropout=DROPOUT_RATE" "algo=locon" \
+  ```
+- with `toml` files
+
+  ```bash
+  accelerate launch train_network.py \
+    --config_file example_configs/training_configs/kohya/loha_config.toml \
+    --dataset_config example_configs/training_configs/kohya/dataset_config.toml
+  ```
+
+  For your convenience, some example `toml` files for kohya LyCORIS training are provided in [example/training_configs/kohya](example_configs/training_configs/kohya).
+
+#### HCP-Diffusion
+
+You can use this package's hcp module to run HCP-Diffusion's training script to train lycoris module for SD models
+
+```bash
+accelerate launch -m hcpdiff.train_ac_single \
+  --cfg example_configs/training_configs/hcp/hcp_diag_oft.yaml
+```
+
+For your convenience, some example `yaml` files for HCP LyCORIS training are provided in [example/training_configs/hcp](example_configs/training_configs/hcp).
+
+For the moment being the outputs of HCP-Diffusion are not directly compatible with a1111/sdwebui.
+You can perform conversion with [tools/batch_hcp_convert.py](tools/batch_hcp_convert.py).
+
+In the case of pivotal tuning, [tools/batch_bundle_convert.py](tools/batch_bundle_convert.py) can be further used to convert to and from bundle formats.
+Check [docs/Conversion-scripts.md](docs/Conversion-scripts.md) for more information.
+
+#### As standalone wrappers
+
+See [standalone_example.py](standalone_example.py) for full example.
+
+Import `create_lycoris` and `LycorisNetwork` from `lycoris` library, put your preset to `LycorisNetwork` and then use `create_lycoris` to create LyCORIS module for your pytorch module.
+
+For example:
+
+```py
+from lycoris import create_lycoris, LycorisNetwork
+
+LycorisNetwork.apply_preset(
+    {"target_name": [".*attn.*"]}
+)
+lycoris_net = create_lycoris(
+    your_model, 
+    1.0, 
+    linear_dim=16, 
+    linear_alpha=2.0, 
+    algo="lokr"
+)
+lycoris_net.apply_to()
+
+# after apply_to(), your_model() will run with LyCORIS net
+lycoris_param = lycoris_net.parameters()
+forward_with_lyco = your_model(x)
+```
+
+You can check my [HakuPhi](https://github.com/KohakuBlueleaf/HakuPhi) project to see how I utilize LyCORIS to finetune the Phi-1.5 models.
+
+#### Bitsandbytes support
+
+See [bnb_example.py](bnb_example.py) for example. Basically as same as standalone wrapper.
+
+#### Graphical interfaces and Colabs (via kohya trainer)
+
+You can also train LyCORIS with the following graphical interfaces
+
+* [bmaltais/kohya_ss](https://github.com/bmaltais/kohya_ss)
+* [derrian-distro/LoRA_Easy_Training_Scripts](https://github.com/derrian-distro/LoRA_Easy_Training_Scripts)
+* [Akegarasu/lora-scripts](https://github.com/Akegarasu/lora-scripts)
+
+and colabs (please help us complete the list!)
+
+* [hollowstrawberry/kohya-colab](https://github.com/hollowstrawberry/kohya-colab)
+* [Linaqruf/kohya-trainer](https://github.com/Linaqruf/kohya-trainer)
+
+However, they are not guaranteed to be up-to-date. In particular, newer types may not be supported. Consider requesting the developers for support or simply use the original kohya script in this case.
+
+## Utilities
+
+### Extract LoCon
+
+You can extract LoCon from a dreambooth model with its base model.
+
+```bash
+python3 extract_locon.py <settings> <base_model> <db_model> <output>
+```
+
+Use --help to get more info
+
+```
+$ python3 extract_locon.py --help
+usage: extract_locon.py [-h] [--is_v2] [--is_sdxl] [--device DEVICE] [--mode MODE] [--safetensors] [--linear_dim LINEAR_DIM]
+                        [--conv_dim CONV_DIM] [--linear_threshold LINEAR_THRESHOLD] [--conv_threshold CONV_THRESHOLD]
+                        [--linear_ratio LINEAR_RATIO] [--conv_ratio CONV_RATIO] [--linear_quantile LINEAR_QUANTILE]
+                        [--conv_quantile CONV_QUANTILE] [--use_sparse_bias] [--sparsity SPARSITY] [--disable_cp]
+                        base_model db_model output_name
+```
+
+### Merge LyCORIS back to model
+
+You can merge your LyCORIS model back to your checkpoint (base model).
+
+```bash
+python3 merge.py <settings> <base_model> <lycoris_model> <output>
+```
+
+Use --help to get more info
+
+```
+$ python3 merge.py --help
+usage: merge.py [-h] [--is_v2] [--is_sdxl] [--device DEVICE] [--dtype DTYPE] [--weight WEIGHT] base_model lycoris_model output_name
+```
+
+### Conversion of LoRA, LyCORIS and full models between HCP and sd-webui format
+
+This script allows you to use the LyCORIS models trained with HCP-Diffusion in sd-webui.
+
+```bash
+python3 batch_hcp_convert.py \
+  --network_path /path/to/ckpts \
+  --dst_dir /path/to/stable-diffusion-webui/models/Lora \
+  --output_prefix something \
+  --auto_scale_alpha --to_webui
+```
+
+See [docs/Conversion-scripts.md](docs/Conversion-scripts.md) for more information.
+
+### Conversion from and to bundle format
+
+This script is particularly useful in the case of pivotal tuning.
+
+```bash
+python3 batch_bundle_convert.py \
+  --network_path /path/to/sd-webui-ssd/models/Lora  \
+  --emb_path /path/to/ckpts \
+  --dst_dir /path/to/sd-webui-ssd/models/Lora/bundle \
+  --to_bundle --verbose 2 
+```
+
+See [docs/Conversion-scripts.md](docs/Conversion-scripts.md) for more information.
+
+## Change Log
+
+For full log, please see [Change.md](Change.md)
+
+## 2024/03/15 update to 2.2.0 - QLyCORIS and DoRA
+
+#### New Algo
+
+* DoRA
+  * Ref: [DoRA: Weight-Decomposed Low-Rank Adaptation](https://github.com/KohakuBlueleaf/LyCORIS)
+* Weight decompose for LoHa and LoKr. (A.K.A DoHa/DoKr)
+  * DoRA/DoHa/DoKr will require smaller Learning rate!
+
+#### New Features
+
+* Support "bypass" (a.k.a. adapter) mode for LoHa/LoKr/OFT/BOFT
+  * LoHa will require 2xFLOPs since we rebuild full diff weight and then do one more forward.
+  * LoKr, OFT, BOFT should be more efficient than LoHa in bypass mode.
+* Support [bnb 8bit/4bit Linear layer](https://github.com/TimDettmers/bitsandbytes) (a.k.a. QLyCORIS) with LoHa/LoKr/OFT/BOFT.
+  * This will force module to enable bypass mode.
+
+#### Fixes, slight changes
+
+* Refine some details about code quality. Based on the report from GitRoll. (Thx you gitroll!)
+* Remove redundant calculation in BOFT
+* rank_dropout has been removed from OFT/BOFT temporarily untill we ensure how to apply it.
+* Fix bugs in lokr when `lokr_w1_a` not exist.
+* Fix bugs in conversion scritps.
+
+## Todo list
+
+- [X] Module and Document for using LyCORIS in any other model, Not only SD.
+- [X] Proposition3 in [FedPara](https://arxiv.org/abs/2108.06098)
+  * also need custom backward to save the vram
+- [ ] Low rank + sparse representation
+  - [X] For extraction
+  - [ ] For training
+- [ ] Support more operation, not only linear and conv2d.
+- [X] Configure varying ranks or dimensions for specific modules as needed.
+- [ ] Automatically selecting an algorithm based on the specific rank requirement.
+- [ ] Explore other low-rank representations or parameter-efficient methods to fine-tune either the entire model or specific parts of it.
+- [ ] More experiments for different task, not only diffusion models.
+
+## Citation
+
+```bibtex
+@inproceedings{
+  yeh2024navigating,
+  title={Navigating Text-To-Image Customization: From Ly{CORIS} Fine-Tuning to Model Evaluation},
+  author={SHIH-YING YEH and Yu-Guan Hsieh and Zhidong Gao and Bernard B W Yang and Giyeong Oh and Yanmin Gong},
+  booktitle={The Twelfth International Conference on Learning Representations},
+  year={2024},
+  url={https://openreview.net/forum?id=wfzXa8e783}
+}
+```
```

### Comparing `lycoris_lora-2.3.0.dev4/lycoris/hcp/diag_oft.py` & `lycoris_lora-2.3.0.dev5/lycoris/hcp/diag_oft.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-import torch
-import torch.nn as nn
-import torch.nn.functional as F
-
-from einops import rearrange
-
-from .base import LycorisPluginBlock
-from ..modules.lokr import factorization
-from ..modules.diag_oft import DiagOFTModule, log_oft_factorize
-
-
-class DiagOFTBlock(DiagOFTModule, LycorisPluginBlock):
-    wrapable_classes = (nn.Conv2d, nn.Linear)
-
-    def __init__(self, *args, constrain=0, rescaled=False, **kwargs):
-        LycorisPluginBlock.__init__(self, *args, **kwargs)
-
-        out_dim = self.shape[0]
-        self.block_size, self.block_num = factorization(out_dim, self.dim)
-        self.scale = 1.0
-        # block_num > block_size
-        self.rescaled = rescaled
-        self.constrain = constrain * out_dim
-        self.oft_blocks = nn.Parameter(
-            torch.zeros(self.block_num, self.block_size, self.block_size)
-        )
-        if rescaled:
-            self.rescale = nn.Parameter(torch.ones(out_dim))
-        log_oft_factorize(
-            dim=out_dim,
-            factor=self.dim,
-            num=self.block_num,
-            bdim=self.block_size,
-        )
-
-    def forward(self, orig_weight, org_bias, new_weight, new_bias, *args, **kwargs):
-        device = self.oft_blocks.device
-        if self.rank_dropout and self.training:
-            drop = (torch.rand(self.oft_blocks, device=device) < self.rank_dropout).to(
-                self.oft_blocks.dtype
-            )
-            if self.rank_dropout_scale:
-                drop /= drop.mean()
-        else:
-            drop = 1
-
-        r = self.get_r()
-        org_weight = orig_weight.to(device, dtype=r.dtype)
-        org_weight = rearrange(
-            org_weight, "(k n) ... -> k n ...", k=self.block_num, n=self.block_size
-        )
-        # Init R=0, so add I on it to ensure the output of step0 is original model output
-        weight = torch.einsum(
-            "k n m, k n ... -> k m ...",
-            r * self.scale + (1 - self.scale) * self.I,
-            org_weight,
-        )
-        weight = rearrange(weight, "k m ... -> (k m) ...")
-        if self.rescaled:
-            weight = self.rescale.to(weight) * weight
-        # disable update weight for replace the weight directly
-        return weight, None, None, False, False
+import torch
+import torch.nn as nn
+import torch.nn.functional as F
+
+from einops import rearrange
+
+from .base import LycorisPluginBlock
+from ..modules.lokr import factorization
+from ..modules.diag_oft import DiagOFTModule, log_oft_factorize
+
+
+class DiagOFTBlock(DiagOFTModule, LycorisPluginBlock):
+    wrapable_classes = (nn.Conv2d, nn.Linear)
+
+    def __init__(self, *args, constrain=0, rescaled=False, **kwargs):
+        LycorisPluginBlock.__init__(self, *args, **kwargs)
+
+        out_dim = self.shape[0]
+        self.block_size, self.block_num = factorization(out_dim, self.dim)
+        self.scale = 1.0
+        # block_num > block_size
+        self.rescaled = rescaled
+        self.constrain = constrain * out_dim
+        self.oft_blocks = nn.Parameter(
+            torch.zeros(self.block_num, self.block_size, self.block_size)
+        )
+        if rescaled:
+            self.rescale = nn.Parameter(torch.ones(out_dim))
+        log_oft_factorize(
+            dim=out_dim,
+            factor=self.dim,
+            num=self.block_num,
+            bdim=self.block_size,
+        )
+
+    def forward(self, orig_weight, org_bias, new_weight, new_bias, *args, **kwargs):
+        device = self.oft_blocks.device
+        if self.rank_dropout and self.training:
+            drop = (torch.rand(self.oft_blocks, device=device) < self.rank_dropout).to(
+                self.oft_blocks.dtype
+            )
+            if self.rank_dropout_scale:
+                drop /= drop.mean()
+        else:
+            drop = 1
+
+        r = self.get_r()
+        org_weight = orig_weight.to(device, dtype=r.dtype)
+        org_weight = rearrange(
+            org_weight, "(k n) ... -> k n ...", k=self.block_num, n=self.block_size
+        )
+        # Init R=0, so add I on it to ensure the output of step0 is original model output
+        weight = torch.einsum(
+            "k n m, k n ... -> k m ...",
+            r * self.scale + (1 - self.scale) * self.I,
+            org_weight,
+        )
+        weight = rearrange(weight, "k m ... -> (k m) ...")
+        if self.rescaled:
+            weight = self.rescale.to(weight) * weight
+        # disable update weight for replace the weight directly
+        return weight, None, None, False, False
```

### Comparing `lycoris_lora-2.3.0.dev4/lycoris/hcp/loha.py` & `lycoris_lora-2.3.0.dev5/lycoris/hcp/loha.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,85 +1,85 @@
-import torch
-import torch.nn as nn
-import torch.nn.functional as F
-
-from .base import LycorisPluginBlock
-from ..modules.loha import make_weight, make_weight_tucker
-
-
-class LohaBlock(LycorisPluginBlock):
-    wrapable_classes = (nn.Conv2d, nn.Linear)
-
-    def __init__(self, *args, **kwargs):
-        super(LohaBlock, self).__init__(*args, **kwargs)
-
-        if self.tucker:
-            self.hada_t1 = nn.Parameter(
-                torch.empty(self.dim, self.dim, self.shape[2], self.shape[3])
-            )
-            self.hada_w1_a = nn.Parameter(
-                torch.empty(self.dim, self.shape[0])
-            )  # out_dim, 1-mode
-            self.hada_w1_b = nn.Parameter(
-                torch.empty(self.dim, self.shape[1])
-            )  # in_dim , 2-mode
-
-            self.hada_t2 = nn.Parameter(
-                torch.empty(self.dim, self.dim, self.shape[2], self.shape[3])
-            )
-            self.hada_w2_a = nn.Parameter(
-                torch.empty(self.dim, self.shape[0])
-            )  # out_dim, 1-mode
-            self.hada_w2_b = nn.Parameter(
-                torch.empty(self.dim, self.shape[1])
-            )  # in_dim , 2-mode
-        else:
-            self.hada_w1_a = nn.Parameter(torch.empty(self.shape[0], self.dim))
-            self.hada_w1_b = nn.Parameter(torch.empty(self.dim, self.shape[1]))
-
-            self.hada_w2_a = nn.Parameter(torch.empty(self.shape[0], self.dim))
-            self.hada_w2_b = nn.Parameter(torch.empty(self.dim, self.shape[1]))
-
-        if type(self.alpha) == torch.Tensor:
-            self.alpha = (
-                self.alpha.detach().float().numpy()
-            )  # without casting, bf16 causes error
-        alpha = self.dim if self.alpha is None or self.alpha == 0 else self.alpha
-        self.scale = alpha / self.dim
-        delattr(self, "alpha")
-        self.register_buffer("alpha", torch.tensor(alpha))  # 定数として扱える
-
-        if self.tucker:
-            torch.nn.init.normal_(self.hada_t1, std=0.1)
-            torch.nn.init.normal_(self.hada_t2, std=0.1)
-        torch.nn.init.normal_(self.hada_w1_b, std=1)
-        torch.nn.init.normal_(self.hada_w1_a, std=0.1)
-        torch.nn.init.normal_(self.hada_w2_b, std=1)
-        torch.nn.init.constant_(self.hada_w2_a, 0)
-
-    def forward(self, orig_weight, org_bias, new_weight, new_bias, *args, **kwargs):
-        if self.tucker:
-            weight = make_weight_tucker(
-                self.hada_t1,
-                self.hada_w1_a,
-                self.hada_w1_b,
-                self.hada_t2,
-                self.hada_w2_a,
-                self.hada_w2_b,
-                scale=torch.tensor(self.scale),
-            )
-        else:
-            weight = make_weight(
-                self.hada_w1_a,
-                self.hada_w1_b,
-                self.hada_w2_a,
-                self.hada_w2_b,
-                scale=torch.tensor(self.scale),
-            )
-        if orig_weight is not None:
-            weight = weight.reshape(orig_weight.shape)
-        if self.training and self.rank_dropout:
-            drop = (torch.rand(weight.size(0)) < self.rank_dropout).to(weight.dtype)
-            drop = drop.view(-1, *[1] * len(weight.shape[1:])).to(weight.device)
-            drop /= drop.mean()
-            weight *= drop
-        return weight, None, None, True, True
+import torch
+import torch.nn as nn
+import torch.nn.functional as F
+
+from .base import LycorisPluginBlock
+from ..modules.loha import make_weight, make_weight_tucker
+
+
+class LohaBlock(LycorisPluginBlock):
+    wrapable_classes = (nn.Conv2d, nn.Linear)
+
+    def __init__(self, *args, **kwargs):
+        super(LohaBlock, self).__init__(*args, **kwargs)
+
+        if self.tucker:
+            self.hada_t1 = nn.Parameter(
+                torch.empty(self.dim, self.dim, self.shape[2], self.shape[3])
+            )
+            self.hada_w1_a = nn.Parameter(
+                torch.empty(self.dim, self.shape[0])
+            )  # out_dim, 1-mode
+            self.hada_w1_b = nn.Parameter(
+                torch.empty(self.dim, self.shape[1])
+            )  # in_dim , 2-mode
+
+            self.hada_t2 = nn.Parameter(
+                torch.empty(self.dim, self.dim, self.shape[2], self.shape[3])
+            )
+            self.hada_w2_a = nn.Parameter(
+                torch.empty(self.dim, self.shape[0])
+            )  # out_dim, 1-mode
+            self.hada_w2_b = nn.Parameter(
+                torch.empty(self.dim, self.shape[1])
+            )  # in_dim , 2-mode
+        else:
+            self.hada_w1_a = nn.Parameter(torch.empty(self.shape[0], self.dim))
+            self.hada_w1_b = nn.Parameter(torch.empty(self.dim, self.shape[1]))
+
+            self.hada_w2_a = nn.Parameter(torch.empty(self.shape[0], self.dim))
+            self.hada_w2_b = nn.Parameter(torch.empty(self.dim, self.shape[1]))
+
+        if type(self.alpha) == torch.Tensor:
+            self.alpha = (
+                self.alpha.detach().float().numpy()
+            )  # without casting, bf16 causes error
+        alpha = self.dim if self.alpha is None or self.alpha == 0 else self.alpha
+        self.scale = alpha / self.dim
+        delattr(self, "alpha")
+        self.register_buffer("alpha", torch.tensor(alpha))  # 定数として扱える
+
+        if self.tucker:
+            torch.nn.init.normal_(self.hada_t1, std=0.1)
+            torch.nn.init.normal_(self.hada_t2, std=0.1)
+        torch.nn.init.normal_(self.hada_w1_b, std=1)
+        torch.nn.init.normal_(self.hada_w1_a, std=0.1)
+        torch.nn.init.normal_(self.hada_w2_b, std=1)
+        torch.nn.init.constant_(self.hada_w2_a, 0)
+
+    def forward(self, orig_weight, org_bias, new_weight, new_bias, *args, **kwargs):
+        if self.tucker:
+            weight = make_weight_tucker(
+                self.hada_t1,
+                self.hada_w1_a,
+                self.hada_w1_b,
+                self.hada_t2,
+                self.hada_w2_a,
+                self.hada_w2_b,
+                scale=torch.tensor(self.scale),
+            )
+        else:
+            weight = make_weight(
+                self.hada_w1_a,
+                self.hada_w1_b,
+                self.hada_w2_a,
+                self.hada_w2_b,
+                scale=torch.tensor(self.scale),
+            )
+        if orig_weight is not None:
+            weight = weight.reshape(orig_weight.shape)
+        if self.training and self.rank_dropout:
+            drop = (torch.rand(weight.size(0)) < self.rank_dropout).to(weight.dtype)
+            drop = drop.view(-1, *[1] * len(weight.shape[1:])).to(weight.device)
+            drop /= drop.mean()
+            weight *= drop
+        return weight, None, None, True, True
```

### Comparing `lycoris_lora-2.3.0.dev4/lycoris/hcp/lokr.py` & `lycoris_lora-2.3.0.dev5/lycoris/hcp/lokr.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,131 +1,131 @@
-import math
-
-import torch
-import torch.nn as nn
-import torch.nn.functional as F
-
-from .base import LycorisPluginBlock
-from ..modules.lokr import make_kron, make_weight_tucker, factorization
-
-
-class LokrBlock(LycorisPluginBlock):
-    wrapable_classes = (nn.Conv2d, nn.Linear)
-
-    def __init__(self, *args, factor=-1, decompose_both=False, **kwargs):
-        super(LokrBlock, self).__init__(*args, **kwargs)
-
-        in_m, in_n = factorization(self.shape[1], factor)
-        out_l, out_k = factorization(self.shape[0], factor)
-
-        self.shape[0] = (out_l, out_k)
-        self.shape[1] = (in_m, in_n)
-
-        if decompose_both and self.dim < max(self.shape[0][0], self.shape[1][0]) / 2:
-            self.lokr_w1_a = nn.Parameter(torch.empty(self.shape[0][0], self.dim))
-            self.lokr_w1_b = nn.Parameter(torch.empty(self.dim, self.shape[1][0]))
-        else:
-            self.use_w1 = True
-            self.lokr_w1 = nn.Parameter(
-                torch.empty(self.shape[0][0], self.shape[1][0])
-            )  # a*c, 1-mode
-
-        if self.module_type == "conv":
-            if self.dim >= max(self.shape[0][1], self.shape[1][1]) / 2:
-                self.use_w2 = True
-                self.lokr_w2 = nn.Parameter(
-                    torch.empty(self.shape[0][1], self.shape[1][1], *self.k_size)
-                )
-            elif self.tucker:
-                self.lokr_t2 = nn.Parameter(
-                    torch.empty(self.dim, self.dim, self.shape[2], self.shape[3])
-                )
-                self.lokr_w2_a = nn.Parameter(
-                    torch.empty(self.dim, self.shape[0][1])
-                )  # b, 1-mode
-                self.lokr_w2_b = nn.Parameter(
-                    torch.empty(self.dim, self.shape[1][1])
-                )  # d, 2-mode
-            else:  # Conv2d not cp
-                # bigger part. weight and LoRA. [b, dim] x [dim, d*k1*k2]
-                self.lokr_w2_a = nn.Parameter(torch.empty(self.shape[0][1], self.dim))
-                self.lokr_w2_b = nn.Parameter(
-                    torch.empty(
-                        self.dim, self.shape[1][1] * self.shape[2] * self.shape[3]
-                    )
-                )
-                # w1 ⊗ (w2_a x w2_b) = (a, b)⊗((c, dim)x(dim, d*k1*k2)) = (a, b)⊗(c, d*k1*k2) = (ac, bd*k1*k2)
-        elif self.module_type == "linear":
-            if self.dim < max(self.shape[0][1], self.shape[1][1]) / 2:
-                # bigger part. weight and LoRA. [b, dim] x [dim, d]
-                self.lokr_w2_a = nn.Parameter(torch.empty(self.shape[0][1], self.dim))
-                self.lokr_w2_b = nn.Parameter(torch.empty(self.dim, self.shape[1][1]))
-                # w1 ⊗ (w2_a x w2_b) = (a, b)⊗((c, dim)x(dim, d)) = (a, b)⊗(c, d) = (ac, bd)
-            else:
-                self.use_w2 = True
-                self.lokr_w2 = nn.Parameter(
-                    torch.empty(self.shape[0][1], self.shape[1][1])
-                )
-        else:
-            raise NotImplementedError
-
-        if self.use_w2:
-            torch.nn.init.constant_(self.lokr_w2, 0)
-        else:
-            if self.tucker:
-                torch.nn.init.kaiming_uniform_(self.lokr_t2, a=math.sqrt(5))
-            torch.nn.init.kaiming_uniform_(self.lokr_w2_a, a=math.sqrt(5))
-            torch.nn.init.constant_(self.lokr_w2_b, 0)
-
-        if self.use_w1:
-            torch.nn.init.kaiming_uniform_(self.lokr_w1, a=math.sqrt(5))
-        else:
-            torch.nn.init.kaiming_uniform_(self.lokr_w1_a, a=math.sqrt(5))
-            torch.nn.init.kaiming_uniform_(self.lokr_w1_b, a=math.sqrt(5))
-
-        if type(self.alpha) == torch.Tensor:
-            self.alpha = (
-                self.alpha.detach().float().numpy()
-            )  # without casting, bf16 causes error
-        alpha = self.dim if self.alpha is None or self.alpha == 0 else self.alpha
-        self.scale = alpha / self.dim
-        print(self.scale)
-        delattr(self, "alpha")
-        self.register_buffer("alpha", torch.tensor(alpha))  # 定数として扱える
-
-        weight = make_kron(
-            self.lokr_w1 if self.use_w1 else self.lokr_w1_a @ self.lokr_w1_b,
-            (
-                self.lokr_w2
-                if self.use_w2
-                else (
-                    make_weight_tucker(self.lokr_t2, self.lokr_w2_a, self.lokr_w2_b)
-                    if self.tucker
-                    else self.lokr_w2_a @ self.lokr_w2_b
-                )
-            ),
-            torch.tensor(self.scale),
-        )
-        assert torch.sum(torch.isnan(weight)) == 0, "lokr init weight is nan"
-
-    def forward(self, orig_weight, org_bias, new_weight, new_bias, *args, **kwargs):
-        weight = make_kron(
-            self.lokr_w1 if self.use_w1 else self.lokr_w1_a @ self.lokr_w1_b,
-            (
-                self.lokr_w2
-                if self.use_w2
-                else (
-                    make_weight_tucker(self.lokr_t2, self.lokr_w2_a, self.lokr_w2_b)
-                    if self.tucker
-                    else self.lokr_w2_a @ self.lokr_w2_b
-                )
-            ),
-            torch.tensor(self.scale),
-        )
-        if orig_weight is not None:
-            weight = weight.reshape(orig_weight.shape)
-        if self.training and self.rank_dropout:
-            drop = (torch.rand(weight.size(0)) < self.rank_dropout).to(weight.dtype)
-            drop = drop.view(-1, *[1] * len(weight.shape[1:])).to(weight.device)
-            drop /= drop.mean()
-            weight *= drop
-        return weight, None, None, True, True
+import math
+
+import torch
+import torch.nn as nn
+import torch.nn.functional as F
+
+from .base import LycorisPluginBlock
+from ..modules.lokr import make_kron, make_weight_tucker, factorization
+
+
+class LokrBlock(LycorisPluginBlock):
+    wrapable_classes = (nn.Conv2d, nn.Linear)
+
+    def __init__(self, *args, factor=-1, decompose_both=False, **kwargs):
+        super(LokrBlock, self).__init__(*args, **kwargs)
+
+        in_m, in_n = factorization(self.shape[1], factor)
+        out_l, out_k = factorization(self.shape[0], factor)
+
+        self.shape[0] = (out_l, out_k)
+        self.shape[1] = (in_m, in_n)
+
+        if decompose_both and self.dim < max(self.shape[0][0], self.shape[1][0]) / 2:
+            self.lokr_w1_a = nn.Parameter(torch.empty(self.shape[0][0], self.dim))
+            self.lokr_w1_b = nn.Parameter(torch.empty(self.dim, self.shape[1][0]))
+        else:
+            self.use_w1 = True
+            self.lokr_w1 = nn.Parameter(
+                torch.empty(self.shape[0][0], self.shape[1][0])
+            )  # a*c, 1-mode
+
+        if self.module_type == "conv":
+            if self.dim >= max(self.shape[0][1], self.shape[1][1]) / 2:
+                self.use_w2 = True
+                self.lokr_w2 = nn.Parameter(
+                    torch.empty(self.shape[0][1], self.shape[1][1], *self.k_size)
+                )
+            elif self.tucker:
+                self.lokr_t2 = nn.Parameter(
+                    torch.empty(self.dim, self.dim, self.shape[2], self.shape[3])
+                )
+                self.lokr_w2_a = nn.Parameter(
+                    torch.empty(self.dim, self.shape[0][1])
+                )  # b, 1-mode
+                self.lokr_w2_b = nn.Parameter(
+                    torch.empty(self.dim, self.shape[1][1])
+                )  # d, 2-mode
+            else:  # Conv2d not cp
+                # bigger part. weight and LoRA. [b, dim] x [dim, d*k1*k2]
+                self.lokr_w2_a = nn.Parameter(torch.empty(self.shape[0][1], self.dim))
+                self.lokr_w2_b = nn.Parameter(
+                    torch.empty(
+                        self.dim, self.shape[1][1] * self.shape[2] * self.shape[3]
+                    )
+                )
+                # w1 ⊗ (w2_a x w2_b) = (a, b)⊗((c, dim)x(dim, d*k1*k2)) = (a, b)⊗(c, d*k1*k2) = (ac, bd*k1*k2)
+        elif self.module_type == "linear":
+            if self.dim < max(self.shape[0][1], self.shape[1][1]) / 2:
+                # bigger part. weight and LoRA. [b, dim] x [dim, d]
+                self.lokr_w2_a = nn.Parameter(torch.empty(self.shape[0][1], self.dim))
+                self.lokr_w2_b = nn.Parameter(torch.empty(self.dim, self.shape[1][1]))
+                # w1 ⊗ (w2_a x w2_b) = (a, b)⊗((c, dim)x(dim, d)) = (a, b)⊗(c, d) = (ac, bd)
+            else:
+                self.use_w2 = True
+                self.lokr_w2 = nn.Parameter(
+                    torch.empty(self.shape[0][1], self.shape[1][1])
+                )
+        else:
+            raise NotImplementedError
+
+        if self.use_w2:
+            torch.nn.init.constant_(self.lokr_w2, 0)
+        else:
+            if self.tucker:
+                torch.nn.init.kaiming_uniform_(self.lokr_t2, a=math.sqrt(5))
+            torch.nn.init.kaiming_uniform_(self.lokr_w2_a, a=math.sqrt(5))
+            torch.nn.init.constant_(self.lokr_w2_b, 0)
+
+        if self.use_w1:
+            torch.nn.init.kaiming_uniform_(self.lokr_w1, a=math.sqrt(5))
+        else:
+            torch.nn.init.kaiming_uniform_(self.lokr_w1_a, a=math.sqrt(5))
+            torch.nn.init.kaiming_uniform_(self.lokr_w1_b, a=math.sqrt(5))
+
+        if type(self.alpha) == torch.Tensor:
+            self.alpha = (
+                self.alpha.detach().float().numpy()
+            )  # without casting, bf16 causes error
+        alpha = self.dim if self.alpha is None or self.alpha == 0 else self.alpha
+        self.scale = alpha / self.dim
+        print(self.scale)
+        delattr(self, "alpha")
+        self.register_buffer("alpha", torch.tensor(alpha))  # 定数として扱える
+
+        weight = make_kron(
+            self.lokr_w1 if self.use_w1 else self.lokr_w1_a @ self.lokr_w1_b,
+            (
+                self.lokr_w2
+                if self.use_w2
+                else (
+                    make_weight_tucker(self.lokr_t2, self.lokr_w2_a, self.lokr_w2_b)
+                    if self.tucker
+                    else self.lokr_w2_a @ self.lokr_w2_b
+                )
+            ),
+            torch.tensor(self.scale),
+        )
+        assert torch.sum(torch.isnan(weight)) == 0, "lokr init weight is nan"
+
+    def forward(self, orig_weight, org_bias, new_weight, new_bias, *args, **kwargs):
+        weight = make_kron(
+            self.lokr_w1 if self.use_w1 else self.lokr_w1_a @ self.lokr_w1_b,
+            (
+                self.lokr_w2
+                if self.use_w2
+                else (
+                    make_weight_tucker(self.lokr_t2, self.lokr_w2_a, self.lokr_w2_b)
+                    if self.tucker
+                    else self.lokr_w2_a @ self.lokr_w2_b
+                )
+            ),
+            torch.tensor(self.scale),
+        )
+        if orig_weight is not None:
+            weight = weight.reshape(orig_weight.shape)
+        if self.training and self.rank_dropout:
+            drop = (torch.rand(weight.size(0)) < self.rank_dropout).to(weight.dtype)
+            drop = drop.view(-1, *[1] * len(weight.shape[1:])).to(weight.device)
+            drop /= drop.mean()
+            weight *= drop
+        return weight, None, None, True, True
```

### Comparing `lycoris_lora-2.3.0.dev4/lycoris/kohya/__init__.py` & `lycoris_lora-2.3.0.dev5/lycoris/kohya/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,864 +1,866 @@
-# network module for kohya
-# reference:
-# https://github.com/microsoft/LoRA/blob/main/loralib/layers.py
-# https://github.com/cloneofsimo/lora/blob/master/lora_diffusion/lora.py
-# https://github.com/kohya-ss/sd-scripts/blob/main/networks/lora.py
-
-import os
-import re
-from typing import List
-
-import torch
-
-from .utils import *
-from ..wrapper import LycorisNetwork
-from ..modules.locon import LoConModule
-from ..modules.loha import LohaModule
-from ..modules.ia3 import IA3Module
-from ..modules.lokr import LokrModule
-from ..modules.dylora import DyLoraModule
-from ..modules.glora import GLoRAModule
-from ..modules.norms import NormModule
-from ..modules.full import FullModule
-from ..modules.diag_oft import DiagOFTModule
-from ..modules.boft import ButterflyOFTModule
-from ..modules import make_module
-
-from ..config import PRESET
-from ..utils.preset import read_preset
-from ..utils import get_module, str_bool
-from ..logging import logger
-
-
-network_module_dict = {
-    "lora": LoConModule,
-    "locon": LoConModule,
-    "loha": LohaModule,
-    "ia3": IA3Module,
-    "lokr": LokrModule,
-    "dylora": DyLoraModule,
-    "glora": GLoRAModule,
-    "full": FullModule,
-    "diag-oft": DiagOFTModule,
-    "boft": ButterflyOFTModule,
-}
-
-
-def create_network(
-    multiplier, network_dim, network_alpha, vae, text_encoder, unet, **kwargs
-):
-    if network_dim is None:
-        network_dim = 4  # default
-    conv_dim = int(kwargs.get("conv_dim", network_dim) or network_dim)
-    conv_alpha = float(kwargs.get("conv_alpha", network_alpha) or network_alpha)
-    dropout = float(kwargs.get("dropout", 0.0) or 0.0)
-    rank_dropout = float(kwargs.get("rank_dropout", 0.0) or 0.0)
-    module_dropout = float(kwargs.get("module_dropout", 0.0) or 0.0)
-    algo = (kwargs.get("algo", "lora") or "lora").lower()
-    use_tucker = str_bool(
-        not kwargs.get("disable_conv_cp", True)
-        or kwargs.get("use_conv_cp", False)
-        or kwargs.get("use_cp", False)
-        or kwargs.get("use_tucker", False)
-    )
-    if "disable_conv_cp" in kwargs or "use_cp" in kwargs or "use_conv_cp" in kwargs:
-        logger.warning(
-            "disable_conv_cp and use_cp are deprecated. Please use use_tucker instead.",
-            stacklevel=2,
-        )
-    use_scalar = str_bool(kwargs.get("use_scalar", False))
-    block_size = int(kwargs.get("block_size", 4) or 4)
-    train_norm = str_bool(kwargs.get("train_norm", False))
-    constrain = float(kwargs.get("constrain", 0) or 0)
-    rescaled = str_bool(kwargs.get("rescaled", False))
-    weight_decompose = str_bool(kwargs.get("dora_wd", False))
-    full_matrix = str_bool(kwargs.get("full_matrix", False))
-    bypass_mode = str_bool(kwargs.get("bypass_mode", False))
-    unbalanced_factorization = str_bool(kwargs.get("unbalanced_factorization", False))
-
-    if unbalanced_factorization:
-        logger.info("Unbalanced factorization for LoKr is enabled")
-
-    if bypass_mode:
-        logger.info("Bypass mode is enabled")
-
-    if weight_decompose:
-        logger.info("Weight decomposition is enabled")
-
-    if full_matrix:
-        logger.info("Full matrix mode for LoKr is enabled")
-
-    if algo == "glora" and conv_dim > 0:
-        conv_dim = 0
-        logger.info("Disable conv layer for GLoRA")
-
-    preset = kwargs.get("preset", "full")
-    if preset not in PRESET:
-        preset = read_preset(preset)
-    else:
-        preset = PRESET[preset]
-    assert preset is not None
-    LycorisNetworkKohya.apply_preset(preset)
-
-    logger.info(f"Using rank adaptation algo: {algo}")
-
-    if (
-        (algo == "loha")
-        and not kwargs.get("no_dim_warn", False)
-        and (network_dim > 64 or conv_dim > 64)
-    ):
-        warning_type = {"loha": "Hadamard Product representation"}
-        warning_msg = f"""You are not supposed to use dim>64 (64*64 = 4096, it already has enough rank)\n
-            in {warning_type[algo]}!\n
-            Please consider use lower dim or disable this warning with --network_args no_dim_warn=True\n
-            If you just want to use high dim {algo}, please consider use lower lr.
-        """
-        logger.warning(warning_msg, stacklevel=2)
-
-    if algo == "ia3":
-        network = IA3Network(
-            text_encoder,
-            unet,
-            multiplier=multiplier,
-        )
-    else:
-        network = LycorisNetworkKohya(
-            text_encoder,
-            unet,
-            multiplier=multiplier,
-            lora_dim=network_dim,
-            conv_lora_dim=conv_dim,
-            alpha=network_alpha,
-            conv_alpha=conv_alpha,
-            dropout=dropout,
-            rank_dropout=rank_dropout,
-            module_dropout=module_dropout,
-            use_tucker=use_tucker,
-            use_scalar=use_scalar,
-            network_module=algo,
-            train_norm=train_norm,
-            decompose_both=kwargs.get("decompose_both", False),
-            factor=kwargs.get("factor", -1),
-            block_size=block_size,
-            constrain=constrain,
-            rescaled=rescaled,
-            weight_decompose=weight_decompose,
-            full_matrix=full_matrix,
-            bypass_mode=bypass_mode,
-            unbalanced_factorization=unbalanced_factorization,
-        )
-
-    if algo == "dylora":
-        # dylora didn't support scale weight norm yet
-        delattr(type(network), "apply_max_norm_regularization")
-
-    return network
-
-
-def create_network_from_weights(
-    multiplier,
-    file,
-    vae,
-    text_encoder,
-    unet,
-    weights_sd=None,
-    for_inference=False,
-    **kwargs,
-):
-    if weights_sd is None:
-        if os.path.splitext(file)[1] == ".safetensors":
-            from safetensors.torch import load_file, safe_open
-
-            weights_sd = load_file(file)
-        else:
-            weights_sd = torch.load(file, map_location="cpu")
-
-    # get dim/alpha mapping
-    unet_loras = {}
-    te_loras = {}
-    for key, value in weights_sd.items():
-        if "." not in key:
-            continue
-
-        lora_name = key.split(".")[0]
-        if lora_name.startswith(LycorisNetworkKohya.LORA_PREFIX_UNET):
-            unet_loras[lora_name] = None
-        elif lora_name.startswith(LycorisNetworkKohya.LORA_PREFIX_TEXT_ENCODER):
-            te_loras[lora_name] = None
-
-    for name, modules in unet.named_modules():
-        lora_name = f"{LycorisNetworkKohya.LORA_PREFIX_UNET}_{name}".replace(".", "_")
-        if lora_name in unet_loras:
-            unet_loras[lora_name] = modules
-
-    if isinstance(text_encoder, list):
-        text_encoders = text_encoder
-        use_index = True
-    else:
-        text_encoders = [text_encoder]
-        use_index = False
-
-    for idx, te in enumerate(text_encoders):
-        if use_index:
-            prefix = f"{LycorisNetworkKohya.LORA_PREFIX_TEXT_ENCODER}{idx+1}"
-        else:
-            prefix = LycorisNetworkKohya.LORA_PREFIX_TEXT_ENCODER
-        for name, modules in te.named_modules():
-            lora_name = f"{prefix}_{name}".replace(".", "_")
-            if lora_name in te_loras:
-                te_loras[lora_name] = modules
-
-    network = LycorisNetworkKohya(text_encoder, unet)
-    network.unet_loras = []
-    network.text_encoder_loras = []
-
-    for lora_name, orig_modules in unet_loras.items():
-        if orig_modules is None:
-            continue
-        lyco_type, params = get_module(weights_sd, lora_name)
-        module = make_module(lyco_type, params, lora_name, orig_modules)
-        if module is not None:
-            network.unet_loras.append(module)
-
-    for lora_name, orig_modules in te_loras.items():
-        if orig_modules is None:
-            continue
-        lyco_type, params = get_module(weights_sd, lora_name)
-        module = make_module(lyco_type, params, lora_name, orig_modules)
-        if module is not None:
-            network.text_encoder_loras.append(module)
-
-    for lora in network.unet_loras + network.text_encoder_loras:
-        lora.multiplier = multiplier
-
-    return network, weights_sd
-
-
-class LycorisNetworkKohya(LycorisNetwork):
-    """
-    LoRA + LoCon
-    """
-
-    # Ignore proj_in or proj_out, their channels is only a few.
-    ENABLE_CONV = True
-    UNET_TARGET_REPLACE_MODULE = [
-        "Transformer2DModel",
-        "ResnetBlock2D",
-        "Downsample2D",
-        "Upsample2D",
-    ]
-    UNET_TARGET_REPLACE_NAME = [
-        "conv_in",
-        "conv_out",
-        "time_embedding.linear_1",
-        "time_embedding.linear_2",
-    ]
-    TEXT_ENCODER_TARGET_REPLACE_MODULE = ["CLIPAttention", "CLIPMLP"]
-    TEXT_ENCODER_TARGET_REPLACE_NAME = []
-    LORA_PREFIX_UNET = "lora_unet"
-    LORA_PREFIX_TEXT_ENCODER = "lora_te"
-    MODULE_ALGO_MAP = {}
-    NAME_ALGO_MAP = {}
-
-    @classmethod
-    def apply_preset(cls, preset):
-        if "enable_conv" in preset:
-            cls.ENABLE_CONV = preset["enable_conv"]
-        if "unet_target_module" in preset:
-            cls.UNET_TARGET_REPLACE_MODULE = preset["unet_target_module"]
-        if "unet_target_name" in preset:
-            cls.UNET_TARGET_REPLACE_NAME = preset["unet_target_name"]
-        if "text_encoder_target_module" in preset:
-            cls.TEXT_ENCODER_TARGET_REPLACE_MODULE = preset[
-                "text_encoder_target_module"
-            ]
-        if "text_encoder_target_name" in preset:
-            cls.TEXT_ENCODER_TARGET_REPLACE_NAME = preset["text_encoder_target_name"]
-        if "module_algo_map" in preset:
-            cls.MODULE_ALGO_MAP = preset["module_algo_map"]
-        if "name_algo_map" in preset:
-            cls.NAME_ALGO_MAP = preset["name_algo_map"]
-        return cls
-
-    def __init__(
-        self,
-        text_encoder,
-        unet,
-        multiplier=1.0,
-        lora_dim=4,
-        conv_lora_dim=4,
-        alpha=1,
-        conv_alpha=1,
-        use_tucker=False,
-        dropout=0,
-        rank_dropout=0,
-        module_dropout=0,
-        network_module: str = "locon",
-        norm_modules=NormModule,
-        train_norm=False,
-        **kwargs,
-    ) -> None:
-        torch.nn.Module.__init__(self)
-        root_kwargs = kwargs
-        self.multiplier = multiplier
-        self.lora_dim = lora_dim
-
-        if not self.ENABLE_CONV:
-            conv_lora_dim = 0
-
-        self.conv_lora_dim = int(conv_lora_dim)
-        if self.conv_lora_dim and self.conv_lora_dim != self.lora_dim:
-            logger.info("Apply different lora dim for conv layer")
-            logger.info(f"Conv Dim: {conv_lora_dim}, Linear Dim: {lora_dim}")
-        elif self.conv_lora_dim == 0:
-            logger.info("Disable conv layer")
-
-        self.alpha = alpha
-        self.conv_alpha = float(conv_alpha)
-        if self.conv_lora_dim and self.alpha != self.conv_alpha:
-            logger.info("Apply different alpha value for conv layer")
-            logger.info(f"Conv alpha: {conv_alpha}, Linear alpha: {alpha}")
-
-        if 1 >= dropout >= 0:
-            logger.info(f"Use Dropout value: {dropout}")
-        self.dropout = dropout
-        self.rank_dropout = rank_dropout
-        self.module_dropout = module_dropout
-
-        self.use_tucker = use_tucker
-
-        def create_single_module(
-            lora_name: str,
-            module: torch.nn.Module,
-            algo_name,
-            dim=None,
-            alpha=None,
-            use_tucker=self.use_tucker,
-            **kwargs,
-        ):
-            for k, v in root_kwargs.items():
-                if k in kwargs:
-                    continue
-                kwargs[k] = v
-
-            if train_norm and "Norm" in module.__class__.__name__:
-                return norm_modules(
-                    lora_name,
-                    module,
-                    self.multiplier,
-                    self.rank_dropout,
-                    self.module_dropout,
-                    **kwargs,
-                )
-            lora = None
-            if isinstance(module, torch.nn.Linear) and lora_dim > 0:
-                dim = dim or lora_dim
-                alpha = alpha or self.alpha
-            elif isinstance(module, torch.nn.Conv2d):
-                k_size, *_ = module.kernel_size
-                if k_size == 1 and lora_dim > 0:
-                    dim = dim or lora_dim
-                    alpha = alpha or self.alpha
-                elif conv_lora_dim > 0 or dim:
-                    dim = dim or conv_lora_dim
-                    alpha = alpha or self.conv_alpha
-                else:
-                    return None
-            else:
-                return None
-            lora = network_module_dict[algo_name](
-                lora_name,
-                module,
-                self.multiplier,
-                dim,
-                alpha,
-                self.dropout,
-                self.rank_dropout,
-                self.module_dropout,
-                use_tucker,
-                **kwargs,
-            )
-            return lora
-
-        def create_modules_(
-            prefix: str,
-            root_module: torch.nn.Module,
-            algo,
-            configs={},
-        ):
-            loras = {}
-            lora_names = []
-            for name, module in root_module.named_modules():
-                if module is root_module:
-                    continue
-                module_name = module.__class__.__name__
-                if module_name in self.MODULE_ALGO_MAP:
-                    next_config = self.MODULE_ALGO_MAP[module_name]
-                    next_algo = next_config.get("algo", algo)
-                    new_loras, new_lora_names = create_modules_(
-                        f"{prefix}_{name}", module, next_algo, next_config
-                    )
-                    for lora_name, lora in zip(new_lora_names, new_loras):
-                        if lora_name not in loras:
-                            loras[lora_name] = lora
-                            lora_names.append(lora_name)
-                    continue
-                lora_name = prefix + "." + name
-                lora_name = lora_name.replace(".", "_")
-                if lora_name in loras:
-                    continue
-
-                lora = create_single_module(lora_name, module, algo, **configs)
-                if lora is not None:
-                    loras[lora_name] = lora
-                    lora_names.append(lora_name)
-            return [loras[lora_name] for lora_name in lora_names], lora_names
-
-        # create module instances
-        def create_modules(
-            prefix,
-            root_module: torch.nn.Module,
-            target_replace_modules,
-            target_replace_names=[],
-        ) -> List:
-            logger.info("Create LyCORIS Module")
-            loras = []
-            next_config = {}
-            for name, module in root_module.named_modules():
-                module_name = module.__class__.__name__
-                if module_name in target_replace_modules:
-                    if module_name in self.MODULE_ALGO_MAP:
-                        next_config = self.MODULE_ALGO_MAP[module_name]
-                        algo = next_config.get("algo", network_module)
-                    else:
-                        algo = network_module
-                    loras.extend(
-                        create_modules_(f"{prefix}_{name}", module, algo, next_config)[
-                            0
-                        ]
-                    )
-                    next_config = {}
-                elif name in target_replace_names or any(
-                    re.match(t, name) for t in target_replace_names
-                ):
-                    if name in self.NAME_ALGO_MAP:
-                        next_config = self.NAME_ALGO_MAP[name]
-                        algo = next_config.get("algo", network_module)
-                    elif module_name in self.MODULE_ALGO_MAP:
-                        next_config = self.MODULE_ALGO_MAP[module_name]
-                        algo = next_config.get("algo", network_module)
-                    else:
-                        algo = network_module
-                    lora_name = prefix + "." + name
-                    lora_name = lora_name.replace(".", "_")
-                    lora = create_single_module(lora_name, module, algo, **next_config)
-                    next_config = {}
-                    if lora is not None:
-                        loras.append(lora)
-            return loras
-
-        if network_module == GLoRAModule:
-            logger.info("GLoRA enabled, only train transformer")
-            # only train transformer (for GLoRA)
-            LycorisNetworkKohya.UNET_TARGET_REPLACE_MODULE = [
-                "Transformer2DModel",
-                "Attention",
-            ]
-            LycorisNetworkKohya.UNET_TARGET_REPLACE_NAME = []
-
-        if isinstance(text_encoder, list):
-            text_encoders = text_encoder
-            use_index = True
-        else:
-            text_encoders = [text_encoder]
-            use_index = False
-
-        self.text_encoder_loras = []
-        for i, te in enumerate(text_encoders):
-            self.text_encoder_loras.extend(
-                create_modules(
-                    LycorisNetworkKohya.LORA_PREFIX_TEXT_ENCODER
-                    + (f"{i+1}" if use_index else ""),
-                    te,
-                    LycorisNetworkKohya.TEXT_ENCODER_TARGET_REPLACE_MODULE,
-                    LycorisNetworkKohya.TEXT_ENCODER_TARGET_REPLACE_NAME,
-                )
-            )
-        logger.info(
-            f"create LyCORIS for Text Encoder: {len(self.text_encoder_loras)} modules."
-        )
-
-        self.unet_loras = create_modules(
-            LycorisNetworkKohya.LORA_PREFIX_UNET,
-            unet,
-            LycorisNetworkKohya.UNET_TARGET_REPLACE_MODULE,
-            LycorisNetworkKohya.UNET_TARGET_REPLACE_NAME,
-        )
-        logger.info(f"create LyCORIS for U-Net: {len(self.unet_loras)} modules.")
-
-        algo_table = {}
-        for lora in self.text_encoder_loras + self.unet_loras:
-            algo_table[lora.__class__.__name__] = (
-                algo_table.get(lora.__class__.__name__, 0) + 1
-            )
-        logger.info(f"module type table: {algo_table}")
-
-        self.weights_sd = None
-
-        self.loras = self.text_encoder_loras + self.unet_loras
-        # assertion
-        names = set()
-        for lora in self.loras:
-            assert (
-                lora.lora_name not in names
-            ), f"duplicated lora name: {lora.lora_name}"
-            names.add(lora.lora_name)
-
-    def load_weights(self, file):
-        if os.path.splitext(file)[1] == ".safetensors":
-            from safetensors.torch import load_file, safe_open
-
-            self.weights_sd = load_file(file)
-        else:
-            self.weights_sd = torch.load(file, map_location="cpu")
-        missing, unexpected = self.load_state_dict(self.weights_sd, strict=False)
-        state = {}
-        if missing:
-            state["missing keys"] = missing
-        if unexpected:
-            state["unexpected keys"] = unexpected
-        return state
-
-    def apply_to(self, text_encoder, unet, apply_text_encoder=None, apply_unet=None):
-        assert (
-            apply_text_encoder is not None and apply_unet is not None
-        ), f"internal error: flag not set"
-
-        if apply_text_encoder:
-            logger.info("enable LyCORIS for text encoder")
-        else:
-            self.text_encoder_loras = []
-
-        if apply_unet:
-            logger.info("enable LyCORIS for U-Net")
-        else:
-            self.unet_loras = []
-
-        self.loras = self.text_encoder_loras + self.unet_loras
-
-        for lora in self.loras:
-            lora.apply_to()
-            self.add_module(lora.lora_name, lora)
-
-        if self.weights_sd:
-            # if some weights are not in state dict, it is ok because initial LoRA does nothing (lora_up is initialized by zeros)
-            info = self.load_state_dict(self.weights_sd, False)
-            logger.info(f"weights are loaded: {info}")
-
-    # TODO refactor to common function with apply_to
-    def merge_to(self, text_encoder, unet, weights_sd, dtype, device):
-        apply_text_encoder = apply_unet = False
-        for key in weights_sd.keys():
-            if key.startswith(LycorisNetworkKohya.LORA_PREFIX_TEXT_ENCODER):
-                apply_text_encoder = True
-            elif key.startswith(LycorisNetworkKohya.LORA_PREFIX_UNET):
-                apply_unet = True
-
-        if apply_text_encoder:
-            logger.info("enable LoRA for text encoder")
-        else:
-            self.text_encoder_loras = []
-
-        if apply_unet:
-            logger.info("enable LoRA for U-Net")
-        else:
-            self.unet_loras = []
-
-        self.loras = self.text_encoder_loras + self.unet_loras
-        super().merge_to(1)
-
-    def prepare_optimizer_params(self, text_encoder_lr, unet_lr, learning_rate):
-        def enumerate_params(loras):
-            params = []
-            for lora in loras:
-                params.extend(lora.parameters())
-            return params
-
-        self.requires_grad_(True)
-        all_params = []
-
-        if self.text_encoder_loras:
-            param_data = {"params": enumerate_params(self.text_encoder_loras)}
-            if text_encoder_lr is not None:
-                param_data["lr"] = text_encoder_lr
-            all_params.append(param_data)
-
-        if self.unet_loras:
-            param_data = {"params": enumerate_params(self.unet_loras)}
-            if unet_lr is not None:
-                param_data["lr"] = unet_lr
-            all_params.append(param_data)
-
-        return all_params
-
-    def save_weights(self, file, dtype, metadata):
-        if metadata is not None and len(metadata) == 0:
-            metadata = None
-
-        state_dict = self.state_dict()
-
-        if dtype is not None:
-            for key in list(state_dict.keys()):
-                v = state_dict[key]
-                v = v.detach().clone().to("cpu").to(dtype)
-                state_dict[key] = v
-
-        if os.path.splitext(file)[1] == ".safetensors":
-            from safetensors.torch import save_file
-
-            # Precalculate model hashes to save time on indexing
-            if metadata is None:
-                metadata = {}
-            model_hash, legacy_hash = precalculate_safetensors_hashes(
-                state_dict, metadata
-            )
-            metadata["sshs_model_hash"] = model_hash
-            metadata["sshs_legacy_hash"] = legacy_hash
-
-            save_file(state_dict, file, metadata)
-        else:
-            torch.save(state_dict, file)
-
-
-class IA3Network(torch.nn.Module):
-    """
-    IA3 network
-    """
-
-    # Ignore proj_in or proj_out, their channels is only a few.
-    UNET_TARGET_REPLACE_MODULE = []
-    UNET_TARGET_REPLACE_NAME = ["to_k", "to_v", "ff.net.2"]
-    TEXT_ENCODER_TARGET_REPLACE_MODULE = []
-    TEXT_ENCODER_TARGET_REPLACE_NAME = ["k_proj", "v_proj", "mlp.fc2"]
-    TRAIN_INPUT = ["mlp.fc2", "ff.net.2"]
-    LORA_PREFIX_UNET = "lora_unet"
-    LORA_PREFIX_TEXT_ENCODER = "lora_te"
-
-    def __init__(
-        self,
-        text_encoder,
-        unet,
-        multiplier=1.0,
-        **kwargs,
-    ) -> None:
-        super().__init__()
-        self.multiplier = multiplier
-
-        # create module instances
-        def create_modules(
-            prefix,
-            root_module: torch.nn.Module,
-            target_replace_modules,
-            target_replace_names=[],
-            target_train_input=[],
-        ) -> List[IA3Module]:
-            logger.info("Create LyCORIS Module")
-            loras = []
-            for name, module in root_module.named_modules():
-                if module.__class__.__name__ in target_replace_modules:
-                    for child_name, child_module in module.named_modules():
-                        lora_name = prefix + "." + name + "." + child_name
-                        lora_name = lora_name.replace(".", "_")
-                        if child_module.__class__.__name__ in {"Linear", "Conv2d"}:
-                            lora = IA3Module(
-                                lora_name,
-                                child_module,
-                                self.multiplier,
-                                name in target_train_input,
-                                **kwargs,
-                            )
-                            loras.append(lora)
-                elif any(i in name for i in target_replace_names):
-                    lora_name = prefix + "." + name
-                    lora_name = lora_name.replace(".", "_")
-                    if module.__class__.__name__ in {"Linear", "Conv2d"}:
-                        lora = IA3Module(
-                            lora_name,
-                            module,
-                            self.multiplier,
-                            name in target_train_input,
-                            **kwargs,
-                        )
-                        loras.append(lora)
-            return loras
-
-        if isinstance(text_encoder, list):
-            text_encoders = text_encoder
-            use_index = True
-        else:
-            text_encoders = [text_encoder]
-            use_index = False
-
-        self.text_encoder_loras = []
-        for i, te in enumerate(text_encoders):
-            self.text_encoder_loras.extend(
-                create_modules(
-                    IA3Network.LORA_PREFIX_TEXT_ENCODER
-                    + (f"{i+1}" if use_index else ""),
-                    te,
-                    IA3Network.TEXT_ENCODER_TARGET_REPLACE_MODULE,
-                    IA3Network.TEXT_ENCODER_TARGET_REPLACE_NAME,
-                    IA3Network.TRAIN_INPUT,
-                )
-            )
-        logger.info(
-            f"create LyCORIS for Text Encoder: {len(self.text_encoder_loras)} modules."
-        )
-
-        self.unet_loras = create_modules(
-            IA3Network.LORA_PREFIX_UNET,
-            unet,
-            IA3Network.UNET_TARGET_REPLACE_MODULE,
-            IA3Network.UNET_TARGET_REPLACE_NAME,
-            IA3Network.TRAIN_INPUT,
-        )
-        logger.info(f"create LyCORIS for U-Net: {len(self.unet_loras)} modules.")
-
-        self.weights_sd = None
-
-        # assertion
-        names = set()
-        for lora in self.text_encoder_loras + self.unet_loras:
-            assert (
-                lora.lora_name not in names
-            ), f"duplicated lora name: {lora.lora_name}"
-            names.add(lora.lora_name)
-
-    def set_multiplier(self, multiplier):
-        self.multiplier = multiplier
-        for lora in self.text_encoder_loras + self.unet_loras:
-            lora.multiplier = self.multiplier
-
-    def load_weights(self, file):
-        if os.path.splitext(file)[1] == ".safetensors":
-            from safetensors.torch import load_file, safe_open
-
-            self.weights_sd = load_file(file)
-        else:
-            self.weights_sd = torch.load(file, map_location="cpu")
-
-    def apply_to(self, text_encoder, unet, apply_text_encoder=None, apply_unet=None):
-        if self.weights_sd:
-            weights_has_text_encoder = weights_has_unet = False
-            for key in self.weights_sd.keys():
-                if key.startswith(LycorisNetworkKohya.LORA_PREFIX_TEXT_ENCODER):
-                    weights_has_text_encoder = True
-                elif key.startswith(LycorisNetworkKohya.LORA_PREFIX_UNET):
-                    weights_has_unet = True
-
-            if apply_text_encoder is None:
-                apply_text_encoder = weights_has_text_encoder
-            else:
-                assert (
-                    apply_text_encoder == weights_has_text_encoder
-                ), f"text encoder weights: {weights_has_text_encoder} but text encoder flag: {apply_text_encoder} / 重みとText Encoderのフラグが矛盾しています"
-
-            if apply_unet is None:
-                apply_unet = weights_has_unet
-            else:
-                assert (
-                    apply_unet == weights_has_unet
-                ), f"u-net weights: {weights_has_unet} but u-net flag: {apply_unet} / 重みとU-Netのフラグが矛盾しています"
-        else:
-            assert (
-                apply_text_encoder is not None and apply_unet is not None
-            ), f"internal error: flag not set"
-
-        if apply_text_encoder:
-            logger.info("enable LyCORIS for text encoder")
-        else:
-            self.text_encoder_loras = []
-
-        if apply_unet:
-            logger.info("enable LyCORIS for U-Net")
-        else:
-            self.unet_loras = []
-
-        for lora in self.text_encoder_loras + self.unet_loras:
-            lora.apply_to()
-            self.add_module(lora.lora_name, lora)
-
-        if self.weights_sd:
-            # if some weights are not in state dict, it is ok because initial LoRA does nothing (lora_up is initialized by zeros)
-            info = self.load_state_dict(self.weights_sd, False)
-            logger.info(f"weights are loaded: {info}")
-
-    def enable_gradient_checkpointing(self):
-        # not supported
-        def make_ckpt(module):
-            if isinstance(module, torch.nn.Module):
-                module.grad_ckpt = True
-
-        self.apply(make_ckpt)
-        pass
-
-    def prepare_optimizer_params(self, text_encoder_lr, unet_lr, learning_rate):
-        def enumerate_params(loras):
-            params = []
-            for lora in loras:
-                params.extend(lora.parameters())
-            return params
-
-        self.requires_grad_(True)
-        all_params = []
-
-        if self.text_encoder_loras:
-            param_data = {"params": enumerate_params(self.text_encoder_loras)}
-            if text_encoder_lr is not None:
-                param_data["lr"] = text_encoder_lr
-            all_params.append(param_data)
-
-        if self.unet_loras:
-            param_data = {"params": enumerate_params(self.unet_loras)}
-            if unet_lr is not None:
-                param_data["lr"] = unet_lr
-            all_params.append(param_data)
-
-        return all_params
-
-    def prepare_grad_etc(self, text_encoder, unet):
-        self.requires_grad_(True)
-
-    def on_epoch_start(self, text_encoder, unet):
-        self.train()
-
-    def get_trainable_params(self):
-        return self.parameters()
-
-    def save_weights(self, file, dtype, metadata):
-        if metadata is not None and len(metadata) == 0:
-            metadata = None
-
-        state_dict = self.state_dict()
-
-        if dtype is not None:
-            for key in list(state_dict.keys()):
-                v = state_dict[key]
-                v = v.detach().clone().to("cpu").to(dtype)
-                state_dict[key] = v
-
-        if os.path.splitext(file)[1] == ".safetensors":
-            from safetensors.torch import save_file
-
-            # Precalculate model hashes to save time on indexing
-            if metadata is None:
-                metadata = {}
-            model_hash, legacy_hash = precalculate_safetensors_hashes(
-                state_dict, metadata
-            )
-            metadata["sshs_model_hash"] = model_hash
-            metadata["sshs_legacy_hash"] = legacy_hash
-
-            save_file(state_dict, file, metadata)
-        else:
-            torch.save(state_dict, file)
+# network module for kohya
+# reference:
+# https://github.com/microsoft/LoRA/blob/main/loralib/layers.py
+# https://github.com/cloneofsimo/lora/blob/master/lora_diffusion/lora.py
+# https://github.com/kohya-ss/sd-scripts/blob/main/networks/lora.py
+
+import os
+import re
+from typing import List
+
+import torch
+
+from .utils import *
+from ..wrapper import LycorisNetwork
+from ..modules.locon import LoConModule
+from ..modules.loha import LohaModule
+from ..modules.ia3 import IA3Module
+from ..modules.lokr import LokrModule
+from ..modules.dylora import DyLoraModule
+from ..modules.glora import GLoRAModule
+from ..modules.norms import NormModule
+from ..modules.full import FullModule
+from ..modules.diag_oft import DiagOFTModule
+from ..modules.boft import ButterflyOFTModule
+from ..modules import make_module
+
+from ..config import PRESET
+from ..utils.preset import read_preset
+from ..utils import get_module, str_bool
+from ..logging import logger
+
+
+network_module_dict = {
+    "lora": LoConModule,
+    "locon": LoConModule,
+    "loha": LohaModule,
+    "ia3": IA3Module,
+    "lokr": LokrModule,
+    "dylora": DyLoraModule,
+    "glora": GLoRAModule,
+    "full": FullModule,
+    "diag-oft": DiagOFTModule,
+    "boft": ButterflyOFTModule,
+}
+
+
+def create_network(
+    multiplier, network_dim, network_alpha, vae, text_encoder, unet, **kwargs
+):
+    if network_dim is None:
+        network_dim = 4  # default
+    conv_dim = int(kwargs.get("conv_dim", network_dim) or network_dim)
+    conv_alpha = float(kwargs.get("conv_alpha", network_alpha) or network_alpha)
+    dropout = float(kwargs.get("dropout", 0.0) or 0.0)
+    rank_dropout = float(kwargs.get("rank_dropout", 0.0) or 0.0)
+    module_dropout = float(kwargs.get("module_dropout", 0.0) or 0.0)
+    algo = (kwargs.get("algo", "lora") or "lora").lower()
+    use_tucker = str_bool(
+        not kwargs.get("disable_conv_cp", True)
+        or kwargs.get("use_conv_cp", False)
+        or kwargs.get("use_cp", False)
+        or kwargs.get("use_tucker", False)
+    )
+    if "disable_conv_cp" in kwargs or "use_cp" in kwargs or "use_conv_cp" in kwargs:
+        logger.warning(
+            "disable_conv_cp and use_cp are deprecated. Please use use_tucker instead.",
+            stacklevel=2,
+        )
+    use_scalar = str_bool(kwargs.get("use_scalar", False))
+    block_size = int(kwargs.get("block_size", 4) or 4)
+    train_norm = str_bool(kwargs.get("train_norm", False))
+    constrain = float(kwargs.get("constrain", 0) or 0)
+    rescaled = str_bool(kwargs.get("rescaled", False))
+    weight_decompose = str_bool(kwargs.get("dora_wd", False))
+    full_matrix = str_bool(kwargs.get("full_matrix", False))
+    bypass_mode = str_bool(kwargs.get("bypass_mode", False))
+    rs_lora = str_bool(kwargs.get("rs_lora", False))
+    unbalanced_factorization = str_bool(kwargs.get("unbalanced_factorization", False))
+
+    if unbalanced_factorization:
+        logger.info("Unbalanced factorization for LoKr is enabled")
+
+    if bypass_mode:
+        logger.info("Bypass mode is enabled")
+
+    if weight_decompose:
+        logger.info("Weight decomposition is enabled")
+
+    if full_matrix:
+        logger.info("Full matrix mode for LoKr is enabled")
+
+    if algo == "glora" and conv_dim > 0:
+        conv_dim = 0
+        logger.info("Disable conv layer for GLoRA")
+
+    preset = kwargs.get("preset", "full")
+    if preset not in PRESET:
+        preset = read_preset(preset)
+    else:
+        preset = PRESET[preset]
+    assert preset is not None
+    LycorisNetworkKohya.apply_preset(preset)
+
+    logger.info(f"Using rank adaptation algo: {algo}")
+
+    if (
+        (algo == "loha")
+        and not kwargs.get("no_dim_warn", False)
+        and (network_dim > 64 or conv_dim > 64)
+    ):
+        warning_type = {"loha": "Hadamard Product representation"}
+        warning_msg = f"""You are not supposed to use dim>64 (64*64 = 4096, it already has enough rank)\n
+            in {warning_type[algo]}!\n
+            Please consider use lower dim or disable this warning with --network_args no_dim_warn=True\n
+            If you just want to use high dim {algo}, please consider use lower lr.
+        """
+        logger.warning(warning_msg, stacklevel=2)
+
+    if algo == "ia3":
+        network = IA3Network(
+            text_encoder,
+            unet,
+            multiplier=multiplier,
+        )
+    else:
+        network = LycorisNetworkKohya(
+            text_encoder,
+            unet,
+            multiplier=multiplier,
+            lora_dim=network_dim,
+            conv_lora_dim=conv_dim,
+            alpha=network_alpha,
+            conv_alpha=conv_alpha,
+            dropout=dropout,
+            rank_dropout=rank_dropout,
+            module_dropout=module_dropout,
+            use_tucker=use_tucker,
+            use_scalar=use_scalar,
+            network_module=algo,
+            train_norm=train_norm,
+            decompose_both=kwargs.get("decompose_both", False),
+            factor=kwargs.get("factor", -1),
+            block_size=block_size,
+            constrain=constrain,
+            rescaled=rescaled,
+            weight_decompose=weight_decompose,
+            full_matrix=full_matrix,
+            bypass_mode=bypass_mode,
+            rs_lora=rs_lora
+            unbalanced_factorization=unbalanced_factorization,
+        )
+
+    if algo == "dylora":
+        # dylora didn't support scale weight norm yet
+        delattr(type(network), "apply_max_norm_regularization")
+
+    return network
+
+
+def create_network_from_weights(
+    multiplier,
+    file,
+    vae,
+    text_encoder,
+    unet,
+    weights_sd=None,
+    for_inference=False,
+    **kwargs,
+):
+    if weights_sd is None:
+        if os.path.splitext(file)[1] == ".safetensors":
+            from safetensors.torch import load_file, safe_open
+
+            weights_sd = load_file(file)
+        else:
+            weights_sd = torch.load(file, map_location="cpu")
+
+    # get dim/alpha mapping
+    unet_loras = {}
+    te_loras = {}
+    for key, value in weights_sd.items():
+        if "." not in key:
+            continue
+
+        lora_name = key.split(".")[0]
+        if lora_name.startswith(LycorisNetworkKohya.LORA_PREFIX_UNET):
+            unet_loras[lora_name] = None
+        elif lora_name.startswith(LycorisNetworkKohya.LORA_PREFIX_TEXT_ENCODER):
+            te_loras[lora_name] = None
+
+    for name, modules in unet.named_modules():
+        lora_name = f"{LycorisNetworkKohya.LORA_PREFIX_UNET}_{name}".replace(".", "_")
+        if lora_name in unet_loras:
+            unet_loras[lora_name] = modules
+
+    if isinstance(text_encoder, list):
+        text_encoders = text_encoder
+        use_index = True
+    else:
+        text_encoders = [text_encoder]
+        use_index = False
+
+    for idx, te in enumerate(text_encoders):
+        if use_index:
+            prefix = f"{LycorisNetworkKohya.LORA_PREFIX_TEXT_ENCODER}{idx+1}"
+        else:
+            prefix = LycorisNetworkKohya.LORA_PREFIX_TEXT_ENCODER
+        for name, modules in te.named_modules():
+            lora_name = f"{prefix}_{name}".replace(".", "_")
+            if lora_name in te_loras:
+                te_loras[lora_name] = modules
+
+    network = LycorisNetworkKohya(text_encoder, unet)
+    network.unet_loras = []
+    network.text_encoder_loras = []
+
+    for lora_name, orig_modules in unet_loras.items():
+        if orig_modules is None:
+            continue
+        lyco_type, params = get_module(weights_sd, lora_name)
+        module = make_module(lyco_type, params, lora_name, orig_modules)
+        if module is not None:
+            network.unet_loras.append(module)
+
+    for lora_name, orig_modules in te_loras.items():
+        if orig_modules is None:
+            continue
+        lyco_type, params = get_module(weights_sd, lora_name)
+        module = make_module(lyco_type, params, lora_name, orig_modules)
+        if module is not None:
+            network.text_encoder_loras.append(module)
+
+    for lora in network.unet_loras + network.text_encoder_loras:
+        lora.multiplier = multiplier
+
+    return network, weights_sd
+
+
+class LycorisNetworkKohya(LycorisNetwork):
+    """
+    LoRA + LoCon
+    """
+
+    # Ignore proj_in or proj_out, their channels is only a few.
+    ENABLE_CONV = True
+    UNET_TARGET_REPLACE_MODULE = [
+        "Transformer2DModel",
+        "ResnetBlock2D",
+        "Downsample2D",
+        "Upsample2D",
+    ]
+    UNET_TARGET_REPLACE_NAME = [
+        "conv_in",
+        "conv_out",
+        "time_embedding.linear_1",
+        "time_embedding.linear_2",
+    ]
+    TEXT_ENCODER_TARGET_REPLACE_MODULE = ["CLIPAttention", "CLIPMLP"]
+    TEXT_ENCODER_TARGET_REPLACE_NAME = []
+    LORA_PREFIX_UNET = "lora_unet"
+    LORA_PREFIX_TEXT_ENCODER = "lora_te"
+    MODULE_ALGO_MAP = {}
+    NAME_ALGO_MAP = {}
+
+    @classmethod
+    def apply_preset(cls, preset):
+        if "enable_conv" in preset:
+            cls.ENABLE_CONV = preset["enable_conv"]
+        if "unet_target_module" in preset:
+            cls.UNET_TARGET_REPLACE_MODULE = preset["unet_target_module"]
+        if "unet_target_name" in preset:
+            cls.UNET_TARGET_REPLACE_NAME = preset["unet_target_name"]
+        if "text_encoder_target_module" in preset:
+            cls.TEXT_ENCODER_TARGET_REPLACE_MODULE = preset[
+                "text_encoder_target_module"
+            ]
+        if "text_encoder_target_name" in preset:
+            cls.TEXT_ENCODER_TARGET_REPLACE_NAME = preset["text_encoder_target_name"]
+        if "module_algo_map" in preset:
+            cls.MODULE_ALGO_MAP = preset["module_algo_map"]
+        if "name_algo_map" in preset:
+            cls.NAME_ALGO_MAP = preset["name_algo_map"]
+        return cls
+
+    def __init__(
+        self,
+        text_encoder,
+        unet,
+        multiplier=1.0,
+        lora_dim=4,
+        conv_lora_dim=4,
+        alpha=1,
+        conv_alpha=1,
+        use_tucker=False,
+        dropout=0,
+        rank_dropout=0,
+        module_dropout=0,
+        network_module: str = "locon",
+        norm_modules=NormModule,
+        train_norm=False,
+        **kwargs,
+    ) -> None:
+        torch.nn.Module.__init__(self)
+        root_kwargs = kwargs
+        self.multiplier = multiplier
+        self.lora_dim = lora_dim
+
+        if not self.ENABLE_CONV:
+            conv_lora_dim = 0
+
+        self.conv_lora_dim = int(conv_lora_dim)
+        if self.conv_lora_dim and self.conv_lora_dim != self.lora_dim:
+            logger.info("Apply different lora dim for conv layer")
+            logger.info(f"Conv Dim: {conv_lora_dim}, Linear Dim: {lora_dim}")
+        elif self.conv_lora_dim == 0:
+            logger.info("Disable conv layer")
+
+        self.alpha = alpha
+        self.conv_alpha = float(conv_alpha)
+        if self.conv_lora_dim and self.alpha != self.conv_alpha:
+            logger.info("Apply different alpha value for conv layer")
+            logger.info(f"Conv alpha: {conv_alpha}, Linear alpha: {alpha}")
+
+        if 1 >= dropout >= 0:
+            logger.info(f"Use Dropout value: {dropout}")
+        self.dropout = dropout
+        self.rank_dropout = rank_dropout
+        self.module_dropout = module_dropout
+
+        self.use_tucker = use_tucker
+
+        def create_single_module(
+            lora_name: str,
+            module: torch.nn.Module,
+            algo_name,
+            dim=None,
+            alpha=None,
+            use_tucker=self.use_tucker,
+            **kwargs,
+        ):
+            for k, v in root_kwargs.items():
+                if k in kwargs:
+                    continue
+                kwargs[k] = v
+
+            if train_norm and "Norm" in module.__class__.__name__:
+                return norm_modules(
+                    lora_name,
+                    module,
+                    self.multiplier,
+                    self.rank_dropout,
+                    self.module_dropout,
+                    **kwargs,
+                )
+            lora = None
+            if isinstance(module, torch.nn.Linear) and lora_dim > 0:
+                dim = dim or lora_dim
+                alpha = alpha or self.alpha
+            elif isinstance(module, torch.nn.Conv2d):
+                k_size, *_ = module.kernel_size
+                if k_size == 1 and lora_dim > 0:
+                    dim = dim or lora_dim
+                    alpha = alpha or self.alpha
+                elif conv_lora_dim > 0 or dim:
+                    dim = dim or conv_lora_dim
+                    alpha = alpha or self.conv_alpha
+                else:
+                    return None
+            else:
+                return None
+            lora = network_module_dict[algo_name](
+                lora_name,
+                module,
+                self.multiplier,
+                dim,
+                alpha,
+                self.dropout,
+                self.rank_dropout,
+                self.module_dropout,
+                use_tucker,
+                **kwargs,
+            )
+            return lora
+
+        def create_modules_(
+            prefix: str,
+            root_module: torch.nn.Module,
+            algo,
+            configs={},
+        ):
+            loras = {}
+            lora_names = []
+            for name, module in root_module.named_modules():
+                if module is root_module:
+                    continue
+                module_name = module.__class__.__name__
+                if module_name in self.MODULE_ALGO_MAP:
+                    next_config = self.MODULE_ALGO_MAP[module_name]
+                    next_algo = next_config.get("algo", algo)
+                    new_loras, new_lora_names = create_modules_(
+                        f"{prefix}_{name}", module, next_algo, next_config
+                    )
+                    for lora_name, lora in zip(new_lora_names, new_loras):
+                        if lora_name not in loras:
+                            loras[lora_name] = lora
+                            lora_names.append(lora_name)
+                    continue
+                lora_name = prefix + "." + name
+                lora_name = lora_name.replace(".", "_")
+                if lora_name in loras:
+                    continue
+
+                lora = create_single_module(lora_name, module, algo, **configs)
+                if lora is not None:
+                    loras[lora_name] = lora
+                    lora_names.append(lora_name)
+            return [loras[lora_name] for lora_name in lora_names], lora_names
+
+        # create module instances
+        def create_modules(
+            prefix,
+            root_module: torch.nn.Module,
+            target_replace_modules,
+            target_replace_names=[],
+        ) -> List:
+            logger.info("Create LyCORIS Module")
+            loras = []
+            next_config = {}
+            for name, module in root_module.named_modules():
+                module_name = module.__class__.__name__
+                if module_name in target_replace_modules:
+                    if module_name in self.MODULE_ALGO_MAP:
+                        next_config = self.MODULE_ALGO_MAP[module_name]
+                        algo = next_config.get("algo", network_module)
+                    else:
+                        algo = network_module
+                    loras.extend(
+                        create_modules_(f"{prefix}_{name}", module, algo, next_config)[
+                            0
+                        ]
+                    )
+                    next_config = {}
+                elif name in target_replace_names or any(
+                    re.match(t, name) for t in target_replace_names
+                ):
+                    if name in self.NAME_ALGO_MAP:
+                        next_config = self.NAME_ALGO_MAP[name]
+                        algo = next_config.get("algo", network_module)
+                    elif module_name in self.MODULE_ALGO_MAP:
+                        next_config = self.MODULE_ALGO_MAP[module_name]
+                        algo = next_config.get("algo", network_module)
+                    else:
+                        algo = network_module
+                    lora_name = prefix + "." + name
+                    lora_name = lora_name.replace(".", "_")
+                    lora = create_single_module(lora_name, module, algo, **next_config)
+                    next_config = {}
+                    if lora is not None:
+                        loras.append(lora)
+            return loras
+
+        if network_module == GLoRAModule:
+            logger.info("GLoRA enabled, only train transformer")
+            # only train transformer (for GLoRA)
+            LycorisNetworkKohya.UNET_TARGET_REPLACE_MODULE = [
+                "Transformer2DModel",
+                "Attention",
+            ]
+            LycorisNetworkKohya.UNET_TARGET_REPLACE_NAME = []
+
+        if isinstance(text_encoder, list):
+            text_encoders = text_encoder
+            use_index = True
+        else:
+            text_encoders = [text_encoder]
+            use_index = False
+
+        self.text_encoder_loras = []
+        for i, te in enumerate(text_encoders):
+            self.text_encoder_loras.extend(
+                create_modules(
+                    LycorisNetworkKohya.LORA_PREFIX_TEXT_ENCODER
+                    + (f"{i+1}" if use_index else ""),
+                    te,
+                    LycorisNetworkKohya.TEXT_ENCODER_TARGET_REPLACE_MODULE,
+                    LycorisNetworkKohya.TEXT_ENCODER_TARGET_REPLACE_NAME,
+                )
+            )
+        logger.info(
+            f"create LyCORIS for Text Encoder: {len(self.text_encoder_loras)} modules."
+        )
+
+        self.unet_loras = create_modules(
+            LycorisNetworkKohya.LORA_PREFIX_UNET,
+            unet,
+            LycorisNetworkKohya.UNET_TARGET_REPLACE_MODULE,
+            LycorisNetworkKohya.UNET_TARGET_REPLACE_NAME,
+        )
+        logger.info(f"create LyCORIS for U-Net: {len(self.unet_loras)} modules.")
+
+        algo_table = {}
+        for lora in self.text_encoder_loras + self.unet_loras:
+            algo_table[lora.__class__.__name__] = (
+                algo_table.get(lora.__class__.__name__, 0) + 1
+            )
+        logger.info(f"module type table: {algo_table}")
+
+        self.weights_sd = None
+
+        self.loras = self.text_encoder_loras + self.unet_loras
+        # assertion
+        names = set()
+        for lora in self.loras:
+            assert (
+                lora.lora_name not in names
+            ), f"duplicated lora name: {lora.lora_name}"
+            names.add(lora.lora_name)
+
+    def load_weights(self, file):
+        if os.path.splitext(file)[1] == ".safetensors":
+            from safetensors.torch import load_file, safe_open
+
+            self.weights_sd = load_file(file)
+        else:
+            self.weights_sd = torch.load(file, map_location="cpu")
+        missing, unexpected = self.load_state_dict(self.weights_sd, strict=False)
+        state = {}
+        if missing:
+            state["missing keys"] = missing
+        if unexpected:
+            state["unexpected keys"] = unexpected
+        return state
+
+    def apply_to(self, text_encoder, unet, apply_text_encoder=None, apply_unet=None):
+        assert (
+            apply_text_encoder is not None and apply_unet is not None
+        ), f"internal error: flag not set"
+
+        if apply_text_encoder:
+            logger.info("enable LyCORIS for text encoder")
+        else:
+            self.text_encoder_loras = []
+
+        if apply_unet:
+            logger.info("enable LyCORIS for U-Net")
+        else:
+            self.unet_loras = []
+
+        self.loras = self.text_encoder_loras + self.unet_loras
+
+        for lora in self.loras:
+            lora.apply_to()
+            self.add_module(lora.lora_name, lora)
+
+        if self.weights_sd:
+            # if some weights are not in state dict, it is ok because initial LoRA does nothing (lora_up is initialized by zeros)
+            info = self.load_state_dict(self.weights_sd, False)
+            logger.info(f"weights are loaded: {info}")
+
+    # TODO refactor to common function with apply_to
+    def merge_to(self, text_encoder, unet, weights_sd, dtype, device):
+        apply_text_encoder = apply_unet = False
+        for key in weights_sd.keys():
+            if key.startswith(LycorisNetworkKohya.LORA_PREFIX_TEXT_ENCODER):
+                apply_text_encoder = True
+            elif key.startswith(LycorisNetworkKohya.LORA_PREFIX_UNET):
+                apply_unet = True
+
+        if apply_text_encoder:
+            logger.info("enable LoRA for text encoder")
+        else:
+            self.text_encoder_loras = []
+
+        if apply_unet:
+            logger.info("enable LoRA for U-Net")
+        else:
+            self.unet_loras = []
+
+        self.loras = self.text_encoder_loras + self.unet_loras
+        super().merge_to(1)
+
+    def prepare_optimizer_params(self, text_encoder_lr, unet_lr, learning_rate):
+        def enumerate_params(loras):
+            params = []
+            for lora in loras:
+                params.extend(lora.parameters())
+            return params
+
+        self.requires_grad_(True)
+        all_params = []
+
+        if self.text_encoder_loras:
+            param_data = {"params": enumerate_params(self.text_encoder_loras)}
+            if text_encoder_lr is not None:
+                param_data["lr"] = text_encoder_lr
+            all_params.append(param_data)
+
+        if self.unet_loras:
+            param_data = {"params": enumerate_params(self.unet_loras)}
+            if unet_lr is not None:
+                param_data["lr"] = unet_lr
+            all_params.append(param_data)
+
+        return all_params
+
+    def save_weights(self, file, dtype, metadata):
+        if metadata is not None and len(metadata) == 0:
+            metadata = None
+
+        state_dict = self.state_dict()
+
+        if dtype is not None:
+            for key in list(state_dict.keys()):
+                v = state_dict[key]
+                v = v.detach().clone().to("cpu").to(dtype)
+                state_dict[key] = v
+
+        if os.path.splitext(file)[1] == ".safetensors":
+            from safetensors.torch import save_file
+
+            # Precalculate model hashes to save time on indexing
+            if metadata is None:
+                metadata = {}
+            model_hash, legacy_hash = precalculate_safetensors_hashes(
+                state_dict, metadata
+            )
+            metadata["sshs_model_hash"] = model_hash
+            metadata["sshs_legacy_hash"] = legacy_hash
+
+            save_file(state_dict, file, metadata)
+        else:
+            torch.save(state_dict, file)
+
+
+class IA3Network(torch.nn.Module):
+    """
+    IA3 network
+    """
+
+    # Ignore proj_in or proj_out, their channels is only a few.
+    UNET_TARGET_REPLACE_MODULE = []
+    UNET_TARGET_REPLACE_NAME = ["to_k", "to_v", "ff.net.2"]
+    TEXT_ENCODER_TARGET_REPLACE_MODULE = []
+    TEXT_ENCODER_TARGET_REPLACE_NAME = ["k_proj", "v_proj", "mlp.fc2"]
+    TRAIN_INPUT = ["mlp.fc2", "ff.net.2"]
+    LORA_PREFIX_UNET = "lora_unet"
+    LORA_PREFIX_TEXT_ENCODER = "lora_te"
+
+    def __init__(
+        self,
+        text_encoder,
+        unet,
+        multiplier=1.0,
+        **kwargs,
+    ) -> None:
+        super().__init__()
+        self.multiplier = multiplier
+
+        # create module instances
+        def create_modules(
+            prefix,
+            root_module: torch.nn.Module,
+            target_replace_modules,
+            target_replace_names=[],
+            target_train_input=[],
+        ) -> List[IA3Module]:
+            logger.info("Create LyCORIS Module")
+            loras = []
+            for name, module in root_module.named_modules():
+                if module.__class__.__name__ in target_replace_modules:
+                    for child_name, child_module in module.named_modules():
+                        lora_name = prefix + "." + name + "." + child_name
+                        lora_name = lora_name.replace(".", "_")
+                        if child_module.__class__.__name__ in {"Linear", "Conv2d"}:
+                            lora = IA3Module(
+                                lora_name,
+                                child_module,
+                                self.multiplier,
+                                name in target_train_input,
+                                **kwargs,
+                            )
+                            loras.append(lora)
+                elif any(i in name for i in target_replace_names):
+                    lora_name = prefix + "." + name
+                    lora_name = lora_name.replace(".", "_")
+                    if module.__class__.__name__ in {"Linear", "Conv2d"}:
+                        lora = IA3Module(
+                            lora_name,
+                            module,
+                            self.multiplier,
+                            name in target_train_input,
+                            **kwargs,
+                        )
+                        loras.append(lora)
+            return loras
+
+        if isinstance(text_encoder, list):
+            text_encoders = text_encoder
+            use_index = True
+        else:
+            text_encoders = [text_encoder]
+            use_index = False
+
+        self.text_encoder_loras = []
+        for i, te in enumerate(text_encoders):
+            self.text_encoder_loras.extend(
+                create_modules(
+                    IA3Network.LORA_PREFIX_TEXT_ENCODER
+                    + (f"{i+1}" if use_index else ""),
+                    te,
+                    IA3Network.TEXT_ENCODER_TARGET_REPLACE_MODULE,
+                    IA3Network.TEXT_ENCODER_TARGET_REPLACE_NAME,
+                    IA3Network.TRAIN_INPUT,
+                )
+            )
+        logger.info(
+            f"create LyCORIS for Text Encoder: {len(self.text_encoder_loras)} modules."
+        )
+
+        self.unet_loras = create_modules(
+            IA3Network.LORA_PREFIX_UNET,
+            unet,
+            IA3Network.UNET_TARGET_REPLACE_MODULE,
+            IA3Network.UNET_TARGET_REPLACE_NAME,
+            IA3Network.TRAIN_INPUT,
+        )
+        logger.info(f"create LyCORIS for U-Net: {len(self.unet_loras)} modules.")
+
+        self.weights_sd = None
+
+        # assertion
+        names = set()
+        for lora in self.text_encoder_loras + self.unet_loras:
+            assert (
+                lora.lora_name not in names
+            ), f"duplicated lora name: {lora.lora_name}"
+            names.add(lora.lora_name)
+
+    def set_multiplier(self, multiplier):
+        self.multiplier = multiplier
+        for lora in self.text_encoder_loras + self.unet_loras:
+            lora.multiplier = self.multiplier
+
+    def load_weights(self, file):
+        if os.path.splitext(file)[1] == ".safetensors":
+            from safetensors.torch import load_file, safe_open
+
+            self.weights_sd = load_file(file)
+        else:
+            self.weights_sd = torch.load(file, map_location="cpu")
+
+    def apply_to(self, text_encoder, unet, apply_text_encoder=None, apply_unet=None):
+        if self.weights_sd:
+            weights_has_text_encoder = weights_has_unet = False
+            for key in self.weights_sd.keys():
+                if key.startswith(LycorisNetworkKohya.LORA_PREFIX_TEXT_ENCODER):
+                    weights_has_text_encoder = True
+                elif key.startswith(LycorisNetworkKohya.LORA_PREFIX_UNET):
+                    weights_has_unet = True
+
+            if apply_text_encoder is None:
+                apply_text_encoder = weights_has_text_encoder
+            else:
+                assert (
+                    apply_text_encoder == weights_has_text_encoder
+                ), f"text encoder weights: {weights_has_text_encoder} but text encoder flag: {apply_text_encoder} / 重みとText Encoderのフラグが矛盾しています"
+
+            if apply_unet is None:
+                apply_unet = weights_has_unet
+            else:
+                assert (
+                    apply_unet == weights_has_unet
+                ), f"u-net weights: {weights_has_unet} but u-net flag: {apply_unet} / 重みとU-Netのフラグが矛盾しています"
+        else:
+            assert (
+                apply_text_encoder is not None and apply_unet is not None
+            ), f"internal error: flag not set"
+
+        if apply_text_encoder:
+            logger.info("enable LyCORIS for text encoder")
+        else:
+            self.text_encoder_loras = []
+
+        if apply_unet:
+            logger.info("enable LyCORIS for U-Net")
+        else:
+            self.unet_loras = []
+
+        for lora in self.text_encoder_loras + self.unet_loras:
+            lora.apply_to()
+            self.add_module(lora.lora_name, lora)
+
+        if self.weights_sd:
+            # if some weights are not in state dict, it is ok because initial LoRA does nothing (lora_up is initialized by zeros)
+            info = self.load_state_dict(self.weights_sd, False)
+            logger.info(f"weights are loaded: {info}")
+
+    def enable_gradient_checkpointing(self):
+        # not supported
+        def make_ckpt(module):
+            if isinstance(module, torch.nn.Module):
+                module.grad_ckpt = True
+
+        self.apply(make_ckpt)
+        pass
+
+    def prepare_optimizer_params(self, text_encoder_lr, unet_lr, learning_rate):
+        def enumerate_params(loras):
+            params = []
+            for lora in loras:
+                params.extend(lora.parameters())
+            return params
+
+        self.requires_grad_(True)
+        all_params = []
+
+        if self.text_encoder_loras:
+            param_data = {"params": enumerate_params(self.text_encoder_loras)}
+            if text_encoder_lr is not None:
+                param_data["lr"] = text_encoder_lr
+            all_params.append(param_data)
+
+        if self.unet_loras:
+            param_data = {"params": enumerate_params(self.unet_loras)}
+            if unet_lr is not None:
+                param_data["lr"] = unet_lr
+            all_params.append(param_data)
+
+        return all_params
+
+    def prepare_grad_etc(self, text_encoder, unet):
+        self.requires_grad_(True)
+
+    def on_epoch_start(self, text_encoder, unet):
+        self.train()
+
+    def get_trainable_params(self):
+        return self.parameters()
+
+    def save_weights(self, file, dtype, metadata):
+        if metadata is not None and len(metadata) == 0:
+            metadata = None
+
+        state_dict = self.state_dict()
+
+        if dtype is not None:
+            for key in list(state_dict.keys()):
+                v = state_dict[key]
+                v = v.detach().clone().to("cpu").to(dtype)
+                state_dict[key] = v
+
+        if os.path.splitext(file)[1] == ".safetensors":
+            from safetensors.torch import save_file
+
+            # Precalculate model hashes to save time on indexing
+            if metadata is None:
+                metadata = {}
+            model_hash, legacy_hash = precalculate_safetensors_hashes(
+                state_dict, metadata
+            )
+            metadata["sshs_model_hash"] = model_hash
+            metadata["sshs_legacy_hash"] = legacy_hash
+
+            save_file(state_dict, file, metadata)
+        else:
+            torch.save(state_dict, file)
```

### Comparing `lycoris_lora-2.3.0.dev4/lycoris/kohya/model_utils.py` & `lycoris_lora-2.3.0.dev5/lycoris/kohya/model_utils.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,1633 +1,1633 @@
-# https://github.com/kohya-ss/sd-scripts/blob/b78c0e2a69e52ce6c79abc6c8c82d1a9cabcf05c/library/model_util.py
-# v1: split from train_db_fixed.py.
-# v2: support safetensors
-
-import math
-import os
-import torch
-import diffusers
-from transformers import CLIPTextModel, CLIPTokenizer, CLIPTextConfig, logging
-from diffusers import (
-    AutoencoderKL,
-    DDIMScheduler,
-    StableDiffusionPipeline,
-)  # , UNet2DConditionModel
-from safetensors.torch import load_file, save_file
-from .original_unet import UNet2DConditionModel
-
-# DiffUsers版StableDiffusionのモデルパラメータ
-NUM_TRAIN_TIMESTEPS = 1000
-BETA_START = 0.00085
-BETA_END = 0.0120
-
-UNET_PARAMS_MODEL_CHANNELS = 320
-UNET_PARAMS_CHANNEL_MULT = [1, 2, 4, 4]
-UNET_PARAMS_ATTENTION_RESOLUTIONS = [4, 2, 1]
-UNET_PARAMS_IMAGE_SIZE = 64  # fixed from old invalid value `32`
-UNET_PARAMS_IN_CHANNELS = 4
-UNET_PARAMS_OUT_CHANNELS = 4
-UNET_PARAMS_NUM_RES_BLOCKS = 2
-UNET_PARAMS_CONTEXT_DIM = 768
-UNET_PARAMS_NUM_HEADS = 8
-# UNET_PARAMS_USE_LINEAR_PROJECTION = False
-
-VAE_PARAMS_Z_CHANNELS = 4
-VAE_PARAMS_RESOLUTION = 256
-VAE_PARAMS_IN_CHANNELS = 3
-VAE_PARAMS_OUT_CH = 3
-VAE_PARAMS_CH = 128
-VAE_PARAMS_CH_MULT = [1, 2, 4, 4]
-VAE_PARAMS_NUM_RES_BLOCKS = 2
-
-# V2
-V2_UNET_PARAMS_ATTENTION_HEAD_DIM = [5, 10, 20, 20]
-V2_UNET_PARAMS_CONTEXT_DIM = 1024
-# V2_UNET_PARAMS_USE_LINEAR_PROJECTION = True
-
-# Diffusersの設定を読み込むための参照モデル
-DIFFUSERS_REF_MODEL_ID_V1 = "runwayml/stable-diffusion-v1-5"
-DIFFUSERS_REF_MODEL_ID_V2 = "stabilityai/stable-diffusion-2-1"
-
-
-# region StableDiffusion->Diffusersの変換コード
-# convert_original_stable_diffusion_to_diffusers をコピーして修正している（ASL 2.0）
-
-
-def shave_segments(path, n_shave_prefix_segments=1):
-    """
-    Removes segments. Positive values shave the first segments, negative shave the last segments.
-    """
-    if n_shave_prefix_segments >= 0:
-        return ".".join(path.split(".")[n_shave_prefix_segments:])
-    else:
-        return ".".join(path.split(".")[:n_shave_prefix_segments])
-
-
-def renew_resnet_paths(old_list, n_shave_prefix_segments=0):
-    """
-    Updates paths inside resnets to the new naming scheme (local renaming)
-    """
-    mapping = []
-    for old_item in old_list:
-        new_item = old_item.replace("in_layers.0", "norm1")
-        new_item = new_item.replace("in_layers.2", "conv1")
-
-        new_item = new_item.replace("out_layers.0", "norm2")
-        new_item = new_item.replace("out_layers.3", "conv2")
-
-        new_item = new_item.replace("emb_layers.1", "time_emb_proj")
-        new_item = new_item.replace("skip_connection", "conv_shortcut")
-
-        new_item = shave_segments(
-            new_item, n_shave_prefix_segments=n_shave_prefix_segments
-        )
-
-        mapping.append({"old": old_item, "new": new_item})
-
-    return mapping
-
-
-def renew_vae_resnet_paths(old_list, n_shave_prefix_segments=0):
-    """
-    Updates paths inside resnets to the new naming scheme (local renaming)
-    """
-    mapping = []
-    for old_item in old_list:
-        new_item = old_item
-
-        new_item = new_item.replace("nin_shortcut", "conv_shortcut")
-        new_item = shave_segments(
-            new_item, n_shave_prefix_segments=n_shave_prefix_segments
-        )
-
-        mapping.append({"old": old_item, "new": new_item})
-
-    return mapping
-
-
-def renew_attention_paths(old_list, n_shave_prefix_segments=0):
-    """
-    Updates paths inside attentions to the new naming scheme (local renaming)
-    """
-    mapping = []
-    for old_item in old_list:
-        new_item = old_item
-
-        #         new_item = new_item.replace('norm.weight', 'group_norm.weight')
-        #         new_item = new_item.replace('norm.bias', 'group_norm.bias')
-
-        #         new_item = new_item.replace('proj_out.weight', 'proj_attn.weight')
-        #         new_item = new_item.replace('proj_out.bias', 'proj_attn.bias')
-
-        #         new_item = shave_segments(new_item, n_shave_prefix_segments=n_shave_prefix_segments)
-
-        mapping.append({"old": old_item, "new": new_item})
-
-    return mapping
-
-
-def renew_vae_attention_paths(old_list, n_shave_prefix_segments=0):
-    """
-    Updates paths inside attentions to the new naming scheme (local renaming)
-    """
-    mapping = []
-    for old_item in old_list:
-        new_item = old_item
-
-        new_item = new_item.replace("norm.weight", "group_norm.weight")
-        new_item = new_item.replace("norm.bias", "group_norm.bias")
-
-        if diffusers.__version__ < "0.17.0":
-            new_item = new_item.replace("q.weight", "query.weight")
-            new_item = new_item.replace("q.bias", "query.bias")
-
-            new_item = new_item.replace("k.weight", "key.weight")
-            new_item = new_item.replace("k.bias", "key.bias")
-
-            new_item = new_item.replace("v.weight", "value.weight")
-            new_item = new_item.replace("v.bias", "value.bias")
-
-            new_item = new_item.replace("proj_out.weight", "proj_attn.weight")
-            new_item = new_item.replace("proj_out.bias", "proj_attn.bias")
-        else:
-            new_item = new_item.replace("q.weight", "to_q.weight")
-            new_item = new_item.replace("q.bias", "to_q.bias")
-
-            new_item = new_item.replace("k.weight", "to_k.weight")
-            new_item = new_item.replace("k.bias", "to_k.bias")
-
-            new_item = new_item.replace("v.weight", "to_v.weight")
-            new_item = new_item.replace("v.bias", "to_v.bias")
-
-            new_item = new_item.replace("proj_out.weight", "to_out.0.weight")
-            new_item = new_item.replace("proj_out.bias", "to_out.0.bias")
-
-        new_item = shave_segments(
-            new_item, n_shave_prefix_segments=n_shave_prefix_segments
-        )
-
-        mapping.append({"old": old_item, "new": new_item})
-
-    return mapping
-
-
-def assign_to_checkpoint(
-    paths,
-    checkpoint,
-    old_checkpoint,
-    attention_paths_to_split=None,
-    additional_replacements=None,
-    config=None,
-):
-    """
-    This does the final conversion step: take locally converted weights and apply a global renaming
-    to them. It splits attention layers, and takes into account additional replacements
-    that may arise.
-
-    Assigns the weights to the new checkpoint.
-    """
-    assert isinstance(
-        paths, list
-    ), "Paths should be a list of dicts containing 'old' and 'new' keys."
-
-    # Splits the attention layers into three variables.
-    if attention_paths_to_split is not None:
-        for path, path_map in attention_paths_to_split.items():
-            old_tensor = old_checkpoint[path]
-            channels = old_tensor.shape[0] // 3
-
-            target_shape = (-1, channels) if len(old_tensor.shape) == 3 else (-1)
-
-            num_heads = old_tensor.shape[0] // config["num_head_channels"] // 3
-
-            old_tensor = old_tensor.reshape(
-                (num_heads, 3 * channels // num_heads) + old_tensor.shape[1:]
-            )
-            query, key, value = old_tensor.split(channels // num_heads, dim=1)
-
-            checkpoint[path_map["query"]] = query.reshape(target_shape)
-            checkpoint[path_map["key"]] = key.reshape(target_shape)
-            checkpoint[path_map["value"]] = value.reshape(target_shape)
-
-    for path in paths:
-        new_path = path["new"]
-
-        # These have already been assigned
-        if (
-            attention_paths_to_split is not None
-            and new_path in attention_paths_to_split
-        ):
-            continue
-
-        # Global renaming happens here
-        new_path = new_path.replace("middle_block.0", "mid_block.resnets.0")
-        new_path = new_path.replace("middle_block.1", "mid_block.attentions.0")
-        new_path = new_path.replace("middle_block.2", "mid_block.resnets.1")
-
-        if additional_replacements is not None:
-            for replacement in additional_replacements:
-                new_path = new_path.replace(replacement["old"], replacement["new"])
-
-        # proj_attn.weight has to be converted from conv 1D to linear
-        reshaping = False
-        if diffusers.__version__ < "0.17.0":
-            if "proj_attn.weight" in new_path:
-                reshaping = True
-        else:
-            if (
-                ".attentions." in new_path
-                and ".0.to_" in new_path
-                and old_checkpoint[path["old"]].ndim > 2
-            ):
-                reshaping = True
-
-        if reshaping:
-            checkpoint[new_path] = old_checkpoint[path["old"]][:, :, 0, 0]
-        else:
-            checkpoint[new_path] = old_checkpoint[path["old"]]
-
-
-def conv_attn_to_linear(checkpoint):
-    keys = list(checkpoint.keys())
-    attn_keys = ["query.weight", "key.weight", "value.weight"]
-    for key in keys:
-        if ".".join(key.split(".")[-2:]) in attn_keys:
-            if checkpoint[key].ndim > 2:
-                checkpoint[key] = checkpoint[key][:, :, 0, 0]
-        elif "proj_attn.weight" in key:
-            if checkpoint[key].ndim > 2:
-                checkpoint[key] = checkpoint[key][:, :, 0]
-
-
-def linear_transformer_to_conv(checkpoint):
-    keys = list(checkpoint.keys())
-    tf_keys = ["proj_in.weight", "proj_out.weight"]
-    for key in keys:
-        if ".".join(key.split(".")[-2:]) in tf_keys:
-            if checkpoint[key].ndim == 2:
-                checkpoint[key] = checkpoint[key].unsqueeze(2).unsqueeze(2)
-
-
-def convert_ldm_unet_checkpoint(v2, checkpoint, config):
-    """
-    Takes a state dict and a config, and returns a converted checkpoint.
-    """
-
-    # extract state_dict for UNet
-    unet_state_dict = {}
-    unet_key = "model.diffusion_model."
-    keys = list(checkpoint.keys())
-    for key in keys:
-        if key.startswith(unet_key):
-            unet_state_dict[key.replace(unet_key, "")] = checkpoint.pop(key)
-
-    new_checkpoint = {}
-
-    new_checkpoint["time_embedding.linear_1.weight"] = unet_state_dict[
-        "time_embed.0.weight"
-    ]
-    new_checkpoint["time_embedding.linear_1.bias"] = unet_state_dict[
-        "time_embed.0.bias"
-    ]
-    new_checkpoint["time_embedding.linear_2.weight"] = unet_state_dict[
-        "time_embed.2.weight"
-    ]
-    new_checkpoint["time_embedding.linear_2.bias"] = unet_state_dict[
-        "time_embed.2.bias"
-    ]
-
-    new_checkpoint["conv_in.weight"] = unet_state_dict["input_blocks.0.0.weight"]
-    new_checkpoint["conv_in.bias"] = unet_state_dict["input_blocks.0.0.bias"]
-
-    new_checkpoint["conv_norm_out.weight"] = unet_state_dict["out.0.weight"]
-    new_checkpoint["conv_norm_out.bias"] = unet_state_dict["out.0.bias"]
-    new_checkpoint["conv_out.weight"] = unet_state_dict["out.2.weight"]
-    new_checkpoint["conv_out.bias"] = unet_state_dict["out.2.bias"]
-
-    # Retrieves the keys for the input blocks only
-    num_input_blocks = len(
-        {
-            ".".join(layer.split(".")[:2])
-            for layer in unet_state_dict
-            if "input_blocks" in layer
-        }
-    )
-    input_blocks = {
-        layer_id: [key for key in unet_state_dict if f"input_blocks.{layer_id}." in key]
-        for layer_id in range(num_input_blocks)
-    }
-
-    # Retrieves the keys for the middle blocks only
-    num_middle_blocks = len(
-        {
-            ".".join(layer.split(".")[:2])
-            for layer in unet_state_dict
-            if "middle_block" in layer
-        }
-    )
-    middle_blocks = {
-        layer_id: [key for key in unet_state_dict if f"middle_block.{layer_id}." in key]
-        for layer_id in range(num_middle_blocks)
-    }
-
-    # Retrieves the keys for the output blocks only
-    num_output_blocks = len(
-        {
-            ".".join(layer.split(".")[:2])
-            for layer in unet_state_dict
-            if "output_blocks" in layer
-        }
-    )
-    output_blocks = {
-        layer_id: [
-            key for key in unet_state_dict if f"output_blocks.{layer_id}." in key
-        ]
-        for layer_id in range(num_output_blocks)
-    }
-
-    for i in range(1, num_input_blocks):
-        block_id = (i - 1) // (config["layers_per_block"] + 1)
-        layer_in_block_id = (i - 1) % (config["layers_per_block"] + 1)
-
-        resnets = [
-            key
-            for key in input_blocks[i]
-            if f"input_blocks.{i}.0" in key and f"input_blocks.{i}.0.op" not in key
-        ]
-        attentions = [key for key in input_blocks[i] if f"input_blocks.{i}.1" in key]
-
-        if f"input_blocks.{i}.0.op.weight" in unet_state_dict:
-            new_checkpoint[f"down_blocks.{block_id}.downsamplers.0.conv.weight"] = (
-                unet_state_dict.pop(f"input_blocks.{i}.0.op.weight")
-            )
-            new_checkpoint[f"down_blocks.{block_id}.downsamplers.0.conv.bias"] = (
-                unet_state_dict.pop(f"input_blocks.{i}.0.op.bias")
-            )
-
-        paths = renew_resnet_paths(resnets)
-        meta_path = {
-            "old": f"input_blocks.{i}.0",
-            "new": f"down_blocks.{block_id}.resnets.{layer_in_block_id}",
-        }
-        assign_to_checkpoint(
-            paths,
-            new_checkpoint,
-            unet_state_dict,
-            additional_replacements=[meta_path],
-            config=config,
-        )
-
-        if len(attentions):
-            paths = renew_attention_paths(attentions)
-            meta_path = {
-                "old": f"input_blocks.{i}.1",
-                "new": f"down_blocks.{block_id}.attentions.{layer_in_block_id}",
-            }
-            assign_to_checkpoint(
-                paths,
-                new_checkpoint,
-                unet_state_dict,
-                additional_replacements=[meta_path],
-                config=config,
-            )
-
-    resnet_0 = middle_blocks[0]
-    attentions = middle_blocks[1]
-    resnet_1 = middle_blocks[2]
-
-    resnet_0_paths = renew_resnet_paths(resnet_0)
-    assign_to_checkpoint(resnet_0_paths, new_checkpoint, unet_state_dict, config=config)
-
-    resnet_1_paths = renew_resnet_paths(resnet_1)
-    assign_to_checkpoint(resnet_1_paths, new_checkpoint, unet_state_dict, config=config)
-
-    attentions_paths = renew_attention_paths(attentions)
-    meta_path = {"old": "middle_block.1", "new": "mid_block.attentions.0"}
-    assign_to_checkpoint(
-        attentions_paths,
-        new_checkpoint,
-        unet_state_dict,
-        additional_replacements=[meta_path],
-        config=config,
-    )
-
-    for i in range(num_output_blocks):
-        block_id = i // (config["layers_per_block"] + 1)
-        layer_in_block_id = i % (config["layers_per_block"] + 1)
-        output_block_layers = [shave_segments(name, 2) for name in output_blocks[i]]
-        output_block_list = {}
-
-        for layer in output_block_layers:
-            layer_id, layer_name = layer.split(".")[0], shave_segments(layer, 1)
-            if layer_id in output_block_list:
-                output_block_list[layer_id].append(layer_name)
-            else:
-                output_block_list[layer_id] = [layer_name]
-
-        if len(output_block_list) > 1:
-            resnets = [key for key in output_blocks[i] if f"output_blocks.{i}.0" in key]
-            attentions = [
-                key for key in output_blocks[i] if f"output_blocks.{i}.1" in key
-            ]
-
-            resnet_0_paths = renew_resnet_paths(resnets)
-            paths = renew_resnet_paths(resnets)
-
-            meta_path = {
-                "old": f"output_blocks.{i}.0",
-                "new": f"up_blocks.{block_id}.resnets.{layer_in_block_id}",
-            }
-            assign_to_checkpoint(
-                paths,
-                new_checkpoint,
-                unet_state_dict,
-                additional_replacements=[meta_path],
-                config=config,
-            )
-
-            # オリジナル：
-            # if ["conv.weight", "conv.bias"] in output_block_list.values():
-            #   index = list(output_block_list.values()).index(["conv.weight", "conv.bias"])
-
-            # biasとweightの順番に依存しないようにする：もっといいやり方がありそうだが
-            for l in output_block_list.values():
-                l.sort()
-
-            if ["conv.bias", "conv.weight"] in output_block_list.values():
-                index = list(output_block_list.values()).index(
-                    ["conv.bias", "conv.weight"]
-                )
-                new_checkpoint[f"up_blocks.{block_id}.upsamplers.0.conv.bias"] = (
-                    unet_state_dict[f"output_blocks.{i}.{index}.conv.bias"]
-                )
-                new_checkpoint[f"up_blocks.{block_id}.upsamplers.0.conv.weight"] = (
-                    unet_state_dict[f"output_blocks.{i}.{index}.conv.weight"]
-                )
-
-                # Clear attentions as they have been attributed above.
-                if len(attentions) == 2:
-                    attentions = []
-
-            if len(attentions):
-                paths = renew_attention_paths(attentions)
-                meta_path = {
-                    "old": f"output_blocks.{i}.1",
-                    "new": f"up_blocks.{block_id}.attentions.{layer_in_block_id}",
-                }
-                assign_to_checkpoint(
-                    paths,
-                    new_checkpoint,
-                    unet_state_dict,
-                    additional_replacements=[meta_path],
-                    config=config,
-                )
-        else:
-            resnet_0_paths = renew_resnet_paths(
-                output_block_layers, n_shave_prefix_segments=1
-            )
-            for path in resnet_0_paths:
-                old_path = ".".join(["output_blocks", str(i), path["old"]])
-                new_path = ".".join(
-                    [
-                        "up_blocks",
-                        str(block_id),
-                        "resnets",
-                        str(layer_in_block_id),
-                        path["new"],
-                    ]
-                )
-
-                new_checkpoint[new_path] = unet_state_dict[old_path]
-
-    # SDのv2では1*1のconv2dがlinearに変わっている
-    # 誤って Diffusers 側を conv2d のままにしてしまったので、変換必要
-    if v2 and not config.get("use_linear_projection", False):
-        linear_transformer_to_conv(new_checkpoint)
-
-    return new_checkpoint
-
-
-def convert_ldm_vae_checkpoint(checkpoint, config):
-    # extract state dict for VAE
-    vae_state_dict = {}
-    vae_key = "first_stage_model."
-    keys = list(checkpoint.keys())
-    for key in keys:
-        if key.startswith(vae_key):
-            vae_state_dict[key.replace(vae_key, "")] = checkpoint.get(key)
-    # if len(vae_state_dict) == 0:
-    #   # 渡されたcheckpointは.ckptから読み込んだcheckpointではなくvaeのstate_dict
-    #   vae_state_dict = checkpoint
-
-    new_checkpoint = {}
-
-    new_checkpoint["encoder.conv_in.weight"] = vae_state_dict["encoder.conv_in.weight"]
-    new_checkpoint["encoder.conv_in.bias"] = vae_state_dict["encoder.conv_in.bias"]
-    new_checkpoint["encoder.conv_out.weight"] = vae_state_dict[
-        "encoder.conv_out.weight"
-    ]
-    new_checkpoint["encoder.conv_out.bias"] = vae_state_dict["encoder.conv_out.bias"]
-    new_checkpoint["encoder.conv_norm_out.weight"] = vae_state_dict[
-        "encoder.norm_out.weight"
-    ]
-    new_checkpoint["encoder.conv_norm_out.bias"] = vae_state_dict[
-        "encoder.norm_out.bias"
-    ]
-
-    new_checkpoint["decoder.conv_in.weight"] = vae_state_dict["decoder.conv_in.weight"]
-    new_checkpoint["decoder.conv_in.bias"] = vae_state_dict["decoder.conv_in.bias"]
-    new_checkpoint["decoder.conv_out.weight"] = vae_state_dict[
-        "decoder.conv_out.weight"
-    ]
-    new_checkpoint["decoder.conv_out.bias"] = vae_state_dict["decoder.conv_out.bias"]
-    new_checkpoint["decoder.conv_norm_out.weight"] = vae_state_dict[
-        "decoder.norm_out.weight"
-    ]
-    new_checkpoint["decoder.conv_norm_out.bias"] = vae_state_dict[
-        "decoder.norm_out.bias"
-    ]
-
-    new_checkpoint["quant_conv.weight"] = vae_state_dict["quant_conv.weight"]
-    new_checkpoint["quant_conv.bias"] = vae_state_dict["quant_conv.bias"]
-    new_checkpoint["post_quant_conv.weight"] = vae_state_dict["post_quant_conv.weight"]
-    new_checkpoint["post_quant_conv.bias"] = vae_state_dict["post_quant_conv.bias"]
-
-    # Retrieves the keys for the encoder down blocks only
-    num_down_blocks = len(
-        {
-            ".".join(layer.split(".")[:3])
-            for layer in vae_state_dict
-            if "encoder.down" in layer
-        }
-    )
-    down_blocks = {
-        layer_id: [key for key in vae_state_dict if f"down.{layer_id}" in key]
-        for layer_id in range(num_down_blocks)
-    }
-
-    # Retrieves the keys for the decoder up blocks only
-    num_up_blocks = len(
-        {
-            ".".join(layer.split(".")[:3])
-            for layer in vae_state_dict
-            if "decoder.up" in layer
-        }
-    )
-    up_blocks = {
-        layer_id: [key for key in vae_state_dict if f"up.{layer_id}" in key]
-        for layer_id in range(num_up_blocks)
-    }
-
-    for i in range(num_down_blocks):
-        resnets = [
-            key
-            for key in down_blocks[i]
-            if f"down.{i}" in key and f"down.{i}.downsample" not in key
-        ]
-
-        if f"encoder.down.{i}.downsample.conv.weight" in vae_state_dict:
-            new_checkpoint[f"encoder.down_blocks.{i}.downsamplers.0.conv.weight"] = (
-                vae_state_dict.pop(f"encoder.down.{i}.downsample.conv.weight")
-            )
-            new_checkpoint[f"encoder.down_blocks.{i}.downsamplers.0.conv.bias"] = (
-                vae_state_dict.pop(f"encoder.down.{i}.downsample.conv.bias")
-            )
-
-        paths = renew_vae_resnet_paths(resnets)
-        meta_path = {"old": f"down.{i}.block", "new": f"down_blocks.{i}.resnets"}
-        assign_to_checkpoint(
-            paths,
-            new_checkpoint,
-            vae_state_dict,
-            additional_replacements=[meta_path],
-            config=config,
-        )
-
-    mid_resnets = [key for key in vae_state_dict if "encoder.mid.block" in key]
-    num_mid_res_blocks = 2
-    for i in range(1, num_mid_res_blocks + 1):
-        resnets = [key for key in mid_resnets if f"encoder.mid.block_{i}" in key]
-
-        paths = renew_vae_resnet_paths(resnets)
-        meta_path = {"old": f"mid.block_{i}", "new": f"mid_block.resnets.{i - 1}"}
-        assign_to_checkpoint(
-            paths,
-            new_checkpoint,
-            vae_state_dict,
-            additional_replacements=[meta_path],
-            config=config,
-        )
-
-    mid_attentions = [key for key in vae_state_dict if "encoder.mid.attn" in key]
-    paths = renew_vae_attention_paths(mid_attentions)
-    meta_path = {"old": "mid.attn_1", "new": "mid_block.attentions.0"}
-    assign_to_checkpoint(
-        paths,
-        new_checkpoint,
-        vae_state_dict,
-        additional_replacements=[meta_path],
-        config=config,
-    )
-    conv_attn_to_linear(new_checkpoint)
-
-    for i in range(num_up_blocks):
-        block_id = num_up_blocks - 1 - i
-        resnets = [
-            key
-            for key in up_blocks[block_id]
-            if f"up.{block_id}" in key and f"up.{block_id}.upsample" not in key
-        ]
-
-        if f"decoder.up.{block_id}.upsample.conv.weight" in vae_state_dict:
-            new_checkpoint[f"decoder.up_blocks.{i}.upsamplers.0.conv.weight"] = (
-                vae_state_dict[f"decoder.up.{block_id}.upsample.conv.weight"]
-            )
-            new_checkpoint[f"decoder.up_blocks.{i}.upsamplers.0.conv.bias"] = (
-                vae_state_dict[f"decoder.up.{block_id}.upsample.conv.bias"]
-            )
-
-        paths = renew_vae_resnet_paths(resnets)
-        meta_path = {"old": f"up.{block_id}.block", "new": f"up_blocks.{i}.resnets"}
-        assign_to_checkpoint(
-            paths,
-            new_checkpoint,
-            vae_state_dict,
-            additional_replacements=[meta_path],
-            config=config,
-        )
-
-    mid_resnets = [key for key in vae_state_dict if "decoder.mid.block" in key]
-    num_mid_res_blocks = 2
-    for i in range(1, num_mid_res_blocks + 1):
-        resnets = [key for key in mid_resnets if f"decoder.mid.block_{i}" in key]
-
-        paths = renew_vae_resnet_paths(resnets)
-        meta_path = {"old": f"mid.block_{i}", "new": f"mid_block.resnets.{i - 1}"}
-        assign_to_checkpoint(
-            paths,
-            new_checkpoint,
-            vae_state_dict,
-            additional_replacements=[meta_path],
-            config=config,
-        )
-
-    mid_attentions = [key for key in vae_state_dict if "decoder.mid.attn" in key]
-    paths = renew_vae_attention_paths(mid_attentions)
-    meta_path = {"old": "mid.attn_1", "new": "mid_block.attentions.0"}
-    assign_to_checkpoint(
-        paths,
-        new_checkpoint,
-        vae_state_dict,
-        additional_replacements=[meta_path],
-        config=config,
-    )
-    conv_attn_to_linear(new_checkpoint)
-    return new_checkpoint
-
-
-def create_unet_diffusers_config(v2, use_linear_projection_in_v2=False):
-    """
-    Creates a config for the diffusers based on the config of the LDM model.
-    """
-    # unet_params = original_config.model.params.unet_config.params
-
-    block_out_channels = [
-        UNET_PARAMS_MODEL_CHANNELS * mult for mult in UNET_PARAMS_CHANNEL_MULT
-    ]
-
-    down_block_types = []
-    resolution = 1
-    for i in range(len(block_out_channels)):
-        block_type = (
-            "CrossAttnDownBlock2D"
-            if resolution in UNET_PARAMS_ATTENTION_RESOLUTIONS
-            else "DownBlock2D"
-        )
-        down_block_types.append(block_type)
-        if i != len(block_out_channels) - 1:
-            resolution *= 2
-
-    up_block_types = []
-    for i in range(len(block_out_channels)):
-        block_type = (
-            "CrossAttnUpBlock2D"
-            if resolution in UNET_PARAMS_ATTENTION_RESOLUTIONS
-            else "UpBlock2D"
-        )
-        up_block_types.append(block_type)
-        resolution //= 2
-
-    config = dict(
-        sample_size=UNET_PARAMS_IMAGE_SIZE,
-        in_channels=UNET_PARAMS_IN_CHANNELS,
-        out_channels=UNET_PARAMS_OUT_CHANNELS,
-        down_block_types=tuple(down_block_types),
-        up_block_types=tuple(up_block_types),
-        block_out_channels=tuple(block_out_channels),
-        layers_per_block=UNET_PARAMS_NUM_RES_BLOCKS,
-        cross_attention_dim=(
-            UNET_PARAMS_CONTEXT_DIM if not v2 else V2_UNET_PARAMS_CONTEXT_DIM
-        ),
-        attention_head_dim=(
-            UNET_PARAMS_NUM_HEADS if not v2 else V2_UNET_PARAMS_ATTENTION_HEAD_DIM
-        ),
-        # use_linear_projection=UNET_PARAMS_USE_LINEAR_PROJECTION if not v2 else V2_UNET_PARAMS_USE_LINEAR_PROJECTION,
-    )
-    if v2 and use_linear_projection_in_v2:
-        config["use_linear_projection"] = True
-
-    return config
-
-
-def create_vae_diffusers_config():
-    """
-    Creates a config for the diffusers based on the config of the LDM model.
-    """
-    # vae_params = original_config.model.params.first_stage_config.params.ddconfig
-    # _ = original_config.model.params.first_stage_config.params.embed_dim
-    block_out_channels = [VAE_PARAMS_CH * mult for mult in VAE_PARAMS_CH_MULT]
-    down_block_types = ["DownEncoderBlock2D"] * len(block_out_channels)
-    up_block_types = ["UpDecoderBlock2D"] * len(block_out_channels)
-
-    config = dict(
-        sample_size=VAE_PARAMS_RESOLUTION,
-        in_channels=VAE_PARAMS_IN_CHANNELS,
-        out_channels=VAE_PARAMS_OUT_CH,
-        down_block_types=tuple(down_block_types),
-        up_block_types=tuple(up_block_types),
-        block_out_channels=tuple(block_out_channels),
-        latent_channels=VAE_PARAMS_Z_CHANNELS,
-        layers_per_block=VAE_PARAMS_NUM_RES_BLOCKS,
-    )
-    return config
-
-
-def convert_ldm_clip_checkpoint_v1(checkpoint):
-    keys = list(checkpoint.keys())
-    text_model_dict = {}
-    for key in keys:
-        if key.startswith("cond_stage_model.transformer"):
-            text_model_dict[key[len("cond_stage_model.transformer.") :]] = checkpoint[
-                key
-            ]
-    return text_model_dict
-
-
-def convert_ldm_clip_checkpoint_v2(checkpoint, max_length):
-    # 嫌になるくらい違うぞ！
-    def convert_key(key):
-        if not key.startswith("cond_stage_model"):
-            return None
-
-        # common conversion
-        key = key.replace("cond_stage_model.model.transformer.", "text_model.encoder.")
-        key = key.replace("cond_stage_model.model.", "text_model.")
-
-        if "resblocks" in key:
-            # resblocks conversion
-            key = key.replace(".resblocks.", ".layers.")
-            if ".ln_" in key:
-                key = key.replace(".ln_", ".layer_norm")
-            elif ".mlp." in key:
-                key = key.replace(".c_fc.", ".fc1.")
-                key = key.replace(".c_proj.", ".fc2.")
-            elif ".attn.out_proj" in key:
-                key = key.replace(".attn.out_proj.", ".self_attn.out_proj.")
-            elif ".attn.in_proj" in key:
-                key = None  # 特殊なので後で処理する
-            else:
-                raise ValueError(f"unexpected key in SD: {key}")
-        elif ".positional_embedding" in key:
-            key = key.replace(
-                ".positional_embedding", ".embeddings.position_embedding.weight"
-            )
-        elif ".text_projection" in key:
-            key = None  # 使われない???
-        elif ".logit_scale" in key:
-            key = None  # 使われない???
-        elif ".token_embedding" in key:
-            key = key.replace(
-                ".token_embedding.weight", ".embeddings.token_embedding.weight"
-            )
-        elif ".ln_final" in key:
-            key = key.replace(".ln_final", ".final_layer_norm")
-        return key
-
-    keys = list(checkpoint.keys())
-    new_sd = {}
-    for key in keys:
-        # remove resblocks 23
-        if ".resblocks.23." in key:
-            continue
-        new_key = convert_key(key)
-        if new_key is None:
-            continue
-        new_sd[new_key] = checkpoint[key]
-
-    # attnの変換
-    for key in keys:
-        if ".resblocks.23." in key:
-            continue
-        if ".resblocks" in key and ".attn.in_proj_" in key:
-            # 三つに分割
-            values = torch.chunk(checkpoint[key], 3)
-
-            key_suffix = ".weight" if "weight" in key else ".bias"
-            key_pfx = key.replace(
-                "cond_stage_model.model.transformer.resblocks.",
-                "text_model.encoder.layers.",
-            )
-            key_pfx = key_pfx.replace("_weight", "")
-            key_pfx = key_pfx.replace("_bias", "")
-            key_pfx = key_pfx.replace(".attn.in_proj", ".self_attn.")
-            new_sd[key_pfx + "q_proj" + key_suffix] = values[0]
-            new_sd[key_pfx + "k_proj" + key_suffix] = values[1]
-            new_sd[key_pfx + "v_proj" + key_suffix] = values[2]
-
-    # rename or add position_ids
-    ANOTHER_POSITION_IDS_KEY = "text_model.encoder.text_model.embeddings.position_ids"
-    if ANOTHER_POSITION_IDS_KEY in new_sd:
-        # waifu diffusion v1.4
-        position_ids = new_sd[ANOTHER_POSITION_IDS_KEY]
-        del new_sd[ANOTHER_POSITION_IDS_KEY]
-    else:
-        position_ids = torch.Tensor([list(range(max_length))]).to(torch.int64)
-
-    new_sd["text_model.embeddings.position_ids"] = position_ids
-    return new_sd
-
-
-# endregion
-
-
-# region Diffusers->StableDiffusion の変換コード
-# convert_diffusers_to_original_stable_diffusion をコピーして修正している（ASL 2.0）
-
-
-def conv_transformer_to_linear(checkpoint):
-    keys = list(checkpoint.keys())
-    tf_keys = ["proj_in.weight", "proj_out.weight"]
-    for key in keys:
-        if ".".join(key.split(".")[-2:]) in tf_keys:
-            if checkpoint[key].ndim > 2:
-                checkpoint[key] = checkpoint[key][:, :, 0, 0]
-
-
-def convert_unet_state_dict_to_sd(v2, unet_state_dict):
-    unet_conversion_map = [
-        # (stable-diffusion, HF Diffusers)
-        ("time_embed.0.weight", "time_embedding.linear_1.weight"),
-        ("time_embed.0.bias", "time_embedding.linear_1.bias"),
-        ("time_embed.2.weight", "time_embedding.linear_2.weight"),
-        ("time_embed.2.bias", "time_embedding.linear_2.bias"),
-        ("input_blocks.0.0.weight", "conv_in.weight"),
-        ("input_blocks.0.0.bias", "conv_in.bias"),
-        ("out.0.weight", "conv_norm_out.weight"),
-        ("out.0.bias", "conv_norm_out.bias"),
-        ("out.2.weight", "conv_out.weight"),
-        ("out.2.bias", "conv_out.bias"),
-    ]
-
-    unet_conversion_map_resnet = [
-        # (stable-diffusion, HF Diffusers)
-        ("in_layers.0", "norm1"),
-        ("in_layers.2", "conv1"),
-        ("out_layers.0", "norm2"),
-        ("out_layers.3", "conv2"),
-        ("emb_layers.1", "time_emb_proj"),
-        ("skip_connection", "conv_shortcut"),
-    ]
-
-    unet_conversion_map_layer = []
-    for i in range(4):
-        # loop over downblocks/upblocks
-
-        for j in range(2):
-            # loop over resnets/attentions for downblocks
-            hf_down_res_prefix = f"down_blocks.{i}.resnets.{j}."
-            sd_down_res_prefix = f"input_blocks.{3*i + j + 1}.0."
-            unet_conversion_map_layer.append((sd_down_res_prefix, hf_down_res_prefix))
-
-            if i < 3:
-                # no attention layers in down_blocks.3
-                hf_down_atn_prefix = f"down_blocks.{i}.attentions.{j}."
-                sd_down_atn_prefix = f"input_blocks.{3*i + j + 1}.1."
-                unet_conversion_map_layer.append(
-                    (sd_down_atn_prefix, hf_down_atn_prefix)
-                )
-
-        for j in range(3):
-            # loop over resnets/attentions for upblocks
-            hf_up_res_prefix = f"up_blocks.{i}.resnets.{j}."
-            sd_up_res_prefix = f"output_blocks.{3*i + j}.0."
-            unet_conversion_map_layer.append((sd_up_res_prefix, hf_up_res_prefix))
-
-            if i > 0:
-                # no attention layers in up_blocks.0
-                hf_up_atn_prefix = f"up_blocks.{i}.attentions.{j}."
-                sd_up_atn_prefix = f"output_blocks.{3*i + j}.1."
-                unet_conversion_map_layer.append((sd_up_atn_prefix, hf_up_atn_prefix))
-
-        if i < 3:
-            # no downsample in down_blocks.3
-            hf_downsample_prefix = f"down_blocks.{i}.downsamplers.0.conv."
-            sd_downsample_prefix = f"input_blocks.{3*(i+1)}.0.op."
-            unet_conversion_map_layer.append(
-                (sd_downsample_prefix, hf_downsample_prefix)
-            )
-
-            # no upsample in up_blocks.3
-            hf_upsample_prefix = f"up_blocks.{i}.upsamplers.0."
-            sd_upsample_prefix = f"output_blocks.{3*i + 2}.{1 if i == 0 else 2}."
-            unet_conversion_map_layer.append((sd_upsample_prefix, hf_upsample_prefix))
-
-    hf_mid_atn_prefix = "mid_block.attentions.0."
-    sd_mid_atn_prefix = "middle_block.1."
-    unet_conversion_map_layer.append((sd_mid_atn_prefix, hf_mid_atn_prefix))
-
-    for j in range(2):
-        hf_mid_res_prefix = f"mid_block.resnets.{j}."
-        sd_mid_res_prefix = f"middle_block.{2*j}."
-        unet_conversion_map_layer.append((sd_mid_res_prefix, hf_mid_res_prefix))
-
-    # buyer beware: this is a *brittle* function,
-    # and correct output requires that all of these pieces interact in
-    # the exact order in which I have arranged them.
-    mapping = {k: k for k in unet_state_dict.keys()}
-    for sd_name, hf_name in unet_conversion_map:
-        mapping[hf_name] = sd_name
-    for k, v in mapping.items():
-        if "resnets" in k:
-            for sd_part, hf_part in unet_conversion_map_resnet:
-                v = v.replace(hf_part, sd_part)
-            mapping[k] = v
-    for k, v in mapping.items():
-        for sd_part, hf_part in unet_conversion_map_layer:
-            v = v.replace(hf_part, sd_part)
-        mapping[k] = v
-    new_state_dict = {v: unet_state_dict[k] for k, v in mapping.items()}
-
-    if v2:
-        conv_transformer_to_linear(new_state_dict)
-
-    return new_state_dict
-
-
-def controlnet_conversion_map():
-    unet_conversion_map = [
-        ("time_embed.0.weight", "time_embedding.linear_1.weight"),
-        ("time_embed.0.bias", "time_embedding.linear_1.bias"),
-        ("time_embed.2.weight", "time_embedding.linear_2.weight"),
-        ("time_embed.2.bias", "time_embedding.linear_2.bias"),
-        ("input_blocks.0.0.weight", "conv_in.weight"),
-        ("input_blocks.0.0.bias", "conv_in.bias"),
-        ("middle_block_out.0.weight", "controlnet_mid_block.weight"),
-        ("middle_block_out.0.bias", "controlnet_mid_block.bias"),
-    ]
-
-    unet_conversion_map_resnet = [
-        ("in_layers.0", "norm1"),
-        ("in_layers.2", "conv1"),
-        ("out_layers.0", "norm2"),
-        ("out_layers.3", "conv2"),
-        ("emb_layers.1", "time_emb_proj"),
-        ("skip_connection", "conv_shortcut"),
-    ]
-
-    unet_conversion_map_layer = []
-    for i in range(4):
-        for j in range(2):
-            hf_down_res_prefix = f"down_blocks.{i}.resnets.{j}."
-            sd_down_res_prefix = f"input_blocks.{3*i + j + 1}.0."
-            unet_conversion_map_layer.append((sd_down_res_prefix, hf_down_res_prefix))
-
-            if i < 3:
-                hf_down_atn_prefix = f"down_blocks.{i}.attentions.{j}."
-                sd_down_atn_prefix = f"input_blocks.{3*i + j + 1}.1."
-                unet_conversion_map_layer.append(
-                    (sd_down_atn_prefix, hf_down_atn_prefix)
-                )
-
-        if i < 3:
-            hf_downsample_prefix = f"down_blocks.{i}.downsamplers.0.conv."
-            sd_downsample_prefix = f"input_blocks.{3*(i+1)}.0.op."
-            unet_conversion_map_layer.append(
-                (sd_downsample_prefix, hf_downsample_prefix)
-            )
-
-    hf_mid_atn_prefix = "mid_block.attentions.0."
-    sd_mid_atn_prefix = "middle_block.1."
-    unet_conversion_map_layer.append((sd_mid_atn_prefix, hf_mid_atn_prefix))
-
-    for j in range(2):
-        hf_mid_res_prefix = f"mid_block.resnets.{j}."
-        sd_mid_res_prefix = f"middle_block.{2*j}."
-        unet_conversion_map_layer.append((sd_mid_res_prefix, hf_mid_res_prefix))
-
-    controlnet_cond_embedding_names = (
-        ["conv_in"] + [f"blocks.{i}" for i in range(6)] + ["conv_out"]
-    )
-    for i, hf_prefix in enumerate(controlnet_cond_embedding_names):
-        hf_prefix = f"controlnet_cond_embedding.{hf_prefix}."
-        sd_prefix = f"input_hint_block.{i*2}."
-        unet_conversion_map_layer.append((sd_prefix, hf_prefix))
-
-    for i in range(12):
-        hf_prefix = f"controlnet_down_blocks.{i}."
-        sd_prefix = f"zero_convs.{i}.0."
-        unet_conversion_map_layer.append((sd_prefix, hf_prefix))
-
-    return unet_conversion_map, unet_conversion_map_resnet, unet_conversion_map_layer
-
-
-def convert_controlnet_state_dict_to_sd(controlnet_state_dict):
-    (
-        unet_conversion_map,
-        unet_conversion_map_resnet,
-        unet_conversion_map_layer,
-    ) = controlnet_conversion_map()
-
-    mapping = {k: k for k in controlnet_state_dict.keys()}
-    for sd_name, diffusers_name in unet_conversion_map:
-        mapping[diffusers_name] = sd_name
-    for k, v in mapping.items():
-        if "resnets" in k:
-            for sd_part, diffusers_part in unet_conversion_map_resnet:
-                v = v.replace(diffusers_part, sd_part)
-            mapping[k] = v
-    for k, v in mapping.items():
-        for sd_part, diffusers_part in unet_conversion_map_layer:
-            v = v.replace(diffusers_part, sd_part)
-        mapping[k] = v
-    new_state_dict = {v: controlnet_state_dict[k] for k, v in mapping.items()}
-    return new_state_dict
-
-
-def convert_controlnet_state_dict_to_diffusers(controlnet_state_dict):
-    (
-        unet_conversion_map,
-        unet_conversion_map_resnet,
-        unet_conversion_map_layer,
-    ) = controlnet_conversion_map()
-
-    mapping = {k: k for k in controlnet_state_dict.keys()}
-    for sd_name, diffusers_name in unet_conversion_map:
-        mapping[sd_name] = diffusers_name
-    for k, v in mapping.items():
-        for sd_part, diffusers_part in unet_conversion_map_layer:
-            v = v.replace(sd_part, diffusers_part)
-        mapping[k] = v
-    for k, v in mapping.items():
-        if "resnets" in v:
-            for sd_part, diffusers_part in unet_conversion_map_resnet:
-                v = v.replace(sd_part, diffusers_part)
-            mapping[k] = v
-    new_state_dict = {v: controlnet_state_dict[k] for k, v in mapping.items()}
-    return new_state_dict
-
-
-# ================#
-# VAE Conversion #
-# ================#
-
-
-def reshape_weight_for_sd(w):
-    # convert HF linear weights to SD conv2d weights
-    return w.reshape(*w.shape, 1, 1)
-
-
-def convert_vae_state_dict(vae_state_dict):
-    vae_conversion_map = [
-        # (stable-diffusion, HF Diffusers)
-        ("nin_shortcut", "conv_shortcut"),
-        ("norm_out", "conv_norm_out"),
-        ("mid.attn_1.", "mid_block.attentions.0."),
-    ]
-
-    for i in range(4):
-        # down_blocks have two resnets
-        for j in range(2):
-            hf_down_prefix = f"encoder.down_blocks.{i}.resnets.{j}."
-            sd_down_prefix = f"encoder.down.{i}.block.{j}."
-            vae_conversion_map.append((sd_down_prefix, hf_down_prefix))
-
-        if i < 3:
-            hf_downsample_prefix = f"down_blocks.{i}.downsamplers.0."
-            sd_downsample_prefix = f"down.{i}.downsample."
-            vae_conversion_map.append((sd_downsample_prefix, hf_downsample_prefix))
-
-            hf_upsample_prefix = f"up_blocks.{i}.upsamplers.0."
-            sd_upsample_prefix = f"up.{3-i}.upsample."
-            vae_conversion_map.append((sd_upsample_prefix, hf_upsample_prefix))
-
-        # up_blocks have three resnets
-        # also, up blocks in hf are numbered in reverse from sd
-        for j in range(3):
-            hf_up_prefix = f"decoder.up_blocks.{i}.resnets.{j}."
-            sd_up_prefix = f"decoder.up.{3-i}.block.{j}."
-            vae_conversion_map.append((sd_up_prefix, hf_up_prefix))
-
-    # this part accounts for mid blocks in both the encoder and the decoder
-    for i in range(2):
-        hf_mid_res_prefix = f"mid_block.resnets.{i}."
-        sd_mid_res_prefix = f"mid.block_{i+1}."
-        vae_conversion_map.append((sd_mid_res_prefix, hf_mid_res_prefix))
-
-    if diffusers.__version__ < "0.17.0":
-        vae_conversion_map_attn = [
-            # (stable-diffusion, HF Diffusers)
-            ("norm.", "group_norm."),
-            ("q.", "query."),
-            ("k.", "key."),
-            ("v.", "value."),
-            ("proj_out.", "proj_attn."),
-        ]
-    else:
-        vae_conversion_map_attn = [
-            # (stable-diffusion, HF Diffusers)
-            ("norm.", "group_norm."),
-            ("q.", "to_q."),
-            ("k.", "to_k."),
-            ("v.", "to_v."),
-            ("proj_out.", "to_out.0."),
-        ]
-
-    mapping = {k: k for k in vae_state_dict.keys()}
-    for k, v in mapping.items():
-        for sd_part, hf_part in vae_conversion_map:
-            v = v.replace(hf_part, sd_part)
-        mapping[k] = v
-    for k, v in mapping.items():
-        if "attentions" in k:
-            for sd_part, hf_part in vae_conversion_map_attn:
-                v = v.replace(hf_part, sd_part)
-            mapping[k] = v
-    new_state_dict = {v: vae_state_dict[k] for k, v in mapping.items()}
-    weights_to_convert = ["q", "k", "v", "proj_out"]
-    for k, v in new_state_dict.items():
-        for weight_name in weights_to_convert:
-            if f"mid.attn_1.{weight_name}.weight" in k:
-                # print(f"Reshaping {k} for SD format: shape {v.shape} -> {v.shape} x 1 x 1")
-                new_state_dict[k] = reshape_weight_for_sd(v)
-
-    return new_state_dict
-
-
-# endregion
-
-# region 自作のモデル読み書きなど
-
-
-def is_safetensors(path):
-    return os.path.splitext(path)[1].lower() == ".safetensors"
-
-
-def load_checkpoint_with_text_encoder_conversion(ckpt_path, device="cpu"):
-    # text encoderの格納形式が違うモデルに対応する ('text_model'がない)
-    TEXT_ENCODER_KEY_REPLACEMENTS = [
-        (
-            "cond_stage_model.transformer.embeddings.",
-            "cond_stage_model.transformer.text_model.embeddings.",
-        ),
-        (
-            "cond_stage_model.transformer.encoder.",
-            "cond_stage_model.transformer.text_model.encoder.",
-        ),
-        (
-            "cond_stage_model.transformer.final_layer_norm.",
-            "cond_stage_model.transformer.text_model.final_layer_norm.",
-        ),
-    ]
-
-    if is_safetensors(ckpt_path):
-        checkpoint = None
-        state_dict = load_file(ckpt_path)  # , device) # may causes error
-    else:
-        checkpoint = torch.load(ckpt_path, map_location=device)
-        if "state_dict" in checkpoint:
-            state_dict = checkpoint["state_dict"]
-        else:
-            state_dict = checkpoint
-            checkpoint = None
-
-    key_reps = []
-    for rep_from, rep_to in TEXT_ENCODER_KEY_REPLACEMENTS:
-        for key in state_dict.keys():
-            if key.startswith(rep_from):
-                new_key = rep_to + key[len(rep_from) :]
-                key_reps.append((key, new_key))
-
-    for key, new_key in key_reps:
-        state_dict[new_key] = state_dict[key]
-        del state_dict[key]
-
-    return checkpoint, state_dict
-
-
-# TODO dtype指定の動作が怪しいので確認する text_encoderを指定形式で作れるか未確認
-def load_models_from_stable_diffusion_checkpoint(
-    v2, ckpt_path, device="cpu", dtype=None, unet_use_linear_projection_in_v2=True
-):
-    _, state_dict = load_checkpoint_with_text_encoder_conversion(ckpt_path, device)
-
-    # Convert the UNet2DConditionModel model.
-    unet_config = create_unet_diffusers_config(v2, unet_use_linear_projection_in_v2)
-    converted_unet_checkpoint = convert_ldm_unet_checkpoint(v2, state_dict, unet_config)
-
-    unet = UNet2DConditionModel(**unet_config).to(device)
-    info = unet.load_state_dict(converted_unet_checkpoint)
-    print("loading u-net:", info)
-
-    # Convert the VAE model.
-    vae_config = create_vae_diffusers_config()
-    converted_vae_checkpoint = convert_ldm_vae_checkpoint(state_dict, vae_config)
-
-    vae = AutoencoderKL(**vae_config).to(device)
-    info = vae.load_state_dict(converted_vae_checkpoint)
-    print("loading vae:", info)
-
-    # convert text_model
-    if v2:
-        converted_text_encoder_checkpoint = convert_ldm_clip_checkpoint_v2(
-            state_dict, 77
-        )
-        cfg = CLIPTextConfig(
-            vocab_size=49408,
-            hidden_size=1024,
-            intermediate_size=4096,
-            num_hidden_layers=23,
-            num_attention_heads=16,
-            max_position_embeddings=77,
-            hidden_act="gelu",
-            layer_norm_eps=1e-05,
-            dropout=0.0,
-            attention_dropout=0.0,
-            initializer_range=0.02,
-            initializer_factor=1.0,
-            pad_token_id=1,
-            bos_token_id=0,
-            eos_token_id=2,
-            model_type="clip_text_model",
-            projection_dim=512,
-            torch_dtype="float32",
-            transformers_version="4.25.0.dev0",
-        )
-        text_model = CLIPTextModel._from_config(cfg)
-        info = text_model.load_state_dict(
-            converted_text_encoder_checkpoint, strict=False
-        )
-    else:
-        converted_text_encoder_checkpoint = convert_ldm_clip_checkpoint_v1(state_dict)
-
-        # logging.set_verbosity_error()  # don't show annoying warning
-        # text_model = CLIPTextModel.from_pretrained("openai/clip-vit-large-patch14").to(device)
-        # logging.set_verbosity_warning()
-        # print(f"config: {text_model.config}")
-        cfg = CLIPTextConfig(
-            vocab_size=49408,
-            hidden_size=768,
-            intermediate_size=3072,
-            num_hidden_layers=12,
-            num_attention_heads=12,
-            max_position_embeddings=77,
-            hidden_act="quick_gelu",
-            layer_norm_eps=1e-05,
-            dropout=0.0,
-            attention_dropout=0.0,
-            initializer_range=0.02,
-            initializer_factor=1.0,
-            pad_token_id=1,
-            bos_token_id=0,
-            eos_token_id=2,
-            model_type="clip_text_model",
-            projection_dim=768,
-            torch_dtype="float32",
-        )
-        text_model = CLIPTextModel._from_config(cfg)
-        info = text_model.load_state_dict(
-            converted_text_encoder_checkpoint, strict=False
-        )
-    print("loading text encoder:", info)
-
-    return text_model, vae, unet
-
-
-def get_model_version_str_for_sd1_sd2(v2, v_parameterization):
-    # only for reference
-    version_str = "sd"
-    if v2:
-        version_str += "_v2"
-    else:
-        version_str += "_v1"
-    if v_parameterization:
-        version_str += "_v"
-    return version_str
-
-
-def convert_text_encoder_state_dict_to_sd_v2(checkpoint, make_dummy_weights=False):
-    def convert_key(key):
-        # position_idsの除去
-        if ".position_ids" in key:
-            return None
-
-        # common
-        key = key.replace("text_model.encoder.", "transformer.")
-        key = key.replace("text_model.", "")
-        if "layers" in key:
-            # resblocks conversion
-            key = key.replace(".layers.", ".resblocks.")
-            if ".layer_norm" in key:
-                key = key.replace(".layer_norm", ".ln_")
-            elif ".mlp." in key:
-                key = key.replace(".fc1.", ".c_fc.")
-                key = key.replace(".fc2.", ".c_proj.")
-            elif ".self_attn.out_proj" in key:
-                key = key.replace(".self_attn.out_proj.", ".attn.out_proj.")
-            elif ".self_attn." in key:
-                key = None  # 特殊なので後で処理する
-            else:
-                raise ValueError(f"unexpected key in DiffUsers model: {key}")
-        elif ".position_embedding" in key:
-            key = key.replace(
-                "embeddings.position_embedding.weight", "positional_embedding"
-            )
-        elif ".token_embedding" in key:
-            key = key.replace(
-                "embeddings.token_embedding.weight", "token_embedding.weight"
-            )
-        elif "final_layer_norm" in key:
-            key = key.replace("final_layer_norm", "ln_final")
-        return key
-
-    keys = list(checkpoint.keys())
-    new_sd = {}
-    for key in keys:
-        new_key = convert_key(key)
-        if new_key is None:
-            continue
-        new_sd[new_key] = checkpoint[key]
-
-    # attnの変換
-    for key in keys:
-        if "layers" in key and "q_proj" in key:
-            # 三つを結合
-            key_q = key
-            key_k = key.replace("q_proj", "k_proj")
-            key_v = key.replace("q_proj", "v_proj")
-
-            value_q = checkpoint[key_q]
-            value_k = checkpoint[key_k]
-            value_v = checkpoint[key_v]
-            value = torch.cat([value_q, value_k, value_v])
-
-            new_key = key.replace(
-                "text_model.encoder.layers.", "transformer.resblocks."
-            )
-            new_key = new_key.replace(".self_attn.q_proj.", ".attn.in_proj_")
-            new_sd[new_key] = value
-
-    # 最後の層などを捏造するか
-    if make_dummy_weights:
-        print("make dummy weights for resblock.23, text_projection and logit scale.")
-        keys = list(new_sd.keys())
-        for key in keys:
-            if key.startswith("transformer.resblocks.22."):
-                new_sd[key.replace(".22.", ".23.")] = new_sd[
-                    key
-                ].clone()  # copyしないとsafetensorsの保存で落ちる
-
-        # Diffusersに含まれない重みを作っておく
-        new_sd["text_projection"] = torch.ones(
-            (1024, 1024), dtype=new_sd[keys[0]].dtype, device=new_sd[keys[0]].device
-        )
-        new_sd["logit_scale"] = torch.tensor(1)
-
-    return new_sd
-
-
-def save_stable_diffusion_checkpoint(
-    v2,
-    output_file,
-    text_encoder,
-    unet,
-    ckpt_path,
-    epochs,
-    steps,
-    save_dtype=None,
-    vae=None,
-):
-    if ckpt_path is not None:
-        # epoch/stepを参照する。またVAEがメモリ上にないときなど、もう一度VAEを含めて読み込む
-        checkpoint, state_dict = load_checkpoint_with_text_encoder_conversion(ckpt_path)
-        if checkpoint is None:  # safetensors または state_dictのckpt
-            checkpoint = {}
-            strict = False
-        else:
-            strict = True
-        if "state_dict" in state_dict:
-            del state_dict["state_dict"]
-    else:
-        # 新しく作る
-        assert (
-            vae is not None
-        ), "VAE is required to save a checkpoint without a given checkpoint"
-        checkpoint = {}
-        state_dict = {}
-        strict = False
-
-    def update_sd(prefix, sd):
-        for k, v in sd.items():
-            key = prefix + k
-            assert not strict or key in state_dict, f"Illegal key in save SD: {key}"
-            if save_dtype is not None:
-                v = v.detach().clone().to("cpu").to(save_dtype)
-            state_dict[key] = v
-
-    # Convert the UNet model
-    unet_state_dict = convert_unet_state_dict_to_sd(v2, unet.state_dict())
-    update_sd("model.diffusion_model.", unet_state_dict)
-
-    # Convert the text encoder model
-    if v2:
-        make_dummy = (
-            ckpt_path is None
-        )  # 参照元のcheckpointがない場合は最後の層を前の層から複製して作るなどダミーの重みを入れる
-        text_enc_dict = convert_text_encoder_state_dict_to_sd_v2(
-            text_encoder.state_dict(), make_dummy
-        )
-        update_sd("cond_stage_model.model.", text_enc_dict)
-    else:
-        text_enc_dict = text_encoder.state_dict()
-        update_sd("cond_stage_model.transformer.", text_enc_dict)
-
-    # Convert the VAE
-    if vae is not None:
-        vae_dict = convert_vae_state_dict(vae.state_dict())
-        update_sd("first_stage_model.", vae_dict)
-
-    # Put together new checkpoint
-    key_count = len(state_dict.keys())
-    new_ckpt = {"state_dict": state_dict}
-
-    # epoch and global_step are sometimes not int
-    try:
-        if "epoch" in checkpoint:
-            epochs += checkpoint["epoch"]
-        if "global_step" in checkpoint:
-            steps += checkpoint["global_step"]
-    except:
-        pass
-
-    new_ckpt["epoch"] = epochs
-    new_ckpt["global_step"] = steps
-
-    if is_safetensors(output_file):
-        # TODO Tensor以外のdictの値を削除したほうがいいか
-        save_file(state_dict, output_file)
-    else:
-        torch.save(new_ckpt, output_file)
-
-    return key_count
-
-
-def save_diffusers_checkpoint(
-    v2,
-    output_dir,
-    text_encoder,
-    unet,
-    pretrained_model_name_or_path,
-    vae=None,
-    use_safetensors=False,
-):
-    if pretrained_model_name_or_path is None:
-        # load default settings for v1/v2
-        if v2:
-            pretrained_model_name_or_path = DIFFUSERS_REF_MODEL_ID_V2
-        else:
-            pretrained_model_name_or_path = DIFFUSERS_REF_MODEL_ID_V1
-
-    scheduler = DDIMScheduler.from_pretrained(
-        pretrained_model_name_or_path, subfolder="scheduler"
-    )
-    tokenizer = CLIPTokenizer.from_pretrained(
-        pretrained_model_name_or_path, subfolder="tokenizer"
-    )
-    if vae is None:
-        vae = AutoencoderKL.from_pretrained(
-            pretrained_model_name_or_path, subfolder="vae"
-        )
-
-    pipeline = StableDiffusionPipeline(
-        unet=unet,
-        text_encoder=text_encoder,
-        vae=vae,
-        scheduler=scheduler,
-        tokenizer=tokenizer,
-        safety_checker=None,
-        feature_extractor=None,
-        requires_safety_checker=None,
-    )
-    pipeline.save_pretrained(output_dir, safe_serialization=use_safetensors)
-
-
-VAE_PREFIX = "first_stage_model."
-
-
-def load_vae(vae_id, dtype):
-    print(f"load VAE: {vae_id}")
-    if os.path.isdir(vae_id) or not os.path.isfile(vae_id):
-        # Diffusers local/remote
-        try:
-            vae = AutoencoderKL.from_pretrained(
-                vae_id, subfolder=None, torch_dtype=dtype
-            )
-        except EnvironmentError as e:
-            print(f"exception occurs in loading vae: {e}")
-            print("retry with subfolder='vae'")
-            vae = AutoencoderKL.from_pretrained(
-                vae_id, subfolder="vae", torch_dtype=dtype
-            )
-        return vae
-
-    # local
-    vae_config = create_vae_diffusers_config()
-
-    if vae_id.endswith(".bin"):
-        # SD 1.5 VAE on Huggingface
-        converted_vae_checkpoint = torch.load(vae_id, map_location="cpu")
-    else:
-        # StableDiffusion
-        vae_model = (
-            load_file(vae_id, "cpu")
-            if is_safetensors(vae_id)
-            else torch.load(vae_id, map_location="cpu")
-        )
-        vae_sd = vae_model["state_dict"] if "state_dict" in vae_model else vae_model
-
-        # vae only or full model
-        full_model = False
-        for vae_key in vae_sd:
-            if vae_key.startswith(VAE_PREFIX):
-                full_model = True
-                break
-        if not full_model:
-            sd = {}
-            for key, value in vae_sd.items():
-                sd[VAE_PREFIX + key] = value
-            vae_sd = sd
-            del sd
-
-        # Convert the VAE model.
-        converted_vae_checkpoint = convert_ldm_vae_checkpoint(vae_sd, vae_config)
-
-    vae = AutoencoderKL(**vae_config)
-    vae.load_state_dict(converted_vae_checkpoint)
-    return vae
-
-
-# endregion
-
-
-def make_bucket_resolutions(max_reso, min_size=256, max_size=1024, divisible=64):
-    max_width, max_height = max_reso
-    max_area = (max_width // divisible) * (max_height // divisible)
-
-    resos = set()
-
-    size = int(math.sqrt(max_area)) * divisible
-    resos.add((size, size))
-
-    size = min_size
-    while size <= max_size:
-        width = size
-        height = min(max_size, (max_area // (width // divisible)) * divisible)
-        resos.add((width, height))
-        resos.add((height, width))
-
-        # # make additional resos
-        # if width >= height and width - divisible >= min_size:
-        #   resos.add((width - divisible, height))
-        #   resos.add((height, width - divisible))
-        # if height >= width and height - divisible >= min_size:
-        #   resos.add((width, height - divisible))
-        #   resos.add((height - divisible, width))
-
-        size += divisible
-
-    resos = list(resos)
-    resos.sort()
-    return resos
-
-
-if __name__ == "__main__":
-    resos = make_bucket_resolutions((512, 768))
-    print(len(resos))
-    print(resos)
-    aspect_ratios = [w / h for w, h in resos]
-    print(aspect_ratios)
-
-    ars = set()
-    for ar in aspect_ratios:
-        if ar in ars:
-            print("error! duplicate ar:", ar)
-        ars.add(ar)
+# https://github.com/kohya-ss/sd-scripts/blob/b78c0e2a69e52ce6c79abc6c8c82d1a9cabcf05c/library/model_util.py
+# v1: split from train_db_fixed.py.
+# v2: support safetensors
+
+import math
+import os
+import torch
+import diffusers
+from transformers import CLIPTextModel, CLIPTokenizer, CLIPTextConfig, logging
+from diffusers import (
+    AutoencoderKL,
+    DDIMScheduler,
+    StableDiffusionPipeline,
+)  # , UNet2DConditionModel
+from safetensors.torch import load_file, save_file
+from .original_unet import UNet2DConditionModel
+
+# DiffUsers版StableDiffusionのモデルパラメータ
+NUM_TRAIN_TIMESTEPS = 1000
+BETA_START = 0.00085
+BETA_END = 0.0120
+
+UNET_PARAMS_MODEL_CHANNELS = 320
+UNET_PARAMS_CHANNEL_MULT = [1, 2, 4, 4]
+UNET_PARAMS_ATTENTION_RESOLUTIONS = [4, 2, 1]
+UNET_PARAMS_IMAGE_SIZE = 64  # fixed from old invalid value `32`
+UNET_PARAMS_IN_CHANNELS = 4
+UNET_PARAMS_OUT_CHANNELS = 4
+UNET_PARAMS_NUM_RES_BLOCKS = 2
+UNET_PARAMS_CONTEXT_DIM = 768
+UNET_PARAMS_NUM_HEADS = 8
+# UNET_PARAMS_USE_LINEAR_PROJECTION = False
+
+VAE_PARAMS_Z_CHANNELS = 4
+VAE_PARAMS_RESOLUTION = 256
+VAE_PARAMS_IN_CHANNELS = 3
+VAE_PARAMS_OUT_CH = 3
+VAE_PARAMS_CH = 128
+VAE_PARAMS_CH_MULT = [1, 2, 4, 4]
+VAE_PARAMS_NUM_RES_BLOCKS = 2
+
+# V2
+V2_UNET_PARAMS_ATTENTION_HEAD_DIM = [5, 10, 20, 20]
+V2_UNET_PARAMS_CONTEXT_DIM = 1024
+# V2_UNET_PARAMS_USE_LINEAR_PROJECTION = True
+
+# Diffusersの設定を読み込むための参照モデル
+DIFFUSERS_REF_MODEL_ID_V1 = "runwayml/stable-diffusion-v1-5"
+DIFFUSERS_REF_MODEL_ID_V2 = "stabilityai/stable-diffusion-2-1"
+
+
+# region StableDiffusion->Diffusersの変換コード
+# convert_original_stable_diffusion_to_diffusers をコピーして修正している（ASL 2.0）
+
+
+def shave_segments(path, n_shave_prefix_segments=1):
+    """
+    Removes segments. Positive values shave the first segments, negative shave the last segments.
+    """
+    if n_shave_prefix_segments >= 0:
+        return ".".join(path.split(".")[n_shave_prefix_segments:])
+    else:
+        return ".".join(path.split(".")[:n_shave_prefix_segments])
+
+
+def renew_resnet_paths(old_list, n_shave_prefix_segments=0):
+    """
+    Updates paths inside resnets to the new naming scheme (local renaming)
+    """
+    mapping = []
+    for old_item in old_list:
+        new_item = old_item.replace("in_layers.0", "norm1")
+        new_item = new_item.replace("in_layers.2", "conv1")
+
+        new_item = new_item.replace("out_layers.0", "norm2")
+        new_item = new_item.replace("out_layers.3", "conv2")
+
+        new_item = new_item.replace("emb_layers.1", "time_emb_proj")
+        new_item = new_item.replace("skip_connection", "conv_shortcut")
+
+        new_item = shave_segments(
+            new_item, n_shave_prefix_segments=n_shave_prefix_segments
+        )
+
+        mapping.append({"old": old_item, "new": new_item})
+
+    return mapping
+
+
+def renew_vae_resnet_paths(old_list, n_shave_prefix_segments=0):
+    """
+    Updates paths inside resnets to the new naming scheme (local renaming)
+    """
+    mapping = []
+    for old_item in old_list:
+        new_item = old_item
+
+        new_item = new_item.replace("nin_shortcut", "conv_shortcut")
+        new_item = shave_segments(
+            new_item, n_shave_prefix_segments=n_shave_prefix_segments
+        )
+
+        mapping.append({"old": old_item, "new": new_item})
+
+    return mapping
+
+
+def renew_attention_paths(old_list, n_shave_prefix_segments=0):
+    """
+    Updates paths inside attentions to the new naming scheme (local renaming)
+    """
+    mapping = []
+    for old_item in old_list:
+        new_item = old_item
+
+        #         new_item = new_item.replace('norm.weight', 'group_norm.weight')
+        #         new_item = new_item.replace('norm.bias', 'group_norm.bias')
+
+        #         new_item = new_item.replace('proj_out.weight', 'proj_attn.weight')
+        #         new_item = new_item.replace('proj_out.bias', 'proj_attn.bias')
+
+        #         new_item = shave_segments(new_item, n_shave_prefix_segments=n_shave_prefix_segments)
+
+        mapping.append({"old": old_item, "new": new_item})
+
+    return mapping
+
+
+def renew_vae_attention_paths(old_list, n_shave_prefix_segments=0):
+    """
+    Updates paths inside attentions to the new naming scheme (local renaming)
+    """
+    mapping = []
+    for old_item in old_list:
+        new_item = old_item
+
+        new_item = new_item.replace("norm.weight", "group_norm.weight")
+        new_item = new_item.replace("norm.bias", "group_norm.bias")
+
+        if diffusers.__version__ < "0.17.0":
+            new_item = new_item.replace("q.weight", "query.weight")
+            new_item = new_item.replace("q.bias", "query.bias")
+
+            new_item = new_item.replace("k.weight", "key.weight")
+            new_item = new_item.replace("k.bias", "key.bias")
+
+            new_item = new_item.replace("v.weight", "value.weight")
+            new_item = new_item.replace("v.bias", "value.bias")
+
+            new_item = new_item.replace("proj_out.weight", "proj_attn.weight")
+            new_item = new_item.replace("proj_out.bias", "proj_attn.bias")
+        else:
+            new_item = new_item.replace("q.weight", "to_q.weight")
+            new_item = new_item.replace("q.bias", "to_q.bias")
+
+            new_item = new_item.replace("k.weight", "to_k.weight")
+            new_item = new_item.replace("k.bias", "to_k.bias")
+
+            new_item = new_item.replace("v.weight", "to_v.weight")
+            new_item = new_item.replace("v.bias", "to_v.bias")
+
+            new_item = new_item.replace("proj_out.weight", "to_out.0.weight")
+            new_item = new_item.replace("proj_out.bias", "to_out.0.bias")
+
+        new_item = shave_segments(
+            new_item, n_shave_prefix_segments=n_shave_prefix_segments
+        )
+
+        mapping.append({"old": old_item, "new": new_item})
+
+    return mapping
+
+
+def assign_to_checkpoint(
+    paths,
+    checkpoint,
+    old_checkpoint,
+    attention_paths_to_split=None,
+    additional_replacements=None,
+    config=None,
+):
+    """
+    This does the final conversion step: take locally converted weights and apply a global renaming
+    to them. It splits attention layers, and takes into account additional replacements
+    that may arise.
+
+    Assigns the weights to the new checkpoint.
+    """
+    assert isinstance(
+        paths, list
+    ), "Paths should be a list of dicts containing 'old' and 'new' keys."
+
+    # Splits the attention layers into three variables.
+    if attention_paths_to_split is not None:
+        for path, path_map in attention_paths_to_split.items():
+            old_tensor = old_checkpoint[path]
+            channels = old_tensor.shape[0] // 3
+
+            target_shape = (-1, channels) if len(old_tensor.shape) == 3 else (-1)
+
+            num_heads = old_tensor.shape[0] // config["num_head_channels"] // 3
+
+            old_tensor = old_tensor.reshape(
+                (num_heads, 3 * channels // num_heads) + old_tensor.shape[1:]
+            )
+            query, key, value = old_tensor.split(channels // num_heads, dim=1)
+
+            checkpoint[path_map["query"]] = query.reshape(target_shape)
+            checkpoint[path_map["key"]] = key.reshape(target_shape)
+            checkpoint[path_map["value"]] = value.reshape(target_shape)
+
+    for path in paths:
+        new_path = path["new"]
+
+        # These have already been assigned
+        if (
+            attention_paths_to_split is not None
+            and new_path in attention_paths_to_split
+        ):
+            continue
+
+        # Global renaming happens here
+        new_path = new_path.replace("middle_block.0", "mid_block.resnets.0")
+        new_path = new_path.replace("middle_block.1", "mid_block.attentions.0")
+        new_path = new_path.replace("middle_block.2", "mid_block.resnets.1")
+
+        if additional_replacements is not None:
+            for replacement in additional_replacements:
+                new_path = new_path.replace(replacement["old"], replacement["new"])
+
+        # proj_attn.weight has to be converted from conv 1D to linear
+        reshaping = False
+        if diffusers.__version__ < "0.17.0":
+            if "proj_attn.weight" in new_path:
+                reshaping = True
+        else:
+            if (
+                ".attentions." in new_path
+                and ".0.to_" in new_path
+                and old_checkpoint[path["old"]].ndim > 2
+            ):
+                reshaping = True
+
+        if reshaping:
+            checkpoint[new_path] = old_checkpoint[path["old"]][:, :, 0, 0]
+        else:
+            checkpoint[new_path] = old_checkpoint[path["old"]]
+
+
+def conv_attn_to_linear(checkpoint):
+    keys = list(checkpoint.keys())
+    attn_keys = ["query.weight", "key.weight", "value.weight"]
+    for key in keys:
+        if ".".join(key.split(".")[-2:]) in attn_keys:
+            if checkpoint[key].ndim > 2:
+                checkpoint[key] = checkpoint[key][:, :, 0, 0]
+        elif "proj_attn.weight" in key:
+            if checkpoint[key].ndim > 2:
+                checkpoint[key] = checkpoint[key][:, :, 0]
+
+
+def linear_transformer_to_conv(checkpoint):
+    keys = list(checkpoint.keys())
+    tf_keys = ["proj_in.weight", "proj_out.weight"]
+    for key in keys:
+        if ".".join(key.split(".")[-2:]) in tf_keys:
+            if checkpoint[key].ndim == 2:
+                checkpoint[key] = checkpoint[key].unsqueeze(2).unsqueeze(2)
+
+
+def convert_ldm_unet_checkpoint(v2, checkpoint, config):
+    """
+    Takes a state dict and a config, and returns a converted checkpoint.
+    """
+
+    # extract state_dict for UNet
+    unet_state_dict = {}
+    unet_key = "model.diffusion_model."
+    keys = list(checkpoint.keys())
+    for key in keys:
+        if key.startswith(unet_key):
+            unet_state_dict[key.replace(unet_key, "")] = checkpoint.pop(key)
+
+    new_checkpoint = {}
+
+    new_checkpoint["time_embedding.linear_1.weight"] = unet_state_dict[
+        "time_embed.0.weight"
+    ]
+    new_checkpoint["time_embedding.linear_1.bias"] = unet_state_dict[
+        "time_embed.0.bias"
+    ]
+    new_checkpoint["time_embedding.linear_2.weight"] = unet_state_dict[
+        "time_embed.2.weight"
+    ]
+    new_checkpoint["time_embedding.linear_2.bias"] = unet_state_dict[
+        "time_embed.2.bias"
+    ]
+
+    new_checkpoint["conv_in.weight"] = unet_state_dict["input_blocks.0.0.weight"]
+    new_checkpoint["conv_in.bias"] = unet_state_dict["input_blocks.0.0.bias"]
+
+    new_checkpoint["conv_norm_out.weight"] = unet_state_dict["out.0.weight"]
+    new_checkpoint["conv_norm_out.bias"] = unet_state_dict["out.0.bias"]
+    new_checkpoint["conv_out.weight"] = unet_state_dict["out.2.weight"]
+    new_checkpoint["conv_out.bias"] = unet_state_dict["out.2.bias"]
+
+    # Retrieves the keys for the input blocks only
+    num_input_blocks = len(
+        {
+            ".".join(layer.split(".")[:2])
+            for layer in unet_state_dict
+            if "input_blocks" in layer
+        }
+    )
+    input_blocks = {
+        layer_id: [key for key in unet_state_dict if f"input_blocks.{layer_id}." in key]
+        for layer_id in range(num_input_blocks)
+    }
+
+    # Retrieves the keys for the middle blocks only
+    num_middle_blocks = len(
+        {
+            ".".join(layer.split(".")[:2])
+            for layer in unet_state_dict
+            if "middle_block" in layer
+        }
+    )
+    middle_blocks = {
+        layer_id: [key for key in unet_state_dict if f"middle_block.{layer_id}." in key]
+        for layer_id in range(num_middle_blocks)
+    }
+
+    # Retrieves the keys for the output blocks only
+    num_output_blocks = len(
+        {
+            ".".join(layer.split(".")[:2])
+            for layer in unet_state_dict
+            if "output_blocks" in layer
+        }
+    )
+    output_blocks = {
+        layer_id: [
+            key for key in unet_state_dict if f"output_blocks.{layer_id}." in key
+        ]
+        for layer_id in range(num_output_blocks)
+    }
+
+    for i in range(1, num_input_blocks):
+        block_id = (i - 1) // (config["layers_per_block"] + 1)
+        layer_in_block_id = (i - 1) % (config["layers_per_block"] + 1)
+
+        resnets = [
+            key
+            for key in input_blocks[i]
+            if f"input_blocks.{i}.0" in key and f"input_blocks.{i}.0.op" not in key
+        ]
+        attentions = [key for key in input_blocks[i] if f"input_blocks.{i}.1" in key]
+
+        if f"input_blocks.{i}.0.op.weight" in unet_state_dict:
+            new_checkpoint[f"down_blocks.{block_id}.downsamplers.0.conv.weight"] = (
+                unet_state_dict.pop(f"input_blocks.{i}.0.op.weight")
+            )
+            new_checkpoint[f"down_blocks.{block_id}.downsamplers.0.conv.bias"] = (
+                unet_state_dict.pop(f"input_blocks.{i}.0.op.bias")
+            )
+
+        paths = renew_resnet_paths(resnets)
+        meta_path = {
+            "old": f"input_blocks.{i}.0",
+            "new": f"down_blocks.{block_id}.resnets.{layer_in_block_id}",
+        }
+        assign_to_checkpoint(
+            paths,
+            new_checkpoint,
+            unet_state_dict,
+            additional_replacements=[meta_path],
+            config=config,
+        )
+
+        if len(attentions):
+            paths = renew_attention_paths(attentions)
+            meta_path = {
+                "old": f"input_blocks.{i}.1",
+                "new": f"down_blocks.{block_id}.attentions.{layer_in_block_id}",
+            }
+            assign_to_checkpoint(
+                paths,
+                new_checkpoint,
+                unet_state_dict,
+                additional_replacements=[meta_path],
+                config=config,
+            )
+
+    resnet_0 = middle_blocks[0]
+    attentions = middle_blocks[1]
+    resnet_1 = middle_blocks[2]
+
+    resnet_0_paths = renew_resnet_paths(resnet_0)
+    assign_to_checkpoint(resnet_0_paths, new_checkpoint, unet_state_dict, config=config)
+
+    resnet_1_paths = renew_resnet_paths(resnet_1)
+    assign_to_checkpoint(resnet_1_paths, new_checkpoint, unet_state_dict, config=config)
+
+    attentions_paths = renew_attention_paths(attentions)
+    meta_path = {"old": "middle_block.1", "new": "mid_block.attentions.0"}
+    assign_to_checkpoint(
+        attentions_paths,
+        new_checkpoint,
+        unet_state_dict,
+        additional_replacements=[meta_path],
+        config=config,
+    )
+
+    for i in range(num_output_blocks):
+        block_id = i // (config["layers_per_block"] + 1)
+        layer_in_block_id = i % (config["layers_per_block"] + 1)
+        output_block_layers = [shave_segments(name, 2) for name in output_blocks[i]]
+        output_block_list = {}
+
+        for layer in output_block_layers:
+            layer_id, layer_name = layer.split(".")[0], shave_segments(layer, 1)
+            if layer_id in output_block_list:
+                output_block_list[layer_id].append(layer_name)
+            else:
+                output_block_list[layer_id] = [layer_name]
+
+        if len(output_block_list) > 1:
+            resnets = [key for key in output_blocks[i] if f"output_blocks.{i}.0" in key]
+            attentions = [
+                key for key in output_blocks[i] if f"output_blocks.{i}.1" in key
+            ]
+
+            resnet_0_paths = renew_resnet_paths(resnets)
+            paths = renew_resnet_paths(resnets)
+
+            meta_path = {
+                "old": f"output_blocks.{i}.0",
+                "new": f"up_blocks.{block_id}.resnets.{layer_in_block_id}",
+            }
+            assign_to_checkpoint(
+                paths,
+                new_checkpoint,
+                unet_state_dict,
+                additional_replacements=[meta_path],
+                config=config,
+            )
+
+            # オリジナル：
+            # if ["conv.weight", "conv.bias"] in output_block_list.values():
+            #   index = list(output_block_list.values()).index(["conv.weight", "conv.bias"])
+
+            # biasとweightの順番に依存しないようにする：もっといいやり方がありそうだが
+            for l in output_block_list.values():
+                l.sort()
+
+            if ["conv.bias", "conv.weight"] in output_block_list.values():
+                index = list(output_block_list.values()).index(
+                    ["conv.bias", "conv.weight"]
+                )
+                new_checkpoint[f"up_blocks.{block_id}.upsamplers.0.conv.bias"] = (
+                    unet_state_dict[f"output_blocks.{i}.{index}.conv.bias"]
+                )
+                new_checkpoint[f"up_blocks.{block_id}.upsamplers.0.conv.weight"] = (
+                    unet_state_dict[f"output_blocks.{i}.{index}.conv.weight"]
+                )
+
+                # Clear attentions as they have been attributed above.
+                if len(attentions) == 2:
+                    attentions = []
+
+            if len(attentions):
+                paths = renew_attention_paths(attentions)
+                meta_path = {
+                    "old": f"output_blocks.{i}.1",
+                    "new": f"up_blocks.{block_id}.attentions.{layer_in_block_id}",
+                }
+                assign_to_checkpoint(
+                    paths,
+                    new_checkpoint,
+                    unet_state_dict,
+                    additional_replacements=[meta_path],
+                    config=config,
+                )
+        else:
+            resnet_0_paths = renew_resnet_paths(
+                output_block_layers, n_shave_prefix_segments=1
+            )
+            for path in resnet_0_paths:
+                old_path = ".".join(["output_blocks", str(i), path["old"]])
+                new_path = ".".join(
+                    [
+                        "up_blocks",
+                        str(block_id),
+                        "resnets",
+                        str(layer_in_block_id),
+                        path["new"],
+                    ]
+                )
+
+                new_checkpoint[new_path] = unet_state_dict[old_path]
+
+    # SDのv2では1*1のconv2dがlinearに変わっている
+    # 誤って Diffusers 側を conv2d のままにしてしまったので、変換必要
+    if v2 and not config.get("use_linear_projection", False):
+        linear_transformer_to_conv(new_checkpoint)
+
+    return new_checkpoint
+
+
+def convert_ldm_vae_checkpoint(checkpoint, config):
+    # extract state dict for VAE
+    vae_state_dict = {}
+    vae_key = "first_stage_model."
+    keys = list(checkpoint.keys())
+    for key in keys:
+        if key.startswith(vae_key):
+            vae_state_dict[key.replace(vae_key, "")] = checkpoint.get(key)
+    # if len(vae_state_dict) == 0:
+    #   # 渡されたcheckpointは.ckptから読み込んだcheckpointではなくvaeのstate_dict
+    #   vae_state_dict = checkpoint
+
+    new_checkpoint = {}
+
+    new_checkpoint["encoder.conv_in.weight"] = vae_state_dict["encoder.conv_in.weight"]
+    new_checkpoint["encoder.conv_in.bias"] = vae_state_dict["encoder.conv_in.bias"]
+    new_checkpoint["encoder.conv_out.weight"] = vae_state_dict[
+        "encoder.conv_out.weight"
+    ]
+    new_checkpoint["encoder.conv_out.bias"] = vae_state_dict["encoder.conv_out.bias"]
+    new_checkpoint["encoder.conv_norm_out.weight"] = vae_state_dict[
+        "encoder.norm_out.weight"
+    ]
+    new_checkpoint["encoder.conv_norm_out.bias"] = vae_state_dict[
+        "encoder.norm_out.bias"
+    ]
+
+    new_checkpoint["decoder.conv_in.weight"] = vae_state_dict["decoder.conv_in.weight"]
+    new_checkpoint["decoder.conv_in.bias"] = vae_state_dict["decoder.conv_in.bias"]
+    new_checkpoint["decoder.conv_out.weight"] = vae_state_dict[
+        "decoder.conv_out.weight"
+    ]
+    new_checkpoint["decoder.conv_out.bias"] = vae_state_dict["decoder.conv_out.bias"]
+    new_checkpoint["decoder.conv_norm_out.weight"] = vae_state_dict[
+        "decoder.norm_out.weight"
+    ]
+    new_checkpoint["decoder.conv_norm_out.bias"] = vae_state_dict[
+        "decoder.norm_out.bias"
+    ]
+
+    new_checkpoint["quant_conv.weight"] = vae_state_dict["quant_conv.weight"]
+    new_checkpoint["quant_conv.bias"] = vae_state_dict["quant_conv.bias"]
+    new_checkpoint["post_quant_conv.weight"] = vae_state_dict["post_quant_conv.weight"]
+    new_checkpoint["post_quant_conv.bias"] = vae_state_dict["post_quant_conv.bias"]
+
+    # Retrieves the keys for the encoder down blocks only
+    num_down_blocks = len(
+        {
+            ".".join(layer.split(".")[:3])
+            for layer in vae_state_dict
+            if "encoder.down" in layer
+        }
+    )
+    down_blocks = {
+        layer_id: [key for key in vae_state_dict if f"down.{layer_id}" in key]
+        for layer_id in range(num_down_blocks)
+    }
+
+    # Retrieves the keys for the decoder up blocks only
+    num_up_blocks = len(
+        {
+            ".".join(layer.split(".")[:3])
+            for layer in vae_state_dict
+            if "decoder.up" in layer
+        }
+    )
+    up_blocks = {
+        layer_id: [key for key in vae_state_dict if f"up.{layer_id}" in key]
+        for layer_id in range(num_up_blocks)
+    }
+
+    for i in range(num_down_blocks):
+        resnets = [
+            key
+            for key in down_blocks[i]
+            if f"down.{i}" in key and f"down.{i}.downsample" not in key
+        ]
+
+        if f"encoder.down.{i}.downsample.conv.weight" in vae_state_dict:
+            new_checkpoint[f"encoder.down_blocks.{i}.downsamplers.0.conv.weight"] = (
+                vae_state_dict.pop(f"encoder.down.{i}.downsample.conv.weight")
+            )
+            new_checkpoint[f"encoder.down_blocks.{i}.downsamplers.0.conv.bias"] = (
+                vae_state_dict.pop(f"encoder.down.{i}.downsample.conv.bias")
+            )
+
+        paths = renew_vae_resnet_paths(resnets)
+        meta_path = {"old": f"down.{i}.block", "new": f"down_blocks.{i}.resnets"}
+        assign_to_checkpoint(
+            paths,
+            new_checkpoint,
+            vae_state_dict,
+            additional_replacements=[meta_path],
+            config=config,
+        )
+
+    mid_resnets = [key for key in vae_state_dict if "encoder.mid.block" in key]
+    num_mid_res_blocks = 2
+    for i in range(1, num_mid_res_blocks + 1):
+        resnets = [key for key in mid_resnets if f"encoder.mid.block_{i}" in key]
+
+        paths = renew_vae_resnet_paths(resnets)
+        meta_path = {"old": f"mid.block_{i}", "new": f"mid_block.resnets.{i - 1}"}
+        assign_to_checkpoint(
+            paths,
+            new_checkpoint,
+            vae_state_dict,
+            additional_replacements=[meta_path],
+            config=config,
+        )
+
+    mid_attentions = [key for key in vae_state_dict if "encoder.mid.attn" in key]
+    paths = renew_vae_attention_paths(mid_attentions)
+    meta_path = {"old": "mid.attn_1", "new": "mid_block.attentions.0"}
+    assign_to_checkpoint(
+        paths,
+        new_checkpoint,
+        vae_state_dict,
+        additional_replacements=[meta_path],
+        config=config,
+    )
+    conv_attn_to_linear(new_checkpoint)
+
+    for i in range(num_up_blocks):
+        block_id = num_up_blocks - 1 - i
+        resnets = [
+            key
+            for key in up_blocks[block_id]
+            if f"up.{block_id}" in key and f"up.{block_id}.upsample" not in key
+        ]
+
+        if f"decoder.up.{block_id}.upsample.conv.weight" in vae_state_dict:
+            new_checkpoint[f"decoder.up_blocks.{i}.upsamplers.0.conv.weight"] = (
+                vae_state_dict[f"decoder.up.{block_id}.upsample.conv.weight"]
+            )
+            new_checkpoint[f"decoder.up_blocks.{i}.upsamplers.0.conv.bias"] = (
+                vae_state_dict[f"decoder.up.{block_id}.upsample.conv.bias"]
+            )
+
+        paths = renew_vae_resnet_paths(resnets)
+        meta_path = {"old": f"up.{block_id}.block", "new": f"up_blocks.{i}.resnets"}
+        assign_to_checkpoint(
+            paths,
+            new_checkpoint,
+            vae_state_dict,
+            additional_replacements=[meta_path],
+            config=config,
+        )
+
+    mid_resnets = [key for key in vae_state_dict if "decoder.mid.block" in key]
+    num_mid_res_blocks = 2
+    for i in range(1, num_mid_res_blocks + 1):
+        resnets = [key for key in mid_resnets if f"decoder.mid.block_{i}" in key]
+
+        paths = renew_vae_resnet_paths(resnets)
+        meta_path = {"old": f"mid.block_{i}", "new": f"mid_block.resnets.{i - 1}"}
+        assign_to_checkpoint(
+            paths,
+            new_checkpoint,
+            vae_state_dict,
+            additional_replacements=[meta_path],
+            config=config,
+        )
+
+    mid_attentions = [key for key in vae_state_dict if "decoder.mid.attn" in key]
+    paths = renew_vae_attention_paths(mid_attentions)
+    meta_path = {"old": "mid.attn_1", "new": "mid_block.attentions.0"}
+    assign_to_checkpoint(
+        paths,
+        new_checkpoint,
+        vae_state_dict,
+        additional_replacements=[meta_path],
+        config=config,
+    )
+    conv_attn_to_linear(new_checkpoint)
+    return new_checkpoint
+
+
+def create_unet_diffusers_config(v2, use_linear_projection_in_v2=False):
+    """
+    Creates a config for the diffusers based on the config of the LDM model.
+    """
+    # unet_params = original_config.model.params.unet_config.params
+
+    block_out_channels = [
+        UNET_PARAMS_MODEL_CHANNELS * mult for mult in UNET_PARAMS_CHANNEL_MULT
+    ]
+
+    down_block_types = []
+    resolution = 1
+    for i in range(len(block_out_channels)):
+        block_type = (
+            "CrossAttnDownBlock2D"
+            if resolution in UNET_PARAMS_ATTENTION_RESOLUTIONS
+            else "DownBlock2D"
+        )
+        down_block_types.append(block_type)
+        if i != len(block_out_channels) - 1:
+            resolution *= 2
+
+    up_block_types = []
+    for i in range(len(block_out_channels)):
+        block_type = (
+            "CrossAttnUpBlock2D"
+            if resolution in UNET_PARAMS_ATTENTION_RESOLUTIONS
+            else "UpBlock2D"
+        )
+        up_block_types.append(block_type)
+        resolution //= 2
+
+    config = dict(
+        sample_size=UNET_PARAMS_IMAGE_SIZE,
+        in_channels=UNET_PARAMS_IN_CHANNELS,
+        out_channels=UNET_PARAMS_OUT_CHANNELS,
+        down_block_types=tuple(down_block_types),
+        up_block_types=tuple(up_block_types),
+        block_out_channels=tuple(block_out_channels),
+        layers_per_block=UNET_PARAMS_NUM_RES_BLOCKS,
+        cross_attention_dim=(
+            UNET_PARAMS_CONTEXT_DIM if not v2 else V2_UNET_PARAMS_CONTEXT_DIM
+        ),
+        attention_head_dim=(
+            UNET_PARAMS_NUM_HEADS if not v2 else V2_UNET_PARAMS_ATTENTION_HEAD_DIM
+        ),
+        # use_linear_projection=UNET_PARAMS_USE_LINEAR_PROJECTION if not v2 else V2_UNET_PARAMS_USE_LINEAR_PROJECTION,
+    )
+    if v2 and use_linear_projection_in_v2:
+        config["use_linear_projection"] = True
+
+    return config
+
+
+def create_vae_diffusers_config():
+    """
+    Creates a config for the diffusers based on the config of the LDM model.
+    """
+    # vae_params = original_config.model.params.first_stage_config.params.ddconfig
+    # _ = original_config.model.params.first_stage_config.params.embed_dim
+    block_out_channels = [VAE_PARAMS_CH * mult for mult in VAE_PARAMS_CH_MULT]
+    down_block_types = ["DownEncoderBlock2D"] * len(block_out_channels)
+    up_block_types = ["UpDecoderBlock2D"] * len(block_out_channels)
+
+    config = dict(
+        sample_size=VAE_PARAMS_RESOLUTION,
+        in_channels=VAE_PARAMS_IN_CHANNELS,
+        out_channels=VAE_PARAMS_OUT_CH,
+        down_block_types=tuple(down_block_types),
+        up_block_types=tuple(up_block_types),
+        block_out_channels=tuple(block_out_channels),
+        latent_channels=VAE_PARAMS_Z_CHANNELS,
+        layers_per_block=VAE_PARAMS_NUM_RES_BLOCKS,
+    )
+    return config
+
+
+def convert_ldm_clip_checkpoint_v1(checkpoint):
+    keys = list(checkpoint.keys())
+    text_model_dict = {}
+    for key in keys:
+        if key.startswith("cond_stage_model.transformer"):
+            text_model_dict[key[len("cond_stage_model.transformer.") :]] = checkpoint[
+                key
+            ]
+    return text_model_dict
+
+
+def convert_ldm_clip_checkpoint_v2(checkpoint, max_length):
+    # 嫌になるくらい違うぞ！
+    def convert_key(key):
+        if not key.startswith("cond_stage_model"):
+            return None
+
+        # common conversion
+        key = key.replace("cond_stage_model.model.transformer.", "text_model.encoder.")
+        key = key.replace("cond_stage_model.model.", "text_model.")
+
+        if "resblocks" in key:
+            # resblocks conversion
+            key = key.replace(".resblocks.", ".layers.")
+            if ".ln_" in key:
+                key = key.replace(".ln_", ".layer_norm")
+            elif ".mlp." in key:
+                key = key.replace(".c_fc.", ".fc1.")
+                key = key.replace(".c_proj.", ".fc2.")
+            elif ".attn.out_proj" in key:
+                key = key.replace(".attn.out_proj.", ".self_attn.out_proj.")
+            elif ".attn.in_proj" in key:
+                key = None  # 特殊なので後で処理する
+            else:
+                raise ValueError(f"unexpected key in SD: {key}")
+        elif ".positional_embedding" in key:
+            key = key.replace(
+                ".positional_embedding", ".embeddings.position_embedding.weight"
+            )
+        elif ".text_projection" in key:
+            key = None  # 使われない???
+        elif ".logit_scale" in key:
+            key = None  # 使われない???
+        elif ".token_embedding" in key:
+            key = key.replace(
+                ".token_embedding.weight", ".embeddings.token_embedding.weight"
+            )
+        elif ".ln_final" in key:
+            key = key.replace(".ln_final", ".final_layer_norm")
+        return key
+
+    keys = list(checkpoint.keys())
+    new_sd = {}
+    for key in keys:
+        # remove resblocks 23
+        if ".resblocks.23." in key:
+            continue
+        new_key = convert_key(key)
+        if new_key is None:
+            continue
+        new_sd[new_key] = checkpoint[key]
+
+    # attnの変換
+    for key in keys:
+        if ".resblocks.23." in key:
+            continue
+        if ".resblocks" in key and ".attn.in_proj_" in key:
+            # 三つに分割
+            values = torch.chunk(checkpoint[key], 3)
+
+            key_suffix = ".weight" if "weight" in key else ".bias"
+            key_pfx = key.replace(
+                "cond_stage_model.model.transformer.resblocks.",
+                "text_model.encoder.layers.",
+            )
+            key_pfx = key_pfx.replace("_weight", "")
+            key_pfx = key_pfx.replace("_bias", "")
+            key_pfx = key_pfx.replace(".attn.in_proj", ".self_attn.")
+            new_sd[key_pfx + "q_proj" + key_suffix] = values[0]
+            new_sd[key_pfx + "k_proj" + key_suffix] = values[1]
+            new_sd[key_pfx + "v_proj" + key_suffix] = values[2]
+
+    # rename or add position_ids
+    ANOTHER_POSITION_IDS_KEY = "text_model.encoder.text_model.embeddings.position_ids"
+    if ANOTHER_POSITION_IDS_KEY in new_sd:
+        # waifu diffusion v1.4
+        position_ids = new_sd[ANOTHER_POSITION_IDS_KEY]
+        del new_sd[ANOTHER_POSITION_IDS_KEY]
+    else:
+        position_ids = torch.Tensor([list(range(max_length))]).to(torch.int64)
+
+    new_sd["text_model.embeddings.position_ids"] = position_ids
+    return new_sd
+
+
+# endregion
+
+
+# region Diffusers->StableDiffusion の変換コード
+# convert_diffusers_to_original_stable_diffusion をコピーして修正している（ASL 2.0）
+
+
+def conv_transformer_to_linear(checkpoint):
+    keys = list(checkpoint.keys())
+    tf_keys = ["proj_in.weight", "proj_out.weight"]
+    for key in keys:
+        if ".".join(key.split(".")[-2:]) in tf_keys:
+            if checkpoint[key].ndim > 2:
+                checkpoint[key] = checkpoint[key][:, :, 0, 0]
+
+
+def convert_unet_state_dict_to_sd(v2, unet_state_dict):
+    unet_conversion_map = [
+        # (stable-diffusion, HF Diffusers)
+        ("time_embed.0.weight", "time_embedding.linear_1.weight"),
+        ("time_embed.0.bias", "time_embedding.linear_1.bias"),
+        ("time_embed.2.weight", "time_embedding.linear_2.weight"),
+        ("time_embed.2.bias", "time_embedding.linear_2.bias"),
+        ("input_blocks.0.0.weight", "conv_in.weight"),
+        ("input_blocks.0.0.bias", "conv_in.bias"),
+        ("out.0.weight", "conv_norm_out.weight"),
+        ("out.0.bias", "conv_norm_out.bias"),
+        ("out.2.weight", "conv_out.weight"),
+        ("out.2.bias", "conv_out.bias"),
+    ]
+
+    unet_conversion_map_resnet = [
+        # (stable-diffusion, HF Diffusers)
+        ("in_layers.0", "norm1"),
+        ("in_layers.2", "conv1"),
+        ("out_layers.0", "norm2"),
+        ("out_layers.3", "conv2"),
+        ("emb_layers.1", "time_emb_proj"),
+        ("skip_connection", "conv_shortcut"),
+    ]
+
+    unet_conversion_map_layer = []
+    for i in range(4):
+        # loop over downblocks/upblocks
+
+        for j in range(2):
+            # loop over resnets/attentions for downblocks
+            hf_down_res_prefix = f"down_blocks.{i}.resnets.{j}."
+            sd_down_res_prefix = f"input_blocks.{3*i + j + 1}.0."
+            unet_conversion_map_layer.append((sd_down_res_prefix, hf_down_res_prefix))
+
+            if i < 3:
+                # no attention layers in down_blocks.3
+                hf_down_atn_prefix = f"down_blocks.{i}.attentions.{j}."
+                sd_down_atn_prefix = f"input_blocks.{3*i + j + 1}.1."
+                unet_conversion_map_layer.append(
+                    (sd_down_atn_prefix, hf_down_atn_prefix)
+                )
+
+        for j in range(3):
+            # loop over resnets/attentions for upblocks
+            hf_up_res_prefix = f"up_blocks.{i}.resnets.{j}."
+            sd_up_res_prefix = f"output_blocks.{3*i + j}.0."
+            unet_conversion_map_layer.append((sd_up_res_prefix, hf_up_res_prefix))
+
+            if i > 0:
+                # no attention layers in up_blocks.0
+                hf_up_atn_prefix = f"up_blocks.{i}.attentions.{j}."
+                sd_up_atn_prefix = f"output_blocks.{3*i + j}.1."
+                unet_conversion_map_layer.append((sd_up_atn_prefix, hf_up_atn_prefix))
+
+        if i < 3:
+            # no downsample in down_blocks.3
+            hf_downsample_prefix = f"down_blocks.{i}.downsamplers.0.conv."
+            sd_downsample_prefix = f"input_blocks.{3*(i+1)}.0.op."
+            unet_conversion_map_layer.append(
+                (sd_downsample_prefix, hf_downsample_prefix)
+            )
+
+            # no upsample in up_blocks.3
+            hf_upsample_prefix = f"up_blocks.{i}.upsamplers.0."
+            sd_upsample_prefix = f"output_blocks.{3*i + 2}.{1 if i == 0 else 2}."
+            unet_conversion_map_layer.append((sd_upsample_prefix, hf_upsample_prefix))
+
+    hf_mid_atn_prefix = "mid_block.attentions.0."
+    sd_mid_atn_prefix = "middle_block.1."
+    unet_conversion_map_layer.append((sd_mid_atn_prefix, hf_mid_atn_prefix))
+
+    for j in range(2):
+        hf_mid_res_prefix = f"mid_block.resnets.{j}."
+        sd_mid_res_prefix = f"middle_block.{2*j}."
+        unet_conversion_map_layer.append((sd_mid_res_prefix, hf_mid_res_prefix))
+
+    # buyer beware: this is a *brittle* function,
+    # and correct output requires that all of these pieces interact in
+    # the exact order in which I have arranged them.
+    mapping = {k: k for k in unet_state_dict.keys()}
+    for sd_name, hf_name in unet_conversion_map:
+        mapping[hf_name] = sd_name
+    for k, v in mapping.items():
+        if "resnets" in k:
+            for sd_part, hf_part in unet_conversion_map_resnet:
+                v = v.replace(hf_part, sd_part)
+            mapping[k] = v
+    for k, v in mapping.items():
+        for sd_part, hf_part in unet_conversion_map_layer:
+            v = v.replace(hf_part, sd_part)
+        mapping[k] = v
+    new_state_dict = {v: unet_state_dict[k] for k, v in mapping.items()}
+
+    if v2:
+        conv_transformer_to_linear(new_state_dict)
+
+    return new_state_dict
+
+
+def controlnet_conversion_map():
+    unet_conversion_map = [
+        ("time_embed.0.weight", "time_embedding.linear_1.weight"),
+        ("time_embed.0.bias", "time_embedding.linear_1.bias"),
+        ("time_embed.2.weight", "time_embedding.linear_2.weight"),
+        ("time_embed.2.bias", "time_embedding.linear_2.bias"),
+        ("input_blocks.0.0.weight", "conv_in.weight"),
+        ("input_blocks.0.0.bias", "conv_in.bias"),
+        ("middle_block_out.0.weight", "controlnet_mid_block.weight"),
+        ("middle_block_out.0.bias", "controlnet_mid_block.bias"),
+    ]
+
+    unet_conversion_map_resnet = [
+        ("in_layers.0", "norm1"),
+        ("in_layers.2", "conv1"),
+        ("out_layers.0", "norm2"),
+        ("out_layers.3", "conv2"),
+        ("emb_layers.1", "time_emb_proj"),
+        ("skip_connection", "conv_shortcut"),
+    ]
+
+    unet_conversion_map_layer = []
+    for i in range(4):
+        for j in range(2):
+            hf_down_res_prefix = f"down_blocks.{i}.resnets.{j}."
+            sd_down_res_prefix = f"input_blocks.{3*i + j + 1}.0."
+            unet_conversion_map_layer.append((sd_down_res_prefix, hf_down_res_prefix))
+
+            if i < 3:
+                hf_down_atn_prefix = f"down_blocks.{i}.attentions.{j}."
+                sd_down_atn_prefix = f"input_blocks.{3*i + j + 1}.1."
+                unet_conversion_map_layer.append(
+                    (sd_down_atn_prefix, hf_down_atn_prefix)
+                )
+
+        if i < 3:
+            hf_downsample_prefix = f"down_blocks.{i}.downsamplers.0.conv."
+            sd_downsample_prefix = f"input_blocks.{3*(i+1)}.0.op."
+            unet_conversion_map_layer.append(
+                (sd_downsample_prefix, hf_downsample_prefix)
+            )
+
+    hf_mid_atn_prefix = "mid_block.attentions.0."
+    sd_mid_atn_prefix = "middle_block.1."
+    unet_conversion_map_layer.append((sd_mid_atn_prefix, hf_mid_atn_prefix))
+
+    for j in range(2):
+        hf_mid_res_prefix = f"mid_block.resnets.{j}."
+        sd_mid_res_prefix = f"middle_block.{2*j}."
+        unet_conversion_map_layer.append((sd_mid_res_prefix, hf_mid_res_prefix))
+
+    controlnet_cond_embedding_names = (
+        ["conv_in"] + [f"blocks.{i}" for i in range(6)] + ["conv_out"]
+    )
+    for i, hf_prefix in enumerate(controlnet_cond_embedding_names):
+        hf_prefix = f"controlnet_cond_embedding.{hf_prefix}."
+        sd_prefix = f"input_hint_block.{i*2}."
+        unet_conversion_map_layer.append((sd_prefix, hf_prefix))
+
+    for i in range(12):
+        hf_prefix = f"controlnet_down_blocks.{i}."
+        sd_prefix = f"zero_convs.{i}.0."
+        unet_conversion_map_layer.append((sd_prefix, hf_prefix))
+
+    return unet_conversion_map, unet_conversion_map_resnet, unet_conversion_map_layer
+
+
+def convert_controlnet_state_dict_to_sd(controlnet_state_dict):
+    (
+        unet_conversion_map,
+        unet_conversion_map_resnet,
+        unet_conversion_map_layer,
+    ) = controlnet_conversion_map()
+
+    mapping = {k: k for k in controlnet_state_dict.keys()}
+    for sd_name, diffusers_name in unet_conversion_map:
+        mapping[diffusers_name] = sd_name
+    for k, v in mapping.items():
+        if "resnets" in k:
+            for sd_part, diffusers_part in unet_conversion_map_resnet:
+                v = v.replace(diffusers_part, sd_part)
+            mapping[k] = v
+    for k, v in mapping.items():
+        for sd_part, diffusers_part in unet_conversion_map_layer:
+            v = v.replace(diffusers_part, sd_part)
+        mapping[k] = v
+    new_state_dict = {v: controlnet_state_dict[k] for k, v in mapping.items()}
+    return new_state_dict
+
+
+def convert_controlnet_state_dict_to_diffusers(controlnet_state_dict):
+    (
+        unet_conversion_map,
+        unet_conversion_map_resnet,
+        unet_conversion_map_layer,
+    ) = controlnet_conversion_map()
+
+    mapping = {k: k for k in controlnet_state_dict.keys()}
+    for sd_name, diffusers_name in unet_conversion_map:
+        mapping[sd_name] = diffusers_name
+    for k, v in mapping.items():
+        for sd_part, diffusers_part in unet_conversion_map_layer:
+            v = v.replace(sd_part, diffusers_part)
+        mapping[k] = v
+    for k, v in mapping.items():
+        if "resnets" in v:
+            for sd_part, diffusers_part in unet_conversion_map_resnet:
+                v = v.replace(sd_part, diffusers_part)
+            mapping[k] = v
+    new_state_dict = {v: controlnet_state_dict[k] for k, v in mapping.items()}
+    return new_state_dict
+
+
+# ================#
+# VAE Conversion #
+# ================#
+
+
+def reshape_weight_for_sd(w):
+    # convert HF linear weights to SD conv2d weights
+    return w.reshape(*w.shape, 1, 1)
+
+
+def convert_vae_state_dict(vae_state_dict):
+    vae_conversion_map = [
+        # (stable-diffusion, HF Diffusers)
+        ("nin_shortcut", "conv_shortcut"),
+        ("norm_out", "conv_norm_out"),
+        ("mid.attn_1.", "mid_block.attentions.0."),
+    ]
+
+    for i in range(4):
+        # down_blocks have two resnets
+        for j in range(2):
+            hf_down_prefix = f"encoder.down_blocks.{i}.resnets.{j}."
+            sd_down_prefix = f"encoder.down.{i}.block.{j}."
+            vae_conversion_map.append((sd_down_prefix, hf_down_prefix))
+
+        if i < 3:
+            hf_downsample_prefix = f"down_blocks.{i}.downsamplers.0."
+            sd_downsample_prefix = f"down.{i}.downsample."
+            vae_conversion_map.append((sd_downsample_prefix, hf_downsample_prefix))
+
+            hf_upsample_prefix = f"up_blocks.{i}.upsamplers.0."
+            sd_upsample_prefix = f"up.{3-i}.upsample."
+            vae_conversion_map.append((sd_upsample_prefix, hf_upsample_prefix))
+
+        # up_blocks have three resnets
+        # also, up blocks in hf are numbered in reverse from sd
+        for j in range(3):
+            hf_up_prefix = f"decoder.up_blocks.{i}.resnets.{j}."
+            sd_up_prefix = f"decoder.up.{3-i}.block.{j}."
+            vae_conversion_map.append((sd_up_prefix, hf_up_prefix))
+
+    # this part accounts for mid blocks in both the encoder and the decoder
+    for i in range(2):
+        hf_mid_res_prefix = f"mid_block.resnets.{i}."
+        sd_mid_res_prefix = f"mid.block_{i+1}."
+        vae_conversion_map.append((sd_mid_res_prefix, hf_mid_res_prefix))
+
+    if diffusers.__version__ < "0.17.0":
+        vae_conversion_map_attn = [
+            # (stable-diffusion, HF Diffusers)
+            ("norm.", "group_norm."),
+            ("q.", "query."),
+            ("k.", "key."),
+            ("v.", "value."),
+            ("proj_out.", "proj_attn."),
+        ]
+    else:
+        vae_conversion_map_attn = [
+            # (stable-diffusion, HF Diffusers)
+            ("norm.", "group_norm."),
+            ("q.", "to_q."),
+            ("k.", "to_k."),
+            ("v.", "to_v."),
+            ("proj_out.", "to_out.0."),
+        ]
+
+    mapping = {k: k for k in vae_state_dict.keys()}
+    for k, v in mapping.items():
+        for sd_part, hf_part in vae_conversion_map:
+            v = v.replace(hf_part, sd_part)
+        mapping[k] = v
+    for k, v in mapping.items():
+        if "attentions" in k:
+            for sd_part, hf_part in vae_conversion_map_attn:
+                v = v.replace(hf_part, sd_part)
+            mapping[k] = v
+    new_state_dict = {v: vae_state_dict[k] for k, v in mapping.items()}
+    weights_to_convert = ["q", "k", "v", "proj_out"]
+    for k, v in new_state_dict.items():
+        for weight_name in weights_to_convert:
+            if f"mid.attn_1.{weight_name}.weight" in k:
+                # print(f"Reshaping {k} for SD format: shape {v.shape} -> {v.shape} x 1 x 1")
+                new_state_dict[k] = reshape_weight_for_sd(v)
+
+    return new_state_dict
+
+
+# endregion
+
+# region 自作のモデル読み書きなど
+
+
+def is_safetensors(path):
+    return os.path.splitext(path)[1].lower() == ".safetensors"
+
+
+def load_checkpoint_with_text_encoder_conversion(ckpt_path, device="cpu"):
+    # text encoderの格納形式が違うモデルに対応する ('text_model'がない)
+    TEXT_ENCODER_KEY_REPLACEMENTS = [
+        (
+            "cond_stage_model.transformer.embeddings.",
+            "cond_stage_model.transformer.text_model.embeddings.",
+        ),
+        (
+            "cond_stage_model.transformer.encoder.",
+            "cond_stage_model.transformer.text_model.encoder.",
+        ),
+        (
+            "cond_stage_model.transformer.final_layer_norm.",
+            "cond_stage_model.transformer.text_model.final_layer_norm.",
+        ),
+    ]
+
+    if is_safetensors(ckpt_path):
+        checkpoint = None
+        state_dict = load_file(ckpt_path)  # , device) # may causes error
+    else:
+        checkpoint = torch.load(ckpt_path, map_location=device)
+        if "state_dict" in checkpoint:
+            state_dict = checkpoint["state_dict"]
+        else:
+            state_dict = checkpoint
+            checkpoint = None
+
+    key_reps = []
+    for rep_from, rep_to in TEXT_ENCODER_KEY_REPLACEMENTS:
+        for key in state_dict.keys():
+            if key.startswith(rep_from):
+                new_key = rep_to + key[len(rep_from) :]
+                key_reps.append((key, new_key))
+
+    for key, new_key in key_reps:
+        state_dict[new_key] = state_dict[key]
+        del state_dict[key]
+
+    return checkpoint, state_dict
+
+
+# TODO dtype指定の動作が怪しいので確認する text_encoderを指定形式で作れるか未確認
+def load_models_from_stable_diffusion_checkpoint(
+    v2, ckpt_path, device="cpu", dtype=None, unet_use_linear_projection_in_v2=True
+):
+    _, state_dict = load_checkpoint_with_text_encoder_conversion(ckpt_path, device)
+
+    # Convert the UNet2DConditionModel model.
+    unet_config = create_unet_diffusers_config(v2, unet_use_linear_projection_in_v2)
+    converted_unet_checkpoint = convert_ldm_unet_checkpoint(v2, state_dict, unet_config)
+
+    unet = UNet2DConditionModel(**unet_config).to(device)
+    info = unet.load_state_dict(converted_unet_checkpoint)
+    print("loading u-net:", info)
+
+    # Convert the VAE model.
+    vae_config = create_vae_diffusers_config()
+    converted_vae_checkpoint = convert_ldm_vae_checkpoint(state_dict, vae_config)
+
+    vae = AutoencoderKL(**vae_config).to(device)
+    info = vae.load_state_dict(converted_vae_checkpoint)
+    print("loading vae:", info)
+
+    # convert text_model
+    if v2:
+        converted_text_encoder_checkpoint = convert_ldm_clip_checkpoint_v2(
+            state_dict, 77
+        )
+        cfg = CLIPTextConfig(
+            vocab_size=49408,
+            hidden_size=1024,
+            intermediate_size=4096,
+            num_hidden_layers=23,
+            num_attention_heads=16,
+            max_position_embeddings=77,
+            hidden_act="gelu",
+            layer_norm_eps=1e-05,
+            dropout=0.0,
+            attention_dropout=0.0,
+            initializer_range=0.02,
+            initializer_factor=1.0,
+            pad_token_id=1,
+            bos_token_id=0,
+            eos_token_id=2,
+            model_type="clip_text_model",
+            projection_dim=512,
+            torch_dtype="float32",
+            transformers_version="4.25.0.dev0",
+        )
+        text_model = CLIPTextModel._from_config(cfg)
+        info = text_model.load_state_dict(
+            converted_text_encoder_checkpoint, strict=False
+        )
+    else:
+        converted_text_encoder_checkpoint = convert_ldm_clip_checkpoint_v1(state_dict)
+
+        # logging.set_verbosity_error()  # don't show annoying warning
+        # text_model = CLIPTextModel.from_pretrained("openai/clip-vit-large-patch14").to(device)
+        # logging.set_verbosity_warning()
+        # print(f"config: {text_model.config}")
+        cfg = CLIPTextConfig(
+            vocab_size=49408,
+            hidden_size=768,
+            intermediate_size=3072,
+            num_hidden_layers=12,
+            num_attention_heads=12,
+            max_position_embeddings=77,
+            hidden_act="quick_gelu",
+            layer_norm_eps=1e-05,
+            dropout=0.0,
+            attention_dropout=0.0,
+            initializer_range=0.02,
+            initializer_factor=1.0,
+            pad_token_id=1,
+            bos_token_id=0,
+            eos_token_id=2,
+            model_type="clip_text_model",
+            projection_dim=768,
+            torch_dtype="float32",
+        )
+        text_model = CLIPTextModel._from_config(cfg)
+        info = text_model.load_state_dict(
+            converted_text_encoder_checkpoint, strict=False
+        )
+    print("loading text encoder:", info)
+
+    return text_model, vae, unet
+
+
+def get_model_version_str_for_sd1_sd2(v2, v_parameterization):
+    # only for reference
+    version_str = "sd"
+    if v2:
+        version_str += "_v2"
+    else:
+        version_str += "_v1"
+    if v_parameterization:
+        version_str += "_v"
+    return version_str
+
+
+def convert_text_encoder_state_dict_to_sd_v2(checkpoint, make_dummy_weights=False):
+    def convert_key(key):
+        # position_idsの除去
+        if ".position_ids" in key:
+            return None
+
+        # common
+        key = key.replace("text_model.encoder.", "transformer.")
+        key = key.replace("text_model.", "")
+        if "layers" in key:
+            # resblocks conversion
+            key = key.replace(".layers.", ".resblocks.")
+            if ".layer_norm" in key:
+                key = key.replace(".layer_norm", ".ln_")
+            elif ".mlp." in key:
+                key = key.replace(".fc1.", ".c_fc.")
+                key = key.replace(".fc2.", ".c_proj.")
+            elif ".self_attn.out_proj" in key:
+                key = key.replace(".self_attn.out_proj.", ".attn.out_proj.")
+            elif ".self_attn." in key:
+                key = None  # 特殊なので後で処理する
+            else:
+                raise ValueError(f"unexpected key in DiffUsers model: {key}")
+        elif ".position_embedding" in key:
+            key = key.replace(
+                "embeddings.position_embedding.weight", "positional_embedding"
+            )
+        elif ".token_embedding" in key:
+            key = key.replace(
+                "embeddings.token_embedding.weight", "token_embedding.weight"
+            )
+        elif "final_layer_norm" in key:
+            key = key.replace("final_layer_norm", "ln_final")
+        return key
+
+    keys = list(checkpoint.keys())
+    new_sd = {}
+    for key in keys:
+        new_key = convert_key(key)
+        if new_key is None:
+            continue
+        new_sd[new_key] = checkpoint[key]
+
+    # attnの変換
+    for key in keys:
+        if "layers" in key and "q_proj" in key:
+            # 三つを結合
+            key_q = key
+            key_k = key.replace("q_proj", "k_proj")
+            key_v = key.replace("q_proj", "v_proj")
+
+            value_q = checkpoint[key_q]
+            value_k = checkpoint[key_k]
+            value_v = checkpoint[key_v]
+            value = torch.cat([value_q, value_k, value_v])
+
+            new_key = key.replace(
+                "text_model.encoder.layers.", "transformer.resblocks."
+            )
+            new_key = new_key.replace(".self_attn.q_proj.", ".attn.in_proj_")
+            new_sd[new_key] = value
+
+    # 最後の層などを捏造するか
+    if make_dummy_weights:
+        print("make dummy weights for resblock.23, text_projection and logit scale.")
+        keys = list(new_sd.keys())
+        for key in keys:
+            if key.startswith("transformer.resblocks.22."):
+                new_sd[key.replace(".22.", ".23.")] = new_sd[
+                    key
+                ].clone()  # copyしないとsafetensorsの保存で落ちる
+
+        # Diffusersに含まれない重みを作っておく
+        new_sd["text_projection"] = torch.ones(
+            (1024, 1024), dtype=new_sd[keys[0]].dtype, device=new_sd[keys[0]].device
+        )
+        new_sd["logit_scale"] = torch.tensor(1)
+
+    return new_sd
+
+
+def save_stable_diffusion_checkpoint(
+    v2,
+    output_file,
+    text_encoder,
+    unet,
+    ckpt_path,
+    epochs,
+    steps,
+    save_dtype=None,
+    vae=None,
+):
+    if ckpt_path is not None:
+        # epoch/stepを参照する。またVAEがメモリ上にないときなど、もう一度VAEを含めて読み込む
+        checkpoint, state_dict = load_checkpoint_with_text_encoder_conversion(ckpt_path)
+        if checkpoint is None:  # safetensors または state_dictのckpt
+            checkpoint = {}
+            strict = False
+        else:
+            strict = True
+        if "state_dict" in state_dict:
+            del state_dict["state_dict"]
+    else:
+        # 新しく作る
+        assert (
+            vae is not None
+        ), "VAE is required to save a checkpoint without a given checkpoint"
+        checkpoint = {}
+        state_dict = {}
+        strict = False
+
+    def update_sd(prefix, sd):
+        for k, v in sd.items():
+            key = prefix + k
+            assert not strict or key in state_dict, f"Illegal key in save SD: {key}"
+            if save_dtype is not None:
+                v = v.detach().clone().to("cpu").to(save_dtype)
+            state_dict[key] = v
+
+    # Convert the UNet model
+    unet_state_dict = convert_unet_state_dict_to_sd(v2, unet.state_dict())
+    update_sd("model.diffusion_model.", unet_state_dict)
+
+    # Convert the text encoder model
+    if v2:
+        make_dummy = (
+            ckpt_path is None
+        )  # 参照元のcheckpointがない場合は最後の層を前の層から複製して作るなどダミーの重みを入れる
+        text_enc_dict = convert_text_encoder_state_dict_to_sd_v2(
+            text_encoder.state_dict(), make_dummy
+        )
+        update_sd("cond_stage_model.model.", text_enc_dict)
+    else:
+        text_enc_dict = text_encoder.state_dict()
+        update_sd("cond_stage_model.transformer.", text_enc_dict)
+
+    # Convert the VAE
+    if vae is not None:
+        vae_dict = convert_vae_state_dict(vae.state_dict())
+        update_sd("first_stage_model.", vae_dict)
+
+    # Put together new checkpoint
+    key_count = len(state_dict.keys())
+    new_ckpt = {"state_dict": state_dict}
+
+    # epoch and global_step are sometimes not int
+    try:
+        if "epoch" in checkpoint:
+            epochs += checkpoint["epoch"]
+        if "global_step" in checkpoint:
+            steps += checkpoint["global_step"]
+    except:
+        pass
+
+    new_ckpt["epoch"] = epochs
+    new_ckpt["global_step"] = steps
+
+    if is_safetensors(output_file):
+        # TODO Tensor以外のdictの値を削除したほうがいいか
+        save_file(state_dict, output_file)
+    else:
+        torch.save(new_ckpt, output_file)
+
+    return key_count
+
+
+def save_diffusers_checkpoint(
+    v2,
+    output_dir,
+    text_encoder,
+    unet,
+    pretrained_model_name_or_path,
+    vae=None,
+    use_safetensors=False,
+):
+    if pretrained_model_name_or_path is None:
+        # load default settings for v1/v2
+        if v2:
+            pretrained_model_name_or_path = DIFFUSERS_REF_MODEL_ID_V2
+        else:
+            pretrained_model_name_or_path = DIFFUSERS_REF_MODEL_ID_V1
+
+    scheduler = DDIMScheduler.from_pretrained(
+        pretrained_model_name_or_path, subfolder="scheduler"
+    )
+    tokenizer = CLIPTokenizer.from_pretrained(
+        pretrained_model_name_or_path, subfolder="tokenizer"
+    )
+    if vae is None:
+        vae = AutoencoderKL.from_pretrained(
+            pretrained_model_name_or_path, subfolder="vae"
+        )
+
+    pipeline = StableDiffusionPipeline(
+        unet=unet,
+        text_encoder=text_encoder,
+        vae=vae,
+        scheduler=scheduler,
+        tokenizer=tokenizer,
+        safety_checker=None,
+        feature_extractor=None,
+        requires_safety_checker=None,
+    )
+    pipeline.save_pretrained(output_dir, safe_serialization=use_safetensors)
+
+
+VAE_PREFIX = "first_stage_model."
+
+
+def load_vae(vae_id, dtype):
+    print(f"load VAE: {vae_id}")
+    if os.path.isdir(vae_id) or not os.path.isfile(vae_id):
+        # Diffusers local/remote
+        try:
+            vae = AutoencoderKL.from_pretrained(
+                vae_id, subfolder=None, torch_dtype=dtype
+            )
+        except EnvironmentError as e:
+            print(f"exception occurs in loading vae: {e}")
+            print("retry with subfolder='vae'")
+            vae = AutoencoderKL.from_pretrained(
+                vae_id, subfolder="vae", torch_dtype=dtype
+            )
+        return vae
+
+    # local
+    vae_config = create_vae_diffusers_config()
+
+    if vae_id.endswith(".bin"):
+        # SD 1.5 VAE on Huggingface
+        converted_vae_checkpoint = torch.load(vae_id, map_location="cpu")
+    else:
+        # StableDiffusion
+        vae_model = (
+            load_file(vae_id, "cpu")
+            if is_safetensors(vae_id)
+            else torch.load(vae_id, map_location="cpu")
+        )
+        vae_sd = vae_model["state_dict"] if "state_dict" in vae_model else vae_model
+
+        # vae only or full model
+        full_model = False
+        for vae_key in vae_sd:
+            if vae_key.startswith(VAE_PREFIX):
+                full_model = True
+                break
+        if not full_model:
+            sd = {}
+            for key, value in vae_sd.items():
+                sd[VAE_PREFIX + key] = value
+            vae_sd = sd
+            del sd
+
+        # Convert the VAE model.
+        converted_vae_checkpoint = convert_ldm_vae_checkpoint(vae_sd, vae_config)
+
+    vae = AutoencoderKL(**vae_config)
+    vae.load_state_dict(converted_vae_checkpoint)
+    return vae
+
+
+# endregion
+
+
+def make_bucket_resolutions(max_reso, min_size=256, max_size=1024, divisible=64):
+    max_width, max_height = max_reso
+    max_area = (max_width // divisible) * (max_height // divisible)
+
+    resos = set()
+
+    size = int(math.sqrt(max_area)) * divisible
+    resos.add((size, size))
+
+    size = min_size
+    while size <= max_size:
+        width = size
+        height = min(max_size, (max_area // (width // divisible)) * divisible)
+        resos.add((width, height))
+        resos.add((height, width))
+
+        # # make additional resos
+        # if width >= height and width - divisible >= min_size:
+        #   resos.add((width - divisible, height))
+        #   resos.add((height, width - divisible))
+        # if height >= width and height - divisible >= min_size:
+        #   resos.add((width, height - divisible))
+        #   resos.add((height - divisible, width))
+
+        size += divisible
+
+    resos = list(resos)
+    resos.sort()
+    return resos
+
+
+if __name__ == "__main__":
+    resos = make_bucket_resolutions((512, 768))
+    print(len(resos))
+    print(resos)
+    aspect_ratios = [w / h for w, h in resos]
+    print(aspect_ratios)
+
+    ars = set()
+    for ar in aspect_ratios:
+        if ar in ars:
+            print("error! duplicate ar:", ar)
+        ars.add(ar)
```

### Comparing `lycoris_lora-2.3.0.dev4/lycoris/kohya/sdxl_model_util.py` & `lycoris_lora-2.3.0.dev5/lycoris/kohya/sdxl_model_util.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,581 +1,581 @@
-import torch
-from safetensors.torch import load_file, save_file
-from transformers import (
-    CLIPTextModel,
-    CLIPTextConfig,
-    CLIPTextModelWithProjection,
-    CLIPTokenizer,
-)
-from diffusers import AutoencoderKL, EulerDiscreteScheduler, UNet2DConditionModel
-from . import model_utils as model_util
-from . import sdxl_original_unet
-
-
-VAE_SCALE_FACTOR = 0.13025
-MODEL_VERSION_SDXL_BASE_V0_9 = "sdxl_base_v0-9"
-
-# Diffusersの設定を読み込むための参照モデル
-DIFFUSERS_REF_MODEL_ID_SDXL = (
-    "stabilityai/stable-diffusion-xl-base-0.9"  # アクセス権が必要
-)
-
-DIFFUSERS_SDXL_UNET_CONFIG = {
-    "act_fn": "silu",
-    "addition_embed_type": "text_time",
-    "addition_embed_type_num_heads": 64,
-    "addition_time_embed_dim": 256,
-    "attention_head_dim": [5, 10, 20],
-    "block_out_channels": [320, 640, 1280],
-    "center_input_sample": False,
-    "class_embed_type": None,
-    "class_embeddings_concat": False,
-    "conv_in_kernel": 3,
-    "conv_out_kernel": 3,
-    "cross_attention_dim": 2048,
-    "cross_attention_norm": None,
-    "down_block_types": ["DownBlock2D", "CrossAttnDownBlock2D", "CrossAttnDownBlock2D"],
-    "downsample_padding": 1,
-    "dual_cross_attention": False,
-    "encoder_hid_dim": None,
-    "encoder_hid_dim_type": None,
-    "flip_sin_to_cos": True,
-    "freq_shift": 0,
-    "in_channels": 4,
-    "layers_per_block": 2,
-    "mid_block_only_cross_attention": None,
-    "mid_block_scale_factor": 1,
-    "mid_block_type": "UNetMidBlock2DCrossAttn",
-    "norm_eps": 1e-05,
-    "norm_num_groups": 32,
-    "num_attention_heads": None,
-    "num_class_embeds": None,
-    "only_cross_attention": False,
-    "out_channels": 4,
-    "projection_class_embeddings_input_dim": 2816,
-    "resnet_out_scale_factor": 1.0,
-    "resnet_skip_time_act": False,
-    "resnet_time_scale_shift": "default",
-    "sample_size": 128,
-    "time_cond_proj_dim": None,
-    "time_embedding_act_fn": None,
-    "time_embedding_dim": None,
-    "time_embedding_type": "positional",
-    "timestep_post_act": None,
-    "transformer_layers_per_block": [1, 2, 10],
-    "up_block_types": ["CrossAttnUpBlock2D", "CrossAttnUpBlock2D", "UpBlock2D"],
-    "upcast_attention": False,
-    "use_linear_projection": True,
-}
-
-
-def convert_sdxl_text_encoder_2_checkpoint(checkpoint, max_length):
-    SDXL_KEY_PREFIX = "conditioner.embedders.1.model."
-
-    # SD2のと、基本的には同じ。logit_scaleを後で使うので、それを追加で返す
-    # logit_scaleはcheckpointの保存時に使用する
-    def convert_key(key):
-        # common conversion
-        key = key.replace(SDXL_KEY_PREFIX + "transformer.", "text_model.encoder.")
-        key = key.replace(SDXL_KEY_PREFIX, "text_model.")
-
-        if "resblocks" in key:
-            # resblocks conversion
-            key = key.replace(".resblocks.", ".layers.")
-            if ".ln_" in key:
-                key = key.replace(".ln_", ".layer_norm")
-            elif ".mlp." in key:
-                key = key.replace(".c_fc.", ".fc1.")
-                key = key.replace(".c_proj.", ".fc2.")
-            elif ".attn.out_proj" in key:
-                key = key.replace(".attn.out_proj.", ".self_attn.out_proj.")
-            elif ".attn.in_proj" in key:
-                key = None  # 特殊なので後で処理する
-            else:
-                raise ValueError(f"unexpected key in SD: {key}")
-        elif ".positional_embedding" in key:
-            key = key.replace(
-                ".positional_embedding", ".embeddings.position_embedding.weight"
-            )
-        elif ".text_projection" in key:
-            key = key.replace("text_model.text_projection", "text_projection.weight")
-        elif ".logit_scale" in key:
-            key = None  # 後で処理する
-        elif ".token_embedding" in key:
-            key = key.replace(
-                ".token_embedding.weight", ".embeddings.token_embedding.weight"
-            )
-        elif ".ln_final" in key:
-            key = key.replace(".ln_final", ".final_layer_norm")
-        # ckpt from comfy has this key: text_model.encoder.text_model.embeddings.position_ids
-        elif ".embeddings.position_ids" in key:
-            key = None  # remove this key: make position_ids by ourselves
-        return key
-
-    keys = list(checkpoint.keys())
-    new_sd = {}
-    for key in keys:
-        new_key = convert_key(key)
-        if new_key is None:
-            continue
-        new_sd[new_key] = checkpoint[key]
-
-    # attnの変換
-    for key in keys:
-        if ".resblocks" in key and ".attn.in_proj_" in key:
-            # 三つに分割
-            values = torch.chunk(checkpoint[key], 3)
-
-            key_suffix = ".weight" if "weight" in key else ".bias"
-            key_pfx = key.replace(
-                SDXL_KEY_PREFIX + "transformer.resblocks.", "text_model.encoder.layers."
-            )
-            key_pfx = key_pfx.replace("_weight", "")
-            key_pfx = key_pfx.replace("_bias", "")
-            key_pfx = key_pfx.replace(".attn.in_proj", ".self_attn.")
-            new_sd[key_pfx + "q_proj" + key_suffix] = values[0]
-            new_sd[key_pfx + "k_proj" + key_suffix] = values[1]
-            new_sd[key_pfx + "v_proj" + key_suffix] = values[2]
-
-    # original SD にはないので、position_idsを追加
-    position_ids = torch.Tensor([list(range(max_length))]).to(torch.int64)
-    new_sd["text_model.embeddings.position_ids"] = position_ids
-
-    # logit_scale はDiffusersには含まれないが、保存時に戻したいので別途返す
-    logit_scale = checkpoint.get(SDXL_KEY_PREFIX + "logit_scale", None)
-
-    return new_sd, logit_scale
-
-
-def load_models_from_sdxl_checkpoint(model_version, ckpt_path, map_location):
-    # model_version is reserved for future use
-
-    # Load the state dict
-    if model_util.is_safetensors(ckpt_path):
-        checkpoint = None
-        state_dict = load_file(ckpt_path, device=map_location)
-        epoch = None
-        global_step = None
-    else:
-        checkpoint = torch.load(ckpt_path, map_location=map_location)
-        if "state_dict" in checkpoint:
-            state_dict = checkpoint["state_dict"]
-            epoch = checkpoint.get("epoch", 0)
-            global_step = checkpoint.get("global_step", 0)
-        else:
-            state_dict = checkpoint
-            epoch = 0
-            global_step = 0
-        checkpoint = None
-
-    # U-Net
-    print("building U-Net")
-    unet = sdxl_original_unet.SdxlUNet2DConditionModel()
-
-    print("loading U-Net from checkpoint")
-    unet_sd = {}
-    for k in list(state_dict.keys()):
-        if k.startswith("model.diffusion_model."):
-            unet_sd[k.replace("model.diffusion_model.", "")] = state_dict.pop(k)
-    info = unet.load_state_dict(unet_sd)
-    print("U-Net: ", info)
-    del unet_sd
-
-    # Text Encoders
-    print("building text encoders")
-
-    # Text Encoder 1 is same to Stability AI's SDXL
-    text_model1_cfg = CLIPTextConfig(
-        vocab_size=49408,
-        hidden_size=768,
-        intermediate_size=3072,
-        num_hidden_layers=12,
-        num_attention_heads=12,
-        max_position_embeddings=77,
-        hidden_act="quick_gelu",
-        layer_norm_eps=1e-05,
-        dropout=0.0,
-        attention_dropout=0.0,
-        initializer_range=0.02,
-        initializer_factor=1.0,
-        pad_token_id=1,
-        bos_token_id=0,
-        eos_token_id=2,
-        model_type="clip_text_model",
-        projection_dim=768,
-        # torch_dtype="float32",
-        # transformers_version="4.25.0.dev0",
-    )
-    text_model1 = CLIPTextModel._from_config(text_model1_cfg)
-
-    # Text Encoder 2 is different from Stability AI's SDXL. SDXL uses open clip, but we use the model from HuggingFace.
-    # Note: Tokenizer from HuggingFace is different from SDXL. We must use open clip's tokenizer.
-    text_model2_cfg = CLIPTextConfig(
-        vocab_size=49408,
-        hidden_size=1280,
-        intermediate_size=5120,
-        num_hidden_layers=32,
-        num_attention_heads=20,
-        max_position_embeddings=77,
-        hidden_act="gelu",
-        layer_norm_eps=1e-05,
-        dropout=0.0,
-        attention_dropout=0.0,
-        initializer_range=0.02,
-        initializer_factor=1.0,
-        pad_token_id=1,
-        bos_token_id=0,
-        eos_token_id=2,
-        model_type="clip_text_model",
-        projection_dim=1280,
-        # torch_dtype="float32",
-        # transformers_version="4.25.0.dev0",
-    )
-    text_model2 = CLIPTextModelWithProjection(text_model2_cfg)
-
-    print("loading text encoders from checkpoint")
-    te1_sd = {}
-    te2_sd = {}
-    for k in list(state_dict.keys()):
-        if k.startswith("conditioner.embedders.0.transformer."):
-            te1_sd[k.replace("conditioner.embedders.0.transformer.", "")] = (
-                state_dict.pop(k)
-            )
-        elif k.startswith("conditioner.embedders.1.model."):
-            te2_sd[k] = state_dict.pop(k)
-
-    info1 = text_model1.load_state_dict(te1_sd, strict=False)
-    print("text encoder 1:", info1)
-
-    converted_sd, logit_scale = convert_sdxl_text_encoder_2_checkpoint(
-        te2_sd, max_length=77
-    )
-    info2 = text_model2.load_state_dict(converted_sd, strict=False)
-    print("text encoder 2:", info2)
-
-    # prepare vae
-    print("building VAE")
-    vae_config = model_util.create_vae_diffusers_config()
-    vae = AutoencoderKL(**vae_config)  # .to(device)
-
-    print("loading VAE from checkpoint")
-    converted_vae_checkpoint = model_util.convert_ldm_vae_checkpoint(
-        state_dict, vae_config
-    )
-    info = vae.load_state_dict(converted_vae_checkpoint)
-    print("VAE:", info)
-
-    ckpt_info = (epoch, global_step) if epoch is not None else None
-    return text_model1, text_model2, vae, unet, logit_scale, ckpt_info
-
-
-def make_unet_conversion_map():
-    unet_conversion_map_layer = []
-
-    for i in range(3):  # num_blocks is 3 in sdxl
-        # loop over downblocks/upblocks
-        for j in range(2):
-            # loop over resnets/attentions for downblocks
-            hf_down_res_prefix = f"down_blocks.{i}.resnets.{j}."
-            sd_down_res_prefix = f"input_blocks.{3*i + j + 1}.0."
-            unet_conversion_map_layer.append((sd_down_res_prefix, hf_down_res_prefix))
-
-            if i < 3:
-                # no attention layers in down_blocks.3
-                hf_down_atn_prefix = f"down_blocks.{i}.attentions.{j}."
-                sd_down_atn_prefix = f"input_blocks.{3*i + j + 1}.1."
-                unet_conversion_map_layer.append(
-                    (sd_down_atn_prefix, hf_down_atn_prefix)
-                )
-
-        for j in range(3):
-            # loop over resnets/attentions for upblocks
-            hf_up_res_prefix = f"up_blocks.{i}.resnets.{j}."
-            sd_up_res_prefix = f"output_blocks.{3*i + j}.0."
-            unet_conversion_map_layer.append((sd_up_res_prefix, hf_up_res_prefix))
-
-            # if i > 0: commentout for sdxl
-            # no attention layers in up_blocks.0
-            hf_up_atn_prefix = f"up_blocks.{i}.attentions.{j}."
-            sd_up_atn_prefix = f"output_blocks.{3*i + j}.1."
-            unet_conversion_map_layer.append((sd_up_atn_prefix, hf_up_atn_prefix))
-
-        if i < 3:
-            # no downsample in down_blocks.3
-            hf_downsample_prefix = f"down_blocks.{i}.downsamplers.0.conv."
-            sd_downsample_prefix = f"input_blocks.{3*(i+1)}.0.op."
-            unet_conversion_map_layer.append(
-                (sd_downsample_prefix, hf_downsample_prefix)
-            )
-
-            # no upsample in up_blocks.3
-            hf_upsample_prefix = f"up_blocks.{i}.upsamplers.0."
-            sd_upsample_prefix = f"output_blocks.{3*i + 2}.{2}."  # change for sdxl
-            unet_conversion_map_layer.append((sd_upsample_prefix, hf_upsample_prefix))
-
-    hf_mid_atn_prefix = "mid_block.attentions.0."
-    sd_mid_atn_prefix = "middle_block.1."
-    unet_conversion_map_layer.append((sd_mid_atn_prefix, hf_mid_atn_prefix))
-
-    for j in range(2):
-        hf_mid_res_prefix = f"mid_block.resnets.{j}."
-        sd_mid_res_prefix = f"middle_block.{2*j}."
-        unet_conversion_map_layer.append((sd_mid_res_prefix, hf_mid_res_prefix))
-
-    unet_conversion_map_resnet = [
-        # (stable-diffusion, HF Diffusers)
-        ("in_layers.0.", "norm1."),
-        ("in_layers.2.", "conv1."),
-        ("out_layers.0.", "norm2."),
-        ("out_layers.3.", "conv2."),
-        ("emb_layers.1.", "time_emb_proj."),
-        ("skip_connection.", "conv_shortcut."),
-    ]
-
-    unet_conversion_map = []
-    for sd, hf in unet_conversion_map_layer:
-        if "resnets" in hf:
-            for sd_res, hf_res in unet_conversion_map_resnet:
-                unet_conversion_map.append((sd + sd_res, hf + hf_res))
-        else:
-            unet_conversion_map.append((sd, hf))
-
-    for j in range(2):
-        hf_time_embed_prefix = f"time_embedding.linear_{j+1}."
-        sd_time_embed_prefix = f"time_embed.{j*2}."
-        unet_conversion_map.append((sd_time_embed_prefix, hf_time_embed_prefix))
-
-    for j in range(2):
-        hf_label_embed_prefix = f"add_embedding.linear_{j+1}."
-        sd_label_embed_prefix = f"label_emb.0.{j*2}."
-        unet_conversion_map.append((sd_label_embed_prefix, hf_label_embed_prefix))
-
-    unet_conversion_map.append(("input_blocks.0.0.", "conv_in."))
-    unet_conversion_map.append(("out.0.", "conv_norm_out."))
-    unet_conversion_map.append(("out.2.", "conv_out."))
-
-    return unet_conversion_map
-
-
-def convert_diffusers_unet_state_dict_to_sdxl(du_sd):
-    unet_conversion_map = make_unet_conversion_map()
-
-    conversion_map = {hf: sd for sd, hf in unet_conversion_map}
-    return convert_unet_state_dict(du_sd, conversion_map)
-
-
-def convert_unet_state_dict(src_sd, conversion_map):
-    converted_sd = {}
-    for src_key, value in src_sd.items():
-        # さすがに全部回すのは時間がかかるので右から要素を削りつつprefixを探す
-        src_key_fragments = src_key.split(".")[:-1]  # remove weight/bias
-        while len(src_key_fragments) > 0:
-            src_key_prefix = ".".join(src_key_fragments) + "."
-            if src_key_prefix in conversion_map:
-                converted_prefix = conversion_map[src_key_prefix]
-                converted_key = converted_prefix + src_key[len(src_key_prefix) :]
-                converted_sd[converted_key] = value
-                break
-            src_key_fragments.pop(-1)
-        assert len(src_key_fragments) > 0, f"key {src_key} not found in conversion map"
-
-    return converted_sd
-
-
-def convert_sdxl_unet_state_dict_to_diffusers(sd):
-    unet_conversion_map = make_unet_conversion_map()
-
-    conversion_dict = {sd: hf for sd, hf in unet_conversion_map}
-    return convert_unet_state_dict(sd, conversion_dict)
-
-
-def convert_text_encoder_2_state_dict_to_sdxl(checkpoint, logit_scale):
-    def convert_key(key):
-        # position_idsの除去
-        if ".position_ids" in key:
-            return None
-
-        # common
-        key = key.replace("text_model.encoder.", "transformer.")
-        key = key.replace("text_model.", "")
-        if "layers" in key:
-            # resblocks conversion
-            key = key.replace(".layers.", ".resblocks.")
-            if ".layer_norm" in key:
-                key = key.replace(".layer_norm", ".ln_")
-            elif ".mlp." in key:
-                key = key.replace(".fc1.", ".c_fc.")
-                key = key.replace(".fc2.", ".c_proj.")
-            elif ".self_attn.out_proj" in key:
-                key = key.replace(".self_attn.out_proj.", ".attn.out_proj.")
-            elif ".self_attn." in key:
-                key = None  # 特殊なので後で処理する
-            else:
-                raise ValueError(f"unexpected key in DiffUsers model: {key}")
-        elif ".position_embedding" in key:
-            key = key.replace(
-                "embeddings.position_embedding.weight", "positional_embedding"
-            )
-        elif ".token_embedding" in key:
-            key = key.replace(
-                "embeddings.token_embedding.weight", "token_embedding.weight"
-            )
-        elif "text_projection" in key:  # no dot in key
-            key = key.replace("text_projection.weight", "text_projection")
-        elif "final_layer_norm" in key:
-            key = key.replace("final_layer_norm", "ln_final")
-        return key
-
-    keys = list(checkpoint.keys())
-    new_sd = {}
-    for key in keys:
-        new_key = convert_key(key)
-        if new_key is None:
-            continue
-        new_sd[new_key] = checkpoint[key]
-
-    # attnの変換
-    for key in keys:
-        if "layers" in key and "q_proj" in key:
-            # 三つを結合
-            key_q = key
-            key_k = key.replace("q_proj", "k_proj")
-            key_v = key.replace("q_proj", "v_proj")
-
-            value_q = checkpoint[key_q]
-            value_k = checkpoint[key_k]
-            value_v = checkpoint[key_v]
-            value = torch.cat([value_q, value_k, value_v])
-
-            new_key = key.replace(
-                "text_model.encoder.layers.", "transformer.resblocks."
-            )
-            new_key = new_key.replace(".self_attn.q_proj.", ".attn.in_proj_")
-            new_sd[new_key] = value
-
-    if logit_scale is not None:
-        new_sd["logit_scale"] = logit_scale
-
-    return new_sd
-
-
-def save_stable_diffusion_checkpoint(
-    output_file,
-    text_encoder1,
-    text_encoder2,
-    unet,
-    epochs,
-    steps,
-    ckpt_info,
-    vae,
-    logit_scale,
-    save_dtype=None,
-):
-    state_dict = {}
-
-    def update_sd(prefix, sd):
-        for k, v in sd.items():
-            key = prefix + k
-            if save_dtype is not None:
-                v = v.detach().clone().to("cpu").to(save_dtype)
-            state_dict[key] = v
-
-    # Convert the UNet model
-    update_sd("model.diffusion_model.", unet.state_dict())
-
-    # Convert the text encoders
-    update_sd("conditioner.embedders.0.transformer.", text_encoder1.state_dict())
-
-    text_enc2_dict = convert_text_encoder_2_state_dict_to_sdxl(
-        text_encoder2.state_dict(), logit_scale
-    )
-    update_sd("conditioner.embedders.1.model.", text_enc2_dict)
-
-    # Convert the VAE
-    vae_dict = model_util.convert_vae_state_dict(vae.state_dict())
-    update_sd("first_stage_model.", vae_dict)
-
-    # Put together new checkpoint
-    key_count = len(state_dict.keys())
-    new_ckpt = {"state_dict": state_dict}
-
-    # epoch and global_step are sometimes not int
-    if ckpt_info is not None:
-        epochs += ckpt_info[0]
-        steps += ckpt_info[1]
-
-    new_ckpt["epoch"] = epochs
-    new_ckpt["global_step"] = steps
-
-    if model_util.is_safetensors(output_file):
-        save_file(state_dict, output_file)
-    else:
-        torch.save(new_ckpt, output_file)
-
-    return key_count
-
-
-def save_diffusers_checkpoint(
-    output_dir,
-    text_encoder1,
-    text_encoder2,
-    unet,
-    pretrained_model_name_or_path,
-    vae=None,
-    use_safetensors=False,
-    save_dtype=None,
-):
-    from diffusers import StableDiffusionXLPipeline
-
-    # convert U-Net
-    unet_sd = unet.state_dict()
-    du_unet_sd = convert_sdxl_unet_state_dict_to_diffusers(unet_sd)
-
-    diffusers_unet = UNet2DConditionModel(**DIFFUSERS_SDXL_UNET_CONFIG)
-    if save_dtype is not None:
-        diffusers_unet.to(save_dtype)
-    diffusers_unet.load_state_dict(du_unet_sd)
-
-    # create pipeline to save
-    if pretrained_model_name_or_path is None:
-        pretrained_model_name_or_path = DIFFUSERS_REF_MODEL_ID_SDXL
-
-    scheduler = EulerDiscreteScheduler.from_pretrained(
-        pretrained_model_name_or_path, subfolder="scheduler"
-    )
-    tokenizer1 = CLIPTokenizer.from_pretrained(
-        pretrained_model_name_or_path, subfolder="tokenizer"
-    )
-    tokenizer2 = CLIPTokenizer.from_pretrained(
-        pretrained_model_name_or_path, subfolder="tokenizer_2"
-    )
-    if vae is None:
-        vae = AutoencoderKL.from_pretrained(
-            pretrained_model_name_or_path, subfolder="vae"
-        )
-
-    # prevent local path from being saved
-    def remove_name_or_path(model):
-        if hasattr(model, "config"):
-            model.config._name_or_path = None
-            model.config._name_or_path = None
-
-    remove_name_or_path(diffusers_unet)
-    remove_name_or_path(text_encoder1)
-    remove_name_or_path(text_encoder2)
-    remove_name_or_path(scheduler)
-    remove_name_or_path(tokenizer1)
-    remove_name_or_path(tokenizer2)
-    remove_name_or_path(vae)
-
-    pipeline = StableDiffusionXLPipeline(
-        unet=diffusers_unet,
-        text_encoder=text_encoder1,
-        text_encoder_2=text_encoder2,
-        vae=vae,
-        scheduler=scheduler,
-        tokenizer=tokenizer1,
-        tokenizer_2=tokenizer2,
-    )
-    if save_dtype is not None:
-        pipeline.to(None, save_dtype)
-    pipeline.save_pretrained(output_dir, safe_serialization=use_safetensors)
+import torch
+from safetensors.torch import load_file, save_file
+from transformers import (
+    CLIPTextModel,
+    CLIPTextConfig,
+    CLIPTextModelWithProjection,
+    CLIPTokenizer,
+)
+from diffusers import AutoencoderKL, EulerDiscreteScheduler, UNet2DConditionModel
+from . import model_utils as model_util
+from . import sdxl_original_unet
+
+
+VAE_SCALE_FACTOR = 0.13025
+MODEL_VERSION_SDXL_BASE_V0_9 = "sdxl_base_v0-9"
+
+# Diffusersの設定を読み込むための参照モデル
+DIFFUSERS_REF_MODEL_ID_SDXL = (
+    "stabilityai/stable-diffusion-xl-base-0.9"  # アクセス権が必要
+)
+
+DIFFUSERS_SDXL_UNET_CONFIG = {
+    "act_fn": "silu",
+    "addition_embed_type": "text_time",
+    "addition_embed_type_num_heads": 64,
+    "addition_time_embed_dim": 256,
+    "attention_head_dim": [5, 10, 20],
+    "block_out_channels": [320, 640, 1280],
+    "center_input_sample": False,
+    "class_embed_type": None,
+    "class_embeddings_concat": False,
+    "conv_in_kernel": 3,
+    "conv_out_kernel": 3,
+    "cross_attention_dim": 2048,
+    "cross_attention_norm": None,
+    "down_block_types": ["DownBlock2D", "CrossAttnDownBlock2D", "CrossAttnDownBlock2D"],
+    "downsample_padding": 1,
+    "dual_cross_attention": False,
+    "encoder_hid_dim": None,
+    "encoder_hid_dim_type": None,
+    "flip_sin_to_cos": True,
+    "freq_shift": 0,
+    "in_channels": 4,
+    "layers_per_block": 2,
+    "mid_block_only_cross_attention": None,
+    "mid_block_scale_factor": 1,
+    "mid_block_type": "UNetMidBlock2DCrossAttn",
+    "norm_eps": 1e-05,
+    "norm_num_groups": 32,
+    "num_attention_heads": None,
+    "num_class_embeds": None,
+    "only_cross_attention": False,
+    "out_channels": 4,
+    "projection_class_embeddings_input_dim": 2816,
+    "resnet_out_scale_factor": 1.0,
+    "resnet_skip_time_act": False,
+    "resnet_time_scale_shift": "default",
+    "sample_size": 128,
+    "time_cond_proj_dim": None,
+    "time_embedding_act_fn": None,
+    "time_embedding_dim": None,
+    "time_embedding_type": "positional",
+    "timestep_post_act": None,
+    "transformer_layers_per_block": [1, 2, 10],
+    "up_block_types": ["CrossAttnUpBlock2D", "CrossAttnUpBlock2D", "UpBlock2D"],
+    "upcast_attention": False,
+    "use_linear_projection": True,
+}
+
+
+def convert_sdxl_text_encoder_2_checkpoint(checkpoint, max_length):
+    SDXL_KEY_PREFIX = "conditioner.embedders.1.model."
+
+    # SD2のと、基本的には同じ。logit_scaleを後で使うので、それを追加で返す
+    # logit_scaleはcheckpointの保存時に使用する
+    def convert_key(key):
+        # common conversion
+        key = key.replace(SDXL_KEY_PREFIX + "transformer.", "text_model.encoder.")
+        key = key.replace(SDXL_KEY_PREFIX, "text_model.")
+
+        if "resblocks" in key:
+            # resblocks conversion
+            key = key.replace(".resblocks.", ".layers.")
+            if ".ln_" in key:
+                key = key.replace(".ln_", ".layer_norm")
+            elif ".mlp." in key:
+                key = key.replace(".c_fc.", ".fc1.")
+                key = key.replace(".c_proj.", ".fc2.")
+            elif ".attn.out_proj" in key:
+                key = key.replace(".attn.out_proj.", ".self_attn.out_proj.")
+            elif ".attn.in_proj" in key:
+                key = None  # 特殊なので後で処理する
+            else:
+                raise ValueError(f"unexpected key in SD: {key}")
+        elif ".positional_embedding" in key:
+            key = key.replace(
+                ".positional_embedding", ".embeddings.position_embedding.weight"
+            )
+        elif ".text_projection" in key:
+            key = key.replace("text_model.text_projection", "text_projection.weight")
+        elif ".logit_scale" in key:
+            key = None  # 後で処理する
+        elif ".token_embedding" in key:
+            key = key.replace(
+                ".token_embedding.weight", ".embeddings.token_embedding.weight"
+            )
+        elif ".ln_final" in key:
+            key = key.replace(".ln_final", ".final_layer_norm")
+        # ckpt from comfy has this key: text_model.encoder.text_model.embeddings.position_ids
+        elif ".embeddings.position_ids" in key:
+            key = None  # remove this key: make position_ids by ourselves
+        return key
+
+    keys = list(checkpoint.keys())
+    new_sd = {}
+    for key in keys:
+        new_key = convert_key(key)
+        if new_key is None:
+            continue
+        new_sd[new_key] = checkpoint[key]
+
+    # attnの変換
+    for key in keys:
+        if ".resblocks" in key and ".attn.in_proj_" in key:
+            # 三つに分割
+            values = torch.chunk(checkpoint[key], 3)
+
+            key_suffix = ".weight" if "weight" in key else ".bias"
+            key_pfx = key.replace(
+                SDXL_KEY_PREFIX + "transformer.resblocks.", "text_model.encoder.layers."
+            )
+            key_pfx = key_pfx.replace("_weight", "")
+            key_pfx = key_pfx.replace("_bias", "")
+            key_pfx = key_pfx.replace(".attn.in_proj", ".self_attn.")
+            new_sd[key_pfx + "q_proj" + key_suffix] = values[0]
+            new_sd[key_pfx + "k_proj" + key_suffix] = values[1]
+            new_sd[key_pfx + "v_proj" + key_suffix] = values[2]
+
+    # original SD にはないので、position_idsを追加
+    position_ids = torch.Tensor([list(range(max_length))]).to(torch.int64)
+    new_sd["text_model.embeddings.position_ids"] = position_ids
+
+    # logit_scale はDiffusersには含まれないが、保存時に戻したいので別途返す
+    logit_scale = checkpoint.get(SDXL_KEY_PREFIX + "logit_scale", None)
+
+    return new_sd, logit_scale
+
+
+def load_models_from_sdxl_checkpoint(model_version, ckpt_path, map_location):
+    # model_version is reserved for future use
+
+    # Load the state dict
+    if model_util.is_safetensors(ckpt_path):
+        checkpoint = None
+        state_dict = load_file(ckpt_path, device=map_location)
+        epoch = None
+        global_step = None
+    else:
+        checkpoint = torch.load(ckpt_path, map_location=map_location)
+        if "state_dict" in checkpoint:
+            state_dict = checkpoint["state_dict"]
+            epoch = checkpoint.get("epoch", 0)
+            global_step = checkpoint.get("global_step", 0)
+        else:
+            state_dict = checkpoint
+            epoch = 0
+            global_step = 0
+        checkpoint = None
+
+    # U-Net
+    print("building U-Net")
+    unet = sdxl_original_unet.SdxlUNet2DConditionModel()
+
+    print("loading U-Net from checkpoint")
+    unet_sd = {}
+    for k in list(state_dict.keys()):
+        if k.startswith("model.diffusion_model."):
+            unet_sd[k.replace("model.diffusion_model.", "")] = state_dict.pop(k)
+    info = unet.load_state_dict(unet_sd)
+    print("U-Net: ", info)
+    del unet_sd
+
+    # Text Encoders
+    print("building text encoders")
+
+    # Text Encoder 1 is same to Stability AI's SDXL
+    text_model1_cfg = CLIPTextConfig(
+        vocab_size=49408,
+        hidden_size=768,
+        intermediate_size=3072,
+        num_hidden_layers=12,
+        num_attention_heads=12,
+        max_position_embeddings=77,
+        hidden_act="quick_gelu",
+        layer_norm_eps=1e-05,
+        dropout=0.0,
+        attention_dropout=0.0,
+        initializer_range=0.02,
+        initializer_factor=1.0,
+        pad_token_id=1,
+        bos_token_id=0,
+        eos_token_id=2,
+        model_type="clip_text_model",
+        projection_dim=768,
+        # torch_dtype="float32",
+        # transformers_version="4.25.0.dev0",
+    )
+    text_model1 = CLIPTextModel._from_config(text_model1_cfg)
+
+    # Text Encoder 2 is different from Stability AI's SDXL. SDXL uses open clip, but we use the model from HuggingFace.
+    # Note: Tokenizer from HuggingFace is different from SDXL. We must use open clip's tokenizer.
+    text_model2_cfg = CLIPTextConfig(
+        vocab_size=49408,
+        hidden_size=1280,
+        intermediate_size=5120,
+        num_hidden_layers=32,
+        num_attention_heads=20,
+        max_position_embeddings=77,
+        hidden_act="gelu",
+        layer_norm_eps=1e-05,
+        dropout=0.0,
+        attention_dropout=0.0,
+        initializer_range=0.02,
+        initializer_factor=1.0,
+        pad_token_id=1,
+        bos_token_id=0,
+        eos_token_id=2,
+        model_type="clip_text_model",
+        projection_dim=1280,
+        # torch_dtype="float32",
+        # transformers_version="4.25.0.dev0",
+    )
+    text_model2 = CLIPTextModelWithProjection(text_model2_cfg)
+
+    print("loading text encoders from checkpoint")
+    te1_sd = {}
+    te2_sd = {}
+    for k in list(state_dict.keys()):
+        if k.startswith("conditioner.embedders.0.transformer."):
+            te1_sd[k.replace("conditioner.embedders.0.transformer.", "")] = (
+                state_dict.pop(k)
+            )
+        elif k.startswith("conditioner.embedders.1.model."):
+            te2_sd[k] = state_dict.pop(k)
+
+    info1 = text_model1.load_state_dict(te1_sd, strict=False)
+    print("text encoder 1:", info1)
+
+    converted_sd, logit_scale = convert_sdxl_text_encoder_2_checkpoint(
+        te2_sd, max_length=77
+    )
+    info2 = text_model2.load_state_dict(converted_sd, strict=False)
+    print("text encoder 2:", info2)
+
+    # prepare vae
+    print("building VAE")
+    vae_config = model_util.create_vae_diffusers_config()
+    vae = AutoencoderKL(**vae_config)  # .to(device)
+
+    print("loading VAE from checkpoint")
+    converted_vae_checkpoint = model_util.convert_ldm_vae_checkpoint(
+        state_dict, vae_config
+    )
+    info = vae.load_state_dict(converted_vae_checkpoint)
+    print("VAE:", info)
+
+    ckpt_info = (epoch, global_step) if epoch is not None else None
+    return text_model1, text_model2, vae, unet, logit_scale, ckpt_info
+
+
+def make_unet_conversion_map():
+    unet_conversion_map_layer = []
+
+    for i in range(3):  # num_blocks is 3 in sdxl
+        # loop over downblocks/upblocks
+        for j in range(2):
+            # loop over resnets/attentions for downblocks
+            hf_down_res_prefix = f"down_blocks.{i}.resnets.{j}."
+            sd_down_res_prefix = f"input_blocks.{3*i + j + 1}.0."
+            unet_conversion_map_layer.append((sd_down_res_prefix, hf_down_res_prefix))
+
+            if i < 3:
+                # no attention layers in down_blocks.3
+                hf_down_atn_prefix = f"down_blocks.{i}.attentions.{j}."
+                sd_down_atn_prefix = f"input_blocks.{3*i + j + 1}.1."
+                unet_conversion_map_layer.append(
+                    (sd_down_atn_prefix, hf_down_atn_prefix)
+                )
+
+        for j in range(3):
+            # loop over resnets/attentions for upblocks
+            hf_up_res_prefix = f"up_blocks.{i}.resnets.{j}."
+            sd_up_res_prefix = f"output_blocks.{3*i + j}.0."
+            unet_conversion_map_layer.append((sd_up_res_prefix, hf_up_res_prefix))
+
+            # if i > 0: commentout for sdxl
+            # no attention layers in up_blocks.0
+            hf_up_atn_prefix = f"up_blocks.{i}.attentions.{j}."
+            sd_up_atn_prefix = f"output_blocks.{3*i + j}.1."
+            unet_conversion_map_layer.append((sd_up_atn_prefix, hf_up_atn_prefix))
+
+        if i < 3:
+            # no downsample in down_blocks.3
+            hf_downsample_prefix = f"down_blocks.{i}.downsamplers.0.conv."
+            sd_downsample_prefix = f"input_blocks.{3*(i+1)}.0.op."
+            unet_conversion_map_layer.append(
+                (sd_downsample_prefix, hf_downsample_prefix)
+            )
+
+            # no upsample in up_blocks.3
+            hf_upsample_prefix = f"up_blocks.{i}.upsamplers.0."
+            sd_upsample_prefix = f"output_blocks.{3*i + 2}.{2}."  # change for sdxl
+            unet_conversion_map_layer.append((sd_upsample_prefix, hf_upsample_prefix))
+
+    hf_mid_atn_prefix = "mid_block.attentions.0."
+    sd_mid_atn_prefix = "middle_block.1."
+    unet_conversion_map_layer.append((sd_mid_atn_prefix, hf_mid_atn_prefix))
+
+    for j in range(2):
+        hf_mid_res_prefix = f"mid_block.resnets.{j}."
+        sd_mid_res_prefix = f"middle_block.{2*j}."
+        unet_conversion_map_layer.append((sd_mid_res_prefix, hf_mid_res_prefix))
+
+    unet_conversion_map_resnet = [
+        # (stable-diffusion, HF Diffusers)
+        ("in_layers.0.", "norm1."),
+        ("in_layers.2.", "conv1."),
+        ("out_layers.0.", "norm2."),
+        ("out_layers.3.", "conv2."),
+        ("emb_layers.1.", "time_emb_proj."),
+        ("skip_connection.", "conv_shortcut."),
+    ]
+
+    unet_conversion_map = []
+    for sd, hf in unet_conversion_map_layer:
+        if "resnets" in hf:
+            for sd_res, hf_res in unet_conversion_map_resnet:
+                unet_conversion_map.append((sd + sd_res, hf + hf_res))
+        else:
+            unet_conversion_map.append((sd, hf))
+
+    for j in range(2):
+        hf_time_embed_prefix = f"time_embedding.linear_{j+1}."
+        sd_time_embed_prefix = f"time_embed.{j*2}."
+        unet_conversion_map.append((sd_time_embed_prefix, hf_time_embed_prefix))
+
+    for j in range(2):
+        hf_label_embed_prefix = f"add_embedding.linear_{j+1}."
+        sd_label_embed_prefix = f"label_emb.0.{j*2}."
+        unet_conversion_map.append((sd_label_embed_prefix, hf_label_embed_prefix))
+
+    unet_conversion_map.append(("input_blocks.0.0.", "conv_in."))
+    unet_conversion_map.append(("out.0.", "conv_norm_out."))
+    unet_conversion_map.append(("out.2.", "conv_out."))
+
+    return unet_conversion_map
+
+
+def convert_diffusers_unet_state_dict_to_sdxl(du_sd):
+    unet_conversion_map = make_unet_conversion_map()
+
+    conversion_map = {hf: sd for sd, hf in unet_conversion_map}
+    return convert_unet_state_dict(du_sd, conversion_map)
+
+
+def convert_unet_state_dict(src_sd, conversion_map):
+    converted_sd = {}
+    for src_key, value in src_sd.items():
+        # さすがに全部回すのは時間がかかるので右から要素を削りつつprefixを探す
+        src_key_fragments = src_key.split(".")[:-1]  # remove weight/bias
+        while len(src_key_fragments) > 0:
+            src_key_prefix = ".".join(src_key_fragments) + "."
+            if src_key_prefix in conversion_map:
+                converted_prefix = conversion_map[src_key_prefix]
+                converted_key = converted_prefix + src_key[len(src_key_prefix) :]
+                converted_sd[converted_key] = value
+                break
+            src_key_fragments.pop(-1)
+        assert len(src_key_fragments) > 0, f"key {src_key} not found in conversion map"
+
+    return converted_sd
+
+
+def convert_sdxl_unet_state_dict_to_diffusers(sd):
+    unet_conversion_map = make_unet_conversion_map()
+
+    conversion_dict = {sd: hf for sd, hf in unet_conversion_map}
+    return convert_unet_state_dict(sd, conversion_dict)
+
+
+def convert_text_encoder_2_state_dict_to_sdxl(checkpoint, logit_scale):
+    def convert_key(key):
+        # position_idsの除去
+        if ".position_ids" in key:
+            return None
+
+        # common
+        key = key.replace("text_model.encoder.", "transformer.")
+        key = key.replace("text_model.", "")
+        if "layers" in key:
+            # resblocks conversion
+            key = key.replace(".layers.", ".resblocks.")
+            if ".layer_norm" in key:
+                key = key.replace(".layer_norm", ".ln_")
+            elif ".mlp." in key:
+                key = key.replace(".fc1.", ".c_fc.")
+                key = key.replace(".fc2.", ".c_proj.")
+            elif ".self_attn.out_proj" in key:
+                key = key.replace(".self_attn.out_proj.", ".attn.out_proj.")
+            elif ".self_attn." in key:
+                key = None  # 特殊なので後で処理する
+            else:
+                raise ValueError(f"unexpected key in DiffUsers model: {key}")
+        elif ".position_embedding" in key:
+            key = key.replace(
+                "embeddings.position_embedding.weight", "positional_embedding"
+            )
+        elif ".token_embedding" in key:
+            key = key.replace(
+                "embeddings.token_embedding.weight", "token_embedding.weight"
+            )
+        elif "text_projection" in key:  # no dot in key
+            key = key.replace("text_projection.weight", "text_projection")
+        elif "final_layer_norm" in key:
+            key = key.replace("final_layer_norm", "ln_final")
+        return key
+
+    keys = list(checkpoint.keys())
+    new_sd = {}
+    for key in keys:
+        new_key = convert_key(key)
+        if new_key is None:
+            continue
+        new_sd[new_key] = checkpoint[key]
+
+    # attnの変換
+    for key in keys:
+        if "layers" in key and "q_proj" in key:
+            # 三つを結合
+            key_q = key
+            key_k = key.replace("q_proj", "k_proj")
+            key_v = key.replace("q_proj", "v_proj")
+
+            value_q = checkpoint[key_q]
+            value_k = checkpoint[key_k]
+            value_v = checkpoint[key_v]
+            value = torch.cat([value_q, value_k, value_v])
+
+            new_key = key.replace(
+                "text_model.encoder.layers.", "transformer.resblocks."
+            )
+            new_key = new_key.replace(".self_attn.q_proj.", ".attn.in_proj_")
+            new_sd[new_key] = value
+
+    if logit_scale is not None:
+        new_sd["logit_scale"] = logit_scale
+
+    return new_sd
+
+
+def save_stable_diffusion_checkpoint(
+    output_file,
+    text_encoder1,
+    text_encoder2,
+    unet,
+    epochs,
+    steps,
+    ckpt_info,
+    vae,
+    logit_scale,
+    save_dtype=None,
+):
+    state_dict = {}
+
+    def update_sd(prefix, sd):
+        for k, v in sd.items():
+            key = prefix + k
+            if save_dtype is not None:
+                v = v.detach().clone().to("cpu").to(save_dtype)
+            state_dict[key] = v
+
+    # Convert the UNet model
+    update_sd("model.diffusion_model.", unet.state_dict())
+
+    # Convert the text encoders
+    update_sd("conditioner.embedders.0.transformer.", text_encoder1.state_dict())
+
+    text_enc2_dict = convert_text_encoder_2_state_dict_to_sdxl(
+        text_encoder2.state_dict(), logit_scale
+    )
+    update_sd("conditioner.embedders.1.model.", text_enc2_dict)
+
+    # Convert the VAE
+    vae_dict = model_util.convert_vae_state_dict(vae.state_dict())
+    update_sd("first_stage_model.", vae_dict)
+
+    # Put together new checkpoint
+    key_count = len(state_dict.keys())
+    new_ckpt = {"state_dict": state_dict}
+
+    # epoch and global_step are sometimes not int
+    if ckpt_info is not None:
+        epochs += ckpt_info[0]
+        steps += ckpt_info[1]
+
+    new_ckpt["epoch"] = epochs
+    new_ckpt["global_step"] = steps
+
+    if model_util.is_safetensors(output_file):
+        save_file(state_dict, output_file)
+    else:
+        torch.save(new_ckpt, output_file)
+
+    return key_count
+
+
+def save_diffusers_checkpoint(
+    output_dir,
+    text_encoder1,
+    text_encoder2,
+    unet,
+    pretrained_model_name_or_path,
+    vae=None,
+    use_safetensors=False,
+    save_dtype=None,
+):
+    from diffusers import StableDiffusionXLPipeline
+
+    # convert U-Net
+    unet_sd = unet.state_dict()
+    du_unet_sd = convert_sdxl_unet_state_dict_to_diffusers(unet_sd)
+
+    diffusers_unet = UNet2DConditionModel(**DIFFUSERS_SDXL_UNET_CONFIG)
+    if save_dtype is not None:
+        diffusers_unet.to(save_dtype)
+    diffusers_unet.load_state_dict(du_unet_sd)
+
+    # create pipeline to save
+    if pretrained_model_name_or_path is None:
+        pretrained_model_name_or_path = DIFFUSERS_REF_MODEL_ID_SDXL
+
+    scheduler = EulerDiscreteScheduler.from_pretrained(
+        pretrained_model_name_or_path, subfolder="scheduler"
+    )
+    tokenizer1 = CLIPTokenizer.from_pretrained(
+        pretrained_model_name_or_path, subfolder="tokenizer"
+    )
+    tokenizer2 = CLIPTokenizer.from_pretrained(
+        pretrained_model_name_or_path, subfolder="tokenizer_2"
+    )
+    if vae is None:
+        vae = AutoencoderKL.from_pretrained(
+            pretrained_model_name_or_path, subfolder="vae"
+        )
+
+    # prevent local path from being saved
+    def remove_name_or_path(model):
+        if hasattr(model, "config"):
+            model.config._name_or_path = None
+            model.config._name_or_path = None
+
+    remove_name_or_path(diffusers_unet)
+    remove_name_or_path(text_encoder1)
+    remove_name_or_path(text_encoder2)
+    remove_name_or_path(scheduler)
+    remove_name_or_path(tokenizer1)
+    remove_name_or_path(tokenizer2)
+    remove_name_or_path(vae)
+
+    pipeline = StableDiffusionXLPipeline(
+        unet=diffusers_unet,
+        text_encoder=text_encoder1,
+        text_encoder_2=text_encoder2,
+        vae=vae,
+        scheduler=scheduler,
+        tokenizer=tokenizer1,
+        tokenizer_2=tokenizer2,
+    )
+    if save_dtype is not None:
+        pipeline.to(None, save_dtype)
+    pipeline.save_pretrained(output_dir, safe_serialization=use_safetensors)
```

### Comparing `lycoris_lora-2.3.0.dev4/lycoris/kohya/sdxl_original_unet.py` & `lycoris_lora-2.3.0.dev5/lycoris/kohya/sdxl_original_unet.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,1243 +1,1243 @@
-# Diffusersのコードをベースとした sd_xl_baseのU-Net
-# state dictの形式をSDXLに合わせてある
-
-"""
-      target: sgm.modules.diffusionmodules.openaimodel.UNetModel
-      params:
-        adm_in_channels: 2816
-        num_classes: sequential
-        use_checkpoint: True
-        in_channels: 4
-        out_channels: 4
-        model_channels: 320
-        attention_resolutions: [4, 2]
-        num_res_blocks: 2
-        channel_mult: [1, 2, 4]
-        num_head_channels: 64
-        use_spatial_transformer: True
-        use_linear_in_transformer: True
-        transformer_depth: [1, 2, 10]  # note: the first is unused (due to attn_res starting at 2) 32, 16, 8 --> 64, 32, 16
-        context_dim: 2048
-        spatial_transformer_attn_type: softmax-xformers
-        legacy: False
-"""
-
-import math
-from types import SimpleNamespace
-from typing import Optional
-import torch
-import torch.utils.checkpoint
-from torch import nn
-from torch.nn import functional as F
-from einops import rearrange
-
-
-IN_CHANNELS: int = 4
-OUT_CHANNELS: int = 4
-ADM_IN_CHANNELS: int = 2816
-CONTEXT_DIM: int = 2048
-MODEL_CHANNELS: int = 320
-TIME_EMBED_DIM = 320 * 4
-
-
-# region memory effcient attention
-
-# FlashAttentionを使うCrossAttention
-# based on https://github.com/lucidrains/memory-efficient-attention-pytorch/blob/main/memory_efficient_attention_pytorch/flash_attention.py
-# LICENSE MIT https://github.com/lucidrains/memory-efficient-attention-pytorch/blob/main/LICENSE
-
-# constants
-
-EPSILON = 1e-6
-
-# helper functions
-
-
-def exists(val):
-    return val is not None
-
-
-def default(val, d):
-    return val if exists(val) else d
-
-
-# flash attention forwards and backwards
-
-# https://arxiv.org/abs/2205.14135
-
-
-class FlashAttentionFunction(torch.autograd.Function):
-    @staticmethod
-    @torch.no_grad()
-    def forward(ctx, q, k, v, mask, causal, q_bucket_size, k_bucket_size):
-        """Algorithm 2 in the paper"""
-
-        device = q.device
-        dtype = q.dtype
-        max_neg_value = -torch.finfo(q.dtype).max
-        qk_len_diff = max(k.shape[-2] - q.shape[-2], 0)
-
-        o = torch.zeros_like(q)
-        all_row_sums = torch.zeros((*q.shape[:-1], 1), dtype=dtype, device=device)
-        all_row_maxes = torch.full(
-            (*q.shape[:-1], 1), max_neg_value, dtype=dtype, device=device
-        )
-
-        scale = q.shape[-1] ** -0.5
-
-        if not exists(mask):
-            mask = (None,) * math.ceil(q.shape[-2] / q_bucket_size)
-        else:
-            mask = rearrange(mask, "b n -> b 1 1 n")
-            mask = mask.split(q_bucket_size, dim=-1)
-
-        row_splits = zip(
-            q.split(q_bucket_size, dim=-2),
-            o.split(q_bucket_size, dim=-2),
-            mask,
-            all_row_sums.split(q_bucket_size, dim=-2),
-            all_row_maxes.split(q_bucket_size, dim=-2),
-        )
-
-        for ind, (qc, oc, row_mask, row_sums, row_maxes) in enumerate(row_splits):
-            q_start_index = ind * q_bucket_size - qk_len_diff
-
-            col_splits = zip(
-                k.split(k_bucket_size, dim=-2),
-                v.split(k_bucket_size, dim=-2),
-            )
-
-            for k_ind, (kc, vc) in enumerate(col_splits):
-                k_start_index = k_ind * k_bucket_size
-
-                attn_weights = (
-                    torch.einsum("... i d, ... j d -> ... i j", qc, kc) * scale
-                )
-
-                if exists(row_mask):
-                    attn_weights.masked_fill_(~row_mask, max_neg_value)
-
-                if causal and q_start_index < (k_start_index + k_bucket_size - 1):
-                    causal_mask = torch.ones(
-                        (qc.shape[-2], kc.shape[-2]), dtype=torch.bool, device=device
-                    ).triu(q_start_index - k_start_index + 1)
-                    attn_weights.masked_fill_(causal_mask, max_neg_value)
-
-                block_row_maxes = attn_weights.amax(dim=-1, keepdims=True)
-                attn_weights -= block_row_maxes
-                exp_weights = torch.exp(attn_weights)
-
-                if exists(row_mask):
-                    exp_weights.masked_fill_(~row_mask, 0.0)
-
-                block_row_sums = exp_weights.sum(dim=-1, keepdims=True).clamp(
-                    min=EPSILON
-                )
-
-                new_row_maxes = torch.maximum(block_row_maxes, row_maxes)
-
-                exp_values = torch.einsum(
-                    "... i j, ... j d -> ... i d", exp_weights, vc
-                )
-
-                exp_row_max_diff = torch.exp(row_maxes - new_row_maxes)
-                exp_block_row_max_diff = torch.exp(block_row_maxes - new_row_maxes)
-
-                new_row_sums = (
-                    exp_row_max_diff * row_sums
-                    + exp_block_row_max_diff * block_row_sums
-                )
-
-                oc.mul_((row_sums / new_row_sums) * exp_row_max_diff).add_(
-                    (exp_block_row_max_diff / new_row_sums) * exp_values
-                )
-
-                row_maxes.copy_(new_row_maxes)
-                row_sums.copy_(new_row_sums)
-
-        ctx.args = (causal, scale, mask, q_bucket_size, k_bucket_size)
-        ctx.save_for_backward(q, k, v, o, all_row_sums, all_row_maxes)
-
-        return o
-
-    @staticmethod
-    @torch.no_grad()
-    def backward(ctx, do):
-        """Algorithm 4 in the paper"""
-
-        causal, scale, mask, q_bucket_size, k_bucket_size = ctx.args
-        q, k, v, o, l, m = ctx.saved_tensors
-
-        device = q.device
-
-        max_neg_value = -torch.finfo(q.dtype).max
-        qk_len_diff = max(k.shape[-2] - q.shape[-2], 0)
-
-        dq = torch.zeros_like(q)
-        dk = torch.zeros_like(k)
-        dv = torch.zeros_like(v)
-
-        row_splits = zip(
-            q.split(q_bucket_size, dim=-2),
-            o.split(q_bucket_size, dim=-2),
-            do.split(q_bucket_size, dim=-2),
-            mask,
-            l.split(q_bucket_size, dim=-2),
-            m.split(q_bucket_size, dim=-2),
-            dq.split(q_bucket_size, dim=-2),
-        )
-
-        for ind, (qc, oc, doc, row_mask, lc, mc, dqc) in enumerate(row_splits):
-            q_start_index = ind * q_bucket_size - qk_len_diff
-
-            col_splits = zip(
-                k.split(k_bucket_size, dim=-2),
-                v.split(k_bucket_size, dim=-2),
-                dk.split(k_bucket_size, dim=-2),
-                dv.split(k_bucket_size, dim=-2),
-            )
-
-            for k_ind, (kc, vc, dkc, dvc) in enumerate(col_splits):
-                k_start_index = k_ind * k_bucket_size
-
-                attn_weights = (
-                    torch.einsum("... i d, ... j d -> ... i j", qc, kc) * scale
-                )
-
-                if causal and q_start_index < (k_start_index + k_bucket_size - 1):
-                    causal_mask = torch.ones(
-                        (qc.shape[-2], kc.shape[-2]), dtype=torch.bool, device=device
-                    ).triu(q_start_index - k_start_index + 1)
-                    attn_weights.masked_fill_(causal_mask, max_neg_value)
-
-                exp_attn_weights = torch.exp(attn_weights - mc)
-
-                if exists(row_mask):
-                    exp_attn_weights.masked_fill_(~row_mask, 0.0)
-
-                p = exp_attn_weights / lc
-
-                dv_chunk = torch.einsum("... i j, ... i d -> ... j d", p, doc)
-                dp = torch.einsum("... i d, ... j d -> ... i j", doc, vc)
-
-                D = (doc * oc).sum(dim=-1, keepdims=True)
-                ds = p * scale * (dp - D)
-
-                dq_chunk = torch.einsum("... i j, ... j d -> ... i d", ds, kc)
-                dk_chunk = torch.einsum("... i j, ... i d -> ... j d", ds, qc)
-
-                dqc.add_(dq_chunk)
-                dkc.add_(dk_chunk)
-                dvc.add_(dv_chunk)
-
-        return dq, dk, dv, None, None, None, None
-
-
-# endregion
-
-
-def get_parameter_dtype(parameter: torch.nn.Module):
-    return next(parameter.parameters()).dtype
-
-
-def get_parameter_device(parameter: torch.nn.Module):
-    return next(parameter.parameters()).device
-
-
-def get_timestep_embedding(
-    timesteps: torch.Tensor,
-    embedding_dim: int,
-    downscale_freq_shift: float = 1,
-    scale: float = 1,
-    max_period: int = 10000,
-):
-    """
-    This matches the implementation in Denoising Diffusion Probabilistic Models: Create sinusoidal timestep embeddings.
-
-    :param timesteps: a 1-D Tensor of N indices, one per batch element.
-                      These may be fractional.
-    :param embedding_dim: the dimension of the output. :param max_period: controls the minimum frequency of the
-    embeddings. :return: an [N x dim] Tensor of positional embeddings.
-    """
-    assert len(timesteps.shape) == 1, "Timesteps should be a 1d-array"
-
-    half_dim = embedding_dim // 2
-    exponent = -math.log(max_period) * torch.arange(
-        start=0, end=half_dim, dtype=torch.float32, device=timesteps.device
-    )
-    exponent = exponent / (half_dim - downscale_freq_shift)
-
-    emb = torch.exp(exponent)
-    emb = timesteps[:, None].float() * emb[None, :]
-
-    # scale embeddings
-    emb = scale * emb
-
-    # concat sine and cosine embeddings: flipped from Diffusers original ver because always flip_sin_to_cos=True
-    emb = torch.cat([torch.cos(emb), torch.sin(emb)], dim=-1)
-
-    # zero pad
-    if embedding_dim % 2 == 1:
-        emb = torch.nn.functional.pad(emb, (0, 1, 0, 0))
-    return emb
-
-
-class GroupNorm32(nn.GroupNorm):
-    def forward(self, x):
-        if self.weight.dtype != torch.float32:
-            return super().forward(x)
-        return super().forward(x.float()).type(x.dtype)
-
-
-class ResnetBlock2D(nn.Module):
-    def __init__(
-        self,
-        in_channels,
-        out_channels,
-    ):
-        super().__init__()
-        self.in_channels = in_channels
-        self.out_channels = out_channels
-
-        self.in_layers = nn.Sequential(
-            GroupNorm32(32, in_channels),
-            nn.SiLU(),
-            nn.Conv2d(in_channels, out_channels, kernel_size=3, stride=1, padding=1),
-        )
-
-        self.emb_layers = nn.Sequential(
-            nn.SiLU(), nn.Linear(TIME_EMBED_DIM, out_channels)
-        )
-
-        self.out_layers = nn.Sequential(
-            GroupNorm32(32, out_channels),
-            nn.SiLU(),
-            nn.Identity(),  # to make state_dict compatible with original model
-            nn.Conv2d(out_channels, out_channels, kernel_size=3, stride=1, padding=1),
-        )
-
-        if in_channels != out_channels:
-            self.skip_connection = nn.Conv2d(
-                in_channels, out_channels, kernel_size=1, stride=1, padding=0
-            )
-        else:
-            self.skip_connection = nn.Identity()
-
-        self.gradient_checkpointing = False
-
-    def forward_body(self, x, emb):
-        h = self.in_layers(x)
-        emb_out = self.emb_layers(emb).type(h.dtype)
-        h = h + emb_out[:, :, None, None]
-        h = self.out_layers(h)
-        x = self.skip_connection(x)
-        return x + h
-
-    def forward(self, x, emb):
-        if self.training and self.gradient_checkpointing:
-            # print("ResnetBlock2D: gradient_checkpointing")
-
-            def create_custom_forward(func):
-                def custom_forward(*inputs):
-                    return func(*inputs)
-
-                return custom_forward
-
-            x = torch.utils.checkpoint.checkpoint(
-                create_custom_forward(self.forward_body), x, emb
-            )
-        else:
-            x = self.forward_body(x, emb)
-
-        return x
-
-
-class Downsample2D(nn.Module):
-    def __init__(self, channels, out_channels):
-        super().__init__()
-
-        self.channels = channels
-        self.out_channels = out_channels
-
-        self.op = nn.Conv2d(self.channels, self.out_channels, 3, stride=2, padding=1)
-
-        self.gradient_checkpointing = False
-
-    def forward_body(self, hidden_states):
-        assert hidden_states.shape[1] == self.channels
-        hidden_states = self.op(hidden_states)
-
-        return hidden_states
-
-    def forward(self, hidden_states):
-        if self.training and self.gradient_checkpointing:
-            # print("Downsample2D: gradient_checkpointing")
-
-            def create_custom_forward(func):
-                def custom_forward(*inputs):
-                    return func(*inputs)
-
-                return custom_forward
-
-            hidden_states = torch.utils.checkpoint.checkpoint(
-                create_custom_forward(self.forward_body), hidden_states
-            )
-        else:
-            hidden_states = self.forward_body(hidden_states)
-
-        return hidden_states
-
-
-class CrossAttention(nn.Module):
-    def __init__(
-        self,
-        query_dim: int,
-        cross_attention_dim: Optional[int] = None,
-        heads: int = 8,
-        dim_head: int = 64,
-        upcast_attention: bool = False,
-    ):
-        super().__init__()
-        inner_dim = dim_head * heads
-        cross_attention_dim = (
-            cross_attention_dim if cross_attention_dim is not None else query_dim
-        )
-        self.upcast_attention = upcast_attention
-
-        self.scale = dim_head**-0.5
-        self.heads = heads
-
-        self.to_q = nn.Linear(query_dim, inner_dim, bias=False)
-        self.to_k = nn.Linear(cross_attention_dim, inner_dim, bias=False)
-        self.to_v = nn.Linear(cross_attention_dim, inner_dim, bias=False)
-
-        self.to_out = nn.ModuleList([])
-        self.to_out.append(nn.Linear(inner_dim, query_dim))
-        # no dropout here
-
-        self.use_memory_efficient_attention_xformers = False
-        self.use_memory_efficient_attention_mem_eff = False
-        self.use_sdpa = False
-
-    def set_use_memory_efficient_attention(self, xformers, mem_eff):
-        self.use_memory_efficient_attention_xformers = xformers
-        self.use_memory_efficient_attention_mem_eff = mem_eff
-
-    def set_use_sdpa(self, sdpa):
-        self.use_sdpa = sdpa
-
-    def reshape_heads_to_batch_dim(self, tensor):
-        batch_size, seq_len, dim = tensor.shape
-        head_size = self.heads
-        tensor = tensor.reshape(batch_size, seq_len, head_size, dim // head_size)
-        tensor = tensor.permute(0, 2, 1, 3).reshape(
-            batch_size * head_size, seq_len, dim // head_size
-        )
-        return tensor
-
-    def reshape_batch_dim_to_heads(self, tensor):
-        batch_size, seq_len, dim = tensor.shape
-        head_size = self.heads
-        tensor = tensor.reshape(batch_size // head_size, head_size, seq_len, dim)
-        tensor = tensor.permute(0, 2, 1, 3).reshape(
-            batch_size // head_size, seq_len, dim * head_size
-        )
-        return tensor
-
-    def forward(self, hidden_states, context=None, mask=None):
-        if self.use_memory_efficient_attention_xformers:
-            return self.forward_memory_efficient_xformers(hidden_states, context, mask)
-        if self.use_memory_efficient_attention_mem_eff:
-            return self.forward_memory_efficient_mem_eff(hidden_states, context, mask)
-        if self.use_sdpa:
-            return self.forward_sdpa(hidden_states, context, mask)
-
-        query = self.to_q(hidden_states)
-        context = context if context is not None else hidden_states
-        key = self.to_k(context)
-        value = self.to_v(context)
-
-        query = self.reshape_heads_to_batch_dim(query)
-        key = self.reshape_heads_to_batch_dim(key)
-        value = self.reshape_heads_to_batch_dim(value)
-
-        hidden_states = self._attention(query, key, value)
-
-        # linear proj
-        hidden_states = self.to_out[0](hidden_states)
-        # hidden_states = self.to_out[1](hidden_states)     # no dropout
-        return hidden_states
-
-    def _attention(self, query, key, value):
-        if self.upcast_attention:
-            query = query.float()
-            key = key.float()
-
-        attention_scores = torch.baddbmm(
-            torch.empty(
-                query.shape[0],
-                query.shape[1],
-                key.shape[1],
-                dtype=query.dtype,
-                device=query.device,
-            ),
-            query,
-            key.transpose(-1, -2),
-            beta=0,
-            alpha=self.scale,
-        )
-        attention_probs = attention_scores.softmax(dim=-1)
-
-        # cast back to the original dtype
-        attention_probs = attention_probs.to(value.dtype)
-
-        # compute attention output
-        hidden_states = torch.bmm(attention_probs, value)
-
-        # reshape hidden_states
-        hidden_states = self.reshape_batch_dim_to_heads(hidden_states)
-        return hidden_states
-
-    # TODO support Hypernetworks
-    def forward_memory_efficient_xformers(self, x, context=None, mask=None):
-        import xformers.ops
-
-        h = self.heads
-        q_in = self.to_q(x)
-        context = context if context is not None else x
-        context = context.to(x.dtype)
-        k_in = self.to_k(context)
-        v_in = self.to_v(context)
-
-        q, k, v = map(
-            lambda t: rearrange(t, "b n (h d) -> b n h d", h=h), (q_in, k_in, v_in)
-        )
-        del q_in, k_in, v_in
-
-        q = q.contiguous()
-        k = k.contiguous()
-        v = v.contiguous()
-        out = xformers.ops.memory_efficient_attention(
-            q, k, v, attn_bias=None
-        )  # 最適なのを選んでくれる
-        del q, k, v
-
-        out = rearrange(out, "b n h d -> b n (h d)", h=h)
-
-        out = self.to_out[0](out)
-        return out
-
-    def forward_memory_efficient_mem_eff(self, x, context=None, mask=None):
-        flash_func = FlashAttentionFunction
-
-        q_bucket_size = 512
-        k_bucket_size = 1024
-
-        h = self.heads
-        q = self.to_q(x)
-        context = context if context is not None else x
-        context = context.to(x.dtype)
-        k = self.to_k(context)
-        v = self.to_v(context)
-        del context, x
-
-        q, k, v = map(lambda t: rearrange(t, "b n (h d) -> b h n d", h=h), (q, k, v))
-
-        out = flash_func.apply(q, k, v, mask, False, q_bucket_size, k_bucket_size)
-
-        out = rearrange(out, "b h n d -> b n (h d)")
-
-        out = self.to_out[0](out)
-        return out
-
-    def forward_sdpa(self, x, context=None, mask=None):
-        h = self.heads
-        q_in = self.to_q(x)
-        context = context if context is not None else x
-        context = context.to(x.dtype)
-        k_in = self.to_k(context)
-        v_in = self.to_v(context)
-
-        q, k, v = map(
-            lambda t: rearrange(t, "b n (h d) -> b h n d", h=h), (q_in, k_in, v_in)
-        )
-        del q_in, k_in, v_in
-
-        out = F.scaled_dot_product_attention(
-            q, k, v, attn_mask=mask, dropout_p=0.0, is_causal=False
-        )
-
-        out = rearrange(out, "b h n d -> b n (h d)", h=h)
-
-        out = self.to_out[0](out)
-        return out
-
-
-# feedforward
-class GEGLU(nn.Module):
-    r"""
-    A variant of the gated linear unit activation function from https://arxiv.org/abs/2002.05202.
-
-    Parameters:
-        dim_in (`int`): The number of channels in the input.
-        dim_out (`int`): The number of channels in the output.
-    """
-
-    def __init__(self, dim_in: int, dim_out: int):
-        super().__init__()
-        self.proj = nn.Linear(dim_in, dim_out * 2)
-
-    def gelu(self, gate):
-        if gate.device.type != "mps":
-            return F.gelu(gate)
-        # mps: gelu is not implemented for float16
-        return F.gelu(gate.to(dtype=torch.float32)).to(dtype=gate.dtype)
-
-    def forward(self, hidden_states):
-        hidden_states, gate = self.proj(hidden_states).chunk(2, dim=-1)
-        return hidden_states * self.gelu(gate)
-
-
-class FeedForward(nn.Module):
-    def __init__(
-        self,
-        dim: int,
-    ):
-        super().__init__()
-        inner_dim = int(dim * 4)  # mult is always 4
-
-        self.net = nn.ModuleList([])
-        # project in
-        self.net.append(GEGLU(dim, inner_dim))
-        # project dropout
-        self.net.append(nn.Identity())  # nn.Dropout(0)) # dummy for dropout with 0
-        # project out
-        self.net.append(nn.Linear(inner_dim, dim))
-
-    def forward(self, hidden_states):
-        for module in self.net:
-            hidden_states = module(hidden_states)
-        return hidden_states
-
-
-class BasicTransformerBlock(nn.Module):
-    def __init__(
-        self,
-        dim: int,
-        num_attention_heads: int,
-        attention_head_dim: int,
-        cross_attention_dim: int,
-        upcast_attention: bool = False,
-    ):
-        super().__init__()
-
-        self.gradient_checkpointing = False
-
-        # 1. Self-Attn
-        self.attn1 = CrossAttention(
-            query_dim=dim,
-            cross_attention_dim=None,
-            heads=num_attention_heads,
-            dim_head=attention_head_dim,
-            upcast_attention=upcast_attention,
-        )
-        self.ff = FeedForward(dim)
-
-        # 2. Cross-Attn
-        self.attn2 = CrossAttention(
-            query_dim=dim,
-            cross_attention_dim=cross_attention_dim,
-            heads=num_attention_heads,
-            dim_head=attention_head_dim,
-            upcast_attention=upcast_attention,
-        )
-
-        self.norm1 = nn.LayerNorm(dim)
-        self.norm2 = nn.LayerNorm(dim)
-
-        # 3. Feed-forward
-        self.norm3 = nn.LayerNorm(dim)
-
-    def set_use_memory_efficient_attention(self, xformers: bool, mem_eff: bool):
-        self.attn1.set_use_memory_efficient_attention(xformers, mem_eff)
-        self.attn2.set_use_memory_efficient_attention(xformers, mem_eff)
-
-    def set_use_sdpa(self, sdpa: bool):
-        self.attn1.set_use_sdpa(sdpa)
-        self.attn2.set_use_sdpa(sdpa)
-
-    def forward_body(self, hidden_states, context=None, timestep=None):
-        # 1. Self-Attention
-        norm_hidden_states = self.norm1(hidden_states)
-
-        hidden_states = self.attn1(norm_hidden_states) + hidden_states
-
-        # 2. Cross-Attention
-        norm_hidden_states = self.norm2(hidden_states)
-        hidden_states = self.attn2(norm_hidden_states, context=context) + hidden_states
-
-        # 3. Feed-forward
-        hidden_states = self.ff(self.norm3(hidden_states)) + hidden_states
-
-        return hidden_states
-
-    def forward(self, hidden_states, context=None, timestep=None):
-        if self.training and self.gradient_checkpointing:
-            # print("BasicTransformerBlock: checkpointing")
-
-            def create_custom_forward(func):
-                def custom_forward(*inputs):
-                    return func(*inputs)
-
-                return custom_forward
-
-            output = torch.utils.checkpoint.checkpoint(
-                create_custom_forward(self.forward_body),
-                hidden_states,
-                context,
-                timestep,
-            )
-        else:
-            output = self.forward_body(hidden_states, context, timestep)
-
-        return output
-
-
-class Transformer2DModel(nn.Module):
-    def __init__(
-        self,
-        num_attention_heads: int = 16,
-        attention_head_dim: int = 88,
-        in_channels: Optional[int] = None,
-        cross_attention_dim: Optional[int] = None,
-        use_linear_projection: bool = False,
-        upcast_attention: bool = False,
-        num_transformer_layers: int = 1,
-    ):
-        super().__init__()
-        self.in_channels = in_channels
-        self.num_attention_heads = num_attention_heads
-        self.attention_head_dim = attention_head_dim
-        inner_dim = num_attention_heads * attention_head_dim
-        self.use_linear_projection = use_linear_projection
-
-        self.norm = torch.nn.GroupNorm(
-            num_groups=32, num_channels=in_channels, eps=1e-6, affine=True
-        )
-        # self.norm = GroupNorm32(32, in_channels, eps=1e-6, affine=True)
-
-        if use_linear_projection:
-            self.proj_in = nn.Linear(in_channels, inner_dim)
-        else:
-            self.proj_in = nn.Conv2d(
-                in_channels, inner_dim, kernel_size=1, stride=1, padding=0
-            )
-
-        blocks = []
-        for _ in range(num_transformer_layers):
-            blocks.append(
-                BasicTransformerBlock(
-                    inner_dim,
-                    num_attention_heads,
-                    attention_head_dim,
-                    cross_attention_dim=cross_attention_dim,
-                    upcast_attention=upcast_attention,
-                )
-            )
-
-        self.transformer_blocks = nn.ModuleList(blocks)
-
-        if use_linear_projection:
-            self.proj_out = nn.Linear(in_channels, inner_dim)
-        else:
-            self.proj_out = nn.Conv2d(
-                inner_dim, in_channels, kernel_size=1, stride=1, padding=0
-            )
-
-        self.gradient_checkpointing = False
-
-    def set_use_memory_efficient_attention(self, xformers, mem_eff):
-        for transformer in self.transformer_blocks:
-            transformer.set_use_memory_efficient_attention(xformers, mem_eff)
-
-    def set_use_sdpa(self, sdpa):
-        for transformer in self.transformer_blocks:
-            transformer.set_use_sdpa(sdpa)
-
-    def forward(self, hidden_states, encoder_hidden_states=None, timestep=None):
-        # 1. Input
-        batch, _, height, weight = hidden_states.shape
-        residual = hidden_states
-
-        hidden_states = self.norm(hidden_states)
-        if not self.use_linear_projection:
-            hidden_states = self.proj_in(hidden_states)
-            inner_dim = hidden_states.shape[1]
-            hidden_states = hidden_states.permute(0, 2, 3, 1).reshape(
-                batch, height * weight, inner_dim
-            )
-        else:
-            inner_dim = hidden_states.shape[1]
-            hidden_states = hidden_states.permute(0, 2, 3, 1).reshape(
-                batch, height * weight, inner_dim
-            )
-            hidden_states = self.proj_in(hidden_states)
-
-        # 2. Blocks
-        for block in self.transformer_blocks:
-            hidden_states = block(
-                hidden_states, context=encoder_hidden_states, timestep=timestep
-            )
-
-        # 3. Output
-        if not self.use_linear_projection:
-            hidden_states = (
-                hidden_states.reshape(batch, height, weight, inner_dim)
-                .permute(0, 3, 1, 2)
-                .contiguous()
-            )
-            hidden_states = self.proj_out(hidden_states)
-        else:
-            hidden_states = self.proj_out(hidden_states)
-            hidden_states = (
-                hidden_states.reshape(batch, height, weight, inner_dim)
-                .permute(0, 3, 1, 2)
-                .contiguous()
-            )
-
-        output = hidden_states + residual
-
-        return output
-
-
-class Upsample2D(nn.Module):
-    def __init__(self, channels, out_channels):
-        super().__init__()
-        self.channels = channels
-        self.out_channels = out_channels
-        self.conv = nn.Conv2d(self.channels, self.out_channels, 3, padding=1)
-
-        self.gradient_checkpointing = False
-
-    def forward_body(self, hidden_states, output_size=None):
-        assert hidden_states.shape[1] == self.channels
-
-        # Cast to float32 to as 'upsample_nearest2d_out_frame' op does not support bfloat16
-        # TODO(Suraj): Remove this cast once the issue is fixed in PyTorch
-        # https://github.com/pytorch/pytorch/issues/86679
-        dtype = hidden_states.dtype
-        if dtype == torch.bfloat16:
-            hidden_states = hidden_states.to(torch.float32)
-
-        # upsample_nearest_nhwc fails with large batch sizes. see https://github.com/huggingface/diffusers/issues/984
-        if hidden_states.shape[0] >= 64:
-            hidden_states = hidden_states.contiguous()
-
-        # if `output_size` is passed we force the interpolation output size and do not make use of `scale_factor=2`
-        if output_size is None:
-            hidden_states = F.interpolate(
-                hidden_states, scale_factor=2.0, mode="nearest"
-            )
-        else:
-            hidden_states = F.interpolate(
-                hidden_states, size=output_size, mode="nearest"
-            )
-
-        # If the input is bfloat16, we cast back to bfloat16
-        if dtype == torch.bfloat16:
-            hidden_states = hidden_states.to(dtype)
-
-        hidden_states = self.conv(hidden_states)
-
-        return hidden_states
-
-    def forward(self, hidden_states, output_size=None):
-        if self.training and self.gradient_checkpointing:
-            # print("Upsample2D: gradient_checkpointing")
-
-            def create_custom_forward(func):
-                def custom_forward(*inputs):
-                    return func(*inputs)
-
-                return custom_forward
-
-            hidden_states = torch.utils.checkpoint.checkpoint(
-                create_custom_forward(self.forward_body), hidden_states, output_size
-            )
-        else:
-            hidden_states = self.forward_body(hidden_states, output_size)
-
-        return hidden_states
-
-
-class SdxlUNet2DConditionModel(nn.Module):
-    _supports_gradient_checkpointing = True
-
-    def __init__(
-        self,
-        **kwargs,
-    ):
-        super().__init__()
-
-        self.in_channels = IN_CHANNELS
-        self.out_channels = OUT_CHANNELS
-        self.model_channels = MODEL_CHANNELS
-        self.time_embed_dim = TIME_EMBED_DIM
-        self.adm_in_channels = ADM_IN_CHANNELS
-
-        self.gradient_checkpointing = False
-        # self.sample_size = sample_size
-
-        # time embedding
-        self.time_embed = nn.Sequential(
-            nn.Linear(self.model_channels, self.time_embed_dim),
-            nn.SiLU(),
-            nn.Linear(self.time_embed_dim, self.time_embed_dim),
-        )
-
-        # label embedding
-        self.label_emb = nn.Sequential(
-            nn.Sequential(
-                nn.Linear(self.adm_in_channels, self.time_embed_dim),
-                nn.SiLU(),
-                nn.Linear(self.time_embed_dim, self.time_embed_dim),
-            )
-        )
-
-        # input
-        self.input_blocks = nn.ModuleList(
-            [
-                nn.Sequential(
-                    nn.Conv2d(
-                        self.in_channels,
-                        self.model_channels,
-                        kernel_size=3,
-                        padding=(1, 1),
-                    ),
-                )
-            ]
-        )
-
-        # level 0
-        for i in range(2):
-            layers = [
-                ResnetBlock2D(
-                    in_channels=1 * self.model_channels,
-                    out_channels=1 * self.model_channels,
-                ),
-            ]
-            self.input_blocks.append(nn.ModuleList(layers))
-
-        self.input_blocks.append(
-            nn.Sequential(
-                Downsample2D(
-                    channels=1 * self.model_channels,
-                    out_channels=1 * self.model_channels,
-                ),
-            )
-        )
-
-        # level 1
-        for i in range(2):
-            layers = [
-                ResnetBlock2D(
-                    in_channels=(1 if i == 0 else 2) * self.model_channels,
-                    out_channels=2 * self.model_channels,
-                ),
-                Transformer2DModel(
-                    num_attention_heads=2 * self.model_channels // 64,
-                    attention_head_dim=64,
-                    in_channels=2 * self.model_channels,
-                    num_transformer_layers=2,
-                    use_linear_projection=True,
-                    cross_attention_dim=2048,
-                ),
-            ]
-            self.input_blocks.append(nn.ModuleList(layers))
-
-        self.input_blocks.append(
-            nn.Sequential(
-                Downsample2D(
-                    channels=2 * self.model_channels,
-                    out_channels=2 * self.model_channels,
-                ),
-            )
-        )
-
-        # level 2
-        for i in range(2):
-            layers = [
-                ResnetBlock2D(
-                    in_channels=(2 if i == 0 else 4) * self.model_channels,
-                    out_channels=4 * self.model_channels,
-                ),
-                Transformer2DModel(
-                    num_attention_heads=4 * self.model_channels // 64,
-                    attention_head_dim=64,
-                    in_channels=4 * self.model_channels,
-                    num_transformer_layers=10,
-                    use_linear_projection=True,
-                    cross_attention_dim=2048,
-                ),
-            ]
-            self.input_blocks.append(nn.ModuleList(layers))
-
-        # mid
-        self.middle_block = nn.ModuleList(
-            [
-                ResnetBlock2D(
-                    in_channels=4 * self.model_channels,
-                    out_channels=4 * self.model_channels,
-                ),
-                Transformer2DModel(
-                    num_attention_heads=4 * self.model_channels // 64,
-                    attention_head_dim=64,
-                    in_channels=4 * self.model_channels,
-                    num_transformer_layers=10,
-                    use_linear_projection=True,
-                    cross_attention_dim=2048,
-                ),
-                ResnetBlock2D(
-                    in_channels=4 * self.model_channels,
-                    out_channels=4 * self.model_channels,
-                ),
-            ]
-        )
-
-        # output
-        self.output_blocks = nn.ModuleList([])
-
-        # level 2
-        for i in range(3):
-            layers = [
-                ResnetBlock2D(
-                    in_channels=4 * self.model_channels
-                    + (4 if i <= 1 else 2) * self.model_channels,
-                    out_channels=4 * self.model_channels,
-                ),
-                Transformer2DModel(
-                    num_attention_heads=4 * self.model_channels // 64,
-                    attention_head_dim=64,
-                    in_channels=4 * self.model_channels,
-                    num_transformer_layers=10,
-                    use_linear_projection=True,
-                    cross_attention_dim=2048,
-                ),
-            ]
-            if i == 2:
-                layers.append(
-                    Upsample2D(
-                        channels=4 * self.model_channels,
-                        out_channels=4 * self.model_channels,
-                    )
-                )
-
-            self.output_blocks.append(nn.ModuleList(layers))
-
-        # level 1
-        for i in range(3):
-            layers = [
-                ResnetBlock2D(
-                    in_channels=2 * self.model_channels
-                    + (4 if i == 0 else (2 if i == 1 else 1)) * self.model_channels,
-                    out_channels=2 * self.model_channels,
-                ),
-                Transformer2DModel(
-                    num_attention_heads=2 * self.model_channels // 64,
-                    attention_head_dim=64,
-                    in_channels=2 * self.model_channels,
-                    num_transformer_layers=2,
-                    use_linear_projection=True,
-                    cross_attention_dim=2048,
-                ),
-            ]
-            if i == 2:
-                layers.append(
-                    Upsample2D(
-                        channels=2 * self.model_channels,
-                        out_channels=2 * self.model_channels,
-                    )
-                )
-
-            self.output_blocks.append(nn.ModuleList(layers))
-
-        # level 0
-        for i in range(3):
-            layers = [
-                ResnetBlock2D(
-                    in_channels=1 * self.model_channels
-                    + (2 if i == 0 else 1) * self.model_channels,
-                    out_channels=1 * self.model_channels,
-                ),
-            ]
-
-            self.output_blocks.append(nn.ModuleList(layers))
-
-        # output
-        self.out = nn.ModuleList(
-            [
-                GroupNorm32(32, self.model_channels),
-                nn.SiLU(),
-                nn.Conv2d(self.model_channels, self.out_channels, 3, padding=1),
-            ]
-        )
-
-    # region diffusers compatibility
-    def prepare_config(self):
-        self.config = SimpleNamespace()
-
-    @property
-    def dtype(self) -> torch.dtype:
-        # `torch.dtype`: The dtype of the module (assuming that all the module parameters have the same dtype).
-        return get_parameter_dtype(self)
-
-    @property
-    def device(self) -> torch.device:
-        # `torch.device`: The device on which the module is (assuming that all the module parameters are on the same device).
-        return get_parameter_device(self)
-
-    def set_attention_slice(self, slice_size):
-        raise NotImplementedError("Attention slicing is not supported for this model.")
-
-    def is_gradient_checkpointing(self) -> bool:
-        return any(
-            hasattr(m, "gradient_checkpointing") and m.gradient_checkpointing
-            for m in self.modules()
-        )
-
-    def enable_gradient_checkpointing(self):
-        self.gradient_checkpointing = True
-        self.set_gradient_checkpointing(value=True)
-
-    def disable_gradient_checkpointing(self):
-        self.gradient_checkpointing = False
-        self.set_gradient_checkpointing(value=False)
-
-    def set_use_memory_efficient_attention(self, xformers: bool, mem_eff: bool) -> None:
-        blocks = self.input_blocks + [self.middle_block] + self.output_blocks
-        for block in blocks:
-            for module in block:
-                if hasattr(module, "set_use_memory_efficient_attention"):
-                    # print(module.__class__.__name__)
-                    module.set_use_memory_efficient_attention(xformers, mem_eff)
-
-    def set_use_sdpa(self, sdpa: bool) -> None:
-        blocks = self.input_blocks + [self.middle_block] + self.output_blocks
-        for block in blocks:
-            for module in block:
-                if hasattr(module, "set_use_sdpa"):
-                    module.set_use_sdpa(sdpa)
-
-    def set_gradient_checkpointing(self, value=False):
-        blocks = self.input_blocks + [self.middle_block] + self.output_blocks
-        for block in blocks:
-            for module in block.modules():
-                if hasattr(module, "gradient_checkpointing"):
-                    # print(module.__class__.__name__, module.gradient_checkpointing, "->", value)
-                    module.gradient_checkpointing = value
-
-    # endregion
-
-    def forward(self, x, timesteps=None, context=None, y=None, **kwargs):
-        # broadcast timesteps to batch dimension
-        timesteps = timesteps.expand(x.shape[0])
-
-        hs = []
-        t_emb = get_timestep_embedding(
-            timesteps, self.model_channels
-        )  # , repeat_only=False)
-        t_emb = t_emb.to(x.dtype)
-        emb = self.time_embed(t_emb)
-
-        assert (
-            x.shape[0] == y.shape[0]
-        ), f"batch size mismatch: {x.shape[0]} != {y.shape[0]}"
-        assert x.dtype == y.dtype, f"dtype mismatch: {x.dtype} != {y.dtype}"
-        # assert x.dtype == self.dtype
-        emb = emb + self.label_emb(y)
-
-        def call_module(module, h, emb, context):
-            x = h
-            for layer in module:
-                # print(layer.__class__.__name__, x.dtype, emb.dtype, context.dtype if context is not None else None)
-                if isinstance(layer, ResnetBlock2D):
-                    x = layer(x, emb)
-                elif isinstance(layer, Transformer2DModel):
-                    x = layer(x, context)
-                else:
-                    x = layer(x)
-            return x
-
-        # h = x.type(self.dtype)
-        h = x
-        for module in self.input_blocks:
-            h = call_module(module, h, emb, context)
-            hs.append(h)
-
-        h = call_module(self.middle_block, h, emb, context)
-
-        for module in self.output_blocks:
-            h = torch.cat([h, hs.pop()], dim=1)
-            h = call_module(module, h, emb, context)
-
-        h = h.type(x.dtype)
-        h = call_module(self.out, h, emb, context)
-
-        return h
-
-
-if __name__ == "__main__":
-    import time
-
-    print("create unet")
-    unet = SdxlUNet2DConditionModel()
-
-    unet.to("cuda")
-    unet.set_use_memory_efficient_attention(True, False)
-    unet.set_gradient_checkpointing(True)
-    unet.train()
-
-    # 使用メモリ量確認用の疑似学習ループ
-    print("preparing optimizer")
-
-    # optimizer = torch.optim.SGD(unet.parameters(), lr=1e-3, nesterov=True, momentum=0.9) # not working
-
-    # import bitsandbytes
-    # optimizer = bitsandbytes.adam.Adam8bit(unet.parameters(), lr=1e-3)        # not working
-    # optimizer = bitsandbytes.optim.RMSprop8bit(unet.parameters(), lr=1e-3)  # working at 23.5 GB with torch2
-    # optimizer=bitsandbytes.optim.Adagrad8bit(unet.parameters(), lr=1e-3)  # working at 23.5 GB with torch2
-
-    import transformers
-
-    optimizer = transformers.optimization.Adafactor(
-        unet.parameters(), relative_step=True
-    )  # working at 22.2GB with torch2
-
-    scaler = torch.cuda.amp.GradScaler(enabled=True)
-
-    print("start training")
-    steps = 10
-    batch_size = 1
-
-    for step in range(steps):
-        print(f"step {step}")
-        if step == 1:
-            time_start = time.perf_counter()
-
-        x = torch.randn(batch_size, 4, 128, 128).cuda()  # 1024x1024
-        t = torch.randint(low=0, high=10, size=(batch_size,), device="cuda")
-        ctx = torch.randn(batch_size, 77, 2048).cuda()
-        y = torch.randn(batch_size, ADM_IN_CHANNELS).cuda()
-
-        with torch.cuda.amp.autocast(enabled=True):
-            output = unet(x, t, ctx, y)
-            target = torch.randn_like(output)
-            loss = torch.nn.functional.mse_loss(output, target)
-
-        scaler.scale(loss).backward()
-        scaler.step(optimizer)
-        scaler.update()
-        optimizer.zero_grad(set_to_none=True)
-
-    time_end = time.perf_counter()
-    print(f"elapsed time: {time_end - time_start} [sec] for last {steps - 1} steps")
+# Diffusersのコードをベースとした sd_xl_baseのU-Net
+# state dictの形式をSDXLに合わせてある
+
+"""
+      target: sgm.modules.diffusionmodules.openaimodel.UNetModel
+      params:
+        adm_in_channels: 2816
+        num_classes: sequential
+        use_checkpoint: True
+        in_channels: 4
+        out_channels: 4
+        model_channels: 320
+        attention_resolutions: [4, 2]
+        num_res_blocks: 2
+        channel_mult: [1, 2, 4]
+        num_head_channels: 64
+        use_spatial_transformer: True
+        use_linear_in_transformer: True
+        transformer_depth: [1, 2, 10]  # note: the first is unused (due to attn_res starting at 2) 32, 16, 8 --> 64, 32, 16
+        context_dim: 2048
+        spatial_transformer_attn_type: softmax-xformers
+        legacy: False
+"""
+
+import math
+from types import SimpleNamespace
+from typing import Optional
+import torch
+import torch.utils.checkpoint
+from torch import nn
+from torch.nn import functional as F
+from einops import rearrange
+
+
+IN_CHANNELS: int = 4
+OUT_CHANNELS: int = 4
+ADM_IN_CHANNELS: int = 2816
+CONTEXT_DIM: int = 2048
+MODEL_CHANNELS: int = 320
+TIME_EMBED_DIM = 320 * 4
+
+
+# region memory effcient attention
+
+# FlashAttentionを使うCrossAttention
+# based on https://github.com/lucidrains/memory-efficient-attention-pytorch/blob/main/memory_efficient_attention_pytorch/flash_attention.py
+# LICENSE MIT https://github.com/lucidrains/memory-efficient-attention-pytorch/blob/main/LICENSE
+
+# constants
+
+EPSILON = 1e-6
+
+# helper functions
+
+
+def exists(val):
+    return val is not None
+
+
+def default(val, d):
+    return val if exists(val) else d
+
+
+# flash attention forwards and backwards
+
+# https://arxiv.org/abs/2205.14135
+
+
+class FlashAttentionFunction(torch.autograd.Function):
+    @staticmethod
+    @torch.no_grad()
+    def forward(ctx, q, k, v, mask, causal, q_bucket_size, k_bucket_size):
+        """Algorithm 2 in the paper"""
+
+        device = q.device
+        dtype = q.dtype
+        max_neg_value = -torch.finfo(q.dtype).max
+        qk_len_diff = max(k.shape[-2] - q.shape[-2], 0)
+
+        o = torch.zeros_like(q)
+        all_row_sums = torch.zeros((*q.shape[:-1], 1), dtype=dtype, device=device)
+        all_row_maxes = torch.full(
+            (*q.shape[:-1], 1), max_neg_value, dtype=dtype, device=device
+        )
+
+        scale = q.shape[-1] ** -0.5
+
+        if not exists(mask):
+            mask = (None,) * math.ceil(q.shape[-2] / q_bucket_size)
+        else:
+            mask = rearrange(mask, "b n -> b 1 1 n")
+            mask = mask.split(q_bucket_size, dim=-1)
+
+        row_splits = zip(
+            q.split(q_bucket_size, dim=-2),
+            o.split(q_bucket_size, dim=-2),
+            mask,
+            all_row_sums.split(q_bucket_size, dim=-2),
+            all_row_maxes.split(q_bucket_size, dim=-2),
+        )
+
+        for ind, (qc, oc, row_mask, row_sums, row_maxes) in enumerate(row_splits):
+            q_start_index = ind * q_bucket_size - qk_len_diff
+
+            col_splits = zip(
+                k.split(k_bucket_size, dim=-2),
+                v.split(k_bucket_size, dim=-2),
+            )
+
+            for k_ind, (kc, vc) in enumerate(col_splits):
+                k_start_index = k_ind * k_bucket_size
+
+                attn_weights = (
+                    torch.einsum("... i d, ... j d -> ... i j", qc, kc) * scale
+                )
+
+                if exists(row_mask):
+                    attn_weights.masked_fill_(~row_mask, max_neg_value)
+
+                if causal and q_start_index < (k_start_index + k_bucket_size - 1):
+                    causal_mask = torch.ones(
+                        (qc.shape[-2], kc.shape[-2]), dtype=torch.bool, device=device
+                    ).triu(q_start_index - k_start_index + 1)
+                    attn_weights.masked_fill_(causal_mask, max_neg_value)
+
+                block_row_maxes = attn_weights.amax(dim=-1, keepdims=True)
+                attn_weights -= block_row_maxes
+                exp_weights = torch.exp(attn_weights)
+
+                if exists(row_mask):
+                    exp_weights.masked_fill_(~row_mask, 0.0)
+
+                block_row_sums = exp_weights.sum(dim=-1, keepdims=True).clamp(
+                    min=EPSILON
+                )
+
+                new_row_maxes = torch.maximum(block_row_maxes, row_maxes)
+
+                exp_values = torch.einsum(
+                    "... i j, ... j d -> ... i d", exp_weights, vc
+                )
+
+                exp_row_max_diff = torch.exp(row_maxes - new_row_maxes)
+                exp_block_row_max_diff = torch.exp(block_row_maxes - new_row_maxes)
+
+                new_row_sums = (
+                    exp_row_max_diff * row_sums
+                    + exp_block_row_max_diff * block_row_sums
+                )
+
+                oc.mul_((row_sums / new_row_sums) * exp_row_max_diff).add_(
+                    (exp_block_row_max_diff / new_row_sums) * exp_values
+                )
+
+                row_maxes.copy_(new_row_maxes)
+                row_sums.copy_(new_row_sums)
+
+        ctx.args = (causal, scale, mask, q_bucket_size, k_bucket_size)
+        ctx.save_for_backward(q, k, v, o, all_row_sums, all_row_maxes)
+
+        return o
+
+    @staticmethod
+    @torch.no_grad()
+    def backward(ctx, do):
+        """Algorithm 4 in the paper"""
+
+        causal, scale, mask, q_bucket_size, k_bucket_size = ctx.args
+        q, k, v, o, l, m = ctx.saved_tensors
+
+        device = q.device
+
+        max_neg_value = -torch.finfo(q.dtype).max
+        qk_len_diff = max(k.shape[-2] - q.shape[-2], 0)
+
+        dq = torch.zeros_like(q)
+        dk = torch.zeros_like(k)
+        dv = torch.zeros_like(v)
+
+        row_splits = zip(
+            q.split(q_bucket_size, dim=-2),
+            o.split(q_bucket_size, dim=-2),
+            do.split(q_bucket_size, dim=-2),
+            mask,
+            l.split(q_bucket_size, dim=-2),
+            m.split(q_bucket_size, dim=-2),
+            dq.split(q_bucket_size, dim=-2),
+        )
+
+        for ind, (qc, oc, doc, row_mask, lc, mc, dqc) in enumerate(row_splits):
+            q_start_index = ind * q_bucket_size - qk_len_diff
+
+            col_splits = zip(
+                k.split(k_bucket_size, dim=-2),
+                v.split(k_bucket_size, dim=-2),
+                dk.split(k_bucket_size, dim=-2),
+                dv.split(k_bucket_size, dim=-2),
+            )
+
+            for k_ind, (kc, vc, dkc, dvc) in enumerate(col_splits):
+                k_start_index = k_ind * k_bucket_size
+
+                attn_weights = (
+                    torch.einsum("... i d, ... j d -> ... i j", qc, kc) * scale
+                )
+
+                if causal and q_start_index < (k_start_index + k_bucket_size - 1):
+                    causal_mask = torch.ones(
+                        (qc.shape[-2], kc.shape[-2]), dtype=torch.bool, device=device
+                    ).triu(q_start_index - k_start_index + 1)
+                    attn_weights.masked_fill_(causal_mask, max_neg_value)
+
+                exp_attn_weights = torch.exp(attn_weights - mc)
+
+                if exists(row_mask):
+                    exp_attn_weights.masked_fill_(~row_mask, 0.0)
+
+                p = exp_attn_weights / lc
+
+                dv_chunk = torch.einsum("... i j, ... i d -> ... j d", p, doc)
+                dp = torch.einsum("... i d, ... j d -> ... i j", doc, vc)
+
+                D = (doc * oc).sum(dim=-1, keepdims=True)
+                ds = p * scale * (dp - D)
+
+                dq_chunk = torch.einsum("... i j, ... j d -> ... i d", ds, kc)
+                dk_chunk = torch.einsum("... i j, ... i d -> ... j d", ds, qc)
+
+                dqc.add_(dq_chunk)
+                dkc.add_(dk_chunk)
+                dvc.add_(dv_chunk)
+
+        return dq, dk, dv, None, None, None, None
+
+
+# endregion
+
+
+def get_parameter_dtype(parameter: torch.nn.Module):
+    return next(parameter.parameters()).dtype
+
+
+def get_parameter_device(parameter: torch.nn.Module):
+    return next(parameter.parameters()).device
+
+
+def get_timestep_embedding(
+    timesteps: torch.Tensor,
+    embedding_dim: int,
+    downscale_freq_shift: float = 1,
+    scale: float = 1,
+    max_period: int = 10000,
+):
+    """
+    This matches the implementation in Denoising Diffusion Probabilistic Models: Create sinusoidal timestep embeddings.
+
+    :param timesteps: a 1-D Tensor of N indices, one per batch element.
+                      These may be fractional.
+    :param embedding_dim: the dimension of the output. :param max_period: controls the minimum frequency of the
+    embeddings. :return: an [N x dim] Tensor of positional embeddings.
+    """
+    assert len(timesteps.shape) == 1, "Timesteps should be a 1d-array"
+
+    half_dim = embedding_dim // 2
+    exponent = -math.log(max_period) * torch.arange(
+        start=0, end=half_dim, dtype=torch.float32, device=timesteps.device
+    )
+    exponent = exponent / (half_dim - downscale_freq_shift)
+
+    emb = torch.exp(exponent)
+    emb = timesteps[:, None].float() * emb[None, :]
+
+    # scale embeddings
+    emb = scale * emb
+
+    # concat sine and cosine embeddings: flipped from Diffusers original ver because always flip_sin_to_cos=True
+    emb = torch.cat([torch.cos(emb), torch.sin(emb)], dim=-1)
+
+    # zero pad
+    if embedding_dim % 2 == 1:
+        emb = torch.nn.functional.pad(emb, (0, 1, 0, 0))
+    return emb
+
+
+class GroupNorm32(nn.GroupNorm):
+    def forward(self, x):
+        if self.weight.dtype != torch.float32:
+            return super().forward(x)
+        return super().forward(x.float()).type(x.dtype)
+
+
+class ResnetBlock2D(nn.Module):
+    def __init__(
+        self,
+        in_channels,
+        out_channels,
+    ):
+        super().__init__()
+        self.in_channels = in_channels
+        self.out_channels = out_channels
+
+        self.in_layers = nn.Sequential(
+            GroupNorm32(32, in_channels),
+            nn.SiLU(),
+            nn.Conv2d(in_channels, out_channels, kernel_size=3, stride=1, padding=1),
+        )
+
+        self.emb_layers = nn.Sequential(
+            nn.SiLU(), nn.Linear(TIME_EMBED_DIM, out_channels)
+        )
+
+        self.out_layers = nn.Sequential(
+            GroupNorm32(32, out_channels),
+            nn.SiLU(),
+            nn.Identity(),  # to make state_dict compatible with original model
+            nn.Conv2d(out_channels, out_channels, kernel_size=3, stride=1, padding=1),
+        )
+
+        if in_channels != out_channels:
+            self.skip_connection = nn.Conv2d(
+                in_channels, out_channels, kernel_size=1, stride=1, padding=0
+            )
+        else:
+            self.skip_connection = nn.Identity()
+
+        self.gradient_checkpointing = False
+
+    def forward_body(self, x, emb):
+        h = self.in_layers(x)
+        emb_out = self.emb_layers(emb).type(h.dtype)
+        h = h + emb_out[:, :, None, None]
+        h = self.out_layers(h)
+        x = self.skip_connection(x)
+        return x + h
+
+    def forward(self, x, emb):
+        if self.training and self.gradient_checkpointing:
+            # print("ResnetBlock2D: gradient_checkpointing")
+
+            def create_custom_forward(func):
+                def custom_forward(*inputs):
+                    return func(*inputs)
+
+                return custom_forward
+
+            x = torch.utils.checkpoint.checkpoint(
+                create_custom_forward(self.forward_body), x, emb
+            )
+        else:
+            x = self.forward_body(x, emb)
+
+        return x
+
+
+class Downsample2D(nn.Module):
+    def __init__(self, channels, out_channels):
+        super().__init__()
+
+        self.channels = channels
+        self.out_channels = out_channels
+
+        self.op = nn.Conv2d(self.channels, self.out_channels, 3, stride=2, padding=1)
+
+        self.gradient_checkpointing = False
+
+    def forward_body(self, hidden_states):
+        assert hidden_states.shape[1] == self.channels
+        hidden_states = self.op(hidden_states)
+
+        return hidden_states
+
+    def forward(self, hidden_states):
+        if self.training and self.gradient_checkpointing:
+            # print("Downsample2D: gradient_checkpointing")
+
+            def create_custom_forward(func):
+                def custom_forward(*inputs):
+                    return func(*inputs)
+
+                return custom_forward
+
+            hidden_states = torch.utils.checkpoint.checkpoint(
+                create_custom_forward(self.forward_body), hidden_states
+            )
+        else:
+            hidden_states = self.forward_body(hidden_states)
+
+        return hidden_states
+
+
+class CrossAttention(nn.Module):
+    def __init__(
+        self,
+        query_dim: int,
+        cross_attention_dim: Optional[int] = None,
+        heads: int = 8,
+        dim_head: int = 64,
+        upcast_attention: bool = False,
+    ):
+        super().__init__()
+        inner_dim = dim_head * heads
+        cross_attention_dim = (
+            cross_attention_dim if cross_attention_dim is not None else query_dim
+        )
+        self.upcast_attention = upcast_attention
+
+        self.scale = dim_head**-0.5
+        self.heads = heads
+
+        self.to_q = nn.Linear(query_dim, inner_dim, bias=False)
+        self.to_k = nn.Linear(cross_attention_dim, inner_dim, bias=False)
+        self.to_v = nn.Linear(cross_attention_dim, inner_dim, bias=False)
+
+        self.to_out = nn.ModuleList([])
+        self.to_out.append(nn.Linear(inner_dim, query_dim))
+        # no dropout here
+
+        self.use_memory_efficient_attention_xformers = False
+        self.use_memory_efficient_attention_mem_eff = False
+        self.use_sdpa = False
+
+    def set_use_memory_efficient_attention(self, xformers, mem_eff):
+        self.use_memory_efficient_attention_xformers = xformers
+        self.use_memory_efficient_attention_mem_eff = mem_eff
+
+    def set_use_sdpa(self, sdpa):
+        self.use_sdpa = sdpa
+
+    def reshape_heads_to_batch_dim(self, tensor):
+        batch_size, seq_len, dim = tensor.shape
+        head_size = self.heads
+        tensor = tensor.reshape(batch_size, seq_len, head_size, dim // head_size)
+        tensor = tensor.permute(0, 2, 1, 3).reshape(
+            batch_size * head_size, seq_len, dim // head_size
+        )
+        return tensor
+
+    def reshape_batch_dim_to_heads(self, tensor):
+        batch_size, seq_len, dim = tensor.shape
+        head_size = self.heads
+        tensor = tensor.reshape(batch_size // head_size, head_size, seq_len, dim)
+        tensor = tensor.permute(0, 2, 1, 3).reshape(
+            batch_size // head_size, seq_len, dim * head_size
+        )
+        return tensor
+
+    def forward(self, hidden_states, context=None, mask=None):
+        if self.use_memory_efficient_attention_xformers:
+            return self.forward_memory_efficient_xformers(hidden_states, context, mask)
+        if self.use_memory_efficient_attention_mem_eff:
+            return self.forward_memory_efficient_mem_eff(hidden_states, context, mask)
+        if self.use_sdpa:
+            return self.forward_sdpa(hidden_states, context, mask)
+
+        query = self.to_q(hidden_states)
+        context = context if context is not None else hidden_states
+        key = self.to_k(context)
+        value = self.to_v(context)
+
+        query = self.reshape_heads_to_batch_dim(query)
+        key = self.reshape_heads_to_batch_dim(key)
+        value = self.reshape_heads_to_batch_dim(value)
+
+        hidden_states = self._attention(query, key, value)
+
+        # linear proj
+        hidden_states = self.to_out[0](hidden_states)
+        # hidden_states = self.to_out[1](hidden_states)     # no dropout
+        return hidden_states
+
+    def _attention(self, query, key, value):
+        if self.upcast_attention:
+            query = query.float()
+            key = key.float()
+
+        attention_scores = torch.baddbmm(
+            torch.empty(
+                query.shape[0],
+                query.shape[1],
+                key.shape[1],
+                dtype=query.dtype,
+                device=query.device,
+            ),
+            query,
+            key.transpose(-1, -2),
+            beta=0,
+            alpha=self.scale,
+        )
+        attention_probs = attention_scores.softmax(dim=-1)
+
+        # cast back to the original dtype
+        attention_probs = attention_probs.to(value.dtype)
+
+        # compute attention output
+        hidden_states = torch.bmm(attention_probs, value)
+
+        # reshape hidden_states
+        hidden_states = self.reshape_batch_dim_to_heads(hidden_states)
+        return hidden_states
+
+    # TODO support Hypernetworks
+    def forward_memory_efficient_xformers(self, x, context=None, mask=None):
+        import xformers.ops
+
+        h = self.heads
+        q_in = self.to_q(x)
+        context = context if context is not None else x
+        context = context.to(x.dtype)
+        k_in = self.to_k(context)
+        v_in = self.to_v(context)
+
+        q, k, v = map(
+            lambda t: rearrange(t, "b n (h d) -> b n h d", h=h), (q_in, k_in, v_in)
+        )
+        del q_in, k_in, v_in
+
+        q = q.contiguous()
+        k = k.contiguous()
+        v = v.contiguous()
+        out = xformers.ops.memory_efficient_attention(
+            q, k, v, attn_bias=None
+        )  # 最適なのを選んでくれる
+        del q, k, v
+
+        out = rearrange(out, "b n h d -> b n (h d)", h=h)
+
+        out = self.to_out[0](out)
+        return out
+
+    def forward_memory_efficient_mem_eff(self, x, context=None, mask=None):
+        flash_func = FlashAttentionFunction
+
+        q_bucket_size = 512
+        k_bucket_size = 1024
+
+        h = self.heads
+        q = self.to_q(x)
+        context = context if context is not None else x
+        context = context.to(x.dtype)
+        k = self.to_k(context)
+        v = self.to_v(context)
+        del context, x
+
+        q, k, v = map(lambda t: rearrange(t, "b n (h d) -> b h n d", h=h), (q, k, v))
+
+        out = flash_func.apply(q, k, v, mask, False, q_bucket_size, k_bucket_size)
+
+        out = rearrange(out, "b h n d -> b n (h d)")
+
+        out = self.to_out[0](out)
+        return out
+
+    def forward_sdpa(self, x, context=None, mask=None):
+        h = self.heads
+        q_in = self.to_q(x)
+        context = context if context is not None else x
+        context = context.to(x.dtype)
+        k_in = self.to_k(context)
+        v_in = self.to_v(context)
+
+        q, k, v = map(
+            lambda t: rearrange(t, "b n (h d) -> b h n d", h=h), (q_in, k_in, v_in)
+        )
+        del q_in, k_in, v_in
+
+        out = F.scaled_dot_product_attention(
+            q, k, v, attn_mask=mask, dropout_p=0.0, is_causal=False
+        )
+
+        out = rearrange(out, "b h n d -> b n (h d)", h=h)
+
+        out = self.to_out[0](out)
+        return out
+
+
+# feedforward
+class GEGLU(nn.Module):
+    r"""
+    A variant of the gated linear unit activation function from https://arxiv.org/abs/2002.05202.
+
+    Parameters:
+        dim_in (`int`): The number of channels in the input.
+        dim_out (`int`): The number of channels in the output.
+    """
+
+    def __init__(self, dim_in: int, dim_out: int):
+        super().__init__()
+        self.proj = nn.Linear(dim_in, dim_out * 2)
+
+    def gelu(self, gate):
+        if gate.device.type != "mps":
+            return F.gelu(gate)
+        # mps: gelu is not implemented for float16
+        return F.gelu(gate.to(dtype=torch.float32)).to(dtype=gate.dtype)
+
+    def forward(self, hidden_states):
+        hidden_states, gate = self.proj(hidden_states).chunk(2, dim=-1)
+        return hidden_states * self.gelu(gate)
+
+
+class FeedForward(nn.Module):
+    def __init__(
+        self,
+        dim: int,
+    ):
+        super().__init__()
+        inner_dim = int(dim * 4)  # mult is always 4
+
+        self.net = nn.ModuleList([])
+        # project in
+        self.net.append(GEGLU(dim, inner_dim))
+        # project dropout
+        self.net.append(nn.Identity())  # nn.Dropout(0)) # dummy for dropout with 0
+        # project out
+        self.net.append(nn.Linear(inner_dim, dim))
+
+    def forward(self, hidden_states):
+        for module in self.net:
+            hidden_states = module(hidden_states)
+        return hidden_states
+
+
+class BasicTransformerBlock(nn.Module):
+    def __init__(
+        self,
+        dim: int,
+        num_attention_heads: int,
+        attention_head_dim: int,
+        cross_attention_dim: int,
+        upcast_attention: bool = False,
+    ):
+        super().__init__()
+
+        self.gradient_checkpointing = False
+
+        # 1. Self-Attn
+        self.attn1 = CrossAttention(
+            query_dim=dim,
+            cross_attention_dim=None,
+            heads=num_attention_heads,
+            dim_head=attention_head_dim,
+            upcast_attention=upcast_attention,
+        )
+        self.ff = FeedForward(dim)
+
+        # 2. Cross-Attn
+        self.attn2 = CrossAttention(
+            query_dim=dim,
+            cross_attention_dim=cross_attention_dim,
+            heads=num_attention_heads,
+            dim_head=attention_head_dim,
+            upcast_attention=upcast_attention,
+        )
+
+        self.norm1 = nn.LayerNorm(dim)
+        self.norm2 = nn.LayerNorm(dim)
+
+        # 3. Feed-forward
+        self.norm3 = nn.LayerNorm(dim)
+
+    def set_use_memory_efficient_attention(self, xformers: bool, mem_eff: bool):
+        self.attn1.set_use_memory_efficient_attention(xformers, mem_eff)
+        self.attn2.set_use_memory_efficient_attention(xformers, mem_eff)
+
+    def set_use_sdpa(self, sdpa: bool):
+        self.attn1.set_use_sdpa(sdpa)
+        self.attn2.set_use_sdpa(sdpa)
+
+    def forward_body(self, hidden_states, context=None, timestep=None):
+        # 1. Self-Attention
+        norm_hidden_states = self.norm1(hidden_states)
+
+        hidden_states = self.attn1(norm_hidden_states) + hidden_states
+
+        # 2. Cross-Attention
+        norm_hidden_states = self.norm2(hidden_states)
+        hidden_states = self.attn2(norm_hidden_states, context=context) + hidden_states
+
+        # 3. Feed-forward
+        hidden_states = self.ff(self.norm3(hidden_states)) + hidden_states
+
+        return hidden_states
+
+    def forward(self, hidden_states, context=None, timestep=None):
+        if self.training and self.gradient_checkpointing:
+            # print("BasicTransformerBlock: checkpointing")
+
+            def create_custom_forward(func):
+                def custom_forward(*inputs):
+                    return func(*inputs)
+
+                return custom_forward
+
+            output = torch.utils.checkpoint.checkpoint(
+                create_custom_forward(self.forward_body),
+                hidden_states,
+                context,
+                timestep,
+            )
+        else:
+            output = self.forward_body(hidden_states, context, timestep)
+
+        return output
+
+
+class Transformer2DModel(nn.Module):
+    def __init__(
+        self,
+        num_attention_heads: int = 16,
+        attention_head_dim: int = 88,
+        in_channels: Optional[int] = None,
+        cross_attention_dim: Optional[int] = None,
+        use_linear_projection: bool = False,
+        upcast_attention: bool = False,
+        num_transformer_layers: int = 1,
+    ):
+        super().__init__()
+        self.in_channels = in_channels
+        self.num_attention_heads = num_attention_heads
+        self.attention_head_dim = attention_head_dim
+        inner_dim = num_attention_heads * attention_head_dim
+        self.use_linear_projection = use_linear_projection
+
+        self.norm = torch.nn.GroupNorm(
+            num_groups=32, num_channels=in_channels, eps=1e-6, affine=True
+        )
+        # self.norm = GroupNorm32(32, in_channels, eps=1e-6, affine=True)
+
+        if use_linear_projection:
+            self.proj_in = nn.Linear(in_channels, inner_dim)
+        else:
+            self.proj_in = nn.Conv2d(
+                in_channels, inner_dim, kernel_size=1, stride=1, padding=0
+            )
+
+        blocks = []
+        for _ in range(num_transformer_layers):
+            blocks.append(
+                BasicTransformerBlock(
+                    inner_dim,
+                    num_attention_heads,
+                    attention_head_dim,
+                    cross_attention_dim=cross_attention_dim,
+                    upcast_attention=upcast_attention,
+                )
+            )
+
+        self.transformer_blocks = nn.ModuleList(blocks)
+
+        if use_linear_projection:
+            self.proj_out = nn.Linear(in_channels, inner_dim)
+        else:
+            self.proj_out = nn.Conv2d(
+                inner_dim, in_channels, kernel_size=1, stride=1, padding=0
+            )
+
+        self.gradient_checkpointing = False
+
+    def set_use_memory_efficient_attention(self, xformers, mem_eff):
+        for transformer in self.transformer_blocks:
+            transformer.set_use_memory_efficient_attention(xformers, mem_eff)
+
+    def set_use_sdpa(self, sdpa):
+        for transformer in self.transformer_blocks:
+            transformer.set_use_sdpa(sdpa)
+
+    def forward(self, hidden_states, encoder_hidden_states=None, timestep=None):
+        # 1. Input
+        batch, _, height, weight = hidden_states.shape
+        residual = hidden_states
+
+        hidden_states = self.norm(hidden_states)
+        if not self.use_linear_projection:
+            hidden_states = self.proj_in(hidden_states)
+            inner_dim = hidden_states.shape[1]
+            hidden_states = hidden_states.permute(0, 2, 3, 1).reshape(
+                batch, height * weight, inner_dim
+            )
+        else:
+            inner_dim = hidden_states.shape[1]
+            hidden_states = hidden_states.permute(0, 2, 3, 1).reshape(
+                batch, height * weight, inner_dim
+            )
+            hidden_states = self.proj_in(hidden_states)
+
+        # 2. Blocks
+        for block in self.transformer_blocks:
+            hidden_states = block(
+                hidden_states, context=encoder_hidden_states, timestep=timestep
+            )
+
+        # 3. Output
+        if not self.use_linear_projection:
+            hidden_states = (
+                hidden_states.reshape(batch, height, weight, inner_dim)
+                .permute(0, 3, 1, 2)
+                .contiguous()
+            )
+            hidden_states = self.proj_out(hidden_states)
+        else:
+            hidden_states = self.proj_out(hidden_states)
+            hidden_states = (
+                hidden_states.reshape(batch, height, weight, inner_dim)
+                .permute(0, 3, 1, 2)
+                .contiguous()
+            )
+
+        output = hidden_states + residual
+
+        return output
+
+
+class Upsample2D(nn.Module):
+    def __init__(self, channels, out_channels):
+        super().__init__()
+        self.channels = channels
+        self.out_channels = out_channels
+        self.conv = nn.Conv2d(self.channels, self.out_channels, 3, padding=1)
+
+        self.gradient_checkpointing = False
+
+    def forward_body(self, hidden_states, output_size=None):
+        assert hidden_states.shape[1] == self.channels
+
+        # Cast to float32 to as 'upsample_nearest2d_out_frame' op does not support bfloat16
+        # TODO(Suraj): Remove this cast once the issue is fixed in PyTorch
+        # https://github.com/pytorch/pytorch/issues/86679
+        dtype = hidden_states.dtype
+        if dtype == torch.bfloat16:
+            hidden_states = hidden_states.to(torch.float32)
+
+        # upsample_nearest_nhwc fails with large batch sizes. see https://github.com/huggingface/diffusers/issues/984
+        if hidden_states.shape[0] >= 64:
+            hidden_states = hidden_states.contiguous()
+
+        # if `output_size` is passed we force the interpolation output size and do not make use of `scale_factor=2`
+        if output_size is None:
+            hidden_states = F.interpolate(
+                hidden_states, scale_factor=2.0, mode="nearest"
+            )
+        else:
+            hidden_states = F.interpolate(
+                hidden_states, size=output_size, mode="nearest"
+            )
+
+        # If the input is bfloat16, we cast back to bfloat16
+        if dtype == torch.bfloat16:
+            hidden_states = hidden_states.to(dtype)
+
+        hidden_states = self.conv(hidden_states)
+
+        return hidden_states
+
+    def forward(self, hidden_states, output_size=None):
+        if self.training and self.gradient_checkpointing:
+            # print("Upsample2D: gradient_checkpointing")
+
+            def create_custom_forward(func):
+                def custom_forward(*inputs):
+                    return func(*inputs)
+
+                return custom_forward
+
+            hidden_states = torch.utils.checkpoint.checkpoint(
+                create_custom_forward(self.forward_body), hidden_states, output_size
+            )
+        else:
+            hidden_states = self.forward_body(hidden_states, output_size)
+
+        return hidden_states
+
+
+class SdxlUNet2DConditionModel(nn.Module):
+    _supports_gradient_checkpointing = True
+
+    def __init__(
+        self,
+        **kwargs,
+    ):
+        super().__init__()
+
+        self.in_channels = IN_CHANNELS
+        self.out_channels = OUT_CHANNELS
+        self.model_channels = MODEL_CHANNELS
+        self.time_embed_dim = TIME_EMBED_DIM
+        self.adm_in_channels = ADM_IN_CHANNELS
+
+        self.gradient_checkpointing = False
+        # self.sample_size = sample_size
+
+        # time embedding
+        self.time_embed = nn.Sequential(
+            nn.Linear(self.model_channels, self.time_embed_dim),
+            nn.SiLU(),
+            nn.Linear(self.time_embed_dim, self.time_embed_dim),
+        )
+
+        # label embedding
+        self.label_emb = nn.Sequential(
+            nn.Sequential(
+                nn.Linear(self.adm_in_channels, self.time_embed_dim),
+                nn.SiLU(),
+                nn.Linear(self.time_embed_dim, self.time_embed_dim),
+            )
+        )
+
+        # input
+        self.input_blocks = nn.ModuleList(
+            [
+                nn.Sequential(
+                    nn.Conv2d(
+                        self.in_channels,
+                        self.model_channels,
+                        kernel_size=3,
+                        padding=(1, 1),
+                    ),
+                )
+            ]
+        )
+
+        # level 0
+        for i in range(2):
+            layers = [
+                ResnetBlock2D(
+                    in_channels=1 * self.model_channels,
+                    out_channels=1 * self.model_channels,
+                ),
+            ]
+            self.input_blocks.append(nn.ModuleList(layers))
+
+        self.input_blocks.append(
+            nn.Sequential(
+                Downsample2D(
+                    channels=1 * self.model_channels,
+                    out_channels=1 * self.model_channels,
+                ),
+            )
+        )
+
+        # level 1
+        for i in range(2):
+            layers = [
+                ResnetBlock2D(
+                    in_channels=(1 if i == 0 else 2) * self.model_channels,
+                    out_channels=2 * self.model_channels,
+                ),
+                Transformer2DModel(
+                    num_attention_heads=2 * self.model_channels // 64,
+                    attention_head_dim=64,
+                    in_channels=2 * self.model_channels,
+                    num_transformer_layers=2,
+                    use_linear_projection=True,
+                    cross_attention_dim=2048,
+                ),
+            ]
+            self.input_blocks.append(nn.ModuleList(layers))
+
+        self.input_blocks.append(
+            nn.Sequential(
+                Downsample2D(
+                    channels=2 * self.model_channels,
+                    out_channels=2 * self.model_channels,
+                ),
+            )
+        )
+
+        # level 2
+        for i in range(2):
+            layers = [
+                ResnetBlock2D(
+                    in_channels=(2 if i == 0 else 4) * self.model_channels,
+                    out_channels=4 * self.model_channels,
+                ),
+                Transformer2DModel(
+                    num_attention_heads=4 * self.model_channels // 64,
+                    attention_head_dim=64,
+                    in_channels=4 * self.model_channels,
+                    num_transformer_layers=10,
+                    use_linear_projection=True,
+                    cross_attention_dim=2048,
+                ),
+            ]
+            self.input_blocks.append(nn.ModuleList(layers))
+
+        # mid
+        self.middle_block = nn.ModuleList(
+            [
+                ResnetBlock2D(
+                    in_channels=4 * self.model_channels,
+                    out_channels=4 * self.model_channels,
+                ),
+                Transformer2DModel(
+                    num_attention_heads=4 * self.model_channels // 64,
+                    attention_head_dim=64,
+                    in_channels=4 * self.model_channels,
+                    num_transformer_layers=10,
+                    use_linear_projection=True,
+                    cross_attention_dim=2048,
+                ),
+                ResnetBlock2D(
+                    in_channels=4 * self.model_channels,
+                    out_channels=4 * self.model_channels,
+                ),
+            ]
+        )
+
+        # output
+        self.output_blocks = nn.ModuleList([])
+
+        # level 2
+        for i in range(3):
+            layers = [
+                ResnetBlock2D(
+                    in_channels=4 * self.model_channels
+                    + (4 if i <= 1 else 2) * self.model_channels,
+                    out_channels=4 * self.model_channels,
+                ),
+                Transformer2DModel(
+                    num_attention_heads=4 * self.model_channels // 64,
+                    attention_head_dim=64,
+                    in_channels=4 * self.model_channels,
+                    num_transformer_layers=10,
+                    use_linear_projection=True,
+                    cross_attention_dim=2048,
+                ),
+            ]
+            if i == 2:
+                layers.append(
+                    Upsample2D(
+                        channels=4 * self.model_channels,
+                        out_channels=4 * self.model_channels,
+                    )
+                )
+
+            self.output_blocks.append(nn.ModuleList(layers))
+
+        # level 1
+        for i in range(3):
+            layers = [
+                ResnetBlock2D(
+                    in_channels=2 * self.model_channels
+                    + (4 if i == 0 else (2 if i == 1 else 1)) * self.model_channels,
+                    out_channels=2 * self.model_channels,
+                ),
+                Transformer2DModel(
+                    num_attention_heads=2 * self.model_channels // 64,
+                    attention_head_dim=64,
+                    in_channels=2 * self.model_channels,
+                    num_transformer_layers=2,
+                    use_linear_projection=True,
+                    cross_attention_dim=2048,
+                ),
+            ]
+            if i == 2:
+                layers.append(
+                    Upsample2D(
+                        channels=2 * self.model_channels,
+                        out_channels=2 * self.model_channels,
+                    )
+                )
+
+            self.output_blocks.append(nn.ModuleList(layers))
+
+        # level 0
+        for i in range(3):
+            layers = [
+                ResnetBlock2D(
+                    in_channels=1 * self.model_channels
+                    + (2 if i == 0 else 1) * self.model_channels,
+                    out_channels=1 * self.model_channels,
+                ),
+            ]
+
+            self.output_blocks.append(nn.ModuleList(layers))
+
+        # output
+        self.out = nn.ModuleList(
+            [
+                GroupNorm32(32, self.model_channels),
+                nn.SiLU(),
+                nn.Conv2d(self.model_channels, self.out_channels, 3, padding=1),
+            ]
+        )
+
+    # region diffusers compatibility
+    def prepare_config(self):
+        self.config = SimpleNamespace()
+
+    @property
+    def dtype(self) -> torch.dtype:
+        # `torch.dtype`: The dtype of the module (assuming that all the module parameters have the same dtype).
+        return get_parameter_dtype(self)
+
+    @property
+    def device(self) -> torch.device:
+        # `torch.device`: The device on which the module is (assuming that all the module parameters are on the same device).
+        return get_parameter_device(self)
+
+    def set_attention_slice(self, slice_size):
+        raise NotImplementedError("Attention slicing is not supported for this model.")
+
+    def is_gradient_checkpointing(self) -> bool:
+        return any(
+            hasattr(m, "gradient_checkpointing") and m.gradient_checkpointing
+            for m in self.modules()
+        )
+
+    def enable_gradient_checkpointing(self):
+        self.gradient_checkpointing = True
+        self.set_gradient_checkpointing(value=True)
+
+    def disable_gradient_checkpointing(self):
+        self.gradient_checkpointing = False
+        self.set_gradient_checkpointing(value=False)
+
+    def set_use_memory_efficient_attention(self, xformers: bool, mem_eff: bool) -> None:
+        blocks = self.input_blocks + [self.middle_block] + self.output_blocks
+        for block in blocks:
+            for module in block:
+                if hasattr(module, "set_use_memory_efficient_attention"):
+                    # print(module.__class__.__name__)
+                    module.set_use_memory_efficient_attention(xformers, mem_eff)
+
+    def set_use_sdpa(self, sdpa: bool) -> None:
+        blocks = self.input_blocks + [self.middle_block] + self.output_blocks
+        for block in blocks:
+            for module in block:
+                if hasattr(module, "set_use_sdpa"):
+                    module.set_use_sdpa(sdpa)
+
+    def set_gradient_checkpointing(self, value=False):
+        blocks = self.input_blocks + [self.middle_block] + self.output_blocks
+        for block in blocks:
+            for module in block.modules():
+                if hasattr(module, "gradient_checkpointing"):
+                    # print(module.__class__.__name__, module.gradient_checkpointing, "->", value)
+                    module.gradient_checkpointing = value
+
+    # endregion
+
+    def forward(self, x, timesteps=None, context=None, y=None, **kwargs):
+        # broadcast timesteps to batch dimension
+        timesteps = timesteps.expand(x.shape[0])
+
+        hs = []
+        t_emb = get_timestep_embedding(
+            timesteps, self.model_channels
+        )  # , repeat_only=False)
+        t_emb = t_emb.to(x.dtype)
+        emb = self.time_embed(t_emb)
+
+        assert (
+            x.shape[0] == y.shape[0]
+        ), f"batch size mismatch: {x.shape[0]} != {y.shape[0]}"
+        assert x.dtype == y.dtype, f"dtype mismatch: {x.dtype} != {y.dtype}"
+        # assert x.dtype == self.dtype
+        emb = emb + self.label_emb(y)
+
+        def call_module(module, h, emb, context):
+            x = h
+            for layer in module:
+                # print(layer.__class__.__name__, x.dtype, emb.dtype, context.dtype if context is not None else None)
+                if isinstance(layer, ResnetBlock2D):
+                    x = layer(x, emb)
+                elif isinstance(layer, Transformer2DModel):
+                    x = layer(x, context)
+                else:
+                    x = layer(x)
+            return x
+
+        # h = x.type(self.dtype)
+        h = x
+        for module in self.input_blocks:
+            h = call_module(module, h, emb, context)
+            hs.append(h)
+
+        h = call_module(self.middle_block, h, emb, context)
+
+        for module in self.output_blocks:
+            h = torch.cat([h, hs.pop()], dim=1)
+            h = call_module(module, h, emb, context)
+
+        h = h.type(x.dtype)
+        h = call_module(self.out, h, emb, context)
+
+        return h
+
+
+if __name__ == "__main__":
+    import time
+
+    print("create unet")
+    unet = SdxlUNet2DConditionModel()
+
+    unet.to("cuda")
+    unet.set_use_memory_efficient_attention(True, False)
+    unet.set_gradient_checkpointing(True)
+    unet.train()
+
+    # 使用メモリ量確認用の疑似学習ループ
+    print("preparing optimizer")
+
+    # optimizer = torch.optim.SGD(unet.parameters(), lr=1e-3, nesterov=True, momentum=0.9) # not working
+
+    # import bitsandbytes
+    # optimizer = bitsandbytes.adam.Adam8bit(unet.parameters(), lr=1e-3)        # not working
+    # optimizer = bitsandbytes.optim.RMSprop8bit(unet.parameters(), lr=1e-3)  # working at 23.5 GB with torch2
+    # optimizer=bitsandbytes.optim.Adagrad8bit(unet.parameters(), lr=1e-3)  # working at 23.5 GB with torch2
+
+    import transformers
+
+    optimizer = transformers.optimization.Adafactor(
+        unet.parameters(), relative_step=True
+    )  # working at 22.2GB with torch2
+
+    scaler = torch.cuda.amp.GradScaler(enabled=True)
+
+    print("start training")
+    steps = 10
+    batch_size = 1
+
+    for step in range(steps):
+        print(f"step {step}")
+        if step == 1:
+            time_start = time.perf_counter()
+
+        x = torch.randn(batch_size, 4, 128, 128).cuda()  # 1024x1024
+        t = torch.randint(low=0, high=10, size=(batch_size,), device="cuda")
+        ctx = torch.randn(batch_size, 77, 2048).cuda()
+        y = torch.randn(batch_size, ADM_IN_CHANNELS).cuda()
+
+        with torch.cuda.amp.autocast(enabled=True):
+            output = unet(x, t, ctx, y)
+            target = torch.randn_like(output)
+            loss = torch.nn.functional.mse_loss(output, target)
+
+        scaler.scale(loss).backward()
+        scaler.step(optimizer)
+        scaler.update()
+        optimizer.zero_grad(set_to_none=True)
+
+    time_end = time.perf_counter()
+    print(f"elapsed time: {time_end - time_start} [sec] for last {steps - 1} steps")
```

### Comparing `lycoris_lora-2.3.0.dev4/lycoris/kohya/utils.py` & `lycoris_lora-2.3.0.dev5/lycoris/kohya/utils.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-# part of https://github.com/kohya-ss/sd-scripts/blob/main/library/train_util.py
-
-import hashlib
-import safetensors
-from io import BytesIO
-
-
-def addnet_hash_legacy(b):
-    """Old model hash used by sd-webui-additional-networks for .safetensors format files"""
-    m = hashlib.sha256()
-
-    b.seek(0x100000)
-    m.update(b.read(0x10000))
-    return m.hexdigest()[0:8]
-
-
-def addnet_hash_safetensors(b):
-    """New model hash used by sd-webui-additional-networks for .safetensors format files"""
-    hash_sha256 = hashlib.sha256()
-    blksize = 1024 * 1024
-
-    b.seek(0)
-    header = b.read(8)
-    n = int.from_bytes(header, "little")
-
-    offset = n + 8
-    b.seek(offset)
-    for chunk in iter(lambda: b.read(blksize), b""):
-        hash_sha256.update(chunk)
-
-    return hash_sha256.hexdigest()
-
-
-def precalculate_safetensors_hashes(tensors, metadata):
-    """Precalculate the model hashes needed by sd-webui-additional-networks to
-    save time on indexing the model later."""
-
-    # Because writing user metadata to the file can change the result of
-    # sd_models.model_hash(), only retain the training metadata for purposes of
-    # calculating the hash, as they are meant to be immutable
-    metadata = {k: v for k, v in metadata.items() if k.startswith("ss_")}
-
-    bytes = safetensors.torch.save(tensors, metadata)
-    b = BytesIO(bytes)
-
-    model_hash = addnet_hash_safetensors(b)
-    legacy_hash = addnet_hash_legacy(b)
-    return model_hash, legacy_hash
+# part of https://github.com/kohya-ss/sd-scripts/blob/main/library/train_util.py
+
+import hashlib
+import safetensors
+from io import BytesIO
+
+
+def addnet_hash_legacy(b):
+    """Old model hash used by sd-webui-additional-networks for .safetensors format files"""
+    m = hashlib.sha256()
+
+    b.seek(0x100000)
+    m.update(b.read(0x10000))
+    return m.hexdigest()[0:8]
+
+
+def addnet_hash_safetensors(b):
+    """New model hash used by sd-webui-additional-networks for .safetensors format files"""
+    hash_sha256 = hashlib.sha256()
+    blksize = 1024 * 1024
+
+    b.seek(0)
+    header = b.read(8)
+    n = int.from_bytes(header, "little")
+
+    offset = n + 8
+    b.seek(offset)
+    for chunk in iter(lambda: b.read(blksize), b""):
+        hash_sha256.update(chunk)
+
+    return hash_sha256.hexdigest()
+
+
+def precalculate_safetensors_hashes(tensors, metadata):
+    """Precalculate the model hashes needed by sd-webui-additional-networks to
+    save time on indexing the model later."""
+
+    # Because writing user metadata to the file can change the result of
+    # sd_models.model_hash(), only retain the training metadata for purposes of
+    # calculating the hash, as they are meant to be immutable
+    metadata = {k: v for k, v in metadata.items() if k.startswith("ss_")}
+
+    bytes = safetensors.torch.save(tensors, metadata)
+    b = BytesIO(bytes)
+
+    model_hash = addnet_hash_safetensors(b)
+    legacy_hash = addnet_hash_legacy(b)
+    return model_hash, legacy_hash
```

### Comparing `lycoris_lora-2.3.0.dev4/lycoris/logging.py` & `lycoris_lora-2.3.0.dev5/lycoris/logging.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-import sys
-import copy
-import logging
-
-
-class ColoredFormatter(logging.Formatter):
-    COLORS = {
-        "DEBUG": "\033[0;36m",  # CYAN
-        "INFO": "\033[0;32m",  # GREEN
-        "WARNING": "\033[0;33m",  # YELLOW
-        "ERROR": "\033[0;31m",  # RED
-        "CRITICAL": "\033[0;37;41m",  # WHITE ON RED
-        "RESET": "\033[0m",  # RESET COLOR
-    }
-
-    def format(self, record):
-        colored_record = copy.copy(record)
-        levelname = colored_record.levelname
-        seq = self.COLORS.get(levelname, self.COLORS["RESET"])
-        colored_record.levelname = f"{seq}{levelname}{self.COLORS['RESET']}"
-        return super().format(colored_record)
-
-
-logger = logging.getLogger("LyCORIS")
-logger.propagate = False
-logger.setLevel(logging.INFO)
-
-
-if not logger.handlers:
-    handler = logging.StreamHandler(sys.stdout)
-    handler.setFormatter(
-        ColoredFormatter(
-            "%(asctime)s|[%(name)s]-%(levelname)s: %(message)s", "%Y-%m-%d %H:%M:%S"
-        )
-    )
-    logger.addHandler(handler)
+import sys
+import copy
+import logging
+
+
+class ColoredFormatter(logging.Formatter):
+    COLORS = {
+        "DEBUG": "\033[0;36m",  # CYAN
+        "INFO": "\033[0;32m",  # GREEN
+        "WARNING": "\033[0;33m",  # YELLOW
+        "ERROR": "\033[0;31m",  # RED
+        "CRITICAL": "\033[0;37;41m",  # WHITE ON RED
+        "RESET": "\033[0m",  # RESET COLOR
+    }
+
+    def format(self, record):
+        colored_record = copy.copy(record)
+        levelname = colored_record.levelname
+        seq = self.COLORS.get(levelname, self.COLORS["RESET"])
+        colored_record.levelname = f"{seq}{levelname}{self.COLORS['RESET']}"
+        return super().format(colored_record)
+
+
+logger = logging.getLogger("LyCORIS")
+logger.propagate = False
+logger.setLevel(logging.INFO)
+
+
+if not logger.handlers:
+    handler = logging.StreamHandler(sys.stdout)
+    handler.setFormatter(
+        ColoredFormatter(
+            "%(asctime)s|[%(name)s]-%(levelname)s: %(message)s", "%Y-%m-%d %H:%M:%S"
+        )
+    )
+    logger.addHandler(handler)
```

### Comparing `lycoris_lora-2.3.0.dev4/lycoris/modules/__init__.py` & `lycoris_lora-2.3.0.dev5/lycoris/modules/__init__.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,133 +1,133 @@
-import torch
-
-from .full import FullModule
-from .norms import NormModule
-from .locon import LoConModule
-from .loha import LohaModule
-from .lokr import LokrModule, factorization
-from .ia3 import IA3Module
-
-
-@torch.no_grad()
-def make_module(lyco_type, params, lora_name, orig_module):
-    module = None
-    if lyco_type == "locon":
-        up, down, mid, alpha, dora_scale = params
-        module = LoConModule(
-            lora_name,
-            orig_module,
-            1,
-            down.size(0),
-            float(alpha),
-            use_tucker=mid is not None,
-            weight_decompose=dora_scale is not None,
-        )
-        module.lora_up.weight.data.copy_(up)
-        module.lora_down.weight.data.copy_(down)
-        if mid is not None:
-            module.lora_mid.weight.data.copy_(mid)
-        if dora_scale is not None:
-            module.dora_scale.copy_(dora_scale)
-    elif lyco_type == "hada":
-        w1a, w1b, w2a, w2b, t1, t2, alpha, dora_scale = params
-        module = LohaModule(
-            lora_name,
-            orig_module,
-            1,
-            w1b.size(0),
-            float(alpha),
-            use_tucker=t1 is not None,
-            weight_decompose=dora_scale is not None,
-        )
-        module.hada_w1_a.copy_(w1a)
-        module.hada_w1_b.copy_(w1b)
-        module.hada_w2_a.copy_(w2a)
-        module.hada_w2_b.copy_(w2b)
-        if t1 is not None:
-            module.hada_t1.copy_(t1)
-            module.hada_t2.copy_(t2)
-        if dora_scale is not None:
-            module.dora_scale.copy_(dora_scale)
-    elif lyco_type == "kron":
-        w1, w1a, w1b, w2, w2a, w2b, _, t2, alpha, dora_scale = params
-        if w1a is not None:
-            lora_dim = w1a.size(1)
-        elif w2a is not None:
-            lora_dim = w2a.size(1)
-        else:
-            lora_dim = 10000000000000
-
-        if w1 is None:
-            out_dim = w1a.size(0)
-            in_dim = w1b.size(1)
-        else:
-            out_dim, in_dim = w1.shape
-
-        shape_s = [out_dim, in_dim]
-
-        if w2 is None:
-            out_dim *= w2a.size(0)
-            in_dim *= w2b.size(1)
-        else:
-            out_dim *= w2.size(0)
-            in_dim *= w2.size(1)
-
-        if (
-            shape_s[0] == factorization(out_dim, -1)[0]
-            and shape_s[1] == factorization(in_dim, -1)[0]
-        ):
-            factor = -1
-        else:
-            factor = max(w1.shape) if w1 is not None else max(w1a.size(0), w1b.size(1))
-
-        module = LokrModule(
-            lora_name,
-            orig_module,
-            1,
-            lora_dim,
-            float(alpha),
-            use_tucker=t2 is not None,
-            decompose_both=w1 is None and w2 is None,
-            factor=factor,
-            weight_decompose=dora_scale is not None,
-        )
-        if w1 is not None:
-            module.lokr_w1.copy_(w1)
-        else:
-            module.lokr_w1_a.copy_(w1a)
-            module.lokr_w1_b.copy_(w1b)
-        if w2 is not None:
-            module.lokr_w2.copy_(w2)
-        else:
-            module.lokr_w2_a.copy_(w2a)
-            module.lokr_w2_b.copy_(w2b)
-        if t2 is not None:
-            module.lokr_t2.copy_(t2)
-        if dora_scale is not None:
-            module.dora_scale.copy_(dora_scale)
-    elif lyco_type == "norm":
-        w_norm, b_norm = params
-        module = NormModule(
-            lora_name,
-            orig_module,
-            1,
-        )
-        module.w_norm.copy_(w_norm)
-        if b_norm is not None:
-            module.b_norm.copy_(b_norm)
-    elif lyco_type == "full":
-        diff, diff_b = params
-        module = FullModule(
-            lora_name,
-            orig_module,
-            1,
-        )
-        module.diff.copy_(diff)
-        if diff_b is not None:
-            module.diff_b.copy_(diff_b)
-    elif lyco_type == "ia3":
-        pass
-    else:
-        return None
-
-    return module
+import torch
+
+from .full import FullModule
+from .norms import NormModule
+from .locon import LoConModule
+from .loha import LohaModule
+from .lokr import LokrModule, factorization
+from .ia3 import IA3Module
+
+
+@torch.no_grad()
+def make_module(lyco_type, params, lora_name, orig_module):
+    module = None
+    if lyco_type == "locon":
+        up, down, mid, alpha, dora_scale = params
+        module = LoConModule(
+            lora_name,
+            orig_module,
+            1,
+            down.size(0),
+            float(alpha),
+            use_tucker=mid is not None,
+            weight_decompose=dora_scale is not None,
+        )
+        module.lora_up.weight.data.copy_(up)
+        module.lora_down.weight.data.copy_(down)
+        if mid is not None:
+            module.lora_mid.weight.data.copy_(mid)
+        if dora_scale is not None:
+            module.dora_scale.copy_(dora_scale)
+    elif lyco_type == "hada":
+        w1a, w1b, w2a, w2b, t1, t2, alpha, dora_scale = params
+        module = LohaModule(
+            lora_name,
+            orig_module,
+            1,
+            w1b.size(0),
+            float(alpha),
+            use_tucker=t1 is not None,
+            weight_decompose=dora_scale is not None,
+        )
+        module.hada_w1_a.copy_(w1a)
+        module.hada_w1_b.copy_(w1b)
+        module.hada_w2_a.copy_(w2a)
+        module.hada_w2_b.copy_(w2b)
+        if t1 is not None:
+            module.hada_t1.copy_(t1)
+            module.hada_t2.copy_(t2)
+        if dora_scale is not None:
+            module.dora_scale.copy_(dora_scale)
+    elif lyco_type == "kron":
+        w1, w1a, w1b, w2, w2a, w2b, _, t2, alpha, dora_scale = params
+        if w1a is not None:
+            lora_dim = w1a.size(1)
+        elif w2a is not None:
+            lora_dim = w2a.size(1)
+        else:
+            lora_dim = 10000000000000
+
+        if w1 is None:
+            out_dim = w1a.size(0)
+            in_dim = w1b.size(1)
+        else:
+            out_dim, in_dim = w1.shape
+
+        shape_s = [out_dim, in_dim]
+
+        if w2 is None:
+            out_dim *= w2a.size(0)
+            in_dim *= w2b.size(1)
+        else:
+            out_dim *= w2.size(0)
+            in_dim *= w2.size(1)
+
+        if (
+            shape_s[0] == factorization(out_dim, -1)[0]
+            and shape_s[1] == factorization(in_dim, -1)[0]
+        ):
+            factor = -1
+        else:
+            factor = max(w1.shape) if w1 is not None else max(w1a.size(0), w1b.size(1))
+
+        module = LokrModule(
+            lora_name,
+            orig_module,
+            1,
+            lora_dim,
+            float(alpha),
+            use_tucker=t2 is not None,
+            decompose_both=w1 is None and w2 is None,
+            factor=factor,
+            weight_decompose=dora_scale is not None,
+        )
+        if w1 is not None:
+            module.lokr_w1.copy_(w1)
+        else:
+            module.lokr_w1_a.copy_(w1a)
+            module.lokr_w1_b.copy_(w1b)
+        if w2 is not None:
+            module.lokr_w2.copy_(w2)
+        else:
+            module.lokr_w2_a.copy_(w2a)
+            module.lokr_w2_b.copy_(w2b)
+        if t2 is not None:
+            module.lokr_t2.copy_(t2)
+        if dora_scale is not None:
+            module.dora_scale.copy_(dora_scale)
+    elif lyco_type == "norm":
+        w_norm, b_norm = params
+        module = NormModule(
+            lora_name,
+            orig_module,
+            1,
+        )
+        module.w_norm.copy_(w_norm)
+        if b_norm is not None:
+            module.b_norm.copy_(b_norm)
+    elif lyco_type == "full":
+        diff, diff_b = params
+        module = FullModule(
+            lora_name,
+            orig_module,
+            1,
+        )
+        module.diff.copy_(diff)
+        if diff_b is not None:
+            module.diff_b.copy_(diff_b)
+    elif lyco_type == "ia3":
+        pass
+    else:
+        return None
+
+    return module
```

### Comparing `lycoris_lora-2.3.0.dev4/lycoris/modules/attention.py` & `lycoris_lora-2.3.0.dev5/lycoris/modules/attention.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,259 +1,259 @@
-import math
-
-import torch
-import torch.nn as nn
-import torch.nn.functional as F
-
-from einops import rearrange, repeat
-
-from lycoris.utils import default
-from lycoris.utils.xformers_utils import XFORMERS_AVAIL, memory_efficient_attention
-
-
-class GEGLU(nn.Module):
-    def __init__(self, dim_in, dim_out):
-        super().__init__()
-        self.proj = nn.Linear(dim_in, dim_out * 2)
-
-    def forward(self, x):
-        x, gate = self.proj(x).chunk(2, dim=-1)
-        return x * F.gelu(gate)
-
-
-class FeedForward(nn.Module):
-    def __init__(self, dim, dim_out=None, mult=4, glu=False):
-        super().__init__()
-        inner_dim = int(dim * mult)
-        dim_out = default(dim_out, dim)
-        project_in = (
-            nn.Sequential(nn.Linear(dim, inner_dim), nn.GELU())
-            if not glu
-            else GEGLU(dim, inner_dim)
-        )
-
-        self.net = nn.Sequential(project_in, nn.Linear(inner_dim, dim_out))
-        # nn.init.constant_(self.net[-1].weight, 0)
-        # nn.init.constant_(self.net[-1].bias, 0)
-
-    def forward(self, x):
-        return self.net(x)
-
-
-def vanilla_attention(q, k, v, mask, scale=None):
-    if scale is None:
-        scale = math.sqrt(q.size(-1))
-    scores = torch.bmm(q, k.transpose(-1, -2)) / scale
-    if mask is not None:
-        mask = rearrange(mask, "b ... -> b (...)")
-        max_neg_value = -torch.finfo(scores.dtype).max
-        mask = repeat(mask, "b j -> (b h) j", h=q.size(-3))
-        scores = scores.masked_fill(~mask, max_neg_value)
-    p_attn = F.softmax(scores, dim=-1)
-    return torch.bmm(p_attn, v)
-
-
-MEMORY_LAYOUTS = {
-    "torch": (
-        "b n (h d) -> b h n d",
-        "b h n d -> b n (h d)",
-        lambda x: (1, x, 1, 1),
-    ),
-    "xformers": (
-        "b n (h d) -> b n h d",
-        "b n h d -> b n (h d)",
-        lambda x: (1, 1, x, 1),
-    ),
-    "vanilla": (
-        "b n (h d) -> b h n d",
-        "b h n d -> b n (h d)",
-        lambda x: (1, x, 1, 1),
-    ),
-}
-ATTN_FUNCTION = {
-    "vanilla": vanilla_attention,
-    "torch": getattr(F, "scaled_dot_product_attention", None),
-    "xformers": memory_efficient_attention,
-}
-
-
-class Attention(nn.Module):
-    """
-    Attention Class without norm and residual
-    (You need to wrap them by your self)
-    """
-
-    def __init__(
-        self,
-        in_ch,
-        context_ch=None,
-        heads=8,
-        head_ch=64,
-        self_cross=False,
-        double_attn=False,
-        single_kv_head=False,
-        attn_backend="torch",
-        cosine_attn=False,
-        qk_head_ch=-1,
-    ):
-        super().__init__()
-        if heads == -1:
-            assert in_ch % head_ch == 0
-            heads = in_ch // head_ch
-        if head_ch == -1:
-            assert in_ch % heads == 0
-            head_ch = in_ch // heads
-        if qk_head_ch == -1:
-            qk_head_ch = head_ch
-        q_ch = heads * qk_head_ch
-        k_ch = (1 if single_kv_head else heads) * qk_head_ch
-        v_ch = (1 if single_kv_head else heads) * head_ch
-        inner_ch = heads * head_ch
-        assert inner_ch == in_ch
-        use_context = context_ch is not None
-        context_ch = default(context_ch, in_ch)
-
-        if attn_backend == "xformers":
-            assert XFORMERS_AVAIL
-        if attn_backend == "torch":
-            assert torch.version.__version__ >= "2.0.0"
-
-        self.heads = heads
-        self.self_cross = self_cross
-        self.double_attn = double_attn
-        self.single_kv_head = single_kv_head
-        self.attn = ATTN_FUNCTION[attn_backend]
-        self.memory_layout = MEMORY_LAYOUTS[attn_backend]
-        self.cosine_attn = cosine_attn
-
-        if cosine_attn:
-            self.scale = nn.Parameter(
-                torch.ones(MEMORY_LAYOUTS[attn_backend][2](heads))
-            )
-        else:
-            self.scale = None
-
-        self.q = nn.Linear(in_ch, q_ch, bias=False)
-        if self_cross and use_context:
-            self.k = nn.Linear(in_ch, k_ch, bias=False)
-            self.v = nn.Linear(in_ch, v_ch, bias=False)
-            self.ck = nn.Linear(context_ch, k_ch, bias=False)
-            self.cv = nn.Linear(context_ch, v_ch, bias=False)
-        else:
-            assert double_attn == False
-            self.k = nn.Linear(context_ch, k_ch, bias=False)
-            self.v = nn.Linear(context_ch, v_ch, bias=False)
-
-        if double_attn:
-            self.out = nn.Linear(inner_ch * 2, in_ch)
-        else:
-            self.out = nn.Linear(inner_ch, in_ch)
-
-    def forward(self, x: torch.Tensor, context=None, mask=None):
-        # Input Projection
-        heads = self.heads
-        q = self.q(x)
-        ck = cv = None
-        if self.self_cross:
-            k = self.k(x)
-            v = self.v(x)
-            if context is not None:
-                ck = self.ck(context)
-                cv = self.cv(context)
-                if not self.double_attn:
-                    k = torch.concat([k, ck], dim=1)
-                    v = torch.concat([v, cv], dim=1)
-        else:
-            ctx = default(context, x)
-            k = self.k(ctx)
-            v = self.v(ctx)
-
-        # Rearrange for Attention
-        q = rearrange(q, self.memory_layout[0], h=heads)
-        if self.single_kv_head:
-            k = k.unsqueeze(1)
-            v = v.unsqueeze(1)
-
-            b, _, seq, _ = k.shape
-            k = k.expand(b, heads, seq, k.size(3))
-            v = v.expand(b, heads, seq, v.size(3))
-        else:
-            k = rearrange(k, self.memory_layout[0], h=heads)
-            v = rearrange(v, self.memory_layout[0], h=heads)
-
-        if self.cosine_attn:
-            q = (F.normalize(q, dim=-1) * math.sqrt(q.size(-1))).to(v.dtype)
-            k = (F.normalize(k, dim=-1) * self.scale).to(v.dtype)
-            if ck is not None and self.double_attn:
-                ck = (F.normalize(ck, dim=-1) * self.scale).to(v.dtype)
-
-        # Attention
-        out = self.attn(q.contiguous(), k.contiguous(), v.contiguous(), mask)
-        out = rearrange(out, self.memory_layout[1], h=heads)
-        if self.double_attn:
-            out2 = self.attn(q.contiguous(), ck.contiguous(), cv.contiguous(), mask)
-            out2 = rearrange(out2, self.memory_layout[1], h=heads)
-            out = torch.cat([out, out2], dim=-1)
-
-        # Output Projection
-        return self.out(out)
-
-
-class TransformerBlock(nn.Module):
-    def __init__(
-        self,
-        dim,
-        n_heads,
-        d_head,
-        context_dim=None,
-        gated_ff=True,
-        self_cross=False,
-        single_kv_head=False,
-        attn_backend="torch",
-        cosine_attn=False,
-        qk_head_ch=-1,
-        disable_self_attn=False,
-        single_attn=False,
-    ):
-        super().__init__()
-        self.single_attn = single_attn
-        self.disable_self_attn = disable_self_attn or single_attn
-
-        self.norm1 = nn.LayerNorm(dim)
-        self.attn1 = Attention(
-            dim,
-            context_dim if self.disable_self_attn else None,
-            n_heads,
-            d_head,
-            self_cross,
-            single_kv_head,
-            attn_backend,
-            cosine_attn,
-            qk_head_ch,
-        )
-        if not single_attn:
-            self.norm2 = nn.LayerNorm(dim)
-            self.attn2 = Attention(
-                dim,
-                context_dim,
-                n_heads,
-                d_head,
-                self_cross,
-                single_kv_head,
-                attn_backend,
-                cosine_attn,
-                qk_head_ch,
-            )
-        self.norm3 = nn.LayerNorm(dim)
-        self.ff = FeedForward(dim, glu=gated_ff)
-
-    def forward(self, x, context=None):
-        x = (
-            self.attn1(
-                self.norm1(x), context=context if self.disable_self_attn else None
-            )
-            + x
-        )
-        if not self.single_attn and (context is not None or self.attn2.self_cross):
-            x = self.attn2(self.norm2(x), context=context) + x
-        x = self.ff(self.norm3(x)) + x
-        return x
+import math
+
+import torch
+import torch.nn as nn
+import torch.nn.functional as F
+
+from einops import rearrange, repeat
+
+from lycoris.utils import default
+from lycoris.utils.xformers_utils import XFORMERS_AVAIL, memory_efficient_attention
+
+
+class GEGLU(nn.Module):
+    def __init__(self, dim_in, dim_out):
+        super().__init__()
+        self.proj = nn.Linear(dim_in, dim_out * 2)
+
+    def forward(self, x):
+        x, gate = self.proj(x).chunk(2, dim=-1)
+        return x * F.gelu(gate)
+
+
+class FeedForward(nn.Module):
+    def __init__(self, dim, dim_out=None, mult=4, glu=False):
+        super().__init__()
+        inner_dim = int(dim * mult)
+        dim_out = default(dim_out, dim)
+        project_in = (
+            nn.Sequential(nn.Linear(dim, inner_dim), nn.GELU())
+            if not glu
+            else GEGLU(dim, inner_dim)
+        )
+
+        self.net = nn.Sequential(project_in, nn.Linear(inner_dim, dim_out))
+        # nn.init.constant_(self.net[-1].weight, 0)
+        # nn.init.constant_(self.net[-1].bias, 0)
+
+    def forward(self, x):
+        return self.net(x)
+
+
+def vanilla_attention(q, k, v, mask, scale=None):
+    if scale is None:
+        scale = math.sqrt(q.size(-1))
+    scores = torch.bmm(q, k.transpose(-1, -2)) / scale
+    if mask is not None:
+        mask = rearrange(mask, "b ... -> b (...)")
+        max_neg_value = -torch.finfo(scores.dtype).max
+        mask = repeat(mask, "b j -> (b h) j", h=q.size(-3))
+        scores = scores.masked_fill(~mask, max_neg_value)
+    p_attn = F.softmax(scores, dim=-1)
+    return torch.bmm(p_attn, v)
+
+
+MEMORY_LAYOUTS = {
+    "torch": (
+        "b n (h d) -> b h n d",
+        "b h n d -> b n (h d)",
+        lambda x: (1, x, 1, 1),
+    ),
+    "xformers": (
+        "b n (h d) -> b n h d",
+        "b n h d -> b n (h d)",
+        lambda x: (1, 1, x, 1),
+    ),
+    "vanilla": (
+        "b n (h d) -> b h n d",
+        "b h n d -> b n (h d)",
+        lambda x: (1, x, 1, 1),
+    ),
+}
+ATTN_FUNCTION = {
+    "vanilla": vanilla_attention,
+    "torch": getattr(F, "scaled_dot_product_attention", None),
+    "xformers": memory_efficient_attention,
+}
+
+
+class Attention(nn.Module):
+    """
+    Attention Class without norm and residual
+    (You need to wrap them by your self)
+    """
+
+    def __init__(
+        self,
+        in_ch,
+        context_ch=None,
+        heads=8,
+        head_ch=64,
+        self_cross=False,
+        double_attn=False,
+        single_kv_head=False,
+        attn_backend="torch",
+        cosine_attn=False,
+        qk_head_ch=-1,
+    ):
+        super().__init__()
+        if heads == -1:
+            assert in_ch % head_ch == 0
+            heads = in_ch // head_ch
+        if head_ch == -1:
+            assert in_ch % heads == 0
+            head_ch = in_ch // heads
+        if qk_head_ch == -1:
+            qk_head_ch = head_ch
+        q_ch = heads * qk_head_ch
+        k_ch = (1 if single_kv_head else heads) * qk_head_ch
+        v_ch = (1 if single_kv_head else heads) * head_ch
+        inner_ch = heads * head_ch
+        assert inner_ch == in_ch
+        use_context = context_ch is not None
+        context_ch = default(context_ch, in_ch)
+
+        if attn_backend == "xformers":
+            assert XFORMERS_AVAIL
+        if attn_backend == "torch":
+            assert torch.version.__version__ >= "2.0.0"
+
+        self.heads = heads
+        self.self_cross = self_cross
+        self.double_attn = double_attn
+        self.single_kv_head = single_kv_head
+        self.attn = ATTN_FUNCTION[attn_backend]
+        self.memory_layout = MEMORY_LAYOUTS[attn_backend]
+        self.cosine_attn = cosine_attn
+
+        if cosine_attn:
+            self.scale = nn.Parameter(
+                torch.ones(MEMORY_LAYOUTS[attn_backend][2](heads))
+            )
+        else:
+            self.scale = None
+
+        self.q = nn.Linear(in_ch, q_ch, bias=False)
+        if self_cross and use_context:
+            self.k = nn.Linear(in_ch, k_ch, bias=False)
+            self.v = nn.Linear(in_ch, v_ch, bias=False)
+            self.ck = nn.Linear(context_ch, k_ch, bias=False)
+            self.cv = nn.Linear(context_ch, v_ch, bias=False)
+        else:
+            assert double_attn == False
+            self.k = nn.Linear(context_ch, k_ch, bias=False)
+            self.v = nn.Linear(context_ch, v_ch, bias=False)
+
+        if double_attn:
+            self.out = nn.Linear(inner_ch * 2, in_ch)
+        else:
+            self.out = nn.Linear(inner_ch, in_ch)
+
+    def forward(self, x: torch.Tensor, context=None, mask=None):
+        # Input Projection
+        heads = self.heads
+        q = self.q(x)
+        ck = cv = None
+        if self.self_cross:
+            k = self.k(x)
+            v = self.v(x)
+            if context is not None:
+                ck = self.ck(context)
+                cv = self.cv(context)
+                if not self.double_attn:
+                    k = torch.concat([k, ck], dim=1)
+                    v = torch.concat([v, cv], dim=1)
+        else:
+            ctx = default(context, x)
+            k = self.k(ctx)
+            v = self.v(ctx)
+
+        # Rearrange for Attention
+        q = rearrange(q, self.memory_layout[0], h=heads)
+        if self.single_kv_head:
+            k = k.unsqueeze(1)
+            v = v.unsqueeze(1)
+
+            b, _, seq, _ = k.shape
+            k = k.expand(b, heads, seq, k.size(3))
+            v = v.expand(b, heads, seq, v.size(3))
+        else:
+            k = rearrange(k, self.memory_layout[0], h=heads)
+            v = rearrange(v, self.memory_layout[0], h=heads)
+
+        if self.cosine_attn:
+            q = (F.normalize(q, dim=-1) * math.sqrt(q.size(-1))).to(v.dtype)
+            k = (F.normalize(k, dim=-1) * self.scale).to(v.dtype)
+            if ck is not None and self.double_attn:
+                ck = (F.normalize(ck, dim=-1) * self.scale).to(v.dtype)
+
+        # Attention
+        out = self.attn(q.contiguous(), k.contiguous(), v.contiguous(), mask)
+        out = rearrange(out, self.memory_layout[1], h=heads)
+        if self.double_attn:
+            out2 = self.attn(q.contiguous(), ck.contiguous(), cv.contiguous(), mask)
+            out2 = rearrange(out2, self.memory_layout[1], h=heads)
+            out = torch.cat([out, out2], dim=-1)
+
+        # Output Projection
+        return self.out(out)
+
+
+class TransformerBlock(nn.Module):
+    def __init__(
+        self,
+        dim,
+        n_heads,
+        d_head,
+        context_dim=None,
+        gated_ff=True,
+        self_cross=False,
+        single_kv_head=False,
+        attn_backend="torch",
+        cosine_attn=False,
+        qk_head_ch=-1,
+        disable_self_attn=False,
+        single_attn=False,
+    ):
+        super().__init__()
+        self.single_attn = single_attn
+        self.disable_self_attn = disable_self_attn or single_attn
+
+        self.norm1 = nn.LayerNorm(dim)
+        self.attn1 = Attention(
+            dim,
+            context_dim if self.disable_self_attn else None,
+            n_heads,
+            d_head,
+            self_cross,
+            single_kv_head,
+            attn_backend,
+            cosine_attn,
+            qk_head_ch,
+        )
+        if not single_attn:
+            self.norm2 = nn.LayerNorm(dim)
+            self.attn2 = Attention(
+                dim,
+                context_dim,
+                n_heads,
+                d_head,
+                self_cross,
+                single_kv_head,
+                attn_backend,
+                cosine_attn,
+                qk_head_ch,
+            )
+        self.norm3 = nn.LayerNorm(dim)
+        self.ff = FeedForward(dim, glu=gated_ff)
+
+    def forward(self, x, context=None):
+        x = (
+            self.attn1(
+                self.norm1(x), context=context if self.disable_self_attn else None
+            )
+            + x
+        )
+        if not self.single_attn and (context is not None or self.attn2.self_cross):
+            x = self.attn2(self.norm2(x), context=context) + x
+        x = self.ff(self.norm3(x)) + x
+        return x
```

### Comparing `lycoris_lora-2.3.0.dev4/lycoris/modules/base.py` & `lycoris_lora-2.3.0.dev5/lycoris/modules/base.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-from collections import OrderedDict
-import torch.nn as nn
-
-
-class ModuleCustomSD(nn.Module):
-    def __init__(self):
-        super().__init__()
-        self._register_load_state_dict_pre_hook(self.load_weight_prehook)
-        self.register_load_state_dict_post_hook(self.load_weight_hook)
-
-    def load_weight_prehook(
-        self,
-        state_dict,
-        prefix,
-        local_metadata,
-        strict,
-        missing_keys,
-        unexpected_keys,
-        error_msgs,
-    ):
-        pass
-
-    def load_weight_hook(self, module, incompatible_keys):
-        pass
-
-    def custom_state_dict(self):
-        return None
-
-    def state_dict(self, *args, destination=None, prefix="", keep_vars=False):
-        # TODO: Remove `args` and the parsing logic when BC allows.
-        if len(args) > 0:
-            if destination is None:
-                destination = args[0]
-            if len(args) > 1 and prefix == "":
-                prefix = args[1]
-            if len(args) > 2 and keep_vars is False:
-                keep_vars = args[2]
-            # DeprecationWarning is ignored by default
-
-        if destination is None:
-            destination = OrderedDict()
-            destination._metadata = OrderedDict()
-
-        local_metadata = dict(version=self._version)
-        if hasattr(destination, "_metadata"):
-            destination._metadata[prefix[:-1]] = local_metadata
-
-        if (custom_sd := self.custom_state_dict()) is not None:
-            for k, v in custom_sd.items():
-                destination[f"{prefix}{k}"] = v
-            return destination
-        else:
-            return super().state_dict(
-                *args, destination=destination, prefix=prefix, keep_vars=keep_vars
-            )
+from collections import OrderedDict
+import torch.nn as nn
+
+
+class ModuleCustomSD(nn.Module):
+    def __init__(self):
+        super().__init__()
+        self._register_load_state_dict_pre_hook(self.load_weight_prehook)
+        self.register_load_state_dict_post_hook(self.load_weight_hook)
+
+    def load_weight_prehook(
+        self,
+        state_dict,
+        prefix,
+        local_metadata,
+        strict,
+        missing_keys,
+        unexpected_keys,
+        error_msgs,
+    ):
+        pass
+
+    def load_weight_hook(self, module, incompatible_keys):
+        pass
+
+    def custom_state_dict(self):
+        return None
+
+    def state_dict(self, *args, destination=None, prefix="", keep_vars=False):
+        # TODO: Remove `args` and the parsing logic when BC allows.
+        if len(args) > 0:
+            if destination is None:
+                destination = args[0]
+            if len(args) > 1 and prefix == "":
+                prefix = args[1]
+            if len(args) > 2 and keep_vars is False:
+                keep_vars = args[2]
+            # DeprecationWarning is ignored by default
+
+        if destination is None:
+            destination = OrderedDict()
+            destination._metadata = OrderedDict()
+
+        local_metadata = dict(version=self._version)
+        if hasattr(destination, "_metadata"):
+            destination._metadata[prefix[:-1]] = local_metadata
+
+        if (custom_sd := self.custom_state_dict()) is not None:
+            for k, v in custom_sd.items():
+                destination[f"{prefix}{k}"] = v
+            return destination
+        else:
+            return super().state_dict(
+                *args, destination=destination, prefix=prefix, keep_vars=keep_vars
+            )
```

### Comparing `lycoris_lora-2.3.0.dev4/lycoris/modules/boft.py` & `lycoris_lora-2.3.0.dev5/lycoris/modules/boft.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,254 +1,254 @@
-from functools import cache
-from math import log2
-
-import torch
-import torch.nn as nn
-import torch.nn.functional as F
-
-from einops import rearrange
-
-from .base import ModuleCustomSD
-from ..logging import logger
-from ..utils.bnb import LinearNF4, QuantLinears, log_bypass
-
-
-@cache
-def log_butterfly_factorize(dim, factor, result):
-    logger.info(
-        f"Use BOFT({int(log2(result[1]))}, {result[0]//2})"
-        f" (equivalent to factor={result[0]}) "
-        f"for {dim=} and {factor=}"
-    )
-
-
-def butterfly_factor(dimension: int, factor: int = -1) -> tuple[int, int]:
-    """
-    m = 2k
-    n = 2**p
-    m*n = dim
-    """
-
-    # Find the first solution and check if it is even doable
-    m = n = 0
-    while m <= factor:
-        m += 2
-        while dimension % m != 0 and m < dimension:
-            m += 2
-        if m > factor:
-            break
-        if sum(int(i) for i in f"{dimension//m:b}") == 1:
-            n = dimension // m
-
-    if n == 0:
-        raise ValueError(
-            f"It is impossible to decompose {dimension} with factor {factor} under BOFT constrains."
-        )
-
-    log_butterfly_factorize(dimension, factor, (dimension // n, n))
-    return dimension // n, n
-
-
-class ButterflyOFTModule(ModuleCustomSD):
-    """
-    modifed from kohya-ss/sd-scripts/networks/lora:LoRAModule
-    """
-
-    def __init__(
-        self,
-        lora_name,
-        org_module: nn.Module,
-        multiplier=1.0,
-        lora_dim=4,
-        alpha=1,
-        dropout=0.0,
-        rank_dropout=0.0,
-        module_dropout=0.0,
-        use_tucker=False,
-        use_scalar=False,
-        rank_dropout_scale=False,
-        constrain=0,
-        rescaled=False,
-        bypass_mode=False,
-        **kwargs,
-    ):
-        """if alpha == 0 or None, alpha is rank (no scaling)."""
-        super().__init__()
-        self.lora_name = lora_name
-
-        if isinstance(org_module, nn.Linear):
-            self.op = F.linear
-            self.dim = org_module.out_features
-            self.kw_dict = {}
-        elif isinstance(org_module, nn.Conv2d):
-            self.op = F.conv2d
-            self.dim = org_module.out_channels
-            self.kw_dict = {
-                "stride": org_module.stride,
-                "padding": org_module.padding,
-                "dilation": org_module.dilation,
-                "groups": org_module.groups,
-            }
-        else:
-            raise NotImplementedError
-
-        if isinstance(org_module, QuantLinears):
-            if not bypass_mode:
-                log_bypass()
-            bypass_mode = True
-        self.bypass_mode = bypass_mode
-
-        out_dim = self.dim
-        b, m_exp = butterfly_factor(out_dim, lora_dim)
-        self.block_size = b
-        self.block_num = m_exp
-        # BOFT(m, b)
-        self.boft_b = b
-        self.boft_m = sum(int(i) for i in f"{m_exp-1:b}") + 1
-        # block_num > block_size
-        self.rescaled = rescaled
-        self.constrain = constrain * out_dim
-        self.register_buffer("alpha", torch.tensor(constrain))
-        self.oft_blocks = nn.Parameter(
-            torch.zeros(self.boft_m, self.block_num, self.block_size, self.block_size)
-        )
-        if rescaled:
-            self.rescale = nn.Parameter(
-                torch.ones(out_dim, *(1 for _ in range(org_module.weight.dim() - 1)))
-            )
-
-        self.rank_dropout = rank_dropout
-        self.rank_dropout_scale = rank_dropout_scale
-        self.module_dropout = module_dropout
-
-        self.multiplier = multiplier
-        self.org_module = [org_module]
-        self.org_forward = self.org_module[0].forward
-
-    @property
-    def I(self):
-        return torch.eye(self.block_size, device=next(self.parameters()).device)
-
-    def apply_to(self, **kwargs):
-        self.org_forward = self.org_module[0].forward
-        self.org_module[0].forward = self.forward
-
-    def restore(self):
-        self.org_module[0].forward = self.org_forward
-
-    def merge_to(self, multiplier=1.0):
-        weight = self.make_weight(scale=multiplier)
-        self.org_module[0].weight.data.copy_(weight)
-
-    def get_r(self):
-        I = self.I
-        # for Q = -Q^T
-        q = self.oft_blocks - self.oft_blocks.transpose(-1, -2)
-        normed_q = q
-        # Diag OFT style constrain
-        if self.constrain > 0:
-            q_norm = torch.norm(q) + 1e-8
-            if q_norm > self.constrain:
-                normed_q = q * self.constrain / q_norm
-        # use float() to prevent unsupported type
-        r = (I + normed_q) @ (I - normed_q).float().inverse()
-        return r
-
-    def make_weight(self, scale=1, device=None):
-        m = self.boft_m
-        b = self.boft_b
-        r_b = b // 2
-        r = self.get_r()
-        inp = self.org_module[0].weight.to(device, dtype=r.dtype)
-
-        for i in range(m):
-            bi = r[i]  # b_num, b_size, b_size
-            if i == 0:
-                # Apply multiplier/scale and rescale into first weight
-                bi = bi * scale + (1 - scale) * self.I
-                if self.rescaled:
-                    bi = bi * self.rescale
-            inp = rearrange(inp, "(c g k) ... -> (c k g) ...", g=2, k=2**i * r_b)
-            inp = rearrange(inp, "(d b) ... -> d b ...", b=b)
-            inp = torch.einsum("b i j, b j ... -> b i ...", bi, inp)
-            inp = rearrange(inp, "d b ... -> (d b) ...")
-            inp = rearrange(inp, "(c k g) ... -> (c g k) ...", g=2, k=2**i * r_b)
-
-        return inp
-
-    @torch.no_grad()
-    def apply_max_norm(self, max_norm, device=None):
-        orig_norm = self.oft_blocks.to(device).norm()
-        norm = torch.clamp(orig_norm, max_norm / 2)
-        desired = torch.clamp(norm, max=max_norm)
-        ratio = desired / norm
-
-        scaled = norm != desired
-        if scaled:
-            self.oft_blocks *= ratio
-
-        return scaled, orig_norm * ratio
-
-    def bypass_forward(self, x, scale=1):
-        m = self.boft_m
-        b = self.boft_b
-        r_b = b // 2
-        r = self.get_r()
-        inp = self.org_forward(x)
-
-        for i in range(m):
-            bi = r[i]  # b_num, b_size, b_size
-            if i == 0:
-                # Apply multiplier/scale and rescale into first weight
-                bi = bi * scale + (1 - scale) * self.I
-                if self.rescaled:
-                    bi = bi * self.rescale
-            inp = rearrange(inp, "... (c g k) ->... (c k g)", g=2, k=2**i * r_b)
-            inp = rearrange(inp, "... (d b) -> ... d b", b=b)
-            inp = torch.einsum("b i j, ... b j -> ... b i", bi, inp)
-            inp = rearrange(inp, "... d b -> ... (d b)")
-            inp = rearrange(inp, "... (c k g) -> ... (c g k)", g=2, k=2**i * r_b)
-
-        return inp
-
-    def forward(self, x):
-        if self.module_dropout and self.training:
-            if torch.rand(1) < self.module_dropout:
-                return self.org_forward(x)
-        scale = self.multiplier
-
-        if self.bypass_mode:
-            return self.bypass_forward(x, scale)
-        else:
-            w = self.make_weight(scale, x.device)
-            kw_dict = self.kw_dict | {"weight": w, "bias": self.org_module[0].bias}
-            return self.op(x, **kw_dict)
-
-
-if __name__ == "__main__":
-    base = nn.Linear(128, 128).cuda()
-    lokr = ButterflyOFTModule("test", base, 1, 4, 1, weight_decompose=True).cuda()
-    print(lokr)
-    test_input = torch.randn(1, 128).cuda()
-    test_output = lokr(test_input)
-    print(test_output.shape)
-    print(F.mse_loss(test_output, lokr.bypass_forward(test_input)))
-
-    base_4bit = LinearNF4(128, 128)
-    base_4bit.load_state_dict(base.state_dict())
-    base_4bit.cuda()
-    qlocon = ButterflyOFTModule(
-        "test", base_4bit, 1, 4, 1, weight_decompose=False
-    ).cuda()
-    print(qlocon)
-    test_input = torch.randn(1, 128).cuda()
-    test_output = qlocon(test_input)
-    print(test_output.shape)
-
-    base = nn.Conv2d(128, 128, 3, 1, 1)
-    lokr = ButterflyOFTModule(
-        "test", base, 1, 4, 1, weight_decompose=True, use_tucker=True
-    )
-    print(lokr)
-    test_input = torch.randn(1, 128, 16, 16)
-    test_output = lokr(test_input)
-    print(test_output.shape)
+from functools import cache
+from math import log2
+
+import torch
+import torch.nn as nn
+import torch.nn.functional as F
+
+from einops import rearrange
+
+from .base import ModuleCustomSD
+from ..logging import logger
+from ..utils.bnb import LinearNF4, QuantLinears, log_bypass
+
+
+@cache
+def log_butterfly_factorize(dim, factor, result):
+    logger.info(
+        f"Use BOFT({int(log2(result[1]))}, {result[0]//2})"
+        f" (equivalent to factor={result[0]}) "
+        f"for {dim=} and {factor=}"
+    )
+
+
+def butterfly_factor(dimension: int, factor: int = -1) -> tuple[int, int]:
+    """
+    m = 2k
+    n = 2**p
+    m*n = dim
+    """
+
+    # Find the first solution and check if it is even doable
+    m = n = 0
+    while m <= factor:
+        m += 2
+        while dimension % m != 0 and m < dimension:
+            m += 2
+        if m > factor:
+            break
+        if sum(int(i) for i in f"{dimension//m:b}") == 1:
+            n = dimension // m
+
+    if n == 0:
+        raise ValueError(
+            f"It is impossible to decompose {dimension} with factor {factor} under BOFT constrains."
+        )
+
+    log_butterfly_factorize(dimension, factor, (dimension // n, n))
+    return dimension // n, n
+
+
+class ButterflyOFTModule(ModuleCustomSD):
+    """
+    modifed from kohya-ss/sd-scripts/networks/lora:LoRAModule
+    """
+
+    def __init__(
+        self,
+        lora_name,
+        org_module: nn.Module,
+        multiplier=1.0,
+        lora_dim=4,
+        alpha=1,
+        dropout=0.0,
+        rank_dropout=0.0,
+        module_dropout=0.0,
+        use_tucker=False,
+        use_scalar=False,
+        rank_dropout_scale=False,
+        constrain=0,
+        rescaled=False,
+        bypass_mode=False,
+        **kwargs,
+    ):
+        """if alpha == 0 or None, alpha is rank (no scaling)."""
+        super().__init__()
+        self.lora_name = lora_name
+
+        if isinstance(org_module, nn.Linear):
+            self.op = F.linear
+            self.dim = org_module.out_features
+            self.kw_dict = {}
+        elif isinstance(org_module, nn.Conv2d):
+            self.op = F.conv2d
+            self.dim = org_module.out_channels
+            self.kw_dict = {
+                "stride": org_module.stride,
+                "padding": org_module.padding,
+                "dilation": org_module.dilation,
+                "groups": org_module.groups,
+            }
+        else:
+            raise NotImplementedError
+
+        if isinstance(org_module, QuantLinears):
+            if not bypass_mode:
+                log_bypass()
+            bypass_mode = True
+        self.bypass_mode = bypass_mode
+
+        out_dim = self.dim
+        b, m_exp = butterfly_factor(out_dim, lora_dim)
+        self.block_size = b
+        self.block_num = m_exp
+        # BOFT(m, b)
+        self.boft_b = b
+        self.boft_m = sum(int(i) for i in f"{m_exp-1:b}") + 1
+        # block_num > block_size
+        self.rescaled = rescaled
+        self.constrain = constrain * out_dim
+        self.register_buffer("alpha", torch.tensor(constrain))
+        self.oft_blocks = nn.Parameter(
+            torch.zeros(self.boft_m, self.block_num, self.block_size, self.block_size)
+        )
+        if rescaled:
+            self.rescale = nn.Parameter(
+                torch.ones(out_dim, *(1 for _ in range(org_module.weight.dim() - 1)))
+            )
+
+        self.rank_dropout = rank_dropout
+        self.rank_dropout_scale = rank_dropout_scale
+        self.module_dropout = module_dropout
+
+        self.multiplier = multiplier
+        self.org_module = [org_module]
+        self.org_forward = self.org_module[0].forward
+
+    @property
+    def I(self):
+        return torch.eye(self.block_size, device=next(self.parameters()).device)
+
+    def apply_to(self, **kwargs):
+        self.org_forward = self.org_module[0].forward
+        self.org_module[0].forward = self.forward
+
+    def restore(self):
+        self.org_module[0].forward = self.org_forward
+
+    def merge_to(self, multiplier=1.0):
+        weight = self.make_weight(scale=multiplier)
+        self.org_module[0].weight.data.copy_(weight)
+
+    def get_r(self):
+        I = self.I
+        # for Q = -Q^T
+        q = self.oft_blocks - self.oft_blocks.transpose(-1, -2)
+        normed_q = q
+        # Diag OFT style constrain
+        if self.constrain > 0:
+            q_norm = torch.norm(q) + 1e-8
+            if q_norm > self.constrain:
+                normed_q = q * self.constrain / q_norm
+        # use float() to prevent unsupported type
+        r = (I + normed_q) @ (I - normed_q).float().inverse()
+        return r
+
+    def make_weight(self, scale=1, device=None):
+        m = self.boft_m
+        b = self.boft_b
+        r_b = b // 2
+        r = self.get_r()
+        inp = self.org_module[0].weight.to(device, dtype=r.dtype)
+
+        for i in range(m):
+            bi = r[i]  # b_num, b_size, b_size
+            if i == 0:
+                # Apply multiplier/scale and rescale into first weight
+                bi = bi * scale + (1 - scale) * self.I
+                if self.rescaled:
+                    bi = bi * self.rescale
+            inp = rearrange(inp, "(c g k) ... -> (c k g) ...", g=2, k=2**i * r_b)
+            inp = rearrange(inp, "(d b) ... -> d b ...", b=b)
+            inp = torch.einsum("b i j, b j ... -> b i ...", bi, inp)
+            inp = rearrange(inp, "d b ... -> (d b) ...")
+            inp = rearrange(inp, "(c k g) ... -> (c g k) ...", g=2, k=2**i * r_b)
+
+        return inp
+
+    @torch.no_grad()
+    def apply_max_norm(self, max_norm, device=None):
+        orig_norm = self.oft_blocks.to(device).norm()
+        norm = torch.clamp(orig_norm, max_norm / 2)
+        desired = torch.clamp(norm, max=max_norm)
+        ratio = desired / norm
+
+        scaled = norm != desired
+        if scaled:
+            self.oft_blocks *= ratio
+
+        return scaled, orig_norm * ratio
+
+    def bypass_forward(self, x, scale=1):
+        m = self.boft_m
+        b = self.boft_b
+        r_b = b // 2
+        r = self.get_r()
+        inp = self.org_forward(x)
+
+        for i in range(m):
+            bi = r[i]  # b_num, b_size, b_size
+            if i == 0:
+                # Apply multiplier/scale and rescale into first weight
+                bi = bi * scale + (1 - scale) * self.I
+                if self.rescaled:
+                    bi = bi * self.rescale
+            inp = rearrange(inp, "... (c g k) ->... (c k g)", g=2, k=2**i * r_b)
+            inp = rearrange(inp, "... (d b) -> ... d b", b=b)
+            inp = torch.einsum("b i j, ... b j -> ... b i", bi, inp)
+            inp = rearrange(inp, "... d b -> ... (d b)")
+            inp = rearrange(inp, "... (c k g) -> ... (c g k)", g=2, k=2**i * r_b)
+
+        return inp
+
+    def forward(self, x):
+        if self.module_dropout and self.training:
+            if torch.rand(1) < self.module_dropout:
+                return self.org_forward(x)
+        scale = self.multiplier
+
+        if self.bypass_mode:
+            return self.bypass_forward(x, scale)
+        else:
+            w = self.make_weight(scale, x.device)
+            kw_dict = self.kw_dict | {"weight": w, "bias": self.org_module[0].bias}
+            return self.op(x, **kw_dict)
+
+
+if __name__ == "__main__":
+    base = nn.Linear(128, 128).cuda()
+    lokr = ButterflyOFTModule("test", base, 1, 4, 1, weight_decompose=True).cuda()
+    print(lokr)
+    test_input = torch.randn(1, 128).cuda()
+    test_output = lokr(test_input)
+    print(test_output.shape)
+    print(F.mse_loss(test_output, lokr.bypass_forward(test_input)))
+
+    base_4bit = LinearNF4(128, 128)
+    base_4bit.load_state_dict(base.state_dict())
+    base_4bit.cuda()
+    qlocon = ButterflyOFTModule(
+        "test", base_4bit, 1, 4, 1, weight_decompose=False
+    ).cuda()
+    print(qlocon)
+    test_input = torch.randn(1, 128).cuda()
+    test_output = qlocon(test_input)
+    print(test_output.shape)
+
+    base = nn.Conv2d(128, 128, 3, 1, 1)
+    lokr = ButterflyOFTModule(
+        "test", base, 1, 4, 1, weight_decompose=True, use_tucker=True
+    )
+    print(lokr)
+    test_input = torch.randn(1, 128, 16, 16)
+    test_output = lokr(test_input)
+    print(test_output.shape)
```

### Comparing `lycoris_lora-2.3.0.dev4/lycoris/modules/dylora.py` & `lycoris_lora-2.3.0.dev5/lycoris/modules/dylora.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,132 +1,132 @@
-import math
-import random
-
-import torch
-import torch.nn as nn
-import torch.nn.functional as F
-
-from .base import ModuleCustomSD
-
-
-class DyLoraModule(ModuleCustomSD):
-    """
-    Hadamard product Implementaion for Dynamic Low Rank adaptation
-    """
-
-    def __init__(
-        self,
-        lora_name,
-        org_module: nn.Module,
-        multiplier=1.0,
-        lora_dim=4,
-        alpha=1,
-        dropout=0.0,
-        rank_dropout=0.0,
-        module_dropout=0.0,
-        use_tucker=False,
-        block_size=1,
-        **kwargs,
-    ):
-        """if alpha == 0 or None, alpha is rank (no scaling)."""
-        super().__init__()
-        self.lora_name = lora_name
-        self.lora_dim = lora_dim
-        assert lora_dim % block_size == 0, "lora_dim must be a multiple of block_size"
-        self.block_count = lora_dim // block_size
-        self.block_size = block_size
-
-        self.shape = org_module.weight.shape
-        if org_module.__class__.__name__ == "Conv2d":
-            in_dim = org_module.in_channels
-            k_size = org_module.kernel_size
-            out_dim = org_module.out_channels
-            shape = (out_dim, in_dim * k_size[0] * k_size[1])
-            self.op = F.conv2d
-            self.extra_args = {
-                "stride": org_module.stride,
-                "padding": org_module.padding,
-                "dilation": org_module.dilation,
-                "groups": org_module.groups,
-            }
-        else:
-            in_dim = org_module.in_features
-            out_dim = org_module.out_features
-            shape = (out_dim, in_dim)
-            self.op = F.linear
-            self.extra_args = {}
-
-        self.lora_dim = lora_dim
-        self.up_list = nn.ParameterList(
-            [torch.empty(shape[0], 1) for i in range(lora_dim)]
-        )
-
-        self.down_list = nn.ParameterList(
-            [torch.empty(1, shape[1]) for i in range(lora_dim)]
-        )
-
-        self.index = 0
-
-        if type(alpha) == torch.Tensor:
-            alpha = alpha.detach().float().numpy()  # without casting, bf16 causes error
-        alpha = lora_dim if alpha is None or alpha == 0 else alpha
-        self.scale = alpha / self.lora_dim
-        self.register_buffer("alpha", torch.tensor(alpha))  # 定数として扱える
-
-        # Need more experiences on init method
-
-        for v in self.down_list:
-            torch.nn.init.kaiming_uniform_(v, a=math.sqrt(5))
-        for v in self.up_list:
-            torch.nn.init.zeros_(v)
-
-        self.multiplier = multiplier
-        self.org_module = [org_module]  # remove in applying
-        self.org_forward = self.org_module[0].forward
-        self.grad_ckpt = False
-        self.state_dict()
-
-    def custom_state_dict(self):
-        destination = {}
-        destination["alpha"] = self.alpha
-        destination["lora_up.weight"] = nn.Parameter(
-            torch.concat(list(self.up_list), dim=1)
-        )
-        destination["lora_down.weight"] = nn.Parameter(
-            torch.concat(list(self.down_list))
-        )
-        return destination
-
-    def apply_to(self):
-        self.org_module[0].forward = self.forward
-
-    def restore(self):
-        self.org_module[0].forward = self.org_forward
-
-    def merge_to(self, multiplier=1.0):
-        up = torch.concat(list(self.up_list), dim=1)
-        down = torch.concat(list(self.down_list))
-        diff_weight = up @ down * self.scale * multiplier / up.size(1)
-        self.org_module[0].weight.data.add_(diff_weight)
-
-    @torch.enable_grad()
-    def forward(self, x):
-        b = random.randint(0, self.block_count - 1)
-
-        down = torch.concat(
-            list(i.data for i in self.down_list[: b * self.block_size])
-            + list(self.down_list[b * self.block_size : (b + 1) * self.block_size])
-        )
-        up = torch.concat(
-            list(i.data for i in self.up_list[: b * self.block_size])
-            + list(self.up_list[b * self.block_size : (b + 1) * self.block_size]),
-            dim=1,
-        )
-
-        bias = None if self.org_module[0].bias is None else self.org_module[0].bias.data
-        return self.op(
-            x,
-            self.org_module[0].weight
-            + (up @ down).view(self.shape) * self.alpha / (b + 1),
-            bias,
-            **self.extra_args,
-        )
+import math
+import random
+
+import torch
+import torch.nn as nn
+import torch.nn.functional as F
+
+from .base import ModuleCustomSD
+
+
+class DyLoraModule(ModuleCustomSD):
+    """
+    Hadamard product Implementaion for Dynamic Low Rank adaptation
+    """
+
+    def __init__(
+        self,
+        lora_name,
+        org_module: nn.Module,
+        multiplier=1.0,
+        lora_dim=4,
+        alpha=1,
+        dropout=0.0,
+        rank_dropout=0.0,
+        module_dropout=0.0,
+        use_tucker=False,
+        block_size=1,
+        **kwargs,
+    ):
+        """if alpha == 0 or None, alpha is rank (no scaling)."""
+        super().__init__()
+        self.lora_name = lora_name
+        self.lora_dim = lora_dim
+        assert lora_dim % block_size == 0, "lora_dim must be a multiple of block_size"
+        self.block_count = lora_dim // block_size
+        self.block_size = block_size
+
+        self.shape = org_module.weight.shape
+        if org_module.__class__.__name__ == "Conv2d":
+            in_dim = org_module.in_channels
+            k_size = org_module.kernel_size
+            out_dim = org_module.out_channels
+            shape = (out_dim, in_dim * k_size[0] * k_size[1])
+            self.op = F.conv2d
+            self.extra_args = {
+                "stride": org_module.stride,
+                "padding": org_module.padding,
+                "dilation": org_module.dilation,
+                "groups": org_module.groups,
+            }
+        else:
+            in_dim = org_module.in_features
+            out_dim = org_module.out_features
+            shape = (out_dim, in_dim)
+            self.op = F.linear
+            self.extra_args = {}
+
+        self.lora_dim = lora_dim
+        self.up_list = nn.ParameterList(
+            [torch.empty(shape[0], 1) for i in range(lora_dim)]
+        )
+
+        self.down_list = nn.ParameterList(
+            [torch.empty(1, shape[1]) for i in range(lora_dim)]
+        )
+
+        self.index = 0
+
+        if type(alpha) == torch.Tensor:
+            alpha = alpha.detach().float().numpy()  # without casting, bf16 causes error
+        alpha = lora_dim if alpha is None or alpha == 0 else alpha
+        self.scale = alpha / self.lora_dim
+        self.register_buffer("alpha", torch.tensor(alpha))  # 定数として扱える
+
+        # Need more experiences on init method
+
+        for v in self.down_list:
+            torch.nn.init.kaiming_uniform_(v, a=math.sqrt(5))
+        for v in self.up_list:
+            torch.nn.init.zeros_(v)
+
+        self.multiplier = multiplier
+        self.org_module = [org_module]  # remove in applying
+        self.org_forward = self.org_module[0].forward
+        self.grad_ckpt = False
+        self.state_dict()
+
+    def custom_state_dict(self):
+        destination = {}
+        destination["alpha"] = self.alpha
+        destination["lora_up.weight"] = nn.Parameter(
+            torch.concat(list(self.up_list), dim=1)
+        )
+        destination["lora_down.weight"] = nn.Parameter(
+            torch.concat(list(self.down_list))
+        )
+        return destination
+
+    def apply_to(self):
+        self.org_module[0].forward = self.forward
+
+    def restore(self):
+        self.org_module[0].forward = self.org_forward
+
+    def merge_to(self, multiplier=1.0):
+        up = torch.concat(list(self.up_list), dim=1)
+        down = torch.concat(list(self.down_list))
+        diff_weight = up @ down * self.scale * multiplier / up.size(1)
+        self.org_module[0].weight.data.add_(diff_weight)
+
+    @torch.enable_grad()
+    def forward(self, x):
+        b = random.randint(0, self.block_count - 1)
+
+        down = torch.concat(
+            list(i.data for i in self.down_list[: b * self.block_size])
+            + list(self.down_list[b * self.block_size : (b + 1) * self.block_size])
+        )
+        up = torch.concat(
+            list(i.data for i in self.up_list[: b * self.block_size])
+            + list(self.up_list[b * self.block_size : (b + 1) * self.block_size]),
+            dim=1,
+        )
+
+        bias = None if self.org_module[0].bias is None else self.org_module[0].bias.data
+        return self.op(
+            x,
+            self.org_module[0].weight
+            + (up @ down).view(self.shape) * self.alpha / (b + 1),
+            bias,
+            **self.extra_args,
+        )
```

### Comparing `lycoris_lora-2.3.0.dev4/lycoris/modules/full.py` & `lycoris_lora-2.3.0.dev5/lycoris/modules/full.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,133 +1,133 @@
-import torch
-import torch.nn as nn
-import torch.nn.functional as F
-
-from .base import ModuleCustomSD
-
-
-class FullModule(ModuleCustomSD):
-    def __init__(
-        self,
-        lora_name,
-        org_module: nn.Module,
-        multiplier=1.0,
-        lora_dim=4,
-        alpha=1,
-        dropout=0.0,
-        rank_dropout=0.0,
-        module_dropout=0.0,
-        use_tucker=False,
-        use_scalar=False,
-        rank_dropout_scale=False,
-        **kwargs,
-    ):
-        super().__init__()
-        self.lora_name = lora_name
-
-        if isinstance(org_module, nn.Linear):
-            self.op = F.linear
-            self.dim = org_module.out_features
-            self.kw_dict = {}
-        elif isinstance(org_module, nn.Conv2d):
-            self.op = F.conv2d
-            self.dim = org_module.out_channels
-            self.kw_dict = {
-                "stride": org_module.stride,
-                "padding": org_module.padding,
-                "dilation": org_module.dilation,
-                "groups": org_module.groups,
-            }
-        else:
-            raise NotImplementedError
-        self.weight = nn.Parameter(torch.zeros_like(org_module.weight))
-        if org_module.bias is not None:
-            self.bias = nn.Parameter(torch.zeros_like(org_module.bias))
-        else:
-            self.bias = None
-
-        self.rank_dropout = rank_dropout
-        self.module_dropout = module_dropout
-
-        self.multiplier = multiplier
-        self.org_module = [org_module]
-
-    def apply_to(self, **kwargs):
-        self.org_forward = self.org_module[0].forward
-        self.org_module[0].forward = self.forward
-        self.weight.data.add_(self.org_module[0].weight.data)
-        self.org_weight = [self.org_module[0].weight.data.cpu().clone()]
-        delattr(self.org_module[0], "weight")
-        if self.org_module[0].bias is not None:
-            self.bias.data.add_(self.org_module[0].bias.data)
-            self.org_bias = [self.org_module[0].bias.data.cpu().clone()]
-            delattr(self.org_module[0], "bias")
-        else:
-            self.org_bias = None
-
-    def merge_to(self, multiplier=1.0):
-        weight, bias = self.make_weight(scale=multiplier)
-        self.org_module[0].weight.data.copy_(weight)
-        if bias is not None:
-            self.org_module[0].bias.data.copy_(bias)
-
-    def custom_state_dict(self):
-        sd = {"diff": self.weight.data.cpu() - self.org_weight[0]}
-        if self.bias is not None:
-            sd["diff_b"] = self.bias.data.cpu() - self.org_bias[0]
-        return sd
-
-    def load_weight_prehook(
-        self,
-        state_dict,
-        prefix,
-        local_metadata,
-        strict,
-        missing_keys,
-        unexpected_keys,
-        error_msgs,
-    ):
-        diff_weight = state_dict["diff"]
-        self.weight.data.add_(diff_weight)
-        if "diff_b" in state_dict:
-            diff_bias = state_dict["diff_b"]
-            self.bias.data.add_(diff_bias)
-
-    def make_weight(self, scale=1, device=None, original=False):
-        if original:
-            weight = self.org_weight[0].to(device, dtype=self.weight.dtype)
-            if self.org_bias is not None:
-                bias = self.org_bias[0].to(device, dtype=self.bias.dtype)
-            else:
-                bias = None
-            return weight, bias
-        drop = (
-            torch.rand(self.dim, device=device) > self.rank_dropout
-            if self.rank_dropout and self.training
-            else 1
-        )
-        if drop != 1 or scale != 1:
-            org_weight = self.org_module[0].weight.to(device, dtype=self.weight.dtype)
-            diff = self.weight.to(device) - org_weight
-            weight = diff * drop * scale + org_weight
-            if self.bias is not None:
-                org_bias = self.org_module[0].bias.to(device, dtype=self.bias.dtype)
-                diff_b = self.bias.to(device) - org_bias
-                bias = diff_b * drop * scale + org_bias
-        else:
-            weight = self.weight
-            bias = self.bias
-        return weight, bias
-
-    def forward(self, x: torch.Tensor):
-        if (
-            self.module_dropout
-            and self.training
-            and torch.rand(1) < self.module_dropout
-        ):
-            original = True
-        else:
-            original = False
-        scale = self.multiplier
-        weight, bias = self.make_weight(scale, x.device, original=original)
-        kw_dict = self.kw_dict | {"weight": weight, "bias": bias}
-        return self.op(x, **kw_dict)
+import torch
+import torch.nn as nn
+import torch.nn.functional as F
+
+from .base import ModuleCustomSD
+
+
+class FullModule(ModuleCustomSD):
+    def __init__(
+        self,
+        lora_name,
+        org_module: nn.Module,
+        multiplier=1.0,
+        lora_dim=4,
+        alpha=1,
+        dropout=0.0,
+        rank_dropout=0.0,
+        module_dropout=0.0,
+        use_tucker=False,
+        use_scalar=False,
+        rank_dropout_scale=False,
+        **kwargs,
+    ):
+        super().__init__()
+        self.lora_name = lora_name
+
+        if isinstance(org_module, nn.Linear):
+            self.op = F.linear
+            self.dim = org_module.out_features
+            self.kw_dict = {}
+        elif isinstance(org_module, nn.Conv2d):
+            self.op = F.conv2d
+            self.dim = org_module.out_channels
+            self.kw_dict = {
+                "stride": org_module.stride,
+                "padding": org_module.padding,
+                "dilation": org_module.dilation,
+                "groups": org_module.groups,
+            }
+        else:
+            raise NotImplementedError
+        self.weight = nn.Parameter(torch.zeros_like(org_module.weight))
+        if org_module.bias is not None:
+            self.bias = nn.Parameter(torch.zeros_like(org_module.bias))
+        else:
+            self.bias = None
+
+        self.rank_dropout = rank_dropout
+        self.module_dropout = module_dropout
+
+        self.multiplier = multiplier
+        self.org_module = [org_module]
+
+    def apply_to(self, **kwargs):
+        self.org_forward = self.org_module[0].forward
+        self.org_module[0].forward = self.forward
+        self.weight.data.add_(self.org_module[0].weight.data)
+        self.org_weight = [self.org_module[0].weight.data.cpu().clone()]
+        delattr(self.org_module[0], "weight")
+        if self.org_module[0].bias is not None:
+            self.bias.data.add_(self.org_module[0].bias.data)
+            self.org_bias = [self.org_module[0].bias.data.cpu().clone()]
+            delattr(self.org_module[0], "bias")
+        else:
+            self.org_bias = None
+
+    def merge_to(self, multiplier=1.0):
+        weight, bias = self.make_weight(scale=multiplier)
+        self.org_module[0].weight.data.copy_(weight)
+        if bias is not None:
+            self.org_module[0].bias.data.copy_(bias)
+
+    def custom_state_dict(self):
+        sd = {"diff": self.weight.data.cpu() - self.org_weight[0]}
+        if self.bias is not None:
+            sd["diff_b"] = self.bias.data.cpu() - self.org_bias[0]
+        return sd
+
+    def load_weight_prehook(
+        self,
+        state_dict,
+        prefix,
+        local_metadata,
+        strict,
+        missing_keys,
+        unexpected_keys,
+        error_msgs,
+    ):
+        diff_weight = state_dict["diff"]
+        self.weight.data.add_(diff_weight)
+        if "diff_b" in state_dict:
+            diff_bias = state_dict["diff_b"]
+            self.bias.data.add_(diff_bias)
+
+    def make_weight(self, scale=1, device=None, original=False):
+        if original:
+            weight = self.org_weight[0].to(device, dtype=self.weight.dtype)
+            if self.org_bias is not None:
+                bias = self.org_bias[0].to(device, dtype=self.bias.dtype)
+            else:
+                bias = None
+            return weight, bias
+        drop = (
+            torch.rand(self.dim, device=device) > self.rank_dropout
+            if self.rank_dropout and self.training
+            else 1
+        )
+        if drop != 1 or scale != 1:
+            org_weight = self.org_module[0].weight.to(device, dtype=self.weight.dtype)
+            diff = self.weight.to(device) - org_weight
+            weight = diff * drop * scale + org_weight
+            if self.bias is not None:
+                org_bias = self.org_module[0].bias.to(device, dtype=self.bias.dtype)
+                diff_b = self.bias.to(device) - org_bias
+                bias = diff_b * drop * scale + org_bias
+        else:
+            weight = self.weight
+            bias = self.bias
+        return weight, bias
+
+    def forward(self, x: torch.Tensor):
+        if (
+            self.module_dropout
+            and self.training
+            and torch.rand(1) < self.module_dropout
+        ):
+            original = True
+        else:
+            original = False
+        scale = self.multiplier
+        weight, bias = self.make_weight(scale, x.device, original=original)
+        kw_dict = self.kw_dict | {"weight": weight, "bias": bias}
+        return self.op(x, **kw_dict)
```

### Comparing `lycoris_lora-2.3.0.dev4/lycoris/modules/glokr.py` & `lycoris_lora-2.3.0.dev5/lycoris/modules/glokr.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,300 +1,310 @@
-import torch
-import torch.nn as nn
-import torch.nn.functional as F
-
-from .base import ModuleCustomSD
-
-
-def factorization(dimension: int, factor: int = -1) -> tuple[int, int]:
-    """
-    return a tuple of two value of input dimension decomposed by the number closest to factor
-    second value is higher or equal than first value.
-
-    In LoRA with Kroneckor Product, first value is a value for weight scale.
-    secon value is a value for weight.
-
-    Becuase of non-commutative property, A⊗B ≠ B⊗A. Meaning of two matrices is slightly different.
-
-    examples)
-    factor
-        -1               2                4               8               16               ...
-    127 -> 127, 1   127 -> 127, 1    127 -> 127, 1   127 -> 127, 1   127 -> 127, 1
-    128 -> 16, 8    128 -> 64, 2     128 -> 32, 4    128 -> 16, 8    128 -> 16, 8
-    250 -> 25, 10   250 -> 125, 2    250 -> 125, 2   250 -> 50, 5   250 -> 25, 10
-    360 -> 45, 8    360 -> 180, 2    360 -> 90, 4    360 -> 45, 8    360 -> 45, 8
-    512 -> 32, 16   512 -> 256, 2    512 -> 128, 4   512 -> 64, 8    512 -> 32, 16
-    1024 -> 32, 32  1024 -> 512, 2   1024 -> 256, 4  1024 -> 128, 8  1024 -> 64, 16
-    """
-
-    if factor > 0 and (dimension % factor) == 0:
-        m = factor
-        n = dimension // factor
-        return m, n
-    if factor == -1:
-        factor = dimension
-    m, n = 1, dimension
-    length = m + n
-    while m < n:
-        new_m = m + 1
-        while dimension % new_m != 0:
-            new_m += 1
-        new_n = dimension // new_m
-        if new_m + new_n > length or new_m > factor:
-            break
-        else:
-            m, n = new_m, new_n
-    if m > n:
-        n, m = m, n
-    return m, n
-
-
-def make_weight_tucker(t, wa, wb):
-    rebuild2 = torch.einsum("i j k l, i p, j r -> p r k l", t, wa, wb)  # [c, d, k1, k2]
-    return rebuild2
-
-
-def make_kron(w1, w2, scale):
-    if len(w2.shape) == 4:
-        w1 = w1.unsqueeze(2).unsqueeze(2)
-    w2 = w2.contiguous()
-    rebuild = torch.kron(w1, w2)
-
-    return rebuild * scale
-
-
-class LokrModule(ModuleCustomSD):
-    """
-    modifed from kohya-ss/sd-scripts/networks/lora:LoRAModule
-        and from KohakuBlueleaf/LyCORIS/lycoris:loha:LoHaModule
-        and from KohakuBlueleaf/LyCORIS/lycoris:locon:LoconModule
-    """
-
-    def __init__(
-        self,
-        lora_name,
-        org_module: nn.Module,
-        multiplier=1.0,
-        lora_dim=4,
-        alpha=1,
-        dropout=0.0,
-        rank_dropout=0.0,
-        module_dropout=0.0,
-        use_tucker=False,
-        decompose_both=False,
-        factor: int = -1,  # factorization factor
-        rank_dropout_scale=False,
-        **kwargs,
-    ):
-        """if alpha == 0 or None, alpha is rank (no scaling)."""
-        super().__init__()
-        factor = int(factor)
-        self.lora_name = lora_name
-        self.lora_dim = lora_dim
-        self.tucker = False
-        self.use_w1 = False
-        self.use_w2 = False
-
-        self.shape = org_module.weight.shape
-        if org_module.__class__.__name__ == "Conv2d":
-            in_dim = org_module.in_channels
-            k_size = org_module.kernel_size
-            out_dim = org_module.out_channels
-
-            in_m, in_n = factorization(in_dim, factor)
-            out_l, out_k = factorization(out_dim, factor)
-            shape = ((out_l, out_k), (in_m, in_n), *k_size)  # ((a, b), (c, d), *k_size)
-
-            self.tucker = use_tucker and k_size != (1, 1)
-            if decompose_both and lora_dim < max(shape[0][0], shape[1][0]) / 2:
-                self.lokr_w1_a = nn.Parameter(torch.empty(shape[0][0], lora_dim))
-                self.lokr_w1_b = nn.Parameter(torch.empty(lora_dim, shape[1][0]))
-            else:
-                self.use_w1 = True
-                self.lokr_w1 = nn.Parameter(
-                    torch.empty(shape[0][0], shape[1][0])
-                )  # a*c, 1-mode
-
-            if lora_dim >= max(shape[0][1], shape[1][1]) / 2:
-                self.use_w2 = True
-                self.lokr_w2 = nn.Parameter(
-                    torch.empty(shape[0][1], shape[1][1], *k_size)
-                )
-            elif self.tucker:
-                self.lokr_t2 = nn.Parameter(
-                    torch.empty(lora_dim, lora_dim, shape[2], shape[3])
-                )
-                self.lokr_w2_a = nn.Parameter(
-                    torch.empty(lora_dim, shape[0][1])
-                )  # b, 1-mode
-                self.lokr_w2_b = nn.Parameter(
-                    torch.empty(lora_dim, shape[1][1])
-                )  # d, 2-mode
-            else:  # Conv2d not cp
-                # bigger part. weight and LoRA. [b, dim] x [dim, d*k1*k2]
-                self.lokr_w2_a = nn.Parameter(torch.empty(shape[0][1], lora_dim))
-                self.lokr_w2_b = nn.Parameter(
-                    torch.empty(lora_dim, shape[1][1] * shape[2] * shape[3])
-                )
-                # w1 ⊗ (w2_a x w2_b) = (a, b)⊗((c, dim)x(dim, d*k1*k2)) = (a, b)⊗(c, d*k1*k2) = (ac, bd*k1*k2)
-
-            self.op = F.conv2d
-            self.extra_args = {
-                "stride": org_module.stride,
-                "padding": org_module.padding,
-                "dilation": org_module.dilation,
-                "groups": org_module.groups,
-            }
-
-        else:  # Linear
-            in_dim = org_module.in_features
-            out_dim = org_module.out_features
-
-            in_m, in_n = factorization(in_dim, factor)
-            out_l, out_k = factorization(out_dim, factor)
-            shape = (
-                (out_l, out_k),
-                (in_m, in_n),
-            )  # ((a, b), (c, d)), out_dim = a*c, in_dim = b*d
-
-            # smaller part. weight scale
-            if decompose_both and lora_dim < max(shape[0][0], shape[1][0]) / 2:
-                self.lokr_w1_a = nn.Parameter(torch.empty(shape[0][0], lora_dim))
-                self.lokr_w1_b = nn.Parameter(torch.empty(lora_dim, shape[1][0]))
-            else:
-                self.use_w1 = True
-                self.lokr_w1 = nn.Parameter(
-                    torch.empty(shape[0][0], shape[1][0])
-                )  # a*c, 1-mode
-
-            if lora_dim < max(shape[0][1], shape[1][1]) / 2:
-                # bigger part. weight and LoRA. [b, dim] x [dim, d]
-                self.lokr_w2_a = nn.Parameter(torch.empty(shape[0][1], lora_dim))
-                self.lokr_w2_b = nn.Parameter(torch.empty(lora_dim, shape[1][1]))
-                # w1 ⊗ (w2_a x w2_b) = (a, b)⊗((c, dim)x(dim, d)) = (a, b)⊗(c, d) = (ac, bd)
-            else:
-                self.use_w2 = True
-                self.lokr_w2 = nn.Parameter(torch.empty(shape[0][1], shape[1][1]))
-
-            self.op = F.linear
-            self.extra_args = {}
-
-        self.dropout = dropout
-        if dropout:
-            print("[WARN]LoHa/LoKr haven't implemented normal dropout yet.")
-        self.rank_dropout = rank_dropout
-        self.rank_dropout_scale = rank_dropout_scale
-        self.module_dropout = module_dropout
-
-        if isinstance(alpha, torch.Tensor):
-            alpha = alpha.detach().float().numpy()  # without casting, bf16 causes error
-        alpha = lora_dim if alpha is None or alpha == 0 else alpha
-        if self.use_w2 and self.use_w1:
-            # use scale = 1
-            alpha = lora_dim
-        self.scale = alpha / self.lora_dim
-        self.register_buffer("alpha", torch.tensor(alpha))  # 定数として扱える
-
-        if self.use_w2:
-            torch.nn.init.constant_(self.lokr_w2, 0)
-        else:
-            if self.tucker:
-                torch.nn.init.normal_(self.lokr_t2, std=0.1)
-            torch.nn.init.normal_(self.lokr_w2_a, std=1)
-            torch.nn.init.constant_(self.lokr_w2_b, 0)
-
-        if self.use_w1:
-            torch.nn.init.normal_(self.lokr_w1, std=1)
-        else:
-            torch.nn.init.normal_(self.lokr_w1_a, std=1)
-            torch.nn.init.normal_(self.lokr_w1_b, std=0.1)
-
-        self.multiplier = multiplier
-        self.org_module = [org_module]
-        weight = make_kron(
-            self.lokr_w1 if self.use_w1 else self.lokr_w1_a @ self.lokr_w1_b,
-            (
-                self.lokr_w2
-                if self.use_w2
-                else (
-                    make_weight_tucker(self.lokr_t2, self.lokr_w2_a, self.lokr_w2_b)
-                    if self.tucker
-                    else self.lokr_w2_a @ self.lokr_w2_b
-                )
-            ),
-            torch.tensor(self.multiplier * self.scale),
-        )
-        assert torch.sum(torch.isnan(weight)) == 0, "weight is nan"
-
-    # Same as locon.py
-    def apply_to(self):
-        self.org_forward = self.org_module[0].forward
-        self.org_module[0].forward = self.forward
-
-    def get_weight(self, orig_weight=None):
-        weight = make_kron(
-            self.lokr_w1 if self.use_w1 else self.lokr_w1_a @ self.lokr_w1_b,
-            (
-                self.lokr_w2
-                if self.use_w2
-                else (
-                    make_weight_tucker(self.lokr_t2, self.lokr_w2_a, self.lokr_w2_b)
-                    if self.tucker
-                    else self.lokr_w2_a @ self.lokr_w2_b
-                )
-            ),
-            torch.tensor(self.scale),
-        )
-        if orig_weight is not None:
-            weight = weight.reshape(orig_weight.shape)
-        if self.training and self.rank_dropout:
-            drop = (torch.rand(weight.size(0)) < self.rank_dropout).to(weight.dtype)
-            drop = drop.view(-1, *[1] * len(weight.shape[1:])).to(weight.device)
-            if self.rank_dropout_scale:
-                drop /= drop.mean()
-            weight *= drop
-        return weight
-
-    @torch.no_grad()
-    def apply_max_norm(self, max_norm, device=None):
-        orig_norm = self.get_weight().norm()
-        norm = torch.clamp(orig_norm, max_norm / 2)
-        desired = torch.clamp(norm, max=max_norm)
-        ratio = desired.cpu() / norm.cpu()
-
-        scaled = norm != desired
-        if scaled:
-            modules = 4 - self.use_w1 - self.use_w2 + (not self.use_w2 and self.tucker)
-            if self.use_w1:
-                self.lokr_w1 *= ratio ** (1 / modules)
-            else:
-                self.lokr_w1_a *= ratio ** (1 / modules)
-                self.lokr_w1_b *= ratio ** (1 / modules)
-
-            if self.use_w2:
-                self.lokr_w2 *= ratio ** (1 / modules)
-            else:
-                if self.tucker:
-                    self.lokr_t2 *= ratio ** (1 / modules)
-                self.lokr_w2_a *= ratio ** (1 / modules)
-                self.lokr_w2_b *= ratio ** (1 / modules)
-
-        return scaled, orig_norm * ratio
-
-    def forward(self, x):
-        if self.module_dropout and self.training:
-            if torch.rand(1) < self.module_dropout:
-                return self.op(
-                    x,
-                    self.org_module[0].weight.data,
-                    (
-                        None
-                        if self.org_module[0].bias is None
-                        else self.org_module[0].bias.data
-                    ),
-                )
-        weight = (
-            self.org_module[0].weight.data
-            + self.get_weight(self.org_module[0].weight.data) * self.multiplier
-        )
-        bias = None if self.org_module[0].bias is None else self.org_module[0].bias.data
-        return self.op(x, weight.view(self.shape), bias, **self.extra_args)
+import math
+
+import torch
+import torch.nn as nn
+import torch.nn.functional as F
+
+from .base import ModuleCustomSD
+
+
+def factorization(dimension: int, factor: int = -1) -> tuple[int, int]:
+    """
+    return a tuple of two value of input dimension decomposed by the number closest to factor
+    second value is higher or equal than first value.
+
+    In LoRA with Kroneckor Product, first value is a value for weight scale.
+    secon value is a value for weight.
+
+    Becuase of non-commutative property, A⊗B ≠ B⊗A. Meaning of two matrices is slightly different.
+
+    examples)
+    factor
+        -1               2                4               8               16               ...
+    127 -> 127, 1   127 -> 127, 1    127 -> 127, 1   127 -> 127, 1   127 -> 127, 1
+    128 -> 16, 8    128 -> 64, 2     128 -> 32, 4    128 -> 16, 8    128 -> 16, 8
+    250 -> 25, 10   250 -> 125, 2    250 -> 125, 2   250 -> 50, 5   250 -> 25, 10
+    360 -> 45, 8    360 -> 180, 2    360 -> 90, 4    360 -> 45, 8    360 -> 45, 8
+    512 -> 32, 16   512 -> 256, 2    512 -> 128, 4   512 -> 64, 8    512 -> 32, 16
+    1024 -> 32, 32  1024 -> 512, 2   1024 -> 256, 4  1024 -> 128, 8  1024 -> 64, 16
+    """
+
+    if factor > 0 and (dimension % factor) == 0:
+        m = factor
+        n = dimension // factor
+        return m, n
+    if factor == -1:
+        factor = dimension
+    m, n = 1, dimension
+    length = m + n
+    while m < n:
+        new_m = m + 1
+        while dimension % new_m != 0:
+            new_m += 1
+        new_n = dimension // new_m
+        if new_m + new_n > length or new_m > factor:
+            break
+        else:
+            m, n = new_m, new_n
+    if m > n:
+        n, m = m, n
+    return m, n
+
+
+def make_weight_tucker(t, wa, wb):
+    rebuild2 = torch.einsum("i j k l, i p, j r -> p r k l", t, wa, wb)  # [c, d, k1, k2]
+    return rebuild2
+
+
+def make_kron(w1, w2, scale):
+    if len(w2.shape) == 4:
+        w1 = w1.unsqueeze(2).unsqueeze(2)
+    w2 = w2.contiguous()
+    rebuild = torch.kron(w1, w2)
+
+    return rebuild * scale
+
+
+class LokrModule(ModuleCustomSD):
+    """
+    modifed from kohya-ss/sd-scripts/networks/lora:LoRAModule
+        and from KohakuBlueleaf/LyCORIS/lycoris:loha:LoHaModule
+        and from KohakuBlueleaf/LyCORIS/lycoris:locon:LoconModule
+    """
+
+    def __init__(
+        self,
+        lora_name,
+        org_module: nn.Module,
+        multiplier=1.0,
+        lora_dim=4,
+        alpha=1,
+        dropout=0.0,
+        rank_dropout=0.0,
+        module_dropout=0.0,
+        use_tucker=False,
+        decompose_both=False,
+        factor: int = -1,  # factorization factor
+        rank_dropout_scale=False,
+        rs_lora=False,
+        **kwargs,
+    ):
+        """if alpha == 0 or None, alpha is rank (no scaling)."""
+        super().__init__()
+        factor = int(factor)
+        self.lora_name = lora_name
+        self.lora_dim = lora_dim
+        self.tucker = False
+        self.use_w1 = False
+        self.use_w2 = False
+        self.rs_lora = rs_lora
+
+        self.shape = org_module.weight.shape
+        if org_module.__class__.__name__ == "Conv2d":
+            in_dim = org_module.in_channels
+            k_size = org_module.kernel_size
+            out_dim = org_module.out_channels
+
+            in_m, in_n = factorization(in_dim, factor)
+            out_l, out_k = factorization(out_dim, factor)
+            shape = ((out_l, out_k), (in_m, in_n), *k_size)  # ((a, b), (c, d), *k_size)
+
+            self.tucker = use_tucker and k_size != (1, 1)
+            if decompose_both and lora_dim < max(shape[0][0], shape[1][0]) / 2:
+                self.lokr_w1_a = nn.Parameter(torch.empty(shape[0][0], lora_dim))
+                self.lokr_w1_b = nn.Parameter(torch.empty(lora_dim, shape[1][0]))
+            else:
+                self.use_w1 = True
+                self.lokr_w1 = nn.Parameter(
+                    torch.empty(shape[0][0], shape[1][0])
+                )  # a*c, 1-mode
+
+            if lora_dim >= max(shape[0][1], shape[1][1]) / 2:
+                self.use_w2 = True
+                self.lokr_w2 = nn.Parameter(
+                    torch.empty(shape[0][1], shape[1][1], *k_size)
+                )
+            elif self.tucker:
+                self.lokr_t2 = nn.Parameter(
+                    torch.empty(lora_dim, lora_dim, shape[2], shape[3])
+                )
+                self.lokr_w2_a = nn.Parameter(
+                    torch.empty(lora_dim, shape[0][1])
+                )  # b, 1-mode
+                self.lokr_w2_b = nn.Parameter(
+                    torch.empty(lora_dim, shape[1][1])
+                )  # d, 2-mode
+            else:  # Conv2d not cp
+                # bigger part. weight and LoRA. [b, dim] x [dim, d*k1*k2]
+                self.lokr_w2_a = nn.Parameter(torch.empty(shape[0][1], lora_dim))
+                self.lokr_w2_b = nn.Parameter(
+                    torch.empty(lora_dim, shape[1][1] * shape[2] * shape[3])
+                )
+                # w1 ⊗ (w2_a x w2_b) = (a, b)⊗((c, dim)x(dim, d*k1*k2)) = (a, b)⊗(c, d*k1*k2) = (ac, bd*k1*k2)
+
+            self.op = F.conv2d
+            self.extra_args = {
+                "stride": org_module.stride,
+                "padding": org_module.padding,
+                "dilation": org_module.dilation,
+                "groups": org_module.groups,
+            }
+
+        else:  # Linear
+            in_dim = org_module.in_features
+            out_dim = org_module.out_features
+
+            in_m, in_n = factorization(in_dim, factor)
+            out_l, out_k = factorization(out_dim, factor)
+            shape = (
+                (out_l, out_k),
+                (in_m, in_n),
+            )  # ((a, b), (c, d)), out_dim = a*c, in_dim = b*d
+
+            # smaller part. weight scale
+            if decompose_both and lora_dim < max(shape[0][0], shape[1][0]) / 2:
+                self.lokr_w1_a = nn.Parameter(torch.empty(shape[0][0], lora_dim))
+                self.lokr_w1_b = nn.Parameter(torch.empty(lora_dim, shape[1][0]))
+            else:
+                self.use_w1 = True
+                self.lokr_w1 = nn.Parameter(
+                    torch.empty(shape[0][0], shape[1][0])
+                )  # a*c, 1-mode
+
+            if lora_dim < max(shape[0][1], shape[1][1]) / 2:
+                # bigger part. weight and LoRA. [b, dim] x [dim, d]
+                self.lokr_w2_a = nn.Parameter(torch.empty(shape[0][1], lora_dim))
+                self.lokr_w2_b = nn.Parameter(torch.empty(lora_dim, shape[1][1]))
+                # w1 ⊗ (w2_a x w2_b) = (a, b)⊗((c, dim)x(dim, d)) = (a, b)⊗(c, d) = (ac, bd)
+            else:
+                self.use_w2 = True
+                self.lokr_w2 = nn.Parameter(torch.empty(shape[0][1], shape[1][1]))
+
+            self.op = F.linear
+            self.extra_args = {}
+
+        self.dropout = dropout
+        if dropout:
+            print("[WARN]LoHa/LoKr haven't implemented normal dropout yet.")
+        self.rank_dropout = rank_dropout
+        self.rank_dropout_scale = rank_dropout_scale
+        self.module_dropout = module_dropout
+
+        if isinstance(alpha, torch.Tensor):
+            alpha = alpha.detach().float().numpy()  # without casting, bf16 causes error
+        alpha = lora_dim if alpha is None or alpha == 0 else alpha
+        if self.use_w2 and self.use_w1:
+            # use scale = 1
+            alpha = lora_dim
+        
+        r_factor = lora_dim
+        if self.rs_lora:
+            r_factor = math.sqrt(r_factor)
+
+        self.scale = alpha / r_factor
+
+        self.register_buffer("alpha", torch.tensor(alpha))  # 定数として扱える
+
+        if self.use_w2:
+            torch.nn.init.constant_(self.lokr_w2, 0)
+        else:
+            if self.tucker:
+                torch.nn.init.normal_(self.lokr_t2, std=0.1)
+            torch.nn.init.normal_(self.lokr_w2_a, std=1)
+            torch.nn.init.constant_(self.lokr_w2_b, 0)
+
+        if self.use_w1:
+            torch.nn.init.normal_(self.lokr_w1, std=1)
+        else:
+            torch.nn.init.normal_(self.lokr_w1_a, std=1)
+            torch.nn.init.normal_(self.lokr_w1_b, std=0.1)
+
+        self.multiplier = multiplier
+        self.org_module = [org_module]
+        weight = make_kron(
+            self.lokr_w1 if self.use_w1 else self.lokr_w1_a @ self.lokr_w1_b,
+            (
+                self.lokr_w2
+                if self.use_w2
+                else (
+                    make_weight_tucker(self.lokr_t2, self.lokr_w2_a, self.lokr_w2_b)
+                    if self.tucker
+                    else self.lokr_w2_a @ self.lokr_w2_b
+                )
+            ),
+            torch.tensor(self.multiplier * self.scale),
+        )
+        assert torch.sum(torch.isnan(weight)) == 0, "weight is nan"
+
+    # Same as locon.py
+    def apply_to(self):
+        self.org_forward = self.org_module[0].forward
+        self.org_module[0].forward = self.forward
+
+    def get_weight(self, orig_weight=None):
+        weight = make_kron(
+            self.lokr_w1 if self.use_w1 else self.lokr_w1_a @ self.lokr_w1_b,
+            (
+                self.lokr_w2
+                if self.use_w2
+                else (
+                    make_weight_tucker(self.lokr_t2, self.lokr_w2_a, self.lokr_w2_b)
+                    if self.tucker
+                    else self.lokr_w2_a @ self.lokr_w2_b
+                )
+            ),
+            torch.tensor(self.scale),
+        )
+        if orig_weight is not None:
+            weight = weight.reshape(orig_weight.shape)
+        if self.training and self.rank_dropout:
+            drop = (torch.rand(weight.size(0)) < self.rank_dropout).to(weight.dtype)
+            drop = drop.view(-1, *[1] * len(weight.shape[1:])).to(weight.device)
+            if self.rank_dropout_scale:
+                drop /= drop.mean()
+            weight *= drop
+        return weight
+
+    @torch.no_grad()
+    def apply_max_norm(self, max_norm, device=None):
+        orig_norm = self.get_weight().norm()
+        norm = torch.clamp(orig_norm, max_norm / 2)
+        desired = torch.clamp(norm, max=max_norm)
+        ratio = desired.cpu() / norm.cpu()
+
+        scaled = norm != desired
+        if scaled:
+            modules = 4 - self.use_w1 - self.use_w2 + (not self.use_w2 and self.tucker)
+            if self.use_w1:
+                self.lokr_w1 *= ratio ** (1 / modules)
+            else:
+                self.lokr_w1_a *= ratio ** (1 / modules)
+                self.lokr_w1_b *= ratio ** (1 / modules)
+
+            if self.use_w2:
+                self.lokr_w2 *= ratio ** (1 / modules)
+            else:
+                if self.tucker:
+                    self.lokr_t2 *= ratio ** (1 / modules)
+                self.lokr_w2_a *= ratio ** (1 / modules)
+                self.lokr_w2_b *= ratio ** (1 / modules)
+
+        return scaled, orig_norm * ratio
+
+    def forward(self, x):
+        if self.module_dropout and self.training:
+            if torch.rand(1) < self.module_dropout:
+                return self.op(
+                    x,
+                    self.org_module[0].weight.data,
+                    (
+                        None
+                        if self.org_module[0].bias is None
+                        else self.org_module[0].bias.data
+                    ),
+                )
+        weight = (
+            self.org_module[0].weight.data
+            + self.get_weight(self.org_module[0].weight.data) * self.multiplier
+        )
+        bias = None if self.org_module[0].bias is None else self.org_module[0].bias.data
+        return self.op(x, weight.view(self.shape), bias, **self.extra_args)
```

### Comparing `lycoris_lora-2.3.0.dev4/lycoris/modules/glora.py` & `lycoris_lora-2.3.0.dev5/lycoris/modules/glora.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,128 +1,136 @@
-import math
-
-import torch
-import torch.nn as nn
-
-from .base import ModuleCustomSD
-
-
-class GLoRAModule(ModuleCustomSD):
-    """
-    modifed from kohya-ss/sd-scripts/networks/lora:LoRAModule
-    """
-
-    def __init__(
-        self,
-        lora_name,
-        org_module: nn.Module,
-        multiplier=1.0,
-        lora_dim=4,
-        alpha=1,
-        dropout=0.0,
-        rank_dropout=0.0,
-        module_dropout=0.0,
-        rank_dropout_scale=False,
-        *args,
-        **kwargs,
-    ):
-        """if alpha == 0 or None, alpha is rank (no scaling)."""
-        super().__init__()
-        self.lora_name = lora_name
-        self.lora_dim = lora_dim
-        self.tucker = False
-
-        if isinstance(org_module, nn.Conv2d):
-            assert org_module.kernel_size == (1, 1)
-            in_dim = org_module.in_channels
-            out_dim = org_module.out_channels
-            self.a1 = nn.Conv2d(in_dim, lora_dim, (1, 1), bias=False)
-            self.a2 = nn.Conv2d(lora_dim, in_dim, (1, 1), bias=False)
-            self.b1 = nn.Conv2d(in_dim, lora_dim, (1, 1), bias=False)
-            self.b2 = nn.Conv2d(lora_dim, out_dim, (1, 1), bias=False)
-        elif isinstance(org_module, nn.Linear):
-            in_dim = org_module.in_features
-            out_dim = org_module.out_features
-            self.a1 = nn.Linear(in_dim, lora_dim, bias=False)
-            self.a2 = nn.Linear(lora_dim, in_dim, bias=False)
-            self.b1 = nn.Linear(in_dim, lora_dim, bias=False)
-            self.b2 = nn.Linear(lora_dim, out_dim, bias=False)
-        else:
-            raise NotImplementedError
-        self.shape = org_module.weight.shape
-
-        if dropout:
-            self.dropout = nn.Dropout(dropout)
-        else:
-            self.dropout = nn.Identity()
-        self.rank_dropout = rank_dropout
-        self.rank_dropout_scale = rank_dropout_scale
-        self.module_dropout = module_dropout
-
-        if type(alpha) == torch.Tensor:
-            alpha = alpha.detach().float().numpy()  # without casting, bf16 causes error
-        alpha = lora_dim if alpha is None or alpha == 0 else alpha
-        self.scale = alpha / self.lora_dim
-        self.register_buffer("alpha", torch.tensor(alpha))  # 定数として扱える
-
-        # same as microsoft's
-        torch.nn.init.kaiming_uniform_(self.a1.weight, a=math.sqrt(5))
-        torch.nn.init.zeros_(self.a2.weight)
-        torch.nn.init.kaiming_uniform_(self.b1.weight, a=math.sqrt(5))
-        torch.nn.init.zeros_(self.b2.weight)
-
-        self.multiplier = multiplier
-        self.org_module = [org_module]
-        self.org_forward = self.org_module[0].forward
-
-    def apply_to(self):
-        self.org_forward = self.org_module[0].forward
-        self.org_module[0].forward = self.forward
-
-    def restore(self):
-        self.org_module[0].forward = self.org_forward
-
-    def merge_to(self, multiplier=1.0):
-        weight = self.make_weight() * self.scale * multiplier
-        self.org_module[0].weight.data.add_(weight)
-
-    def make_weight(self, device=None):
-        wa1 = self.a1.weight.view(self.a1.weight.size(0), -1)
-        wa2 = self.a2.weight.view(self.a2.weight.size(0), -1)
-        wb1 = self.b1.weight.view(self.b1.weight.size(0), -1)
-        wb2 = self.b2.weight.view(self.b2.weight.size(0), -1)
-        orig = self.org_module[0].weight.view(self.org_module[0].weight.size(0), -1)
-        return (wb2 @ wb1) + ((orig @ wa2) @ wa1)
-
-    def forward(self, x):
-        if self.module_dropout and self.training:
-            if torch.rand(1) < self.module_dropout:
-                return self.org_forward(x)
-        scale = self.scale * self.multiplier
-
-        ax_mid = self.a1(x) * scale
-        bx_mid = self.b1(x) * scale
-
-        if self.rank_dropout and self.training:
-            drop_a = (
-                torch.rand(self.lora_dim, device=ax_mid.device) < self.rank_dropout
-            ).to(ax_mid.dtype)
-            if self.rank_dropout_scale:
-                drop_a /= drop_a.mean()
-            drop_b = (
-                torch.rand(self.lora_dim, device=bx_mid.device) < self.rank_dropout
-            ).to(bx_mid.dtype)
-            if self.rank_dropout_scale:
-                drop_b /= drop_b.mean()
-            if (dims := len(x.shape)) == 4:
-                drop_a = drop_a.view(1, -1, 1, 1)
-                drop_b = drop_b.view(1, -1, 1, 1)
-            else:
-                drop_a = drop_a.view(*[1] * (dims - 1), -1)
-                drop_b = drop_b.view(*[1] * (dims - 1), -1)
-            ax_mid = ax_mid * drop_a
-            bx_mid = bx_mid * drop_b
-
-        return (
-            self.org_forward(x + self.dropout(self.a2(ax_mid)) * self.scale)
-            + self.dropout(self.b2(bx_mid)) * self.scale
-        )
+import math
+
+import torch
+import torch.nn as nn
+
+from .base import ModuleCustomSD
+
+
+class GLoRAModule(ModuleCustomSD):
+    """
+    modifed from kohya-ss/sd-scripts/networks/lora:LoRAModule
+    """
+
+    def __init__(
+        self,
+        lora_name,
+        org_module: nn.Module,
+        multiplier=1.0,
+        lora_dim=4,
+        alpha=1,
+        dropout=0.0,
+        rank_dropout=0.0,
+        module_dropout=0.0,
+        rank_dropout_scale=False,
+        rs_lora=False,
+        *args,
+        **kwargs,
+    ):
+        """if alpha == 0 or None, alpha is rank (no scaling)."""
+        super().__init__()
+        self.lora_name = lora_name
+        self.lora_dim = lora_dim
+        self.tucker = False
+        self.rs_lora = rs_lora
+
+        if isinstance(org_module, nn.Conv2d):
+            assert org_module.kernel_size == (1, 1)
+            in_dim = org_module.in_channels
+            out_dim = org_module.out_channels
+            self.a1 = nn.Conv2d(in_dim, lora_dim, (1, 1), bias=False)
+            self.a2 = nn.Conv2d(lora_dim, in_dim, (1, 1), bias=False)
+            self.b1 = nn.Conv2d(in_dim, lora_dim, (1, 1), bias=False)
+            self.b2 = nn.Conv2d(lora_dim, out_dim, (1, 1), bias=False)
+        elif isinstance(org_module, nn.Linear):
+            in_dim = org_module.in_features
+            out_dim = org_module.out_features
+            self.a1 = nn.Linear(in_dim, lora_dim, bias=False)
+            self.a2 = nn.Linear(lora_dim, in_dim, bias=False)
+            self.b1 = nn.Linear(in_dim, lora_dim, bias=False)
+            self.b2 = nn.Linear(lora_dim, out_dim, bias=False)
+        else:
+            raise NotImplementedError
+        self.shape = org_module.weight.shape
+
+        if dropout:
+            self.dropout = nn.Dropout(dropout)
+        else:
+            self.dropout = nn.Identity()
+        self.rank_dropout = rank_dropout
+        self.rank_dropout_scale = rank_dropout_scale
+        self.module_dropout = module_dropout
+
+        if type(alpha) == torch.Tensor:
+            alpha = alpha.detach().float().numpy()  # without casting, bf16 causes error
+        alpha = lora_dim if alpha is None or alpha == 0 else alpha
+
+        r_factor = lora_dim
+        if self.rs_lora:
+            r_factor = math.sqrt(r_factor)
+
+        self.scale = alpha / r_factor
+    
+        self.register_buffer("alpha", torch.tensor(alpha))  # 定数として扱える
+
+        # same as microsoft's
+        torch.nn.init.kaiming_uniform_(self.a1.weight, a=math.sqrt(5))
+        torch.nn.init.zeros_(self.a2.weight)
+        torch.nn.init.kaiming_uniform_(self.b1.weight, a=math.sqrt(5))
+        torch.nn.init.zeros_(self.b2.weight)
+
+        self.multiplier = multiplier
+        self.org_module = [org_module]
+        self.org_forward = self.org_module[0].forward
+
+    def apply_to(self):
+        self.org_forward = self.org_module[0].forward
+        self.org_module[0].forward = self.forward
+
+    def restore(self):
+        self.org_module[0].forward = self.org_forward
+
+    def merge_to(self, multiplier=1.0):
+        weight = self.make_weight() * self.scale * multiplier
+        self.org_module[0].weight.data.add_(weight)
+
+    def make_weight(self, device=None):
+        wa1 = self.a1.weight.view(self.a1.weight.size(0), -1)
+        wa2 = self.a2.weight.view(self.a2.weight.size(0), -1)
+        wb1 = self.b1.weight.view(self.b1.weight.size(0), -1)
+        wb2 = self.b2.weight.view(self.b2.weight.size(0), -1)
+        orig = self.org_module[0].weight.view(self.org_module[0].weight.size(0), -1)
+        return (wb2 @ wb1) + ((orig @ wa2) @ wa1)
+
+    def forward(self, x):
+        if self.module_dropout and self.training:
+            if torch.rand(1) < self.module_dropout:
+                return self.org_forward(x)
+        scale = self.scale * self.multiplier
+
+        ax_mid = self.a1(x) * scale
+        bx_mid = self.b1(x) * scale
+
+        if self.rank_dropout and self.training:
+            drop_a = (
+                torch.rand(self.lora_dim, device=ax_mid.device) < self.rank_dropout
+            ).to(ax_mid.dtype)
+            if self.rank_dropout_scale:
+                drop_a /= drop_a.mean()
+            drop_b = (
+                torch.rand(self.lora_dim, device=bx_mid.device) < self.rank_dropout
+            ).to(bx_mid.dtype)
+            if self.rank_dropout_scale:
+                drop_b /= drop_b.mean()
+            if (dims := len(x.shape)) == 4:
+                drop_a = drop_a.view(1, -1, 1, 1)
+                drop_b = drop_b.view(1, -1, 1, 1)
+            else:
+                drop_a = drop_a.view(*[1] * (dims - 1), -1)
+                drop_b = drop_b.view(*[1] * (dims - 1), -1)
+            ax_mid = ax_mid * drop_a
+            bx_mid = bx_mid * drop_b
+
+        return (
+            self.org_forward(x + self.dropout(self.a2(ax_mid)) * self.scale)
+            + self.dropout(self.b2(bx_mid)) * self.scale
+        )
```

### Comparing `lycoris_lora-2.3.0.dev4/lycoris/modules/ia3.py` & `lycoris_lora-2.3.0.dev5/lycoris/modules/ia3.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-import torch
-import torch.nn as nn
-
-from .base import ModuleCustomSD
-
-
-class IA3Module(ModuleCustomSD):
-    """
-    Hadamard product Implementaion for Low Rank Adaptation
-    """
-
-    def __init__(
-        self,
-        lora_name,
-        org_module: nn.Module,
-        multiplier=1.0,
-        train_on_input=False,
-        **kwargs
-    ):
-        """if alpha == 0 or None, alpha is rank (no scaling)."""
-        super().__init__()
-        self.lora_name = lora_name
-        self.tucker = False
-
-        self.shape = org_module.weight.shape
-        if org_module.__class__.__name__ == "Conv2d":
-            in_dim = org_module.in_channels
-            out_dim = org_module.out_channels
-            if train_on_input:
-                train_dim = in_dim
-            else:
-                train_dim = out_dim
-            self.weight = nn.Parameter(torch.empty(1, train_dim, 1, 1))
-        else:
-            in_dim = org_module.in_features
-            out_dim = org_module.out_features
-            if train_on_input:
-                train_dim = in_dim
-            else:
-                train_dim = out_dim
-
-            self.weight = nn.Parameter(torch.empty(train_dim))
-
-        # Need more experiences on init method
-        torch.nn.init.constant_(self.weight, 0)
-
-        self.multiplier = multiplier
-        self.org_forward = None
-        self.org_module = [org_module]  # remove in applying
-        self.grad_ckpt = False
-        self.train_input = train_on_input
-        self.register_buffer("on_input", torch.tensor(int(train_on_input)))
-
-    def apply_to(self):
-        self.org_forward = self.org_module[0].forward
-        self.org_module[0].forward = self.forward
-
-    @torch.enable_grad()
-    def forward(self, x):
-        if self.train_input:
-            x = x * (1 + self.weight * self.multiplier)
-        out = self.org_forward(x)
-        dtype = out.dtype
-        if not self.train_input:
-            out = out * (1 + self.weight * self.multiplier)
-            out = out.to(dtype)
-        return out
+import torch
+import torch.nn as nn
+
+from .base import ModuleCustomSD
+
+
+class IA3Module(ModuleCustomSD):
+    """
+    Hadamard product Implementaion for Low Rank Adaptation
+    """
+
+    def __init__(
+        self,
+        lora_name,
+        org_module: nn.Module,
+        multiplier=1.0,
+        train_on_input=False,
+        **kwargs
+    ):
+        """if alpha == 0 or None, alpha is rank (no scaling)."""
+        super().__init__()
+        self.lora_name = lora_name
+        self.tucker = False
+
+        self.shape = org_module.weight.shape
+        if org_module.__class__.__name__ == "Conv2d":
+            in_dim = org_module.in_channels
+            out_dim = org_module.out_channels
+            if train_on_input:
+                train_dim = in_dim
+            else:
+                train_dim = out_dim
+            self.weight = nn.Parameter(torch.empty(1, train_dim, 1, 1))
+        else:
+            in_dim = org_module.in_features
+            out_dim = org_module.out_features
+            if train_on_input:
+                train_dim = in_dim
+            else:
+                train_dim = out_dim
+
+            self.weight = nn.Parameter(torch.empty(train_dim))
+
+        # Need more experiences on init method
+        torch.nn.init.constant_(self.weight, 0)
+
+        self.multiplier = multiplier
+        self.org_forward = None
+        self.org_module = [org_module]  # remove in applying
+        self.grad_ckpt = False
+        self.train_input = train_on_input
+        self.register_buffer("on_input", torch.tensor(int(train_on_input)))
+
+    def apply_to(self):
+        self.org_forward = self.org_module[0].forward
+        self.org_module[0].forward = self.forward
+
+    @torch.enable_grad()
+    def forward(self, x):
+        if self.train_input:
+            x = x * (1 + self.weight * self.multiplier)
+        out = self.org_forward(x)
+        dtype = out.dtype
+        if not self.train_input:
+            out = out * (1 + self.weight * self.multiplier)
+            out = out.to(dtype)
+        return out
```

### Comparing `lycoris_lora-2.3.0.dev4/lycoris/modules/lilora.py` & `lycoris_lora-2.3.0.dev5/lycoris/modules/lilora.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,326 +1,339 @@
-import math
-from functools import cache
-
-import torch
-import torch.nn as nn
-import torch.nn.functional as F
-
-from .base import ModuleCustomSD
-from ..logging import logger
-
-
-@cache
-def log_wd():
-    return logger.warning(
-        "Using weight_decompose=True with LoRA (DoRA) will ignore network_dropout."
-        "Only rank dropout and module dropout will be applied"
-    )
-
-
-class LiLoConModule(ModuleCustomSD):
-    """
-    modifed from kohya-ss/sd-scripts/networks/lora:LoRAModule
-    """
-
-    def __init__(
-        self,
-        lora_name,
-        org_module: nn.Module,
-        multiplier=1.0,
-        lora_dim=4,
-        alpha=1,
-        dropout=0.0,
-        rank_dropout=0.0,
-        module_dropout=0.0,
-        use_tucker=False,
-        use_scalar=False,
-        rank_dropout_scale=False,
-        weight_decompose=False,
-        bypass_mode=False,
-        **kwargs,
-    ):
-        """if alpha == 0 or None, alpha is rank (no scaling)."""
-        super().__init__()
-        self.lora_name = lora_name
-        self.lora_dim = lora_dim
-        self.tucker = False
-        assert not (
-            bypass_mode and weight_decompose
-        ), "bypass_mode and dora_wd cannot be used together"
-
-        if isinstance(org_module, nn.Conv2d):
-            in_dim = org_module.in_channels
-            k_size = org_module.kernel_size
-            out_dim = org_module.out_channels
-            self.tucker = use_tucker and k_size != (1, 1)
-            self.op = F.conv2d
-            self.extra_args = {
-                "stride": org_module.stride,
-                "padding": org_module.padding,
-                "dilation": org_module.dilation,
-                "groups": org_module.groups,
-            }
-        else:
-            in_dim = org_module.in_features
-            out_dim = org_module.out_features
-            self.op = F.linear
-            self.extra_args = {}
-
-        if isinstance(org_module, nn.Conv2d):
-            self.isconv = True
-            # For general LoCon
-            in_dim = org_module.in_channels
-            k_size = org_module.kernel_size
-            stride = org_module.stride
-            padding = org_module.padding
-            out_dim = org_module.out_channels
-            self.down_op = F.conv2d
-            self.up_op = F.conv2d
-            if use_tucker and k_size != (1, 1):
-                self.lora_down = nn.Conv2d(in_dim, lora_dim, (1, 1), bias=False)
-                self.lora_mid = nn.Conv2d(
-                    lora_dim, lora_dim, k_size, stride, padding, bias=False
-                )
-                self.tucker = True
-            else:
-                self.lora_down = nn.Conv2d(
-                    in_dim, lora_dim, k_size, stride, padding, bias=False
-                )
-            self.lora_up = nn.Conv2d(lora_dim, out_dim, (1, 1), bias=False)
-        elif isinstance(org_module, nn.Linear):
-            self.isconv = False
-            self.down_op = F.linear
-            self.up_op = F.linear
-            in_dim = org_module.in_features
-            out_dim = org_module.out_features
-            self.lora_down = nn.Linear(in_dim, lora_dim, bias=False)
-            self.lora_up = nn.Linear(lora_dim, out_dim, bias=False)
-        else:
-            raise NotImplementedError
-        self.shape = org_module.weight.shape
-
-        self.wd = weight_decompose
-        if self.wd:
-            org_weight: nn.Parameter = org_module.weight
-            self.dora_mean_dim = tuple(i for i in range(org_weight.dim()) if i != 1)
-            self.dora_scale = nn.Parameter(
-                torch.mean(org_weight, dim=self.dora_mean_dim, keepdim=True)
-            )
-
-        if dropout:
-            self.dropout = nn.Dropout(dropout)
-            if self.wd:
-                log_wd()
-        else:
-            self.dropout = nn.Identity()
-        self.rank_dropout = rank_dropout
-        self.rank_dropout_scale = rank_dropout_scale
-        self.module_dropout = module_dropout
-
-        if type(alpha) == torch.Tensor:
-            alpha = alpha.detach().float().numpy()  # without casting, bf16 causes error
-        alpha = lora_dim if alpha is None or alpha == 0 else alpha
-        self.scale = alpha / self.lora_dim
-        self.register_buffer("alpha", torch.tensor(alpha))  # 定数として扱える
-
-        if use_scalar:
-            self.scalar = nn.Parameter(torch.tensor(0.0))
-        else:
-            self.scalar: torch.FloatTensor
-            self.register_buffer("scalar", torch.tensor(1.0), persistent=False)
-        # same as microsoft's
-        torch.nn.init.kaiming_uniform_(self.lora_down.weight, a=math.sqrt(5))
-        if use_scalar:
-            torch.nn.init.kaiming_uniform_(self.lora_up.weight, a=math.sqrt(5))
-        else:
-            torch.nn.init.constant_(self.lora_up.weight, 0)
-        if self.tucker:
-            torch.nn.init.kaiming_uniform_(self.lora_mid.weight, a=math.sqrt(5))
-
-        self.multiplier = multiplier
-        self.org_module = [org_module]
-        self.org_forward = self.org_module[0].forward
-
-    def load_weight_hook(self, module: nn.Module, incompatible_keys):
-        missing_keys = incompatible_keys.missing_keys
-        for key in missing_keys:
-            if "scalar" in key:
-                del missing_keys[missing_keys.index(key)]
-        self.scalar = nn.Parameter(torch.ones_like(self.scalar))
-
-    def apply_to(self, is_hypernet=False, **kwargs):
-        self.org_forward = self.org_module[0].forward
-        if is_hypernet:
-            self.org_module[0].forward = self.hypernet_forward
-        else:
-            self.org_module[0].forward = self.forward
-
-    def restore(self):
-        self.org_module[0].forward = self.org_forward
-
-    def merge_to(self, multiplier=1.0):
-        weight = self.make_weight() * self.scale * multiplier
-        self.org_module[0].weight.data.add_(weight)
-
-    def make_weight(self, device=None):
-        wa = self.lora_up.weight.to(device)
-        wb = self.lora_down.weight.to(device)
-        if self.tucker:
-            t = self.lora_mid.weight.to(device)
-            wa = wa.squeeze(-1, -2)
-            wb = wb.squeeze(-1, -2)
-            weight = torch.einsum("i j k l, p i, j r -> p r k l", t, wa, wb)
-        else:
-            weight = wa.view(wa.size(0), -1) @ wb.view(wb.size(0), -1)
-
-        weight = weight.view(self.shape)
-        if self.training and self.rank_dropout:
-            drop = (torch.rand(weight.size(0)) > self.rank_dropout).to(weight.dtype)
-            drop = drop.view(-1, *[1] * len(weight.shape[1:])).to(weight.device)
-            if self.rank_dropout_scale:
-                drop /= drop.mean()
-            weight *= drop
-
-        return weight * self.scalar.to(device)
-
-    def apply_weight_decompose(self, weight):
-        return (
-            weight / weight.mean(dim=self.dora_mean_dim, keepdim=True) * self.dora_scale
-        )
-
-    def custom_state_dict(self):
-        destination = {}
-        if self.wd:
-            destination["dora_scale"] = self.dora_scale
-        destination["alpha"] = self.alpha
-        destination["lora_up.weight"] = self.lora_up.weight * self.scalar
-        destination["lora_down.weight"] = self.lora_down.weight
-        if self.tucker:
-            destination["lora_mid.weight"] = self.lora_mid.weight
-        return destination
-
-    @torch.no_grad()
-    def apply_max_norm(self, max_norm, device=None):
-        orig_norm = self.make_weight(device).norm() * self.scale
-        norm = torch.clamp(orig_norm, max_norm / 2)
-        desired = torch.clamp(norm, max=max_norm)
-        ratio = desired.cpu() / norm.cpu()
-
-        scaled = norm != desired
-        if scaled:
-            self.scalar *= ratio
-
-        return scaled, orig_norm * ratio
-
-    def update_weights(self, down, up, idx):
-        self.down, self.up = self.make_lightweight(down.squeeze(1), up.squeeze(1), idx)
-
-    def make_lightweight(self, down, up, seed=None, down_aux=None, up_aux=None):
-        if down.dim() == 3:
-            down = down.reshape(down.size(0), self.lora_dim, -1)
-            up = up.reshape(up.size(0), -1, self.lora_dim)
-        else:
-            down = down.reshape(self.lora_dim, -1)
-            up = up.reshape(-1, self.lora_dim)
-        # print(up.shape)
-        if seed is None:
-            assert down_aux is not None and up_aux is not None
-        else:
-            rng_state = torch.get_rng_state()
-            torch.manual_seed(seed)
-            if down_aux is None or up_aux is None:
-                down_aux = torch.empty(
-                    down.size(down.dim() - 1),
-                    self.lora_down.weight.size(1),
-                    device=down.device,
-                )
-                up_aux = torch.empty(
-                    self.lora_up.weight.size(0), up.size(up.dim() - 2), device=up.device
-                )
-                nn.init.orthogonal_(down_aux)
-                nn.init.orthogonal_(up_aux)
-                # print(up_aux.shape)
-            torch.set_rng_state(rng_state)
-        if down.dim() == 3 and down.size(0) == 1:
-            down = down.squeeze(0)
-        if up.dim() == 3 and up.size(0) == 1:
-            up = up.squeeze(0)
-        down = down + 1  # avoid zero grad or slow training, give it a constant
-        return (down @ down_aux), (up_aux @ up)
-
-    def apply_lightweight(self, down, up, seed=None, down_aux=None, up_aux=None):
-        down_weight, up_weight = self.make_lightweight(down, up, seed, down_aux, up_aux)
-        self.lora_down.weight.data = down_weight
-        self.lora_up.weight.data = up_weight
-        return down_weight, up_weight
-
-    def hypernet_forward(self, x):
-        if self.module_dropout and self.training:
-            if torch.rand(1) < self.module_dropout:
-                return self.org_forward(x)
-        scale = self.scale * self.multiplier
-
-        down_weight = self.down
-        up_weight = self.up
-
-        x_batch = None
-        if down_weight.dim() == 3:
-            if x.size(0) != down_weight.size(0):
-                assert (
-                    self.isconv == False
-                ), "Convolutional hypernet with batch size mismatch is not supported"
-                x_batch = x.size(0)
-                x = x.view(down_weight.size(0), -1, *x.shape[1:])
-
-            if self.isconv:
-                mid = torch.einsum("ijk, ik... -> ij...", down_weight, x)
-            else:
-                mid = torch.einsum("ijk, i...k -> i...j", down_weight, x)
-        else:
-            if self.isconv:
-                weight = down_weight.unsqueeze(-1).unsqueeze(-1)
-            else:
-                weight = down_weight
-            mid = self.down_op(x, weight)
-
-        if self.rank_dropout and self.training:
-            drop = (
-                torch.rand(self.lora_dim, device=mid.device) < self.rank_dropout
-            ).to(mid.dtype)
-            if self.rank_dropout_scale:
-                drop /= drop.mean()
-            if (dims := len(x.shape)) == 4:
-                drop = drop.view(1, -1, 1, 1)
-            else:
-                drop = drop.view(*[1] * (dims - 1), -1)
-            mid = mid * drop
-
-        if up_weight.dim() == 3:
-            mid_batch = None
-            if mid.size(0) != up_weight.size(0):
-                assert (
-                    self.isconv == False
-                ), "Convolutional hypernet with batch size mismatch is not supported"
-                mid_batch = mid.size(0)
-                mid = mid.view(up_weight.size(0), -1, *mid.shape[1:])
-
-            if self.isconv:
-                up = torch.einsum("ijk, ik... -> ij...", up_weight, mid)
-            else:
-                up = torch.einsum("ijk, i...k -> i...j", up_weight, mid)
-
-            if mid_batch is not None:
-                up = up.view(mid_batch, *up.shape[2:])
-        else:
-            if self.isconv:
-                weight = up_weight.unsqueeze(-1).unsqueeze(-1)
-            else:
-                weight = up_weight
-            up = self.up_op(mid, weight)
-
-        if x_batch is not None:
-            up = up.view(x_batch, *up.shape[2:])
-
-        org_out = self.org_forward(x)
-        # print(x.shape, org_out.shape, up.shape)
-        return org_out + self.dropout(up) * scale
+import math
+from functools import cache
+
+import torch
+import torch.nn as nn
+import torch.nn.functional as F
+
+from .base import ModuleCustomSD
+from ..logging import logger
+
+
+@cache
+def log_wd():
+    return logger.warning(
+        "Using weight_decompose=True with LoRA (DoRA) will ignore network_dropout."
+        "Only rank dropout and module dropout will be applied"
+    )
+
+
+class LiLoConModule(ModuleCustomSD):
+    """
+    modifed from kohya-ss/sd-scripts/networks/lora:LoRAModule
+    """
+
+    def __init__(
+        self,
+        lora_name,
+        org_module: nn.Module,
+        multiplier=1.0,
+        lora_dim=4,
+        alpha=1,
+        dropout=0.0,
+        rank_dropout=0.0,
+        module_dropout=0.0,
+        use_tucker=False,
+        use_scalar=False,
+        rank_dropout_scale=False,
+        weight_decompose=False,
+        bypass_mode=False,
+        rs_lora=False,
+        **kwargs,
+    ):
+        """if alpha == 0 or None, alpha is rank (no scaling)."""
+        super().__init__()
+        self.lora_name = lora_name
+        self.lora_dim = lora_dim
+        self.tucker = False
+        self.rs_lora = rs_lora
+        
+        assert not (
+            bypass_mode and weight_decompose
+        ), "bypass_mode and dora_wd cannot be used together"
+
+        if isinstance(org_module, nn.Conv2d):
+            in_dim = org_module.in_channels
+            k_size = org_module.kernel_size
+            out_dim = org_module.out_channels
+            self.tucker = use_tucker and k_size != (1, 1)
+            self.op = F.conv2d
+            self.extra_args = {
+                "stride": org_module.stride,
+                "padding": org_module.padding,
+                "dilation": org_module.dilation,
+                "groups": org_module.groups,
+            }
+        else:
+            in_dim = org_module.in_features
+            out_dim = org_module.out_features
+            self.op = F.linear
+            self.extra_args = {}
+
+        if isinstance(org_module, nn.Conv2d):
+            self.isconv = True
+            # For general LoCon
+            in_dim = org_module.in_channels
+            k_size = org_module.kernel_size
+            stride = org_module.stride
+            padding = org_module.padding
+            out_dim = org_module.out_channels
+            self.down_op = F.conv2d
+            self.up_op = F.conv2d
+            if use_tucker and k_size != (1, 1):
+                self.lora_down = nn.Conv2d(in_dim, lora_dim, (1, 1), bias=False)
+                self.lora_mid = nn.Conv2d(
+                    lora_dim, lora_dim, k_size, stride, padding, bias=False
+                )
+                self.tucker = True
+            else:
+                self.lora_down = nn.Conv2d(
+                    in_dim, lora_dim, k_size, stride, padding, bias=False
+                )
+            self.lora_up = nn.Conv2d(lora_dim, out_dim, (1, 1), bias=False)
+        elif isinstance(org_module, nn.Linear):
+            self.isconv = False
+            self.down_op = F.linear
+            self.up_op = F.linear
+            in_dim = org_module.in_features
+            out_dim = org_module.out_features
+            self.lora_down = nn.Linear(in_dim, lora_dim, bias=False)
+            self.lora_up = nn.Linear(lora_dim, out_dim, bias=False)
+        else:
+            raise NotImplementedError
+        self.shape = org_module.weight.shape
+
+        self.wd = weight_decompose
+        if self.wd:
+            org_weight: nn.Parameter = org_module.weight
+            self.dora_mean_dim = tuple(i for i in range(org_weight.dim()) if i != 1)
+            self.dora_scale = nn.Parameter(
+                torch.mean(org_weight, dim=self.dora_mean_dim, keepdim=True)
+            )
+
+        if dropout:
+            self.dropout = nn.Dropout(dropout)
+            if self.wd:
+                log_wd()
+        else:
+            self.dropout = nn.Identity()
+        self.rank_dropout = rank_dropout
+        self.rank_dropout_scale = rank_dropout_scale
+        self.module_dropout = module_dropout
+
+        if type(alpha) == torch.Tensor:
+            alpha = alpha.detach().float().numpy()  # without casting, bf16 causes error
+
+        alpha = lora_dim if alpha is None or alpha == 0 else alpha
+
+        r_factor = lora_dim
+        if self.rs_lora:
+            r_factor = math.sqrt(r_factor)
+
+        self.scale = alpha / r_factor
+
+        self.register_buffer("alpha", torch.tensor(alpha))  # 定数として扱える
+
+        if use_scalar:
+            self.scalar = nn.Parameter(torch.tensor(0.0))
+        else:
+            self.scalar: torch.FloatTensor
+            self.register_buffer("scalar", torch.tensor(1.0), persistent=False)
+        # same as microsoft's
+        torch.nn.init.kaiming_uniform_(self.lora_down.weight, a=math.sqrt(5))
+        if use_scalar:
+            torch.nn.init.kaiming_uniform_(self.lora_up.weight, a=math.sqrt(5))
+        else:
+            torch.nn.init.constant_(self.lora_up.weight, 0)
+        if self.tucker:
+            torch.nn.init.kaiming_uniform_(self.lora_mid.weight, a=math.sqrt(5))
+
+        self.multiplier = multiplier
+        self.org_module = [org_module]
+        self.org_forward = self.org_module[0].forward
+
+    def load_weight_hook(self, module: nn.Module, incompatible_keys):
+        missing_keys = incompatible_keys.missing_keys
+        for key in missing_keys:
+            if "scalar" in key:
+                del missing_keys[missing_keys.index(key)]
+        if isinstance(self.scalar, nn.Parameter):
+            self.scalar.copy_(torch.ones_like(self.scalar))
+        else:
+            self.scalar = torch.ones_like(self.scalar)
+
+    def apply_to(self, is_hypernet=False, **kwargs):
+        self.org_forward = self.org_module[0].forward
+        if is_hypernet:
+            self.org_module[0].forward = self.hypernet_forward
+        else:
+            self.org_module[0].forward = self.forward
+
+    def restore(self):
+        self.org_module[0].forward = self.org_forward
+
+    def merge_to(self, multiplier=1.0):
+        weight = self.make_weight() * self.scale * multiplier
+        self.org_module[0].weight.data.add_(weight)
+
+    def make_weight(self, device=None):
+        wa = self.lora_up.weight.to(device)
+        wb = self.lora_down.weight.to(device)
+        if self.tucker:
+            t = self.lora_mid.weight.to(device)
+            wa = wa.squeeze(-1, -2)
+            wb = wb.squeeze(-1, -2)
+            weight = torch.einsum("i j k l, p i, j r -> p r k l", t, wa, wb)
+        else:
+            weight = wa.view(wa.size(0), -1) @ wb.view(wb.size(0), -1)
+
+        weight = weight.view(self.shape)
+        if self.training and self.rank_dropout:
+            drop = (torch.rand(weight.size(0)) > self.rank_dropout).to(weight.dtype)
+            drop = drop.view(-1, *[1] * len(weight.shape[1:])).to(weight.device)
+            if self.rank_dropout_scale:
+                drop /= drop.mean()
+            weight *= drop
+
+        return weight * self.scalar.to(device)
+
+    def apply_weight_decompose(self, weight):
+        return (
+            weight / weight.mean(dim=self.dora_mean_dim, keepdim=True) * self.dora_scale
+        )
+
+    def custom_state_dict(self):
+        destination = {}
+        if self.wd:
+            destination["dora_scale"] = self.dora_scale
+        destination["alpha"] = self.alpha
+        destination["lora_up.weight"] = self.lora_up.weight * self.scalar
+        destination["lora_down.weight"] = self.lora_down.weight
+        if self.tucker:
+            destination["lora_mid.weight"] = self.lora_mid.weight
+        return destination
+
+    @torch.no_grad()
+    def apply_max_norm(self, max_norm, device=None):
+        orig_norm = self.make_weight(device).norm() * self.scale
+        norm = torch.clamp(orig_norm, max_norm / 2)
+        desired = torch.clamp(norm, max=max_norm)
+        ratio = desired.cpu() / norm.cpu()
+
+        scaled = norm != desired
+        if scaled:
+            self.scalar *= ratio
+
+        return scaled, orig_norm * ratio
+
+    def update_weights(self, down, up, idx):
+        self.down, self.up = self.make_lightweight(down.squeeze(1), up.squeeze(1), idx)
+
+    def make_lightweight(self, down, up, seed=None, down_aux=None, up_aux=None):
+        if down.dim() == 3:
+            down = down.reshape(down.size(0), self.lora_dim, -1)
+            up = up.reshape(up.size(0), -1, self.lora_dim)
+        else:
+            down = down.reshape(self.lora_dim, -1)
+            up = up.reshape(-1, self.lora_dim)
+        # print(up.shape)
+        if seed is None:
+            assert down_aux is not None and up_aux is not None
+        else:
+            rng_state = torch.get_rng_state()
+            torch.manual_seed(seed)
+            if down_aux is None or up_aux is None:
+                down_aux = torch.empty(
+                    down.size(down.dim() - 1),
+                    self.lora_down.weight.size(1),
+                    device=down.device,
+                )
+                up_aux = torch.empty(
+                    self.lora_up.weight.size(0), up.size(up.dim() - 2), device=up.device
+                )
+                nn.init.orthogonal_(down_aux)
+                nn.init.orthogonal_(up_aux)
+                # print(up_aux.shape)
+            torch.set_rng_state(rng_state)
+        if down.dim() == 3 and down.size(0) == 1:
+            down = down.squeeze(0)
+        if up.dim() == 3 and up.size(0) == 1:
+            up = up.squeeze(0)
+        down = down + 1  # avoid zero grad or slow training, give it a constant
+        return (down @ down_aux), (up_aux @ up)
+
+    def apply_lightweight(self, down, up, seed=None, down_aux=None, up_aux=None):
+        down_weight, up_weight = self.make_lightweight(down, up, seed, down_aux, up_aux)
+        self.lora_down.weight.data = down_weight
+        self.lora_up.weight.data = up_weight
+        return down_weight, up_weight
+
+    def hypernet_forward(self, x):
+        if self.module_dropout and self.training:
+            if torch.rand(1) < self.module_dropout:
+                return self.org_forward(x)
+        scale = self.scale * self.multiplier
+
+        down_weight = self.down
+        up_weight = self.up
+
+        x_batch = None
+        if down_weight.dim() == 3:
+            if x.size(0) != down_weight.size(0):
+                assert (
+                    self.isconv == False
+                ), "Convolutional hypernet with batch size mismatch is not supported"
+                x_batch = x.size(0)
+                x = x.view(down_weight.size(0), -1, *x.shape[1:])
+
+            if self.isconv:
+                mid = torch.einsum("ijk, ik... -> ij...", down_weight, x)
+            else:
+                mid = torch.einsum("ijk, i...k -> i...j", down_weight, x)
+        else:
+            if self.isconv:
+                weight = down_weight.unsqueeze(-1).unsqueeze(-1)
+            else:
+                weight = down_weight
+            mid = self.down_op(x, weight)
+
+        if self.rank_dropout and self.training:
+            drop = (
+                torch.rand(self.lora_dim, device=mid.device) < self.rank_dropout
+            ).to(mid.dtype)
+            if self.rank_dropout_scale:
+                drop /= drop.mean()
+            if (dims := len(x.shape)) == 4:
+                drop = drop.view(1, -1, 1, 1)
+            else:
+                drop = drop.view(*[1] * (dims - 1), -1)
+            mid = mid * drop
+
+        if up_weight.dim() == 3:
+            mid_batch = None
+            if mid.size(0) != up_weight.size(0):
+                assert (
+                    self.isconv == False
+                ), "Convolutional hypernet with batch size mismatch is not supported"
+                mid_batch = mid.size(0)
+                mid = mid.view(up_weight.size(0), -1, *mid.shape[1:])
+
+            if self.isconv:
+                up = torch.einsum("ijk, ik... -> ij...", up_weight, mid)
+            else:
+                up = torch.einsum("ijk, i...k -> i...j", up_weight, mid)
+
+            if mid_batch is not None:
+                up = up.view(mid_batch, *up.shape[2:])
+        else:
+            if self.isconv:
+                weight = up_weight.unsqueeze(-1).unsqueeze(-1)
+            else:
+                weight = up_weight
+            up = self.up_op(mid, weight)
+
+        if x_batch is not None:
+            up = up.view(x_batch, *up.shape[2:])
+
+        org_out = self.org_forward(x)
+        # print(x.shape, org_out.shape, up.shape)
+        return org_out + self.dropout(up) * scale
```

### Comparing `lycoris_lora-2.3.0.dev4/lycoris/modules/locon.py` & `lycoris_lora-2.3.0.dev5/lycoris/modules/locon.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,299 +1,310 @@
-import math
-from functools import cache
-
-import torch
-import torch.nn as nn
-import torch.nn.functional as F
-
-from .base import ModuleCustomSD
-from ..logging import logger
-from ..utils.bnb import LinearNF4, QuantLinears, log_bypass
-
-
-@cache
-def log_wd():
-    return logger.warning(
-        "Using weight_decompose=True with LoRA (DoRA) will ignore network_dropout."
-        "Only rank dropout and module dropout will be applied"
-    )
-
-
-class LoConModule(ModuleCustomSD):
-    """
-    modifed from kohya-ss/sd-scripts/networks/lora:LoRAModule
-    """
-
-    def __init__(
-        self,
-        lora_name,
-        org_module: nn.Module,
-        multiplier=1.0,
-        lora_dim=4,
-        alpha=1,
-        dropout=0.0,
-        rank_dropout=0.0,
-        module_dropout=0.0,
-        use_tucker=False,
-        use_scalar=False,
-        rank_dropout_scale=False,
-        weight_decompose=False,
-        bypass_mode=False,
-        **kwargs,
-    ):
-        """if alpha == 0 or None, alpha is rank (no scaling)."""
-        super().__init__()
-        self.lora_name = lora_name
-        self.lora_dim = lora_dim
-        self.tucker = False
-
-        if isinstance(org_module, nn.Conv2d):
-            in_dim = org_module.in_channels
-            k_size = org_module.kernel_size
-            out_dim = org_module.out_channels
-            self.tucker = use_tucker and k_size != (1, 1)
-            self.op = F.conv2d
-            self.extra_args = {
-                "stride": org_module.stride,
-                "padding": org_module.padding,
-                "dilation": org_module.dilation,
-                "groups": org_module.groups,
-            }
-        else:
-            in_dim = org_module.in_features
-            out_dim = org_module.out_features
-            self.op = F.linear
-            self.extra_args = {}
-
-        if isinstance(org_module, QuantLinears):
-            if not bypass_mode:
-                log_bypass()
-            bypass_mode = True
-        self.bypass_mode = bypass_mode
-        assert not (
-            bypass_mode and weight_decompose
-        ), "bypass_mode and dora_wd cannot be used together"
-
-        if isinstance(org_module, nn.Conv2d):
-            self.isconv = True
-            # For general LoCon
-            in_dim = org_module.in_channels
-            k_size = org_module.kernel_size
-            stride = org_module.stride
-            padding = org_module.padding
-            out_dim = org_module.out_channels
-            self.down_op = F.conv2d
-            self.up_op = F.conv2d
-            if use_tucker and k_size != (1, 1):
-                self.lora_down = nn.Conv2d(in_dim, lora_dim, (1, 1), bias=False)
-                self.lora_mid = nn.Conv2d(
-                    lora_dim, lora_dim, k_size, stride, padding, bias=False
-                )
-                self.tucker = True
-            else:
-                self.lora_down = nn.Conv2d(
-                    in_dim, lora_dim, k_size, stride, padding, bias=False
-                )
-            self.lora_up = nn.Conv2d(lora_dim, out_dim, (1, 1), bias=False)
-        elif isinstance(org_module, nn.Linear):
-            self.isconv = False
-            self.down_op = F.linear
-            self.up_op = F.linear
-            in_dim = org_module.in_features
-            out_dim = org_module.out_features
-            self.lora_down = nn.Linear(in_dim, lora_dim, bias=False)
-            self.lora_up = nn.Linear(lora_dim, out_dim, bias=False)
-        else:
-            raise NotImplementedError
-        self.shape = org_module.weight.shape
-
-        self.wd = weight_decompose
-        if self.wd:
-            org_weight: nn.Parameter = org_module.weight
-            self.dora_norm_dims = org_weight.dim() - 1
-            self.dora_scale = nn.Parameter(
-                torch.norm(
-                    org_weight.transpose(1, 0).reshape(org_weight.shape[1], -1),
-                    dim=1,
-                    keepdim=True,
-                )
-                .reshape(org_weight.shape[1], *[1] * self.dora_norm_dims)
-                .transpose(1, 0)
-            ).float()
-
-        if dropout:
-            self.dropout = nn.Dropout(dropout)
-            if self.wd:
-                log_wd()
-        else:
-            self.dropout = nn.Identity()
-        self.rank_dropout = rank_dropout
-        self.rank_dropout_scale = rank_dropout_scale
-        self.module_dropout = module_dropout
-
-        if type(alpha) == torch.Tensor:
-            alpha = alpha.detach().float().numpy()  # without casting, bf16 causes error
-        alpha = lora_dim if alpha is None or alpha == 0 else alpha
-        self.scale = alpha / self.lora_dim
-        self.register_buffer("alpha", torch.tensor(alpha))  # 定数として扱える
-
-        if use_scalar:
-            self.scalar = nn.Parameter(torch.tensor(0.0))
-        else:
-            self.register_buffer("scalar", torch.tensor(1.0), persistent=False)
-        # same as microsoft's
-        torch.nn.init.kaiming_uniform_(self.lora_down.weight, a=math.sqrt(5))
-        if use_scalar:
-            torch.nn.init.kaiming_uniform_(self.lora_up.weight, a=math.sqrt(5))
-        else:
-            torch.nn.init.constant_(self.lora_up.weight, 0)
-        if self.tucker:
-            torch.nn.init.kaiming_uniform_(self.lora_mid.weight, a=math.sqrt(5))
-
-        self.multiplier = multiplier
-        self.org_module = [org_module]
-        self.org_forward = self.org_module[0].forward
-
-    def load_weight_hook(self, module: nn.Module, incompatible_keys):
-        missing_keys = incompatible_keys.missing_keys
-        for key in missing_keys:
-            if "scalar" in key:
-                del missing_keys[missing_keys.index(key)]
-        self.scalar = nn.Parameter(torch.ones_like(self.scalar))
-
-    def apply_to(self, is_hypernet=False, **kwargs):
-        self.org_forward = self.org_module[0].forward
-        if is_hypernet:
-            self.org_module[0].forward = self.hypernet_forward
-        else:
-            self.org_module[0].forward = self.forward
-
-    def restore(self):
-        self.org_module[0].forward = self.org_forward
-
-    def merge_to(self, multiplier=1.0):
-        weight = self.make_weight() * self.scale * multiplier
-        self.org_module[0].weight.data.add_(weight)
-
-    def make_weight(self, device=None):
-        wa = self.lora_up.weight.to(device)
-        wb = self.lora_down.weight.to(device)
-        if self.tucker:
-            t = self.lora_mid.weight.to(device)
-            wa = wa.squeeze(-1, -2)
-            wb = wb.squeeze(-1, -2)
-            weight = torch.einsum("i j k l, p i, j r -> p r k l", t, wa, wb)
-        else:
-            weight = wa.view(wa.size(0), -1) @ wb.view(wb.size(0), -1)
-
-        weight = weight.view(self.shape)
-        if self.training and self.rank_dropout:
-            drop = (torch.rand(weight.size(0)) > self.rank_dropout).to(weight.dtype)
-            drop = drop.view(-1, *[1] * len(weight.shape[1:])).to(weight.device)
-            if self.rank_dropout_scale:
-                drop /= drop.mean()
-            weight *= drop
-
-        return weight * self.scalar.to(device)
-
-    def apply_weight_decompose(self, weight):
-        weight = weight.to(self.dora_scale.dtype)
-        weight_norm = (
-            weight.transpose(0, 1)
-            .reshape(weight.shape[1], -1)
-            .norm(dim=1, keepdim=True)
-            .reshape(weight.shape[1], *[1] * self.dora_norm_dims)
-            .transpose(0, 1)
-        )
-
-        return weight * (self.dora_scale.to(weight.device) / weight_norm)
-
-    def custom_state_dict(self):
-        destination = {}
-        if self.wd:
-            destination["dora_scale"] = self.dora_scale
-        destination["alpha"] = self.alpha
-        destination["lora_up.weight"] = self.lora_up.weight * self.scalar
-        destination["lora_down.weight"] = self.lora_down.weight
-        if self.tucker:
-            destination["lora_mid.weight"] = self.lora_mid.weight
-        return destination
-
-    @torch.no_grad()
-    def apply_max_norm(self, max_norm, device=None):
-        orig_norm = self.make_weight(device).norm() * self.scale
-        norm = torch.clamp(orig_norm, max_norm / 2)
-        desired = torch.clamp(norm, max=max_norm)
-        ratio = desired.cpu() / norm.cpu()
-
-        scaled = norm != desired
-        if scaled:
-            self.scalar *= ratio
-
-        return scaled, orig_norm * ratio
-
-    def forward(self, x):
-        if self.module_dropout and self.training:
-            if torch.rand(1) < self.module_dropout:
-                return self.org_forward(x)
-        scale = self.scale * self.multiplier
-
-        dtype = next(self.parameters()).dtype
-        if not self.bypass_mode:
-            weight = (
-                self.org_module[0].weight.data.to(device=x.device, dtype=dtype)
-                + self.make_weight(x.device).to(device=x.device, dtype=dtype) * scale
-            )
-            if self.wd:
-                weight = self.apply_weight_decompose(weight)
-            bias = (
-                None
-                if self.org_module[0].bias is None
-                else self.org_module[0].bias.data
-            )
-            return self.op(x, weight, bias, **self.extra_args)
-        else:
-            if self.tucker:
-                mid = self.lora_mid(self.lora_down(x))
-            else:
-                mid = self.lora_down(x)
-
-            if self.rank_dropout and self.training:
-                drop = (
-                    torch.rand(self.lora_dim, device=mid.device) > self.rank_dropout
-                ).to(mid.dtype)
-                if self.rank_dropout_scale:
-                    drop /= drop.mean()
-                if (dims := len(x.shape)) == 4:
-                    drop = drop.view(1, -1, 1, 1)
-                else:
-                    drop = drop.view(*[1] * (dims - 1), -1)
-                mid = mid * drop
-
-            return self.org_forward(x) + self.dropout(
-                self.lora_up(mid) * self.scalar * scale
-            )
-
-
-if __name__ == "__main__":
-    base = nn.Linear(128, 128).cuda()
-    lokr = LoConModule("test", base, 1, 4, 1, weight_decompose=True).cuda()
-    print(lokr)
-    test_input = torch.randn(1, 128).cuda()
-    test_output = lokr(test_input)
-    print(test_output.shape)
-
-    base_4bit = LinearNF4(128, 128)
-    base_4bit.load_state_dict(base.state_dict())
-    base_4bit.cuda()
-    qlocon = LoConModule("test", base_4bit, 1, 4, 1, weight_decompose=False).cuda()
-    print(qlocon)
-    test_input = torch.randn(1, 128).cuda()
-    test_output = qlocon(test_input)
-    print(test_output.shape)
-
-    base = nn.Conv2d(128, 128, 3, 1, 1)
-    lokr = LoConModule("test", base, 1, 4, 1, weight_decompose=True, use_tucker=True)
-    print(lokr)
-    test_input = torch.randn(1, 128, 16, 16)
-    test_output = lokr(test_input)
-    print(test_output.shape)
+import math
+from functools import cache
+
+import torch
+import torch.nn as nn
+import torch.nn.functional as F
+
+from .base import ModuleCustomSD
+from ..logging import logger
+from ..utils.bnb import LinearNF4, QuantLinears, log_bypass
+
+
+@cache
+def log_wd():
+    return logger.warning(
+        "Using weight_decompose=True with LoRA (DoRA) will ignore network_dropout."
+        "Only rank dropout and module dropout will be applied"
+    )
+
+
+class LoConModule(ModuleCustomSD):
+    """
+    modifed from kohya-ss/sd-scripts/networks/lora:LoRAModule
+    """
+
+    def __init__(
+        self,
+        lora_name,
+        org_module: nn.Module,
+        multiplier=1.0,
+        lora_dim=4,
+        alpha=1,
+        dropout=0.0,
+        rank_dropout=0.0,
+        module_dropout=0.0,
+        use_tucker=False,
+        use_scalar=False,
+        rank_dropout_scale=False,
+        weight_decompose=False,
+        bypass_mode=False,
+        rs_lora=False,
+        **kwargs,
+    ):
+        """if alpha == 0 or None, alpha is rank (no scaling)."""
+        super().__init__()
+        self.lora_name = lora_name
+        self.lora_dim = lora_dim
+        self.tucker = False
+        self.rs_lora = rs_lora
+
+        if isinstance(org_module, nn.Conv2d):
+            in_dim = org_module.in_channels
+            k_size = org_module.kernel_size
+            out_dim = org_module.out_channels
+            self.tucker = use_tucker and k_size != (1, 1)
+            self.op = F.conv2d
+            self.extra_args = {
+                "stride": org_module.stride,
+                "padding": org_module.padding,
+                "dilation": org_module.dilation,
+                "groups": org_module.groups,
+            }
+        else:
+            in_dim = org_module.in_features
+            out_dim = org_module.out_features
+            self.op = F.linear
+            self.extra_args = {}
+
+        if isinstance(org_module, QuantLinears):
+            if not bypass_mode:
+                log_bypass()
+            bypass_mode = True
+        self.bypass_mode = bypass_mode
+        assert not (
+            bypass_mode and weight_decompose
+        ), "bypass_mode and dora_wd cannot be used together"
+
+        if isinstance(org_module, nn.Conv2d):
+            self.isconv = True
+            # For general LoCon
+            in_dim = org_module.in_channels
+            k_size = org_module.kernel_size
+            stride = org_module.stride
+            padding = org_module.padding
+            out_dim = org_module.out_channels
+            self.down_op = F.conv2d
+            self.up_op = F.conv2d
+            if use_tucker and k_size != (1, 1):
+                self.lora_down = nn.Conv2d(in_dim, lora_dim, (1, 1), bias=False)
+                self.lora_mid = nn.Conv2d(
+                    lora_dim, lora_dim, k_size, stride, padding, bias=False
+                )
+                self.tucker = True
+            else:
+                self.lora_down = nn.Conv2d(
+                    in_dim, lora_dim, k_size, stride, padding, bias=False
+                )
+            self.lora_up = nn.Conv2d(lora_dim, out_dim, (1, 1), bias=False)
+        elif isinstance(org_module, nn.Linear):
+            self.isconv = False
+            self.down_op = F.linear
+            self.up_op = F.linear
+            in_dim = org_module.in_features
+            out_dim = org_module.out_features
+            self.lora_down = nn.Linear(in_dim, lora_dim, bias=False)
+            self.lora_up = nn.Linear(lora_dim, out_dim, bias=False)
+        else:
+            raise NotImplementedError
+        self.shape = org_module.weight.shape
+
+        self.wd = weight_decompose
+        if self.wd:
+            org_weight: nn.Parameter = org_module.weight
+            self.dora_norm_dims = org_weight.dim() - 1
+            self.dora_scale = nn.Parameter(
+                torch.norm(
+                    org_weight.transpose(1, 0).reshape(org_weight.shape[1], -1),
+                    dim=1,
+                    keepdim=True,
+                )
+                .reshape(org_weight.shape[1], *[1] * self.dora_norm_dims)
+                .transpose(1, 0)
+            ).float()
+
+        if dropout:
+            self.dropout = nn.Dropout(dropout)
+            if self.wd:
+                log_wd()
+        else:
+            self.dropout = nn.Identity()
+        self.rank_dropout = rank_dropout
+        self.rank_dropout_scale = rank_dropout_scale
+        self.module_dropout = module_dropout
+
+        if type(alpha) == torch.Tensor:
+            alpha = alpha.detach().float().numpy()  # without casting, bf16 causes error
+        alpha = lora_dim if alpha is None or alpha == 0 else alpha
+
+        r_factor = lora_dim
+        if self.rs_lora:
+            r_factor = math.sqrt(r_factor)
+
+        self.scale = alpha / r_factor
+    
+        self.register_buffer("alpha", torch.tensor(alpha))  # 定数として扱える
+
+        if use_scalar:
+            self.scalar = nn.Parameter(torch.tensor(0.0))
+        else:
+            self.register_buffer("scalar", torch.tensor(1.0), persistent=False)
+        # same as microsoft's
+        torch.nn.init.kaiming_uniform_(self.lora_down.weight, a=math.sqrt(5))
+        if use_scalar:
+            torch.nn.init.kaiming_uniform_(self.lora_up.weight, a=math.sqrt(5))
+        else:
+            torch.nn.init.constant_(self.lora_up.weight, 0)
+        if self.tucker:
+            torch.nn.init.kaiming_uniform_(self.lora_mid.weight, a=math.sqrt(5))
+
+        self.multiplier = multiplier
+        self.org_module = [org_module]
+        self.org_forward = self.org_module[0].forward
+
+    def load_weight_hook(self, module: nn.Module, incompatible_keys):
+        missing_keys = incompatible_keys.missing_keys
+        for key in missing_keys:
+            if "scalar" in key:
+                del missing_keys[missing_keys.index(key)]
+        if isinstance(self.scalar, nn.Parameter):
+            self.scalar.copy_(torch.ones_like(self.scalar))
+        else:
+            self.scalar = torch.ones_like(self.scalar)
+
+    def apply_to(self, is_hypernet=False, **kwargs):
+        self.org_forward = self.org_module[0].forward
+        if is_hypernet:
+            self.org_module[0].forward = self.hypernet_forward
+        else:
+            self.org_module[0].forward = self.forward
+
+    def restore(self):
+        self.org_module[0].forward = self.org_forward
+
+    def merge_to(self, multiplier=1.0):
+        weight = self.make_weight() * self.scale * multiplier
+        self.org_module[0].weight.data.add_(weight)
+
+    def make_weight(self, device=None):
+        wa = self.lora_up.weight.to(device)
+        wb = self.lora_down.weight.to(device)
+        if self.tucker:
+            t = self.lora_mid.weight.to(device)
+            wa = wa.squeeze(-1, -2)
+            wb = wb.squeeze(-1, -2)
+            weight = torch.einsum("i j k l, p i, j r -> p r k l", t, wa, wb)
+        else:
+            weight = wa.view(wa.size(0), -1) @ wb.view(wb.size(0), -1)
+
+        weight = weight.view(self.shape)
+        if self.training and self.rank_dropout:
+            drop = (torch.rand(weight.size(0)) > self.rank_dropout).to(weight.dtype)
+            drop = drop.view(-1, *[1] * len(weight.shape[1:])).to(weight.device)
+            if self.rank_dropout_scale:
+                drop /= drop.mean()
+            weight *= drop
+
+        return weight * self.scalar.to(device)
+
+    def apply_weight_decompose(self, weight):
+        weight = weight.to(self.dora_scale.dtype)
+        weight_norm = (
+            weight.transpose(0, 1)
+            .reshape(weight.shape[1], -1)
+            .norm(dim=1, keepdim=True)
+            .reshape(weight.shape[1], *[1] * self.dora_norm_dims)
+            .transpose(0, 1)
+        ) + torch.finfo(weight.dtype).eps
+
+        return weight * (self.dora_scale.to(weight.device) / weight_norm)
+
+    def custom_state_dict(self):
+        destination = {}
+        if self.wd:
+            destination["dora_scale"] = self.dora_scale
+        destination["alpha"] = self.alpha
+        destination["lora_up.weight"] = self.lora_up.weight * self.scalar
+        destination["lora_down.weight"] = self.lora_down.weight
+        if self.tucker:
+            destination["lora_mid.weight"] = self.lora_mid.weight
+        return destination
+
+    @torch.no_grad()
+    def apply_max_norm(self, max_norm, device=None):
+        orig_norm = self.make_weight(device).norm() * self.scale
+        norm = torch.clamp(orig_norm, max_norm / 2)
+        desired = torch.clamp(norm, max=max_norm)
+        ratio = desired.cpu() / norm.cpu()
+
+        scaled = norm != desired
+        if scaled:
+            self.scalar *= ratio
+
+        return scaled, orig_norm * ratio
+
+    def forward(self, x):
+        if self.module_dropout and self.training:
+            if torch.rand(1) < self.module_dropout:
+                return self.org_forward(x)
+        scale = self.scale * self.multiplier
+
+        dtype = next(self.parameters()).dtype
+        if not self.bypass_mode:
+            weight = (
+                self.org_module[0].weight.data.to(device=x.device, dtype=dtype)
+                + self.make_weight(x.device).to(device=x.device, dtype=dtype) * scale
+            )
+            if self.wd:
+                weight = self.apply_weight_decompose(weight)
+            bias = (
+                None
+                if self.org_module[0].bias is None
+                else self.org_module[0].bias.data
+            )
+            return self.op(x, weight, bias, **self.extra_args)
+        else:
+            if self.tucker:
+                mid = self.lora_mid(self.lora_down(x))
+            else:
+                mid = self.lora_down(x)
+
+            if self.rank_dropout and self.training:
+                drop = (
+                    torch.rand(self.lora_dim, device=mid.device) > self.rank_dropout
+                ).to(mid.dtype)
+                if self.rank_dropout_scale:
+                    drop /= drop.mean()
+                if (dims := len(x.shape)) == 4:
+                    drop = drop.view(1, -1, 1, 1)
+                else:
+                    drop = drop.view(*[1] * (dims - 1), -1)
+                mid = mid * drop
+
+            return self.org_forward(x) + self.dropout(
+                self.lora_up(mid) * self.scalar * scale
+            )
+
+
+if __name__ == "__main__":
+    base = nn.Linear(128, 128).cuda()
+    lokr = LoConModule("test", base, 1, 4, 1, weight_decompose=True).cuda()
+    print(lokr)
+    test_input = torch.randn(1, 128).cuda()
+    test_output = lokr(test_input)
+    print(test_output.shape)
+
+    base_4bit = LinearNF4(128, 128)
+    base_4bit.load_state_dict(base.state_dict())
+    base_4bit.cuda()
+    qlocon = LoConModule("test", base_4bit, 1, 4, 1, weight_decompose=False).cuda()
+    print(qlocon)
+    test_input = torch.randn(1, 128).cuda()
+    test_output = qlocon(test_input)
+    print(test_output.shape)
+
+    base = nn.Conv2d(128, 128, 3, 1, 1)
+    lokr = LoConModule("test", base, 1, 4, 1, weight_decompose=True, use_tucker=True)
+    print(lokr)
+    test_input = torch.randn(1, 128, 16, 16)
+    test_output = lokr(test_input)
+    print(test_output.shape)
```

### Comparing `lycoris_lora-2.3.0.dev4/lycoris/modules/lokr.py` & `lycoris_lora-2.3.0.dev5/lycoris/modules/lokr.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,500 +1,511 @@
-import math
-from functools import cache
-
-import torch
-import torch.nn as nn
-import torch.nn.functional as F
-
-from einops import rearrange
-
-from .base import ModuleCustomSD
-from ..logging import logger
-from ..utils.bnb import LinearNF4, QuantLinears, log_bypass
-
-
-@cache
-def logging_force_full_matrix(lora_dim, dim, factor):
-    logger.warning(
-        f"lora_dim {lora_dim} is too large for"
-        f" dim={dim} and {factor=}"
-        ", using full matrix mode."
-    )
-
-
-def factorization(dimension: int, factor: int = -1) -> tuple[int, int]:
-    """
-    return a tuple of two value of input dimension decomposed by the number closest to factor
-    second value is higher or equal than first value.
-
-    In LoRA with Kroneckor Product, first value is a value for weight scale.
-    second value is a value for weight.
-
-    Because of non-commutative property, A⊗B ≠ B⊗A. Meaning of two matrices is slightly different.
-
-    examples)
-    factor
-        -1               2                4               8               16               ...
-    127 -> 1, 127   127 -> 1, 127    127 -> 1, 127   127 -> 1, 127   127 -> 1, 127
-    128 -> 8, 16    128 -> 2, 64     128 -> 4, 32    128 -> 8, 16    128 -> 8, 16
-    250 -> 10, 25   250 -> 2, 125    250 -> 2, 125   250 -> 5, 50    250 -> 10, 25
-    360 -> 8, 45    360 -> 2, 180    360 -> 4, 90    360 -> 8, 45    360 -> 12, 30
-    512 -> 16, 32   512 -> 2, 256    512 -> 4, 128   512 -> 8, 64    512 -> 16, 32
-    1024 -> 32, 32  1024 -> 2, 512   1024 -> 4, 256  1024 -> 8, 128  1024 -> 16, 64
-    """
-
-    if factor > 0 and (dimension % factor) == 0:
-        m = factor
-        n = dimension // factor
-        if m > n:
-            n, m = m, n
-        return m, n
-    if factor < 0:
-        factor = dimension
-    m, n = 1, dimension
-    length = m + n
-    while m < n:
-        new_m = m + 1
-        while dimension % new_m != 0:
-            new_m += 1
-        new_n = dimension // new_m
-        if new_m + new_n > length or new_m > factor:
-            break
-        else:
-            m, n = new_m, new_n
-    if m > n:
-        n, m = m, n
-    return m, n
-
-
-def make_weight_tucker(t, wa, wb):
-    rebuild2 = torch.einsum("i j k l, i p, j r -> p r k l", t, wa, wb)  # [c, d, k1, k2]
-    return rebuild2
-
-
-def make_kron(w1, w2, scale):
-    if len(w2.shape) == 4:
-        w1 = w1.unsqueeze(2).unsqueeze(2)
-    w2 = w2.contiguous()
-    rebuild = torch.kron(w1, w2)
-
-    return rebuild * scale
-
-
-class LokrModule(ModuleCustomSD):
-    """
-    modifed from kohya-ss/sd-scripts/networks/lora:LoRAModule
-        and from KohakuBlueleaf/LyCORIS/lycoris:loha:LoHaModule
-        and from KohakuBlueleaf/LyCORIS/lycoris:locon:LoconModule
-    """
-
-    def __init__(
-        self,
-        lora_name,
-        org_module: nn.Module,
-        multiplier=1.0,
-        lora_dim=4,
-        alpha=1,
-        dropout=0.0,
-        rank_dropout=0.0,
-        module_dropout=0.0,
-        use_tucker=False,
-        use_scalar=False,
-        decompose_both=False,
-        factor: int = -1,  # factorization factor
-        rank_dropout_scale=False,
-        weight_decompose=False,
-        full_matrix=False,
-        bypass_mode=False,
-        unbalanced_factorization=False,
-        **kwargs,
-    ):
-        """if alpha == 0 or None, alpha is rank (no scaling)."""
-        super().__init__()
-        factor = int(factor)
-        self.lora_name = lora_name
-        self.lora_dim = lora_dim
-        self.tucker = False
-        self.use_w1 = False
-        self.use_w2 = False
-        self.full_matrix = full_matrix
-
-        self.shape = org_module.weight.shape
-        if org_module.__class__.__name__ == "Conv2d":
-            in_dim = org_module.in_channels
-            k_size = org_module.kernel_size
-            out_dim = org_module.out_channels
-            self.shape = (out_dim, in_dim, *k_size)
-
-            in_m, in_n = factorization(in_dim, factor)
-            out_l, out_k = factorization(out_dim, factor)
-            if unbalanced_factorization:
-                out_l, out_k = out_k, out_l
-            shape = ((out_l, out_k), (in_m, in_n), *k_size)  # ((a, b), (c, d), *k_size)
-            self.tucker = use_tucker and k_size != (1, 1)
-            if (
-                decompose_both
-                and lora_dim < max(shape[0][0], shape[1][0]) / 2
-                and not self.full_matrix
-            ):
-                self.lokr_w1_a = nn.Parameter(torch.empty(shape[0][0], lora_dim))
-                self.lokr_w1_b = nn.Parameter(torch.empty(lora_dim, shape[1][0]))
-            else:
-                self.use_w1 = True
-                self.lokr_w1 = nn.Parameter(
-                    torch.empty(shape[0][0], shape[1][0])
-                )  # a*c, 1-mode
-
-            if lora_dim >= max(shape[0][1], shape[1][1]) / 2 or self.full_matrix:
-                if not self.full_matrix:
-                    logging_force_full_matrix(lora_dim, max(in_dim, out_dim), factor)
-                self.use_w2 = True
-                self.lokr_w2 = nn.Parameter(
-                    torch.empty(shape[0][1], shape[1][1], *k_size)
-                )
-            elif self.tucker:
-                self.lokr_t2 = nn.Parameter(
-                    torch.empty(lora_dim, lora_dim, shape[2], shape[3])
-                )
-                self.lokr_w2_a = nn.Parameter(
-                    torch.empty(lora_dim, shape[0][1])
-                )  # b, 1-mode
-                self.lokr_w2_b = nn.Parameter(
-                    torch.empty(lora_dim, shape[1][1])
-                )  # d, 2-mode
-            else:  # Conv2d not tucker
-                # bigger part. weight and LoRA. [b, dim] x [dim, d*k1*k2]
-                self.lokr_w2_a = nn.Parameter(torch.empty(shape[0][1], lora_dim))
-                self.lokr_w2_b = nn.Parameter(
-                    torch.empty(lora_dim, shape[1][1] * shape[2] * shape[3])
-                )
-                # w1 ⊗ (w2_a x w2_b) = (a, b)⊗((c, dim)x(dim, d*k1*k2)) = (a, b)⊗(c, d*k1*k2) = (ac, bd*k1*k2)
-
-            self.op = F.conv2d
-            self.extra_args = {
-                "stride": org_module.stride,
-                "padding": org_module.padding,
-                "dilation": org_module.dilation,
-                "groups": org_module.groups,
-            }
-
-        else:  # Linear
-            in_dim = org_module.in_features
-            out_dim = org_module.out_features
-            self.shape = (out_dim, in_dim)
-
-            in_m, in_n = factorization(in_dim, factor)
-            out_l, out_k = factorization(out_dim, factor)
-            if unbalanced_factorization:
-                out_l, out_k = out_k, out_l
-            shape = (
-                (out_l, out_k),
-                (in_m, in_n),
-            )  # ((a, b), (c, d)), out_dim = a*c, in_dim = b*d
-            # smaller part. weight scale
-            if decompose_both and lora_dim < max(shape[0][0], shape[1][0]) / 2:
-                self.lokr_w1_a = nn.Parameter(torch.empty(shape[0][0], lora_dim))
-                self.lokr_w1_b = nn.Parameter(torch.empty(lora_dim, shape[1][0]))
-            else:
-                self.use_w1 = True
-                self.lokr_w1 = nn.Parameter(
-                    torch.empty(shape[0][0], shape[1][0])
-                )  # a*c, 1-mode
-            if lora_dim < max(shape[0][1], shape[1][1]) / 2:
-                # bigger part. weight and LoRA. [b, dim] x [dim, d]
-                self.lokr_w2_a = nn.Parameter(torch.empty(shape[0][1], lora_dim))
-                self.lokr_w2_b = nn.Parameter(torch.empty(lora_dim, shape[1][1]))
-                # w1 ⊗ (w2_a x w2_b) = (a, b)⊗((c, dim)x(dim, d)) = (a, b)⊗(c, d) = (ac, bd)
-            else:
-                self.use_w2 = True
-                self.lokr_w2 = nn.Parameter(torch.empty(shape[0][1], shape[1][1]))
-
-            self.op = F.linear
-            self.extra_args = {}
-
-        if isinstance(org_module, QuantLinears):
-            if not bypass_mode:
-                log_bypass()
-            bypass_mode = True
-        self.bypass_mode = bypass_mode
-        assert not (
-            bypass_mode and weight_decompose
-        ), "bypass_mode and dora_wd cannot be used together"
-
-        self.wd = weight_decompose
-        if self.wd:
-            org_weight: nn.Parameter = org_module.weight
-            self.dora_norm_dims = org_weight.dim() - 1
-            self.dora_scale = nn.Parameter(
-                torch.norm(
-                    org_weight.transpose(1, 0).reshape(org_weight.shape[1], -1),
-                    dim=1,
-                    keepdim=True,
-                )
-                .reshape(org_weight.shape[1], *[1] * self.dora_norm_dims)
-                .transpose(1, 0)
-            ).float()
-
-        self.dropout = dropout
-        if dropout:
-            print("[WARN]LoHa/LoKr haven't implemented normal dropout yet.")
-        self.rank_dropout = rank_dropout
-        self.rank_dropout_scale = rank_dropout_scale
-        self.module_dropout = module_dropout
-
-        if isinstance(alpha, torch.Tensor):
-            alpha = alpha.detach().float().numpy()  # without casting, bf16 causes error
-        alpha = lora_dim if alpha is None or alpha == 0 else alpha
-        if self.use_w2 and self.use_w1:
-            # use scale = 1
-            alpha = lora_dim
-        self.scale = alpha / self.lora_dim
-        self.register_buffer("alpha", torch.tensor(alpha))  # 定数として扱える
-
-        if use_scalar:
-            self.scalar = nn.Parameter(torch.tensor(0.0))
-        else:
-            self.scalar = torch.tensor(1.0)
-
-        if self.use_w2:
-            if use_scalar:
-                torch.nn.init.kaiming_uniform_(self.lokr_w2, a=math.sqrt(5))
-            else:
-                torch.nn.init.constant_(self.lokr_w2, 0)
-        else:
-            if self.tucker:
-                torch.nn.init.kaiming_uniform_(self.lokr_t2, a=math.sqrt(5))
-            torch.nn.init.kaiming_uniform_(self.lokr_w2_a, a=math.sqrt(5))
-            if use_scalar:
-                torch.nn.init.kaiming_uniform_(self.lokr_w2_b, a=math.sqrt(5))
-            else:
-                torch.nn.init.constant_(self.lokr_w2_b, 0)
-
-        if self.use_w1:
-            torch.nn.init.kaiming_uniform_(self.lokr_w1, a=math.sqrt(5))
-        else:
-            torch.nn.init.kaiming_uniform_(self.lokr_w1_a, a=math.sqrt(5))
-            torch.nn.init.kaiming_uniform_(self.lokr_w1_b, a=math.sqrt(5))
-
-        self.multiplier = multiplier
-        self.org_module = [org_module]
-        self.org_forward = self.org_module[0].forward
-        weight = make_kron(
-            self.lokr_w1 if self.use_w1 else self.lokr_w1_a @ self.lokr_w1_b,
-            (
-                self.lokr_w2
-                if self.use_w2
-                else (
-                    make_weight_tucker(self.lokr_t2, self.lokr_w2_a, self.lokr_w2_b)
-                    if self.tucker
-                    else self.lokr_w2_a @ self.lokr_w2_b
-                )
-            ),
-            torch.tensor(self.multiplier * self.scale),
-        )
-        assert torch.sum(torch.isnan(weight)) == 0, "weight is nan"
-
-    def load_weight_hook(self, module: nn.Module, incompatible_keys):
-        missing_keys = incompatible_keys.missing_keys
-        for key in missing_keys:
-            if "scalar" in key:
-                del missing_keys[missing_keys.index(key)]
-        self.scalar = nn.Parameter(torch.ones_like(self.scalar))
-
-    # Same as locon.py
-    def apply_to(self):
-        self.org_forward = self.org_module[0].forward
-        self.org_module[0].forward = self.forward
-
-    def restore(self):
-        self.org_module[0].forward = self.org_forward
-
-    def merge_to(self, multiplier=1.0):
-        weight = self.get_weight(self.shape)
-        self.org_module[0].weight.data.add_(weight * multiplier)
-
-    def get_weight(self, shape):
-        weight = make_kron(
-            self.lokr_w1 if self.use_w1 else self.lokr_w1_a @ self.lokr_w1_b,
-            (
-                self.lokr_w2
-                if self.use_w2
-                else (
-                    make_weight_tucker(self.lokr_t2, self.lokr_w2_a, self.lokr_w2_b)
-                    if self.tucker
-                    else self.lokr_w2_a @ self.lokr_w2_b
-                )
-            ),
-            torch.tensor(self.scale),
-        )
-        if shape is not None:
-            weight = weight.reshape(shape)
-        if self.training and self.rank_dropout:
-            drop = (torch.rand(weight.size(0)) > self.rank_dropout).to(weight.dtype)
-            drop = drop.view(-1, *[1] * len(weight.shape[1:])).to(weight.device)
-            if self.rank_dropout_scale:
-                drop /= drop.mean()
-            weight *= drop
-        return weight
-
-    def apply_weight_decompose(self, weight):
-        weight = weight.to(self.dora_scale.dtype)
-        weight_norm = (
-            weight.transpose(0, 1)
-            .reshape(weight.shape[1], -1)
-            .norm(dim=1, keepdim=True)
-            .reshape(weight.shape[1], *[1] * self.dora_norm_dims)
-            .transpose(0, 1)
-        )
-
-        return weight * (self.dora_scale.to(weight.device) / weight_norm)
-
-    def custom_state_dict(self):
-        destination = {}
-        destination["alpha"] = self.alpha
-        if self.wd:
-            destination["dora_scale"] = self.dora_scale
-        if self.use_w1:
-            destination["lokr_w1"] = self.lokr_w1 * self.scalar
-        else:
-            destination["lokr_w1_a"] = self.lokr_w1_a * self.scalar
-            destination["lokr_w1_b"] = self.lokr_w1_b
-
-        if self.use_w2:
-            destination["lokr_w2"] = self.lokr_w2
-        else:
-            destination["lokr_w2_a"] = self.lokr_w2_a
-            destination["lokr_w2_b"] = self.lokr_w2_b
-            if self.tucker:
-                destination["lokr_t2"] = self.lokr_t2
-        return destination
-
-    @torch.no_grad()
-    def apply_max_norm(self, max_norm, device=None):
-        orig_norm = self.get_weight(self.shape).norm()
-        norm = torch.clamp(orig_norm, max_norm / 2)
-        desired = torch.clamp(norm, max=max_norm)
-        ratio = desired.cpu() / norm.cpu()
-
-        scaled = norm != desired
-        if scaled:
-            modules = 4 - self.use_w1 - self.use_w2 + (not self.use_w2 and self.tucker)
-            if self.use_w1:
-                self.lokr_w1 *= ratio ** (1 / modules)
-            else:
-                self.lokr_w1_a *= ratio ** (1 / modules)
-                self.lokr_w1_b *= ratio ** (1 / modules)
-
-            if self.use_w2:
-                self.lokr_w2 *= ratio ** (1 / modules)
-            else:
-                if self.tucker:
-                    self.lokr_t2 *= ratio ** (1 / modules)
-                self.lokr_w2_a *= ratio ** (1 / modules)
-                self.lokr_w2_b *= ratio ** (1 / modules)
-
-        return scaled, orig_norm * ratio
-
-    def bypass_forward(self, h):
-        if isinstance(self.org_module[0], nn.Conv2d):
-            h = h.transpose(1, -1)
-        if self.use_w2:
-            ba = self.lokr_w2
-        else:
-            a = self.lokr_w2_b
-            b = self.lokr_w2_a
-        if self.use_w1:
-            c = self.lokr_w1
-        else:
-            c = self.lokr_w1_a @ self.lokr_w1_b
-        uq = c.size(1)
-
-        if self.use_w2:
-            vq = ba.size(1)
-            h_in_group = rearrange(h, "b ... (uq vq) -> b ... uq vq", uq=uq, vq=vq)
-            hb = F.linear(h_in_group, ba)
-        else:
-            vq = a.size(1)
-            h_in_group = rearrange(h, "b ... (uq vq) -> b ... uq vq", uq=uq, vq=vq)
-            ha = F.linear(h_in_group, a)
-            hb = F.linear(ha, b)
-
-        h_cross_group = hb.transpose(-1, -2)
-        hc = F.linear(h_cross_group, c)
-
-        h = rearrange(hc, "b ... vp up -> b ... (up vp)")
-        if isinstance(self.org_module[0], nn.Conv2d):
-            h = h.transpose(1, -1)
-
-        return h
-
-    def forward(self, x):
-        if self.module_dropout and self.training:
-            if torch.rand(1) < self.module_dropout:
-                return self.op(
-                    x,
-                    self.org_module[0].weight.data,
-                    (
-                        None
-                        if self.org_module[0].bias is None
-                        else self.org_module[0].bias.data
-                    ),
-                )
-        if self.bypass_mode:
-            if len(self.shape) > 2 and self.shape[2] > 1:
-                return self.org_forward(x) + self.op(
-                    x, self.get_weight(self.shape), **self.extra_args
-                )
-            else:
-                return self.org_forward(x) + self.bypass_forward(x)
-        else:
-            weight = (
-                self.org_module[0].weight.data.to(
-                    x.device, dtype=next(self.parameters()).dtype
-                )
-                + self.get_weight(self.shape) * self.scalar * self.multiplier
-            )
-            bias = (
-                None
-                if self.org_module[0].bias is None
-                else self.org_module[0].bias.data
-            )
-
-            if self.wd:
-                weight = self.apply_weight_decompose(weight)
-            return self.op(x, weight.view(self.shape), bias, **self.extra_args)
-
-
-if __name__ == "__main__":
-    base = nn.Linear(128, 128).cuda()
-    lokr = LokrModule("test", base, 1, 4, 1, weight_decompose=True, factor=8).cuda()
-    print(lokr)
-    test_input = torch.randn(1, 77, 128).cuda()
-    test_output = lokr(test_input)
-    print(test_output.shape)
-
-    # opt = torch.optim.AdamW(lokr.parameters(), lr=1e-2)
-    # for _ in range(100):
-    #     x = torch.randn(128, 128).cuda()
-    #     t = x / 10
-    #     y = lokr(x)
-    #     loss = F.mse_loss(y, t)
-    #     loss.backward()
-    #     opt.step()
-    #     opt.zero_grad()
-    #     print(loss.item())
-
-    base_4bit = LinearNF4(128, 128)
-    base_4bit.load_state_dict(base.state_dict())
-    base_4bit.cuda()
-    qlocon = LokrModule("test", base_4bit, 1, 4, 1, weight_decompose=False).cuda()
-    print(qlocon)
-    test_output2 = qlocon(test_input)
-    print(test_output2.shape)
-    print(F.mse_loss(test_output, test_output2))
-
-    base = nn.Conv2d(128, 128, 3, 1, 1)
-    lokr = LokrModule("test", base, 1, 4, 1, weight_decompose=True, use_tucker=True)
-    print(lokr)
-    test_input = torch.randn(1, 128, 16, 16)
-    test_output = lokr(test_input)
-    print(test_output.shape)
+import math
+from functools import cache
+
+import torch
+import torch.nn as nn
+import torch.nn.functional as F
+
+from einops import rearrange
+
+from .base import ModuleCustomSD
+from ..logging import logger
+from ..utils.bnb import LinearNF4, QuantLinears, log_bypass
+
+
+@cache
+def logging_force_full_matrix(lora_dim, dim, factor):
+    logger.warning(
+        f"lora_dim {lora_dim} is too large for"
+        f" dim={dim} and {factor=}"
+        ", using full matrix mode."
+    )
+
+
+def factorization(dimension: int, factor: int = -1) -> tuple[int, int]:
+    """
+    return a tuple of two value of input dimension decomposed by the number closest to factor
+    second value is higher or equal than first value.
+
+    In LoRA with Kroneckor Product, first value is a value for weight scale.
+    second value is a value for weight.
+
+    Because of non-commutative property, A⊗B ≠ B⊗A. Meaning of two matrices is slightly different.
+
+    examples)
+    factor
+        -1               2                4               8               16               ...
+    127 -> 1, 127   127 -> 1, 127    127 -> 1, 127   127 -> 1, 127   127 -> 1, 127
+    128 -> 8, 16    128 -> 2, 64     128 -> 4, 32    128 -> 8, 16    128 -> 8, 16
+    250 -> 10, 25   250 -> 2, 125    250 -> 2, 125   250 -> 5, 50    250 -> 10, 25
+    360 -> 8, 45    360 -> 2, 180    360 -> 4, 90    360 -> 8, 45    360 -> 12, 30
+    512 -> 16, 32   512 -> 2, 256    512 -> 4, 128   512 -> 8, 64    512 -> 16, 32
+    1024 -> 32, 32  1024 -> 2, 512   1024 -> 4, 256  1024 -> 8, 128  1024 -> 16, 64
+    """
+
+    if factor > 0 and (dimension % factor) == 0:
+        m = factor
+        n = dimension // factor
+        if m > n:
+            n, m = m, n
+        return m, n
+    if factor < 0:
+        factor = dimension
+    m, n = 1, dimension
+    length = m + n
+    while m < n:
+        new_m = m + 1
+        while dimension % new_m != 0:
+            new_m += 1
+        new_n = dimension // new_m
+        if new_m + new_n > length or new_m > factor:
+            break
+        else:
+            m, n = new_m, new_n
+    if m > n:
+        n, m = m, n
+    return m, n
+
+
+def make_weight_tucker(t, wa, wb):
+    rebuild2 = torch.einsum("i j k l, i p, j r -> p r k l", t, wa, wb)  # [c, d, k1, k2]
+    return rebuild2
+
+
+def make_kron(w1, w2, scale):
+    if len(w2.shape) == 4:
+        w1 = w1.unsqueeze(2).unsqueeze(2)
+    w2 = w2.contiguous()
+    rebuild = torch.kron(w1, w2)
+
+    return rebuild * scale
+
+
+class LokrModule(ModuleCustomSD):
+    """
+    modifed from kohya-ss/sd-scripts/networks/lora:LoRAModule
+        and from KohakuBlueleaf/LyCORIS/lycoris:loha:LoHaModule
+        and from KohakuBlueleaf/LyCORIS/lycoris:locon:LoconModule
+    """
+
+    def __init__(
+        self,
+        lora_name,
+        org_module: nn.Module,
+        multiplier=1.0,
+        lora_dim=4,
+        alpha=1,
+        dropout=0.0,
+        rank_dropout=0.0,
+        module_dropout=0.0,
+        use_tucker=False,
+        use_scalar=False,
+        decompose_both=False,
+        factor: int = -1,  # factorization factor
+        rank_dropout_scale=False,
+        weight_decompose=False,
+        full_matrix=False,
+        bypass_mode=False,
+        rs_lora=False,
+        unbalanced_factorization=False,
+        **kwargs,
+    ):
+        """if alpha == 0 or None, alpha is rank (no scaling)."""
+        super().__init__()
+        factor = int(factor)
+        self.lora_name = lora_name
+        self.lora_dim = lora_dim
+        self.tucker = False
+        self.use_w1 = False
+        self.use_w2 = False
+        self.full_matrix = full_matrix
+        self.rs_lora = rs_lora
+
+        self.shape = org_module.weight.shape
+        if org_module.__class__.__name__ == "Conv2d":
+            in_dim = org_module.in_channels
+            k_size = org_module.kernel_size
+            out_dim = org_module.out_channels
+            self.shape = (out_dim, in_dim, *k_size)
+
+            in_m, in_n = factorization(in_dim, factor)
+            out_l, out_k = factorization(out_dim, factor)
+            if unbalanced_factorization:
+                out_l, out_k = out_k, out_l
+            shape = ((out_l, out_k), (in_m, in_n), *k_size)  # ((a, b), (c, d), *k_size)
+            self.tucker = use_tucker and k_size != (1, 1)
+            if (
+                decompose_both
+                and lora_dim < max(shape[0][0], shape[1][0]) / 2
+                and not self.full_matrix
+            ):
+                self.lokr_w1_a = nn.Parameter(torch.empty(shape[0][0], lora_dim))
+                self.lokr_w1_b = nn.Parameter(torch.empty(lora_dim, shape[1][0]))
+            else:
+                self.use_w1 = True
+                self.lokr_w1 = nn.Parameter(
+                    torch.empty(shape[0][0], shape[1][0])
+                )  # a*c, 1-mode
+
+            if lora_dim >= max(shape[0][1], shape[1][1]) / 2 or self.full_matrix:
+                if not self.full_matrix:
+                    logging_force_full_matrix(lora_dim, max(in_dim, out_dim), factor)
+                self.use_w2 = True
+                self.lokr_w2 = nn.Parameter(
+                    torch.empty(shape[0][1], shape[1][1], *k_size)
+                )
+            elif self.tucker:
+                self.lokr_t2 = nn.Parameter(
+                    torch.empty(lora_dim, lora_dim, shape[2], shape[3])
+                )
+                self.lokr_w2_a = nn.Parameter(
+                    torch.empty(lora_dim, shape[0][1])
+                )  # b, 1-mode
+                self.lokr_w2_b = nn.Parameter(
+                    torch.empty(lora_dim, shape[1][1])
+                )  # d, 2-mode
+            else:  # Conv2d not tucker
+                # bigger part. weight and LoRA. [b, dim] x [dim, d*k1*k2]
+                self.lokr_w2_a = nn.Parameter(torch.empty(shape[0][1], lora_dim))
+                self.lokr_w2_b = nn.Parameter(
+                    torch.empty(lora_dim, shape[1][1] * shape[2] * shape[3])
+                )
+                # w1 ⊗ (w2_a x w2_b) = (a, b)⊗((c, dim)x(dim, d*k1*k2)) = (a, b)⊗(c, d*k1*k2) = (ac, bd*k1*k2)
+
+            self.op = F.conv2d
+            self.extra_args = {
+                "stride": org_module.stride,
+                "padding": org_module.padding,
+                "dilation": org_module.dilation,
+                "groups": org_module.groups,
+            }
+
+        else:  # Linear
+            in_dim = org_module.in_features
+            out_dim = org_module.out_features
+            self.shape = (out_dim, in_dim)
+
+            in_m, in_n = factorization(in_dim, factor)
+            out_l, out_k = factorization(out_dim, factor)
+            if unbalanced_factorization:
+                out_l, out_k = out_k, out_l
+            shape = (
+                (out_l, out_k),
+                (in_m, in_n),
+            )  # ((a, b), (c, d)), out_dim = a*c, in_dim = b*d
+            # smaller part. weight scale
+            if decompose_both and lora_dim < max(shape[0][0], shape[1][0]) / 2:
+                self.lokr_w1_a = nn.Parameter(torch.empty(shape[0][0], lora_dim))
+                self.lokr_w1_b = nn.Parameter(torch.empty(lora_dim, shape[1][0]))
+            else:
+                self.use_w1 = True
+                self.lokr_w1 = nn.Parameter(
+                    torch.empty(shape[0][0], shape[1][0])
+                )  # a*c, 1-mode
+            if lora_dim < max(shape[0][1], shape[1][1]) / 2:
+                # bigger part. weight and LoRA. [b, dim] x [dim, d]
+                self.lokr_w2_a = nn.Parameter(torch.empty(shape[0][1], lora_dim))
+                self.lokr_w2_b = nn.Parameter(torch.empty(lora_dim, shape[1][1]))
+                # w1 ⊗ (w2_a x w2_b) = (a, b)⊗((c, dim)x(dim, d)) = (a, b)⊗(c, d) = (ac, bd)
+            else:
+                self.use_w2 = True
+                self.lokr_w2 = nn.Parameter(torch.empty(shape[0][1], shape[1][1]))
+
+            self.op = F.linear
+            self.extra_args = {}
+
+        if isinstance(org_module, QuantLinears):
+            if not bypass_mode:
+                log_bypass()
+            bypass_mode = True
+        self.bypass_mode = bypass_mode
+        assert not (
+            bypass_mode and weight_decompose
+        ), "bypass_mode and dora_wd cannot be used together"
+
+        self.wd = weight_decompose
+        if self.wd:
+            org_weight: nn.Parameter = org_module.weight
+            self.dora_norm_dims = org_weight.dim() - 1
+            self.dora_scale = nn.Parameter(
+                torch.norm(
+                    org_weight.transpose(1, 0).reshape(org_weight.shape[1], -1),
+                    dim=1,
+                    keepdim=True,
+                )
+                .reshape(org_weight.shape[1], *[1] * self.dora_norm_dims)
+                .transpose(1, 0)
+            ).float()
+
+        self.dropout = dropout
+        if dropout:
+            print("[WARN]LoHa/LoKr haven't implemented normal dropout yet.")
+        self.rank_dropout = rank_dropout
+        self.rank_dropout_scale = rank_dropout_scale
+        self.module_dropout = module_dropout
+
+        if isinstance(alpha, torch.Tensor):
+            alpha = alpha.detach().float().numpy()  # without casting, bf16 causes error
+        alpha = lora_dim if alpha is None or alpha == 0 else alpha
+        if self.use_w2 and self.use_w1:
+            # use scale = 1
+            alpha = lora_dim
+
+        r_factor = lora_dim
+        if self.rs_lora:
+            r_factor = math.sqrt(r_factor)
+
+        self.scale = alpha / r_factor
+
+        self.register_buffer("alpha", torch.tensor(alpha))  # 定数として扱える
+
+        if use_scalar:
+            self.scalar = nn.Parameter(torch.tensor(0.0))
+        else:
+            self.scalar = torch.tensor(1.0)
+
+        if self.use_w2:
+            if use_scalar:
+                torch.nn.init.kaiming_uniform_(self.lokr_w2, a=math.sqrt(5))
+            else:
+                torch.nn.init.constant_(self.lokr_w2, 0)
+        else:
+            if self.tucker:
+                torch.nn.init.kaiming_uniform_(self.lokr_t2, a=math.sqrt(5))
+            torch.nn.init.kaiming_uniform_(self.lokr_w2_a, a=math.sqrt(5))
+            if use_scalar:
+                torch.nn.init.kaiming_uniform_(self.lokr_w2_b, a=math.sqrt(5))
+            else:
+                torch.nn.init.constant_(self.lokr_w2_b, 0)
+
+        if self.use_w1:
+            torch.nn.init.kaiming_uniform_(self.lokr_w1, a=math.sqrt(5))
+        else:
+            torch.nn.init.kaiming_uniform_(self.lokr_w1_a, a=math.sqrt(5))
+            torch.nn.init.kaiming_uniform_(self.lokr_w1_b, a=math.sqrt(5))
+
+        self.multiplier = multiplier
+        self.org_module = [org_module]
+        self.org_forward = self.org_module[0].forward
+        weight = make_kron(
+            self.lokr_w1 if self.use_w1 else self.lokr_w1_a @ self.lokr_w1_b,
+            (
+                self.lokr_w2
+                if self.use_w2
+                else (
+                    make_weight_tucker(self.lokr_t2, self.lokr_w2_a, self.lokr_w2_b)
+                    if self.tucker
+                    else self.lokr_w2_a @ self.lokr_w2_b
+                )
+            ),
+            torch.tensor(self.multiplier * self.scale),
+        )
+        assert torch.sum(torch.isnan(weight)) == 0, "weight is nan"
+
+    def load_weight_hook(self, module: nn.Module, incompatible_keys):
+        missing_keys = incompatible_keys.missing_keys
+        for key in missing_keys:
+            if "scalar" in key:
+                del missing_keys[missing_keys.index(key)]
+        if isinstance(self.scalar, nn.Parameter):
+            self.scalar.copy_(torch.ones_like(self.scalar))
+        else:
+            self.scalar = torch.ones_like(self.scalar)
+
+    # Same as locon.py
+    def apply_to(self):
+        self.org_forward = self.org_module[0].forward
+        self.org_module[0].forward = self.forward
+
+    def restore(self):
+        self.org_module[0].forward = self.org_forward
+
+    def merge_to(self, multiplier=1.0):
+        weight = self.get_weight(self.shape)
+        self.org_module[0].weight.data.add_(weight * multiplier)
+
+    def get_weight(self, shape):
+        weight = make_kron(
+            self.lokr_w1 if self.use_w1 else self.lokr_w1_a @ self.lokr_w1_b,
+            (
+                self.lokr_w2
+                if self.use_w2
+                else (
+                    make_weight_tucker(self.lokr_t2, self.lokr_w2_a, self.lokr_w2_b)
+                    if self.tucker
+                    else self.lokr_w2_a @ self.lokr_w2_b
+                )
+            ),
+            torch.tensor(self.scale),
+        )
+        if shape is not None:
+            weight = weight.reshape(shape)
+        if self.training and self.rank_dropout:
+            drop = (torch.rand(weight.size(0)) > self.rank_dropout).to(weight.dtype)
+            drop = drop.view(-1, *[1] * len(weight.shape[1:])).to(weight.device)
+            if self.rank_dropout_scale:
+                drop /= drop.mean()
+            weight *= drop
+        return weight
+
+    def apply_weight_decompose(self, weight):
+        weight = weight.to(self.dora_scale.dtype)
+        weight_norm = (
+            weight.transpose(0, 1)
+            .reshape(weight.shape[1], -1)
+            .norm(dim=1, keepdim=True)
+            .reshape(weight.shape[1], *[1] * self.dora_norm_dims)
+            .transpose(0, 1)
+        ) + torch.finfo(weight.dtype).eps
+
+        return weight * (self.dora_scale.to(weight.device) / weight_norm)
+
+    def custom_state_dict(self):
+        destination = {}
+        destination["alpha"] = self.alpha
+        if self.wd:
+            destination["dora_scale"] = self.dora_scale
+        if self.use_w1:
+            destination["lokr_w1"] = self.lokr_w1 * self.scalar
+        else:
+            destination["lokr_w1_a"] = self.lokr_w1_a * self.scalar
+            destination["lokr_w1_b"] = self.lokr_w1_b
+
+        if self.use_w2:
+            destination["lokr_w2"] = self.lokr_w2
+        else:
+            destination["lokr_w2_a"] = self.lokr_w2_a
+            destination["lokr_w2_b"] = self.lokr_w2_b
+            if self.tucker:
+                destination["lokr_t2"] = self.lokr_t2
+        return destination
+
+    @torch.no_grad()
+    def apply_max_norm(self, max_norm, device=None):
+        orig_norm = self.get_weight(self.shape).norm()
+        norm = torch.clamp(orig_norm, max_norm / 2)
+        desired = torch.clamp(norm, max=max_norm)
+        ratio = desired.cpu() / norm.cpu()
+
+        scaled = norm != desired
+        if scaled:
+            modules = 4 - self.use_w1 - self.use_w2 + (not self.use_w2 and self.tucker)
+            if self.use_w1:
+                self.lokr_w1 *= ratio ** (1 / modules)
+            else:
+                self.lokr_w1_a *= ratio ** (1 / modules)
+                self.lokr_w1_b *= ratio ** (1 / modules)
+
+            if self.use_w2:
+                self.lokr_w2 *= ratio ** (1 / modules)
+            else:
+                if self.tucker:
+                    self.lokr_t2 *= ratio ** (1 / modules)
+                self.lokr_w2_a *= ratio ** (1 / modules)
+                self.lokr_w2_b *= ratio ** (1 / modules)
+
+        return scaled, orig_norm * ratio
+
+    def bypass_forward(self, h):
+        if isinstance(self.org_module[0], nn.Conv2d):
+            h = h.transpose(1, -1)
+        if self.use_w2:
+            ba = self.lokr_w2
+        else:
+            a = self.lokr_w2_b
+            b = self.lokr_w2_a
+        if self.use_w1:
+            c = self.lokr_w1
+        else:
+            c = self.lokr_w1_a @ self.lokr_w1_b
+        uq = c.size(1)
+
+        if self.use_w2:
+            vq = ba.size(1)
+            h_in_group = rearrange(h, "b ... (uq vq) -> b ... uq vq", uq=uq, vq=vq)
+            hb = F.linear(h_in_group, ba)
+        else:
+            vq = a.size(1)
+            h_in_group = rearrange(h, "b ... (uq vq) -> b ... uq vq", uq=uq, vq=vq)
+            ha = F.linear(h_in_group, a)
+            hb = F.linear(ha, b)
+
+        h_cross_group = hb.transpose(-1, -2)
+        hc = F.linear(h_cross_group, c)
+
+        h = rearrange(hc, "b ... vp up -> b ... (up vp)")
+        if isinstance(self.org_module[0], nn.Conv2d):
+            h = h.transpose(1, -1)
+
+        return h
+
+    def forward(self, x):
+        if self.module_dropout and self.training:
+            if torch.rand(1) < self.module_dropout:
+                return self.op(
+                    x,
+                    self.org_module[0].weight.data,
+                    (
+                        None
+                        if self.org_module[0].bias is None
+                        else self.org_module[0].bias.data
+                    ),
+                )
+        if self.bypass_mode:
+            if len(self.shape) > 2 and self.shape[2] > 1:
+                return self.org_forward(x) + self.op(
+                    x, self.get_weight(self.shape), **self.extra_args
+                )
+            else:
+                return self.org_forward(x) + self.bypass_forward(x)
+        else:
+            weight = (
+                self.org_module[0].weight.data.to(
+                    x.device, dtype=next(self.parameters()).dtype
+                )
+                + self.get_weight(self.shape) * self.scalar * self.multiplier
+            )
+            bias = (
+                None
+                if self.org_module[0].bias is None
+                else self.org_module[0].bias.data
+            )
+
+            if self.wd:
+                weight = self.apply_weight_decompose(weight)
+            return self.op(x, weight.view(self.shape), bias, **self.extra_args)
+
+
+if __name__ == "__main__":
+    base = nn.Linear(128, 128).cuda()
+    lokr = LokrModule("test", base, 1, 4, 1, weight_decompose=True, factor=8).cuda()
+    print(lokr)
+    test_input = torch.randn(1, 77, 128).cuda()
+    test_output = lokr(test_input)
+    print(test_output.shape)
+
+    # opt = torch.optim.AdamW(lokr.parameters(), lr=1e-2)
+    # for _ in range(100):
+    #     x = torch.randn(128, 128).cuda()
+    #     t = x / 10
+    #     y = lokr(x)
+    #     loss = F.mse_loss(y, t)
+    #     loss.backward()
+    #     opt.step()
+    #     opt.zero_grad()
+    #     print(loss.item())
+
+    base_4bit = LinearNF4(128, 128)
+    base_4bit.load_state_dict(base.state_dict())
+    base_4bit.cuda()
+    qlocon = LokrModule("test", base_4bit, 1, 4, 1, weight_decompose=False).cuda()
+    print(qlocon)
+    test_output2 = qlocon(test_input)
+    print(test_output2.shape)
+    print(F.mse_loss(test_output, test_output2))
+
+    base = nn.Conv2d(128, 128, 3, 1, 1)
+    lokr = LokrModule("test", base, 1, 4, 1, weight_decompose=True, use_tucker=True)
+    print(lokr)
+    test_input = torch.randn(1, 128, 16, 16)
+    test_output = lokr(test_input)
+    print(test_output.shape)
```

### Comparing `lycoris_lora-2.3.0.dev4/lycoris/modules/norms.py` & `lycoris_lora-2.3.0.dev5/lycoris/modules/norms.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,92 +1,92 @@
-import torch
-import torch.nn as nn
-import torch.nn.functional as F
-
-from .base import ModuleCustomSD
-
-
-class NormModule(ModuleCustomSD):
-    """
-    modifed from kohya-ss/sd-scripts/networks/lora:LoRAModule
-    """
-
-    def __init__(
-        self,
-        lora_name,
-        org_module: nn.Module,
-        multiplier=1.0,
-        rank_dropout=0.0,
-        module_dropout=0.0,
-        rank_dropout_scale=False,
-        **kwargs,
-    ):
-        """if alpha == 0 or None, alpha is rank (no scaling)."""
-        super().__init__()
-        self.lora_name = lora_name
-
-        if isinstance(org_module, nn.LayerNorm):
-            self.op = F.layer_norm
-            self.dim = org_module.normalized_shape[0]
-            self.kw_dict = {
-                "normalized_shape": org_module.normalized_shape,
-                "eps": org_module.eps,
-            }
-        elif isinstance(org_module, nn.GroupNorm):
-            self.op = F.group_norm
-            self.group_num = org_module.num_groups
-            self.dim = org_module.num_channels
-            self.kw_dict = {"num_groups": org_module.num_groups, "eps": org_module.eps}
-        else:
-            raise NotImplementedError
-        self.w_norm = nn.Parameter(torch.zeros(self.dim))
-        self.b_norm = nn.Parameter(torch.zeros(self.dim))
-
-        self.rank_dropout = rank_dropout
-        self.rank_dropout_scale = rank_dropout_scale
-        self.module_dropout = module_dropout
-
-        self.multiplier = multiplier
-        self.org_module = [org_module]
-        self.org_forward = self.org_module[0].forward
-
-    def apply_to(self, **kwargs):
-        self.org_forward = self.org_module[0].forward
-        self.org_module[0].forward = self.forward
-
-    def restore(self):
-        self.org_module[0].forward = self.org_forward
-
-    def merge_to(self, multiplier=1.0):
-        weight, bias = self.make_weight(scale=multiplier)
-        self.org_module[0].weight.data.copy_(weight)
-        self.org_module[0].bias.data.copy_(bias)
-
-    def make_weight(self, scale=1, device=None):
-        org_weight = self.org_module[0].weight.to(device, dtype=self.w_norm.dtype)
-        org_bias = self.org_module[0].bias.to(device, dtype=self.b_norm.dtype)
-        if self.rank_dropout and self.training:
-            drop = (torch.rand(self.dim, device=device) < self.rank_dropout).to(
-                self.w_norm.device
-            )
-            if self.rank_dropout_scale:
-                drop /= drop.mean()
-        else:
-            drop = 1
-        drop = (
-            torch.rand(self.dim, device=device) < self.rank_dropout
-            if self.rank_dropout and self.training
-            else 1
-        )
-        weight = self.w_norm.to(device) * drop * scale
-        bias = self.b_norm.to(device) * drop * scale
-        return org_weight + weight, org_bias + bias
-
-    def forward(self, x):
-        if self.module_dropout and self.training:
-            if torch.rand(1) < self.module_dropout:
-                return self.org_forward(x)
-        scale = self.multiplier
-
-        w, b = self.make_weight(scale, x.device)
-        kw_dict = self.kw_dict | {"weight": w, "bias": b}
-        return self.op(x, **kw_dict)
+import torch
+import torch.nn as nn
+import torch.nn.functional as F
+
+from .base import ModuleCustomSD
+
+
+class NormModule(ModuleCustomSD):
+    """
+    modifed from kohya-ss/sd-scripts/networks/lora:LoRAModule
+    """
+
+    def __init__(
+        self,
+        lora_name,
+        org_module: nn.Module,
+        multiplier=1.0,
+        rank_dropout=0.0,
+        module_dropout=0.0,
+        rank_dropout_scale=False,
+        **kwargs,
+    ):
+        """if alpha == 0 or None, alpha is rank (no scaling)."""
+        super().__init__()
+        self.lora_name = lora_name
+
+        if isinstance(org_module, nn.LayerNorm):
+            self.op = F.layer_norm
+            self.dim = org_module.normalized_shape[0]
+            self.kw_dict = {
+                "normalized_shape": org_module.normalized_shape,
+                "eps": org_module.eps,
+            }
+        elif isinstance(org_module, nn.GroupNorm):
+            self.op = F.group_norm
+            self.group_num = org_module.num_groups
+            self.dim = org_module.num_channels
+            self.kw_dict = {"num_groups": org_module.num_groups, "eps": org_module.eps}
+        else:
+            raise NotImplementedError
+        self.w_norm = nn.Parameter(torch.zeros(self.dim))
+        self.b_norm = nn.Parameter(torch.zeros(self.dim))
+
+        self.rank_dropout = rank_dropout
+        self.rank_dropout_scale = rank_dropout_scale
+        self.module_dropout = module_dropout
+
+        self.multiplier = multiplier
+        self.org_module = [org_module]
+        self.org_forward = self.org_module[0].forward
+
+    def apply_to(self, **kwargs):
+        self.org_forward = self.org_module[0].forward
+        self.org_module[0].forward = self.forward
+
+    def restore(self):
+        self.org_module[0].forward = self.org_forward
+
+    def merge_to(self, multiplier=1.0):
+        weight, bias = self.make_weight(scale=multiplier)
+        self.org_module[0].weight.data.copy_(weight)
+        self.org_module[0].bias.data.copy_(bias)
+
+    def make_weight(self, scale=1, device=None):
+        org_weight = self.org_module[0].weight.to(device, dtype=self.w_norm.dtype)
+        org_bias = self.org_module[0].bias.to(device, dtype=self.b_norm.dtype)
+        if self.rank_dropout and self.training:
+            drop = (torch.rand(self.dim, device=device) < self.rank_dropout).to(
+                self.w_norm.device
+            )
+            if self.rank_dropout_scale:
+                drop /= drop.mean()
+        else:
+            drop = 1
+        drop = (
+            torch.rand(self.dim, device=device) < self.rank_dropout
+            if self.rank_dropout and self.training
+            else 1
+        )
+        weight = self.w_norm.to(device) * drop * scale
+        bias = self.b_norm.to(device) * drop * scale
+        return org_weight + weight, org_bias + bias
+
+    def forward(self, x):
+        if self.module_dropout and self.training:
+            if torch.rand(1) < self.module_dropout:
+                return self.org_forward(x)
+        scale = self.multiplier
+
+        w, b = self.make_weight(scale, x.device)
+        kw_dict = self.kw_dict | {"weight": w, "bias": b}
+        return self.op(x, **kw_dict)
```

### Comparing `lycoris_lora-2.3.0.dev4/lycoris/utils/__init__.py` & `lycoris_lora-2.3.0.dev5/lycoris/utils/__init__.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,640 +1,640 @@
-import re
-from typing import Dict, Tuple, Union
-
-import numpy as np
-
-import torch
-import torch.nn as nn
-import torch.nn.functional as F
-
-import torch.linalg as linalg
-
-from tqdm import tqdm
-
-
-def str_bool(val):
-    return str(val).lower() != "false"
-
-
-def default(val, d):
-    return val if val is not None else d
-
-
-def make_sparse(t: torch.Tensor, sparsity=0.95):
-    abs_t = torch.abs(t)
-    np_array = abs_t.detach().cpu().numpy()
-    quan = float(np.quantile(np_array, sparsity))
-    sparse_t = t.masked_fill(abs_t < quan, 0)
-    return sparse_t
-
-
-def extract_conv(
-    weight: Union[torch.Tensor, nn.Parameter],
-    mode="fixed",
-    mode_param=0,
-    device="cpu",
-    is_cp=False,
-) -> Tuple[nn.Parameter, nn.Parameter]:
-    weight = weight.to(device)
-    out_ch, in_ch, kernel_size, _ = weight.shape
-
-    U, S, Vh = linalg.svd(weight.reshape(out_ch, -1))
-
-    if mode == "full":
-        return weight, "full"
-    elif mode == "fixed":
-        lora_rank = mode_param
-    elif mode == "threshold":
-        assert mode_param >= 0
-        lora_rank = torch.sum(S > mode_param)
-    elif mode == "ratio":
-        assert 1 >= mode_param >= 0
-        min_s = torch.max(S) * mode_param
-        lora_rank = torch.sum(S > min_s)
-    elif mode == "quantile" or mode == "percentile":
-        assert 1 >= mode_param >= 0
-        s_cum = torch.cumsum(S, dim=0)
-        min_cum_sum = mode_param * torch.sum(S)
-        lora_rank = torch.sum(s_cum < min_cum_sum)
-    else:
-        raise NotImplementedError(
-            'Extract mode should be "fixed", "threshold", "ratio" or "quantile"'
-        )
-    lora_rank = max(1, lora_rank)
-    lora_rank = min(out_ch, in_ch, lora_rank)
-    if lora_rank >= out_ch / 2 and not is_cp:
-        return weight, "full"
-
-    U = U[:, :lora_rank]
-    S = S[:lora_rank]
-    U = U @ torch.diag(S).to(device)
-    Vh = Vh[:lora_rank, :]
-
-    diff = (weight - (U @ Vh).reshape(out_ch, in_ch, kernel_size, kernel_size)).detach()
-    extract_weight_A = Vh.reshape(lora_rank, in_ch, kernel_size, kernel_size).detach()
-    extract_weight_B = U.reshape(out_ch, lora_rank, 1, 1).detach()
-    del U, S, Vh, weight
-    return (extract_weight_A, extract_weight_B, diff), "low rank"
-
-
-def extract_linear(
-    weight: Union[torch.Tensor, nn.Parameter],
-    mode="fixed",
-    mode_param=0,
-    device="cpu",
-) -> Tuple[nn.Parameter, nn.Parameter]:
-    weight = weight.to(device)
-    out_ch, in_ch = weight.shape
-
-    U, S, Vh = linalg.svd(weight)
-
-    if mode == "full":
-        return weight, "full"
-    elif mode == "fixed":
-        lora_rank = mode_param
-    elif mode == "threshold":
-        assert mode_param >= 0
-        lora_rank = torch.sum(S > mode_param)
-    elif mode == "ratio":
-        assert 1 >= mode_param >= 0
-        min_s = torch.max(S) * mode_param
-        lora_rank = torch.sum(S > min_s)
-    elif mode == "quantile" or mode == "percentile":
-        assert 1 >= mode_param >= 0
-        s_cum = torch.cumsum(S, dim=0)
-        min_cum_sum = mode_param * torch.sum(S)
-        lora_rank = torch.sum(s_cum < min_cum_sum)
-    else:
-        raise NotImplementedError(
-            'Extract mode should be "fixed", "threshold", "ratio" or "quantile"'
-        )
-    lora_rank = max(1, lora_rank)
-    lora_rank = min(out_ch, in_ch, lora_rank)
-    if lora_rank >= out_ch / 2:
-        return weight, "full"
-
-    U = U[:, :lora_rank]
-    S = S[:lora_rank]
-    U = U @ torch.diag(S).to(device)
-    Vh = Vh[:lora_rank, :]
-
-    diff = (weight - U @ Vh).detach()
-    extract_weight_A = Vh.reshape(lora_rank, in_ch).detach()
-    extract_weight_B = U.reshape(out_ch, lora_rank).detach()
-    del U, S, Vh, weight
-    return (extract_weight_A, extract_weight_B, diff), "low rank"
-
-
-@torch.no_grad()
-def extract_diff(
-    base_tes,
-    db_tes,
-    base_unet,
-    db_unet,
-    mode="fixed",
-    linear_mode_param=0,
-    conv_mode_param=0,
-    extract_device="cpu",
-    use_bias=False,
-    sparsity=0.98,
-    small_conv=True,
-):
-    UNET_TARGET_REPLACE_MODULE = [
-        "Linear",
-        "Conv2d",
-        "LayerNorm",
-        "GroupNorm",
-        "GroupNorm32",
-    ]
-    TEXT_ENCODER_TARGET_REPLACE_MODULE = [
-        "Embedding",
-        "Linear",
-        "Conv2d",
-        "LayerNorm",
-        "GroupNorm",
-        "GroupNorm32",
-    ]
-    LORA_PREFIX_UNET = "lora_unet"
-    LORA_PREFIX_TEXT_ENCODER = "lora_te"
-
-    def make_state_dict(
-        prefix,
-        root_module: torch.nn.Module,
-        target_module: torch.nn.Module,
-        target_replace_modules,
-    ):
-        loras = {}
-        temp = {}
-
-        for name, module in root_module.named_modules():
-            if module.__class__.__name__ in target_replace_modules:
-                temp[name] = module
-
-        for name, module in tqdm(
-            list((n, m) for n, m in target_module.named_modules() if n in temp)
-        ):
-            weights = temp[name]
-            lora_name = prefix + "." + name
-            lora_name = lora_name.replace(".", "_")
-            layer = module.__class__.__name__
-
-            if layer in {
-                "Linear",
-                "Conv2d",
-                "LayerNorm",
-                "GroupNorm",
-                "GroupNorm32",
-                "Embedding",
-            }:
-                root_weight = module.weight
-                if torch.allclose(root_weight, weights.weight):
-                    continue
-            else:
-                continue
-            module = module.to(extract_device)
-            weights = weights.to(extract_device)
-
-            if mode == "full":
-                decompose_mode = "full"
-            elif layer == "Linear":
-                weight, decompose_mode = extract_linear(
-                    (root_weight - weights.weight),
-                    mode,
-                    linear_mode_param,
-                    device=extract_device,
-                )
-                if decompose_mode == "low rank":
-                    extract_a, extract_b, diff = weight
-            elif layer == "Conv2d":
-                is_linear = root_weight.shape[2] == 1 and root_weight.shape[3] == 1
-                weight, decompose_mode = extract_conv(
-                    (root_weight - weights.weight),
-                    mode,
-                    linear_mode_param if is_linear else conv_mode_param,
-                    device=extract_device,
-                )
-                if decompose_mode == "low rank":
-                    extract_a, extract_b, diff = weight
-                if small_conv and not is_linear and decompose_mode == "low rank":
-                    dim = extract_a.size(0)
-                    (extract_c, extract_a, _), _ = extract_conv(
-                        extract_a.transpose(0, 1),
-                        "fixed",
-                        dim,
-                        extract_device,
-                        True,
-                    )
-                    extract_a = extract_a.transpose(0, 1)
-                    extract_c = extract_c.transpose(0, 1)
-                    loras[f"{lora_name}.lora_mid.weight"] = (
-                        extract_c.detach().cpu().contiguous().half()
-                    )
-                    diff = (
-                        (
-                            root_weight
-                            - torch.einsum(
-                                "i j k l, j r, p i -> p r k l",
-                                extract_c,
-                                extract_a.flatten(1, -1),
-                                extract_b.flatten(1, -1),
-                            )
-                        )
-                        .detach()
-                        .cpu()
-                        .contiguous()
-                    )
-                    del extract_c
-            else:
-                module = module.to("cpu")
-                weights = weights.to("cpu")
-                continue
-
-            if decompose_mode == "low rank":
-                loras[f"{lora_name}.lora_down.weight"] = (
-                    extract_a.detach().cpu().contiguous().half()
-                )
-                loras[f"{lora_name}.lora_up.weight"] = (
-                    extract_b.detach().cpu().contiguous().half()
-                )
-                loras[f"{lora_name}.alpha"] = torch.Tensor([extract_a.shape[0]]).half()
-                if use_bias:
-                    diff = diff.detach().cpu().reshape(extract_b.size(0), -1)
-                    sparse_diff = make_sparse(diff, sparsity).to_sparse().coalesce()
-
-                    indices = sparse_diff.indices().to(torch.int16)
-                    values = sparse_diff.values().half()
-                    loras[f"{lora_name}.bias_indices"] = indices
-                    loras[f"{lora_name}.bias_values"] = values
-                    loras[f"{lora_name}.bias_size"] = torch.tensor(diff.shape).to(
-                        torch.int16
-                    )
-                del extract_a, extract_b, diff
-            elif decompose_mode == "full":
-                if "Norm" in layer:
-                    w_key = "w_norm"
-                    b_key = "b_norm"
-                else:
-                    w_key = "diff"
-                    b_key = "diff_b"
-                weight_diff = module.weight - weights.weight
-                loras[f"{lora_name}.{w_key}"] = (
-                    weight_diff.detach().cpu().contiguous().half()
-                )
-                if getattr(weights, "bias", None) is not None:
-                    bias_diff = module.bias - weights.bias
-                    loras[f"{lora_name}.{b_key}"] = (
-                        bias_diff.detach().cpu().contiguous().half()
-                    )
-            else:
-                raise NotImplementedError
-            module = module.to("cpu")
-            weights = weights.to("cpu")
-        return loras
-
-    all_loras = {}
-
-    all_loras |= make_state_dict(
-        LORA_PREFIX_UNET,
-        base_unet,
-        db_unet,
-        UNET_TARGET_REPLACE_MODULE,
-    )
-    del base_unet, db_unet
-    if torch.cuda.is_available():
-        torch.cuda.empty_cache()
-
-    for idx, (te1, te2) in enumerate(zip(base_tes, db_tes)):
-        if len(base_tes) > 1:
-            prefix = f"{LORA_PREFIX_TEXT_ENCODER}{idx+1}"
-        else:
-            prefix = LORA_PREFIX_TEXT_ENCODER
-        all_loras |= make_state_dict(
-            prefix,
-            te1,
-            te2,
-            TEXT_ENCODER_TARGET_REPLACE_MODULE,
-        )
-        del te1, te2
-
-    all_lora_name = set()
-    for k in all_loras:
-        lora_name, weight = k.rsplit(".", 1)
-        all_lora_name.add(lora_name)
-    print(len(all_lora_name))
-    return all_loras
-
-
-re_digits = re.compile(r"\d+")
-re_compiled = {}
-
-suffix_conversion = {
-    "attentions": {},
-    "resnets": {
-        "conv1": "in_layers_2",
-        "conv2": "out_layers_3",
-        "norm1": "in_layers_0",
-        "norm2": "out_layers_0",
-        "time_emb_proj": "emb_layers_1",
-        "conv_shortcut": "skip_connection",
-    },
-}
-
-
-def convert_diffusers_name_to_compvis(key):
-    def match(match_list, regex_text):
-        regex = re_compiled.get(regex_text)
-        if regex is None:
-            regex = re.compile(regex_text)
-            re_compiled[regex_text] = regex
-
-        r = re.match(regex, key)
-        if not r:
-            return False
-
-        match_list.clear()
-        match_list.extend([int(x) if re.match(re_digits, x) else x for x in r.groups()])
-        return True
-
-    m = []
-
-    if match(m, r"lora_unet_conv_in(.*)"):
-        return f"lora_unet_input_blocks_0_0{m[0]}"
-
-    if match(m, r"lora_unet_conv_out(.*)"):
-        return f"lora_unet_out_2{m[0]}"
-
-    if match(m, r"lora_unet_time_embedding_linear_(\d+)(.*)"):
-        return f"lora_unet_time_embed_{m[0] * 2 - 2}{m[1]}"
-
-    if match(m, r"lora_unet_down_blocks_(\d+)_(attentions|resnets)_(\d+)_(.+)"):
-        suffix = suffix_conversion.get(m[1], {}).get(m[3], m[3])
-        return f"lora_unet_input_blocks_{1 + m[0] * 3 + m[2]}_{1 if m[1] == 'attentions' else 0}_{suffix}"
-
-    if match(m, r"lora_unet_mid_block_(attentions|resnets)_(\d+)_(.+)"):
-        suffix = suffix_conversion.get(m[0], {}).get(m[2], m[2])
-        return (
-            f"lora_unet_middle_block_{1 if m[0] == 'attentions' else m[1] * 2}_{suffix}"
-        )
-
-    if match(m, r"lora_unet_up_blocks_(\d+)_(attentions|resnets)_(\d+)_(.+)"):
-        suffix = suffix_conversion.get(m[1], {}).get(m[3], m[3])
-        return f"lora_unet_output_blocks_{m[0] * 3 + m[2]}_{1 if m[1] == 'attentions' else 0}_{suffix}"
-
-    if match(m, r"lora_unet_down_blocks_(\d+)_downsamplers_0_conv"):
-        return f"lora_unet_input_blocks_{3 + m[0] * 3}_0_op"
-
-    if match(m, r"lora_unet_up_blocks_(\d+)_upsamplers_0_conv"):
-        return f"lora_unet_output_blocks_{2 + m[0] * 3}_2_conv"
-    return key
-
-
-def get_module(lyco_state_dict: Dict, lora_name):
-    if f"{lora_name}.lora_up.weight" in lyco_state_dict:
-        up = lyco_state_dict[f"{lora_name}.lora_up.weight"]
-        down = lyco_state_dict[f"{lora_name}.lora_down.weight"]
-        mid = lyco_state_dict.get(f"{lora_name}.lora_mid.weight", None)
-        alpha = lyco_state_dict.get(f"{lora_name}.alpha", None)
-        dora_scale = lyco_state_dict.get(f"{lora_name}.dora_scale", None)
-        return "locon", (up, down, mid, alpha, dora_scale)
-    elif f"{lora_name}.hada_w1_a" in lyco_state_dict:
-        w1a = lyco_state_dict[f"{lora_name}.hada_w1_a"]
-        w1b = lyco_state_dict[f"{lora_name}.hada_w1_b"]
-        w2a = lyco_state_dict[f"{lora_name}.hada_w2_a"]
-        w2b = lyco_state_dict[f"{lora_name}.hada_w2_b"]
-        t1 = lyco_state_dict.get(f"{lora_name}.hada_t1", None)
-        t2 = lyco_state_dict.get(f"{lora_name}.hada_t2", None)
-        alpha = lyco_state_dict.get(f"{lora_name}.alpha", None)
-        dora_scale = lyco_state_dict.get(f"{lora_name}.dora_scale", None)
-        return "hada", (w1a, w1b, w2a, w2b, t1, t2, alpha, dora_scale)
-    elif f"{lora_name}.weight" in lyco_state_dict:
-        weight = lyco_state_dict[f"{lora_name}.weight"]
-        on_input = lyco_state_dict.get(f"{lora_name}.on_input", False)
-        return "ia3", (weight, on_input)
-    elif (
-        f"{lora_name}.lokr_w1" in lyco_state_dict
-        or f"{lora_name}.lokr_w1_a" in lyco_state_dict
-    ):
-        w1 = lyco_state_dict.get(f"{lora_name}.lokr_w1", None)
-        w1a = lyco_state_dict.get(f"{lora_name}.lokr_w1_a", None)
-        w1b = lyco_state_dict.get(f"{lora_name}.lokr_w1_b", None)
-        w2 = lyco_state_dict.get(f"{lora_name}.lokr_w2", None)
-        w2a = lyco_state_dict.get(f"{lora_name}.lokr_w2_a", None)
-        w2b = lyco_state_dict.get(f"{lora_name}.lokr_w2_b", None)
-        t1 = lyco_state_dict.get(f"{lora_name}.lokr_t1", None)
-        t2 = lyco_state_dict.get(f"{lora_name}.lokr_t2", None)
-        alpha = lyco_state_dict.get(f"{lora_name}.alpha", None)
-        dora_scale = lyco_state_dict.get(f"{lora_name}.dora_scale", None)
-        return "kron", (w1, w1a, w1b, w2, w2a, w2b, t1, t2, alpha, dora_scale)
-    elif f"{lora_name}.diff" in lyco_state_dict:
-        diff = lyco_state_dict[f"{lora_name}.diff"]
-        diff_b = lyco_state_dict.get(f"{lora_name}.diff_b", None)
-        return "full", (diff, diff_b)
-    elif f"{lora_name}.w_norm" in lyco_state_dict:
-        w_norm = lyco_state_dict[f"{lora_name}.w_norm"]
-        b_norm = lyco_state_dict.get(f"{lora_name}.b_norm", None)
-        return "norm", (w_norm, b_norm)
-    else:
-        return "None", ()
-
-
-def tucker_weight_from_conv(up, down, mid):
-    up = up.reshape(up.size(0), up.size(1))
-    down = down.reshape(down.size(0), down.size(1))
-    return torch.einsum("m n w h, i m, n j -> i j w h", mid, up, down)
-
-
-def tucker_weight(wa, wb, t):
-    temp = torch.einsum("i j k l, j r -> i r k l", t, wb)
-    return torch.einsum("i j k l, i r -> r j k l", temp, wa)
-
-
-def apply_dora_scale(org_weight, rebuild, dora_scale, scale):
-    dora_norm_dims = org_weight.dim() - 1
-    weight = org_weight + rebuild
-    weight = weight.to(dora_scale.dtype)
-    weight_norm = (
-        weight.transpose(0, 1)
-        .reshape(weight.shape[1], -1)
-        .norm(dim=1, keepdim=True)
-        .reshape(weight.shape[1], *[1] * dora_norm_dims)
-        .transpose(0, 1)
-    )
-    merged_scale1 = weight / weight_norm * dora_scale
-    diff_weight = merged_scale1 - org_weight
-    return org_weight + diff_weight * scale
-
-
-@torch.no_grad()
-def rebuild_weight(module_type, params, orig_weight, orig_bias, scale=1):
-    if orig_weight is None:
-        return None, None
-    merged = orig_weight
-    merged_bias = orig_bias
-    if module_type == "locon":
-        up, down, mid, alpha, dora_scale = params
-        if alpha is not None:
-            scale *= alpha / up.size(1)
-        if mid is not None:
-            rebuild = tucker_weight_from_conv(up, down, mid)
-        else:
-            rebuild = up.reshape(up.size(0), -1) @ down.reshape(down.size(0), -1)
-        rebuild = rebuild.reshape(orig_weight.shape)
-        if dora_scale is None:
-            merged = orig_weight + rebuild * scale
-        else:
-            merged = apply_dora_scale(orig_weight, rebuild, dora_scale, scale)
-        del up, down, mid, alpha, params, rebuild
-    elif module_type == "hada":
-        w1a, w1b, w2a, w2b, t1, t2, alpha, dora_scale = params
-        if alpha is not None:
-            scale *= alpha / w1b.size(0)
-        if t1 is not None:
-            rebuild1 = tucker_weight(w1a, w1b, t1)
-        else:
-            rebuild1 = w1a @ w1b
-        if t2 is not None:
-            rebuild2 = tucker_weight(w2a, w2b, t2)
-        else:
-            rebuild2 = w2a @ w2b
-        rebuild = (rebuild1 * rebuild2).reshape(orig_weight.shape)
-        if dora_scale is None:
-            merged = orig_weight + rebuild * scale
-        else:
-            merged = apply_dora_scale(orig_weight, rebuild, dora_scale, scale)
-        del w1a, w1b, w2a, w2b, t1, t2, alpha, params, rebuild, rebuild1, rebuild2
-    elif module_type == "ia3":
-        weight, on_input = params
-        if not on_input:
-            weight = weight.reshape(-1, 1)
-        merged = orig_weight + weight * orig_weight * scale
-        del weight, on_input, params
-    elif module_type == "kron":
-        w1, w1a, w1b, w2, w2a, w2b, t1, t2, alpha, dora_scale = params
-        if alpha is not None and (w1b is not None or w2b is not None):
-            scale *= alpha / (w1b.size(0) if w1b else w2b.size(0))
-        if w1a is not None and w1b is not None:
-            if t1 is not None:
-                w1 = tucker_weight(w1a, w1b, t1)
-            else:
-                w1 = w1a @ w1b
-        if w2a is not None and w2b is not None:
-            if t2 is not None:
-                w2 = tucker_weight(w2a, w2b, t2)
-            else:
-                w2 = w2a @ w2b
-        if len(w2.shape) == 4:
-            w1 = w1.unsqueeze(2).unsqueeze(2)
-        w2 = w2.contiguous()
-        rebuild = torch.kron(w1, w2).reshape(orig_weight.shape)
-        if dora_scale is None:
-            merged = orig_weight + rebuild * scale
-        else:
-            merged = apply_dora_scale(orig_weight, rebuild, dora_scale, scale)
-        del w1, w1a, w1b, w2, w2a, w2b, t1, t2, alpha, params, rebuild
-    elif module_type == "full":
-        rebuild = params[0].reshape(orig_weight.shape)
-        rebuild_b = (
-            params[1].reshape(orig_bias.shape) if orig_bias is not None else None
-        )
-        merged = orig_weight + rebuild * scale
-        if rebuild_b is not None:
-            merged_bias = orig_bias + rebuild_b * scale
-        del params, rebuild, rebuild_b
-    elif module_type == "norm":
-        rebuild = params[0].reshape(orig_weight.shape)
-        rebuild_b = params[1].reshape(orig_bias.shape)
-        merged = orig_weight + rebuild * scale
-        merged_bias = orig_bias + rebuild_b * scale
-    else:
-        return None, None
-
-    return merged, merged_bias
-
-
-@torch.no_grad()
-def merge(tes, unet, lyco_state_dict, scale: float = 1.0, device="cpu"):
-    UNET_TARGET_REPLACE_MODULE = [
-        "Linear",
-        "Conv2d",
-        "LayerNorm",
-        "GroupNorm",
-        "GroupNorm32",
-    ]
-    TEXT_ENCODER_TARGET_REPLACE_MODULE = [
-        "Embedding",
-        "Linear",
-        "Conv2d",
-        "LayerNorm",
-        "GroupNorm",
-        "GroupNorm32",
-        "Embedding",
-    ]
-    LORA_PREFIX_UNET = "lora_unet"
-    LORA_PREFIX_TEXT_ENCODER = "lora_te"
-    merged = 0
-
-    def merge_state_dict(
-        prefix,
-        root_module: torch.nn.Module,
-        lyco_state_dict: Dict[str, torch.Tensor],
-        target_replace_modules,
-    ):
-        nonlocal merged
-        for child_name, child_module in tqdm(
-            list(root_module.named_modules()), desc=f"Merging {prefix}"
-        ):
-            if child_module.__class__.__name__ in target_replace_modules:
-                lora_name = prefix + "." + child_name
-                lora_name = lora_name.replace(".", "_")
-
-                result, result_b = rebuild_weight(
-                    *get_module(lyco_state_dict, lora_name),
-                    getattr(child_module, "weight"),
-                    getattr(child_module, "bias", None),
-                    scale,
-                )
-                if result is not None:
-                    key_dict.pop(lora_name)
-                    merged += 1
-                    child_module.requires_grad_(False)
-                    child_module.weight.copy_(result)
-                if result_b is not None:
-                    child_module.bias.copy_(result_b)
-
-    key_dict = {}
-    for k, v in tqdm(list(lyco_state_dict.items()), desc="Converting Dtype and Device"):
-        module, weight_key = k.split(".", 1)
-        convert_key = convert_diffusers_name_to_compvis(module)
-        if convert_key != module and len(tes) > 1:
-            # kohya's format for sdxl is as same as SGM, not diffusers
-            del lyco_state_dict[k]
-            key_dict[convert_key] = key_dict.get(convert_key, []) + [k]
-            k = f"{convert_key}.{weight_key}"
-        else:
-            key_dict[module] = key_dict.get(module, []) + [k]
-        if device == "cpu":
-            lyco_state_dict[k] = v.float().cpu()
-        else:
-            lyco_state_dict[k] = v.to(
-                device, dtype=tes[0].parameters().__next__().dtype
-            )
-
-    for idx, te in enumerate(tes):
-        if len(tes) > 1:
-            prefix = LORA_PREFIX_TEXT_ENCODER + str(idx + 1)
-        else:
-            prefix = LORA_PREFIX_TEXT_ENCODER
-        merge_state_dict(
-            prefix,
-            te.to(device),
-            lyco_state_dict,
-            TEXT_ENCODER_TARGET_REPLACE_MODULE,
-        )
-    merge_state_dict(
-        LORA_PREFIX_UNET,
-        unet.to(device),
-        lyco_state_dict,
-        UNET_TARGET_REPLACE_MODULE,
-    )
-    print(f"Unused state dict key: {key_dict}")
-    print(f"{merged} Modules been merged")
+import re
+from typing import Dict, Tuple, Union
+
+import numpy as np
+
+import torch
+import torch.nn as nn
+import torch.nn.functional as F
+
+import torch.linalg as linalg
+
+from tqdm import tqdm
+
+
+def str_bool(val):
+    return str(val).lower() != "false"
+
+
+def default(val, d):
+    return val if val is not None else d
+
+
+def make_sparse(t: torch.Tensor, sparsity=0.95):
+    abs_t = torch.abs(t)
+    np_array = abs_t.detach().cpu().numpy()
+    quan = float(np.quantile(np_array, sparsity))
+    sparse_t = t.masked_fill(abs_t < quan, 0)
+    return sparse_t
+
+
+def extract_conv(
+    weight: Union[torch.Tensor, nn.Parameter],
+    mode="fixed",
+    mode_param=0,
+    device="cpu",
+    is_cp=False,
+) -> Tuple[nn.Parameter, nn.Parameter]:
+    weight = weight.to(device)
+    out_ch, in_ch, kernel_size, _ = weight.shape
+
+    U, S, Vh = linalg.svd(weight.reshape(out_ch, -1))
+
+    if mode == "full":
+        return weight, "full"
+    elif mode == "fixed":
+        lora_rank = mode_param
+    elif mode == "threshold":
+        assert mode_param >= 0
+        lora_rank = torch.sum(S > mode_param)
+    elif mode == "ratio":
+        assert 1 >= mode_param >= 0
+        min_s = torch.max(S) * mode_param
+        lora_rank = torch.sum(S > min_s)
+    elif mode == "quantile" or mode == "percentile":
+        assert 1 >= mode_param >= 0
+        s_cum = torch.cumsum(S, dim=0)
+        min_cum_sum = mode_param * torch.sum(S)
+        lora_rank = torch.sum(s_cum < min_cum_sum)
+    else:
+        raise NotImplementedError(
+            'Extract mode should be "fixed", "threshold", "ratio" or "quantile"'
+        )
+    lora_rank = max(1, lora_rank)
+    lora_rank = min(out_ch, in_ch, lora_rank)
+    if lora_rank >= out_ch / 2 and not is_cp:
+        return weight, "full"
+
+    U = U[:, :lora_rank]
+    S = S[:lora_rank]
+    U = U @ torch.diag(S).to(device)
+    Vh = Vh[:lora_rank, :]
+
+    diff = (weight - (U @ Vh).reshape(out_ch, in_ch, kernel_size, kernel_size)).detach()
+    extract_weight_A = Vh.reshape(lora_rank, in_ch, kernel_size, kernel_size).detach()
+    extract_weight_B = U.reshape(out_ch, lora_rank, 1, 1).detach()
+    del U, S, Vh, weight
+    return (extract_weight_A, extract_weight_B, diff), "low rank"
+
+
+def extract_linear(
+    weight: Union[torch.Tensor, nn.Parameter],
+    mode="fixed",
+    mode_param=0,
+    device="cpu",
+) -> Tuple[nn.Parameter, nn.Parameter]:
+    weight = weight.to(device)
+    out_ch, in_ch = weight.shape
+
+    U, S, Vh = linalg.svd(weight)
+
+    if mode == "full":
+        return weight, "full"
+    elif mode == "fixed":
+        lora_rank = mode_param
+    elif mode == "threshold":
+        assert mode_param >= 0
+        lora_rank = torch.sum(S > mode_param)
+    elif mode == "ratio":
+        assert 1 >= mode_param >= 0
+        min_s = torch.max(S) * mode_param
+        lora_rank = torch.sum(S > min_s)
+    elif mode == "quantile" or mode == "percentile":
+        assert 1 >= mode_param >= 0
+        s_cum = torch.cumsum(S, dim=0)
+        min_cum_sum = mode_param * torch.sum(S)
+        lora_rank = torch.sum(s_cum < min_cum_sum)
+    else:
+        raise NotImplementedError(
+            'Extract mode should be "fixed", "threshold", "ratio" or "quantile"'
+        )
+    lora_rank = max(1, lora_rank)
+    lora_rank = min(out_ch, in_ch, lora_rank)
+    if lora_rank >= out_ch / 2:
+        return weight, "full"
+
+    U = U[:, :lora_rank]
+    S = S[:lora_rank]
+    U = U @ torch.diag(S).to(device)
+    Vh = Vh[:lora_rank, :]
+
+    diff = (weight - U @ Vh).detach()
+    extract_weight_A = Vh.reshape(lora_rank, in_ch).detach()
+    extract_weight_B = U.reshape(out_ch, lora_rank).detach()
+    del U, S, Vh, weight
+    return (extract_weight_A, extract_weight_B, diff), "low rank"
+
+
+@torch.no_grad()
+def extract_diff(
+    base_tes,
+    db_tes,
+    base_unet,
+    db_unet,
+    mode="fixed",
+    linear_mode_param=0,
+    conv_mode_param=0,
+    extract_device="cpu",
+    use_bias=False,
+    sparsity=0.98,
+    small_conv=True,
+):
+    UNET_TARGET_REPLACE_MODULE = [
+        "Linear",
+        "Conv2d",
+        "LayerNorm",
+        "GroupNorm",
+        "GroupNorm32",
+    ]
+    TEXT_ENCODER_TARGET_REPLACE_MODULE = [
+        "Embedding",
+        "Linear",
+        "Conv2d",
+        "LayerNorm",
+        "GroupNorm",
+        "GroupNorm32",
+    ]
+    LORA_PREFIX_UNET = "lora_unet"
+    LORA_PREFIX_TEXT_ENCODER = "lora_te"
+
+    def make_state_dict(
+        prefix,
+        root_module: torch.nn.Module,
+        target_module: torch.nn.Module,
+        target_replace_modules,
+    ):
+        loras = {}
+        temp = {}
+
+        for name, module in root_module.named_modules():
+            if module.__class__.__name__ in target_replace_modules:
+                temp[name] = module
+
+        for name, module in tqdm(
+            list((n, m) for n, m in target_module.named_modules() if n in temp)
+        ):
+            weights = temp[name]
+            lora_name = prefix + "." + name
+            lora_name = lora_name.replace(".", "_")
+            layer = module.__class__.__name__
+
+            if layer in {
+                "Linear",
+                "Conv2d",
+                "LayerNorm",
+                "GroupNorm",
+                "GroupNorm32",
+                "Embedding",
+            }:
+                root_weight = module.weight
+                if torch.allclose(root_weight, weights.weight):
+                    continue
+            else:
+                continue
+            module = module.to(extract_device)
+            weights = weights.to(extract_device)
+
+            if mode == "full":
+                decompose_mode = "full"
+            elif layer == "Linear":
+                weight, decompose_mode = extract_linear(
+                    (root_weight - weights.weight),
+                    mode,
+                    linear_mode_param,
+                    device=extract_device,
+                )
+                if decompose_mode == "low rank":
+                    extract_a, extract_b, diff = weight
+            elif layer == "Conv2d":
+                is_linear = root_weight.shape[2] == 1 and root_weight.shape[3] == 1
+                weight, decompose_mode = extract_conv(
+                    (root_weight - weights.weight),
+                    mode,
+                    linear_mode_param if is_linear else conv_mode_param,
+                    device=extract_device,
+                )
+                if decompose_mode == "low rank":
+                    extract_a, extract_b, diff = weight
+                if small_conv and not is_linear and decompose_mode == "low rank":
+                    dim = extract_a.size(0)
+                    (extract_c, extract_a, _), _ = extract_conv(
+                        extract_a.transpose(0, 1),
+                        "fixed",
+                        dim,
+                        extract_device,
+                        True,
+                    )
+                    extract_a = extract_a.transpose(0, 1)
+                    extract_c = extract_c.transpose(0, 1)
+                    loras[f"{lora_name}.lora_mid.weight"] = (
+                        extract_c.detach().cpu().contiguous().half()
+                    )
+                    diff = (
+                        (
+                            root_weight
+                            - torch.einsum(
+                                "i j k l, j r, p i -> p r k l",
+                                extract_c,
+                                extract_a.flatten(1, -1),
+                                extract_b.flatten(1, -1),
+                            )
+                        )
+                        .detach()
+                        .cpu()
+                        .contiguous()
+                    )
+                    del extract_c
+            else:
+                module = module.to("cpu")
+                weights = weights.to("cpu")
+                continue
+
+            if decompose_mode == "low rank":
+                loras[f"{lora_name}.lora_down.weight"] = (
+                    extract_a.detach().cpu().contiguous().half()
+                )
+                loras[f"{lora_name}.lora_up.weight"] = (
+                    extract_b.detach().cpu().contiguous().half()
+                )
+                loras[f"{lora_name}.alpha"] = torch.Tensor([extract_a.shape[0]]).half()
+                if use_bias:
+                    diff = diff.detach().cpu().reshape(extract_b.size(0), -1)
+                    sparse_diff = make_sparse(diff, sparsity).to_sparse().coalesce()
+
+                    indices = sparse_diff.indices().to(torch.int16)
+                    values = sparse_diff.values().half()
+                    loras[f"{lora_name}.bias_indices"] = indices
+                    loras[f"{lora_name}.bias_values"] = values
+                    loras[f"{lora_name}.bias_size"] = torch.tensor(diff.shape).to(
+                        torch.int16
+                    )
+                del extract_a, extract_b, diff
+            elif decompose_mode == "full":
+                if "Norm" in layer:
+                    w_key = "w_norm"
+                    b_key = "b_norm"
+                else:
+                    w_key = "diff"
+                    b_key = "diff_b"
+                weight_diff = module.weight - weights.weight
+                loras[f"{lora_name}.{w_key}"] = (
+                    weight_diff.detach().cpu().contiguous().half()
+                )
+                if getattr(weights, "bias", None) is not None:
+                    bias_diff = module.bias - weights.bias
+                    loras[f"{lora_name}.{b_key}"] = (
+                        bias_diff.detach().cpu().contiguous().half()
+                    )
+            else:
+                raise NotImplementedError
+            module = module.to("cpu")
+            weights = weights.to("cpu")
+        return loras
+
+    all_loras = {}
+
+    all_loras |= make_state_dict(
+        LORA_PREFIX_UNET,
+        base_unet,
+        db_unet,
+        UNET_TARGET_REPLACE_MODULE,
+    )
+    del base_unet, db_unet
+    if torch.cuda.is_available():
+        torch.cuda.empty_cache()
+
+    for idx, (te1, te2) in enumerate(zip(base_tes, db_tes)):
+        if len(base_tes) > 1:
+            prefix = f"{LORA_PREFIX_TEXT_ENCODER}{idx+1}"
+        else:
+            prefix = LORA_PREFIX_TEXT_ENCODER
+        all_loras |= make_state_dict(
+            prefix,
+            te1,
+            te2,
+            TEXT_ENCODER_TARGET_REPLACE_MODULE,
+        )
+        del te1, te2
+
+    all_lora_name = set()
+    for k in all_loras:
+        lora_name, weight = k.rsplit(".", 1)
+        all_lora_name.add(lora_name)
+    print(len(all_lora_name))
+    return all_loras
+
+
+re_digits = re.compile(r"\d+")
+re_compiled = {}
+
+suffix_conversion = {
+    "attentions": {},
+    "resnets": {
+        "conv1": "in_layers_2",
+        "conv2": "out_layers_3",
+        "norm1": "in_layers_0",
+        "norm2": "out_layers_0",
+        "time_emb_proj": "emb_layers_1",
+        "conv_shortcut": "skip_connection",
+    },
+}
+
+
+def convert_diffusers_name_to_compvis(key):
+    def match(match_list, regex_text):
+        regex = re_compiled.get(regex_text)
+        if regex is None:
+            regex = re.compile(regex_text)
+            re_compiled[regex_text] = regex
+
+        r = re.match(regex, key)
+        if not r:
+            return False
+
+        match_list.clear()
+        match_list.extend([int(x) if re.match(re_digits, x) else x for x in r.groups()])
+        return True
+
+    m = []
+
+    if match(m, r"lora_unet_conv_in(.*)"):
+        return f"lora_unet_input_blocks_0_0{m[0]}"
+
+    if match(m, r"lora_unet_conv_out(.*)"):
+        return f"lora_unet_out_2{m[0]}"
+
+    if match(m, r"lora_unet_time_embedding_linear_(\d+)(.*)"):
+        return f"lora_unet_time_embed_{m[0] * 2 - 2}{m[1]}"
+
+    if match(m, r"lora_unet_down_blocks_(\d+)_(attentions|resnets)_(\d+)_(.+)"):
+        suffix = suffix_conversion.get(m[1], {}).get(m[3], m[3])
+        return f"lora_unet_input_blocks_{1 + m[0] * 3 + m[2]}_{1 if m[1] == 'attentions' else 0}_{suffix}"
+
+    if match(m, r"lora_unet_mid_block_(attentions|resnets)_(\d+)_(.+)"):
+        suffix = suffix_conversion.get(m[0], {}).get(m[2], m[2])
+        return (
+            f"lora_unet_middle_block_{1 if m[0] == 'attentions' else m[1] * 2}_{suffix}"
+        )
+
+    if match(m, r"lora_unet_up_blocks_(\d+)_(attentions|resnets)_(\d+)_(.+)"):
+        suffix = suffix_conversion.get(m[1], {}).get(m[3], m[3])
+        return f"lora_unet_output_blocks_{m[0] * 3 + m[2]}_{1 if m[1] == 'attentions' else 0}_{suffix}"
+
+    if match(m, r"lora_unet_down_blocks_(\d+)_downsamplers_0_conv"):
+        return f"lora_unet_input_blocks_{3 + m[0] * 3}_0_op"
+
+    if match(m, r"lora_unet_up_blocks_(\d+)_upsamplers_0_conv"):
+        return f"lora_unet_output_blocks_{2 + m[0] * 3}_2_conv"
+    return key
+
+
+def get_module(lyco_state_dict: Dict, lora_name):
+    if f"{lora_name}.lora_up.weight" in lyco_state_dict:
+        up = lyco_state_dict[f"{lora_name}.lora_up.weight"]
+        down = lyco_state_dict[f"{lora_name}.lora_down.weight"]
+        mid = lyco_state_dict.get(f"{lora_name}.lora_mid.weight", None)
+        alpha = lyco_state_dict.get(f"{lora_name}.alpha", None)
+        dora_scale = lyco_state_dict.get(f"{lora_name}.dora_scale", None)
+        return "locon", (up, down, mid, alpha, dora_scale)
+    elif f"{lora_name}.hada_w1_a" in lyco_state_dict:
+        w1a = lyco_state_dict[f"{lora_name}.hada_w1_a"]
+        w1b = lyco_state_dict[f"{lora_name}.hada_w1_b"]
+        w2a = lyco_state_dict[f"{lora_name}.hada_w2_a"]
+        w2b = lyco_state_dict[f"{lora_name}.hada_w2_b"]
+        t1 = lyco_state_dict.get(f"{lora_name}.hada_t1", None)
+        t2 = lyco_state_dict.get(f"{lora_name}.hada_t2", None)
+        alpha = lyco_state_dict.get(f"{lora_name}.alpha", None)
+        dora_scale = lyco_state_dict.get(f"{lora_name}.dora_scale", None)
+        return "hada", (w1a, w1b, w2a, w2b, t1, t2, alpha, dora_scale)
+    elif f"{lora_name}.weight" in lyco_state_dict:
+        weight = lyco_state_dict[f"{lora_name}.weight"]
+        on_input = lyco_state_dict.get(f"{lora_name}.on_input", False)
+        return "ia3", (weight, on_input)
+    elif (
+        f"{lora_name}.lokr_w1" in lyco_state_dict
+        or f"{lora_name}.lokr_w1_a" in lyco_state_dict
+    ):
+        w1 = lyco_state_dict.get(f"{lora_name}.lokr_w1", None)
+        w1a = lyco_state_dict.get(f"{lora_name}.lokr_w1_a", None)
+        w1b = lyco_state_dict.get(f"{lora_name}.lokr_w1_b", None)
+        w2 = lyco_state_dict.get(f"{lora_name}.lokr_w2", None)
+        w2a = lyco_state_dict.get(f"{lora_name}.lokr_w2_a", None)
+        w2b = lyco_state_dict.get(f"{lora_name}.lokr_w2_b", None)
+        t1 = lyco_state_dict.get(f"{lora_name}.lokr_t1", None)
+        t2 = lyco_state_dict.get(f"{lora_name}.lokr_t2", None)
+        alpha = lyco_state_dict.get(f"{lora_name}.alpha", None)
+        dora_scale = lyco_state_dict.get(f"{lora_name}.dora_scale", None)
+        return "kron", (w1, w1a, w1b, w2, w2a, w2b, t1, t2, alpha, dora_scale)
+    elif f"{lora_name}.diff" in lyco_state_dict:
+        diff = lyco_state_dict[f"{lora_name}.diff"]
+        diff_b = lyco_state_dict.get(f"{lora_name}.diff_b", None)
+        return "full", (diff, diff_b)
+    elif f"{lora_name}.w_norm" in lyco_state_dict:
+        w_norm = lyco_state_dict[f"{lora_name}.w_norm"]
+        b_norm = lyco_state_dict.get(f"{lora_name}.b_norm", None)
+        return "norm", (w_norm, b_norm)
+    else:
+        return "None", ()
+
+
+def tucker_weight_from_conv(up, down, mid):
+    up = up.reshape(up.size(0), up.size(1))
+    down = down.reshape(down.size(0), down.size(1))
+    return torch.einsum("m n w h, i m, n j -> i j w h", mid, up, down)
+
+
+def tucker_weight(wa, wb, t):
+    temp = torch.einsum("i j k l, j r -> i r k l", t, wb)
+    return torch.einsum("i j k l, i r -> r j k l", temp, wa)
+
+
+def apply_dora_scale(org_weight, rebuild, dora_scale, scale):
+    dora_norm_dims = org_weight.dim() - 1
+    weight = org_weight + rebuild
+    weight = weight.to(dora_scale.dtype)
+    weight_norm = (
+        weight.transpose(0, 1)
+        .reshape(weight.shape[1], -1)
+        .norm(dim=1, keepdim=True)
+        .reshape(weight.shape[1], *[1] * dora_norm_dims)
+        .transpose(0, 1)
+    )
+    merged_scale1 = weight / weight_norm * dora_scale
+    diff_weight = merged_scale1 - org_weight
+    return org_weight + diff_weight * scale
+
+
+@torch.no_grad()
+def rebuild_weight(module_type, params, orig_weight, orig_bias, scale=1):
+    if orig_weight is None:
+        return None, None
+    merged = orig_weight
+    merged_bias = orig_bias
+    if module_type == "locon":
+        up, down, mid, alpha, dora_scale = params
+        if alpha is not None:
+            scale *= alpha / up.size(1)
+        if mid is not None:
+            rebuild = tucker_weight_from_conv(up, down, mid)
+        else:
+            rebuild = up.reshape(up.size(0), -1) @ down.reshape(down.size(0), -1)
+        rebuild = rebuild.reshape(orig_weight.shape)
+        if dora_scale is None:
+            merged = orig_weight + rebuild * scale
+        else:
+            merged = apply_dora_scale(orig_weight, rebuild, dora_scale, scale)
+        del up, down, mid, alpha, params, rebuild
+    elif module_type == "hada":
+        w1a, w1b, w2a, w2b, t1, t2, alpha, dora_scale = params
+        if alpha is not None:
+            scale *= alpha / w1b.size(0)
+        if t1 is not None:
+            rebuild1 = tucker_weight(w1a, w1b, t1)
+        else:
+            rebuild1 = w1a @ w1b
+        if t2 is not None:
+            rebuild2 = tucker_weight(w2a, w2b, t2)
+        else:
+            rebuild2 = w2a @ w2b
+        rebuild = (rebuild1 * rebuild2).reshape(orig_weight.shape)
+        if dora_scale is None:
+            merged = orig_weight + rebuild * scale
+        else:
+            merged = apply_dora_scale(orig_weight, rebuild, dora_scale, scale)
+        del w1a, w1b, w2a, w2b, t1, t2, alpha, params, rebuild, rebuild1, rebuild2
+    elif module_type == "ia3":
+        weight, on_input = params
+        if not on_input:
+            weight = weight.reshape(-1, 1)
+        merged = orig_weight + weight * orig_weight * scale
+        del weight, on_input, params
+    elif module_type == "kron":
+        w1, w1a, w1b, w2, w2a, w2b, t1, t2, alpha, dora_scale = params
+        if alpha is not None and (w1b is not None or w2b is not None):
+            scale *= alpha / (w1b.size(0) if w1b else w2b.size(0))
+        if w1a is not None and w1b is not None:
+            if t1 is not None:
+                w1 = tucker_weight(w1a, w1b, t1)
+            else:
+                w1 = w1a @ w1b
+        if w2a is not None and w2b is not None:
+            if t2 is not None:
+                w2 = tucker_weight(w2a, w2b, t2)
+            else:
+                w2 = w2a @ w2b
+        if len(w2.shape) == 4:
+            w1 = w1.unsqueeze(2).unsqueeze(2)
+        w2 = w2.contiguous()
+        rebuild = torch.kron(w1, w2).reshape(orig_weight.shape)
+        if dora_scale is None:
+            merged = orig_weight + rebuild * scale
+        else:
+            merged = apply_dora_scale(orig_weight, rebuild, dora_scale, scale)
+        del w1, w1a, w1b, w2, w2a, w2b, t1, t2, alpha, params, rebuild
+    elif module_type == "full":
+        rebuild = params[0].reshape(orig_weight.shape)
+        rebuild_b = (
+            params[1].reshape(orig_bias.shape) if orig_bias is not None else None
+        )
+        merged = orig_weight + rebuild * scale
+        if rebuild_b is not None:
+            merged_bias = orig_bias + rebuild_b * scale
+        del params, rebuild, rebuild_b
+    elif module_type == "norm":
+        rebuild = params[0].reshape(orig_weight.shape)
+        rebuild_b = params[1].reshape(orig_bias.shape)
+        merged = orig_weight + rebuild * scale
+        merged_bias = orig_bias + rebuild_b * scale
+    else:
+        return None, None
+
+    return merged, merged_bias
+
+
+@torch.no_grad()
+def merge(tes, unet, lyco_state_dict, scale: float = 1.0, device="cpu"):
+    UNET_TARGET_REPLACE_MODULE = [
+        "Linear",
+        "Conv2d",
+        "LayerNorm",
+        "GroupNorm",
+        "GroupNorm32",
+    ]
+    TEXT_ENCODER_TARGET_REPLACE_MODULE = [
+        "Embedding",
+        "Linear",
+        "Conv2d",
+        "LayerNorm",
+        "GroupNorm",
+        "GroupNorm32",
+        "Embedding",
+    ]
+    LORA_PREFIX_UNET = "lora_unet"
+    LORA_PREFIX_TEXT_ENCODER = "lora_te"
+    merged = 0
+
+    def merge_state_dict(
+        prefix,
+        root_module: torch.nn.Module,
+        lyco_state_dict: Dict[str, torch.Tensor],
+        target_replace_modules,
+    ):
+        nonlocal merged
+        for child_name, child_module in tqdm(
+            list(root_module.named_modules()), desc=f"Merging {prefix}"
+        ):
+            if child_module.__class__.__name__ in target_replace_modules:
+                lora_name = prefix + "." + child_name
+                lora_name = lora_name.replace(".", "_")
+
+                result, result_b = rebuild_weight(
+                    *get_module(lyco_state_dict, lora_name),
+                    getattr(child_module, "weight"),
+                    getattr(child_module, "bias", None),
+                    scale,
+                )
+                if result is not None:
+                    key_dict.pop(lora_name)
+                    merged += 1
+                    child_module.requires_grad_(False)
+                    child_module.weight.copy_(result)
+                if result_b is not None:
+                    child_module.bias.copy_(result_b)
+
+    key_dict = {}
+    for k, v in tqdm(list(lyco_state_dict.items()), desc="Converting Dtype and Device"):
+        module, weight_key = k.split(".", 1)
+        convert_key = convert_diffusers_name_to_compvis(module)
+        if convert_key != module and len(tes) > 1:
+            # kohya's format for sdxl is as same as SGM, not diffusers
+            del lyco_state_dict[k]
+            key_dict[convert_key] = key_dict.get(convert_key, []) + [k]
+            k = f"{convert_key}.{weight_key}"
+        else:
+            key_dict[module] = key_dict.get(module, []) + [k]
+        if device == "cpu":
+            lyco_state_dict[k] = v.float().cpu()
+        else:
+            lyco_state_dict[k] = v.to(
+                device, dtype=tes[0].parameters().__next__().dtype
+            )
+
+    for idx, te in enumerate(tes):
+        if len(tes) > 1:
+            prefix = LORA_PREFIX_TEXT_ENCODER + str(idx + 1)
+        else:
+            prefix = LORA_PREFIX_TEXT_ENCODER
+        merge_state_dict(
+            prefix,
+            te.to(device),
+            lyco_state_dict,
+            TEXT_ENCODER_TARGET_REPLACE_MODULE,
+        )
+    merge_state_dict(
+        LORA_PREFIX_UNET,
+        unet.to(device),
+        lyco_state_dict,
+        UNET_TARGET_REPLACE_MODULE,
+    )
+    print(f"Unused state dict key: {key_dict}")
+    print(f"{merged} Modules been merged")
```

### Comparing `lycoris_lora-2.3.0.dev4/lycoris/utils/logger.py` & `lycoris_lora-2.3.0.dev5/lycoris/utils/logger.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-import logging
-import copy
-import sys
-
-
-class ColoredFormatter(logging.Formatter):
-    COLORS = {
-        "DEBUG": "\033[0;36m",  # CYAN
-        "INFO": "\033[0;32m",  # GREEN
-        "WARNING": "\033[0;33m",  # YELLOW
-        "ERROR": "\033[0;31m",  # RED
-        "CRITICAL": "\033[0;37;41m",  # WHITE ON RED
-        "RESET": "\033[0m",  # RESET COLOR
-    }
-
-    def format(self, record):
-        colored_record = copy.copy(record)
-        levelname = colored_record.levelname
-        seq = self.COLORS.get(levelname, self.COLORS["RESET"])
-        colored_record.levelname = f"{seq}{levelname}{self.COLORS['RESET']}"
-        return super().format(colored_record)
-
-
-# Create a new logger
-logger = logging.getLogger("LyCORIS")
-logger.propagate = False
-
-# Add handler if we don't have one.
-if not logger.handlers:
-    handler = logging.StreamHandler(sys.stdout)
-    handler.setFormatter(ColoredFormatter("[%(name)s]-%(levelname)s: %(message)s"))
-    logger.addHandler(handler)
-
-logger.setLevel(logging.DEBUG)
-logger.debug("Logger initialized.")
+import logging
+import copy
+import sys
+
+
+class ColoredFormatter(logging.Formatter):
+    COLORS = {
+        "DEBUG": "\033[0;36m",  # CYAN
+        "INFO": "\033[0;32m",  # GREEN
+        "WARNING": "\033[0;33m",  # YELLOW
+        "ERROR": "\033[0;31m",  # RED
+        "CRITICAL": "\033[0;37;41m",  # WHITE ON RED
+        "RESET": "\033[0m",  # RESET COLOR
+    }
+
+    def format(self, record):
+        colored_record = copy.copy(record)
+        levelname = colored_record.levelname
+        seq = self.COLORS.get(levelname, self.COLORS["RESET"])
+        colored_record.levelname = f"{seq}{levelname}{self.COLORS['RESET']}"
+        return super().format(colored_record)
+
+
+# Create a new logger
+logger = logging.getLogger("LyCORIS")
+logger.propagate = False
+
+# Add handler if we don't have one.
+if not logger.handlers:
+    handler = logging.StreamHandler(sys.stdout)
+    handler.setFormatter(ColoredFormatter("[%(name)s]-%(levelname)s: %(message)s"))
+    logger.addHandler(handler)
+
+logger.setLevel(logging.DEBUG)
+logger.debug("Logger initialized.")
```

### Comparing `lycoris_lora-2.3.0.dev4/lycoris/wrapper.py` & `lycoris_lora-2.3.0.dev5/lycoris/wrapper.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,534 +1,534 @@
-# General LyCORIS wrapper based on kohya-ss/sd-scripts' style
-
-import math
-import os
-import regex as re
-import sys
-
-sys.setrecursionlimit(10000)
-from typing import List
-
-import torch
-import torch.nn as nn
-
-from .modules.locon import LoConModule
-from .modules.loha import LohaModule
-from .modules.lokr import LokrModule
-from .modules.dylora import DyLoraModule
-from .modules.glora import GLoRAModule
-from .modules.norms import NormModule
-from .modules.full import FullModule
-from .modules.diag_oft import DiagOFTModule
-from .modules.boft import ButterflyOFTModule
-from .modules import make_module
-
-from .config import PRESET
-from .utils.preset import read_preset
-from .utils import get_module, str_bool
-from .logging import logger
-
-
-network_module_dict = {
-    "lora": LoConModule,
-    "locon": LoConModule,
-    "loha": LohaModule,
-    "lokr": LokrModule,
-    "dylora": DyLoraModule,
-    "glora": GLoRAModule,
-    "full": FullModule,
-    "diag-oft": DiagOFTModule,
-    "boft": ButterflyOFTModule,
-}
-
-
-def create_lycoris(module, multiplier, linear_dim, linear_alpha, **kwargs):
-    if linear_dim is None:
-        linear_dim = 4  # default
-    conv_dim = int(kwargs.get("conv_dim", linear_dim) or linear_dim)
-    conv_alpha = float(kwargs.get("conv_alpha", linear_alpha) or linear_alpha)
-    dropout = float(kwargs.get("dropout", 0.0) or 0.0)
-    rank_dropout = float(kwargs.get("rank_dropout", 0.0) or 0.0)
-    module_dropout = float(kwargs.get("module_dropout", 0.0) or 0.0)
-    algo = (kwargs.get("algo", "lora") or "lora").lower()
-    use_tucker = str_bool(
-        not kwargs.get("disable_conv_cp", True)
-        or kwargs.get("use_conv_cp", False)
-        or kwargs.get("use_cp", False)
-        or kwargs.get("use_tucker", False)
-    )
-    if "disable_conv_cp" in kwargs or "use_cp" in kwargs or "use_conv_cp" in kwargs:
-        logger.warning(
-            "disable_conv_cp and use_cp are deprecated. Please use use_tucker instead.",
-            stacklevel=2,
-        )
-    use_scalar = str_bool(kwargs.get("use_scalar", False))
-    block_size = int(kwargs.get("block_size", 4) or 4)
-    train_norm = str_bool(kwargs.get("train_norm", False))
-    constrain = float(kwargs.get("constrain", 0) or 0)
-    rescaled = str_bool(kwargs.get("rescaled", False))
-    weight_decompose = str_bool(kwargs.get("dora_wd", False))
-    full_matrix = str_bool(kwargs.get("full_matrix", False))
-    bypass_mode = str_bool(kwargs.get("bypass_mode", False))
-    unbalanced_factorization = str_bool(kwargs.get("unbalanced_factorization", False))
-
-    if unbalanced_factorization:
-        logger.info("Unbalanced factorization for LoKr is enabled")
-
-    if bypass_mode:
-        logger.info("Bypass mode is enabled")
-
-    if weight_decompose:
-        logger.info("Weight decomposition is enabled")
-
-    if full_matrix:
-        logger.info("Full matrix mode for LoKr is enabled")
-
-    if algo == "glora" and conv_dim > 0:
-        conv_dim = 0
-        logger.info("Disable conv layer for GLoRA")
-
-    preset = kwargs.get("preset", "full")
-    if preset not in PRESET:
-        preset = read_preset(preset)
-    else:
-        preset = PRESET[preset]
-    assert preset is not None
-    LycorisNetwork.apply_preset(preset)
-
-    logger.info(f"Using rank adaptation algo: {algo}")
-
-    if (
-        (algo == "loha")
-        and not kwargs.get("no_dim_warn", False)
-        and (linear_dim > 64 or conv_dim > 64)
-    ):
-        warning_type = {"loha": "Hadamard Product representation"}
-        warning_msg = (
-            "You are not supposed to use dim>64 (64*64 = 4096, it already has enough rank)\n"
-            f"in {warning_type[algo]}!\n"
-            "Please consider use lower dim or disable this warning with --network_args no_dim_warn=True\n"
-            f"If you just want to use high dim {algo}, please consider use lower lr."
-        )
-        logger.warning(warning_msg, stacklevel=2)
-
-    network = LycorisNetwork(
-        module,
-        multiplier=multiplier,
-        lora_dim=linear_dim,
-        conv_lora_dim=conv_dim,
-        alpha=linear_alpha,
-        conv_alpha=conv_alpha,
-        dropout=dropout,
-        rank_dropout=rank_dropout,
-        module_dropout=module_dropout,
-        use_tucker=use_tucker,
-        use_scalar=use_scalar,
-        network_module=algo,
-        train_norm=train_norm,
-        decompose_both=kwargs.get("decompose_both", False),
-        factor=kwargs.get("factor", -1),
-        block_size=block_size,
-        constrain=constrain,
-        rescaled=rescaled,
-        weight_decompose=weight_decompose,
-        full_matrix=full_matrix,
-        bypass_mode=bypass_mode,
-        unbalanced_factorization=unbalanced_factorization,
-    )
-
-    if algo == "dylora":
-        # dylora didn't support scale weight norm yet
-        delattr(type(network), "apply_max_norm_regularization")
-
-    return network
-
-
-def create_lycoris_from_weights(multiplier, file, module, weights_sd=None, **kwargs):
-    if weights_sd is None:
-        if os.path.splitext(file)[1] == ".safetensors":
-            from safetensors.torch import load_file
-
-            weights_sd = load_file(file)
-        else:
-            weights_sd = torch.load(file, map_location="cpu")
-
-    # get dim/alpha mapping
-    loras = {}
-    for key in weights_sd:
-        if "." not in key:
-            continue
-
-        lora_name = key.split(".")[0]
-        loras[lora_name] = None
-
-    for name, modules in module.named_modules():
-        lora_name = f"{LycorisNetwork.LORA_PREFIX}_{name}".replace(".", "_")
-        if lora_name in loras:
-            loras[lora_name] = modules
-
-    network = LycorisNetwork(module, init_only=True)
-    network.multiplier = multiplier
-    network.loras = []
-
-    for lora_name, orig_modules in loras.items():
-        if orig_modules is None:
-            continue
-        lyco_type, params = get_module(weights_sd, lora_name)
-        module = make_module(lyco_type, params, lora_name, orig_modules)
-        if module is not None:
-            network.loras.append(module)
-            network.algo_table[module.__class__.__name__] = (
-                network.algo_table.get(module.__class__.__name__, 0) + 1
-            )
-
-    for lora in network.loras:
-        lora.multiplier = multiplier
-
-    return network, weights_sd
-
-
-class LycorisNetwork(torch.nn.Module):
-    ENABLE_CONV = True
-    TARGET_REPLACE_MODULE = []
-    TARGET_REPLACE_NAME = []
-    LORA_PREFIX = "lycoris"
-    MODULE_ALGO_MAP = {}
-    NAME_ALGO_MAP = {}
-
-    @classmethod
-    def apply_preset(cls, preset):
-        if "enable_conv" in preset:
-            cls.ENABLE_CONV = preset["enable_conv"]
-        if "target_module" in preset:
-            cls.TARGET_REPLACE_MODULE = preset["target_module"]
-        if "target_name" in preset:
-            cls.TARGET_REPLACE_NAME = preset["target_name"]
-        if "module_algo_map" in preset:
-            cls.MODULE_ALGO_MAP = preset["module_algo_map"]
-        if "name_algo_map" in preset:
-            cls.NAME_ALGO_MAP = preset["name_algo_map"]
-        return cls
-
-    def __init__(
-        self,
-        module: nn.Module,
-        multiplier=1.0,
-        lora_dim=4,
-        conv_lora_dim=4,
-        alpha=1,
-        conv_alpha=1,
-        use_tucker=False,
-        dropout=0,
-        rank_dropout=0,
-        module_dropout=0,
-        network_module: str = "locon",
-        norm_modules=NormModule,
-        train_norm=False,
-        init_only=False,
-        **kwargs,
-    ) -> None:
-        super().__init__()
-        root_kwargs = kwargs
-        if init_only:
-            self.multiplier = 1
-            self.lora_dim = 0
-            self.alpha = 1
-            self.conv_lora_dim = 0
-            self.conv_alpha = 1
-            self.dropout = 0
-            self.rank_dropout = 0
-            self.module_dropout = 0
-            self.use_tucker = False
-            self.loras = []
-            self.algo_table = {}
-            return
-        self.multiplier = multiplier
-        self.lora_dim = lora_dim
-
-        if not self.ENABLE_CONV:
-            conv_lora_dim = 0
-
-        self.conv_lora_dim = int(conv_lora_dim)
-        if self.conv_lora_dim and self.conv_lora_dim != self.lora_dim:
-            logger.info("Apply different lora dim for conv layer")
-            logger.info(f"Conv Dim: {conv_lora_dim}, Linear Dim: {lora_dim}")
-        elif self.conv_lora_dim == 0:
-            logger.info("Disable conv layer")
-
-        self.alpha = alpha
-        self.conv_alpha = float(conv_alpha)
-        if self.conv_lora_dim and self.alpha != self.conv_alpha:
-            logger.info("Apply different alpha value for conv layer")
-            logger.info(f"Conv alpha: {conv_alpha}, Linear alpha: {alpha}")
-
-        if 1 >= dropout >= 0:
-            logger.info(f"Use Dropout value: {dropout}")
-        self.dropout = dropout
-        self.rank_dropout = rank_dropout
-        self.module_dropout = module_dropout
-
-        self.use_tucker = use_tucker
-
-        def create_single_module(
-            lora_name: str,
-            module: torch.nn.Module,
-            algo_name,
-            dim=None,
-            alpha=None,
-            use_tucker=self.use_tucker,
-            **kwargs,
-        ):
-            for k, v in root_kwargs.items():
-                if k in kwargs:
-                    continue
-                kwargs[k] = v
-
-            if train_norm and "Norm" in module.__class__.__name__:
-                return norm_modules(
-                    lora_name,
-                    module,
-                    self.multiplier,
-                    self.rank_dropout,
-                    self.module_dropout,
-                    **kwargs,
-                )
-            lora = None
-            if isinstance(module, torch.nn.Linear) and lora_dim > 0:
-                dim = dim or lora_dim
-                alpha = alpha or self.alpha
-            elif isinstance(module, torch.nn.Conv2d):
-                k_size, *_ = module.kernel_size
-                if k_size == 1 and lora_dim > 0:
-                    dim = dim or lora_dim
-                    alpha = alpha or self.alpha
-                elif conv_lora_dim > 0 or dim:
-                    dim = dim or conv_lora_dim
-                    alpha = alpha or self.conv_alpha
-                else:
-                    return None
-            else:
-                return None
-            lora = network_module_dict[algo_name](
-                lora_name,
-                module,
-                self.multiplier,
-                dim,
-                alpha,
-                self.dropout,
-                self.rank_dropout,
-                self.module_dropout,
-                use_tucker,
-                **kwargs,
-            )
-            return lora
-
-        def create_modules_(
-            prefix: str,
-            root_module: torch.nn.Module,
-            algo,
-            configs={},
-        ):
-            loras = {}
-            lora_names = []
-            for name, module in root_module.named_modules():
-                module_name = module.__class__.__name__
-                if module_name in self.MODULE_ALGO_MAP:
-                    next_config = self.MODULE_ALGO_MAP[module_name]
-                    next_algo = next_config.get("algo", algo)
-                    new_loras, new_lora_names = create_modules_(
-                        f"{prefix}_{name}", module, next_algo, next_config
-                    )
-                    for lora_name, lora in zip(new_lora_names, new_loras):
-                        if lora_name not in loras:
-                            loras[lora_name] = lora
-                            lora_names.append(lora_name)
-                    continue
-                lora_name = prefix + "." + name
-                lora_name = lora_name.replace(".", "_")
-                if lora_name in loras:
-                    continue
-
-                lora = create_single_module(lora_name, module, algo, **configs)
-                if lora is not None:
-                    loras[lora_name] = lora
-                    lora_names.append(lora_name)
-            return [loras[lora_name] for lora_name in lora_names], lora_names
-
-        # create module instances
-        def create_modules(
-            prefix,
-            root_module: torch.nn.Module,
-            target_replace_modules,
-            target_replace_names=[],
-        ) -> List:
-            logger.info("Create LyCORIS Module")
-            loras = []
-            next_config = {}
-            for name, module in root_module.named_modules():
-                module_name = module.__class__.__name__
-                if module_name in target_replace_modules:
-                    if module_name in self.MODULE_ALGO_MAP:
-                        next_config = self.MODULE_ALGO_MAP[module_name]
-                        algo = next_config.get("algo", network_module)
-                    else:
-                        algo = network_module
-                    loras.extend(
-                        create_modules_(f"{prefix}_{name}", module, algo, next_config)[
-                            0
-                        ]
-                    )
-                    next_config = {}
-                elif name in target_replace_names or any(
-                    re.match(t, name) for t in target_replace_names
-                ):
-                    if name in self.NAME_ALGO_MAP:
-                        next_config = self.NAME_ALGO_MAP[name]
-                        algo = next_config.get("algo", network_module)
-                    elif module_name in self.MODULE_ALGO_MAP:
-                        next_config = self.MODULE_ALGO_MAP[module_name]
-                        algo = next_config.get("algo", network_module)
-                    else:
-                        algo = network_module
-                    lora_name = prefix + "." + name
-                    lora_name = lora_name.replace(".", "_")
-                    lora = create_single_module(lora_name, module, algo, **next_config)
-                    next_config = {}
-                    if lora is not None:
-                        loras.append(lora)
-            return loras
-
-        self.loras = create_modules(
-            LycorisNetwork.LORA_PREFIX,
-            module,
-            LycorisNetwork.TARGET_REPLACE_MODULE,
-            LycorisNetwork.TARGET_REPLACE_NAME,
-        )
-        logger.info(f"create LyCORIS: {len(self.loras)} modules.")
-
-        algo_table = {}
-        for lora in self.loras:
-            algo_table[lora.__class__.__name__] = (
-                algo_table.get(lora.__class__.__name__, 0) + 1
-            )
-        logger.info(f"module type table: {algo_table}")
-
-        self.weights_sd = None
-
-        # assertion
-        names = set()
-        for lora in self.loras:
-            assert (
-                lora.lora_name not in names
-            ), f"duplicated lora name: {lora.lora_name}"
-            names.add(lora.lora_name)
-
-    def set_multiplier(self, multiplier):
-        self.multiplier = multiplier
-        for lora in self.loras:
-            lora.multiplier = self.multiplier
-
-    def load_weights(self, file):
-        if os.path.splitext(file)[1] == ".safetensors":
-            from safetensors.torch import load_file, safe_open
-
-            self.weights_sd = load_file(file)
-        else:
-            self.weights_sd = torch.load(file, map_location="cpu")
-        missing, unexpected = self.load_state_dict(self.weights_sd, strict=False)
-        state = {}
-        if missing:
-            state["missing keys"] = missing
-        if unexpected:
-            state["unexpected keys"] = unexpected
-        return state
-
-    def apply_to(self):
-        for lora in self.loras:
-            lora.apply_to()
-            self.add_module(lora.lora_name, lora)
-
-        if self.weights_sd:
-            # if some weights are not in state dict, it is ok because initial LoRA does nothing (lora_up is initialized by zeros)
-            info = self.load_state_dict(self.weights_sd, False)
-            logger.info(f"weights are loaded: {info}")
-
-    def is_mergeable(self):
-        return True
-
-    def restore(self):
-        for lora in self.loras:
-            lora.restore()
-
-    def merge_to(self, weight=1.0):
-        for lora in self.loras:
-            lora.merge_to(weight)
-
-    def apply_max_norm_regularization(self, max_norm_value, device):
-        key_scaled = 0
-        norms = []
-        for model in self.loras:
-            if hasattr(model, "apply_max_norm"):
-                scaled, norm = model.apply_max_norm(max_norm_value, device)
-                norms.append(norm)
-                key_scaled += scaled
-
-        if key_scaled == 0:
-            return key_scaled, 0, 0
-
-        return key_scaled, sum(norms) / len(norms), max(norms)
-
-    def enable_gradient_checkpointing(self):
-        # not supported
-        def make_ckpt(module):
-            if isinstance(module, torch.nn.Module):
-                module.grad_ckpt = True
-
-        self.apply(make_ckpt)
-        pass
-
-    def prepare_optimizer_params(self, lr):
-        def enumerate_params(loras):
-            params = []
-            for lora in loras:
-                params.extend(lora.parameters())
-            return params
-
-        self.requires_grad_(True)
-        all_params = []
-
-        param_data = {"params": enumerate_params(self.loras)}
-        if lr is not None:
-            param_data["lr"] = lr
-        all_params.append(param_data)
-        return all_params
-
-    def prepare_grad_etc(self, *args):
-        self.requires_grad_(True)
-
-    def on_epoch_start(self, *args):
-        self.train()
-
-    def get_trainable_params(self, *args):
-        return self.parameters()
-
-    def save_weights(self, file, dtype, metadata):
-        if metadata is not None and len(metadata) == 0:
-            metadata = None
-
-        state_dict = self.state_dict()
-
-        if dtype is not None:
-            for key in list(state_dict.keys()):
-                v = state_dict[key]
-                v = v.detach().clone().to("cpu").to(dtype)
-                state_dict[key] = v
-
-        if os.path.splitext(file)[1] == ".safetensors":
-            from safetensors.torch import save_file
-
-            # Precalculate model hashes to save time on indexing
-            if metadata is None:
-                metadata = {}
-            save_file(state_dict, file, metadata)
-        else:
-            torch.save(state_dict, file)
+# General LyCORIS wrapper based on kohya-ss/sd-scripts' style
+
+import math
+import os
+import regex as re
+import sys
+
+sys.setrecursionlimit(10000)
+from typing import List
+
+import torch
+import torch.nn as nn
+
+from .modules.locon import LoConModule
+from .modules.loha import LohaModule
+from .modules.lokr import LokrModule
+from .modules.dylora import DyLoraModule
+from .modules.glora import GLoRAModule
+from .modules.norms import NormModule
+from .modules.full import FullModule
+from .modules.diag_oft import DiagOFTModule
+from .modules.boft import ButterflyOFTModule
+from .modules import make_module
+
+from .config import PRESET
+from .utils.preset import read_preset
+from .utils import get_module, str_bool
+from .logging import logger
+
+
+network_module_dict = {
+    "lora": LoConModule,
+    "locon": LoConModule,
+    "loha": LohaModule,
+    "lokr": LokrModule,
+    "dylora": DyLoraModule,
+    "glora": GLoRAModule,
+    "full": FullModule,
+    "diag-oft": DiagOFTModule,
+    "boft": ButterflyOFTModule,
+}
+
+
+def create_lycoris(module, multiplier, linear_dim, linear_alpha, **kwargs):
+    if linear_dim is None:
+        linear_dim = 4  # default
+    conv_dim = int(kwargs.get("conv_dim", linear_dim) or linear_dim)
+    conv_alpha = float(kwargs.get("conv_alpha", linear_alpha) or linear_alpha)
+    dropout = float(kwargs.get("dropout", 0.0) or 0.0)
+    rank_dropout = float(kwargs.get("rank_dropout", 0.0) or 0.0)
+    module_dropout = float(kwargs.get("module_dropout", 0.0) or 0.0)
+    algo = (kwargs.get("algo", "lora") or "lora").lower()
+    use_tucker = str_bool(
+        not kwargs.get("disable_conv_cp", True)
+        or kwargs.get("use_conv_cp", False)
+        or kwargs.get("use_cp", False)
+        or kwargs.get("use_tucker", False)
+    )
+    if "disable_conv_cp" in kwargs or "use_cp" in kwargs or "use_conv_cp" in kwargs:
+        logger.warning(
+            "disable_conv_cp and use_cp are deprecated. Please use use_tucker instead.",
+            stacklevel=2,
+        )
+    use_scalar = str_bool(kwargs.get("use_scalar", False))
+    block_size = int(kwargs.get("block_size", 4) or 4)
+    train_norm = str_bool(kwargs.get("train_norm", False))
+    constrain = float(kwargs.get("constrain", 0) or 0)
+    rescaled = str_bool(kwargs.get("rescaled", False))
+    weight_decompose = str_bool(kwargs.get("dora_wd", False))
+    full_matrix = str_bool(kwargs.get("full_matrix", False))
+    bypass_mode = str_bool(kwargs.get("bypass_mode", False))
+    unbalanced_factorization = str_bool(kwargs.get("unbalanced_factorization", False))
+
+    if unbalanced_factorization:
+        logger.info("Unbalanced factorization for LoKr is enabled")
+
+    if bypass_mode:
+        logger.info("Bypass mode is enabled")
+
+    if weight_decompose:
+        logger.info("Weight decomposition is enabled")
+
+    if full_matrix:
+        logger.info("Full matrix mode for LoKr is enabled")
+
+    if algo == "glora" and conv_dim > 0:
+        conv_dim = 0
+        logger.info("Disable conv layer for GLoRA")
+
+    preset = kwargs.get("preset", "full")
+    if preset not in PRESET:
+        preset = read_preset(preset)
+    else:
+        preset = PRESET[preset]
+    assert preset is not None
+    LycorisNetwork.apply_preset(preset)
+
+    logger.info(f"Using rank adaptation algo: {algo}")
+
+    if (
+        (algo == "loha")
+        and not kwargs.get("no_dim_warn", False)
+        and (linear_dim > 64 or conv_dim > 64)
+    ):
+        warning_type = {"loha": "Hadamard Product representation"}
+        warning_msg = (
+            "You are not supposed to use dim>64 (64*64 = 4096, it already has enough rank)\n"
+            f"in {warning_type[algo]}!\n"
+            "Please consider use lower dim or disable this warning with --network_args no_dim_warn=True\n"
+            f"If you just want to use high dim {algo}, please consider use lower lr."
+        )
+        logger.warning(warning_msg, stacklevel=2)
+
+    network = LycorisNetwork(
+        module,
+        multiplier=multiplier,
+        lora_dim=linear_dim,
+        conv_lora_dim=conv_dim,
+        alpha=linear_alpha,
+        conv_alpha=conv_alpha,
+        dropout=dropout,
+        rank_dropout=rank_dropout,
+        module_dropout=module_dropout,
+        use_tucker=use_tucker,
+        use_scalar=use_scalar,
+        network_module=algo,
+        train_norm=train_norm,
+        decompose_both=kwargs.get("decompose_both", False),
+        factor=kwargs.get("factor", -1),
+        block_size=block_size,
+        constrain=constrain,
+        rescaled=rescaled,
+        weight_decompose=weight_decompose,
+        full_matrix=full_matrix,
+        bypass_mode=bypass_mode,
+        unbalanced_factorization=unbalanced_factorization,
+    )
+
+    if algo == "dylora":
+        # dylora didn't support scale weight norm yet
+        delattr(type(network), "apply_max_norm_regularization")
+
+    return network
+
+
+def create_lycoris_from_weights(multiplier, file, module, weights_sd=None, **kwargs):
+    if weights_sd is None:
+        if os.path.splitext(file)[1] == ".safetensors":
+            from safetensors.torch import load_file
+
+            weights_sd = load_file(file)
+        else:
+            weights_sd = torch.load(file, map_location="cpu")
+
+    # get dim/alpha mapping
+    loras = {}
+    for key in weights_sd:
+        if "." not in key:
+            continue
+
+        lora_name = key.split(".")[0]
+        loras[lora_name] = None
+
+    for name, modules in module.named_modules():
+        lora_name = f"{LycorisNetwork.LORA_PREFIX}_{name}".replace(".", "_")
+        if lora_name in loras:
+            loras[lora_name] = modules
+
+    network = LycorisNetwork(module, init_only=True)
+    network.multiplier = multiplier
+    network.loras = []
+
+    for lora_name, orig_modules in loras.items():
+        if orig_modules is None:
+            continue
+        lyco_type, params = get_module(weights_sd, lora_name)
+        module = make_module(lyco_type, params, lora_name, orig_modules)
+        if module is not None:
+            network.loras.append(module)
+            network.algo_table[module.__class__.__name__] = (
+                network.algo_table.get(module.__class__.__name__, 0) + 1
+            )
+
+    for lora in network.loras:
+        lora.multiplier = multiplier
+
+    return network, weights_sd
+
+
+class LycorisNetwork(torch.nn.Module):
+    ENABLE_CONV = True
+    TARGET_REPLACE_MODULE = []
+    TARGET_REPLACE_NAME = []
+    LORA_PREFIX = "lycoris"
+    MODULE_ALGO_MAP = {}
+    NAME_ALGO_MAP = {}
+
+    @classmethod
+    def apply_preset(cls, preset):
+        if "enable_conv" in preset:
+            cls.ENABLE_CONV = preset["enable_conv"]
+        if "target_module" in preset:
+            cls.TARGET_REPLACE_MODULE = preset["target_module"]
+        if "target_name" in preset:
+            cls.TARGET_REPLACE_NAME = preset["target_name"]
+        if "module_algo_map" in preset:
+            cls.MODULE_ALGO_MAP = preset["module_algo_map"]
+        if "name_algo_map" in preset:
+            cls.NAME_ALGO_MAP = preset["name_algo_map"]
+        return cls
+
+    def __init__(
+        self,
+        module: nn.Module,
+        multiplier=1.0,
+        lora_dim=4,
+        conv_lora_dim=4,
+        alpha=1,
+        conv_alpha=1,
+        use_tucker=False,
+        dropout=0,
+        rank_dropout=0,
+        module_dropout=0,
+        network_module: str = "locon",
+        norm_modules=NormModule,
+        train_norm=False,
+        init_only=False,
+        **kwargs,
+    ) -> None:
+        super().__init__()
+        root_kwargs = kwargs
+        if init_only:
+            self.multiplier = 1
+            self.lora_dim = 0
+            self.alpha = 1
+            self.conv_lora_dim = 0
+            self.conv_alpha = 1
+            self.dropout = 0
+            self.rank_dropout = 0
+            self.module_dropout = 0
+            self.use_tucker = False
+            self.loras = []
+            self.algo_table = {}
+            return
+        self.multiplier = multiplier
+        self.lora_dim = lora_dim
+
+        if not self.ENABLE_CONV:
+            conv_lora_dim = 0
+
+        self.conv_lora_dim = int(conv_lora_dim)
+        if self.conv_lora_dim and self.conv_lora_dim != self.lora_dim:
+            logger.info("Apply different lora dim for conv layer")
+            logger.info(f"Conv Dim: {conv_lora_dim}, Linear Dim: {lora_dim}")
+        elif self.conv_lora_dim == 0:
+            logger.info("Disable conv layer")
+
+        self.alpha = alpha
+        self.conv_alpha = float(conv_alpha)
+        if self.conv_lora_dim and self.alpha != self.conv_alpha:
+            logger.info("Apply different alpha value for conv layer")
+            logger.info(f"Conv alpha: {conv_alpha}, Linear alpha: {alpha}")
+
+        if 1 >= dropout >= 0:
+            logger.info(f"Use Dropout value: {dropout}")
+        self.dropout = dropout
+        self.rank_dropout = rank_dropout
+        self.module_dropout = module_dropout
+
+        self.use_tucker = use_tucker
+
+        def create_single_module(
+            lora_name: str,
+            module: torch.nn.Module,
+            algo_name,
+            dim=None,
+            alpha=None,
+            use_tucker=self.use_tucker,
+            **kwargs,
+        ):
+            for k, v in root_kwargs.items():
+                if k in kwargs:
+                    continue
+                kwargs[k] = v
+
+            if train_norm and "Norm" in module.__class__.__name__:
+                return norm_modules(
+                    lora_name,
+                    module,
+                    self.multiplier,
+                    self.rank_dropout,
+                    self.module_dropout,
+                    **kwargs,
+                )
+            lora = None
+            if isinstance(module, torch.nn.Linear) and lora_dim > 0:
+                dim = dim or lora_dim
+                alpha = alpha or self.alpha
+            elif isinstance(module, torch.nn.Conv2d):
+                k_size, *_ = module.kernel_size
+                if k_size == 1 and lora_dim > 0:
+                    dim = dim or lora_dim
+                    alpha = alpha or self.alpha
+                elif conv_lora_dim > 0 or dim:
+                    dim = dim or conv_lora_dim
+                    alpha = alpha or self.conv_alpha
+                else:
+                    return None
+            else:
+                return None
+            lora = network_module_dict[algo_name](
+                lora_name,
+                module,
+                self.multiplier,
+                dim,
+                alpha,
+                self.dropout,
+                self.rank_dropout,
+                self.module_dropout,
+                use_tucker,
+                **kwargs,
+            )
+            return lora
+
+        def create_modules_(
+            prefix: str,
+            root_module: torch.nn.Module,
+            algo,
+            configs={},
+        ):
+            loras = {}
+            lora_names = []
+            for name, module in root_module.named_modules():
+                module_name = module.__class__.__name__
+                if module_name in self.MODULE_ALGO_MAP:
+                    next_config = self.MODULE_ALGO_MAP[module_name]
+                    next_algo = next_config.get("algo", algo)
+                    new_loras, new_lora_names = create_modules_(
+                        f"{prefix}_{name}", module, next_algo, next_config
+                    )
+                    for lora_name, lora in zip(new_lora_names, new_loras):
+                        if lora_name not in loras:
+                            loras[lora_name] = lora
+                            lora_names.append(lora_name)
+                    continue
+                lora_name = prefix + "." + name
+                lora_name = lora_name.replace(".", "_")
+                if lora_name in loras:
+                    continue
+
+                lora = create_single_module(lora_name, module, algo, **configs)
+                if lora is not None:
+                    loras[lora_name] = lora
+                    lora_names.append(lora_name)
+            return [loras[lora_name] for lora_name in lora_names], lora_names
+
+        # create module instances
+        def create_modules(
+            prefix,
+            root_module: torch.nn.Module,
+            target_replace_modules,
+            target_replace_names=[],
+        ) -> List:
+            logger.info("Create LyCORIS Module")
+            loras = []
+            next_config = {}
+            for name, module in root_module.named_modules():
+                module_name = module.__class__.__name__
+                if module_name in target_replace_modules:
+                    if module_name in self.MODULE_ALGO_MAP:
+                        next_config = self.MODULE_ALGO_MAP[module_name]
+                        algo = next_config.get("algo", network_module)
+                    else:
+                        algo = network_module
+                    loras.extend(
+                        create_modules_(f"{prefix}_{name}", module, algo, next_config)[
+                            0
+                        ]
+                    )
+                    next_config = {}
+                elif name in target_replace_names or any(
+                    re.match(t, name) for t in target_replace_names
+                ):
+                    if name in self.NAME_ALGO_MAP:
+                        next_config = self.NAME_ALGO_MAP[name]
+                        algo = next_config.get("algo", network_module)
+                    elif module_name in self.MODULE_ALGO_MAP:
+                        next_config = self.MODULE_ALGO_MAP[module_name]
+                        algo = next_config.get("algo", network_module)
+                    else:
+                        algo = network_module
+                    lora_name = prefix + "." + name
+                    lora_name = lora_name.replace(".", "_")
+                    lora = create_single_module(lora_name, module, algo, **next_config)
+                    next_config = {}
+                    if lora is not None:
+                        loras.append(lora)
+            return loras
+
+        self.loras = create_modules(
+            LycorisNetwork.LORA_PREFIX,
+            module,
+            LycorisNetwork.TARGET_REPLACE_MODULE,
+            LycorisNetwork.TARGET_REPLACE_NAME,
+        )
+        logger.info(f"create LyCORIS: {len(self.loras)} modules.")
+
+        algo_table = {}
+        for lora in self.loras:
+            algo_table[lora.__class__.__name__] = (
+                algo_table.get(lora.__class__.__name__, 0) + 1
+            )
+        logger.info(f"module type table: {algo_table}")
+
+        self.weights_sd = None
+
+        # assertion
+        names = set()
+        for lora in self.loras:
+            assert (
+                lora.lora_name not in names
+            ), f"duplicated lora name: {lora.lora_name}"
+            names.add(lora.lora_name)
+
+    def set_multiplier(self, multiplier):
+        self.multiplier = multiplier
+        for lora in self.loras:
+            lora.multiplier = self.multiplier
+
+    def load_weights(self, file):
+        if os.path.splitext(file)[1] == ".safetensors":
+            from safetensors.torch import load_file, safe_open
+
+            self.weights_sd = load_file(file)
+        else:
+            self.weights_sd = torch.load(file, map_location="cpu")
+        missing, unexpected = self.load_state_dict(self.weights_sd, strict=False)
+        state = {}
+        if missing:
+            state["missing keys"] = missing
+        if unexpected:
+            state["unexpected keys"] = unexpected
+        return state
+
+    def apply_to(self):
+        for lora in self.loras:
+            lora.apply_to()
+            self.add_module(lora.lora_name, lora)
+
+        if self.weights_sd:
+            # if some weights are not in state dict, it is ok because initial LoRA does nothing (lora_up is initialized by zeros)
+            info = self.load_state_dict(self.weights_sd, False)
+            logger.info(f"weights are loaded: {info}")
+
+    def is_mergeable(self):
+        return True
+
+    def restore(self):
+        for lora in self.loras:
+            lora.restore()
+
+    def merge_to(self, weight=1.0):
+        for lora in self.loras:
+            lora.merge_to(weight)
+
+    def apply_max_norm_regularization(self, max_norm_value, device):
+        key_scaled = 0
+        norms = []
+        for model in self.loras:
+            if hasattr(model, "apply_max_norm"):
+                scaled, norm = model.apply_max_norm(max_norm_value, device)
+                norms.append(norm)
+                key_scaled += scaled
+
+        if key_scaled == 0:
+            return key_scaled, 0, 0
+
+        return key_scaled, sum(norms) / len(norms), max(norms)
+
+    def enable_gradient_checkpointing(self):
+        # not supported
+        def make_ckpt(module):
+            if isinstance(module, torch.nn.Module):
+                module.grad_ckpt = True
+
+        self.apply(make_ckpt)
+        pass
+
+    def prepare_optimizer_params(self, lr):
+        def enumerate_params(loras):
+            params = []
+            for lora in loras:
+                params.extend(lora.parameters())
+            return params
+
+        self.requires_grad_(True)
+        all_params = []
+
+        param_data = {"params": enumerate_params(self.loras)}
+        if lr is not None:
+            param_data["lr"] = lr
+        all_params.append(param_data)
+        return all_params
+
+    def prepare_grad_etc(self, *args):
+        self.requires_grad_(True)
+
+    def on_epoch_start(self, *args):
+        self.train()
+
+    def get_trainable_params(self, *args):
+        return self.parameters()
+
+    def save_weights(self, file, dtype, metadata):
+        if metadata is not None and len(metadata) == 0:
+            metadata = None
+
+        state_dict = self.state_dict()
+
+        if dtype is not None:
+            for key in list(state_dict.keys()):
+                v = state_dict[key]
+                v = v.detach().clone().to("cpu").to(dtype)
+                state_dict[key] = v
+
+        if os.path.splitext(file)[1] == ".safetensors":
+            from safetensors.torch import save_file
+
+            # Precalculate model hashes to save time on indexing
+            if metadata is None:
+                metadata = {}
+            save_file(state_dict, file, metadata)
+        else:
+            torch.save(state_dict, file)
```

### Comparing `lycoris_lora-2.3.0.dev4/lycoris_lora.egg-info/PKG-INFO` & `lycoris_lora-2.3.0.dev5/lycoris_lora.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1
-Name: lycoris_lora
-Version: 2.3.0.dev4
-Summary: Lora beYond Conventional methods, Other Rank adaptation Implementations for Stable diffusion
-Home-page: https://github.com/KohakuBlueleaf/LyCORIS
-Author: Shih-Ying Yeh(KohakuBlueLeaf), Yu-Guan Hsieh, Zhidong Gao
-Author-email: apolloyeh0123@gmail.com
-Requires-Python: >=3.10
-License-File: LICENSE.md
-Requires-Dist: torch
-Requires-Dist: safetensors
-Requires-Dist: diffusers
-Requires-Dist: transformers
-Requires-Dist: einops
-Requires-Dist: toml
+Metadata-Version: 2.1
+Name: lycoris_lora
+Version: 2.3.0.dev5
+Summary: Lora beYond Conventional methods, Other Rank adaptation Implementations for Stable diffusion
+Home-page: https://github.com/KohakuBlueleaf/LyCORIS
+Author: Shih-Ying Yeh(KohakuBlueLeaf), Yu-Guan Hsieh, Zhidong Gao
+Author-email: apolloyeh0123@gmail.com
+Requires-Python: >=3.10
+License-File: LICENSE.md
+Requires-Dist: torch
+Requires-Dist: safetensors
+Requires-Dist: diffusers
+Requires-Dist: transformers
+Requires-Dist: einops
+Requires-Dist: toml
```

### Comparing `lycoris_lora-2.3.0.dev4/lycoris_lora.egg-info/SOURCES.txt` & `lycoris_lora-2.3.0.dev5/lycoris_lora.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 lycoris/hcp/loha.py
 lycoris/hcp/lokr.py
 lycoris/kohya/__init__.py
 lycoris/kohya/model_utils.py
 lycoris/kohya/original_unet.py
 lycoris/kohya/sdxl_model_util.py
 lycoris/kohya/sdxl_original_unet.py
-lycoris/kohya/test_hyperdream.py
 lycoris/kohya/utils.py
 lycoris/modules/__init__.py
 lycoris/modules/attention.py
 lycoris/modules/base.py
 lycoris/modules/boft.py
 lycoris/modules/diag_oft.py
 lycoris/modules/dylora.py
@@ -35,15 +34,14 @@
 lycoris/modules/hypernet/__init__.py
 lycoris/modules/hypernet/generater.py
 lycoris/modules/hypernet/text_encoder.py
 lycoris/utils/__init__.py
 lycoris/utils/bnb.py
 lycoris/utils/logger.py
 lycoris/utils/preset.py
-lycoris/utils/tensor_norm.py
 lycoris/utils/xformers_utils.py
 lycoris_lora.egg-info/PKG-INFO
 lycoris_lora.egg-info/SOURCES.txt
 lycoris_lora.egg-info/dependency_links.txt
 lycoris_lora.egg-info/not-zip-safe
 lycoris_lora.egg-info/requires.txt
 lycoris_lora.egg-info/top_level.txt
```

