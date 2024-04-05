# Comparing `tmp/netbox_textdatastore-0.0.4.tar.gz` & `tmp/netbox_textdatastore-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_textdatastore-0.0.4.tar", last modified: Sat Mar 11 15:08:58 2023, max compression
+gzip compressed data, was "netbox_textdatastore-0.0.5.tar", last modified: Fri Apr  5 18:59:05 2024, max compression
```

## Comparing `netbox_textdatastore-0.0.4.tar` & `netbox_textdatastore-0.0.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-03-11 15:08:58.816162 netbox_textdatastore-0.0.4/
--rw-rw-rw-   0        0        0     7169 2023-01-18 13:40:43.000000 netbox_textdatastore-0.0.4/LICENSE
--rw-rw-rw-   0        0        0       50 2023-01-18 17:12:49.000000 netbox_textdatastore-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0    11270 2023-03-11 15:08:58.814658 netbox_textdatastore-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2645 2023-01-18 17:10:24.000000 netbox_textdatastore-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-03-11 15:08:58.771649 netbox_textdatastore-0.0.4/netbox_textdatastore/
--rw-rw-rw-   0        0        0      385 2023-01-18 13:44:51.000000 netbox_textdatastore-0.0.4/netbox_textdatastore/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-11 15:08:58.802151 netbox_textdatastore-0.0.4/netbox_textdatastore/api/
--rw-rw-rw-   0        0        0        0 2022-09-24 16:48:07.000000 netbox_textdatastore-0.0.4/netbox_textdatastore/api/__init__.py
--rw-rw-rw-   0        0        0      328 2023-01-18 13:45:59.000000 netbox_textdatastore-0.0.4/netbox_textdatastore/api/serializers.py
--rw-rw-rw-   0        0        0      215 2023-01-18 13:47:57.000000 netbox_textdatastore-0.0.4/netbox_textdatastore/api/urls.py
--rw-rw-rw-   0        0        0      374 2023-01-18 13:45:59.000000 netbox_textdatastore-0.0.4/netbox_textdatastore/api/views.py
--rw-rw-rw-   0        0        0      631 2023-01-18 13:44:36.000000 netbox_textdatastore-0.0.4/netbox_textdatastore/filtersets.py
--rw-rw-rw-   0        0        0      954 2023-01-18 13:46:03.000000 netbox_textdatastore-0.0.4/netbox_textdatastore/forms.py
-drwxrwxrwx   0        0        0        0 2023-03-11 15:08:58.807149 netbox_textdatastore-0.0.4/netbox_textdatastore/migrations/
--rw-rw-rw-   0        0        0     1518 2023-01-18 13:48:28.000000 netbox_textdatastore-0.0.4/netbox_textdatastore/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2022-09-24 16:48:07.000000 netbox_textdatastore-0.0.4/netbox_textdatastore/migrations/__init__.py
--rw-rw-rw-   0        0        0      825 2023-03-11 15:08:20.000000 netbox_textdatastore-0.0.4/netbox_textdatastore/models.py
--rw-rw-rw-   0        0        0      189 2023-03-11 14:53:46.000000 netbox_textdatastore-0.0.4/netbox_textdatastore/navigation.py
--rw-rw-rw-   0        0        0      491 2023-01-18 13:45:59.000000 netbox_textdatastore-0.0.4/netbox_textdatastore/tables.py
--rw-rw-rw-   0        0        0      448 2023-01-18 13:46:36.000000 netbox_textdatastore-0.0.4/netbox_textdatastore/template_content.py
-drwxrwxrwx   0        0        0        0 2023-03-11 15:08:58.726402 netbox_textdatastore-0.0.4/netbox_textdatastore/templates/
-drwxrwxrwx   0        0        0        0 2023-03-11 15:08:58.811154 netbox_textdatastore-0.0.4/netbox_textdatastore/templates/netbox_textdatastore/
--rw-rw-rw-   0        0        0      182 2022-09-24 16:48:07.000000 netbox_textdatastore-0.0.4/netbox_textdatastore/templates/netbox_textdatastore/device_incl.html
--rw-rw-rw-   0        0        0     1335 2022-09-24 16:48:07.000000 netbox_textdatastore-0.0.4/netbox_textdatastore/templates/netbox_textdatastore/textdataobject.html
--rw-rw-rw-   0        0        0      818 2023-03-11 14:33:57.000000 netbox_textdatastore-0.0.4/netbox_textdatastore/urls.py
--rw-rw-rw-   0        0        0      706 2023-01-18 13:45:59.000000 netbox_textdatastore-0.0.4/netbox_textdatastore/views.py
-drwxrwxrwx   0        0        0        0 2023-03-11 15:08:58.794651 netbox_textdatastore-0.0.4/netbox_textdatastore.egg-info/
--rw-rw-rw-   0        0        0    11270 2023-03-11 15:08:58.000000 netbox_textdatastore-0.0.4/netbox_textdatastore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      892 2023-03-11 15:08:58.000000 netbox_textdatastore-0.0.4/netbox_textdatastore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-11 15:08:58.000000 netbox_textdatastore-0.0.4/netbox_textdatastore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-03-11 15:08:58.000000 netbox_textdatastore-0.0.4/netbox_textdatastore.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      671 2023-03-11 15:08:27.000000 netbox_textdatastore-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-11 15:08:58.816660 netbox_textdatastore-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-05 18:59:05.093707 netbox_textdatastore-0.0.5/
+-rw-rw-rw-   0        0        0     7169 2023-01-18 13:40:43.000000 netbox_textdatastore-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0       50 2023-01-18 17:12:49.000000 netbox_textdatastore-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0    11270 2024-04-05 18:59:05.091191 netbox_textdatastore-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2645 2023-01-18 17:10:24.000000 netbox_textdatastore-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-05 18:59:05.024816 netbox_textdatastore-0.0.5/netbox_textdatastore/
+-rw-rw-rw-   0        0        0      385 2023-01-18 13:44:51.000000 netbox_textdatastore-0.0.5/netbox_textdatastore/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 18:59:05.074092 netbox_textdatastore-0.0.5/netbox_textdatastore/api/
+-rw-rw-rw-   0        0        0        0 2022-09-24 16:48:07.000000 netbox_textdatastore-0.0.5/netbox_textdatastore/api/__init__.py
+-rw-rw-rw-   0        0        0      328 2023-01-18 13:45:59.000000 netbox_textdatastore-0.0.5/netbox_textdatastore/api/serializers.py
+-rw-rw-rw-   0        0        0      215 2023-01-18 13:47:57.000000 netbox_textdatastore-0.0.5/netbox_textdatastore/api/urls.py
+-rw-rw-rw-   0        0        0      374 2023-01-18 13:45:59.000000 netbox_textdatastore-0.0.5/netbox_textdatastore/api/views.py
+-rw-rw-rw-   0        0        0      638 2024-04-05 18:55:58.000000 netbox_textdatastore-0.0.5/netbox_textdatastore/filtersets.py
+-rw-rw-rw-   0        0        0      954 2023-01-18 13:46:03.000000 netbox_textdatastore-0.0.5/netbox_textdatastore/forms.py
+drwxrwxrwx   0        0        0        0 2024-04-05 18:59:05.078608 netbox_textdatastore-0.0.5/netbox_textdatastore/migrations/
+-rw-rw-rw-   0        0        0     1518 2023-01-18 13:48:28.000000 netbox_textdatastore-0.0.5/netbox_textdatastore/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2022-09-24 16:48:07.000000 netbox_textdatastore-0.0.5/netbox_textdatastore/migrations/__init__.py
+-rw-rw-rw-   0        0        0      825 2023-03-11 15:08:20.000000 netbox_textdatastore-0.0.5/netbox_textdatastore/models.py
+-rw-rw-rw-   0        0        0      189 2023-03-11 14:53:46.000000 netbox_textdatastore-0.0.5/netbox_textdatastore/navigation.py
+-rw-rw-rw-   0        0        0      491 2023-01-18 13:45:59.000000 netbox_textdatastore-0.0.5/netbox_textdatastore/tables.py
+-rw-rw-rw-   0        0        0      448 2023-01-18 13:46:36.000000 netbox_textdatastore-0.0.5/netbox_textdatastore/template_content.py
+drwxrwxrwx   0        0        0        0 2024-04-05 18:59:04.982464 netbox_textdatastore-0.0.5/netbox_textdatastore/templates/
+drwxrwxrwx   0        0        0        0 2024-04-05 18:59:05.085107 netbox_textdatastore-0.0.5/netbox_textdatastore/templates/netbox_textdatastore/
+-rw-rw-rw-   0        0        0      182 2022-09-24 16:48:07.000000 netbox_textdatastore-0.0.5/netbox_textdatastore/templates/netbox_textdatastore/device_incl.html
+-rw-rw-rw-   0        0        0     1335 2022-09-24 16:48:07.000000 netbox_textdatastore-0.0.5/netbox_textdatastore/templates/netbox_textdatastore/textdataobject.html
+-rw-rw-rw-   0        0        0      818 2023-03-11 14:33:57.000000 netbox_textdatastore-0.0.5/netbox_textdatastore/urls.py
+-rw-rw-rw-   0        0        0      706 2023-01-18 13:45:59.000000 netbox_textdatastore-0.0.5/netbox_textdatastore/views.py
+drwxrwxrwx   0        0        0        0 2024-04-05 18:59:05.089668 netbox_textdatastore-0.0.5/netbox_textdatastore.egg-info/
+-rw-rw-rw-   0        0        0    11270 2024-04-05 18:59:04.000000 netbox_textdatastore-0.0.5/netbox_textdatastore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      892 2024-04-05 18:59:04.000000 netbox_textdatastore-0.0.5/netbox_textdatastore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 18:59:04.000000 netbox_textdatastore-0.0.5/netbox_textdatastore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-04-05 18:59:04.000000 netbox_textdatastore-0.0.5/netbox_textdatastore.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      671 2024-04-05 18:58:19.000000 netbox_textdatastore-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-05 18:59:05.094208 netbox_textdatastore-0.0.5/setup.cfg
```

### Comparing `netbox_textdatastore-0.0.4/LICENSE` & `netbox_textdatastore-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_textdatastore-0.0.4/PKG-INFO` & `netbox_textdatastore-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox_textdatastore
-Version: 0.0.4
+Version: 0.0.5
 Summary: Netbox Plugin to store textfiles(e.g. configs) alongside devices
 Author-email: shrank <info@murxs.ch>
 License: Creative Commons Legal Code
         
         CC0 1.0 Universal
         
             CREATIVE COMMONS CORPORATION IS NOT A LAW FIRM AND DOES NOT PROVIDE
