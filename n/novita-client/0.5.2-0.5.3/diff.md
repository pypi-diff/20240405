# Comparing `tmp/novita_client-0.5.2.tar.gz` & `tmp/novita_client-0.5.3.tar.gz`

## Comparing `novita_client-0.5.2.tar` & `novita_client-0.5.3.tar`

### file list

```diff
@@ -1,57 +1,61 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 novita_client-0.5.2/.python-version
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 novita_client-0.5.2/Makefile
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 novita_client-0.5.2/generate-readme.sh
--rw-r--r--   0        0        0    88494 2020-02-02 00:00:00.000000 novita_client-0.5.2/image.jpg
--rw-r--r--   0        0        0    57730 2020-02-02 00:00:00.000000 novita_client-0.5.2/image1.jpg
--rw-r--r--   0        0        0    97725 2020-02-02 00:00:00.000000 novita_client-0.5.2/image2.jpg
--rw-r--r--   0        0        0   696352 2020-02-02 00:00:00.000000 novita_client-0.5.2/img2img-controlnet.png
--rw-r--r--   0        0        0   288795 2020-02-02 00:00:00.000000 novita_client-0.5.2/img2img-logo.png
--rw-r--r--   0        0        0   159522 2020-02-02 00:00:00.000000 novita_client-0.5.2/img2img.png
--rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 novita_client-0.5.2/logo.py
--rw-r--r--   0        0        0   583721 2020-02-02 00:00:00.000000 novita_client-0.5.2/outpainting.png
--rw-r--r--   0        0        0     6617 2020-02-02 00:00:00.000000 novita_client-0.5.2/requirements-dev.lock
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 novita_client-0.5.2/requirements.lock
--rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 novita_client-0.5.2/shanginn.py
--rw-r--r--   0        0        0   348899 2020-02-02 00:00:00.000000 novita_client-0.5.2/test.mp4
--rw-r--r--   0        0        0   711146 2020-02-02 00:00:00.000000 novita_client-0.5.2/txt2img_with_hiresfix.png
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 novita_client-0.5.2/examples/cleanup.py
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 novita_client-0.5.2/examples/controlnet.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 novita_client-0.5.2/examples/create-tile.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 novita_client-0.5.2/examples/doodle.py
--rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 novita_client-0.5.2/examples/img2img.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 novita_client-0.5.2/examples/img2video.py
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 novita_client-0.5.2/examples/instantid.py
--rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 novita_client-0.5.2/examples/latent-consistency-txt2img.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 novita_client-0.5.2/examples/lcm-img2img.py
--rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 novita_client-0.5.2/examples/lcm-vs-txt2img.py
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 novita_client-0.5.2/examples/make-photo.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 novita_client-0.5.2/examples/merge-face.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 novita_client-0.5.2/examples/mixpose.py
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 novita_client-0.5.2/examples/model-search.py
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 novita_client-0.5.2/examples/outpainting.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 novita_client-0.5.2/examples/reimagine.py
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 novita_client-0.5.2/examples/remove-background.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 novita_client-0.5.2/examples/remove-text.py
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 novita_client-0.5.2/examples/replace-background.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 novita_client-0.5.2/examples/replace-object.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 novita_client-0.5.2/examples/replace-sky.py
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 novita_client-0.5.2/examples/txt2img-with-hiresfix.py
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 novita_client-0.5.2/examples/txt2img-with-lora.py
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 novita_client-0.5.2/examples/txt2img-with-refiner.py
--rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 novita_client-0.5.2/examples/fixtures/qrcode.png
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 novita_client-0.5.2/src/novita_client/__init__.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 novita_client-0.5.2/src/novita_client/exceptions.py
--rw-r--r--   0        0        0    44796 2020-02-02 00:00:00.000000 novita_client-0.5.2/src/novita_client/novita.py
--rw-r--r--   0        0        0    36436 2020-02-02 00:00:00.000000 novita_client-0.5.2/src/novita_client/proto.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 novita_client-0.5.2/src/novita_client/serializer.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 novita_client-0.5.2/src/novita_client/settings.py
--rw-r--r--   0        0        0     3609 2020-02-02 00:00:00.000000 novita_client-0.5.2/src/novita_client/utils.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 novita_client-0.5.2/src/novita_client/version.py
--rw-r--r--   0        0        0    12841 2020-02-02 00:00:00.000000 novita_client-0.5.2/tests/test_basics.py
--rw-r--r--   0        0        0     8539 2020-02-02 00:00:00.000000 novita_client-0.5.2/tests/test_enhance.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 novita_client-0.5.2/tests/test_model.py
--rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 novita_client-0.5.2/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 novita_client-0.5.2/LICENSE
--rw-r--r--   0        0        0    22761 2020-02-02 00:00:00.000000 novita_client-0.5.2/README.md
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 novita_client-0.5.2/pyproject.toml
--rw-r--r--   0        0        0    24574 2020-02-02 00:00:00.000000 novita_client-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 novita_client-0.5.3/.python-version
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 novita_client-0.5.3/Makefile
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 novita_client-0.5.3/generate-readme.sh
+-rw-r--r--   0        0        0    88494 2020-02-02 00:00:00.000000 novita_client-0.5.3/image.jpg
+-rw-r--r--   0        0        0   101219 2020-02-02 00:00:00.000000 novita_client-0.5.3/image1 copy.jpg
+-rw-r--r--   0        0        0    35406 2020-02-02 00:00:00.000000 novita_client-0.5.3/image1.jpg
+-rw-r--r--   0        0        0    97725 2020-02-02 00:00:00.000000 novita_client-0.5.3/image2.jpg
+-rw-r--r--   0        0        0   696352 2020-02-02 00:00:00.000000 novita_client-0.5.3/img2img-controlnet.png
+-rw-r--r--   0        0        0   288795 2020-02-02 00:00:00.000000 novita_client-0.5.3/img2img-logo.png
+-rw-r--r--   0        0        0   159522 2020-02-02 00:00:00.000000 novita_client-0.5.3/img2img.png
+-rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 novita_client-0.5.3/logo.py
+-rw-r--r--   0        0        0   583721 2020-02-02 00:00:00.000000 novita_client-0.5.3/outpainting.png
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 novita_client-0.5.3/ow.py
+-rw-r--r--   0        0        0     6617 2020-02-02 00:00:00.000000 novita_client-0.5.3/requirements-dev.lock
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 novita_client-0.5.3/requirements.lock
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 novita_client-0.5.3/shanginn.py
+-rw-r--r--   0        0        0   382237 2020-02-02 00:00:00.000000 novita_client-0.5.3/test.mp4
+-rw-r--r--   0        0        0   314009 2020-02-02 00:00:00.000000 novita_client-0.5.3/test.png
+-rw-r--r--   0        0        0   479432 2020-02-02 00:00:00.000000 novita_client-0.5.3/txt2img-lora-compare.png
+-rw-r--r--   0        0        0   711146 2020-02-02 00:00:00.000000 novita_client-0.5.3/txt2img_with_hiresfix.png
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 novita_client-0.5.3/examples/cleanup.py
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 novita_client-0.5.3/examples/controlnet.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 novita_client-0.5.3/examples/create-tile.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 novita_client-0.5.3/examples/doodle.py
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 novita_client-0.5.3/examples/img2img.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 novita_client-0.5.3/examples/img2video.py
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 novita_client-0.5.3/examples/instantid.py
+-rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 novita_client-0.5.3/examples/latent-consistency-txt2img.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 novita_client-0.5.3/examples/lcm-img2img.py
+-rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 novita_client-0.5.3/examples/lcm-vs-txt2img.py
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 novita_client-0.5.3/examples/make-photo.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 novita_client-0.5.3/examples/merge-face.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 novita_client-0.5.3/examples/mixpose.py
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 novita_client-0.5.3/examples/model-search.py
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 novita_client-0.5.3/examples/outpainting.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 novita_client-0.5.3/examples/reimagine.py
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 novita_client-0.5.3/examples/remove-background.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 novita_client-0.5.3/examples/remove-text.py
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 novita_client-0.5.3/examples/replace-background.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 novita_client-0.5.3/examples/replace-object.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 novita_client-0.5.3/examples/replace-sky.py
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 novita_client-0.5.3/examples/txt2img-with-hiresfix.py
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 novita_client-0.5.3/examples/txt2img-with-lora.py
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 novita_client-0.5.3/examples/txt2img-with-refiner.py
+-rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 novita_client-0.5.3/examples/fixtures/qrcode.png
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 novita_client-0.5.3/src/novita_client/__init__.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 novita_client-0.5.3/src/novita_client/exceptions.py
+-rw-r--r--   0        0        0    45014 2020-02-02 00:00:00.000000 novita_client-0.5.3/src/novita_client/novita.py
+-rw-r--r--   0        0        0    37956 2020-02-02 00:00:00.000000 novita_client-0.5.3/src/novita_client/proto.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 novita_client-0.5.3/src/novita_client/serializer.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 novita_client-0.5.3/src/novita_client/settings.py
+-rw-r--r--   0        0        0     3609 2020-02-02 00:00:00.000000 novita_client-0.5.3/src/novita_client/utils.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 novita_client-0.5.3/src/novita_client/version.py
+-rw-r--r--   0        0        0    12841 2020-02-02 00:00:00.000000 novita_client-0.5.3/tests/test_basics.py
+-rw-r--r--   0        0        0     8539 2020-02-02 00:00:00.000000 novita_client-0.5.3/tests/test_enhance.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 novita_client-0.5.3/tests/test_model.py
+-rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 novita_client-0.5.3/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 novita_client-0.5.3/LICENSE
+-rw-r--r--   0        0        0    22761 2020-02-02 00:00:00.000000 novita_client-0.5.3/README.md
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 novita_client-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0    24574 2020-02-02 00:00:00.000000 novita_client-0.5.3/PKG-INFO
```

