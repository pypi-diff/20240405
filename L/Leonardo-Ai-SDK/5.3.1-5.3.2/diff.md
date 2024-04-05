# Comparing `tmp/Leonardo-Ai-SDK-5.3.1.tar.gz` & `tmp/Leonardo-Ai-SDK-5.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Leonardo-Ai-SDK-5.3.1.tar", last modified: Wed Apr  3 00:40:24 2024, max compression
+gzip compressed data, was "Leonardo-Ai-SDK-5.3.2.tar", last modified: Fri Apr  5 00:03:25 2024, max compression
```

## Comparing `Leonardo-Ai-SDK-5.3.1.tar` & `Leonardo-Ai-SDK-5.3.2.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:40:24.307907 Leonardo-Ai-SDK-5.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    12098 2024-04-03 00:40:24.307907 Leonardo-Ai-SDK-5.3.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     9597 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 00:40:24.307907 Leonardo-Ai-SDK-5.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:40:24.295907 Leonardo-Ai-SDK-5.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:40:24.299907 Leonardo-Ai-SDK-5.3.1/src/Leonardo_Ai_SDK.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12098 2024-04-03 00:40:24.000000 Leonardo-Ai-SDK-5.3.1/src/Leonardo_Ai_SDK.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-04-03 00:40:24.000000 Leonardo-Ai-SDK-5.3.1/src/Leonardo_Ai_SDK.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 00:40:24.000000 Leonardo-Ai-SDK-5.3.1/src/Leonardo_Ai_SDK.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-03 00:40:24.000000 Leonardo-Ai-SDK-5.3.1/src/Leonardo_Ai_SDK.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-03 00:40:24.000000 Leonardo-Ai-SDK-5.3.1/src/Leonardo_Ai_SDK.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:40:24.299907 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:40:24.299907 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/_hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/_hooks/sdkhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/_hooks/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    17468 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/element.py
--rw-r--r--   0 runner    (1001) docker     (127)    45180 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/generation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10093 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/initimage.py
--rw-r--r--   0 runner    (1001) docker     (127)    27312 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:40:24.299907 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:40:24.299907 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/errors/sdkerror.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:40:24.307907 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/
--rw-r--r--   0 runner    (1001) docker     (127)     6157 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/createdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    15090 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/creategeneration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4960 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/createlcmgeneration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4497 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/createmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/createsvdmotiongeneration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/createtexturegeneration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/createvariationnobg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/createvariationunzoom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/createvariationupscale.py
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/delete3dmodelbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/deletedatasetbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/deletegenerationbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/deleteinitimagebyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/deletemodelbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/deletetexturegenerationbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/get3dmodelbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/get3dmodelsbyuserid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/getdatasetbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)    14832 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/getgenerationbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)    15044 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/getgenerationsbyuserid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/getinitimagebyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/getmodelbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/gettexturegenerationbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/gettexturegenerationsbymodelid.py
--rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/getuserself.py
--rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/getvariationbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/listelements.py
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/listplatformmodels.py
--rw-r--r--   0 runner    (1001) docker     (127)     6200 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/performalchemyupscalelcm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5351 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/performinpaintinglcm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/performinstantrefine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/uploaddatasetimage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/uploaddatasetimagefromgen.py
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/uploadinitimage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/uploadmodelasset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:40:24.307907 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/shared/
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/shared/controlnet_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/shared/custom_model_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/shared/element_input.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/shared/job_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/shared/lcm_generation_style.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/shared/model_asset_texture_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/shared/sd_generation_schedulers.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/shared/sd_generation_style.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/shared/sd_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/shared/security.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/shared/strength.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/shared/variation_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/sdkconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:40:24.307907 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/utils/retries.py
--rw-r--r--   0 runner    (1001) docker     (127)    30022 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13782 2024-04-03 00:40:15.000000 Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/variation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:03:25.378001 Leonardo-Ai-SDK-5.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    15122 2024-04-05 00:03:25.378001 Leonardo-Ai-SDK-5.3.2/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9597 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 00:03:25.378001 Leonardo-Ai-SDK-5.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:03:25.366001 Leonardo-Ai-SDK-5.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:03:25.370000 Leonardo-Ai-SDK-5.3.2/src/Leonardo_Ai_SDK.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15122 2024-04-05 00:03:25.000000 Leonardo-Ai-SDK-5.3.2/src/Leonardo_Ai_SDK.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-04-05 00:03:25.000000 Leonardo-Ai-SDK-5.3.2/src/Leonardo_Ai_SDK.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 00:03:25.000000 Leonardo-Ai-SDK-5.3.2/src/Leonardo_Ai_SDK.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-05 00:03:25.000000 Leonardo-Ai-SDK-5.3.2/src/Leonardo_Ai_SDK.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-05 00:03:25.000000 Leonardo-Ai-SDK-5.3.2/src/Leonardo_Ai_SDK.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:03:25.370000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:03:25.370000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/_hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/_hooks/sdkhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/_hooks/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17468 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/element.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45180 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10093 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/initimage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27312 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:03:25.370000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:03:25.370000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/errors/sdkerror.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:03:25.378001 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)     6157 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/createdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15135 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/creategeneration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4960 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/createlcmgeneration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/createmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/createsvdmotiongeneration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/createtexturegeneration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/createvariationnobg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/createvariationunzoom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/createvariationupscale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/delete3dmodelbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/deletedatasetbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/deletegenerationbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/deleteinitimagebyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/deletemodelbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/deletetexturegenerationbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/get3dmodelbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/get3dmodelsbyuserid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/getdatasetbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14922 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/getgenerationbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15134 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/getgenerationsbyuserid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/getinitimagebyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/getmodelbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/gettexturegenerationbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/gettexturegenerationsbymodelid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/getuserself.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/getvariationbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/listelements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/listplatformmodels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6200 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/performalchemyupscalelcm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5351 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/performinpaintinglcm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/performinstantrefine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/uploaddatasetimage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/uploaddatasetimagefromgen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/uploadinitimage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/uploadmodelasset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:03:25.378001 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/shared/controlnet_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/shared/custom_model_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/shared/element_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/shared/job_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/shared/lcm_generation_style.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/shared/model_asset_texture_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/shared/sd_generation_schedulers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/shared/sd_generation_style.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/shared/sd_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/shared/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/shared/strength.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/shared/variation_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/sdkconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:03:25.378001 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/utils/retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30022 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13782 2024-04-05 00:03:14.000000 Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/variation.py
```

### Comparing `Leonardo-Ai-SDK-5.3.1/LICENSE.md` & `Leonardo-Ai-SDK-5.3.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.1/PKG-INFO` & `Leonardo-Ai-SDK-5.3.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,284 +1,272 @@
-Metadata-Version: 2.1
-Name: Leonardo-Ai-SDK
-Version: 5.3.1
-Summary: Leonardo AI Python Client SDK
-Home-page: https://github.com/Leonardo-Interactive/leonardo-python-sdk.git
-Author: Leonardo-Ai
-License: UNKNOWN
-Description: # Leonardo-Ai-SDK
-        
-        <a href="https://codespaces.new/Leonardo-Interactive/leonardo-python-sdk.git/tree/main"><img src="https://github.com/codespaces/badge.svg" /></a>
-        
-        <!-- Start SDK Installation [installation] -->
-        ## SDK Installation
-        
-        ```bash
-        pip install Leonardo-Ai-SDK
-        ```
-        <!-- End SDK Installation [installation] -->
-        
-        <!-- Start SDK Example Usage [usage] -->
-        ## SDK Example Usage
-        
-        ### Example
-        
-        ```python
-        import leonardoaisdk
-        from leonardoaisdk.models import operations
-        
-        s = leonardoaisdk.LeonardoAiSDK(
-            bearer_auth="<YOUR_BEARER_TOKEN_HERE>",
-        )
-        
-        req = operations.CreateDatasetRequestBody(
-            name='<value>',
-        )
-        
-        res = s.dataset.create_dataset(req)
-        
-        if res.object is not None:
-            # handle response
-            pass
-        
-        ```
-        <!-- End SDK Example Usage [usage] -->
-        
-        <!-- Start Available Resources and Operations [operations] -->
-        ## Available Resources and Operations
-        
-        ### [dataset](docs/sdks/dataset/README.md)
-        
-        * [create_dataset](docs/sdks/dataset/README.md#create_dataset) - Create a Dataset
-        * [delete_dataset_by_id](docs/sdks/dataset/README.md#delete_dataset_by_id) - Delete a Single Dataset by ID
-        * [get_dataset_by_id](docs/sdks/dataset/README.md#get_dataset_by_id) - Get a Single Dataset by ID
-        * [upload_dataset_image](docs/sdks/dataset/README.md#upload_dataset_image) - Upload dataset image
-        * [upload_dataset_image_from_gen](docs/sdks/dataset/README.md#upload_dataset_image_from_gen) - Upload a Single Generated Image to a Dataset
-        
-        ### [element](docs/sdks/element/README.md)
-        
-        * [list_elements](docs/sdks/element/README.md#list_elements) - List Elements
-        
-        ### [generation](docs/sdks/generation/README.md)
-        
-        * [create_generation](docs/sdks/generation/README.md#create_generation) - Create a Generation of Images
-        * [create_lcm_generation](docs/sdks/generation/README.md#create_lcm_generation) - Create LCM Generation
-        * [create_svd_motion_generation](docs/sdks/generation/README.md#create_svd_motion_generation) - Create SVD Motion Generation
-        * [create_texture_generation](docs/sdks/generation/README.md#create_texture_generation) - Create Texture Generation
-        * [delete_generation_by_id](docs/sdks/generation/README.md#delete_generation_by_id) - Delete a Single Generation
-        * [delete_texture_generation_by_id](docs/sdks/generation/README.md#delete_texture_generation_by_id) - Delete Texture Generation by ID
-        * [get_generation_by_id](docs/sdks/generation/README.md#get_generation_by_id) - Get a Single Generation
-        * [get_generations_by_user_id](docs/sdks/generation/README.md#get_generations_by_user_id) - Get generations by user ID
-        * [get_texture_generation_by_id](docs/sdks/generation/README.md#get_texture_generation_by_id) - Get Texture Generation by ID
-        * [get_texture_generations_by_model_id](docs/sdks/generation/README.md#get_texture_generations_by_model_id) - Get texture generations by 3D Model ID
-        * [perform_alchemy_upscale_lcm](docs/sdks/generation/README.md#perform_alchemy_upscale_lcm) - Perform Alchemy Upscale on a LCM image
-        * [perform_inpainting_lcm](docs/sdks/generation/README.md#perform_inpainting_lcm) - Perform inpainting on a LCM image
-        * [perform_instant_refine](docs/sdks/generation/README.md#perform_instant_refine) - Perform instant refine on a LCM image
-        
-        ### [init_image](docs/sdks/initimage/README.md)
-        
-        * [delete_init_image_by_id](docs/sdks/initimage/README.md#delete_init_image_by_id) - Delete init image
-        * [get_init_image_by_id](docs/sdks/initimage/README.md#get_init_image_by_id) - Get single init image
-        * [upload_init_image](docs/sdks/initimage/README.md#upload_init_image) - Upload init image
-        
-        ### [user](docs/sdks/user/README.md)
-        
-        * [get_user_self](docs/sdks/user/README.md#get_user_self) - Get user information
-        
-        ### [model](docs/sdks/model/README.md)
-        
-        * [create_model](docs/sdks/model/README.md#create_model) - Train a Custom Model
-        * [delete3_d_model_by_id](docs/sdks/model/README.md#delete3_d_model_by_id) - Delete 3D Model by ID
-        * [delete_model_by_id](docs/sdks/model/README.md#delete_model_by_id) - Delete a Single Custom Model by ID
-        * [get3_d_model_by_id](docs/sdks/model/README.md#get3_d_model_by_id) - Get 3D Model by ID
-        * [get3_d_models_by_user_id](docs/sdks/model/README.md#get3_d_models_by_user_id) - Get 3D models by user ID
-        * [get_model_by_id](docs/sdks/model/README.md#get_model_by_id) - Get a Single Custom Model by ID
-        * [list_platform_models](docs/sdks/model/README.md#list_platform_models) - List Platform Models
-        * [upload_model_asset](docs/sdks/model/README.md#upload_model_asset) - Upload 3D Model
-        
-        ### [variation](docs/sdks/variation/README.md)
-        
-        * [create_variation_no_bg](docs/sdks/variation/README.md#create_variation_no_bg) - Create no background
-        * [create_variation_unzoom](docs/sdks/variation/README.md#create_variation_unzoom) - Create unzoom
-        * [create_variation_upscale](docs/sdks/variation/README.md#create_variation_upscale) - Create upscale
-        * [get_variation_by_id](docs/sdks/variation/README.md#get_variation_by_id) - Get variation by ID
-        <!-- End Available Resources and Operations [operations] -->
-        
-        
-        
-        
-        
-        
-        
-        <!-- Start Error Handling [errors] -->
-        ## Error Handling
-        
-        Handling errors in this SDK should largely match your expectations.  All operations return a response object or raise an error.  If Error objects are specified in your OpenAPI Spec, the SDK will raise the appropriate Error type.
-        
-        | Error Object    | Status Code     | Content Type    |
-        | --------------- | --------------- | --------------- |
-        | errors.SDKError | 4xx-5xx         | */*             |
-        
-        ### Example
-        
-        ```python
-        import leonardoaisdk
-        from leonardoaisdk.models import errors, operations
-        
-        s = leonardoaisdk.LeonardoAiSDK(
-            bearer_auth="<YOUR_BEARER_TOKEN_HERE>",
-        )
-        
-        req = operations.CreateDatasetRequestBody(
-            name='<value>',
-        )
-        
-        res = None
-        try:
-            res = s.dataset.create_dataset(req)
-        except errors.SDKError as e:
-            # handle exception
-            raise(e)
-        
-        if res.object is not None:
-            # handle response
-            pass
-        
-        ```
-        <!-- End Error Handling [errors] -->
-        
-        
-        
-        <!-- Start Custom HTTP Client [http-client] -->
-        ## Custom HTTP Client
-        
-        The Python SDK makes API calls using the [requests](https://pypi.org/project/requests/) HTTP library.  In order to provide a convenient way to configure timeouts, cookies, proxies, custom headers, and other low-level configuration, you can initialize the SDK client with a custom `requests.Session` object.
-        
-        For example, you could specify a header for every request that this sdk makes as follows:
-        ```python
-        import leonardoaisdk
-        import requests
-        
-        http_client = requests.Session()
-        http_client.headers.update({'x-custom-header': 'someValue'})
-        s = leonardoaisdk.LeonardoAiSDK(client=http_client)
-        ```
-        <!-- End Custom HTTP Client [http-client] -->
-        
-        
-        
-        <!-- Start Server Selection [server] -->
-        ## Server Selection
-        
-        ### Select Server by Index
-        
-        You can override the default server globally by passing a server index to the `server_idx: int` optional parameter when initializing the SDK client instance. The selected server will then be used as the default on the operations that use it. This table lists the indexes associated with the available servers:
-        
-        | # | Server | Variables |
-        | - | ------ | --------- |
-        | 0 | `https://cloud.leonardo.ai/api/rest/v1` | None |
-        
-        #### Example
-        
-        ```python
-        import leonardoaisdk
-        from leonardoaisdk.models import operations
-        
-        s = leonardoaisdk.LeonardoAiSDK(
-            server_idx=0,
-            bearer_auth="<YOUR_BEARER_TOKEN_HERE>",
-        )
-        
-        req = operations.CreateDatasetRequestBody(
-            name='<value>',
-        )
-        
-        res = s.dataset.create_dataset(req)
-        
-        if res.object is not None:
-            # handle response
-            pass
-        
-        ```
-        
-        
-        ### Override Server URL Per-Client
-        
-        The default server can also be overridden globally by passing a URL to the `server_url: str` optional parameter when initializing the SDK client instance. For example:
-        ```python
-        import leonardoaisdk
-        from leonardoaisdk.models import operations
-        
-        s = leonardoaisdk.LeonardoAiSDK(
-            server_url="https://cloud.leonardo.ai/api/rest/v1",
-            bearer_auth="<YOUR_BEARER_TOKEN_HERE>",
-        )
-        
-        req = operations.CreateDatasetRequestBody(
-            name='<value>',
-        )
-        
-        res = s.dataset.create_dataset(req)
-        
-        if res.object is not None:
-            # handle response
-            pass
-        
-        ```
-        <!-- End Server Selection [server] -->
-        
-        
-        
-        <!-- Start Authentication [security] -->
-        ## Authentication
-        
-        ### Per-Client Security Schemes
-        
-        This SDK supports the following security scheme globally:
-        
-        | Name          | Type          | Scheme        |
-        | ------------- | ------------- | ------------- |
-        | `bearer_auth` | http          | HTTP Bearer   |
-        
-        To authenticate with the API the `bearer_auth` parameter must be set when initializing the SDK client instance. For example:
-        ```python
-        import leonardoaisdk
-        from leonardoaisdk.models import operations
-        
-        s = leonardoaisdk.LeonardoAiSDK(
-            bearer_auth="<YOUR_BEARER_TOKEN_HERE>",
-        )
-        
-        req = operations.CreateDatasetRequestBody(
-            name='<value>',
-        )
-        
-        res = s.dataset.create_dataset(req)
-        
-        if res.object is not None:
-            # handle response
-            pass
-        
-        ```
-        <!-- End Authentication [security] -->
-        
-        <!-- Placeholder for Future Speakeasy SDK Sections -->
-        
-        
-        
-        ### Maturity
-        
-        This SDK is in beta, and there may be breaking changes between versions without a major version update. Therefore, we recommend pinning usage
-        to a specific package version. This way, you can install the same version each time without breaking changes unless you are intentionally
-        looking for the latest version.
-        
-        ### Contributions
-        
-        While we value open-source contributions to this SDK, this library is generated programmatically.
-        Feel free to open a PR or a Github issue as a proof of concept and we'll do our best to include it in a future release !
-        
-        ### SDK Created by [Speakeasy](https://docs.speakeasyapi.dev/docs/using-speakeasy/client-sdks)
-        
-Platform: UNKNOWN
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
+# Leonardo-Ai-SDK
+
+<a href="https://codespaces.new/Leonardo-Interactive/leonardo-python-sdk.git/tree/main"><img src="https://github.com/codespaces/badge.svg" /></a>
+
+<!-- Start SDK Installation [installation] -->
+## SDK Installation
+
+```bash
+pip install Leonardo-Ai-SDK
+```
+<!-- End SDK Installation [installation] -->
+
+<!-- Start SDK Example Usage [usage] -->
+## SDK Example Usage
+
+### Example
+
+```python
+import leonardoaisdk
+from leonardoaisdk.models import operations
+
+s = leonardoaisdk.LeonardoAiSDK(
+    bearer_auth="<YOUR_BEARER_TOKEN_HERE>",
+)
+
+req = operations.CreateDatasetRequestBody(
+    name='<value>',
+)
+
+res = s.dataset.create_dataset(req)
+
+if res.object is not None:
+    # handle response
+    pass
+
+```
+<!-- End SDK Example Usage [usage] -->
+
+<!-- Start Available Resources and Operations [operations] -->
+## Available Resources and Operations
+
+### [dataset](docs/sdks/dataset/README.md)
+
+* [create_dataset](docs/sdks/dataset/README.md#create_dataset) - Create a Dataset
+* [delete_dataset_by_id](docs/sdks/dataset/README.md#delete_dataset_by_id) - Delete a Single Dataset by ID
+* [get_dataset_by_id](docs/sdks/dataset/README.md#get_dataset_by_id) - Get a Single Dataset by ID
+* [upload_dataset_image](docs/sdks/dataset/README.md#upload_dataset_image) - Upload dataset image
+* [upload_dataset_image_from_gen](docs/sdks/dataset/README.md#upload_dataset_image_from_gen) - Upload a Single Generated Image to a Dataset
+
+### [element](docs/sdks/element/README.md)
+
+* [list_elements](docs/sdks/element/README.md#list_elements) - List Elements
+
+### [generation](docs/sdks/generation/README.md)
+
+* [create_generation](docs/sdks/generation/README.md#create_generation) - Create a Generation of Images
+* [create_lcm_generation](docs/sdks/generation/README.md#create_lcm_generation) - Create LCM Generation
+* [create_svd_motion_generation](docs/sdks/generation/README.md#create_svd_motion_generation) - Create SVD Motion Generation
+* [create_texture_generation](docs/sdks/generation/README.md#create_texture_generation) - Create Texture Generation
+* [delete_generation_by_id](docs/sdks/generation/README.md#delete_generation_by_id) - Delete a Single Generation
+* [delete_texture_generation_by_id](docs/sdks/generation/README.md#delete_texture_generation_by_id) - Delete Texture Generation by ID
+* [get_generation_by_id](docs/sdks/generation/README.md#get_generation_by_id) - Get a Single Generation
+* [get_generations_by_user_id](docs/sdks/generation/README.md#get_generations_by_user_id) - Get generations by user ID
+* [get_texture_generation_by_id](docs/sdks/generation/README.md#get_texture_generation_by_id) - Get Texture Generation by ID
+* [get_texture_generations_by_model_id](docs/sdks/generation/README.md#get_texture_generations_by_model_id) - Get texture generations by 3D Model ID
+* [perform_alchemy_upscale_lcm](docs/sdks/generation/README.md#perform_alchemy_upscale_lcm) - Perform Alchemy Upscale on a LCM image
+* [perform_inpainting_lcm](docs/sdks/generation/README.md#perform_inpainting_lcm) - Perform inpainting on a LCM image
+* [perform_instant_refine](docs/sdks/generation/README.md#perform_instant_refine) - Perform instant refine on a LCM image
+
+### [init_image](docs/sdks/initimage/README.md)
+
+* [delete_init_image_by_id](docs/sdks/initimage/README.md#delete_init_image_by_id) - Delete init image
+* [get_init_image_by_id](docs/sdks/initimage/README.md#get_init_image_by_id) - Get single init image
+* [upload_init_image](docs/sdks/initimage/README.md#upload_init_image) - Upload init image
+
+### [user](docs/sdks/user/README.md)
+
+* [get_user_self](docs/sdks/user/README.md#get_user_self) - Get user information
+
+### [model](docs/sdks/model/README.md)
+
+* [create_model](docs/sdks/model/README.md#create_model) - Train a Custom Model
+* [delete3_d_model_by_id](docs/sdks/model/README.md#delete3_d_model_by_id) - Delete 3D Model by ID
+* [delete_model_by_id](docs/sdks/model/README.md#delete_model_by_id) - Delete a Single Custom Model by ID
+* [get3_d_model_by_id](docs/sdks/model/README.md#get3_d_model_by_id) - Get 3D Model by ID
+* [get3_d_models_by_user_id](docs/sdks/model/README.md#get3_d_models_by_user_id) - Get 3D models by user ID
+* [get_model_by_id](docs/sdks/model/README.md#get_model_by_id) - Get a Single Custom Model by ID
+* [list_platform_models](docs/sdks/model/README.md#list_platform_models) - List Platform Models
+* [upload_model_asset](docs/sdks/model/README.md#upload_model_asset) - Upload 3D Model
+
+### [variation](docs/sdks/variation/README.md)
+
+* [create_variation_no_bg](docs/sdks/variation/README.md#create_variation_no_bg) - Create no background
+* [create_variation_unzoom](docs/sdks/variation/README.md#create_variation_unzoom) - Create unzoom
+* [create_variation_upscale](docs/sdks/variation/README.md#create_variation_upscale) - Create upscale
+* [get_variation_by_id](docs/sdks/variation/README.md#get_variation_by_id) - Get variation by ID
+<!-- End Available Resources and Operations [operations] -->
+
+
+
+
+
+
+
+<!-- Start Error Handling [errors] -->
+## Error Handling
+
+Handling errors in this SDK should largely match your expectations.  All operations return a response object or raise an error.  If Error objects are specified in your OpenAPI Spec, the SDK will raise the appropriate Error type.
+
+| Error Object    | Status Code     | Content Type    |
+| --------------- | --------------- | --------------- |
+| errors.SDKError | 4xx-5xx         | */*             |
+
+### Example
+
+```python
+import leonardoaisdk
+from leonardoaisdk.models import errors, operations
+
+s = leonardoaisdk.LeonardoAiSDK(
+    bearer_auth="<YOUR_BEARER_TOKEN_HERE>",
+)
+
+req = operations.CreateDatasetRequestBody(
+    name='<value>',
+)
+
+res = None
+try:
+    res = s.dataset.create_dataset(req)
+except errors.SDKError as e:
+    # handle exception
+    raise(e)
+
+if res.object is not None:
+    # handle response
+    pass
+
+```
+<!-- End Error Handling [errors] -->
+
+
+
+<!-- Start Custom HTTP Client [http-client] -->
+## Custom HTTP Client
+
+The Python SDK makes API calls using the [requests](https://pypi.org/project/requests/) HTTP library.  In order to provide a convenient way to configure timeouts, cookies, proxies, custom headers, and other low-level configuration, you can initialize the SDK client with a custom `requests.Session` object.
+
+For example, you could specify a header for every request that this sdk makes as follows:
+```python
+import leonardoaisdk
+import requests
+
+http_client = requests.Session()
+http_client.headers.update({'x-custom-header': 'someValue'})
+s = leonardoaisdk.LeonardoAiSDK(client=http_client)
+```
+<!-- End Custom HTTP Client [http-client] -->
+
+
+
+<!-- Start Server Selection [server] -->
+## Server Selection
+
+### Select Server by Index
+
+You can override the default server globally by passing a server index to the `server_idx: int` optional parameter when initializing the SDK client instance. The selected server will then be used as the default on the operations that use it. This table lists the indexes associated with the available servers:
+
+| # | Server | Variables |
+| - | ------ | --------- |
+| 0 | `https://cloud.leonardo.ai/api/rest/v1` | None |
+
+#### Example
+
+```python
+import leonardoaisdk
+from leonardoaisdk.models import operations
+
+s = leonardoaisdk.LeonardoAiSDK(
+    server_idx=0,
+    bearer_auth="<YOUR_BEARER_TOKEN_HERE>",
+)
+
+req = operations.CreateDatasetRequestBody(
+    name='<value>',
+)
+
+res = s.dataset.create_dataset(req)
+
+if res.object is not None:
+    # handle response
+    pass
+
+```
+
+
+### Override Server URL Per-Client
+
+The default server can also be overridden globally by passing a URL to the `server_url: str` optional parameter when initializing the SDK client instance. For example:
+```python
+import leonardoaisdk
+from leonardoaisdk.models import operations
+
+s = leonardoaisdk.LeonardoAiSDK(
+    server_url="https://cloud.leonardo.ai/api/rest/v1",
+    bearer_auth="<YOUR_BEARER_TOKEN_HERE>",
+)
+
+req = operations.CreateDatasetRequestBody(
+    name='<value>',
+)
+
+res = s.dataset.create_dataset(req)
+
+if res.object is not None:
+    # handle response
+    pass
+
+```
+<!-- End Server Selection [server] -->
+
+
+
+<!-- Start Authentication [security] -->
+## Authentication
+
+### Per-Client Security Schemes
+
+This SDK supports the following security scheme globally:
+
+| Name          | Type          | Scheme        |
+| ------------- | ------------- | ------------- |
+| `bearer_auth` | http          | HTTP Bearer   |
+
+To authenticate with the API the `bearer_auth` parameter must be set when initializing the SDK client instance. For example:
+```python
+import leonardoaisdk
+from leonardoaisdk.models import operations
+
+s = leonardoaisdk.LeonardoAiSDK(
+    bearer_auth="<YOUR_BEARER_TOKEN_HERE>",
+)
+
+req = operations.CreateDatasetRequestBody(
+    name='<value>',
+)
+
+res = s.dataset.create_dataset(req)
+
+if res.object is not None:
+    # handle response
+    pass
+
+```
+<!-- End Authentication [security] -->
+
+<!-- Placeholder for Future Speakeasy SDK Sections -->
+
+
+
+### Maturity
+
+This SDK is in beta, and there may be breaking changes between versions without a major version update. Therefore, we recommend pinning usage
+to a specific package version. This way, you can install the same version each time without breaking changes unless you are intentionally
+looking for the latest version.
+
+### Contributions
+
+While we value open-source contributions to this SDK, this library is generated programmatically.
+Feel free to open a PR or a Github issue as a proof of concept and we'll do our best to include it in a future release !
+
+### SDK Created by [Speakeasy](https://docs.speakeasyapi.dev/docs/using-speakeasy/client-sdks)
```

#### html2text {}

```diff
@@ -1,13 +1,10 @@
-Metadata-Version: 2.1 Name: Leonardo-Ai-SDK Version: 5.3.1 Summary: Leonardo AI
-Python Client SDK Home-page: https://github.com/Leonardo-Interactive/leonardo-
-python-sdk.git Author: Leonardo-Ai License: UNKNOWN Description: # Leonardo-Ai-
-SDK _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_c_o_d_e_s_p_a_c_e_s_/_b_a_d_g_e_._s_v_g_]## SDK Installation ```bash pip
-install Leonardo-Ai-SDK ``` ## SDK Example Usage ### Example ```python import
-leonardoaisdk from leonardoaisdk.models import operations s =
+# Leonardo-Ai-SDK _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_c_o_d_e_s_p_a_c_e_s_/_b_a_d_g_e_._s_v_g_]## SDK Installation
+```bash pip install Leonardo-Ai-SDK ``` ## SDK Example Usage ### Example
+```python import leonardoaisdk from leonardoaisdk.models import operations s =
 leonardoaisdk.LeonardoAiSDK( bearer_auth="", ) req =
 operations.CreateDatasetRequestBody( name='', ) res = s.dataset.create_dataset
 (req) if res.object is not None: # handle response pass ``` ## Available
 Resources and Operations ### [dataset](docs/sdks/dataset/README.md) *
 [create_dataset](docs/sdks/dataset/README.md#create_dataset) - Create a Dataset
 * [delete_dataset_by_id](docs/sdks/dataset/README.md#delete_dataset_by_id) -
 Delete a Single Dataset by ID * [get_dataset_by_id](docs/sdks/dataset/
@@ -112,9 +109,8 @@
 major version update. Therefore, we recommend pinning usage to a specific
 package version. This way, you can install the same version each time without
 breaking changes unless you are intentionally looking for the latest version.
 ### Contributions While we value open-source contributions to this SDK, this
 library is generated programmatically. Feel free to open a PR or a Github issue
 as a proof of concept and we'll do our best to include it in a future release !
 ### SDK Created by [Speakeasy](https://docs.speakeasyapi.dev/docs/using-
-speakeasy/client-sdks) Platform: UNKNOWN Requires-Python: >=3.8 Description-
-Content-Type: text/markdown Provides-Extra: dev
+speakeasy/client-sdks)
```

### Comparing `Leonardo-Ai-SDK-5.3.1/src/Leonardo_Ai_SDK.egg-info/SOURCES.txt` & `Leonardo-Ai-SDK-5.3.2/src/Leonardo_Ai_SDK.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/_hooks/sdkhooks.py` & `Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/_hooks/sdkhooks.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/_hooks/types.py` & `Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/_hooks/types.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/dataset.py` & `Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/dataset.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/element.py` & `Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/element.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/generation.py` & `Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/generation.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/initimage.py` & `Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/initimage.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/model.py` & `Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/model.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/errors/sdkerror.py` & `Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/errors/sdkerror.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/__init__.py` & `Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/createdataset.py` & `Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/createdataset.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/creategeneration.py` & `Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/creategeneration.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
     prompt_magic_version: Optional[str] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('promptMagicVersion'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""Prompt magic version v2 or v3, for use when promptMagic: true"""
     public: Optional[bool] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('public'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""Whether the generated images should show in the community feed."""
     scheduler: Optional[shared_sd_generation_schedulers.SdGenerationSchedulers] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('scheduler'), 'exclude': lambda f: f is None }})
     r"""The scheduler to generate images with. Defaults to EULER_DISCRETE if not specified."""
     sd_version: Optional[shared_sd_versions.SdVersions] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sd_version'), 'exclude': lambda f: f is None }})
-    r"""The base version of stable diffusion to use if not using a custom model. v1_5 is 1.5, v2 is 2.1, if not specified it will default to v1_5."""
+    r"""The base version of stable diffusion to use if not using a custom model. v1_5 is 1.5, v2 is 2.1, if not specified it will default to v1_5. Also includes SDXL and SDXL Lightning models"""
     seed: Optional[int] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('seed'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     tiling: Optional[bool] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tiling'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""Whether the generated images should tile on all axis."""
     transparency: Optional[TransparencyType] = dataclasses.field(default=TransparencyType.DISABLED, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('transparency'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""Which type of transparency this image should use"""
     unzoom: Optional[bool] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('unzoom'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""Whether the generated images should be unzoomed (requires unzoomAmount and init_image_id to be set)."""
```

### Comparing `Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/createlcmgeneration.py` & `Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/createlcmgeneration.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/createmodel.py` & `Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/createmodel.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     model_type: Optional[shared_custom_model_type.CustomModelType] = dataclasses.field(default=shared_custom_model_type.CustomModelType.GENERAL, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modelType'), 'exclude': lambda f: f is None }})
     r"""The category the most accurately reflects the model."""
     nsfw: Optional[bool] = dataclasses.field(default=False, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nsfw'), 'exclude': lambda f: f is CreateModelRequestBody.UNSET }})
     r"""Whether or not the model is NSFW."""
     resolution: Optional[int] = dataclasses.field(default=512, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('resolution'), 'exclude': lambda f: f is CreateModelRequestBody.UNSET }})
     r"""The resolution for training. Must be 512 or 768."""
     sd_version: Optional[shared_sd_versions.SdVersions] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sd_Version'), 'exclude': lambda f: f is None }})
-    r"""The base version of stable diffusion to use if not using a custom model. v1_5 is 1.5, v2 is 2.1, if not specified it will default to v1_5."""
+    r"""The base version of stable diffusion to use if not using a custom model. v1_5 is 1.5, v2 is 2.1, if not specified it will default to v1_5. Also includes SDXL and SDXL Lightning models"""
     strength: Optional[shared_strength.Strength] = dataclasses.field(default=shared_strength.Strength.MEDIUM, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('strength'), 'exclude': lambda f: f is None }})
     r"""When training using the PIXEL_ART model type, this influences the training strength."""
     
 
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
```

### Comparing `Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/createsvdmotiongeneration.py` & `Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/createsvdmotiongeneration.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/createtexturegeneration.py` & `Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/createtexturegeneration.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/createvariationnobg.py` & `Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/createvariationnobg.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/createvariationunzoom.py` & `Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/createvariationunzoom.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/createvariationupscale.py` & `Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/createvariationupscale.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/delete3dmodelbyid.py` & `Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/delete3dmodelbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/deletedatasetbyid.py` & `Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/deletedatasetbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/deletegenerationbyid.py` & `Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/deletegenerationbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/deleteinitimagebyid.py` & `Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/deleteinitimagebyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/deletemodelbyid.py` & `Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/deletemodelbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/deletetexturegenerationbyid.py` & `Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/deletetexturegenerationbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/get3dmodelbyid.py` & `Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/get3dmodelbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/get3dmodelsbyuserid.py` & `Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/get3dmodelsbyuserid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/getdatasetbyid.py` & `Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/getdatasetbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/getgenerationbyid.py` & `Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/getgenerationbyid.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 @dataclasses.dataclass
 class GetGenerationByIDLoras:
     r"""Element used for the generation."""
     UNSET='__SPEAKEASY_UNSET__'
     ak_uuid: Optional[str] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('akUUID'), 'exclude': lambda f: f is GetGenerationByIDLoras.UNSET }})
     r"""Unique identifier for the element. Elements can be found from the List Elements endpoint."""
     base_model: Optional[shared_sd_versions.SdVersions] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('baseModel'), 'exclude': lambda f: f is None }})
-    r"""The base version of stable diffusion to use if not using a custom model. v1_5 is 1.5, v2 is 2.1, if not specified it will default to v1_5."""
+    r"""The base version of stable diffusion to use if not using a custom model. v1_5 is 1.5, v2 is 2.1, if not specified it will default to v1_5. Also includes SDXL and SDXL Lightning models"""
     description: Optional[str] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is GetGenerationByIDLoras.UNSET }})
     r"""Description for the element"""
     name: Optional[str] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is GetGenerationByIDLoras.UNSET }})
     r"""Name of the element"""
     url_image: Optional[str] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('urlImage'), 'exclude': lambda f: f is GetGenerationByIDLoras.UNSET }})
     r"""URL of the element image"""
     weight_default: Optional[int] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('weightDefault'), 'exclude': lambda f: f is GetGenerationByIDLoras.UNSET }})
@@ -129,15 +129,15 @@
     r"""Strength of prompt magic used."""
     prompt_magic_version: Optional[str] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('promptMagicVersion'), 'exclude': lambda f: f is GetGenerationByIDGenerations.UNSET }})
     r"""Version of prompt magic used."""
     public: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('public'), 'exclude': lambda f: f is None }})
     scheduler: Optional[shared_sd_generation_schedulers.SdGenerationSchedulers] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('scheduler'), 'exclude': lambda f: f is None }})
     r"""The scheduler to generate images with. Defaults to EULER_DISCRETE if not specified."""
     sd_version: Optional[shared_sd_versions.SdVersions] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sdVersion'), 'exclude': lambda f: f is None }})
-    r"""The base version of stable diffusion to use if not using a custom model. v1_5 is 1.5, v2 is 2.1, if not specified it will default to v1_5."""
+    r"""The base version of stable diffusion to use if not using a custom model. v1_5 is 1.5, v2 is 2.1, if not specified it will default to v1_5. Also includes SDXL and SDXL Lightning models"""
     seed: Optional[int] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('seed'), 'exclude': lambda f: f is GetGenerationByIDGenerations.UNSET }})
     status: Optional[shared_job_status.JobStatus] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
     r"""The status of the current task."""
```

### Comparing `Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/getgenerationsbyuserid.py` & `Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/getgenerationsbyuserid.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 @dataclasses.dataclass
 class Elements:
     r"""Element used for the generation."""
     UNSET='__SPEAKEASY_UNSET__'
     ak_uuid: Optional[str] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('akUUID'), 'exclude': lambda f: f is Elements.UNSET }})
     r"""Unique identifier for the element. Elements can be found from the List Elements endpoint."""
     base_model: Optional[shared_sd_versions.SdVersions] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('baseModel'), 'exclude': lambda f: f is None }})
