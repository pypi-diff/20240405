# Comparing `tmp/mkdocs_puml-1.2.4.tar.gz` & `tmp/mkdocs_puml-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_puml-1.2.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "mkdocs_puml-1.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `mkdocs_puml-1.2.4.tar` & `mkdocs_puml-1.3.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      237 2022-09-15 12:01:38.953711 mkdocs_puml-1.2.4/.coveragerc
--rw-r--r--   0        0        0    31089 2023-01-25 09:20:39.582596 mkdocs_puml-1.2.4/.docs/logo.png
--rw-r--r--   0        0        0       43 2022-09-15 12:01:38.953802 mkdocs_puml-1.2.4/.flake8
--rw-r--r--   0        0        0      655 2023-01-25 09:42:12.642417 mkdocs_puml-1.2.4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2022-11-13 12:18:46.573988 mkdocs_puml-1.2.4/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1284 2024-01-02 10:06:29.414708 mkdocs_puml-1.2.4/.github/workflows/checks.yml
--rw-r--r--   0        0        0     5494 2023-07-30 09:50:18.334236 mkdocs_puml-1.2.4/.gitignore
--rw-r--r--   0        0        0      404 2024-01-02 10:06:29.415474 mkdocs_puml-1.2.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      220 2023-07-30 09:50:18.334890 mkdocs_puml-1.2.4/.vscode/settings.json
--rw-r--r--   0        0        0     1082 2022-09-15 12:01:38.954367 mkdocs_puml-1.2.4/LICENSE
--rw-r--r--   0        0        0      581 2024-01-02 10:06:29.415940 mkdocs_puml-1.2.4/Pipfile
--rw-r--r--   0        0        0    78518 2024-01-02 10:06:29.416725 mkdocs_puml-1.2.4/Pipfile.lock
--rw-r--r--   0        0        0     3881 2024-01-02 09:32:21.156073 mkdocs_puml-1.2.4/README.md
--rw-r--r--   0        0        0       68 2024-01-02 10:06:29.417130 mkdocs_puml-1.2.4/mkdocs_puml/__init__.py
--rw-r--r--   0        0        0      948 2023-02-18 11:50:55.936744 mkdocs_puml-1.2.4/mkdocs_puml/encoder.py
--rw-r--r--   0        0        0     5143 2024-01-02 09:32:34.230339 mkdocs_puml-1.2.4/mkdocs_puml/plugin.py
--rw-r--r--   0        0        0     3841 2024-01-02 09:32:46.850243 mkdocs_puml-1.2.4/mkdocs_puml/puml.py
--rw-r--r--   0        0        0      628 2024-01-02 09:06:43.936369 mkdocs_puml-1.2.4/pyproject.toml
--rw-r--r--   0        0        0        0 2022-09-15 12:01:38.956165 mkdocs_puml-1.2.4/tests/__init__.py
--rw-r--r--   0        0        0      866 2023-03-22 10:02:51.667442 mkdocs_puml-1.2.4/tests/conftest.py
--rw-r--r--   0        0        0        0 2022-09-20 17:56:58.447859 mkdocs_puml-1.2.4/tests/plugins/__init__.py
--rw-r--r--   0        0        0     2374 2023-06-28 09:10:05.717513 mkdocs_puml-1.2.4/tests/plugins/conftest.py
--rw-r--r--   0        0        0     2247 2023-06-28 09:10:05.717746 mkdocs_puml-1.2.4/tests/plugins/test_plugin.py
--rw-r--r--   0        0        0      197 2022-09-15 12:01:38.956431 mkdocs_puml-1.2.4/tests/test_encoder.py
--rw-r--r--   0        0        0      876 2023-01-25 09:21:05.750584 mkdocs_puml-1.2.4/tests/test_puml.py
--rw-r--r--   0        0        0     1074 2023-03-22 10:02:51.667954 mkdocs_puml-1.2.4/tests/testdata/markdown.md
--rw-r--r--   0        0        0      375 2022-09-20 17:56:58.448279 mkdocs_puml-1.2.4/tests/testdata/output.html
--rw-r--r--   0        0        0     2255 2022-09-15 12:01:38.956767 mkdocs_puml-1.2.4/tests/testdata/plantuml.svg
--rw-r--r--   0        0        0     4334 1970-01-01 00:00:00.000000 mkdocs_puml-1.2.4/PKG-INFO
+-rw-r--r--   0        0        0      237 2022-09-15 12:01:38.953711 mkdocs_puml-1.3.0/.coveragerc
+-rw-r--r--   0        0        0    31089 2023-01-25 09:20:39.582596 mkdocs_puml-1.3.0/.docs/logo.png
+-rw-r--r--   0        0        0       43 2022-09-15 12:01:38.953802 mkdocs_puml-1.3.0/.flake8
+-rw-r--r--   0        0        0      655 2023-01-25 09:42:12.642417 mkdocs_puml-1.3.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2022-11-13 12:18:46.573988 mkdocs_puml-1.3.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1284 2024-01-02 10:06:29.414708 mkdocs_puml-1.3.0/.github/workflows/checks.yml
+-rw-r--r--   0        0        0     5494 2023-07-30 09:50:18.334236 mkdocs_puml-1.3.0/.gitignore
+-rw-r--r--   0        0        0      404 2024-01-02 10:06:29.415474 mkdocs_puml-1.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      220 2023-07-30 09:50:18.334890 mkdocs_puml-1.3.0/.vscode/settings.json
+-rw-r--r--   0        0        0     1082 2022-09-15 12:01:38.954367 mkdocs_puml-1.3.0/LICENSE
+-rw-r--r--   0        0        0      581 2024-01-02 10:06:29.415940 mkdocs_puml-1.3.0/Pipfile
+-rw-r--r--   0        0        0    79073 2024-04-05 14:23:42.978809 mkdocs_puml-1.3.0/Pipfile.lock
+-rw-r--r--   0        0        0     4005 2024-04-05 14:07:33.659657 mkdocs_puml-1.3.0/README.md
+-rw-r--r--   0        0        0       68 2024-04-05 14:06:58.394749 mkdocs_puml-1.3.0/mkdocs_puml/__init__.py
+-rw-r--r--   0        0        0      948 2023-02-18 11:50:55.936744 mkdocs_puml-1.3.0/mkdocs_puml/encoder.py
+-rw-r--r--   0        0        0     5370 2024-04-05 14:15:19.574845 mkdocs_puml-1.3.0/mkdocs_puml/plugin.py
+-rw-r--r--   0        0        0     4054 2024-04-05 14:05:29.674877 mkdocs_puml-1.3.0/mkdocs_puml/puml.py
+-rw-r--r--   0        0        0      628 2024-01-02 09:06:43.936369 mkdocs_puml-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-09-15 12:01:38.956165 mkdocs_puml-1.3.0/tests/__init__.py
+-rw-r--r--   0        0        0      866 2023-03-22 10:02:51.667442 mkdocs_puml-1.3.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2022-09-20 17:56:58.447859 mkdocs_puml-1.3.0/tests/plugins/__init__.py
+-rw-r--r--   0        0        0     2374 2023-06-28 09:10:05.717513 mkdocs_puml-1.3.0/tests/plugins/conftest.py
+-rw-r--r--   0        0        0     2247 2023-06-28 09:10:05.717746 mkdocs_puml-1.3.0/tests/plugins/test_plugin.py
+-rw-r--r--   0        0        0      197 2022-09-15 12:01:38.956431 mkdocs_puml-1.3.0/tests/test_encoder.py
+-rw-r--r--   0        0        0      876 2023-01-25 09:21:05.750584 mkdocs_puml-1.3.0/tests/test_puml.py
+-rw-r--r--   0        0        0     1074 2023-03-22 10:02:51.667954 mkdocs_puml-1.3.0/tests/testdata/markdown.md
+-rw-r--r--   0        0        0      375 2022-09-20 17:56:58.448279 mkdocs_puml-1.3.0/tests/testdata/output.html
+-rw-r--r--   0        0        0     2255 2022-09-15 12:01:38.956767 mkdocs_puml-1.3.0/tests/testdata/plantuml.svg
+-rw-r--r--   0        0        0     4458 1970-01-01 00:00:00.000000 mkdocs_puml-1.3.0/PKG-INFO
```

### Comparing `mkdocs_puml-1.2.4/.docs/logo.png` & `mkdocs_puml-1.3.0/.docs/logo.png`

 * *Files identical despite different names*

### Comparing `mkdocs_puml-1.2.4/.github/ISSUE_TEMPLATE/bug_report.md` & `mkdocs_puml-1.3.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `mkdocs_puml-1.2.4/.github/ISSUE_TEMPLATE/feature_request.md` & `mkdocs_puml-1.3.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `mkdocs_puml-1.2.4/.github/workflows/checks.yml` & `mkdocs_puml-1.3.0/.github/workflows/checks.yml`

 * *Files identical despite different names*

### Comparing `mkdocs_puml-1.2.4/.gitignore` & `mkdocs_puml-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `mkdocs_puml-1.2.4/LICENSE` & `mkdocs_puml-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_puml-1.2.4/Pipfile` & `mkdocs_puml-1.3.0/Pipfile`

 * *Files identical despite different names*