### Comparing `novita_client-0.5.2/generate-readme.sh` & `novita_client-0.5.3/generate-readme.sh`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.2/image.jpg` & `novita_client-0.5.3/image.jpg`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.2/image2.jpg` & `novita_client-0.5.3/image2.jpg`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.2/img2img-controlnet.png` & `novita_client-0.5.3/img2img-controlnet.png`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.2/img2img-logo.png` & `novita_client-0.5.3/img2img-logo.png`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.2/img2img.png` & `novita_client-0.5.3/img2img.png`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.2/logo.py` & `novita_client-0.5.3/logo.py`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.2/outpainting.png` & `novita_client-0.5.3/outpainting.png`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.2/requirements-dev.lock` & `novita_client-0.5.3/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.2/shanginn.py` & `novita_client-0.5.3/examples/img2img.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,34 @@
-#!/usr/bin/env python
-# -*- coding: UTF-8 -*-
-
+import pdb
 import os
-from novita_client import NovitaClient, Txt2ImgV3LoRA, Samplers, Txt2ImgV3HiresFix, Txt2ImgV3Refiner
-from novita_client.utils import base64_to_image
 
+from novita_client import NovitaClient, Img2ImgV3ControlNetUnit, ControlNetPreprocessor, Img2ImgV3Embedding
+from novita_client.utils import base64_to_image, input_image_to_pil
 
 client = NovitaClient(os.getenv('NOVITA_API_KEY'), os.getenv('NOVITA_API_URI', None))