-    r"""The base version of stable diffusion to use if not using a custom model. v1_5 is 1.5, v2 is 2.1, if not specified it will default to v1_5."""
+    r"""The base version of stable diffusion to use if not using a custom model. v1_5 is 1.5, v2 is 2.1, if not specified it will default to v1_5. Also includes SDXL and SDXL Lightning models"""
     description: Optional[str] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is Elements.UNSET }})
     r"""Description for the element"""
     name: Optional[str] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is Elements.UNSET }})
     r"""Name of the element"""
     url_image: Optional[str] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('urlImage'), 'exclude': lambda f: f is Elements.UNSET }})
     r"""URL of the element image"""
     weight_default: Optional[int] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('weightDefault'), 'exclude': lambda f: f is Elements.UNSET }})
@@ -128,15 +128,15 @@
     r"""Strength of prompt magic used."""
     prompt_magic_version: Optional[str] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('promptMagicVersion'), 'exclude': lambda f: f is GetGenerationsByUserIDGenerations.UNSET }})
     r"""Version of prompt magic used."""
     public: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('public'), 'exclude': lambda f: f is None }})
     scheduler: Optional[shared_sd_generation_schedulers.SdGenerationSchedulers] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('scheduler'), 'exclude': lambda f: f is None }})
     r"""The scheduler to generate images with. Defaults to EULER_DISCRETE if not specified."""
     sd_version: Optional[shared_sd_versions.SdVersions] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sdVersion'), 'exclude': lambda f: f is None }})
