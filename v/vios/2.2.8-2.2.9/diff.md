# Comparing `tmp/vios-2.2.8-py3-none-any.whl.zip` & `tmp/vios-2.2.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 46664 bytes, number of entries: 25
+Zip file size: 46668 bytes, number of entries: 25
 -rw-rw-rw-  2.0 fat     2858 b- defN 24-Mar-19 11:19 quark/__main__.py
--rw-rw-rw-  2.0 fat    18903 b- defN 24-Apr-05 13:13 quark/proxy.py
+-rw-rw-rw-  2.0 fat    18911 b- defN 24-Apr-05 13:39 quark/proxy.py
 -rw-rw-rw-  2.0 fat    18861 b- defN 24-Mar-21 10:46 quark/app/__init__.py
 -rw-rw-rw-  2.0 fat     2575 b- defN 24-Mar-19 11:19 quark/app/_data.py
 -rw-rw-rw-  2.0 fat    10205 b- defN 24-Mar-19 11:19 quark/app/demo.py
 -rw-rw-rw-  2.0 fat     9043 b- defN 24-Mar-19 11:19 quark/app/task.py
 -rw-rw-rw-  2.0 fat     5876 b- defN 24-Mar-19 11:19 quark/app/uapi.py
 -rw-rw-rw-  2.0 fat     7914 b- defN 24-Mar-19 11:19 quark/driver/VirtualDevice.py
 -rw-rw-rw-  2.0 fat      386 b- defN 24-Mar-19 11:19 quark/driver/__init__.py
@@ -15,13 +15,13 @@
 -rw-rw-rw-  2.0 fat     1188 b- defN 24-Mar-19 11:19 quark/envelope/__init__.py
 -rw-rw-rw-  2.0 fat    15111 b- defN 24-Mar-19 11:19 quark/envelope/assembler.py
 -rw-rw-rw-  2.0 fat     4322 b- defN 24-Mar-19 11:19 quark/envelope/calculator.py
 -rw-rw-rw-  2.0 fat     1106 b- defN 24-Mar-19 11:19 quark/envelope/device.py
 -rw-rw-rw-  2.0 fat     3758 b- defN 24-Mar-23 03:45 quark/envelope/processor.py
 -rw-rw-rw-  2.0 fat     4224 b- defN 24-Apr-04 12:39 quark/envelope/router.py
 -rw-rw-rw-  2.0 fat     2841 b- defN 24-Mar-21 12:16 quark/envelope/systemq.py
--rw-rw-rw-  2.0 fat     1085 b- defN 24-Apr-05 13:20 vios-2.2.8.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1211 b- defN 24-Apr-05 13:20 vios-2.2.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-05 13:20 vios-2.2.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 24-Apr-05 13:20 vios-2.2.8.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1995 b- defN 24-Apr-05 13:20 vios-2.2.8.dist-info/RECORD
-25 files, 128350 bytes uncompressed, 43488 bytes compressed:  66.1%
+-rw-rw-rw-  2.0 fat     1085 b- defN 24-Apr-05 13:42 vios-2.2.9.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1211 b- defN 24-Apr-05 13:42 vios-2.2.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-05 13:42 vios-2.2.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 24-Apr-05 13:42 vios-2.2.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1995 b- defN 24-Apr-05 13:42 vios-2.2.9.dist-info/RECORD
+25 files, 128358 bytes uncompressed, 43492 bytes compressed:  66.1%
```

## zipnote {}

```diff
@@ -54,23 +54,23 @@
 
 Filename: quark/envelope/router.py
 Comment: 
 
 Filename: quark/envelope/systemq.py
 Comment: 
 
-Filename: vios-2.2.8.dist-info/LICENSE
+Filename: vios-2.2.9.dist-info/LICENSE
 Comment: 
 
-Filename: vios-2.2.8.dist-info/METADATA
+Filename: vios-2.2.9.dist-info/METADATA
 Comment: 
 
-Filename: vios-2.2.8.dist-info/WHEEL
+Filename: vios-2.2.9.dist-info/WHEEL
 Comment: 
 
-Filename: vios-2.2.8.dist-info/top_level.txt
+Filename: vios-2.2.9.dist-info/top_level.txt
 Comment: 
 
-Filename: vios-2.2.8.dist-info/RECORD
+Filename: vios-2.2.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## quark/proxy.py

```diff
@@ -458,15 +458,15 @@
 
     def cancel(self, tid: int):
         return self.server.cancel(tid)
 
     def status(self, tid: int = 0):
         if not tid:
             pending = []
-            for tid, task in self.server.getid(True):
+            for tid, task in self.server.getid(True).items():
                 if 'Pending' in task:
                     pending.append(tid)
             return len(pending)
         else:
             return self.server.track(tid)['status']
 
     def result(self, tid: int, raw: bool = False):
```

