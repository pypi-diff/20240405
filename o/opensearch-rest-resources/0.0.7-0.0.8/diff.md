# Comparing `tmp/opensearch-rest-resources-0.0.7.tar.gz` & `tmp/opensearch-rest-resources-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opensearch-rest-resources-0.0.7.tar", last modified: Thu Apr  4 10:49:01 2024, max compression
+gzip compressed data, was "opensearch-rest-resources-0.0.8.tar", last modified: Fri Apr  5 11:12:20 2024, max compression
```

## Comparing `opensearch-rest-resources-0.0.7.tar` & `opensearch-rest-resources-0.0.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:49:01.517143 opensearch-rest-resources-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-04 10:48:51.000000 opensearch-rest-resources-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-04 10:48:51.000000 opensearch-rest-resources-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-04-04 10:49:01.517143 opensearch-rest-resources-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-04 10:48:51.000000 opensearch-rest-resources-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-04 10:48:51.000000 opensearch-rest-resources-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 10:49:01.517143 opensearch-rest-resources-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-04 10:48:51.000000 opensearch-rest-resources-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:49:01.513143 opensearch-rest-resources-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:49:01.513143 opensearch-rest-resources-0.0.7/src/opensearch_rest_resources/
--rw-r--r--   0 runner    (1001) docker     (127)    52758 2024-04-04 10:48:51.000000 opensearch-rest-resources-0.0.7/src/opensearch_rest_resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:49:01.517143 opensearch-rest-resources-0.0.7/src/opensearch_rest_resources/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-04 10:48:51.000000 opensearch-rest-resources-0.0.7/src/opensearch_rest_resources/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    85444 2024-04-04 10:48:51.000000 opensearch-rest-resources-0.0.7/src/opensearch_rest_resources/_jsii/opensearch-rest-resources@0.0.7.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 10:48:51.000000 opensearch-rest-resources-0.0.7/src/opensearch_rest_resources/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:49:01.517143 opensearch-rest-resources-0.0.7/src/opensearch_rest_resources.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-04-04 10:49:01.000000 opensearch-rest-resources-0.0.7/src/opensearch_rest_resources.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-04 10:49:01.000000 opensearch-rest-resources-0.0.7/src/opensearch_rest_resources.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 10:49:01.000000 opensearch-rest-resources-0.0.7/src/opensearch_rest_resources.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-04 10:49:01.000000 opensearch-rest-resources-0.0.7/src/opensearch_rest_resources.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-04 10:49:01.000000 opensearch-rest-resources-0.0.7/src/opensearch_rest_resources.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:12:20.200490 opensearch-rest-resources-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-05 11:12:10.000000 opensearch-rest-resources-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-05 11:12:10.000000 opensearch-rest-resources-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-04-05 11:12:20.196490 opensearch-rest-resources-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-04-05 11:12:10.000000 opensearch-rest-resources-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-05 11:12:10.000000 opensearch-rest-resources-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 11:12:20.200490 opensearch-rest-resources-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-05 11:12:10.000000 opensearch-rest-resources-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:12:20.196490 opensearch-rest-resources-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:12:20.196490 opensearch-rest-resources-0.0.8/src/opensearch_rest_resources/
+-rw-r--r--   0 runner    (1001) docker     (127)    54134 2024-04-05 11:12:10.000000 opensearch-rest-resources-0.0.8/src/opensearch_rest_resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:12:20.196490 opensearch-rest-resources-0.0.8/src/opensearch_rest_resources/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-05 11:12:10.000000 opensearch-rest-resources-0.0.8/src/opensearch_rest_resources/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85850 2024-04-05 11:12:10.000000 opensearch-rest-resources-0.0.8/src/opensearch_rest_resources/_jsii/opensearch-rest-resources@0.0.8.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 11:12:10.000000 opensearch-rest-resources-0.0.8/src/opensearch_rest_resources/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:12:20.196490 opensearch-rest-resources-0.0.8/src/opensearch_rest_resources.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-04-05 11:12:20.000000 opensearch-rest-resources-0.0.8/src/opensearch_rest_resources.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-05 11:12:20.000000 opensearch-rest-resources-0.0.8/src/opensearch_rest_resources.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 11:12:20.000000 opensearch-rest-resources-0.0.8/src/opensearch_rest_resources.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-05 11:12:20.000000 opensearch-rest-resources-0.0.8/src/opensearch_rest_resources.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-05 11:12:20.000000 opensearch-rest-resources-0.0.8/src/opensearch_rest_resources.egg-info/top_level.txt
```

### Comparing `opensearch-rest-resources-0.0.7/LICENSE` & `opensearch-rest-resources-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `opensearch-rest-resources-0.0.7/PKG-INFO` & `opensearch-rest-resources-0.0.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opensearch-rest-resources
-Version: 0.0.7
+Version: 0.0.8
 Summary: Manage OpenSearch REST resources from AWS CDK.
 Home-page: https://github.com/tmokmss/opensearch-rest-resources.git
 Author: tmokmss<tomookam@live.jp>
 License: MIT
 Project-URL: Source, https://github.com/tmokmss/opensearch-rest-resources.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -80,21 +80,20 @@
     removalPolicy: RemovalPolicy.RETAIN,
 });
 roleMapping.node.addDependency(role);
 ```
 
 ## Limitation
 
