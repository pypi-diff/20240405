# Comparing `tmp/gammarer.aws-secure-cloudfront-origin-bucket-1.3.3.tar.gz` & `tmp/gammarer.aws-secure-cloudfront-origin-bucket-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammarer.aws-secure-cloudfront-origin-bucket-1.3.3.tar", last modified: Sun Mar 31 18:24:28 2024, max compression
+gzip compressed data, was "gammarer.aws-secure-cloudfront-origin-bucket-1.4.0.tar", last modified: Fri Apr  5 07:09:43 2024, max compression
```

## Comparing `gammarer.aws-secure-cloudfront-origin-bucket-1.3.3.tar` & `gammarer.aws-secure-cloudfront-origin-bucket-1.4.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 18:24:28.113794 gammarer.aws-secure-cloudfront-origin-bucket-1.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-31 18:24:10.000000 gammarer.aws-secure-cloudfront-origin-bucket-1.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-31 18:24:10.000000 gammarer.aws-secure-cloudfront-origin-bucket-1.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-03-31 18:24:28.113794 gammarer.aws-secure-cloudfront-origin-bucket-1.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-03-31 18:24:10.000000 gammarer.aws-secure-cloudfront-origin-bucket-1.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-31 18:24:10.000000 gammarer.aws-secure-cloudfront-origin-bucket-1.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 18:24:28.117794 gammarer.aws-secure-cloudfront-origin-bucket-1.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-03-31 18:24:10.000000 gammarer.aws-secure-cloudfront-origin-bucket-1.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 18:24:28.113794 gammarer.aws-secure-cloudfront-origin-bucket-1.3.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 18:24:28.113794 gammarer.aws-secure-cloudfront-origin-bucket-1.3.3/src/gammarer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 18:24:28.113794 gammarer.aws-secure-cloudfront-origin-bucket-1.3.3/src/gammarer/aws_secure_cloudfront_origin_bucket/
--rw-r--r--   0 runner    (1001) docker     (127)     7747 2024-03-31 18:24:10.000000 gammarer.aws-secure-cloudfront-origin-bucket-1.3.3/src/gammarer/aws_secure_cloudfront_origin_bucket/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 18:24:28.113794 gammarer.aws-secure-cloudfront-origin-bucket-1.3.3/src/gammarer/aws_secure_cloudfront_origin_bucket/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-31 18:24:10.000000 gammarer.aws-secure-cloudfront-origin-bucket-1.3.3/src/gammarer/aws_secure_cloudfront_origin_bucket/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29860 2024-03-31 18:24:10.000000 gammarer.aws-secure-cloudfront-origin-bucket-1.3.3/src/gammarer/aws_secure_cloudfront_origin_bucket/_jsii/aws-secure-cloudfront-origin-bucket@1.3.3.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 18:24:10.000000 gammarer.aws-secure-cloudfront-origin-bucket-1.3.3/src/gammarer/aws_secure_cloudfront_origin_bucket/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 18:24:28.113794 gammarer.aws-secure-cloudfront-origin-bucket-1.3.3/src/gammarer.aws_secure_cloudfront_origin_bucket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-03-31 18:24:28.000000 gammarer.aws-secure-cloudfront-origin-bucket-1.3.3/src/gammarer.aws_secure_cloudfront_origin_bucket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-03-31 18:24:28.000000 gammarer.aws-secure-cloudfront-origin-bucket-1.3.3/src/gammarer.aws_secure_cloudfront_origin_bucket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 18:24:28.000000 gammarer.aws-secure-cloudfront-origin-bucket-1.3.3/src/gammarer.aws_secure_cloudfront_origin_bucket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-31 18:24:28.000000 gammarer.aws-secure-cloudfront-origin-bucket-1.3.3/src/gammarer.aws_secure_cloudfront_origin_bucket.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-31 18:24:28.000000 gammarer.aws-secure-cloudfront-origin-bucket-1.3.3/src/gammarer.aws_secure_cloudfront_origin_bucket.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:09:43.149055 gammarer.aws-secure-cloudfront-origin-bucket-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-05 07:09:33.000000 gammarer.aws-secure-cloudfront-origin-bucket-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-05 07:09:33.000000 gammarer.aws-secure-cloudfront-origin-bucket-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-04-05 07:09:43.149055 gammarer.aws-secure-cloudfront-origin-bucket-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-04-05 07:09:33.000000 gammarer.aws-secure-cloudfront-origin-bucket-1.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-05 07:09:33.000000 gammarer.aws-secure-cloudfront-origin-bucket-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 07:09:43.149055 gammarer.aws-secure-cloudfront-origin-bucket-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-05 07:09:33.000000 gammarer.aws-secure-cloudfront-origin-bucket-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:09:43.145055 gammarer.aws-secure-cloudfront-origin-bucket-1.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:09:43.145055 gammarer.aws-secure-cloudfront-origin-bucket-1.4.0/src/gammarer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:09:43.149055 gammarer.aws-secure-cloudfront-origin-bucket-1.4.0/src/gammarer/aws_secure_cloudfront_origin_bucket/
+-rw-r--r--   0 runner    (1001) docker     (127)    12700 2024-04-05 07:09:33.000000 gammarer.aws-secure-cloudfront-origin-bucket-1.4.0/src/gammarer/aws_secure_cloudfront_origin_bucket/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:09:43.149055 gammarer.aws-secure-cloudfront-origin-bucket-1.4.0/src/gammarer/aws_secure_cloudfront_origin_bucket/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-05 07:09:33.000000 gammarer.aws-secure-cloudfront-origin-bucket-1.4.0/src/gammarer/aws_secure_cloudfront_origin_bucket/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32547 2024-04-05 07:09:33.000000 gammarer.aws-secure-cloudfront-origin-bucket-1.4.0/src/gammarer/aws_secure_cloudfront_origin_bucket/_jsii/aws-secure-cloudfront-origin-bucket@1.4.0.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 07:09:33.000000 gammarer.aws-secure-cloudfront-origin-bucket-1.4.0/src/gammarer/aws_secure_cloudfront_origin_bucket/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:09:43.149055 gammarer.aws-secure-cloudfront-origin-bucket-1.4.0/src/gammarer.aws_secure_cloudfront_origin_bucket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-04-05 07:09:43.000000 gammarer.aws-secure-cloudfront-origin-bucket-1.4.0/src/gammarer.aws_secure_cloudfront_origin_bucket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-05 07:09:43.000000 gammarer.aws-secure-cloudfront-origin-bucket-1.4.0/src/gammarer.aws_secure_cloudfront_origin_bucket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 07:09:43.000000 gammarer.aws-secure-cloudfront-origin-bucket-1.4.0/src/gammarer.aws_secure_cloudfront_origin_bucket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-05 07:09:43.000000 gammarer.aws-secure-cloudfront-origin-bucket-1.4.0/src/gammarer.aws_secure_cloudfront_origin_bucket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-05 07:09:43.000000 gammarer.aws-secure-cloudfront-origin-bucket-1.4.0/src/gammarer.aws_secure_cloudfront_origin_bucket.egg-info/top_level.txt
```

### Comparing `gammarer.aws-secure-cloudfront-origin-bucket-1.3.3/LICENSE` & `gammarer.aws-secure-cloudfront-origin-bucket-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gammarer.aws-secure-cloudfront-origin-bucket-1.3.3/PKG-INFO` & `gammarer.aws-secure-cloudfront-origin-bucket-1.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-secure-cloudfront-origin-bucket
-Version: 1.3.3
+Version: 1.4.0
 Summary: AWS CloudFront distribution origin S3 bucket.
 Home-page: https://github.com/gammarer/aws-secure-cloudfront-origin-bucket.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarer/aws-secure-cloudfront-origin-bucket.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -39,14 +39,18 @@
 
 ### TypeScript
 
 ```shell
 npm install @gammarer/aws-secure-cloudfront-origin-bucket
 # or
 yarn add @gammarer/aws-secure-cloudfront-origin-bucket
+# or
+pnpm add @gammarer/aws-secure-cloudfront-origin-bucket
+# or
+bun add @gammarer/aws-secure-cloudfront-origin-bucket
 ```
 
 ### Python
 
 ```shell
 pip install gammarer.aws-secure-cloudfront-origin-bucket
 ```
