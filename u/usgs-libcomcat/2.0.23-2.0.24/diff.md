# Comparing `tmp/usgs-libcomcat-2.0.23.tar.gz` & `tmp/usgs-libcomcat-2.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usgs-libcomcat-2.0.23.tar", last modified: Wed Oct 25 19:24:29 2023, max compression
+gzip compressed data, was "usgs-libcomcat-2.0.24.tar", last modified: Fri Apr  5 17:52:35 2024, max compression
```

## Comparing `usgs-libcomcat-2.0.23.tar` & `usgs-libcomcat-2.0.24.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-10-25 19:24:29.111003 usgs-libcomcat-2.0.23/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2263 2023-10-25 18:33:21.000000 usgs-libcomcat-2.0.23/LICENSE.md
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)       51 2023-10-25 19:15:29.000000 usgs-libcomcat-2.0.23/MANIFEST.in
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)     8030 2023-10-25 19:24:29.111003 usgs-libcomcat-2.0.23/PKG-INFO
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3954 2023-10-25 18:33:21.000000 usgs-libcomcat-2.0.23/README.md
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1583 2023-10-25 19:15:29.000000 usgs-libcomcat-2.0.23/pyproject.toml
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)       38 2023-10-25 19:24:29.111003 usgs-libcomcat-2.0.23/setup.cfg
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-10-25 19:24:29.099003 usgs-libcomcat-2.0.23/src/
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-10-25 19:24:29.103003 usgs-libcomcat-2.0.23/src/libcomcat/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)       93 2023-10-25 18:33:21.000000 usgs-libcomcat-2.0.23/src/libcomcat/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    18456 2023-10-25 18:33:21.000000 usgs-libcomcat-2.0.23/src/libcomcat/_version.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-10-25 19:24:29.103003 usgs-libcomcat-2.0.23/src/libcomcat/bin/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-10-25 19:22:32.000000 usgs-libcomcat-2.0.23/src/libcomcat/bin/__init__.py
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     7957 2023-10-25 18:33:21.000000 usgs-libcomcat-2.0.23/src/libcomcat/bin/findid.py
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    19989 2023-10-25 18:33:21.000000 usgs-libcomcat-2.0.23/src/libcomcat/bin/getcsv.py
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    16608 2023-10-25 18:33:21.000000 usgs-libcomcat-2.0.23/src/libcomcat/bin/geteventhist.py
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     8607 2023-10-25 18:33:21.000000 usgs-libcomcat-2.0.23/src/libcomcat/bin/getmags.py
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    11005 2023-10-25 18:33:21.000000 usgs-libcomcat-2.0.23/src/libcomcat/bin/getpager.py
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    12388 2023-10-25 18:33:21.000000 usgs-libcomcat-2.0.23/src/libcomcat/bin/getphases.py
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    15973 2023-10-25 18:33:21.000000 usgs-libcomcat-2.0.23/src/libcomcat/bin/getproduct.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    42199 2023-10-25 18:33:21.000000 usgs-libcomcat-2.0.23/src/libcomcat/classes.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-10-25 19:24:29.107003 usgs-libcomcat-2.0.23/src/libcomcat/data/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   324036 2023-10-25 18:33:21.000000 usgs-libcomcat-2.0.23/src/libcomcat/data/economy.xml
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   214515 2023-10-25 18:33:21.000000 usgs-libcomcat-2.0.23/src/libcomcat/data/fatality.xml
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        5 2023-10-25 18:33:21.000000 usgs-libcomcat-2.0.23/src/libcomcat/data/ne_50m_admin_0_countries.cpg
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)   546979 2023-10-25 18:33:21.000000 usgs-libcomcat-2.0.23/src/libcomcat/data/ne_50m_admin_0_countries.dbf
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)      143 2023-10-25 18:33:21.000000 usgs-libcomcat-2.0.23/src/libcomcat/data/ne_50m_admin_0_countries.prj
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)  1612740 2023-10-25 18:33:21.000000 usgs-libcomcat-2.0.23/src/libcomcat/data/ne_50m_admin_0_countries.shp
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     2028 2023-10-25 18:33:21.000000 usgs-libcomcat-2.0.23/src/libcomcat/data/ne_50m_admin_0_countries.shx
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    76028 2023-10-25 18:33:21.000000 usgs-libcomcat-2.0.23/src/libcomcat/dataframes.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      864 2023-10-25 18:33:21.000000 usgs-libcomcat-2.0.23/src/libcomcat/exceptions.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2278 2023-10-25 18:33:21.000000 usgs-libcomcat-2.0.23/src/libcomcat/logging.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    25810 2023-10-25 18:33:21.000000 usgs-libcomcat-2.0.23/src/libcomcat/search.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      327 2023-10-25 18:33:21.000000 usgs-libcomcat-2.0.23/src/libcomcat/test_utils.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    11702 2023-10-25 18:33:21.000000 usgs-libcomcat-2.0.23/src/libcomcat/utils.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-10-25 19:24:29.107003 usgs-libcomcat-2.0.23/src/usgs_libcomcat.egg-info/
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)     8030 2023-10-25 19:24:29.000000 usgs-libcomcat-2.0.23/src/usgs_libcomcat.egg-info/PKG-INFO
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)     1079 2023-10-25 19:24:29.000000 usgs-libcomcat-2.0.23/src/usgs_libcomcat.egg-info/SOURCES.txt
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)        1 2023-10-25 19:24:29.000000 usgs-libcomcat-2.0.23/src/usgs_libcomcat.egg-info/dependency_links.txt
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)      295 2023-10-25 19:24:29.000000 usgs-libcomcat-2.0.23/src/usgs_libcomcat.egg-info/entry_points.txt
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)      380 2023-10-25 19:24:29.000000 usgs-libcomcat-2.0.23/src/usgs_libcomcat.egg-info/requires.txt
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)       15 2023-10-25 19:24:29.000000 usgs-libcomcat-2.0.23/src/usgs_libcomcat.egg-info/top_level.txt
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-05 17:52:35.918095 usgs-libcomcat-2.0.24/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2263 2024-04-05 17:33:03.000000 usgs-libcomcat-2.0.24/LICENSE.md
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)       51 2024-04-05 17:33:03.000000 usgs-libcomcat-2.0.24/MANIFEST.in
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)     8030 2024-04-05 17:52:35.918095 usgs-libcomcat-2.0.24/PKG-INFO
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3954 2024-04-05 17:33:03.000000 usgs-libcomcat-2.0.24/README.md
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1583 2024-04-05 17:33:03.000000 usgs-libcomcat-2.0.24/pyproject.toml
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)       38 2024-04-05 17:52:35.918095 usgs-libcomcat-2.0.24/setup.cfg
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-05 17:52:35.906095 usgs-libcomcat-2.0.24/src/
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-05 17:52:35.910095 usgs-libcomcat-2.0.24/src/libcomcat/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)       93 2024-04-05 17:33:03.000000 usgs-libcomcat-2.0.24/src/libcomcat/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    18456 2024-04-05 17:33:03.000000 usgs-libcomcat-2.0.24/src/libcomcat/_version.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-05 17:52:35.910095 usgs-libcomcat-2.0.24/src/libcomcat/bin/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-04-05 17:51:21.000000 usgs-libcomcat-2.0.24/src/libcomcat/bin/__init__.py
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     7957 2024-04-05 17:33:03.000000 usgs-libcomcat-2.0.24/src/libcomcat/bin/findid.py
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    19989 2024-04-05 17:33:03.000000 usgs-libcomcat-2.0.24/src/libcomcat/bin/getcsv.py
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    16608 2024-04-05 17:33:03.000000 usgs-libcomcat-2.0.24/src/libcomcat/bin/geteventhist.py
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     8607 2024-04-05 17:33:03.000000 usgs-libcomcat-2.0.24/src/libcomcat/bin/getmags.py
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    11005 2024-04-05 17:33:03.000000 usgs-libcomcat-2.0.24/src/libcomcat/bin/getpager.py
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    12388 2024-04-05 17:33:03.000000 usgs-libcomcat-2.0.24/src/libcomcat/bin/getphases.py
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    15973 2024-04-05 17:33:03.000000 usgs-libcomcat-2.0.24/src/libcomcat/bin/getproduct.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    42526 2024-04-05 17:33:03.000000 usgs-libcomcat-2.0.24/src/libcomcat/classes.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-05 17:52:35.914095 usgs-libcomcat-2.0.24/src/libcomcat/data/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   324036 2024-04-05 17:33:03.000000 usgs-libcomcat-2.0.24/src/libcomcat/data/economy.xml
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   214515 2024-04-05 17:33:03.000000 usgs-libcomcat-2.0.24/src/libcomcat/data/fatality.xml
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        5 2024-04-05 17:33:03.000000 usgs-libcomcat-2.0.24/src/libcomcat/data/ne_50m_admin_0_countries.cpg
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)   546979 2024-04-05 17:33:03.000000 usgs-libcomcat-2.0.24/src/libcomcat/data/ne_50m_admin_0_countries.dbf
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)      143 2024-04-05 17:33:03.000000 usgs-libcomcat-2.0.24/src/libcomcat/data/ne_50m_admin_0_countries.prj
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)  1612740 2024-04-05 17:33:03.000000 usgs-libcomcat-2.0.24/src/libcomcat/data/ne_50m_admin_0_countries.shp
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     2028 2024-04-05 17:33:03.000000 usgs-libcomcat-2.0.24/src/libcomcat/data/ne_50m_admin_0_countries.shx
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    76040 2024-04-05 17:33:03.000000 usgs-libcomcat-2.0.24/src/libcomcat/dataframes.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      864 2024-04-05 17:33:03.000000 usgs-libcomcat-2.0.24/src/libcomcat/exceptions.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2278 2024-04-05 17:33:03.000000 usgs-libcomcat-2.0.24/src/libcomcat/logging.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    25810 2024-04-05 17:33:03.000000 usgs-libcomcat-2.0.24/src/libcomcat/search.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      327 2024-04-05 17:33:03.000000 usgs-libcomcat-2.0.24/src/libcomcat/test_utils.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    11702 2024-04-05 17:33:03.000000 usgs-libcomcat-2.0.24/src/libcomcat/utils.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-05 17:52:35.918095 usgs-libcomcat-2.0.24/src/usgs_libcomcat.egg-info/
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)     8030 2024-04-05 17:52:35.000000 usgs-libcomcat-2.0.24/src/usgs_libcomcat.egg-info/PKG-INFO
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)     1079 2024-04-05 17:52:35.000000 usgs-libcomcat-2.0.24/src/usgs_libcomcat.egg-info/SOURCES.txt
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)        1 2024-04-05 17:52:35.000000 usgs-libcomcat-2.0.24/src/usgs_libcomcat.egg-info/dependency_links.txt
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)      295 2024-04-05 17:52:35.000000 usgs-libcomcat-2.0.24/src/usgs_libcomcat.egg-info/entry_points.txt
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)      380 2024-04-05 17:52:35.000000 usgs-libcomcat-2.0.24/src/usgs_libcomcat.egg-info/requires.txt
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)       15 2024-04-05 17:52:35.000000 usgs-libcomcat-2.0.24/src/usgs_libcomcat.egg-info/top_level.txt
```

### Comparing `usgs-libcomcat-2.0.23/LICENSE.md` & `usgs-libcomcat-2.0.24/LICENSE.md`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.23/PKG-INFO` & `usgs-libcomcat-2.0.24/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usgs-libcomcat
-Version: 2.0.23
+Version: 2.0.24
 Summary: Python wrapper around ComCat web API
 Author-email: Mike Hearne <mhearne@usgs.gov>, Heather Hunsinger <hhunsinger@usgs.gov>
 License: License
         =======
         
         Unless otherwise noted, This project is in the public domain in the United
         States because it contains materials that originally came from the United
```

