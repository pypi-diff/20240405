# Comparing `tmp/pytexmk-0.4.2.240322.tar.gz` & `tmp/pytexmk-0.4.3.240405.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytexmk-0.4.2.240322.tar", last modified: Fri Mar 22 06:51:53 2024, max compression
+gzip compressed data, was "pytexmk-0.4.3.240405.tar", last modified: Fri Apr  5 01:10:10 2024, max compression
```

## Comparing `pytexmk-0.4.2.240322.tar` & `pytexmk-0.4.3.240405.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 yanming   (1000) yanming   (1000)        0 2024-03-22 06:51:53.978723 pytexmk-0.4.2.240322/
--rw-rw-r--   0 yanming   (1000) yanming   (1000)    35149 2024-02-28 15:10:35.000000 pytexmk-0.4.2.240322/LICENSE
--rw-rw-r--   0 yanming   (1000) yanming   (1000)       30 2024-03-06 03:27:48.000000 pytexmk-0.4.2.240322/MANIFEST.in
--rw-rw-r--   0 yanming   (1000) yanming   (1000)      466 2024-03-06 03:27:48.000000 pytexmk-0.4.2.240322/Makefile
--rw-r--r--   0 yanming   (1000) yanming   (1000)     7406 2024-03-22 06:51:53.974723 pytexmk-0.4.2.240322/PKG-INFO
--rw-rw-r--   0 yanming   (1000) yanming   (1000)     6360 2024-03-22 06:40:11.000000 pytexmk-0.4.2.240322/README.md
--rw-rw-r--   0 yanming   (1000) yanming   (1000)     1195 2024-03-21 15:51:11.000000 pytexmk-0.4.2.240322/pyproject.toml
--rw-rw-r--   0 yanming   (1000) yanming   (1000)       38 2024-03-22 06:51:53.978723 pytexmk-0.4.2.240322/setup.cfg
-drwxrwxr-x   0 yanming   (1000) yanming   (1000)        0 2024-03-22 06:51:53.970723 pytexmk-0.4.2.240322/src/
-drwxrwxr-x   0 yanming   (1000) yanming   (1000)        0 2024-03-22 06:51:53.974723 pytexmk-0.4.2.240322/src/pytexmk/
--rw-rw-r--   0 yanming   (1000) yanming   (1000)     1940 2024-02-29 11:40:30.000000 pytexmk-0.4.2.240322/src/pytexmk/__init__.py
--rw-rw-r--   0 yanming   (1000) yanming   (1000)     9638 2024-03-22 06:44:14.000000 pytexmk-0.4.2.240322/src/pytexmk/__main__.py
--rw-rw-r--   0 yanming   (1000) yanming   (1000)     8546 2024-03-22 05:49:42.000000 pytexmk-0.4.2.240322/src/pytexmk/additional_operation.py
--rw-rw-r--   0 yanming   (1000) yanming   (1000)     9922 2024-03-22 06:51:11.000000 pytexmk-0.4.2.240322/src/pytexmk/compile_model.py
--rw-rw-r--   0 yanming   (1000) yanming   (1000)     5896 2024-03-22 06:50:52.000000 pytexmk-0.4.2.240322/src/pytexmk/info_print.py
--rw-rw-r--   0 yanming   (1000) yanming   (1000)     1922 2024-03-22 06:51:36.000000 pytexmk-0.4.2.240322/src/pytexmk/version.py
-drwxrwxr-x   0 yanming   (1000) yanming   (1000)        0 2024-03-22 06:51:53.974723 pytexmk-0.4.2.240322/src/pytexmk.egg-info/
--rw-r--r--   0 yanming   (1000) yanming   (1000)     7406 2024-03-22 06:51:53.000000 pytexmk-0.4.2.240322/src/pytexmk.egg-info/PKG-INFO
--rw-rw-r--   0 yanming   (1000) yanming   (1000)      441 2024-03-22 06:51:53.000000 pytexmk-0.4.2.240322/src/pytexmk.egg-info/SOURCES.txt
--rw-rw-r--   0 yanming   (1000) yanming   (1000)        1 2024-03-22 06:51:53.000000 pytexmk-0.4.2.240322/src/pytexmk.egg-info/dependency_links.txt
--rw-rw-r--   0 yanming   (1000) yanming   (1000)       41 2024-03-22 06:51:53.000000 pytexmk-0.4.2.240322/src/pytexmk.egg-info/entry_points.txt
--rw-rw-r--   0 yanming   (1000) yanming   (1000)       13 2024-03-22 06:51:53.000000 pytexmk-0.4.2.240322/src/pytexmk.egg-info/requires.txt
--rw-rw-r--   0 yanming   (1000) yanming   (1000)        8 2024-03-22 06:51:53.000000 pytexmk-0.4.2.240322/src/pytexmk.egg-info/top_level.txt
-drwxrwxr-x   0 yanming   (1000) yanming   (1000)        0 2024-03-22 06:51:53.974723 pytexmk-0.4.2.240322/tests/
--rw-rw-r--   0 yanming   (1000) yanming   (1000)     9643 2024-03-22 06:30:29.000000 pytexmk-0.4.2.240322/tests/test.py
+drwxrwxr-x   0 yanming   (1000) yanming   (1000)        0 2024-04-05 01:10:10.311704 pytexmk-0.4.3.240405/
+-rw-rw-r--   0 yanming   (1000) yanming   (1000)    35149 2024-02-28 15:10:35.000000 pytexmk-0.4.3.240405/LICENSE
+-rw-rw-r--   0 yanming   (1000) yanming   (1000)       30 2024-03-06 03:27:48.000000 pytexmk-0.4.3.240405/MANIFEST.in
+-rw-rw-r--   0 yanming   (1000) yanming   (1000)      466 2024-03-06 03:27:48.000000 pytexmk-0.4.3.240405/Makefile
+-rw-r--r--   0 yanming   (1000) yanming   (1000)     7406 2024-04-05 01:10:10.311704 pytexmk-0.4.3.240405/PKG-INFO
+-rw-rw-r--   0 yanming   (1000) yanming   (1000)     6360 2024-03-22 06:40:11.000000 pytexmk-0.4.3.240405/README.md
+-rw-rw-r--   0 yanming   (1000) yanming   (1000)     1195 2024-03-21 15:51:11.000000 pytexmk-0.4.3.240405/pyproject.toml
+-rw-rw-r--   0 yanming   (1000) yanming   (1000)       38 2024-04-05 01:10:10.311704 pytexmk-0.4.3.240405/setup.cfg
+drwxrwxr-x   0 yanming   (1000) yanming   (1000)        0 2024-04-05 01:10:10.307703 pytexmk-0.4.3.240405/src/
+drwxrwxr-x   0 yanming   (1000) yanming   (1000)        0 2024-04-05 01:10:10.311704 pytexmk-0.4.3.240405/src/pytexmk/
+-rw-rw-r--   0 yanming   (1000) yanming   (1000)     1940 2024-02-29 11:40:30.000000 pytexmk-0.4.3.240405/src/pytexmk/__init__.py
+-rw-rw-r--   0 yanming   (1000) yanming   (1000)     9617 2024-04-05 01:04:06.000000 pytexmk-0.4.3.240405/src/pytexmk/__main__.py
+-rw-rw-r--   0 yanming   (1000) yanming   (1000)     8126 2024-04-05 00:55:30.000000 pytexmk-0.4.3.240405/src/pytexmk/additional_operation.py
+-rw-rw-r--   0 yanming   (1000) yanming   (1000)     9922 2024-03-22 06:51:11.000000 pytexmk-0.4.3.240405/src/pytexmk/compile_model.py
+-rw-rw-r--   0 yanming   (1000) yanming   (1000)     5896 2024-03-22 06:50:52.000000 pytexmk-0.4.3.240405/src/pytexmk/info_print.py
+-rw-rw-r--   0 yanming   (1000) yanming   (1000)     1922 2024-04-05 01:06:45.000000 pytexmk-0.4.3.240405/src/pytexmk/version.py
+drwxrwxr-x   0 yanming   (1000) yanming   (1000)        0 2024-04-05 01:10:10.311704 pytexmk-0.4.3.240405/src/pytexmk.egg-info/
+-rw-r--r--   0 yanming   (1000) yanming   (1000)     7406 2024-04-05 01:10:10.000000 pytexmk-0.4.3.240405/src/pytexmk.egg-info/PKG-INFO
+-rw-rw-r--   0 yanming   (1000) yanming   (1000)      441 2024-04-05 01:10:10.000000 pytexmk-0.4.3.240405/src/pytexmk.egg-info/SOURCES.txt
+-rw-rw-r--   0 yanming   (1000) yanming   (1000)        1 2024-04-05 01:10:10.000000 pytexmk-0.4.3.240405/src/pytexmk.egg-info/dependency_links.txt
+-rw-rw-r--   0 yanming   (1000) yanming   (1000)       41 2024-04-05 01:10:10.000000 pytexmk-0.4.3.240405/src/pytexmk.egg-info/entry_points.txt
+-rw-rw-r--   0 yanming   (1000) yanming   (1000)       13 2024-04-05 01:10:10.000000 pytexmk-0.4.3.240405/src/pytexmk.egg-info/requires.txt
+-rw-rw-r--   0 yanming   (1000) yanming   (1000)        8 2024-04-05 01:10:10.000000 pytexmk-0.4.3.240405/src/pytexmk.egg-info/top_level.txt
+drwxrwxr-x   0 yanming   (1000) yanming   (1000)        0 2024-04-05 01:10:10.311704 pytexmk-0.4.3.240405/tests/
+-rw-rw-r--   0 yanming   (1000) yanming   (1000)     9643 2024-03-22 06:30:29.000000 pytexmk-0.4.3.240405/tests/test.py
```

### Comparing `pytexmk-0.4.2.240322/LICENSE` & `pytexmk-0.4.3.240405/LICENSE`

 * *Files identical despite different names*

### Comparing `pytexmk-0.4.2.240322/PKG-INFO` & `pytexmk-0.4.3.240405/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytexmk
-Version: 0.4.2.240322
+Version: 0.4.3.240405
 Summary: LaTeX 辅助编译命令行工具 LaTeX Auxiliary Compilation Command Line Tool
 Author-email: 焱铭 <lxb-yanming@foxmail.com>
 Project-URL: Homepage, https://github.com/YanMing-lxb/PyTeXMK
 Project-URL: Bug Tracker, https://github.com/YanMing-lxb/PyTeXMK/issues
 Keywords: LaTeX,build,latexmk
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `pytexmk-0.4.2.240322/README.md` & `pytexmk-0.4.3.240405/README.md`

 * *Files identical despite different names*