@@ -66,21 +70,38 @@
   <groupId>com.gammarer</groupId>
   <artifactId>aws-secure-cloudfront-origin-bucket</artifactId>
 </dependency>
 ```
 
 ## Example
 
+### for OAI(Origin Access Identity)
+
 ```python
-import { SecureCloudFrontOriginBucket } from '@gammarer/aws-secure-cloudfront-origin-bucket';
+import { SecureCloudFrontOriginBucket, SecureCloudFrontOriginType } from '@gammarer/aws-secure-cloudfront-origin-bucket';
 
 const oai = new cloudfront.OriginAccessIdentity(stack, 'OriginAccessIdentity');
 
 new SecureCloudFrontOriginBucket(stack, 'SecureCloudFrontOriginBucket', {
   bucketName: 'example-origin-bucket',
+  cloudFrontOriginType: SecureCloudFrontOriginType.ORIGIN_ACCESS_IDENTITY,
   cloudFrontOriginAccessIdentityS3CanonicalUserId: oai.cloudFrontOriginAccessIdentityS3CanonicalUserId,
 });
 ```
 
+### for OAC(Origin Access Control)
+
+```python
+import { SecureCloudFrontOriginBucket, SecureCloudFrontOriginType } from '@gammarer/aws-secure-cloudfront-origin-bucket';
+
+declare const s3Bucket: cloudfront.Distribution;
+
+new SecureCloudFrontOriginBucket(stack, 'SecureCloudFrontOriginBucket', {
+  bucketName: 'example-origin-bucket',
+  cloudFrontOriginType: SecureCloudFrontOriginType.ORIGIN_ACCESS_CONTROL,
+  cloudFrontArn: 'arn:aws:cloudfront::123456789:distribution/DISTRIBUTIONID',
+});
+```
+
 ## License
 
 This project is licensed under the Apache-2.0 License.
```

