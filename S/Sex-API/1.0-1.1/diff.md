# Comparing `tmp/Sex_API-1.0.tar.gz` & `tmp/Sex_API-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Sex_API-1.0.tar", last modified: Fri Apr  5 00:12:44 2024, max compression
+gzip compressed data, was "Sex_API-1.1.tar", last modified: Fri Apr  5 00:39:28 2024, max compression
```

## Comparing `Sex_API-1.0.tar` & `Sex_API-1.1.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-04-05 00:12:44.058442 Sex_API-1.0/
--rw-r--r--   0 asuna     (1000) asuna     (1000)     7369 2024-04-04 23:26:39.000000 Sex_API-1.0/LICENSE
--rw-r--r--   0 asuna     (1000) asuna     (1000)     2775 2024-04-05 00:12:44.058442 Sex_API-1.0/PKG-INFO
--rw-r--r--   0 asuna     (1000) asuna     (1000)     2300 2024-04-04 23:57:50.000000 Sex_API-1.0/README.md
-drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-04-05 00:12:44.058442 Sex_API-1.0/Sex_API.egg-info/
--rw-r--r--   0 asuna     (1000) asuna     (1000)     2775 2024-04-05 00:12:44.000000 Sex_API-1.0/Sex_API.egg-info/PKG-INFO
--rw-r--r--   0 asuna     (1000) asuna     (1000)      480 2024-04-05 00:12:44.000000 Sex_API-1.0/Sex_API.egg-info/SOURCES.txt
--rw-r--r--   0 asuna     (1000) asuna     (1000)        1 2024-04-05 00:12:44.000000 Sex_API-1.0/Sex_API.egg-info/dependency_links.txt
--rw-r--r--   0 asuna     (1000) asuna     (1000)       45 2024-04-05 00:12:44.000000 Sex_API-1.0/Sex_API.egg-info/entry_points.txt
--rw-r--r--   0 asuna     (1000) asuna     (1000)       22 2024-04-05 00:12:44.000000 Sex_API-1.0/Sex_API.egg-info/requires.txt
--rw-r--r--   0 asuna     (1000) asuna     (1000)        8 2024-04-05 00:12:44.000000 Sex_API-1.0/Sex_API.egg-info/top_level.txt
--rw-r--r--   0 asuna     (1000) asuna     (1000)       38 2024-04-05 00:12:44.058442 Sex_API-1.0/setup.cfg
--rw-r--r--   0 asuna     (1000) asuna     (1000)      788 2024-04-04 23:27:49.000000 Sex_API-1.0/setup.py
-drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-04-05 00:12:44.058442 Sex_API-1.0/sex_api/
--rw-r--r--   0 asuna     (1000) asuna     (1000)        0 2024-03-27 15:00:37.000000 Sex_API-1.0/sex_api/__init__.py
--rw-r--r--   0 asuna     (1000) asuna     (1000)    11205 2024-04-04 23:25:11.000000 Sex_API-1.0/sex_api/api.py
-drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-04-05 00:12:44.058442 Sex_API-1.0/sex_api/modules/
--rw-r--r--   0 asuna     (1000) asuna     (1000)        0 2024-03-27 15:00:23.000000 Sex_API-1.0/sex_api/modules/__init__.py
--rw-r--r--   0 asuna     (1000) asuna     (1000)     2566 2024-04-04 20:44:12.000000 Sex_API-1.0/sex_api/modules/consts.py
--rw-r--r--   0 asuna     (1000) asuna     (1000)       87 2024-03-27 15:00:20.000000 Sex_API-1.0/sex_api/modules/errors.py
--rw-r--r--   0 asuna     (1000) asuna     (1000)      180 2024-04-04 23:18:07.000000 Sex_API-1.0/sex_api/modules/searching_filters.py
-drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-04-05 00:12:44.058442 Sex_API-1.0/sex_api/tests/
--rw-r--r--   0 asuna     (1000) asuna     (1000)        0 2024-04-05 00:00:33.000000 Sex_API-1.0/sex_api/tests/__init__.py
--rw-r--r--   0 asuna     (1000) asuna     (1000)      598 2024-04-05 00:10:02.000000 Sex_API-1.0/sex_api/tests/test_board.py
--rw-r--r--   0 asuna     (1000) asuna     (1000)      436 2024-04-05 00:03:41.000000 Sex_API-1.0/sex_api/tests/test_pin.py
--rw-r--r--   0 asuna     (1000) asuna     (1000)     1058 2024-04-05 00:08:02.000000 Sex_API-1.0/sex_api/tests/test_user.py
+drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-04-05 00:39:28.232545 Sex_API-1.1/
+-rw-r--r--   0 asuna     (1000) asuna     (1000)     7369 2024-04-04 23:26:39.000000 Sex_API-1.1/LICENSE
+-rw-r--r--   0 asuna     (1000) asuna     (1000)     2775 2024-04-05 00:39:28.232545 Sex_API-1.1/PKG-INFO
+-rw-r--r--   0 asuna     (1000) asuna     (1000)     2300 2024-04-04 23:57:50.000000 Sex_API-1.1/README.md
+drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-04-05 00:39:28.232545 Sex_API-1.1/Sex_API.egg-info/
+-rw-r--r--   0 asuna     (1000) asuna     (1000)     2775 2024-04-05 00:39:28.000000 Sex_API-1.1/Sex_API.egg-info/PKG-INFO
+-rw-r--r--   0 asuna     (1000) asuna     (1000)      512 2024-04-05 00:39:28.000000 Sex_API-1.1/Sex_API.egg-info/SOURCES.txt
+-rw-r--r--   0 asuna     (1000) asuna     (1000)        1 2024-04-05 00:39:28.000000 Sex_API-1.1/Sex_API.egg-info/dependency_links.txt
+-rw-r--r--   0 asuna     (1000) asuna     (1000)       45 2024-04-05 00:39:28.000000 Sex_API-1.1/Sex_API.egg-info/entry_points.txt
+-rw-r--r--   0 asuna     (1000) asuna     (1000)       22 2024-04-05 00:39:28.000000 Sex_API-1.1/Sex_API.egg-info/requires.txt
+-rw-r--r--   0 asuna     (1000) asuna     (1000)        8 2024-04-05 00:39:28.000000 Sex_API-1.1/Sex_API.egg-info/top_level.txt
+-rw-r--r--   0 asuna     (1000) asuna     (1000)       38 2024-04-05 00:39:28.232545 Sex_API-1.1/setup.cfg
+-rw-r--r--   0 asuna     (1000) asuna     (1000)      788 2024-04-05 00:34:37.000000 Sex_API-1.1/setup.py
+drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-04-05 00:39:28.232545 Sex_API-1.1/sex_api/
+-rw-r--r--   0 asuna     (1000) asuna     (1000)        0 2024-03-27 15:00:37.000000 Sex_API-1.1/sex_api/__init__.py
+-rw-r--r--   0 asuna     (1000) asuna     (1000)    11752 2024-04-05 00:34:37.000000 Sex_API-1.1/sex_api/api.py
+drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-04-05 00:39:28.232545 Sex_API-1.1/sex_api/modules/
+-rw-r--r--   0 asuna     (1000) asuna     (1000)        0 2024-03-27 15:00:23.000000 Sex_API-1.1/sex_api/modules/__init__.py
+-rw-r--r--   0 asuna     (1000) asuna     (1000)     2668 2024-04-05 00:27:38.000000 Sex_API-1.1/sex_api/modules/consts.py
+-rw-r--r--   0 asuna     (1000) asuna     (1000)       87 2024-03-27 15:00:20.000000 Sex_API-1.1/sex_api/modules/errors.py
+-rw-r--r--   0 asuna     (1000) asuna     (1000)      211 2024-04-05 00:34:37.000000 Sex_API-1.1/sex_api/modules/searching_filters.py
+drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-04-05 00:39:28.232545 Sex_API-1.1/sex_api/tests/
+-rw-r--r--   0 asuna     (1000) asuna     (1000)        0 2024-04-05 00:00:33.000000 Sex_API-1.1/sex_api/tests/__init__.py
+-rw-r--r--   0 asuna     (1000) asuna     (1000)      598 2024-04-05 00:10:02.000000 Sex_API-1.1/sex_api/tests/test_board.py
+-rw-r--r--   0 asuna     (1000) asuna     (1000)      436 2024-04-05 00:03:41.000000 Sex_API-1.1/sex_api/tests/test_pin.py
+-rw-r--r--   0 asuna     (1000) asuna     (1000)      271 2024-04-05 00:32:51.000000 Sex_API-1.1/sex_api/tests/test_searching.py
+-rw-r--r--   0 asuna     (1000) asuna     (1000)     1058 2024-04-05 00:08:02.000000 Sex_API-1.1/sex_api/tests/test_user.py
```

### Comparing `Sex_API-1.0/LICENSE` & `Sex_API-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Sex_API-1.0/PKG-INFO` & `Sex_API-1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Sex_API
-Version: 1.0
+Version: 1.1
 Summary: A Python API for the Porn Site Sex.com/pins
 Home-page: https://github.com/EchterAlsFake/Sex_API
 Author: Johannes Habel
 Author-email: EchterAlsFake@proton.me
 License: LGPLv3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Sex_API Version: 1.0 Summary: A Python API for the
