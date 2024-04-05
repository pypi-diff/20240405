# Comparing `tmp/substrate-120240403.0.2.tar.gz` & `tmp/substrate-120240405.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "substrate-120240403.0.2.tar", max compression
+gzip compressed data, was "substrate-120240405.0.2.tar", max compression
```

## Comparing `substrate-120240403.0.2.tar` & `substrate-120240405.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1066 2024-03-19 21:46:08.735767 substrate-120240403.0.2/LICENSE
--rw-r--r--   0        0        0       45 2024-03-19 21:55:57.200047 substrate-120240403.0.2/README.md
--rw-r--r--   0        0        0     2023 2024-04-03 07:21:03.109601 substrate-120240403.0.2/pyproject.toml
--rw-r--r--   0        0        0       17 2024-04-03 04:58:23.000000 substrate-120240403.0.2/substrate/GEN_VERSION
--rw-r--r--   0        0        0     1508 2024-04-03 04:58:24.000000 substrate-120240403.0.2/substrate/__init__.py
--rw-r--r--   0        0        0     5582 2024-03-21 22:51:25.550938 substrate-120240403.0.2/substrate/_client.py
--rw-r--r--   0        0        0       30 2024-03-13 14:46:31.829473 substrate-120240403.0.2/substrate/_version.py
--rw-r--r--   0        0        0        1 2024-04-03 05:00:31.508855 substrate-120240403.0.2/substrate/core/__init__.py
--rw-r--r--   0        0        0       27 2024-04-03 05:00:31.508762 substrate-120240403.0.2/substrate/core/_version.py
--rw-r--r--   0        0        0     2200 2024-04-03 05:00:31.509086 substrate-120240403.0.2/substrate/core/base_future.py
--rw-r--r--   0        0        0        0 2024-04-03 05:00:31.509323 substrate-120240403.0.2/substrate/core/client/__init__.py
--rw-r--r--   0        0        0     1750 2024-04-03 05:00:31.509454 substrate-120240403.0.2/substrate/core/client/find_futures_client.py
--rw-r--r--   0        0        0     2620 2024-04-03 05:00:31.509658 substrate-120240403.0.2/substrate/core/client/future.py
--rw-r--r--   0        0        0     1212 2024-04-03 05:00:31.509261 substrate-120240403.0.2/substrate/core/client/graph.py
--rw-r--r--   0        0        0     1149 2024-04-03 05:00:31.508969 substrate-120240403.0.2/substrate/core/coregraph.py
--rw-r--r--   0        0        0     1960 2024-04-03 05:00:31.508332 substrate-120240403.0.2/substrate/core/corenode.py
--rw-r--r--   0        0        0      894 2024-04-03 05:00:31.508168 substrate-120240403.0.2/substrate/core/id_generator.py
--rw-r--r--   0        0        0    31860 2024-04-03 05:00:31.508519 substrate-120240403.0.2/substrate/core/models.py
--rw-r--r--   0        0        0     1405 2024-04-03 05:00:31.507983 substrate-120240403.0.2/substrate/core/sb.py
--rw-r--r--   0        0        0    27585 2024-04-03 04:58:22.000000 substrate-120240403.0.2/substrate/dataclass_models.py
--rw-r--r--   0        0        0    36470 2024-04-03 04:58:23.000000 substrate-120240403.0.2/substrate/future_dataclass_models.py
--rw-r--r--   0        0        0    40093 2024-04-03 04:58:24.000000 substrate-120240403.0.2/substrate/nodes.py
--rw-r--r--   0        0        0        0 2024-02-07 23:39:17.000078 substrate-120240403.0.2/substrate/py.typed
--rw-r--r--   0        0        0     1609 2024-04-03 07:20:12.598479 substrate-120240403.0.2/substrate/substrate.py
--rw-r--r--   0        0        0    29794 2024-04-03 04:58:21.000000 substrate-120240403.0.2/substrate/typeddict_models.py
--rw-r--r--   0        0        0      648 1970-01-01 00:00:00.000000 substrate-120240403.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-03-19 21:46:08.735767 substrate-120240405.0.2/LICENSE
+-rw-r--r--   0        0        0       45 2024-03-19 21:55:57.200047 substrate-120240405.0.2/README.md
+-rw-r--r--   0        0        0     2023 2024-04-05 17:46:23.893237 substrate-120240405.0.2/pyproject.toml
+-rw-r--r--   0        0        0       17 2024-04-05 15:54:24.000000 substrate-120240405.0.2/substrate/GEN_VERSION
+-rw-r--r--   0        0        0     1982 2024-04-05 15:55:06.000000 substrate-120240405.0.2/substrate/__init__.py
+-rw-r--r--   0        0        0     5645 2024-04-05 17:45:09.481547 substrate-120240405.0.2/substrate/_client.py
+-rw-r--r--   0        0        0       30 2024-03-13 14:46:31.829473 substrate-120240405.0.2/substrate/_version.py
+-rw-r--r--   0        0        0        1 2024-04-05 17:45:52.679181 substrate-120240405.0.2/substrate/core/__init__.py
+-rw-r--r--   0        0        0       27 2024-04-05 17:45:52.679078 substrate-120240405.0.2/substrate/core/_version.py
+-rw-r--r--   0        0        0     2200 2024-04-05 17:45:52.679407 substrate-120240405.0.2/substrate/core/base_future.py
+-rw-r--r--   0        0        0        0 2024-04-05 17:45:52.679662 substrate-120240405.0.2/substrate/core/client/__init__.py
+-rw-r--r--   0        0        0     1750 2024-04-05 17:45:52.679764 substrate-120240405.0.2/substrate/core/client/find_futures_client.py
+-rw-r--r--   0        0        0     2620 2024-04-05 17:45:52.679873 substrate-120240405.0.2/substrate/core/client/future.py
+-rw-r--r--   0        0        0     1212 2024-04-05 17:45:52.679592 substrate-120240405.0.2/substrate/core/client/graph.py
+-rw-r--r--   0        0        0     1149 2024-04-05 17:45:52.679293 substrate-120240405.0.2/substrate/core/coregraph.py
+-rw-r--r--   0        0        0     1960 2024-04-05 17:45:52.678464 substrate-120240405.0.2/substrate/core/corenode.py
+-rw-r--r--   0        0        0      894 2024-04-05 17:45:52.678318 substrate-120240405.0.2/substrate/core/id_generator.py
+-rw-r--r--   0        0        0    36616 2024-04-05 17:45:52.678693 substrate-120240405.0.2/substrate/core/models.py
+-rw-r--r--   0        0        0     1405 2024-04-05 17:45:52.678152 substrate-120240405.0.2/substrate/core/sb.py
+-rw-r--r--   0        0        0    31518 2024-04-05 15:54:13.000000 substrate-120240405.0.2/substrate/dataclass_models.py
+-rw-r--r--   0        0        0    41860 2024-04-05 15:54:13.000000 substrate-120240405.0.2/substrate/future_dataclass_models.py
+-rw-r--r--   0        0        0    57918 2024-04-05 15:55:06.000000 substrate-120240405.0.2/substrate/nodes.py
+-rw-r--r--   0        0        0        0 2024-02-07 23:39:17.000078 substrate-120240405.0.2/substrate/py.typed
+-rw-r--r--   0        0        0     1609 2024-04-03 07:20:12.598479 substrate-120240405.0.2/substrate/substrate.py
+-rw-r--r--   0        0        0    34044 2024-04-05 15:54:13.000000 substrate-120240405.0.2/substrate/typeddict_models.py
+-rw-r--r--   0        0        0      648 1970-01-01 00:00:00.000000 substrate-120240405.0.2/PKG-INFO
```

### Comparing `substrate-120240403.0.2/LICENSE` & `substrate-120240405.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `substrate-120240403.0.2/pyproject.toml` & `substrate-120240405.0.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "substrate"
-version = "120240403.0.2"
+version = "120240405.0.2"
 description = "Substrate Python SDK"
 readme = "README.md"
 authors = [ "vprtwn <ben@substrate.run>", "liamgriffiths <liam@substrate.run>",]
 [[tool.poetry.packages]]
 include = "substrate"
 
 [tool.pyright]
```

### Comparing `substrate-120240403.0.2/substrate/_client.py` & `substrate-120240405.0.2/substrate/_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -142,21 +142,18 @@
 class APIClient:
     api_key: str
     base_url: str
     _client: httpx.Client
     _async_client: httpx.AsyncClient
     _version: str
 
-    def __init__(
-        self,
-        api_key: str,
-        base_url: str,
-    ) -> None:
+    def __init__(self, api_key: str, base_url: str, backend: str) -> None:
         self.api_key = api_key
         self.base_url = base_url
+        self.backend = backend
         timeout = httpx.Timeout(60.0)  # default is 5s
         self._client = httpx.Client(timeout=timeout)
         self._async_client = httpx.AsyncClient(timeout=timeout)
         self._version = __version__
 
     @property
     def user_agent(self) -> str:
@@ -183,14 +180,15 @@
 
     @property
     def default_headers(self) -> Dict[str, str]:
         return {
             "Accept": "application/json",
             "Content-Type": "application/json",
             "User-Agent": self.user_agent,
+            "X-Substrate-Backend": self.backend,
             **self.platform_headers,
             **self.auth_headers,
         }
 
     def post_compose(self, dag: Dict[str, Any]) -> APIResponse:
         url = f"{self.base_url}/compose"
         body = {"dag": dag}
```

### Comparing `substrate-120240403.0.2/substrate/core/base_future.py` & `substrate-120240405.0.2/substrate/core/base_future.py`

 * *Files identical despite different names*

### Comparing `substrate-120240403.0.2/substrate/core/client/find_futures_client.py` & `substrate-120240405.0.2/substrate/core/client/find_futures_client.py`

 * *Files identical despite different names*

### Comparing `substrate-120240403.0.2/substrate/core/client/future.py` & `substrate-120240405.0.2/substrate/core/client/future.py`

 * *Files identical despite different names*

### Comparing `substrate-120240403.0.2/substrate/core/client/graph.py` & `substrate-120240405.0.2/substrate/core/client/graph.py`

 * *Files identical despite different names*

### Comparing `substrate-120240403.0.2/substrate/core/coregraph.py` & `substrate-120240405.0.2/substrate/core/coregraph.py`

 * *Files identical despite different names*

### Comparing `substrate-120240403.0.2/substrate/core/corenode.py` & `substrate-120240405.0.2/substrate/core/corenode.py`

 * *Files identical despite different names*

### Comparing `substrate-120240403.0.2/substrate/core/id_generator.py` & `substrate-120240405.0.2/substrate/core/id_generator.py`

 * *Files identical despite different names*

### Comparing `substrate-120240403.0.2/substrate/core/models.py` & `substrate-120240405.0.2/substrate/core/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,15 +177,15 @@
     """
     Number of choices to generate.
     """
     json_schema: Optional[Dict[str, Any]] = None
     """
     JSON schema to guide response.
     """
