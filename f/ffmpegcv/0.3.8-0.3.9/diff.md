# Comparing `tmp/ffmpegcv-0.3.8.tar.gz` & `tmp/ffmpegcv-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ffmpegcv-0.3.8.tar", last modified: Sat Nov 25 03:01:23 2023, max compression
+gzip compressed data, was "ffmpegcv-0.3.9.tar", last modified: Fri Jan 12 06:51:33 2024, max compression
```

## Comparing `ffmpegcv-0.3.8.tar` & `ffmpegcv-0.3.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 03:01:23.655910 ffmpegcv-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (127)    13007 2023-11-25 03:01:23.655910 ffmpegcv-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12767 2023-11-25 03:01:12.000000 ffmpegcv-0.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 03:01:23.651910 ffmpegcv-0.3.8/ffmpegcv/
--rw-r--r--   0 runner    (1001) docker     (127)    11975 2023-11-25 03:01:12.000000 ffmpegcv-0.3.8/ffmpegcv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2023-11-25 03:01:12.000000 ffmpegcv-0.3.8/ffmpegcv/ffmpeg_noblock.py
--rw-r--r--   0 runner    (1001) docker     (127)    10470 2023-11-25 03:01:12.000000 ffmpegcv-0.3.8/ffmpegcv/ffmpeg_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    15081 2023-11-25 03:01:12.000000 ffmpegcv-0.3.8/ffmpegcv/ffmpeg_reader_camera.py
--rw-r--r--   0 runner    (1001) docker     (127)     2569 2023-11-25 03:01:12.000000 ffmpegcv-0.3.8/ffmpegcv/ffmpeg_reader_noblock.py
--rw-r--r--   0 runner    (1001) docker     (127)     3522 2023-11-25 03:01:12.000000 ffmpegcv-0.3.8/ffmpegcv/ffmpeg_reader_qsv.py
--rw-r--r--   0 runner    (1001) docker     (127)     4100 2023-11-25 03:01:12.000000 ffmpegcv-0.3.8/ffmpegcv/ffmpeg_reader_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2023-11-25 03:01:12.000000 ffmpegcv-0.3.8/ffmpegcv/ffmpeg_reader_stream_realtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     4264 2023-11-25 03:01:12.000000 ffmpegcv-0.3.8/ffmpegcv/ffmpeg_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2023-11-25 03:01:12.000000 ffmpegcv-0.3.8/ffmpegcv/ffmpeg_writer_noblock.py
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2023-11-25 03:01:12.000000 ffmpegcv-0.3.8/ffmpegcv/ffmpeg_writer_qsv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2023-11-25 03:01:12.000000 ffmpegcv-0.3.8/ffmpegcv/ffmpeg_writer_stream_realtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2023-11-25 03:01:12.000000 ffmpegcv-0.3.8/ffmpegcv/stream_info.py
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-11-25 03:01:12.000000 ffmpegcv-0.3.8/ffmpegcv/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5089 2023-11-25 03:01:12.000000 ffmpegcv-0.3.8/ffmpegcv/video_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 03:01:23.655910 ffmpegcv-0.3.8/ffmpegcv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13007 2023-11-25 03:01:23.000000 ffmpegcv-0.3.8/ffmpegcv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      622 2023-11-25 03:01:23.000000 ffmpegcv-0.3.8/ffmpegcv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-25 03:01:23.000000 ffmpegcv-0.3.8/ffmpegcv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-11-25 03:01:23.000000 ffmpegcv-0.3.8/ffmpegcv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-11-25 03:01:23.000000 ffmpegcv-0.3.8/ffmpegcv.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-25 03:01:23.655910 ffmpegcv-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      656 2023-11-25 03:01:12.000000 ffmpegcv-0.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 06:51:33.125850 ffmpegcv-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    13073 2024-01-12 06:51:33.125850 ffmpegcv-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12833 2024-01-12 06:51:23.000000 ffmpegcv-0.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 06:51:33.121850 ffmpegcv-0.3.9/ffmpegcv/
+-rw-r--r--   0 runner    (1001) docker     (127)    12194 2024-01-12 06:51:23.000000 ffmpegcv-0.3.9/ffmpegcv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-01-12 06:51:23.000000 ffmpegcv-0.3.9/ffmpegcv/ffmpeg_noblock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10460 2024-01-12 06:51:23.000000 ffmpegcv-0.3.9/ffmpegcv/ffmpeg_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12360 2024-01-12 06:51:23.000000 ffmpegcv-0.3.9/ffmpegcv/ffmpeg_reader_camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-01-12 06:51:23.000000 ffmpegcv-0.3.9/ffmpegcv/ffmpeg_reader_noblock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-01-12 06:51:23.000000 ffmpegcv-0.3.9/ffmpegcv/ffmpeg_reader_qsv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-01-12 06:51:23.000000 ffmpegcv-0.3.9/ffmpegcv/ffmpeg_reader_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-01-12 06:51:23.000000 ffmpegcv-0.3.9/ffmpegcv/ffmpeg_reader_stream_realtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-01-12 06:51:23.000000 ffmpegcv-0.3.9/ffmpegcv/ffmpeg_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-01-12 06:51:23.000000 ffmpegcv-0.3.9/ffmpegcv/ffmpeg_writer_noblock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-01-12 06:51:23.000000 ffmpegcv-0.3.9/ffmpegcv/ffmpeg_writer_qsv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-01-12 06:51:23.000000 ffmpegcv-0.3.9/ffmpegcv/ffmpeg_writer_stream_realtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-01-12 06:51:23.000000 ffmpegcv-0.3.9/ffmpegcv/stream_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-01-12 06:51:23.000000 ffmpegcv-0.3.9/ffmpegcv/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5089 2024-01-12 06:51:23.000000 ffmpegcv-0.3.9/ffmpegcv/video_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 06:51:33.125850 ffmpegcv-0.3.9/ffmpegcv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13073 2024-01-12 06:51:33.000000 ffmpegcv-0.3.9/ffmpegcv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-01-12 06:51:33.000000 ffmpegcv-0.3.9/ffmpegcv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-12 06:51:33.000000 ffmpegcv-0.3.9/ffmpegcv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-01-12 06:51:33.000000 ffmpegcv-0.3.9/ffmpegcv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-12 06:51:33.000000 ffmpegcv-0.3.9/ffmpegcv.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-12 06:51:33.125850 ffmpegcv-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-01-12 06:51:23.000000 ffmpegcv-0.3.9/setup.py
```

### Comparing `ffmpegcv-0.3.8/PKG-INFO` & `ffmpegcv-0.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffmpegcv
-Version: 0.3.8
+Version: 0.3.9
 Home-page: https://github.com/chenxinfeng4/ffmpegcv
 Author: chenxf
 Author-email: cxf529125853@163.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 