+Metadata-Version: 2.1 Name: Sex_API Version: 1.1 Summary: A Python API for the
 Porn Site Sex.com/pins Home-page: https://github.com/EchterAlsFake/Sex_API
 Author: Johannes Habel Author-email: EchterAlsFake@proton.me License: LGPLv3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3
 (LGPLv3) Classifier: Programming Language :: Python Description-Content-Type:
 text/markdown License-File: LICENSE Requires-Dist: requests Requires-Dist:
 eaf_base_api
                            ************ SSeexx..ccoomm AAPPII ************
```

### Comparing `Sex_API-1.0/README.md` & `Sex_API-1.1/README.md`

 * *Files identical despite different names*

### Comparing `Sex_API-1.0/Sex_API.egg-info/PKG-INFO` & `Sex_API-1.1/Sex_API.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Sex_API
-Version: 1.0
+Version: 1.1
 Summary: A Python API for the Porn Site Sex.com/pins
 Home-page: https://github.com/EchterAlsFake/Sex_API
 Author: Johannes Habel
 Author-email: EchterAlsFake@proton.me
 License: LGPLv3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Sex_API Version: 1.0 Summary: A Python API for the
+Metadata-Version: 2.1 Name: Sex_API Version: 1.1 Summary: A Python API for the
 Porn Site Sex.com/pins Home-page: https://github.com/EchterAlsFake/Sex_API
 Author: Johannes Habel Author-email: EchterAlsFake@proton.me License: LGPLv3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3
 (LGPLv3) Classifier: Programming Language :: Python Description-Content-Type:
 text/markdown License-File: LICENSE Requires-Dist: requests Requires-Dist:
 eaf_base_api
                            ************ SSeexx..ccoomm AAPPII ************
