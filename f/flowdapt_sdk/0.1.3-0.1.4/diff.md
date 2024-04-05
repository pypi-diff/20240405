# Comparing `tmp/flowdapt_sdk-0.1.3-py3-none-any.whl.zip` & `tmp/flowdapt_sdk-0.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 21396 bytes, number of entries: 31
+Zip file size: 21388 bytes, number of entries: 31
 -rw-r--r--  2.0 unx      227 b- defN 80-Jan-01 00:00 flowdapt_sdk/__init__.py
 -rw-r--r--  2.0 unx     1885 b- defN 80-Jan-01 00:00 flowdapt_sdk/_compat.py
 -rw-r--r--  2.0 unx      418 b- defN 80-Jan-01 00:00 flowdapt_sdk/api/__init__.py
 -rw-r--r--  2.0 unx      139 b- defN 80-Jan-01 00:00 flowdapt_sdk/api/base.py
--rw-r--r--  2.0 unx     6203 b- defN 80-Jan-01 00:00 flowdapt_sdk/api/configs.py
+-rw-r--r--  2.0 unx     6298 b- defN 80-Jan-01 00:00 flowdapt_sdk/api/configs.py
 -rw-r--r--  2.0 unx     2162 b- defN 80-Jan-01 00:00 flowdapt_sdk/api/metrics.py
 -rw-r--r--  2.0 unx     4194 b- defN 80-Jan-01 00:00 flowdapt_sdk/api/plugins.py
 -rw-r--r--  2.0 unx     1415 b- defN 80-Jan-01 00:00 flowdapt_sdk/api/system.py
 -rw-r--r--  2.0 unx     6445 b- defN 80-Jan-01 00:00 flowdapt_sdk/api/triggers.py
 -rw-r--r--  2.0 unx    11208 b- defN 80-Jan-01 00:00 flowdapt_sdk/api/workflows.py
 -rw-r--r--  2.0 unx     8822 b- defN 80-Jan-01 00:00 flowdapt_sdk/client.py
 -rw-r--r--  2.0 unx       35 b- defN 80-Jan-01 00:00 flowdapt_sdk/constants.py
@@ -22,12 +22,12 @@
 -rw-r--r--  2.0 unx     2336 b- defN 80-Jan-01 00:00 flowdapt_sdk/dto/triggers.py
 -rw-r--r--  2.0 unx     3088 b- defN 80-Jan-01 00:00 flowdapt_sdk/dto/workflows.py
 -rw-r--r--  2.0 unx     1249 b- defN 80-Jan-01 00:00 flowdapt_sdk/errors.py
 -rw-r--r--  2.0 unx     1842 b- defN 80-Jan-01 00:00 flowdapt_sdk/sdk.py
 -rw-r--r--  2.0 unx      172 b- defN 80-Jan-01 00:00 flowdapt_sdk/serialize.py
 -rw-r--r--  2.0 unx     2400 b- defN 80-Jan-01 00:00 flowdapt_sdk/utils.py
 -rw-r--r--  2.0 unx       22 b- defN 80-Jan-01 00:00 flowdapt_sdk/version.py
--rw-r--r--  2.0 unx     1073 b- defN 80-Jan-01 00:00 flowdapt_sdk-0.1.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     2028 b- defN 80-Jan-01 00:00 flowdapt_sdk-0.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 flowdapt_sdk-0.1.3.dist-info/WHEEL
-?rw-r--r--  2.0 unx     2531 b- defN 16-Jan-01 00:00 flowdapt_sdk-0.1.3.dist-info/RECORD
-31 files, 70555 bytes uncompressed, 17358 bytes compressed:  75.4%
+-rw-r--r--  2.0 unx     1073 b- defN 80-Jan-01 00:00 flowdapt_sdk-0.1.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2028 b- defN 80-Jan-01 00:00 flowdapt_sdk-0.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 flowdapt_sdk-0.1.4.dist-info/WHEEL
+?rw-r--r--  2.0 unx     2531 b- defN 16-Jan-01 00:00 flowdapt_sdk-0.1.4.dist-info/RECORD
+31 files, 70650 bytes uncompressed, 17350 bytes compressed:  75.4%
```

## zipnote {}

```diff
@@ -75,20 +75,20 @@
 
 Filename: flowdapt_sdk/utils.py
 Comment: 
 
 Filename: flowdapt_sdk/version.py
 Comment: 
 
-Filename: flowdapt_sdk-0.1.3.dist-info/LICENSE
+Filename: flowdapt_sdk-0.1.4.dist-info/LICENSE
 Comment: 
 
-Filename: flowdapt_sdk-0.1.3.dist-info/METADATA
+Filename: flowdapt_sdk-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: flowdapt_sdk-0.1.3.dist-info/WHEEL
+Filename: flowdapt_sdk-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: flowdapt_sdk-0.1.3.dist-info/RECORD
+Filename: flowdapt_sdk-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## flowdapt_sdk/api/configs.py

```diff
@@ -152,23 +152,28 @@
             headers={APIVersionHeader: build_version_header(ResourceType, version)},
             accept=[(response_dto.__content_type__, 1.0)],
             params={"identifier": identifier}
         )
 
         return validate_model(response_dto, response.content)
 
-    async def delete_config(self, identifier: str | UUID, version: str | None = None) -> None:
+    async def delete_config(
+        self,
+        identifier: str | UUID,
+        version: str | None = None,
+    ) -> ConfigReadResponse:
         """
         Delete a config by its identifier.
 
         :param identifier: The identifier of the config.
         :type identifier: str | UUID
         :param version: The version of the DTO to use. Defaults to the latest supported version.
         :type version: str | None
-        :return: None
+        :return: The deleted config.
+        :rtype: ConfigReadResponse
         """
         response_dto, _, version = build_request_data(ConfigReadRequestDTOs, version=version)
 
         response = await self.client.delete(
             endpoint=f"/configs/{identifier}",
             headers={APIVersionHeader: build_version_header(ResourceType, version)},
             accept=[(response_dto.__content_type__, 1.0)],
```

