# Comparing `tmp/cdk-use-cases.custom-cloud9-ssm-1.3.0.tar.gz` & `tmp/cdk-use-cases.custom-cloud9-ssm-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-use-cases.custom-cloud9-ssm-1.3.0.tar", last modified: Tue Feb 28 19:57:10 2023, max compression
+gzip compressed data, was "cdk-use-cases.custom-cloud9-ssm-1.3.1.tar", last modified: Fri Apr  5 13:40:15 2024, max compression
```

## Comparing `cdk-use-cases.custom-cloud9-ssm-1.3.0.tar` & `cdk-use-cases.custom-cloud9-ssm-1.3.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 bpguasch (1650823157) 1896053708        0 2023-02-28 19:57:10.924619 cdk-use-cases.custom-cloud9-ssm-1.3.0/
--rw-r--r--   0 bpguasch (1650823157) 1896053708    10279 2023-02-28 19:57:02.000000 cdk-use-cases.custom-cloud9-ssm-1.3.0/LICENSE
--rw-r--r--   0 bpguasch (1650823157) 1896053708       23 2023-02-28 19:57:02.000000 cdk-use-cases.custom-cloud9-ssm-1.3.0/MANIFEST.in
--rw-r--r--   0 bpguasch (1650823157) 1896053708     6961 2023-02-28 19:57:10.924198 cdk-use-cases.custom-cloud9-ssm-1.3.0/PKG-INFO
--rw-r--r--   0 bpguasch (1650823157) 1896053708     6039 2023-02-28 19:57:02.000000 cdk-use-cases.custom-cloud9-ssm-1.3.0/README.md
--rw-r--r--   0 bpguasch (1650823157) 1896053708      106 2023-02-28 19:57:02.000000 cdk-use-cases.custom-cloud9-ssm-1.3.0/pyproject.toml
--rw-r--r--   0 bpguasch (1650823157) 1896053708       38 2023-02-28 19:57:10.924773 cdk-use-cases.custom-cloud9-ssm-1.3.0/setup.cfg
--rw-r--r--   0 bpguasch (1650823157) 1896053708     1858 2023-02-28 19:57:02.000000 cdk-use-cases.custom-cloud9-ssm-1.3.0/setup.py
-drwxr-xr-x   0 bpguasch (1650823157) 1896053708        0 2023-02-28 19:57:10.915407 cdk-use-cases.custom-cloud9-ssm-1.3.0/src/
-drwxr-xr-x   0 bpguasch (1650823157) 1896053708        0 2023-02-28 19:57:10.915544 cdk-use-cases.custom-cloud9-ssm-1.3.0/src/cdk_use_cases/
-drwxr-xr-x   0 bpguasch (1650823157) 1896053708        0 2023-02-28 19:57:10.921920 cdk-use-cases.custom-cloud9-ssm-1.3.0/src/cdk_use_cases/custom_cloud9_ssm/
--rw-r--r--   0 bpguasch (1650823157) 1896053708    11803 2023-02-28 19:57:02.000000 cdk-use-cases.custom-cloud9-ssm-1.3.0/src/cdk_use_cases/custom_cloud9_ssm/__init__.py
-drwxr-xr-x   0 bpguasch (1650823157) 1896053708        0 2023-02-28 19:57:10.922741 cdk-use-cases.custom-cloud9-ssm-1.3.0/src/cdk_use_cases/custom_cloud9_ssm/_jsii/
--rw-r--r--   0 bpguasch (1650823157) 1896053708      395 2023-02-28 19:57:02.000000 cdk-use-cases.custom-cloud9-ssm-1.3.0/src/cdk_use_cases/custom_cloud9_ssm/_jsii/__init__.py
-drwxr-xr-x   0 bpguasch (1650823157) 1896053708        0 2023-02-28 19:57:10.923481 cdk-use-cases.custom-cloud9-ssm-1.3.0/src/cdk_use_cases/custom_cloud9_ssm/_jsii/bin/
--rw-r--r--   0 bpguasch (1650823157) 1896053708      337 2023-02-28 19:57:02.000000 cdk-use-cases.custom-cloud9-ssm-1.3.0/src/cdk_use_cases/custom_cloud9_ssm/_jsii/bin/custom-cloud9-ssm
--rw-r--r--   0 bpguasch (1650823157) 1896053708   274492 2023-02-28 19:57:02.000000 cdk-use-cases.custom-cloud9-ssm-1.3.0/src/cdk_use_cases/custom_cloud9_ssm/_jsii/custom-cloud9-ssm@1.3.0.jsii.tgz
--rw-r--r--   0 bpguasch (1650823157) 1896053708        1 2023-02-28 19:57:02.000000 cdk-use-cases.custom-cloud9-ssm-1.3.0/src/cdk_use_cases/custom_cloud9_ssm/py.typed
-drwxr-xr-x   0 bpguasch (1650823157) 1896053708        0 2023-02-28 19:57:10.920868 cdk-use-cases.custom-cloud9-ssm-1.3.0/src/cdk_use_cases.custom_cloud9_ssm.egg-info/
--rw-r--r--   0 bpguasch (1650823157) 1896053708     6961 2023-02-28 19:57:10.000000 cdk-use-cases.custom-cloud9-ssm-1.3.0/src/cdk_use_cases.custom_cloud9_ssm.egg-info/PKG-INFO
--rw-r--r--   0 bpguasch (1650823157) 1896053708      633 2023-02-28 19:57:10.000000 cdk-use-cases.custom-cloud9-ssm-1.3.0/src/cdk_use_cases.custom_cloud9_ssm.egg-info/SOURCES.txt
--rw-r--r--   0 bpguasch (1650823157) 1896053708        1 2023-02-28 19:57:10.000000 cdk-use-cases.custom-cloud9-ssm-1.3.0/src/cdk_use_cases.custom_cloud9_ssm.egg-info/dependency_links.txt
--rw-r--r--   0 bpguasch (1650823157) 1896053708       85 2023-02-28 19:57:10.000000 cdk-use-cases.custom-cloud9-ssm-1.3.0/src/cdk_use_cases.custom_cloud9_ssm.egg-info/requires.txt
--rw-r--r--   0 bpguasch (1650823157) 1896053708       14 2023-02-28 19:57:10.000000 cdk-use-cases.custom-cloud9-ssm-1.3.0/src/cdk_use_cases.custom_cloud9_ssm.egg-info/top_level.txt
+drwxr-xr-x   0 bpguasch (1650823157) 1896053708        0 2024-04-05 13:40:15.974522 cdk-use-cases.custom-cloud9-ssm-1.3.1/
+-rw-r--r--   0 bpguasch (1650823157) 1896053708    10279 2024-04-05 13:39:58.000000 cdk-use-cases.custom-cloud9-ssm-1.3.1/LICENSE
+-rw-r--r--   0 bpguasch (1650823157) 1896053708       23 2024-04-05 13:39:58.000000 cdk-use-cases.custom-cloud9-ssm-1.3.1/MANIFEST.in
+-rw-r--r--   0 bpguasch (1650823157) 1896053708     6376 2024-04-05 13:40:15.974038 cdk-use-cases.custom-cloud9-ssm-1.3.1/PKG-INFO
+-rw-r--r--   0 bpguasch (1650823157) 1896053708     5472 2024-04-05 13:39:58.000000 cdk-use-cases.custom-cloud9-ssm-1.3.1/README.md
+-rw-r--r--   0 bpguasch (1650823157) 1896053708      234 2024-04-05 13:39:58.000000 cdk-use-cases.custom-cloud9-ssm-1.3.1/pyproject.toml
+-rw-r--r--   0 bpguasch (1650823157) 1896053708       38 2024-04-05 13:40:15.974702 cdk-use-cases.custom-cloud9-ssm-1.3.1/setup.cfg
+-rw-r--r--   0 bpguasch (1650823157) 1896053708     1899 2024-04-05 13:39:58.000000 cdk-use-cases.custom-cloud9-ssm-1.3.1/setup.py
+drwxr-xr-x   0 bpguasch (1650823157) 1896053708        0 2024-04-05 13:40:15.953557 cdk-use-cases.custom-cloud9-ssm-1.3.1/src/
+drwxr-xr-x   0 bpguasch (1650823157) 1896053708        0 2024-04-05 13:40:15.953912 cdk-use-cases.custom-cloud9-ssm-1.3.1/src/cdk_use_cases/
+drwxr-xr-x   0 bpguasch (1650823157) 1896053708        0 2024-04-05 13:40:15.967335 cdk-use-cases.custom-cloud9-ssm-1.3.1/src/cdk_use_cases/custom_cloud9_ssm/
+-rw-r--r--   0 bpguasch (1650823157) 1896053708    15620 2024-04-05 13:39:58.000000 cdk-use-cases.custom-cloud9-ssm-1.3.1/src/cdk_use_cases/custom_cloud9_ssm/__init__.py
+drwxr-xr-x   0 bpguasch (1650823157) 1896053708        0 2024-04-05 13:40:15.969694 cdk-use-cases.custom-cloud9-ssm-1.3.1/src/cdk_use_cases/custom_cloud9_ssm/_jsii/
+-rw-r--r--   0 bpguasch (1650823157) 1896053708      505 2024-04-05 13:39:58.000000 cdk-use-cases.custom-cloud9-ssm-1.3.1/src/cdk_use_cases/custom_cloud9_ssm/_jsii/__init__.py
+drwxr-xr-x   0 bpguasch (1650823157) 1896053708        0 2024-04-05 13:40:15.972756 cdk-use-cases.custom-cloud9-ssm-1.3.1/src/cdk_use_cases/custom_cloud9_ssm/_jsii/bin/
+-rw-r--r--   0 bpguasch (1650823157) 1896053708      485 2024-04-05 13:39:58.000000 cdk-use-cases.custom-cloud9-ssm-1.3.1/src/cdk_use_cases/custom_cloud9_ssm/_jsii/bin/custom-cloud9-ssm
+-rw-r--r--   0 bpguasch (1650823157) 1896053708   294717 2024-04-05 13:39:58.000000 cdk-use-cases.custom-cloud9-ssm-1.3.1/src/cdk_use_cases/custom_cloud9_ssm/_jsii/custom-cloud9-ssm@1.3.1.jsii.tgz
+-rw-r--r--   0 bpguasch (1650823157) 1896053708        1 2024-04-05 13:39:58.000000 cdk-use-cases.custom-cloud9-ssm-1.3.1/src/cdk_use_cases/custom_cloud9_ssm/py.typed
+drwxr-xr-x   0 bpguasch (1650823157) 1896053708        0 2024-04-05 13:40:15.964522 cdk-use-cases.custom-cloud9-ssm-1.3.1/src/cdk_use_cases.custom_cloud9_ssm.egg-info/
+-rw-r--r--   0 bpguasch (1650823157) 1896053708     6376 2024-04-05 13:40:15.000000 cdk-use-cases.custom-cloud9-ssm-1.3.1/src/cdk_use_cases.custom_cloud9_ssm.egg-info/PKG-INFO
+-rw-r--r--   0 bpguasch (1650823157) 1896053708      633 2024-04-05 13:40:15.000000 cdk-use-cases.custom-cloud9-ssm-1.3.1/src/cdk_use_cases.custom_cloud9_ssm.egg-info/SOURCES.txt
+-rw-r--r--   0 bpguasch (1650823157) 1896053708        1 2024-04-05 13:40:15.000000 cdk-use-cases.custom-cloud9-ssm-1.3.1/src/cdk_use_cases.custom_cloud9_ssm.egg-info/dependency_links.txt
+-rw-r--r--   0 bpguasch (1650823157) 1896053708      112 2024-04-05 13:40:15.000000 cdk-use-cases.custom-cloud9-ssm-1.3.1/src/cdk_use_cases.custom_cloud9_ssm.egg-info/requires.txt
+-rw-r--r--   0 bpguasch (1650823157) 1896053708       14 2024-04-05 13:40:15.000000 cdk-use-cases.custom-cloud9-ssm-1.3.1/src/cdk_use_cases.custom_cloud9_ssm.egg-info/top_level.txt
```

### Comparing `cdk-use-cases.custom-cloud9-ssm-1.3.0/LICENSE` & `cdk-use-cases.custom-cloud9-ssm-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-use-cases.custom-cloud9-ssm-1.3.0/PKG-INFO` & `cdk-use-cases.custom-cloud9-ssm-1.3.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: cdk-use-cases.custom-cloud9-ssm
-Version: 1.3.0
+Version: 1.3.1
 Summary: Pattern for Cloud9 EC2 environment and SSM Document.
 Home-page: https://github.com/aws-samples/cdk-use-cases.git
 Author: Borja Pérez Guasch
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws-samples/cdk-use-cases.git
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved
-Requires-Python: >=3.6
+Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # custom-cloud9-ssm
 
 <!--BEGIN STABILITY BANNER-->---
 
