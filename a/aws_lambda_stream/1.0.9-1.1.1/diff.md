# Comparing `tmp/aws_lambda_stream-1.0.9.tar.gz` & `tmp/aws_lambda_stream-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_lambda_stream-1.0.9.tar", max compression
+gzip compressed data, was "aws_lambda_stream-1.1.1.tar", max compression
```

## Comparing `aws_lambda_stream-1.0.9.tar` & `aws_lambda_stream-1.1.1.tar`

### file list

```diff
@@ -1,58 +1,62 @@
--rw-r--r--   0        0        0     1076 2023-02-08 05:37:14.950615 aws_lambda_stream-1.0.9/LICENSE
--rw-r--r--   0        0        0      478 2023-02-08 06:37:38.252467 aws_lambda_stream-1.0.9/README.md
--rw-r--r--   0        0        0      747 2023-02-03 18:24:04.273418 aws_lambda_stream-1.0.9/aws_lambda_stream/__init__.py
--rw-r--r--   0        0        0      352 2023-03-01 04:00:26.276550 aws_lambda_stream-1.0.9/aws_lambda_stream/connectors/__init__.py
--rw-r--r--   0        0        0     1602 2023-02-03 19:26:10.049622 aws_lambda_stream-1.0.9/aws_lambda_stream/connectors/dynamodb.py
--rw-r--r--   0        0        0     3509 2022-11-10 14:59:59.886154 aws_lambda_stream-1.0.9/aws_lambda_stream/connectors/elasticsearch.py
--rw-r--r--   0        0        0      221 2022-10-05 04:58:41.716315 aws_lambda_stream-1.0.9/aws_lambda_stream/connectors/eventbridge.py
--rw-r--r--   0        0        0      186 2023-03-01 03:52:09.979571 aws_lambda_stream-1.0.9/aws_lambda_stream/connectors/lambda_.py
--rw-r--r--   0        0        0      908 2022-10-12 14:15:26.216275 aws_lambda_stream-1.0.9/aws_lambda_stream/connectors/s3.py
--rw-r--r--   0        0        0      678 2023-02-14 05:33:36.467074 aws_lambda_stream-1.0.9/aws_lambda_stream/connectors/sns.py
--rw-r--r--   0        0        0      563 2023-02-14 05:28:39.331132 aws_lambda_stream-1.0.9/aws_lambda_stream/connectors/sqs.py
--rw-r--r--   0        0        0       70 2022-09-07 12:25:07.481058 aws_lambda_stream-1.0.9/aws_lambda_stream/events/__init__.py
--rw-r--r--   0        0        0     4650 2023-02-16 05:15:17.334571 aws_lambda_stream-1.0.9/aws_lambda_stream/events/dynamodb.py
--rw-r--r--   0        0        0     1016 2023-02-08 23:12:04.697392 aws_lambda_stream-1.0.9/aws_lambda_stream/events/kinesis.py
--rw-r--r--   0        0        0     2301 2023-02-03 18:24:04.276261 aws_lambda_stream-1.0.9/aws_lambda_stream/events/s3.py
--rw-r--r--   0        0        0     2073 2023-02-03 18:24:04.276592 aws_lambda_stream-1.0.9/aws_lambda_stream/events/sns.py
--rw-r--r--   0        0        0     1470 2023-02-03 18:24:04.277239 aws_lambda_stream-1.0.9/aws_lambda_stream/events/sqs.py
--rw-r--r--   0        0        0      172 2023-02-03 18:24:04.278143 aws_lambda_stream-1.0.9/aws_lambda_stream/filters/__init__.py
--rw-r--r--   0        0        0      204 2023-02-03 18:24:04.278452 aws_lambda_stream-1.0.9/aws_lambda_stream/filters/content.py
--rw-r--r--   0        0        0      639 2022-11-15 14:34:45.024830 aws_lambda_stream-1.0.9/aws_lambda_stream/filters/event_type.py
--rw-r--r--   0        0        0      754 2023-02-08 03:34:42.274970 aws_lambda_stream-1.0.9/aws_lambda_stream/filters/latch.py
--rw-r--r--   0        0        0      504 2023-02-03 18:24:04.278934 aws_lambda_stream-1.0.9/aws_lambda_stream/filters/skip.py
--rw-r--r--   0        0        0        0 2022-10-05 03:29:29.473147 aws_lambda_stream-1.0.9/aws_lambda_stream/flavors/__init__.py
--rw-r--r--   0        0        0     1041 2023-02-07 23:38:45.570357 aws_lambda_stream-1.0.9/aws_lambda_stream/flavors/cdc.py
--rw-r--r--   0        0        0     2487 2023-02-03 18:24:04.279800 aws_lambda_stream-1.0.9/aws_lambda_stream/flavors/collect.py
--rw-r--r--   0        0        0     2820 2023-02-03 18:24:04.280222 aws_lambda_stream-1.0.9/aws_lambda_stream/flavors/correlate.py
--rw-r--r--   0        0        0     1071 2023-02-03 18:24:04.281121 aws_lambda_stream-1.0.9/aws_lambda_stream/flavors/elasticsearch.py
--rw-r--r--   0        0        0     7191 2023-02-22 21:55:44.377898 aws_lambda_stream-1.0.9/aws_lambda_stream/flavors/evaluate.py
--rw-r--r--   0        0        0     1124 2023-02-08 03:37:45.548460 aws_lambda_stream-1.0.9/aws_lambda_stream/flavors/materialize.py
--rw-r--r--   0        0        0      992 2023-02-08 04:33:57.896213 aws_lambda_stream-1.0.9/aws_lambda_stream/flavors/s3.py
--rw-r--r--   0        0        0      896 2023-02-03 18:24:04.282923 aws_lambda_stream-1.0.9/aws_lambda_stream/flavors/sns.py
--rw-r--r--   0        0        0     2813 2023-03-01 04:42:58.732633 aws_lambda_stream-1.0.9/aws_lambda_stream/flavors/task.py
--rw-r--r--   0        0        0     2892 2023-02-16 05:07:21.062429 aws_lambda_stream-1.0.9/aws_lambda_stream/pipelines/__init__.py
--rw-r--r--   0        0        0     3570 2023-02-16 05:06:42.204097 aws_lambda_stream-1.0.9/aws_lambda_stream/repositories/__init__.py
--rw-r--r--   0        0        0      436 2022-10-05 03:50:07.747050 aws_lambda_stream-1.0.9/aws_lambda_stream/utils/__init__.py
--rw-r--r--   0        0        0      140 2023-02-14 05:32:21.038521 aws_lambda_stream-1.0.9/aws_lambda_stream/utils/aws.py
--rw-r--r--   0        0        0      153 2022-10-05 04:49:33.238263 aws_lambda_stream-1.0.9/aws_lambda_stream/utils/batch.py
--rw-r--r--   0        0        0      244 2022-10-05 04:49:17.299087 aws_lambda_stream-1.0.9/aws_lambda_stream/utils/concurrency.py
--rw-r--r--   0        0        0      163 2022-10-05 04:43:54.856386 aws_lambda_stream-1.0.9/aws_lambda_stream/utils/decorators.py
--rw-r--r--   0        0        0     4794 2023-02-08 23:10:24.837093 aws_lambda_stream-1.0.9/aws_lambda_stream/utils/dynamodb.py
--rw-r--r--   0        0        0     1889 2023-02-14 06:26:12.182019 aws_lambda_stream-1.0.9/aws_lambda_stream/utils/elasticsearch.py
--rw-r--r--   0        0        0     2256 2023-02-09 19:29:00.766950 aws_lambda_stream-1.0.9/aws_lambda_stream/utils/eventbridge.py
--rw-r--r--   0        0        0     2750 2023-02-03 18:24:04.286064 aws_lambda_stream-1.0.9/aws_lambda_stream/utils/faults.py
--rw-r--r--   0        0        0      413 2023-02-03 18:24:04.286668 aws_lambda_stream-1.0.9/aws_lambda_stream/utils/filters.py
--rw-r--r--   0        0        0      333 2023-02-03 18:24:04.287082 aws_lambda_stream-1.0.9/aws_lambda_stream/utils/json_encoder.py
--rw-r--r--   0        0        0      558 2023-03-01 04:10:54.251855 aws_lambda_stream-1.0.9/aws_lambda_stream/utils/lambda_.py
--rw-r--r--   0        0        0      618 2022-09-20 05:37:59.968618 aws_lambda_stream-1.0.9/aws_lambda_stream/utils/logger.py
--rw-r--r--   0        0        0     1982 2023-02-03 18:24:04.287769 aws_lambda_stream-1.0.9/aws_lambda_stream/utils/operators.py
--rw-r--r--   0        0        0      268 2022-10-05 03:53:16.892335 aws_lambda_stream-1.0.9/aws_lambda_stream/utils/opt.py
--rw-r--r--   0        0        0      345 2022-11-15 05:45:17.281224 aws_lambda_stream-1.0.9/aws_lambda_stream/utils/pluralize.py
--rw-r--r--   0        0        0      440 2022-10-12 16:28:48.582840 aws_lambda_stream-1.0.9/aws_lambda_stream/utils/s3.py
--rw-r--r--   0        0        0      908 2022-11-15 05:25:05.442119 aws_lambda_stream-1.0.9/aws_lambda_stream/utils/sns.py
--rw-r--r--   0        0        0      964 2023-02-09 19:19:31.634487 aws_lambda_stream-1.0.9/aws_lambda_stream/utils/split.py
--rw-r--r--   0        0        0      994 2023-02-03 18:24:04.288012 aws_lambda_stream-1.0.9/aws_lambda_stream/utils/tags.py
--rw-r--r--   0        0        0      370 2023-02-03 18:24:04.288204 aws_lambda_stream-1.0.9/aws_lambda_stream/utils/time.py
--rw-r--r--   0        0        0      609 2023-03-01 05:04:42.270007 aws_lambda_stream-1.0.9/pyproject.toml
--rw-r--r--   0        0        0     1550 2023-03-01 05:05:26.601549 aws_lambda_stream-1.0.9/setup.py
--rw-r--r--   0        0        0     1287 2023-03-01 05:05:26.601696 aws_lambda_stream-1.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-02-08 05:37:14.950615 aws_lambda_stream-1.1.1/LICENSE
+-rw-r--r--   0        0        0      882 2023-07-20 01:42:51.651718 aws_lambda_stream-1.1.1/README.md
+-rw-r--r--   0        0        0      747 2023-03-22 23:49:01.698319 aws_lambda_stream-1.1.1/aws_lambda_stream/__init__.py
+-rw-r--r--   0        0        0      409 2023-03-23 15:58:19.551309 aws_lambda_stream-1.1.1/aws_lambda_stream/connectors/__init__.py
+-rw-r--r--   0        0        0      245 2024-04-05 05:09:27.902257 aws_lambda_stream-1.1.1/aws_lambda_stream/connectors/cloudwatch.py
+-rw-r--r--   0        0        0     3249 2024-04-05 05:09:30.949910 aws_lambda_stream-1.1.1/aws_lambda_stream/connectors/dynamodb.py
+-rw-r--r--   0        0        0     3509 2022-11-10 14:59:59.886154 aws_lambda_stream-1.1.1/aws_lambda_stream/connectors/elasticsearch.py
+-rw-r--r--   0        0        0      260 2024-04-05 05:06:54.782848 aws_lambda_stream-1.1.1/aws_lambda_stream/connectors/eventbridge.py
+-rw-r--r--   0        0        0      224 2024-04-05 05:09:42.303801 aws_lambda_stream-1.1.1/aws_lambda_stream/connectors/lambda_.py
+-rw-r--r--   0        0        0      950 2024-04-05 05:09:52.136330 aws_lambda_stream-1.1.1/aws_lambda_stream/connectors/s3.py
+-rw-r--r--   0        0        0      715 2024-04-05 05:07:56.740726 aws_lambda_stream-1.1.1/aws_lambda_stream/connectors/sns.py
+-rw-r--r--   0        0        0      603 2024-04-05 05:08:13.436957 aws_lambda_stream-1.1.1/aws_lambda_stream/connectors/sqs.py
+-rw-r--r--   0        0        0       70 2022-09-07 12:25:07.481058 aws_lambda_stream-1.1.1/aws_lambda_stream/events/__init__.py
+-rw-r--r--   0        0        0     4891 2023-10-24 23:27:55.788628 aws_lambda_stream-1.1.1/aws_lambda_stream/events/dynamodb.py
+-rw-r--r--   0        0        0     1151 2023-10-24 23:22:13.708172 aws_lambda_stream-1.1.1/aws_lambda_stream/events/kinesis.py
+-rw-r--r--   0        0        0     2299 2023-03-23 19:20:35.970538 aws_lambda_stream-1.1.1/aws_lambda_stream/events/s3.py
+-rw-r--r--   0        0        0     2073 2023-02-03 18:24:04.276592 aws_lambda_stream-1.1.1/aws_lambda_stream/events/sns.py
+-rw-r--r--   0        0        0     1470 2023-02-03 18:24:04.277239 aws_lambda_stream-1.1.1/aws_lambda_stream/events/sqs.py
+-rw-r--r--   0        0        0      172 2023-02-03 18:24:04.278143 aws_lambda_stream-1.1.1/aws_lambda_stream/filters/__init__.py
+-rw-r--r--   0        0        0      204 2023-02-03 18:24:04.278452 aws_lambda_stream-1.1.1/aws_lambda_stream/filters/content.py
+-rw-r--r--   0        0        0      639 2022-11-15 14:34:45.024830 aws_lambda_stream-1.1.1/aws_lambda_stream/filters/event_type.py
+-rw-r--r--   0        0        0      754 2023-02-08 03:34:42.274970 aws_lambda_stream-1.1.1/aws_lambda_stream/filters/latch.py
+-rw-r--r--   0        0        0      504 2023-02-03 18:24:04.278934 aws_lambda_stream-1.1.1/aws_lambda_stream/filters/skip.py
+-rw-r--r--   0        0        0        0 2022-10-05 03:29:29.473147 aws_lambda_stream-1.1.1/aws_lambda_stream/flavors/__init__.py
+-rw-r--r--   0        0        0     1033 2023-07-28 14:02:21.679238 aws_lambda_stream-1.1.1/aws_lambda_stream/flavors/cdc.py
+-rw-r--r--   0        0        0     2487 2023-02-03 18:24:04.279800 aws_lambda_stream-1.1.1/aws_lambda_stream/flavors/collect.py
+-rw-r--r--   0        0        0     2820 2023-02-03 18:24:04.280222 aws_lambda_stream-1.1.1/aws_lambda_stream/flavors/correlate.py
+-rw-r--r--   0        0        0     1015 2023-07-28 14:02:21.679644 aws_lambda_stream-1.1.1/aws_lambda_stream/flavors/elasticsearch.py
+-rw-r--r--   0        0        0     7265 2023-07-28 14:02:21.679983 aws_lambda_stream-1.1.1/aws_lambda_stream/flavors/evaluate.py
+-rw-r--r--   0        0        0     1124 2023-06-20 04:55:40.314770 aws_lambda_stream-1.1.1/aws_lambda_stream/flavors/materialize.py
+-rw-r--r--   0        0        0      992 2023-02-08 04:33:57.896213 aws_lambda_stream-1.1.1/aws_lambda_stream/flavors/s3.py
+-rw-r--r--   0        0        0      896 2023-02-03 18:24:04.282923 aws_lambda_stream-1.1.1/aws_lambda_stream/flavors/sns.py
+-rw-r--r--   0        0        0     2790 2023-07-28 14:02:21.680228 aws_lambda_stream-1.1.1/aws_lambda_stream/flavors/task.py
+-rw-r--r--   0        0        0     2806 2023-07-28 14:02:21.681145 aws_lambda_stream-1.1.1/aws_lambda_stream/pipelines/__init__.py
+-rw-r--r--   0        0        0     3693 2023-04-06 14:36:11.361064 aws_lambda_stream-1.1.1/aws_lambda_stream/repositories/__init__.py
+-rw-r--r--   0        0        0      436 2022-10-05 03:50:07.747050 aws_lambda_stream-1.1.1/aws_lambda_stream/utils/__init__.py
+-rw-r--r--   0        0        0     1361 2023-04-06 14:36:18.917107 aws_lambda_stream-1.1.1/aws_lambda_stream/utils/apigateway.py
+-rw-r--r--   0        0        0      140 2023-02-14 05:32:21.038521 aws_lambda_stream-1.1.1/aws_lambda_stream/utils/aws.py
+-rw-r--r--   0        0        0      153 2022-10-05 04:49:33.238263 aws_lambda_stream-1.1.1/aws_lambda_stream/utils/batch.py
+-rw-r--r--   0        0        0      538 2023-03-23 16:10:15.770876 aws_lambda_stream-1.1.1/aws_lambda_stream/utils/cloudwatch.py
+-rw-r--r--   0        0        0     1334 2023-06-21 01:32:44.777692 aws_lambda_stream-1.1.1/aws_lambda_stream/utils/concurrency.py
+-rw-r--r--   0        0        0      163 2022-10-05 04:43:54.856386 aws_lambda_stream-1.1.1/aws_lambda_stream/utils/decorators.py
+-rw-r--r--   0        0        0     5572 2023-04-10 01:56:19.355174 aws_lambda_stream-1.1.1/aws_lambda_stream/utils/dynamodb.py
+-rw-r--r--   0        0        0     2504 2023-07-28 14:02:21.681495 aws_lambda_stream-1.1.1/aws_lambda_stream/utils/elasticsearch.py
+-rw-r--r--   0        0        0     2454 2023-09-23 16:57:16.981960 aws_lambda_stream-1.1.1/aws_lambda_stream/utils/eventbridge.py
+-rw-r--r--   0        0        0     2660 2023-07-28 14:02:21.682559 aws_lambda_stream-1.1.1/aws_lambda_stream/utils/faults.py
+-rw-r--r--   0        0        0      413 2023-02-03 18:24:04.286668 aws_lambda_stream-1.1.1/aws_lambda_stream/utils/filters.py
+-rw-r--r--   0        0        0      333 2023-02-03 18:24:04.287082 aws_lambda_stream-1.1.1/aws_lambda_stream/utils/json_encoder.py
+-rw-r--r--   0        0        0      558 2023-03-01 04:10:54.251855 aws_lambda_stream-1.1.1/aws_lambda_stream/utils/lambda_.py
+-rw-r--r--   0        0        0      618 2022-09-20 05:37:59.968618 aws_lambda_stream-1.1.1/aws_lambda_stream/utils/logger.py
+-rw-r--r--   0        0        0     1982 2023-02-03 18:24:04.287769 aws_lambda_stream-1.1.1/aws_lambda_stream/utils/operators.py
+-rw-r--r--   0        0        0      268 2022-10-05 03:53:16.892335 aws_lambda_stream-1.1.1/aws_lambda_stream/utils/opt.py
+-rw-r--r--   0        0        0      345 2022-11-15 05:45:17.281224 aws_lambda_stream-1.1.1/aws_lambda_stream/utils/pluralize.py
+-rw-r--r--   0        0        0      646 2023-04-10 01:56:19.355426 aws_lambda_stream-1.1.1/aws_lambda_stream/utils/retry.py
+-rw-r--r--   0        0        0     2792 2023-03-22 23:47:26.627754 aws_lambda_stream-1.1.1/aws_lambda_stream/utils/s3.py
+-rw-r--r--   0        0        0      950 2023-03-03 19:53:38.454506 aws_lambda_stream-1.1.1/aws_lambda_stream/utils/sns.py
+-rw-r--r--   0        0        0      964 2023-02-09 19:19:31.634487 aws_lambda_stream-1.1.1/aws_lambda_stream/utils/split.py
+-rw-r--r--   0        0        0     1569 2023-07-28 14:02:21.683502 aws_lambda_stream-1.1.1/aws_lambda_stream/utils/sqs.py
+-rw-r--r--   0        0        0     1045 2023-09-23 16:57:24.696498 aws_lambda_stream-1.1.1/aws_lambda_stream/utils/tags.py
+-rw-r--r--   0        0        0      370 2023-02-03 18:24:04.288204 aws_lambda_stream-1.1.1/aws_lambda_stream/utils/time.py
+-rw-r--r--   0        0        0      665 2024-04-05 05:10:54.286953 aws_lambda_stream-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1786 1970-01-01 00:00:00.000000 aws_lambda_stream-1.1.1/PKG-INFO
```

### Comparing `aws_lambda_stream-1.0.9/LICENSE` & `aws_lambda_stream-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aws_lambda_stream-1.0.9/aws_lambda_stream/__init__.py` & `aws_lambda_stream-1.1.1/aws_lambda_stream/__init__.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_stream-1.0.9/aws_lambda_stream/connectors/elasticsearch.py` & `aws_lambda_stream-1.1.1/aws_lambda_stream/connectors/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_stream-1.0.9/aws_lambda_stream/connectors/s3.py` & `aws_lambda_stream-1.1.1/aws_lambda_stream/connectors/s3.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 import boto3
 
 
 class Connector():