-    temperature: Annotated[Optional[float], Field(ge=0.0)] = None
+    temperature: Annotated[Optional[float], Field(ge=0.0, le=2.0)] = None
     """
     Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
     max_tokens: Optional[int] = None
     """
     Maximum number of tokens to generate.
     """
@@ -664,25 +664,53 @@
     """
     Input image.
     """
     mask_image_uri: str
     """
     Mask image that controls which pixels are inpainted.
     """
-    model: Optional[Literal["big-lama"]] = "big-lama"
+    store: Optional[str] = None
     """
-    Selected model.
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    """
+    node: Optional[Literal["BigLaMa"]] = "BigLaMa"
+    """
+    Selected node.
+    """
+
+
+class FillMaskOut(BaseModel):
+    class Config:
+        extra = Extra.allow
+
+    image_uri: str
+    """
+    Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
+    """
+
+
+class BigLaMaIn(BaseModel):
+    class Config:
+        extra = Extra.allow
+
+    image_uri: str
+    """
+    Input image.
+    """
+    mask_image_uri: str
+    """
+    Mask image that controls which pixels are inpainted.
     """
     store: Optional[str] = None
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
 
 
-class FillMaskOut(BaseModel):
+class BigLaMaOut(BaseModel):
     class Config:
         extra = Extra.allow
 
     image_uri: str
     """
     Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
     """
@@ -700,25 +728,57 @@
     """
     Return a mask image instead of the original content.
     """
     background_color: Optional[str] = None
     """
     Hex value background color. Transparent if unset.
     """
-    model: Optional[Literal["isnet"]] = "isnet"
+    store: Optional[str] = None
     """
-    Selected model.
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    """
+    node: Optional[Literal["DISISNet"]] = "DISISNet"
+    """
+    Selected node.
+    """
+
+
+class RemoveBackgroundOut(BaseModel):
+    class Config:
+        extra = Extra.allow
+
+    image_uri: str
+    """
+    Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
+    """
+
+
+class DISISNetIn(BaseModel):
+    class Config:
+        extra = Extra.allow
+
+    image_uri: str
+    """
+    Input image.
+    """
+    return_mask: Optional[bool] = None
+    """
+    Return a mask image instead of the original content.
+    """
+    background_color: Optional[str] = None
+    """
+    Hex value background color. Transparent if unset.
     """
     store: Optional[str] = None
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
 
 
-class RemoveBackgroundOut(BaseModel):
+class DISISNetOut(BaseModel):
     class Config:
         extra = Extra.allow
 
     image_uri: str
     """
     Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
     """
@@ -728,35 +788,95 @@
     class Config:
         extra = Extra.allow
 
     image_uri: str
     """
     Input image.
     """
+    store: Optional[str] = None
+    """
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    """
+    node: Optional[Literal["RealESRGAN"]] = "RealESRGAN"
+    """
+    Selected node.
+    """
+
+
+class UpscaleImageOut(BaseModel):
+    class Config:
+        extra = Extra.allow
+
+    image_uri: str
+    """
+    Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
+    """
+
+
+class RealESRGANIn(BaseModel):
+    class Config:
+        extra = Extra.allow
+
+    image_uri: str
+    """
+    Input image.
+    """
     model: Optional[Literal["real-esrgan-x4"]] = "real-esrgan-x4"
     """
     Selected model.
     """
     store: Optional[str] = None
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
 
 
-class UpscaleImageOut(BaseModel):
+class RealESRGANOut(BaseModel):
     class Config:
         extra = Extra.allow
 
     image_uri: str
     """
     Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
     """
 
 
-class DetectSegmentsIn(BaseModel):
+class SegmentUnderPointIn(BaseModel):
+    class Config:
+        extra = Extra.allow
+
+    image_uri: str
+    """
+    Input image.
+    """
+    point: Point
+    """
+    Point prompt.
+    """
+    store: Optional[str] = None
+    """
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    """
+    node: Optional[Literal["SegmentAnything"]] = "SegmentAnything"
+    """
+    Selected node.
+    """
+
+
+class SegmentUnderPointOut(BaseModel):
+    class Config:
+        extra = Extra.allow
+
+    mask_image_uri: str
+    """
+    Detected segments in 'mask image' format. Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
+    """
+
+
+class SegmentAnythingIn(BaseModel):
     class Config:
         extra = Extra.allow
 
     image_uri: str
     """
     Input image.
     """
@@ -764,25 +884,21 @@
     """
     Point prompts, to detect a segment under the point. One of `point_prompts` or `box_prompts` must be set.
     """
     box_prompts: Optional[List[BoundingBox]] = None
     """
     Box prompts, to detect a segment within the bounding box. One of `point_prompts` or `box_prompts` must be set.
     """
-    model: Optional[Literal["segment-anything"]] = "segment-anything"
-    """
-    Selected model.
-    """
     store: Optional[str] = None
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
 
 
-class DetectSegmentsOut(BaseModel):
+class SegmentAnythingOut(BaseModel):
     class Config:
         extra = Extra.allow
 
     mask_image_uri: str
     """
     Detected segments in 'mask image' format. Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
     """
@@ -906,29 +1022,57 @@
     class Config:
         extra = Extra.allow
 
     text: str
     """
     Input text.
     """
+    store: Optional[str] = None
+    """
+    Use "hosted" to return an audio URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the audio data will be returned as a base64-encoded string.
+    """
+    node: Optional[Literal["XTTSV2"]] = "XTTSV2"
+    """
+    Selected node.
+    """
+
+
+class GenerateSpeechOut(BaseModel):
+    class Config:
+        extra = Extra.allow
+
+    audio_uri: str
+    """
+    Base 64-encoded WAV audio bytes, or a hosted audio url if `store` is provided.
+    """
+
+
+class XTTSV2In(BaseModel):
+    class Config:
+        extra = Extra.allow
+
+    text: str
+    """
+    Input text.
+    """
     audio_uri: Optional[str] = None
     """
     Reference audio used to synthesize the speaker. If unset, a default speaker voice will be used.
     """
     language: Optional[str] = "en"
     """
     Language of input text. Supported languages: `en, de, fr, es, it, pt, pl, zh, ar, cs, ru, nl, tr, hu, ko`.
     """
     store: Optional[str] = None
     """
     Use "hosted" to return an audio URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the audio data will be returned as a base64-encoded string.
     """
 
 
-class GenerateSpeechOut(BaseModel):
+class XTTSV2Out(BaseModel):
     class Config:
         extra = Extra.allow
 
     audio_uri: str
     """
     Base 64-encoded WAV audio bytes, or a hosted audio url if `store` is provided.
     """
@@ -1190,15 +1334,15 @@
 
     embeddings: List[Embedding]
     """
     Generated embeddings.
     """
 
 
-class VectorStoreParams(BaseModel):
+class CreateVectorStoreIn(BaseModel):
     class Config:
         extra = Extra.allow
 
     name: Annotated[str, Field(max_length=63, min_length=1)]
     """
     Vector store name.
     """
@@ -1216,15 +1360,72 @@
     """
     metric: Optional[Literal["cosine", "l2", "inner"]] = "inner"
     """
     The distance metric to construct the index with.
     """
 
 
-class DeleteVectorStoreParams(BaseModel):
+class CreateVectorStoreOut(BaseModel):
+    class Config:
+        extra = Extra.allow
+
+    name: Annotated[str, Field(max_length=63, min_length=1)]
+    """
+    Vector store name.
+    """
+    model: Literal["jina-v2", "clip"]
+    """
+    Selected embedding model
+    """
+    m: Annotated[int, Field(ge=1, le=64)]
+    """
+    The max number of connections per layer for the index.
+    """
+    ef_construction: Annotated[int, Field(ge=1, le=128)]
+    """
+    The size of the dynamic candidate list for constructing the index graph.
+    """
+    metric: Literal["cosine", "l2", "inner"]
+    """
+    The distance metric to construct the index with.
+    """
+
+
+class ListVectorStoresIn(BaseModel):
+    pass
+
+    class Config:
+        extra = Extra.allow
+
+
+class ListVectorStoresOut(BaseModel):
+    class Config:
+        extra = Extra.allow
+
+    stores: Optional[List[CreateVectorStoreOut]] = None
+    """
+    List of vector stores.
+    """
+
+
+class DeleteVectorStoreIn(BaseModel):
+    class Config:
+        extra = Extra.allow
+
+    name: str
+    """
+    Vector store name.
+    """
+    model: Literal["jina-v2", "clip"]
+    """
+    Selected embedding model
+    """
+
+
+class DeleteVectorStoreOut(BaseModel):
     class Config:
         extra = Extra.allow
 
     name: str
     """
     Vector store name.
     """
@@ -1252,15 +1453,15 @@
     """
     metadata: Dict[str, Any]
     """
     Document metadata.
     """
 
 
-class GetVectorsParams(BaseModel):
+class FetchVectorsIn(BaseModel):
     class Config:
         extra = Extra.allow
 
     name: str
     """
     Vector store name.
     """
@@ -1270,39 +1471,45 @@
     """
     ids: Annotated[List[str], Field(max_items=100)]
     """
     Document IDs to retrieve.
     """
 
 
-class GetVectorsResponse(BaseModel):
+class FetchVectorsOut(BaseModel):
     class Config:
         extra = Extra.allow
 
     vectors: List[Vector]
     """
     Retrieved vectors.
     """
 
 
-class VectorUpdateCountResponse(BaseModel):
+class UpdateVectorsOut(BaseModel):
     class Config:
         extra = Extra.allow
 
     count: int
     """
     Number of vectors modified.
     """
 
 
-class UpdateVectorParams(BaseModel):
+class DeleteVectorsOut(BaseModel):
+    class Config:
+        extra = Extra.allow
+
+    count: int
     """
-    Document to update.
+    Number of vectors modified.
     """
 
+
+class UpdateVectorParams(BaseModel):
     class Config:
         extra = Extra.allow
 
     id: str
     """
     Document ID.
     """
@@ -1312,15 +1519,15 @@
     """
     metadata: Optional[Dict[str, Any]] = None
     """
     Document metadata.
     """
 
 
-class UpdateVectorsParams(BaseModel):
+class UpdateVectorsIn(BaseModel):
     class Config:
         extra = Extra.allow
 
     name: str
     """
     Vector store name.
     """
@@ -1330,15 +1537,15 @@
     """
     vectors: Annotated[List[UpdateVectorParams], Field(max_items=100)]
     """
     Vectors to upsert.
     """
 
 
-class DeleteVectorsParams(BaseModel):
+class DeleteVectorsIn(BaseModel):
     class Config:
         extra = Extra.allow
 
     name: str
     """
     Vector store name.
     """