## Comparing `flowdapt_sdk-0.1.3.dist-info/LICENSE` & `flowdapt_sdk-0.1.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `flowdapt_sdk-0.1.3.dist-info/METADATA` & `flowdapt_sdk-0.1.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowdapt_sdk
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python SDK for Flowdapt
 Home-page: https://gitlab.com/emergentmethods/flowdapt-python-sdk
 License: MIT
 Author: Emergent Methods
 Author-email: contact@emergentmethods.ai
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `flowdapt_sdk-0.1.3.dist-info/RECORD` & `flowdapt_sdk-0.1.4.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 flowdapt_sdk/__init__.py,sha256=RFWxkEJG3SpUmiQhcaSxZvIfdQysFdb7gCCqToMKc-0,227
 flowdapt_sdk/_compat.py,sha256=BY1dRLoyE22XsW4UoWZk7yIOKWlemprLGPqFl1G2rdE,1885
 flowdapt_sdk/api/__init__.py,sha256=QTZHblyMjjyoQfmMSIe1Qs7bc4N6wWpjTMelPTRrOw0,418
 flowdapt_sdk/api/base.py,sha256=wARM0r_8xvCUgAPy_b2FcDsdk73i1jcY3BcGRrnZLpg,139
-flowdapt_sdk/api/configs.py,sha256=x0mgJ76SlqgkbVs8HUUe3X3_aBOV83eEMi6Do192CdE,6203
+flowdapt_sdk/api/configs.py,sha256=4ryx601-u_jXcnP4Qgq_Z6b2IwSqu5nGXqMRv_bzEHU,6298
 flowdapt_sdk/api/metrics.py,sha256=wBzWDNurXXrLpwYxsiO1Pujtieyr34oz_Kp1wxjBTm8,2162
 flowdapt_sdk/api/plugins.py,sha256=0OIVYAam7J5F1pZfiGTUDAtDJRFJzqK0-YDPpM3C8OA,4194
 flowdapt_sdk/api/system.py,sha256=x3ebLpmTmRRUH9703nD7BVJlqn3t5d5kO0w83of21xg,1415
 flowdapt_sdk/api/triggers.py,sha256=FOp-OZv_3Oy822iK5eN_CEpwQhjDBDNSsTnNzDM42Q4,6445
 flowdapt_sdk/api/workflows.py,sha256=6VVYT_4DHeaCzXCLO0GQdrLuskotCKnmr476i0nISbs,11208
 flowdapt_sdk/client.py,sha256=SbcfuHyBsp6DGd62ldmrsC9CHMb8bJvO3-0nQ1l7MB0,8822
 flowdapt_sdk/constants.py,sha256=2Ou6j4B7zi9c7-oZLdLqzST7n6kIjnpUGdTvxJSLdDI,35
@@ -21,11 +21,11 @@
 flowdapt_sdk/dto/triggers.py,sha256=nn8daHjEFLFJqhOfwtkdrhWR1RLWN8KVACt8uJ6YVQ4,2336
 flowdapt_sdk/dto/workflows.py,sha256=p2az4NptrlHqMjW9kbn3QNZVl_XLZaok-9A6M2rLa4w,3088
 flowdapt_sdk/errors.py,sha256=yTNgjfQNIZXBvt2MCBoGQSqdqud39pcnLgl6deFf6Dc,1249
 flowdapt_sdk/sdk.py,sha256=Adh-UwqykMIMZFiGc5xT5i8wPNMjRe8JHYdVcHpTbHo,1842
 flowdapt_sdk/serialize.py,sha256=KKc4AbAz_Bc9f_qzBcbJqU3HWnZidSK3-M-n7JHXEpo,172
 flowdapt_sdk/utils.py,sha256=7DMBCN63DoBK76auaTN_XUNprxrwd2NGUcNY0DGXpgk,2400
 flowdapt_sdk/version.py,sha256=J-j-u0itpEFT6irdmWmixQqYMadNl1X91TxUmoiLHMI,22
-flowdapt_sdk-0.1.3.dist-info/LICENSE,sha256=PphLPr74YBd3DwU0qher5XzGzcSJdOH9MYgApVO6wIo,1073
-flowdapt_sdk-0.1.3.dist-info/METADATA,sha256=GM3hRtK43dOBbLS_ItPt9QgUYcOOgxP7yN0jJtIIyus,2028
-flowdapt_sdk-0.1.3.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-flowdapt_sdk-0.1.3.dist-info/RECORD,,
+flowdapt_sdk-0.1.4.dist-info/LICENSE,sha256=PphLPr74YBd3DwU0qher5XzGzcSJdOH9MYgApVO6wIo,1073
+flowdapt_sdk-0.1.4.dist-info/METADATA,sha256=Nm1UwzqL59K7nsE1A3YORACrc9HQyMrUB4DehBL5PvQ,2028
+flowdapt_sdk-0.1.4.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+flowdapt_sdk-0.1.4.dist-info/RECORD,,
```

