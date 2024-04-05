# Comparing `tmp/imagery-mapilio-0.0.8.tar.gz` & `tmp/imagery-mapilio-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/imagery-mapilio-0.0.8.tar", last modified: Tue Dec  7 15:03:05 2021, max compression
+gzip compressed data, was "dist/imagery-mapilio-0.0.9.tar", last modified: Mon Feb 28 15:26:27 2022, max compression
```

## Comparing `imagery-mapilio-0.0.8.tar` & `imagery-mapilio-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 15:03:05.000000 imagery-mapilio-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1273 2021-12-07 15:02:29.000000 imagery-mapilio-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 15:03:05.000000 imagery-mapilio-0.0.8/imagery_mapilio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      366 2021-12-07 15:03:05.000000 imagery-mapilio-0.0.8/imagery_mapilio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)      474 2021-12-07 15:03:04.000000 imagery-mapilio-0.0.8/imagery_mapilio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       90 2021-12-07 15:03:04.000000 imagery-mapilio-0.0.8/imagery_mapilio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-07 15:03:04.000000 imagery-mapilio-0.0.8/imagery_mapilio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2021-12-07 15:03:04.000000 imagery-mapilio-0.0.8/imagery_mapilio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      474 2021-12-07 15:03:05.000000 imagery-mapilio-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-12-07 15:03:05.000000 imagery-mapilio-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 15:03:05.000000 imagery-mapilio-0.0.8/imagery/
--rw-r--r--   0 runner    (1001) docker     (121)     3228 2021-12-07 15:02:29.000000 imagery-mapilio-0.0.8/imagery/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (121)      311 2021-12-07 15:02:29.000000 imagery-mapilio-0.0.8/imagery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      227 2021-12-07 15:02:29.000000 imagery-mapilio-0.0.8/imagery/util.py
--rw-r--r--   0 runner    (1001) docker     (121)      655 2021-12-07 15:02:29.000000 imagery-mapilio-0.0.8/imagery/torch_predictor.py
--rw-r--r--   0 runner    (1001) docker     (121)     4175 2021-12-07 15:02:29.000000 imagery-mapilio-0.0.8/imagery/operations.py
--rw-r--r--   0 runner    (1001) docker     (121)      500 2021-12-07 15:02:29.000000 imagery-mapilio-0.0.8/imagery/reflection.py
--rw-r--r--   0 runner    (1001) docker     (121)     8202 2021-12-07 15:02:29.000000 imagery-mapilio-0.0.8/imagery/postprocessor.py
--rw-r--r--   0 runner    (1001) docker     (121)      142 2021-12-07 15:02:29.000000 imagery-mapilio-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 15:26:27.000000 imagery-mapilio-0.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 15:26:27.000000 imagery-mapilio-0.0.9/imagery/
+-rw-r--r--   0 runner    (1001) docker     (121)      500 2022-02-28 15:25:32.000000 imagery-mapilio-0.0.9/imagery/reflection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8202 2022-02-28 15:25:32.000000 imagery-mapilio-0.0.9/imagery/postprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4687 2022-02-28 15:25:32.000000 imagery-mapilio-0.0.9/imagery/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4274 2022-02-28 15:25:32.000000 imagery-mapilio-0.0.9/imagery/operations.py
+-rw-r--r--   0 runner    (1001) docker     (121)      227 2022-02-28 15:25:32.000000 imagery-mapilio-0.0.9/imagery/util.py
+-rw-r--r--   0 runner    (1001) docker     (121)      655 2022-02-28 15:25:32.000000 imagery-mapilio-0.0.9/imagery/torch_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (121)      311 2022-02-28 15:25:32.000000 imagery-mapilio-0.0.9/imagery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1273 2022-02-28 15:25:32.000000 imagery-mapilio-0.0.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-28 15:26:27.000000 imagery-mapilio-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 15:26:27.000000 imagery-mapilio-0.0.9/imagery_mapilio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-02-28 15:26:27.000000 imagery-mapilio-0.0.9/imagery_mapilio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      474 2022-02-28 15:26:27.000000 imagery-mapilio-0.0.9/imagery_mapilio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      366 2022-02-28 15:26:27.000000 imagery-mapilio-0.0.9/imagery_mapilio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       90 2022-02-28 15:26:27.000000 imagery-mapilio-0.0.9/imagery_mapilio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-28 15:26:27.000000 imagery-mapilio-0.0.9/imagery_mapilio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      474 2022-02-28 15:26:27.000000 imagery-mapilio-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      142 2022-02-28 15:25:32.000000 imagery-mapilio-0.0.9/README.md
```

### Comparing `imagery-mapilio-0.0.8/setup.py` & `imagery-mapilio-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `imagery-mapilio-0.0.8/imagery/torch_predictor.py` & `imagery-mapilio-0.0.9/imagery/torch_predictor.py`

 * *Files identical despite different names*