@@ -55,15 +55,15 @@
 - The `opencv` didn't support `h264`/`h265` and other video writers.
 - You want to **crop**, **resize** and **pad** the video/camero ROI.
 
 ## Basic example
 Read a video by CPU, and rewrite it by GPU.
 ```python
 vidin = ffmpegcv.VideoCapture(vfile_in)
-vidout = ffmpegcv.VideoWriterNV(vfile_out, 'h264', vidin.fps)
+vidout = ffmpegcv.VideoWriterNV(vfile_out, 'h264', vidin.fps)  #NVIDIA-GPU
 
 with vidin, vidout:
     for frame in vidin:
         cv2.imshow('image', frame)
         vidout.write(frame)
 ```
 
@@ -71,14 +71,16 @@
 ```python
 # by device ID
 cap = ffmpegcv.VideoCaptureCAM(0)
 # by device name
 cap = ffmpegcv.VideoCaptureCAM("Integrated Camera")
 ```
 
+## Cross platform
+
 ## GPU Accelation
 - Support **NVIDIA** card only, test in x86_64 only.
 - Works in **Windows**, **Linux** and **Anaconda**.
 - Works in the **Google Colab** notebook. 
 - Infeasible in the **MacOS**. That ffmpeg didn't supports NVIDIA at all.
 
 > \* The ffmegcv GPU reader is a bit slower than CPU reader, but much faster when use ROI operations (crop, resize, pad).
@@ -301,15 +303,15 @@
 # The macOS requires full argument.
 cap = ffmpegcv.VideoCaptureCAM('FaceTime HD Camera', camsize_wh=(1280,720), camfps=30, campix_fmt='nv12')
 ```
 
 2. The VideoCaptureCAM cann't list the FPS in linux. Because the `ffmpeg` cound't query the device's FPS using linux native `v4l2` module. However, it's just OK to let the FPS empty.
 
 
-## Stream Reader
+## Stream Reader (Live streaming, RTSP IP cameras)
 **Experimental feature**. The ffmpegcv offers Stream reader. Which is consistent with VideoFiler reader, and more similiar to the camera.
 Becareful when using it.
 
 - Support `RTSP`, `RTP`, `RTMP`, `HTTP`, `HTTPS` streams.
 - The `VideoCaptureStream` will be laggy and dropping frames if your post-process takes long time. The VideoCaptureCAM will buffer the recent frames.
 - The `VideoCaptureStream` is continously working on background even if you didn't read it. **Please release it in time**.
 - It's still experimental. Recommand you to use opencv.
```

### Comparing `ffmpegcv-0.3.8/README.md` & `ffmpegcv-0.3.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 - The `opencv` didn't support `h264`/`h265` and other video writers.
 - You want to **crop**, **resize** and **pad** the video/camero ROI.
 
 ## Basic example
 Read a video by CPU, and rewrite it by GPU.
 ```python
 vidin = ffmpegcv.VideoCapture(vfile_in)
-vidout = ffmpegcv.VideoWriterNV(vfile_out, 'h264', vidin.fps)
+vidout = ffmpegcv.VideoWriterNV(vfile_out, 'h264', vidin.fps)  #NVIDIA-GPU
 
 with vidin, vidout:
     for frame in vidin:
         cv2.imshow('image', frame)
         vidout.write(frame)
 ```
 
@@ -61,14 +61,16 @@
 ```python
 # by device ID
 cap = ffmpegcv.VideoCaptureCAM(0)
 # by device name
 cap = ffmpegcv.VideoCaptureCAM("Integrated Camera")
 ```
 
+## Cross platform
+
 ## GPU Accelation
 - Support **NVIDIA** card only, test in x86_64 only.
 - Works in **Windows**, **Linux** and **Anaconda**.
 - Works in the **Google Colab** notebook. 
 - Infeasible in the **MacOS**. That ffmpeg didn't supports NVIDIA at all.
 
 > \* The ffmegcv GPU reader is a bit slower than CPU reader, but much faster when use ROI operations (crop, resize, pad).
