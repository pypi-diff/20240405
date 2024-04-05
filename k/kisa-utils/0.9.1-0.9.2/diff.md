# Comparing `tmp/kisa_utils-0.9.1-py3-none-any.whl.zip` & `tmp/kisa_utils-0.9.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 20888 bytes, number of entries: 18
+Zip file size: 20925 bytes, number of entries: 18
 -rw-rw-r--  2.0 unx      364 b- defN 24-Feb-08 14:19 kisa_utils/__init__.py
 -rw-rw-r--  2.0 unx      627 b- defN 24-Feb-04 18:18 kisa_utils/codes.py
 -rw-rw-r--  2.0 unx     2013 b- defN 23-Oct-13 10:07 kisa_utils/config.py
 -rw-rw-r--  2.0 unx     6576 b- defN 23-Oct-11 15:56 kisa_utils/dates.py
--rw-rw-r--  2.0 unx    26111 b- defN 24-Feb-28 06:42 kisa_utils/db.py
+-rw-rw-r--  2.0 unx    26306 b- defN 24-Feb-29 17:28 kisa_utils/db.py
 -rw-rw-r--  2.0 unx     3321 b- defN 24-Feb-08 09:51 kisa_utils/encryption.py
 -rw-rw-r--  2.0 unx     1860 b- defN 23-Oct-11 15:57 kisa_utils/figures.py
 -rw-rw-r--  2.0 unx     2120 b- defN 23-Oct-13 11:53 kisa_utils/log.py
 -rw-rw-r--  2.0 unx     1702 b- defN 23-Oct-11 15:57 kisa_utils/remote.py
 -rw-rw-r--  2.0 unx     1256 b- defN 23-Oct-11 15:58 kisa_utils/standardize.py
 -rw-rw-r--  2.0 unx     6737 b- defN 23-Oct-20 16:01 kisa_utils/storage.py
 -rw-rw-r--  2.0 unx     8015 b- defN 24-Feb-08 14:15 kisa_utils/token.py
 -rw-rw-r--  2.0 unx       43 b- defN 23-Oct-11 11:44 kisa_utils/structures/__init__.py
 -rw-rw-r--  2.0 unx     1919 b- defN 23-Aug-31 10:31 kisa_utils/structures/validator.py
--rw-rw-r--  2.0 unx      374 b- defN 24-Feb-28 06:43 kisa_utils-0.9.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Feb-28 06:43 kisa_utils-0.9.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       33 b- defN 24-Feb-28 06:43 kisa_utils-0.9.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1414 b- defN 24-Feb-28 06:43 kisa_utils-0.9.1.dist-info/RECORD
-18 files, 64577 bytes uncompressed, 18598 bytes compressed:  71.2%
+-rw-rw-r--  2.0 unx      374 b- defN 24-Feb-29 17:29 kisa_utils-0.9.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Feb-29 17:29 kisa_utils-0.9.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       33 b- defN 24-Feb-29 17:29 kisa_utils-0.9.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1414 b- defN 24-Feb-29 17:29 kisa_utils-0.9.2.dist-info/RECORD
+18 files, 64772 bytes uncompressed, 18635 bytes compressed:  71.2%
```

## zipnote {}

```diff
@@ -36,20 +36,20 @@
 
 Filename: kisa_utils/structures/__init__.py
 Comment: 
 
 Filename: kisa_utils/structures/validator.py
 Comment: 
 
-Filename: kisa_utils-0.9.1.dist-info/METADATA
+Filename: kisa_utils-0.9.2.dist-info/METADATA
 Comment: 
 
-Filename: kisa_utils-0.9.1.dist-info/WHEEL
+Filename: kisa_utils-0.9.2.dist-info/WHEEL
 Comment: 
 
-Filename: kisa_utils-0.9.1.dist-info/top_level.txt
+Filename: kisa_utils-0.9.2.dist-info/top_level.txt
 Comment: 
 
-Filename: kisa_utils-0.9.1.dist-info/RECORD
+Filename: kisa_utils-0.9.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kisa_utils/db.py