### Comparing `gammarer.aws-secure-cloudfront-origin-bucket-1.3.3/README.md` & `gammarer.aws-secure-cloudfront-origin-bucket-1.4.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -16,14 +16,18 @@
 
 ### TypeScript
 
 ```shell
 npm install @gammarer/aws-secure-cloudfront-origin-bucket
 # or
 yarn add @gammarer/aws-secure-cloudfront-origin-bucket
+# or
+pnpm add @gammarer/aws-secure-cloudfront-origin-bucket
+# or
+bun add @gammarer/aws-secure-cloudfront-origin-bucket
 ```
 
 ### Python
 
 ```shell
 pip install gammarer.aws-secure-cloudfront-origin-bucket
 ```
@@ -43,21 +47,38 @@
   <groupId>com.gammarer</groupId>
   <artifactId>aws-secure-cloudfront-origin-bucket</artifactId>
 </dependency>
 ```
 
 ## Example
 
+### for OAI(Origin Access Identity)
+
 ```python
-import { SecureCloudFrontOriginBucket } from '@gammarer/aws-secure-cloudfront-origin-bucket';
+import { SecureCloudFrontOriginBucket, SecureCloudFrontOriginType } from '@gammarer/aws-secure-cloudfront-origin-bucket';
 
 const oai = new cloudfront.OriginAccessIdentity(stack, 'OriginAccessIdentity');
 
 new SecureCloudFrontOriginBucket(stack, 'SecureCloudFrontOriginBucket', {
   bucketName: 'example-origin-bucket',
+  cloudFrontOriginType: SecureCloudFrontOriginType.ORIGIN_ACCESS_IDENTITY,
   cloudFrontOriginAccessIdentityS3CanonicalUserId: oai.cloudFrontOriginAccessIdentityS3CanonicalUserId,
 });
 ```
 
+### for OAC(Origin Access Control)
+
+```python
+import { SecureCloudFrontOriginBucket, SecureCloudFrontOriginType } from '@gammarer/aws-secure-cloudfront-origin-bucket';
+
+declare const s3Bucket: cloudfront.Distribution;
+
+new SecureCloudFrontOriginBucket(stack, 'SecureCloudFrontOriginBucket', {
+  bucketName: 'example-origin-bucket',
+  cloudFrontOriginType: SecureCloudFrontOriginType.ORIGIN_ACCESS_CONTROL,
+  cloudFrontArn: 'arn:aws:cloudfront::123456789:distribution/DISTRIBUTIONID',
+});
+```
+
 ## License
 
 This project is licensed under the Apache-2.0 License.
```

