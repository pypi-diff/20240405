# Comparing `tmp/dotlocalslashbin-0.0.2.tar.gz` & `tmp/dotlocalslashbin-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dotlocalslashbin-0.0.2.tar", last modified: Thu Apr  4 07:35:12 2024, max compression
+gzip compressed data, was "dotlocalslashbin-0.0.3.tar", last modified: Fri Apr  5 05:58:57 2024, max compression
```

## Comparing `dotlocalslashbin-0.0.2.tar` & `dotlocalslashbin-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 07:35:12.000000 dotlocalslashbin-0.0.2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 07:35:12.000000 dotlocalslashbin-0.0.2/LICENSES/
--rw-r--r--   0 root         (0) root         (0)    16727 2024-04-04 07:35:12.000000 dotlocalslashbin-0.0.2/LICENSES/MPL-2.0.txt
--rw-r--r--   0 root         (0) root         (0)      879 2024-04-04 07:35:12.000000 dotlocalslashbin-0.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      223 2024-04-04 07:35:12.000000 dotlocalslashbin-0.0.2/README.md
--rw-r--r--   0 root         (0) root         (0)      797 2024-04-04 07:35:12.000000 dotlocalslashbin-0.0.2/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 07:35:12.000000 dotlocalslashbin-0.0.2/src/
--rwxr-xr-x   0 root         (0) root         (0)     5579 2024-04-04 07:35:12.000000 dotlocalslashbin-0.0.2/src/dotlocalslashbin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 05:58:57.000000 dotlocalslashbin-0.0.3/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 05:58:57.000000 dotlocalslashbin-0.0.3/LICENSES/
+-rw-r--r--   0 root         (0) root         (0)    16727 2024-04-05 05:58:57.000000 dotlocalslashbin-0.0.3/LICENSES/MPL-2.0.txt
+-rw-r--r--   0 root         (0) root         (0)      880 2024-04-05 05:58:57.000000 dotlocalslashbin-0.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      224 2024-04-05 05:58:57.000000 dotlocalslashbin-0.0.3/README.md
+-rw-r--r--   0 root         (0) root         (0)      797 2024-04-05 05:58:57.000000 dotlocalslashbin-0.0.3/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 05:58:57.000000 dotlocalslashbin-0.0.3/src/
+-rwxr-xr-x   0 root         (0) root         (0)     5693 2024-04-05 05:58:57.000000 dotlocalslashbin-0.0.3/src/dotlocalslashbin.py
```

### Comparing `dotlocalslashbin-0.0.2/LICENSES/MPL-2.0.txt` & `dotlocalslashbin-0.0.3/LICENSES/MPL-2.0.txt`

 * *Files identical despite different names*

### Comparing `dotlocalslashbin-0.0.2/PKG-INFO` & `dotlocalslashbin-0.0.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dotlocalslashbin
-Version: 0.0.2
+Version: 0.0.3
 Summary: Download and extract files to ~/.local/bin/
 Author-email: Keith Maxwell <keith.maxwell@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Requires-Dist: black ; extra == "test"
 Requires-Dist: codespell ; extra == "test"
@@ -14,14 +14,13 @@
 Requires-Dist: usort ; extra == "test"
 Project-URL: Home, https://github.com/maxwell-k/dotlocalslashbin/
 Provides-Extra: test
 
 Download and extract files to ~/.local/bin/
 
 <!--
-.flake8
+README.md
 SPDX-FileCopyrightText: 2024 Keith Maxwell <keith.maxwell@gmail.com>
 SPDX-License-Identifier: CC0-1.0
 -->
-
 <!-- vim: set filetype=markdown.htmlCommentNoSpell  : -->
```

### Comparing `dotlocalslashbin-0.0.2/pyproject.toml` & `dotlocalslashbin-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dotlocalslashbin-0.0.2/src/dotlocalslashbin.py` & `dotlocalslashbin-0.0.3/src/dotlocalslashbin.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,30 +14,29 @@
 from hashlib import file_digest
 from pathlib import Path
 from shlex import split
 from shutil import copy
 from stat import S_IEXEC
 from subprocess import run
 from tomllib import load
-from typing import cast
 from urllib.request import urlopen
 from zipfile import ZipFile
 
 
-__version__ = "0.0.2"
+__version__ = "0.0.3"
 
 
 @contextmanager
 def _download(
     args: Namespace,
     *,
     name: str,
     url: str,
+    target: Path | None = None,
     action: str | None = None,
-    target: str | None = None,
     expected: str | None = None,
     version: str | None = None,
     prefix: str | None = None,
     completions: str | None = None,
     command: str | None = None,
     ignore: set = set(),
 ) -> Generator[tuple[Path, Path], None, None]:
@@ -50,15 +49,16 @@
         expected: the SHA256 or SHA512 hex-digest of the file at URL
         version: an argument to display the version for example --version
         prefix: to remove when untarring
         completions: whether to generate ZSH completions
         command: command to run to install after download
     """
     if target is None:
-        target = cast(str, args.output) + name
+        target = args.output.joinpath(name)
+    assert target is not None
 
     if url.startswith("https://"):
         downloaded = Path(args.downloaded).expanduser() / url.rsplit("/", 1)[1]
         downloaded.parent.mkdir(parents=True, exist_ok=True)
         if not downloaded.is_file():
             with urlopen(url) as fp, downloaded.open("wb") as dp:
                 if "content-length" in fp.headers:
@@ -82,90 +82,90 @@
             if (actual := digest.hexdigest()) != expected:
                 raise RuntimeError(
                     f"Unexpected digest for {downloaded}: {actual=} {expected=}"
                 )
     else:
         downloaded = Path(url)
 
-    target_path = Path(target).expanduser()
-    target_path.parent.mkdir(parents=True, exist_ok=True)
-    target_path.unlink(missing_ok=True)
-
     if action is None:
         if url.endswith(".tar.gz"):
             action = "untar"
         elif url.endswith(".zip"):
             action = "unzip"
         elif url.startswith("/"):
             action = "symlink"
         elif command:
             action = "command"
         else:
             action = "copy"
 
+    message = ("#" if version else "$") + f" {target} " + (version or "")
+    target = target.expanduser()
+    target.parent.mkdir(parents=True, exist_ok=True)
+    target.unlink(missing_ok=True)
     if action == "copy":
-        copy(downloaded, target_path)
+        copy(downloaded, target)
     elif action == "symlink":
-        target_path.symlink_to(downloaded)
+        target.symlink_to(downloaded)
     elif action == "unzip":
         with ZipFile(downloaded, "r") as file:
-            file.extract(target_path.name, path=target_path.parent)
+            file.extract(target.name, path=target.parent)
     elif action == "untar":
         with tarfile.open(downloaded, "r") as file:
             for member in file.getmembers():
                 if prefix:
                     member.path = member.path.removeprefix(prefix)
                 if member.path in ignore:
                     continue
-                file.extract(member, path=target_path.parent)
+                file.extract(member, path=target.parent)
     elif action == "command" and command is not None:
-        kwargs = dict(target=target_path, downloaded=downloaded)
+        kwargs = dict(target=target, downloaded=downloaded)
         run(split(command.format(**kwargs)), check=True)
 
-    yield downloaded, target_path
+    yield downloaded, target
 
-    if not target_path.is_symlink():
-        target_path.chmod(target_path.stat().st_mode | S_IEXEC)
+    if not target.is_symlink():
+        target.chmod(target.stat().st_mode | S_IEXEC)
 
     if completions:
-        output = Path(args.completions).expanduser() / f"_{target_path.name}"
+        output = Path(args.completions).expanduser() / f"_{target.name}"
         output.parent.mkdir(parents=True, exist_ok=True)
-        kwargs = dict(target=target_path)  # target may not be on PATH
+        kwargs = dict(target=target)  # target may not be on PATH
         with output.open("w") as file:
             run(split(completions.format(**kwargs)), check=True, stdout=file)
 
-    if version is None:
-        print(f"# {target}")
-    else:
-        print(f"$ {target} {version}")
-        run([target_path, version], check=True)
+    print(message)
+    if version:
+        run([target, version], check=True)
 
     print()
 
 
 def main() -> int:
     parser = ArgumentParser(prog=Path(__file__).name, formatter_class=formatter_class)
     parser.add_argument("--version", action="version", version=__version__)
-    parser.add_argument("--input", default="bin.toml", help="TOML specification")
-    parser.add_argument("--output", default="~/.local/bin/", help="Target directory")
-    parser.add_argument(
-        "--downloaded", default="~/.cache/dotlocalslashbin/", help="Download directory"
-    )
-    parser.add_argument(
-        "--completions",
-        default="~/.local/share/zsh/site-functions/",
-        help="Directory for ZSH completions",
-    )
+    help_ = "TOML specification"
+    parser.add_argument("--input", default="bin.toml", help=help_, type=Path)
+    help_ = "Target directory"
+    parser.add_argument("--output", default="~/.local/bin/", help=help_, type=Path)
+    help_ = "Download directory"
+    default = "~/.cache/dotlocalslashbin/"
+    parser.add_argument("--downloaded", default=default, help=help_)
+    help_ = "Directory for ZSH completions"
+    default = "~/.local/share/zsh/site-functions/"
+    parser.add_argument("--completions", default=default, help=help_)
     args = parser.parse_args()
 
-    with open(args.input, "rb") as file:
+    with args.input.expanduser().open("rb") as file:
         data = load(file)
 
     for name, kwargs in data.items():
         kwargs["name"] = name
+        if "target" in kwargs:
+            kwargs["target"] = Path(kwargs["target"])
         with _download(args, **kwargs) as (downloaded, target):
             pass
 
     return 0
 
 
 if __name__ == "__main__":
```