-Currently this library assumes your OpenSearch domain is configured as:
+Currently this library assumes your OpenSearch domain is configured such that:
 
 * [Fine-grained access control](https://docs.aws.amazon.com/opensearch-service/latest/developerguide/fgac.html) is enabled
-* Deployed within a VPC
 * Use the [`Domain`](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_opensearchservice.Domain.html) L2 construct
-* The credential for the master user (username and password) is stored in Secret Manager
-* [Domain access policy](https://docs.aws.amazon.com/opensearch-service/latest/developerguide/fgac.html#fgac-recommendations) is permissive enough like below:
+* The master is authenticated with username and password, and the credential is stored in Secret Manager
+* [Domain access policy](https://docs.aws.amazon.com/opensearch-service/latest/developerguide/fgac.html#fgac-recommendations) is configured to allow access from the master user
 
 ```json
 {
   "Version": "2012-10-17",
   "Statement": [
     {
       "Effect": "Allow",
```

### Comparing `opensearch-rest-resources-0.0.7/README.md` & `opensearch-rest-resources-0.0.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -57,21 +57,20 @@
     removalPolicy: RemovalPolicy.RETAIN,
 });
 roleMapping.node.addDependency(role);
 ```
 
 ## Limitation
 
-Currently this library assumes your OpenSearch domain is configured as:
+Currently this library assumes your OpenSearch domain is configured such that:
 
 * [Fine-grained access control](https://docs.aws.amazon.com/opensearch-service/latest/developerguide/fgac.html) is enabled
-* Deployed within a VPC
 * Use the [`Domain`](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_opensearchservice.Domain.html) L2 construct
-* The credential for the master user (username and password) is stored in Secret Manager
-* [Domain access policy](https://docs.aws.amazon.com/opensearch-service/latest/developerguide/fgac.html#fgac-recommendations) is permissive enough like below:
+* The master is authenticated with username and password, and the credential is stored in Secret Manager
+* [Domain access policy](https://docs.aws.amazon.com/opensearch-service/latest/developerguide/fgac.html#fgac-recommendations) is configured to allow access from the master user
 
 ```json
 {
   "Version": "2012-10-17",
   "Statement": [
     {
       "Effect": "Allow",
```

### Comparing `opensearch-rest-resources-0.0.7/setup.py` & `opensearch-rest-resources-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "opensearch-rest-resources",
-    "version": "0.0.7",
+    "version": "0.0.8",
     "description": "Manage OpenSearch REST resources from AWS CDK.",
     "license": "MIT",
     "url": "https://github.com/tmokmss/opensearch-rest-resources.git",
     "long_description_content_type": "text/markdown",
     "author": "tmokmss<tomookam@live.jp>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "opensearch_rest_resources",
         "opensearch_rest_resources._jsii"
     ],
     "package_data": {
         "opensearch_rest_resources._jsii": [
-            "opensearch-rest-resources@0.0.7.jsii.tgz"
+            "opensearch-rest-resources@0.0.8.jsii.tgz"
         ],
         "opensearch_rest_resources": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `opensearch-rest-resources-0.0.7/src/opensearch_rest_resources/__init__.py` & `opensearch-rest-resources-0.0.8/src/opensearch_rest_resources/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,21 +58,20 @@
     removalPolicy: RemovalPolicy.RETAIN,
 });
 roleMapping.node.addDependency(role);
 ```
 
 ## Limitation
 
-Currently this library assumes your OpenSearch domain is configured as:
+Currently this library assumes your OpenSearch domain is configured such that:
 
 * [Fine-grained access control](https://docs.aws.amazon.com/opensearch-service/latest/developerguide/fgac.html) is enabled
-* Deployed within a VPC
 * Use the [`Domain`](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_opensearchservice.Domain.html) L2 construct
-* The credential for the master user (username and password) is stored in Secret Manager
-* [Domain access policy](https://docs.aws.amazon.com/opensearch-service/latest/developerguide/fgac.html#fgac-recommendations) is permissive enough like below:
+* The master is authenticated with username and password, and the credential is stored in Secret Manager
+* [Domain access policy](https://docs.aws.amazon.com/opensearch-service/latest/developerguide/fgac.html#fgac-recommendations) is configured to allow access from the master user
 
 ```json
 {
   "Version": "2012-10-17",
   "Statement": [
     {
       "Effect": "Allow",
@@ -205,84 +204,85 @@
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         domain: _aws_cdk_aws_opensearchservice_ceddda9d.Domain,
         payload_json: builtins.str,
         rest_endpoint: builtins.str,
-        vpc: _aws_cdk_aws_ec2_ceddda9d.IVpc,
         removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
+        vpc: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
         :param domain: The OpenSearch domain you want to create a resource in.
         :param payload_json: A payload in JSON string to send with a request on create/update event.
         :param rest_endpoint: A REST endpoint to call from the custom resource handler. It sends PUT request on a create/update event and DELETE request on a delete event.
-        :param vpc: The VPC your OpenSearch domain is in.
         :param removal_policy: Policy to apply when the resource is removed from the stack. Default: RemovalPolicy.DESTROY
+        :param vpc: The VPC your OpenSearch domain is in. Default: Assumes your Domain is not deployed within a VPC
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__88b7de23b7128611fcf29d3404857d67dca8a603b41add8856c8e8e50273d72f)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = OpenSearchCustomResourceProps(
             domain=domain,
             payload_json=payload_json,
             rest_endpoint=rest_endpoint,
-            vpc=vpc,
             removal_policy=removal_policy,
+            vpc=vpc,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
 
 @jsii.data_type(
     jsii_type="opensearch-rest-resources.OpenSearchCustomResourceProps",
     jsii_struct_bases=[],
     name_mapping={
         "domain": "domain",
         "payload_json": "payloadJson",
         "rest_endpoint": "restEndpoint",
-        "vpc": "vpc",
         "removal_policy": "removalPolicy",
+        "vpc": "vpc",
     },
 )
 class OpenSearchCustomResourceProps:
     def __init__(
         self,
         *,
         domain: _aws_cdk_aws_opensearchservice_ceddda9d.Domain,
         payload_json: builtins.str,
         rest_endpoint: builtins.str,
-        vpc: _aws_cdk_aws_ec2_ceddda9d.IVpc,
         removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
+        vpc: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc] = None,
     ) -> None:
         '''
         :param domain: The OpenSearch domain you want to create a resource in.
         :param payload_json: A payload in JSON string to send with a request on create/update event.
         :param rest_endpoint: A REST endpoint to call from the custom resource handler. It sends PUT request on a create/update event and DELETE request on a delete event.
-        :param vpc: The VPC your OpenSearch domain is in.
         :param removal_policy: Policy to apply when the resource is removed from the stack. Default: RemovalPolicy.DESTROY
+        :param vpc: The VPC your OpenSearch domain is in. Default: Assumes your Domain is not deployed within a VPC
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__bdfb6ebf47fc374b01c571ea7c22a6ef12e6a8ba43b993c7a76b892ec0afda3a)
             check_type(argname="argument domain", value=domain, expected_type=type_hints["domain"])
             check_type(argname="argument payload_json", value=payload_json, expected_type=type_hints["payload_json"])
             check_type(argname="argument rest_endpoint", value=rest_endpoint, expected_type=type_hints["rest_endpoint"])
-            check_type(argname="argument vpc", value=vpc, expected_type=type_hints["vpc"])
             check_type(argname="argument removal_policy", value=removal_policy, expected_type=type_hints["removal_policy"])
+            check_type(argname="argument vpc", value=vpc, expected_type=type_hints["vpc"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "domain": domain,
             "payload_json": payload_json,
             "rest_endpoint": rest_endpoint,
-            "vpc": vpc,
         }
         if removal_policy is not None:
             self._values["removal_policy"] = removal_policy
+        if vpc is not None:
+            self._values["vpc"] = vpc
 
     @builtins.property
     def domain(self) -> _aws_cdk_aws_opensearchservice_ceddda9d.Domain:
         '''The OpenSearch domain you want to create a resource in.'''
         result = self._values.get("domain")
         assert result is not None, "Required property 'domain' is missing"
         return typing.cast(_aws_cdk_aws_opensearchservice_ceddda9d.Domain, result)
@@ -305,29 +305,31 @@
             _plugins/_security/api/roles/roleName
         '''
         result = self._values.get("rest_endpoint")
         assert result is not None, "Required property 'rest_endpoint' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
-    def vpc(self) -> _aws_cdk_aws_ec2_ceddda9d.IVpc:
-        '''The VPC your OpenSearch domain is in.'''
-        result = self._values.get("vpc")
-        assert result is not None, "Required property 'vpc' is missing"
-        return typing.cast(_aws_cdk_aws_ec2_ceddda9d.IVpc, result)
-
-    @builtins.property
     def removal_policy(self) -> typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy]:
         '''Policy to apply when the resource is removed from the stack.
 
         :default: RemovalPolicy.DESTROY
         '''
         result = self._values.get("removal_policy")
         return typing.cast(typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy], result)
 
+    @builtins.property
+    def vpc(self) -> typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc]:
+        '''The VPC your OpenSearch domain is in.
+
+        :default: Assumes your Domain is not deployed within a VPC
+        '''
+        result = self._values.get("vpc")
+        return typing.cast(typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc], result)
+
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
@@ -345,36 +347,36 @@
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         payload: typing.Union["RolePayload", typing.Dict[builtins.str, typing.Any]],
         role_name: builtins.str,
         domain: _aws_cdk_aws_opensearchservice_ceddda9d.Domain,
-        vpc: _aws_cdk_aws_ec2_ceddda9d.IVpc,
         removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
+        vpc: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
         :param payload: See https://opensearch.org/docs/latest/security/access-control/api/#create-role for the details.
         :param role_name: The name of this role.
         :param domain: The OpenSearch domain you want to create a resource in.
-        :param vpc: The VPC your OpenSearch domain is in.
         :param removal_policy: Policy to apply when the resource is removed from the stack. Default: RemovalPolicy.DESTROY
+        :param vpc: The VPC your OpenSearch domain is in. Default: Assumes your Domain is not deployed within a VPC
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__11b3dbdadf9ad4e9eb287cd1fb49920a34f29982e1c81061e7655c436c58310e)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = OpenSearchRoleProps(
             payload=payload,
             role_name=role_name,
             domain=domain,
-            vpc=vpc,
             removal_policy=removal_policy,
+            vpc=vpc,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
 
 class OpenSearchRoleMapping(
     _constructs_77d1e7e8.Construct,
@@ -385,36 +387,36 @@
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         payload: typing.Union["RoleMappingPayload", typing.Dict[builtins.str, typing.Any]],
         role_name: builtins.str,
         domain: _aws_cdk_aws_opensearchservice_ceddda9d.Domain,
-        vpc: _aws_cdk_aws_ec2_ceddda9d.IVpc,
         removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
+        vpc: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
         :param payload: See https://opensearch.org/docs/latest/security/access-control/api/#create-role-mapping for the details.
         :param role_name: The role you create a role mapping for. Create a role by {@link OpenSearchRole} class, or use `a predefined role <https://opensearch.org/docs/latest/security/access-control/users-roles/#predefined-roles>`_.
         :param domain: The OpenSearch domain you want to create a resource in.
-        :param vpc: The VPC your OpenSearch domain is in.
         :param removal_policy: Policy to apply when the resource is removed from the stack. Default: RemovalPolicy.DESTROY
+        :param vpc: The VPC your OpenSearch domain is in. Default: Assumes your Domain is not deployed within a VPC
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__a648bd6553d5af4908ea24e1f83ff607db47eb845ef54b6dc7d9a6e22a0d8c36)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = OpenSearchRoleMappingProps(
             payload=payload,
             role_name=role_name,
             domain=domain,
-            vpc=vpc,
             removal_policy=removal_policy,
+            vpc=vpc,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
 
 class OpenSearchUser(
     _constructs_77d1e7e8.Construct,
@@ -425,94 +427,97 @@
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         payload: typing.Union["UserPayload", typing.Dict[builtins.str, typing.Any]],
         user_name: builtins.str,
         domain: _aws_cdk_aws_opensearchservice_ceddda9d.Domain,
-        vpc: _aws_cdk_aws_ec2_ceddda9d.IVpc,
         removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
+        vpc: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
         :param payload: See https://opensearch.org/docs/latest/security/access-control/api/#create-user for the details.
         :param user_name: The name of this user.
         :param domain: The OpenSearch domain you want to create a resource in.
-        :param vpc: The VPC your OpenSearch domain is in.
         :param removal_policy: Policy to apply when the resource is removed from the stack. Default: RemovalPolicy.DESTROY
+        :param vpc: The VPC your OpenSearch domain is in. Default: Assumes your Domain is not deployed within a VPC
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__020b51bbd8211c5405011c19762bef3c8303e05f610a6b7e6f2b64bcf9151850)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = OpenSearchUserProps(
             payload=payload,
             user_name=user_name,
             domain=domain,
-            vpc=vpc,
             removal_policy=removal_policy,
+            vpc=vpc,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
 
 @jsii.data_type(
     jsii_type="opensearch-rest-resources.ResourcePropsBase",
     jsii_struct_bases=[],
-    name_mapping={"domain": "domain", "vpc": "vpc", "removal_policy": "removalPolicy"},
+    name_mapping={"domain": "domain", "removal_policy": "removalPolicy", "vpc": "vpc"},
 )
 class ResourcePropsBase:
     def __init__(
         self,
         *,
         domain: _aws_cdk_aws_opensearchservice_ceddda9d.Domain,
-        vpc: _aws_cdk_aws_ec2_ceddda9d.IVpc,
         removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
+        vpc: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc] = None,
     ) -> None:
         '''
         :param domain: The OpenSearch domain you want to create a resource in.
-        :param vpc: The VPC your OpenSearch domain is in.
         :param removal_policy: Policy to apply when the resource is removed from the stack. Default: RemovalPolicy.DESTROY
+        :param vpc: The VPC your OpenSearch domain is in. Default: Assumes your Domain is not deployed within a VPC
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__925237d929be76edf0f5d1670f8f84caac9877c0ca124747b7db826a1ad69fbc)
             check_type(argname="argument domain", value=domain, expected_type=type_hints["domain"])
-            check_type(argname="argument vpc", value=vpc, expected_type=type_hints["vpc"])
             check_type(argname="argument removal_policy", value=removal_policy, expected_type=type_hints["removal_policy"])
+            check_type(argname="argument vpc", value=vpc, expected_type=type_hints["vpc"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "domain": domain,
-            "vpc": vpc,
         }
         if removal_policy is not None:
             self._values["removal_policy"] = removal_policy
+        if vpc is not None:
+            self._values["vpc"] = vpc
 
     @builtins.property
     def domain(self) -> _aws_cdk_aws_opensearchservice_ceddda9d.Domain:
         '''The OpenSearch domain you want to create a resource in.'''
         result = self._values.get("domain")
         assert result is not None, "Required property 'domain' is missing"
         return typing.cast(_aws_cdk_aws_opensearchservice_ceddda9d.Domain, result)
 
     @builtins.property
-    def vpc(self) -> _aws_cdk_aws_ec2_ceddda9d.IVpc:
-        '''The VPC your OpenSearch domain is in.'''
-        result = self._values.get("vpc")
-        assert result is not None, "Required property 'vpc' is missing"
-        return typing.cast(_aws_cdk_aws_ec2_ceddda9d.IVpc, result)
-
-    @builtins.property
     def removal_policy(self) -> typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy]:
         '''Policy to apply when the resource is removed from the stack.
 
         :default: RemovalPolicy.DESTROY
         '''
         result = self._values.get("removal_policy")
         return typing.cast(typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy], result)
 
+    @builtins.property
+    def vpc(self) -> typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc]:
+        '''The VPC your OpenSearch domain is in.
+
+        :default: Assumes your Domain is not deployed within a VPC
+        '''
+        result = self._values.get("vpc")
+        return typing.cast(typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc], result)
+
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
@@ -777,79 +782,82 @@
 
 
 @jsii.data_type(
     jsii_type="opensearch-rest-resources.OpenSearchRoleMappingProps",
     jsii_struct_bases=[ResourcePropsBase],
     name_mapping={
         "domain": "domain",
-        "vpc": "vpc",
         "removal_policy": "removalPolicy",
+        "vpc": "vpc",
         "payload": "payload",
         "role_name": "roleName",
     },
 )
 class OpenSearchRoleMappingProps(ResourcePropsBase):
     def __init__(
         self,
         *,
         domain: _aws_cdk_aws_opensearchservice_ceddda9d.Domain,
-        vpc: _aws_cdk_aws_ec2_ceddda9d.IVpc,
         removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
+        vpc: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc] = None,
         payload: typing.Union[RoleMappingPayload, typing.Dict[builtins.str, typing.Any]],
         role_name: builtins.str,
     ) -> None:
         '''
         :param domain: The OpenSearch domain you want to create a resource in.
-        :param vpc: The VPC your OpenSearch domain is in.
         :param removal_policy: Policy to apply when the resource is removed from the stack. Default: RemovalPolicy.DESTROY
+        :param vpc: The VPC your OpenSearch domain is in. Default: Assumes your Domain is not deployed within a VPC
         :param payload: See https://opensearch.org/docs/latest/security/access-control/api/#create-role-mapping for the details.
         :param role_name: The role you create a role mapping for. Create a role by {@link OpenSearchRole} class, or use `a predefined role <https://opensearch.org/docs/latest/security/access-control/users-roles/#predefined-roles>`_.
         '''
         if isinstance(payload, dict):
             payload = RoleMappingPayload(**payload)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__1af952f6c3707964cd4342b6a769c893ee65a7acf2a698f5c20d050a2a4e678b)
             check_type(argname="argument domain", value=domain, expected_type=type_hints["domain"])
-            check_type(argname="argument vpc", value=vpc, expected_type=type_hints["vpc"])
             check_type(argname="argument removal_policy", value=removal_policy, expected_type=type_hints["removal_policy"])
+            check_type(argname="argument vpc", value=vpc, expected_type=type_hints["vpc"])
             check_type(argname="argument payload", value=payload, expected_type=type_hints["payload"])
             check_type(argname="argument role_name", value=role_name, expected_type=type_hints["role_name"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "domain": domain,
-            "vpc": vpc,
             "payload": payload,
             "role_name": role_name,
         }
         if removal_policy is not None:
             self._values["removal_policy"] = removal_policy
+        if vpc is not None:
+            self._values["vpc"] = vpc
 
     @builtins.property
     def domain(self) -> _aws_cdk_aws_opensearchservice_ceddda9d.Domain:
         '''The OpenSearch domain you want to create a resource in.'''
         result = self._values.get("domain")
         assert result is not None, "Required property 'domain' is missing"
         return typing.cast(_aws_cdk_aws_opensearchservice_ceddda9d.Domain, result)
 
     @builtins.property
-    def vpc(self) -> _aws_cdk_aws_ec2_ceddda9d.IVpc:
-        '''The VPC your OpenSearch domain is in.'''
-        result = self._values.get("vpc")
-        assert result is not None, "Required property 'vpc' is missing"
-        return typing.cast(_aws_cdk_aws_ec2_ceddda9d.IVpc, result)
-
-    @builtins.property
     def removal_policy(self) -> typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy]:
         '''Policy to apply when the resource is removed from the stack.
 
         :default: RemovalPolicy.DESTROY
         '''
         result = self._values.get("removal_policy")
         return typing.cast(typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy], result)
 
     @builtins.property
+    def vpc(self) -> typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc]:
+        '''The VPC your OpenSearch domain is in.
+
+        :default: Assumes your Domain is not deployed within a VPC
+        '''
+        result = self._values.get("vpc")
+        return typing.cast(typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc], result)
+
+    @builtins.property
     def payload(self) -> RoleMappingPayload:
         '''See https://opensearch.org/docs/latest/security/access-control/api/#create-role-mapping for the details.'''
         result = self._values.get("payload")
         assert result is not None, "Required property 'payload' is missing"
         return typing.cast(RoleMappingPayload, result)
 
     @builtins.property
@@ -875,79 +883,82 @@
 
 
 @jsii.data_type(
     jsii_type="opensearch-rest-resources.OpenSearchRoleProps",
     jsii_struct_bases=[ResourcePropsBase],
     name_mapping={
         "domain": "domain",
-        "vpc": "vpc",
         "removal_policy": "removalPolicy",
+        "vpc": "vpc",
         "payload": "payload",
         "role_name": "roleName",
     },
 )
 class OpenSearchRoleProps(ResourcePropsBase):
     def __init__(
         self,
         *,
         domain: _aws_cdk_aws_opensearchservice_ceddda9d.Domain,
-        vpc: _aws_cdk_aws_ec2_ceddda9d.IVpc,
         removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
+        vpc: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc] = None,
         payload: typing.Union[RolePayload, typing.Dict[builtins.str, typing.Any]],
         role_name: builtins.str,
     ) -> None:
         '''
         :param domain: The OpenSearch domain you want to create a resource in.
-        :param vpc: The VPC your OpenSearch domain is in.
         :param removal_policy: Policy to apply when the resource is removed from the stack. Default: RemovalPolicy.DESTROY
+        :param vpc: The VPC your OpenSearch domain is in. Default: Assumes your Domain is not deployed within a VPC
         :param payload: See https://opensearch.org/docs/latest/security/access-control/api/#create-role for the details.
         :param role_name: The name of this role.
         '''
         if isinstance(payload, dict):
             payload = RolePayload(**payload)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__2b004c82f4d985ce97c47e706a94cf07027b40eefaffe2857093b1b9a2966f74)
             check_type(argname="argument domain", value=domain, expected_type=type_hints["domain"])
-            check_type(argname="argument vpc", value=vpc, expected_type=type_hints["vpc"])
             check_type(argname="argument removal_policy", value=removal_policy, expected_type=type_hints["removal_policy"])
+            check_type(argname="argument vpc", value=vpc, expected_type=type_hints["vpc"])
             check_type(argname="argument payload", value=payload, expected_type=type_hints["payload"])
             check_type(argname="argument role_name", value=role_name, expected_type=type_hints["role_name"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "domain": domain,
-            "vpc": vpc,
             "payload": payload,
             "role_name": role_name,
         }
         if removal_policy is not None:
             self._values["removal_policy"] = removal_policy
+        if vpc is not None:
+            self._values["vpc"] = vpc
 
     @builtins.property
     def domain(self) -> _aws_cdk_aws_opensearchservice_ceddda9d.Domain:
         '''The OpenSearch domain you want to create a resource in.'''
         result = self._values.get("domain")
         assert result is not None, "Required property 'domain' is missing"
         return typing.cast(_aws_cdk_aws_opensearchservice_ceddda9d.Domain, result)
 
     @builtins.property
-    def vpc(self) -> _aws_cdk_aws_ec2_ceddda9d.IVpc:
-        '''The VPC your OpenSearch domain is in.'''
-        result = self._values.get("vpc")
-        assert result is not None, "Required property 'vpc' is missing"
-        return typing.cast(_aws_cdk_aws_ec2_ceddda9d.IVpc, result)
-
-    @builtins.property
     def removal_policy(self) -> typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy]:
         '''Policy to apply when the resource is removed from the stack.
 
         :default: RemovalPolicy.DESTROY
         '''
         result = self._values.get("removal_policy")
         return typing.cast(typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy], result)
 
     @builtins.property
+    def vpc(self) -> typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc]:
+        '''The VPC your OpenSearch domain is in.
+
+        :default: Assumes your Domain is not deployed within a VPC
+        '''
+        result = self._values.get("vpc")
+        return typing.cast(typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc], result)
+
+    @builtins.property
     def payload(self) -> RolePayload:
         '''See https://opensearch.org/docs/latest/security/access-control/api/#create-role for the details.'''
         result = self._values.get("payload")
         assert result is not None, "Required property 'payload' is missing"
         return typing.cast(RolePayload, result)
 
     @builtins.property
@@ -970,79 +981,82 @@
 
 
 @jsii.data_type(
     jsii_type="opensearch-rest-resources.OpenSearchUserProps",
     jsii_struct_bases=[ResourcePropsBase],
     name_mapping={
         "domain": "domain",
-        "vpc": "vpc",
         "removal_policy": "removalPolicy",
+        "vpc": "vpc",
         "payload": "payload",
         "user_name": "userName",
     },
 )
 class OpenSearchUserProps(ResourcePropsBase):
     def __init__(
         self,
         *,
         domain: _aws_cdk_aws_opensearchservice_ceddda9d.Domain,
-        vpc: _aws_cdk_aws_ec2_ceddda9d.IVpc,
         removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
+        vpc: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc] = None,
         payload: typing.Union[UserPayload, typing.Dict[builtins.str, typing.Any]],
         user_name: builtins.str,
     ) -> None:
         '''
         :param domain: The OpenSearch domain you want to create a resource in.
-        :param vpc: The VPC your OpenSearch domain is in.
         :param removal_policy: Policy to apply when the resource is removed from the stack. Default: RemovalPolicy.DESTROY
+        :param vpc: The VPC your OpenSearch domain is in. Default: Assumes your Domain is not deployed within a VPC
         :param payload: See https://opensearch.org/docs/latest/security/access-control/api/#create-user for the details.
         :param user_name: The name of this user.
         '''
         if isinstance(payload, dict):
             payload = UserPayload(**payload)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__2e62d78568436419f29a2ab3ef0f6237e2b48cfd8f32a81c9cc98f1ebd718146)
             check_type(argname="argument domain", value=domain, expected_type=type_hints["domain"])
