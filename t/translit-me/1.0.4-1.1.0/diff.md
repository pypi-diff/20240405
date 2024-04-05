# Comparing `tmp/translit_me-1.0.4.tar.gz` & `tmp/translit_me-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "translit_me-1.0.4.tar", last modified: Wed Dec 21 09:25:55 2022, max compression
+gzip compressed data, was "translit_me-1.1.0.tar", last modified: Fri Apr  5 11:58:09 2024, max compression
```

## Comparing `translit_me-1.0.4.tar` & `translit_me-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2022-12-21 09:25:55.856269 translit_me-1.0.4/
--rw-rw-rw-   0        0        0      603 2022-11-02 14:34:22.000000 translit_me-1.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0     3361 2022-12-21 09:25:55.855275 translit_me-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2716 2022-11-03 08:49:23.000000 translit_me-1.0.4/README.md
--rw-rw-rw-   0        0        0      990 2022-12-21 09:25:12.000000 translit_me-1.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-12-21 09:25:55.856269 translit_me-1.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-12-21 09:25:55.804945 translit_me-1.0.4/translit_me/
--rw-rw-rw-   0        0        0        0 2022-09-01 08:28:12.000000 translit_me-1.0.4/translit_me/__init__.py
--rw-rw-rw-   0        0        0     5944 2022-12-21 09:15:30.000000 translit_me-1.0.4/translit_me/lang_tables.py
--rw-rw-rw-   0        0        0     1564 2022-10-26 07:09:49.000000 translit_me-1.0.4/translit_me/main.py
-drwxrwxrwx   0        0        0        0 2022-12-21 09:25:55.853741 translit_me-1.0.4/translit_me/tests/
--rw-rw-rw-   0        0        0      622 2022-09-05 12:17:29.000000 translit_me-1.0.4/translit_me/tests/testCharTrie.py
--rw-rw-rw-   0        0        0     1183 2022-11-02 14:30:31.000000 translit_me-1.0.4/translit_me/tests/test_remove_vowels.py
--rw-rw-rw-   0        0        0     2382 2022-12-21 09:15:51.000000 translit_me-1.0.4/translit_me/tests/test_transliterate.py
--rw-rw-rw-   0        0        0     5866 2022-12-15 11:43:56.000000 translit_me-1.0.4/translit_me/transliterator.py
-drwxrwxrwx   0        0        0        0 2022-12-21 09:25:55.829944 translit_me-1.0.4/translit_me.egg-info/
--rw-rw-rw-   0        0        0     3361 2022-12-21 09:25:55.000000 translit_me-1.0.4/translit_me.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      391 2022-12-21 09:25:55.000000 translit_me-1.0.4/translit_me.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-21 09:25:55.000000 translit_me-1.0.4/translit_me.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2022-12-21 09:25:55.000000 translit_me-1.0.4/translit_me.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 11:58:09.867502 translit_me-1.1.0/
+-rw-rw-rw-   0        0        0      603 2022-11-02 14:34:22.000000 translit_me-1.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     3361 2024-04-05 11:58:09.865499 translit_me-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2716 2022-11-03 08:49:23.000000 translit_me-1.1.0/README.md
+-rw-rw-rw-   0        0        0      990 2024-04-05 11:50:55.000000 translit_me-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-05 11:58:09.868501 translit_me-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-05 11:58:09.780266 translit_me-1.1.0/translit_me/
+-rw-rw-rw-   0        0        0        0 2022-09-01 08:28:12.000000 translit_me-1.1.0/translit_me/__init__.py
+-rw-rw-rw-   0        0        0     7556 2024-04-05 08:50:03.000000 translit_me-1.1.0/translit_me/lang_tables.py
+-rw-rw-rw-   0        0        0     1585 2024-04-04 07:27:08.000000 translit_me-1.1.0/translit_me/main.py
+drwxrwxrwx   0        0        0        0 2024-04-05 11:58:09.860754 translit_me-1.1.0/translit_me/tests/
+-rw-rw-rw-   0        0        0      622 2022-09-05 12:17:29.000000 translit_me-1.1.0/translit_me/tests/testCharTrie.py
+-rw-rw-rw-   0        0        0     1183 2022-11-02 14:30:31.000000 translit_me-1.1.0/translit_me/tests/test_remove_vowels.py
+-rw-rw-rw-   0        0        0     2844 2024-04-05 08:49:18.000000 translit_me-1.1.0/translit_me/tests/test_transliterate.py
+-rw-rw-rw-   0        0        0     6548 2024-04-04 18:59:57.000000 translit_me-1.1.0/translit_me/transliterator.py
+drwxrwxrwx   0        0        0        0 2024-04-05 11:58:09.863486 translit_me-1.1.0/translit_me.egg-info/
+-rw-rw-rw-   0        0        0     3361 2024-04-05 11:58:09.000000 translit_me-1.1.0/translit_me.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      391 2024-04-05 11:58:09.000000 translit_me-1.1.0/translit_me.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 11:58:09.000000 translit_me-1.1.0/translit_me.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-04-05 11:58:09.000000 translit_me-1.1.0/translit_me.egg-info/top_level.txt
```

### Comparing `translit_me-1.0.4/LICENSE.txt` & `translit_me-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `translit_me-1.0.4/PKG-INFO` & `translit_me-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: translit_me
-Version: 1.0.4
+Version: 1.1.0
 Summary: A transliteration service for Middle-Eastern languages. 
 Author-email: Tomer Sagi <tsagi@cs.aau.dk>, Sinai Rusinek <sinai.rusinek@mail.huji.ac.il>, Moran Zaga <mzaga@Staff.haifa.ac.il>
 Project-URL: Homepage, https://mehdie.org/
 Project-URL: Bug Tracker, https://gitlab.com/m8417/hebrew-transliteration-service/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `translit_me-1.0.4/README.md` & `translit_me-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `translit_me-1.0.4/pyproject.toml` & `translit_me-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "uvicorn~=0.18.2", "fastapi~=0.78.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "translit_me"
-version = "1.0.4"
+version = "1.1.0"
 authors = [
   { name="Tomer Sagi", email="tsagi@cs.aau.dk" }, { name="Sinai Rusinek", email="sinai.rusinek@mail.huji.ac.il" },
     { name="Moran Zaga", email="mzaga@Staff.haifa.ac.il" }
 ]
 description = "A transliteration service for Middle-Eastern languages. \n The service was developed as part of the MEHDIE project- https://mehdie.org/. \n MEHDIE is funded by the Israel Ministry of Science and Technology (MOST)."
 
 readme = "README.md"
```

