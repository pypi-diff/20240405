# Comparing `tmp/Hollos_Module-0.0.6-py3-none-any.whl.zip` & `tmp/Hollos_Module-0.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,9 @@
-Zip file size: 10934 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat    19137 b- defN 24-Mar-27 01:09 hollosmodule.py
--rw-rw-rw-  2.0 fat    19137 b- defN 24-Mar-27 01:09 Hollos_Module-0.0.6.data/scripts/hollosmodule.py
--rw-rw-rw-  2.0 fat      632 b- defN 24-Mar-27 01:20 Hollos_Module-0.0.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Mar-27 01:20 Hollos_Module-0.0.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       13 b- defN 24-Mar-27 01:20 Hollos_Module-0.0.6.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      500 b- defN 24-Mar-27 01:20 Hollos_Module-0.0.6.dist-info/RECORD
-6 files, 39511 bytes uncompressed, 10026 bytes compressed:  74.6%
+Zip file size: 14246 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat    22392 b- defN 24-Apr-05 06:20 hollosmodule.py
+-rw-rw-rw-  2.0 fat    22392 b- defN 24-Apr-05 06:20 Hollos_Module-0.0.7.data/scripts/hollosmodule.py
+-rw-rw-rw-  2.0 fat     1099 b- defN 24-Apr-05 06:38 Hollos_Module-0.0.7.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      911 b- defN 24-Apr-05 06:38 Hollos_Module-0.0.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-05 06:38 Hollos_Module-0.0.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       13 b- defN 24-Apr-05 06:38 Hollos_Module-0.0.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      594 b- defN 24-Apr-05 06:38 Hollos_Module-0.0.7.dist-info/RECORD
+7 files, 47493 bytes uncompressed, 13188 bytes compressed:  72.2%
```

## zipnote {}

```diff
@@ -1,19 +1,22 @@
 Filename: hollosmodule.py
 Comment: 
 
-Filename: Hollos_Module-0.0.6.data/scripts/hollosmodule.py
+Filename: Hollos_Module-0.0.7.data/scripts/hollosmodule.py
 Comment: 
 
-Filename: Hollos_Module-0.0.6.dist-info/METADATA
+Filename: Hollos_Module-0.0.7.dist-info/LICENSE
 Comment: 
 
-Filename: Hollos_Module-0.0.6.dist-info/WHEEL
+Filename: Hollos_Module-0.0.7.dist-info/METADATA
 Comment: 
 
-Filename: Hollos_Module-0.0.6.dist-info/top_level.txt
+Filename: Hollos_Module-0.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: Hollos_Module-0.0.6.dist-info/RECORD
+Filename: Hollos_Module-0.0.7.dist-info/top_level.txt
+Comment: 
+
+Filename: Hollos_Module-0.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hollosmodule.py

