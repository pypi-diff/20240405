# Comparing `tmp/contentstack_utils-1.2.3.tar.gz` & `tmp/contentstack_utils-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contentstack_utils-1.2.3.tar", last modified: Thu Feb 29 05:30:54 2024, max compression
+gzip compressed data, was "contentstack_utils-1.3.0.tar", last modified: Fri Apr  5 13:15:53 2024, max compression
```

## Comparing `contentstack_utils-1.2.3.tar` & `contentstack_utils-1.3.0.tar`

### file list

```diff
@@ -1,23 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 05:30:54.726466 contentstack_utils-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-02-29 05:30:46.000000 contentstack_utils-1.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-02-29 05:30:54.726466 contentstack_utils-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4166 2024-02-29 05:30:46.000000 contentstack_utils-1.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 05:30:54.726466 contentstack_utils-1.2.3/contentstack_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-02-29 05:30:54.000000 contentstack_utils-1.2.3/contentstack_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-02-29 05:30:54.000000 contentstack_utils-1.2.3/contentstack_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 05:30:54.000000 contentstack_utils-1.2.3/contentstack_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 05:30:54.000000 contentstack_utils-1.2.3/contentstack_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-29 05:30:54.726466 contentstack_utils-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-02-29 05:30:46.000000 contentstack_utils-1.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 05:30:54.722466 contentstack_utils-1.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-02-29 05:30:46.000000 contentstack_utils-1.2.3/tests/test_default_opt_others.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-02-29 05:30:46.000000 contentstack_utils-1.2.3/tests/test_gql_to_html_func.py
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-02-29 05:30:46.000000 contentstack_utils-1.2.3/tests/test_helper_node_to_html.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-02-29 05:30:46.000000 contentstack_utils-1.2.3/tests/test_item_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-02-29 05:30:46.000000 contentstack_utils-1.2.3/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-02-29 05:30:46.000000 contentstack_utils-1.2.3/tests/test_option_render_mark.py
--rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-02-29 05:30:46.000000 contentstack_utils-1.2.3/tests/test_render_default_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-02-29 05:30:46.000000 contentstack_utils-1.2.3/tests/test_render_options.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-02-29 05:30:46.000000 contentstack_utils-1.2.3/tests/test_style_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     5439 2024-02-29 05:30:46.000000 contentstack_utils-1.2.3/tests/test_util_srte.py
--rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-02-29 05:30:46.000000 contentstack_utils-1.2.3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:15:53.332076 contentstack_utils-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-05 13:15:45.000000 contentstack_utils-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-04-05 13:15:53.332076 contentstack_utils-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4166 2024-04-05 13:15:45.000000 contentstack_utils-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:15:53.328076 contentstack_utils-1.3.0/contentstack_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-05 13:15:45.000000 contentstack_utils-1.3.0/contentstack_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7389 2024-04-05 13:15:45.000000 contentstack_utils-1.3.0/contentstack_utils/automate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:15:53.332076 contentstack_utils-1.3.0/contentstack_utils/embedded/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-05 13:15:45.000000 contentstack_utils-1.3.0/contentstack_utils/embedded/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-05 13:15:45.000000 contentstack_utils-1.3.0/contentstack_utils/embedded/item_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-05 13:15:45.000000 contentstack_utils-1.3.0/contentstack_utils/embedded/styletype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-05 13:15:45.000000 contentstack_utils-1.3.0/contentstack_utils/gql.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:15:53.332076 contentstack_utils-1.3.0/contentstack_utils/helper/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-05 13:15:45.000000 contentstack_utils-1.3.0/contentstack_utils/helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-05 13:15:45.000000 contentstack_utils-1.3.0/contentstack_utils/helper/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-05 13:15:45.000000 contentstack_utils-1.3.0/contentstack_utils/helper/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-05 13:15:45.000000 contentstack_utils-1.3.0/contentstack_utils/helper/node_to_html.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:15:53.332076 contentstack_utils-1.3.0/contentstack_utils/render/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-05 13:15:45.000000 contentstack_utils-1.3.0/contentstack_utils/render/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-04-05 13:15:45.000000 contentstack_utils-1.3.0/contentstack_utils/render/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-04-05 13:15:45.000000 contentstack_utils-1.3.0/contentstack_utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:15:53.332076 contentstack_utils-1.3.0/contentstack_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-04-05 13:15:53.000000 contentstack_utils-1.3.0/contentstack_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-05 13:15:53.000000 contentstack_utils-1.3.0/contentstack_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 13:15:53.000000 contentstack_utils-1.3.0/contentstack_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-05 13:15:53.000000 contentstack_utils-1.3.0/contentstack_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 13:15:53.332076 contentstack_utils-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-05 13:15:45.000000 contentstack_utils-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:15:53.332076 contentstack_utils-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-05 13:15:45.000000 contentstack_utils-1.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-05 13:15:45.000000 contentstack_utils-1.3.0/tests/convert_style.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-04-05 13:15:45.000000 contentstack_utils-1.3.0/tests/test_default_opt_others.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-05 13:15:45.000000 contentstack_utils-1.3.0/tests/test_gql_to_html_func.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-04-05 13:15:45.000000 contentstack_utils-1.3.0/tests/test_helper_node_to_html.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-05 13:15:45.000000 contentstack_utils-1.3.0/tests/test_item_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-05 13:15:45.000000 contentstack_utils-1.3.0/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-04-05 13:15:45.000000 contentstack_utils-1.3.0/tests/test_option_render_mark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-04-05 13:15:45.000000 contentstack_utils-1.3.0/tests/test_render_default_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-05 13:15:45.000000 contentstack_utils-1.3.0/tests/test_render_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-05 13:15:45.000000 contentstack_utils-1.3.0/tests/test_style_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5951 2024-04-05 13:15:45.000000 contentstack_utils-1.3.0/tests/test_util_srte.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-04-05 13:15:45.000000 contentstack_utils-1.3.0/tests/test_utils.py
```

### Comparing `contentstack_utils-1.2.3/LICENSE` & `contentstack_utils-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `contentstack_utils-1.2.3/PKG-INFO` & `contentstack_utils-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contentstack_utils
-Version: 1.2.3
+Version: 1.3.0
 Summary: contentstack_utils is a Utility package for Contentstack headless CMS with an API-first approach.
 Home-page: https://github.com/contentstack/contentstack-utils-python
 Author: contentstack
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
```

