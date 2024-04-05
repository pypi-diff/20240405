# Comparing `tmp/sarufi-0.1.8-py3-none-any.whl.zip` & `tmp/sarufi-0.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 13210 bytes, number of entries: 6
--rw-r--r--  2.0 unx    32452 b- defN 23-Dec-13 13:22 sarufi/__init__.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Dec-13 13:34 sarufi-0.1.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     6273 b- defN 23-Dec-13 13:34 sarufi-0.1.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Dec-13 13:34 sarufi-0.1.8.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Dec-13 13:34 sarufi-0.1.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      457 b- defN 23-Dec-13 13:34 sarufi-0.1.8.dist-info/RECORD
-6 files, 50638 bytes uncompressed, 12388 bytes compressed:  75.5%
+Zip file size: 13203 bytes, number of entries: 6
+-rw-r--r--  2.0 unx    32452 b- defN 24-Apr-05 16:21 sarufi/__init__.py
+-rw-r--r--  2.0 unx    11357 b- defN 24-Apr-05 16:34 sarufi-0.1.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6253 b- defN 24-Apr-05 16:34 sarufi-0.1.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-05 16:34 sarufi-0.1.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 24-Apr-05 16:34 sarufi-0.1.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      457 b- defN 24-Apr-05 16:34 sarufi-0.1.9.dist-info/RECORD
+6 files, 50618 bytes uncompressed, 12381 bytes compressed:  75.5%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: sarufi/__init__.py
 Comment: 
 
-Filename: sarufi-0.1.8.dist-info/LICENSE
+Filename: sarufi-0.1.9.dist-info/LICENSE
 Comment: 
 
-Filename: sarufi-0.1.8.dist-info/METADATA
+Filename: sarufi-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: sarufi-0.1.8.dist-info/WHEEL
+Filename: sarufi-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: sarufi-0.1.8.dist-info/top_level.txt
+Filename: sarufi-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: sarufi-0.1.8.dist-info/RECORD
+Filename: sarufi-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sarufi/__init__.py

```diff
@@ -472,18 +472,18 @@
         if response.status_code == 200:
             return [Bot(data=bot, api_key=self.token) for bot in response.json()]
         return response.json()
 
     def _fetch_response(
         self, bot_id: int, chat_id: str, message: str, message_type: str, channel: str
     ):
-        url = self._BASE_URL + "conversation/"
+        url = self._BASE_URL + "conversation"
         if channel.lower() == "whatsapp":
             logger.info("Sending message to bot via whatsapp")
-            url = url + "whatsapp"
+            url = f"{url}/whatsapp"
 
         data = {
             "chat_id": chat_id,
             "bot_id": bot_id,
             "message": message,
             "message_type": message_type,
         }
```

## Comparing `sarufi-0.1.8.dist-info/LICENSE` & `sarufi-0.1.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sarufi-0.1.8.dist-info/METADATA` & `sarufi-0.1.9.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: sarufi
-Version: 0.1.8
+Version: 0.1.9
 Summary: Opensource python wrapper to Sarufi Conversation API
 Home-page: https://github.com/Neurotech-HQ/sarufi-python-sdk
+Download-URL: https://github.com/Neurotech-HQ/sarufi-python-sdk/archive/refs/tags/v0.0.2.tar.gz
 Author: Jordan Kalebu
 Author-email: isaackeinstein@gmail.com
 License: MIT
-Download-URL: https://github.com/Neurotech-HQ/sarufi-python-sdk/archive/refs/tags/v0.0.2.tar.gz
 Keywords: sarufi,Sarufi Python SDK,Conversation API python,Swahili Conversational API,Conversational platform Python
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -208,9 +207,7 @@
 Are you facing any issue with the usage of the package, please raise one
 
 ## Contributors
 
 1. [kalebu](https://github.com/kalebu/)
 2. [Anthony Mipawa](https://github.com/Tonyloyt)
 </samp>
-
-
```

