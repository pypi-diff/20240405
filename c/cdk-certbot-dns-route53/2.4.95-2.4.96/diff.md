# Comparing `tmp/cdk-certbot-dns-route53-2.4.95.tar.gz` & `tmp/cdk-certbot-dns-route53-2.4.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-certbot-dns-route53-2.4.95.tar", last modified: Wed Apr  3 00:26:48 2024, max compression
+gzip compressed data, was "cdk-certbot-dns-route53-2.4.96.tar", last modified: Thu Apr  4 00:27:23 2024, max compression
```

## Comparing `cdk-certbot-dns-route53-2.4.95.tar` & `cdk-certbot-dns-route53-2.4.96.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:26:48.870284 cdk-certbot-dns-route53-2.4.95/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-03 00:26:36.000000 cdk-certbot-dns-route53-2.4.95/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-03 00:26:36.000000 cdk-certbot-dns-route53-2.4.95/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-04-03 00:26:48.870284 cdk-certbot-dns-route53-2.4.95/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-04-03 00:26:36.000000 cdk-certbot-dns-route53-2.4.95/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-03 00:26:36.000000 cdk-certbot-dns-route53-2.4.95/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 00:26:48.870284 cdk-certbot-dns-route53-2.4.95/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-03 00:26:36.000000 cdk-certbot-dns-route53-2.4.95/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:26:48.866284 cdk-certbot-dns-route53-2.4.95/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:26:48.870284 cdk-certbot-dns-route53-2.4.95/src/cdk_certbot_dns_route53/
--rw-r--r--   0 runner    (1001) docker     (127)    36178 2024-04-03 00:26:36.000000 cdk-certbot-dns-route53-2.4.95/src/cdk_certbot_dns_route53/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:26:48.870284 cdk-certbot-dns-route53-2.4.95/src/cdk_certbot_dns_route53/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-03 00:26:36.000000 cdk-certbot-dns-route53-2.4.95/src/cdk_certbot_dns_route53/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33227 2024-04-03 00:26:36.000000 cdk-certbot-dns-route53-2.4.95/src/cdk_certbot_dns_route53/_jsii/cdk-certbot-dns-route53@2.4.95.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 00:26:36.000000 cdk-certbot-dns-route53-2.4.95/src/cdk_certbot_dns_route53/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:26:48.870284 cdk-certbot-dns-route53-2.4.95/src/cdk_certbot_dns_route53.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-04-03 00:26:48.000000 cdk-certbot-dns-route53-2.4.95/src/cdk_certbot_dns_route53.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-03 00:26:48.000000 cdk-certbot-dns-route53-2.4.95/src/cdk_certbot_dns_route53.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 00:26:48.000000 cdk-certbot-dns-route53-2.4.95/src/cdk_certbot_dns_route53.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-03 00:26:48.000000 cdk-certbot-dns-route53-2.4.95/src/cdk_certbot_dns_route53.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-03 00:26:48.000000 cdk-certbot-dns-route53-2.4.95/src/cdk_certbot_dns_route53.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:27:23.977557 cdk-certbot-dns-route53-2.4.96/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-04 00:27:10.000000 cdk-certbot-dns-route53-2.4.96/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-04 00:27:10.000000 cdk-certbot-dns-route53-2.4.96/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-04-04 00:27:23.977557 cdk-certbot-dns-route53-2.4.96/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-04-04 00:27:10.000000 cdk-certbot-dns-route53-2.4.96/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-04 00:27:10.000000 cdk-certbot-dns-route53-2.4.96/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 00:27:23.977557 cdk-certbot-dns-route53-2.4.96/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-04 00:27:10.000000 cdk-certbot-dns-route53-2.4.96/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:27:23.973557 cdk-certbot-dns-route53-2.4.96/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:27:23.973557 cdk-certbot-dns-route53-2.4.96/src/cdk_certbot_dns_route53/
+-rw-r--r--   0 runner    (1001) docker     (127)    36178 2024-04-04 00:27:10.000000 cdk-certbot-dns-route53-2.4.96/src/cdk_certbot_dns_route53/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:27:23.977557 cdk-certbot-dns-route53-2.4.96/src/cdk_certbot_dns_route53/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-04 00:27:10.000000 cdk-certbot-dns-route53-2.4.96/src/cdk_certbot_dns_route53/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33227 2024-04-04 00:27:10.000000 cdk-certbot-dns-route53-2.4.96/src/cdk_certbot_dns_route53/_jsii/cdk-certbot-dns-route53@2.4.96.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 00:27:10.000000 cdk-certbot-dns-route53-2.4.96/src/cdk_certbot_dns_route53/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:27:23.973557 cdk-certbot-dns-route53-2.4.96/src/cdk_certbot_dns_route53.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-04-04 00:27:23.000000 cdk-certbot-dns-route53-2.4.96/src/cdk_certbot_dns_route53.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-04 00:27:23.000000 cdk-certbot-dns-route53-2.4.96/src/cdk_certbot_dns_route53.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 00:27:23.000000 cdk-certbot-dns-route53-2.4.96/src/cdk_certbot_dns_route53.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-04 00:27:23.000000 cdk-certbot-dns-route53-2.4.96/src/cdk_certbot_dns_route53.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-04 00:27:23.000000 cdk-certbot-dns-route53-2.4.96/src/cdk_certbot_dns_route53.egg-info/top_level.txt
```

### Comparing `cdk-certbot-dns-route53-2.4.95/LICENSE` & `cdk-certbot-dns-route53-2.4.96/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-certbot-dns-route53-2.4.95/PKG-INFO` & `cdk-certbot-dns-route53-2.4.96/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-certbot-dns-route53
-Version: 2.4.95
+Version: 2.4.96
 Summary: Create Cron Job Via Lambda, to update certificate and put it to S3 Bucket.
 Home-page: https://github.com/neilkuan/cdk-certbot-dns-route53.git
 Author: Neil Kuan<guan840912@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/neilkuan/cdk-certbot-dns-route53.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-certbot-dns-route53-2.4.95/README.md` & `cdk-certbot-dns-route53-2.4.96/README.md`

 * *Files identical despite different names*

### Comparing `cdk-certbot-dns-route53-2.4.95/setup.py` & `cdk-certbot-dns-route53-2.4.96/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-certbot-dns-route53",
-    "version": "2.4.95",
+    "version": "2.4.96",
     "description": "Create Cron Job Via Lambda, to update certificate and put it to S3 Bucket.",
     "license": "Apache-2.0",
     "url": "https://github.com/neilkuan/cdk-certbot-dns-route53.git",
     "long_description_content_type": "text/markdown",
     "author": "Neil Kuan<guan840912@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_certbot_dns_route53",
         "cdk_certbot_dns_route53._jsii"
     ],
     "package_data": {
         "cdk_certbot_dns_route53._jsii": [
-            "cdk-certbot-dns-route53@2.4.95.jsii.tgz"
+            "cdk-certbot-dns-route53@2.4.96.jsii.tgz"
         ],
         "cdk_certbot_dns_route53": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `cdk-certbot-dns-route53-2.4.95/src/cdk_certbot_dns_route53/__init__.py` & `cdk-certbot-dns-route53-2.4.96/src/cdk_certbot_dns_route53/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-certbot-dns-route53-2.4.95/src/cdk_certbot_dns_route53/_jsii/__init__.py` & `cdk-certbot-dns-route53-2.4.96/src/cdk_certbot_dns_route53/_jsii/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 
 import aws_cdk._jsii
 import aws_cdk.aws_lambda_python_alpha._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "cdk-certbot-dns-route53",
-    "2.4.95",
+    "2.4.96",
     __name__[0:-6],
-    "cdk-certbot-dns-route53@2.4.95.jsii.tgz",
+    "cdk-certbot-dns-route53@2.4.96.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `cdk-certbot-dns-route53-2.4.95/src/cdk_certbot_dns_route53/_jsii/cdk-certbot-dns-route53@2.4.95.jsii.tgz` & `cdk-certbot-dns-route53-2.4.96/src/cdk_certbot_dns_route53/_jsii/cdk-certbot-dns-route53@2.4.96.jsii.tgz`

 * *Files 26% similar despite different names*

#### Comparing `cdk-certbot-dns-route53@2.4.95.jsii.tgz-content` & `cdk-certbot-dns-route53@2.4.96.jsii.tgz-content`

##### package/.jsii

###### Pretty-printed

 * *Similarity: 0.9444444444444444%*

 * *Differences: {"'fingerprint'": "'iStFBGNL2PYJGG5xWCJbP0d3pBA9FqFqHH7Ca5T3V0M='", "'version'": "'2.4.96'"}*

```diff
@@ -3689,15 +3689,15 @@
             }
         }
     },
     "description": "Create Cron Job Via Lambda, to update certificate and put it to S3 Bucket.",
     "docs": {
         "stability": "stable"
     },
