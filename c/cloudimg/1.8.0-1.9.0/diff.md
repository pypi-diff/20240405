# Comparing `tmp/cloudimg-1.8.0.tar.gz` & `tmp/cloudimg-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudimg-1.8.0.tar", last modified: Wed Aug 16 08:54:32 2023, max compression
+gzip compressed data, was "cloudimg-1.9.0.tar", last modified: Tue Sep  5 22:26:16 2023, max compression
```

## Comparing `cloudimg-1.8.0.tar` & `cloudimg-1.9.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-16 08:54:32.974401 cloudimg-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-08-16 08:54:19.000000 cloudimg-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-08-16 08:54:19.000000 cloudimg-1.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-08-16 08:54:32.974401 cloudimg-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-08-16 08:54:19.000000 cloudimg-1.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-16 08:54:32.974401 cloudimg-1.8.0/cloudimg/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-16 08:54:19.000000 cloudimg-1.8.0/cloudimg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25885 2023-08-16 08:54:19.000000 cloudimg-1.8.0/cloudimg/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-08-16 08:54:19.000000 cloudimg-1.8.0/cloudimg/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    21006 2023-08-16 08:54:19.000000 cloudimg-1.8.0/cloudimg/ms_azure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-16 08:54:32.974401 cloudimg-1.8.0/cloudimg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-08-16 08:54:32.000000 cloudimg-1.8.0/cloudimg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-08-16 08:54:32.000000 cloudimg-1.8.0/cloudimg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-16 08:54:32.000000 cloudimg-1.8.0/cloudimg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-08-16 08:54:32.000000 cloudimg-1.8.0/cloudimg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-16 08:54:32.000000 cloudimg-1.8.0/cloudimg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-16 08:54:19.000000 cloudimg-1.8.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-08-16 08:54:19.000000 cloudimg-1.8.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-16 08:54:32.974401 cloudimg-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-08-16 08:54:19.000000 cloudimg-1.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-16 08:54:32.974401 cloudimg-1.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    35880 2023-08-16 08:54:19.000000 cloudimg-1.8.0/tests/test_aws.py
--rw-r--r--   0 runner    (1001) docker     (123)    27301 2023-08-16 08:54:19.000000 cloudimg-1.8.0/tests/test_azure.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-08-16 08:54:19.000000 cloudimg-1.8.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 22:26:16.800579 cloudimg-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (999)    35147 2023-09-05 22:26:06.000000 cloudimg-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (999)      124 2023-09-05 22:26:06.000000 cloudimg-1.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (999)      690 2023-09-05 22:26:16.800579 cloudimg-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)     1504 2023-09-05 22:26:06.000000 cloudimg-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 22:26:16.796579 cloudimg-1.9.0/cloudimg/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 22:26:06.000000 cloudimg-1.9.0/cloudimg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)    27008 2023-09-05 22:26:06.000000 cloudimg-1.9.0/cloudimg/aws.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4224 2023-09-05 22:26:06.000000 cloudimg-1.9.0/cloudimg/common.py
+-rw-r--r--   0 runner    (1001) docker     (999)    21006 2023-09-05 22:26:06.000000 cloudimg-1.9.0/cloudimg/ms_azure.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 22:26:16.800579 cloudimg-1.9.0/cloudimg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (999)      690 2023-09-05 22:26:16.000000 cloudimg-1.9.0/cloudimg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)      359 2023-09-05 22:26:16.000000 cloudimg-1.9.0/cloudimg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (999)        1 2023-09-05 22:26:16.000000 cloudimg-1.9.0/cloudimg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       96 2023-09-05 22:26:16.000000 cloudimg-1.9.0/cloudimg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (999)        9 2023-09-05 22:26:16.000000 cloudimg-1.9.0/cloudimg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (999)      171 2023-09-05 22:26:06.000000 cloudimg-1.9.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       93 2023-09-05 22:26:06.000000 cloudimg-1.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       38 2023-09-05 22:26:16.800579 cloudimg-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (999)      988 2023-09-05 22:26:06.000000 cloudimg-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 22:26:16.800579 cloudimg-1.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (999)    39173 2023-09-05 22:26:06.000000 cloudimg-1.9.0/tests/test_aws.py
+-rw-r--r--   0 runner    (1001) docker     (999)    27301 2023-09-05 22:26:06.000000 cloudimg-1.9.0/tests/test_azure.py
+-rw-r--r--   0 runner    (1001) docker     (999)      551 2023-09-05 22:26:06.000000 cloudimg-1.9.0/tox.ini
```

### Comparing `cloudimg-1.8.0/LICENSE` & `cloudimg-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudimg-1.8.0/PKG-INFO` & `cloudimg-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: cloudimg
-Version: 1.8.0
+Version: 1.9.0
 Summary: Services for building and releasing products in cloud environments
 Home-page: https://github.com/release-engineering/cloudimg
 Author: Alex Misstear
 Author-email: amisstea@redhat.com
 License: GPLv3
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `cloudimg-1.8.0/README.md` & `cloudimg-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `cloudimg-1.8.0/cloudimg/aws.py` & `cloudimg-1.9.0/cloudimg/aws.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import enum
 import logging
 import os
 import threading
 import time
 import lzma
 
 from boto3.session import Session