### Comparing `usgs-libcomcat-2.0.23/README.md` & `usgs-libcomcat-2.0.24/README.md`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.23/pyproject.toml` & `usgs-libcomcat-2.0.24/pyproject.toml`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.23/src/libcomcat/_version.py` & `usgs-libcomcat-2.0.24/src/libcomcat/_version.py`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.23/src/libcomcat/bin/findid.py` & `usgs-libcomcat-2.0.24/src/libcomcat/bin/findid.py`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.23/src/libcomcat/bin/getcsv.py` & `usgs-libcomcat-2.0.24/src/libcomcat/bin/getcsv.py`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.23/src/libcomcat/bin/geteventhist.py` & `usgs-libcomcat-2.0.24/src/libcomcat/bin/geteventhist.py`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.23/src/libcomcat/bin/getmags.py` & `usgs-libcomcat-2.0.24/src/libcomcat/bin/getmags.py`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.23/src/libcomcat/bin/getpager.py` & `usgs-libcomcat-2.0.24/src/libcomcat/bin/getpager.py`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.23/src/libcomcat/bin/getphases.py` & `usgs-libcomcat-2.0.24/src/libcomcat/bin/getphases.py`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.23/src/libcomcat/bin/getproduct.py` & `usgs-libcomcat-2.0.24/src/libcomcat/bin/getproduct.py`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.23/src/libcomcat/classes.py` & `usgs-libcomcat-2.0.24/src/libcomcat/classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -799,15 +799,21 @@
         # first sort the dataframe by source and then time
         psources = df["source"].unique()
         newframe = pd.DataFrame(columns=df.columns.to_list() + ["version"])
         for psource in psources:
             dft = df[df["source"] == psource]
             dft = dft.sort_values("time")
             dft["version"] = np.arange(1, len(dft) + 1)