@@ -291,15 +293,15 @@
 # The macOS requires full argument.
 cap = ffmpegcv.VideoCaptureCAM('FaceTime HD Camera', camsize_wh=(1280,720), camfps=30, campix_fmt='nv12')
 ```
 
 2. The VideoCaptureCAM cann't list the FPS in linux. Because the `ffmpeg` cound't query the device's FPS using linux native `v4l2` module. However, it's just OK to let the FPS empty.
 
 
-## Stream Reader
+## Stream Reader (Live streaming, RTSP IP cameras)
 **Experimental feature**. The ffmpegcv offers Stream reader. Which is consistent with VideoFiler reader, and more similiar to the camera.
 Becareful when using it.
 
 - Support `RTSP`, `RTP`, `RTMP`, `HTTP`, `HTTPS` streams.
 - The `VideoCaptureStream` will be laggy and dropping frames if your post-process takes long time. The VideoCaptureCAM will buffer the recent frames.
 - The `VideoCaptureStream` is continously working on background even if you didn't read it. **Please release it in time**.
 - It's still experimental. Recommand you to use opencv.
```

### Comparing `ffmpegcv-0.3.8/ffmpegcv/__init__.py` & `ffmpegcv-0.3.9/ffmpegcv/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from .ffmpeg_writer import FFmpegWriter, FFmpegWriterNV
 from .ffmpeg_reader_camera import FFmpegReaderCAM
 from .ffmpeg_reader_stream import FFmpegReaderStream
 from .ffmpeg_reader_stream_realtime import FFmpegReaderStreamRT
 from .ffmpeg_writer_stream_realtime import FFmpegWriterStreamRT
 from .ffmpeg_reader_qsv import FFmpegReaderQSV
 from .ffmpeg_writer_qsv import FFmpegWriterQSV
-from .ffmpeg_noblock import noblock
+from .ffmpeg_noblock import noblock, ReadLiveLast
 from .video_info import get_num_NVIDIA_GPUs
 import shutil
 from subprocess import DEVNULL, check_output
 
 from .version import __version__ 
 
 def _check():
@@ -373,14 +373,15 @@
 
 
 VideoReaderCAM = VideoCaptureCAM
 
 
 def VideoCaptureStream(
     stream_url,
+    codec=None,
     pix_fmt="bgr24",
     crop_xywh=None,
     resize=None,
     resize_keepratio=True,
     resize_keepratioalign="center"
 ):
     """
@@ -424,27 +425,40 @@
         pass
     ```
 
     Author: Chenxinfeng 2023-05-31, cxf529125853@163.com
     """
     return FFmpegReaderStream.VideoReader(
         stream_url,
+        codec,
         pix_fmt,
         crop_xywh,
         resize,
         resize_keepratio,
         resize_keepratioalign
     )
 
 
 VideoReaderStream = VideoCaptureStream
 
 
 def VideoCaptureStreamRT(
     stream_url,
+    codec=None,
     pix_fmt="bgr24",
-    camsize_wh=None
+    crop_xywh=None,
+    resize=None,
+    resize_keepratio=True,
+    resize_keepratioalign="center",
 ):
-    assert camsize_wh is not None
-    return FFmpegReaderStreamRT.VideoReader(stream_url, pix_fmt, camsize=camsize_wh)
+    return FFmpegReaderStreamRT.VideoReader(
+        stream_url, 
+        codec, 
+        pix_fmt,
+        crop_xywh,
+        resize,
+        resize_keepratio,
+        resize_keepratioalign
+    )
+
 
 VideoReaderStreamRT = VideoCaptureStreamRT
```

### Comparing `ffmpegcv-0.3.8/ffmpegcv/ffmpeg_noblock.py` & `ffmpegcv-0.3.9/ffmpegcv/ffmpeg_noblock.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,9 +40,9 @@
     def release(self):
         self._isopen = False
         self.vid.release()
 
     def run(self):
         while self._isopen:
             self.ret, self.img = self.vid.read()
-            if self.ret:
+            if not self.ret:
                 break
```

### Comparing `ffmpegcv-0.3.8/ffmpegcv/ffmpeg_reader.py` & `ffmpegcv-0.3.9/ffmpegcv/ffmpeg_reader.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,20 +6,94 @@
     get_info,
     get_num_NVIDIA_GPUs,
     decoder_to_nvidia,
     release_process,
 )
 
 