-    def __init__(self, bucket_name) -> None:
+
+    def __init__(self, bucket_name, client = None) -> None:
         self.bucket_name = bucket_name
-        self.client = boto3.client('s3')
+        self.client = client if client else boto3.client('s3')
+
     def put_object(self, input_params):
         params = {
             'Bucket': self.bucket_name,
             **input_params
         }
         return self.client.put_object(**params)
+
     def get_object(self, input_params):
         params = {
             'Bucket': self.bucket_name,
             **input_params
         }
         return self.client.get_object(**params)
+
     def list_objects(self, input_params):
         params = {
             'Bucket': self.bucket_name,
             **input_params
         }
         return self.client.list_objects_v2(**params)
+
     def delete_object(self, input_params):
         params = {
             'Bucket': self.bucket_name,
             **input_params
         }
         return self.client.delete_object(**params)
```

### Comparing `aws_lambda_stream-1.0.9/aws_lambda_stream/connectors/sns.py` & `aws_lambda_stream-1.1.1/aws_lambda_stream/connectors/sns.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import boto3
 from aws_lambda_stream.utils.aws import get_region
 
 class Connector():
-    def __init__(self,topic_arn = os.getenv('TOPIC_ARN')) -> None:
+    def __init__(self,topic_arn = os.getenv('TOPIC_ARN'), client = None) -> None:
         self.topic_arn = topic_arn