-            check_type(argname="argument vpc", value=vpc, expected_type=type_hints["vpc"])
             check_type(argname="argument removal_policy", value=removal_policy, expected_type=type_hints["removal_policy"])
+            check_type(argname="argument vpc", value=vpc, expected_type=type_hints["vpc"])
             check_type(argname="argument payload", value=payload, expected_type=type_hints["payload"])
             check_type(argname="argument user_name", value=user_name, expected_type=type_hints["user_name"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "domain": domain,
-            "vpc": vpc,
             "payload": payload,
             "user_name": user_name,
         }
         if removal_policy is not None:
             self._values["removal_policy"] = removal_policy
+        if vpc is not None:
+            self._values["vpc"] = vpc
 
     @builtins.property
     def domain(self) -> _aws_cdk_aws_opensearchservice_ceddda9d.Domain:
         '''The OpenSearch domain you want to create a resource in.'''
         result = self._values.get("domain")
         assert result is not None, "Required property 'domain' is missing"
         return typing.cast(_aws_cdk_aws_opensearchservice_ceddda9d.Domain, result)
 
     @builtins.property
-    def vpc(self) -> _aws_cdk_aws_ec2_ceddda9d.IVpc:
-        '''The VPC your OpenSearch domain is in.'''
-        result = self._values.get("vpc")
-        assert result is not None, "Required property 'vpc' is missing"
-        return typing.cast(_aws_cdk_aws_ec2_ceddda9d.IVpc, result)
-
-    @builtins.property
     def removal_policy(self) -> typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy]:
         '''Policy to apply when the resource is removed from the stack.
 
         :default: RemovalPolicy.DESTROY
         '''
         result = self._values.get("removal_policy")
         return typing.cast(typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy], result)
 
     @builtins.property