-    r"""The base version of stable diffusion to use if not using a custom model. v1_5 is 1.5, v2 is 2.1, if not specified it will default to v1_5."""
+    r"""The base version of stable diffusion to use if not using a custom model. v1_5 is 1.5, v2 is 2.1, if not specified it will default to v1_5. Also includes SDXL and SDXL Lightning models"""
     seed: Optional[int] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('seed'), 'exclude': lambda f: f is GetGenerationsByUserIDGenerations.UNSET }})
     status: Optional[shared_job_status.JobStatus] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
     r"""The status of the current task."""
```

### Comparing `Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/getinitimagebyid.py` & `Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/getinitimagebyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/getmodelbyid.py` & `Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/getmodelbyid.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     id: Optional[str] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is GetModelByIDCustomModels.UNSET }})
     instance_prompt: Optional[str] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('instancePrompt'), 'exclude': lambda f: f is GetModelByIDCustomModels.UNSET }})
     model_height: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modelHeight'), 'exclude': lambda f: f is None }})
     model_width: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modelWidth'), 'exclude': lambda f: f is None }})
     name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
     public: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('public'), 'exclude': lambda f: f is None }})
     sd_version: Optional[shared_sd_versions.SdVersions] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sdVersion'), 'exclude': lambda f: f is None }})
-    r"""The base version of stable diffusion to use if not using a custom model. v1_5 is 1.5, v2 is 2.1, if not specified it will default to v1_5."""
+    r"""The base version of stable diffusion to use if not using a custom model. v1_5 is 1.5, v2 is 2.1, if not specified it will default to v1_5. Also includes SDXL and SDXL Lightning models"""
     status: Optional[shared_job_status.JobStatus] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
     r"""The status of the current task."""
     type: Optional[shared_custom_model_type.CustomModelType] = dataclasses.field(default=shared_custom_model_type.CustomModelType.GENERAL, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type'), 'exclude': lambda f: f is None }})
     r"""The category the most accurately reflects the model."""
     updated_at: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('updatedAt'), 'exclude': lambda f: f is None }})