```diff
@@ -1,24 +1,54 @@
 """
+The MIT License (MIT)
+
+Copyright (c) 2023-present Hollo
+
+Permission is hereby granted, free of charge, to any person obtaining a
+copy of this software and associated documentation files (the "Software"),
+to deal in the Software without restriction, including without limitation
+the rights to use, copy, modify, merge, publish, distribute, sublicense,
+and/or sell copies of the Software, and to permit persons to whom the
+Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
+OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
+FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+
+----------------
+
 ![logo](https://devhollo.github.io/!assets/dev_assets/hollosmodule/img/logo.png)
 see the Github page [here](https://github.com/DevHollo/Hollos-Module)
 """
-from typing import Literal, Union
+from typing import (
+    Literal,
+    Union,
+    TypeAlias,
+    NoReturn,
+    Self
+)
 
 def check_for_latest_hollosmodule_version():
     """
     Checks if you have the latest version of Hollo's Module. If not, it installs the latest version.
     """
     from importlib import metadata as pypi
     import subprocess
     import requests
     import logging
     try:
-        user_ver = str(pypi.version('hxml'))
-        pypi_ver = str(requests.get("https://pypi.org/pypi/HollosModule/json").json()['info']['version'])
+        user_ver = str(pypi.version('Hollos-Module'))
+        pypi_ver = str(requests.get("https://pypi.org/pypi/Hollos-Module/json").json()['info']['version'])
         if not user_ver == pypi_ver:
             subprocess.run(['pip', 'install', f'hxml=={pypi_ver}'])
         else:
             pass
     except pypi.PackageNotFoundError as e:
         logging.error(f"Package HollosModule not found: {e}")
     except requests.RequestException as e:
@@ -601,26 +631,92 @@
             )
             self.__qrraw.add_data(data)
             self.__qrraw.make(fit=True)
             self.__qrimg = self.__qrraw.make_image(fill_color=fill_color, back_color=background_color)
         except Exception as e:
             raise Exception(e)
 
-    def save_qr(self, p: str):
+    def save_qr(self, p: str, *args, **kwargs):
         """
         Save QR code.
         """
         try:
             self.__qrimg.save(p)
             self.fp = p
         except Exception as e:
             raise Exception(e)
         
-    def delete_qr(self):
+    def delete_qr(self, *args, **kwargs):
         """
         Delete the QR code.
         """
         import os
         if self.fp:
             os.remove(os.path.abspath(self.fp))
         else:
-            raise FileNotFoundError("File not found")
+            raise FileNotFoundError("File not found")
+        
+    def visualize(self, *args, **kwargs):
+        self.__qrimg.show()
+
+class WinOS:
+    """
+    Commands for the Windows OS!
+    """
+    def __init__(self: Self, *args, **kwargs):
+        pass
+
+    @staticmethod
+    def exit(__status: TypeAlias | str | int | None = None, /) -> NoReturn:
+        """
+        Exit the console/app
+        """
+        import sys
+        sys.exit(__status)
+
+    @staticmethod
+    def pause(hide: bool = True, /) -> None:
+        """
+        This method pauses the script execution until the user presses a key. It optionally hides the `Press any key to continue...` message.
+        """
+        import os
+        if hide is True:
+            os.system("pause > nul")
+        elif hide is False:
+            os.system("pause")
+        else:
+            raise ValueError("Error with kw \'hide\'")
+        
+    @staticmethod
+    def timeout(t: int | float, /, *, nobreak: bool = True, hide: bool = False) -> None:
+        """
+        This method waits for a specified amount of time (in seconds). It can optionally hide the countdown timer and/or prevent users from breaking out of the wait by pressing a key.
+        """
+        import os
+        if nobreak is True:
+            if hide is True:
+                os.system(f"timeout /t {t} /nobreak > nul")
+            elif hide is False:
+                os.system(f"timeout /t {t} /nobreak")
+        elif nobreak is False:
+            if hide is True:
+                os.system(f"timeout /t {t} > nul")
+            elif hide is False:
+                os.system(f"timeout /t {t}")
+        else:
+            raise ValueError("Error with keywords in func \'WinOS().timeout()\'")
+        
+    @staticmethod
+    def cls() -> None:
+        """
+        Clear the console
+        """
+        import os
+        os.system("cls")
+    
+    @staticmethod
+    def cmd(command: str | None, /) -> None:
+        """
+        Run a command
+        """
+        import os
+        os.system(command)
```

## Comparing `Hollos_Module-0.0.6.data/scripts/hollosmodule.py` & `Hollos_Module-0.0.7.data/scripts/hollosmodule.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,54 @@
 """
+The MIT License (MIT)
+
+Copyright (c) 2023-present Hollo
+
+Permission is hereby granted, free of charge, to any person obtaining a
+copy of this software and associated documentation files (the "Software"),
+to deal in the Software without restriction, including without limitation
+the rights to use, copy, modify, merge, publish, distribute, sublicense,
+and/or sell copies of the Software, and to permit persons to whom the
+Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
+OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
+FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+
+----------------
+
 ![logo](https://devhollo.github.io/!assets/dev_assets/hollosmodule/img/logo.png)
 see the Github page [here](https://github.com/DevHollo/Hollos-Module)
 """
-from typing import Literal, Union
+from typing import (
+    Literal,
+    Union,
+    TypeAlias,
+    NoReturn,
+    Self
+)
 
 def check_for_latest_hollosmodule_version():
     """
     Checks if you have the latest version of Hollo's Module. If not, it installs the latest version.
     """
     from importlib import metadata as pypi
     import subprocess
     import requests
     import logging
     try:
-        user_ver = str(pypi.version('hxml'))
-        pypi_ver = str(requests.get("https://pypi.org/pypi/HollosModule/json").json()['info']['version'])
+        user_ver = str(pypi.version('Hollos-Module'))
+        pypi_ver = str(requests.get("https://pypi.org/pypi/Hollos-Module/json").json()['info']['version'])
         if not user_ver == pypi_ver:
             subprocess.run(['pip', 'install', f'hxml=={pypi_ver}'])
         else:
             pass
     except pypi.PackageNotFoundError as e:
         logging.error(f"Package HollosModule not found: {e}")
     except requests.RequestException as e:
@@ -601,26 +631,92 @@
             )
             self.__qrraw.add_data(data)
             self.__qrraw.make(fit=True)
             self.__qrimg = self.__qrraw.make_image(fill_color=fill_color, back_color=background_color)
         except Exception as e:
             raise Exception(e)
 
-    def save_qr(self, p: str):
+    def save_qr(self, p: str, *args, **kwargs):
         """
         Save QR code.
         """
         try:
             self.__qrimg.save(p)
             self.fp = p
         except Exception as e:
             raise Exception(e)
         
-    def delete_qr(self):
+    def delete_qr(self, *args, **kwargs):
         """
         Delete the QR code.
         """
         import os
         if self.fp:
             os.remove(os.path.abspath(self.fp))
         else:
-            raise FileNotFoundError("File not found")
+            raise FileNotFoundError("File not found")
+        
+    def visualize(self, *args, **kwargs):
+        self.__qrimg.show()
+
+class WinOS:
+    """
+    Commands for the Windows OS!
+    """
+    def __init__(self: Self, *args, **kwargs):
+        pass
+
+    @staticmethod
+    def exit(__status: TypeAlias | str | int | None = None, /) -> NoReturn:
+        """
+        Exit the console/app
+        """
+        import sys
+        sys.exit(__status)
+
+    @staticmethod
+    def pause(hide: bool = True, /) -> None:
+        """
+        This method pauses the script execution until the user presses a key. It optionally hides the `Press any key to continue...` message.
+        """
+        import os
+        if hide is True:
+            os.system("pause > nul")
+        elif hide is False:
+            os.system("pause")
+        else:
+            raise ValueError("Error with kw \'hide\'")
+        
+    @staticmethod
+    def timeout(t: int | float, /, *, nobreak: bool = True, hide: bool = False) -> None:
+        """
+        This method waits for a specified amount of time (in seconds). It can optionally hide the countdown timer and/or prevent users from breaking out of the wait by pressing a key.
+        """
+        import os
+        if nobreak is True:
+            if hide is True:
+                os.system(f"timeout /t {t} /nobreak > nul")
+            elif hide is False:
+                os.system(f"timeout /t {t} /nobreak")
+        elif nobreak is False:
+            if hide is True:
+                os.system(f"timeout /t {t} > nul")
+            elif hide is False:
+                os.system(f"timeout /t {t}")
+        else:
+            raise ValueError("Error with keywords in func \'WinOS().timeout()\'")
+        
+    @staticmethod
+    def cls() -> None:
+        """
+        Clear the console
+        """
+        import os
+        os.system("cls")
+    
+    @staticmethod
+    def cmd(command: str | None, /) -> None:
+        """
+        Run a command
+        """
+        import os
+        os.system(command)
```

## Comparing `Hollos_Module-0.0.6.dist-info/METADATA` & `Hollos_Module-0.0.7.dist-info/METADATA`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,28 @@
 Metadata-Version: 2.1
 Name: Hollos-Module
-Version: 0.0.6
+Version: 0.0.7
 Home-page: https://github.com/DevHollo/Hollos-Module
 Author: Hollo
 Author-email: hollo1234567890e@gmail.com
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: sty ==1.0.6
 Requires-Dist: requests ==2.31.0
 Requires-Dist: getpass4 ==0.0.14.1
 Requires-Dist: pillow ==10.2.0
 Requires-Dist: qrcode ==7.4.2
 
 # Hollo's Module
 ![logo](https://devhollo.github.io/!assets/dev_assets/hollosmodule/img/logo.png)<br/>
 Hollo's Module is a module with a BUNCH of cool stuff
 
 # Examples
 See examples [here](https://github.com/DevHollo/Hollos-Module/tree/main/examples)
+
+# Other Stuff/Info
+- [License](https://github.com/DevHollo/Hollos-Module/blob/main/LICENSE)
+- [Source Code](https://github.com/DevHollo/Hollos-Module/tree/main)
+
+----
+
+***FULL CREDIT FOR A LOT OF STUFF GOES TO THE MODULES USED IN THIS MODULE!!***
```