```

### Comparing `netbox_textdatastore-0.0.4/README.md` & `netbox_textdatastore-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `netbox_textdatastore-0.0.4/netbox_textdatastore/filtersets.py` & `netbox_textdatastore-0.0.5/netbox_textdatastore/filtersets.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,8 +14,8 @@
         queryset=Device.objects.all(),
         to_field_name='name',
         label='Device (name)',
     )
 
     class Meta:
         model = TextDataObject
-        fields = ['id', 'name', 'hash']
+        fields = ['id', 'name', 'hash','data']
```

### Comparing `netbox_textdatastore-0.0.4/netbox_textdatastore/forms.py` & `netbox_textdatastore-0.0.5/netbox_textdatastore/forms.py`

 * *Files identical despite different names*

### Comparing `netbox_textdatastore-0.0.4/netbox_textdatastore/migrations/0001_initial.py` & `netbox_textdatastore-0.0.5/netbox_textdatastore/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox_textdatastore-0.0.4/netbox_textdatastore/models.py` & `netbox_textdatastore-0.0.5/netbox_textdatastore/models.py`

 * *Files identical despite different names*

### Comparing `netbox_textdatastore-0.0.4/netbox_textdatastore/templates/netbox_textdatastore/textdataobject.html` & `netbox_textdatastore-0.0.5/netbox_textdatastore/templates/netbox_textdatastore/textdataobject.html`

 * *Files identical despite different names*