```

### Comparing `Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/gettexturegenerationbyid.py` & `Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/gettexturegenerationbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/gettexturegenerationsbymodelid.py` & `Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/gettexturegenerationsbymodelid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/getuserself.py` & `Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/getuserself.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/getvariationbyid.py` & `Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/getvariationbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/listelements.py` & `Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/listelements.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 @dataclasses.dataclass
 class Loras:
     r"""columns and relationships of \\"elements\\" """
     UNSET='__SPEAKEASY_UNSET__'
     ak_uuid: Optional[str] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('akUUID'), 'exclude': lambda f: f is Loras.UNSET }})
     r"""Unique identifier for the element. Elements can be found from the List Elements endpoint."""
     base_model: Optional[shared_sd_versions.SdVersions] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('baseModel'), 'exclude': lambda f: f is None }})
-    r"""The base version of stable diffusion to use if not using a custom model. v1_5 is 1.5, v2 is 2.1, if not specified it will default to v1_5."""
+    r"""The base version of stable diffusion to use if not using a custom model. v1_5 is 1.5, v2 is 2.1, if not specified it will default to v1_5. Also includes SDXL and SDXL Lightning models"""
     creator_name: Optional[str] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('creatorName'), 'exclude': lambda f: f is Loras.UNSET }})
     r"""Name of the creator of the element"""
     description: Optional[str] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is Loras.UNSET }})
     r"""Description for the element"""
     name: Optional[str] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is Loras.UNSET }})
     r"""Name of the element"""
     url_image: Optional[str] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('urlImage'), 'exclude': lambda f: f is Loras.UNSET }})