### Comparing `imagery-mapilio-0.0.8/imagery/operations.py` & `imagery-mapilio-0.0.9/imagery/operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
             file_id: specif prediction dir id
 
         Returns:
             write local directory, detected objects as a array, pca angle
         """
         params = Dict(kwargs)
         xmin, ymin, xmax, ymax = [int(item) for item in params.finalBox]
-        detectedObject = params.copyImage[ymin:ymax, xmin:xmax] # if detectedObject dont want color open this
+        detectedObject = params.copyImage[ymin:ymax, xmin:xmax]  # if detectedObject dont want color open this
         if len(params.mask_boundary):
             cv2.polylines(params.image, [params.mask_boundary], True, (0, 255, 0), 3)
             # TODO mask deprecated
             # image_pca, image_rgb = PostProcessor.image_coloring(params.image, params.rgb_mask)
             # detectedObject_pca = image_pca[ymin:ymax, xmin:xmax]
             # detectedObject = image_rgb[ymin:ymax, xmin:xmax]
             # del image_pca
@@ -56,15 +56,18 @@
             cv2.putText(params.image, params.objectId, (cX + 20, cY + 20),
                         cv2.FONT_HERSHEY_SIMPLEX, 0.5, (0, 0, 255), 1)
 
             cv2.rectangle(params.image, (xmin, ymin), (xmax, ymax), (255, 0, 255), thickness=2)
 
         imageNumber = os.path.basename(params.writePaths[1]).split(".")[0]
         imageSaveType = os.path.basename(params.writePaths[1]).split(".")[1]
-        saveName = imageNumber + "_{}.".format(Generator.unique_matchId_generator()) + imageSaveType
+        saveName = imageNumber + "_{}.".format(Generator.unique_matchId_generator()) + imageSaveType + '.jpeg'
+
+        if not saveName in ['jpg', 'jpeg']:
+            saveName = saveName + '.jpeg'
         detectedObjectPath = os.path.join("Exports", params.file_id, "ObjectsImage", saveName)
         cv2.imwrite(detectedObjectPath, detectedObject)
 
         del params.copyImage
 
         return detectedObjectPath, params.image
 
@@ -73,15 +76,15 @@
         return cv2.imread(detectedObjectPath)
 
     @staticmethod
     def image_read_rgb_as_gray(detectedObjectPath: str) -> np.ndarray:
         return cv2.imread(detectedObjectPath, 0)
 
     @staticmethod
-    def binary_mask_to_polygon(binary_mask: np.ndarray, tolerance: int=0) -> np.ndarray:
+    def binary_mask_to_polygon(binary_mask: np.ndarray, tolerance: int = 0) -> np.ndarray:
         def close_contour(contour: np.ndarray) -> np.ndarray:
             if not np.array_equal(contour[0], contour[-1]):
                 contour = np.vstack((contour, contour[0]))
             return contour
 
         polygons = []
         # pad mask to close contours of shapes which start and end at an edge
@@ -96,8 +99,7 @@
             contour = np.flip(contour, axis=1)
             segmentation = contour.ravel().tolist()
             # after padding and subtracting 1 we may get -0.5 points in our segmentation
             segmentation = [0 if i < 0 else i for i in segmentation]
             polygons.append(segmentation)
 
         return polygons
-
```

### Comparing `imagery-mapilio-0.0.8/imagery/postprocessor.py` & `imagery-mapilio-0.0.9/imagery/postprocessor.py`

 * *Files identical despite different names*

