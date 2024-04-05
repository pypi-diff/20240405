# Comparing `tmp/autohelper-0.0.5.tar.gz` & `tmp/autohelper-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autohelper-0.0.5.tar", last modified: Tue Mar 19 01:45:49 2024, max compression
+gzip compressed data, was "autohelper-0.0.6.tar", last modified: Fri Apr  5 12:04:46 2024, max compression
```

## Comparing `autohelper-0.0.5.tar` & `autohelper-0.0.6.tar`

### file list

```diff
@@ -1,138 +1,170 @@
-drwxrwxrwx   0        0        0        0 2024-03-19 01:45:49.230324 autohelper-0.0.5/
--rw-rw-rw-   0        0        0     1998 2024-03-19 01:45:49.230324 autohelper-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1513 2024-02-09 15:31:41.000000 autohelper-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-03-19 01:45:49.141937 autohelper-0.0.5/autohelper/
--rw-rw-rw-   0        0        0     4774 2024-03-17 10:06:37.000000 autohelper-0.0.5/autohelper/AutoHelper.py
--rw-rw-rw-   0        0        0        0 2023-12-13 14:30:39.000000 autohelper-0.0.5/autohelper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 01:45:49.148101 autohelper-0.0.5/autohelper/capture/
--rw-rw-rw-   0        0        0      636 2024-03-16 12:36:30.000000 autohelper-0.0.5/autohelper/capture/BaseCaptureMethod.py
--rw-rw-rw-   0        0        0     4306 2024-03-18 15:03:53.000000 autohelper-0.0.5/autohelper/capture/HwndWindow.py
--rw-rw-rw-   0        0        0        0 2024-01-26 14:29:44.000000 autohelper-0.0.5/autohelper/capture/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 01:45:49.152734 autohelper-0.0.5/autohelper/capture/adb/
--rw-rw-rw-   0        0        0      999 2024-03-16 12:49:29.000000 autohelper-0.0.5/autohelper/capture/adb/ADBCaptureMethod.py
--rw-rw-rw-   0        0        0     1729 2024-03-16 12:36:40.000000 autohelper-0.0.5/autohelper/capture/adb/DeviceManager.py
--rw-rw-rw-   0        0        0        0 2024-02-04 14:45:00.000000 autohelper-0.0.5/autohelper/capture/adb/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 01:45:49.153759 autohelper-0.0.5/autohelper/capture/adb/bin/
--rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 autohelper-0.0.5/autohelper/capture/adb/bin/__init__.py
--rw-rw-rw-   0        0        0     2355 2024-03-14 10:16:17.000000 autohelper-0.0.5/autohelper/capture/adb/targets.py
--rw-rw-rw-   0        0        0     5824 2024-03-16 09:25:50.000000 autohelper-0.0.5/autohelper/capture/adb/vbox.py
-drwxrwxrwx   0        0        0        0 2024-03-19 01:45:49.158387 autohelper-0.0.5/autohelper/capture/windows/
--rw-rw-rw-   0        0        0     9051 2024-03-15 17:26:56.000000 autohelper-0.0.5/autohelper/capture/windows/WindowsGraphicsCaptureMethod.py
--rw-rw-rw-   0        0        0        0 2024-02-03 03:10:06.000000 autohelper-0.0.5/autohelper/capture/windows/__init__.py
--rw-rw-rw-   0        0        0     2689 2024-03-12 10:11:44.000000 autohelper-0.0.5/autohelper/capture/windows/d3d11.py
--rw-rw-rw-   0        0        0     4639 2024-03-16 14:22:58.000000 autohelper-0.0.5/autohelper/capture/windows/utils.py
--rw-rw-rw-   0        0        0     1826 2024-03-16 14:37:02.000000 autohelper-0.0.5/autohelper/capture/windows/window.py
-drwxrwxrwx   0        0        0        0 2024-03-19 01:45:49.159938 autohelper-0.0.5/autohelper/color/
--rw-rw-rw-   0        0        0     1550 2024-03-18 15:46:15.000000 autohelper-0.0.5/autohelper/color/Color.py
--rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 autohelper-0.0.5/autohelper/color/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 01:45:49.165095 autohelper-0.0.5/autohelper/feature/
--rw-rw-rw-   0        0        0     7164 2024-03-18 15:35:54.000000 autohelper-0.0.5/autohelper/feature/Box.py
--rw-rw-rw-   0        0        0      739 2024-03-16 12:36:18.000000 autohelper-0.0.5/autohelper/feature/Feature.py
--rw-rw-rw-   0        0        0     9049 2024-03-18 09:58:58.000000 autohelper-0.0.5/autohelper/feature/FeatureSet.py
--rw-rw-rw-   0        0        0     2112 2024-03-18 00:55:14.000000 autohelper-0.0.5/autohelper/feature/FindFeature.py
--rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 autohelper-0.0.5/autohelper/feature/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 01:45:49.170240 autohelper-0.0.5/autohelper/gui/
--rw-rw-rw-   0        0        0     2901 2024-03-17 08:42:26.000000 autohelper-0.0.5/autohelper/gui/App.py
--rw-rw-rw-   0        0        0      431 2024-03-18 09:57:16.000000 autohelper-0.0.5/autohelper/gui/Communicate.py
--rw-rw-rw-   0        0        0     2502 2024-03-16 09:31:51.000000 autohelper-0.0.5/autohelper/gui/MainWindow.py
--rw-rw-rw-   0        0        0     1849 2024-03-07 15:43:39.000000 autohelper-0.0.5/autohelper/gui/TabTitles.py
--rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 autohelper-0.0.5/autohelper/gui/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 01:45:49.175886 autohelper-0.0.5/autohelper/gui/debug/
--rw-rw-rw-   0        0        0     1213 2024-03-08 05:29:34.000000 autohelper-0.0.5/autohelper/gui/debug/AspectRatioWidget.py
--rw-rw-rw-   0        0        0     1358 2024-03-16 10:12:34.000000 autohelper-0.0.5/autohelper/gui/debug/DebugTab.py
--rw-rw-rw-   0        0        0     5111 2024-03-18 10:58:13.000000 autohelper-0.0.5/autohelper/gui/debug/FrameWidget.py
--rw-rw-rw-   0        0        0     1219 2024-03-12 10:11:44.000000 autohelper-0.0.5/autohelper/gui/debug/InfoWidget.py
--rw-rw-rw-   0        0        0     2698 2024-03-12 10:11:44.000000 autohelper-0.0.5/autohelper/gui/debug/LoggerWidget.py
--rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 autohelper-0.0.5/autohelper/gui/debug/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 01:45:49.177380 autohelper-0.0.5/autohelper/gui/loading/
--rw-rw-rw-   0        0        0      851 2024-03-17 08:31:48.000000 autohelper-0.0.5/autohelper/gui/loading/LoadingWindow.py
--rw-rw-rw-   0        0        0        0 2024-03-17 08:31:48.000000 autohelper-0.0.5/autohelper/gui/loading/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 01:45:49.179348 autohelper-0.0.5/autohelper/gui/overlay/
--rw-rw-rw-   0        0        0     1409 2024-03-16 14:14:14.000000 autohelper-0.0.5/autohelper/gui/overlay/OverlayWindow.py
--rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 autohelper-0.0.5/autohelper/gui/overlay/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 01:45:49.180855 autohelper-0.0.5/autohelper/gui/tasks/
--rw-rw-rw-   0        0        0     2744 2024-03-12 10:12:49.000000 autohelper-0.0.5/autohelper/gui/tasks/TaskTab.py
--rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 autohelper-0.0.5/autohelper/gui/tasks/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 01:45:49.185373 autohelper-0.0.5/autohelper/interaction/
--rw-rw-rw-   0        0        0     1169 2024-03-14 10:16:17.000000 autohelper-0.0.5/autohelper/interaction/ADBInteraction.py
--rw-rw-rw-   0        0        0     1016 2024-03-18 12:48:19.000000 autohelper-0.0.5/autohelper/interaction/BaseInteraction.py
--rw-rw-rw-   0        0        0     1643 2024-03-16 14:47:32.000000 autohelper-0.0.5/autohelper/interaction/Win32Interaction.py
--rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 autohelper-0.0.5/autohelper/interaction/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 01:45:49.187395 autohelper-0.0.5/autohelper/logging/
--rw-rw-rw-   0        0        0     3884 2024-03-17 14:34:48.000000 autohelper-0.0.5/autohelper/logging/Logger.py
--rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 autohelper-0.0.5/autohelper/logging/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 01:45:49.188942 autohelper-0.0.5/autohelper/ocr/
--rw-rw-rw-   0        0        0     2149 2024-03-18 10:57:13.000000 autohelper-0.0.5/autohelper/ocr/OCR.py
--rw-rw-rw-   0        0        0        0 2024-03-17 08:31:48.000000 autohelper-0.0.5/autohelper/ocr/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 01:45:49.191009 autohelper-0.0.5/autohelper/predict/
--rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 autohelper-0.0.5/autohelper/predict/__init__.py
--rw-rw-rw-   0        0        0     1595 2023-12-15 17:49:57.000000 autohelper-0.0.5/autohelper/predict/predict.py
-drwxrwxrwx   0        0        0        0 2024-03-19 01:45:49.198722 autohelper-0.0.5/autohelper/rotypes/
-drwxrwxrwx   0        0        0        0 2024-03-19 01:45:49.199751 autohelper-0.0.5/autohelper/rotypes/Windows/
-drwxrwxrwx   0        0        0        0 2024-03-19 01:45:49.201257 autohelper-0.0.5/autohelper/rotypes/Windows/Foundation/
--rw-rw-rw-   0        0        0     2039 2024-03-12 10:11:44.000000 autohelper-0.0.5/autohelper/rotypes/Windows/Foundation/Collections.py
--rw-rw-rw-   0        0        0     5409 2024-03-12 10:11:44.000000 autohelper-0.0.5/autohelper/rotypes/Windows/Foundation/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 01:45:49.202253 autohelper-0.0.5/autohelper/rotypes/Windows/Globalization/
--rw-rw-rw-   0        0        0      933 2024-03-12 10:11:44.000000 autohelper-0.0.5/autohelper/rotypes/Windows/Globalization/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 01:45:49.203564 autohelper-0.0.5/autohelper/rotypes/Windows/Graphics/
-drwxrwxrwx   0        0        0        0 2024-03-19 01:45:49.203564 autohelper-0.0.5/autohelper/rotypes/Windows/Graphics/Capture/
--rw-rw-rw-   0        0        0     4731 2024-03-12 10:11:44.000000 autohelper-0.0.5/autohelper/rotypes/Windows/Graphics/Capture/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 01:45:49.205066 autohelper-0.0.5/autohelper/rotypes/Windows/Graphics/DirectX/
-drwxrwxrwx   0        0        0        0 2024-03-19 01:45:49.206079 autohelper-0.0.5/autohelper/rotypes/Windows/Graphics/DirectX/Direct3D11/
--rw-rw-rw-   0        0        0     1266 2024-03-12 10:11:44.000000 autohelper-0.0.5/autohelper/rotypes/Windows/Graphics/DirectX/Direct3D11/__init__.py
--rw-rw-rw-   0        0        0     4189 2024-03-12 10:11:44.000000 autohelper-0.0.5/autohelper/rotypes/Windows/Graphics/DirectX/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 01:45:49.207087 autohelper-0.0.5/autohelper/rotypes/Windows/Graphics/Imaging/
--rw-rw-rw-   0        0        0     1093 2024-03-12 10:11:44.000000 autohelper-0.0.5/autohelper/rotypes/Windows/Graphics/Imaging/__init__.py
--rw-rw-rw-   0        0        0      127 2024-01-26 14:10:34.000000 autohelper-0.0.5/autohelper/rotypes/Windows/Graphics/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 01:45:49.208083 autohelper-0.0.5/autohelper/rotypes/Windows/Media/
-drwxrwxrwx   0        0        0        0 2024-03-19 01:45:49.209071 autohelper-0.0.5/autohelper/rotypes/Windows/Media/Ocr/
--rw-rw-rw-   0        0        0     3095 2024-03-12 10:11:44.000000 autohelper-0.0.5/autohelper/rotypes/Windows/Media/Ocr/__init__.py
--rw-rw-rw-   0        0        0        0 2024-01-26 14:10:34.000000 autohelper-0.0.5/autohelper/rotypes/Windows/Media/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 01:45:49.210059 autohelper-0.0.5/autohelper/rotypes/Windows/Security/
-drwxrwxrwx   0        0        0        0 2024-03-19 01:45:49.211053 autohelper-0.0.5/autohelper/rotypes/Windows/Security/Cryptography/
--rw-rw-rw-   0        0        0      691 2024-03-12 10:11:44.000000 autohelper-0.0.5/autohelper/rotypes/Windows/Security/Cryptography/__init__.py
--rw-rw-rw-   0        0        0        0 2024-01-26 14:10:34.000000 autohelper-0.0.5/autohelper/rotypes/Windows/Security/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 01:45:49.212333 autohelper-0.0.5/autohelper/rotypes/Windows/Storage/
-drwxrwxrwx   0        0        0        0 2024-03-19 01:45:49.213322 autohelper-0.0.5/autohelper/rotypes/Windows/Storage/Streams/
--rw-rw-rw-   0        0        0      853 2024-03-12 10:11:44.000000 autohelper-0.0.5/autohelper/rotypes/Windows/Storage/Streams/__init__.py
--rw-rw-rw-   0        0        0        0 2024-01-26 14:10:34.000000 autohelper-0.0.5/autohelper/rotypes/Windows/Storage/__init__.py
--rw-rw-rw-   0        0        0        0 2024-01-26 14:10:34.000000 autohelper-0.0.5/autohelper/rotypes/Windows/__init__.py
--rw-rw-rw-   0        0        0      145 2024-01-26 14:10:34.000000 autohelper-0.0.5/autohelper/rotypes/__init__.py
--rw-rw-rw-   0        0        0     3532 2024-01-26 14:10:34.000000 autohelper-0.0.5/autohelper/rotypes/delegate.py
--rw-rw-rw-   0        0        0      575 2024-01-26 14:10:34.000000 autohelper-0.0.5/autohelper/rotypes/export.py
--rw-rw-rw-   0        0        0     9281 2024-01-26 14:10:34.000000 autohelper-0.0.5/autohelper/rotypes/idldsl.py
--rw-rw-rw-   0        0        0     2311 2024-01-26 14:10:34.000000 autohelper-0.0.5/autohelper/rotypes/inspectable.py
--rw-rw-rw-   0        0        0      840 2024-03-14 16:08:07.000000 autohelper-0.0.5/autohelper/rotypes/roapi.py
--rw-rw-rw-   0        0        0     2560 2024-01-26 14:10:34.000000 autohelper-0.0.5/autohelper/rotypes/types.py
--rw-rw-rw-   0        0        0     1566 2024-01-26 14:10:34.000000 autohelper-0.0.5/autohelper/rotypes/winstring.py
-drwxrwxrwx   0        0        0        0 2024-03-19 01:45:49.218723 autohelper-0.0.5/autohelper/save/
--rw-rw-rw-   0        0        0      804 2024-03-16 12:48:02.000000 autohelper-0.0.5/autohelper/save/BlackBarProcessor.py
--rw-rw-rw-   0        0        0       97 2024-03-16 12:49:02.000000 autohelper-0.0.5/autohelper/save/PostProcessor.py
--rw-rw-rw-   0        0        0      836 2024-03-12 10:11:44.000000 autohelper-0.0.5/autohelper/save/SaveByInterval.py
--rw-rw-rw-   0        0        0     1043 2024-03-12 10:11:44.000000 autohelper-0.0.5/autohelper/save/SaveByKeyPress.py
--rw-rw-rw-   0        0        0     1471 2024-03-12 10:11:44.000000 autohelper-0.0.5/autohelper/save/SaveMethodBase.py
--rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 autohelper-0.0.5/autohelper/save/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 01:45:49.220720 autohelper-0.0.5/autohelper/scene/
--rw-rw-rw-   0        0        0      344 2024-03-18 15:05:37.000000 autohelper-0.0.5/autohelper/scene/FeatureScene.py
--rw-rw-rw-   0        0        0      397 2024-03-18 15:06:49.000000 autohelper-0.0.5/autohelper/scene/Scene.py
--rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 autohelper-0.0.5/autohelper/scene/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 01:45:49.223106 autohelper-0.0.5/autohelper/stats/
--rw-rw-rw-   0        0        0     1014 2024-02-26 12:12:14.000000 autohelper-0.0.5/autohelper/stats/StreamStats.py
--rw-rw-rw-   0        0        0        0 2024-02-06 15:39:35.000000 autohelper-0.0.5/autohelper/stats/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 01:45:49.226079 autohelper-0.0.5/autohelper/task/
--rw-rw-rw-   0        0        0     5338 2024-03-18 09:59:37.000000 autohelper-0.0.5/autohelper/task/BaseTask.py
--rw-rw-rw-   0        0        0      164 2024-03-12 10:11:44.000000 autohelper-0.0.5/autohelper/task/FindFeatureTask.py
--rw-rw-rw-   0        0        0     7982 2024-03-18 10:14:01.000000 autohelper-0.0.5/autohelper/task/TaskExecutor.py
--rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 autohelper-0.0.5/autohelper/task/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 01:45:49.229333 autohelper-0.0.5/autohelper/util/
--rw-rw-rw-   0        0        0        0 2023-12-13 14:30:39.000000 autohelper-0.0.5/autohelper/util/__init__.py
--rw-rw-rw-   0        0        0      177 2024-03-13 17:50:38.000000 autohelper-0.0.5/autohelper/util/path.py
--rw-rw-rw-   0        0        0     2923 2024-03-14 10:21:07.000000 autohelper-0.0.5/autohelper/util/win32_process.py
-drwxrwxrwx   0        0        0        0 2024-03-19 01:45:49.145545 autohelper-0.0.5/autohelper.egg-info/
--rw-rw-rw-   0        0        0     1998 2024-03-19 01:45:49.000000 autohelper-0.0.5/autohelper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3457 2024-03-19 01:45:49.000000 autohelper-0.0.5/autohelper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-19 01:45:49.000000 autohelper-0.0.5/autohelper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      144 2024-03-19 01:45:49.000000 autohelper-0.0.5/autohelper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-03-19 01:45:49.000000 autohelper-0.0.5/autohelper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-19 01:45:49.230324 autohelper-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1003 2024-03-19 01:43:38.000000 autohelper-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:04:46.129094 autohelper-0.0.6/
+-rw-rw-rw-   0        0        0     2270 2024-04-05 12:04:46.128120 autohelper-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1513 2024-02-09 15:31:41.000000 autohelper-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-05 12:04:46.022735 autohelper-0.0.6/autohelper/
+-rw-rw-rw-   0        0        0     4554 2024-04-05 03:49:20.000000 autohelper-0.0.6/autohelper/AutoHelper.py
+-rw-rw-rw-   0        0        0        0 2023-12-13 14:30:39.000000 autohelper-0.0.6/autohelper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:04:46.032193 autohelper-0.0.6/autohelper/capture/
+-rw-rw-rw-   0        0        0      602 2024-04-05 09:34:11.000000 autohelper-0.0.6/autohelper/capture/BaseCaptureMethod.py
+-rw-rw-rw-   0        0        0     5371 2024-04-05 09:41:17.000000 autohelper-0.0.6/autohelper/capture/HwndWindow.py
+-rw-rw-rw-   0        0        0        0 2024-01-26 14:29:44.000000 autohelper-0.0.6/autohelper/capture/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:04:46.037096 autohelper-0.0.6/autohelper/capture/adb/
+-rw-rw-rw-   0        0        0      924 2024-04-05 03:42:41.000000 autohelper-0.0.6/autohelper/capture/adb/ADBCaptureMethod.py
+-rw-rw-rw-   0        0        0     8482 2024-04-05 09:38:11.000000 autohelper-0.0.6/autohelper/capture/adb/DeviceManager.py
+-rw-rw-rw-   0        0        0        0 2024-02-04 14:45:00.000000 autohelper-0.0.6/autohelper/capture/adb/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:04:46.037096 autohelper-0.0.6/autohelper/capture/adb/bin/
+-rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 autohelper-0.0.6/autohelper/capture/adb/bin/__init__.py
+-rw-rw-rw-   0        0        0     2355 2024-03-14 10:16:17.000000 autohelper-0.0.6/autohelper/capture/adb/targets.py
+-rw-rw-rw-   0        0        0     5808 2024-04-02 12:02:15.000000 autohelper-0.0.6/autohelper/capture/adb/vbox.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:04:46.041486 autohelper-0.0.6/autohelper/capture/windows/
+-rw-rw-rw-   0        0        0     9246 2024-04-03 01:37:12.000000 autohelper-0.0.6/autohelper/capture/windows/WindowsGraphicsCaptureMethod.py
+-rw-rw-rw-   0        0        0        0 2024-02-03 03:10:06.000000 autohelper-0.0.6/autohelper/capture/windows/__init__.py
+-rw-rw-rw-   0        0        0     2689 2024-03-12 10:11:44.000000 autohelper-0.0.6/autohelper/capture/windows/d3d11.py
+-rw-rw-rw-   0        0        0     4639 2024-03-16 14:22:58.000000 autohelper-0.0.6/autohelper/capture/windows/utils.py
+-rw-rw-rw-   0        0        0     1320 2024-04-01 01:55:20.000000 autohelper-0.0.6/autohelper/capture/windows/window.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:04:46.043434 autohelper-0.0.6/autohelper/color/
+-rw-rw-rw-   0        0        0     1550 2024-03-18 15:46:15.000000 autohelper-0.0.6/autohelper/color/Color.py
+-rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 autohelper-0.0.6/autohelper/color/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:04:46.045910 autohelper-0.0.6/autohelper/config/
+-rw-rw-rw-   0        0        0     2211 2024-04-02 04:15:06.000000 autohelper-0.0.6/autohelper/config/Config.py
+-rw-rw-rw-   0        0        0      394 2024-04-03 09:47:40.000000 autohelper-0.0.6/autohelper/config/InfoDict.py
+-rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 autohelper-0.0.6/autohelper/config/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:04:46.051007 autohelper-0.0.6/autohelper/feature/
+-rw-rw-rw-   0        0        0     7181 2024-03-24 13:07:51.000000 autohelper-0.0.6/autohelper/feature/Box.py
+-rw-rw-rw-   0        0        0      739 2024-03-16 12:36:18.000000 autohelper-0.0.6/autohelper/feature/Feature.py
+-rw-rw-rw-   0        0        0     9084 2024-04-02 17:38:24.000000 autohelper-0.0.6/autohelper/feature/FeatureSet.py
+-rw-rw-rw-   0        0        0     2112 2024-03-18 00:55:14.000000 autohelper-0.0.6/autohelper/feature/FindFeature.py
+-rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 autohelper-0.0.6/autohelper/feature/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:04:46.054895 autohelper-0.0.6/autohelper/gui/
+-rw-rw-rw-   0        0        0     4581 2024-04-04 16:24:15.000000 autohelper-0.0.6/autohelper/gui/App.py
+-rw-rw-rw-   0        0        0      604 2024-04-03 09:22:41.000000 autohelper-0.0.6/autohelper/gui/Communicate.py
+-rw-rw-rw-   0        0        0     2565 2024-04-03 02:56:02.000000 autohelper-0.0.6/autohelper/gui/MainWindow.py
+-rw-rw-rw-   0        0        0     1849 2024-03-07 15:43:39.000000 autohelper-0.0.6/autohelper/gui/TabTitles.py
+-rw-rw-rw-   0        0        0      140 2024-04-02 11:24:03.000000 autohelper-0.0.6/autohelper/gui/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:04:46.060050 autohelper-0.0.6/autohelper/gui/debug/
+-rw-rw-rw-   0        0        0     1213 2024-03-08 05:29:34.000000 autohelper-0.0.6/autohelper/gui/debug/AspectRatioWidget.py
+-rw-rw-rw-   0        0        0     1358 2024-03-16 10:12:34.000000 autohelper-0.0.6/autohelper/gui/debug/DebugTab.py
+-rw-rw-rw-   0        0        0     5111 2024-03-18 10:58:13.000000 autohelper-0.0.6/autohelper/gui/debug/FrameWidget.py
+-rw-rw-rw-   0        0        0     1219 2024-03-12 10:11:44.000000 autohelper-0.0.6/autohelper/gui/debug/InfoWidget.py
+-rw-rw-rw-   0        0        0     2698 2024-03-12 10:11:44.000000 autohelper-0.0.6/autohelper/gui/debug/LoggerWidget.py
+-rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 autohelper-0.0.6/autohelper/gui/debug/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:04:46.061996 autohelper-0.0.6/autohelper/gui/i18n/
+-rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 autohelper-0.0.6/autohelper/gui/i18n/__init__.py
+-rw-rw-rw-   0        0        0       52 2024-04-01 11:14:15.000000 autohelper-0.0.6/autohelper/gui/i18n/path.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:04:46.062969 autohelper-0.0.6/autohelper/gui/icon/
+-rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 autohelper-0.0.6/autohelper/gui/icon/__init__.py
+-rw-rw-rw-   0        0        0      174 2024-03-26 17:34:24.000000 autohelper-0.0.6/autohelper/gui/icon/icon.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:04:46.065890 autohelper-0.0.6/autohelper/gui/loading/
+-rw-rw-rw-   0        0        0     6236 2024-04-05 09:39:36.000000 autohelper-0.0.6/autohelper/gui/loading/LoadingWindow.py
+-rw-rw-rw-   0        0        0        0 2024-03-17 08:31:48.000000 autohelper-0.0.6/autohelper/gui/loading/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:04:46.066894 autohelper-0.0.6/autohelper/gui/overlay/
+-rw-rw-rw-   0        0        0     1434 2024-03-23 15:09:36.000000 autohelper-0.0.6/autohelper/gui/overlay/OverlayWindow.py
+-rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 autohelper-0.0.6/autohelper/gui/overlay/__init__.py
+-rw-rw-rw-   0        0        0    22185 2024-04-04 16:18:48.000000 autohelper-0.0.6/autohelper/gui/resources.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:04:46.071967 autohelper-0.0.6/autohelper/gui/tasks/
+-rw-rw-rw-   0        0        0      692 2024-03-25 16:13:40.000000 autohelper-0.0.6/autohelper/gui/tasks/ConfigItemFactory.py
+-rw-rw-rw-   0        0        0     1615 2024-04-03 02:52:44.000000 autohelper-0.0.6/autohelper/gui/tasks/StartButton.py
+-rw-rw-rw-   0        0        0      919 2024-04-03 04:00:06.000000 autohelper-0.0.6/autohelper/gui/tasks/TaskOpButton.py
+-rw-rw-rw-   0        0        0     6041 2024-04-03 15:23:26.000000 autohelper-0.0.6/autohelper/gui/tasks/TaskTab.py
+-rw-rw-rw-   0        0        0     1546 2024-04-03 14:53:01.000000 autohelper-0.0.6/autohelper/gui/tasks/TooltipTableWidget.py
+-rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 autohelper-0.0.6/autohelper/gui/tasks/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:04:46.074892 autohelper-0.0.6/autohelper/gui/util/
+-rw-rw-rw-   0        0        0      416 2024-03-30 15:38:52.000000 autohelper-0.0.6/autohelper/gui/util/Alert.py
+-rw-rw-rw-   0        0        0      372 2024-04-02 10:49:06.000000 autohelper-0.0.6/autohelper/gui/util/InitWorker.py
+-rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 autohelper-0.0.6/autohelper/gui/util/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:04:46.081663 autohelper-0.0.6/autohelper/gui/widget/
+-rw-rw-rw-   0        0        0      951 2024-03-25 16:12:19.000000 autohelper-0.0.6/autohelper/gui/widget/ListTableWidgetItem.py
+-rw-rw-rw-   0        0        0     1324 2024-03-26 06:35:12.000000 autohelper-0.0.6/autohelper/gui/widget/NumericTableWidgetItem.py
+-rw-rw-rw-   0        0        0     2126 2024-04-02 12:32:43.000000 autohelper-0.0.6/autohelper/gui/widget/RoundCornerContainer.py
+-rw-rw-rw-   0        0        0      830 2024-03-25 08:54:00.000000 autohelper-0.0.6/autohelper/gui/widget/TabWidget.py
+-rw-rw-rw-   0        0        0      399 2024-03-25 14:18:22.000000 autohelper-0.0.6/autohelper/gui/widget/UpdateConfigWidgetItem.py
+-rw-rw-rw-   0        0        0      693 2024-03-25 14:39:29.000000 autohelper-0.0.6/autohelper/gui/widget/YesNonWidgetItem.py
+-rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 autohelper-0.0.6/autohelper/gui/widget/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:04:46.084601 autohelper-0.0.6/autohelper/interaction/
+-rw-rw-rw-   0        0        0     1169 2024-04-02 04:25:35.000000 autohelper-0.0.6/autohelper/interaction/ADBInteraction.py
+-rw-rw-rw-   0        0        0     1074 2024-04-02 17:41:04.000000 autohelper-0.0.6/autohelper/interaction/BaseInteraction.py
+-rw-rw-rw-   0        0        0     1717 2024-04-03 01:37:12.000000 autohelper-0.0.6/autohelper/interaction/Win32Interaction.py
+-rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 autohelper-0.0.6/autohelper/interaction/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:04:46.085574 autohelper-0.0.6/autohelper/logging/
+-rw-rw-rw-   0        0        0     3642 2024-04-02 02:22:11.000000 autohelper-0.0.6/autohelper/logging/Logger.py
+-rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 autohelper-0.0.6/autohelper/logging/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:04:46.088074 autohelper-0.0.6/autohelper/ocr/
+-rw-rw-rw-   0        0        0     2123 2024-04-03 02:48:38.000000 autohelper-0.0.6/autohelper/ocr/OCR.py
+-rw-rw-rw-   0        0        0        0 2024-03-17 08:31:48.000000 autohelper-0.0.6/autohelper/ocr/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:04:46.089047 autohelper-0.0.6/autohelper/predict/
+-rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 autohelper-0.0.6/autohelper/predict/__init__.py
+-rw-rw-rw-   0        0        0     1595 2023-12-15 17:49:57.000000 autohelper-0.0.6/autohelper/predict/predict.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:04:46.095860 autohelper-0.0.6/autohelper/rotypes/
+drwxrwxrwx   0        0        0        0 2024-04-05 12:04:46.096863 autohelper-0.0.6/autohelper/rotypes/Windows/
+drwxrwxrwx   0        0        0        0 2024-04-05 12:04:46.098899 autohelper-0.0.6/autohelper/rotypes/Windows/Foundation/
+-rw-rw-rw-   0        0        0     2039 2024-03-12 10:11:44.000000 autohelper-0.0.6/autohelper/rotypes/Windows/Foundation/Collections.py
+-rw-rw-rw-   0        0        0     5409 2024-03-12 10:11:44.000000 autohelper-0.0.6/autohelper/rotypes/Windows/Foundation/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:04:46.099875 autohelper-0.0.6/autohelper/rotypes/Windows/Globalization/
+-rw-rw-rw-   0        0        0      933 2024-03-12 10:11:44.000000 autohelper-0.0.6/autohelper/rotypes/Windows/Globalization/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:04:46.100848 autohelper-0.0.6/autohelper/rotypes/Windows/Graphics/
+drwxrwxrwx   0        0        0        0 2024-04-05 12:04:46.101826 autohelper-0.0.6/autohelper/rotypes/Windows/Graphics/Capture/
+-rw-rw-rw-   0        0        0     4731 2024-03-12 10:11:44.000000 autohelper-0.0.6/autohelper/rotypes/Windows/Graphics/Capture/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:04:46.101826 autohelper-0.0.6/autohelper/rotypes/Windows/Graphics/DirectX/
+drwxrwxrwx   0        0        0        0 2024-04-05 12:04:46.102795 autohelper-0.0.6/autohelper/rotypes/Windows/Graphics/DirectX/Direct3D11/
+-rw-rw-rw-   0        0        0     1266 2024-03-12 10:11:44.000000 autohelper-0.0.6/autohelper/rotypes/Windows/Graphics/DirectX/Direct3D11/__init__.py
+-rw-rw-rw-   0        0        0     4189 2024-03-12 10:11:44.000000 autohelper-0.0.6/autohelper/rotypes/Windows/Graphics/DirectX/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:04:46.103768 autohelper-0.0.6/autohelper/rotypes/Windows/Graphics/Imaging/
+-rw-rw-rw-   0        0        0     1093 2024-03-12 10:11:44.000000 autohelper-0.0.6/autohelper/rotypes/Windows/Graphics/Imaging/__init__.py
+-rw-rw-rw-   0        0        0      127 2024-01-26 14:10:34.000000 autohelper-0.0.6/autohelper/rotypes/Windows/Graphics/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:04:46.104741 autohelper-0.0.6/autohelper/rotypes/Windows/Media/
+drwxrwxrwx   0        0        0        0 2024-04-05 12:04:46.104741 autohelper-0.0.6/autohelper/rotypes/Windows/Media/Ocr/
+-rw-rw-rw-   0        0        0     3095 2024-03-12 10:11:44.000000 autohelper-0.0.6/autohelper/rotypes/Windows/Media/Ocr/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-01-26 14:10:34.000000 autohelper-0.0.6/autohelper/rotypes/Windows/Media/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:04:46.105714 autohelper-0.0.6/autohelper/rotypes/Windows/Security/
+drwxrwxrwx   0        0        0        0 2024-04-05 12:04:46.105714 autohelper-0.0.6/autohelper/rotypes/Windows/Security/Cryptography/
+-rw-rw-rw-   0        0        0      691 2024-03-12 10:11:44.000000 autohelper-0.0.6/autohelper/rotypes/Windows/Security/Cryptography/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-01-26 14:10:34.000000 autohelper-0.0.6/autohelper/rotypes/Windows/Security/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:04:46.107217 autohelper-0.0.6/autohelper/rotypes/Windows/Storage/
+drwxrwxrwx   0        0        0        0 2024-04-05 12:04:46.107217 autohelper-0.0.6/autohelper/rotypes/Windows/Storage/Streams/
+-rw-rw-rw-   0        0        0      853 2024-03-12 10:11:44.000000 autohelper-0.0.6/autohelper/rotypes/Windows/Storage/Streams/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-01-26 14:10:34.000000 autohelper-0.0.6/autohelper/rotypes/Windows/Storage/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-01-26 14:10:34.000000 autohelper-0.0.6/autohelper/rotypes/Windows/__init__.py
+-rw-rw-rw-   0        0        0      145 2024-01-26 14:10:34.000000 autohelper-0.0.6/autohelper/rotypes/__init__.py
+-rw-rw-rw-   0        0        0     3532 2024-01-26 14:10:34.000000 autohelper-0.0.6/autohelper/rotypes/delegate.py
+-rw-rw-rw-   0        0        0      575 2024-01-26 14:10:34.000000 autohelper-0.0.6/autohelper/rotypes/export.py
+-rw-rw-rw-   0        0        0     9281 2024-01-26 14:10:34.000000 autohelper-0.0.6/autohelper/rotypes/idldsl.py
+-rw-rw-rw-   0        0        0     2311 2024-01-26 14:10:34.000000 autohelper-0.0.6/autohelper/rotypes/inspectable.py
+-rw-rw-rw-   0        0        0      840 2024-03-14 16:08:07.000000 autohelper-0.0.6/autohelper/rotypes/roapi.py
+-rw-rw-rw-   0        0        0     2560 2024-01-26 14:10:34.000000 autohelper-0.0.6/autohelper/rotypes/types.py
+-rw-rw-rw-   0        0        0     1566 2024-01-26 14:10:34.000000 autohelper-0.0.6/autohelper/rotypes/winstring.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:04:46.113444 autohelper-0.0.6/autohelper/save/
+-rw-rw-rw-   0        0        0      804 2024-03-16 12:48:02.000000 autohelper-0.0.6/autohelper/save/BlackBarProcessor.py
+-rw-rw-rw-   0        0        0       97 2024-03-16 12:49:02.000000 autohelper-0.0.6/autohelper/save/PostProcessor.py
+-rw-rw-rw-   0        0        0      836 2024-03-12 10:11:44.000000 autohelper-0.0.6/autohelper/save/SaveByInterval.py
+-rw-rw-rw-   0        0        0     1043 2024-03-12 10:11:44.000000 autohelper-0.0.6/autohelper/save/SaveByKeyPress.py
+-rw-rw-rw-   0        0        0     1471 2024-03-12 10:11:44.000000 autohelper-0.0.6/autohelper/save/SaveMethodBase.py
+-rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 autohelper-0.0.6/autohelper/save/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:04:46.115390 autohelper-0.0.6/autohelper/scene/
+-rw-rw-rw-   0        0        0      344 2024-03-18 15:05:37.000000 autohelper-0.0.6/autohelper/scene/FeatureScene.py
+-rw-rw-rw-   0        0        0      600 2024-04-02 18:02:38.000000 autohelper-0.0.6/autohelper/scene/Scene.py
+-rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 autohelper-0.0.6/autohelper/scene/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:04:46.117889 autohelper-0.0.6/autohelper/stats/
+-rw-rw-rw-   0        0        0     1014 2024-02-26 12:12:14.000000 autohelper-0.0.6/autohelper/stats/StreamStats.py
+-rw-rw-rw-   0        0        0        0 2024-02-06 15:39:35.000000 autohelper-0.0.6/autohelper/stats/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:04:46.121358 autohelper-0.0.6/autohelper/task/
+-rw-rw-rw-   0        0        0     3136 2024-04-03 13:39:04.000000 autohelper-0.0.6/autohelper/task/BaseTask.py
+-rw-rw-rw-   0        0        0     4812 2024-04-02 18:06:06.000000 autohelper-0.0.6/autohelper/task/ExecutorOperation.py
+-rw-rw-rw-   0        0        0      164 2024-03-12 10:11:44.000000 autohelper-0.0.6/autohelper/task/FindFeatureTask.py
+-rw-rw-rw-   0        0        0     9557 2024-04-03 09:25:57.000000 autohelper-0.0.6/autohelper/task/TaskExecutor.py
+-rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 autohelper-0.0.6/autohelper/task/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:04:46.127124 autohelper-0.0.6/autohelper/util/
+-rw-rw-rw-   0        0        0        0 2023-12-13 14:30:39.000000 autohelper-0.0.6/autohelper/util/__init__.py
+-rw-rw-rw-   0        0        0      707 2024-04-02 04:07:38.000000 autohelper-0.0.6/autohelper/util/json.py
+-rw-rw-rw-   0        0        0      109 2024-04-02 11:28:23.000000 autohelper-0.0.6/autohelper/util/list.py
+-rw-rw-rw-   0        0        0     1127 2024-04-04 17:00:56.000000 autohelper-0.0.6/autohelper/util/path.py
+-rw-rw-rw-   0        0        0      246 2024-03-26 05:25:09.000000 autohelper-0.0.6/autohelper/util/thread.py
+-rw-rw-rw-   0        0        0     2923 2024-03-14 10:21:07.000000 autohelper-0.0.6/autohelper/util/win32_process.py
+-rw-rw-rw-   0        0        0      735 2024-03-26 06:27:07.000000 autohelper-0.0.6/autohelper/util/yaml.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:04:46.029683 autohelper-0.0.6/autohelper.egg-info/
+-rw-rw-rw-   0        0        0     2270 2024-04-05 12:04:45.000000 autohelper-0.0.6/autohelper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4379 2024-04-05 12:04:45.000000 autohelper-0.0.6/autohelper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 12:04:45.000000 autohelper-0.0.6/autohelper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      144 2024-04-05 12:04:45.000000 autohelper-0.0.6/autohelper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-05 12:04:45.000000 autohelper-0.0.6/autohelper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-05 12:04:46.129094 autohelper-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1003 2024-04-04 14:44:28.000000 autohelper-0.0.6/setup.py
```

### Comparing `autohelper-0.0.5/README.md` & `autohelper-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `autohelper-0.0.5/autohelper/capture/BaseCaptureMethod.py` & `autohelper-0.0.6/autohelper/capture/BaseCaptureMethod.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,15 +7,14 @@
     last_captured_frame: np.ndarray
     top_cut = 0
     bottom_cut = 0
     left_cut = 0
     right_cut = 0
     width = 0
     height = 0
-    window_change_listeners = []
 
     def __init__(self):
         # Some capture methods don't need an initialization process
         pass
 
     def close(self):
         # Some capture methods don't need an initialization process
```