@@ -1348,15 +1555,15 @@
     """
     ids: Annotated[List[str], Field(max_items=100)]
     """
     Document IDs to delete.
     """
 
 
-class QueryVectorStoreParams(BaseModel):
+class QueryVectorStoreIn(BaseModel):
     class Config:
         extra = Extra.allow
 
     name: str
     """
     Vector store to query against.
     """
@@ -1420,15 +1627,15 @@
     """
     metadata: Optional[Dict[str, Any]] = None
     """
     Document metadata.
     """
 
 
-class QueryVectorStoreResponse(BaseModel):
+class QueryVectorStoreOut(BaseModel):
     class Config:
         extra = Extra.allow
 
     results: List[List[VectorStoreQueryResult]]
     """
     Query results.
     """
```

### Comparing `substrate-120240403.0.2/substrate/core/sb.py` & `substrate-120240405.0.2/substrate/core/sb.py`

 * *Files identical despite different names*

### Comparing `substrate-120240403.0.2/substrate/dataclass_models.py` & `substrate-120240405.0.2/substrate/dataclass_models.py`

 * *Files 12% similar despite different names*

```diff
@@ -591,26 +591,50 @@
     """
     Input image.
     """
     mask_image_uri: str
     """
     Mask image that controls which pixels are inpainted.
     """
-    model: Optional[Literal["big-lama"]] = "big-lama"
+    store: Optional[str] = None
     """
-    Selected model.
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    """
+    node: Optional[Literal["BigLaMa"]] = "BigLaMa"
+    """
+    Selected node.
+    """
+
+
+@dataclass
+class FillMaskOut:
+    image_uri: str
+    """
+    Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
+    """
+
+
+@dataclass
+class BigLaMaIn:
+    image_uri: str
+    """
+    Input image.
+    """
+    mask_image_uri: str
+    """
+    Mask image that controls which pixels are inpainted.
     """
     store: Optional[str] = None
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
 
 
 @dataclass
-class FillMaskOut:
+class BigLaMaOut:
     image_uri: str
     """
     Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
     """
 
 
 @dataclass
@@ -623,82 +647,158 @@
     """
     Return a mask image instead of the original content.
     """
     background_color: Optional[str] = None
     """
     Hex value background color. Transparent if unset.
     """
-    model: Optional[Literal["isnet"]] = "isnet"
+    store: Optional[str] = None
     """
-    Selected model.
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    """
+    node: Optional[Literal["DISISNet"]] = "DISISNet"
+    """
+    Selected node.
+    """
+
+
+@dataclass
+class RemoveBackgroundOut:
+    image_uri: str
+    """
+    Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
+    """
+
+
+@dataclass
+class DISISNetIn:
+    image_uri: str
+    """
+    Input image.
+    """
+    return_mask: Optional[bool] = None
+    """
+    Return a mask image instead of the original content.
+    """
+    background_color: Optional[str] = None
+    """
+    Hex value background color. Transparent if unset.
     """
     store: Optional[str] = None
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
 
 
 @dataclass
-class RemoveBackgroundOut:
+class DISISNetOut:
     image_uri: str
     """
     Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
     """
 
 
 @dataclass
 class UpscaleImageIn:
     image_uri: str
     """
     Input image.
     """
+    store: Optional[str] = None
+    """
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    """
+    node: Optional[Literal["RealESRGAN"]] = "RealESRGAN"
+    """
+    Selected node.
+    """
+
+
+@dataclass
+class UpscaleImageOut:
+    image_uri: str
+    """
+    Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
+    """
+
+
+@dataclass
+class RealESRGANIn:
+    image_uri: str
+    """
+    Input image.
+    """
     model: Optional[Literal["real-esrgan-x4"]] = "real-esrgan-x4"
     """
     Selected model.
     """
     store: Optional[str] = None
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
 
 
 @dataclass
-class UpscaleImageOut:
+class RealESRGANOut:
     image_uri: str
     """
     Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
     """
 
 
 @dataclass
-class DetectSegmentsIn:
+class SegmentUnderPointIn:
+    image_uri: str
+    """
+    Input image.
+    """
+    point: Point
+    """
+    Point prompt.
+    """
+    store: Optional[str] = None
+    """
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    """
+    node: Optional[Literal["SegmentAnything"]] = "SegmentAnything"
+    """
+    Selected node.
+    """
+
+
+@dataclass
+class SegmentUnderPointOut:
+    mask_image_uri: str
+    """
+    Detected segments in 'mask image' format. Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
+    """
+
+
+@dataclass
+class SegmentAnythingIn:
     image_uri: str
     """
     Input image.
     """
     point_prompts: Optional[List[Point]] = None
     """
     Point prompts, to detect a segment under the point. One of `point_prompts` or `box_prompts` must be set.
     """
     box_prompts: Optional[List[BoundingBox]] = None
     """
     Box prompts, to detect a segment within the bounding box. One of `point_prompts` or `box_prompts` must be set.
     """
-    model: Optional[Literal["segment-anything"]] = "segment-anything"
-    """
-    Selected model.
-    """
     store: Optional[str] = None
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
 
 
 @dataclass
-class DetectSegmentsOut:
+class SegmentAnythingOut:
     mask_image_uri: str
     """
     Detected segments in 'mask image' format. Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
     """
 
 
 @dataclass
@@ -807,14 +907,38 @@
 
 @dataclass
 class GenerateSpeechIn:
     text: str
     """
     Input text.
     """
+    store: Optional[str] = None
+    """
+    Use "hosted" to return an audio URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the audio data will be returned as a base64-encoded string.
+    """
+    node: Optional[Literal["XTTSV2"]] = "XTTSV2"
+    """
+    Selected node.
+    """
+
+
+@dataclass
+class GenerateSpeechOut:
+    audio_uri: str
+    """
+    Base 64-encoded WAV audio bytes, or a hosted audio url if `store` is provided.
+    """
+
+
+@dataclass
+class XTTSV2In:
+    text: str
+    """
+    Input text.
+    """
     audio_uri: Optional[str] = None
     """
     Reference audio used to synthesize the speaker. If unset, a default speaker voice will be used.
     """
     language: Optional[str] = "en"
     """
     Language of input text. Supported languages: `en, de, fr, es, it, pt, pl, zh, ar, cs, ru, nl, tr, hu, ko`.
@@ -822,15 +946,15 @@
     store: Optional[str] = None
     """
     Use "hosted" to return an audio URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the audio data will be returned as a base64-encoded string.
     """
 
 
 @dataclass
-class GenerateSpeechOut:
+class XTTSV2Out:
     audio_uri: str
     """
     Base 64-encoded WAV audio bytes, or a hosted audio url if `store` is provided.
     """
 
 
 @dataclass
@@ -1058,15 +1182,15 @@
     embeddings: List[Embedding]
     """
     Generated embeddings.
     """
 
 
 @dataclass
-class VectorStoreParams:
+class CreateVectorStoreIn:
     name: str
     """
     Vector store name.
     """
     model: Literal["jina-v2", "clip"]
     """
     Selected embedding model
@@ -1082,15 +1206,64 @@
     metric: Optional[Literal["cosine", "l2", "inner"]] = "inner"
     """
     The distance metric to construct the index with.
     """
 
 
 @dataclass
-class DeleteVectorStoreParams:
+class CreateVectorStoreOut:
+    name: str
+    """
+    Vector store name.
+    """
+    model: Literal["jina-v2", "clip"]
+    """
+    Selected embedding model
+    """
+    m: int
+    """
+    The max number of connections per layer for the index.
+    """
+    ef_construction: int
+    """
+    The size of the dynamic candidate list for constructing the index graph.
+    """
+    metric: Literal["cosine", "l2", "inner"]
+    """
+    The distance metric to construct the index with.
+    """
+
+
+@dataclass
+class ListVectorStoresIn:
+    pass
+
+
+@dataclass
+class ListVectorStoresOut:
+    stores: Optional[List[CreateVectorStoreOut]] = None
+    """
+    List of vector stores.
+    """
+
+
+@dataclass
+class DeleteVectorStoreIn:
+    name: str
+    """
+    Vector store name.
+    """
+    model: Literal["jina-v2", "clip"]
+    """
+    Selected embedding model
+    """
+
+
+@dataclass
+class DeleteVectorStoreOut:
     name: str
     """
     Vector store name.
     """
     model: Literal["jina-v2", "clip"]
     """
     Selected embedding model
@@ -1114,15 +1287,15 @@
     metadata: Dict[str, Any]
     """
     Document metadata.
     """
 
 
 @dataclass
-class GetVectorsParams:
+class FetchVectorsIn:
     name: str
     """
     Vector store name.
     """
     model: Literal["jina-v2", "clip"]
     """
     Selected embedding model
@@ -1130,35 +1303,39 @@
     ids: List[str]
     """
     Document IDs to retrieve.
     """
 
 
 @dataclass
-class GetVectorsResponse:
+class FetchVectorsOut:
     vectors: List[Vector]
     """
     Retrieved vectors.
     """
 
 
 @dataclass
-class VectorUpdateCountResponse:
+class UpdateVectorsOut:
     count: int
     """
     Number of vectors modified.
     """
 
 
 @dataclass
-class UpdateVectorParams:
+class DeleteVectorsOut:
+    count: int
     """
-    Document to update.
+    Number of vectors modified.
     """
 
+
+@dataclass
+class UpdateVectorParams:
     id: str
     """
     Document ID.
     """
     vector: Optional[List[float]] = None
     """
     Embedding vector.
@@ -1166,15 +1343,15 @@
     metadata: Optional[Dict[str, Any]] = None
     """
     Document metadata.
     """
 
 
 @dataclass
-class UpdateVectorsParams:
+class UpdateVectorsIn:
     name: str
     """
     Vector store name.
     """
     model: Literal["jina-v2", "clip"]
     """
     Selected embedding model
@@ -1182,15 +1359,15 @@
     vectors: List[UpdateVectorParams]
     """
     Vectors to upsert.
     """
 
 
 @dataclass
-class DeleteVectorsParams:
+class DeleteVectorsIn:
     name: str
     """
     Vector store name.
     """
     model: Literal["jina-v2", "clip"]
     """
     Selected embedding model
@@ -1198,15 +1375,15 @@
     ids: List[str]
     """
     Document IDs to delete.
     """
 
 
 @dataclass
-class QueryVectorStoreParams:
+class QueryVectorStoreIn:
     name: str
     """
     Vector store to query against.
     """
     model: Literal["jina-v2", "clip"]
     """
     Selected embedding model
@@ -1266,15 +1443,15 @@
     metadata: Optional[Dict[str, Any]] = None
     """
     Document metadata.
     """
 
 
 @dataclass
-class QueryVectorStoreResponse:
+class QueryVectorStoreOut:
     results: List[List[VectorStoreQueryResult]]
     """
     Query results.
     """
     name: Optional[str] = None
     """
     Vector store name.
```

### Comparing `substrate-120240403.0.2/substrate/future_dataclass_models.py` & `substrate-120240405.0.2/substrate/future_dataclass_models.py`

 * *Files 8% similar despite different names*

```diff
@@ -843,28 +843,64 @@
     Input image.
     """
     mask_image_uri: str
     """
     (Future reference)
     Mask image that controls which pixels are inpainted.
     """