-        self.client = boto3.client('sns',
+        self.client = client if client else boto3.client('sns',
                                    region_name=get_region(topic_arn))
 
     def publish(self, input_params):
         params = {
             'TopicArn': self.topic_arn,
             **input_params
         }
```

### Comparing `aws_lambda_stream-1.0.9/aws_lambda_stream/connectors/sqs.py` & `aws_lambda_stream-1.1.1/aws_lambda_stream/connectors/sqs.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import os
 import boto3
 
 
 class Connector():
-    def __init__(self,queue_url = os.getenv('QUEUE_URL')) -> None:
+
+    def __init__(self,queue_url = os.getenv('QUEUE_URL'), client = None) -> None:
         self.queue_url = queue_url
-        self.client = boto3.client('sqs')
+        self.client = client if client else boto3.client('sqs')
+
     def send_message(self, input_params):
         params = {
             'QueueUrl': self.queue_url,
             **input_params
         }
 
         self.client.send_message(**params)
+
     def send_message_batch(self, input_params):
         params = {
             'QueueUrl': self.queue_url,
             **input_params
         }
         self.client.send_message_batch(**params)
```

### Comparing `aws_lambda_stream-1.0.9/aws_lambda_stream/events/dynamodb.py` & `aws_lambda_stream-1.1.1/aws_lambda_stream/events/dynamodb.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import json
 from decimal import Decimal
 import pydash
+from pydash import get
 from aws_lambda_stream.utils.dynamodb import unmarshall,marshall
 
 
 def from_dynamodb(
     event,
     pk_fn = 'pk',
     sk_fn = 'sk',
@@ -45,14 +46,16 @@
                 lambda uow: {
                     **uow,
                     'event': {
                         **uow['event'],
                         'timestamp': _get_timestamp(uow)
                     },
                 }
+            ).sort_by(
+                lambda uow: pydash.get(uow, 'event.timestamp', 0)
             ).value()
 
 def _calculate_event_type_prefix(record, opt):
     if opt.get('event_type_prefix'):
         return opt['event_type_prefix']
     image = record.get('dynamodb').get('NewImage') or record.get('dynamodb').get('OldImage')
     discriminator = image.get(opt['discriminator_fn']) or image.get(opt['sk_fn'])
@@ -65,25 +68,28 @@
         'REMOVE': 'deleted'
     })[record['eventName']]
     if suffix != 'deleted':
         new_image = record.get('dynamodb').get('NewImage')
         old_image = record.get('dynamodb').get('OldImage')
         if ((new_image and new_image.get('deleted')) or
             (old_image and old_image.get('deleted'))):
