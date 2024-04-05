# Comparing `tmp/VisionCraftAPI-1.0.1.tar.gz` & `tmp/VisionCraftAPI-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VisionCraftAPI-1.0.1.tar", last modified: Thu Mar 28 13:07:56 2024, max compression
+gzip compressed data, was "VisionCraftAPI-1.0.2.tar", last modified: Thu Apr  4 18:12:27 2024, max compression
```

## Comparing `VisionCraftAPI-1.0.1.tar` & `VisionCraftAPI-1.0.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-03-28 13:07:56.004974 VisionCraftAPI-1.0.1/
--rw-rw-rw-   0        0        0     1091 2024-03-28 06:00:02.000000 VisionCraftAPI-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     2002 2024-03-28 13:07:56.004974 VisionCraftAPI-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1680 2024-03-28 07:28:53.000000 VisionCraftAPI-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-03-28 13:07:55.908983 VisionCraftAPI-1.0.1/VisionCraftAPI/
--rw-rw-rw-   0        0        0       34 2024-03-26 11:28:25.000000 VisionCraftAPI-1.0.1/VisionCraftAPI/__init__.py
--rw-rw-rw-   0        0        0    22557 2024-03-28 06:18:16.000000 VisionCraftAPI-1.0.1/VisionCraftAPI/api.py
-drwxrwxrwx   0        0        0        0 2024-03-28 13:07:55.980989 VisionCraftAPI-1.0.1/VisionCraftAPI/enums/
--rw-rw-rw-   0        0        0      125 2024-03-26 22:05:26.000000 VisionCraftAPI-1.0.1/VisionCraftAPI/enums/__init__.py
--rw-rw-rw-   0        0        0      160 2024-03-26 22:04:43.000000 VisionCraftAPI-1.0.1/VisionCraftAPI/enums/modes.py
--rw-rw-rw-   0        0        0      162 2024-03-26 22:04:35.000000 VisionCraftAPI-1.0.1/VisionCraftAPI/enums/task_statuses.py
-drwxrwxrwx   0        0        0        0 2024-03-28 13:07:55.980989 VisionCraftAPI-1.0.1/VisionCraftAPI/exceptions/
--rw-rw-rw-   0        0        0      309 2024-03-27 16:35:37.000000 VisionCraftAPI-1.0.1/VisionCraftAPI/exceptions/__init__.py
--rw-rw-rw-   0        0        0     2377 2024-03-27 16:42:14.000000 VisionCraftAPI-1.0.1/VisionCraftAPI/exceptions/types.py
--rw-rw-rw-   0        0        0     2032 2024-03-28 06:08:49.000000 VisionCraftAPI-1.0.1/VisionCraftAPI/http_client.py
-drwxrwxrwx   0        0        0        0 2024-03-28 13:07:55.996974 VisionCraftAPI-1.0.1/VisionCraftAPI/models/
--rw-rw-rw-   0        0        0      303 2024-03-27 20:35:50.000000 VisionCraftAPI-1.0.1/VisionCraftAPI/models/__init__.py
--rw-rw-rw-   0        0        0      336 2024-03-27 20:24:16.000000 VisionCraftAPI-1.0.1/VisionCraftAPI/models/limits.py
--rw-rw-rw-   0        0        0      147 2024-03-26 17:31:11.000000 VisionCraftAPI-1.0.1/VisionCraftAPI/models/llm.py
--rw-rw-rw-   0        0        0      488 2024-03-27 20:28:11.000000 VisionCraftAPI-1.0.1/VisionCraftAPI/models/midjourney.py
--rw-rw-rw-   0        0        0      823 2024-03-27 20:30:01.000000 VisionCraftAPI-1.0.1/VisionCraftAPI/models/whisper.py
-drwxrwxrwx   0        0        0        0 2024-03-28 13:07:55.996974 VisionCraftAPI-1.0.1/VisionCraftAPI/utils/
--rw-rw-rw-   0        0        0       69 2024-03-26 22:05:35.000000 VisionCraftAPI-1.0.1/VisionCraftAPI/utils/__init__.py
--rw-rw-rw-   0        0        0     1469 2024-03-27 16:55:54.000000 VisionCraftAPI-1.0.1/VisionCraftAPI/utils/checker.py
-drwxrwxrwx   0        0        0        0 2024-03-28 13:07:55.972984 VisionCraftAPI-1.0.1/VisionCraftAPI.egg-info/
--rw-rw-rw-   0        0        0     2002 2024-03-28 13:07:55.000000 VisionCraftAPI-1.0.1/VisionCraftAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      744 2024-03-28 13:07:55.000000 VisionCraftAPI-1.0.1/VisionCraftAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-28 13:07:55.000000 VisionCraftAPI-1.0.1/VisionCraftAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-03-28 13:07:55.000000 VisionCraftAPI-1.0.1/VisionCraftAPI.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       25 2024-03-28 13:07:55.000000 VisionCraftAPI-1.0.1/VisionCraftAPI.egg-info/requires.txt
--rw-rw-rw-   0        0        0      105 2024-03-28 13:07:55.000000 VisionCraftAPI-1.0.1/VisionCraftAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-28 13:07:56.004974 VisionCraftAPI-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      784 2024-03-28 13:07:30.000000 VisionCraftAPI-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 18:12:27.037027 VisionCraftAPI-1.0.2/
+-rw-rw-rw-   0        0        0     1091 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2542 2024-04-04 18:12:27.038025 VisionCraftAPI-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2222 2024-04-04 18:09:23.000000 VisionCraftAPI-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-04 18:12:26.972030 VisionCraftAPI-1.0.2/VisionCraftAPI/
+-rw-rw-rw-   0        0        0       34 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.2/VisionCraftAPI/__init__.py
+-rw-rw-rw-   0        0        0    22764 2024-04-04 18:02:34.000000 VisionCraftAPI-1.0.2/VisionCraftAPI/api.py
+drwxrwxrwx   0        0        0        0 2024-04-04 18:12:26.994025 VisionCraftAPI-1.0.2/VisionCraftAPI/enums/
+-rw-rw-rw-   0        0        0      125 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.2/VisionCraftAPI/enums/__init__.py
+-rw-rw-rw-   0        0        0      160 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.2/VisionCraftAPI/enums/modes.py
+-rw-rw-rw-   0        0        0      162 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.2/VisionCraftAPI/enums/task_statuses.py
+drwxrwxrwx   0        0        0        0 2024-04-04 18:12:26.997025 VisionCraftAPI-1.0.2/VisionCraftAPI/exceptions/
+-rw-rw-rw-   0        0        0      309 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.2/VisionCraftAPI/exceptions/__init__.py
+-rw-rw-rw-   0        0        0     2377 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.2/VisionCraftAPI/exceptions/types.py
+-rw-rw-rw-   0        0        0     2032 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.2/VisionCraftAPI/http_client.py
+drwxrwxrwx   0        0        0        0 2024-04-04 18:12:27.008030 VisionCraftAPI-1.0.2/VisionCraftAPI/models/
+-rw-rw-rw-   0        0        0      303 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.2/VisionCraftAPI/models/__init__.py
+-rw-rw-rw-   0        0        0      336 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.2/VisionCraftAPI/models/limits.py
+-rw-rw-rw-   0        0        0      147 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.2/VisionCraftAPI/models/llm.py
+-rw-rw-rw-   0        0        0      488 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.2/VisionCraftAPI/models/midjourney.py
+-rw-rw-rw-   0        0        0      823 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.2/VisionCraftAPI/models/whisper.py
+drwxrwxrwx   0        0        0        0 2024-04-04 18:12:27.036028 VisionCraftAPI-1.0.2/VisionCraftAPI/utils/
+-rw-rw-rw-   0        0        0       69 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.2/VisionCraftAPI/utils/__init__.py
+-rw-rw-rw-   0        0        0     1469 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.2/VisionCraftAPI/utils/checker.py
+drwxrwxrwx   0        0        0        0 2024-04-04 18:12:26.987026 VisionCraftAPI-1.0.2/VisionCraftAPI.egg-info/
+-rw-rw-rw-   0        0        0     2542 2024-04-04 18:12:26.000000 VisionCraftAPI-1.0.2/VisionCraftAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      744 2024-04-04 18:12:26.000000 VisionCraftAPI-1.0.2/VisionCraftAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 18:12:26.000000 VisionCraftAPI-1.0.2/VisionCraftAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-04 18:12:26.000000 VisionCraftAPI-1.0.2/VisionCraftAPI.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       25 2024-04-04 18:12:26.000000 VisionCraftAPI-1.0.2/VisionCraftAPI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      105 2024-04-04 18:12:26.000000 VisionCraftAPI-1.0.2/VisionCraftAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-04 18:12:27.040028 VisionCraftAPI-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      784 2024-04-04 18:12:19.000000 VisionCraftAPI-1.0.2/setup.py
```

### Comparing `VisionCraftAPI-1.0.1/LICENSE` & `VisionCraftAPI-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `VisionCraftAPI-1.0.1/PKG-INFO` & `VisionCraftAPI-1.0.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-Metadata-Version: 2.1
-Name: VisionCraftAPI
-Version: 1.0.1
-Summary: Fully async python wrapper for VisionCraft API
-Home-page: https://github.com/Belyashik2K/VisionCraftAPI
-Author: Belyashik2K
-Author-email: work@belyashik2k.ru
-License: MIT license
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-![photo_2024-03-28_10-22-45](https://github.com/Belyashik2K/TruckersMP/assets/126521808/b19a4f29-a2bf-4692-8de3-221dd166e42a)
+![photo (4)](https://github.com/Belyashik2K/VisionCraftAPI/assets/126521808/fa32e4fa-37bd-47a7-9574-bbc02191796b)
 # VisionCraft API
 > Fully async python wrapper for [VisionCraft API](https://api.visioncraft.top/docs)
 
 ## Installing
 
     pip install VisionCraftAPI
 
 ## Features
 * Fully async methods
 * Important methods return Pydantic model as result for easier interaction with data
 * Full exception handling
+* Full [documentation](https://vision.b2k.tech/) is available
 
 ## Usage
 ```python
 import asyncio