### Comparing `gammarer.aws-secure-cloudfront-origin-bucket-1.3.3/setup.py` & `gammarer.aws-secure-cloudfront-origin-bucket-1.4.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "gammarer.aws-secure-cloudfront-origin-bucket",
-    "version": "1.3.3",
+    "version": "1.4.0",
     "description": "AWS CloudFront distribution origin S3 bucket.",
     "license": "Apache-2.0",
     "url": "https://github.com/gammarer/aws-secure-cloudfront-origin-bucket.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "gammarer.aws_secure_cloudfront_origin_bucket",
         "gammarer.aws_secure_cloudfront_origin_bucket._jsii"
     ],
     "package_data": {
         "gammarer.aws_secure_cloudfront_origin_bucket._jsii": [
-            "aws-secure-cloudfront-origin-bucket@1.3.3.jsii.tgz"
+            "aws-secure-cloudfront-origin-bucket@1.4.0.jsii.tgz"
         ],
         "gammarer.aws_secure_cloudfront_origin_bucket": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `gammarer.aws-secure-cloudfront-origin-bucket-1.3.3/src/gammarer/aws_secure_cloudfront_origin_bucket/_jsii/__init__.py` & `gammarer.aws-secure-cloudfront-origin-bucket-1.4.0/src/gammarer/aws_secure_cloudfront_origin_bucket/_jsii/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 
 import aws_cdk._jsii
 import constructs._jsii
 import gammarer.aws_secure_bucket._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "@gammarer/aws-secure-cloudfront-origin-bucket",
-    "1.3.3",
+    "1.4.0",
     __name__[0:-6],
-    "aws-secure-cloudfront-origin-bucket@1.3.3.jsii.tgz",
+    "aws-secure-cloudfront-origin-bucket@1.4.0.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `gammarer.aws-secure-cloudfront-origin-bucket-1.3.3/src/gammarer.aws_secure_cloudfront_origin_bucket.egg-info/PKG-INFO` & `gammarer.aws-secure-cloudfront-origin-bucket-1.4.0/src/gammarer.aws_secure_cloudfront_origin_bucket.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-secure-cloudfront-origin-bucket
-Version: 1.3.3
+Version: 1.4.0
 Summary: AWS CloudFront distribution origin S3 bucket.
 Home-page: https://github.com/gammarer/aws-secure-cloudfront-origin-bucket.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarer/aws-secure-cloudfront-origin-bucket.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -39,14 +39,18 @@
 
 ### TypeScript
 
 ```shell
 npm install @gammarer/aws-secure-cloudfront-origin-bucket
 # or
 yarn add @gammarer/aws-secure-cloudfront-origin-bucket
+# or
+pnpm add @gammarer/aws-secure-cloudfront-origin-bucket
+# or
+bun add @gammarer/aws-secure-cloudfront-origin-bucket
 ```
 
 ### Python
 
 ```shell
 pip install gammarer.aws-secure-cloudfront-origin-bucket
 ```
@@ -66,21 +70,38 @@
   <groupId>com.gammarer</groupId>
   <artifactId>aws-secure-cloudfront-origin-bucket</artifactId>
 </dependency>
 ```
 
 ## Example
 
+### for OAI(Origin Access Identity)
+
 ```python
-import { SecureCloudFrontOriginBucket } from '@gammarer/aws-secure-cloudfront-origin-bucket';
+import { SecureCloudFrontOriginBucket, SecureCloudFrontOriginType } from '@gammarer/aws-secure-cloudfront-origin-bucket';
 
 const oai = new cloudfront.OriginAccessIdentity(stack, 'OriginAccessIdentity');
 
 new SecureCloudFrontOriginBucket(stack, 'SecureCloudFrontOriginBucket', {
   bucketName: 'example-origin-bucket',
+  cloudFrontOriginType: SecureCloudFrontOriginType.ORIGIN_ACCESS_IDENTITY,
   cloudFrontOriginAccessIdentityS3CanonicalUserId: oai.cloudFrontOriginAccessIdentityS3CanonicalUserId,
 });
 ```
 
+### for OAC(Origin Access Control)
+
+```python
+import { SecureCloudFrontOriginBucket, SecureCloudFrontOriginType } from '@gammarer/aws-secure-cloudfront-origin-bucket';
+
+declare const s3Bucket: cloudfront.Distribution;
+
+new SecureCloudFrontOriginBucket(stack, 'SecureCloudFrontOriginBucket', {
+  bucketName: 'example-origin-bucket',
+  cloudFrontOriginType: SecureCloudFrontOriginType.ORIGIN_ACCESS_CONTROL,
+  cloudFrontArn: 'arn:aws:cloudfront::123456789:distribution/DISTRIBUTIONID',
+});
+```
+
 ## License
 
 This project is licensed under the Apache-2.0 License.
```

### Comparing `gammarer.aws-secure-cloudfront-origin-bucket-1.3.3/src/gammarer.aws_secure_cloudfront_origin_bucket.egg-info/SOURCES.txt` & `gammarer.aws-secure-cloudfront-origin-bucket-1.4.0/src/gammarer.aws_secure_cloudfront_origin_bucket.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/gammarer.aws_secure_cloudfront_origin_bucket.egg-info/SOURCES.txt
 src/gammarer.aws_secure_cloudfront_origin_bucket.egg-info/dependency_links.txt
 src/gammarer.aws_secure_cloudfront_origin_bucket.egg-info/requires.txt
 src/gammarer.aws_secure_cloudfront_origin_bucket.egg-info/top_level.txt
 src/gammarer/aws_secure_cloudfront_origin_bucket/__init__.py
 src/gammarer/aws_secure_cloudfront_origin_bucket/py.typed
 src/gammarer/aws_secure_cloudfront_origin_bucket/_jsii/__init__.py
-src/gammarer/aws_secure_cloudfront_origin_bucket/_jsii/aws-secure-cloudfront-origin-bucket@1.3.3.jsii.tgz
+src/gammarer/aws_secure_cloudfront_origin_bucket/_jsii/aws-secure-cloudfront-origin-bucket@1.4.0.jsii.tgz
```