### Comparing `pytexmk-0.4.2.240322/pyproject.toml` & `pytexmk-0.4.3.240405/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytexmk-0.4.2.240322/src/pytexmk/__init__.py` & `pytexmk-0.4.3.240405/src/pytexmk/__init__.py`

 * *Files identical despite different names*

### Comparing `pytexmk-0.4.2.240322/src/pytexmk/__main__.py` & `pytexmk-0.4.3.240405/src/pytexmk/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
  ··························································Y8b·d88P·····
  ···························································"Y88P"······
  =======================================================================
 
  -----------------------------------------------------------------------
 Author       : 焱铭
 Date         : 2024-02-28 23:11:52 +0800
-LastEditTime : 2024-03-22 14:44:14 +0800
+LastEditTime : 2024-04-05 09:03:28 +0800
 Github       : https://github.com/YanMing-lxb/
 FilePath     : /PyTeXMK/src/pytexmk/__main__.py
 Description  : 
  -----------------------------------------------------------------------
 '''
 # -*- coding: utf-8 -*-
 import argparse
@@ -139,15 +139,15 @@
         file_name = search_file() # 运行 search_file 函数判断
 
     if file_name: # 如果存在 file_name
         if args.clean:
             remove_aux(file_name)
         elif args.Clean:
             remove_aux(file_name)
-            remove_result(build_path,build_path,file_name)
+            remove_result(build_path)
             remove_result_in_root(file_name)
         elif args.clean_pdf:
             clean_all_pdf('.', build_path, file_name)
         else:
             compile(start_time, tex_name, file_name, not args.no_quiet, build_path)
```

### Comparing `pytexmk-0.4.2.240322/src/pytexmk/additional_operation.py` & `pytexmk-0.4.3.240405/src/pytexmk/additional_operation.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
  ··························································Y8b·d88P·····
  ···························································"Y88P"······
  =======================================================================
 
  -----------------------------------------------------------------------
 Author       : 焱铭
 Date         : 2024-02-29 16:02:37 +0800
-LastEditTime : 2024-03-22 13:49:42 +0800
+LastEditTime : 2024-04-05 08:55:30 +0800
 Github       : https://github.com/YanMing-lxb/
 FilePath     : /PyTeXMK/src/pytexmk/additional_operation.py
 Description  : 
  -----------------------------------------------------------------------
 '''
 # -*- coding: utf-8 -*-
 import os