### Comparing `mkdocs_puml-1.2.4/Pipfile.lock` & `mkdocs_puml-1.3.0/Pipfile.lock`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9770646640906538%*

 * *Differences: {"'default'": "{'certifi': {'hashes': "*

 * *              "['sha256:0569859f95fc761b18b45ef421b1290a0f65f147e92a1e5eb3e635f9a5e4e66f', "*

 * *              "'sha256:dc383c07b76109f368f6106eee2b593b04a011ea4d55f652c6ca24a754d1cdd1'], "*

 * *              "'version': '==2024.2.2'}, 'jinja2': {'hashes': "*

 * *              "['sha256:7d6d50dd97d52cbc355597bd845fabfbac3f551e1f99619e39a35ce8c370b5fa', "*

 * *              "'sha256:ac8bd6544d4bb2c9792bf3a159e80bba8fda7f07e81bc3aed565432d5925ba90'], "*

 * *              "'version': '==3.1.3'} […]*

```diff
@@ -14,19 +14,19 @@
                 "verify_ssl": true
             }
         ]
     },
     "default": {
         "certifi": {
             "hashes": [
-                "sha256:9b469f3a900bf28dc19b8cfbf8019bf47f7fdd1a65a1d4ffb98fc14166beb4d1",
-                "sha256:e036ab49d5b79556f99cfc2d9320b34cfbe5be05c5871b51de9329f0603b0474"
+                "sha256:0569859f95fc761b18b45ef421b1290a0f65f147e92a1e5eb3e635f9a5e4e66f",
+                "sha256:dc383c07b76109f368f6106eee2b593b04a011ea4d55f652c6ca24a754d1cdd1"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==2023.11.17"
+            "version": "==2024.2.2"
         },
         "charset-normalizer": {
             "hashes": [
                 "sha256:06435b539f889b1f6f4ac1758871aae42dc3a8c0e24ac9e60c2384973ad73027",
                 "sha256:06a81e93cd441c56a9b65d8e1d043daeb97a3d0856d177d5c90ba85acb3db087",
                 "sha256:0a55554a2fa0d408816b3b5cedf0045f4b8e1a6065aec45849de2d6f3f8e9786",
                 "sha256:0b2b64d2bb6d3fb9112bafa732def486049e63de9618b5843bcdd081d8144cd8",
@@ -166,93 +166,93 @@
                 "sha256:c05567e9c24a6b9faaa835c4821bad0590fbb9d5779e7caa6e1cc4978e7eb24f"
             ],
             "markers": "python_version >= '3.5'",
             "version": "==3.6"
         },
         "jinja2": {
             "hashes": [
-                "sha256:31351a702a408a9e7595a8fc6150fc3f43bb6bf7e319770cbc0db9df9437e852",
-                "sha256:6088930bfe239f0e6710546ab9c19c9ef35e29792895fed6e6e31a023a182a61"
+                "sha256:7d6d50dd97d52cbc355597bd845fabfbac3f551e1f99619e39a35ce8c370b5fa",
+                "sha256:ac8bd6544d4bb2c9792bf3a159e80bba8fda7f07e81bc3aed565432d5925ba90"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.1.2"
+            "version": "==3.1.3"
         },
         "markdown": {
             "hashes": [
-                "sha256:5874b47d4ee3f0b14d764324d2c94c03ea66bee56f2d929da9f2508d65e722dc",
-                "sha256:b65d7beb248dc22f2e8a31fb706d93798093c308dc1aba295aedeb9d41a813bd"
+                "sha256:48f276f4d8cfb8ce6527c8f79e2ee29708508bf4d40aa410fbc3b4ee832c850f",
+                "sha256:ed4f41f6daecbeeb96e576ce414c41d2d876daa9a16cb35fa8ed8c2ddfad0224"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==3.5.1"
+            "version": "==3.6"
         },
         "markupsafe": {
             "hashes": [
-                "sha256:05fb21170423db021895e1ea1e1f3ab3adb85d1c2333cbc2310f2a26bc77272e",
-                "sha256:0a4e4a1aff6c7ac4cd55792abf96c915634c2b97e3cc1c7129578aa68ebd754e",
-                "sha256:10bbfe99883db80bdbaff2dcf681dfc6533a614f700da1287707e8a5d78a8431",
-                "sha256:134da1eca9ec0ae528110ccc9e48041e0828d79f24121a1a146161103c76e686",
-                "sha256:14ff806850827afd6b07a5f32bd917fb7f45b046ba40c57abdb636674a8b559c",
-                "sha256:1577735524cdad32f9f694208aa75e422adba74f1baee7551620e43a3141f559",
-                "sha256:1b40069d487e7edb2676d3fbdb2b0829ffa2cd63a2ec26c4938b2d34391b4ecc",
-                "sha256:1b8dd8c3fd14349433c79fa8abeb573a55fc0fdd769133baac1f5e07abf54aeb",
-                "sha256:1f67c7038d560d92149c060157d623c542173016c4babc0c1913cca0564b9939",
-                "sha256:282c2cb35b5b673bbcadb33a585408104df04f14b2d9b01d4c345a3b92861c2c",
-                "sha256:2c1b19b3aaacc6e57b7e25710ff571c24d6c3613a45e905b1fde04d691b98ee0",
-                "sha256:2ef12179d3a291be237280175b542c07a36e7f60718296278d8593d21ca937d4",
-                "sha256:338ae27d6b8745585f87218a3f23f1512dbf52c26c28e322dbe54bcede54ccb9",
-                "sha256:3c0fae6c3be832a0a0473ac912810b2877c8cb9d76ca48de1ed31e1c68386575",
-                "sha256:3fd4abcb888d15a94f32b75d8fd18ee162ca0c064f35b11134be77050296d6ba",
-                "sha256:42de32b22b6b804f42c5d98be4f7e5e977ecdd9ee9b660fda1a3edf03b11792d",
-                "sha256:47d4f1c5f80fc62fdd7777d0d40a2e9dda0a05883ab11374334f6c4de38adffd",
-                "sha256:504b320cd4b7eff6f968eddf81127112db685e81f7e36e75f9f84f0df46041c3",
-                "sha256:525808b8019e36eb524b8c68acdd63a37e75714eac50e988180b169d64480a00",
-                "sha256:56d9f2ecac662ca1611d183feb03a3fa4406469dafe241673d521dd5ae92a155",
-                "sha256:5bbe06f8eeafd38e5d0a4894ffec89378b6c6a625ff57e3028921f8ff59318ac",
-                "sha256:65c1a9bcdadc6c28eecee2c119465aebff8f7a584dd719facdd9e825ec61ab52",
-                "sha256:68e78619a61ecf91e76aa3e6e8e33fc4894a2bebe93410754bd28fce0a8a4f9f",
-                "sha256:69c0f17e9f5a7afdf2cc9fb2d1ce6aabdb3bafb7f38017c0b77862bcec2bbad8",
-                "sha256:6b2b56950d93e41f33b4223ead100ea0fe11f8e6ee5f641eb753ce4b77a7042b",
-                "sha256:715d3562f79d540f251b99ebd6d8baa547118974341db04f5ad06d5ea3eb8007",
-                "sha256:787003c0ddb00500e49a10f2844fac87aa6ce977b90b0feaaf9de23c22508b24",
-                "sha256:7ef3cb2ebbf91e330e3bb937efada0edd9003683db6b57bb108c4001f37a02ea",
-                "sha256:8023faf4e01efadfa183e863fefde0046de576c6f14659e8782065bcece22198",
-                "sha256:8758846a7e80910096950b67071243da3e5a20ed2546e6392603c096778d48e0",
-                "sha256:8afafd99945ead6e075b973fefa56379c5b5c53fd8937dad92c662da5d8fd5ee",
-                "sha256:8c41976a29d078bb235fea9b2ecd3da465df42a562910f9022f1a03107bd02be",
-                "sha256:8e254ae696c88d98da6555f5ace2279cf7cd5b3f52be2b5cf97feafe883b58d2",
-                "sha256:8f9293864fe09b8149f0cc42ce56e3f0e54de883a9de90cd427f191c346eb2e1",
-                "sha256:9402b03f1a1b4dc4c19845e5c749e3ab82d5078d16a2a4c2cd2df62d57bb0707",
-                "sha256:962f82a3086483f5e5f64dbad880d31038b698494799b097bc59c2edf392fce6",
-                "sha256:9aad3c1755095ce347e26488214ef77e0485a3c34a50c5a5e2471dff60b9dd9c",
-                "sha256:9dcdfd0eaf283af041973bff14a2e143b8bd64e069f4c383416ecd79a81aab58",
-                "sha256:aa57bd9cf8ae831a362185ee444e15a93ecb2e344c8e52e4d721ea3ab6ef1823",
-                "sha256:aa7bd130efab1c280bed0f45501b7c8795f9fdbeb02e965371bbef3523627779",
-                "sha256:ab4a0df41e7c16a1392727727e7998a467472d0ad65f3ad5e6e765015df08636",
-                "sha256:ad9e82fb8f09ade1c3e1b996a6337afac2b8b9e365f926f5a61aacc71adc5b3c",
-                "sha256:af598ed32d6ae86f1b747b82783958b1a4ab8f617b06fe68795c7f026abbdcad",
-                "sha256:b076b6226fb84157e3f7c971a47ff3a679d837cf338547532ab866c57930dbee",
-                "sha256:b7ff0f54cb4ff66dd38bebd335a38e2c22c41a8ee45aa608efc890ac3e3931bc",
-                "sha256:bfce63a9e7834b12b87c64d6b155fdd9b3b96191b6bd334bf37db7ff1fe457f2",
-                "sha256:c011a4149cfbcf9f03994ec2edffcb8b1dc2d2aede7ca243746df97a5d41ce48",
-                "sha256:c9c804664ebe8f83a211cace637506669e7890fec1b4195b505c214e50dd4eb7",
-                "sha256:ca379055a47383d02a5400cb0d110cef0a776fc644cda797db0c5696cfd7e18e",
-                "sha256:cb0932dc158471523c9637e807d9bfb93e06a95cbf010f1a38b98623b929ef2b",
-                "sha256:cd0f502fe016460680cd20aaa5a76d241d6f35a1c3350c474bac1273803893fa",
-                "sha256:ceb01949af7121f9fc39f7d27f91be8546f3fb112c608bc4029aef0bab86a2a5",
-                "sha256:d080e0a5eb2529460b30190fcfcc4199bd7f827663f858a226a81bc27beaa97e",
-                "sha256:dd15ff04ffd7e05ffcb7fe79f1b98041b8ea30ae9234aed2a9168b5797c3effb",
-                "sha256:df0be2b576a7abbf737b1575f048c23fb1d769f267ec4358296f31c2479db8f9",
-                "sha256:e09031c87a1e51556fdcb46e5bd4f59dfb743061cf93c4d6831bf894f125eb57",
-                "sha256:e4dd52d80b8c83fdce44e12478ad2e85c64ea965e75d66dbeafb0a3e77308fcc",
-                "sha256:f698de3fd0c4e6972b92290a45bd9b1536bffe8c6759c62471efaa8acb4c37bc",
-                "sha256:fec21693218efe39aa7f8599346e90c705afa52c5b31ae019b2e57e8f6542bb2",
-                "sha256:ffcc3f7c66b5f5b7931a5aa68fc9cecc51e685ef90282f4a82f0f5e9b704ad11"
+                "sha256:00e046b6dd71aa03a41079792f8473dc494d564611a8f89bbbd7cb93295ebdcf",
+                "sha256:075202fa5b72c86ad32dc7d0b56024ebdbcf2048c0ba09f1cde31bfdd57bcfff",
+                "sha256:0e397ac966fdf721b2c528cf028494e86172b4feba51d65f81ffd65c63798f3f",
+                "sha256:17b950fccb810b3293638215058e432159d2b71005c74371d784862b7e4683f3",
+                "sha256:1f3fbcb7ef1f16e48246f704ab79d79da8a46891e2da03f8783a5b6fa41a9532",
+                "sha256:2174c595a0d73a3080ca3257b40096db99799265e1c27cc5a610743acd86d62f",
+                "sha256:2b7c57a4dfc4f16f7142221afe5ba4e093e09e728ca65c51f5620c9aaeb9a617",
+                "sha256:2d2d793e36e230fd32babe143b04cec8a8b3eb8a3122d2aceb4a371e6b09b8df",
+                "sha256:30b600cf0a7ac9234b2638fbc0fb6158ba5bdcdf46aeb631ead21248b9affbc4",
+                "sha256:397081c1a0bfb5124355710fe79478cdbeb39626492b15d399526ae53422b906",
+                "sha256:3a57fdd7ce31c7ff06cdfbf31dafa96cc533c21e443d57f5b1ecc6cdc668ec7f",
+                "sha256:3c6b973f22eb18a789b1460b4b91bf04ae3f0c4234a0a6aa6b0a92f6f7b951d4",
+                "sha256:3e53af139f8579a6d5f7b76549125f0d94d7e630761a2111bc431fd820e163b8",
+                "sha256:4096e9de5c6fdf43fb4f04c26fb114f61ef0bf2e5604b6ee3019d51b69e8c371",
+                "sha256:4275d846e41ecefa46e2015117a9f491e57a71ddd59bbead77e904dc02b1bed2",
+                "sha256:4c31f53cdae6ecfa91a77820e8b151dba54ab528ba65dfd235c80b086d68a465",
+                "sha256:4f11aa001c540f62c6166c7726f71f7573b52c68c31f014c25cc7901deea0b52",
+                "sha256:5049256f536511ee3f7e1b3f87d1d1209d327e818e6ae1365e8653d7e3abb6a6",
+                "sha256:58c98fee265677f63a4385256a6d7683ab1832f3ddd1e66fe948d5880c21a169",
+                "sha256:598e3276b64aff0e7b3451b72e94fa3c238d452e7ddcd893c3ab324717456bad",
+                "sha256:5b7b716f97b52c5a14bffdf688f971b2d5ef4029127f1ad7a513973cfd818df2",
+                "sha256:5dedb4db619ba5a2787a94d877bc8ffc0566f92a01c0ef214865e54ecc9ee5e0",
+                "sha256:619bc166c4f2de5caa5a633b8b7326fbe98e0ccbfacabd87268a2b15ff73a029",
+                "sha256:629ddd2ca402ae6dbedfceeba9c46d5f7b2a61d9749597d4307f943ef198fc1f",
+                "sha256:656f7526c69fac7f600bd1f400991cc282b417d17539a1b228617081106feb4a",
+                "sha256:6ec585f69cec0aa07d945b20805be741395e28ac1627333b1c5b0105962ffced",
+                "sha256:72b6be590cc35924b02c78ef34b467da4ba07e4e0f0454a2c5907f473fc50ce5",
+                "sha256:7502934a33b54030eaf1194c21c692a534196063db72176b0c4028e140f8f32c",
+                "sha256:7a68b554d356a91cce1236aa7682dc01df0edba8d043fd1ce607c49dd3c1edcf",
+                "sha256:7b2e5a267c855eea6b4283940daa6e88a285f5f2a67f2220203786dfa59b37e9",
+                "sha256:823b65d8706e32ad2df51ed89496147a42a2a6e01c13cfb6ffb8b1e92bc910bb",
+                "sha256:8590b4ae07a35970728874632fed7bd57b26b0102df2d2b233b6d9d82f6c62ad",
+                "sha256:8dd717634f5a044f860435c1d8c16a270ddf0ef8588d4887037c5028b859b0c3",
+                "sha256:8dec4936e9c3100156f8a2dc89c4b88d5c435175ff03413b443469c7c8c5f4d1",
+                "sha256:97cafb1f3cbcd3fd2b6fbfb99ae11cdb14deea0736fc2b0952ee177f2b813a46",
+                "sha256:a17a92de5231666cfbe003f0e4b9b3a7ae3afb1ec2845aadc2bacc93ff85febc",
+                "sha256:a549b9c31bec33820e885335b451286e2969a2d9e24879f83fe904a5ce59d70a",
+                "sha256:ac07bad82163452a6884fe8fa0963fb98c2346ba78d779ec06bd7a6262132aee",
+                "sha256:ae2ad8ae6ebee9d2d94b17fb62763125f3f374c25618198f40cbb8b525411900",
+                "sha256:b91c037585eba9095565a3556f611e3cbfaa42ca1e865f7b8015fe5c7336d5a5",
+                "sha256:bc1667f8b83f48511b94671e0e441401371dfd0f0a795c7daa4a3cd1dde55bea",
+                "sha256:bec0a414d016ac1a18862a519e54b2fd0fc8bbfd6890376898a6c0891dd82e9f",
+                "sha256:bf50cd79a75d181c9181df03572cdce0fbb75cc353bc350712073108cba98de5",
+                "sha256:bff1b4290a66b490a2f4719358c0cdcd9bafb6b8f061e45c7a2460866bf50c2e",
+                "sha256:c061bb86a71b42465156a3ee7bd58c8c2ceacdbeb95d05a99893e08b8467359a",
+                "sha256:c8b29db45f8fe46ad280a7294f5c3ec36dbac9491f2d1c17345be8e69cc5928f",
+                "sha256:ce409136744f6521e39fd8e2a24c53fa18ad67aa5bc7c2cf83645cce5b5c4e50",
+                "sha256:d050b3361367a06d752db6ead6e7edeb0009be66bc3bae0ee9d97fb326badc2a",
+                "sha256:d283d37a890ba4c1ae73ffadf8046435c76e7bc2247bbb63c00bd1a709c6544b",
+                "sha256:d9fad5155d72433c921b782e58892377c44bd6252b5af2f67f16b194987338a4",
+                "sha256:daa4ee5a243f0f20d528d939d06670a298dd39b1ad5f8a72a4275124a7819eff",
+                "sha256:db0b55e0f3cc0be60c1f19efdde9a637c32740486004f20d1cff53c3c0ece4d2",
+                "sha256:e61659ba32cf2cf1481e575d0462554625196a1f2fc06a1c777d3f48e8865d46",
+                "sha256:ea3d8a3d18833cf4304cd2fc9cbb1efe188ca9b5efef2bdac7adc20594a0e46b",
+                "sha256:ec6a563cff360b50eed26f13adc43e61bc0c04d94b8be985e6fb24b81f6dcfdf",
+                "sha256:f5dfb42c4604dddc8e4305050aa6deb084540643ed5804d7455b5df8fe16f5e5",
+                "sha256:fa173ec60341d6bb97a89f5ea19c85c5643c1e7dedebc22f5181eb73573142c5",
+                "sha256:fa9db3f79de01457b03d4f01b34cf91bc0048eb2c3846ff26f66687c2f6d16ab",
+                "sha256:fce659a462a1be54d2ffcacea5e3ba2d74daa74f30f5f143fe0c58636e355fdd",
+                "sha256:ffee1f21e5ef0d712f9033568f8344d5da8cc2869dbd08d87c84656e6a2d2f68"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.1.3"
+            "version": "==2.1.5"
         },
         "mergedeep": {
             "hashes": [
                 "sha256:0096d52e9dad9939c3d975a774666af186eda617e6ca84df4c94dec30004f2a8",
                 "sha256:70775750742b25c0d8f36c55aed03d24c3384d17c951b3175d898bd778ef0307"
             ],
             "markers": "python_version >= '3.6'",
@@ -265,43 +265,43 @@
             ],
             "index": "pypi",
             "markers": "python_version >= '3.7'",
             "version": "==1.5.3"
         },
         "packaging": {
             "hashes": [
-                "sha256:048fb0e9405036518eaaf48a55953c750c11e1a1b68e0dd1a9d62ed0c092cfc5",
-                "sha256:8c491190033a9af7e1d931d0b5dacc2ef47509b34dd0de67ed209b5203fc88c7"
+                "sha256:2ddfb553fdf02fb784c234c7ba6ccc288296ceabec964ad2eae3777778130bc5",
+                "sha256:eb82c5e3e56209074766e6885bb04b8c38a0c015d0a30036ebe7ece34c9989e9"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==23.2"
+            "version": "==24.0"
         },
         "pathspec": {
             "hashes": [
                 "sha256:a0d503e138a4c123b27490a4f7beda6a01c6f288df0e4a8b79c7eb0dc7b4cc08",
                 "sha256:a482d51503a1ab33b1c67a6c3813a26953dbdc71c31dacaef9a838c4e29f5712"
             ],
             "markers": "python_version >= '3.8'",
             "version": "==0.12.1"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:11c8f37bcca40db96d8144522d925583bdb7a31f7b0e37e3ed4318400a8e2380",
-                "sha256:906d548203468492d432bcb294d4bc2fff751bf84971fbb2c10918cc206ee420"
+                "sha256:0614df2a2f37e1a662acbd8e2b25b92ccf8632929bc6d43467e17fe89c75e068",
+                "sha256:ef0cc731df711022c174543cb70a9b5bd22e5a9337c8624ef2c2ceb8ddad8768"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==4.1.0"
+            "version": "==4.2.0"
         },
         "python-dateutil": {
             "hashes": [
-                "sha256:0123cacc1627ae19ddf3c27a5de5bd67ee4586fbdd6440d9748f8abb483d3e86",
-                "sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9"
+                "sha256:37dd54208da7e1cd875388217d5e00ebd4179249f90fb72437e91a35459a0ad3",
+                "sha256:a8b2bc7bffae282281c8140a97d3aa9c14da0b136dfe83f850eea9a5f7470427"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==2.8.2"
+            "version": "==2.9.0.post0"
         },
         "pyyaml": {
             "hashes": [
                 "sha256:04ac92ad1925b2cff1db0cfebffb6ffc43457495c9b3c39d3fcae417d7125dc5",
                 "sha256:062582fca9fabdd2c8b54a3ef1c978d786e0f6b3a1510e0ac93ef59e0ddae2bc",
                 "sha256:0d3304d8c0adc42be59c5f8a4d9e3d7379e6955ad754aa9d6ab7a398b59dd1df",
                 "sha256:1635fd110e8d85d55237ab316b5b011de701ea0f29d07611174a1b42f1444741",
@@ -326,14 +326,15 @@
                 "sha256:704219a11b772aea0d8ecd7058d0082713c3562b4e271b849ad7dc4a5c90c13c",
                 "sha256:7e07cbde391ba96ab58e532ff4803f79c4129397514e1413a7dc761ccd755735",
                 "sha256:81e0b275a9ecc9c0c0c07b4b90ba548307583c125f54d5b6946cfee6360c733d",
                 "sha256:855fb52b0dc35af121542a76b9a84f8d1cd886ea97c84703eaa6d88e37a2ad28",
                 "sha256:8d4e9c88387b0f5c7d5f281e55304de64cf7f9c0021a3525bd3b1c542da3b0e4",
                 "sha256:9046c58c4395dff28dd494285c82ba00b546adfc7ef001486fbf0324bc174fba",
                 "sha256:9eb6caa9a297fc2c2fb8862bc5370d0303ddba53ba97e71f08023b6cd73d16a8",
+                "sha256:a08c6f0fe150303c1c6b71ebcd7213c2858041a7e01975da3a99aed1e7a378ef",
                 "sha256:a0cd17c15d3bb3fa06978b4e8958dcdc6e0174ccea823003a106c7d4d7899ac5",
                 "sha256:afd7e57eddb1a54f0f1a974bc4391af8bcce0b444685d936840f125cf046d5bd",
                 "sha256:b1275ad35a5d18c62a7220633c913e1b42d44b46ee12554e5fd39c70a243d6a3",
                 "sha256:b786eecbdf8499b9ca1d697215862083bd6d2a99965554781d0d8d1ad31e13a0",
                 "sha256:ba336e390cd8e4d1739f42dfe9bb83a3cc2e80f567d8805e11b46f4a943f5515",
                 "sha256:baa90d3f661d43131ca170712d903e6295d1f7a0f595074f151c0aed377c9b9c",
                 "sha256:bc1bf2925a1ecd43da378f4db9e4f799775d6367bdb94671027b73b393a7c42c",
@@ -386,52 +387,54 @@
                 "sha256:f463434305e0336248cac9c2dc8076b707d8a12d019dd349f5c1e382dd1ae1b9"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==1.0.0"
         },
         "urllib3": {
             "hashes": [
-                "sha256:55901e917a5896a349ff771be919f8bd99aff50b79fe58fec595eb37bbc56bb3",
-                "sha256:df7aa8afb0148fa78488e7899b2c59b5f4ffcfa82e6c54ccb9dd37c1d7b52d54"
+                "sha256:450b20ec296a467077128bff42b73080516e71b56ff59a60a02bef2232c4fa9d",
+                "sha256:d0570876c61ab9e520d776c38acbbb5b05a776d3f9ff98a5c8fd5162a444cf19"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==2.1.0"
+            "version": "==2.2.1"
         },
         "watchdog": {
             "hashes": [
-                "sha256:0e06ab8858a76e1219e68c7573dfeba9dd1c0219476c5a44d5333b01d7e1743a",
-                "sha256:13bbbb462ee42ec3c5723e1205be8ced776f05b100e4737518c67c8325cf6100",
-                "sha256:233b5817932685d39a7896b1090353fc8efc1ef99c9c054e46c8002561252fb8",
-                "sha256:25f70b4aa53bd743729c7475d7ec41093a580528b100e9a8c5b5efe8899592fc",
-                "sha256:2b57a1e730af3156d13b7fdddfc23dea6487fceca29fc75c5a868beed29177ae",
-                "sha256:336adfc6f5cc4e037d52db31194f7581ff744b67382eb6021c868322e32eef41",
-                "sha256:3aa7f6a12e831ddfe78cdd4f8996af9cf334fd6346531b16cec61c3b3c0d8da0",
-                "sha256:3ed7c71a9dccfe838c2f0b6314ed0d9b22e77d268c67e015450a29036a81f60f",
-                "sha256:4c9956d27be0bb08fc5f30d9d0179a855436e655f046d288e2bcc11adfae893c",
-                "sha256:4d98a320595da7a7c5a18fc48cb633c2e73cda78f93cac2ef42d42bf609a33f9",
-                "sha256:4f94069eb16657d2c6faada4624c39464f65c05606af50bb7902e036e3219be3",
-                "sha256:5113334cf8cf0ac8cd45e1f8309a603291b614191c9add34d33075727a967709",
-                "sha256:51f90f73b4697bac9c9a78394c3acbbd331ccd3655c11be1a15ae6fe289a8c83",
-                "sha256:5d9f3a10e02d7371cd929b5d8f11e87d4bad890212ed3901f9b4d68767bee759",
-                "sha256:7ade88d0d778b1b222adebcc0927428f883db07017618a5e684fd03b83342bd9",
-                "sha256:7c5f84b5194c24dd573fa6472685b2a27cc5a17fe5f7b6fd40345378ca6812e3",
-                "sha256:7e447d172af52ad204d19982739aa2346245cc5ba6f579d16dac4bfec226d2e7",
-                "sha256:8ae9cda41fa114e28faf86cb137d751a17ffd0316d1c34ccf2235e8a84365c7f",
-                "sha256:8f3ceecd20d71067c7fd4c9e832d4e22584318983cabc013dbf3f70ea95de346",
-                "sha256:9fac43a7466eb73e64a9940ac9ed6369baa39b3bf221ae23493a9ec4d0022674",
-                "sha256:a70a8dcde91be523c35b2bf96196edc5730edb347e374c7de7cd20c43ed95397",
-                "sha256:adfdeab2da79ea2f76f87eb42a3ab1966a5313e5a69a0213a3cc06ef692b0e96",
-                "sha256:ba07e92756c97e3aca0912b5cbc4e5ad802f4557212788e72a72a47ff376950d",
-                "sha256:c07253088265c363d1ddf4b3cdb808d59a0468ecd017770ed716991620b8f77a",
-                "sha256:c9d8c8ec7efb887333cf71e328e39cffbf771d8f8f95d308ea4125bf5f90ba64",
-                "sha256:d00e6be486affb5781468457b21a6cbe848c33ef43f9ea4a73b4882e5f188a44",
-                "sha256:d429c2430c93b7903914e4db9a966c7f2b068dd2ebdd2fa9b9ce094c7d459f33"
+                "sha256:11e12fafb13372e18ca1bbf12d50f593e7280646687463dd47730fd4f4d5d257",
+                "sha256:2895bf0518361a9728773083908801a376743bcc37dfa252b801af8fd281b1ca",
+                "sha256:39cb34b1f1afbf23e9562501673e7146777efe95da24fab5707b88f7fb11649b",
+                "sha256:45cc09cc4c3b43fb10b59ef4d07318d9a3ecdbff03abd2e36e77b6dd9f9a5c85",
+                "sha256:4986db5e8880b0e6b7cd52ba36255d4793bf5cdc95bd6264806c233173b1ec0b",
+                "sha256:5369136a6474678e02426bd984466343924d1df8e2fd94a9b443cb7e3aa20d19",
+                "sha256:557ba04c816d23ce98a06e70af6abaa0485f6d94994ec78a42b05d1c03dcbd50",
+                "sha256:6a4db54edea37d1058b08947c789a2354ee02972ed5d1e0dca9b0b820f4c7f92",
+                "sha256:6a80d5cae8c265842c7419c560b9961561556c4361b297b4c431903f8c33b269",
+                "sha256:6a9c71a0b02985b4b0b6d14b875a6c86ddea2fdbebd0c9a720a806a8bbffc69f",
+                "sha256:6c47bdd680009b11c9ac382163e05ca43baf4127954c5f6d0250e7d772d2b80c",
+                "sha256:6e949a8a94186bced05b6508faa61b7adacc911115664ccb1923b9ad1f1ccf7b",
+                "sha256:73c7a935e62033bd5e8f0da33a4dcb763da2361921a69a5a95aaf6c93aa03a87",
+                "sha256:76ad8484379695f3fe46228962017a7e1337e9acadafed67eb20aabb175df98b",
+                "sha256:8350d4055505412a426b6ad8c521bc7d367d1637a762c70fdd93a3a0d595990b",
+                "sha256:87e9df830022488e235dd601478c15ad73a0389628588ba0b028cb74eb72fed8",
+                "sha256:8f9a542c979df62098ae9c58b19e03ad3df1c9d8c6895d96c0d51da17b243b1c",
+                "sha256:8fec441f5adcf81dd240a5fe78e3d83767999771630b5ddfc5867827a34fa3d3",
+                "sha256:9a03e16e55465177d416699331b0f3564138f1807ecc5f2de9d55d8f188d08c7",
+                "sha256:ba30a896166f0fee83183cec913298151b73164160d965af2e93a20bbd2ab605",
+                "sha256:c17d98799f32e3f55f181f19dd2021d762eb38fdd381b4a748b9f5a36738e935",
+                "sha256:c522392acc5e962bcac3b22b9592493ffd06d1fc5d755954e6be9f4990de932b",
+                "sha256:d0f9bd1fd919134d459d8abf954f63886745f4660ef66480b9d753a7c9d40927",
+                "sha256:d18d7f18a47de6863cd480734613502904611730f8def45fc52a5d97503e5101",
+                "sha256:d31481ccf4694a8416b681544c23bd271f5a123162ab603c7d7d2dd7dd901a07",
+                "sha256:e3e7065cbdabe6183ab82199d7a4f6b3ba0a438c5a512a68559846ccb76a78ec",
+                "sha256:eed82cdf79cd7f0232e2fdc1ad05b06a5e102a43e331f7d041e5f0e0a34a51c4",
+                "sha256:f970663fa4f7e80401a7b0cbeec00fa801bf0287d93d48368fc3e6fa32716245",
+                "sha256:f9b2fdca47dc855516b2d66eef3c39f2672cbf7e7a42e7e67ad2cbfcd6ba107d"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==3.0.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==4.0.0"
         }
     },
     "develop": {
         "babel": {
             "hashes": [
                 "sha256:6919867db036398ba21eb5c7a0f6b28ab8cbc3ae7a73a44ebe34ae74a4e7d363",
                 "sha256:efb1a25b7118e67ce3a259bed20545c29cb68be8ad2c784c83689981b7a57287"
@@ -445,19 +448,19 @@
                 "sha256:efdc71eff95eaff5e0f8cfebe7d01adf2c8637c8c92edaf63ef348c241a82418"
             ],
             "markers": "python_version >= '3.8'",
             "version": "==2.4"
         },
         "certifi": {
             "hashes": [
-                "sha256:9b469f3a900bf28dc19b8cfbf8019bf47f7fdd1a65a1d4ffb98fc14166beb4d1",
-                "sha256:e036ab49d5b79556f99cfc2d9320b34cfbe5be05c5871b51de9329f0603b0474"
+                "sha256:0569859f95fc761b18b45ef421b1290a0f65f147e92a1e5eb3e635f9a5e4e66f",
+                "sha256:dc383c07b76109f368f6106eee2b593b04a011ea4d55f652c6ca24a754d1cdd1"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==2023.11.17"
+            "version": "==2024.2.2"
         },
         "cfgv": {
             "hashes": [
                 "sha256:b7265b1f29fd3316bfcd2b330d63d024f2bfd8bcb8b0272f8e19a504856c48f9",
                 "sha256:e52591d4c5f5dead8e0f673fb16db7949d2cfb3f7da4582893288f0ded8fe560"
             ],
             "markers": "python_version >= '3.8'",
@@ -576,111 +579,111 @@
             "version": "==0.4.6"
         },
         "coverage": {
             "extras": [
                 "toml"
             ],
             "hashes": [
-                "sha256:04387a4a6ecb330c1878907ce0dc04078ea72a869263e53c72a1ba5bbdf380ca",
-                "sha256:0676cd0ba581e514b7f726495ea75aba3eb20899d824636c6f59b0ed2f88c471",
-                "sha256:0e8d06778e8fbffccfe96331a3946237f87b1e1d359d7fbe8b06b96c95a5407a",
-                "sha256:0eb3c2f32dabe3a4aaf6441dde94f35687224dfd7eb2a7f47f3fd9428e421058",
-                "sha256:109f5985182b6b81fe33323ab4707011875198c41964f014579cf82cebf2bb85",
-                "sha256:13eaf476ec3e883fe3e5fe3707caeb88268a06284484a3daf8250259ef1ba143",
-                "sha256:164fdcc3246c69a6526a59b744b62e303039a81e42cfbbdc171c91a8cc2f9446",
-                "sha256:26776ff6c711d9d835557ee453082025d871e30b3fd6c27fcef14733f67f0590",
-                "sha256:26f66da8695719ccf90e794ed567a1549bb2644a706b41e9f6eae6816b398c4a",
-                "sha256:29f3abe810930311c0b5d1a7140f6395369c3db1be68345638c33eec07535105",
-                "sha256:316543f71025a6565677d84bc4df2114e9b6a615aa39fb165d697dba06a54af9",
-                "sha256:36b0ea8ab20d6a7564e89cb6135920bc9188fb5f1f7152e94e8300b7b189441a",
-                "sha256:3cc9d4bc55de8003663ec94c2f215d12d42ceea128da8f0f4036235a119c88ac",
-                "sha256:485e9f897cf4856a65a57c7f6ea3dc0d4e6c076c87311d4bc003f82cfe199d25",
-                "sha256:5040148f4ec43644702e7b16ca864c5314ccb8ee0751ef617d49aa0e2d6bf4f2",
-                "sha256:51456e6fa099a8d9d91497202d9563a320513fcf59f33991b0661a4a6f2ad450",
-                "sha256:53d7d9158ee03956e0eadac38dfa1ec8068431ef8058fe6447043db1fb40d932",
-                "sha256:5a10a4920def78bbfff4eff8a05c51be03e42f1c3735be42d851f199144897ba",
-                "sha256:5b14b4f8760006bfdb6e08667af7bc2d8d9bfdb648351915315ea17645347137",
-                "sha256:5b2ccb7548a0b65974860a78c9ffe1173cfb5877460e5a229238d985565574ae",
-                "sha256:697d1317e5290a313ef0d369650cfee1a114abb6021fa239ca12b4849ebbd614",
-                "sha256:6ae8c9d301207e6856865867d762a4b6fd379c714fcc0607a84b92ee63feff70",
-                "sha256:707c0f58cb1712b8809ece32b68996ee1e609f71bd14615bd8f87a1293cb610e",
-                "sha256:74775198b702868ec2d058cb92720a3c5a9177296f75bd97317c787daf711505",
-                "sha256:756ded44f47f330666843b5781be126ab57bb57c22adbb07d83f6b519783b870",
-                "sha256:76f03940f9973bfaee8cfba70ac991825611b9aac047e5c80d499a44079ec0bc",
-                "sha256:79287fd95585ed36e83182794a57a46aeae0b64ca53929d1176db56aacc83451",
-                "sha256:799c8f873794a08cdf216aa5d0531c6a3747793b70c53f70e98259720a6fe2d7",
-                "sha256:7d360587e64d006402b7116623cebf9d48893329ef035278969fa3bbf75b697e",
-                "sha256:80b5ee39b7f0131ebec7968baa9b2309eddb35b8403d1869e08f024efd883566",
-                "sha256:815ac2d0f3398a14286dc2cea223a6f338109f9ecf39a71160cd1628786bc6f5",
-                "sha256:83c2dda2666fe32332f8e87481eed056c8b4d163fe18ecc690b02802d36a4d26",
-                "sha256:846f52f46e212affb5bcf131c952fb4075b55aae6b61adc9856222df89cbe3e2",
-                "sha256:936d38794044b26c99d3dd004d8af0035ac535b92090f7f2bb5aa9c8e2f5cd42",
-                "sha256:9864463c1c2f9cb3b5db2cf1ff475eed2f0b4285c2aaf4d357b69959941aa555",
-                "sha256:995ea5c48c4ebfd898eacb098164b3cc826ba273b3049e4a889658548e321b43",
-                "sha256:a1526d265743fb49363974b7aa8d5899ff64ee07df47dd8d3e37dcc0818f09ed",
-                "sha256:a56de34db7b7ff77056a37aedded01b2b98b508227d2d0979d373a9b5d353daa",
-                "sha256:a7c97726520f784239f6c62506bc70e48d01ae71e9da128259d61ca5e9788516",
-                "sha256:b8e99f06160602bc64da35158bb76c73522a4010f0649be44a4e167ff8555952",
-                "sha256:bb1de682da0b824411e00a0d4da5a784ec6496b6850fdf8c865c1d68c0e318dd",
-                "sha256:bf477c355274a72435ceb140dc42de0dc1e1e0bf6e97195be30487d8eaaf1a09",
-                "sha256:bf635a52fc1ea401baf88843ae8708591aa4adff875e5c23220de43b1ccf575c",
-                "sha256:bfd5db349d15c08311702611f3dccbef4b4e2ec148fcc636cf8739519b4a5c0f",
-                "sha256:c530833afc4707fe48524a44844493f36d8727f04dcce91fb978c414a8556cc6",
-                "sha256:cc6d65b21c219ec2072c1293c505cf36e4e913a3f936d80028993dd73c7906b1",
-                "sha256:cd3c1e4cb2ff0083758f09be0f77402e1bdf704adb7f89108007300a6da587d0",
-                "sha256:cfd2a8b6b0d8e66e944d47cdec2f47c48fef2ba2f2dff5a9a75757f64172857e",
-                "sha256:d0ca5c71a5a1765a0f8f88022c52b6b8be740e512980362f7fdbb03725a0d6b9",
-                "sha256:e7defbb9737274023e2d7af02cac77043c86ce88a907c58f42b580a97d5bcca9",
-                "sha256:e9d1bf53c4c8de58d22e0e956a79a5b37f754ed1ffdbf1a260d9dcfa2d8a325e",
-                "sha256:ea81d8f9691bb53f4fb4db603203029643caffc82bf998ab5b59ca05560f4c06"
+                "sha256:00838a35b882694afda09f85e469c96367daa3f3f2b097d846a7216993d37f4c",
+                "sha256:0513b9508b93da4e1716744ef6ebc507aff016ba115ffe8ecff744d1322a7b63",
+                "sha256:09c3255458533cb76ef55da8cc49ffab9e33f083739c8bd4f58e79fecfe288f7",
+                "sha256:09ef9199ed6653989ebbcaacc9b62b514bb63ea2f90256e71fea3ed74bd8ff6f",
+                "sha256:09fa497a8ab37784fbb20ab699c246053ac294d13fc7eb40ec007a5043ec91f8",
+                "sha256:0f9f50e7ef2a71e2fae92774c99170eb8304e3fdf9c8c3c7ae9bab3e7229c5cf",
+                "sha256:137eb07173141545e07403cca94ab625cc1cc6bc4c1e97b6e3846270e7e1fea0",
+                "sha256:1f384c3cc76aeedce208643697fb3e8437604b512255de6d18dae3f27655a384",
+                "sha256:201bef2eea65e0e9c56343115ba3814e896afe6d36ffd37bab783261db430f76",
+                "sha256:38dd60d7bf242c4ed5b38e094baf6401faa114fc09e9e6632374388a404f98e7",
+                "sha256:3b799445b9f7ee8bf299cfaed6f5b226c0037b74886a4e11515e569b36fe310d",
+                "sha256:3ea79bb50e805cd6ac058dfa3b5c8f6c040cb87fe83de10845857f5535d1db70",
+                "sha256:40209e141059b9370a2657c9b15607815359ab3ef9918f0196b6fccce8d3230f",
+                "sha256:41c9c5f3de16b903b610d09650e5e27adbfa7f500302718c9ffd1c12cf9d6818",
+                "sha256:54eb8d1bf7cacfbf2a3186019bcf01d11c666bd495ed18717162f7eb1e9dd00b",
+                "sha256:598825b51b81c808cb6f078dcb972f96af96b078faa47af7dfcdf282835baa8d",
+                "sha256:5fc1de20b2d4a061b3df27ab9b7c7111e9a710f10dc2b84d33a4ab25065994ec",
+                "sha256:623512f8ba53c422fcfb2ce68362c97945095b864cda94a92edbaf5994201083",
+                "sha256:690db6517f09336559dc0b5f55342df62370a48f5469fabf502db2c6d1cffcd2",
+                "sha256:69eb372f7e2ece89f14751fbcbe470295d73ed41ecd37ca36ed2eb47512a6ab9",
+                "sha256:73bfb9c09951125d06ee473bed216e2c3742f530fc5acc1383883125de76d9cd",
+                "sha256:742a76a12aa45b44d236815d282b03cfb1de3b4323f3e4ec933acfae08e54ade",
+                "sha256:7c95949560050d04d46b919301826525597f07b33beba6187d04fa64d47ac82e",
+                "sha256:8130a2aa2acb8788e0b56938786c33c7c98562697bf9f4c7d6e8e5e3a0501e4a",
+                "sha256:8a2b2b78c78293782fd3767d53e6474582f62443d0504b1554370bde86cc8227",
+                "sha256:8ce1415194b4a6bd0cdcc3a1dfbf58b63f910dcb7330fe15bdff542c56949f87",
+                "sha256:9ca28a302acb19b6af89e90f33ee3e1906961f94b54ea37de6737b7ca9d8827c",
+                "sha256:a4cdc86d54b5da0df6d3d3a2f0b710949286094c3a6700c21e9015932b81447e",
+                "sha256:aa5b1c1bfc28384f1f53b69a023d789f72b2e0ab1b3787aae16992a7ca21056c",
+                "sha256:aadacf9a2f407a4688d700e4ebab33a7e2e408f2ca04dbf4aef17585389eff3e",
+                "sha256:ae71e7ddb7a413dd60052e90528f2f65270aad4b509563af6d03d53e979feafd",
+                "sha256:b14706df8b2de49869ae03a5ccbc211f4041750cd4a66f698df89d44f4bd30ec",
+                "sha256:b1a93009cb80730c9bca5d6d4665494b725b6e8e157c1cb7f2db5b4b122ea562",
+                "sha256:b2991665420a803495e0b90a79233c1433d6ed77ef282e8e152a324bbbc5e0c8",
+                "sha256:b2c5edc4ac10a7ef6605a966c58929ec6c1bd0917fb8c15cb3363f65aa40e677",
+                "sha256:b4d33f418f46362995f1e9d4f3a35a1b6322cb959c31d88ae56b0298e1c22357",
+                "sha256:b91cbc4b195444e7e258ba27ac33769c41b94967919f10037e6355e998af255c",
+                "sha256:c74880fc64d4958159fbd537a091d2a585448a8f8508bf248d72112723974cbd",
+                "sha256:c901df83d097649e257e803be22592aedfd5182f07b3cc87d640bbb9afd50f49",
+                "sha256:cac99918c7bba15302a2d81f0312c08054a3359eaa1929c7e4b26ebe41e9b286",
+                "sha256:cc4f1358cb0c78edef3ed237ef2c86056206bb8d9140e73b6b89fbcfcbdd40e1",
+                "sha256:ccd341521be3d1b3daeb41960ae94a5e87abe2f46f17224ba5d6f2b8398016cf",
+                "sha256:ce4b94265ca988c3f8e479e741693d143026632672e3ff924f25fab50518dd51",
+                "sha256:cf271892d13e43bc2b51e6908ec9a6a5094a4df1d8af0bfc360088ee6c684409",
+                "sha256:d5ae728ff3b5401cc320d792866987e7e7e880e6ebd24433b70a33b643bb0384",
+                "sha256:d71eec7d83298f1af3326ce0ff1d0ea83c7cb98f72b577097f9083b20bdaf05e",
+                "sha256:d898fe162d26929b5960e4e138651f7427048e72c853607f2b200909794ed978",
+                "sha256:d89d7b2974cae412400e88f35d86af72208e1ede1a541954af5d944a8ba46c57",
+                "sha256:dfa8fe35a0bb90382837b238fff375de15f0dcdb9ae68ff85f7a63649c98527e",
+                "sha256:e0be5efd5127542ef31f165de269f77560d6cdef525fffa446de6f7e9186cfb2",
+                "sha256:fdfafb32984684eb03c2d83e1e51f64f0906b11e64482df3c5db936ce3839d48",
+                "sha256:ff7687ca3d7028d8a5f0ebae95a6e4827c5616b31a4ee1192bdfde697db110d4"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==7.4.0"
+            "version": "==7.4.4"
         },
         "distlib": {
             "hashes": [
                 "sha256:034db59a0b96f8ca18035f36290806a9a6e6bd9d1ff91e45a7f172eb17e51784",
                 "sha256:1530ea13e350031b6312d8580ddb6b27a104275a31106523b8f123787f494f64"
             ],
             "version": "==0.3.8"
         },
         "exceptiongroup": {
             "markers": "python_version < '3.11'"
         },
         "filelock": {
             "hashes": [
-                "sha256:521f5f56c50f8426f5e03ad3b281b490a87ef15bc6c526f168290f0c7148d44e",
-                "sha256:57dbda9b35157b05fb3e58ee91448612eb674172fab98ee235ccb0b5bee19a1c"
+                "sha256:5ffa845303983e7a0b7ae17636509bc97997d58afeafa72fb141a17b152284cb",
+                "sha256:a79895a25bbefdf55d1a2a0a80968f7dbb28edcd6d4234a0afb3f37ecde4b546"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==3.13.1"
+            "version": "==3.13.3"
         },
         "flake8": {
             "hashes": [
-                "sha256:d5b3857f07c030bdb5bf41c7f53799571d75c4491748a3adcd47de929e34cd23",
-                "sha256:ffdfce58ea94c6580c77888a86506937f9a1a227dfcd15f245d694ae20a6b6e5"
+                "sha256:33f96621059e65eec474169085dc92bf26e7b2d47366b70be2f67ab80dc25132",
+                "sha256:a6dfbb75e03252917f2473ea9653f7cd799c3064e54d4c8140044c5c065f53c3"
             ],
             "index": "pypi",
             "markers": "python_full_version >= '3.8.1'",
-            "version": "==6.1.0"
+            "version": "==7.0.0"
         },
         "ghp-import": {
             "hashes": [
                 "sha256:8337dd7b50877f163d4c0289bc1f1c7f127550241988d568c1db512c4324a619",
                 "sha256:9c535c4c61193c2df8871222567d7fd7e5014d835f97dc7b7439069e2413d343"
             ],
             "version": "==2.1.0"
         },
         "identify": {
             "hashes": [
-                "sha256:161558f9fe4559e1557e1bff323e8631f6a0e4837f7497767c1782832f16b62d",
-                "sha256:d40ce5fcd762817627670da8a7d8d8e65f24342d14539c59488dc603bf662e34"
+                "sha256:10a7ca245cfcd756a554a7288159f72ff105ad233c7c4b9c6f0f4d108f5f6791",
+                "sha256:c4de0081837b211594f8e877a6b4fad7ca32bbfc1a9307fdd61c28bfe923f13e"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==2.5.33"
+            "version": "==2.5.35"
         },
         "idna": {
             "hashes": [
                 "sha256:9ecdbbd083b06798ae1e86adcbfe8ab1479cf864e4ee30fe4e46a003d12491ca",
                 "sha256:c05567e9c24a6b9faaa835c4821bad0590fbb9d5779e7caa6e1cc4978e7eb24f"
             ],
             "markers": "python_version >= '3.5'",
@@ -695,93 +698,93 @@
                 "sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.0.0"
         },
         "jinja2": {
             "hashes": [
-                "sha256:31351a702a408a9e7595a8fc6150fc3f43bb6bf7e319770cbc0db9df9437e852",
-                "sha256:6088930bfe239f0e6710546ab9c19c9ef35e29792895fed6e6e31a023a182a61"
+                "sha256:7d6d50dd97d52cbc355597bd845fabfbac3f551e1f99619e39a35ce8c370b5fa",
+                "sha256:ac8bd6544d4bb2c9792bf3a159e80bba8fda7f07e81bc3aed565432d5925ba90"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.1.2"
+            "version": "==3.1.3"
         },
         "markdown": {
             "hashes": [
-                "sha256:5874b47d4ee3f0b14d764324d2c94c03ea66bee56f2d929da9f2508d65e722dc",
-                "sha256:b65d7beb248dc22f2e8a31fb706d93798093c308dc1aba295aedeb9d41a813bd"
+                "sha256:48f276f4d8cfb8ce6527c8f79e2ee29708508bf4d40aa410fbc3b4ee832c850f",
+                "sha256:ed4f41f6daecbeeb96e576ce414c41d2d876daa9a16cb35fa8ed8c2ddfad0224"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==3.5.1"
+            "version": "==3.6"
         },
         "markupsafe": {
             "hashes": [
-                "sha256:05fb21170423db021895e1ea1e1f3ab3adb85d1c2333cbc2310f2a26bc77272e",
-                "sha256:0a4e4a1aff6c7ac4cd55792abf96c915634c2b97e3cc1c7129578aa68ebd754e",
-                "sha256:10bbfe99883db80bdbaff2dcf681dfc6533a614f700da1287707e8a5d78a8431",
-                "sha256:134da1eca9ec0ae528110ccc9e48041e0828d79f24121a1a146161103c76e686",
-                "sha256:14ff806850827afd6b07a5f32bd917fb7f45b046ba40c57abdb636674a8b559c",
-                "sha256:1577735524cdad32f9f694208aa75e422adba74f1baee7551620e43a3141f559",
-                "sha256:1b40069d487e7edb2676d3fbdb2b0829ffa2cd63a2ec26c4938b2d34391b4ecc",
-                "sha256:1b8dd8c3fd14349433c79fa8abeb573a55fc0fdd769133baac1f5e07abf54aeb",
-                "sha256:1f67c7038d560d92149c060157d623c542173016c4babc0c1913cca0564b9939",
-                "sha256:282c2cb35b5b673bbcadb33a585408104df04f14b2d9b01d4c345a3b92861c2c",
-                "sha256:2c1b19b3aaacc6e57b7e25710ff571c24d6c3613a45e905b1fde04d691b98ee0",
-                "sha256:2ef12179d3a291be237280175b542c07a36e7f60718296278d8593d21ca937d4",
-                "sha256:338ae27d6b8745585f87218a3f23f1512dbf52c26c28e322dbe54bcede54ccb9",
-                "sha256:3c0fae6c3be832a0a0473ac912810b2877c8cb9d76ca48de1ed31e1c68386575",
-                "sha256:3fd4abcb888d15a94f32b75d8fd18ee162ca0c064f35b11134be77050296d6ba",
-                "sha256:42de32b22b6b804f42c5d98be4f7e5e977ecdd9ee9b660fda1a3edf03b11792d",
-                "sha256:47d4f1c5f80fc62fdd7777d0d40a2e9dda0a05883ab11374334f6c4de38adffd",
-                "sha256:504b320cd4b7eff6f968eddf81127112db685e81f7e36e75f9f84f0df46041c3",
-                "sha256:525808b8019e36eb524b8c68acdd63a37e75714eac50e988180b169d64480a00",
-                "sha256:56d9f2ecac662ca1611d183feb03a3fa4406469dafe241673d521dd5ae92a155",
-                "sha256:5bbe06f8eeafd38e5d0a4894ffec89378b6c6a625ff57e3028921f8ff59318ac",
-                "sha256:65c1a9bcdadc6c28eecee2c119465aebff8f7a584dd719facdd9e825ec61ab52",
-                "sha256:68e78619a61ecf91e76aa3e6e8e33fc4894a2bebe93410754bd28fce0a8a4f9f",
-                "sha256:69c0f17e9f5a7afdf2cc9fb2d1ce6aabdb3bafb7f38017c0b77862bcec2bbad8",
-                "sha256:6b2b56950d93e41f33b4223ead100ea0fe11f8e6ee5f641eb753ce4b77a7042b",
-                "sha256:715d3562f79d540f251b99ebd6d8baa547118974341db04f5ad06d5ea3eb8007",
-                "sha256:787003c0ddb00500e49a10f2844fac87aa6ce977b90b0feaaf9de23c22508b24",
-                "sha256:7ef3cb2ebbf91e330e3bb937efada0edd9003683db6b57bb108c4001f37a02ea",
-                "sha256:8023faf4e01efadfa183e863fefde0046de576c6f14659e8782065bcece22198",
-                "sha256:8758846a7e80910096950b67071243da3e5a20ed2546e6392603c096778d48e0",
-                "sha256:8afafd99945ead6e075b973fefa56379c5b5c53fd8937dad92c662da5d8fd5ee",
-                "sha256:8c41976a29d078bb235fea9b2ecd3da465df42a562910f9022f1a03107bd02be",
-                "sha256:8e254ae696c88d98da6555f5ace2279cf7cd5b3f52be2b5cf97feafe883b58d2",
-                "sha256:8f9293864fe09b8149f0cc42ce56e3f0e54de883a9de90cd427f191c346eb2e1",
-                "sha256:9402b03f1a1b4dc4c19845e5c749e3ab82d5078d16a2a4c2cd2df62d57bb0707",
-                "sha256:962f82a3086483f5e5f64dbad880d31038b698494799b097bc59c2edf392fce6",
-                "sha256:9aad3c1755095ce347e26488214ef77e0485a3c34a50c5a5e2471dff60b9dd9c",
-                "sha256:9dcdfd0eaf283af041973bff14a2e143b8bd64e069f4c383416ecd79a81aab58",
-                "sha256:aa57bd9cf8ae831a362185ee444e15a93ecb2e344c8e52e4d721ea3ab6ef1823",
-                "sha256:aa7bd130efab1c280bed0f45501b7c8795f9fdbeb02e965371bbef3523627779",
-                "sha256:ab4a0df41e7c16a1392727727e7998a467472d0ad65f3ad5e6e765015df08636",
-                "sha256:ad9e82fb8f09ade1c3e1b996a6337afac2b8b9e365f926f5a61aacc71adc5b3c",
-                "sha256:af598ed32d6ae86f1b747b82783958b1a4ab8f617b06fe68795c7f026abbdcad",
-                "sha256:b076b6226fb84157e3f7c971a47ff3a679d837cf338547532ab866c57930dbee",
-                "sha256:b7ff0f54cb4ff66dd38bebd335a38e2c22c41a8ee45aa608efc890ac3e3931bc",
-                "sha256:bfce63a9e7834b12b87c64d6b155fdd9b3b96191b6bd334bf37db7ff1fe457f2",
-                "sha256:c011a4149cfbcf9f03994ec2edffcb8b1dc2d2aede7ca243746df97a5d41ce48",
-                "sha256:c9c804664ebe8f83a211cace637506669e7890fec1b4195b505c214e50dd4eb7",
-                "sha256:ca379055a47383d02a5400cb0d110cef0a776fc644cda797db0c5696cfd7e18e",
-                "sha256:cb0932dc158471523c9637e807d9bfb93e06a95cbf010f1a38b98623b929ef2b",
-                "sha256:cd0f502fe016460680cd20aaa5a76d241d6f35a1c3350c474bac1273803893fa",
-                "sha256:ceb01949af7121f9fc39f7d27f91be8546f3fb112c608bc4029aef0bab86a2a5",
-                "sha256:d080e0a5eb2529460b30190fcfcc4199bd7f827663f858a226a81bc27beaa97e",
-                "sha256:dd15ff04ffd7e05ffcb7fe79f1b98041b8ea30ae9234aed2a9168b5797c3effb",
-                "sha256:df0be2b576a7abbf737b1575f048c23fb1d769f267ec4358296f31c2479db8f9",
-                "sha256:e09031c87a1e51556fdcb46e5bd4f59dfb743061cf93c4d6831bf894f125eb57",
-                "sha256:e4dd52d80b8c83fdce44e12478ad2e85c64ea965e75d66dbeafb0a3e77308fcc",
-                "sha256:f698de3fd0c4e6972b92290a45bd9b1536bffe8c6759c62471efaa8acb4c37bc",
-                "sha256:fec21693218efe39aa7f8599346e90c705afa52c5b31ae019b2e57e8f6542bb2",
-                "sha256:ffcc3f7c66b5f5b7931a5aa68fc9cecc51e685ef90282f4a82f0f5e9b704ad11"
+                "sha256:00e046b6dd71aa03a41079792f8473dc494d564611a8f89bbbd7cb93295ebdcf",
+                "sha256:075202fa5b72c86ad32dc7d0b56024ebdbcf2048c0ba09f1cde31bfdd57bcfff",
+                "sha256:0e397ac966fdf721b2c528cf028494e86172b4feba51d65f81ffd65c63798f3f",
+                "sha256:17b950fccb810b3293638215058e432159d2b71005c74371d784862b7e4683f3",
+                "sha256:1f3fbcb7ef1f16e48246f704ab79d79da8a46891e2da03f8783a5b6fa41a9532",
+                "sha256:2174c595a0d73a3080ca3257b40096db99799265e1c27cc5a610743acd86d62f",
+                "sha256:2b7c57a4dfc4f16f7142221afe5ba4e093e09e728ca65c51f5620c9aaeb9a617",
+                "sha256:2d2d793e36e230fd32babe143b04cec8a8b3eb8a3122d2aceb4a371e6b09b8df",
+                "sha256:30b600cf0a7ac9234b2638fbc0fb6158ba5bdcdf46aeb631ead21248b9affbc4",
+                "sha256:397081c1a0bfb5124355710fe79478cdbeb39626492b15d399526ae53422b906",
+                "sha256:3a57fdd7ce31c7ff06cdfbf31dafa96cc533c21e443d57f5b1ecc6cdc668ec7f",
+                "sha256:3c6b973f22eb18a789b1460b4b91bf04ae3f0c4234a0a6aa6b0a92f6f7b951d4",
+                "sha256:3e53af139f8579a6d5f7b76549125f0d94d7e630761a2111bc431fd820e163b8",
+                "sha256:4096e9de5c6fdf43fb4f04c26fb114f61ef0bf2e5604b6ee3019d51b69e8c371",
+                "sha256:4275d846e41ecefa46e2015117a9f491e57a71ddd59bbead77e904dc02b1bed2",
+                "sha256:4c31f53cdae6ecfa91a77820e8b151dba54ab528ba65dfd235c80b086d68a465",
+                "sha256:4f11aa001c540f62c6166c7726f71f7573b52c68c31f014c25cc7901deea0b52",
+                "sha256:5049256f536511ee3f7e1b3f87d1d1209d327e818e6ae1365e8653d7e3abb6a6",
+                "sha256:58c98fee265677f63a4385256a6d7683ab1832f3ddd1e66fe948d5880c21a169",
+                "sha256:598e3276b64aff0e7b3451b72e94fa3c238d452e7ddcd893c3ab324717456bad",
+                "sha256:5b7b716f97b52c5a14bffdf688f971b2d5ef4029127f1ad7a513973cfd818df2",
+                "sha256:5dedb4db619ba5a2787a94d877bc8ffc0566f92a01c0ef214865e54ecc9ee5e0",
+                "sha256:619bc166c4f2de5caa5a633b8b7326fbe98e0ccbfacabd87268a2b15ff73a029",
+                "sha256:629ddd2ca402ae6dbedfceeba9c46d5f7b2a61d9749597d4307f943ef198fc1f",
+                "sha256:656f7526c69fac7f600bd1f400991cc282b417d17539a1b228617081106feb4a",
+                "sha256:6ec585f69cec0aa07d945b20805be741395e28ac1627333b1c5b0105962ffced",
+                "sha256:72b6be590cc35924b02c78ef34b467da4ba07e4e0f0454a2c5907f473fc50ce5",
+                "sha256:7502934a33b54030eaf1194c21c692a534196063db72176b0c4028e140f8f32c",
+                "sha256:7a68b554d356a91cce1236aa7682dc01df0edba8d043fd1ce607c49dd3c1edcf",
+                "sha256:7b2e5a267c855eea6b4283940daa6e88a285f5f2a67f2220203786dfa59b37e9",
+                "sha256:823b65d8706e32ad2df51ed89496147a42a2a6e01c13cfb6ffb8b1e92bc910bb",
+                "sha256:8590b4ae07a35970728874632fed7bd57b26b0102df2d2b233b6d9d82f6c62ad",
+                "sha256:8dd717634f5a044f860435c1d8c16a270ddf0ef8588d4887037c5028b859b0c3",
+                "sha256:8dec4936e9c3100156f8a2dc89c4b88d5c435175ff03413b443469c7c8c5f4d1",
+                "sha256:97cafb1f3cbcd3fd2b6fbfb99ae11cdb14deea0736fc2b0952ee177f2b813a46",
+                "sha256:a17a92de5231666cfbe003f0e4b9b3a7ae3afb1ec2845aadc2bacc93ff85febc",
+                "sha256:a549b9c31bec33820e885335b451286e2969a2d9e24879f83fe904a5ce59d70a",
+                "sha256:ac07bad82163452a6884fe8fa0963fb98c2346ba78d779ec06bd7a6262132aee",
+                "sha256:ae2ad8ae6ebee9d2d94b17fb62763125f3f374c25618198f40cbb8b525411900",
+                "sha256:b91c037585eba9095565a3556f611e3cbfaa42ca1e865f7b8015fe5c7336d5a5",
+                "sha256:bc1667f8b83f48511b94671e0e441401371dfd0f0a795c7daa4a3cd1dde55bea",
+                "sha256:bec0a414d016ac1a18862a519e54b2fd0fc8bbfd6890376898a6c0891dd82e9f",
+                "sha256:bf50cd79a75d181c9181df03572cdce0fbb75cc353bc350712073108cba98de5",
+                "sha256:bff1b4290a66b490a2f4719358c0cdcd9bafb6b8f061e45c7a2460866bf50c2e",
+                "sha256:c061bb86a71b42465156a3ee7bd58c8c2ceacdbeb95d05a99893e08b8467359a",
+                "sha256:c8b29db45f8fe46ad280a7294f5c3ec36dbac9491f2d1c17345be8e69cc5928f",
+                "sha256:ce409136744f6521e39fd8e2a24c53fa18ad67aa5bc7c2cf83645cce5b5c4e50",
+                "sha256:d050b3361367a06d752db6ead6e7edeb0009be66bc3bae0ee9d97fb326badc2a",
+                "sha256:d283d37a890ba4c1ae73ffadf8046435c76e7bc2247bbb63c00bd1a709c6544b",
+                "sha256:d9fad5155d72433c921b782e58892377c44bd6252b5af2f67f16b194987338a4",
+                "sha256:daa4ee5a243f0f20d528d939d06670a298dd39b1ad5f8a72a4275124a7819eff",
+                "sha256:db0b55e0f3cc0be60c1f19efdde9a637c32740486004f20d1cff53c3c0ece4d2",
+                "sha256:e61659ba32cf2cf1481e575d0462554625196a1f2fc06a1c777d3f48e8865d46",
+                "sha256:ea3d8a3d18833cf4304cd2fc9cbb1efe188ca9b5efef2bdac7adc20594a0e46b",
+                "sha256:ec6a563cff360b50eed26f13adc43e61bc0c04d94b8be985e6fb24b81f6dcfdf",
+                "sha256:f5dfb42c4604dddc8e4305050aa6deb084540643ed5804d7455b5df8fe16f5e5",
+                "sha256:fa173ec60341d6bb97a89f5ea19c85c5643c1e7dedebc22f5181eb73573142c5",
+                "sha256:fa9db3f79de01457b03d4f01b34cf91bc0048eb2c3846ff26f66687c2f6d16ab",
+                "sha256:fce659a462a1be54d2ffcacea5e3ba2d74daa74f30f5f143fe0c58636e355fdd",
+                "sha256:ffee1f21e5ef0d712f9033568f8344d5da8cc2869dbd08d87c84656e6a2d2f68"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.1.3"
+            "version": "==2.1.5"
         },
         "mccabe": {
             "hashes": [
                 "sha256:348e0240c33b60bbdf4e523192ef919f28cb2c3d7d5c7794f74009290f236325",
                 "sha256:6c2d30ab6be0e4a46919781807b4f0d834ebdd6c6e3dca0bda5a15f863427b6e"
             ],
             "markers": "python_version >= '3.6'",
@@ -811,20 +814,20 @@
             ],
             "index": "pypi",
             "markers": "python_version >= '3.7'",
             "version": "==2.9.2"
         },
         "mkdocs-material": {
             "hashes": [
-                "sha256:5899219f422f0a6de784232d9d40374416302ffae3c160cacc72969fcc1ee372",
-                "sha256:76c93a8525cceb0b395b9cedab3428bf518cf6439adef2b940f1c1574b775d89"
+                "sha256:06ae1275a72db1989cf6209de9e9ecdfbcfdbc24c58353877b2bb927dbe413e4",
+                "sha256:14a2a60119a785e70e765dd033e6211367aca9fc70230e577c1cf6a326949571"
             ],
             "index": "pypi",
             "markers": "python_version >= '3.8'",
-            "version": "==9.5.3"
+            "version": "==9.5.17"
         },
         "mkdocs-material-extensions": {
             "hashes": [
                 "sha256:10c9511cea88f568257f960358a467d12b970e1f7b2c0e5fb2bb48cab1928443",
                 "sha256:adff8b62700b25cb77b53358dad940f3ef973dd6db797907c49e3c2ef3ab4e31"
             ],
             "markers": "python_version >= '3.8'",
@@ -844,19 +847,19 @@
                 "sha256:df865724bb3c3adc86b3876fa209771517b0cfe596beff01a92700e0e8be4cec"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6'",
             "version": "==1.8.0"
         },
         "packaging": {
             "hashes": [
-                "sha256:048fb0e9405036518eaaf48a55953c750c11e1a1b68e0dd1a9d62ed0c092cfc5",
-                "sha256:8c491190033a9af7e1d931d0b5dacc2ef47509b34dd0de67ed209b5203fc88c7"
+                "sha256:2ddfb553fdf02fb784c234c7ba6ccc288296ceabec964ad2eae3777778130bc5",
+                "sha256:eb82c5e3e56209074766e6885bb04b8c38a0c015d0a30036ebe7ece34c9989e9"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==23.2"
+            "version": "==24.0"
         },
         "paginate": {
             "hashes": [
                 "sha256:5e6007b6a9398177a7e1648d04fdd9f8c9766a1a945bceac82f1929e8c78af2d"
             ],
             "version": "==0.5.6"
         },
@@ -866,94 +869,94 @@
                 "sha256:a482d51503a1ab33b1c67a6c3813a26953dbdc71c31dacaef9a838c4e29f5712"
             ],
             "markers": "python_version >= '3.8'",
             "version": "==0.12.1"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:11c8f37bcca40db96d8144522d925583bdb7a31f7b0e37e3ed4318400a8e2380",
-                "sha256:906d548203468492d432bcb294d4bc2fff751bf84971fbb2c10918cc206ee420"
+                "sha256:0614df2a2f37e1a662acbd8e2b25b92ccf8632929bc6d43467e17fe89c75e068",
+                "sha256:ef0cc731df711022c174543cb70a9b5bd22e5a9337c8624ef2c2ceb8ddad8768"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==4.1.0"
+            "version": "==4.2.0"
         },
         "pluggy": {
             "hashes": [
-                "sha256:cf61ae8f126ac6f7c451172cf30e3e43d3ca77615509771b3a984a0730651e12",
-                "sha256:d89c696a773f8bd377d18e5ecda92b7a3793cbe66c87060a6fb58c7b6e1061f7"
+                "sha256:7db9f7b503d67d1c5b95f59773ebb58a8c1c288129a88665838012cfb07b8981",
+                "sha256:8c85c2876142a764e5b7548e7d9a0e0ddb46f5185161049a79b7e974454223be"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==1.3.0"
+            "version": "==1.4.0"
         },
         "pre-commit": {
             "hashes": [
-                "sha256:c255039ef399049a5544b6ce13d135caba8f2c28c3b4033277a788f434308376",
-                "sha256:d30bad9abf165f7785c15a21a1f46da7d0677cb00ee7ff4c579fd38922efe15d"
+                "sha256:5eae9e10c2b5ac51577c3452ec0a490455c45a0533f7960f993a0d01e59decab",
+                "sha256:e209d61b8acdcf742404408531f0c37d49d2c734fd7cff2d6076083d191cb060"
             ],
             "index": "pypi",
             "markers": "python_version >= '3.9'",
-            "version": "==3.6.0"
+            "version": "==3.7.0"
         },
         "pycodestyle": {
             "hashes": [
                 "sha256:41ba0e7afc9752dfb53ced5489e89f8186be00e599e712660695b7a75ff2663f",
                 "sha256:44fe31000b2d866f2e41841b18528a505fbd7fef9017b04eff4e2648a0fadc67"
             ],
             "markers": "python_version >= '3.8'",
             "version": "==2.11.1"
         },
         "pyflakes": {
             "hashes": [
-                "sha256:4132f6d49cb4dae6819e5379898f2b8cce3c5f23994194c24b77d5da2e36f774",
-                "sha256:a0aae034c444db0071aa077972ba4768d40c830d9539fd45bf4cd3f8f6992efc"
+                "sha256:1c61603ff154621fb2a9172037d84dca3500def8c8b630657d1701f026f8af3f",
+                "sha256:84b5be138a2dfbb40689ca07e2152deb896a65c3a3e24c251c5c62489568074a"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==3.1.0"
+            "version": "==3.2.0"
         },
         "pygments": {
             "hashes": [
                 "sha256:b27c2826c47d0f3219f29554824c30c5e8945175d888647acd804ddd04af846c",
                 "sha256:da46cec9fd2de5be3a8a784f434e4c4ab670b4ff54d605c4c2717e9d49c4c367"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.17.2"
         },
         "pymdown-extensions": {
             "hashes": [
-                "sha256:6ca215bc57bc12bf32b414887a68b810637d039124ed9b2e5bd3325cbb2c050c",
-                "sha256:c0d64d5cf62566f59e6b2b690a4095c931107c250a8c8e1351c1de5f6b036deb"
+                "sha256:c70e146bdd83c744ffc766b4671999796aba18842b268510a329f7f64700d584",
+                "sha256:f5cc7000d7ff0d1ce9395d216017fa4df3dde800afb1fb72d1c7d3fd35e710f4"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==10.7"
+            "version": "==10.7.1"
         },
         "pytest": {
             "hashes": [
-                "sha256:2cf0005922c6ace4a3e2ec8b4080eb0d9753fdc93107415332f50ce9e7994280",
-                "sha256:b090cdf5ed60bf4c45261be03239c2c1c22df034fbffe691abe93cd80cea01d8"
+                "sha256:2a8386cfc11fa9d2c50ee7b2a57e7d898ef90470a7a34c4b949ff59662bb78b7",
+                "sha256:ac978141a75948948817d360297b7aae0fcb9d6ff6bc9ec6d514b85d5a65c044"
             ],
             "index": "pypi",
-            "markers": "python_version >= '3.7'",
-            "version": "==7.4.4"
+            "markers": "python_version >= '3.8'",
+            "version": "==8.1.1"
         },
         "pytest-cov": {
             "hashes": [
-                "sha256:3904b13dfbfec47f003b8e77fd5b589cd11904a21ddf1ab38a64f204d6a10ef6",
-                "sha256:6ba70b9e97e69fcc3fb45bfeab2d0a138fb65c4d0d6a41ef33983ad114be8c3a"
+                "sha256:4f0764a1219df53214206bf1feea4633c3b558a2925c8b59f144f682861ce652",
+                "sha256:5837b58e9f6ebd335b0f8060eecce69b662415b16dc503883a02f45dfeb14857"
             ],
             "index": "pypi",
-            "markers": "python_version >= '3.7'",
-            "version": "==4.1.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==5.0.0"
         },
         "python-dateutil": {
             "hashes": [
-                "sha256:0123cacc1627ae19ddf3c27a5de5bd67ee4586fbdd6440d9748f8abb483d3e86",
-                "sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9"
+                "sha256:37dd54208da7e1cd875388217d5e00ebd4179249f90fb72437e91a35459a0ad3",
+                "sha256:a8b2bc7bffae282281c8140a97d3aa9c14da0b136dfe83f850eea9a5f7470427"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==2.8.2"
+            "version": "==2.9.0.post0"
         },
         "pyyaml": {
             "hashes": [
                 "sha256:04ac92ad1925b2cff1db0cfebffb6ffc43457495c9b3c39d3fcae417d7125dc5",
                 "sha256:062582fca9fabdd2c8b54a3ef1c978d786e0f6b3a1510e0ac93ef59e0ddae2bc",
                 "sha256:0d3304d8c0adc42be59c5f8a4d9e3d7379e6955ad754aa9d6ab7a398b59dd1df",
                 "sha256:1635fd110e8d85d55237ab316b5b011de701ea0f29d07611174a1b42f1444741",
@@ -978,14 +981,15 @@
                 "sha256:704219a11b772aea0d8ecd7058d0082713c3562b4e271b849ad7dc4a5c90c13c",
                 "sha256:7e07cbde391ba96ab58e532ff4803f79c4129397514e1413a7dc761ccd755735",
                 "sha256:81e0b275a9ecc9c0c0c07b4b90ba548307583c125f54d5b6946cfee6360c733d",
                 "sha256:855fb52b0dc35af121542a76b9a84f8d1cd886ea97c84703eaa6d88e37a2ad28",
                 "sha256:8d4e9c88387b0f5c7d5f281e55304de64cf7f9c0021a3525bd3b1c542da3b0e4",
                 "sha256:9046c58c4395dff28dd494285c82ba00b546adfc7ef001486fbf0324bc174fba",
                 "sha256:9eb6caa9a297fc2c2fb8862bc5370d0303ddba53ba97e71f08023b6cd73d16a8",
+                "sha256:a08c6f0fe150303c1c6b71ebcd7213c2858041a7e01975da3a99aed1e7a378ef",
                 "sha256:a0cd17c15d3bb3fa06978b4e8958dcdc6e0174ccea823003a106c7d4d7899ac5",
                 "sha256:afd7e57eddb1a54f0f1a974bc4391af8bcce0b444685d936840f125cf046d5bd",
                 "sha256:b1275ad35a5d18c62a7220633c913e1b42d44b46ee12554e5fd39c70a243d6a3",
                 "sha256:b786eecbdf8499b9ca1d697215862083bd6d2a99965554781d0d8d1ad31e13a0",
                 "sha256:ba336e390cd8e4d1739f42dfe9bb83a3cc2e80f567d8805e11b46f4a943f5515",
                 "sha256:baa90d3f661d43131ca170712d903e6295d1f7a0f595074f151c0aed377c9b9c",
                 "sha256:bc1bf2925a1ecd43da378f4db9e4f799775d6367bdb94671027b73b393a7c42c",
@@ -1121,86 +1125,88 @@
             ],
             "index": "pypi",
             "markers": "python_version >= '3.7'",
             "version": "==2.31.0"
         },
         "setuptools": {
             "hashes": [
-                "sha256:385eb4edd9c9d5c17540511303e39a147ce2fc04bc55289c322b9e5904fe2c05",
-                "sha256:be1af57fc409f93647f2e8e4573a142ed38724b8cdd389706a867bb4efcf1e78"
+                "sha256:0ff4183f8f42cd8fa3acea16c45205521a4ef28f73c6391d8a25e92893134f2e",
+                "sha256:c21c49fb1042386df081cb5d86759792ab89efca84cf114889191cd09aacc80c"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==69.0.3"
+            "version": "==69.2.0"
         },
         "six": {
             "hashes": [
                 "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926",
                 "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==1.16.0"
         },
         "tomli": {
             "markers": "python_version < '3.11'"
         },
         "urllib3": {
             "hashes": [
-                "sha256:55901e917a5896a349ff771be919f8bd99aff50b79fe58fec595eb37bbc56bb3",
-                "sha256:df7aa8afb0148fa78488e7899b2c59b5f4ffcfa82e6c54ccb9dd37c1d7b52d54"
+                "sha256:450b20ec296a467077128bff42b73080516e71b56ff59a60a02bef2232c4fa9d",
+                "sha256:d0570876c61ab9e520d776c38acbbb5b05a776d3f9ff98a5c8fd5162a444cf19"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==2.1.0"
+            "version": "==2.2.1"
         },
         "virtualenv": {
             "hashes": [
-                "sha256:4238949c5ffe6876362d9c0180fc6c3a824a7b12b80604eeb8085f2ed7460de3",
-                "sha256:bf51c0d9c7dd63ea8e44086fa1e4fb1093a31e963b86959257378aef020e1f1b"
+                "sha256:961c026ac520bac5f69acb8ea063e8a4f071bcc9457b9c1f28f6b085c511583a",
+                "sha256:e08e13ecdca7a0bd53798f356d5831434afa5b07b93f0abdf0797b7a06ffe197"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==20.25.0"
+            "version": "==20.25.1"
         },
         "watchdog": {
             "hashes": [
-                "sha256:0e06ab8858a76e1219e68c7573dfeba9dd1c0219476c5a44d5333b01d7e1743a",
-                "sha256:13bbbb462ee42ec3c5723e1205be8ced776f05b100e4737518c67c8325cf6100",
-                "sha256:233b5817932685d39a7896b1090353fc8efc1ef99c9c054e46c8002561252fb8",
-                "sha256:25f70b4aa53bd743729c7475d7ec41093a580528b100e9a8c5b5efe8899592fc",
-                "sha256:2b57a1e730af3156d13b7fdddfc23dea6487fceca29fc75c5a868beed29177ae",
-                "sha256:336adfc6f5cc4e037d52db31194f7581ff744b67382eb6021c868322e32eef41",
-                "sha256:3aa7f6a12e831ddfe78cdd4f8996af9cf334fd6346531b16cec61c3b3c0d8da0",
-                "sha256:3ed7c71a9dccfe838c2f0b6314ed0d9b22e77d268c67e015450a29036a81f60f",
-                "sha256:4c9956d27be0bb08fc5f30d9d0179a855436e655f046d288e2bcc11adfae893c",
-                "sha256:4d98a320595da7a7c5a18fc48cb633c2e73cda78f93cac2ef42d42bf609a33f9",
-                "sha256:4f94069eb16657d2c6faada4624c39464f65c05606af50bb7902e036e3219be3",
-                "sha256:5113334cf8cf0ac8cd45e1f8309a603291b614191c9add34d33075727a967709",
-                "sha256:51f90f73b4697bac9c9a78394c3acbbd331ccd3655c11be1a15ae6fe289a8c83",
-                "sha256:5d9f3a10e02d7371cd929b5d8f11e87d4bad890212ed3901f9b4d68767bee759",
-                "sha256:7ade88d0d778b1b222adebcc0927428f883db07017618a5e684fd03b83342bd9",
-                "sha256:7c5f84b5194c24dd573fa6472685b2a27cc5a17fe5f7b6fd40345378ca6812e3",
-                "sha256:7e447d172af52ad204d19982739aa2346245cc5ba6f579d16dac4bfec226d2e7",
-                "sha256:8ae9cda41fa114e28faf86cb137d751a17ffd0316d1c34ccf2235e8a84365c7f",
-                "sha256:8f3ceecd20d71067c7fd4c9e832d4e22584318983cabc013dbf3f70ea95de346",
-                "sha256:9fac43a7466eb73e64a9940ac9ed6369baa39b3bf221ae23493a9ec4d0022674",
-                "sha256:a70a8dcde91be523c35b2bf96196edc5730edb347e374c7de7cd20c43ed95397",
-                "sha256:adfdeab2da79ea2f76f87eb42a3ab1966a5313e5a69a0213a3cc06ef692b0e96",
-                "sha256:ba07e92756c97e3aca0912b5cbc4e5ad802f4557212788e72a72a47ff376950d",
-                "sha256:c07253088265c363d1ddf4b3cdb808d59a0468ecd017770ed716991620b8f77a",
-                "sha256:c9d8c8ec7efb887333cf71e328e39cffbf771d8f8f95d308ea4125bf5f90ba64",
-                "sha256:d00e6be486affb5781468457b21a6cbe848c33ef43f9ea4a73b4882e5f188a44",
-                "sha256:d429c2430c93b7903914e4db9a966c7f2b068dd2ebdd2fa9b9ce094c7d459f33"
+                "sha256:11e12fafb13372e18ca1bbf12d50f593e7280646687463dd47730fd4f4d5d257",
+                "sha256:2895bf0518361a9728773083908801a376743bcc37dfa252b801af8fd281b1ca",
+                "sha256:39cb34b1f1afbf23e9562501673e7146777efe95da24fab5707b88f7fb11649b",
+                "sha256:45cc09cc4c3b43fb10b59ef4d07318d9a3ecdbff03abd2e36e77b6dd9f9a5c85",
+                "sha256:4986db5e8880b0e6b7cd52ba36255d4793bf5cdc95bd6264806c233173b1ec0b",
+                "sha256:5369136a6474678e02426bd984466343924d1df8e2fd94a9b443cb7e3aa20d19",
+                "sha256:557ba04c816d23ce98a06e70af6abaa0485f6d94994ec78a42b05d1c03dcbd50",
+                "sha256:6a4db54edea37d1058b08947c789a2354ee02972ed5d1e0dca9b0b820f4c7f92",
+                "sha256:6a80d5cae8c265842c7419c560b9961561556c4361b297b4c431903f8c33b269",
+                "sha256:6a9c71a0b02985b4b0b6d14b875a6c86ddea2fdbebd0c9a720a806a8bbffc69f",
+                "sha256:6c47bdd680009b11c9ac382163e05ca43baf4127954c5f6d0250e7d772d2b80c",
+                "sha256:6e949a8a94186bced05b6508faa61b7adacc911115664ccb1923b9ad1f1ccf7b",
+                "sha256:73c7a935e62033bd5e8f0da33a4dcb763da2361921a69a5a95aaf6c93aa03a87",
+                "sha256:76ad8484379695f3fe46228962017a7e1337e9acadafed67eb20aabb175df98b",
+                "sha256:8350d4055505412a426b6ad8c521bc7d367d1637a762c70fdd93a3a0d595990b",
+                "sha256:87e9df830022488e235dd601478c15ad73a0389628588ba0b028cb74eb72fed8",
+                "sha256:8f9a542c979df62098ae9c58b19e03ad3df1c9d8c6895d96c0d51da17b243b1c",
+                "sha256:8fec441f5adcf81dd240a5fe78e3d83767999771630b5ddfc5867827a34fa3d3",
+                "sha256:9a03e16e55465177d416699331b0f3564138f1807ecc5f2de9d55d8f188d08c7",
+                "sha256:ba30a896166f0fee83183cec913298151b73164160d965af2e93a20bbd2ab605",
+                "sha256:c17d98799f32e3f55f181f19dd2021d762eb38fdd381b4a748b9f5a36738e935",
+                "sha256:c522392acc5e962bcac3b22b9592493ffd06d1fc5d755954e6be9f4990de932b",
+                "sha256:d0f9bd1fd919134d459d8abf954f63886745f4660ef66480b9d753a7c9d40927",
+                "sha256:d18d7f18a47de6863cd480734613502904611730f8def45fc52a5d97503e5101",
+                "sha256:d31481ccf4694a8416b681544c23bd271f5a123162ab603c7d7d2dd7dd901a07",
+                "sha256:e3e7065cbdabe6183ab82199d7a4f6b3ba0a438c5a512a68559846ccb76a78ec",
+                "sha256:eed82cdf79cd7f0232e2fdc1ad05b06a5e102a43e331f7d041e5f0e0a34a51c4",
+                "sha256:f970663fa4f7e80401a7b0cbeec00fa801bf0287d93d48368fc3e6fa32716245",
+                "sha256:f9b2fdca47dc855516b2d66eef3c39f2672cbf7e7a42e7e67ad2cbfcd6ba107d"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==3.0.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==4.0.0"
         },
         "wcmatch": {
             "hashes": [
-                "sha256:14554e409b142edeefab901dc68ad570b30a72a8ab9a79106c5d5e9a6d241bd5",
-                "sha256:86c17572d0f75cbf3bcb1a18f3bf2f9e72b39a9c08c9b4a74e991e1882a8efb3"
+                "sha256:24c19cedc92bc9c9e27f39db4e1824d72f95bd2cea32b254a47a45b1a1b227ed",
+                "sha256:c0088c7f6426cf6bf27e530e2b7b734031905f7e490475fd83c7c5008ab581b3"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==8.5"
+            "version": "==8.5.1"
         },
         "zipp": {
             "markers": "python_version < '3.10'"
         }
     }
 }
```

### Comparing `mkdocs_puml-1.2.4/README.md` & `mkdocs_puml-1.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -32,23 +32,25 @@
 
 ```yaml
 plugins:
     - plantuml:
         puml_url: https://www.plantuml.com/plantuml/
         num_workers: 8
         puml_keyword: puml
+        verify_ssl: true
 ```
 
 Where
 
 | Parmeter | Type                 | Descripton                                                     |
 |----------|----------------------|----------------------------------------------------------------|
 | `puml_url` | `str`. Required      | URL to the plantuml service                                    |
 | `num_workers` | `int`. Default `8`   | Max amount of concurrent workers that request plantuml service |
 | `puml_keyword` | `str`. Default `puml` | The keyword for PlantUML code fence, i.e. \```puml \```        |
+| `verify_ssl` | `bool`. Default `True` | Designates whether `requests` should verify SSL or not |
 
 Now, you can put your puml diagrams into your `.md` documentation. For example,
 
 <pre>
 ## PUML Diagram
 
 ```puml
```

### Comparing `mkdocs_puml-1.2.4/mkdocs_puml/encoder.py` & `mkdocs_puml-1.3.0/mkdocs_puml/encoder.py`

 * *Files identical despite different names*

### Comparing `mkdocs_puml-1.2.4/mkdocs_puml/plugin.py` & `mkdocs_puml-1.3.0/mkdocs_puml/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,22 +27,24 @@
         config_scheme (str): config scheme to set by user in mkdocs.yml file
 
         regex (re.Pattern): regex to find all puml code blocks
         uuid_regex (re.Pattern): regex to find all uuid <pre> blocks
         puml (PlantUML): PlantUML instance that requests PlantUML service
         diagrams (dict): Dictionary containing the diagrams (puml and later svg) and their keys
         puml_keyword (str): keyword used to find PlantUML blocks within Markdown files
+        verify_ssl (bool): Designates whether the ``requests`` should verify SSL certiticate
     """
     div_class_name = "puml"
     pre_class_name = "diagram-uuid"
 
     config_scheme = (
         ('puml_url', Type(str, required=True)),
         ('num_workers', Type(int, default=8)),
-        ('puml_keyword', Type(str, default='puml'))
+        ('puml_keyword', Type(str, default='puml')),
+        ('verify_ssl', Type(bool, default=True))
     )
 
     def __init__(self):
         self.regex: typing.Optional[typing.Any] = None
         self.uuid_regex = re.compile(rf'<pre class="{self.pre_class_name}">(.+?)</pre>', flags=re.DOTALL)
 
         self.puml: typing.Optional[PlantUML] = None
@@ -58,15 +60,19 @@
         Args:
             config: Full mkdocs.yml config file. To access configs of PlantUMLPlugin only,
                     use self.config attribute.
 
         Returns:
             Full config of the mkdocs
         """
-        self.puml = PlantUML(self.config['puml_url'], num_workers=self.config['num_workers'])
+        self.puml = PlantUML(
+            self.config['puml_url'],
+            num_workers=self.config['num_workers'],
+            verify_ssl=self.config['verify_ssl']
+        )
         self.puml_keyword = self.config['puml_keyword']
         self.regex = re.compile(rf"```{self.puml_keyword}(.+?)```", flags=re.DOTALL)
         return config
 
     def on_page_markdown(self, markdown: str, *args, **kwargs) -> str:
         """Event to fire for each .md page.
```

### Comparing `mkdocs_puml-1.2.4/mkdocs_puml/puml.py` & `mkdocs_puml-1.3.0/mkdocs_puml/puml.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,30 +13,32 @@
     """PlantUML converter class.
     It requests PUML service, updates received `svg`
     and returns it to the user.
 
     Attributes:
         base_url (str): Base URL to the PUML service
         num_workers (int): The size of pool to run requests in
+        verify_ssl (bool): Designates whether the ``requests`` should verify SSL certiticate
 
     Examples:
         Use this class as::
 
             puml = PlantUML("https://www.plantuml.com")
             svg = puml.translate([diagram])[0]
     """
     _format = 'svg'
     _html_comment_regex = re.compile(r"<!--.*?-->", flags=re.DOTALL)
 
-    def __init__(self, base_url: str, num_workers: int = 5):
+    def __init__(self, base_url: str, num_workers: int = 5, verify_ssl: bool = True):
         self.base_url = base_url if base_url.endswith('/') else f"{base_url}/"
 
         if num_workers <= 0:
             raise ValueError("`num_workers` argument should be bigger than 0.")
         self.num_workers = num_workers
+        self.verify_ssl = verify_ssl
 
     def translate(self, diagrams: typing.Iterable[str]) -> typing.List[str]:
         """Translate string diagram into HTML div
         block containing the received SVG image.
 
         Examples:
                 This method translates content
@@ -92,15 +94,18 @@
         return SVG content
 
         Args:
             encoded_diagram (str): Encoded string representation of the diagram
         Returns:
             SVG representation of the diagram
         """
-        resp = requests.get(urljoin(self.base_url, f"{self._format}/{encoded_diagram}"))
+        resp = requests.get(
+            urljoin(self.base_url, f"{self._format}/{encoded_diagram}"),
+            verify=self.verify_ssl
+        )
 
         # Use 'ignore' to strip non-utf chars
         return resp.content.decode('utf-8', errors='ignore')
 
     def _clean_comments(self, content: str) -> str:
         return self._html_comment_regex.sub("", content)
```

### Comparing `mkdocs_puml-1.2.4/pyproject.toml` & `mkdocs_puml-1.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mkdocs_puml-1.2.4/tests/conftest.py` & `mkdocs_puml-1.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mkdocs_puml-1.2.4/tests/plugins/conftest.py` & `mkdocs_puml-1.3.0/tests/plugins/conftest.py`

 * *Files identical despite different names*

### Comparing `mkdocs_puml-1.2.4/tests/plugins/test_plugin.py` & `mkdocs_puml-1.3.0/tests/plugins/test_plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs_puml-1.2.4/tests/test_puml.py` & `mkdocs_puml-1.3.0/tests/test_puml.py`

 * *Files identical despite different names*

### Comparing `mkdocs_puml-1.2.4/tests/testdata/markdown.md` & `mkdocs_puml-1.3.0/tests/testdata/markdown.md`

 * *Files identical despite different names*

### Comparing `mkdocs_puml-1.2.4/tests/testdata/plantuml.svg` & `mkdocs_puml-1.3.0/tests/testdata/plantuml.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_puml-1.2.4/PKG-INFO` & `mkdocs_puml-1.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs_puml
-Version: 1.2.4
+Version: 1.3.0
 Summary: Package that brings PlantUML to MkDocs
 Author-email: Mikhail Kravets <michkravets@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: requests >= 2.27, < 3.0
 Requires-Dist: markdown >= 3.2.1, < 4.0
@@ -45,23 +45,25 @@
 
 ```yaml
 plugins:
     - plantuml:
         puml_url: https://www.plantuml.com/plantuml/
         num_workers: 8
         puml_keyword: puml
+        verify_ssl: true
 ```
 
 Where
 
 | Parmeter | Type                 | Descripton                                                     |
 |----------|----------------------|----------------------------------------------------------------|
 | `puml_url` | `str`. Required      | URL to the plantuml service                                    |
 | `num_workers` | `int`. Default `8`   | Max amount of concurrent workers that request plantuml service |
 | `puml_keyword` | `str`. Default `puml` | The keyword for PlantUML code fence, i.e. \```puml \```        |
+| `verify_ssl` | `bool`. Default `True` | Designates whether `requests` should verify SSL or not |
 
 Now, you can put your puml diagrams into your `.md` documentation. For example,
 
 <pre>
 ## PUML Diagram
 
 ```puml
```