+def get_videofilter_cpu(originsize:list, pix_fmt:str,  crop_xywh:list, resize:list,
+               resize_keepratio:bool, resize_keepratioalign:str):
+    """
+    ONGONING: common filter for video/cam/stream capture.
+    """
+    origin_width, origin_height = originsize
+    if crop_xywh:
+        crop_w, crop_h = crop_xywh[2:]
+        x, y, w, h = crop_xywh
+        cropopt = f"crop={w}:{h}:{x}:{y}"
+    else:
+        crop_w, crop_h = origin_width, origin_height
+        cropopt = ""
+
+    crop_wh = (crop_w, crop_h)
+    if resize is None or tuple(resize) == crop_wh:
+        scaleopt = ""
+        padopt = ""
+        final_size_wh = crop_wh
+    else:
+        final_size_wh = dst_width, dst_height = resize
+        if not resize_keepratio:
+            scaleopt = f"scale={dst_width}x{dst_height}"
+            padopt = ""
+        else:
+            re_width, re_height = crop_w / (crop_h / dst_height), dst_height
+            if re_width > dst_width:
+                re_width, re_height = dst_width, crop_h / (crop_w / dst_width)
+            re_width, re_height = int(re_width), int(re_height)
+            scaleopt = f"scale={re_width}x{re_height}"
+            if resize_keepratioalign is None:
+                resize_keepratioalign = "center"
+            paddings = {
+                "center": (
+                    (dst_width - re_width) // 2,
+                    (dst_height - re_height) // 2,
+                ),
+                "topleft": (0, 0),
+                "topright": (dst_width - re_width, 0),
+                "bottomleft": (0, dst_height - re_height),
+                "bottomright": (dst_width - re_width, dst_height - re_height),
+            }
+            assert (
+                resize_keepratioalign in paddings
+            ), 'resize_keepratioalign must be one of "center"(mmpose), "topleft"(mmdetection), "topright", "bottomleft", "bottomright"'
+            xpading, ypading = paddings[resize_keepratioalign]
+            padopt = f"pad={dst_width}:{dst_height}:{xpading}:{ypading}:black"
+
+    pix_fmtopt = 'extractplanes=y' if pix_fmt=='gray' else ''
+    if any([cropopt, scaleopt, padopt, pix_fmtopt]):
+        filterstr = ",".join(x for x in [cropopt, scaleopt, padopt, pix_fmtopt] if x)
+        filteropt = f"-vf {filterstr}"
+    else:
+        filteropt = ""
+    return crop_wh, final_size_wh, filteropt
+
+
+def get_outnumpyshape(size_wh:list, pix_fmt:str) -> tuple:
+    width, height = size_wh
+    assert (not pix_fmt == "yuv420p") or (
+            height % 2 == 0 and width % 2 == 0
+        ), "yuv420p must be even"
+    out_numpy_shape = {
+            "rgb24": (height, width, 3),
+            "bgr24": (height, width, 3),
+            "yuv420p": (int(height * 1.5), width),
+            "yuvj420p": (int(height * 1.5), width),
+            "nv12": (int(height * 1.5), width),
+            "gray": (height, width, 1)
+        }[pix_fmt]
+    return out_numpy_shape
+
+
 class FFmpegReader:
     def __init__(self):
         self.iframe = -1
         self.waitInit = True
         self.process = None
         self._isopen = True
+        self.out_numpy_shape = (None, None, None)
 
     def __repr__(self):
         props = pprint.pformat(self.__dict__).replace("{", " ").replace("}", " ")
         return f"{self.__class__}\n" + props
 
     def __enter__(self):
         return self
@@ -49,108 +123,38 @@
         resize,
         resize_keepratio,
         resize_keepratioalign,
     ):
         assert os.path.exists(filename) and os.path.isfile(
             filename
         ), f"{filename} not exists"
-        assert pix_fmt in ["rgb24", "bgr24", "yuv420p", "nv12", "gray"]
+        assert pix_fmt in ["rgb24", "bgr24", "yuv420p", "yuvj420p", "nv12", "gray"]
 
         vid = FFmpegReader()
         videoinfo = get_info(filename)
-        vid.width = videoinfo.width
-        vid.height = videoinfo.height
+        vid.origin_width = videoinfo.width
+        vid.origin_height = videoinfo.height
         vid.fps = videoinfo.fps
         vid.count = videoinfo.count
-        vid.origin_width, vid.origin_height = vid.width, vid.height
+        vid.pix_fmt = pix_fmt
         vid.codec = codec if codec else videoinfo.codec
-        if crop_xywh:
-            crop_w, crop_h = crop_xywh[2:]
-            vid.width, vid.height = crop_w, crop_h
-            x, y, w, h = crop_xywh
-            cropopt = f"crop={w}:{h}:{x}:{y}"
-        else:
-            crop_w, crop_h = vid.origin_width, vid.origin_height
-            cropopt = ""
 
-        vid.crop_width, vid.crop_height = crop_w, crop_h
-
-        if resize is None or tuple(resize) == (vid.crop_width, vid.crop_height):
-            scaleopt = ""
-            padopt = ""
-        else:
-            vid.width, vid.height = dst_width, dst_height = resize
-            if not resize_keepratio:
-                scaleopt = f"scale={dst_width}x{dst_height}"
-                padopt = ""
-            else:
-                re_width, re_height = crop_w / (crop_h / dst_height), dst_height
-                if re_width > dst_width:
-                    re_width, re_height = dst_width, crop_h / (crop_w / dst_width)
-                re_width, re_height = int(re_width), int(re_height)
-                scaleopt = f"scale={re_width}x{re_height}"
-                if resize_keepratioalign is None:
-                    resize_keepratioalign = "center"
-                paddings = {
-                    "center": (
-                        (dst_width - re_width) // 2,
-                        (dst_height - re_height) // 2,
-                    ),
-                    "topleft": (0, 0),
-                    "topright": (dst_width - re_width, 0),
-                    "bottomleft": (0, dst_height - re_height),
-                    "bottomright": (dst_width - re_width, dst_height - re_height),
-                }
-                assert (
-                    resize_keepratioalign in paddings
-                ), 'resize_keepratioalign must be one of "center"(mmpose), "topleft"(mmdetection), "topright", "bottomleft", "bottomright"'
-                xpading, ypading = paddings[resize_keepratioalign]
-                padopt = f"pad={dst_width}:{dst_height}:{xpading}:{ypading}:black"
-
-        pix_fmtopt = 'extractplanes=y' if pix_fmt=='gray' else ''
-        if any([cropopt, scaleopt, padopt, pix_fmtopt]):
-            filterstr = ",".join(x for x in [cropopt, scaleopt, padopt, pix_fmtopt] if x)
-            filteropt = f"-vf {filterstr}"
-        else:
-            filteropt = ""
+        (vid.crop_width, vid.crop_height), (vid.width, vid.height), filteropt = get_videofilter_cpu(
+                (vid.origin_width, vid.origin_height), pix_fmt, crop_xywh, resize, 
+                resize_keepratio, resize_keepratioalign)
+        vid.size = (vid.width, vid.height)
 
         vid.ffmpeg_cmd = (
             f"ffmpeg -loglevel warning "
             f' -vcodec {vid.codec} -r {vid.fps} -i "{filename}" '
             f" {filteropt} -pix_fmt {pix_fmt} -r {vid.fps} -f rawvideo pipe:"
         )  