```

### Comparing `Sex_API-1.0/setup.py` & `Sex_API-1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="Sex_API",
-    version="1.0",
+    version="1.1",
     packages=find_packages(),
     install_requires=[
         "requests", "eaf_base_api"
     ],
     entry_points={
         'console_scripts': ['sex_api=sex_api.api:main'],
     },
```

### Comparing `Sex_API-1.0/sex_api/api.py` & `Sex_API-1.1/sex_api/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -290,29 +290,41 @@
         """
         :param url: (str) The URL of the Pin
         :return: (Pin) The Pin object which can be used to access the Pin and receive data from it and download it.
         """
         return Pin(url)
 
     @classmethod
-    def search(cls, query, sort_relevance: Relevance = Relevance.popular, mode: Mode = Mode.pics, pages: int = 5) -> Generator[Pin, None, None]:
+    def search(cls, query, sort_relevance: Relevance = Relevance.popular, mode: Mode = Mode.pics, pages: int = 5) -> Generator:
         """
         :param query: (str) The search query
         :param sort_relevance: (Relevance) The Relevance object (see searching_filters.py)
         :param mode: (Mode) The Mode object (see searching_filters.py)
         :param pages: (int) The page count (one page contains ~50-60 Pins)
         """
         query = query.replace(" ", "+")
 
         for page in range(1, pages):
-            content = Core().get_content(url=f"https://sex.com/search/{mode}?query={query}&sort={sort_relevance}&page={page}").decode("utf-8")
-            pins = regex_extract_pins.findall(content)
+            content = Core().get_content(url=f"https://sex.com/search/{mode}?query={query}{sort_relevance}&page={page}").decode("utf-8")
 