+import aiohttp
 
 from VisionCraftAPI import VisionCraftClient
 
 async def generate_xl_image(client: VisionCraftClient,
                             prompt: str,
                             model: str,
-                            sampler: str) -> bytes:
+                            sampler: str,
+                            image_count: int):
     images = await client.generate_xl_image(
         prompt=prompt,
         model=model,
-        sampler=sampler
+        sampler=sampler,
+        image_count=image_count
     )
     
-    print('Image generated! Saving to image.png...')
-    with open('image.png', 'wb') as file:
-        file.write(images)   
-
+    print('Images generated! Saving it...')
+    # Download and save the generated images
+    async with aiohttp.ClientSession() as session:
+        for i, image_url in enumerate(images):
+            async with session.get(image_url) as image_response:
+                image_data = await image_response.read()
+                # Save the image locally
+                with open(f"generated_image_{i}.png", "wb") as f:
+                    f.write(image_data)
+                    
 async def main():
     # Set your API key
     api_key = "YOUR_API_KEY"
     # Create a VisionCraftClient instance
     client = VisionCraftClient(api_key=api_key)
     
     # Get all SDXL models and samplers
     models = await client.get_xl_models()
     samplers = await client.get_xl_samplers()
 
     # Generate an image with the first model and sampler
     await generate_xl_image(client=client,
                             prompt='A beautiful sunset',
                             model=models[0],
-                            sampler=samplers[0])
+                            sampler=samplers[0],
+                            image_count=4)
             
 if __name__ == '__main__':
     asyncio.run(main())
 ```
 
 ## Docs
 > Go to https://vision.b2k.tech/ for more information about SDK
```