-        vid.size = (vid.width, vid.height)
-        vid.pix_fmt = pix_fmt
-        assert (not pix_fmt == "yuv420p") or (
-            vid.height % 2 == 0 and vid.width % 2 == 0
-        ), "yuv420p must be even"
-        vid.out_numpy_shape = {
-            "rgb24": (vid.height, vid.width, 3),
-            "bgr24": (vid.height, vid.width, 3),
-            "nv12": (int(vid.height * 1.5), vid.width),
-            "yuv420p": (int(vid.height * 1.5), vid.width),
-            "gray": (vid.height, vid.width, 1)
-        }[pix_fmt]
+        vid.out_numpy_shape = get_outnumpyshape(vid.size, pix_fmt)
         return vid
 
-    def read_gray(self):
-        # It's an experimental function
-        # return 'ret, img_gray'
-        # img_gray: Height x Width x 1
-        if self.pix_fmt == "gray":
-            return self.read()
-        
-        assert self.pix_fmt in ("nv12", "yuv420p")
-        ret, img = self.read()
-        if not ret:
-            return False, None
-        assert img.shape == (int(self.height * 1.5), self.width)
-        img_gray = img[: self.height, :, None]
-        return True, img_gray
-
     def read(self):
         if self.waitInit:
             self.process = run_async(self.ffmpeg_cmd)
             self.waitInit = False
             
         in_bytes = self.process.stdout.read(np.prod(self.out_numpy_shape))
         if not in_bytes:
```

### Comparing `ffmpegcv-0.3.8/ffmpegcv/ffmpeg_reader_camera.py` & `ffmpegcv-0.3.9/ffmpegcv/ffmpeg_reader_camera.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from .video_info import run_async, release_process
 import re
 import subprocess
 from threading import Thread
 from queue import Queue
 import sys
 import os
+from ffmpegcv.ffmpeg_reader import get_videofilter_cpu, get_outnumpyshape
 
 
 class platform:
     win = 0
     linux = 1
     mac = 2
     other = 3
@@ -200,24 +201,23 @@
 class ProducerThread(Thread):
     def __init__(self, vid, q):
         super(ProducerThread, self).__init__()
         self.vid = vid
         self.q = q
 
     def run(self):
+        q = self.q
         while True:
             if not self.vid.isOpened():
                 break
             ret, img = self.vid.read_()
 
-            try:
-                self.q.put_nowait((ret, img))  # drop frames
-            except Exception:
-                pass
-            continue
+            if q.full():
+                q.get() # drop frames
+            q.put((ret, img))  
 
 
 class FFmpegReaderCAM:
     def __init__(self):
         self.iframe = -1
         self._isopen = True
 
@@ -286,26 +286,27 @@
 
         if camsize_wh is None:
             cam_options = query_camera_options(camname)
             resolutions = [c["camsize_wh"] for c in cam_options]
             camsize_wh = max(resolutions, key=lambda x: sum(x))
 
         assert len(camsize_wh) == 2
-        vid.width, vid.height = camsize_wh
+        vid.origin_width, vid.origin_height = camsize_wh
 
         opt_camfps = f" -framerate {camfps} " if camfps else ""
         vid.camfps = camfps if camfps else None
 
         opt_camcodec_ = {
             platform.linux: "input_format",
             platform.mac: "",
             platform.win: "vcodec",
         }[this_os]
         opt_camcodec = f" -{opt_camcodec_} {camcodec} " if camcodec else ""
         vid.camcodec = camcodec if camcodec else None
+        vid.pix_fmt = pix_fmt
 
         opt_campix_fmt_ = {
             platform.linux: "input_format",
             platform.mac: "pixel_format",
             platform.win: "pixel_format",
         }[this_os]
         opt_campix_fmt = f" -{opt_campix_fmt_} {campix_fmt} " if campix_fmt else ""
@@ -313,63 +314,17 @@
 
         opt_camname = {
             platform.linux: f'"{camname}"',
             platform.win: f'video="{camname}"',
             platform.mac: f"{camid}:none",
         }[this_os]
 
