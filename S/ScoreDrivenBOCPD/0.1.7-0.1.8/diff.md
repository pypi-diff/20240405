# Comparing `tmp/ScoreDrivenBOCPD-0.1.7-py3-none-any.whl.zip` & `tmp/ScoreDrivenBOCPD-0.1.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,13 @@
-Zip file size: 8758 bytes, number of entries: 10
+Zip file size: 9458 bytes, number of entries: 11
 -rw-rw-rw-  2.0 fat       34 b- defN 24-Apr-03 14:55 ScoreDrivenBOCPD/__init__.py
 -rw-rw-rw-  2.0 fat     2156 b- defN 24-Apr-05 08:39 ScoreDrivenBOCPD/data.py
--rw-rw-rw-  2.0 fat     6417 b- defN 24-Apr-05 08:54 ScoreDrivenBOCPD/prob_model.py
+-rw-rw-rw-  2.0 fat     6434 b- defN 24-Apr-05 09:30 ScoreDrivenBOCPD/prob_model.py
 -rw-rw-rw-  2.0 fat     2273 b- defN 24-Mar-22 06:47 ScoreDrivenBOCPD/sd_ar.py
 -rw-rw-rw-  2.0 fat     7711 b- defN 24-Apr-05 08:27 ScoreDrivenBOCPD/sd_bocpd.py
--rw-rw-rw-  2.0 fat     1093 b- defN 24-Apr-05 09:13 ScoreDrivenBOCPD-0.1.7.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      382 b- defN 24-Apr-05 09:13 ScoreDrivenBOCPD-0.1.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-05 09:13 ScoreDrivenBOCPD-0.1.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 24-Apr-05 09:13 ScoreDrivenBOCPD-0.1.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      848 b- defN 24-Apr-05 09:13 ScoreDrivenBOCPD-0.1.7.dist-info/RECORD
-10 files, 21023 bytes uncompressed, 7298 bytes compressed:  65.3%
+-rw-rw-rw-  2.0 fat     1181 b- defN 24-Apr-05 08:30 ScoreDrivenBOCPD/untitled1.py
+-rw-rw-rw-  2.0 fat     1093 b- defN 24-Apr-05 09:33 ScoreDrivenBOCPD-0.1.8.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      382 b- defN 24-Apr-05 09:33 ScoreDrivenBOCPD-0.1.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-05 09:33 ScoreDrivenBOCPD-0.1.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 24-Apr-05 09:33 ScoreDrivenBOCPD-0.1.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      934 b- defN 24-Apr-05 09:33 ScoreDrivenBOCPD-0.1.8.dist-info/RECORD
+11 files, 22307 bytes uncompressed, 7864 bytes compressed:  64.7%
```

## zipnote {}

```diff
@@ -9,23 +9,26 @@
 
 Filename: ScoreDrivenBOCPD/sd_ar.py
 Comment: 
 
 Filename: ScoreDrivenBOCPD/sd_bocpd.py
 Comment: 
 
-Filename: ScoreDrivenBOCPD-0.1.7.dist-info/LICENSE
+Filename: ScoreDrivenBOCPD/untitled1.py
 Comment: 
 
-Filename: ScoreDrivenBOCPD-0.1.7.dist-info/METADATA
+Filename: ScoreDrivenBOCPD-0.1.8.dist-info/LICENSE
 Comment: 
 
-Filename: ScoreDrivenBOCPD-0.1.7.dist-info/WHEEL
+Filename: ScoreDrivenBOCPD-0.1.8.dist-info/METADATA
 Comment: 
 
-Filename: ScoreDrivenBOCPD-0.1.7.dist-info/top_level.txt
+Filename: ScoreDrivenBOCPD-0.1.8.dist-info/WHEEL
 Comment: 
 
-Filename: ScoreDrivenBOCPD-0.1.7.dist-info/RECORD
+Filename: ScoreDrivenBOCPD-0.1.8.dist-info/top_level.txt
+Comment: 
+
+Filename: ScoreDrivenBOCPD-0.1.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ScoreDrivenBOCPD/prob_model.py

```diff
@@ -7,15 +7,15 @@
 Bayesian Change-Point Detection Methods" 
 by Tsaknaki,Lillo,Mazzarisi, 2023
 
 see: https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4500960 
 """
 import numpy as np
 from   scipy.stats import norm
-import sd_ar as sd
+import ScoreDrivenBOCPD.sd_ar as sd
 
 
 class GaussianModel:
     
     def __init__(self, mean0, var0, varx, init_theta, q, init_cor = 0):
         
         varx = 1e-8 + varx
```

## Comparing `ScoreDrivenBOCPD-0.1.7.dist-info/LICENSE` & `ScoreDrivenBOCPD-0.1.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ScoreDrivenBOCPD-0.1.7.dist-info/RECORD` & `ScoreDrivenBOCPD-0.1.8.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 ScoreDrivenBOCPD/__init__.py,sha256=MHuUwF05F2TPiYu5QDp2yIpuRqw07SBGQyC5Qp05dgE,34
 ScoreDrivenBOCPD/data.py,sha256=CC5FxsuzDF7v-UxBmYJVn7BpFktpwX2N8bglPu5oZVw,2156
-ScoreDrivenBOCPD/prob_model.py,sha256=mTPkmViq-RcEojKjnhMO5qUXFuHV7jiUK2mnNV5Hwoo,6417
+ScoreDrivenBOCPD/prob_model.py,sha256=FXQMFsYiniyn1hi_dF4VYrdrdFEiCZCz7vN178DgxQI,6434
 ScoreDrivenBOCPD/sd_ar.py,sha256=qPVxciaaahB7rC4FF5xcrkG9iiXQPptaYS-Wb5t25ek,2273
 ScoreDrivenBOCPD/sd_bocpd.py,sha256=xTp7rm5DWTE9x_RoS2NAMJO0iv3UzoFUCXQpoqLGeYE,7711
-ScoreDrivenBOCPD-0.1.7.dist-info/LICENSE,sha256=tqaU2RKeRvOViWELR1Jc-XujDbQku657gN6LbIw1mvw,1093
-ScoreDrivenBOCPD-0.1.7.dist-info/METADATA,sha256=BFWsErtqtUurDgP5aqg0ZRjcrzEvrqFJ7jXs5X_T9FU,382
-ScoreDrivenBOCPD-0.1.7.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-ScoreDrivenBOCPD-0.1.7.dist-info/top_level.txt,sha256=z4HtCrg_hwaOBm6rmY9ylxXWRWZ5qgIpcepyEqtpPGQ,17
-ScoreDrivenBOCPD-0.1.7.dist-info/RECORD,,
+ScoreDrivenBOCPD/untitled1.py,sha256=-oWlCILiVcsGJLQhrz5fbdohn8gs4ffQvPf7TqqASCs,1181
+ScoreDrivenBOCPD-0.1.8.dist-info/LICENSE,sha256=tqaU2RKeRvOViWELR1Jc-XujDbQku657gN6LbIw1mvw,1093
+ScoreDrivenBOCPD-0.1.8.dist-info/METADATA,sha256=-asDiuclKhCCByn3PDUSJ6JpxmYZFJTMAL2yqSrplO8,382
+ScoreDrivenBOCPD-0.1.8.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+ScoreDrivenBOCPD-0.1.8.dist-info/top_level.txt,sha256=z4HtCrg_hwaOBm6rmY9ylxXWRWZ5qgIpcepyEqtpPGQ,17
+ScoreDrivenBOCPD-0.1.8.dist-info/RECORD,,
```