### Comparing `translit_me-1.0.4/translit_me/main.py` & `translit_me-1.1.0/translit_me/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from fastapi import FastAPI, Request, Response
 
 from transliterator import transliterate, remove_vowels as rv
 from lang_tables import *
 
 app = FastAPI()
 
-lang_tables = {('he', 'ar'): HE_AR, ('ar', 'he'): AR_HE, ('he', 'en'): HE_EN, ('ar', 'en'): AR_EN}
+lang_tables = {('he', 'ar'): HE_AR, ('ar', 'he'): AR_HE, ('he', 'en'): HE_EN, ('ar', 'en'): AR_EN, ('de', 'he'): DE_HE}
 
 
 @app.post("/")
 async def home(request: Request):
     body = await request.json()
     # ToDo tests input for type list
     # ToDo tests input for language
```

### Comparing `translit_me-1.0.4/translit_me/tests/testCharTrie.py` & `translit_me-1.1.0/translit_me/tests/testCharTrie.py`

 * *Files identical despite different names*

### Comparing `translit_me-1.0.4/translit_me/tests/test_remove_vowels.py` & `translit_me-1.1.0/translit_me/tests/test_remove_vowels.py`

 * *Files identical despite different names*

### Comparing `translit_me-1.0.4/translit_me/tests/test_transliterate.py` & `translit_me-1.1.0/translit_me/tests/test_transliterate.py`

 * *Files 10% similar despite different names*

```diff
@@ -43,10 +43,24 @@
     def test_multi_word(self):
         names = ['כפר סבא', 'כפר סבא רבא', 'בן פורד יוסף']
         expected = ['كفر سبا', 'كفر سبا ربا', 'بن فورد يوسف', 'بن فورض يوسف']
         res = tr(names, HE_AR)
         print(res)
         self.assertListEqual(res, expected)
 
+    def test_de_he(self):
+        names = ['Ytzchak Neufeld', 'Deutschkreutz']
+        expected = ['וצחק נופלד', 'דויטשקרויץ']
+        res = tr(names, DE_HE)
+        print(res)
+        self.assertListEqual(res, expected)
+
+    def test_for_whg(self):
+        def he_en(name, conversion):
+            return tr([name], conversion)
+
+        t = he_en("שמורות הפנדה הענק בסצ'ואן", HE_EN)
+        len(t)  # 4608
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `translit_me-1.0.4/translit_me/transliterator.py` & `translit_me-1.1.0/translit_me/transliterator.py`

 * *Files 14% similar despite different names*

```diff
@@ -93,24 +93,38 @@
 def transliterate_word(name: str, table):
     new_name_trie = CharTrie()
     skip = 0
     for i in range(len(name)):  # ToDo split words on spaces
         if skip > 0:  # need to skip one or more characters due to character combinations
             skip -= 1
             continue
-        if name[i: i + 3] in table.keys() and i + 2 < len(name):
+        if name[i: i + 4] in table.keys() and i + 3 < len(name):
+            to_add = table[name[i: i + 4]]
+            if callable(to_add):  # resolved by a function
+                to_add = table[name[i:i+4]](name, i)
+            if type(to_add) is list:
+                new_name_trie.split(to_add)
+            else:
+                new_name_trie.add(to_add)
+            # if callable(to_add): # resolved by a function
+            skip = 3
+        elif name[i: i + 3] in table.keys() and i + 2 < len(name):
             to_add = table[name[i: i + 3]]
+            if callable(to_add):  # resolved by a function
+                to_add = table[name[i:i+3]](name, i)
             if type(to_add) is list:
                 new_name_trie.split(to_add)
             else:
                 new_name_trie.add(to_add)
             # if callable(to_add): # resolved by a function
             skip = 2
         elif name[i: i + 2] in table.keys() and i + 1 < len(name):
             to_add = table[name[i: i + 2]]
+            if callable(to_add):  # resolved by a function
+                to_add = table[name[i:i+2]](name, i)
             if type(to_add) is list:
                 new_name_trie.split(to_add)
             else:
                 new_name_trie.add(to_add)
             skip = 1
         elif name[i] in table.keys():
             to_add = table[name[i]]
```

### Comparing `translit_me-1.0.4/translit_me.egg-info/PKG-INFO` & `translit_me-1.1.0/translit_me.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: translit-me
-Version: 1.0.4
+Name: translit_me
+Version: 1.1.0
 Summary: A transliteration service for Middle-Eastern languages. 
 Author-email: Tomer Sagi <tsagi@cs.aau.dk>, Sinai Rusinek <sinai.rusinek@mail.huji.ac.il>, Moran Zaga <mzaga@Staff.haifa.ac.il>
 Project-URL: Homepage, https://mehdie.org/
 Project-URL: Bug Tracker, https://gitlab.com/m8417/hebrew-transliteration-service/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

