# Comparing `tmp/notion_export_prettify-1.0.0.tar.gz` & `tmp/notion_export_prettify-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notion_export_prettify-1.0.0.tar", max compression
+gzip compressed data, was "notion_export_prettify-1.1.0.tar", max compression
```

## Comparing `notion_export_prettify-1.0.0.tar` & `notion_export_prettify-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,32 @@
--rw-r--r--   0        0        0    35149 2024-04-01 18:48:50.198602 notion_export_prettify-1.0.0/LICENSE
--rw-r--r--   0        0        0     1086 2024-04-04 18:39:58.140253 notion_export_prettify-1.0.0/README.md
--rw-r--r--   0        0        0     2271 2024-04-04 07:33:39.560878 notion_export_prettify-1.0.0/notion_export_prettify/args.py
--rw-r--r--   0        0        0      627 2024-04-03 10:13:09.261587 notion_export_prettify-1.0.0/notion_export_prettify/html_templator.py
--rw-r--r--   0        0        0     7604 2024-04-04 18:55:12.219877 notion_export_prettify-1.0.0/notion_export_prettify/main.py
--rw-r--r--   0        0        0     4198 2024-04-03 13:05:17.580220 notion_export_prettify-1.0.0/notion_export_prettify/notion_html_manipulator.py
--rw-r--r--   0        0        0     3584 2024-04-03 07:52:48.091170 notion_export_prettify-1.0.0/notion_export_prettify/pdf_maker.py
--rw-r--r--   0        0        0      487 2024-04-02 12:21:37.599209 notion_export_prettify-1.0.0/notion_export_prettify/print_color.py
--rw-r--r--   0        0        0      544 2024-04-04 09:04:38.247121 notion_export_prettify-1.0.0/notion_export_prettify/resource_loader.py
--rw-r--r--   0        0        0      501 2024-04-04 18:46:18.101599 notion_export_prettify-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1699 1970-01-01 00:00:00.000000 notion_export_prettify-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-01 18:48:50.198602 notion_export_prettify-1.1.0/LICENSE
+-rw-r--r--   0        0        0     1086 2024-04-04 18:39:58.140253 notion_export_prettify-1.1.0/README.md
+-rw-r--r--   0        0        0     4206 2024-04-04 19:37:10.910941 notion_export_prettify-1.1.0/notion_export_prettify/args.py
+-rw-r--r--   0        0        0      627 2024-04-03 10:13:09.261587 notion_export_prettify-1.1.0/notion_export_prettify/html_templator.py
+-rw-r--r--   0        0        0     7604 2024-04-04 18:55:12.219877 notion_export_prettify-1.1.0/notion_export_prettify/main.py
+-rw-r--r--   0        0        0     4198 2024-04-03 13:05:17.580220 notion_export_prettify-1.1.0/notion_export_prettify/notion_html_manipulator.py
+-rw-r--r--   0        0        0     3584 2024-04-03 07:52:48.091170 notion_export_prettify-1.1.0/notion_export_prettify/pdf_maker.py
+-rw-r--r--   0        0        0      487 2024-04-02 12:21:37.599209 notion_export_prettify-1.1.0/notion_export_prettify/print_color.py
+-rw-r--r--   0        0        0      544 2024-04-04 09:04:38.247121 notion_export_prettify-1.1.0/notion_export_prettify/resource_loader.py
+-rw-r--r--   0        0        0      564 2024-04-04 19:38:57.143780 notion_export_prettify-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0   230377 2024-04-03 13:43:21.151671 notion_export_prettify-1.1.0/templates/example/Template.docx
+-rw-r--r--   0        0        0   276675 2024-04-03 13:43:42.403006 notion_export_prettify-1.1.0/templates/example/Template.pdf
+-rw-r--r--   0        0        0     1548 2024-04-04 05:57:48.789967 notion_export_prettify-1.1.0/templates/example/background.html
+-rw-r--r--   0        0        0   189801 2024-04-01 19:09:41.200162 notion_export_prettify-1.1.0/templates/example/background.pdf
+-rw-r--r--   0        0        0      866 2024-04-03 10:32:49.294889 notion_export_prettify-1.1.0/templates/example/cover.html
+-rw-r--r--   0        0        0   189503 2024-04-04 05:51:52.153098 notion_export_prettify-1.1.0/templates/example/cover.pdf
+-rw-r--r--   0        0        0      259 2024-04-02 14:09:30.587923 notion_export_prettify-1.1.0/templates/example/header.html
+-rw-r--r--   0        0        0     1312 2024-04-04 08:58:09.824206 notion_export_prettify-1.1.0/templates/example/overwrites.css
+-rw-r--r--   0        0        0      284 2024-04-03 10:28:49.768673 notion_export_prettify-1.1.0/templates/example/page.css
+-rw-r--r--   0        0        0      274 2024-04-04 18:40:58.122618 notion_export_prettify-1.1.0/templates/example/template.cfg
+-rw-r--r--   0        0        0   230377 2024-04-03 13:43:21.151671 notion_export_prettify-1.1.0/templates/example-landscape/Template.docx
+-rw-r--r--   0        0        0   276675 2024-04-03 13:43:42.403006 notion_export_prettify-1.1.0/templates/example-landscape/Template.pdf
+-rw-r--r--   0        0        0     1647 2024-04-03 14:34:54.616855 notion_export_prettify-1.1.0/templates/example-landscape/background.html
+-rw-r--r--   0        0        0   145726 2024-04-03 14:26:33.234530 notion_export_prettify-1.1.0/templates/example-landscape/background.pdf
+-rw-r--r--   0        0        0      610 2024-04-03 14:31:54.174634 notion_export_prettify-1.1.0/templates/example-landscape/cover.html
+-rw-r--r--   0        0        0   189801 2024-04-03 14:26:30.773443 notion_export_prettify-1.1.0/templates/example-landscape/cover.pdf
+-rw-r--r--   0        0        0      259 2024-04-02 14:09:30.587923 notion_export_prettify-1.1.0/templates/example-landscape/header.html
+-rw-r--r--   0        0        0     1292 2024-04-04 06:00:32.145611 notion_export_prettify-1.1.0/templates/example-landscape/overwrites.css
+-rw-r--r--   0        0        0      285 2024-04-03 14:27:19.637736 notion_export_prettify-1.1.0/templates/example-landscape/page.css
+-rw-r--r--   0        0        0      272 2024-04-04 18:41:06.629196 notion_export_prettify-1.1.0/templates/example-landscape/template.cfg
+-rw-r--r--   0        0        0      162 2024-04-03 13:38:07.479218 notion_export_prettify-1.1.0/templates/example-landscape/~$mplate.docx
+-rw-r--r--   0        0        0     1699 1970-01-01 00:00:00.000000 notion_export_prettify-1.1.0/PKG-INFO
```

### Comparing `notion_export_prettify-1.0.0/LICENSE` & `notion_export_prettify-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `notion_export_prettify-1.0.0/README.md` & `notion_export_prettify-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `notion_export_prettify-1.0.0/notion_export_prettify/html_templator.py` & `notion_export_prettify-1.1.0/notion_export_prettify/html_templator.py`

 * *Files identical despite different names*

### Comparing `notion_export_prettify-1.0.0/notion_export_prettify/main.py` & `notion_export_prettify-1.1.0/notion_export_prettify/main.py`

 * *Files identical despite different names*

### Comparing `notion_export_prettify-1.0.0/notion_export_prettify/notion_html_manipulator.py` & `notion_export_prettify-1.1.0/notion_export_prettify/notion_html_manipulator.py`

 * *Files identical despite different names*

### Comparing `notion_export_prettify-1.0.0/notion_export_prettify/pdf_maker.py` & `notion_export_prettify-1.1.0/notion_export_prettify/pdf_maker.py`

 * *Files identical despite different names*

### Comparing `notion_export_prettify-1.0.0/notion_export_prettify/resource_loader.py` & `notion_export_prettify-1.1.0/notion_export_prettify/resource_loader.py`

 * *Files identical despite different names*

### Comparing `notion_export_prettify-1.0.0/PKG-INFO` & `notion_export_prettify-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notion-export-prettify
-Version: 1.0.0
+Version: 1.1.0
 Summary: 
 Author: Fabre Lambeau
 Author-email: fabre.lambeau@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

