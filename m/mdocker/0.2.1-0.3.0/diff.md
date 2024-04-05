# Comparing `tmp/mdocker-0.2.1.tar.gz` & `tmp/mdocker-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdocker-0.2.1.tar", max compression
+gzip compressed data, was "mdocker-0.3.0.tar", max compression
```

## Comparing `mdocker-0.2.1.tar` & `mdocker-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,19 @@
--rw-r--r--   0        0        0     1065 2023-12-01 08:47:05.685802 mdocker-0.2.1/LICENSE.md
--rw-r--r--   0        0        0     2305 2023-12-01 08:47:05.685802 mdocker-0.2.1/README.md
--rw-r--r--   0        0        0     1724 2023-12-01 08:47:05.685802 mdocker-0.2.1/mdocker/__main__.py
--rw-r--r--   0        0        0       34 2023-12-01 08:47:05.685802 mdocker-0.2.1/mdocker/models/__init__.py
--rw-r--r--   0        0        0      175 2023-12-01 08:47:27.541732 mdocker-0.2.1/mdocker/models/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     4737 2023-12-01 08:47:27.541732 mdocker-0.2.1/mdocker/models/__pycache__/builder.cpython-312.pyc
--rw-r--r--   0        0        0     3118 2023-12-01 08:47:05.685802 mdocker-0.2.1/mdocker/models/builder.py
--rw-r--r--   0        0        0       74 2023-12-01 08:47:05.685802 mdocker-0.2.1/mdocker/tools/__init__.py
--rw-r--r--   0        0        0      255 2023-12-01 08:47:27.541732 mdocker-0.2.1/mdocker/tools/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     1608 2023-12-01 08:47:27.541732 mdocker-0.2.1/mdocker/tools/__pycache__/commands.cpython-312.pyc
--rw-r--r--   0        0        0      948 2023-12-01 08:47:27.545732 mdocker-0.2.1/mdocker/tools/__pycache__/messages.cpython-312.pyc
--rw-r--r--   0        0        0     1116 2023-12-01 08:47:05.685802 mdocker-0.2.1/mdocker/tools/commands.py
--rw-r--r--   0        0        0      404 2023-12-01 08:47:05.685802 mdocker-0.2.1/mdocker/tools/messages.py
--rw-r--r--   0        0        0      575 2023-12-01 08:47:05.685802 mdocker-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2960 1970-01-01 00:00:00.000000 mdocker-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-05 17:46:07.774645 mdocker-0.3.0/LICENSE.md
+-rw-r--r--   0        0        0     2332 2024-04-05 17:46:07.774645 mdocker-0.3.0/README.md
+-rw-r--r--   0        0        0     2306 2024-04-05 17:46:07.774645 mdocker-0.3.0/mdocker/__main__.py
+-rw-r--r--   0        0        0       34 2024-04-05 17:46:07.774645 mdocker-0.3.0/mdocker/interfaces/__init__.py
+-rw-r--r--   0        0        0      179 2024-04-05 17:46:28.766705 mdocker-0.3.0/mdocker/interfaces/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     1489 2024-04-05 17:46:28.766705 mdocker-0.3.0/mdocker/interfaces/__pycache__/models.cpython-312.pyc
+-rw-r--r--   0        0        0      789 2024-04-05 17:46:07.774645 mdocker-0.3.0/mdocker/interfaces/models.py
+-rw-r--r--   0        0        0       40 2024-04-05 17:46:07.774645 mdocker-0.3.0/mdocker/models/__init__.py
+-rw-r--r--   0        0        0      181 2024-04-05 17:46:28.602705 mdocker-0.3.0/mdocker/models/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     3988 2024-04-05 17:46:28.602705 mdocker-0.3.0/mdocker/models/__pycache__/image_builder.cpython-312.pyc
+-rw-r--r--   0        0        0     2669 2024-04-05 17:46:07.774645 mdocker-0.3.0/mdocker/models/image_builder.py
+-rw-r--r--   0        0        0        0 2024-04-05 17:46:07.774645 mdocker-0.3.0/mdocker/tools/__init__.py
+-rw-r--r--   0        0        0      127 2024-04-05 17:46:28.766705 mdocker-0.3.0/mdocker/tools/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     1627 2024-04-05 17:46:28.766705 mdocker-0.3.0/mdocker/tools/__pycache__/commands.cpython-312.pyc
+-rw-r--r--   0        0        0      968 2024-04-05 17:46:28.766705 mdocker-0.3.0/mdocker/tools/__pycache__/messages.cpython-312.pyc
+-rw-r--r--   0        0        0     1166 2024-04-05 17:46:07.774645 mdocker-0.3.0/mdocker/tools/commands.py
+-rw-r--r--   0        0        0      424 2024-04-05 17:46:07.774645 mdocker-0.3.0/mdocker/tools/messages.py
+-rw-r--r--   0        0        0      753 2024-04-05 17:46:07.778645 mdocker-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3111 1970-01-01 00:00:00.000000 mdocker-0.3.0/PKG-INFO
```

### Comparing `mdocker-0.2.1/LICENSE.md` & `mdocker-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mdocker-0.2.1/README.md` & `mdocker-0.3.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # mdocker
 
