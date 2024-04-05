# Comparing `tmp/CodingRider-1.1.tar.gz` & `tmp/CodingRider-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CodingRider-1.1.tar", last modified: Thu Apr  4 04:14:28 2024, max compression
+gzip compressed data, was "CodingRider-2.0.tar", last modified: Fri Apr  5 00:20:22 2024, max compression
```

## Comparing `CodingRider-1.1.tar` & `CodingRider-2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 04:14:28.606468 CodingRider-1.1/
-drwxrwxrwx   0        0        0        0 2024-04-04 04:14:28.589754 CodingRider-1.1/CodingRider/
--rw-rw-rw-   0        0        0      109 2024-04-04 04:14:10.000000 CodingRider-1.1/CodingRider/__init__.py
--rw-rw-rw-   0        0        0      484 2023-12-25 23:04:18.000000 CodingRider-1.1/CodingRider/__main__.py
--rw-rw-rw-   0        0        0     4609 2023-03-28 08:35:12.000000 CodingRider-1.1/CodingRider/crc.py
--rw-rw-rw-   0        0        0    43609 2024-03-28 06:44:10.000000 CodingRider-1.1/CodingRider/drone.py
--rw-rw-rw-   0        0        0    70379 2024-04-04 03:58:07.000000 CodingRider-1.1/CodingRider/protocol.py
--rw-rw-rw-   0        0        0     7088 2023-11-15 01:18:50.000000 CodingRider-1.1/CodingRider/receiver.py
--rw-rw-rw-   0        0        0     1904 2023-12-25 23:03:04.000000 CodingRider-1.1/CodingRider/storage.py
--rw-rw-rw-   0        0        0    10249 2023-03-28 08:35:12.000000 CodingRider-1.1/CodingRider/system.py
-drwxrwxrwx   0        0        0        0 2024-04-04 04:14:28.604434 CodingRider-1.1/CodingRider.egg-info/
--rw-rw-rw-   0        0        0      626 2024-04-04 04:14:28.000000 CodingRider-1.1/CodingRider.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      393 2024-04-04 04:14:28.000000 CodingRider-1.1/CodingRider.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 04:14:28.000000 CodingRider-1.1/CodingRider.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2024-04-04 04:14:28.000000 CodingRider-1.1/CodingRider.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-04 04:14:28.000000 CodingRider-1.1/CodingRider.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-03-28 08:35:12.000000 CodingRider-1.1/LICENSE
--rw-rw-rw-   0        0        0       36 2023-03-28 08:35:12.000000 CodingRider-1.1/MANIFEST.in
--rw-rw-rw-   0        0        0      626 2024-04-04 04:14:28.605470 CodingRider-1.1/PKG-INFO
--rw-rw-rw-   0        0        0      359 2023-11-15 03:15:25.000000 CodingRider-1.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-04 04:14:28.606468 CodingRider-1.1/setup.cfg
--rw-rw-rw-   0        0        0      778 2024-04-04 04:06:45.000000 CodingRider-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 00:20:22.026727 CodingRider-2.0/
+drwxrwxrwx   0        0        0        0 2024-04-05 00:20:22.007502 CodingRider-2.0/CodingRider/
+-rw-rw-rw-   0        0        0      132 2024-04-05 00:09:09.000000 CodingRider-2.0/CodingRider/__init__.py
+-rw-rw-rw-   0        0        0      484 2023-12-25 23:04:18.000000 CodingRider-2.0/CodingRider/__main__.py
+-rw-rw-rw-   0        0        0     4609 2023-03-28 08:35:12.000000 CodingRider-2.0/CodingRider/crc.py
+-rw-rw-rw-   0        0        0    44020 2024-04-05 00:11:47.000000 CodingRider-2.0/CodingRider/drone.py
+-rw-rw-rw-   0        0        0    70439 2024-04-05 00:10:08.000000 CodingRider-2.0/CodingRider/protocol.py
+-rw-rw-rw-   0        0        0     7088 2023-11-15 01:18:50.000000 CodingRider-2.0/CodingRider/receiver.py
+-rw-rw-rw-   0        0        0     1904 2023-12-25 23:03:04.000000 CodingRider-2.0/CodingRider/storage.py
+-rw-rw-rw-   0        0        0    10249 2023-03-28 08:35:12.000000 CodingRider-2.0/CodingRider/system.py
+drwxrwxrwx   0        0        0        0 2024-04-05 00:20:22.023500 CodingRider-2.0/CodingRider.egg-info/
+-rw-rw-rw-   0        0        0      626 2024-04-05 00:20:21.000000 CodingRider-2.0/CodingRider.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      393 2024-04-05 00:20:21.000000 CodingRider-2.0/CodingRider.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 00:20:21.000000 CodingRider-2.0/CodingRider.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2024-04-05 00:20:21.000000 CodingRider-2.0/CodingRider.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-05 00:20:21.000000 CodingRider-2.0/CodingRider.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-03-28 08:35:12.000000 CodingRider-2.0/LICENSE
+-rw-rw-rw-   0        0        0       36 2023-03-28 08:35:12.000000 CodingRider-2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      626 2024-04-05 00:20:22.025501 CodingRider-2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      359 2023-11-15 03:15:25.000000 CodingRider-2.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-05 00:20:22.026727 CodingRider-2.0/setup.cfg
+-rw-rw-rw-   0        0        0      772 2024-04-05 00:19:45.000000 CodingRider-2.0/setup.py
```

### Comparing `CodingRider-1.1/CodingRider/crc.py` & `CodingRider-2.0/CodingRider/crc.py`

 * *Files identical despite different names*

### Comparing `CodingRider-1.1/CodingRider/drone.py` & `CodingRider-2.0/CodingRider/drone.py`

 * *Files 1% similar despite different names*

```diff
@@ -1034,14 +1034,32 @@
 
         data.commandType    = CommandType.Backlight
         data.option         = int(flagPower)
 
         return self.transfer(header, data)
 
 