@@ -98,37 +98,27 @@
             # 如果当前处理的是根目录文件，则跳过
             continue 
 
         for file in files:
             if file.endswith('.pdf') and file != f'{file_name}.pdf':
                 pdf_files.append(os.path.join(root, file))  # 仅清理子文件夹中的pdf文件
     
+    # 对pdf文件进行打开和关闭操作，解决origin批量导出pdf文件时由于未关闭pdf导致的报错
     if pdf_files:
         print(f"共发现 {len(pdf_files)} 个PDF文件。")
         for pdf_file in pdf_files:
             try:
                 doc = fitz.open(pdf_file)
-                clean_doc = fitz.open()
-                
-                for page_num in range(doc.page_count):
-                    page = doc.load_page(page_num)
-                    clean_doc.insert_page(page_num, width=page.rect.width, height=page.rect.height)
-                    clean_doc[page_num].show_pdf_page(page.rect, doc, page_num)
-                
-                output_path = f"{pdf_file}.cleancopied.pdf"
-                clean_doc.save(output_path)
-                clean_doc.close()
-                
-                os.replace(output_path, pdf_file)
+                doc.close()
                 print(f"已处理: {pdf_file}")
             except Exception as e:
                 print(f"处理出错 {pdf_file}: {e}")
         print("所有PDF文件已处理完成。")
     else:
-        print("当前路径下未发现PDF文件。") 
+        print("当前路径下未发现PDF文件。")
     
 # --------------------------------------------------------------------------------
 # 定义输入检查函数
 # --------------------------------------------------------------------------------
 def check_file_name(file_name):
     base_name, file_extension = os.path.splitext(
         os.path.basename(file_name))  # 去掉路径，提取文件名和后缀
```

### Comparing `pytexmk-0.4.2.240322/src/pytexmk/compile_model.py` & `pytexmk-0.4.3.240405/src/pytexmk/compile_model.py`

 * *Files identical despite different names*

### Comparing `pytexmk-0.4.2.240322/src/pytexmk/info_print.py` & `pytexmk-0.4.3.240405/src/pytexmk/info_print.py`

 * *Files identical despite different names*

### Comparing `pytexmk-0.4.2.240322/src/pytexmk/version.py` & `pytexmk-0.4.3.240405/src/pytexmk/version.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,18 +12,18 @@
  ··························································Y8b·d88P·····
  ···························································"Y88P"······
  =======================================================================
 
  -----------------------------------------------------------------------
 Author       : 焱铭
 Date         : 2024-03-01 15:52:28 +0800
-LastEditTime : 2024-03-22 14:51:36 +0800
+LastEditTime : 2024-04-05 08:57:01 +0800
 Github       : https://github.com/YanMing-lxb/
 FilePath     : /PyTeXMK/src/pytexmk/version.py
 Description  : 
  -----------------------------------------------------------------------
 '''
 # -*- coding: utf-8 -*-
 #!/usr/bin/env python
 
 script_name = 'PyTeXMK'
-__version__ = '0.4.2.240322'
+__version__ = '0.4.3.240405'
```

### Comparing `pytexmk-0.4.2.240322/src/pytexmk.egg-info/PKG-INFO` & `pytexmk-0.4.3.240405/src/pytexmk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytexmk
-Version: 0.4.2.240322
+Version: 0.4.3.240405
 Summary: LaTeX 辅助编译命令行工具 LaTeX Auxiliary Compilation Command Line Tool
 Author-email: 焱铭 <lxb-yanming@foxmail.com>
 Project-URL: Homepage, https://github.com/YanMing-lxb/PyTeXMK
 Project-URL: Bug Tracker, https://github.com/YanMing-lxb/PyTeXMK/issues
 Keywords: LaTeX,build,latexmk
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `pytexmk-0.4.2.240322/tests/test.py` & `pytexmk-0.4.3.240405/tests/test.py`

 * *Files identical despite different names*

