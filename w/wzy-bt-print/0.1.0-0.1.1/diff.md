# Comparing `tmp/wzy_bt_print-0.1.0.tar.gz` & `tmp/wzy_bt_print-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wzy_bt_print-0.1.0.tar", last modified: Thu Apr  4 14:26:08 2024, max compression
+gzip compressed data, was "wzy_bt_print-0.1.1.tar", last modified: Fri Apr  5 00:45:57 2024, max compression
```

## Comparing `wzy_bt_print-0.1.0.tar` & `wzy_bt_print-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 14:26:08.758419 wzy_bt_print-0.1.0/
--rw-rw-rw-   0        0        0     1071 2024-03-07 08:39:08.000000 wzy_bt_print-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      436 2024-04-04 14:26:08.758419 wzy_bt_print-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       20 2024-04-04 14:24:38.000000 wzy_bt_print-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-04 14:26:08.758419 wzy_bt_print-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      604 2024-04-04 14:23:42.000000 wzy_bt_print-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-04 14:26:08.695496 wzy_bt_print-0.1.0/wzy_bt_print/
--rw-rw-rw-   0        0        0     2131 2024-04-04 14:23:40.000000 wzy_bt_print-0.1.0/wzy_bt_print/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 14:26:08.742797 wzy_bt_print-0.1.0/wzy_bt_print.egg-info/
--rw-rw-rw-   0        0        0      436 2024-04-04 14:26:08.000000 wzy_bt_print-0.1.0/wzy_bt_print.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      195 2024-04-04 14:26:08.000000 wzy_bt_print-0.1.0/wzy_bt_print.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 14:26:08.000000 wzy_bt_print-0.1.0/wzy_bt_print.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-04 14:26:08.000000 wzy_bt_print-0.1.0/wzy_bt_print.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 00:45:57.273275 wzy_bt_print-0.1.1/
+-rw-rw-rw-   0        0        0     1071 2024-03-07 08:39:08.000000 wzy_bt_print-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      436 2024-04-05 00:45:57.273275 wzy_bt_print-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       20 2024-04-04 14:24:38.000000 wzy_bt_print-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-05 00:45:57.273275 wzy_bt_print-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      604 2024-04-05 00:44:18.000000 wzy_bt_print-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 00:45:57.199836 wzy_bt_print-0.1.1/wzy_bt_print/
+-rw-rw-rw-   0        0        0     2191 2024-04-05 00:45:18.000000 wzy_bt_print-0.1.1/wzy_bt_print/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 00:45:57.262446 wzy_bt_print-0.1.1/wzy_bt_print.egg-info/
+-rw-rw-rw-   0        0        0      436 2024-04-05 00:45:57.000000 wzy_bt_print-0.1.1/wzy_bt_print.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      195 2024-04-05 00:45:57.000000 wzy_bt_print-0.1.1/wzy_bt_print.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 00:45:57.000000 wzy_bt_print-0.1.1/wzy_bt_print.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-05 00:45:57.000000 wzy_bt_print-0.1.1/wzy_bt_print.egg-info/top_level.txt
```

### Comparing `wzy_bt_print-0.1.0/LICENSE` & `wzy_bt_print-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wzy_bt_print-0.1.0/setup.py` & `wzy_bt_print-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # setup.py
 
 from setuptools import setup, find_packages
 
 setup(
     name='wzy_bt_print',
-    version='0.1.0',
+    version='0.1.1',
     packages=find_packages(),
     install_requires=[
     ],
     description='Binary Tree Printout',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Dr. Zhiyuan Wang',
```

### Comparing `wzy_bt_print-0.1.0/wzy_bt_print/__init__.py` & `wzy_bt_print-0.1.1/wzy_bt_print/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 # wzy_bt_print/__init__.py
 
 def print_tree_helper(root, curr_index=0, index=False, delimiter='-'):
+    '''
+    helper function, abstract away. 
+    '''
     if root is None:
         return '', 0, 0, 0
 
     line1 = []
     line2 = []
     try:
         node_repr = str(root.data)
@@ -48,18 +51,18 @@
     for i in range(max(len(l_box), len(r_box))):
         l_line = l_box[i] if i < len(l_box) else ' ' * l_box_width
         r_line = r_box[i] if i < len(r_box) else ' ' * r_box_width
         new_box.append(l_line + gap + r_line)
 
     return new_box, len(new_box[0]), new_root_start, new_root_end
 
-def print_tree(root):
+def print_tree_new(root):
     '''
     Input: a root node
     Output: a vertical binary tree printout,
             without rotating your stiff neck :)
-    - 4 Apr 2024, Dr.Z.Wang, at Singapore
+    - 4 Apr 2024, Dr.Z.Wang, in Singapore
     '''
     lines, *_ = print_tree_helper(root)
     for line in lines:
         print(line)
```