### Comparing `VisionCraftAPI-1.0.1/VisionCraftAPI/api.py` & `VisionCraftAPI-1.0.2/VisionCraftAPI/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -214,46 +214,50 @@
                                 prompt: str,
                                 model: str,
                                 sampler: str,
                                 width: Optional[int] = 1024,
                                 height: Optional[int] = 1024,
                                 negative_prompt: Optional[str] = str(),
                                 cfg_scale: Optional[int] = 10,
-                                steps: Optional[int] = 30) -> bytes:
+                                steps: Optional[int] = 30,
+                                image_count: Optional[int] = 1) -> list[str]:
         """
         Generate an image using StableDiffusion XL models.
         
         API Docs: https://docs.visioncraft.top/interacting-with-the-api/stablediffusion-xl-models/image-generation
         SDK Docs: https://vision.b2k.tech/docs/api-methods/stablediffusion-xl-models/generate_xl_image
         
         :param prompt: A text prompt for image generation
         :param model: A StableDiffusion XL model from the list of available models
         :param sampler: A sampler from the list of available samplers
         :param width: Width of the generated image (min: 512, max: 1024, default: 1024)
         :param height: Height of the generated image (min: 512, max: 1024, default: 1024)
         :param negative_prompt: A negative text prompt for image generation
         :param cfg_scale: A scale for the configuration (min: 1, max: 20, default: 10)
         :param steps: Number of steps for image generation (min: 1, max: 50, default: 30)
+        :param image_count: Number of images to generate (max: 5, default: 1)
         
-        :return: A bytes object of the generated image
+        :return: A list of image URLs
         """
         
         json = {
             "prompt": prompt,
             "model": model,
             "negative_prompt": negative_prompt,
             "token": self.api_key,
             "height": height,
             "width": width,
             "sampler": sampler,
             "cfg_scale": cfg_scale,
-            "steps": steps
+            "steps": steps,
+            "image_count": image_count
         }
         
