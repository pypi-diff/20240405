# Comparing `tmp/s3-credentials-0.8.tar.gz` & `tmp/s3-credentials-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s3-credentials-0.8.tar", last modified: Tue Dec  7 07:01:07 2021, max compression
+gzip compressed data, was "s3-credentials-0.9.tar", last modified: Tue Jan 18 02:12:35 2022, max compression
```

## Comparing `s3-credentials-0.8.tar` & `s3-credentials-0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 07:01:07.685294 s3-credentials-0.8/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2021-12-07 07:00:52.000000 s3-credentials-0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    21920 2021-12-07 07:01:07.685294 s3-credentials-0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    21350 2021-12-07 07:00:52.000000 s3-credentials-0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 07:01:07.685294 s3-credentials-0.8/s3_credentials/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-07 07:00:52.000000 s3-credentials-0.8/s3_credentials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    26605 2021-12-07 07:00:52.000000 s3-credentials-0.8/s3_credentials/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     1921 2021-12-07 07:00:52.000000 s3-credentials-0.8/s3_credentials/policies.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 07:01:07.685294 s3-credentials-0.8/s3_credentials.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    21920 2021-12-07 07:01:07.000000 s3-credentials-0.8/s3_credentials.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      332 2021-12-07 07:01:07.000000 s3-credentials-0.8/s3_credentials.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-07 07:01:07.000000 s3-credentials-0.8/s3_credentials.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       77 2021-12-07 07:01:07.000000 s3-credentials-0.8/s3_credentials.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       46 2021-12-07 07:01:07.000000 s3-credentials-0.8/s3_credentials.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2021-12-07 07:01:07.000000 s3-credentials-0.8/s3_credentials.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-12-07 07:01:07.685294 s3-credentials-0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1104 2021-12-07 07:00:52.000000 s3-credentials-0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-18 02:12:35.036553 s3-credentials-0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-01-18 02:12:18.000000 s3-credentials-0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)    25460 2022-01-18 02:12:35.036553 s3-credentials-0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    24890 2022-01-18 02:12:18.000000 s3-credentials-0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-18 02:12:35.032553 s3-credentials-0.9/s3_credentials/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-18 02:12:18.000000 s3-credentials-0.9/s3_credentials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28981 2022-01-18 02:12:18.000000 s3-credentials-0.9/s3_credentials/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3090 2022-01-18 02:12:18.000000 s3-credentials-0.9/s3_credentials/policies.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-18 02:12:35.036553 s3-credentials-0.9/s3_credentials.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    25460 2022-01-18 02:12:35.000000 s3-credentials-0.9/s3_credentials.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      332 2022-01-18 02:12:35.000000 s3-credentials-0.9/s3_credentials.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-18 02:12:35.000000 s3-credentials-0.9/s3_credentials.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       77 2022-01-18 02:12:35.000000 s3-credentials-0.9/s3_credentials.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       46 2022-01-18 02:12:35.000000 s3-credentials-0.9/s3_credentials.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2022-01-18 02:12:35.000000 s3-credentials-0.9/s3_credentials.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-18 02:12:35.036553 s3-credentials-0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-01-18 02:12:18.000000 s3-credentials-0.9/setup.py
```

### Comparing `s3-credentials-0.8/LICENSE` & `s3-credentials-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `s3-credentials-0.8/PKG-INFO` & `s3-credentials-0.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s3-credentials
-Version: 0.8
+Version: 0.9
 Summary: A tool for creating credentials for accessing S3 buckets
 Home-page: https://github.com/simonw/s3-credentials
 Author: Simon Willison
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/simonw/s3-credentials/issues
 Project-URL: CI, https://github.com/simonw/s3-credentials/actions
 Project-URL: Changelog, https://github.com/simonw/s3-credentials/releases
@@ -21,20 +21,14 @@
 [![Tests](https://github.com/simonw/s3-credentials/workflows/Test/badge.svg)](https://github.com/simonw/s3-credentials/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/simonw/s3-credentials/blob/master/LICENSE)
 
 A tool for creating credentials for accessing S3 buckets
 
 For project background, see [s3-credentials: a tool for creating credentials for S3 buckets](https://simonwillison.net/2021/Nov/3/s3-credentials/) on my blog.
 
-## ⚠️ Warning
-
-I am not an AWS security expert. You shoud review how this tool works carefully before using it against with own AWS account.
-
-If you are an AWS security expert I would [love to get your feedback](https://github.com/simonw/s3-credentials/issues/7)!
-
 ## Installation
 
 Install this tool using `pip`:
 
     $ pip install s3-credentials
 
 ## Configuration
@@ -102,14 +96,15 @@
 
 The `create` command has a number of options:
 
 - `--format TEXT`: The output format to use. Defaults to `json`, but can also be `ini`.
 - `--duration 15m`: For temporary credentials, how long should they last? This can be specified in seconds, minutes or hours using a suffix of `s`, `m` or `h` - but must be between 15 minutes and 12 hours.
 - `--username TEXT`: The username to use for the user that is created by the command (or the username of an existing user if you do not want to create a new one). If ommitted a default such as `s3.read-write.static.niche-museums.com` will be used.
 - `-c, --create-bucket`: Create the buckets if they do not exist. Without this any missing buckets will be treated as an error.
+- `--prefix my-prefix/`: Credentials should only allow access to keys in the S3 bucket that start with this prefix.
 - `--public`: When creating a bucket, set it so that any file uploaded to that bucket can be downloaded by anyone who knows its filename. This attaches the [public bucket policy](#public-bucket-policy) shown below.
 - `--read-only`: The user should only be allowed to read files from the bucket.
 - `--write-only`: The user should only be allowed to write files to the bucket, but not read them. This can be useful for logging and backups.
 - `--policy filepath-or-string`: A custom policy document (as a file path, literal JSON string or `-` for standard input) - see below.
 - `--bucket-region`: If creating buckets, the region in which they should be created.
 - `--silent`: Don't output details of what is happening, just output the JSON for the created access credentials at the end.
 - `--dry-run`: Output details of AWS changes that would have been made without applying them.
@@ -119,15 +114,15 @@
 
 How the tool works varies depending on if you are creating temporary or permanent credentials.
 
 For permanent credentials, the steps are as follows:
 
 1. Confirm that each of the specified buckets exists. If they do not and `--create-bucket` was passed create them - otherwise exit with an error.
 2. If a username was not specified, derive a username using the `s3.$permission.$buckets` format.
-3. If a user with that username does not exist, create one with an S3 permissions boundary that respects the `--read-only` option - unless `--user-permissions-boundary=none` was passed (or a custom permissions boundary string).
+3. If a user with that username does not exist, create one with an S3 permissions boundary of [AmazonS3ReadOnlyAccess](https://github.com/glassechidna/trackiam/blob/master/policies/AmazonS3ReadOnlyAccess.json) for `--read-only` or [AmazonS3FullAccess](https://github.com/glassechidna/trackiam/blob/master/policies/AmazonS3FullAccess.json) otherwise - unless `--user-permissions-boundary=none` was passed, or a custom permissions boundary string.
 4. For each specified bucket, add an inline IAM policy to the user that gives them permission to either read-only, write-only or read-write against that bucket.
 5. Create a new access key for that user and output the key and its secret to the console.
 
 For temporary credentials:
 
 1. Confirm or create buckets, in the same way as for permanent credentials.
 2. Check if an AWS role called `s3-credentials.AmazonS3FullAccess` exists. If it does not exist create it, configured to allow the user's AWS account to assume it and with the `arn:aws:iam::aws:policy/AmazonS3FullAccess` policy attached.
@@ -184,14 +179,15 @@
 
 ### policy
 
 You can use the `s3-credentials policy` command to generate the JSON policy document that would be used without applying it. The command takes one or more required bucket names and a subset of the options available on the `create` command:
 
 - `--read-only` - generate a read-only policy
 - `--write-only` - generate a write-only policy
+- `--prefix` - policy should be restricted to keys in the bucket that start with this prefix
 - `--public-bucket` - generate a bucket policy for a public bucket
 
 With none of these options it defaults to a read-write policy.
 ```
 % s3-credentials policy my-bucket --read-only
 {
     "Version": "2012-10-17",
@@ -218,19 +214,19 @@
 ```
 ### list-users
 
 To see a list of all users that exist for your AWS account:
 
     s3-credentials list-users
 
-This will return pretty-printed JSON objects by default.
+This will a pretty-printed array of JSON objects by default.
 
 Add `--nl` to collapse these to single lines as valid newline-delimited JSON.
 
-Add `--array` to output a valid JSON array of objects instead.
+Add `--csv` or `--tsv` to get back CSV or TSV data.
 
 ### list-buckets
 
 Shows a list of all buckets in your AWS account.
 
     % s3-credentials list-buckets
     {
@@ -246,15 +242,15 @@
 
     % s3-credentials list-buckets simonw-test-bucket-for-s3-credentials
     {
         "Name": "simonw-test-bucket-for-s3-credentials",
         "CreationDate": "2021-11-03 21:46:12+00:00"
     }
 
-This accepts the same `--nl` and `--array` options as `list-users`.
+This accepts the same `--nl`, `--csv` and `--tsv` options as `list-users`.
 
 Add `--details` to include details of the bucket ACL, website configuration and public access block settings. This is useful for running a security audit of your buckets.
 
 Using `--details` adds three additional API calls for each bucket, so it is advisable to use it with one or more explicit bucket names.
 ```
 % s3-credentials list-buckets simonw-test-public-website-bucket --details
 {
@@ -314,14 +310,39 @@
     "BlockPublicPolicy": true,
     "RestrictPublicBuckets": true
   },
   "bucket_website": null
 }
 ```
 
+### list-bucket
+
+To list the contents of a bucket, use `list-bucket`:
+
+```
+% s3-credentials list-bucket static.niche-museums.com
+[
+  {
+    "Key": "Griffith-Observatory.jpg",
+    "LastModified": "2020-01-05 16:51:01+00:00",
+    "ETag": "\"a4cff17d189e7eb0c4d3bf0257e56885\"",
+    "Size": 3360040,
+    "StorageClass": "STANDARD"
+  },
+  {
+    "Key": "IMG_0353.jpeg",
+    "LastModified": "2019-10-25 02:50:49+00:00",
+    "ETag": "\"d45bab0b65c0e4b03b2ac0359c7267e3\"",
+    "Size": 2581023,
+    "StorageClass": "STANDARD"
+  }
+]
+```
+This accepts the same `--nl`, `--csv` and `--tsv` options as `list-users`.
+
 ### list-user-policies
 
 To see a list of inline policies belonging to users:
 
 ```
 % s3-credentials list-user-policies s3.read-write.static.niche-museums.com
 
