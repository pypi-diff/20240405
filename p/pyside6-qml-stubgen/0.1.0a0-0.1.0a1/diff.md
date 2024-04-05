# Comparing `tmp/pyside6_qml_stubgen-0.1.0a0.tar.gz` & `tmp/pyside6_qml_stubgen-0.1.0a1.tar.gz`

## Comparing `pyside6_qml_stubgen-0.1.0a0.tar` & `pyside6_qml_stubgen-0.1.0a1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a0/conftest.py
--rw-r--r--   0        0        0    22454 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a0/pyside6_qml_stubgen.py
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a0/requirements.txt
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a0/.github/workflows/test.yml
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a0/tests/__init__.py
--rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a0/tests/test_run.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a0/tests/reference/README
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a0/tests/reference/target/qmldir
--rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a0/tests/reference/target/qmltyperegistrations1-0.cpp
--rw-r--r--   0        0        0    15713 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a0/tests/reference/target/types1-0.json
--rw-r--r--   0        0        0     5207 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a0/tests/reference/target/types1-0.qmltypes
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a0/tests/reference/target/advanced/qmldir
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a0/tests/reference/target/advanced/qmltyperegistrations1-100.cpp
--rw-r--r--   0        0        0     5144 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a0/tests/reference/target/advanced/types1-100.json
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a0/tests/reference/target/advanced/types1-100.qmltypes
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a0/tests/reference/target/advanced2/qmldir
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a0/tests/reference/target/advanced2/qmltyperegistrations1-100.cpp
--rw-r--r--   0        0        0     5172 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a0/tests/reference/target/advanced2/types1-100.json
--rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a0/tests/reference/target/advanced2/types1-100.qmltypes
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a0/tests/reference/target/sub/qmldir
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a0/tests/reference/target/sub/qmltyperegistrations2-1.cpp
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a0/tests/reference/target/sub/types2-1.json
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a0/tests/reference/target/sub/types2-1.qmltypes
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a0/tests/target/__init__.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a0/tests/target/advanced.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a0/tests/target/advanced2.py
--rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a0/tests/target/clses.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a0/tests/target/clses2.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a0/tests/target/submodule.py
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a0/.gitignore
--rw-r--r--   0        0        0     7559 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a0/LICENCE.md
--rw-r--r--   0        0        0     2662 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a0/README.md
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a0/pyproject.toml
--rw-r--r--   0        0        0     4049 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a0/PKG-INFO
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/conftest.py
+-rw-r--r--   0        0        0    22552 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/pyside6_qml_stubgen.py
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/requirements.txt
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/.github/workflows/test.yml
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/tests/__init__.py
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/tests/test_run.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/tests/reference/README
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/tests/reference/target/qmldir
+-rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/tests/reference/target/qmltyperegistrations1-0.cpp
+-rw-r--r--   0        0        0    15713 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/tests/reference/target/types1-0.json
+-rw-r--r--   0        0        0     5207 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/tests/reference/target/types1-0.qmltypes
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/tests/reference/target/advanced/qmldir
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/tests/reference/target/advanced/qmltyperegistrations1-100.cpp
+-rw-r--r--   0        0        0     5144 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/tests/reference/target/advanced/types1-100.json
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/tests/reference/target/advanced/types1-100.qmltypes
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/tests/reference/target/advanced2/qmldir
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/tests/reference/target/advanced2/qmltyperegistrations1-100.cpp
+-rw-r--r--   0        0        0     5172 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/tests/reference/target/advanced2/types1-100.json
+-rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/tests/reference/target/advanced2/types1-100.qmltypes
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/tests/reference/target/sub/qmldir
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/tests/reference/target/sub/qmltyperegistrations2-1.cpp
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/tests/reference/target/sub/types2-1.json
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/tests/reference/target/sub/types2-1.qmltypes
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/tests/target/__init__.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/tests/target/advanced.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/tests/target/advanced2.py
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/tests/target/clses.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/tests/target/clses2.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/tests/target/submodule.py
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/.gitignore
+-rw-r--r--   0        0        0     7559 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/LICENCE.md
+-rw-r--r--   0        0        0     2662 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/README.md
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/pyproject.toml
+-rw-r--r--   0        0        0     4049 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/PKG-INFO
```

### Comparing `pyside6_qml_stubgen-0.1.0a0/pyside6_qml_stubgen.py` & `pyside6_qml_stubgen-0.1.0a1/pyside6_qml_stubgen.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Generate QML stub files (.qmltypes) from Python modules (which use PySide6)
 
 Usage:
-    pyside6-qml-stubgen <in-dir> --out-dir=<out-dir> [--ignore=<path>...] [--metatypes-dir=<dir>] [--qmltyperegistrar-path=<path>]
+    pyside6-qml-stubgen <in-dir>... --out-dir=<out-dir> [--ignore=<path>...] [--metatypes-dir=<dir>] [--qmltyperegistrar-path=<path>]
 
 Options:
     --ignore=<path>                     Ignore all Python files that are children of thispath
     --metatypes-dir=<dir>               Directory of the Qt 6 metatype files for core modules (automatically detected if not provided)
     --qmltyperegistrar-path=<path>      Path of the qmltyperegistrar tool (automatically detected if not provided)
 """
 
@@ -20,15 +20,14 @@
 import shutil
 import subprocess
 import sys
 import types
 import typing
 
 import docopt
-import typing_extensions
 from PySide6 import QtCore, QtQml
 
 T_TypeQObject = typing.TypeVar("T_TypeQObject", bound=QtCore.QObject)
 
 
 @dataclasses.dataclass
 class ExtraCollectedInfo:
@@ -534,15 +533,15 @@
 
     raise RuntimeError(
         "Could not find qmltyperegistrar. Provide it manually using the --qmltyperegistrar-path option"
     )
 
 
 def process(
-    in_dir: pathlib.Path,
+    in_dirs: typing.Sequence[pathlib.Path],
     ignore_dirs: typing.Sequence[pathlib.Path],
     out_dir: pathlib.Path,
     metatypes_dir: pathlib.Path | None,
     qmltyperegistrar_path: pathlib.Path | None,
     *,
     file_relative_path: pathlib.Path | None = None,
 ) -> None:
@@ -554,24 +553,26 @@
     extra_info = patches()
 
     if out_dir.exists():
         shutil.rmtree(out_dir)
     out_dir.mkdir()
     (out_dir / "README").write_text(
         f"""QML type stubs generated automatically using
-pyside6-qml-stubgen {in_dir} --out-dir {out_dir} {' '.join(f'--ignore {i}' for i in ignore_dirs)} --metatypes-dir {metatypes_dir} --qmltyperegistrar-path {qmltyperegistrar_path}"""
+pyside6-qml-stubgen {' '.join(map(str, in_dirs))} --out-dir {out_dir} {' '.join(f'--ignore {i}' for i in ignore_dirs)} --metatypes-dir {metatypes_dir} --qmltyperegistrar-path {qmltyperegistrar_path}"""
     )
 
     foreign_types = list(metatypes_dir.glob("*_metatypes.json"))
     type_dirs = []
 
     sys.path.append(".")
 
     print("Importing Python modules")
-    for fname in in_dir.rglob("*.py"):
+    for fname in itertools.chain.from_iterable(
+        in_dir.rglob("*.py") for in_dir in in_dirs
+    ):
         if any(ig in fname.parents for ig in ignore_dirs):
             continue
         module = ".".join(
             [x.name for x in fname.parents if x.name][::-1] + [fname.stem]
         )
         if module.endswith(".__init__"):
             module = module.removesuffix(".__init__")