### Comparing `autohelper-0.0.5/autohelper/capture/HwndWindow.py` & `autohelper-0.0.6/autohelper/capture/HwndWindow.py`

 * *Files 18% similar despite different names*

```diff
@@ -30,41 +30,53 @@
     hwnd = None
     frame_width = 0
     frame_height = 0
     exists = False
 
     def __init__(self, title="", exit_event=threading.Event(), frame_width=0, frame_height=0):
         super().__init__()
-        self.title = title
+        self.app_exit_event = exit_event
+        self.stop_event = threading.Event()
+        self.update_title_re(title)
         self.visible = False
         self.update_frame_size(frame_width, frame_height)
         self.do_update_window_size()
         self.thread = threading.Thread(target=self.update_window_size)
-        self.exit_event = exit_event
         self.thread.start()
 
     @override
     def close(self):
-        self.exit_event.set()
+        self.app_exit_event.set()
+
+    def stop(self):
+        self.stop_event.set()
+
+    def update_title_re(self, title):
+        self.title = re.compile(title)
 
     def update_frame_size(self, width, height):
         if width != self.frame_width or height != self.frame_height:
             self.frame_width = width
             self.frame_height = height
             if width > 0 and height > 0:
                 self.frame_aspect_ratio = width / height
                 logger.debug(f"HwndWindow: frame ratio:{self.frame_aspect_ratio} width: {width}, height: {height}")
 
     def update_window_size(self):
-        while not self.exit_event.is_set():
+        while not self.app_exit_event.is_set() and not self.stop_event.is_set():
             self.do_update_window_size()
-            self.exit_event.wait(0.1)
+            self.app_exit_event.wait(0.1)
 
     def get_abs_cords(self, x, y):
-        return int(self.x + (self.border + x) / self.scaling), int(self.y + (y + self.title_height) / self.scaling)
+        return int(self.x * self.scaling + (self.border * self.scaling + x)), int(
+            self.y * self.scaling + (y + self.title_height * self.scaling))
+
+    def get_top_left_frame_offset(self):
+        return int(self.border * self.scaling), int(
+            self.title_height * self.scaling)
 
     def do_update_window_size(self):
         visible, x, y, border, title_height, width, height, scaling = self.visible, self.x, self.y, self.border, self.title_height, self.width, self.height, self.scaling
         if self.hwnd is None:
             self.hwnd = find_hwnds_by_title(self.title)
         if self.hwnd is not None:
             self.exists = win32gui.IsWindow(self.hwnd)
@@ -79,32 +91,48 @@
                         title_height += height - cropped_window_height
                         height = cropped_window_height
                 height = height
                 width = width
                 title_height = title_height
             else:
                 self.hwnd = None
-        if visible != self.visible or x != self.x or y != self.y or border != self.border or title_height != self.title_height or width != self.width or height != self.height or scaling != self.scaling:
-            self.visible, self.x, self.y, self.border, self.title_height, self.width, self.height, self.scaling = visible, x, y, border, title_height, width, height, scaling
-            communicate.window.emit(visible, x, y, border, title_height, width, height, scaling)
+            changed = False
+            if visible != self.visible or self.scaling != scaling:
+                self.visible = visible
+                self.scaling = scaling
+                changed = True
+            if (
+                    x != self.x or y != self.y or border != self.border or title_height != self.title_height or width != self.width or height != self.height or scaling != self.scaling) and (
+                    (x >= 0 and y >= 0) or self.visible):
+                self.x, self.y, self.border, self.title_height, self.width, self.height = x, y, border, title_height, width, height
+                changed = True
+            if changed:
+                logger.debug(
+                    f"do_update_window_size changed: {self.visible} {self.x} {self.y} {self.border} {self.width} {self.height} {self.scaling}")
+                communicate.window.emit(self.visible, self.x, self.y, self.border, self.title_height, self.width,
+                                        self.height, self.scaling)
 
     def frame_ratio(self, size):
         if self.frame_width > 0 and self.width > 0:
             return int(size / self.frame_width * self.width)
         else:
             return size
 
+    def title_text(self):
+        if self.hwnd:
+            return win32gui.GetWindowText(self.hwnd)
+        return ""
+
 
 def find_hwnds_by_title(title):
-    if isinstance(title, re.Pattern):
-        hwnds = []
+    hwnds = []
 
-        def enum_windows_proc(hwnd, lParam):
-            if win32gui.IsWindowVisible(hwnd) and win32gui.GetWindowText(hwnd):
-                if re.search(title, win32gui.GetWindowText(hwnd)):
-                    hwnds.append(hwnd)
-
-        win32gui.EnumWindows(enum_windows_proc, None)
-        if len(hwnds) > 0:
-            return hwnds[0]
-    else:
-        return win32gui.FindWindow(None, title)
+    def enum_windows_proc(hwnd, lParam):
+        if win32gui.IsWindowVisible(hwnd) and win32gui.GetWindowText(hwnd):
+            if re.search(title, win32gui.GetWindowText(hwnd)):
+                hwnds.append(hwnd)
+
+    win32gui.EnumWindows(enum_windows_proc, None)
+    if len(hwnds) > 0:
+        if len(hwnds) > 1:
+            logger.warning(f"Found multiple hwnds {len(hwnds)}")
+        return hwnds[0]
```