-            if new_image and new_image.get('deleted'):
+            if new_image and get(new_image, 'deleted.BOOL'):
                 return 'deleted'
-            if old_image and old_image.get('deleted'):
+            if old_image and get(old_image, 'deleted.BOOL'):
                 return 'undeleted'
     return suffix
 
 
 def _get_timestamp(uow):
     _new = uow['event']['raw']['new']
-    if 'timestamp' in _new:
+    _old = uow['event']['raw']['old']
+    if _new and 'timestamp' in _new:
         return _new['timestamp']
+    if _old and 'timestamp' in _old:
+        return _old['timestamp']
     return int(uow['event']['timestamp'])
 
 def _out_replicas(record):
     image = pydash.get(record, 'dynamodb.NewImage') or \
         pydash.get(record, 'dynamodb.OldImage')
     if 'awsregion' in image:
         return image['awsregion']['S'] == os.getenv('REGION')
```

### Comparing `aws_lambda_stream-1.0.9/aws_lambda_stream/events/kinesis.py` & `aws_lambda_stream-1.1.1/aws_lambda_stream/events/kinesis.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,25 +16,29 @@
         lambda uow: {
             **uow,
             'event': {
                 'id': uow['record']['eventID'],
                 **json.loads(uow['event'])
             },
         }