@@ -630,15 +631,15 @@
             for line in sorted(lines):
                 f.write(line)
 
 
 def main() -> None:
     args = docopt.docopt(__doc__)
     process(
-        in_dir=pathlib.Path(args["<in-dir>"]),
+        in_dirs=[pathlib.Path(p) for p in args["<in-dir>"]],
         ignore_dirs=[pathlib.Path(ig) for ig in args["--ignore"]],
         out_dir=pathlib.Path(args["--out-dir"]),
         metatypes_dir=(
             pathlib.Path(args["--metatypes-dir"]) if args["--metatypes-dir"] else None
         ),
         qmltyperegistrar_path=(
             pathlib.Path(args["--qmltyperegistrar-path"])
```

### Comparing `pyside6_qml_stubgen-0.1.0a0/.github/workflows/test.yml` & `pyside6_qml_stubgen-0.1.0a1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a0/tests/test_run.py` & `pyside6_qml_stubgen-0.1.0a1/tests/test_run.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 TARGET_DIR = pathlib.Path(__file__).parent / "target"
 REFERENCE_DIR = pathlib.Path(__file__).parent / "reference"
 
 
 def test_run_and_compare(tmp_path: pathlib.Path) -> None:
     pyside6_qml_stubgen.process(
-        in_dir=TARGET_DIR.relative_to(pathlib.Path().resolve()),
+        in_dirs=[TARGET_DIR.relative_to(pathlib.Path().resolve())],
         ignore_dirs=[],
         out_dir=tmp_path,
         metatypes_dir=None,
         qmltyperegistrar_path=None,
         file_relative_path=TARGET_DIR.parent.parent,
     )
```

### Comparing `pyside6_qml_stubgen-0.1.0a0/tests/reference/target/qmltyperegistrations1-0.cpp` & `pyside6_qml_stubgen-0.1.0a1/tests/reference/target/qmltyperegistrations1-0.cpp`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a0/tests/reference/target/types1-0.json` & `pyside6_qml_stubgen-0.1.0a1/tests/reference/target/types1-0.json`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a0/tests/reference/target/types1-0.qmltypes` & `pyside6_qml_stubgen-0.1.0a1/tests/reference/target/types1-0.qmltypes`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a0/tests/reference/target/advanced/qmltyperegistrations1-100.cpp` & `pyside6_qml_stubgen-0.1.0a1/tests/reference/target/advanced/qmltyperegistrations1-100.cpp`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a0/tests/reference/target/advanced/types1-100.json` & `pyside6_qml_stubgen-0.1.0a1/tests/reference/target/advanced/types1-100.json`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a0/tests/reference/target/advanced/types1-100.qmltypes` & `pyside6_qml_stubgen-0.1.0a1/tests/reference/target/advanced/types1-100.qmltypes`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a0/tests/reference/target/advanced2/qmltyperegistrations1-100.cpp` & `pyside6_qml_stubgen-0.1.0a1/tests/reference/target/advanced2/qmltyperegistrations1-100.cpp`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a0/tests/reference/target/advanced2/types1-100.json` & `pyside6_qml_stubgen-0.1.0a1/tests/reference/target/advanced2/types1-100.json`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a0/tests/reference/target/advanced2/types1-100.qmltypes` & `pyside6_qml_stubgen-0.1.0a1/tests/reference/target/advanced2/types1-100.qmltypes`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a0/tests/reference/target/sub/qmltyperegistrations2-1.cpp` & `pyside6_qml_stubgen-0.1.0a1/tests/reference/target/sub/qmltyperegistrations2-1.cpp`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a0/tests/reference/target/sub/types2-1.json` & `pyside6_qml_stubgen-0.1.0a1/tests/reference/target/sub/types2-1.json`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a0/tests/reference/target/sub/types2-1.qmltypes` & `pyside6_qml_stubgen-0.1.0a1/tests/reference/target/sub/types2-1.qmltypes`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a0/tests/target/advanced.py` & `pyside6_qml_stubgen-0.1.0a1/tests/target/advanced.py`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a0/tests/target/advanced2.py` & `pyside6_qml_stubgen-0.1.0a1/tests/target/advanced2.py`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a0/tests/target/clses.py` & `pyside6_qml_stubgen-0.1.0a1/tests/target/clses.py`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a0/tests/target/clses2.py` & `pyside6_qml_stubgen-0.1.0a1/tests/target/clses2.py`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a0/LICENCE.md` & `pyside6_qml_stubgen-0.1.0a1/LICENCE.md`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a0/README.md` & `pyside6_qml_stubgen-0.1.0a1/README.md`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a0/pyproject.toml` & `pyside6_qml_stubgen-0.1.0a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a0/PKG-INFO` & `pyside6_qml_stubgen-0.1.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyside6-qml-stubgen
-Version: 0.1.0a0
+Version: 0.1.0a1
 Summary: Generate QML stub files (.qmltypes) from Python modules (which use PySide6)
 Project-URL: Homepage, https://github.com/matsjoyce/pyside6-qml-stubgen
 Project-URL: Repository, https://github.com/matsjoyce/pyside6-qml-stubgen.git
 Project-URL: Issues, https://github.com/matsjoyce/pyside6-qml-stubgen/issues
 Author: Matthew Joyce
 License-File: LICENCE.md
 Keywords: pyside6,qml,qt6,type checking
```