-    "fingerprint": "ZmRSbdgw5ij17OEASAPW0Z9hNCY9vf6n2rbhgkU8Plc=",
+    "fingerprint": "iStFBGNL2PYJGG5xWCJbP0d3pBA9FqFqHH7Ca5T3V0M=",
     "homepage": "https://github.com/neilkuan/cdk-certbot-dns-route53.git",
     "jsiiVersion": "5.3.33 (build 023495c)",
     "keywords": [
         "aws",
         "cdk",
         "certbot"
     ],
@@ -4351,9 +4351,9 @@
                         "fqn": "@aws-cdk/aws-lambda-python-alpha.PythonFunction"
                     }
                 }
             ],
             "symbolId": "src/lambda-python:LambdaPythonFunction"
         }
     },
-    "version": "2.4.95"
+    "version": "2.4.96"
 }
```

##### package/lib/lambda-bash.js

###### js-beautify {}

```diff
@@ -33,10 +33,10 @@
         });
     }
 }
 exports.BashExecFunction = BashExecFunction;
 _a = JSII_RTTI_SYMBOL_1;
 BashExecFunction[_a] = {
     fqn: "cdk-certbot-dns-route53.BashExecFunction",
-    version: "2.4.95"
+    version: "2.4.96"
 };
 //# sourceMappingURL=data:application/json;base64,eyJ2ZXJzaW9uIjozLCJmaWxlIjoibGFtYmRhLWJhc2guanMiLCJzb3VyY2VSb290IjoiIiwic291cmNlcyI6WyIuLi9zcmMvbGFtYmRhLWJhc2gudHMiXSwibmFtZXMiOltdLCJtYXBwaW5ncyI6Ijs7Ozs7QUFBQSx5QkFBeUI7QUFDekIsNkJBQTZCO0FBQzdCLDZDQUFrRDtBQUVsRCxpREFBaUQ7QUFDakQsNkNBQTZDO0FBQzdDLDJDQUF1QztBQXdDdkMsTUFBYSxnQkFBaUIsU0FBUSxzQkFBUztJQUU3QyxZQUFZLEtBQWdCLEVBQUUsRUFBVSxFQUFFLEtBQTRCO1FBQ3BFLEtBQUssQ0FBQyxLQUFLLEVBQUUsRUFBRSxDQUFDLENBQUM7UUFFakIsTUFBTSxhQUFhLEdBQUcsSUFBSSxDQUFDLElBQUksQ0FBQyxTQUFTLEVBQUUsYUFBYSxDQUFDLENBQUM7UUFDMUQsTUFBTSxVQUFVLEdBQUcsS0FBSyxDQUFDLE1BQU0sQ0FBQztRQUVoQywyR0FBMkc7UUFDM0csTUFBTSxRQUFRLEdBQUcsSUFBSSxDQUFDLElBQUksQ0FBQyxhQUFhLEVBQUUsVUFBVSxDQUFDLENBQUM7UUFDdEQsRUFBRSxDQUFDLFlBQVksQ0FBQyxVQUFVLEVBQUUsUUFBUSxDQUFDLENBQUM7UUFFdEMsSUFBSSxDQUFDLE9BQU8sR0FBRyxJQUFJLE1BQU0sQ0FBQyxtQkFBbUIsQ0FBQyxJQUFJLEVBQUUsa0JBQWtCLEVBQUU7WUFDdEUsSUFBSSxFQUFFLE1BQU0sQ0FBQyxlQUFlLENBQUMsY0FBYyxDQUFDLGFBQWEsRUFBRSxFQUMxRCxDQUFDO1lBQ0YsT0FBTyxFQUFFLEtBQUssQ0FBQyxPQUFPLElBQUksc0JBQVEsQ0FBQyxPQUFPLENBQUMsRUFBRSxDQUFDO1lBQzlDLFlBQVksRUFBRSxJQUFJLENBQUMsYUFBYSxDQUFDLE9BQU87WUFDeEMsV0FBVyxFQUFFLEtBQUssQ0FBQyxXQUFXO1lBQzlCLElBQUksRUFBRSxLQUFLLENBQUMsSUFBSTtZQUNoQixZQUFZLEVBQUUsS0FBSyxDQUFDLFlBQVk7WUFDaEMsVUFBVSxFQUFFLElBQUk7U0FDakIsQ0FBQyxDQUFDO1FBQ0gsSUFBSSx1QkFBUyxDQUFDLElBQUksRUFBRSxVQUFVLEVBQUUsRUFBRSxLQUFLLEVBQUUsSUFBSSxDQUFDLE9BQU8sQ0FBQyxRQUFRLENBQUMsWUFBWSxFQUFFLENBQUMsQ0FBQztJQUNqRixDQUFDOztBQXZCSCw0Q0F3QkMiLCJzb3VyY2VzQ29udGVudCI6WyJpbXBvcnQgKiBhcyBmcyBmcm9tICdmcyc7XG5pbXBvcnQgKiBhcyBwYXRoIGZyb20gJ3BhdGgnO1xuaW1wb3J0IHsgQ2ZuT3V0cHV0LCBEdXJhdGlvbiB9IGZyb20gJ2F3cy1jZGstbGliJztcbmltcG9ydCAqIGFzIGlhbSBmcm9tICdhd3MtY2RrLWxpYi9hd3MtaWFtJztcbmltcG9ydCAqIGFzIGxhbWJkYSBmcm9tICdhd3MtY2RrLWxpYi9hd3MtbGFtYmRhJztcbmltcG9ydCAqIGFzIGxvZ3MgZnJvbSAnYXdzLWNkay1saWIvYXdzLWxvZ3MnO1xuaW1wb3J0IHsgQ29uc3RydWN0IH0gZnJvbSAnY29uc3RydWN0cyc7XG5cbmV4cG9ydCBpbnRlcmZhY2UgQmFzaEV4ZWNGdW5jdGlvblByb3BzIHtcbiAgLyoqXG4gICAqIFRoZSBwYXRoIG9mIHRoZSBzaGVsbCBzY3JpcHQgdG8gYmUgZXhlY3V0ZWQuXG4gICAqL1xuICByZWFkb25seSBzY3JpcHQ6IHN0cmluZztcblxuICAvKipcbiAgICogVGhlIHBhdGggb2YgeW91ciBjdXN0b20gZG9ja2VyZmlsZS5cbiAgICovXG4gIHJlYWRvbmx5IGRvY2tlcmZpbGU/OiBzdHJpbmc7XG5cbiAgLyoqXG4gICAqIExhbWJkYSBlbnZpcm9ubWVudCB2YXJpYWJsZXMuXG4gICAqL1xuICByZWFkb25seSBlbnZpcm9ubWVudD86IHsgW2tleTogc3RyaW5nXTogc3RyaW5nIH07XG5cbiAgLyoqXG4gICAqIFRoZSBmdW5jdGlvbiBleGVjdXRpb24gdGltZSAoaW4gc2Vjb25kcykgYWZ0ZXIgd2hpY2ggTGFtYmRhIHRlcm1pbmF0ZXMgdGhlIGZ1bmN0aW9uLlxuICAgKiBCZWNhdXNlIHRoZSBleGVjdXRpb24gdGltZSBhZmZlY3RzIGNvc3QsIHNldCB0aGlzIHZhbHVlIGJhc2VkIG9uIHRoZSBmdW5jdGlvbidzIGV4cGVjdGVkIGV4ZWN1dGlvbiB0aW1lLlxuICAgKiBAZGVmYXVsdCAtIER1cmF0aW9uLnNlY29uZHMoNjApXG4gICAqICovXG4gIHJlYWRvbmx5IHRpbWVvdXQ/OiBEdXJhdGlvbjtcblxuICAvKipcbiAgICogQ3VzdG9tIGxhbWJkYSBleGVjdXRpb24gcm9sZS5cbiAgICpcbiAgICogQGRlZmF1bHQgLSBhdXRvIGdlbmVyYXRlZCByb2xlLlxuICAgKi9cbiAgcmVhZG9ubHkgcm9sZT86IGlhbS5JUm9sZTtcblxuICAvKipcbiAgICogQ3VzdG9tIGxhbWJkYSBJbWFnZSBBcmNoaXRlY3R1cmUuXG4gICAqXG4gICAqIEBkZWZhdWx0IC0gbGFtYmRhLkFyY2hpdGVjdHVyZS5YODZfNjRcbiAgICovXG4gIHJlYWRvbmx5IGFyY2hpdGVjdHVyZT86IGxhbWJkYS5BcmNoaXRlY3R1cmU7XG59XG5cbmV4cG9ydCBjbGFzcyBCYXNoRXhlY0Z1bmN0aW9uIGV4dGVuZHMgQ29uc3RydWN0IHtcbiAgcmVhZG9ubHkgaGFuZGxlcjogbGFtYmRhLkRvY2tlckltYWdlRnVuY3Rpb247XG4gIGNvbnN0cnVjdG9yKHNjb3BlOiBDb25zdHJ1Y3QsIGlkOiBzdHJpbmcsIHByb3BzOiBCYXNoRXhlY0Z1bmN0aW9uUHJvcHMpIHtcbiAgICBzdXBlcihzY29wZSwgaWQpO1xuXG4gICAgY29uc3QgZG9ja2VyRGlyUGF0aCA9IHBhdGguam9pbihfX2Rpcm5hbWUsICcuLi9kb2NrZXIuZCcpO1xuICAgIGNvbnN0IHNjcmlwdFBhdGggPSBwcm9wcy5zY3JpcHQ7XG5cbiAgICAvLyBjb3B5IHRoZSB1c2VyIHNjcmlwdCB0byB0aGUgZG9ja2VyLmQgZGlyZWN0b3J5IGFzIG1haW4uc2ggc28gd2UgY2FuIGJ1bmRsZSBpdCB1cCBpbnRvIGEgbmV3IGRvY2tlciBpbWFnZVxuICAgIGNvbnN0IG1haW5GaWxlID0gcGF0aC5qb2luKGRvY2tlckRpclBhdGgsICcvbWFpbi5zaCcpO1xuICAgIGZzLmNvcHlGaWxlU3luYyhzY3JpcHRQYXRoLCBtYWluRmlsZSk7XG5cbiAgICB0aGlzLmhhbmRsZXIgPSBuZXcgbGFtYmRhLkRvY2tlckltYWdlRnVuY3Rpb24odGhpcywgJ0Jhc2hFeGVjRnVuY3Rpb24nLCB7XG4gICAgICBjb2RlOiBsYW1iZGEuRG9ja2VySW1hZ2VDb2RlLmZyb21JbWFnZUFzc2V0KGRvY2tlckRpclBhdGgsIHtcbiAgICAgIH0pLFxuICAgICAgdGltZW91dDogcHJvcHMudGltZW91dCA/PyBEdXJhdGlvbi5zZWNvbmRzKDYwKSxcbiAgICAgIGxvZ1JldGVudGlvbjogbG9ncy5SZXRlbnRpb25EYXlzLk9ORV9EQVksXG4gICAgICBlbnZpcm9ubWVudDogcHJvcHMuZW52aXJvbm1lbnQsXG4gICAgICByb2xlOiBwcm9wcy5yb2xlLFxuICAgICAgYXJjaGl0ZWN0dXJlOiBwcm9wcy5hcmNoaXRlY3R1cmUsXG4gICAgICBtZW1vcnlTaXplOiAxMDI0LFxuICAgIH0pO1xuICAgIG5ldyBDZm5PdXRwdXQodGhpcywgJ0xvZ0dyb3VwJywgeyB2YWx1ZTogdGhpcy5oYW5kbGVyLmxvZ0dyb3VwLmxvZ0dyb3VwTmFtZSB9KTtcbiAgfVxufSJdfQ==