+    ).sort_by(
+        lambda uow: pydash.get(uow, 'event.timestamp', 0)
     ).value()
 
 # test helper
 def to_kinesis_records(events):
     return {
         'Records': [
             {
                 'eventSource': 'aws:kinesis',
                 'eventID': f"shardId-000000000000:{i}",
                 'awsRegion': 'us-west-2',
                 'kinesis': {
                     'sequenceNumber': f"{i}",
-                    'data': base64.b64encode(json.dumps(e, cls=JSONEncoder).encode('utf-8'))
+                    'data': base64.b64encode(
+                        json.dumps(e, cls=JSONEncoder).encode('utf-8')
+                    ).decode('utf-8')
                 }
             }
             for i,e in enumerate(events)
         ]
     }
```

### Comparing `aws_lambda_stream-1.0.9/aws_lambda_stream/events/s3.py` & `aws_lambda_stream-1.1.1/aws_lambda_stream/events/s3.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     return {
         'Records': [
             {
                 # 'eventVersion': '2.1',
                 'eventSource': 'aws:s3',
                 'awsRegion': 'us-west-2',
                 # 'eventTime': '2019-09-03T19:37:27.192Z',
-                # 'eventName': 'ObjectCreated:Put',
+                'eventName': 'ObjectCreated:Put',
                 # 'userIdentity': {
                 #   'principalId': 'AWS:AIDAINPONIXQXHT3IKHL2',
                 # },
                 # 'requestParameters': {
                 #   'sourceIPAddress': '205.255.255.255',
                 # },
                 'responseElements': {
```

### Comparing `aws_lambda_stream-1.0.9/aws_lambda_stream/events/sns.py` & `aws_lambda_stream-1.1.1/aws_lambda_stream/events/sns.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_stream-1.0.9/aws_lambda_stream/events/sqs.py` & `aws_lambda_stream-1.1.1/aws_lambda_stream/events/sqs.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_stream-1.0.9/aws_lambda_stream/filters/event_type.py` & `aws_lambda_stream-1.1.1/aws_lambda_stream/filters/event_type.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_stream-1.0.9/aws_lambda_stream/filters/latch.py` & `aws_lambda_stream-1.1.1/aws_lambda_stream/filters/latch.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_stream-1.0.9/aws_lambda_stream/flavors/cdc.py` & `aws_lambda_stream-1.1.1/aws_lambda_stream/flavors/cdc.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,16 @@
         return source.pipe(
             rx_filter(out_latched),
             rx_filter(on_event_type(rule)),
             rx_filter(on_content(rule)),
             rx_map(_to_event(rule)),
             rule['publish'](pick(rule,[
                 'logger',
-                'max_batch_size',
-                'bus_name'
+                'bus_name',
+                'source'
             ])),
         )
     return wrapper
 
 def _to_event(rule):
     def wrapper(uow):
         # pylint: disable=unnecessary-lambda
```

### Comparing `aws_lambda_stream-1.0.9/aws_lambda_stream/flavors/collect.py` & `aws_lambda_stream-1.1.1/aws_lambda_stream/flavors/collect.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_stream-1.0.9/aws_lambda_stream/flavors/correlate.py` & `aws_lambda_stream-1.1.1/aws_lambda_stream/flavors/correlate.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_stream-1.0.9/aws_lambda_stream/flavors/evaluate.py` & `aws_lambda_stream-1.1.1/aws_lambda_stream/flavors/evaluate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from functools import reduce
 from reactivex import Observable
-from pydash import get, pick, omit, merge
+from pydash import get, pick, omit, merge, sort_by
 from aws_lambda_stream.utils.faults import faulty
 from aws_lambda_stream.utils.filters import on_event_type, on_content
 from aws_lambda_stream.utils.dynamodb import query_dynamodb
 from aws_lambda_stream.utils.operators import rx_filter, rx_map, split_buffer
 
 
 def evaluate(rule):
@@ -32,18 +32,17 @@
             rx_filter(on_content(rule)),
             _complex(rule),
             rx_map(_to_higher_order_events(rule)),
             split_buffer(),
             rule['publish']({
                     **pick(rule,[
                         'logger',
-                        'max_batch_size',
-                        'bus_name'
+                        'bus_name',
+                        'source'
                     ]),
-                    'max_batch_size': 1,
                     'event_field': 'emit'
                 }),
         )
     return wrapper
 
 
 def _for_events(uow):
@@ -93,15 +92,19 @@
                     'table_name',
                     'query_request_field',
                     'query_response_field'
                 ])
             ),
             rx_map(lambda uow: {
                 **uow,
-                'correlated': [i['event'] for i in uow['correlated']]
+                'correlated': sort_by(
+                    [i['event'] for i in uow['correlated']],
+                    'timestamp',
+                    reverse=True
+                )
             }),
             rx_map(_expression(rule)),
             rx_filter(lambda uow: uow['expression'])
         )
     return wrapper