```diff
@@ -97,14 +97,15 @@
 
         self._in_with_statement = False
         self.isOpen = False
         self.functions:dict = {}
         self._txnDecorated = False
         
         self.__transactionMode = True if transactionMode else False
+        self._closeOnExitContext = True
 
         if  path not in [':memory:', ':ram:',':RAM:']:
             while path.endswith('/'): path = path[:-1]
             if not path.endswith(f'.{__EXT__}') and not os.path.isfile(path):
                 path += f'.{__EXT__}'
 
             path_root = os.path.split(path)[0]
@@ -595,30 +596,32 @@
         if self.isOpen:
             self.db.execute('pragma optimize;')
             if self.__transactionMode:
                 pass # self.commitTransaction()
             else:
                 self.db.commit()
 
-            self.db.close()
-            # self.db, self.cursor = None,None
-            self.isOpen = False
+            if self._closeOnExitContext:
+                self.db.close()
+                # self.db, self.cursor = None,None
+                self.isOpen = False
 
     # @_checkContext
     def release(self):
         return self.close()
 
     # methods to add context to the handle
     def __enter__(self) -> 'Api':
         self._in_with_statement = True
         return self
 
     def __exit__(self, *args) -> bool:
         # args = [exc_type, exc_value, traceback]
         self.release()
+
         self._in_with_statement = False
 
         # False=propagate exceptions, True=supress them
         # you want to propagate exceptions so that the calling code can know what went wrong
         if args[0] is None:
             return True
         else:
@@ -659,23 +662,25 @@
 
             if not handle.isOpen:
                 reply['log'] = '[TXN-E02] failed to open database'
                 return reply
 
             with handle:
                 handle._txnDecorated = True
+                handle._closeOnExitContext = False
                 kwargs['handle'] = handle
                 funcReply = func(*args, **kwargs)
                 if (not isinstance(funcReply,dict)) or ('status' not in funcReply):
                     reply['log'] = '[TXN-E03] decorated function does not conform to the expected return structure'
                     return reply
 
                 if not funcReply['status']:
                     return funcReply
 
+                handle._closeOnExitContext = True
                 txnCommitReply = handle.commitTransaction()
                 if not txnCommitReply['status']:
                     return txnCommitReply
 
                 return funcReply
 
         return wrapper
```

## Comparing `kisa_utils-0.9.1.dist-info/RECORD` & `kisa_utils-0.9.2.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 kisa_utils/__init__.py,sha256=TxUjPE3Yu_-Ls46Au2f6TelkHi4jDvHPnJibc3gwYyg,364
 kisa_utils/codes.py,sha256=Qfq5JhLgqp7N6DXZLWFY1rh5EJSMielfaRnNr48e9DA,627
 kisa_utils/config.py,sha256=FZ-xGqyldN_4vrI8l6f9E7dbLLQnZtsOAGI1mP9loo0,2013
 kisa_utils/dates.py,sha256=47-OAKPUCkabyIxEhpJjtgkZG37NwsPf8JIQuqwvNiE,6576
-kisa_utils/db.py,sha256=Zypwr9Iwt24IYYGl1ELXydJ7RtMPA8E7SfDTgtV7dNA,26111
+kisa_utils/db.py,sha256=3JRxv3RN2CHL31kAUP1WzsRCsc8VQwPT08Frhihsmqs,26306
 kisa_utils/encryption.py,sha256=KF4kLQIkFBPMU4aQT5-fo87aPLsl7hkIgNbzcBANDC8,3321
 kisa_utils/figures.py,sha256=ossQHBR7T9rOV1yhQJLDbwrY23xf0RIGOmjcFH7P0ss,1860
 kisa_utils/log.py,sha256=EKBAVvDpY_hgALDCC6i-ARdqQzZwxBxxeHR4NsYgs9U,2120
 kisa_utils/remote.py,sha256=UMiq8wIEwNGNMLO-j0er-vOnjVIw-tP6BFaDYsbNsjA,1702
 kisa_utils/standardize.py,sha256=uyPddNa4RH2GneuPOZKRlbN70UYXIwv3fZkJ6hP6LVY,1256
 kisa_utils/storage.py,sha256=jcWyTYWkUzfL206V_ZVvPMCSbDqZkXb5TOBB_c2xZDw,6737
 kisa_utils/token.py,sha256=ReCIBsq95RMYCrDCyHgU1y_Eq-xp_PBpZiHxwsY6Fj4,8015
 kisa_utils/structures/__init__.py,sha256=A1kzyP4H7yYZbmVwg-S1hmSFQtjFCh_Phfbcmc6my14,43
 kisa_utils/structures/validator.py,sha256=2FQdhLAAVdJg7wSFNe-_NbPAb_mFHtsSBAUlkwQUOSM,1919
-kisa_utils-0.9.1.dist-info/METADATA,sha256=arcs9245m-StvVMaDDxUOC6V5Ho1q72bmDAZW8ySrqY,374
-kisa_utils-0.9.1.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-kisa_utils-0.9.1.dist-info/top_level.txt,sha256=qaX0laAi8F4Quk8EtmeewczncEc6b3aUZrMz8UX9kOI,33
-kisa_utils-0.9.1.dist-info/RECORD,,
+kisa_utils-0.9.2.dist-info/METADATA,sha256=TPS8oVERCZ9o411bTSez0F_Y1h9kGOGQ7zM_RMg9hyw,374
+kisa_utils-0.9.2.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+kisa_utils-0.9.2.dist-info/top_level.txt,sha256=qaX0laAi8F4Quk8EtmeewczncEc6b3aUZrMz8UX9kOI,33
+kisa_utils-0.9.2.dist-info/RECORD,,
```