@@ -23,39 +24,63 @@
 class SnapshotTimeout(Exception):
     """
     Raised when a snapshot related timeout occurs.
     """
     pass
 
 
+class AWSBootMode(enum.Enum):
+    """The boot mode options supported by AWS when registering an AMI."""
+
+    uefi = "uefi"
+    """Support UEFI only."""
+
+    bios = "legacy-bios"
+    """Support BIOS only."""
+
+    hybrid = "uefi-preferred"
+    """Support UEFI and BIOS giving the preference to UEFI."""
+
+    not_set = None
+    """Use the default boot mode from AWS."""
+
+
 class AWSPublishingMetadata(PublishingMetadata):
     """
     A collection of metadata necessary for uploading and publishing a disk
     image to AWS.
 
     Args:
         ena_support (bool, optional): Enables enhanced network adapters. By
                                       default this option is enabled.
         sriov_net_support (str, optional): Set to 'simple' to enable enhanced
                                            network adapters for Intel 82599 VF
                                            interfaces. By default this option
                                            is enabled.
         billing_products (list, optional): Billing product identifiers
+
+        boot_mode (str, optional): The boot mode for booting up the AMI on EC2.
     """
 
     def __init__(self, *args, **kwargs):
         self.ena_support = kwargs.pop('ena_support', True)
         self.sriov_net_support = kwargs.pop('sriov_net_support', 'simple')
         self.billing_products = kwargs.pop('billing_products', None)
+        bmode_str = kwargs.pop('boot_mode', None) or "not_set"
+        self.boot_mode = AWSBootMode[bmode_str]
 
         super(AWSPublishingMetadata, self).__init__(*args, **kwargs)
 
-        # Convert uefi_support bool into AWS specific values
-        self.boot_mode = "uefi-preferred" if self.uefi_support \
-            else "legacy-bios"
+        # Set the UEFI mode when the boolean is used instead of Enum.
+        if (
+            self.boot_mode == AWSBootMode.not_set and
+            self.uefi_support is not None
+        ):
+            self.boot_mode = AWSBootMode.hybrid if self.uefi_support \
+                             else AWSBootMode.bios
 
         assert self.container, 'A container must be defined'
 
 
 class AWSDeleteMetadata(DeleteMetadata):
     pass
 
@@ -632,26 +657,35 @@
             'Ebs': {
                 'SnapshotId': snapshot.id,
                 'VolumeType': metadata.volume_type,
                 'DeleteOnTermination': True,
             },
         }]
 