```

### Comparing `aws_lambda_stream-1.0.9/aws_lambda_stream/flavors/materialize.py` & `aws_lambda_stream-1.1.1/aws_lambda_stream/flavors/materialize.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_stream-1.0.9/aws_lambda_stream/flavors/s3.py` & `aws_lambda_stream-1.1.1/aws_lambda_stream/flavors/s3.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_stream-1.0.9/aws_lambda_stream/flavors/sns.py` & `aws_lambda_stream-1.1.1/aws_lambda_stream/flavors/sns.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_stream-1.0.9/aws_lambda_stream/flavors/task.py` & `aws_lambda_stream-1.1.1/aws_lambda_stream/flavors/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         'id': str
         'flavor': task,
         'event_type': str | List[str] | Callable,
         'execute': Callable # execute task
         'emit': Optional[str | Callable]
     }
     """
-        
+
     def wrapper(source: Observable):
         return source.pipe(
             rx_filter(on_event_type(rule)),
             rx_filter(on_content(rule)),
             _execute(rule),
             _execute_operators(rule),
             _to_event(rule),
@@ -35,15 +35,15 @@
     def _call(uow):
         result_key = rule.get('result_key', 'result')
         return set_(
             uow,
             result_key,
             rule['execute'](uow, rule)
         )
-        
+
     def wrapper(source: Observable):
         execute = get(rule, 'execute')
         if execute:
             return source.pipe(
                 rx_map(faulty(_call)),
             )
         return source.pipe()
@@ -66,17 +66,17 @@
         if get(rule, 'emit'):
             return source.pipe(
                 rx_map(_to_emit(rule)),
                 split_buffer(),
                 rule['publish']({
                         **pick(rule,[
                             'logger',
-                            'bus_name'
+                            'bus_name',
+                            'source'
                         ]),
-                        'max_batch_size': 1,
                         'event_field': 'emit'
                 }),
             )
         return source.pipe()
     return wrapper
```

### Comparing `aws_lambda_stream-1.0.9/aws_lambda_stream/pipelines/__init__.py` & `aws_lambda_stream-1.1.1/aws_lambda_stream/pipelines/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,16 +44,15 @@
                     **uow,
                 }),
                 self.the_pipelines[k](
                     {
                         'id': k,
                         'pipeline': copy.copy(k),
                         **self.opt,
-                        'logger': Logger(k),
-                        'max_batch_size': len(iterable) if len(iterable) > 0 else 10
+                        'logger': Logger(k)
                     }
                 )
             )
             p.id = k
             return p
 
         lines = list(map(make_lines, self.the_pipelines.keys()))
```

### Comparing `aws_lambda_stream-1.0.9/aws_lambda_stream/repositories/__init__.py` & `aws_lambda_stream-1.1.1/aws_lambda_stream/repositories/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,14 +58,17 @@
                     'ttl': ttl(timestamp, 33),
                     'awsregion': os.getenv('REGION'),
                     'timestamp': timestamp,
                 },
             ),
         }
         self.connector.update(params)
+    def delete_bulk(self, pks: list, sk = None, data = None):
+        for pk in pks:
+            self.delete(pk, sk, data)
     def query(self, input_params):
         return self.connector.query(input_params)
     def get_item(self, params):
         result = self.query(params)
         if result['Count'] == 0:
             return None
         return result['Items'][0]
```

### Comparing `aws_lambda_stream-1.0.9/aws_lambda_stream/utils/dynamodb.py` & `aws_lambda_stream-1.1.1/aws_lambda_stream/utils/dynamodb.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import boto3
 from boto3.dynamodb.types import TypeDeserializer, TypeSerializer
 from reactivex import Observable
 from aws_lambda_stream.connectors.dynamodb import Connector
 from aws_lambda_stream.utils.faults import faulty
 from aws_lambda_stream.utils.operators import rx_map
 from aws_lambda_stream.utils.json_encoder import JSONEncoder
+from aws_lambda_stream.utils.retry import DEFAULT_RETRY_CONFIG
 
 
 def serialize_number(number: str) -> Union[float, int]:
     if '.' in number:
         return float(number)
     return int(number)
 
@@ -125,14 +126,39 @@
                     parse_float=Decimal
                 )
             )
         }
     return faulty(wrapper)
 
 
+def batch_get_dynamodb( # pylint: disable=W0102
+    table_name= os.getenv('EVENT_TABLE_NAME') or os.getenv('ENTITY_TABLE_NAME'),
+    batch_get_request_field='batch_get_request',
+    batch_get_response_field='batch_get_response',
+    retry_config=DEFAULT_RETRY_CONFIG
+    ):
+    connector = Connector(table_name, retry_config)
+
+    def invoke(uow):
+        if not batch_get_request_field in uow:
+            return uow
+        return {
+            **uow,
+            batch_get_response_field: connector.batch_get(
+                uow[batch_get_request_field]
+            )
+        }
+
+    def wrapper(source: Observable):
+        return source.pipe(
+            rx_map(faulty(invoke)),
+        )
+    return wrapper
+
+
 def query_dynamodb(
         table_name= os.getenv('EVENT_TABLE_NAME') or os.getenv('ENTITY_TABLE_NAME'),
         query_request_field = 'query_request',
         query_response_field = 'query_response'
     ):
     connector = Connector(table_name)
```

### Comparing `aws_lambda_stream-1.0.9/aws_lambda_stream/utils/elasticsearch.py` & `aws_lambda_stream-1.1.1/aws_lambda_stream/utils/elasticsearch.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import os
 import json
+from pydash import get, pick
 from reactivex import Observable, operators as ops
 from aws_lambda_stream.connectors.elasticsearch import Connector
 from aws_lambda_stream.utils.json_encoder import JSONEncoder
 from aws_lambda_stream.utils.operators import split_buffer, rx_map
 from aws_lambda_stream.utils.faults import faulty
 from .batch import to_batch_uow, unbatch_uow
 
 
 def update_elasticsearch(
     connector: Connector,
     update_field='update_request',
-    batch_size=os.getenv('PUBLISH_BATCH_SIZE') or os.getenv('BATCH_SIZE') or 10,
-    max_batch_size=os.getenv('PUBLISH_BATCH_SIZE') or os.getenv('BATCH_SIZE') or 10,
+    batch_size=os.getenv('PUBLISH_BATCH_SIZE') or os.getenv('BATCH_SIZE') or 10
 ):
     def to_input_params(batch_uow):
         return {
             **batch_uow,
             'input_params': "\n".join(list(map(
                     lambda uow: "{}\n{}".format(
                         json.dumps({
@@ -36,15 +36,45 @@
     def put_items(batch_uow):
         return {
             **batch_uow,
             'elasticsearch_response': connector.bulk(batch_uow['input_params'])
         }
     def wrapper(source: Observable):
         return source.pipe(
-            ops.buffer_with_count(max_batch_size if batch_size > max_batch_size else batch_size),
+            ops.buffer_with_count(batch_size, batch_size),
             rx_map(to_batch_uow),
             rx_map(to_input_params),
             rx_map(faulty(put_items)),
             rx_map(unbatch_uow),
             split_buffer()
         )
     return wrapper
+
+
+def query_elasticsearch(
+    host = os.getenv('ES_DOMAIN_HOST'),
+    region = os.getenv('REGION'),
+    query_request_field = 'query_request',
+    query_response_field = 'query_response'
+    ):
+
+    connector = Connector(host, region)
+
+    def search(uow):
+        if not uow.get(query_request_field):
+            return uow
+
+        return {
+            **uow,
+            query_response_field: connector.search(
+                **pick(
+                    get(uow, query_request_field),
+                    'index', 'payload' ,'query'
+                )
+            )
+        }
+
+    def wrapper(source: Observable):
+        return source.pipe(
+            rx_map(faulty(search)),
+        )
+    return wrapper
```

### Comparing `aws_lambda_stream-1.0.9/aws_lambda_stream/utils/faults.py` & `aws_lambda_stream-1.1.1/aws_lambda_stream/utils/faults.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 
 def format_fault(err: Exception):
     return {
         'id': str(uuid1()),
         'partition_key': str(uuid4()),
         'type': FAULT_EVENT_TYPE,
         'timestamp': now(),
-        'pipeline': err.uow.get('pipeline') or 'undefined',
         'tags':{
             'functionname': os.getenv('AWS_LAMBDA_FUNCTION_NAME'),
             'pipeline': err.uow.get('pipeline') or 'undefined'
         },
         'err': {
             'name': type(err).__name__,
             'message': str(err),
@@ -58,15 +57,14 @@
         while len(the_faults) > 0:
             observer.on_next(the_faults.pop(0))
         observer.on_completed()
     create(push_errors).pipe(
         ops.map(lambda fault: {'event': fault}),
         rule['publish'](pick(rule,[
             'logger',
-            'max_batch_size',
             'bus_name'
         ])),
     ).subscribe()
 
 
 def _trim_and_redact(_uow):
     # pylint: disable=unused-argument,inconsistent-return-statements
```

### Comparing `aws_lambda_stream-1.0.9/aws_lambda_stream/utils/lambda_.py` & `aws_lambda_stream-1.1.1/aws_lambda_stream/utils/lambda_.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_stream-1.0.9/aws_lambda_stream/utils/logger.py` & `aws_lambda_stream-1.1.1/aws_lambda_stream/utils/logger.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_stream-1.0.9/aws_lambda_stream/utils/operators.py` & `aws_lambda_stream-1.1.1/aws_lambda_stream/utils/operators.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_stream-1.0.9/aws_lambda_stream/utils/sns.py` & `aws_lambda_stream-1.1.1/aws_lambda_stream/utils/sns.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from uuid import uuid1
-from reactivex import Observable, operators as ops
+from reactivex import Observable
 from pydash import map_
 from aws_lambda_stream.connectors.sns import Connector
+from aws_lambda_stream import rx_map, faulty
 
 def publish_to_sns(
     connector: Connector,
-    publish_message_field='sns_payload'
+    publish_message_field='sns_payload',
 ):
     def to_input_params(uow):
         return {
             **uow,
             'input_params': {
                 'PublishBatchRequestEntries': map_(
                     uow[publish_message_field],
@@ -21,11 +22,11 @@
             }
         }
     def publish_batch(uow):
         uow['publish_response'] = connector.publish_batch(uow['input_params'])
         return uow
     def _wrapper(source: Observable):
         return source.pipe(
-            ops.map(to_input_params),
-            ops.map(publish_batch)
+            rx_map(faulty(to_input_params)),
+            rx_map(faulty(publish_batch))
         )
     return _wrapper
```

### Comparing `aws_lambda_stream-1.0.9/aws_lambda_stream/utils/split.py` & `aws_lambda_stream-1.1.1/aws_lambda_stream/utils/split.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_stream-1.0.9/aws_lambda_stream/utils/tags.py` & `aws_lambda_stream-1.1.1/aws_lambda_stream/utils/tags.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 import os
 from aws_lambda_stream.filters.skip import skip_tag
 
 
 def adorn_standard_tags(event_field):
     def wrapper(uow: dict):
-        return uow if not event_field in uow else {
+        return uow if not uow.get(event_field) else {
             **uow,
             event_field: {
                 **uow[event_field],
                 'tags': {
                     **env_tags(uow.get('pipeline', None)),
                     **skip_tag(),
-                    **(uow.get('event_field', {}).get('tags', {}))
+                    **(uow.get(event_field, {}).get('tags', {}))
                 }
             }
         }
     return wrapper
 
 
 def env_tags(pipeline):
     return {
         'account': os.getenv('ACCOUNT_NAME', 'undefined'),
         'region': os.getenv('AWS_REGION', 'undefined'),
         'stage': os.getenv('STAGE', 'undefined'),
+        'app': os.getenv('APP_NAME', 'undefined'),
         'source': (
             os.getenv('SERVICE') or
             os.getenv('PROJECT') or
             os.getenv('SERVERLESS_PROJECT') or 'undefined'),
         'functionname': os.getenv('AWS_LAMBDA_FUNCTION_NAME', 'undefined'),
         'pipeline': pipeline or 'undefined'
     }
```

### Comparing `aws_lambda_stream-1.0.9/pyproject.toml` & `aws_lambda_stream-1.1.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 [tool.poetry]
 name = "aws_lambda_stream"
-version = "1.0.9"
+version = "1.1.1"
 description = "Create stream processors with AWS Lambda functions"
 authors = ["Alejandro Hernández <clandro89@gmail.com>"]
 repository="https://github.com/clandro89/aws-lambda-stream"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 reactivex = "^4.0.4"
 boto3 = "^1.24.66"
-aws-lambda-powertools = "^1.29.1"
+aws-lambda-powertools = "1.29.1"
 pydash = "^5.1.1"
 requests-aws4auth = "^1.1.2"
 
 [tool.poetry.dev-dependencies]
 pylint= "~=2.7.4"
 pytest = "^7.1.2"
 expects = "^0.9.0"
 
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.pytest.ini_options]
+addopts = "--ignore=templates"
```