-        vid.origin_width, vid.origin_height = vid.width, vid.height
-        if crop_xywh:
-            crop_w, crop_h = crop_xywh[2:]
-            vid.width, vid.height = crop_w, crop_h
-            x, y, w, h = crop_xywh
-            cropopt = f"crop={w}:{h}:{x}:{y}"
-        else:
-            crop_w, crop_h = vid.origin_width, vid.origin_height
-            cropopt = ""
-
-        vid.crop_width, vid.crop_height = crop_w, crop_h
-
-        if resize is None or resize == (vid.crop_width, vid.crop_height):
-            scaleopt = ""
-            padopt = ""
-        else:
-            vid.width, vid.height = dst_width, dst_height = resize
-            if not resize_keepratio:
-                scaleopt = f"scale={dst_width}x{dst_height}"
-                padopt = ""
-            else:
-                re_width, re_height = crop_w / (crop_h / dst_height), dst_height
-                if re_width > dst_width:
-                    re_width, re_height = dst_width, crop_h / (crop_w / dst_width)
-                re_width, re_height = int(re_width), int(re_height)
-                scaleopt = f"scale={re_width}x{re_height}"
-                if resize_keepratioalign is None:
-                    resize_keepratioalign = "center"
-                paddings = {
-                    "center": (
-                        (dst_width - re_width) // 2,
-                        (dst_height - re_height) // 2,
-                    ),
-                    "topleft": (0, 0),
-                    "topright": (dst_width - re_width, 0),
-                    "bottomleft": (0, dst_height - re_height),
-                    "bottomright": (dst_width - re_width, dst_height - re_height),
-                }
-                assert (
-                    resize_keepratioalign in paddings
-                ), 'resize_keepratioalign must be one of "center"(mmpose), "topleft"(mmdetection), "topright", "bottomleft", "bottomright"'
-                xpading, ypading = paddings[resize_keepratioalign]
-                padopt = f"pad={dst_width}:{dst_height}:{xpading}:{ypading}:black"
-
-        if any([cropopt, scaleopt, padopt]):
-            filterstr = ",".join(x for x in [cropopt, scaleopt, padopt] if x)
-            filteropt = f"-vf {filterstr}"
-        else:
-            filteropt = ""
+        (vid.crop_width, vid.crop_height), (vid.width, vid.height), filteropt = get_videofilter_cpu(
+                (vid.origin_width, vid.origin_height), crop_xywh, resize, resize_keepratio, resize_keepratioalign)
+        vid.size = (vid.width, vid.height)
 
         opt_driver_ = {
             platform.linux: "v4l2",
             platform.mac: "avfoundation",
             platform.win: "dshow",
         }[this_os]
 
@@ -378,25 +333,15 @@
             f" -f {opt_driver_} "
             f" -video_size {vid.origin_width}x{vid.origin_height} "
             f" {opt_camfps} {opt_camcodec} {opt_campix_fmt} "
             f" -i {opt_camname} "
             f" {filteropt} -pix_fmt {pix_fmt} -f rawvideo pipe:"
         )
 
-        vid.size = (vid.width, vid.height)
-        vid.pix_fmt = pix_fmt
-        assert (not pix_fmt == "yuv420p") or (
-            vid.height % 2 == 0 and vid.width % 2 == 0
-        ), "yuv420p must be even"
-        vid.out_numpy_shape = {
-            "rgb24": (vid.height, vid.width, 3),
-            "bgr24": (vid.height, vid.width, 3),
-            "yuv420p": (int(vid.height * 1.5), vid.width),
-            "nv12": (int(vid.height * 1.5), vid.width),
-        }[pix_fmt]
+        vid.out_numpy_shape = get_outnumpyshape(vid.size, pix_fmt)
         vid.process = run_async(args)
 
         # producer
         assert step >= 1 and isinstance(step, int)
         vid.step = step
         vid.q = Queue(maxsize=30)
         producer = ProducerThread(vid, vid.q)
@@ -411,26 +356,14 @@
             return False, None
 
         self.iframe += 1
         img = None
         img = np.frombuffer(in_bytes, np.uint8).reshape(self.out_numpy_shape)
         return True, img
 
-    def read_gray(self):
-        # It's an experimental function
-        # return 'ret, img_gray'
-        # img_gray: Height x Width x 1
-        assert self.pix_fmt in ("nv12", "yuv420p")
-        ret, img = self.read()
-        if not ret:
-            return False, None
-        assert img.shape == (int(self.height * 1.5), self.width)
-        img_gray = img[: self.height, :, None]
-        return True, img_gray
-
     def read(self):
         ret, img = self.q.get()
         return ret, img
 
     def isOpened(self):
         return self._isopen
```

### Comparing `ffmpegcv-0.3.8/ffmpegcv/ffmpeg_reader_noblock.py` & `ffmpegcv-0.3.9/ffmpegcv/ffmpeg_reader_noblock.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
         # 将共享内存的NumPy数组转换为NumPy数组
         self.np_array = np.frombuffer(shared_array.get_obj(), dtype=np.uint8).reshape((NFRAME,*self.out_numpy_shape))
         
         self.shared_array = shared_array
         self.vcap_args = vcap_args
         self.vcap_kwargs = vcap_kwargs
-        self.q = Queue(maxsize=(NFRAME-1)*2)
+        self.q = Queue(maxsize=(NFRAME-2)*2)
         self.vcap_fun = vcap_fun
         self.has_init = False
         self.process = None
 
     def read(self):
         if not self.has_init:
             self.has_init = True
```

### Comparing `ffmpegcv-0.3.8/ffmpegcv/ffmpeg_reader_qsv.py` & `ffmpegcv-0.3.9/ffmpegcv/ffmpeg_reader_qsv.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,55 +1,17 @@
 import os