-            newframe = pd.concat([newframe, dft])
+            newframe = (
+                newframe.copy()
+                if dft.empty
+                else (
+                    dft.copy() if newframe.empty else pd.concat([newframe, dft])
+                )  # if both DataFrames non empty
+            )
         df = newframe
 
         if source == "preferred":
             idx = weights.index(max(weights))
             tproduct = self._jdict["properties"]["products"][product_name][idx]
             prefsource = tproduct["source"]
             df = df[df["source"] == prefsource]
@@ -1030,14 +1036,17 @@
                 after two tries.
         """
         content_name = "a" * 1000
         content_url = None
         for contentkey, content in self._product["contents"].items():
             if re.search(regexp + "$", contentkey) is None:
                 continue
+            if "url" not in content.keys() and "bytes" in content.keys():
+                return (content["bytes"], None)
+
             url = content["url"]
             parts = urlparse(url)
             fname = parts.path.split("/")[-1]
             if len(fname) < len(content_name):
                 content_name = fname
                 content_url = url
         if content_url is None:
```

### Comparing `usgs-libcomcat-2.0.23/src/libcomcat/data/economy.xml` & `usgs-libcomcat-2.0.24/src/libcomcat/data/economy.xml`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.23/src/libcomcat/data/fatality.xml` & `usgs-libcomcat-2.0.24/src/libcomcat/data/fatality.xml`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.23/src/libcomcat/data/ne_50m_admin_0_countries.dbf` & `usgs-libcomcat-2.0.24/src/libcomcat/data/ne_50m_admin_0_countries.dbf`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.23/src/libcomcat/data/ne_50m_admin_0_countries.shp` & `usgs-libcomcat-2.0.24/src/libcomcat/data/ne_50m_admin_0_countries.shp`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.23/src/libcomcat/data/ne_50m_admin_0_countries.shx` & `usgs-libcomcat-2.0.24/src/libcomcat/data/ne_50m_admin_0_countries.shx`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.23/src/libcomcat/dataframes.py` & `usgs-libcomcat-2.0.24/src/libcomcat/dataframes.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     "No. of responses": "nresp",
     "Hypocentral distance": "distance",
     "Epicentral distance": "distance",
     "ZIP/Location": "station",
 }
 
 MIN_API_TIME = (
-    0.7  # required number of seconds between calls (with a little safety factor)
+    0.9  # required number of seconds between calls (with a little safety factor)
 )
 
 PRODUCT_COLUMNS = [
     "Update Time",
     "Product",
     "Authoritative Event ID",
     "Code",
@@ -1236,15 +1236,15 @@
         ndyfi = 0
         if len(product.getContentsMatching("stationlist.json")):
             stationbytes = product.getContentBytes("stationlist.json")[0]
             stationdict = json.loads(stationbytes.decode("utf-8"))
             ninstrument = 0
             ndyfi = 0
             for feature in stationdict["features"]:
-                if feature["properties"]["source"] == "DYFI":
+                if feature["properties"]["instrumentType"] == "OBSERVED":
                     ndyfi += 1
                 else:
                     ninstrument += 1
     elif len(product.getContentsMatching("info.xml")):
         infobytes = product.getContentBytes("info.xml")[0]
         root = minidom.parseString(infobytes.decode("utf-8"))
         fault_ref = ""
```

### Comparing `usgs-libcomcat-2.0.23/src/libcomcat/exceptions.py` & `usgs-libcomcat-2.0.24/src/libcomcat/exceptions.py`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.23/src/libcomcat/logging.py` & `usgs-libcomcat-2.0.24/src/libcomcat/logging.py`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.23/src/libcomcat/search.py` & `usgs-libcomcat-2.0.24/src/libcomcat/search.py`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.23/src/libcomcat/utils.py` & `usgs-libcomcat-2.0.24/src/libcomcat/utils.py`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.23/src/usgs_libcomcat.egg-info/PKG-INFO` & `usgs-libcomcat-2.0.24/src/usgs_libcomcat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usgs-libcomcat
-Version: 2.0.23
+Version: 2.0.24
 Summary: Python wrapper around ComCat web API
 Author-email: Mike Hearne <mhearne@usgs.gov>, Heather Hunsinger <hhunsinger@usgs.gov>
 License: License
         =======
         
         Unless otherwise noted, This project is in the public domain in the United
         States because it contains materials that originally came from the United
```

### Comparing `usgs-libcomcat-2.0.23/src/usgs_libcomcat.egg-info/SOURCES.txt` & `usgs-libcomcat-2.0.24/src/usgs_libcomcat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