@@ -560,14 +581,160 @@
       ]
     }
   ]
 }
 ```
 <!-- [[[end]]] -->
 
+### --prefix my-prefix/
+
+<!-- [[[cog
+result = runner.invoke(cli.cli, ["policy", "my-s3-bucket", "--prefix", "my-prefix/"])
+cog.out(
+    "```\n{}\n```".format(json.dumps(json.loads(result.output), indent=2))
+)
+]]] -->
+```
+{
+  "Version": "2012-10-17",
+  "Statement": [
+    {
+      "Effect": "Allow",
+      "Action": [
+        "s3:GetBucketLocation"
+      ],
+      "Resource": [
+        "arn:aws:s3:::my-s3-bucket"
+      ]
+    },
+    {
+      "Effect": "Allow",
+      "Action": [
+        "s3:ListBucket"
+      ],
+      "Resource": [
+        "arn:aws:s3:::my-s3-bucket"
+      ],
+      "Condition": {
+        "StringLike": {
+          "s3:prefix": [
+            "my-prefix/*"
+          ]
+        }
+      }
+    },
+    {
+      "Effect": "Allow",
+      "Action": [
+        "s3:GetObject",
+        "s3:GetObjectAcl",
+        "s3:GetObjectLegalHold",
+        "s3:GetObjectRetention",
+        "s3:GetObjectTagging"
+      ],
+      "Resource": [
+        "arn:aws:s3:::my-s3-bucket/my-prefix/*"
+      ]
+    },
+    {
+      "Effect": "Allow",
+      "Action": [
+        "s3:PutObject",
+        "s3:DeleteObject"
+      ],
+      "Resource": [
+        "arn:aws:s3:::my-s3-bucket/my-prefix/*"
+      ]
+    }
+  ]
+}
+```
+<!-- [[[end]]] -->
+
+### --prefix my-prefix/ --read-only
+
+<!-- [[[cog
+result = runner.invoke(cli.cli, ["policy", "my-s3-bucket", "--prefix", "my-prefix/", "--read-only"])
+cog.out(
+    "```\n{}\n```".format(json.dumps(json.loads(result.output), indent=2))
+)
+]]] -->
+```
+{
+  "Version": "2012-10-17",
+  "Statement": [
+    {
+      "Effect": "Allow",
+      "Action": [
+        "s3:GetBucketLocation"
+      ],
+      "Resource": [
+        "arn:aws:s3:::my-s3-bucket"
+      ]
+    },
+    {
+      "Effect": "Allow",
+      "Action": [
+        "s3:ListBucket"
+      ],
+      "Resource": [
+        "arn:aws:s3:::my-s3-bucket"
+      ],
+      "Condition": {
+        "StringLike": {
+          "s3:prefix": [
+            "my-prefix/*"
+          ]
+        }
+      }
+    },
+    {
+      "Effect": "Allow",
+      "Action": [
+        "s3:GetObject",
+        "s3:GetObjectAcl",
+        "s3:GetObjectLegalHold",
+        "s3:GetObjectRetention",
+        "s3:GetObjectTagging"
+      ],
+      "Resource": [
+        "arn:aws:s3:::my-s3-bucket/my-prefix/*"
+      ]
+    }
+  ]
+}
+```
+<!-- [[[end]]] -->
+
+### --prefix my-prefix/ --write-only
+
+<!-- [[[cog
+result = runner.invoke(cli.cli, ["policy", "my-s3-bucket", "--prefix", "my-prefix/", "--write-only"])
+cog.out(
+    "```\n{}\n```".format(json.dumps(json.loads(result.output), indent=2))
+)
+]]] -->
+```
+{
+  "Version": "2012-10-17",
+  "Statement": [
+    {
+      "Effect": "Allow",
+      "Action": [
+        "s3:PutObject"
+      ],
+      "Resource": [
+        "arn:aws:s3:::my-s3-bucket/my-prefix/*"
+      ]
+    }
+  ]
+}
+```
+<!-- [[[end]]] -->
+
 ### public bucket policy
 
 Buckets created using the `--public` option will have the following bucket policy attached to them:
 
 <!-- [[[cog
 result = runner.invoke(cli.cli, ["policy", "my-s3-bucket", "--public-bucket"])
 cog.out(
@@ -620,14 +787,14 @@
 
 ### Integration tests
 
 The main tests all use stubbed interfaces to AWS, so will not make any outbound API calls.
 
 There is also a suite of integration tests in `tests/test_integration.py` which DO make API calls to AWS, using credentials from your environment variables or `~/.aws/credentials` file.
 
-These tests are skipped by default. If you have AWS configured with an account that has permission to run `s3-credentials` (create users, roles, buckets etc) you can run these tests using:
+These tests are skipped by default. If you have AWS configured with an account that has permission to run the actions required by `s3-credentials` (create users, roles, buckets etc) you can run these tests using:
 
     pytest --integration
 
 The tests will create a number of different users and buckets and should then delete them once they finish running.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `s3-credentials-0.8/README.md` & `s3-credentials-0.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -5,20 +5,14 @@
 [![Tests](https://github.com/simonw/s3-credentials/workflows/Test/badge.svg)](https://github.com/simonw/s3-credentials/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/simonw/s3-credentials/blob/master/LICENSE)
 
 A tool for creating credentials for accessing S3 buckets
 
 For project background, see [s3-credentials: a tool for creating credentials for S3 buckets](https://simonwillison.net/2021/Nov/3/s3-credentials/) on my blog.
 
-## ⚠️ Warning
-
-I am not an AWS security expert. You shoud review how this tool works carefully before using it against with own AWS account.
-
-If you are an AWS security expert I would [love to get your feedback](https://github.com/simonw/s3-credentials/issues/7)!
-
 ## Installation
 
 Install this tool using `pip`:
 
     $ pip install s3-credentials
 
 ## Configuration
@@ -86,14 +80,15 @@
 
 The `create` command has a number of options:
 
 - `--format TEXT`: The output format to use. Defaults to `json`, but can also be `ini`.
 - `--duration 15m`: For temporary credentials, how long should they last? This can be specified in seconds, minutes or hours using a suffix of `s`, `m` or `h` - but must be between 15 minutes and 12 hours.
 - `--username TEXT`: The username to use for the user that is created by the command (or the username of an existing user if you do not want to create a new one). If ommitted a default such as `s3.read-write.static.niche-museums.com` will be used.
 - `-c, --create-bucket`: Create the buckets if they do not exist. Without this any missing buckets will be treated as an error.
+- `--prefix my-prefix/`: Credentials should only allow access to keys in the S3 bucket that start with this prefix.
 - `--public`: When creating a bucket, set it so that any file uploaded to that bucket can be downloaded by anyone who knows its filename. This attaches the [public bucket policy](#public-bucket-policy) shown below.
 - `--read-only`: The user should only be allowed to read files from the bucket.
 - `--write-only`: The user should only be allowed to write files to the bucket, but not read them. This can be useful for logging and backups.
 - `--policy filepath-or-string`: A custom policy document (as a file path, literal JSON string or `-` for standard input) - see below.
 - `--bucket-region`: If creating buckets, the region in which they should be created.
 - `--silent`: Don't output details of what is happening, just output the JSON for the created access credentials at the end.
 - `--dry-run`: Output details of AWS changes that would have been made without applying them.
@@ -103,15 +98,15 @@
 
 How the tool works varies depending on if you are creating temporary or permanent credentials.
 
 For permanent credentials, the steps are as follows:
 
 1. Confirm that each of the specified buckets exists. If they do not and `--create-bucket` was passed create them - otherwise exit with an error.
 2. If a username was not specified, derive a username using the `s3.$permission.$buckets` format.
-3. If a user with that username does not exist, create one with an S3 permissions boundary that respects the `--read-only` option - unless `--user-permissions-boundary=none` was passed (or a custom permissions boundary string).
+3. If a user with that username does not exist, create one with an S3 permissions boundary of [AmazonS3ReadOnlyAccess](https://github.com/glassechidna/trackiam/blob/master/policies/AmazonS3ReadOnlyAccess.json) for `--read-only` or [AmazonS3FullAccess](https://github.com/glassechidna/trackiam/blob/master/policies/AmazonS3FullAccess.json) otherwise - unless `--user-permissions-boundary=none` was passed, or a custom permissions boundary string.
 4. For each specified bucket, add an inline IAM policy to the user that gives them permission to either read-only, write-only or read-write against that bucket.
 5. Create a new access key for that user and output the key and its secret to the console.
 
 For temporary credentials:
 
 1. Confirm or create buckets, in the same way as for permanent credentials.
 2. Check if an AWS role called `s3-credentials.AmazonS3FullAccess` exists. If it does not exist create it, configured to allow the user's AWS account to assume it and with the `arn:aws:iam::aws:policy/AmazonS3FullAccess` policy attached.
@@ -168,14 +163,15 @@
 
 ### policy
 
 You can use the `s3-credentials policy` command to generate the JSON policy document that would be used without applying it. The command takes one or more required bucket names and a subset of the options available on the `create` command:
 
 - `--read-only` - generate a read-only policy
 - `--write-only` - generate a write-only policy
+- `--prefix` - policy should be restricted to keys in the bucket that start with this prefix
 - `--public-bucket` - generate a bucket policy for a public bucket
 
 With none of these options it defaults to a read-write policy.
 ```
 % s3-credentials policy my-bucket --read-only
 {
     "Version": "2012-10-17",
@@ -202,19 +198,19 @@
 ```
 ### list-users
 
 To see a list of all users that exist for your AWS account:
 
     s3-credentials list-users
 
-This will return pretty-printed JSON objects by default.
+This will a pretty-printed array of JSON objects by default.
 
 Add `--nl` to collapse these to single lines as valid newline-delimited JSON.
 
-Add `--array` to output a valid JSON array of objects instead.
+Add `--csv` or `--tsv` to get back CSV or TSV data.
 
 ### list-buckets
 
 Shows a list of all buckets in your AWS account.
 
     % s3-credentials list-buckets
     {
@@ -230,15 +226,15 @@
 
     % s3-credentials list-buckets simonw-test-bucket-for-s3-credentials
     {
         "Name": "simonw-test-bucket-for-s3-credentials",
         "CreationDate": "2021-11-03 21:46:12+00:00"
     }
 
-This accepts the same `--nl` and `--array` options as `list-users`.
+This accepts the same `--nl`, `--csv` and `--tsv` options as `list-users`.
 
 Add `--details` to include details of the bucket ACL, website configuration and public access block settings. This is useful for running a security audit of your buckets.
 
 Using `--details` adds three additional API calls for each bucket, so it is advisable to use it with one or more explicit bucket names.
 ```
 % s3-credentials list-buckets simonw-test-public-website-bucket --details
 {
@@ -298,14 +294,39 @@
     "BlockPublicPolicy": true,
     "RestrictPublicBuckets": true
   },
   "bucket_website": null
 }
 ```
 
+### list-bucket
+
+To list the contents of a bucket, use `list-bucket`:
+
+```
+% s3-credentials list-bucket static.niche-museums.com
+[
+  {
+    "Key": "Griffith-Observatory.jpg",
+    "LastModified": "2020-01-05 16:51:01+00:00",
+    "ETag": "\"a4cff17d189e7eb0c4d3bf0257e56885\"",
+    "Size": 3360040,
+    "StorageClass": "STANDARD"
+  },
+  {
+    "Key": "IMG_0353.jpeg",
+    "LastModified": "2019-10-25 02:50:49+00:00",
+    "ETag": "\"d45bab0b65c0e4b03b2ac0359c7267e3\"",
+    "Size": 2581023,
+    "StorageClass": "STANDARD"
+  }
+]
+```
+This accepts the same `--nl`, `--csv` and `--tsv` options as `list-users`.
+
 ### list-user-policies
 
 To see a list of inline policies belonging to users:
 
 ```
 % s3-credentials list-user-policies s3.read-write.static.niche-museums.com
 
@@ -544,14 +565,160 @@
       ]
     }
   ]
 }
 ```
 <!-- [[[end]]] -->
 
+### --prefix my-prefix/
+
+<!-- [[[cog
+result = runner.invoke(cli.cli, ["policy", "my-s3-bucket", "--prefix", "my-prefix/"])
+cog.out(
+    "```\n{}\n```".format(json.dumps(json.loads(result.output), indent=2))
+)
+]]] -->
+```
+{
+  "Version": "2012-10-17",
+  "Statement": [
+    {
+      "Effect": "Allow",
+      "Action": [
+        "s3:GetBucketLocation"
+      ],
+      "Resource": [
+        "arn:aws:s3:::my-s3-bucket"
+      ]
+    },
+    {
+      "Effect": "Allow",
+      "Action": [
+        "s3:ListBucket"
+      ],
+      "Resource": [
+        "arn:aws:s3:::my-s3-bucket"
+      ],
+      "Condition": {
+        "StringLike": {
+          "s3:prefix": [
+            "my-prefix/*"
+          ]
+        }
+      }
+    },
+    {
+      "Effect": "Allow",
+      "Action": [
+        "s3:GetObject",
+        "s3:GetObjectAcl",
+        "s3:GetObjectLegalHold",
+        "s3:GetObjectRetention",
+        "s3:GetObjectTagging"
+      ],
+      "Resource": [
+        "arn:aws:s3:::my-s3-bucket/my-prefix/*"
+      ]
+    },
+    {
+      "Effect": "Allow",
+      "Action": [
+        "s3:PutObject",
+        "s3:DeleteObject"
+      ],
+      "Resource": [
+        "arn:aws:s3:::my-s3-bucket/my-prefix/*"
+      ]
+    }
+  ]
+}
+```
+<!-- [[[end]]] -->
+
+### --prefix my-prefix/ --read-only
+
+<!-- [[[cog
+result = runner.invoke(cli.cli, ["policy", "my-s3-bucket", "--prefix", "my-prefix/", "--read-only"])
+cog.out(
+    "```\n{}\n```".format(json.dumps(json.loads(result.output), indent=2))
+)
+]]] -->
+```
+{
+  "Version": "2012-10-17",
+  "Statement": [
+    {
+      "Effect": "Allow",
+      "Action": [
+        "s3:GetBucketLocation"
+      ],
+      "Resource": [
+        "arn:aws:s3:::my-s3-bucket"
+      ]
+    },
+    {
+      "Effect": "Allow",
+      "Action": [
+        "s3:ListBucket"
+      ],
+      "Resource": [
+        "arn:aws:s3:::my-s3-bucket"
+      ],
+      "Condition": {
+        "StringLike": {
+          "s3:prefix": [
+            "my-prefix/*"
+          ]
+        }
+      }
+    },
+    {
+      "Effect": "Allow",
+      "Action": [
+        "s3:GetObject",
+        "s3:GetObjectAcl",
+        "s3:GetObjectLegalHold",
+        "s3:GetObjectRetention",
+        "s3:GetObjectTagging"
+      ],
+      "Resource": [
+        "arn:aws:s3:::my-s3-bucket/my-prefix/*"
+      ]
+    }
+  ]
+}
+```
+<!-- [[[end]]] -->
+
+### --prefix my-prefix/ --write-only
+
+<!-- [[[cog
+result = runner.invoke(cli.cli, ["policy", "my-s3-bucket", "--prefix", "my-prefix/", "--write-only"])
+cog.out(
+    "```\n{}\n```".format(json.dumps(json.loads(result.output), indent=2))
+)
+]]] -->
+```
+{
+  "Version": "2012-10-17",
+  "Statement": [
+    {
+      "Effect": "Allow",
+      "Action": [
+        "s3:PutObject"
+      ],
+      "Resource": [
+        "arn:aws:s3:::my-s3-bucket/my-prefix/*"
+      ]
+    }
+  ]
+}
+```
+<!-- [[[end]]] -->
+
 ### public bucket policy
 
 Buckets created using the `--public` option will have the following bucket policy attached to them:
 
 <!-- [[[cog
 result = runner.invoke(cli.cli, ["policy", "my-s3-bucket", "--public-bucket"])
 cog.out(
@@ -604,12 +771,12 @@
 
 ### Integration tests
 
 The main tests all use stubbed interfaces to AWS, so will not make any outbound API calls.
 
 There is also a suite of integration tests in `tests/test_integration.py` which DO make API calls to AWS, using credentials from your environment variables or `~/.aws/credentials` file.
 
-These tests are skipped by default. If you have AWS configured with an account that has permission to run `s3-credentials` (create users, roles, buckets etc) you can run these tests using:
+These tests are skipped by default. If you have AWS configured with an account that has permission to run the actions required by `s3-credentials` (create users, roles, buckets etc) you can run these tests using:
 
     pytest --integration
 
 The tests will create a number of different users and buckets and should then delete them once they finish running.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `s3-credentials-0.8/s3_credentials/cli.py` & `s3-credentials-0.9/s3_credentials/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from re import A
 import boto3
 import botocore
 import click
 import configparser
+from csv import DictWriter
 import io
+import itertools
 import json
 import mimetypes
 import os
 import re
 import sys
+import textwrap
 from . import policies
 
 
 def bucket_exists(s3, bucket):
     try:
         s3.head_bucket(Bucket=bucket)
         return True
@@ -55,14 +58,26 @@
             ),
         )
     ):
         fn = decorator(fn)
     return fn
 
 
+def common_output_options(fn):
+    for decorator in reversed(
+        (
+            click.option("--nl", help="Output newline-delimited JSON", is_flag=True),
+            click.option("--csv", help="Output CSV", is_flag=True),
+            click.option("--tsv", help="Output TSV", is_flag=True),
+        )
+    ):
+        fn = decorator(fn)
+    return fn
+
+
 @click.group()
 @click.version_option()
 def cli():
     "A tool for creating credentials for accessing S3 buckets"
 
 
 class PolicyParam(click.ParamType):
@@ -120,43 +135,47 @@
     "buckets",
     nargs=-1,
     required=True,
 )
 @click.option("--read-only", help="Only allow reading from the bucket", is_flag=True)
 @click.option("--write-only", help="Only allow writing to the bucket", is_flag=True)
 @click.option(
+    "--prefix", help="Restrict to keys starting with this prefix", default="*"
+)
+@click.option(
     "--public-bucket",
     help="Bucket policy for allowing public access",
     is_flag=True,
 )
-def policy(buckets, read_only, write_only, public_bucket):
+def policy(buckets, read_only, write_only, prefix, public_bucket):
+    "Generate JSON policy for one or more buckets"
     if public_bucket:
         if len(buckets) != 1:
             raise click.ClickException(
-                "--public-bucket-policy can only be generated for a single bucket"
+                "--public-bucket policy can only be generated for a single bucket"
             )
         click.echo(
             json.dumps(policies.bucket_policy_allow_all_get(buckets[0]), indent=4)
         )
         return
     permission = "read-write"
     if read_only:
         permission = "read-only"
     if write_only:
         permission = "write-only"
     statements = []
     if permission == "read-write":
         for bucket in buckets:
-            statements.extend(policies.read_write_statements(bucket))
+            statements.extend(policies.read_write_statements(bucket, prefix))
     elif permission == "read-only":
         for bucket in buckets:
-            statements.extend(policies.read_only_statements(bucket))
+            statements.extend(policies.read_only_statements(bucket, prefix))
     elif permission == "write-only":
         for bucket in buckets:
-            statements.extend(policies.write_only_statements(bucket))
+            statements.extend(policies.write_only_statements(bucket, prefix))
     else:
         assert False, "Unknown permission: {}".format(permission)
     bucket_access_policy = policies.wrap_policy(statements)
     click.echo(json.dumps(bucket_access_policy, indent=4))
 
 
 @cli.command()
@@ -183,14 +202,17 @@
 @click.option(
     "-c",
     "--create-bucket",
     help="Create buckets if they do not already exist",
     is_flag=True,
 )
 @click.option(
+    "--prefix", help="Restrict to keys starting with this prefix", default="*"
+)
+@click.option(
     "--public",
     help="Make the created bucket public: anyone will be able to download files if they know their name",
     is_flag=True,
 )
 @click.option("--read-only", help="Only allow reading from the bucket", is_flag=True)
 @click.option("--write-only", help="Only allow writing to the bucket", is_flag=True)
 @click.option(
@@ -212,14 +234,15 @@
 @common_boto3_options
 def create(
     buckets,
     format_,
     duration,
     username,
     create_bucket,
+    prefix,
     public,
     read_only,
     write_only,
     policy,
     bucket_region,
     user_permissions_boundary,
     silent,
@@ -281,66 +304,68 @@
                                 " with args {}".format(json.dumps(kwargs, indent=4))
                                 if kwargs
                                 else ""
                             ),
                         )
                     )
                     if bucket_policy:
-                        click.echo("... then the following bucket policy:")
+                        click.echo("... then attach the following bucket policy to it:")
                         click.echo(json.dumps(bucket_policy, indent=4))
                 else:
                     s3.create_bucket(Bucket=bucket, **kwargs)
                     info = "Created bucket: {}".format(bucket)
                     if bucket_region:
-                        info += "in region: {}".format(bucket_region)
+                        info += " in region: {}".format(bucket_region)
                     log(info)
+
                     if bucket_policy:
                         s3.put_bucket_policy(
                             Bucket=bucket, Policy=json.dumps(bucket_policy)
                         )
                         log("Attached bucket policy allowing public access")
-    # At this point the buckets definitely exist - create the inline policy
+    # At this point the buckets definitely exist - create the inline policy for assume_role()
+    assume_role_policy = {}
     bucket_access_policy = {}
     if policy:
-        bucket_access_policy = json.loads(policy.replace("$!BUCKET_NAME!$", bucket))
+        assume_role_policy = json.loads(policy.replace("$!BUCKET_NAME!$", bucket))
     else:
         statements = []
         if permission == "read-write":
             for bucket in buckets:
-                statements.extend(policies.read_write_statements(bucket))
+                statements.extend(policies.read_write_statements(bucket, prefix))
         elif permission == "read-only":
             for bucket in buckets:
-                statements.extend(policies.read_only_statements(bucket))
+                statements.extend(policies.read_only_statements(bucket, prefix))
         elif permission == "write-only":
             for bucket in buckets:
-                statements.extend(policies.write_only_statements(bucket))
+                statements.extend(policies.write_only_statements(bucket, prefix))
         else:
             assert False, "Unknown permission: {}".format(permission)
-        bucket_access_policy = policies.wrap_policy(statements)
+        assume_role_policy = policies.wrap_policy(statements)
 
     if duration:
         # We're going to use sts.assume_role() rather than creating a user
         if dry_run:
             click.echo("Would ensure role: 's3-credentials.AmazonS3FullAccess'")
             click.echo(
                 "Would assume role using following policy for {} seconds:".format(
                     duration
                 )
             )
-            click.echo(json.dumps(bucket_access_policy, indent=4))
+            click.echo(json.dumps(assume_role_policy, indent=4))
         else:
             s3_role_arn = ensure_s3_role_exists(iam, sts)
             log("Assume role against {} for {}s".format(s3_role_arn, duration))
             credentials_response = sts.assume_role(
                 RoleArn=s3_role_arn,
                 RoleSessionName="s3.{permission}.{buckets}".format(
                     permission="custom" if policy else permission,
                     buckets=",".join(buckets),
                 ),
-                Policy=json.dumps(bucket_access_policy),
+                Policy=json.dumps(assume_role_policy),
                 DurationSeconds=duration,
             )
             if format_ == "ini":
                 click.echo(
                     (
                         "[default]\naws_access_key_id={}\n"
                         "aws_secret_access_key={}\naws_session_token={}"
@@ -387,42 +412,43 @@
         if dry_run:
             click.echo("Would create{}".format(info))
         else:
             iam.create_user(**kwargs)
             log("Created {}".format(info))
 
     # Add inline policies to the user so they can access the buckets
+    user_policy = {}
     for bucket in buckets:
         policy_name = "s3.{permission}.{bucket}".format(
             permission="custom" if policy else permission,
             bucket=bucket,
         )
         if policy:
-            policy_dict = json.loads(policy.replace("$!BUCKET_NAME!$", bucket))
+            user_policy = json.loads(policy.replace("$!BUCKET_NAME!$", bucket))
         else:
             if permission == "read-write":
-                policy_dict = policies.read_write(bucket)
+                user_policy = policies.read_write(bucket, prefix)
             elif permission == "read-only":
-                policy_dict = policies.read_only(bucket)
+                user_policy = policies.read_only(bucket, prefix)
             elif permission == "write-only":
-                policy_dict = policies.write_only(bucket)
+                user_policy = policies.write_only(bucket, prefix)
             else:
                 assert False, "Unknown permission: {}".format(permission)
 
         if dry_run:
             click.echo(
                 "Would attach policy called '{}' to user '{}', details:\n{}".format(
                     policy_name,
                     username,
-                    json.dumps(policy_dict, indent=4),
+                    json.dumps(user_policy, indent=4),
                 )
             )
         else:
             iam.put_user_policy(
-                PolicyDocument=json.dumps(policy_dict),
+                PolicyDocument=json.dumps(user_policy),
                 PolicyName=policy_name,
                 UserName=username,
             )
             log("Attached policy {} to user {}".format(policy_name, username))
 
     # Retrieve and print out the credentials
     if dry_run:
@@ -450,33 +476,43 @@
     sts = make_client("sts", **boto_options)
     identity = sts.get_caller_identity()
     identity.pop("ResponseMetadata")
     click.echo(json.dumps(identity, indent=4, default=str))
 
 
 @cli.command()
-@click.option("--array", help="Output a valid JSON array", is_flag=True)
-@click.option("--nl", help="Output newline-delimited JSON", is_flag=True)
+@common_output_options
 @common_boto3_options
-def list_users(array, nl, **boto_options):
+def list_users(nl, csv, tsv, **boto_options):
     "List all users"
     iam = make_client("iam", **boto_options)
     paginator = iam.get_paginator("list_users")
     gathered = []
-    for response in paginator.paginate():
-        for user in response["Users"]:
-            if array:
-                gathered.append(user)
-            else:
-                if nl:
-                    click.echo(json.dumps(user, default=str))
-                else:
-                    click.echo(json.dumps(user, indent=4, default=str))
-    if gathered:
-        click.echo(json.dumps(gathered, indent=4, default=str))
+
+    def iterate():
+        for response in paginator.paginate():
+            for user in response["Users"]:
+                yield user
+
+    output(
+        iterate(),
+        (
+            "UserName",
+            "UserId",
+            "Arn",
+            "Path",
+            "CreateDate",
+            "PasswordLastUsed",
+            "PermissionsBoundary",
+            "Tags",
+        ),
+        nl,
+        csv,
+        tsv,
+    )
 
 
 @cli.command()
 @click.argument("usernames", nargs=-1)
 @common_boto3_options
 def list_user_policies(usernames, **boto_options):
     "List inline policies for specified user"
@@ -501,60 +537,58 @@
                     json.dumps(policy_response["PolicyDocument"], indent=4, default=str)
                 )
 
 
 @cli.command()
 @click.argument("buckets", nargs=-1)
 @click.option("--details", help="Include extra bucket details (slower)", is_flag=True)
-@click.option("--array", help="Output a valid JSON array", is_flag=True)
-@click.option("--nl", help="Output newline-delimited JSON", is_flag=True)
+@common_output_options
 @common_boto3_options
-def list_buckets(buckets, details, array, nl, **boto_options):
+def list_buckets(buckets, details, nl, csv, tsv, **boto_options):
     "List buckets - defaults to all, or pass one or more bucket names"
     s3 = make_client("s3", **boto_options)
-    gathered = []
-    for bucket in s3.list_buckets()["Buckets"]:
-        if buckets and (bucket["Name"] not in buckets):
-            continue
-        if details:
-            bucket_acl = dict(
-                (key, value)
-                for key, value in s3.get_bucket_acl(
-                    Bucket=bucket["Name"],
-                ).items()
-                if key != "ResponseMetadata"
-            )
-            try:
-                pab = s3.get_public_access_block(
-                    Bucket=bucket["Name"],
-                )["PublicAccessBlockConfiguration"]
-            except s3.exceptions.ClientError:
-                pab = None
-            try:
-                bucket_website = dict(
+
+    headers = ["Name", "CreationDate"]
+    if details:
+        headers += ["bucket_acl", "public_access_block", "bucket_website"]
+
+    def iterator():
+        for bucket in s3.list_buckets()["Buckets"]:
+            if buckets and (bucket["Name"] not in buckets):
+                continue
+            if details:
+                bucket_acl = dict(
                     (key, value)
-                    for key, value in s3.get_bucket_website(
+                    for key, value in s3.get_bucket_acl(
                         Bucket=bucket["Name"],
                     ).items()
                     if key != "ResponseMetadata"
                 )
-            except s3.exceptions.ClientError:
-                bucket_website = None
-            bucket["bucket_acl"] = bucket_acl
-            bucket["public_access_block"] = pab
-            bucket["bucket_website"] = bucket_website
-        if array:
-            gathered.append(bucket)
-        else:
-            if nl:
-                click.echo(json.dumps(bucket, default=str))
-            else:
-                click.echo(json.dumps(bucket, indent=4, default=str))
-    if gathered:
-        click.echo(json.dumps(gathered, indent=4, default=str))
+                try:
+                    pab = s3.get_public_access_block(
+                        Bucket=bucket["Name"],
+                    )["PublicAccessBlockConfiguration"]
+                except s3.exceptions.ClientError:
+                    pab = None
+                try:
+                    bucket_website = dict(
+                        (key, value)
+                        for key, value in s3.get_bucket_website(
+                            Bucket=bucket["Name"],
+                        ).items()
+                        if key != "ResponseMetadata"
+                    )
+                except s3.exceptions.ClientError:
+                    bucket_website = None
+                bucket["bucket_acl"] = bucket_acl
+                bucket["public_access_block"] = pab
+                bucket["bucket_website"] = bucket_website
+            yield bucket
+
+    output(iterator(), headers, nl, csv, tsv)
 
 
 @cli.command()
 @click.argument("usernames", nargs=-1, required=True)
 @common_boto3_options
 def delete_user(usernames, **boto_options):
     "Delete specified users, their access keys and their inline policies"
@@ -663,22 +697,40 @@
             PolicyArn="arn:aws:iam::aws:policy/AmazonS3FullAccess",
         )
         return create_role_response["Role"]["Arn"]
 
 
 @cli.command()
 @click.argument("bucket")
+@click.option("--prefix", help="List keys starting with this prefix")
+@common_output_options
 @common_boto3_options
-def list_bucket(bucket, **boto_options):
+def list_bucket(bucket, prefix, nl, csv, tsv, **boto_options):
     "List content of bucket"
     s3 = make_client("s3", **boto_options)
     paginator = s3.get_paginator("list_objects_v2")
-    for page in paginator.paginate(Bucket=bucket):
-        for row in page["Contents"]:
-            click.echo(json.dumps(row, indent=4, default=str))
+    kwargs = {"Bucket": bucket}
+    if prefix:
+        kwargs["Prefix"] = prefix
+
+    def iterate():
+        try:
+            for page in paginator.paginate(**kwargs):
+                for row in page["Contents"]:
+                    yield row
+        except botocore.exceptions.ClientError as e:
+            raise click.ClickException(e)
+
+    output(
+        iterate(),
+        ("Key", "LastModified", "ETag", "Size", "StorageClass", "Owner"),
+        nl,
+        csv,
+        tsv,
+    )
 
 
 @cli.command()
 @click.argument("bucket")
 @click.argument("key")
 @click.argument(
     "content",
@@ -735,7 +787,47 @@
     "Download an object from an S3 bucket"
     s3 = make_client("s3", **boto_options)
     if not output:
         fp = sys.stdout.buffer
     else:
         fp = click.open_file(output, "wb")
     s3.download_fileobj(bucket, key, fp)
+
+
+def output(iterator, headers, nl, csv, tsv):
+    if nl:
+        for item in iterator:
+            click.echo(json.dumps(item, default=str))
+    elif csv or tsv:
+        writer = DictWriter(
+            sys.stdout, headers, dialect="excel-tab" if tsv else "excel"
+        )
+        writer.writeheader()
+        writer.writerows(iterator)
+    else:
+        for line in stream_indented_json(iterator):
+            click.echo(line)
+
+
+def stream_indented_json(iterator, indent=2):
+    # We have to iterate two-at-a-time so we can know if we
+    # should output a trailing comma or if we have reached
+    # the last item.
+    current_iter, next_iter = itertools.tee(iterator, 2)
+    next(next_iter, None)
+    first = True
+    for item, next_item in itertools.zip_longest(current_iter, next_iter):
+        is_last = next_item is None
+        data = item
+        line = "{first}{serialized}{separator}{last}".format(
+            first="[\n" if first else "",
+            serialized=textwrap.indent(
+                json.dumps(data, indent=indent, default=str), " " * indent
+            ),
+            separator="," if not is_last else "",
+            last="\n]" if is_last else "",
+        )
+        yield line
+        first = False
+    if first:
+        # We didn't output anything, so yield the empty list
+        yield "[]"
```

### Comparing `s3-credentials-0.8/s3_credentials.egg-info/PKG-INFO` & `s3-credentials-0.9/s3_credentials.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s3-credentials
-Version: 0.8
+Version: 0.9
 Summary: A tool for creating credentials for accessing S3 buckets
 Home-page: https://github.com/simonw/s3-credentials
 Author: Simon Willison
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/simonw/s3-credentials/issues
 Project-URL: CI, https://github.com/simonw/s3-credentials/actions
 Project-URL: Changelog, https://github.com/simonw/s3-credentials/releases
@@ -21,20 +21,14 @@
 [![Tests](https://github.com/simonw/s3-credentials/workflows/Test/badge.svg)](https://github.com/simonw/s3-credentials/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/simonw/s3-credentials/blob/master/LICENSE)
 
 A tool for creating credentials for accessing S3 buckets
 
 For project background, see [s3-credentials: a tool for creating credentials for S3 buckets](https://simonwillison.net/2021/Nov/3/s3-credentials/) on my blog.
 
-## ⚠️ Warning
-
-I am not an AWS security expert. You shoud review how this tool works carefully before using it against with own AWS account.
-
-If you are an AWS security expert I would [love to get your feedback](https://github.com/simonw/s3-credentials/issues/7)!
-
 ## Installation
 
 Install this tool using `pip`:
 
     $ pip install s3-credentials
 
 ## Configuration
@@ -102,14 +96,15 @@
 
 The `create` command has a number of options:
 
 - `--format TEXT`: The output format to use. Defaults to `json`, but can also be `ini`.
 - `--duration 15m`: For temporary credentials, how long should they last? This can be specified in seconds, minutes or hours using a suffix of `s`, `m` or `h` - but must be between 15 minutes and 12 hours.
 - `--username TEXT`: The username to use for the user that is created by the command (or the username of an existing user if you do not want to create a new one). If ommitted a default such as `s3.read-write.static.niche-museums.com` will be used.
 - `-c, --create-bucket`: Create the buckets if they do not exist. Without this any missing buckets will be treated as an error.
+- `--prefix my-prefix/`: Credentials should only allow access to keys in the S3 bucket that start with this prefix.
 - `--public`: When creating a bucket, set it so that any file uploaded to that bucket can be downloaded by anyone who knows its filename. This attaches the [public bucket policy](#public-bucket-policy) shown below.
 - `--read-only`: The user should only be allowed to read files from the bucket.
 - `--write-only`: The user should only be allowed to write files to the bucket, but not read them. This can be useful for logging and backups.
 - `--policy filepath-or-string`: A custom policy document (as a file path, literal JSON string or `-` for standard input) - see below.
 - `--bucket-region`: If creating buckets, the region in which they should be created.
 - `--silent`: Don't output details of what is happening, just output the JSON for the created access credentials at the end.
 - `--dry-run`: Output details of AWS changes that would have been made without applying them.
@@ -119,15 +114,15 @@
 
 How the tool works varies depending on if you are creating temporary or permanent credentials.
 
 For permanent credentials, the steps are as follows:
 
 1. Confirm that each of the specified buckets exists. If they do not and `--create-bucket` was passed create them - otherwise exit with an error.
 2. If a username was not specified, derive a username using the `s3.$permission.$buckets` format.
-3. If a user with that username does not exist, create one with an S3 permissions boundary that respects the `--read-only` option - unless `--user-permissions-boundary=none` was passed (or a custom permissions boundary string).
+3. If a user with that username does not exist, create one with an S3 permissions boundary of [AmazonS3ReadOnlyAccess](https://github.com/glassechidna/trackiam/blob/master/policies/AmazonS3ReadOnlyAccess.json) for `--read-only` or [AmazonS3FullAccess](https://github.com/glassechidna/trackiam/blob/master/policies/AmazonS3FullAccess.json) otherwise - unless `--user-permissions-boundary=none` was passed, or a custom permissions boundary string.
 4. For each specified bucket, add an inline IAM policy to the user that gives them permission to either read-only, write-only or read-write against that bucket.
 5. Create a new access key for that user and output the key and its secret to the console.
 
 For temporary credentials:
 
 1. Confirm or create buckets, in the same way as for permanent credentials.
 2. Check if an AWS role called `s3-credentials.AmazonS3FullAccess` exists. If it does not exist create it, configured to allow the user's AWS account to assume it and with the `arn:aws:iam::aws:policy/AmazonS3FullAccess` policy attached.
@@ -184,14 +179,15 @@
 
 ### policy
 
 You can use the `s3-credentials policy` command to generate the JSON policy document that would be used without applying it. The command takes one or more required bucket names and a subset of the options available on the `create` command:
 
 - `--read-only` - generate a read-only policy
 - `--write-only` - generate a write-only policy
+- `--prefix` - policy should be restricted to keys in the bucket that start with this prefix
 - `--public-bucket` - generate a bucket policy for a public bucket
 
 With none of these options it defaults to a read-write policy.
 ```
 % s3-credentials policy my-bucket --read-only
 {
     "Version": "2012-10-17",
@@ -218,19 +214,19 @@
 ```
 ### list-users
 
 To see a list of all users that exist for your AWS account:
 
     s3-credentials list-users
 
-This will return pretty-printed JSON objects by default.
+This will a pretty-printed array of JSON objects by default.
 
 Add `--nl` to collapse these to single lines as valid newline-delimited JSON.
 
-Add `--array` to output a valid JSON array of objects instead.
+Add `--csv` or `--tsv` to get back CSV or TSV data.
 
 ### list-buckets
 
 Shows a list of all buckets in your AWS account.
 
     % s3-credentials list-buckets
     {
@@ -246,15 +242,15 @@
 
     % s3-credentials list-buckets simonw-test-bucket-for-s3-credentials
     {
         "Name": "simonw-test-bucket-for-s3-credentials",
         "CreationDate": "2021-11-03 21:46:12+00:00"
     }
 
-This accepts the same `--nl` and `--array` options as `list-users`.
+This accepts the same `--nl`, `--csv` and `--tsv` options as `list-users`.
 
 Add `--details` to include details of the bucket ACL, website configuration and public access block settings. This is useful for running a security audit of your buckets.
 
 Using `--details` adds three additional API calls for each bucket, so it is advisable to use it with one or more explicit bucket names.
 ```
 % s3-credentials list-buckets simonw-test-public-website-bucket --details
 {
@@ -314,14 +310,39 @@
     "BlockPublicPolicy": true,
     "RestrictPublicBuckets": true
   },
   "bucket_website": null
 }
 ```
 
+### list-bucket
+
+To list the contents of a bucket, use `list-bucket`:
+
+```
+% s3-credentials list-bucket static.niche-museums.com
+[
+  {
+    "Key": "Griffith-Observatory.jpg",
+    "LastModified": "2020-01-05 16:51:01+00:00",
+    "ETag": "\"a4cff17d189e7eb0c4d3bf0257e56885\"",
+    "Size": 3360040,
+    "StorageClass": "STANDARD"
+  },
+  {
+    "Key": "IMG_0353.jpeg",
+    "LastModified": "2019-10-25 02:50:49+00:00",
+    "ETag": "\"d45bab0b65c0e4b03b2ac0359c7267e3\"",
+    "Size": 2581023,
+    "StorageClass": "STANDARD"
+  }
+]
+```
+This accepts the same `--nl`, `--csv` and `--tsv` options as `list-users`.
+
 ### list-user-policies
 
 To see a list of inline policies belonging to users:
 
 ```
 % s3-credentials list-user-policies s3.read-write.static.niche-museums.com
 
@@ -560,14 +581,160 @@
       ]
     }
   ]
 }
 ```
 <!-- [[[end]]] -->
 
+### --prefix my-prefix/
+
+<!-- [[[cog
+result = runner.invoke(cli.cli, ["policy", "my-s3-bucket", "--prefix", "my-prefix/"])
+cog.out(
+    "```\n{}\n```".format(json.dumps(json.loads(result.output), indent=2))
+)
+]]] -->
+```
+{
+  "Version": "2012-10-17",
+  "Statement": [
+    {
+      "Effect": "Allow",
+      "Action": [
+        "s3:GetBucketLocation"
+      ],
+      "Resource": [
+        "arn:aws:s3:::my-s3-bucket"
+      ]
+    },
+    {
+      "Effect": "Allow",
+      "Action": [
+        "s3:ListBucket"
+      ],
+      "Resource": [
+        "arn:aws:s3:::my-s3-bucket"
+      ],
+      "Condition": {
+        "StringLike": {
+          "s3:prefix": [
+            "my-prefix/*"
+          ]
+        }
+      }
+    },
+    {
+      "Effect": "Allow",
+      "Action": [
+        "s3:GetObject",
+        "s3:GetObjectAcl",
+        "s3:GetObjectLegalHold",
+        "s3:GetObjectRetention",
+        "s3:GetObjectTagging"
+      ],
+      "Resource": [
+        "arn:aws:s3:::my-s3-bucket/my-prefix/*"
+      ]
+    },
+    {
+      "Effect": "Allow",
+      "Action": [
+        "s3:PutObject",
+        "s3:DeleteObject"
+      ],
+      "Resource": [
+        "arn:aws:s3:::my-s3-bucket/my-prefix/*"
+      ]
+    }
+  ]
+}
+```
+<!-- [[[end]]] -->
+
+### --prefix my-prefix/ --read-only
+
+<!-- [[[cog
+result = runner.invoke(cli.cli, ["policy", "my-s3-bucket", "--prefix", "my-prefix/", "--read-only"])
+cog.out(
+    "```\n{}\n```".format(json.dumps(json.loads(result.output), indent=2))
+)
+]]] -->
+```
+{
+  "Version": "2012-10-17",
+  "Statement": [
+    {
+      "Effect": "Allow",
+      "Action": [
+        "s3:GetBucketLocation"
+      ],
+      "Resource": [
+        "arn:aws:s3:::my-s3-bucket"
+      ]
+    },
+    {
+      "Effect": "Allow",
+      "Action": [
+        "s3:ListBucket"
+      ],
+      "Resource": [
+        "arn:aws:s3:::my-s3-bucket"
+      ],
+      "Condition": {
+        "StringLike": {
+          "s3:prefix": [
+            "my-prefix/*"
+          ]
+        }
+      }
+    },
+    {
+      "Effect": "Allow",
+      "Action": [
+        "s3:GetObject",
+        "s3:GetObjectAcl",
+        "s3:GetObjectLegalHold",
+        "s3:GetObjectRetention",
+        "s3:GetObjectTagging"
+      ],
+      "Resource": [
+        "arn:aws:s3:::my-s3-bucket/my-prefix/*"
+      ]
+    }
+  ]
+}
+```
+<!-- [[[end]]] -->
+
+### --prefix my-prefix/ --write-only
+
+<!-- [[[cog
+result = runner.invoke(cli.cli, ["policy", "my-s3-bucket", "--prefix", "my-prefix/", "--write-only"])
+cog.out(
+    "```\n{}\n```".format(json.dumps(json.loads(result.output), indent=2))
+)
+]]] -->
+```
+{
+  "Version": "2012-10-17",
+  "Statement": [
+    {
+      "Effect": "Allow",
+      "Action": [
+        "s3:PutObject"
+      ],
+      "Resource": [
+        "arn:aws:s3:::my-s3-bucket/my-prefix/*"
+      ]
+    }
+  ]
+}
+```
+<!-- [[[end]]] -->
+
 ### public bucket policy
 
 Buckets created using the `--public` option will have the following bucket policy attached to them:
 
 <!-- [[[cog
 result = runner.invoke(cli.cli, ["policy", "my-s3-bucket", "--public-bucket"])
 cog.out(
@@ -620,14 +787,14 @@
 
 ### Integration tests
 
 The main tests all use stubbed interfaces to AWS, so will not make any outbound API calls.
 
 There is also a suite of integration tests in `tests/test_integration.py` which DO make API calls to AWS, using credentials from your environment variables or `~/.aws/credentials` file.
 
-These tests are skipped by default. If you have AWS configured with an account that has permission to run `s3-credentials` (create users, roles, buckets etc) you can run these tests using:
+These tests are skipped by default. If you have AWS configured with an account that has permission to run the actions required by `s3-credentials` (create users, roles, buckets etc) you can run these tests using:
 
     pytest --integration
 
 The tests will create a number of different users and buckets and should then delete them once they finish running.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `s3-credentials-0.8/setup.py` & `s3-credentials-0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-VERSION = "0.8"
+VERSION = "0.9"
 
 
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
```