@@ -42,24 +41,22 @@
 |![Typescript Logo](https://docs.aws.amazon.com/cdk/api/latest/img/typescript32.png) Typescript|[`@cdk-use-cases/custom-cloud9-ssm`](https://www.npmjs.com/package/@cdk-use-cases/custom-cloud9-ssm)|
 
 This pattern implements a Cloud9 EC2 environment, applying an initial configuration to the EC2 instance using an SSM Document. It includes helper methods to add steps and parameters to the SSM Document and to resize the EBS volume of the EC2 instance to a given size.
 
 Here is a minimal deployable pattern definition in Typescript:
 
 ```python
-# Example automatically generated from non-compiling source. May contain errors.
 new CustomCloud9Ssm(stack, 'CustomCloud9Ssm');
 ```
 
 You can view [other usage examples](#other-usage-examples).
 
 ## Initializer
 
 ```python
-# Example automatically generated from non-compiling source. May contain errors.
 new CustomCloud9Ssm(scope: Construct, id: string, props: CustomCloud9SsmProps);
 ```
 
 *Parameters*
 
 * scope [`Construct`](https://docs.aws.amazon.com/cdk/api/latest/docs/@aws-cdk_core.Construct.html)
 * id `string`
@@ -77,41 +74,38 @@
 | **Name**     | **Type**        | **Description** |
 |:-------------|:----------------|-----------------|
 | ec2Role | [iam.Role](https://docs.aws.amazon.com/cdk/api/latest/docs/@aws-cdk_aws-iam.Role.html) | The IAM Role that is attached to the EC2 instance launched with the Cloud9 environment to grant it permissions to execute the statements in the SSM Document. |
 
 ## Pattern Methods
 
 ```python
-# Example automatically generated from non-compiling source. May contain errors.
 public addDocumentSteps(steps: string): void
 ```
 
 *Description*
 
 Adds one or more steps to the content of the SSM Document.
 
 *Parameters*
 
 * steps `string`: YAML formatted string containing one or more steps to be added to the `mainSteps` section of the SSM Document.
 
 ```python
-# Example automatically generated from non-compiling source. May contain errors.
 public addDocumentParameters(parameters: string): void
 ```
 
 *Description*
 
 Adds one or more parameters to the content of the SSM Document.
 
 *Parameters*
 
 * parameters `string`: YAML formatted string containing one or more parameters to be added to the `parameters` section of the SSM Document.
 
 ```python
-# Example automatically generated from non-compiling source. May contain errors.
 public resizeEBSTo(size: number): void
 ```
 
 *Description*
 
 Adds a step to the SSM Document content that resizes the EBS volume of the EC2 instance. Attaches the required policies to `ec2Role`.
 
@@ -141,15 +135,14 @@
 ![Architecture Diagram](architecture.png)
 
 ## Other usage examples
 
 *Using default configuration and adding steps*
 
 ```python
-# Example automatically generated from non-compiling source. May contain errors.
 import {CustomCloud9Ssm} from '@cdk-use-cases/custom-cloud9-ssm';
 
 // Define a step that installs boto3
 const boto3Step = `
 - name: InstallBoto3
   action: aws:runShellScript
   inputs:
@@ -164,15 +157,14 @@
 // Add your step to the default document configuration
 customCloud9.addDocumentSteps(boto3Step)
 ```
 
 *Providing props for the SSM Document and resizing the EBS volume*
 
 ```python
-# Example automatically generated from non-compiling source. May contain errors.
 import {CustomCloud9Ssm, CustomCloud9SsmProps} from '@cdk-use-cases/custom-cloud9-ssm';
 const yaml = require('yaml')
 
 // Define the content of the document
 const content = `
 schemaVersion: '2.2'
 description: Bootstrap Cloud9 EC2 instance
@@ -201,9 +193,7 @@
 customCloud9.resizeEBSTo(50)
 ```
 
 ---
 
 
 © Copyright 2021 Amazon.com, Inc. or its affiliates. All Rights Reserved.
-
-
```

### Comparing `cdk-use-cases.custom-cloud9-ssm-1.3.0/README.md` & `cdk-use-cases.custom-cloud9-ssm-1.3.1/src/cdk_use_cases.custom_cloud9_ssm.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+Metadata-Version: 2.1
+Name: cdk-use-cases.custom-cloud9-ssm
+Version: 1.3.1
+Summary: Pattern for Cloud9 EC2 environment and SSM Document.
+Home-page: https://github.com/aws-samples/cdk-use-cases.git
+Author: Borja Pérez Guasch
+License: Apache-2.0
+Project-URL: Source, https://github.com/aws-samples/cdk-use-cases.git
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: JavaScript
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Typing :: Typed
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved
+Requires-Python: ~=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # custom-cloud9-ssm
 
 <!--BEGIN STABILITY BANNER-->---
 
 
 ![Stability: Experimental](https://img.shields.io/badge/stability-Experimental-important.svg?style=for-the-badge)
 
@@ -18,24 +41,22 @@
 |![Typescript Logo](https://docs.aws.amazon.com/cdk/api/latest/img/typescript32.png) Typescript|[`@cdk-use-cases/custom-cloud9-ssm`](https://www.npmjs.com/package/@cdk-use-cases/custom-cloud9-ssm)|
 
 This pattern implements a Cloud9 EC2 environment, applying an initial configuration to the EC2 instance using an SSM Document. It includes helper methods to add steps and parameters to the SSM Document and to resize the EBS volume of the EC2 instance to a given size.
 
 Here is a minimal deployable pattern definition in Typescript:
 
 ```python
-# Example automatically generated from non-compiling source. May contain errors.
 new CustomCloud9Ssm(stack, 'CustomCloud9Ssm');
 ```
 
 You can view [other usage examples](#other-usage-examples).
 
 ## Initializer
 
 ```python
-# Example automatically generated from non-compiling source. May contain errors.
 new CustomCloud9Ssm(scope: Construct, id: string, props: CustomCloud9SsmProps);
 ```
 
 *Parameters*
 
 * scope [`Construct`](https://docs.aws.amazon.com/cdk/api/latest/docs/@aws-cdk_core.Construct.html)
 * id `string`
@@ -53,41 +74,38 @@
 | **Name**     | **Type**        | **Description** |
 |:-------------|:----------------|-----------------|
 | ec2Role | [iam.Role](https://docs.aws.amazon.com/cdk/api/latest/docs/@aws-cdk_aws-iam.Role.html) | The IAM Role that is attached to the EC2 instance launched with the Cloud9 environment to grant it permissions to execute the statements in the SSM Document. |
 
 ## Pattern Methods
 
 ```python
-# Example automatically generated from non-compiling source. May contain errors.
 public addDocumentSteps(steps: string): void
 ```
 
 *Description*
 
 Adds one or more steps to the content of the SSM Document.
 
 *Parameters*
 
 * steps `string`: YAML formatted string containing one or more steps to be added to the `mainSteps` section of the SSM Document.
 
 ```python
-# Example automatically generated from non-compiling source. May contain errors.
 public addDocumentParameters(parameters: string): void
 ```
 
 *Description*
 
 Adds one or more parameters to the content of the SSM Document.
 
 *Parameters*
 
 * parameters `string`: YAML formatted string containing one or more parameters to be added to the `parameters` section of the SSM Document.
 
 ```python
-# Example automatically generated from non-compiling source. May contain errors.
 public resizeEBSTo(size: number): void
 ```
 
 *Description*
 
 Adds a step to the SSM Document content that resizes the EBS volume of the EC2 instance. Attaches the required policies to `ec2Role`.
 
@@ -117,15 +135,14 @@
 ![Architecture Diagram](architecture.png)
 
 ## Other usage examples
 
 *Using default configuration and adding steps*
 
 ```python
-# Example automatically generated from non-compiling source. May contain errors.
 import {CustomCloud9Ssm} from '@cdk-use-cases/custom-cloud9-ssm';
 
 // Define a step that installs boto3
 const boto3Step = `
 - name: InstallBoto3
   action: aws:runShellScript
   inputs:
@@ -140,15 +157,14 @@
 // Add your step to the default document configuration
 customCloud9.addDocumentSteps(boto3Step)
 ```
 
 *Providing props for the SSM Document and resizing the EBS volume*
 
 ```python
-# Example automatically generated from non-compiling source. May contain errors.
 import {CustomCloud9Ssm, CustomCloud9SsmProps} from '@cdk-use-cases/custom-cloud9-ssm';
 const yaml = require('yaml')
 
 // Define the content of the document
 const content = `
 schemaVersion: '2.2'
 description: Bootstrap Cloud9 EC2 instance
```

### Comparing `cdk-use-cases.custom-cloud9-ssm-1.3.0/setup.py` & `cdk-use-cases.custom-cloud9-ssm-1.3.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-use-cases.custom-cloud9-ssm",
-    "version": "1.3.0",
+    "version": "1.3.1",
     "description": "Pattern for Cloud9 EC2 environment and SSM Document.",
     "license": "Apache-2.0",
     "url": "https://github.com/aws-samples/cdk-use-cases.git",
     "long_description_content_type": "text/markdown",
     "author": "Borja Pérez Guasch",
     "bdist_wheel": {
         "universal": true
@@ -22,36 +22,37 @@
     },
     "packages": [
         "cdk_use_cases.custom_cloud9_ssm",
         "cdk_use_cases.custom_cloud9_ssm._jsii"
     ],
     "package_data": {
         "cdk_use_cases.custom_cloud9_ssm._jsii": [
-            "custom-cloud9-ssm@1.3.0.jsii.tgz"
+            "custom-cloud9-ssm@1.3.1.jsii.tgz"
         ],
         "cdk_use_cases.custom_cloud9_ssm": [
             "py.typed"
         ]
     },
-    "python_requires": ">=3.6",
+    "python_requires": "~=3.8",
     "install_requires": [
-        "aws-cdk-lib==2.3.0",
-        "constructs>=10.0.0, <11.0.0",
-        "jsii>=1.50.0, <2.0.0",
-        "publication>=0.0.3"
+        "aws-cdk-lib>=2.135.0, <3.0.0",
+        "constructs>=10.3.0, <11.0.0",
+        "jsii>=1.96.0, <2.0.0",
+        "publication>=0.0.3",
+        "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
         "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
         "Development Status :: 4 - Beta",
         "License :: OSI Approved"
     ],
     "scripts": [
         "src/cdk_use_cases/custom_cloud9_ssm/_jsii/bin/custom-cloud9-ssm"
     ]
```

### Comparing `cdk-use-cases.custom-cloud9-ssm-1.3.0/src/cdk_use_cases/custom_cloud9_ssm/__init__.py` & `cdk-use-cases.custom-cloud9-ssm-1.3.1/src/cdk_use_cases/custom_cloud9_ssm/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -19,24 +19,22 @@
 |![Typescript Logo](https://docs.aws.amazon.com/cdk/api/latest/img/typescript32.png) Typescript|[`@cdk-use-cases/custom-cloud9-ssm`](https://www.npmjs.com/package/@cdk-use-cases/custom-cloud9-ssm)|
 
 This pattern implements a Cloud9 EC2 environment, applying an initial configuration to the EC2 instance using an SSM Document. It includes helper methods to add steps and parameters to the SSM Document and to resize the EBS volume of the EC2 instance to a given size.
 
 Here is a minimal deployable pattern definition in Typescript:
 
 ```python
-# Example automatically generated from non-compiling source. May contain errors.
 new CustomCloud9Ssm(stack, 'CustomCloud9Ssm');
 ```
 
 You can view [other usage examples](#other-usage-examples).
 
 ## Initializer
 
 ```python
-# Example automatically generated from non-compiling source. May contain errors.
 new CustomCloud9Ssm(scope: Construct, id: string, props: CustomCloud9SsmProps);
 ```
 
 *Parameters*
 
 * scope [`Construct`](https://docs.aws.amazon.com/cdk/api/latest/docs/@aws-cdk_core.Construct.html)
 * id `string`
@@ -54,41 +52,38 @@
 | **Name**     | **Type**        | **Description** |
 |:-------------|:----------------|-----------------|
 | ec2Role | [iam.Role](https://docs.aws.amazon.com/cdk/api/latest/docs/@aws-cdk_aws-iam.Role.html) | The IAM Role that is attached to the EC2 instance launched with the Cloud9 environment to grant it permissions to execute the statements in the SSM Document. |
 
 ## Pattern Methods
 
 ```python
-# Example automatically generated from non-compiling source. May contain errors.
 public addDocumentSteps(steps: string): void
 ```
 
 *Description*
 
 Adds one or more steps to the content of the SSM Document.
 
 *Parameters*
 
 * steps `string`: YAML formatted string containing one or more steps to be added to the `mainSteps` section of the SSM Document.
 
 ```python
-# Example automatically generated from non-compiling source. May contain errors.
 public addDocumentParameters(parameters: string): void
 ```
 
 *Description*
 
 Adds one or more parameters to the content of the SSM Document.
 
 *Parameters*
 
 * parameters `string`: YAML formatted string containing one or more parameters to be added to the `parameters` section of the SSM Document.
 
 ```python
-# Example automatically generated from non-compiling source. May contain errors.
 public resizeEBSTo(size: number): void
 ```
 
 *Description*
 
 Adds a step to the SSM Document content that resizes the EBS volume of the EC2 instance. Attaches the required policies to `ec2Role`.
 
@@ -118,15 +113,14 @@
 ![Architecture Diagram](architecture.png)
 
 ## Other usage examples
 
 *Using default configuration and adding steps*
 
 ```python
-# Example automatically generated from non-compiling source. May contain errors.
 import {CustomCloud9Ssm} from '@cdk-use-cases/custom-cloud9-ssm';
 
 // Define a step that installs boto3
 const boto3Step = `
 - name: InstallBoto3
   action: aws:runShellScript
   inputs:
@@ -141,15 +135,14 @@
 // Add your step to the default document configuration
 customCloud9.addDocumentSteps(boto3Step)
 ```
 
 *Providing props for the SSM Document and resizing the EBS volume*
 
 ```python
-# Example automatically generated from non-compiling source. May contain errors.
 import {CustomCloud9Ssm, CustomCloud9SsmProps} from '@cdk-use-cases/custom-cloud9-ssm';
 const yaml = require('yaml')
 
 // Define the content of the document
 const content = `
 schemaVersion: '2.2'
 description: Bootstrap Cloud9 EC2 instance
@@ -179,159 +172,196 @@
 ```
 
 ---
 
 
 © Copyright 2021 Amazon.com, Inc. or its affiliates. All Rights Reserved.
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
 import publication
 import typing_extensions
 
+from typeguard import check_type
+
 from ._jsii import *
 
-import aws_cdk.aws_cloud9
-import aws_cdk.aws_iam
-import aws_cdk.aws_ssm
-import constructs
+import aws_cdk.aws_cloud9 as _aws_cdk_aws_cloud9_ceddda9d
+import aws_cdk.aws_iam as _aws_cdk_aws_iam_ceddda9d
+import aws_cdk.aws_ssm as _aws_cdk_aws_ssm_ceddda9d
+import constructs as _constructs_77d1e7e8
 
 
 class CustomCloud9Ssm(
-    constructs.Construct,
+    _constructs_77d1e7e8.Construct,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdk-use-cases/custom-cloud9-ssm.CustomCloud9Ssm",
 ):
     '''
     :stability: experimental
     '''
 
     def __init__(
         self,
-        scope: constructs.Construct,
+        scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
-        cloud9_ec2_props: typing.Optional[aws_cdk.aws_cloud9.CfnEnvironmentEC2Props] = None,
-        ssm_document_props: typing.Optional[aws_cdk.aws_ssm.CfnDocumentProps] = None,
+        cloud9_ec2_props: typing.Optional[typing.Union[_aws_cdk_aws_cloud9_ceddda9d.CfnEnvironmentEC2Props, typing.Dict[builtins.str, typing.Any]]] = None,
+        ssm_document_props: typing.Optional[typing.Union[_aws_cdk_aws_ssm_ceddda9d.CfnDocumentProps, typing.Dict[builtins.str, typing.Any]]] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
         :param cloud9_ec2_props: (experimental) Optional configuration for the Cloud9 EC2 environment. Default: : none
         :param ssm_document_props: (experimental) Optional configuration for the SSM Document. Default: : none
 
         :stability: experimental
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__9331dc95faf0e493016ac3a0982aaa83cefaaccd48d693be757169708d3581c3)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = CustomCloud9SsmProps(
             cloud9_ec2_props=cloud9_ec2_props, ssm_document_props=ssm_document_props
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
     @jsii.member(jsii_name="addDocumentParameters")
     def add_document_parameters(self, parameters: builtins.str) -> None:
         '''(experimental) Adds one or more parameters to the content of the SSM Document.
 
-        :param parameters: : YAML formatted string containing one or more parameters to be added to the parameters section of the SSM Document.
+        :param parameters: YAML formatted string containing one or more parameters to be added to the parameters section of the SSM Document.
 
         :stability: experimental
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__bcb54d511e5e5d5e6230c31ceb0565e1fdc0fd1eb25c19bc2847f64e4f4f54bb)
+            check_type(argname="argument parameters", value=parameters, expected_type=type_hints["parameters"])
         return typing.cast(None, jsii.invoke(self, "addDocumentParameters", [parameters]))
 
     @jsii.member(jsii_name="addDocumentSteps")
     def add_document_steps(self, steps: builtins.str) -> None:
         '''(experimental) Adds one or more steps to the content of the SSM Document.
 
-        :param steps: : YAML formatted string containing one or more steps to be added to the mainSteps section of the SSM Document.
+        :param steps: YAML formatted string containing one or more steps to be added to the mainSteps section of the SSM Document.
 
         :stability: experimental
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__7f65e24a0b3f838e5cc13a77ae47fdb74efac64f4f101d19732cdd9f146ed4c7)
+            check_type(argname="argument steps", value=steps, expected_type=type_hints["steps"])
         return typing.cast(None, jsii.invoke(self, "addDocumentSteps", [steps]))
 
+    @jsii.member(jsii_name="deployCDKProject")
+    def deploy_cdk_project(self, url: builtins.str) -> None:
+        '''(experimental) Adds a step to the SSM Document content that deploys a CDK project from its compressed version.
+
+        :param url: from where to download the file using the wget command.
+
+        :stability: experimental
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__3a3fb410590672b4abade9ba4a825a4c40ab6b12910dff2df7e9165adfcea34e)
+            check_type(argname="argument url", value=url, expected_type=type_hints["url"])
+        return typing.cast(None, jsii.invoke(self, "deployCDKProject", [url]))
+
     @jsii.member(jsii_name="resizeEBSTo")
     def resize_ebs_to(self, size: jsii.Number) -> None:
         '''(experimental) Adds a step to the SSM Document content that resizes the EBS volume of the EC2 instance.
 
         Attaches the required policies to ec2Role.
 
-        :param size: : size in GiB to resize the EBS volume to.
+        :param size: in GiB to resize the EBS volume to.
 
         :stability: experimental
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__56ddfa2b8a6c41e3fd5100c991019ee37f14df788c7b63e1ef9a4ac192f29f29)
+            check_type(argname="argument size", value=size, expected_type=type_hints["size"])
         return typing.cast(None, jsii.invoke(self, "resizeEBSTo", [size]))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="ec2Role")
-    def ec2_role(self) -> aws_cdk.aws_iam.Role:
+    def ec2_role(self) -> _aws_cdk_aws_iam_ceddda9d.Role:
         '''(experimental) The IAM Role that is attached to the EC2 instance launched with the Cloud9 environment to grant it permissions to execute the statements in the SSM Document.
 
         :stability: experimental
         '''
-        return typing.cast(aws_cdk.aws_iam.Role, jsii.get(self, "ec2Role"))
+        return typing.cast(_aws_cdk_aws_iam_ceddda9d.Role, jsii.get(self, "ec2Role"))
 
 
 @jsii.data_type(
     jsii_type="@cdk-use-cases/custom-cloud9-ssm.CustomCloud9SsmProps",
     jsii_struct_bases=[],
     name_mapping={
         "cloud9_ec2_props": "cloud9Ec2Props",
         "ssm_document_props": "ssmDocumentProps",
     },
 )
 class CustomCloud9SsmProps:
     def __init__(
         self,
         *,
-        cloud9_ec2_props: typing.Optional[aws_cdk.aws_cloud9.CfnEnvironmentEC2Props] = None,
-        ssm_document_props: typing.Optional[aws_cdk.aws_ssm.CfnDocumentProps] = None,
+        cloud9_ec2_props: typing.Optional[typing.Union[_aws_cdk_aws_cloud9_ceddda9d.CfnEnvironmentEC2Props, typing.Dict[builtins.str, typing.Any]]] = None,
+        ssm_document_props: typing.Optional[typing.Union[_aws_cdk_aws_ssm_ceddda9d.CfnDocumentProps, typing.Dict[builtins.str, typing.Any]]] = None,
     ) -> None:
         '''
         :param cloud9_ec2_props: (experimental) Optional configuration for the Cloud9 EC2 environment. Default: : none
         :param ssm_document_props: (experimental) Optional configuration for the SSM Document. Default: : none
 
         :stability: experimental
         '''
         if isinstance(cloud9_ec2_props, dict):
-            cloud9_ec2_props = aws_cdk.aws_cloud9.CfnEnvironmentEC2Props(**cloud9_ec2_props)
+            cloud9_ec2_props = _aws_cdk_aws_cloud9_ceddda9d.CfnEnvironmentEC2Props(**cloud9_ec2_props)
         if isinstance(ssm_document_props, dict):
-            ssm_document_props = aws_cdk.aws_ssm.CfnDocumentProps(**ssm_document_props)
-        self._values: typing.Dict[str, typing.Any] = {}
+            ssm_document_props = _aws_cdk_aws_ssm_ceddda9d.CfnDocumentProps(**ssm_document_props)
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__039fbf3a0e07870378db7192288c961d9677ae0f7343c84767d57be4a8ae9634)
+            check_type(argname="argument cloud9_ec2_props", value=cloud9_ec2_props, expected_type=type_hints["cloud9_ec2_props"])
+            check_type(argname="argument ssm_document_props", value=ssm_document_props, expected_type=type_hints["ssm_document_props"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {}
         if cloud9_ec2_props is not None:
             self._values["cloud9_ec2_props"] = cloud9_ec2_props
         if ssm_document_props is not None:
             self._values["ssm_document_props"] = ssm_document_props
 
     @builtins.property
     def cloud9_ec2_props(
         self,
-    ) -> typing.Optional[aws_cdk.aws_cloud9.CfnEnvironmentEC2Props]:
+    ) -> typing.Optional[_aws_cdk_aws_cloud9_ceddda9d.CfnEnvironmentEC2Props]:
         '''(experimental) Optional configuration for the Cloud9 EC2 environment.
 
         :default: : none
 
         :stability: experimental
         '''
         result = self._values.get("cloud9_ec2_props")
-        return typing.cast(typing.Optional[aws_cdk.aws_cloud9.CfnEnvironmentEC2Props], result)
+        return typing.cast(typing.Optional[_aws_cdk_aws_cloud9_ceddda9d.CfnEnvironmentEC2Props], result)
 
     @builtins.property
-    def ssm_document_props(self) -> typing.Optional[aws_cdk.aws_ssm.CfnDocumentProps]:
+    def ssm_document_props(
+        self,
+    ) -> typing.Optional[_aws_cdk_aws_ssm_ceddda9d.CfnDocumentProps]:
         '''(experimental) Optional configuration for the SSM Document.
 
         :default: : none
 
         :stability: experimental
         '''
         result = self._values.get("ssm_document_props")
-        return typing.cast(typing.Optional[aws_cdk.aws_ssm.CfnDocumentProps], result)
+        return typing.cast(typing.Optional[_aws_cdk_aws_ssm_ceddda9d.CfnDocumentProps], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
@@ -343,7 +373,49 @@
 
 __all__ = [
     "CustomCloud9Ssm",
     "CustomCloud9SsmProps",
 ]
 
 publication.publish()
+
+def _typecheckingstub__9331dc95faf0e493016ac3a0982aaa83cefaaccd48d693be757169708d3581c3(
+    scope: _constructs_77d1e7e8.Construct,
+    id: builtins.str,
+    *,
+    cloud9_ec2_props: typing.Optional[typing.Union[_aws_cdk_aws_cloud9_ceddda9d.CfnEnvironmentEC2Props, typing.Dict[builtins.str, typing.Any]]] = None,
+    ssm_document_props: typing.Optional[typing.Union[_aws_cdk_aws_ssm_ceddda9d.CfnDocumentProps, typing.Dict[builtins.str, typing.Any]]] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__bcb54d511e5e5d5e6230c31ceb0565e1fdc0fd1eb25c19bc2847f64e4f4f54bb(
+    parameters: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__7f65e24a0b3f838e5cc13a77ae47fdb74efac64f4f101d19732cdd9f146ed4c7(
+    steps: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__3a3fb410590672b4abade9ba4a825a4c40ab6b12910dff2df7e9165adfcea34e(
+    url: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__56ddfa2b8a6c41e3fd5100c991019ee37f14df788c7b63e1ef9a4ac192f29f29(
+    size: jsii.Number,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__039fbf3a0e07870378db7192288c961d9677ae0f7343c84767d57be4a8ae9634(
+    *,
+    cloud9_ec2_props: typing.Optional[typing.Union[_aws_cdk_aws_cloud9_ceddda9d.CfnEnvironmentEC2Props, typing.Dict[builtins.str, typing.Any]]] = None,
+    ssm_document_props: typing.Optional[typing.Union[_aws_cdk_aws_ssm_ceddda9d.CfnDocumentProps, typing.Dict[builtins.str, typing.Any]]] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
```

### Comparing `cdk-use-cases.custom-cloud9-ssm-1.3.0/src/cdk_use_cases.custom_cloud9_ssm.egg-info/SOURCES.txt` & `cdk-use-cases.custom-cloud9-ssm-1.3.1/src/cdk_use_cases.custom_cloud9_ssm.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,9 +7,9 @@
 src/cdk_use_cases.custom_cloud9_ssm.egg-info/SOURCES.txt
 src/cdk_use_cases.custom_cloud9_ssm.egg-info/dependency_links.txt
 src/cdk_use_cases.custom_cloud9_ssm.egg-info/requires.txt
 src/cdk_use_cases.custom_cloud9_ssm.egg-info/top_level.txt
 src/cdk_use_cases/custom_cloud9_ssm/__init__.py
 src/cdk_use_cases/custom_cloud9_ssm/py.typed
 src/cdk_use_cases/custom_cloud9_ssm/_jsii/__init__.py
-src/cdk_use_cases/custom_cloud9_ssm/_jsii/custom-cloud9-ssm@1.3.0.jsii.tgz
+src/cdk_use_cases/custom_cloud9_ssm/_jsii/custom-cloud9-ssm@1.3.1.jsii.tgz
 src/cdk_use_cases/custom_cloud9_ssm/_jsii/bin/custom-cloud9-ssm
```