-    model: Optional[Literal["big-lama"]] = "big-lama"
+    store: Optional[str] = None
     """
     (Future reference)
-    Selected model.
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    """
+    node: Optional[Literal["BigLaMa"]] = "BigLaMa"
+    """
+    (Future reference)
+    Selected node.
+    """
+
+
+@dataclass
+class FutureFillMaskOut:
+    """
+    (Future reference)
+    """
+
+    image_uri: str
+    """
+    (Future reference)
+    Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
+    """
+
+
+@dataclass
+class FutureBigLaMaIn:
+    """
+    (Future reference)
+    """
+
+    image_uri: str
+    """
+    (Future reference)
+    Input image.
+    """
+    mask_image_uri: str
+    """
+    (Future reference)
+    Mask image that controls which pixels are inpainted.
     """
     store: Optional[str] = None
     """
     (Future reference)
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
 
 
 @dataclass
-class FutureFillMaskOut:
+class FutureBigLaMaOut:
     """
     (Future reference)
     """
 
     image_uri: str
     """
     (Future reference)
@@ -889,28 +925,69 @@
     Return a mask image instead of the original content.
     """
     background_color: Optional[str] = None
     """
     (Future reference)
     Hex value background color. Transparent if unset.
     """
-    model: Optional[Literal["isnet"]] = "isnet"
+    store: Optional[str] = None
     """
     (Future reference)
-    Selected model.
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    """
+    node: Optional[Literal["DISISNet"]] = "DISISNet"
+    """
+    (Future reference)
+    Selected node.
+    """
+
+
+@dataclass
+class FutureRemoveBackgroundOut:
+    """
+    (Future reference)
+    """
+
+    image_uri: str
+    """
+    (Future reference)
+    Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
+    """
+
+
+@dataclass
+class FutureDISISNetIn:
+    """
+    (Future reference)
+    """
+
+    image_uri: str
+    """
+    (Future reference)
+    Input image.
+    """
+    return_mask: Optional[bool] = None
+    """
+    (Future reference)
+    Return a mask image instead of the original content.
+    """
+    background_color: Optional[str] = None
+    """
+    (Future reference)
+    Hex value background color. Transparent if unset.
     """
     store: Optional[str] = None
     """
     (Future reference)
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
 
 
 @dataclass
-class FutureRemoveBackgroundOut:
+class FutureDISISNetOut:
     """
     (Future reference)
     """
 
     image_uri: str
     """
     (Future reference)
@@ -925,41 +1002,118 @@
     """
 
     image_uri: str
     """
     (Future reference)
     Input image.
     """
+    store: Optional[str] = None
+    """
+    (Future reference)
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    """
+    node: Optional[Literal["RealESRGAN"]] = "RealESRGAN"
+    """
+    (Future reference)
+    Selected node.
+    """
+
+
+@dataclass
+class FutureUpscaleImageOut:
+    """
+    (Future reference)
+    """
+
+    image_uri: str
+    """
+    (Future reference)
+    Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
+    """
+
+
+@dataclass
+class FutureRealESRGANIn:
+    """
+    (Future reference)
+    """
+
+    image_uri: str
+    """
+    (Future reference)
+    Input image.
+    """
     model: Optional[Literal["real-esrgan-x4"]] = "real-esrgan-x4"
     """
     (Future reference)
     Selected model.
     """
     store: Optional[str] = None
     """
     (Future reference)
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
 
 
 @dataclass
-class FutureUpscaleImageOut:
+class FutureRealESRGANOut:
     """
     (Future reference)
     """
 
     image_uri: str
     """
     (Future reference)
     Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
     """
 
 
 @dataclass
-class FutureDetectSegmentsIn:
+class FutureSegmentUnderPointIn:
+    """
+    (Future reference)
+    """
+
+    image_uri: str
+    """
+    (Future reference)
+    Input image.
+    """
+    point: Point
+    """
+    (Future reference)
+    Point prompt.
+    """
+    store: Optional[str] = None
+    """
+    (Future reference)
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    """
+    node: Optional[Literal["SegmentAnything"]] = "SegmentAnything"
+    """
+    (Future reference)
+    Selected node.
+    """
+
+
+@dataclass
+class FutureSegmentUnderPointOut:
+    """
+    (Future reference)
+    """
+
+    mask_image_uri: str
+    """
+    (Future reference)
+    Detected segments in 'mask image' format. Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
+    """
+
+
+@dataclass
+class FutureSegmentAnythingIn:
     """
     (Future reference)
     """
 
     image_uri: str
     """
     (Future reference)
@@ -971,28 +1125,23 @@
     Point prompts, to detect a segment under the point. One of `point_prompts` or `box_prompts` must be set.
     """
     box_prompts: Optional[List[BoundingBox]] = None
     """
     (Future reference)
     Box prompts, to detect a segment within the bounding box. One of `point_prompts` or `box_prompts` must be set.
     """
-    model: Optional[Literal["segment-anything"]] = "segment-anything"
-    """
-    (Future reference)
-    Selected model.
-    """
     store: Optional[str] = None
     """
     (Future reference)
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
 
 
 @dataclass
-class FutureDetectSegmentsOut:
+class FutureSegmentAnythingOut:
     """
     (Future reference)
     """
 
     mask_image_uri: str
     """
     (Future reference)
@@ -1152,14 +1301,50 @@
     """
 
     text: str
     """
     (Future reference)
     Input text.
     """
+    store: Optional[str] = None
+    """
+    (Future reference)
+    Use "hosted" to return an audio URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the audio data will be returned as a base64-encoded string.
+    """
+    node: Optional[Literal["XTTSV2"]] = "XTTSV2"
+    """
+    (Future reference)
+    Selected node.
+    """
+
+
+@dataclass
+class FutureGenerateSpeechOut:
+    """
+    (Future reference)
+    """
+
+    audio_uri: str
+    """
+    (Future reference)
+    Base 64-encoded WAV audio bytes, or a hosted audio url if `store` is provided.
+    """
+
+
+@dataclass
+class FutureXTTSV2In:
+    """
+    (Future reference)
+    """
+
+    text: str
+    """
+    (Future reference)
+    Input text.
+    """
     audio_uri: Optional[str] = None
     """
     (Future reference)
     Reference audio used to synthesize the speaker. If unset, a default speaker voice will be used.
     """
     language: Optional[str] = "en"
     """
@@ -1170,15 +1355,15 @@
     """
     (Future reference)
     Use "hosted" to return an audio URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the audio data will be returned as a base64-encoded string.
     """
 
 
 @dataclass
-class FutureGenerateSpeechOut:
+class FutureXTTSV2Out:
     """
     (Future reference)
     """
 
     audio_uri: str
     """
     (Future reference)
@@ -1516,15 +1701,15 @@
     """
     (Future reference)
     Generated embeddings.
     """
 
 
 @dataclass
-class VectorStoreParams:
+class FutureCreateVectorStoreIn:
     """
     (Future reference)
     """
 
     name: str
     """
     (Future reference)
@@ -1549,15 +1734,88 @@
     """
     (Future reference)
     The distance metric to construct the index with.
     """
 
 
 @dataclass
-class DeleteVectorStoreParams:
+class FutureCreateVectorStoreOut:
+    """
+    (Future reference)
+    """
+
+    name: str
+    """
+    (Future reference)
+    Vector store name.
+    """
+    model: Literal["jina-v2", "clip"]
+    """
+    (Future reference)
+    Selected embedding model
+    """
+    m: int
+    """
+    (Future reference)
+    The max number of connections per layer for the index.
+    """
+    ef_construction: int
+    """
+    (Future reference)
+    The size of the dynamic candidate list for constructing the index graph.
+    """
+    metric: Literal["cosine", "l2", "inner"]
+    """
+    (Future reference)
+    The distance metric to construct the index with.
+    """
+
+
+@dataclass
+class FutureListVectorStoresIn:
+    """
+    (Future reference)
+    """
+
+    pass
+
+
+@dataclass
+class FutureListVectorStoresOut:
+    """
+    (Future reference)
+    """
+
+    stores: Optional[List[FutureCreateVectorStoreOut]] = None
+    """
+    (Future reference)
+    List of vector stores.
+    """
+
+
+@dataclass
+class FutureDeleteVectorStoreIn:
+    """
+    (Future reference)
+    """
+
+    name: str
+    """
+    (Future reference)
+    Vector store name.
+    """
+    model: Literal["jina-v2", "clip"]
+    """
+    (Future reference)
+    Selected embedding model
+    """
+
+
+@dataclass
+class FutureDeleteVectorStoreOut:
     """
     (Future reference)
     """
 
     name: str
     """
     (Future reference)
@@ -1591,15 +1849,15 @@
     """
     (Future reference)
     Document metadata.
     """
 
 
 @dataclass
-class GetVectorsParams:
+class FutureFetchVectorsIn:
     """
     (Future reference)
     """
 
     name: str
     """
     (Future reference)
@@ -1614,28 +1872,41 @@
     """
     (Future reference)
     Document IDs to retrieve.
     """
 
 
 @dataclass
-class GetVectorsResponse:
+class FutureFetchVectorsOut:
     """
     (Future reference)
     """
 
     vectors: List[Vector]
     """
     (Future reference)
     Retrieved vectors.
     """
 
 
 @dataclass
-class VectorUpdateCountResponse:
+class FutureUpdateVectorsOut:
+    """
+    (Future reference)
+    """
+
+    count: int
+    """
+    (Future reference)
+    Number of vectors modified.
+    """
+
+
+@dataclass
+class FutureDeleteVectorsOut:
     """
     (Future reference)
     """
 
     count: int
     """
     (Future reference)
@@ -1643,15 +1914,14 @@
     """
 
 
 @dataclass
 class UpdateVectorParams:
     """
     (Future reference)
-    Document to update.
     """
 
     id: str
     """
     (Future reference)
     Document ID.
     """
@@ -1664,15 +1934,15 @@
     """
     (Future reference)
     Document metadata.
     """
 
 
 @dataclass
-class UpdateVectorsParams:
+class FutureUpdateVectorsIn:
     """
     (Future reference)
     """
 
     name: str
     """
     (Future reference)
@@ -1687,15 +1957,15 @@
     """
     (Future reference)
     Vectors to upsert.
     """
 
 
 @dataclass
-class DeleteVectorsParams:
+class FutureDeleteVectorsIn:
     """
     (Future reference)
     """
 
     name: str
     """
     (Future reference)
@@ -1710,15 +1980,15 @@
     """
     (Future reference)
     Document IDs to delete.
     """
 
 
 @dataclass
-class QueryVectorStoreParams:
+class FutureQueryVectorStoreIn:
     """
     (Future reference)
     """
 
     name: str
     """
     (Future reference)
@@ -1801,15 +2071,15 @@
     """
     (Future reference)
     Document metadata.
     """
 
 
 @dataclass