```

##### package/lib/lambda-python.js

###### js-beautify {}

```diff
@@ -33,10 +33,10 @@
         });
     }
 }
 exports.LambdaPythonFunction = LambdaPythonFunction;
 _a = JSII_RTTI_SYMBOL_1;
 LambdaPythonFunction[_a] = {
     fqn: "cdk-certbot-dns-route53.LambdaPythonFunction",
-    version: "2.4.95"
+    version: "2.4.96"
 };
 //# sourceMappingURL=data:application/json;base64,eyJ2ZXJzaW9uIjozLCJmaWxlIjoibGFtYmRhLXB5dGhvbi5qcyIsInNvdXJjZVJvb3QiOiIiLCJzb3VyY2VzIjpbIi4uL3NyYy9sYW1iZGEtcHl0aG9uLnRzIl0sIm5hbWVzIjpbXSwibWFwcGluZ3MiOiI7Ozs7O0FBQUEsNkJBQTZCO0FBQzdCLGlFQUFpRTtBQUNqRSw2Q0FBa0Q7QUFFbEQsaURBQWlEO0FBQ2pELDZDQUE2QztBQUM3QywyQ0FBdUM7QUFVdkMsTUFBYSxvQkFBcUIsU0FBUSxzQkFBUztJQUVqRCxZQUFZLEtBQWdCLEVBQUUsRUFBVSxFQUFFLEtBQTBCO1FBQ2xFLEtBQUssQ0FBQyxLQUFLLEVBQUUsRUFBRSxDQUFDLENBQUM7UUFDakIsSUFBSSxDQUFDLE9BQU8sR0FBRyxJQUFJLFlBQVksQ0FBQyxjQUFjLENBQUMsSUFBSSxFQUFFLGdCQUFnQixFQUFFO1lBQ3JFLEtBQUssRUFBRSxJQUFJLENBQUMsSUFBSSxDQUFDLFNBQVMsRUFBRSxZQUFZLENBQUM7WUFDekMsT0FBTyxFQUFFLFNBQVM7WUFDbEIsS0FBSyxFQUFFLFNBQVM7WUFDaEIsT0FBTyxFQUFFLE1BQU0sQ0FBQyxPQUFPLENBQUMsV0FBVztZQUNuQyxPQUFPLEVBQUUsS0FBSyxDQUFDLE9BQU8sSUFBSSxzQkFBUSxDQUFDLE9BQU8sQ0FBQyxFQUFFLENBQUM7WUFDOUMsWUFBWSxFQUFFLElBQUksQ0FBQyxhQUFhLENBQUMsT0FBTztZQUN4QyxXQUFXLEVBQUUsS0FBSyxDQUFDLFdBQVc7WUFDOUIsSUFBSSxFQUFFLEtBQUssQ0FBQyxJQUFJO1lBQ2hCLFVBQVUsRUFBRSxJQUFJO1lBQ2hCLFFBQVEsRUFBRTtnQkFDUixRQUFRLEVBQUUsS0FBSyxDQUFDLFlBQVksQ0FBQyxjQUFjO2FBQzVDO1NBQ0YsQ0FBQyxDQUFDO1FBQ0gsSUFBSSx1QkFBUyxDQUFDLElBQUksRUFBRSxVQUFVLEVBQUUsRUFBRSxLQUFLLEVBQUUsSUFBSSxDQUFDLE9BQU8sQ0FBQyxRQUFRLENBQUMsWUFBWSxFQUFFLENBQUMsQ0FBQztJQUNqRixDQUFDOztBQW5CSCxvREFvQkMiLCJzb3VyY2VzQ29udGVudCI6WyJpbXBvcnQgKiBhcyBwYXRoIGZyb20gJ3BhdGgnO1xuaW1wb3J0ICogYXMgbGFtYmRhUHl0aG9uIGZyb20gJ0Bhd3MtY2RrL2F3cy1sYW1iZGEtcHl0aG9uLWFscGhhJztcbmltcG9ydCB7IENmbk91dHB1dCwgRHVyYXRpb24gfSBmcm9tICdhd3MtY2RrLWxpYic7XG5pbXBvcnQgKiBhcyBpYW0gZnJvbSAnYXdzLWNkay1saWIvYXdzLWlhbSc7XG5pbXBvcnQgKiBhcyBsYW1iZGEgZnJvbSAnYXdzLWNkay1saWIvYXdzLWxhbWJkYSc7XG5pbXBvcnQgKiBhcyBsb2dzIGZyb20gJ2F3cy1jZGstbGliL2F3cy1sb2dzJztcbmltcG9ydCB7IENvbnN0cnVjdCB9IGZyb20gJ2NvbnN0cnVjdHMnO1xuXG5leHBvcnQgaW50ZXJmYWNlIExhbWJkYUZ1bmN0aW9uUHJvcHMge1xuICByZWFkb25seSB0aW1lb3V0OiBEdXJhdGlvbjtcbiAgcmVhZG9ubHkgZW52aXJvbm1lbnQ/OiB7IFtrZXk6IHN0cmluZ106IHN0cmluZyB9O1xuICByZWFkb25seSByb2xlPzogaWFtLklSb2xlO1xuICByZWFkb25seSBhcmNoaXRlY3R1cmU6IGxhbWJkYS5BcmNoaXRlY3R1cmU7XG59XG5cblxuZXhwb3J0IGNsYXNzIExhbWJkYVB5dGhvbkZ1bmN0aW9uIGV4dGVuZHMgQ29uc3RydWN0IHtcbiAgcmVhZG9ubHkgaGFuZGxlcjogbGFtYmRhUHl0aG9uLlB5dGhvbkZ1bmN0aW9uO1xuICBjb25zdHJ1Y3RvcihzY29wZTogQ29uc3RydWN0LCBpZDogc3RyaW5nLCBwcm9wczogTGFtYmRhRnVuY3Rpb25Qcm9wcykge1xuICAgIHN1cGVyKHNjb3BlLCBpZCk7XG4gICAgdGhpcy5oYW5kbGVyID0gbmV3IGxhbWJkYVB5dGhvbi5QeXRob25GdW5jdGlvbih0aGlzLCAnUHl0aG9uRnVuY3Rpb24nLCB7XG4gICAgICBlbnRyeTogcGF0aC5qb2luKF9fZGlybmFtZSwgJy4uL2Fzc2V0cy8nKSxcbiAgICAgIGhhbmRsZXI6ICdoYW5kbGVyJyxcbiAgICAgIGluZGV4OiAnbWFpbi5weScsXG4gICAgICBydW50aW1lOiBsYW1iZGEuUnVudGltZS5QWVRIT05fM18xMixcbiAgICAgIHRpbWVvdXQ6IHByb3BzLnRpbWVvdXQgPz8gRHVyYXRpb24uc2Vjb25kcyg2MCksXG4gICAgICBsb2dSZXRlbnRpb246IGxvZ3MuUmV0ZW50aW9uRGF5cy5PTkVfREFZLFxuICAgICAgZW52aXJvbm1lbnQ6IHByb3BzLmVudmlyb25tZW50LFxuICAgICAgcm9sZTogcHJvcHMucm9sZSxcbiAgICAgIG1lbW9yeVNpemU6IDEwMjQsXG4gICAgICBidW5kbGluZzoge1xuICAgICAgICBwbGF0Zm9ybTogcHJvcHMuYXJjaGl0ZWN0dXJlLmRvY2tlclBsYXRmb3JtLFxuICAgICAgfSxcbiAgICB9KTtcbiAgICBuZXcgQ2ZuT3V0cHV0KHRoaXMsICdMb2dHcm91cCcsIHsgdmFsdWU6IHRoaXMuaGFuZGxlci5sb2dHcm91cC5sb2dHcm91cE5hbWUgfSk7XG4gIH1cbn0iXX0=