-from ffmpegcv.ffmpeg_reader import FFmpegReader
+from ffmpegcv.ffmpeg_reader import FFmpegReader, get_videofilter_cpu, get_outnumpyshape
 from .video_info import (
     get_info,
     get_num_QSV_GPUs,
     decoder_to_qsv,
 )
 
 
 class FFmpegReaderQSV(FFmpegReader):
-    def _get_opts(
-        vid, videoinfo, crop_xywh, resize, resize_keepratio, resize_keepratioalign, isgray
-    ):
-        vid.origin_width = videoinfo.width
-        vid.origin_height = videoinfo.height
-        vid.fps = videoinfo.fps
-        vid.count = videoinfo.count
-        vid.width, vid.height = vid.origin_width, vid.origin_height
-        vid.codec = videoinfo.codec
-        assert crop_xywh is None, 'Function not implemented yet'
-        assert resize is None, 'Function not implemented yet'
-        assert resize_keepratio is None or resize_keepratio==True, 'Function not implemented yet'
-        assert resize_keepratioalign is None or resize_keepratioalign=="center", 'Function not implemented yet'
-        assert vid.origin_height % 2 == 0, "height must be even"
-        assert vid.origin_width % 2 == 0, "width must be even"
-        if crop_xywh:
-            pass
-        else:
-            crop_w, crop_h = vid.origin_width, vid.origin_height
-            cropopt = ""
-
-        vid.crop_width, vid.crop_height = crop_w, crop_h
-
-        if resize is None or tuple(resize) == (vid.crop_width, vid.crop_height):
-            scaleopt = ""
-            filteropt = ""
-        else:
-            pass
-
-        if isgray:
-            if filteropt:
-                filteropt=f'{filteropt},extractplanes=y'
-            else:
-                filteropt=f'-vf extractplanes=y'
-        
-        vid.size = (vid.width, vid.height)
-        return cropopt, scaleopt, filteropt
-
     @staticmethod
     def VideoReader(
         filename,
         pix_fmt,
         crop_xywh,
         resize,
         resize_keepratio,
@@ -67,33 +29,30 @@
         assert gpu is None or gpu == 0, 'Cannot use multiple QSV gpu yet.'
         numGPU = get_num_QSV_GPUs()
         assert numGPU > 0, "No GPU found"
         gpu = int(gpu) % numGPU if gpu is not None else 0
         assert (
             resize is None or len(resize) == 2
         ), "resize must be a tuple of (width, height)"
-        videoinfo = get_info(filename)
+
         vid = FFmpegReaderQSV()
-        isgray = pix_fmt == "gray"
-        cropopt, scaleopt, filteropt = vid._get_opts(
-            videoinfo, crop_xywh, resize, resize_keepratio, resize_keepratioalign, isgray
-        )
-        vid.codecQSV = decoder_to_qsv(vid.codec)
+        videoinfo = get_info(filename)
+        vid.origin_width = videoinfo.width
+        vid.origin_height = videoinfo.height
+        vid.fps = videoinfo.fps
+        vid.count = videoinfo.count
+        vid.codecQSV = decoder_to_qsv(videoinfo.codec)
+        vid.pix_fmt = pix_fmt
+
+        (vid.crop_width, vid.crop_height), (vid.width, vid.height), filteropt = get_videofilter_cpu(
+                (vid.origin_width, vid.origin_height), pix_fmt, crop_xywh, resize, 
+                resize_keepratio, resize_keepratioalign)
+        vid.size = (vid.width, vid.height)
 
         vid.ffmpeg_cmd = (
             f"ffmpeg -loglevel warning "
             f' -vcodec {vid.codecQSV} -r {vid.fps} -i "{filename}" '
             f" {filteropt} -pix_fmt {pix_fmt} -r {vid.fps} -f rawvideo pipe:"
         )
 
-        vid.pix_fmt = pix_fmt
-        assert (not pix_fmt == "yuv420p") or (
-            vid.height % 2 == 0 and vid.width % 2 == 0
-        ), "yuv420p must be even"
-        vid.out_numpy_shape = {
-            "rgb24": (vid.height, vid.width, 3),
-            "bgr24": (vid.height, vid.width, 3),
-            "yuv420p": (int(vid.height * 1.5), vid.width),
-            "nv12": (int(vid.height * 1.5), vid.width),
-            "gray": (vid.height, vid.width, 1)
-        }[pix_fmt]
+        vid.out_numpy_shape = get_outnumpyshape(vid.size, pix_fmt)
         return vid
```

### Comparing `ffmpegcv-0.3.8/ffmpegcv/ffmpeg_writer.py` & `ffmpegcv-0.3.9/ffmpegcv/ffmpeg_writer.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,22 +54,28 @@
                 f'-f rawvideo -pix_fmt {self.pix_fmt} -s {self.width}x{self.height} -r {self.fps} -i pipe: '
                 f'{bitrate_str} '
                 f'-r {self.fps} -c:v {self.codec} -pix_fmt yuv420p "{self.filename}"')
         self.process = run_async(self.ffmpeg_cmd)
 
     def write(self, img:np.ndarray):
         if self.waitInit:
-            if self.size is None:
-                self.size = (img.shape[1], img.shape[0])
-            self.width, self.height = self.size
+            if self.pix_fmt in ('nv12', 'yuv420p', 'yuvj420p'):
+                assert width%2==0 and height_15*2%3==0
+                height_15, width = img.shape[:2]
+                height = int(height_15 / 1.5)
+            else:
+                height, width = img.shape[:2]
+            self.width, self.height = width, height
+            self.in_numpy_shape = img.shape
+            self.size = (width, height)
             self._init_video_stream()
             self.waitInit = False
 
         self.iframe += 1
-        assert self.size == (img.shape[1], img.shape[0])
+        assert self.in_numpy_shape == img.shape
         img = img.astype(np.uint8).tobytes()
         self.process.stdin.write(img)
 
     def isOpened(self):
         return self._isopen
 
     def release(self):
```

### Comparing `ffmpegcv-0.3.8/ffmpegcv/ffmpeg_writer_noblock.py` & `ffmpegcv-0.3.9/ffmpegcv/ffmpeg_writer_noblock.py`

 * *Files identical despite different names*

### Comparing `ffmpegcv-0.3.8/ffmpegcv/ffmpeg_writer_qsv.py` & `ffmpegcv-0.3.9/ffmpegcv/ffmpeg_writer_qsv.py`

 * *Files identical despite different names*

### Comparing `ffmpegcv-0.3.8/ffmpegcv/ffmpeg_writer_stream_realtime.py` & `ffmpegcv-0.3.9/ffmpegcv/ffmpeg_writer_stream_realtime.py`

 * *Files identical despite different names*

### Comparing `ffmpegcv-0.3.8/ffmpegcv/stream_info.py` & `ffmpegcv-0.3.9/ffmpegcv/stream_info.py`

 * *Files identical despite different names*

### Comparing `ffmpegcv-0.3.8/ffmpegcv/video_info.py` & `ffmpegcv-0.3.9/ffmpegcv/video_info.py`

 * *Files identical despite different names*

### Comparing `ffmpegcv-0.3.8/ffmpegcv.egg-info/PKG-INFO` & `ffmpegcv-0.3.9/ffmpegcv.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffmpegcv
-Version: 0.3.8
+Version: 0.3.9
 Home-page: https://github.com/chenxinfeng4/ffmpegcv
 Author: chenxf
 Author-email: cxf529125853@163.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 
@@ -55,15 +55,15 @@
 - The `opencv` didn't support `h264`/`h265` and other video writers.
 - You want to **crop**, **resize** and **pad** the video/camero ROI.
 
 ## Basic example
 Read a video by CPU, and rewrite it by GPU.
 ```python
 vidin = ffmpegcv.VideoCapture(vfile_in)
-vidout = ffmpegcv.VideoWriterNV(vfile_out, 'h264', vidin.fps)
+vidout = ffmpegcv.VideoWriterNV(vfile_out, 'h264', vidin.fps)  #NVIDIA-GPU
 
 with vidin, vidout:
     for frame in vidin:
         cv2.imshow('image', frame)
         vidout.write(frame)
 ```
 
@@ -71,14 +71,16 @@
 ```python
 # by device ID
 cap = ffmpegcv.VideoCaptureCAM(0)
 # by device name
 cap = ffmpegcv.VideoCaptureCAM("Integrated Camera")
 ```
 
+## Cross platform
+
 ## GPU Accelation
 - Support **NVIDIA** card only, test in x86_64 only.
 - Works in **Windows**, **Linux** and **Anaconda**.
 - Works in the **Google Colab** notebook. 
 - Infeasible in the **MacOS**. That ffmpeg didn't supports NVIDIA at all.
 
 > \* The ffmegcv GPU reader is a bit slower than CPU reader, but much faster when use ROI operations (crop, resize, pad).
@@ -301,15 +303,15 @@
 # The macOS requires full argument.
 cap = ffmpegcv.VideoCaptureCAM('FaceTime HD Camera', camsize_wh=(1280,720), camfps=30, campix_fmt='nv12')
 ```
 
 2. The VideoCaptureCAM cann't list the FPS in linux. Because the `ffmpeg` cound't query the device's FPS using linux native `v4l2` module. However, it's just OK to let the FPS empty.
 
 
-## Stream Reader
+## Stream Reader (Live streaming, RTSP IP cameras)
 **Experimental feature**. The ffmpegcv offers Stream reader. Which is consistent with VideoFiler reader, and more similiar to the camera.
 Becareful when using it.
 
 - Support `RTSP`, `RTP`, `RTMP`, `HTTP`, `HTTPS` streams.
 - The `VideoCaptureStream` will be laggy and dropping frames if your post-process takes long time. The VideoCaptureCAM will buffer the recent frames.
 - The `VideoCaptureStream` is continously working on background even if you didn't read it. **Please release it in time**.
 - It's still experimental. Recommand you to use opencv.
```

### Comparing `ffmpegcv-0.3.8/ffmpegcv.egg-info/SOURCES.txt` & `ffmpegcv-0.3.9/ffmpegcv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ffmpegcv-0.3.8/setup.py` & `ffmpegcv-0.3.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text('utf-8')
 
 setup(
     name='ffmpegcv', # 应用名
-    version='0.3.8', # 版本号
+    version='0.3.9', # 版本号
     packages=find_packages(include=['ffmpegcv*']), # 包括在安装包内的 Python 包
     author='chenxf',
     author_email='cxf529125853@163.com',
     url='https://github.com/chenxinfeng4/ffmpegcv',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