-class QueryVectorStoreResponse:
+class FutureQueryVectorStoreOut:
     """
     (Future reference)
     """
 
     results: List[List[VectorStoreQueryResult]]
     """
     (Future reference)
```

### Comparing `substrate-120240403.0.2/substrate/nodes.py` & `substrate-120240405.0.2/substrate/nodes.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,93 +1,129 @@
 """
 ꩜ Substrate
 @GENERATED FILE
-20240403.20240403
+20240405.20240405
 """
 
 from .substrate import SubstrateResponse
 from .core.corenode import CoreNode
 from .dataclass_models import (
     CLIPOut,
     JinaV2Out,
+    XTTSV2Out,
+    BigLaMaOut,
+    DISISNetOut,
     FillMaskOut,
     EmbedTextOut,
     EmbedImageOut,
+    RealESRGANOut,
+    FetchVectorsOut,
     Firellava13BOut,
     GenerateJSONOut,
     GenerateTextOut,
     UpscaleImageOut,
+    DeleteVectorsOut,
     GenerateImageOut,
-    DetectSegmentsOut,
+    UpdateVectorsOut,
     GenerateSpeechOut,
     MultiEmbedTextOut,
     MultiEmbedImageOut,
+    SegmentAnythingOut,
     TranscribeMediaOut,
+    ListVectorStoresOut,
+    QueryVectorStoreOut,
     RemoveBackgroundOut,
+    CreateVectorStoreOut,
+    DeleteVectorStoreOut,
     Mistral7BInstructOut,
     MultiGenerateJSONOut,
     MultiGenerateTextOut,
+    SegmentUnderPointOut,
     StableDiffusionXLOut,
     GenerateTextVisionOut,
     MultiGenerateImageOut,
     GenerativeEditImageOut,
     MultiGenerativeEditImageOut,
     StableDiffusionXLInpaintOut,
     StableDiffusionXLIPAdapterOut,
     StableDiffusionXLControlNetOut,
 )
 from .typeddict_models import (
     CLIPIn,
     JinaV2In,
+    XTTSV2In,
+    BigLaMaIn,
+    DISISNetIn,
     FillMaskIn,
     EmbedTextIn,
     EmbedImageIn,
+    RealESRGANIn,
+    FetchVectorsIn,
     Firellava13BIn,
     GenerateJSONIn,
     GenerateTextIn,
     UpscaleImageIn,
+    DeleteVectorsIn,
     GenerateImageIn,
-    DetectSegmentsIn,
+    UpdateVectorsIn,
     GenerateSpeechIn,
     MultiEmbedTextIn,
     MultiEmbedImageIn,
+    SegmentAnythingIn,
     TranscribeMediaIn,
+    ListVectorStoresIn,
+    QueryVectorStoreIn,
     RemoveBackgroundIn,
+    CreateVectorStoreIn,
+    DeleteVectorStoreIn,
     Mistral7BInstructIn,
     MultiGenerateJSONIn,
     MultiGenerateTextIn,
+    SegmentUnderPointIn,
     StableDiffusionXLIn,
     GenerateTextVisionIn,
     MultiGenerateImageIn,
     GenerativeEditImageIn,
     MultiGenerativeEditImageIn,
     StableDiffusionXLInpaintIn,
     StableDiffusionXLIPAdapterIn,
     StableDiffusionXLControlNetIn,
 )
 from .future_dataclass_models import (
     FutureCLIPOut,
     FutureJinaV2Out,
+    FutureXTTSV2Out,
+    FutureBigLaMaOut,
+    FutureDISISNetOut,
     FutureFillMaskOut,
     FutureEmbedTextOut,
     FutureEmbedImageOut,
+    FutureRealESRGANOut,
+    FutureFetchVectorsOut,
     FutureFirellava13BOut,
     FutureGenerateJSONOut,
     FutureGenerateTextOut,
     FutureUpscaleImageOut,
+    FutureDeleteVectorsOut,
     FutureGenerateImageOut,
-    FutureDetectSegmentsOut,
+    FutureUpdateVectorsOut,
     FutureGenerateSpeechOut,
     FutureMultiEmbedTextOut,
     FutureMultiEmbedImageOut,
+    FutureSegmentAnythingOut,
     FutureTranscribeMediaOut,
+    FutureListVectorStoresOut,
+    FutureQueryVectorStoreOut,
     FutureRemoveBackgroundOut,
+    FutureCreateVectorStoreOut,
+    FutureDeleteVectorStoreOut,
     FutureMistral7BInstructOut,
     FutureMultiGenerateJSONOut,
     FutureMultiGenerateTextOut,
+    FutureSegmentUnderPointOut,
     FutureStableDiffusionXLOut,
     FutureGenerateTextVisionOut,
     FutureMultiGenerateImageOut,
     FutureGenerativeEditImageOut,
     FutureMultiGenerativeEditImageOut,
     FutureStableDiffusionXLInpaintOut,
     FutureStableDiffusionXLIPAdapterOut,
@@ -328,15 +364,15 @@
         https://substrate.run/library#GenerateTextVision
         """
         return super().future  # type: ignore
 
 
 class Mistral7BInstruct(CoreNode):
     """
-    Generate text using Mistral 7B Instruct.
+    Generate text using [Mistral 7B Instruct](https://mistral.ai/news/announcing-mistral-7b).
 
     https://substrate.run/library#Mistral7BInstruct
     """
 
     def __init__(self, args: Mistral7BInstructIn):
         """
         Input arguments: `prompt`, `num_choices`, `json_schema` (optional), `temperature` (optional), `max_tokens` (optional)
@@ -375,15 +411,15 @@
         https://substrate.run/library#Mistral7BInstruct
         """
         return super().future  # type: ignore
 
 
 class Firellava13B(CoreNode):
     """
-    Generate text with image input using FireLLaVA 13B.
+    Generate text with image input using [FireLLaVA 13B](https://fireworks.ai/blog/firellava-the-first-commercially-permissive-oss-llava-model).
 
     https://substrate.run/library#Firellava13B
     """
 
     def __init__(self, args: Firellava13BIn):
         """
         Input arguments: `prompt`, `image_uris`, `temperature` (optional), `max_tokens` (optional)
@@ -610,15 +646,15 @@
         https://substrate.run/library#MultiGenerativeEditImage
         """
         return super().future  # type: ignore
 
 
 class StableDiffusionXL(CoreNode):
     """
-    Generate an image using Stable Diffusion XL.
+    Generate an image using [Stable Diffusion XL](https://arxiv.org/abs/2307.01952).
 
     https://substrate.run/library#StableDiffusionXL
     """
 
     def __init__(self, args: StableDiffusionXLIn):
         """
         Input arguments: `prompt`, `negative_prompt` (optional), `steps` (optional), `num_images` (optional), `store` (optional), `height` (optional), `width` (optional), `seeds` (optional), `guidance_scale` (optional)
@@ -657,15 +693,15 @@
         https://substrate.run/library#StableDiffusionXL
         """
         return super().future  # type: ignore
 
 
 class StableDiffusionXLInpaint(CoreNode):
     """
-    Inpaint an image using Stable Diffusion XL.
+    Edit an image using [Stable Diffusion XL](https://arxiv.org/abs/2307.01952). Supports inpainting (edit part of the image with a mask) and image-to-image (edit the full image).
 
     https://substrate.run/library#StableDiffusionXLInpaint
     """
 
     def __init__(self, args: StableDiffusionXLInpaintIn):
         """
         Input arguments: `image_uri`, `prompt`, `mask_image_uri` (optional), `num_images`, `output_resolution` (optional), `negative_prompt` (optional), `store` (optional), `strength` (optional), `seeds` (optional)
@@ -704,15 +740,15 @@
         https://substrate.run/library#StableDiffusionXLInpaint
         """
         return super().future  # type: ignore
 
 
 class StableDiffusionXLIPAdapter(CoreNode):
     """
-    Generate an image using Stable Diffusion XL with an image prompt.
+    Generate an image with an image prompt, using Stable Diffusion XL with [IP-Adapter](https://arxiv.org/abs/2308.06721).
 
     https://substrate.run/library#StableDiffusionXLIPAdapter
     """
 
     def __init__(self, args: StableDiffusionXLIPAdapterIn):
         """
         Input arguments: `prompt`, `image_prompt_uri` (optional), `num_images`, `ip_adapter_scale` (optional), `negative_prompt` (optional), `store` (optional), `width` (optional), `height` (optional), `seeds` (optional)
@@ -751,15 +787,15 @@
         https://substrate.run/library#StableDiffusionXLIPAdapter
         """
         return super().future  # type: ignore
 
 
 class StableDiffusionXLControlNet(CoreNode):
     """
-    Generate an image using Stable Diffusion XL structuring generation with an input image.
+    Generate an image with generation structured by an input image, using Stable Diffusion XL with [ControlNet](https://arxiv.org/abs/2302.05543).
 
     https://substrate.run/library#StableDiffusionXLControlNet
     """
 
     def __init__(self, args: StableDiffusionXLControlNetIn):
         """
         Input arguments: `image_uri`, `control_method`, `prompt`, `num_images`, `output_resolution` (optional), `negative_prompt` (optional), `store` (optional), `conditioning_scale` (optional), `seeds` (optional)
@@ -798,22 +834,22 @@
         https://substrate.run/library#StableDiffusionXLControlNet
         """
         return super().future  # type: ignore
 
 
 class FillMask(CoreNode):
     """
-    Edit an image with a generative model.
+    Fill (inpaint) part of an image, e.g. to 'remove' an object.
 
     https://substrate.run/library#FillMask
     """
 
     def __init__(self, args: FillMaskIn):
         """
-        Input arguments: `image_uri`, `mask_image_uri`, `model` (optional), `store` (optional)
+        Input arguments: `image_uri`, `mask_image_uri`, `store` (optional), `node` (optional)
 
         Output fields: `future.image_uri`
 
         https://substrate.run/library#FillMask
         """
         super().__init__(**args)
         self.node = "FillMask"