### Comparing `netbox_textdatastore-0.0.4/netbox_textdatastore/urls.py` & `netbox_textdatastore-0.0.5/netbox_textdatastore/urls.py`

 * *Files identical despite different names*

### Comparing `netbox_textdatastore-0.0.4/netbox_textdatastore/views.py` & `netbox_textdatastore-0.0.5/netbox_textdatastore/views.py`

 * *Files identical despite different names*

### Comparing `netbox_textdatastore-0.0.4/netbox_textdatastore.egg-info/PKG-INFO` & `netbox_textdatastore-0.0.5/netbox_textdatastore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: netbox-textdatastore
-Version: 0.0.4
+Name: netbox_textdatastore
+Version: 0.0.5
 Summary: Netbox Plugin to store textfiles(e.g. configs) alongside devices
 Author-email: shrank <info@murxs.ch>
 License: Creative Commons Legal Code
         
         CC0 1.0 Universal
         
             CREATIVE COMMONS CORPORATION IS NOT A LAW FIRM AND DOES NOT PROVIDE
```

### Comparing `netbox_textdatastore-0.0.4/netbox_textdatastore.egg-info/SOURCES.txt` & `netbox_textdatastore-0.0.5/netbox_textdatastore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netbox_textdatastore-0.0.4/pyproject.toml` & `netbox_textdatastore-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "netbox_textdatastore"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
     { name="shrank", email="info@murxs.ch" },
 ]
 license = { file = "LICENSE" }
 readme = "README.md"
 description = "Netbox Plugin to store textfiles(e.g. configs) alongside devices"
 requires-python = ">=3.0"
```

