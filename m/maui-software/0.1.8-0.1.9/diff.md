# Comparing `tmp/maui_software-0.1.8.tar.gz` & `tmp/maui_software-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maui_software-0.1.8.tar", max compression
+gzip compressed data, was "maui_software-0.1.9.tar", max compression
```

## Comparing `maui_software-0.1.8.tar` & `maui_software-0.1.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rwxr-xr-x   0        0        0        0 2023-09-08 23:52:51.603000 maui_software-0.1.8/README.md
--rwxr-xr-x   0        0        0        0 2023-09-08 23:52:51.587000 maui_software-0.1.8/maui/__init__.py
--rwxr-xr-x   0        0        0    17889 2023-09-10 14:38:50.035000 maui_software-0.1.8/maui/acoustic_indices.py
--rwxr-xr-x   0        0        0      435 2022-08-14 22:24:14.814000 maui_software-0.1.8/maui/data/letterhead.png
--rwxr-xr-x   0        0        0     3204 2022-08-14 23:33:16.968000 maui_software-0.1.8/maui/data/letterhead_cover.png
--rwxr-xr-x   0        0        0    11262 2023-09-09 03:54:51.131000 maui_software-0.1.8/maui/eda.py
--rwxr-xr-x   0        0        0     3165 2023-09-10 14:22:44.659000 maui_software-0.1.8/maui/io.py
--rwxr-xr-x   0        0        0    24290 2023-09-09 03:20:56.396000 maui_software-0.1.8/maui/visualizations.py
--rwxr-xr-x   0        0        0      509 2023-09-10 18:15:27.643000 maui_software-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      728 1970-01-01 00:00:00.000000 maui_software-0.1.8/PKG-INFO
+-rwxr-xr-x   0        0        0        0 2023-09-08 23:52:51.603000 maui_software-0.1.9/README.md
+-rwxr-xr-x   0        0        0        0 2023-09-08 23:52:51.587000 maui_software-0.1.9/maui/__init__.py
+-rwxr-xr-x   0        0        0    17889 2023-09-10 14:38:50.035000 maui_software-0.1.9/maui/acoustic_indices.py
+-rwxr-xr-x   0        0        0      435 2022-08-14 22:24:14.814000 maui_software-0.1.9/maui/data/letterhead.png
+-rwxr-xr-x   0        0        0     3204 2022-08-14 23:33:16.968000 maui_software-0.1.9/maui/data/letterhead_cover.png
+-rwxr-xr-x   0        0        0    11262 2023-09-09 03:54:51.131000 maui_software-0.1.9/maui/eda.py
+-rwxr-xr-x   0        0        0     3165 2023-09-10 14:22:44.659000 maui_software-0.1.9/maui/io.py
+-rwxr-xr-x   0        0        0    24290 2023-09-09 03:20:56.396000 maui_software-0.1.9/maui/visualizations.py
+-rwxr-xr-x   0        0        0      400 2023-09-10 18:27:37.880000 maui_software-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      493 1970-01-01 00:00:00.000000 maui_software-0.1.9/PKG-INFO
```

### Comparing `maui_software-0.1.8/maui/acoustic_indices.py` & `maui_software-0.1.9/maui/acoustic_indices.py`

 * *Files identical despite different names*

### Comparing `maui_software-0.1.8/maui/data/letterhead_cover.png` & `maui_software-0.1.9/maui/data/letterhead_cover.png`

 * *Files identical despite different names*

### Comparing `maui_software-0.1.8/maui/eda.py` & `maui_software-0.1.9/maui/eda.py`

 * *Files identical despite different names*

### Comparing `maui_software-0.1.8/maui/io.py` & `maui_software-0.1.9/maui/io.py`

 * *Files identical despite different names*

### Comparing `maui_software-0.1.8/maui/visualizations.py` & `maui_software-0.1.9/maui/visualizations.py`

 * *Files identical despite different names*