-        return await self.__post(f'{self.API_HOST}/generate-xl', json=json)
+        result = await self.__post(f'{self.API_HOST}/generate-xl', json=json)
+        return result['images']
         
     async def create_midjourney_task(self,
                                      prompt: str) -> MidjourneyTask:
         """
         Create a Midjourney image generation task.
         
         API Docs: https://docs.visioncraft.top/interacting-with-the-api/midjourney/create-task
```

### Comparing `VisionCraftAPI-1.0.1/VisionCraftAPI/exceptions/types.py` & `VisionCraftAPI-1.0.2/VisionCraftAPI/exceptions/types.py`

 * *Files identical despite different names*

### Comparing `VisionCraftAPI-1.0.1/VisionCraftAPI/http_client.py` & `VisionCraftAPI-1.0.2/VisionCraftAPI/http_client.py`

 * *Files identical despite different names*

### Comparing `VisionCraftAPI-1.0.1/VisionCraftAPI/models/whisper.py` & `VisionCraftAPI-1.0.2/VisionCraftAPI/models/whisper.py`

 * *Files identical despite different names*

### Comparing `VisionCraftAPI-1.0.1/VisionCraftAPI/utils/checker.py` & `VisionCraftAPI-1.0.2/VisionCraftAPI/utils/checker.py`

 * *Files identical despite different names*

### Comparing `VisionCraftAPI-1.0.1/VisionCraftAPI.egg-info/PKG-INFO` & `VisionCraftAPI-1.0.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,66 +1,77 @@
 Metadata-Version: 2.1
 Name: VisionCraftAPI
-Version: 1.0.1
+Version: 1.0.2
 Summary: Fully async python wrapper for VisionCraft API
 Home-page: https://github.com/Belyashik2K/VisionCraftAPI
 Author: Belyashik2K
 Author-email: work@belyashik2k.ru
 License: MIT license
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-![photo_2024-03-28_10-22-45](https://github.com/Belyashik2K/TruckersMP/assets/126521808/b19a4f29-a2bf-4692-8de3-221dd166e42a)
+![photo (4)](https://github.com/Belyashik2K/VisionCraftAPI/assets/126521808/fa32e4fa-37bd-47a7-9574-bbc02191796b)
 # VisionCraft API
 > Fully async python wrapper for [VisionCraft API](https://api.visioncraft.top/docs)
 
 ## Installing
 
     pip install VisionCraftAPI
 
 ## Features
 * Fully async methods
 * Important methods return Pydantic model as result for easier interaction with data
 * Full exception handling
+* Full [documentation](https://vision.b2k.tech/) is available
 
 ## Usage
 ```python
 import asyncio
+import aiohttp
 
 from VisionCraftAPI import VisionCraftClient
 
 async def generate_xl_image(client: VisionCraftClient,
                             prompt: str,
                             model: str,
-                            sampler: str) -> bytes:
+                            sampler: str,
+                            image_count: int):
     images = await client.generate_xl_image(
         prompt=prompt,
         model=model,
-        sampler=sampler
+        sampler=sampler,
+        image_count=image_count
     )
     
-    print('Image generated! Saving to image.png...')
-    with open('image.png', 'wb') as file:
-        file.write(images)   
-
+    print('Images generated! Saving it...')
+    # Download and save the generated images
+    async with aiohttp.ClientSession() as session:
+        for i, image_url in enumerate(images):
+            async with session.get(image_url) as image_response:
+                image_data = await image_response.read()
+                # Save the image locally
+                with open(f"generated_image_{i}.png", "wb") as f:
+                    f.write(image_data)
+                    
 async def main():
     # Set your API key
     api_key = "YOUR_API_KEY"
     # Create a VisionCraftClient instance
     client = VisionCraftClient(api_key=api_key)
     
     # Get all SDXL models and samplers
     models = await client.get_xl_models()
     samplers = await client.get_xl_samplers()
 
     # Generate an image with the first model and sampler
     await generate_xl_image(client=client,
                             prompt='A beautiful sunset',
                             model=models[0],
-                            sampler=samplers[0])
+                            sampler=samplers[0],
+                            image_count=4)
             
 if __name__ == '__main__':
     asyncio.run(main())
 ```
 
 ## Docs
 > Go to https://vision.b2k.tech/ for more information about SDK
```

### Comparing `VisionCraftAPI-1.0.1/VisionCraftAPI.egg-info/SOURCES.txt` & `VisionCraftAPI-1.0.2/VisionCraftAPI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `VisionCraftAPI-1.0.1/setup.py` & `VisionCraftAPI-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = '1.0.1'
+version = '1.0.2'
 
 with open('README.md', 'r') as f:
       long_description = f.read()
 
 setup(name='VisionCraftAPI',
       version=version,
```