### Comparing `autohelper-0.0.5/autohelper/capture/adb/ADBCaptureMethod.py` & `autohelper-0.0.6/autohelper/capture/adb/ADBCaptureMethod.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 class ADBCaptureMethod(BaseCaptureMethod):
     name = "ADB command line Capture"
     description = "use the adb screencap command, slow but works when in background/minimized, takes 300ms per frame"
 
     def __init__(self, device_manager):
         super().__init__()
         self.device_manager = device_manager
-        logger.info(f"ADBCaptureMethod size: {self.width}x{self.height}")
 
     @property
     def width(self):
         return self.device_manager.width
 
     @property
     def height(self):
```

### Comparing `autohelper-0.0.5/autohelper/capture/adb/targets.py` & `autohelper-0.0.6/autohelper/capture/adb/targets.py`

 * *Files identical despite different names*

### Comparing `autohelper-0.0.5/autohelper/capture/adb/vbox.py` & `autohelper-0.0.6/autohelper/capture/adb/vbox.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
                             rule_name, proto, host, port, guest_host, guest_port = forward.split(',', 5)
                             if proto == '1' and guest_port == '5555':
                                 address = f'127.0.0.1:{port}'
                                 identifier = f'vbox:{server.tag}:{machine_name}'
                                 logger.debug(
                                     f'adb_server, None, {server.vendor}: {machine_name}, {address}, 2, 1, override_identifier={identifier}')
                                 results.append(
-                                    ADBControllerTarget(None, f'{server.vendor}: {machine_name}',
+                                    ADBControllerTarget(None, f'{server.vendor}',
                                                         address, 2, 1, override_identifier=identifier,
                                                         preload_device_info={'emulator_hypervisor': 'vbox'}))
             logger.debug(f'try checking {server}')
         except Exception as e:
             logger.error(f'failed to check server :{server} {e}', e)
     return results
```

### Comparing `autohelper-0.0.5/autohelper/capture/windows/WindowsGraphicsCaptureMethod.py` & `autohelper-0.0.6/autohelper/capture/windows/WindowsGraphicsCaptureMethod.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,24 +172,29 @@
             frame = self.last_frame
             self.last_frame = None
             latency = time.time() - self.last_frame_time
             self.last_frame_time = time.time()
             if latency > 1:
                 logger.warning(f"latency too large return None frame: {latency}")
                 return None
-            if frame is not None and (self.hwnd_window.title_height != 0 or self.hwnd_window.border != 0):
-                frame = crop_image(frame, self.hwnd_window.border, self.hwnd_window.title_height)
+            if frame is not None:
+                x, y = self.hwnd_window.get_top_left_frame_offset()
+                if x > 0 or y > 0:
+                    frame = crop_image(frame, x, y)
 
             if frame is not None:
                 new_height, new_width = frame.shape[:2]
-                self.width = new_width
-                self.height = new_height
-
-                if frame.shape[2] == 4:
-                    frame = frame[:, :, :3]
+                if new_width <= 0 or new_width <= 0:
+                    logger.warning(f"get_frame size <=0 {new_width}x{new_height}")
+                    frame = None
+                else:
+                    self.width = new_width
+                    self.height = new_height
+                    if frame.shape[2] == 4:
+                        frame = frame[:, :, :3]
             return frame
 
     def reset_framepool(self, size, reset_device=False):
         if reset_device:
             self.create_device()
         self.frame_pool.Recreate(self.rtdevice,
                                  DirectXPixelFormat.B8G8R8A8UIntNormalized, 1, size)
```

### Comparing `autohelper-0.0.5/autohelper/capture/windows/d3d11.py` & `autohelper-0.0.6/autohelper/capture/windows/d3d11.py`

 * *Files identical despite different names*

### Comparing `autohelper-0.0.5/autohelper/capture/windows/utils.py` & `autohelper-0.0.6/autohelper/capture/windows/utils.py`

 * *Files identical despite different names*

### Comparing `autohelper-0.0.5/autohelper/capture/windows/window.py` & `autohelper-0.0.6/autohelper/capture/windows/window.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,27 +17,20 @@
     ctypes.windll.dwmapi.DwmGetWindowAttribute(
         hwnd,
         DWMWA_EXTENDED_FRAME_BOUNDS,
         ctypes.byref(extended_frame_bounds),
         ctypes.sizeof(extended_frame_bounds),
     )
     scaling = user32.GetDpiForWindow(hwnd) / 96
-    window_rect = win32gui.GetWindowRect(hwnd)
-    window_width = window_rect[2] - window_rect[0]
-    window_height = window_rect[3] - window_rect[1]
     client_x, client_y, client_width, client_height = win32gui.GetClientRect(hwnd)
-    # print(f"get_window_bounds: scaling:{scaling},window_rect:{window_rect}, client:({client_x},{client_y},{client_width},{client_height}))")
-    # window_left_bounds = extended_frame_bounds.left - window_rect[0]
-    # window_top_bounds = extended_frame_bounds.top - window_rect[1]
-    client_width = int(client_width * scaling)
-    client_height = int(client_height * scaling)
-    window_width = extended_frame_bounds.right - extended_frame_bounds.left
-    window_height = extended_frame_bounds.bottom - extended_frame_bounds.top
-    # print(f"window_width:{window_width} client_width:{client_width}")
+    client_width = int(client_width / scaling)
+    client_height = int(client_height / scaling)
+    window_width = int((extended_frame_bounds.right - extended_frame_bounds.left) / scaling)
+    window_height = int((extended_frame_bounds.bottom - extended_frame_bounds.top) / scaling)
     border = int((window_width - client_width) / 2)
     title = window_height - client_height - border
-    # print(f"{border}, {title}, {client_width}, {client_height}")
-    return extended_frame_bounds.left, extended_frame_bounds.top, border, title, client_width, client_height, scaling
+    return int(extended_frame_bounds.left / scaling), int(
+        extended_frame_bounds.top / scaling), border, title, client_width, client_height, scaling
 
 
 def is_foreground_window(hwnd):
     return win32gui.IsWindowVisible(hwnd) and win32gui.GetForegroundWindow() == hwnd
```

### Comparing `autohelper-0.0.5/autohelper/color/Color.py` & `autohelper-0.0.6/autohelper/color/Color.py`

 * *Files identical despite different names*

### Comparing `autohelper-0.0.5/autohelper/feature/Box.py` & `autohelper-0.0.6/autohelper/feature/Box.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
             vertical_distance = top2 - bottom1
         elif bottom2 < top1:
             vertical_distance = top1 - bottom2
         else:
             vertical_distance = 0
 
         # If boxes overlap or touch, the closest distance is 0
-        if horizontal_distance == 0 or vertical_distance == 0:
+        if horizontal_distance == 0 and vertical_distance == 0:
             return 0
 
         # If boxes are diagonally aligned, calculate diagonal distance
         return math.sqrt(horizontal_distance ** 2 + vertical_distance ** 2)
 
     def relative_with_variance(self, relative_x=0.5, relative_y=0.5):
         # Calculate the center of the box
@@ -88,21 +88,21 @@
             box_center_x, box_center_y = box.center()
 
             dx = box_center_x - orig_center_x
             dy = box_center_y - orig_center_y
             distance = math.sqrt(dx ** 2 + dy ** 2)
             if box == self:
                 return float('inf')
-            elif direction == 'up' and self.y - (box.y + box.height) >= 0:
+            elif direction == 'up' and self.y - (box.y + box.height / 2) >= 0:
                 return distance
-            elif direction == 'down' and box.y - (self.y + self.height) >= 0:
+            elif direction == 'down' and box.y - (self.y + self.height / 2) >= 0:
                 return distance
-            elif direction == 'left' and self.x - (box.x + box.width) >= 0:
+            elif direction == 'left' and self.x - (box.x + box.width / 2) >= 0:
                 return distance
-            elif direction == 'right' and box.x - (self.x + self.width) >= 0:
+            elif direction == 'right' and box.x - (self.x + self.width / 2) >= 0:
                 return distance
             else:
                 return float('inf')
 
         filtered_boxes = sorted(boxes, key=distance_criteria)
         # Removed debug print statement for cleanliness
```

### Comparing `autohelper-0.0.5/autohelper/feature/Feature.py` & `autohelper-0.0.6/autohelper/feature/Feature.py`

 * *Files identical despite different names*

### Comparing `autohelper-0.0.5/autohelper/feature/FeatureSet.py` & `autohelper-0.0.6/autohelper/feature/FeatureSet.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,16 +38,16 @@
             default_threshold = 0.95
         self.default_threshold = default_threshold
         self.default_horizontal_variance = default_horizontal_variance
         self.default_vertical_variance = default_vertical_variance
 
     def check_size(self, frame):
         height, width = frame.shape[:2]
-        if self.width != width or self.height != height:
-            print(f"FeatureSet: Width and height changed from {self.width}x{self.height} to {width}x{height}")
+        if self.width != width or self.height != height and height > 0 and width > 0:
+            logger.info(f"FeatureSet: Width and height changed from {self.width}x{self.height} to {width}x{height}")
             self.width = width
             self.height = height
             self.process_data()
 
     def process_data(self) -> None:
         """
         Process the images and annotations from the COCO dataset.
```

### Comparing `autohelper-0.0.5/autohelper/feature/FindFeature.py` & `autohelper-0.0.6/autohelper/feature/FindFeature.py`

 * *Files identical despite different names*

### Comparing `autohelper-0.0.5/autohelper/gui/MainWindow.py` & `autohelper-0.0.6/autohelper/gui/MainWindow.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,21 +9,22 @@
 
 
 class Communicate(QObject):
     speak = Signal(str)
 
 
 class MainWindow(QTabWidget):
-    def __init__(self, tasks, exit_event):
+    def __init__(self, tasks, debug=False, exit_event=None):
         super().__init__()
         self.exit_event = exit_event
-        debug_tab = DebugTab()
         task_tab = TaskTab(tasks)
-        self.addTab(task_tab, "Task")
-        self.addTab(debug_tab, "Debug")
+        self.addTab(task_tab, self.tr("Task"))
+        if debug:
+            debug_tab = DebugTab()
+            self.addTab(debug_tab, self.tr("Debug"))
         # ... Add other tabs similarly
 
         # Styling the tabs and content if needed, for example:
         self.setStyleSheet("""
                             QTabWidget::tab-bar {
                                 alignment: center;
                             }
```

### Comparing `autohelper-0.0.5/autohelper/gui/TabTitles.py` & `autohelper-0.0.6/autohelper/gui/TabTitles.py`

 * *Files identical despite different names*

### Comparing `autohelper-0.0.5/autohelper/gui/debug/AspectRatioWidget.py` & `autohelper-0.0.6/autohelper/gui/debug/AspectRatioWidget.py`

 * *Files identical despite different names*

### Comparing `autohelper-0.0.5/autohelper/gui/debug/DebugTab.py` & `autohelper-0.0.6/autohelper/gui/debug/DebugTab.py`

 * *Files identical despite different names*

### Comparing `autohelper-0.0.5/autohelper/gui/debug/FrameWidget.py` & `autohelper-0.0.6/autohelper/gui/debug/FrameWidget.py`

 * *Files identical despite different names*

### Comparing `autohelper-0.0.5/autohelper/gui/debug/InfoWidget.py` & `autohelper-0.0.6/autohelper/gui/debug/InfoWidget.py`

 * *Files identical despite different names*

### Comparing `autohelper-0.0.5/autohelper/gui/debug/LoggerWidget.py` & `autohelper-0.0.6/autohelper/gui/debug/LoggerWidget.py`

 * *Files identical despite different names*

### Comparing `autohelper-0.0.5/autohelper/gui/overlay/OverlayWindow.py` & `autohelper-0.0.6/autohelper/gui/overlay/OverlayWindow.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,12 +22,13 @@
         self.setWindowFlag(Qt.Tool)
         communicate.window.connect(self.update_overlay)
         self.update_overlay(hwnd_window.visible, hwnd_window.x, hwnd_window.y, hwnd_window.border,
                             hwnd_window.title_height, hwnd_window.width, hwnd_window.height, hwnd_window.scaling)
 
     def update_overlay(self, visible, x, y, border, title_height, width, height, scaling):
         logger.debug(f'update_overlay: {visible}, {x}, {y}, {border}, {title_height} {width}, {height}, {scaling}')
-        self.setGeometry(x + border, y + title_height, width, height)
+        if visible:
+            self.setGeometry(x + border, y + title_height, width, height)
         if visible:
             self.show()
         else:
             self.hide()
```

### Comparing `autohelper-0.0.5/autohelper/interaction/ADBInteraction.py` & `autohelper-0.0.6/autohelper/interaction/ADBInteraction.py`

 * *Files identical despite different names*

### Comparing `autohelper-0.0.5/autohelper/interaction/BaseInteraction.py` & `autohelper-0.0.6/autohelper/interaction/BaseInteraction.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 
 
 class BaseInteraction:
 
     def __init__(self, capture):
         self.capture = capture
 
+    def should_capture(self):
+        return True
+    
     def send_key(self, key, down_time=0.02):
         pass
 
     def move(self, x, y):
         pass
 
     def click_relative(self, x, y):
```

### Comparing `autohelper-0.0.5/autohelper/interaction/Win32Interaction.py` & `autohelper-0.0.6/autohelper/interaction/Win32Interaction.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,14 +40,17 @@
         # lParam = win32api.MAKELONG(x, y)
         if x != -1 and y != -1:
             x, y = self.capture.get_abs_cords(x, y)
             logger.info(f"left_click {x, y}")
             pydirectinput.moveTo(x, y)
         pydirectinput.click()
 
+    def should_capture(self):
+        return self.capture.clickable()
+
 
 def is_admin():
     try:
         # Only Windows users with admin privileges can read the C drive directly
         return ctypes.windll.shell32.IsUserAnAdmin()
     except:
         return False
```

### Comparing `autohelper-0.0.5/autohelper/logging/Logger.py` & `autohelper-0.0.6/autohelper/logging/Logger.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 import os
 import traceback
 from logging.handlers import TimedRotatingFileHandler
 
 from autohelper.gui.Communicate import communicate
+from autohelper.util.path import get_path_relative_to_exe, ensure_dir_for_file
 
 
 class CommunicateHandler(logging.Handler):
     def __init__(self):
         super().__init__()
 
     def emit(self, record):
@@ -43,41 +44,43 @@
     console_handler = logging.StreamHandler()
     console_handler.setFormatter(formatter)
     auto_helper_logger.addHandler(console_handler)
     auto_helper_logger.addHandler(communicate_handler)
     logging.getLogger().handlers = []
 
     if config.get('log_file'):
-        ensure_dir_for_file(config['log_file'])
+        logger_file = get_path_relative_to_exe(config.get('log_file'))
+        ensure_dir_for_file(logger_file)
 
         os.makedirs("logs", exist_ok=True)
         # File handler with rotation
-        file_handler = TimedRotatingFileHandler(config['log_file'], when="midnight", interval=1,
+        file_handler = TimedRotatingFileHandler(logger_file, when="midnight", interval=1,
                                                 backupCount=7, encoding='utf-8')
         file_handler.setFormatter(formatter)
         file_handler.setLevel(logging.DEBUG)  # File handler level
         auto_helper_logger.addHandler(file_handler)
 
     if config.get('error_log_file'):
-        ensure_dir_for_file(config['error_log_file'])
+        error_log_file = get_path_relative_to_exe(config.get('error_log_file'))
+        ensure_dir_for_file(error_log_file)
 
         os.makedirs("logs", exist_ok=True)
         # File handler with rotation
-        file_handler = TimedRotatingFileHandler(config['error_log_file'], when="midnight", interval=1,
+        file_handler = TimedRotatingFileHandler(error_log_file, when="midnight", interval=1,
                                                 backupCount=7, encoding='utf-8')
         file_handler.setFormatter(formatter)
         file_handler.setLevel(logging.ERROR)  # File handler level
         auto_helper_logger.addHandler(file_handler)
 
 
 class Logger:
     def __init__(self, name):
         # Initialize the logger with the name of the subclass
         self.logger = auto_helper_logger
-        self.name = name
+        self.name = name.split('.')[-1]
 
     def debug(self, message):
         self.logger.debug(f"{self.name}:{message}")
 
     def info(self, message):
         self.logger.info(f"{self.name}:{message}")
 
@@ -94,20 +97,7 @@
 
     def critical(self, message):
         self.logger.critical(f"{self.name}:{message}")
 
 
 def get_logger(name):
     return Logger(name)
-
-
-def ensure_dir_for_file(file_path):
-    # Extract the directory from the file path
-    directory = os.path.dirname(file_path)
-
-    # Check if the directory exists
-    if not os.path.exists(directory):
-        # If the directory does not exist, create it (including any intermediate directories)
-        os.makedirs(directory)
-        print(f"Directory created: {directory}")
-    else:
-        print(f"Directory already exists: {directory}")
```

### Comparing `autohelper-0.0.5/autohelper/ocr/OCR.py` & `autohelper-0.0.6/autohelper/ocr/OCR.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,48 +4,45 @@
 from autohelper.gui.Communicate import communicate
 from autohelper.logging.Logger import get_logger
 
 logger = get_logger(__name__)
 
 
 class OCR:
-
-    def __init__(self):
-        self.executor = None
-        self.default_threshold = 0.9
+    executor = None
+    default_threshold = 0.6
 
     def ocr(self, box: Box = None, match=None, threshold=0):
         if threshold == 0:
-            threshold = 0.9
+            threshold = self.default_threshold
         start = time.time()
         image = self.frame
         if image is not None:
             if box is not None:
                 x, y, w, h = box.x, box.y, box.width, box.height
                 image = image[y:y + h, x:x + w]
 
-            result = self.executor.ocr.ocr(image)
-
+            result, _ = self.executor.ocr(image, use_det=True, use_cls=False, use_rec=True)
             detected_boxes = []
             # Process the results and create Box objects
-            for res in result:
-                if res is not None:
-                    for line in res:
-                        pos = line[0]
-                        text, confidence = line[1]
-                        if confidence >= threshold:
-                            detected_box = Box(int(pos[0][0]), int(pos[0][1]), int(pos[2][0] - pos[0][0]),
-                                               int(pos[2][1] - pos[0][1]),
-                                               confidence, text)
-                            if box is not None:
-                                detected_box.x += box.x
-                                detected_box.y += box.y
-                            detected_boxes.append(detected_box)
-            if match is not None:
-                detected_boxes = find_boxes_by_name(detected_boxes, match)
+            if result is not None:
+                for res in result:
+                    pos = res[0]
+                    text = res[1]
+                    confidence = res[2]
+                    if confidence >= threshold:
+                        detected_box = Box(int(pos[0][0]), int(pos[0][1]), int(pos[2][0] - pos[0][0]),
+                                           int(pos[2][1] - pos[0][1]),
+                                           confidence, text)
+                        if box is not None:
+                            detected_box.x += box.x
+                            detected_box.y += box.y
+                        detected_boxes.append(detected_box)
+                if match is not None:
+                    detected_boxes = find_boxes_by_name(detected_boxes, match)
             communicate.draw_box.emit("ocr", detected_boxes, "red")
             communicate.draw_box.emit("ocr_zone", box, "blue")
             logger.debug(f"ocr_zone {box} found result: {len(detected_boxes)}) time: {time.time() - start}")
             return sort_boxes(detected_boxes)
 
     def find_text(self, text, box: Box = None, confidence=0):
         for result in self.ocr(box, confidence):
```

### Comparing `autohelper-0.0.5/autohelper/predict/predict.py` & `autohelper-0.0.6/autohelper/predict/predict.py`

 * *Files identical despite different names*

### Comparing `autohelper-0.0.5/autohelper/rotypes/Windows/Foundation/Collections.py` & `autohelper-0.0.6/autohelper/rotypes/Windows/Foundation/Collections.py`

 * *Files identical despite different names*

### Comparing `autohelper-0.0.5/autohelper/rotypes/Windows/Foundation/__init__.py` & `autohelper-0.0.6/autohelper/rotypes/Windows/Foundation/__init__.py`

 * *Files identical despite different names*

### Comparing `autohelper-0.0.5/autohelper/rotypes/Windows/Globalization/__init__.py` & `autohelper-0.0.6/autohelper/rotypes/Windows/Globalization/__init__.py`

 * *Files identical despite different names*

### Comparing `autohelper-0.0.5/autohelper/rotypes/Windows/Graphics/Capture/__init__.py` & `autohelper-0.0.6/autohelper/rotypes/Windows/Graphics/Capture/__init__.py`

 * *Files identical despite different names*

### Comparing `autohelper-0.0.5/autohelper/rotypes/Windows/Graphics/DirectX/Direct3D11/__init__.py` & `autohelper-0.0.6/autohelper/rotypes/Windows/Graphics/DirectX/Direct3D11/__init__.py`

 * *Files identical despite different names*

### Comparing `autohelper-0.0.5/autohelper/rotypes/Windows/Graphics/DirectX/__init__.py` & `autohelper-0.0.6/autohelper/rotypes/Windows/Graphics/DirectX/__init__.py`

 * *Files identical despite different names*

### Comparing `autohelper-0.0.5/autohelper/rotypes/Windows/Graphics/Imaging/__init__.py` & `autohelper-0.0.6/autohelper/rotypes/Windows/Graphics/Imaging/__init__.py`

 * *Files identical despite different names*

### Comparing `autohelper-0.0.5/autohelper/rotypes/Windows/Media/Ocr/__init__.py` & `autohelper-0.0.6/autohelper/rotypes/Windows/Media/Ocr/__init__.py`

 * *Files identical despite different names*

### Comparing `autohelper-0.0.5/autohelper/rotypes/Windows/Security/Cryptography/__init__.py` & `autohelper-0.0.6/autohelper/rotypes/Windows/Security/Cryptography/__init__.py`

 * *Files identical despite different names*

### Comparing `autohelper-0.0.5/autohelper/rotypes/Windows/Storage/Streams/__init__.py` & `autohelper-0.0.6/autohelper/rotypes/Windows/Storage/Streams/__init__.py`

 * *Files identical despite different names*

### Comparing `autohelper-0.0.5/autohelper/rotypes/delegate.py` & `autohelper-0.0.6/autohelper/rotypes/delegate.py`

 * *Files identical despite different names*

### Comparing `autohelper-0.0.5/autohelper/rotypes/export.py` & `autohelper-0.0.6/autohelper/rotypes/export.py`

 * *Files identical despite different names*

### Comparing `autohelper-0.0.5/autohelper/rotypes/idldsl.py` & `autohelper-0.0.6/autohelper/rotypes/idldsl.py`

 * *Files identical despite different names*

### Comparing `autohelper-0.0.5/autohelper/rotypes/inspectable.py` & `autohelper-0.0.6/autohelper/rotypes/inspectable.py`

 * *Files identical despite different names*

### Comparing `autohelper-0.0.5/autohelper/rotypes/roapi.py` & `autohelper-0.0.6/autohelper/rotypes/roapi.py`

 * *Files identical despite different names*

### Comparing `autohelper-0.0.5/autohelper/rotypes/types.py` & `autohelper-0.0.6/autohelper/rotypes/types.py`

 * *Files identical despite different names*

### Comparing `autohelper-0.0.5/autohelper/rotypes/winstring.py` & `autohelper-0.0.6/autohelper/rotypes/winstring.py`

 * *Files identical despite different names*

### Comparing `autohelper-0.0.5/autohelper/save/BlackBarProcessor.py` & `autohelper-0.0.6/autohelper/save/BlackBarProcessor.py`

 * *Files identical despite different names*

### Comparing `autohelper-0.0.5/autohelper/save/SaveByInterval.py` & `autohelper-0.0.6/autohelper/save/SaveByInterval.py`

 * *Files identical despite different names*

### Comparing `autohelper-0.0.5/autohelper/save/SaveByKeyPress.py` & `autohelper-0.0.6/autohelper/save/SaveByKeyPress.py`

 * *Files identical despite different names*

### Comparing `autohelper-0.0.5/autohelper/save/SaveMethodBase.py` & `autohelper-0.0.6/autohelper/save/SaveMethodBase.py`

 * *Files identical despite different names*

### Comparing `autohelper-0.0.5/autohelper/stats/StreamStats.py` & `autohelper-0.0.6/autohelper/stats/StreamStats.py`

 * *Files identical despite different names*

### Comparing `autohelper-0.0.5/autohelper/task/BaseTask.py` & `autohelper-0.0.6/autohelper/task/ExecutorOperation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,16 @@
 from autohelper.feature.Box import Box, find_box_by_name
 from autohelper.gui.Communicate import communicate
 from autohelper.logging.Logger import get_logger
-from autohelper.task.TaskExecutor import TaskExecutor
 
 logger = get_logger(__name__)
 
 
-class BaseTask:
-    executor: TaskExecutor
-    _done = False
-
-    def __init__(self):
-        self.logger = get_logger(self.__class__.__name__)
-        self.name = self.__class__.__name__
-        self.success_count = 0
-        self.error_count = 0
-        self.enabled = True
-        self.running = False
-        self.config = {}
-
-    def run_frame(self):
-        pass
-
-    def reset(self):
-        self._done = False
-        pass
+class ExecutorOperation:
+    executor = None
 
     def box_in_horizontal_center(self, box, off_percent=0.02):
         center = self.executor.method.width / 2
         left = center - box.x
         right = box.x + box.width - center
         if left > 0 and right > 0 and abs(left - right) / box.width < off_percent:
             return True
@@ -64,18 +46,20 @@
         """
         to_click = find_box_by_name(boxes, names)
         if to_click is not None:
             logger.info(f"click_box_if_name_match found {to_click}")
             self.click_box(to_click, relative_x, relative_y)
             return to_click
 
-    def box_of_screen(self, x, y, width, height):
+    def box_of_screen(self, x, y, width, height, name=None):
+        if name is None:
+            name = f"{x} {y} {width} {height}"
         return Box(int(x * self.executor.method.width), int(y * self.executor.method.height),
                    int(width * self.executor.method.width), int(height * self.executor.method.height),
-                   name=f"{x} {y} {width} {height}")
+                   name=name)
 
     def click_relative(self, x, y):
         self.executor.reset_scene()
         self.executor.interaction.click_relative(x, y)
 
     @property
     def height(self):
@@ -105,21 +89,14 @@
 
     def wait_scene(self, scene_type=None, time_out=0, pre_action=None, post_action=None):
         return self.executor.wait_scene(scene_type, time_out, pre_action, post_action)
 
     def sleep(self, timeout):
         self.executor.sleep(timeout)
 
-    @property
-    def done(self):
-        return self._done
-
-    def set_done(self, done=True):
-        self._done = done
-
     def send_key(self, key, down_time=0.02):
         self.executor.interaction.send_key(key, down_time)
 
     def wait_until(self, condition, time_out=0, pre_action=None, post_action=None):
         return self.executor.wait_condition(condition, time_out, pre_action, post_action)
 
     def wait_click_box(self, condition, time_out=0, pre_action=None, post_action=None, raise_if_not_found=True):
```

### Comparing `autohelper-0.0.5/autohelper/task/TaskExecutor.py` & `autohelper-0.0.6/autohelper/task/TaskExecutor.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,66 +1,80 @@
 import threading
 import time
 import traceback
 
-from autohelper.capture.BaseCaptureMethod import BaseCaptureMethod
+from autohelper.capture.adb.DeviceManager import DeviceManager
 from autohelper.gui.Communicate import communicate
-from autohelper.interaction.BaseInteraction import BaseInteraction
 from autohelper.logging.Logger import get_logger
 from autohelper.scene.Scene import Scene
 from autohelper.stats.StreamStats import StreamStats
 
 logger = get_logger(__name__)
 
 
+class TaskDisabledException(Exception):
+    pass
+
+
 class TaskExecutor:
     current_scene: Scene | None = None
     last_scene: Scene | None = None
     frame_stats = StreamStats()
     _frame = None
     paused = True
     ocr = None
+    pause_start = time.time()
+    pause_end_time = time.time()
 
-    def __init__(self, method: BaseCaptureMethod, interaction: BaseInteraction, target_fps=10,
+    def __init__(self, device_manager: DeviceManager,
                  wait_until_timeout=10, wait_until_before_delay=1, wait_until_check_delay=1,
-                 exit_event=threading.Event(), tasks=[], scenes=[], feature_set=None, ocr=None):
-        self.interaction = interaction
+                 exit_event=threading.Event(), tasks=[], scenes=[], feature_set=None, ocr=None, config_folder=None):
+        self.device_manager = device_manager
         self.feature_set = feature_set
         self.wait_until_check_delay = wait_until_check_delay
         self.wait_until_before_delay = wait_until_before_delay
-        self.method = method
         self.wait_scene_timeout = wait_until_timeout
-        self.target_delay = 1.0 / target_fps
         self.exit_event = exit_event
         self.ocr = ocr
+        self.current_task = None
         self.tasks = tasks
         self.scenes = scenes
+        self.config_folder = config_folder or "config"
         for scene in self.scenes:
             scene.executor = self
             scene.feature_set = self.feature_set
         for task in self.tasks:
             task.executor = self
             task.feature_set = self.feature_set
-        self.thread = threading.Thread(target=self.execute)
+            task.load_config(self.config_folder)
+        self.thread = threading.Thread(target=self.execute, name="TaskExecutor")
         self.thread.start()
 
-    def wait_fps(self, start):
-        cost = time.time() - start
-        if cost < self.target_delay:
-            self.sleep(self.target_delay - cost)
+    @property
+    def interaction(self):
+        return self.device_manager.interaction
+
+    @property
+    def method(self):
+        return self.device_manager.capture_method
 
     def next_frame(self):
         self.reset_scene()
         start = time.time()
         while not self.exit_event.is_set():
-            self._frame = self.method.get_frame()
-            if self._frame is not None:
-                communicate.frame.emit(self._frame)
-                return self._frame
-            time.sleep(0.01)
+            if self.method and self.interaction.should_capture():
+                self._frame = self.method.get_frame()
+                if self._frame is not None:
+                    height, width = self._frame.shape[:2]
+                    if height <= 0 or width <= 0:
+                        logger.warning(f"captured wrong size frame: {width}x{height}")
+                        self._frame = None
+                    communicate.frame.emit(self._frame)
+                    return self._frame
+            self.sleep(0.001)
             if time.time() - start > self.wait_scene_timeout:
                 return None
 
     @property
     def frame(self):
         if self._frame is None:
             return self.next_frame()
@@ -70,23 +84,46 @@
     def sleep(self, timeout):
         """
         Sleeps for the specified timeout, checking for an exit event every 100ms, with adjustments to prevent oversleeping.
 
         :param timeout: The total time to sleep in seconds.
         """
         self.frame_stats.add_sleep(timeout)
-        end_time = time.time() + timeout
+        self.pause_end_time = time.time() + timeout
         while True:
             if self.exit_event.is_set():
                 logger.info("Exit event set. Exiting early.")
                 return
-            remaining = end_time - time.time()
-            if remaining <= 0:
-                return
-            time.sleep(min(0.1, remaining))  # Sleep for 100ms or the remaining time, whichever is smaller
+            if self.current_task and not self.current_task.enabled:
+                raise TaskDisabledException()
+            if not (self.paused or not self.interaction.should_capture()):
+                to_sleep = self.pause_end_time - time.time()
+                if to_sleep <= 0:
+                    return
+            time.sleep(0.01)  # Sleep for 100ms or the remaining time, whichever is smaller
+
+    def pause(self):
+        self.paused = True
+        self.pause_start = time.time()
+        communicate.executor_paused.emit(self.paused)
+        communicate.tasks.emit()
+
+    def start(self):
+        can_run = False
+        for task in self.tasks:
+            if task.can_run():
+                can_run = True
+                break
+        if not can_run:
+            return False
+        self.pause_end_time += self.pause_start - time.time()
+        self.paused = False
+        communicate.executor_paused.emit(self.paused)
+        communicate.tasks.emit()
+        return True
 
     def wait_scene(self, scene_type, time_out, pre_action, post_action):
         return self.wait_condition(lambda: self.detect_scene(scene_type), time_out, pre_action, post_action)
 
     def wait_condition(self, condition, time_out, pre_action, post_action):
         self.sleep(self.wait_until_before_delay)
         start = time.time()
@@ -103,18 +140,18 @@
                 result_str = list_or_obj_to_str(result)
                 if result:
                     logger.debug(f"found result {result_str}")
                     self.sleep(self.wait_until_check_delay)
                     return result
             if post_action is not None:
                 post_action()
-            self.wait_fps(start)
             if time.time() - start > time_out:
                 logger.info(f"wait_until timeout {condition} {time_out} seconds")
                 break
+            self.sleep(0.01)
         return None
 
     def reset_scene(self):
         self._frame = None
         self.last_scene = self.current_scene
         self.current_scene = None
 
@@ -122,42 +159,48 @@
         logger.info(f"start execute")
         while not self.exit_event.is_set():
             self._frame = self.next_frame()
             start = time.time()
             if self._frame is not None:
                 self.detect_scene()
                 task_executed = 0
-                for task in self.tasks:
-                    if task.done:
+                for index, task in enumerate(self.tasks):
+                    if task.done or not task.enabled:
                         continue
+                    self.current_task = task
                     task.running = True
-                    communicate.tasks.emit()
+                    task.last_execute_time = start
                     try:
                         result = task.run_frame()
                         if result is not None:
                             if result:
                                 task.success_count += 1
                             else:
                                 task.error_count += 1
+                    except TaskDisabledException:
+                        logger.info(f"{task.name} is disabled, breaking")
                     except Exception as e:
                         traceback.print_exc()
                         stack_trace_str = traceback.format_exc()
                         logger.error(f"{task.name} exception: {e}, traceback: {stack_trace_str}")
                         task.error_count += 1
+                    self.current_task = None
                     task.running = False
-                    communicate.tasks.emit()
                     processing_time = time.time() - start
                     task_executed += 1
-                    if processing_time > 0.2:
+                    if processing_time > 0.5:
                         logger.debug(
                             f"{task.__class__.__name__} taking too long get new frame {processing_time} {task_executed} {len(self.tasks)}")
                         self.next_frame()
                         start = time.time()
+
+                # if task_executed == 0:
+                #     self.pause()
                 self.add_frame_stats()
-            self.wait_fps(start)
+                self.sleep(0.001)
 
     def add_frame_stats(self):
         self.frame_stats.add_frame()
         mean = self.frame_stats.mean()
         if mean > 0:
             communicate.frame_time.emit(mean)
             communicate.fps.emit(round(1000 / mean))
```

### Comparing `autohelper-0.0.5/autohelper/util/win32_process.py` & `autohelper-0.0.6/autohelper/util/win32_process.py`

 * *Files identical despite different names*

### Comparing `autohelper-0.0.5/autohelper.egg-info/SOURCES.txt` & `autohelper-0.0.6/autohelper.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -19,36 +19,58 @@
 autohelper/capture/windows/WindowsGraphicsCaptureMethod.py
 autohelper/capture/windows/__init__.py
 autohelper/capture/windows/d3d11.py
 autohelper/capture/windows/utils.py
 autohelper/capture/windows/window.py
 autohelper/color/Color.py
 autohelper/color/__init__.py
+autohelper/config/Config.py
+autohelper/config/InfoDict.py
+autohelper/config/__init__.py
 autohelper/feature/Box.py
 autohelper/feature/Feature.py
 autohelper/feature/FeatureSet.py
 autohelper/feature/FindFeature.py
 autohelper/feature/__init__.py
 autohelper/gui/App.py
 autohelper/gui/Communicate.py
 autohelper/gui/MainWindow.py
 autohelper/gui/TabTitles.py
 autohelper/gui/__init__.py
+autohelper/gui/resources.py
 autohelper/gui/debug/AspectRatioWidget.py
 autohelper/gui/debug/DebugTab.py
 autohelper/gui/debug/FrameWidget.py
 autohelper/gui/debug/InfoWidget.py
 autohelper/gui/debug/LoggerWidget.py
 autohelper/gui/debug/__init__.py
+autohelper/gui/i18n/__init__.py
+autohelper/gui/i18n/path.py
+autohelper/gui/icon/__init__.py
+autohelper/gui/icon/icon.py
 autohelper/gui/loading/LoadingWindow.py
 autohelper/gui/loading/__init__.py
 autohelper/gui/overlay/OverlayWindow.py
 autohelper/gui/overlay/__init__.py
+autohelper/gui/tasks/ConfigItemFactory.py
+autohelper/gui/tasks/StartButton.py
+autohelper/gui/tasks/TaskOpButton.py
 autohelper/gui/tasks/TaskTab.py
+autohelper/gui/tasks/TooltipTableWidget.py
 autohelper/gui/tasks/__init__.py
+autohelper/gui/util/Alert.py
+autohelper/gui/util/InitWorker.py
+autohelper/gui/util/__init__.py
+autohelper/gui/widget/ListTableWidgetItem.py
+autohelper/gui/widget/NumericTableWidgetItem.py
+autohelper/gui/widget/RoundCornerContainer.py
+autohelper/gui/widget/TabWidget.py
+autohelper/gui/widget/UpdateConfigWidgetItem.py
+autohelper/gui/widget/YesNonWidgetItem.py
+autohelper/gui/widget/__init__.py
 autohelper/interaction/ADBInteraction.py
 autohelper/interaction/BaseInteraction.py
 autohelper/interaction/Win32Interaction.py
 autohelper/interaction/__init__.py
 autohelper/logging/Logger.py
 autohelper/logging/__init__.py
 autohelper/ocr/OCR.py
@@ -86,13 +108,18 @@
 autohelper/save/__init__.py
 autohelper/scene/FeatureScene.py
 autohelper/scene/Scene.py
 autohelper/scene/__init__.py
 autohelper/stats/StreamStats.py
 autohelper/stats/__init__.py
 autohelper/task/BaseTask.py
+autohelper/task/ExecutorOperation.py
 autohelper/task/FindFeatureTask.py
 autohelper/task/TaskExecutor.py
 autohelper/task/__init__.py
 autohelper/util/__init__.py
+autohelper/util/json.py
+autohelper/util/list.py
 autohelper/util/path.py
-autohelper/util/win32_process.py
+autohelper/util/thread.py
+autohelper/util/win32_process.py
+autohelper/util/yaml.py
```

### Comparing `autohelper-0.0.5/setup.py` & `autohelper-0.0.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="autohelper",
-    version="0.0.5",
+    version="0.0.6",
     author="CTO",
     author_email="firedcto@gmail.com",
     description="Automation with Computer Vision for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/CrashTechnologyOfficer/autoui",
     packages=setuptools.find_packages(),
```