+        # Here we just set the "BootMode" whenever we have a proper
+        # value for it. Otherwise we leave it so AWS will use the
+        # instance type default.
+        #
+        # https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ami-boot.html
+        optional_kwargs = {}
+        if metadata.boot_mode != AWSBootMode.not_set:
+            optional_kwargs["BootMode"] = metadata.boot_mode.value
+
         log.info('Registering image: %s', metadata.image_name)
         image = self.ec2.register_image(
             Name=metadata.image_name,
             Description=metadata.description,
             Architecture=metadata.arch,
             VirtualizationType=metadata.virt_type,
             RootDeviceName=metadata.root_device_name,
             BlockDeviceMappings=block_device_mapping,
             EnaSupport=metadata.ena_support,
             SriovNetSupport=metadata.sriov_net_support,
             BillingProducts=metadata.billing_products,
-            BootMode=metadata.boot_mode
+            **optional_kwargs,
         )
         if metadata.tags:
             self.tag_image(image, metadata.tags)
         return image
 
     def share_image(self, image, accounts=[], groups=[]):
         """
```

### Comparing `cloudimg-1.8.0/cloudimg/common.py` & `cloudimg-1.9.0/cloudimg/common.py`

 * *Files identical despite different names*

### Comparing `cloudimg-1.8.0/cloudimg/ms_azure.py` & `cloudimg-1.9.0/cloudimg/ms_azure.py`

 * *Files identical despite different names*

### Comparing `cloudimg-1.8.0/cloudimg.egg-info/PKG-INFO` & `cloudimg-1.9.0/cloudimg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: cloudimg
-Version: 1.8.0
+Version: 1.9.0
 Summary: Services for building and releasing products in cloud environments
 Home-page: https://github.com/release-engineering/cloudimg
 Author: Alex Misstear
 Author-email: amisstea@redhat.com
 License: GPLv3
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `cloudimg-1.8.0/setup.py` & `cloudimg-1.9.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cloudimg',
-    version='1.8.0',
+    version='1.9.0',
     author='Alex Misstear',
     author_email='amisstea@redhat.com',
     description=('Services for building and releasing products in cloud '
                  'environments'),
     license='GPLv3',
     url='https://github.com/release-engineering/cloudimg',
     packages=find_packages(),
```

### Comparing `cloudimg-1.8.0/tests/test_aws.py` & `cloudimg-1.9.0/tests/test_aws.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from copy import deepcopy
 from tempfile import NamedTemporaryFile
 import unittest
 
 from unittest.mock import MagicMock, patch
 
 from cloudimg.aws import (
-    AWSService, AWSPublishingMetadata, ClientError,
+    AWSBootMode, AWSService, AWSPublishingMetadata, ClientError,
     SnapshotError, SnapshotTimeout, AWSDeleteMetadata, UploadProgress
 )
 
 
 class TestAWSPublishingMetadata(unittest.TestCase):
 
     def test_container_not_defined(self):
@@ -608,15 +608,14 @@
             Architecture=self.md.arch,
             VirtualizationType=self.md.virt_type,
             RootDeviceName=self.md.root_device_name,
             BlockDeviceMappings=block_device_mapping,
             EnaSupport=self.md.ena_support,
             SriovNetSupport=self.md.sriov_net_support,
             BillingProducts=self.md.billing_products,
-            BootMode=self.md.boot_mode
         )
         tag_image.assert_not_called()
         self.assertEqual(res, "fakeimg")
 
     @patch('cloudimg.aws.AWSService.tag_image')
     def test_register_image_tags(self, tag_image):
         self.md.tags = {"tag": "tag"}
@@ -624,14 +623,96 @@
 
         res = self.svc.register_image(MagicMock(), self.md)
 
         self.mock_register_image.assert_called_once()
         tag_image.assert_called_once_with("fakeimg", self.md.tags)
         self.assertEqual(res, "fakeimg")
 
+    @patch('cloudimg.aws.AWSService.tag_image')
+    def test_register_image_boot_mode(self, tag_image):
+        self.mock_register_image.return_value = "fakeimg"
+        boot_modes = ["uefi", "bios", "hybrid"]
+
+        for bmode in boot_modes:
+            self.md.boot_mode = AWSBootMode[bmode]
+            mock_snapshot = MagicMock()
+            mock_snapshot.id = 'foo'
+            block_device_mapping = [{
+                'DeviceName': self.md.root_device_name,
+                'Ebs': {
+                    'SnapshotId': mock_snapshot.id,
+                    'VolumeType': self.md.volume_type,
+                    'DeleteOnTermination': True,
+                },
+            }]
+
+            res = self.svc.register_image(mock_snapshot, self.md)
+
+            self.mock_register_image.assert_called_once_with(
+                Name=self.md.image_name,
+                Description=self.md.description,
+                Architecture=self.md.arch,
+                VirtualizationType=self.md.virt_type,
+                RootDeviceName=self.md.root_device_name,
+                BlockDeviceMappings=block_device_mapping,
+                EnaSupport=self.md.ena_support,
+                SriovNetSupport=self.md.sriov_net_support,
+                BillingProducts=self.md.billing_products,
+                BootMode=AWSBootMode[bmode].value
+            )
+            tag_image.assert_not_called()
+            self.assertEqual(res, "fakeimg")
+            self.mock_register_image.reset_mock()
+            tag_image.reset_mock()
+
+    @patch('cloudimg.aws.AWSService.tag_image')
+    def test_register_image_uefi_support_bool(self, tag_image):
+        self.mock_register_image.return_value = "fakeimg"
+        uefi_support_map = {
+            True: AWSBootMode.hybrid,
+            False: AWSBootMode.bios,
+        }
+
+        for bool_value, b_mode in uefi_support_map.items():
+            self.md = AWSPublishingMetadata(
+                image_path='/some/fake/path/to/image.raw',
+                image_name='fakeimagename',
+                container='fakecontainername',
+                uefi_support=bool_value,
+            )
+            mock_snapshot = MagicMock()
+            mock_snapshot.id = 'foo'
+            block_device_mapping = [{
+                'DeviceName': self.md.root_device_name,
+                'Ebs': {
+                    'SnapshotId': mock_snapshot.id,
+                    'VolumeType': self.md.volume_type,
+                    'DeleteOnTermination': True,
+                },
+            }]
+
+            res = self.svc.register_image(mock_snapshot, self.md)
+
+            self.mock_register_image.assert_called_once_with(
+                Name=self.md.image_name,
+                Description=self.md.description,
+                Architecture=self.md.arch,
+                VirtualizationType=self.md.virt_type,
+                RootDeviceName=self.md.root_device_name,
+                BlockDeviceMappings=block_device_mapping,
+                EnaSupport=self.md.ena_support,
+                SriovNetSupport=self.md.sriov_net_support,
+                BillingProducts=self.md.billing_products,
+                BootMode=b_mode.value,
+            )
+            tag_image.assert_not_called()
+            self.assertEqual(res, "fakeimg")
+            self.mock_register_image.reset_mock()
+            tag_image.reset_mock()
+
     def test_deregister_image(self):
         image = MagicMock()
         out = self.svc.deregister_image(image)
         image.deregister.assert_called_once()
         assert out
 
     def test_delete_snapshot(self):
```

### Comparing `cloudimg-1.8.0/tests/test_azure.py` & `cloudimg-1.9.0/tests/test_azure.py`

 * *Files identical despite different names*

### Comparing `cloudimg-1.8.0/tox.ini` & `cloudimg-1.9.0/tox.ini`

 * *Files identical despite different names*