+    def vpc(self) -> typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc]:
+        '''The VPC your OpenSearch domain is in.
+
+        :default: Assumes your Domain is not deployed within a VPC
+        '''
+        result = self._values.get("vpc")
+        return typing.cast(typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc], result)
+
+    @builtins.property
     def payload(self) -> UserPayload:
         '''See https://opensearch.org/docs/latest/security/access-control/api/#create-user for the details.'''
         result = self._values.get("payload")
         assert result is not None, "Required property 'payload' is missing"
         return typing.cast(UserPayload, result)
 
     @builtins.property
@@ -1097,75 +1111,75 @@
 def _typecheckingstub__88b7de23b7128611fcf29d3404857d67dca8a603b41add8856c8e8e50273d72f(
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
     domain: _aws_cdk_aws_opensearchservice_ceddda9d.Domain,
     payload_json: builtins.str,
     rest_endpoint: builtins.str,
-    vpc: _aws_cdk_aws_ec2_ceddda9d.IVpc,
     removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
+    vpc: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__bdfb6ebf47fc374b01c571ea7c22a6ef12e6a8ba43b993c7a76b892ec0afda3a(
     *,
     domain: _aws_cdk_aws_opensearchservice_ceddda9d.Domain,
     payload_json: builtins.str,
     rest_endpoint: builtins.str,
-    vpc: _aws_cdk_aws_ec2_ceddda9d.IVpc,
     removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
+    vpc: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__11b3dbdadf9ad4e9eb287cd1fb49920a34f29982e1c81061e7655c436c58310e(
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
     payload: typing.Union[RolePayload, typing.Dict[builtins.str, typing.Any]],
     role_name: builtins.str,
     domain: _aws_cdk_aws_opensearchservice_ceddda9d.Domain,
-    vpc: _aws_cdk_aws_ec2_ceddda9d.IVpc,
     removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
+    vpc: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__a648bd6553d5af4908ea24e1f83ff607db47eb845ef54b6dc7d9a6e22a0d8c36(
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
     payload: typing.Union[RoleMappingPayload, typing.Dict[builtins.str, typing.Any]],
     role_name: builtins.str,
     domain: _aws_cdk_aws_opensearchservice_ceddda9d.Domain,
-    vpc: _aws_cdk_aws_ec2_ceddda9d.IVpc,
     removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
+    vpc: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__020b51bbd8211c5405011c19762bef3c8303e05f610a6b7e6f2b64bcf9151850(
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
     payload: typing.Union[UserPayload, typing.Dict[builtins.str, typing.Any]],
     user_name: builtins.str,
     domain: _aws_cdk_aws_opensearchservice_ceddda9d.Domain,
-    vpc: _aws_cdk_aws_ec2_ceddda9d.IVpc,
     removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
+    vpc: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__925237d929be76edf0f5d1670f8f84caac9877c0ca124747b7db826a1ad69fbc(
     *,
     domain: _aws_cdk_aws_opensearchservice_ceddda9d.Domain,
-    vpc: _aws_cdk_aws_ec2_ceddda9d.IVpc,
     removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
+    vpc: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__9f1cf8f23f1d4b6ee0af1c6ca2f78d22a4dd0c97fca39b46d40e032a11fd6eee(
     *,
     backend_roles: typing.Optional[typing.Sequence[builtins.str]] = None,
@@ -1202,36 +1216,36 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__1af952f6c3707964cd4342b6a769c893ee65a7acf2a698f5c20d050a2a4e678b(
     *,
     domain: _aws_cdk_aws_opensearchservice_ceddda9d.Domain,
-    vpc: _aws_cdk_aws_ec2_ceddda9d.IVpc,
     removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
+    vpc: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc] = None,
     payload: typing.Union[RoleMappingPayload, typing.Dict[builtins.str, typing.Any]],
     role_name: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__2b004c82f4d985ce97c47e706a94cf07027b40eefaffe2857093b1b9a2966f74(
     *,
     domain: _aws_cdk_aws_opensearchservice_ceddda9d.Domain,
-    vpc: _aws_cdk_aws_ec2_ceddda9d.IVpc,
     removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
+    vpc: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc] = None,
     payload: typing.Union[RolePayload, typing.Dict[builtins.str, typing.Any]],
     role_name: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__2e62d78568436419f29a2ab3ef0f6237e2b48cfd8f32a81c9cc98f1ebd718146(
     *,
     domain: _aws_cdk_aws_opensearchservice_ceddda9d.Domain,
-    vpc: _aws_cdk_aws_ec2_ceddda9d.IVpc,
     removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
+    vpc: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc] = None,
     payload: typing.Union[UserPayload, typing.Dict[builtins.str, typing.Any]],
     user_name: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `opensearch-rest-resources-0.0.7/src/opensearch_rest_resources.egg-info/PKG-INFO` & `opensearch-rest-resources-0.0.8/src/opensearch_rest_resources.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opensearch-rest-resources
-Version: 0.0.7
+Version: 0.0.8
 Summary: Manage OpenSearch REST resources from AWS CDK.
 Home-page: https://github.com/tmokmss/opensearch-rest-resources.git
 Author: tmokmss<tomookam@live.jp>
 License: MIT
 Project-URL: Source, https://github.com/tmokmss/opensearch-rest-resources.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -80,21 +80,20 @@
     removalPolicy: RemovalPolicy.RETAIN,
 });
 roleMapping.node.addDependency(role);
 ```
 
 ## Limitation
 
-Currently this library assumes your OpenSearch domain is configured as:
+Currently this library assumes your OpenSearch domain is configured such that:
 
 * [Fine-grained access control](https://docs.aws.amazon.com/opensearch-service/latest/developerguide/fgac.html) is enabled
-* Deployed within a VPC
 * Use the [`Domain`](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_opensearchservice.Domain.html) L2 construct
-* The credential for the master user (username and password) is stored in Secret Manager
-* [Domain access policy](https://docs.aws.amazon.com/opensearch-service/latest/developerguide/fgac.html#fgac-recommendations) is permissive enough like below:
+* The master is authenticated with username and password, and the credential is stored in Secret Manager
+* [Domain access policy](https://docs.aws.amazon.com/opensearch-service/latest/developerguide/fgac.html#fgac-recommendations) is configured to allow access from the master user
 
 ```json
 {
   "Version": "2012-10-17",
   "Statement": [
     {
       "Effect": "Allow",
```

### Comparing `opensearch-rest-resources-0.0.7/src/opensearch_rest_resources.egg-info/SOURCES.txt` & `opensearch-rest-resources-0.0.8/src/opensearch_rest_resources.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/opensearch_rest_resources/py.typed
 src/opensearch_rest_resources.egg-info/PKG-INFO
 src/opensearch_rest_resources.egg-info/SOURCES.txt
 src/opensearch_rest_resources.egg-info/dependency_links.txt
 src/opensearch_rest_resources.egg-info/requires.txt
 src/opensearch_rest_resources.egg-info/top_level.txt
 src/opensearch_rest_resources/_jsii/__init__.py
-src/opensearch_rest_resources/_jsii/opensearch-rest-resources@0.0.7.jsii.tgz
+src/opensearch_rest_resources/_jsii/opensearch-rest-resources@0.0.8.jsii.tgz
```