-# client.set_extra_headers({
-#     "X-Novita-Debug-Host": "http://7e30796b0529afb6c59fceecb9099a01-8860.npipe.internal.omniinfer.io:8080"
-# })
-
-res = client.txt2img_v3(
-    prompt="a photo of handsome man, close up",
-    negative_prompt="wrong",
-    image_num=1,
-    guidance_scale=7.0,
-    sampler_name=Samplers.DPMPP_M_KARRAS,
-    model_name="leosamsHelloworldSDXL_helloworldSDXL50_268813.safetensors",
-    height=1024,
+res = client.img2img_v3(
+    model_name="MeinaHentai_V5.safetensors",
+    steps=30,
+    height=512,
+    width=512,
+    input_image="https://img.freepik.com/premium-photo/close-up-dogs-face-with-big-smile-generative-ai_900101-62851.jpg",
+    prompt="1 cute dog",
+    strength=0.5,
+    guidance_scale=7,
+    embeddings=[Img2ImgV3Embedding(model_name=_) for _ in [
+        "bad-image-v2-39000",
+        "verybadimagenegative_v1.3_21434",
+        "BadDream_53202",
+        "badhandv4_16755",
+        "easynegative_8955.safetensors"]],
     seed=-1,
-    # hires_fix=Txt2ImgV3HiresFix(
-    #     upscaler="RealESRNet_x4plus",
-    #     target_height=2048,
-    #     target_width=2048,
-    #     strength=0.5
-    # ),
-    # refiner=Txt2ImgV3Refiner(
-    #     switch_at=0.75
-    # ),
-    loras=[Txt2ImgV3LoRA(
-        model_name="sdxl_wrong_lora",
-        strength=0.8
-    )
-    ]
+    sampler_name="DPM++ 2M Karras",
+    clip_skip=2,
+    # controlnet_units=[Img2ImgV3ControlNetUnit(
+    #     model_name="control_v11f1p_sd15_depth",
+    #     preprocessor="depth",
+    #     image_base64="./20240309-003206.jpeg",
+    #     strength=1.0
+    # )]
 )
 
-base64_to_image(res.images_encoded[0]).save("image1.jpg")
-# base64_to_image(res.images_encoded[1]).save("image2.jpg")
+base64_to_image(res.images_encoded[0]).save("./img2img.png")
```

### Comparing `novita_client-0.5.2/txt2img_with_hiresfix.png` & `novita_client-0.5.3/txt2img_with_hiresfix.png`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.2/examples/cleanup.py` & `novita_client-0.5.3/examples/cleanup.py`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.2/examples/controlnet.py` & `novita_client-0.5.3/examples/controlnet.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,27 +7,24 @@
 from novita_client.utils import base64_to_image
 
 
 client = NovitaClient(os.getenv('NOVITA_API_KEY'), os.getenv('NOVITA_API_URI', None))
 res = client.img2img_v3(
     input_image="https://img.freepik.com/premium-photo/close-up-dogs-face-with-big-smile-generative-ai_900101-62851.jpg",
     model_name="dreamshaper_8_93211.safetensors",
-    prompt="a cute dog, masterpiece, best quality",
+    prompt="a cute dog",
     sampler_name=Samplers.DPMPP_M_KARRAS,
     width=512,
     height=512,
     steps=30,
-    strength=1.0,
     controlnet_units=[
         Img2ImgV3ControlNetUnit(
-            # image_base64="https://img.freepik.com/premium-photo/close-up-dogs-face-with-big-smile-generative-ai_900101-62851.jpg",
-            image_base64="examples/fixtures/qrcode.png",
-            model_name="control_v1p_sd15_brightness",
-            preprocessor=None,
-            strength=1
+            image_base64="https://img.freepik.com/premium-photo/close-up-dogs-face-with-big-smile-generative-ai_900101-62851.jpg",
+            model_name="control_v11f1p_sd15_depth",
+            strength=1.0
         )
     ],
     embeddings=[Img2ImgV3Embedding(model_name=_) for _ in [
         "BadDream_53202",
     ]],
     seed=-1,
 )
```

### Comparing `novita_client-0.5.2/examples/instantid.py` & `novita_client-0.5.3/examples/instantid.py`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.2/examples/latent-consistency-txt2img.py` & `novita_client-0.5.3/examples/latent-consistency-txt2img.py`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.2/examples/lcm-vs-txt2img.py` & `novita_client-0.5.3/examples/lcm-vs-txt2img.py`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.2/examples/make-photo.py` & `novita_client-0.5.3/examples/make-photo.py`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.2/examples/model-search.py` & `novita_client-0.5.3/examples/model-search.py`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.2/examples/txt2img-with-hiresfix.py` & `novita_client-0.5.3/examples/txt2img-with-hiresfix.py`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.2/examples/txt2img-with-lora.py` & `novita_client-0.5.3/examples/txt2img-with-lora.py`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.2/examples/txt2img-with-refiner.py` & `novita_client-0.5.3/examples/txt2img-with-refiner.py`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.2/examples/fixtures/qrcode.png` & `novita_client-0.5.3/examples/fixtures/qrcode.png`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.2/src/novita_client/novita.py` & `novita_client-0.5.3/src/novita_client/novita.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,27 +185,29 @@
             i += 1
 
         raise NovitaTimeoutError(
             f"Task {task_id} failed to complete in {wait_for} seconds")
 
     def wait_for_task_v3(self, task_id, wait_for: int = 300, callback: callable = None) -> V3TaskResponse:
         i = 0
+
         while i < wait_for:
             logger.info(f"Waiting for task {task_id} to complete")
 
             progress = self.async_task_result(task_id)
 
             if callback and callable(callback):
                 try:
                     callback(progress)
                 except Exception as e:
                     logger.error(f"Task {task_id} progress callback failed: {e}")
 
             if progress.finished():
                 logger.info(f"Task {task_id} completed")
+                logging.debug(f"Task {progress.task.task_type}/{progress.task.task_id} debug_info: {progress.extra.debug_info}")
                 return progress
 
             sleep(settings.DEFAULT_POLL_INTERVAL)
             i += 1
         raise NovitaTimeoutError(
             f"Task {task_id} failed to complete in {wait_for} seconds")
 
@@ -794,15 +796,15 @@
 
         if response_image_type is not None:
             payload_data.set_image_type(response_image_type)
 
         res = self._post("/v3/async/instant-id", payload_data.to_dict())
         final_res = self.wait_for_task_v3(res["task_id"], callback=callback)
         if final_res.task.status != V3TaskResponseStatus.TASK_STATUS_SUCCEED:
-            logger.error(f"Task {final_res.task_id} failed with status {final_res.task.status}")
+            logger.error(f"Task {final_res.task.task_id} failed with status {final_res.task.status}")
         else:
             if download_images:
                 final_res.download_images()
 
         return final_res
 
     def raw_img2img_v3(self, req: Img2ImgV3Request, extra: CommonV3Extra = None) -> Img2ImgV3Response:
@@ -856,15 +858,15 @@
                 final_res.download_images()
         return final_res
 
     def raw_txt2img_v3(self, req: Txt2ImgV3Request, extra: CommonV3Extra = None) -> Txt2ImgV3Response:
         _req = CommonV3Request(request=req, extra=extra)
         return Txt2ImgV3Response.from_dict(self._post('/v3/async/txt2img', _req.to_dict()))
 
-    def txt2img_v3(self, model_name: str, prompt: str, height: int = None, width: int = None, negative_prompt: str = None, sd_vae: str = None, steps: int = None, guidance_scale: float = None, image_num: int = None, clip_skip: int = None, seed: int = None, strength: float = None, sampler_name: str = None, response_image_type: str = None, loras: List[Txt2ImgV3LoRA] = None, embeddings: List[Txt2ImgV3Embedding] = None, hires_fix: Txt2ImgV3HiresFix = None, refiner: Txt2ImgV3Refiner = None, download_images: bool = True, callback: callable = None, **kwargs) -> Txt2ImgV3Response:
+    def txt2img_v3(self, model_name: str, prompt: str, height: int = None, width: int = None, negative_prompt: str = None, sd_vae: str = None, steps: int = None, guidance_scale: float = None, image_num: int = None, clip_skip: int = None, seed: int = None, strength: float = None, sampler_name: str = None, response_image_type: str = None, loras: List[Txt2ImgV3LoRA] = None, embeddings: List[Txt2ImgV3Embedding] = None, hires_fix: Txt2ImgV3HiresFix = None, refiner: Txt2ImgV3Refiner = None, download_images: bool = True, callback: callable = None, **kwargs) -> V3TaskResponse:
         req = Txt2ImgV3Request(
             model_name=model_name,
             prompt=prompt,
             negative_prompt=negative_prompt,
             sd_vae=sd_vae,
             clip_skip=clip_skip,
             loras=loras,
@@ -892,15 +894,16 @@
         extra = CommonV3Extra(**kwargs)
         if response_image_type is not None:
             extra.response_image_type = response_image_type
 
         res = self.raw_txt2img_v3(req, extra)
         final_res = self.wait_for_task_v3(res.task_id, callback=callback)
         if final_res.task.status != V3TaskResponseStatus.TASK_STATUS_SUCCEED:
-            logger.error(f"Task {final_res.task_id} failed with status {final_res.task.status}")
+            logger.error(f"Task {res.task_id} failed with status {final_res}")
+            raise NovitaResponseError(f"Task {res.task_id} failed with status {final_res.task.status}")
         else:
             if download_images:
                 final_res.download_images()
         return final_res
 
     def user_info(self) -> UserInfoResponse:
         return UserInfoResponse.from_dict(self._get("/v3/user"))
```

### Comparing `novita_client-0.5.2/src/novita_client/proto.py` & `novita_client-0.5.3/src/novita_client/proto.py`

 * *Files 3% similar despite different names*

```diff
@@ -138,14 +138,20 @@
     steps: Optional[int] = 20
     strength: Optional[float] = 0.5
     seed: Optional[int] = None
 
 
 # --------------- Text2Image ---------------
 
+@dataclass
+class Txt2ImgExtra(JSONe):
+    enable_nsfw_detection: bool = False
+    nsfw_detection_level: int = 0
+    enable_progress_info: bool = True
+
 
 @dataclass
 class Txt2ImgRequest(JSONe):
     prompt: str
     negative_prompt: Optional[str] = None
     model_name: str = 'dreamshaper_5BakedVae.safetensors'
     sampler_name: str = None
@@ -170,14 +176,16 @@
     hr_resize_x: Optional[int] = None
     hr_resize_y: Optional[int] = None
 
     sd_refiner: Optional[Refiner] = None
 
     adetailer: Optional[ADEtailer] = None
 
+    extra: Optional[Txt2ImgExtra] = None
+
 
 class Txt2ImgResponseCode(Enum):
     NORMAL = 0
     INTERNAL_ERROR = -1
     INVALID_JSON = 1
     MODEL_NOT_EXISTS = 2
     TASK_ID_NOT_EXISTS = 3
@@ -208,14 +216,20 @@
     data: Optional[Txt2ImgResponseData] = None
 
 
 #  --------------- Image2Image ---------------
 
 
 @dataclass
+class Img2ImgExtra(JSONe):
+    enable_nsfw_detection: bool = False
+    nsfw_detection_level: int = 0
+    enable_progress_info: bool = True
+
+@dataclass
 class Img2ImgRequest(JSONe):
     model_name: str = 'dreamshaper_5BakedVae.safetensors'
     sampler_name: str = None
     init_images: List[str] = None
     mask: Optional[str] = None
     resize_mode: Optional[int] = 0
     denoising_strength: Optional[float] = 0.75
@@ -239,14 +253,16 @@
     clip_skip: Optional[int] = None
 
     controlnet_units: Optional[List[ControlnetUnit]] = None
     controlnet_no_detectmap: Optional[bool] = False
 
     sd_refiner: Optional[Refiner] = None
 
+    extra: Optional[Img2ImgExtra] = None
+
 
 class Img2ImgResponseCode(Enum):
     NORMAL = 0
     INTERNAL_ERROR = -1
     INVALID_JSON = 1
     MODEL_NOT_EXISTS = 2
     TASK_ID_NOT_EXISTS = 3
@@ -293,28 +309,46 @@
         return cls(cls.UNKNOWN)
 
     def finished(self):
         return self in (ProgressResponseStatusCode.SUCCESSFUL, ProgressResponseStatusCode.FAILED, ProgressResponseStatusCode.TIMEOUT)
 
 
 @dataclass
+class ProgressDataDebugInfo(JSONe):
+    submit_time_ms: int
+    execution_time_ms: int
+    txt2img_time_ms: int
+    finish_time_ms: int
+
+
+@dataclass
+class ProgressDataNSFWResult(JSONe):
+    valid: bool = False
+    confidence: float = 0.0
+
+
+@dataclass
 class ProgressData(JSONe):
     status: ProgressResponseStatusCode
     progress: int
     eta_relative: int
     imgs: Optional[List[str]] = None
     imgs_bytes: Optional[List[str]] = None
     info: Optional[str] = ""
     failed_reason: Optional[str] = ""
     current_images: Optional[List[str]] = None
     submit_time: Optional[str] = ""
     execution_time: Optional[str] = ""
     txt2img_time: Optional[str] = ""
     finish_time: Optional[str] = ""
 
+    enable_nsfw_detection: Optional[bool] = False
+    nsfw_detection_result: Optional[Union[List[ProgressDataNSFWResult], None]] = None
+    debug_info: Optional[ProgressDataDebugInfo] = None
+
 
 class ProgressResponseCode(Enum):
     NORMAL = 0
     INTERNAL_ERROR = -1
     INVALID_JSON = 1
     MODEL_NOT_EXISTS = 2
     TASK_ID_NOT_EXISTS = 3
@@ -598,18 +632,25 @@
 #       "image_type": "png",
 #       "image_url_ttl": 3600
 #     }
 #   ]
 # }
 
 @dataclass
+class V3TaskImageNSFWDetectionResult(JSONe):
+    valid: bool
+    confidence: float
+
+
+@dataclass
 class V3TaskImage(JSONe):
     image_url: str
     image_type: str
     image_url_ttl: int
+    nsfw_detection_result: Optional[V3TaskImageNSFWDetectionResult] = None
 
 
 @dataclass
 class V3TaskVideo(JSONe):
     video_url: str
     video_type: str
     video_url_ttl: int
@@ -627,21 +668,41 @@
     task_id: str
 
 
 @dataclass
 class V3TaskResponseTask(JSONe):
     task_id: str
     status: V3TaskResponseStatus
+    reason: Optional[str] = None
+    task_type: Optional[str] = None
+    eta: Optional[int] = None
+    progress_percent: Optional[int] = None
+
+
+@dataclass
+class V3TaskResponseDebugInfo(JSONe):
+    submit_time_ms: int
+    execute_time_ms: int
+    complete_time_ms: int
+    request_info: str = None
+
+
+@dataclass
+class V3TaskResponseExtra(JSONe):
+    seed: Optional[int] = None
+    enable_nsfw_detection: Optional[bool] = False
+    debug_info: Optional[V3TaskResponseDebugInfo] = None
 
 
 @dataclass
 class V3TaskResponse(JSONe):
     task: V3TaskResponseTask
     images: List[V3TaskImage] = None
     videos: List[V3TaskVideo] = None
+    extra: V3TaskResponseExtra = None
 
     def finished(self):
         return self.task.status == V3TaskResponseStatus.TASK_STATUS_SUCCEED or self.task.status == V3TaskResponseStatus.TASK_STATUS_FAILED
 
     def get_image_urls(self):
         return [image.image_url for image in self.images]
```

### Comparing `novita_client-0.5.2/src/novita_client/utils.py` & `novita_client-0.5.3/src/novita_client/utils.py`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.2/tests/test_basics.py` & `novita_client-0.5.3/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.2/tests/test_enhance.py` & `novita_client-0.5.3/tests/test_enhance.py`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.2/tests/test_model.py` & `novita_client-0.5.3/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.2/.gitignore` & `novita_client-0.5.3/.gitignore`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.2/LICENSE` & `novita_client-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.2/README.md` & `novita_client-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.2/pyproject.toml` & `novita_client-0.5.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "novita_client"
-version = "0.5.2"
+version = "0.5.3"
 description = "novita SDK for Python"
 authors = [
     { name = "novita", email = "novitalabs@gmail.com" }
 ]
 
 
 dependencies = [
```

### Comparing `novita_client-0.5.2/PKG-INFO` & `novita_client-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: novita_client
-Version: 0.5.2
+Version: 0.5.3
 Summary: novita SDK for Python
 Project-URL: Homepage, https://github.com/novita/python-sdk
 Project-URL: Bug Tracker, https://discord.gg/nzqq8UScpx
 Author-email: novita <novitalabs@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 novita.ai
```

