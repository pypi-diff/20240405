# Comparing `tmp/ljl-api-1.0.0.tar.gz` & `tmp/ljl-api-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ljl-api-1.0.0.tar", last modified: Thu Apr  4 14:56:25 2024, max compression
+gzip compressed data, was "dist\ljl-api-1.0.1.tar", last modified: Fri Apr  5 02:21:43 2024, max compression
```

## Comparing `ljl-api-1.0.0.tar` & `ljl-api-1.0.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 14:56:25.000000 ljl-api-1.0.0/
--rw-rw-rw-   0        0        0      316 2024-04-04 14:56:25.000000 ljl-api-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-04 14:56:25.000000 ljl-api-1.0.0/common/
--rw-rw-rw-   0        0        0       91 2024-04-04 07:32:39.000000 ljl-api-1.0.0/common/__init__.py
--rw-rw-rw-   0        0        0      455 2024-04-04 07:32:39.000000 ljl-api-1.0.0/common/base_request.py
--rw-rw-rw-   0        0        0     1800 2024-04-04 07:32:39.000000 ljl-api-1.0.0/common/base_response.py
--rw-rw-rw-   0        0        0     3315 2024-04-04 07:32:39.000000 ljl-api-1.0.0/common/base_send_request.py
--rw-rw-rw-   0        0        0      142 2024-04-04 07:32:39.000000 ljl-api-1.0.0/common/custom_exception.py
--rw-rw-rw-   0        0        0     3461 2024-04-04 07:32:39.000000 ljl-api-1.0.0/common/descriptions.py
--rw-rw-rw-   0        0        0      706 2024-04-04 07:32:39.000000 ljl-api-1.0.0/common/key_map.py
--rw-rw-rw-   0        0        0     4367 2024-04-04 07:32:39.000000 ljl-api-1.0.0/common/keys_driver.py
--rw-rw-rw-   0        0        0      921 2024-04-04 14:52:48.000000 ljl-api-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-04 14:56:25.000000 ljl-api-1.0.0/tools/
--rw-rw-rw-   0        0        0       91 2024-04-04 07:32:39.000000 ljl-api-1.0.0/tools/__init__.py
--rw-rw-rw-   0        0        0     2929 2024-04-04 07:32:39.000000 ljl-api-1.0.0/tools/assert_methods.py
--rw-rw-rw-   0        0        0     2631 2024-04-04 07:32:39.000000 ljl-api-1.0.0/tools/common_methods.py
--rw-rw-rw-   0        0        0     1271 2024-04-04 07:32:39.000000 ljl-api-1.0.0/tools/config.py
--rw-rw-rw-   0        0        0     2301 2024-04-04 07:32:39.000000 ljl-api-1.0.0/tools/excel_tools.py
--rw-rw-rw-   0        0        0     2488 2024-04-04 07:32:39.000000 ljl-api-1.0.0/tools/log.py
--rw-rw-rw-   0        0        0     2169 2024-04-04 07:32:39.000000 ljl-api-1.0.0/tools/mysql_tools.py
--rw-rw-rw-   0        0        0     2240 2024-04-04 07:32:39.000000 ljl-api-1.0.0/tools/post_process_methods.py
--rw-rw-rw-   0        0        0      643 2024-04-04 07:32:39.000000 ljl-api-1.0.0/tools/random_data.py
--rw-rw-rw-   0        0        0     1446 2024-04-04 07:32:39.000000 ljl-api-1.0.0/tools/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-05 02:21:43.000000 ljl-api-1.0.1/
+-rw-rw-rw-   0        0        0      316 2024-04-05 02:21:43.000000 ljl-api-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-05 02:21:43.000000 ljl-api-1.0.1/common/
+-rw-rw-rw-   0        0        0       91 2024-04-04 07:32:39.000000 ljl-api-1.0.1/common/__init__.py
+-rw-rw-rw-   0        0        0      455 2024-04-04 07:32:39.000000 ljl-api-1.0.1/common/base_request.py
+-rw-rw-rw-   0        0        0     1800 2024-04-04 07:32:39.000000 ljl-api-1.0.1/common/base_response.py
+-rw-rw-rw-   0        0        0     3315 2024-04-04 07:32:39.000000 ljl-api-1.0.1/common/base_send_request.py
+-rw-rw-rw-   0        0        0      142 2024-04-04 07:32:39.000000 ljl-api-1.0.1/common/custom_exception.py
+-rw-rw-rw-   0        0        0     3461 2024-04-04 07:32:39.000000 ljl-api-1.0.1/common/descriptions.py
+-rw-rw-rw-   0        0        0      706 2024-04-04 07:32:39.000000 ljl-api-1.0.1/common/key_map.py
+-rw-rw-rw-   0        0        0     4367 2024-04-04 07:32:39.000000 ljl-api-1.0.1/common/keys_driver.py
+-rw-rw-rw-   0        0        0      929 2024-04-05 02:21:39.000000 ljl-api-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 02:21:43.000000 ljl-api-1.0.1/tools/
+-rw-rw-rw-   0        0        0       91 2024-04-04 07:32:39.000000 ljl-api-1.0.1/tools/__init__.py
+-rw-rw-rw-   0        0        0     2929 2024-04-04 07:32:39.000000 ljl-api-1.0.1/tools/assert_methods.py
+-rw-rw-rw-   0        0        0     2631 2024-04-04 07:32:39.000000 ljl-api-1.0.1/tools/common_methods.py
+-rw-rw-rw-   0        0        0     1271 2024-04-04 07:32:39.000000 ljl-api-1.0.1/tools/config.py
+-rw-rw-rw-   0        0        0     2301 2024-04-04 07:32:39.000000 ljl-api-1.0.1/tools/excel_tools.py
+-rw-rw-rw-   0        0        0     2488 2024-04-04 07:32:39.000000 ljl-api-1.0.1/tools/log.py
+-rw-rw-rw-   0        0        0     2169 2024-04-04 07:32:39.000000 ljl-api-1.0.1/tools/mysql_tools.py
+-rw-rw-rw-   0        0        0     2240 2024-04-04 07:32:39.000000 ljl-api-1.0.1/tools/post_process_methods.py
+-rw-rw-rw-   0        0        0      643 2024-04-04 07:32:39.000000 ljl-api-1.0.1/tools/random_data.py
+-rw-rw-rw-   0        0        0     1446 2024-04-04 07:32:39.000000 ljl-api-1.0.1/tools/utils.py
```

### Comparing `ljl-api-1.0.0/common/base_response.py` & `ljl-api-1.0.1/common/base_response.py`

 * *Files identical despite different names*

### Comparing `ljl-api-1.0.0/common/base_send_request.py` & `ljl-api-1.0.1/common/base_send_request.py`

 * *Files identical despite different names*

### Comparing `ljl-api-1.0.0/common/descriptions.py` & `ljl-api-1.0.1/common/descriptions.py`

 * *Files identical despite different names*

### Comparing `ljl-api-1.0.0/common/key_map.py` & `ljl-api-1.0.1/common/key_map.py`

 * *Files identical despite different names*

### Comparing `ljl-api-1.0.0/common/keys_driver.py` & `ljl-api-1.0.1/common/keys_driver.py`

 * *Files identical despite different names*

### Comparing `ljl-api-1.0.0/setup.py` & `ljl-api-1.0.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,33 +4,33 @@
 @file: setup.py.py
 @date: 2024/04/04 20:47
 """
 from distutils.core import setup
 
 setup(
     name="ljl-api",   # 这里是pip项目发布的名称
-    version="1.0.0",
+    version="1.0.1",
     keywords=["init", "auto-test"],  # pip 官网搜索关键字
     description="to simplify auto test",   # 简单描述
     long_description="A init package,to simplify develope auto test",  # 详细描述
     license="MIT Licence",
 
     url="https://git.code.tencent.com/2024111/lijl.git",
     author="ljl",
     author_email="1316597471@qq.com",
     packages=["tools", 'common'],
     platforms="python",
     install_requires=[
-        'allure-pytest==2.9.45'
-        'configparser==5.2.0'
-        'Faker==13.3.4'
-        'jsonpath==0.82'
-        'PyMySQL==1.0.2'
-        'pytest==7.1.1'
-        'requests==2.27.1'
-        'xlwt==1.3.0'
+        'allure-pytest==2.9.45',
+        'configparser==5.2.0',
+        'Faker==13.3.4',
+        'jsonpath==0.82',
+        'PyMySQL==1.0.2',
+        'pytest==7.1.1',
+        'requests==2.27.1',
+        'xlwt==1.3.0',
         'xlrd==2.0.1'
     ]
 
 )
```

### Comparing `ljl-api-1.0.0/tools/assert_methods.py` & `ljl-api-1.0.1/tools/assert_methods.py`

 * *Files identical despite different names*

### Comparing `ljl-api-1.0.0/tools/common_methods.py` & `ljl-api-1.0.1/tools/common_methods.py`

 * *Files identical despite different names*

### Comparing `ljl-api-1.0.0/tools/config.py` & `ljl-api-1.0.1/tools/config.py`

 * *Files identical despite different names*

### Comparing `ljl-api-1.0.0/tools/excel_tools.py` & `ljl-api-1.0.1/tools/excel_tools.py`

 * *Files identical despite different names*

### Comparing `ljl-api-1.0.0/tools/log.py` & `ljl-api-1.0.1/tools/log.py`

 * *Files identical despite different names*

### Comparing `ljl-api-1.0.0/tools/mysql_tools.py` & `ljl-api-1.0.1/tools/mysql_tools.py`

 * *Files identical despite different names*

### Comparing `ljl-api-1.0.0/tools/post_process_methods.py` & `ljl-api-1.0.1/tools/post_process_methods.py`

 * *Files identical despite different names*

### Comparing `ljl-api-1.0.0/tools/random_data.py` & `ljl-api-1.0.1/tools/random_data.py`

 * *Files identical despite different names*

### Comparing `ljl-api-1.0.0/tools/utils.py` & `ljl-api-1.0.1/tools/utils.py`

 * *Files identical despite different names*