```

##### package/lib/main.js

###### js-beautify {}

```diff
@@ -73,15 +73,15 @@
         };
     }
 }
 exports.CertbotDnsRoute53Job = CertbotDnsRoute53Job;
 _a = JSII_RTTI_SYMBOL_1;
 CertbotDnsRoute53Job[_a] = {
     fqn: "cdk-certbot-dns-route53.CertbotDnsRoute53Job",
-    version: "2.4.95"
+    version: "2.4.96"
 };
 class CertbotDnsRoute53JobPython extends constructs_1.Construct {
     constructor(scope, id, props) {
         super(scope, id);
         const certOptions = {
             BUCKET_NAME: props.destinationBucket.bucketName,
             EMAIL: props.certbotOptions.email,
@@ -137,10 +137,10 @@
         };
     }
 }
 exports.CertbotDnsRoute53JobPython = CertbotDnsRoute53JobPython;
 _b = JSII_RTTI_SYMBOL_1;
 CertbotDnsRoute53JobPython[_b] = {
     fqn: "cdk-certbot-dns-route53.CertbotDnsRoute53JobPython",
-    version: "2.4.95"
+    version: "2.4.96"
 };
 //# sourceMappingURL=data:application/json;base64,eyJ2ZXJzaW9uIjozLCJmaWxlIjoibWFpbi5qcyIsInNvdXJjZVJvb3QiOiIiLCJzb3VyY2VzIjpbIi4uL3NyYy9tYWluLnRzIl0sIm5hbWVzIjpbXSwibWFwcGluZ3MiOiI7Ozs7O0FBQUEsNkJBQTZCO0FBQzdCLG1DQUFtQztBQUNuQyxpREFBaUQ7QUFDakQseURBQXlEO0FBQ3pELDJDQUEyQztBQUMzQyxpREFBaUQ7QUFHakQsMkNBQXVDO0FBQ3ZDLCtDQUFpRDtBQUNqRCxtREFBdUQ7QUFvRXZELE1BQWEsb0JBQXFCLFNBQVEsc0JBQVM7SUFDakQsWUFBWSxLQUFnQixFQUFFLEVBQVUsRUFBRSxLQUFnQztRQUN4RSxLQUFLLENBQUMsS0FBSyxFQUFFLEVBQUUsQ0FBQyxDQUFDO1FBQ2pCLE1BQU0sV0FBVyxHQUFHO1lBQ2xCLFdBQVcsRUFBRSxLQUFLLENBQUMsaUJBQWlCLENBQUMsVUFBVTtZQUMvQyxLQUFLLEVBQUUsS0FBSyxDQUFDLGNBQWMsQ0FBQyxLQUFLO1lBQ2pDLFdBQVcsRUFBRSxLQUFLLENBQUMsY0FBYyxDQUFDLFVBQVU7WUFDNUMsdUJBQXVCLEVBQUUsS0FBSyxDQUFDLGNBQWMsQ0FBQyxxQkFBc0I7U0FDckUsQ0FBQztRQUVGLE1BQU0sU0FBUyxHQUFHLElBQUksOEJBQWdCLENBQUMsSUFBSSxFQUFFLDRCQUE0QixFQUFFO1lBQ3pFLE1BQU0sRUFBRSxJQUFJLENBQUMsSUFBSSxDQUFDLFNBQVMsRUFBRSwyQkFBMkIsQ0FBQztZQUN6RCxPQUFPLEVBQUUsR0FBRyxDQUFDLFFBQVEsQ0FBQyxPQUFPLENBQUMsQ0FBQyxDQUFDO1lBQ2hDLFlBQVksRUFBRSxLQUFLLENBQUMsWUFBWSxJQUFJLE1BQU0sQ0FBQyxZQUFZLENBQUMsTUFBTTtZQUM5RCxXQUFXLEVBQUU7Z0JBQ1gsR0FBRyxXQUFXO2FBQ2Y7U0FDRixDQUFDLENBQUM7UUFFSCxLQUFLLENBQUMsaUJBQWlCLENBQUMsY0FBYyxDQUFDLFNBQVMsQ0FBQyxPQUFPLENBQUMsSUFBSyxDQUFDLENBQUM7UUFDaEUsTUFBTSxx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QUNmLENBQUMsQ0FBQztRQUNMLENBQUM7UUFBQSxDQUFDO0lBQ0osQ0FBQzs7QUFqRUgsZ0VBa0VDIiwic291cmNlc0NvbnRlbnQiOlsiaW1wb3J0ICogYXMgcGF0aCBmcm9tICdwYXRoJztcbmltcG9ydCAqIGFzIGNkayBmcm9tICdhd3MtY2RrLWxpYic7XG5pbXBvcnQgKiBhcyBldmVudHMgZnJvbSAnYXdzLWNkay1saWIvYXdzLWV2ZW50cyc7XG5pbXBvcnQgKiBhcyB0YXJnZXQgZnJvbSAnYXdzLWNkay1saWIvYXdzLWV2ZW50cy10YXJnZXRzJztcbmltcG9ydCAqIGFzIGlhbSBmcm9tICdhd3MtY2RrLWxpYi9hd3MtaWFtJztcbmltcG9ydCAqIGFzIGxhbWJkYSBmcm9tICdhd3MtY2RrLWxpYi9hd3MtbGFtYmRhJztcbmltcG9ydCAqIGFzIHI1MyBmcm9tICdhd3MtY2RrLWxpYi9hd3Mtcm91dGU1Myc7XG5pbXBvcnQgKiBhcyBzMyBmcm9tICdhd3MtY2RrLWxpYi9hd3MtczMnO1xuaW1wb3J0IHsgQ29uc3RydWN0IH0gZnJvbSAnY29uc3RydWN0cyc7XG5pbXBvcnQgeyBCYXNoRXhlY0Z1bmN0aW9uIH0gZnJvbSAnLi9sYW1iZGEtYmFzaCc7XG5pbXBvcnQgeyBMYW1iZGFQeXRob25GdW5jdGlvbiB9IGZyb20gJy4vbGFtYmRhLXB5dGhvbic7XG5cbmV4cG9ydCBpbnRlcmZhY2UgQ2VydGJvdE9wdGlvbnMge1xuICAvKipcbiAgICogdGhlIGRvbWFpbiBtdXN0IGhvc3Qgb24gcm91dGU1MyBsaWtlIGV4YW1wbGUuY29tLlxuICAgKlxuICAgKiBAZXhhbXBsZSAtIGAqLmV4YW1wbGUuY29tYCBvciBgYS5leGFtcGxlLmNvbWAgLlxuICAgKi9cbiAgcmVhZG9ubHkgZG9tYWluTmFtZTogc3RyaW5nO1xuXG4gIC8qKlxuICAgKiBFbWFpbCBhZGRyZXNzIGZvciBpbXBvcnRhbnQgYWNjb3VudCBub3RpZmljYXRpb25zLlxuICAgKi9cbiAgcmVhZG9ubHkgZW1haWw6IHN0cmluZztcblxuICAvKipcbiAgICogQ3VzdG9tIHByZWZpeCBkaXJlY3Rvcnkgb24gczMgYnVja2V0IG9iamVjdCBwYXRoLlxuICAgKiBAZGVmYXVsdCAtIGBzMzovL1lPVVJfQlVDS0VUX05BTUUvMjAyMS0wMS0wMS95b3VyLmRvbWFpbi5uYW1lL2BcbiAgICpcbiAgICogQGV4YW1wbGUgLSBjdXN0b21QcmVmaXhEaXJlY3Rvcnk6ICcvJyAtPiBgczM6Ly9ZT1VSX0JVQ0tFVF9OQU1FL3lvdXIuZG9tYWluLm5hbWUvYFxuICAgKlxuICAgKiBAZXhhbXBsZSAtIGN1c3RvbVByZWZpeERpcmVjdG9yeTogJ2FiYycgLT4gYHMzOi8vWU9VUl9CVUNLRVRfTkFNRS9hYmMveW91ci5kb21haW4ubmFtZS9gXG4gICAqL1xuICByZWFkb25seSBjdXN0b21QcmVmaXhEaXJlY3Rvcnk/OiBzdHJpbmc7XG59XG5cbmV4cG9ydCBpbnRlcmZhY2UgQ2VydGJvdERuc1JvdXRlNTNKb2JQcm9wcyB7XG4gIC8qKlxuICAgKiBydW4gdGhlIEpvYiB3aXRoIGRlZmluZWQgc2NoZWR1bGVcbiAgICogQGRlZmF1bHQgLSBubyBzY2hlZHVsZVxuICAgKi9cbiAgcmVhZG9ubHkgc2NoZWR1bGU/OiBldmVudHMuU2NoZWR1bGU7XG5cbiAgLyoqXG4gICAqIFRoZSBTMyBidWNrZXQgdG8gc3RvcmUgY2VydGlmaWNhdGUuXG4gICAqL1xuICByZWFkb25seSBkZXN0aW5hdGlvbkJ1Y2tldDogczMuSUJ1Y2tldDtcblxuICAvKipcbiAgICogVGhlIEhvc3Rab25lIG9uIHJvdXRlNTMgdG8gZG5zLTAxIGNoYWxsZW5nZS5cbiAgICovXG4gIHJlYWRvbmx5IHpvbmU6IHI1My5JSG9zdGVkWm9uZTtcblxuICAvKipcbiAgICogY2VydGJvdCBjbWQgb3B0aW9ucy5cbiAgICovXG4gIHJlYWRvbmx5IGNlcnRib3RPcHRpb25zOiBDZXJ0Ym90T3B0aW9ucztcblxuICAvKipcbiAgICogQ3VzdG9tIGxhbWJkYSBJbWFnZSBBcmNoaXRlY3R1cmUuXG4gICAqXG4gICAqIEBkZWZhdWx0IC0gbGFtYmRhLkFyY2hpdGVjdHVyZS5YODZfNjRcbiAgICovXG4gIHJlYWRvbmx5IGFyY2hpdGVjdHVyZT86IGxhbWJkYS5BcmNoaXRlY3R1cmU7XG5cbiAgLyoqXG4gICAqIEVuYWJsZWQgTGFtYmRhIEZ1bmN0aW9uIFVSTFxuICAgKiBAZGVmYXVsdCAtIGZhbHNlXG4gICAqL1xuICByZWFkb25seSBlbmFibGVkTGFtYmRhRnVuY3Rpb25Vcmw/OiBib29sZWFuO1xuXG4gIC8qKlxuICAgKiBPcHRpb25zIHRvIGFkZCBhIHVybCB0byBhIExhbWJkYSBmdW5jdGlvblxuICAgKiBAZGVmYXVsdCAtIGF1dGhUeXBlOiBsYW1iZGEuRnVuY3Rpb25VcmxBdXRoVHlwZS5OT05FXG4gICAqL1xuICByZWFkb25seSBmdW5jdGlvblVybE9wdGlvbnM/OiBsYW1iZGEuRnVuY3Rpb25VcmxPcHRpb25zO1xufVxuXG5leHBvcnQgY2xhc3MgQ2VydGJvdERuc1JvdXRlNTNKb2IgZXh0ZW5kcyBDb25zdHJ1Y3Qge1xuICBjb25zdHJ1Y3RvcihzY29wZTogQ29uc3RydWN0LCBpZDogc3RyaW5nLCBwcm9wczogQ2VydGJvdERuc1JvdXRlNTNKb2JQcm9wcyApIHtcbiAgICBzdXBlcihzY29wZSwgaWQpO1xuICAgIGNvbnN0IGNlcnRPcHRpb25zID0ge1xuICAgICAgQlVDS0VUX05BTUU6IHByb3BzLmRlc3RpbmF0aW9uQnVja2V0LmJ1Y2tldE5hbWUsXG4gICAgICBFTUFJTDogcHJvcHMuY2VydGJvdE9wdGlvbnMuZW1haWwsXG4gICAgICBET01BSU5fTkFNRTogcHJvcHMuY2VydGJvdE9wdGlvbnMuZG9tYWluTmFtZSxcbiAgICAgIENVU1RPTV9QUkVGSVhfRElSRUNUT1JZOiBwcm9wcy5jZXJ0Ym90T3B0aW9ucy5jdXN0b21QcmVmaXhEaXJlY3RvcnkhLFxuICAgIH07XG5cbiAgICBjb25zdCBsYW1iZGFGdW4gPSBuZXcgQmFzaEV4ZWNGdW5jdGlvbih0aGlzLCAnY2VydGJvdERuc1JvdXRlNTNKb2JMYW1iZGEnLCB7XG4gICAgICBzY3JpcHQ6IHBhdGguam9pbihfX2Rpcm5hbWUsICcuLi9kb2NrZXIuZC9lbnRyeXBvaW50LnNoJyksXG4gICAgICB0aW1lb3V0OiBjZGsuRHVyYXRpb24ubWludXRlcyg1KSxcbiAgICAgIGFyY2hpdGVjdHVyZTogcHJvcHMuYXJjaGl0ZWN0dXJlID8/IGxhbWJkYS5BcmNoaXRlY3R1cmUuWDg2XzY0LFxuICAgICAgZW52aXJvbm1lbnQ6IHtcbiAgICAgICAgLi4uY2VydE9wdGlvbnMsXG4gICAgICB9LFxuICAgIH0pO1xuXG4gICAgcHJvcHMuZGVzdGluYXRpb25CdWNrZXQuZ3JhbnRSZWFkV3JpdGUobGFtYmRhRnVuLmhhbmRsZXIucm9sZSEpO1xuICAgIGNvbnN0IHJvdXRlNTNQb2xpY3lKc29uTGlzdCA9IFt7XG4gICAgICBFZmZlY3Q6ICdBbGxvdycsXG4gICAgICBBY3Rpb246IFtcbiAgICAgICAgJ3JvdXRlNTM6TGlzdEhvc3RlZFpvbmVzJyxcbiAgICAgICAgJ3JvdXRlNTM6R2V0Q2hhbmdlJyxcbiAgICAgIF0sXG4gICAgICBSZXNvdXJjZTogW1xuICAgICAgICAnKicsXG4gICAgICBdLFxuICAgIH0sXG4gICAge1xuICAgICAgRWZmZWN0OiAnQWxsb3cnLFxuICAgICAgQWN0aW9uOiBbXG4gICAgICAgICdyb3V0ZTUzOkNoYW5nZVJlc291cmNlUmVjb3JkU2V0cycsXG4gICAgICBdLFxuICAgICAgUmVzb3VyY2U6IFtcbiAgICAgICAgYGFybjoke25ldyBjZGsuU2NvcGVkQXdzKHRoaXMpLnBhcnRpdGlvbn06cm91dGU1Mzo6Omhvc3RlZHpvbmUvJHtwcm9wcy56b25lLmhvc3RlZFpvbmVJZH1gLFxuICAgICAgXSxcbiAgICB9XTtcbiAgICByb3V0ZTUzUG9saWN5SnNvbkxpc3QuZm9yRWFjaChcbiAgICAgIGUgPT4ge1xuICAgICAgICBsYW1iZGFGdW4uaGFuZGxlci5yb2xlIS5hZGRUb1ByaW5jaXBhbFBvbGljeShpYW0uUG9saWN5U3RhdGVtZW50LmZyb21Kc29uKGUpKTtcbiAgICAgIH0sXG4gICAgKTtcblxuXG4gICAgaWYgKHByb3BzLnNjaGVkdWxlKSB7XG4gICAgICBuZXcgZXZlbnRzLlJ1bGUodGhpcywgJ1NjaGVkdWxlUnVsZScsIHtcbiAgICAgICAgc2NoZWR1bGU6IHByb3BzLnNjaGVkdWxlLFxuICAgICAgICB0YXJnZXRzOiBbXG4gICAgICAgICAgbmV3IHRhcmdldC5MYW1iZGFGdW5jdGlvbihsYW1iZGFGdW4uaGFuZGxlciksXG4gICAgICAgIF0sXG4gICAgICB9KTtcbiAgICB9O1xuXG4gICAgaWYgKHByb3BzLmVuYWJsZWRMYW1iZGFGdW5jdGlvblVybCkge1xuICAgICAgY29uc3QgdXJsID0gbmV3IGxhbWJkYS5GdW5jdGlvblVybCh0aGlzLCAnTGFtYmRhRnVuY3Rpb25VcmwnLCB7XG4gICAgICAgIGZ1bmN0aW9uOiBsYW1iZGFGdW4uaGFuZGxlcixcbiAgICAgICAgYXV0aFR5cGU6IGxhbWJkYS5GdW5jdGlvblVybEF1dGhUeXBlLk5PTkUsXG4gICAgICAgIC4uLnByb3BzLmZ1bmN0aW9uVXJsT3B0aW9ucyxcbiAgICAgIH0pO1xuXG4gICAgICBuZXcgY2RrLkNmbk91dHB1dCh0aGlzLCAnbGFtYmRhRnVuY3Rpb25VcmwnLCB7XG4gICAgICAgIHZhbHVlOiB1cmwudXJsLFxuICAgICAgfSk7XG4gICAgfTtcbiAgfVxufVxuXG5leHBvcnQgaW50ZXJmYWNlIENlcnRib3RPcHRpb25zIHtcbiAgLyoqXG4gICAqIHRoZSBkb21haW4gbXVzdCBob3N0IG9uIHJvdXRlNTMgbGlrZSBleGFtcGxlLmNvbS5cbiAgICpcbiAgICogQGV4YW1wbGUgLSBgKi5leGFtcGxlLmNvbWAgb3IgYGEuZXhhbXBsZS5jb21gIC5cbiAgICovXG4gIHJlYWRvbmx5IGRvbWFpbk5hbWU6IHN0cmluZztcblxuICAvKipcbiAgICogRW1haWwgYWRkcmVzcyBmb3IgaW1wb3J0YW50IGFjY291bnQgbm90aWZpY2F0aW9ucy5cbiAgICovXG4gIHJlYWRvbmx5IGVtYWlsOiBzdHJpbmc7XG5cbiAgLyoqXG4gICAqIEN1c3RvbSBwcmVmaXggZGlyZWN0b3J5IG9uIHMzIGJ1Y2tldCBvYmplY3QgcGF0aC5cbiAgICogQGRlZmF1bHQgLSBgczM6Ly9ZT1VSX0JVQ0tFVF9OQU1FLzIwMjEtMDEtMDEveW91ci5kb21haW4ubmFtZS9gXG4gICAqXG4gICAqIEBleGFtcGxlIC0gY3VzdG9tUHJlZml4RGlyZWN0b3J5OiAnLycgLT4gYHMzOi8vWU9VUl9CVUNLRVRfTkFNRS95b3VyLmRvbWFpbi5uYW1lL2BcbiAgICpcbiAgICogQGV4YW1wbGUgLSBjdXN0b21QcmVmaXhEaXJlY3Rvcnk6ICdhYmMnIC0+IGBzMzovL1lPVVJfQlVDS0VUX05BTUUvYWJjL3lvdXIuZG9tYWluLm5hbWUvYFxuICAgKi9cbiAgcmVhZG9ubHkgY3VzdG9tUHJlZml4RGlyZWN0b3J5Pzogc3RyaW5nO1xufVxuXG5cbmV4cG9ydCBjbGFzcyBDZXJ0Ym90RG5zUm91dGU1M0pvYlB5dGhvbiBleHRlbmRzIENvbnN0cnVjdCB7XG4gIGNvbnN0cnVjdG9yKHNjb3BlOiBDb25zdHJ1Y3QsIGlkOiBzdHJpbmcsIHByb3BzOiBDZXJ0Ym90RG5zUm91dGU1M0pvYlByb3BzICkge1xuICAgIHN1cGVyKHNjb3BlLCBpZCk7XG4gICAgY29uc3QgY2VydE9wdGlvbnMgPSB7XG4gICAgICBCVUNLRVRfTkFNRTogcHJvcHMuZGVzdGluYXRpb25CdWNrZXQuYnVja2V0TmFtZSxcbiAgICAgIEVNQUlMOiBwcm9wcy5jZXJ0Ym90T3B0aW9ucy5lbWFpbCxcbiAgICAgIERPTUFJTl9OQU1FOiBwcm9wcy5jZXJ0Ym90T3B0aW9ucy5kb21haW5OYW1lLFxuICAgICAgQ1VTVE9NX1BSRUZJWF9ESVJFQ1RPUlk6IHByb3BzLmNlcnRib3RPcHRpb25zLmN1c3RvbVByZWZpeERpcmVjdG9yeSEsXG4gICAgfTtcblxuICAgIGNvbnN0IGxhbWJkYUZ1biA9IG5ldyBMYW1iZGFQeXRob25GdW5jdGlvbih0aGlzLCAnY2VydGJvdERuc1JvdXRlNTNKb2JQeXRob25MYW1iZGEnLCB7XG4gICAgICB0aW1lb3V0OiBjZGsuRHVyYXRpb24ubWludXRlcyg1KSxcbiAgICAgIGFyY2hpdGVjdHVyZTogbGFtYmRhLkFyY2hpdGVjdHVyZS5YODZfNjQsXG4gICAgICBlbnZpcm9ubWVudDoge1xuICAgICAgICAuLi5jZXJ0T3B0aW9ucyxcbiAgICAgIH0sXG4gICAgfSk7XG5cbiAgICBwcm9wcy5kZXN0aW5hdGlvbkJ1Y2tldC5ncmFudFJlYWRXcml0ZShsYW1iZGFGdW4uaGFuZGxlci5yb2xlISk7XG4gICAgY29uc3Qgcm91dGU1M1BvbGljeUpzb25MaXN0ID0gW3tcbiAgICAgIEVmZmVjdDogJ0FsbG93JyxcbiAgICAgIEFjdGlvbjogW1xuICAgICAgICAncm91dGU1MzpMaXN0SG9zdGVkWm9uZXMnLFxuICAgICAgICAncm91dGU1MzpHZXRDaGFuZ2UnLFxuICAgICAgXSxcbiAgICAgIFJlc291cmNlOiBbXG4gICAgICAgICcqJyxcbiAgICAgIF0sXG4gICAgfSxcbiAgICB7XG4gICAgICBFZmZlY3Q6ICdBbGxvdycsXG4gICAgICBBY3Rpb246IFtcbiAgICAgICAgJ3JvdXRlNTM6Q2hhbmdlUmVzb3VyY2VSZWNvcmRTZXRzJyxcbiAgICAgIF0sXG4gICAgICBSZXNvdXJjZTogW1xuICAgICAgICBgYXJuOiR7bmV3IGNkay5TY29wZWRBd3ModGhpcykucGFydGl0aW9ufTpyb3V0ZTUzOjo6aG9zdGVkem9uZS8ke3Byb3BzLnpvbmUuaG9zdGVkWm9uZUlkfWAsXG4gICAgICBdLFxuICAgIH1dO1xuICAgIHJvdXRlNTNQb2xpY3lKc29uTGlzdC5mb3JFYWNoKFxuICAgICAgZSA9PiB7XG4gICAgICAgIGxhbWJkYUZ1bi5oYW5kbGVyLnJvbGUhLmFkZFRvUHJpbmNpcGFsUG9saWN5KGlhbS5Qb2xpY3lTdGF0ZW1lbnQuZnJvbUpzb24oZSkpO1xuICAgICAgfSxcbiAgICApO1xuXG5cbiAgICBpZiAocHJvcHMuc2NoZWR1bGUpIHtcbiAgICAgIG5ldyBldmVudHMuUnVsZSh0aGlzLCAnU2NoZWR1bGVSdWxlJywge1xuICAgICAgICBzY2hlZHVsZTogcHJvcHMuc2NoZWR1bGUsXG4gICAgICAgIHRhcmdldHM6IFtcbiAgICAgICAgICBuZXcgdGFyZ2V0LkxhbWJkYUZ1bmN0aW9uKGxhbWJkYUZ1bi5oYW5kbGVyKSxcbiAgICAgICAgXSxcbiAgICAgIH0pO1xuICAgIH07XG5cbiAgICBpZiAocHJvcHMuZW5hYmxlZExhbWJkYUZ1bmN0aW9uVXJsKSB7XG4gICAgICBjb25zdCB1cmwgPSBuZXcgbGFtYmRhLkZ1bmN0aW9uVXJsKHRoaXMsICdMYW1iZGFGdW5jdGlvblVybCcsIHtcbiAgICAgICAgZnVuY3Rpb246IGxhbWJkYUZ1bi5oYW5kbGVyLFxuICAgICAgICBhdXRoVHlwZTogbGFtYmRhLkZ1bmN0aW9uVXJsQXV0aFR5cGUuTk9ORSxcbiAgICAgICAgLi4ucHJvcHMuZnVuY3Rpb25VcmxPcHRpb25zLFxuICAgICAgfSk7XG5cbiAgICAgIG5ldyBjZGsuQ2ZuT3V0cHV0KHRoaXMsICdsYW1iZGFGdW5jdGlvblVybCcsIHtcbiAgICAgICAgdmFsdWU6IHVybC51cmwsXG4gICAgICB9KTtcbiAgICB9O1xuICB9XG59Il19