-            for pin in pins:
-                yield Pin(f"https://sex.com{pin}")
+            if mode == "pics" or mode == "gifs" or mode == "clips":
+                pins = regex_extract_pins.findall(content)
+
+                for pin in pins:
+                    yield Pin(f"https://sex.com{pin}")
+
+            elif mode == "users":
+                users = regex_get_users.findall(content)
+                for user in users:
+                    yield User(f"https://sex.com{user}")
+
+            elif mode == "boards":
+                boards = regex_get_boards.findall(content)
+                for board in boards:
+                    yield Board(f"https://sex.com{board}")
 
     @classmethod
     def get_user(cls, url) -> User:
         """
         :param url: (str) The URL of the User
         :return User: Returns the User object
         """
@@ -346,7 +358,13 @@
 
         for pin in pins:
             pin.download(path=args.output)
 
 
 if __name__ == "__main__":
     main()
+
+
+client = Client()
+search = client.search("Ai Porn", mode=Mode.pics)
+for pin in search:
+    print(pin.embed_url)
```

### Comparing `Sex_API-1.0/sex_api/modules/consts.py` & `Sex_API-1.1/sex_api/modules/consts.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 regex_description = re.compile(r'<div class="description">(.*?)</div>')
 regex_amount_boards = re.compile(r'">(.*?) Boards')
 regex_amount_following = re.compile(r'">(.*?) Following')
 regex_amount_pins = re.compile(r'/pins/">(.*?) Pins')
 regex_amount_repins = re.compile(r'">(.*?) Repins')
 regex_amount_likes = re.compile(r'">(.*?) Likes')
 regex_get_boards = re.compile(r'<a href="(.*?)/"><strong>')
+regex_get_users = re.compile(r'<div class="title"><a href="(.*?)"><i class="fa fa-user">', re.DOTALL)
 
 # Boards
 regex_follower_count = re.compile(r'<div class="followerCount">(.*?) followers</div>')
 regex_pin_count = re.compile(r'<div class="pinCount">(.*?) pins</div>')
 
 # Other
 regex_get_total_pages = re.compile(r'page=(.*?)" class="btn btn-default">')
```

#### html2text {}

```diff
@@ -28,13 +28,14 @@
 ((rr''hh11>>((..**??)) ************
 ') regex_description = re.compile(r'
 (.*?)
 ') regex_amount_boards = re.compile(r'">(.*?) Boards') regex_amount_following =
 re.compile(r'">(.*?) Following') regex_amount_pins = re.compile(r'/pins/">(.*?)
 Pins') regex_amount_repins = re.compile(r'">(.*?) Repins') regex_amount_likes =
 re.compile(r'">(.*?) Likes') regex_get_boards = re.compile(r'
-_''_))_ _##_ _BB_oo_aa_rr_dd_ss_ _rr_ee_gg_ee_xx____ff_oo_ll_ll_oo_ww_ee_rr____cc_oo_uu_nn_tt_ _==_ _rr_ee_.._cc_oo_mm_pp_ii_ll_ee_((_rr_''
+_''_))_ _rr_ee_gg_ee_xx____gg_ee_tt____uu_ss_ee_rr_ss_ _==_ _rr_ee_.._cc_oo_mm_pp_ii_ll_ee_((_rr_''
+_'_,_ _r_e_._D_O_T_A_L_L_)_ _#_ _B_o_a_r_d_s_ _r_e_g_e_x___f_o_l_l_o_w_e_r___c_o_u_n_t_ _=_ _r_e_._c_o_m_p_i_l_e_(_r_'
 _(_._*_?_)_ _f_o_l_l_o_w_e_r_s
 _'_)_ _r_e_g_e_x___p_i_n___c_o_u_n_t_ _=_ _r_e_._c_o_m_p_i_l_e_(_r_'
 _(_._*_?_)_ _p_i_n_s
 _'_)_ _#_ _O_t_h_e_r_ _r_e_g_e_x___g_e_t___t_o_t_a_l___p_a_g_e_s_ _=_ _r_e_._c_o_m_p_i_l_e_(_r_'_p_a_g_e_=_(_._*_?_)_"_ _c_l_a_s_s_=_"_b_t_n_ _b_t_n_-
 _d_e_f_a_u_l_t_"_>_'_)
```

### Comparing `Sex_API-1.0/sex_api/tests/test_board.py` & `Sex_API-1.1/sex_api/tests/test_board.py`

 * *Files identical despite different names*

### Comparing `Sex_API-1.0/sex_api/tests/test_user.py` & `Sex_API-1.1/sex_api/tests/test_user.py`

 * *Files identical despite different names*

