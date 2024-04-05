# Comparing `tmp/torchlens-0.1.8-py2.py3-none-any.whl.zip` & `tmp/torchlens-0.1.9-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 81008 bytes, number of entries: 10
+Zip file size: 81017 bytes, number of entries: 10
 -rw-r--r--  2.0 unx      252 b- defN 23-Sep-03 19:11 torchlens/__init__.py
 -rw-r--r--  2.0 unx    12794 b- defN 23-Sep-09 12:39 torchlens/constants.py
 -rw-r--r--  2.0 unx    17980 b- defN 23-Sep-17 14:17 torchlens/helper_funcs.py
--rw-r--r--  2.0 unx   287716 b- defN 23-Sep-21 18:24 torchlens/model_history.py
+-rw-r--r--  2.0 unx   287738 b- defN 23-Sep-24 13:36 torchlens/model_history.py
 -rw-r--r--  2.0 unx    14946 b- defN 23-Sep-09 12:05 torchlens/user_funcs.py
--rw-r--r--  2.0 unx    35130 b- defN 23-Sep-21 18:26 torchlens-0.1.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     1131 b- defN 23-Sep-21 18:26 torchlens-0.1.8.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Sep-21 18:26 torchlens-0.1.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Sep-21 18:26 torchlens-0.1.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      804 b- defN 23-Sep-21 18:26 torchlens-0.1.8.dist-info/RECORD
-10 files, 370873 bytes uncompressed, 79654 bytes compressed:  78.5%
+-rw-r--r--  2.0 unx    35130 b- defN 23-Sep-24 15:16 torchlens-0.1.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1131 b- defN 23-Sep-24 15:16 torchlens-0.1.9.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Sep-24 15:16 torchlens-0.1.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Sep-24 15:16 torchlens-0.1.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      804 b- defN 23-Sep-24 15:16 torchlens-0.1.9.dist-info/RECORD
+10 files, 370895 bytes uncompressed, 79663 bytes compressed:  78.5%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: torchlens/model_history.py
 Comment: 
 
 Filename: torchlens/user_funcs.py
 Comment: 
 
-Filename: torchlens-0.1.8.dist-info/LICENSE
+Filename: torchlens-0.1.9.dist-info/LICENSE
 Comment: 
 
-Filename: torchlens-0.1.8.dist-info/METADATA
+Filename: torchlens-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: torchlens-0.1.8.dist-info/WHEEL
+Filename: torchlens-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: torchlens-0.1.8.dist-info/top_level.txt
+Filename: torchlens-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: torchlens-0.1.8.dist-info/RECORD
+Filename: torchlens-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## torchlens/model_history.py

```diff
@@ -1290,15 +1290,15 @@
 
             # "Pre-hook" operations:
             module_address = module.tl_module_address
             module.tl_module_pass_num += 1
             module_pass_label = (module_address, module.tl_module_pass_num)
             module.tl_module_pass_labels.append(module_pass_label)
             input_tensors = get_vars_of_type_from_obj(
-                [args, kwargs], torch.Tensor, search_depth=4
+                [args, kwargs], torch.Tensor, [torch.nn.Parameter], search_depth=4
             )
             input_tensor_labels = set()
             for t in input_tensors:
                 tensor_entry = self.raw_tensor_dict[t.tl_tensor_label_raw]
                 input_tensor_labels.add(t.tl_tensor_label_raw)
                 module.tl_tensors_entered_labels.append(t.tl_tensor_label_raw)
                 tensor_entry.modules_entered.append(module_address)
```

## Comparing `torchlens-0.1.8.dist-info/LICENSE` & `torchlens-0.1.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `torchlens-0.1.8.dist-info/METADATA` & `torchlens-0.1.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchlens
-Version: 0.1.8
+Version: 0.1.9
 Summary: A package for extracting activations from PyTorch models
 Home-page: https://github.com/johnmarktaylor91/torchlens
 Author: JohnMark Taylor
 Author-email: johnmarkedwardtaylor@gmail.com
 License: GNU GPL v3
 Keywords: torch torchlens features
 Classifier: Development Status :: 3 - Alpha
```