```

##### package/package.json

###### Pretty-printed

 * *Similarity: 0.9730263157894737%*

 * *Differences: {"'devDependencies'": "{'projen': '^0.80.17'}", "'version'": "'2.4.96'"}*

```diff
@@ -26,15 +26,15 @@
         "jest": "^27",
         "jest-junit": "^15",
         "jsii": "5.3.x",
         "jsii-diff": "^1.96.0",
         "jsii-docgen": "^3.8.31",
         "jsii-pacmak": "^1.96.0",
         "jsii-rosetta": "5.3.x",
-        "projen": "^0.80.16",
+        "projen": "^0.80.17",
         "standard-version": "^9",
         "ts-jest": "^27",
         "typescript": "^5"
     },
     "engines": {
         "node": ">= 20.10.0"
     },
@@ -131,9 +131,9 @@
         "test:watch": "npx projen test:watch",
         "unbump": "npx projen unbump",
         "upgrade": "npx projen upgrade",
         "watch": "npx projen watch"
     },
     "stability": "stable",
     "types": "lib/index.d.ts",
-    "version": "2.4.95"
+    "version": "2.4.96"
 }
```

### Comparing `cdk-certbot-dns-route53-2.4.95/src/cdk_certbot_dns_route53.egg-info/PKG-INFO` & `cdk-certbot-dns-route53-2.4.96/src/cdk_certbot_dns_route53.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-certbot-dns-route53
-Version: 2.4.95
+Version: 2.4.96
 Summary: Create Cron Job Via Lambda, to update certificate and put it to S3 Bucket.
 Home-page: https://github.com/neilkuan/cdk-certbot-dns-route53.git
 Author: Neil Kuan<guan840912@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/neilkuan/cdk-certbot-dns-route53.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