+
+    def sendSetSwarm(self):
+
+        header = Header()
+        
+        header.dataType = DataType.Command
+        header.length   = Command.getSize()
+        header.from_    = DeviceType.Base
+        header.to_      = DeviceType.Drone
+
+        data = Command()
+
+        data.commandType    = CommandType.SetSwarm
+        data.option         = 0
+
+        return self.transfer(header, data)
+
+
 # Setup End
 
 
 
 # Device Start
 
     def sendMotor(self, motor0, motor1, motor2, motor3):
```

### Comparing `CodingRider-1.1/CodingRider/protocol.py` & `CodingRider-2.0/CodingRider/protocol.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,14 +108,16 @@
 
     FlightEvent             = 0x07      # 비행 이벤트 실행
 
     SetDefault              = 0x08      # 기본 설정으로 초기화
     ModeController          = 0x0A      # 조종기 동작 모드(0x10:조종, 0x80:링크)
     Link                    = 0x0B      # 링크 제어(0:Client Mode, 1:Server Mode, 2:Pairing Start)
 
+    SetSwarm				= 0x0F		# 군집 고도제어 설정
+    
     ModeTest				= 0xF0      # 테스트 모드
     
     EndOfType               = 0xEC
 
 
 # CommandType End
```

### Comparing `CodingRider-1.1/CodingRider/receiver.py` & `CodingRider-2.0/CodingRider/receiver.py`

 * *Files identical despite different names*

### Comparing `CodingRider-1.1/CodingRider/storage.py` & `CodingRider-2.0/CodingRider/storage.py`

 * *Files identical despite different names*

### Comparing `CodingRider-1.1/CodingRider/system.py` & `CodingRider-2.0/CodingRider/system.py`

 * *Files identical despite different names*

### Comparing `CodingRider-1.1/CodingRider.egg-info/PKG-INFO` & `CodingRider-2.0/CodingRider.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CodingRider
-Version: 1.1
+Version: 2.0
 Summary: Library for CodingRider
 Home-page: https://imssam.me/shop/view.php?index_no=4031
 Author: ALUX
 Author-email: devdrone@aluxonline.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `CodingRider-1.1/PKG-INFO` & `CodingRider-2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CodingRider
-Version: 1.1
+Version: 2.0
 Summary: Library for CodingRider
 Home-page: https://imssam.me/shop/view.php?index_no=4031
 Author: ALUX
 Author-email: devdrone@aluxonline.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `CodingRider-1.1/setup.py` & `CodingRider-2.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,23 +2,20 @@
 # http://swdeveloper.tistory.com/34
 # https://code.tutsplus.com/ko/tutorials/how-to-share-your-python-packages--cms-26114
 # https://code.tutsplus.com/ko/tutorials/how-to-write-your-own-python-packages--cms-26076
 from setuptools import setup, find_packages
 
 setup(
     name = "CodingRider",
-    version = "1.1",
+    version = "2.0",
     description = "Library for CodingRider",
     author = "ALUX",
     author_email = "devdrone@aluxonline.com",
     url = "https://imssam.me/shop/view.php?index_no=4031",
     packages = find_packages(exclude=['tests']),
     install_requires = [
         'pyserial>=3.4',
         'numpy>=1.15.4',
         'colorama>=0.4.0'],
     long_description = open('README.md').read(),
     long_description_content_type='text/markdown',
 )
-
-
-
```