```

### Comparing `Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/listplatformmodels.py` & `Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/listplatformmodels.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/performalchemyupscalelcm.py` & `Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/performalchemyupscalelcm.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/performinpaintinglcm.py` & `Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/performinpaintinglcm.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/performinstantrefine.py` & `Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/performinstantrefine.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/uploaddatasetimage.py` & `Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/uploaddatasetimage.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/uploaddatasetimagefromgen.py` & `Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/uploaddatasetimagefromgen.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/uploadinitimage.py` & `Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/uploadinitimage.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/operations/uploadmodelasset.py` & `Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/operations/uploadmodelasset.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/shared/__init__.py` & `Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/shared/custom_model_type.py` & `Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/shared/custom_model_type.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/shared/element_input.py` & `Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/shared/element_input.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/shared/lcm_generation_style.py` & `Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/shared/lcm_generation_style.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/models/shared/sd_generation_style.py` & `Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/models/shared/sd_generation_style.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/sdk.py` & `Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/sdk.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/sdkconfiguration.py` & `Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/sdkconfiguration.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 class SDKConfiguration:
     client: requests_http.Session
     security: Union[shared.Security,Callable[[], shared.Security]] = None
     server_url: Optional[str] = ''
     server_idx: Optional[int] = 0
     language: str = 'python'
     openapi_doc_version: str = 'v1.0.0'
-    sdk_version: str = '5.3.1'
-    gen_version: str = '2.298.0'
-    user_agent: str = 'speakeasy-sdk/python 5.3.1 2.298.0 v1.0.0 Leonardo-Ai-SDK'
+    sdk_version: str = '5.3.2'
+    gen_version: str = '2.298.2'
+    user_agent: str = 'speakeasy-sdk/python 5.3.2 2.298.2 v1.0.0 Leonardo-Ai-SDK'
     retry_config: Optional[RetryConfig] = None
     _hooks: Optional[SDKHooks] = None
 
     def get_server_details(self) -> Tuple[str, Dict[str, str]]:
         if self.server_url is not None and self.server_url != '':
             return utils.remove_suffix(self.server_url, '/'), {}
         if self.server_idx is None:
```

### Comparing `Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/user.py` & `Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/user.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/utils/retries.py` & `Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/utils/retries.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/utils/utils.py` & `Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/utils/utils.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.1/src/leonardoaisdk/variation.py` & `Leonardo-Ai-SDK-5.3.2/src/leonardoaisdk/variation.py`

 * *Files identical despite different names*