-An easy-to-use wrapper for multiplatform Docker image builds.
+An easy-to-use wrapper for multi-platform Docker image builds.
 
 ## Contents
 
 - [mdocker](#mdocker)
   - [Contents](#contents)
   - [Description](#description)
   - [Usage](#usage)
@@ -29,26 +29,26 @@
 
 mdocker requires an installation of Python 3.10+.
 
 Below is a help message with the description of arguments.
 
 ```help
 $ python3 -m mdocker --help
-usage:  [-h] [--context CONTEXT] [--file FILE] [--platform PLATFORM] [--push]
-        name
+usage: [-h] [--context BCONTEXT] [--file DFILE] [--platforms PLATFORMS] [--push] name
 
 positional arguments:
-  name                 specify a name for the image
+  name                  specify a name for the image
 
 options:
-  -h, --help           show this help message and exit
-  --context CONTEXT    specify a path to build context
-  --file FILE          specify a path to Dockerfile
-  --platform PLATFORM  specify target platforms (e.g., --platform linux/amd64,linux/arm64)
-  --push               push image to remote registry
+  -h, --help            show this help message and exit
+  --context BCONTEXT    specify a path to build context
+  --file DFILE          specify a path to Dockerfile
+  --platforms PLATFORMS
+                        specify target platforms (e.g., --platforms linux/amd64,linux/arm64)
+  --push                push image to remote registry
 ```
 
 ## Installation
 
 ### From PyPI (recommended)
 
 To install latest mdocker package from PyPI, use:
```

### Comparing `mdocker-0.2.1/mdocker/__main__.py` & `mdocker-0.3.0/mdocker/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,64 +1,80 @@
 import os
 import io
 import sys
 import argparse
+from pathlib import Path
 
-import mdocker.tools.messages as msg
-import mdocker.tools.commands as ccmd
-
-from mdocker.models.builder import ImageBuilder
+from mdocker.tools import commands as ccmd, messages as msg
+from mdocker.models import ImageBuilder
 
 
 def parse_args() -> argparse.Namespace:
     """Parse arguments."""
     args = None if sys.argv[1:] else ["-h"]
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "name",
         help="specify a name for the image"
     )
     parser.add_argument(
         "--context",
+        dest="bcontext",
         help="specify a path to build context"
     )
     parser.add_argument(
         "--file",
+        dest="dfile",
+        default=Path("Dockerfile"),
         help="specify a path to Dockerfile"
     )
     parser.add_argument(
-        "--platform",
-        help="specify target platforms (e.g., --platform linux/amd64,linux/arm64)"
+        "--platforms",
+        default=[
+            f"linux/{ccmd.launch('uname -m', get_output=True, quiet=True).replace('x86_64', 'amd64')}"
+        ],
+        help="specify target platforms (e.g., --platforms linux/amd64,linux/arm64)"
     )
     parser.add_argument(
         "--push",
         action="store_true",
         help="push image to remote registry"
     )
     return parser.parse_args(args)
 
 
-def validate() -> None:
+def validate_env() -> None:
     """Check and validate build environment."""
     # try calling "buildx" directly
     try:
         ccmd.launch("docker buildx version", quiet=True, dont_exit=True)
     except Exception:
         # attempt to enable buildx via environment variable
         msg.note("Attempting to enable buildx via environment variable..")
         os.environ["DOCKER_BUILDKIT"] = "1"
         ccmd.launch("docker buildx version", quiet=True)
         print("[ + ] Done!")
 
 
+def process_platforms(platforms: str | list[str]) -> list[str]:
+    """Process target platform list."""
+    if not isinstance(platforms, list):
+        return platforms.replace("x86_64", "amd64").split(",")
+    else:
+        return platforms
+
+
 def main(args: argparse.Namespace) -> None:
-    # for logs to always show in order
-    sys.stdout = io.TextIOWrapper(open(sys.stdout.fileno(), 'wb', 0), write_through=True)
-    # parse arguments and run
-    parse_args()
-    validate()
-    config = vars(args)
-    ImageBuilder(config).run()
+    # for logs to show in order in various CI/CD / Build systems
+    sys.stdout = io.TextIOWrapper(open(sys.stdout.fileno(), "wb", 0), write_through=True)
+    validate_env()
+    ImageBuilder(
+        name=args.name,
+        bcontext=args.bcontext,
+        dfile=args.dfile,
+        platforms=process_platforms(args.platforms),
+        push=args.push
+    ).run()
 
 
 if __name__ == "__main__":
     main(parse_args())
```

### Comparing `mdocker-0.2.1/mdocker/tools/__pycache__/commands.cpython-312.pyc` & `mdocker-0.3.0/mdocker/tools/__pycache__/commands.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Fri Dec  1 08:47:05 2023 UTC, .py size: 1116 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 15% similar despite different names*

```diff
@@ -1,101 +1,102 @@
-00000000: cb0d 0d0a 0000 0000 899d 6965 5c04 0000  ..........ie\...
-00000010: e300 0000 0000 0000 0000 0000 000d 0000  ................
-00000020: 0000 0000 00f3 6e00 0000 9700 6400 6401  ......n.....d.d.
-00000030: 6c00 5a00 6400 6402 6c01 6d02 5a02 6d03  l.Z.d.d.l.m.Z.m.
-00000040: 5a03 0100 6400 6401 6c04 6d05 6302 0100  Z...d.d.l.m.c...
-00000050: 6d06 5a07 0100 0900 0900 0900 6409 6403  m.Z.........d.d.
-00000060: 6508 6404 6503 6509 1900 0000 6405 6503  e.d.e.e.....d.e.
-00000070: 6509 1900 0000 6406 6503 6509 1900 0000  e.....d.e.e.....
-00000080: 6407 6502 6401 6508 6602 1900 0000 660a  d.e.d.e.f.....f.
-00000090: 6408 8405 5a0a 7901 290a e900 0000 004e  d...Z.y.)......N
-000000a0: 2902 da05 556e 696f 6eda 084f 7074 696f  )...Union..Optio
-000000b0: 6e61 6cda 0363 6d64 da05 7175 6965 74da  nal..cmd..quiet.
-000000c0: 0964 6f6e 745f 6578 6974 da0a 6765 745f  .dont_exit..get_
-000000d0: 6f75 7470 7574 da06 7265 7475 726e 6304  output..returnc.
-000000e0: 0000 0000 0000 0000 0000 0007 0000 0003  ................
-000000f0: 0000 00f3 7c01 0000 9700 7c01 730e 7401  ....|.....|.s.t.
-00000100: 0000 0000 0000 0000 6401 7c00 9b00 9d02  ........d.|.....
-00000110: ab01 0000 0000 0000 0100 7c01 7210 7402  ..........|.r.t.
-00000120: 0000 0000 0000 0000 6a04 0000 0000 0000  ........j.......
-00000130: 0000 0000 0000 0000 0000 0000 6e01 6402  ............n.d.
-00000140: 7d04 7c03 6403 7500 7210 7402 0000 0000  }.|.d.u.r.t.....
-00000150: 0000 0000 6a06 0000 0000 0000 0000 0000  ....j...........
-00000160: 0000 0000 0000 0000 7d04 0900 7403 0000  ........}...t...
-00000170: 0000 0000 0000 6a08 0000 0000 0000 0000  ......j.........
-00000180: 0000 0000 0000 0000 0000 7c00 6403 6403  ..........|.d.d.
-00000190: 7c04 7402 0000 0000 0000 0000 6a0a 0000  |.t.........j...
-000001a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000001b0: ac04 ab05 0000 0000 0000 7d05 7c03 6403  ..........}.|.d.
-000001c0: 7500 722c 7c05 6a0c 0000 0000 0000 0000  u.r,|.j.........
-000001d0: 0000 0000 0000 0000 0000 6a0f 0000 0000  ..........j.....
-000001e0: 0000 0000 0000 0000 0000 0000 0000 6405  ..............d.
-000001f0: ab01 0000 0000 0000 6a11 0000 0000 0000  ........j.......
-00000200: 0000 0000 0000 0000 0000 0000 ab00 0000  ................
-00000210: 0000 0000 6406 1900 0000 5300 7902 2300  ....d.....S.y.#.
-00000220: 7412 0000 0000 0000 0000 2400 721f 0100  t.........$.r...
-00000230: 7c02 731a 7415 0000 0000 0000 0000 6a16  |.s.t.........j.
-00000240: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000250: 0000 6407 7c00 9b00 9d02 ab01 0000 0000  ..d.|...........
-00000260: 0000 0100 5900 7902 5900 7902 7700 7803  ....Y.y.Y.y.w.x.
-00000270: 5900 7701 2908 6101 0100 0041 2073 696d  Y.w.).a....A sim
-00000280: 706c 6520 636f 6d6d 616e 6420 7772 6170  ple command wrap
-00000290: 7065 722e 0a0a 2020 2020 3a70 6172 616d  per...    :param
-000002a0: 2063 6d64 3a20 4120 636f 6d6d 616e 6420   cmd: A command 
-000002b0: 7468 6174 2069 7320 6265 696e 6720 6578  that is being ex
-000002c0: 6563 7574 6564 2e0a 2020 2020 3a70 6172  ecuted..    :par
-000002d0: 616d 2071 7569 6574 3a20 4f6d 6974 2063  am quiet: Omit c
-000002e0: 6f6d 6d61 6e64 2070 7269 6e74 6f75 742e  ommand printout.
-000002f0: 0a20 2020 203a 7061 7261 6d20 646f 6e74  .    :param dont
-00000300: 5f65 7869 743a 2044 6f20 6e6f 7420 6578  _exit: Do not ex
-00000310: 6974 2070 726f 6772 616d 2069 6620 616e  it program if an
-00000320: 2065 7272 6f72 206f 6363 7572 6564 2e0a   error occured..
-00000330: 2020 2020 3a70 6172 616d 2067 6574 5f6f      :param get_o
-00000340: 7574 7075 743a 2041 2073 7769 7463 6820  utput: A switch 
-00000350: 746f 2067 6574 2074 6865 2070 6970 6564  to get the piped
-00000360: 206f 7574 7075 7420 6f66 2074 6865 2063   output of the c
-00000370: 6f6d 6d61 6e64 2e0a 2020 2020 7a06 5b63  ommand..    z.[c
-00000380: 6d64 5d20 4e54 2904 da05 7368 656c 6cda  md] NT)...shell.
-00000390: 0563 6865 636b da06 7374 646f 7574 da06  .check..stdout..
-000003a0: 7374 6465 7272 7a05 7574 662d 3872 0200  stderrz.utf-8r..
-000003b0: 0000 7a19 4572 726f 7220 6578 6563 7574  ..z.Error execut
-000003c0: 696e 6720 636f 6d6d 616e 643a 2029 0cda  ing command: )..
-000003d0: 0570 7269 6e74 da0a 7375 6270 726f 6365  .print..subproce
-000003e0: 7373 da07 4445 564e 554c 4cda 0450 4950  ss..DEVNULL..PIP
-000003f0: 45da 0372 756e da06 5354 444f 5554 720d  E..run..STDOUTr.
-00000400: 0000 00da 0664 6563 6f64 65da 0a73 706c  .....decode..spl
-00000410: 6974 6c69 6e65 73da 0945 7863 6570 7469  itlines..Excepti
-00000420: 6f6e da03 6d73 67da 0565 7272 6f72 2906  on..msg..error).
-00000430: 7205 0000 0072 0600 0000 7207 0000 0072  r....r....r....r
-00000440: 0800 0000 da07 6373 7464 6f75 74da 0672  ......cstdout..r
-00000450: 6573 756c 7473 0600 0000 2020 2020 2020  esults....      
-00000460: fa1e 2f6f 7074 2f6d 646f 636b 6572 2f74  ../opt/mdocker/t
-00000470: 6f6f 6c73 2f63 6f6d 6d61 6e64 732e 7079  ools/commands.py
-00000480: da06 6c61 756e 6368 721d 0000 0007 0000  ..launchr.......
-00000490: 0073 b200 0000 8000 f11c 000c 11dc 080d  .s..............
-000004a0: 9006 9073 9065 886e d408 1de1 2429 8c6a  ...s.e.n....$).j
-000004b0: d70e 20d2 0e20 a874 8047 d807 1190 54d1  .. .. .t.G....T.
-000004c0: 0719 dc12 1c97 2f91 2f88 07f0 0207 0539  .....././......9
-000004d0: dc11 1b97 1e91 1ea0 03a8 34b0 74c0 47d4  ..........4.t.G.
-000004e0: 545e d754 65d1 5465 d411 6688 06e0 0b15  T^.Te.Te..f.....
-000004f0: 9814 d10b 1dd8 1319 973d 913d d713 27d1  .........=.=..'.
-00000500: 1327 a807 d313 30d7 133b d113 3bd3 133d  .'....0..;..;..=
-00000510: b861 d113 40d0 0c40 f003 000c 1ef8 e40b  .a..@..@........
-00000520: 14f2 0002 0539 d90f 18dc 0c0f 8f49 8949  .....9.......I.I
-00000530: d018 31b0 23b0 15d0 1637 d60c 38f1 0300  ..1.#....7..8...
-00000540: 1019 f003 0205 39fa 7312 0000 00ba 4117  ......9.s.....A.
-00000550: 4213 00c2 1323 423b 03c2 3a01 423b 0329  B....#B;..:.B;.)
-00000560: 0346 4646 290b 7210 0000 00da 0674 7970  .FFF).r......typ
-00000570: 696e 6772 0300 0000 7204 0000 00da 166d  ingr....r......m
-00000580: 646f 636b 6572 2e74 6f6f 6c73 2e6d 6573  docker.tools.mes
-00000590: 7361 6765 73da 0574 6f6f 6c73 da08 6d65  sages..tools..me
-000005a0: 7373 6167 6573 7218 0000 00da 0373 7472  ssagesr......str
-000005b0: da04 626f 6f6c 721d 0000 00a9 00f3 0000  ..boolr.........
-000005c0: 0000 721c 0000 00fa 083c 6d6f 6475 6c65  ..r......<module
-000005d0: 3e72 2600 0000 0100 0000 7364 0000 00f0  >r&.......sd....
-000005e0: 0301 0101 db00 11df 0022 e700 24d0 0024  ........."..$..$
-000005f0: f00a 0021 26d8 2429 d825 2af1 091b 0139  ...!&.$).%*....9
-00000600: d80d 10f0 031b 0139 e00f 1798 0489 7ef0  .......9......~.
-00000610: 051b 0139 f006 0014 1c98 4491 3ef0 071b  ...9......D.>...
-00000620: 0139 f008 0015 1d98 5491 4ef0 091b 0139  .9......T.N....9
-00000630: f00a 000a 0f88 7490 5388 79d1 0919 f40b  ......t.S.y.....
-00000640: 1b01 3972 2500 0000                      ..9r%...
+00000000: cb0d 0d0a 0000 0000 df38 1066 8e04 0000  .........8.f....
+00000010: e300 0000 0000 0000 0000 0000 000c 0000  ................
+00000020: 0000 0000 00f3 8000 0000 9700 6400 6401  ............d.d.
+00000030: 6c00 5a00 6400 6402 6c01 6d02 5a02 0100  l.Z.d.d.l.m.Z...
+00000040: 6400 6401 6c03 6d04 6302 0100 6d05 5a06  d.d.l.m.c...m.Z.
+00000050: 0100 0900 0900 0900 6409 6403 6507 6404  ........d.d.e.d.
+00000060: 6502 6508 1900 0000 6405 6502 6508 1900  e.e.....d.e.e...
+00000070: 0000 6406 6502 6508 1900 0000 6407 6500  ..d.e.e.....d.e.
+00000080: 6a12 0000 0000 0000 0000 0000 0000 0000  j...............
+00000090: 0000 0000 6507 7a07 0000 6401 7a07 0000  ....e.z...d.z...
+000000a0: 660a 6408 8405 5a0a 7901 290a e900 0000  f.d...Z.y.).....
+000000b0: 004e 2901 da08 4f70 7469 6f6e 616c da03  .N)...Optional..
+000000c0: 636d 64da 0571 7569 6574 da09 646f 6e74  cmd..quiet..dont
+000000d0: 5f65 7869 74da 0a67 6574 5f6f 7574 7075  _exit..get_outpu
+000000e0: 74da 0672 6574 7572 6e63 0400 0000 0000  t..returnc......
+000000f0: 0000 0000 0000 0700 0000 0300 0000 f378  ...............x
+00000100: 0100 0097 007c 0173 0e74 0100 0000 0000  .....|.s.t......
+00000110: 0000 0064 017c 009b 009d 02ab 0100 0000  ...d.|..........
+00000120: 0000 0001 007c 0172 1074 0200 0000 0000  .....|.r.t......
+00000130: 0000 006a 0400 0000 0000 0000 0000 0000  ...j............
+00000140: 0000 0000 0000 006e 0164 027d 047c 0364  .......n.d.}.|.d
+00000150: 0375 0072 1074 0200 0000 0000 0000 006a  .u.r.t.........j
+00000160: 0600 0000 0000 0000 0000 0000 0000 0000  ................
+00000170: 0000 007d 0409 0074 0300 0000 0000 0000  ...}...t........
+00000180: 006a 0800 0000 0000 0000 0000 0000 0000  .j..............
+00000190: 0000 0000 007c 0064 0364 037c 0474 0200  .....|.d.d.|.t..
+000001a0: 0000 0000 0000 006a 0a00 0000 0000 0000  .......j........
+000001b0: 0000 0000 0000 0000 0000 00ac 04ab 0500  ................
+000001c0: 0000 0000 007d 057c 0364 0375 0072 297c  .....}.|.d.u.r)|
+000001d0: 056a 0c00 0000 0000 0000 0000 0000 0000  .j..............
+000001e0: 0000 0000 006a 0f00 0000 0000 0000 0000  .....j..........
+000001f0: 0000 0000 0000 0000 0064 05ab 0100 0000  .........d......
+00000200: 0000 006a 1100 0000 0000 0000 0000 0000  ...j............
+00000210: 0000 0000 0000 00ab 0000 0000 0000 0053  ...............S
+00000220: 007c 0553 0023 0074 1200 0000 0000 0000  .|.S.#.t........
+00000230: 0024 0072 1f01 007c 0273 1a74 1500 0000  .$.r...|.s.t....
+00000240: 0000 0000 006a 1600 0000 0000 0000 0000  .....j..........
+00000250: 0000 0000 0000 0000 0064 067c 009b 009d  .........d.|....
+00000260: 02ab 0100 0000 0000 0001 0059 0079 0259  ...........Y.y.Y
+00000270: 0079 0277 0078 0359 0077 0129 0761 0101  .y.w.x.Y.w.).a..
+00000280: 0000 4120 7369 6d70 6c65 2063 6f6d 6d61  ..A simple comma
+00000290: 6e64 2077 7261 7070 6572 2e0a 0a20 2020  nd wrapper...   
+000002a0: 203a 7061 7261 6d20 636d 643a 2041 2063   :param cmd: A c
+000002b0: 6f6d 6d61 6e64 2074 6861 7420 6973 2062  ommand that is b
+000002c0: 6569 6e67 2065 7865 6375 7465 642e 0a20  eing executed.. 
+000002d0: 2020 203a 7061 7261 6d20 7175 6965 743a     :param quiet:
+000002e0: 204f 6d69 7420 636f 6d6d 616e 6420 7072   Omit command pr
+000002f0: 696e 746f 7574 2e0a 2020 2020 3a70 6172  intout..    :par
+00000300: 616d 2064 6f6e 745f 6578 6974 3a20 446f  am dont_exit: Do
+00000310: 206e 6f74 2065 7869 7420 7072 6f67 7261   not exit progra
+00000320: 6d20 6966 2061 6e20 6572 726f 7220 6f63  m if an error oc
+00000330: 6375 7265 642e 0a20 2020 203a 7061 7261  cured..    :para
+00000340: 6d20 6765 745f 6f75 7470 7574 3a20 4120  m get_output: A 
+00000350: 7377 6974 6368 2074 6f20 6765 7420 7468  switch to get th
+00000360: 6520 7069 7065 6420 6f75 7470 7574 206f  e piped output o
+00000370: 6620 7468 6520 636f 6d6d 616e 642e 0a20  f the command.. 
+00000380: 2020 207a 065b 636d 645d 204e 5429 04da     z.[cmd] NT)..
+00000390: 0573 6865 6c6c da05 6368 6563 6bda 0673  .shell..check..s
+000003a0: 7464 6f75 74da 0673 7464 6572 727a 0575  tdout..stderrz.u
+000003b0: 7466 2d38 7a19 4572 726f 7220 6578 6563  tf-8z.Error exec
+000003c0: 7574 696e 6720 636f 6d6d 616e 643a 2029  uting command: )
+000003d0: 0cda 0570 7269 6e74 da0a 7375 6270 726f  ...print..subpro
+000003e0: 6365 7373 da07 4445 564e 554c 4cda 0450  cess..DEVNULL..P
+000003f0: 4950 45da 0372 756e da06 5354 444f 5554  IPE..run..STDOUT
+00000400: 720c 0000 00da 0664 6563 6f64 65da 0672  r......decode..r
+00000410: 7374 7269 70da 0945 7863 6570 7469 6f6e  strip..Exception
+00000420: da03 6d73 67da 0565 7272 6f72 2906 7204  ..msg..error).r.
+00000430: 0000 0072 0500 0000 7206 0000 0072 0700  ...r....r....r..
+00000440: 0000 da07 6373 7464 6f75 74da 0672 6573  ....cstdout..res
+00000450: 756c 7473 0600 0000 2020 2020 2020 fa1e  ults....      ..
+00000460: 2f6f 7074 2f6d 646f 636b 6572 2f74 6f6f  /opt/mdocker/too
+00000470: 6c73 2f63 6f6d 6d61 6e64 732e 7079 da06  ls/commands.py..
+00000480: 6c61 756e 6368 721c 0000 0007 0000 0073  launchr........s
+00000490: ad00 0000 8000 f11c 000c 11dc 080d 9006  ................
+000004a0: 9073 9065 886e d408 1de1 2429 8c6a d70e  .s.e.n....$).j..
+000004b0: 20d2 0e20 a874 8047 d807 1190 54d1 0719   .. .t.G....T...
+000004c0: dc12 1c97 2f91 2f88 07f0 0209 0539 dc11  ...././......9..
+000004d0: 1b97 1e91 1ea0 03a8 34b0 74c0 47d4 545e  ........4.t.G.T^
+000004e0: d754 65d1 5465 d411 6688 06e0 0b15 9814  .Te.Te..f.......
+000004f0: d10b 1dd8 1319 973d 913d d713 27d1 1327  .......=.=..'..'
+00000500: a807 d313 30d7 1337 d113 37d3 1339 d00c  ....0..7..7..9..
+00000510: 39e0 1319 884d f8dc 0b14 f200 0205 39d9  9....M........9.
+00000520: 0f18 dc0c 0f8f 4989 49d0 1831 b023 b015  ......I.I..1.#..
+00000530: d016 37d6 0c38 f103 0010 19f0 0302 0539  ..7..8.........9
+00000540: fa73 1800 0000 ba41 1442 1100 c20f 0142  .s.....A.B.....B
+00000550: 1100 c211 2342 3903 c238 0142 3903 2903  ....#B9..8.B9.).
+00000560: 4646 4629 0b72 0f00 0000 da06 7479 7069  FFF).r......typi
+00000570: 6e67 7203 0000 00da 166d 646f 636b 6572  ngr......mdocker
+00000580: 2e74 6f6f 6c73 2e6d 6573 7361 6765 73da  .tools.messages.
+00000590: 0574 6f6f 6c73 da08 6d65 7373 6167 6573  .tools..messages
+000005a0: 7217 0000 00da 0373 7472 da04 626f 6f6c  r......str..bool
+000005b0: da10 436f 6d70 6c65 7465 6450 726f 6365  ..CompletedProce
+000005c0: 7373 721c 0000 00a9 00f3 0000 0000 721b  ssr...........r.
+000005d0: 0000 00fa 083c 6d6f 6475 6c65 3e72 2600  .....<module>r&.
+000005e0: 0000 0100 0000 736b 0000 00f0 0301 0101  ......sk........
+000005f0: db00 11dd 001b e700 24d0 0024 f00a 0021  ........$..$...!
+00000600: 26d8 2429 d825 2af1 091d 0139 d80d 10f0  &.$).%*....9....
+00000610: 031d 0139 e00f 1798 0489 7ef0 051d 0139  ...9......~....9
+00000620: f006 0014 1c98 4491 3ef0 071d 0139 f008  ......D.>....9..
+00000630: 0015 1d98 5491 4ef0 091d 0139 f00a 000a  ....T.N....9....
+00000640: 14d7 0924 d109 24a0 73d1 092a a854 d109  ...$..$.s..*.T..
+00000650: 31f4 0b1d 0139 7225 0000 00              1....9r%...
```

### Comparing `mdocker-0.2.1/mdocker/tools/__pycache__/messages.cpython-312.pyc` & `mdocker-0.3.0/mdocker/tools/__pycache__/messages.cpython-312.pyc`

 * *Files 6% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xcb0d0d0a
-moddate:  0x899d6965 (Fri Dec  1 08:47:05 2023 UTC)
-files sz: 404
+moddate:  0xdf381066 (Fri Apr  5 17:46:07 2024 UTC)
+files sz: 424
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
       0x9700640064016c005a00640284005a016406640384015a02640484005a
@@ -49,15 +49,15 @@
            6           2 LOAD_GLOBAL              1 (NULL + print)
                       14 LOAD_FAST                0 (msgtext)
                       16 FORMAT_VALUE             0
                       18 BUILD_STRING             2
                       20 CALL                     1
                       30 PRECALL                  2
          consts
-            'A "note" wrapper.'
+            'A "note" text wrapper.'
             '[ * ] '
             None
          names      ('print',)
          varnames   ('msgtext',)
          freevars   ()
          cellvars   ()
          filename   '/opt/mdocker/tools/messages.py'
@@ -106,15 +106,15 @@
                       90 CACHE
                       92 CACHE
                       94 CACHE
                       96 LOAD_CONST               3 (1)
                       98 CALL                     1
                      108 PRECALL                  4
          consts
-            'An "error" wrapper.'
+            'An "error" text wrapper.'
             '[ ! ] '
             ('file',)
             1
             None
          names      ('print', 'sys', 'stderr', 'exit')
          varnames   ('msgtext', 'dont_exit')
          freevars   ()
@@ -136,15 +136,15 @@
           18           2 LOAD_GLOBAL              1 (NULL + print)
                       14 LOAD_FAST                0 (msgtext)
                       16 FORMAT_VALUE             0
                       18 BUILD_STRING             2
                       20 CALL                     1
                       30 PRECALL                  2
          consts
-            'A "done" wrapper.'
+            'A "done" text wrapper.'
             '[ + ] '
             None
          names      ('print',)
          varnames   ('msgtext',)
          freevars   ()
          cellvars   ()
          filename   '/opt/mdocker/tools/messages.py'
@@ -164,15 +164,15 @@
           23           2 LOAD_GLOBAL              1 (NULL + print)
                       14 LOAD_FAST                0 (msgtext)
                       16 FORMAT_VALUE             0
                       18 BUILD_STRING             2
                       20 CALL                     1
                       30 PRECALL                  2
          consts
-            'A "cmd" wrapper.'
+            'A "cmd" text wrapper.'
             '[cmd] '
             None
          names      ('print',)
          varnames   ('msgtext',)
          freevars   ()
          cellvars   ()
          filename   '/opt/mdocker/tools/messages.py'
```

### Comparing `mdocker-0.2.1/mdocker/tools/commands.py` & `mdocker-0.3.0/mdocker/tools/commands.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import subprocess
-from typing import Union, Optional
+from typing import Optional
 
 import mdocker.tools.messages as msg
 
 
 def launch(
         cmd: str,
         quiet: Optional[bool] = False,
         dont_exit: Optional[bool] = False,
         get_output: Optional[bool] = False
-    ) -> Union[None, str]:
+    ) -> subprocess.CompletedProcess | str | None:
     """A simple command wrapper.
 
     :param cmd: A command that is being executed.
     :param quiet: Omit command printout.
     :param dont_exit: Do not exit program if an error occured.
     :param get_output: A switch to get the piped output of the command.
     """
@@ -24,11 +24,13 @@
     cstdout = subprocess.DEVNULL if quiet else None
     if get_output is True:
         cstdout = subprocess.PIPE
     try:
         result = subprocess.run(cmd, shell=True, check=True, stdout=cstdout, stderr=subprocess.STDOUT)
         # return only output if required
         if get_output is True:
-            return result.stdout.decode('utf-8').splitlines()[0]
+            return result.stdout.decode("utf-8").rstrip()
+        else:
+            return result
     except Exception:
         if not dont_exit:
             msg.error(f"Error executing command: {cmd}")
```

### Comparing `mdocker-0.2.1/PKG-INFO` & `mdocker-0.3.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 Metadata-Version: 2.1
 Name: mdocker
-Version: 0.2.1
-Summary: An easy-to-use wrapper for multiplatform Docker image builds.
+Version: 0.3.0
+Summary: An easy-to-use wrapper for multi-platform Docker image builds.
 Home-page: https://github.com/seppzer0/mdocker
 License: MIT
-Keywords: docker,docker-buildx
+Keywords: docker,docker-buildx,multi-platform
 Author: seppzer0
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: argparse (>=1.4.0,<2.0.0)
+Requires-Dist: pathlib (>=1.0,<2.0)
+Requires-Dist: pydantic (>=2.6,<3.0)
+Requires-Dist: typing (>=3.7,<4.0)
 Project-URL: Repository, https://github.com/seppzer0/mdocker
 Description-Content-Type: text/markdown
 
 # mdocker
 
-An easy-to-use wrapper for multiplatform Docker image builds.
+An easy-to-use wrapper for multi-platform Docker image builds.
 
 ## Contents
 
 - [mdocker](#mdocker)
   - [Contents](#contents)
   - [Description](#description)
   - [Usage](#usage)
@@ -47,26 +50,26 @@
 
 mdocker requires an installation of Python 3.10+.
 
 Below is a help message with the description of arguments.
 
 ```help
 $ python3 -m mdocker --help
-usage:  [-h] [--context CONTEXT] [--file FILE] [--platform PLATFORM] [--push]
-        name
+usage: [-h] [--context BCONTEXT] [--file DFILE] [--platforms PLATFORMS] [--push] name
 
 positional arguments:
-  name                 specify a name for the image
+  name                  specify a name for the image
 
 options:
-  -h, --help           show this help message and exit
-  --context CONTEXT    specify a path to build context
-  --file FILE          specify a path to Dockerfile
-  --platform PLATFORM  specify target platforms (e.g., --platform linux/amd64,linux/arm64)
-  --push               push image to remote registry
+  -h, --help            show this help message and exit
+  --context BCONTEXT    specify a path to build context
+  --file DFILE          specify a path to Dockerfile
+  --platforms PLATFORMS
+                        specify target platforms (e.g., --platforms linux/amd64,linux/arm64)
+  --push                push image to remote registry
 ```
 
 ## Installation
 
 ### From PyPI (recommended)
 
 To install latest mdocker package from PyPI, use:
```