@@ -843,24 +879,71 @@
         Output fields: `future.image_uri`
 
         https://substrate.run/library#FillMask
         """
         return super().future  # type: ignore
 
 
+class BigLaMa(CoreNode):
+    """
+    Inpaint a mask using [LaMa](https://github.com/advimman/lama).
+
+    https://substrate.run/library#BigLaMa
+    """
+
+    def __init__(self, args: BigLaMaIn):
+        """
+        Input arguments: `image_uri`, `mask_image_uri`, `store` (optional)
+
+        Output fields: `future.image_uri`
+
+        https://substrate.run/library#BigLaMa
+        """
+        super().__init__(**args)
+        self.node = "BigLaMa"
+
+    def output(self, response: SubstrateResponse) -> BigLaMaOut:
+        """
+        Retrieve this node's output from a response.
+
+        Output fields: `future.image_uri`
+
+        https://substrate.run/library#BigLaMa
+        """
+        klass = BigLaMaOut
+        json = response.api_response.json
+        if json and json.get("data"):
+            data = json["data"]
+            node_id = self.id
+            if data.get(self.id):
+                return klass(**data[self.id])
+        raise ValueError(f"Node {self.id} not found in response")
+
+    @property
+    def future(self) -> FutureBigLaMaOut:  # type: ignore
+        """
+        Future reference to this node's output.
+
+        Output fields: `future.image_uri`
+
+        https://substrate.run/library#BigLaMa
+        """
+        return super().future  # type: ignore
+
+
 class UpscaleImage(CoreNode):
     """
     Upscale an image.
 
     https://substrate.run/library#UpscaleImage
     """
 
     def __init__(self, args: UpscaleImageIn):
         """
-        Input arguments: `image_uri`, `model` (optional), `store` (optional)
+        Input arguments: `image_uri`, `store` (optional), `node` (optional)
 
         Output fields: `future.image_uri`
 
         https://substrate.run/library#UpscaleImage
         """
         super().__init__(**args)
         self.node = "UpscaleImage"
@@ -890,24 +973,71 @@
         Output fields: `future.image_uri`
 
         https://substrate.run/library#UpscaleImage
         """
         return super().future  # type: ignore
 
 
+class RealESRGAN(CoreNode):
+    """
+    Upscale an image using [RealESRGAN](https://github.com/xinntao/Real-ESRGAN).
+
+    https://substrate.run/library#RealESRGAN
+    """
+
+    def __init__(self, args: RealESRGANIn):
+        """
+        Input arguments: `image_uri`, `model` (optional), `store` (optional)
+
+        Output fields: `future.image_uri`
+
+        https://substrate.run/library#RealESRGAN
+        """
+        super().__init__(**args)
+        self.node = "RealESRGAN"
+
+    def output(self, response: SubstrateResponse) -> RealESRGANOut:
+        """
+        Retrieve this node's output from a response.
+
+        Output fields: `future.image_uri`
+
+        https://substrate.run/library#RealESRGAN
+        """
+        klass = RealESRGANOut
+        json = response.api_response.json
+        if json and json.get("data"):
+            data = json["data"]
+            node_id = self.id
+            if data.get(self.id):
+                return klass(**data[self.id])
+        raise ValueError(f"Node {self.id} not found in response")
+
+    @property
+    def future(self) -> FutureRealESRGANOut:  # type: ignore
+        """
+        Future reference to this node's output.
+
+        Output fields: `future.image_uri`
+
+        https://substrate.run/library#RealESRGAN
+        """
+        return super().future  # type: ignore
+
+
 class RemoveBackground(CoreNode):
     """
     Remove the background from an image, with the option to return the foreground as a mask.
 
     https://substrate.run/library#RemoveBackground
     """
 
     def __init__(self, args: RemoveBackgroundIn):
         """
-        Input arguments: `image_uri`, `return_mask` (optional), `background_color` (optional), `model` (optional), `store` (optional)
+        Input arguments: `image_uri`, `return_mask` (optional), `background_color` (optional), `store` (optional), `node` (optional)
 
         Output fields: `future.image_uri`
 
         https://substrate.run/library#RemoveBackground
         """
         super().__init__(**args)
         self.node = "RemoveBackground"
@@ -937,57 +1067,151 @@
         Output fields: `future.image_uri`
 
         https://substrate.run/library#RemoveBackground
         """
         return super().future  # type: ignore
 
 
-class DetectSegments(CoreNode):
+class DISISNet(CoreNode):
+    """
+    Segment an image using [DIS IS-Net](https://github.com/xuebinqin/DIS).
+
+    https://substrate.run/library#DISISNet
+    """
+
+    def __init__(self, args: DISISNetIn):
+        """
+        Input arguments: `image_uri`, `return_mask` (optional), `background_color` (optional), `store` (optional)
+
+        Output fields: `future.image_uri`
+
+        https://substrate.run/library#DISISNet
+        """
+        super().__init__(**args)
+        self.node = "DISISNet"
+
+    def output(self, response: SubstrateResponse) -> DISISNetOut:
+        """
+        Retrieve this node's output from a response.
+
+        Output fields: `future.image_uri`
+
+        https://substrate.run/library#DISISNet
+        """
+        klass = DISISNetOut
+        json = response.api_response.json
+        if json and json.get("data"):
+            data = json["data"]
+            node_id = self.id
+            if data.get(self.id):
+                return klass(**data[self.id])
+        raise ValueError(f"Node {self.id} not found in response")
+
+    @property
+    def future(self) -> FutureDISISNetOut:  # type: ignore
+        """
+        Future reference to this node's output.
+
+        Output fields: `future.image_uri`
+
+        https://substrate.run/library#DISISNet
+        """
+        return super().future  # type: ignore
+
+
+class SegmentUnderPoint(CoreNode):
     """
-    Detect segments in an image given point(s) or bounding box(es).
+    Segment an image under a point and return the segment.
 
-    https://substrate.run/library#DetectSegments
+    https://substrate.run/library#SegmentUnderPoint
     """
 
-    def __init__(self, args: DetectSegmentsIn):
+    def __init__(self, args: SegmentUnderPointIn):
         """
-        Input arguments: `image_uri`, `point_prompts` (optional), `box_prompts` (optional), `model` (optional), `store` (optional)
+        Input arguments: `image_uri`, `point`, `store` (optional), `node` (optional)
 
         Output fields: `future.mask_image_uri`
 
-        https://substrate.run/library#DetectSegments
+        https://substrate.run/library#SegmentUnderPoint
         """
         super().__init__(**args)
-        self.node = "DetectSegments"
+        self.node = "SegmentUnderPoint"
 
-    def output(self, response: SubstrateResponse) -> DetectSegmentsOut:
+    def output(self, response: SubstrateResponse) -> SegmentUnderPointOut:
         """
         Retrieve this node's output from a response.
 
         Output fields: `future.mask_image_uri`
 
-        https://substrate.run/library#DetectSegments
+        https://substrate.run/library#SegmentUnderPoint
         """
-        klass = DetectSegmentsOut
+        klass = SegmentUnderPointOut
         json = response.api_response.json
         if json and json.get("data"):
             data = json["data"]
             node_id = self.id
             if data.get(self.id):
                 return klass(**data[self.id])
         raise ValueError(f"Node {self.id} not found in response")
 
     @property
-    def future(self) -> FutureDetectSegmentsOut:  # type: ignore
+    def future(self) -> FutureSegmentUnderPointOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.mask_image_uri`
 
-        https://substrate.run/library#DetectSegments
+        https://substrate.run/library#SegmentUnderPoint
+        """
+        return super().future  # type: ignore
+
+
+class SegmentAnything(CoreNode):
+    """
+    Segment an image using [SegmentAnything](https://github.com/facebookresearch/segment-anything).
+
+    https://substrate.run/library#SegmentAnything
+    """
+
+    def __init__(self, args: SegmentAnythingIn):
+        """
+        Input arguments: `image_uri`, `point_prompts` (optional), `box_prompts` (optional), `store` (optional)
+
+        Output fields: `future.mask_image_uri`
+
+        https://substrate.run/library#SegmentAnything
+        """
+        super().__init__(**args)
+        self.node = "SegmentAnything"
+
+    def output(self, response: SubstrateResponse) -> SegmentAnythingOut:
+        """
+        Retrieve this node's output from a response.
+
+        Output fields: `future.mask_image_uri`
+
+        https://substrate.run/library#SegmentAnything
+        """
+        klass = SegmentAnythingOut
+        json = response.api_response.json
+        if json and json.get("data"):
+            data = json["data"]
+            node_id = self.id
+            if data.get(self.id):
+                return klass(**data[self.id])
+        raise ValueError(f"Node {self.id} not found in response")
+
+    @property
+    def future(self) -> FutureSegmentAnythingOut:  # type: ignore
+        """
+        Future reference to this node's output.
+
+        Output fields: `future.mask_image_uri`
+
+        https://substrate.run/library#SegmentAnything
         """
         return super().future  # type: ignore
 
 
 class TranscribeMedia(CoreNode):
     """
     Transcribe speech in an audio or video file.
@@ -1040,15 +1264,15 @@
     Generate speech from text.
 
     https://substrate.run/library#GenerateSpeech
     """
 
     def __init__(self, args: GenerateSpeechIn):
         """
-        Input arguments: `text`, `audio_uri` (optional), `language` (optional), `store` (optional)
+        Input arguments: `text`, `store` (optional), `node` (optional)
 
         Output fields: `future.audio_uri`
 
         https://substrate.run/library#GenerateSpeech
         """
         super().__init__(**args)
         self.node = "GenerateSpeech"
@@ -1078,14 +1302,61 @@
         Output fields: `future.audio_uri`
 
         https://substrate.run/library#GenerateSpeech
         """
         return super().future  # type: ignore
 
 
+class XTTSV2(CoreNode):
+    """
+    Generate speech from text using [XTTS v2](https://docs.coqui.ai/en/latest/models/xtts.html).
+
+    https://substrate.run/library#XTTSV2
+    """
+
+    def __init__(self, args: XTTSV2In):
+        """
+        Input arguments: `text`, `audio_uri` (optional), `language` (optional), `store` (optional)
+
+        Output fields: `future.audio_uri`
+
+        https://substrate.run/library#XTTSV2
+        """
+        super().__init__(**args)
+        self.node = "XTTSV2"
+
+    def output(self, response: SubstrateResponse) -> XTTSV2Out:
+        """
+        Retrieve this node's output from a response.
+
+        Output fields: `future.audio_uri`
+
+        https://substrate.run/library#XTTSV2
+        """
+        klass = XTTSV2Out
+        json = response.api_response.json
+        if json and json.get("data"):
+            data = json["data"]
+            node_id = self.id
+            if data.get(self.id):
+                return klass(**data[self.id])
+        raise ValueError(f"Node {self.id} not found in response")
+
+    @property
+    def future(self) -> FutureXTTSV2Out:  # type: ignore
+        """
+        Future reference to this node's output.
+
+        Output fields: `future.audio_uri`
+
+        https://substrate.run/library#XTTSV2
+        """
+        return super().future  # type: ignore
+
+
 class EmbedText(CoreNode):
     """
     Generate embedding for a text document.
 
     https://substrate.run/library#EmbedText
     """
 
@@ -1268,15 +1539,15 @@
         https://substrate.run/library#MultiEmbedImage
         """
         return super().future  # type: ignore
 
 
 class JinaV2(CoreNode):
     """
-    Generate embeddings for multiple text documents using Jina V2.
+    Generate embeddings for multiple text documents using [Jina Embeddings 2](https://arxiv.org/abs/2310.19923).
 
     https://substrate.run/library#JinaV2
     """
 
     def __init__(self, args: JinaV2In):
         """
         Input arguments: `items`, `store` (optional), `embedded_metadata_keys` (optional)
@@ -1315,15 +1586,15 @@
         https://substrate.run/library#JinaV2
         """
         return super().future  # type: ignore
 
 
 class CLIP(CoreNode):
     """
-    Generate embeddings for text or images using CLIP.
+    Generate embeddings for text or images using [CLIP](https://openai.com/research/clip).
 
     https://substrate.run/library#CLIP
     """
 
     def __init__(self, args: CLIPIn):
         """
         Input arguments: `items`, `embedded_metadata_keys` (optional), `store` (optional)
@@ -1358,7 +1629,336 @@
         Future reference to this node's output.
 
         Output fields: `future.embeddings`
 
         https://substrate.run/library#CLIP
         """
         return super().future  # type: ignore
+
+
+class CreateVectorStore(CoreNode):
+    """
+    Create a vector store for storing and querying embeddings.
+
+    https://substrate.run/library#CreateVectorStore
+    """
+
+    def __init__(self, args: CreateVectorStoreIn):
+        """
+        Input arguments: `name`, `model`, `m` (optional), `ef_construction` (optional), `metric` (optional)
+
+        Output fields: `future.name`, `future.model`, `future.m`, `future.ef_construction`, `future.metric`
+
+        https://substrate.run/library#CreateVectorStore
+        """
+        super().__init__(**args)
+        self.node = "CreateVectorStore"
+
+    def output(self, response: SubstrateResponse) -> CreateVectorStoreOut:
+        """
+        Retrieve this node's output from a response.
+
+        Output fields: `future.name`, `future.model`, `future.m`, `future.ef_construction`, `future.metric`
+
+        https://substrate.run/library#CreateVectorStore
+        """
+        klass = CreateVectorStoreOut
+        json = response.api_response.json
+        if json and json.get("data"):
+            data = json["data"]
+            node_id = self.id
+            if data.get(self.id):
+                return klass(**data[self.id])
+        raise ValueError(f"Node {self.id} not found in response")
+
+    @property
+    def future(self) -> FutureCreateVectorStoreOut:  # type: ignore
+        """
+        Future reference to this node's output.
+
+        Output fields: `future.name`, `future.model`, `future.m`, `future.ef_construction`, `future.metric`
+
+        https://substrate.run/library#CreateVectorStore
+        """
+        return super().future  # type: ignore
+
+
+class ListVectorStores(CoreNode):
+    """
+    List all vector stores.
+
+    https://substrate.run/library#ListVectorStores
+    """
+
+    def __init__(self, args: ListVectorStoresIn):
+        """
+        Input arguments:
+
+        Output fields: `future.stores` (optional)
+
+        https://substrate.run/library#ListVectorStores
+        """
+        super().__init__(**args)
+        self.node = "ListVectorStores"
+
+    def output(self, response: SubstrateResponse) -> ListVectorStoresOut:
+        """
+        Retrieve this node's output from a response.
+
+        Output fields: `future.stores` (optional)
+
+        https://substrate.run/library#ListVectorStores
+        """
+        klass = ListVectorStoresOut
+        json = response.api_response.json
+        if json and json.get("data"):
+            data = json["data"]
+            node_id = self.id
+            if data.get(self.id):
+                return klass(**data[self.id])
+        raise ValueError(f"Node {self.id} not found in response")
+
+    @property
+    def future(self) -> FutureListVectorStoresOut:  # type: ignore
+        """
+        Future reference to this node's output.
+
+        Output fields: `future.stores` (optional)
+
+        https://substrate.run/library#ListVectorStores
+        """
+        return super().future  # type: ignore
+
+
+class DeleteVectorStore(CoreNode):
+    """
+    Delete a vector store.
+
+    https://substrate.run/library#DeleteVectorStore
+    """
+
+    def __init__(self, args: DeleteVectorStoreIn):
+        """
+        Input arguments: `name`, `model`
+
+        Output fields: `future.name`, `future.model`
+
+        https://substrate.run/library#DeleteVectorStore
+        """
+        super().__init__(**args)
+        self.node = "DeleteVectorStore"
+
+    def output(self, response: SubstrateResponse) -> DeleteVectorStoreOut:
+        """
+        Retrieve this node's output from a response.
+
+        Output fields: `future.name`, `future.model`
+
+        https://substrate.run/library#DeleteVectorStore
+        """
+        klass = DeleteVectorStoreOut
+        json = response.api_response.json
+        if json and json.get("data"):
+            data = json["data"]
+            node_id = self.id
+            if data.get(self.id):
+                return klass(**data[self.id])
+        raise ValueError(f"Node {self.id} not found in response")
+
+    @property
+    def future(self) -> FutureDeleteVectorStoreOut:  # type: ignore
+        """
+        Future reference to this node's output.
+
+        Output fields: `future.name`, `future.model`
+
+        https://substrate.run/library#DeleteVectorStore
+        """
+        return super().future  # type: ignore
+
+
+class QueryVectorStore(CoreNode):
+    """
+    Query a vector store for similar vectors.
+
+    https://substrate.run/library#QueryVectorStore
+    """
+
+    def __init__(self, args: QueryVectorStoreIn):
+        """
+        Input arguments: `name`, `model`, `query_ids` (optional), `query_image_uris` (optional), `query_vectors` (optional), `query_strings` (optional), `top_k` (optional), `ef_search` (optional), `include_values` (optional), `include_metadata` (optional), `filters` (optional)
+
+        Output fields: `future.results`, `future.name` (optional), `future.model` (optional), `future.metric` (optional)
+
+        https://substrate.run/library#QueryVectorStore
+        """
+        super().__init__(**args)
+        self.node = "QueryVectorStore"
+
+    def output(self, response: SubstrateResponse) -> QueryVectorStoreOut:
+        """
+        Retrieve this node's output from a response.
+
+        Output fields: `future.results`, `future.name` (optional), `future.model` (optional), `future.metric` (optional)
+
+        https://substrate.run/library#QueryVectorStore
+        """
+        klass = QueryVectorStoreOut
+        json = response.api_response.json
+        if json and json.get("data"):
+            data = json["data"]
+            node_id = self.id
+            if data.get(self.id):
+                return klass(**data[self.id])
+        raise ValueError(f"Node {self.id} not found in response")
+
+    @property
+    def future(self) -> FutureQueryVectorStoreOut:  # type: ignore
+        """
+        Future reference to this node's output.
+
+        Output fields: `future.results`, `future.name` (optional), `future.model` (optional), `future.metric` (optional)
+
+        https://substrate.run/library#QueryVectorStore
+        """
+        return super().future  # type: ignore
+
+
+class FetchVectors(CoreNode):
+    """
+    Fetch vectors from a vector store.
+
+    https://substrate.run/library#FetchVectors
+    """
+
+    def __init__(self, args: FetchVectorsIn):
+        """
+        Input arguments: `name`, `model`, `ids`
+
+        Output fields: `future.vectors`
+
+        https://substrate.run/library#FetchVectors
+        """
+        super().__init__(**args)
+        self.node = "FetchVectors"
+
+    def output(self, response: SubstrateResponse) -> FetchVectorsOut:
+        """
+        Retrieve this node's output from a response.
+
+        Output fields: `future.vectors`
+
+        https://substrate.run/library#FetchVectors
+        """
+        klass = FetchVectorsOut
+        json = response.api_response.json
+        if json and json.get("data"):
+            data = json["data"]
+            node_id = self.id
+            if data.get(self.id):
+                return klass(**data[self.id])
+        raise ValueError(f"Node {self.id} not found in response")
+
+    @property
+    def future(self) -> FutureFetchVectorsOut:  # type: ignore
+        """
+        Future reference to this node's output.
+
+        Output fields: `future.vectors`
+
+        https://substrate.run/library#FetchVectors
+        """
+        return super().future  # type: ignore
+
+
+class UpdateVectors(CoreNode):
+    """
+    Update vectors in a vector store.
+
+    https://substrate.run/library#UpdateVectors
+    """
+
+    def __init__(self, args: UpdateVectorsIn):
+        """
+        Input arguments: `name`, `model`, `vectors`
+
+        Output fields: `future.count`
+
+        https://substrate.run/library#UpdateVectors
+        """
+        super().__init__(**args)
+        self.node = "UpdateVectors"
+
+    def output(self, response: SubstrateResponse) -> UpdateVectorsOut:
+        """
+        Retrieve this node's output from a response.
+
+        Output fields: `future.count`
+
+        https://substrate.run/library#UpdateVectors
+        """
+        klass = UpdateVectorsOut
+        json = response.api_response.json
+        if json and json.get("data"):
+            data = json["data"]
+            node_id = self.id
+            if data.get(self.id):
+                return klass(**data[self.id])
+        raise ValueError(f"Node {self.id} not found in response")
+
+    @property
+    def future(self) -> FutureUpdateVectorsOut:  # type: ignore
+        """
+        Future reference to this node's output.
+
+        Output fields: `future.count`
+
+        https://substrate.run/library#UpdateVectors
+        """
+        return super().future  # type: ignore
+
+
+class DeleteVectors(CoreNode):
+    """
+    Delete vectors in a vector store.
+
+    https://substrate.run/library#DeleteVectors
+    """
+
+    def __init__(self, args: DeleteVectorsIn):
+        """
+        Input arguments: `name`, `model`, `ids`
+
+        Output fields: `future.count`
+
+        https://substrate.run/library#DeleteVectors
+        """
+        super().__init__(**args)
+        self.node = "DeleteVectors"
+
+    def output(self, response: SubstrateResponse) -> DeleteVectorsOut:
+        """
+        Retrieve this node's output from a response.
+
+        Output fields: `future.count`
+
+        https://substrate.run/library#DeleteVectors
+        """
+        klass = DeleteVectorsOut
+        json = response.api_response.json
+        if json and json.get("data"):
+            data = json["data"]
+            node_id = self.id
+            if data.get(self.id):
+                return klass(**data[self.id])
+        raise ValueError(f"Node {self.id} not found in response")
+
+    @property
+    def future(self) -> FutureDeleteVectorsOut:  # type: ignore
+        """
+        Future reference to this node's output.
+
+        Output fields: `future.count`
+
+        https://substrate.run/library#DeleteVectors
+        """
+        return super().future  # type: ignore
```

### Comparing `substrate-120240403.0.2/substrate/substrate.py` & `substrate-120240405.0.2/substrate/substrate.py`

 * *Files identical despite different names*

### Comparing `substrate-120240403.0.2/substrate/typeddict_models.py` & `substrate-120240405.0.2/substrate/typeddict_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -554,25 +554,47 @@
     """
     Input image.
     """
     mask_image_uri: NotRequired[str]
     """
     Mask image that controls which pixels are inpainted.
     """
-    model: NotRequired[Literal["big-lama"]]
+    store: NotRequired[str]
     """
-    (Optional) Selected model.
+    (Optional) Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    """
+    node: NotRequired[Literal["BigLaMa"]]
+    """
+    (Optional) Selected node.
+    """
+
+
+class FillMaskOut(TypedDict):
+    image_uri: NotRequired[str]
+    """
+    Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
+    """
+
+
+class BigLaMaIn(TypedDict):
+    image_uri: NotRequired[str]
+    """
+    Input image.
+    """
+    mask_image_uri: NotRequired[str]
+    """
+    Mask image that controls which pixels are inpainted.
     """
     store: NotRequired[str]
     """
     (Optional) Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
 
 
-class FillMaskOut(TypedDict):
+class BigLaMaOut(TypedDict):
     image_uri: NotRequired[str]
     """
     Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
     """
 
 
 class RemoveBackgroundIn(TypedDict):
@@ -584,77 +606,147 @@
     """
     (Optional) Return a mask image instead of the original content.
     """
     background_color: NotRequired[str]
     """
     (Optional) Hex value background color. Transparent if unset.
     """
-    model: NotRequired[Literal["isnet"]]
+    store: NotRequired[str]
+    """
+    (Optional) Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
-    (Optional) Selected model.
+    node: NotRequired[Literal["DISISNet"]]
+    """
+    (Optional) Selected node.
+    """
+
+
+class RemoveBackgroundOut(TypedDict):
+    image_uri: NotRequired[str]
+    """
+    Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
+    """
+
+
+class DISISNetIn(TypedDict):
+    image_uri: NotRequired[str]
+    """
+    Input image.
+    """
+    return_mask: NotRequired[bool]
+    """
+    (Optional) Return a mask image instead of the original content.
+    """
+    background_color: NotRequired[str]
+    """
+    (Optional) Hex value background color. Transparent if unset.
     """
     store: NotRequired[str]
     """
     (Optional) Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
 
 
-class RemoveBackgroundOut(TypedDict):
+class DISISNetOut(TypedDict):
     image_uri: NotRequired[str]
     """
     Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
     """
 
 
 class UpscaleImageIn(TypedDict):
     image_uri: NotRequired[str]
     """
     Input image.
     """
+    store: NotRequired[str]
+    """
+    (Optional) Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    """
+    node: NotRequired[Literal["RealESRGAN"]]
+    """
+    (Optional) Selected node.
+    """
+
+
+class UpscaleImageOut(TypedDict):
+    image_uri: NotRequired[str]
+    """
+    Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
+    """
+
+
+class RealESRGANIn(TypedDict):
+    image_uri: NotRequired[str]
+    """
+    Input image.
+    """
     model: NotRequired[Literal["real-esrgan-x4"]]
     """
     (Optional) Selected model.
     """
     store: NotRequired[str]
     """
     (Optional) Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
 
 
-class UpscaleImageOut(TypedDict):
+class RealESRGANOut(TypedDict):
     image_uri: NotRequired[str]
     """
     Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
     """
 
 
-class DetectSegmentsIn(TypedDict):
+class SegmentUnderPointIn(TypedDict):
+    image_uri: NotRequired[str]
+    """
+    Input image.
+    """
+    point: NotRequired[Point]
+    """
+    Point prompt.
+    """
+    store: NotRequired[str]
+    """
+    (Optional) Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    """
+    node: NotRequired[Literal["SegmentAnything"]]
+    """
+    (Optional) Selected node.
+    """
+
+
+class SegmentUnderPointOut(TypedDict):
+    mask_image_uri: NotRequired[str]
+    """
+    Detected segments in 'mask image' format. Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
+    """
+
+
+class SegmentAnythingIn(TypedDict):
     image_uri: NotRequired[str]
     """
     Input image.
     """
     point_prompts: NotRequired[List[Point]]
     """
     (Optional) Point prompts, to detect a segment under the point. One of `point_prompts` or `box_prompts` must be set.
     """
     box_prompts: NotRequired[List[BoundingBox]]
     """
     (Optional) Box prompts, to detect a segment within the bounding box. One of `point_prompts` or `box_prompts` must be set.
     """
-    model: NotRequired[Literal["segment-anything"]]
-    """
-    (Optional) Selected model.
-    """
     store: NotRequired[str]
     """
     (Optional) Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
 
 
-class DetectSegmentsOut(TypedDict):
+class SegmentAnythingOut(TypedDict):
     mask_image_uri: NotRequired[str]
     """
     Detected segments in 'mask image' format. Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
     """
 
 
 class TranscribeMediaIn(TypedDict):
@@ -757,29 +849,51 @@
 
 
 class GenerateSpeechIn(TypedDict):
     text: NotRequired[str]
     """
     Input text.
     """
+    store: NotRequired[str]
+    """
+    (Optional) Use "hosted" to return an audio URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the audio data will be returned as a base64-encoded string.
+    """
+    node: NotRequired[Literal["XTTSV2"]]
+    """
+    (Optional) Selected node.
+    """
+
+
+class GenerateSpeechOut(TypedDict):
+    audio_uri: NotRequired[str]
+    """
+    Base 64-encoded WAV audio bytes, or a hosted audio url if `store` is provided.
+    """
+
+
+class XTTSV2In(TypedDict):
+    text: NotRequired[str]
+    """
+    Input text.
+    """
     audio_uri: NotRequired[str]
     """
     (Optional) Reference audio used to synthesize the speaker. If unset, a default speaker voice will be used.
     """
     language: NotRequired[str]
     """
     (Optional) Language of input text. Supported languages: `en, de, fr, es, it, pt, pl, zh, ar, cs, ru, nl, tr, hu, ko`.
     """
     store: NotRequired[str]
     """
     (Optional) Use "hosted" to return an audio URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the audio data will be returned as a base64-encoded string.
     """
 
 
-class GenerateSpeechOut(TypedDict):
+class XTTSV2Out(TypedDict):
     audio_uri: NotRequired[str]
     """
     Base 64-encoded WAV audio bytes, or a hosted audio url if `store` is provided.
     """
 
 
 class Embedding(TypedDict):
@@ -990,15 +1104,15 @@
 class CLIPOut(TypedDict):
     embeddings: NotRequired[List[Embedding]]
     """
     Generated embeddings.
     """
 
 
-class VectorStoreParams(TypedDict):
+class CreateVectorStoreIn(TypedDict):
     name: NotRequired[str]
     """
     Vector store name.
     """
     model: NotRequired[Literal["jina-v2", "clip"]]
     """
     Selected embedding model
@@ -1013,15 +1127,60 @@
     """
     metric: NotRequired[Literal["cosine", "l2", "inner"]]
     """
     (Optional) The distance metric to construct the index with.
     """
 
 
-class DeleteVectorStoreParams(TypedDict):
+class CreateVectorStoreOut(TypedDict):
+    name: NotRequired[str]
+    """
+    Vector store name.
+    """
+    model: NotRequired[Literal["jina-v2", "clip"]]
+    """
+    Selected embedding model
+    """
+    m: NotRequired[int]
+    """
+    The max number of connections per layer for the index.
+    """
+    ef_construction: NotRequired[int]
+    """
+    The size of the dynamic candidate list for constructing the index graph.
+    """
+    metric: NotRequired[Literal["cosine", "l2", "inner"]]
+    """
+    The distance metric to construct the index with.
+    """
+
+
+class ListVectorStoresIn(TypedDict):
+    pass
+
+
+class ListVectorStoresOut(TypedDict):
+    stores: NotRequired[List[CreateVectorStoreOut]]
+    """
+    (Optional) List of vector stores.
+    """
+
+
+class DeleteVectorStoreIn(TypedDict):
+    name: NotRequired[str]
+    """
+    Vector store name.
+    """
+    model: NotRequired[Literal["jina-v2", "clip"]]
+    """
+    Selected embedding model
+    """
+
+
+class DeleteVectorStoreOut(TypedDict):
     name: NotRequired[str]
     """
     Vector store name.
     """
     model: NotRequired[Literal["jina-v2", "clip"]]
     """
     Selected embedding model
@@ -1043,93 +1202,96 @@
     """
     metadata: NotRequired[Dict[str, Any]]
     """
     Document metadata.
     """
 
 
-class GetVectorsParams(TypedDict):
+class FetchVectorsIn(TypedDict):
     name: NotRequired[str]
     """
     Vector store name.
     """
     model: NotRequired[Literal["jina-v2", "clip"]]
     """
     Selected embedding model
     """
     ids: NotRequired[List[str]]
     """
     Document IDs to retrieve.
     """
 
 
-class GetVectorsResponse(TypedDict):
+class FetchVectorsOut(TypedDict):
     vectors: NotRequired[List[Vector]]
     """
     Retrieved vectors.
     """
 
 
-class VectorUpdateCountResponse(TypedDict):
+class UpdateVectorsOut(TypedDict):
     count: NotRequired[int]
     """
     Number of vectors modified.
     """
 
 
-class UpdateVectorParams(TypedDict):
+class DeleteVectorsOut(TypedDict):
+    count: NotRequired[int]
     """
-    Document to update.
+    Number of vectors modified.
     """
 
+
+class UpdateVectorParams(TypedDict):
     id: NotRequired[str]
     """
     Document ID.
     """
     vector: NotRequired[List[float]]
     """
     (Optional) Embedding vector.
     """
     metadata: NotRequired[Dict[str, Any]]
     """
     (Optional) Document metadata.
     """
 
 
-class UpdateVectorsParams(TypedDict):
+class UpdateVectorsIn(TypedDict):
     name: NotRequired[str]
     """
     Vector store name.
     """
     model: NotRequired[Literal["jina-v2", "clip"]]
     """
     Selected embedding model
     """
     vectors: NotRequired[List[UpdateVectorParams]]
     """
     Vectors to upsert.
     """
 
 
-class DeleteVectorsParams(TypedDict):
+class DeleteVectorsIn(TypedDict):
     name: NotRequired[str]
     """
     Vector store name.
     """
     model: NotRequired[Literal["jina-v2", "clip"]]
     """
     Selected embedding model
     """
     ids: NotRequired[List[str]]
     """
     Document IDs to delete.
     """
 
 
-class QueryVectorStoreParams(TypedDict):
+class QueryVectorStoreIn(TypedDict):
     name: NotRequired[str]
     """
     Vector store to query against.
     """
     model: NotRequired[Literal["jina-v2", "clip"]]
     """
     Selected embedding model
@@ -1187,15 +1349,15 @@
     """
     metadata: NotRequired[Dict[str, Any]]
     """
     (Optional) Document metadata.
     """
 
 
-class QueryVectorStoreResponse(TypedDict):
+class QueryVectorStoreOut(TypedDict):
     results: NotRequired[List[List[VectorStoreQueryResult]]]
     """
     Query results.
     """
     name: NotRequired[str]
     """
     (Optional) Vector store name.
```

### Comparing `substrate-120240403.0.2/PKG-INFO` & `substrate-120240405.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: substrate
-Version: 120240403.0.2
+Version: 120240405.0.2
 Summary: Substrate Python SDK
 Author: vprtwn
 Author-email: ben@substrate.run
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