### Comparing `contentstack_utils-1.2.3/README.md` & `contentstack_utils-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `contentstack_utils-1.2.3/contentstack_utils.egg-info/PKG-INFO` & `contentstack_utils-1.3.0/contentstack_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contentstack_utils
-Version: 1.2.3
+Version: 1.3.0
 Summary: contentstack_utils is a Utility package for Contentstack headless CMS with an API-first approach.
 Home-page: https://github.com/contentstack/contentstack-utils-python
 Author: contentstack
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
```

### Comparing `contentstack_utils-1.2.3/setup.py` & `contentstack_utils-1.3.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import os
 
-from setuptools import find_packages
+from setuptools import setup, find_packages
 from distutils.core import setup
 
 with open(os.path.join(os.path.dirname(__file__), 'README.md')) as readme:
     long_description = readme.read()
 
 setup(
     name='contentstack_utils',
-    packages=find_packages(include=['contentstack']),
+    packages=find_packages(),
     description="contentstack_utils is a Utility package for Contentstack headless CMS with an API-first approach.",
     author='contentstack',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/contentstack/contentstack-utils-python",
     license='MIT',
-    version='1.2.3',
+    version='1.3.0',
     install_requires=[
         
     ],
     setup_requires=['pytest-runner'],
     tests_require=['pytest==4.4.1'],
     test_suite='tests',
     classifiers=[
```

### Comparing `contentstack_utils-1.2.3/tests/test_default_opt_others.py` & `contentstack_utils-1.3.0/tests/test_default_opt_others.py`

 * *Files identical despite different names*

### Comparing `contentstack_utils-1.2.3/tests/test_helper_node_to_html.py` & `contentstack_utils-1.3.0/tests/test_helper_node_to_html.py`

 * *Files identical despite different names*

### Comparing `contentstack_utils-1.2.3/tests/test_metadata.py` & `contentstack_utils-1.3.0/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `contentstack_utils-1.2.3/tests/test_option_render_mark.py` & `contentstack_utils-1.3.0/tests/test_option_render_mark.py`

 * *Files identical despite different names*

### Comparing `contentstack_utils-1.2.3/tests/test_render_default_options.py` & `contentstack_utils-1.3.0/tests/test_render_default_options.py`

 * *Files identical despite different names*

### Comparing `contentstack_utils-1.2.3/tests/test_render_options.py` & `contentstack_utils-1.3.0/tests/test_render_options.py`

 * *Files identical despite different names*

### Comparing `contentstack_utils-1.2.3/tests/test_style_type.py` & `contentstack_utils-1.3.0/tests/test_style_type.py`

 * *Files identical despite different names*

### Comparing `contentstack_utils-1.2.3/tests/test_util_srte.py` & `contentstack_utils-1.3.0/tests/test_util_srte.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,96 +26,107 @@
     global _json_data  # Note that the PyCharm warnings are not actual python errors
 
     def setUp(self):
         self._json_data = load_mock()
 
     def test_plaintext_in_supercharged_dict_to_html(self):
         array_str = ['plaintext']
-        Utils.json_to_html(self._json_data, array_str, Options())
-        self.assertEqual(Results.plainTextHtml, self._json_data['plaintext'])
+        response = Utils.json_to_html(self._json_data, array_str, Options())
+        self.assertEqual(Results.plainTextHtml, response)
 
     def test_plaintext_in_supercharged_list_to_html(self):
         array_str = ['plaintext_array']
-        Utils.json_to_html(self._json_data, array_str, Options())
-        self.assertEqual(Results.plainTextHtml, self._json_data['plaintext_array'][0])
+        response = Utils.json_to_html(self._json_data, array_str, Options())
+        self.assertEqual(Results.plainTextHtml, response)
 
     def test_paragraph_in_supercharged_dict_to_html(self):
         array_str = ['paragraph']
-        Utils.json_to_html([self._json_data], array_str, Options())
-        self.assertEqual(Results.paragraphHtml, self._json_data['paragraph'])
+        response = Utils.json_to_html([self._json_data], array_str, Options())
+        self.assertEqual(Results.paragraphHtml, response)
 
     def test_h1_in_supercharged_dict_to_html(self):
         array_str = ['h_one']
-        Utils.json_to_html([self._json_data], array_str, Options())
-        self.assertEqual(Results.h1Html, self._json_data['h_one'])
+        response = Utils.json_to_html([self._json_data], array_str, Options())
+        self.assertEqual(Results.h1Html, response)
 
     def test_h2_in_supercharged_dict_to_html(self):
         array_str = ['h_two']
-        Utils.json_to_html([self._json_data], array_str, Options())
-        self.assertEqual(Results.h2Html, self._json_data['h_two'])
+        response = Utils.json_to_html([self._json_data], array_str, Options())
+        self.assertEqual(Results.h2Html, response)
 
     def test_h3_in_supercharged_dict_to_html(self):
         array_str = ['h_three']
-        Utils.json_to_html([self._json_data], array_str, Options())
-        self.assertEqual(Results.h3Html, self._json_data['h_three'])
+        response = Utils.json_to_html([self._json_data], array_str, Options())
+        self.assertEqual(Results.h3Html, response)
 
     def test_h4_in_supercharged_dict_to_html(self):
         array_str = ['h_four']
-        Utils.json_to_html([self._json_data], array_str, Options())
-        self.assertEqual(Results.h4Html, self._json_data['h_four'])
+        response = Utils.json_to_html([self._json_data], array_str, Options())
+        self.assertEqual(Results.h4Html, response)
 
     def test_h5_in_supercharged_dict_to_html(self):
         array_str = ['h_five']
-        Utils.json_to_html([self._json_data], array_str, Options())
-        self.assertEqual(Results.h5Html, self._json_data['h_five'])
+        response = Utils.json_to_html([self._json_data], array_str, Options())
+        self.assertEqual(Results.h5Html, response)
 
     def test_h6_in_supercharged_dict_to_html(self):
         array_str = ['h_six']
-        Utils.json_to_html([self._json_data], array_str, Options())
-        self.assertEqual(Results.h6Html, self._json_data['h_six'])
+        response = Utils.json_to_html([self._json_data], array_str, Options())
+        self.assertEqual(Results.h6Html, response)
 
     def test_order_list_in_supercharged_dict_to_html(self):
         array_str = ['order_list']
-        Utils.json_to_html([self._json_data], array_str, Options())
-        self.assertEqual(Results.orderListHtml, self._json_data['order_list'])
+        response = Utils.json_to_html([self._json_data], array_str, Options())
+        self.assertEqual(Results.orderListHtml, response)
 
     def test_un_order_list_in_supercharged_dict_to_html(self):
         array_str = ['un_order_list']
-        Utils.json_to_html([self._json_data], array_str, Options())
-        self.assertEqual(Results.unorderListHtml, self._json_data['un_order_list'])
+        response = Utils.json_to_html([self._json_data], array_str, Options())
+        self.assertEqual(Results.unorderListHtml, response)
 
     def test_image_list_in_supercharged_dict_to_html(self):
         array_str = ['img']
-        Utils.json_to_html([self._json_data], array_str, Options())
-        self.assertEqual(Results.imgHtml, self._json_data['img'])
+        response = Utils.json_to_html([self._json_data], array_str, Options())
+        self.assertEqual(Results.imgHtml, response)
 
     def test_table_list_in_supercharged_dict_to_html(self):
         array_str = ['table']
-        Utils.json_to_html([self._json_data], array_str, Options())
-        self.assertEqual(Results.tableHtml, self._json_data['table'])
+        response = Utils.json_to_html([self._json_data], array_str, Options())
+        self.assertEqual(Results.tableHtml, response)
 
     def test_blockquote_list_in_supercharged_dict_to_html(self):
         array_str = ['blockquote']
-        Utils.json_to_html([self._json_data], array_str, Options())
-        self.assertEqual(Results.blockquoteHtml, self._json_data['blockquote'])
+        response = Utils.json_to_html([self._json_data], array_str, Options())
+        self.assertEqual(Results.blockquoteHtml, response)
 
     def test_code_list_in_supercharged_dict_to_html(self):
         array_str = ['code']
-        Utils.json_to_html([self._json_data], array_str, Options())
-        self.assertEqual(Results.codeHtml, self._json_data['code'])
+        response = Utils.json_to_html([self._json_data], array_str, Options())
+        self.assertEqual(Results.codeHtml, response)
 
     def test_linkin_list_in_supercharged_dict_to_html(self):
         array_str = ['link']
+        response = Utils.json_to_html([self._json_data], array_str, Options())
+        self.assertEqual(Results.linkInPHtml, response)
+
+    def test_reference_list_in_supercharged_dict_to_html(self):
+        array_str = ['reference']
+        response = response = Utils.json_to_html([self._json_data], array_str, Options())
+        self.assertEqual(Results.refImgHtml, response)
+    
+    def test_nested_order_list_in_supercharged_dict_to_html(self):
+        array_str = ['nested_order_list_with_fragment']
         Utils.json_to_html([self._json_data], array_str, Options())
-        self.assertEqual(Results.linkInPHtml, self._json_data['link'])
+        self.assertEqual(Results.nested_order_list_with_fragment, "<ol><li><fragment>List Item 1</fragment><ol><li>List Item 1.1</li><li>List Item 1.2</li><li>List Item 1.3</li></ol></li></ol>")
+
 
-    # def test_reference_list_in_supercharged_dict_to_html(self):
-    #     array_str = ['reference']
-    #     Utils.json_to_html([self._json_data], array_str, Options())
-    #     self.assertEqual(Results.linkInPHtml, self._json_data['reference'])
+    def test_reference_list_in_supercharged_dict_to_html(self):
+         array_str = ['reference']
+         Utils.json_to_html([self._json_data], array_str, Options())
+         self.assertEqual(Results.linkInPHtml, self._json_data['reference'])
     
     def test_nested_order_list_in_supercharged_dict_to_html(self):
         array_str = ['nested_order_list_with_fragment']
         Utils.json_to_html([self._json_data], array_str, Options())
         self.assertEqual(Results.nested_order_list_with_fragment, "<ol><li><fragment>List Item 1</fragment><ol><li>List Item 1.1</li><li>List Item 1.2</li><li>List Item 1.3</li></ol></li></ol>")
 
     def test_nested_unorder_list_in_supercharged_dict_to_html(self):
```

### Comparing `contentstack_utils-1.2.3/tests/test_utils.py` & `contentstack_utils-1.3.0/tests/test_utils.py`

 * *Files identical despite different names*