## Comparing `vios-2.2.8.dist-info/LICENSE` & `vios-2.2.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `vios-2.2.8.dist-info/METADATA` & `vios-2.2.9.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vios
-Version: 2.2.8
+Version: 2.2.9
 Summary: runtime requirements for systemq
 Author-email: YL Feng <fengyl@baqis.ac.cn>
 Project-URL: homepage, https://gitee.com
 Project-URL: bugs, https://gitee.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

## Comparing `vios-2.2.8.dist-info/RECORD` & `vios-2.2.9.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 quark/__main__.py,sha256=ky318p_RHmGRdMyzIL2meu-JOgqzRrH-hWfFvhceZGE,2858
-quark/proxy.py,sha256=sZWcb7DkHqoAOs7-PGZVXoU92uXn5ku7ZBY_hb1BaKQ,18903
+quark/proxy.py,sha256=dQfdU1SoQ5sJR1zVpTmTeoPDSOGeJNbCSUvTJPIT_Ko,18911
 quark/app/__init__.py,sha256=MjOh4mkjvwFzEEfPNv-dMOcoktAtYCBtl-P5_UA7MzQ,18861
 quark/app/_data.py,sha256=EGGTD2FrZ8vlbMh4jlmWhYk4fEG3FolGoWaQ26qxoss,2575
 quark/app/demo.py,sha256=eod5vSXKB0XI-Rr8UVKkNc9tOUfWCjI109Imd8bKmuo,10205
 quark/app/task.py,sha256=QEZuNia59sLEWa8pl2XIjItx2NismSTPZFnFt8-90HM,9043
 quark/app/uapi.py,sha256=itjEa89SUXozZqBGLH-3o4mKtRssNQODDj60knC-cGE,5876
 quark/driver/VirtualDevice.py,sha256=Cswl_ykFhIsocGV6Okh_YS1b48FeLm2fh1ruXqmNoyw,7914
 quark/driver/__init__.py,sha256=p1pVx1xTulBT8-qdp_zJ859tdIsA92XdvwrkqcVHL4s,386
@@ -14,12 +14,12 @@
 quark/envelope/__init__.py,sha256=5_cs0tZ7mV4GjOsY2isx8sUQu4u6Y3WN-9DUGG27SQM,1188
 quark/envelope/assembler.py,sha256=ENwX7FutJvpg6_Wcm42_Zx-ddq40JozuYqHPwJp09ZA,15111
 quark/envelope/calculator.py,sha256=0rZAA46sWh_X8wOBmpBvmljqCV53ID4VHPX1cE_abEc,4322
 quark/envelope/device.py,sha256=5E3oWZ84IYnQdzlmzltgPyayYz_au7p7UIbFVpJUa0Q,1106
 quark/envelope/processor.py,sha256=uMIwu83a4SDZVM3OE5_WrBya_4jxtdcXPd6pYa0osrk,3758
 quark/envelope/router.py,sha256=wVx-rWnCZg_BrPV8fja4kjI5jiQ5vEoAyXsCtDpdBdA,4224
 quark/envelope/systemq.py,sha256=QAaHLv68C9UjMp9qHt9t-HJkOTpCkbHZTlNVOsAzIBc,2841
-vios-2.2.8.dist-info/LICENSE,sha256=B_BP5ebph3-SqRxXvo-6Bh7vzPL2nPY5qSFQfr7xM_s,1085
-vios-2.2.8.dist-info/METADATA,sha256=jTnVZniJigPdD2BqxAMV-s1MyTAyvS5rSRch_quNLn4,1211
-vios-2.2.8.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-vios-2.2.8.dist-info/top_level.txt,sha256=7SspgYXMW_50_NVkPj0EbFg4jFlGVsaIDfpqNsA1IMY,6
-vios-2.2.8.dist-info/RECORD,,
+vios-2.2.9.dist-info/LICENSE,sha256=B_BP5ebph3-SqRxXvo-6Bh7vzPL2nPY5qSFQfr7xM_s,1085
+vios-2.2.9.dist-info/METADATA,sha256=zQS7ExtZ485hD9MsYFdRMMcqHhwm_R0zzY2pIh8_bYk,1211
+vios-2.2.9.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+vios-2.2.9.dist-info/top_level.txt,sha256=7SspgYXMW_50_NVkPj0EbFg4jFlGVsaIDfpqNsA1IMY,6
+vios-2.2.9.dist-info/RECORD,,
```

