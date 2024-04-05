# Comparing `tmp/sheetfusion-1.0.5.tar.gz` & `tmp/sheetfusion-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "sheetfusion-1.0.6.tar", last modified: Fri Apr  5 14:19:32 2024, max compression
```

## Comparing `sheetfusion-1.0.5.tar` & `sheetfusion-1.0.6.tar`

### file list

```diff
@@ -1,12 +1,38 @@
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 sheetfusion-1.0.5/sheetfusion/__init__.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 sheetfusion-1.0.5/sheetfusion/__main__.py
--rw-r--r--   0        0        0     4435 2020-02-02 00:00:00.000000 sheetfusion-1.0.5/sheetfusion/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sheetfusion-1.0.5/sheetfusion/args/__init__.py
--rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 sheetfusion-1.0.5/sheetfusion/args/parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sheetfusion-1.0.5/sheetfusion/utils/__init__.py
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 sheetfusion-1.0.5/sheetfusion/utils/progress.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 sheetfusion-1.0.5/.gitignore
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 sheetfusion-1.0.5/LICENSE
--rw-r--r--   0        0        0     4289 2020-02-02 00:00:00.000000 sheetfusion-1.0.5/README.md
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 sheetfusion-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     4851 2020-02-02 00:00:00.000000 sheetfusion-1.0.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:19:32.367844 sheetfusion-1.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:19:32.359844 sheetfusion-1.0.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:19:32.363844 sheetfusion-1.0.6/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-05 14:19:24.000000 sheetfusion-1.0.6/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-05 14:19:24.000000 sheetfusion-1.0.6/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:19:32.363844 sheetfusion-1.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-04-05 14:19:24.000000 sheetfusion-1.0.6/.github/workflows/workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-05 14:19:24.000000 sheetfusion-1.0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-05 14:19:24.000000 sheetfusion-1.0.6/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-05 14:19:24.000000 sheetfusion-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-04-05 14:19:32.367844 sheetfusion-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-04-05 14:19:24.000000 sheetfusion-1.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:19:32.363844 sheetfusion-1.0.6/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)   181035 2024-04-05 14:19:24.000000 sheetfusion-1.0.6/assets/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-05 14:19:24.000000 sheetfusion-1.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-05 14:19:24.000000 sheetfusion-1.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 14:19:32.367844 sheetfusion-1.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:19:32.359844 sheetfusion-1.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:19:32.363844 sheetfusion-1.0.6/src/sheetfusion/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-05 14:19:24.000000 sheetfusion-1.0.6/src/sheetfusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-05 14:19:24.000000 sheetfusion-1.0.6/src/sheetfusion/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-05 14:19:32.000000 sheetfusion-1.0.6/src/sheetfusion/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:19:32.363844 sheetfusion-1.0.6/src/sheetfusion/args/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 14:19:24.000000 sheetfusion-1.0.6/src/sheetfusion/args/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-04-05 14:19:24.000000 sheetfusion-1.0.6/src/sheetfusion/args/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:19:32.363844 sheetfusion-1.0.6/src/sheetfusion/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-05 14:19:24.000000 sheetfusion-1.0.6/src/sheetfusion/assets/ascii_logo.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-04-05 14:19:24.000000 sheetfusion-1.0.6/src/sheetfusion/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:19:32.367844 sheetfusion-1.0.6/src/sheetfusion/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 14:19:24.000000 sheetfusion-1.0.6/src/sheetfusion/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-05 14:19:24.000000 sheetfusion-1.0.6/src/sheetfusion/utils/progress.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:19:32.367844 sheetfusion-1.0.6/src/sheetfusion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-04-05 14:19:32.000000 sheetfusion-1.0.6/src/sheetfusion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-05 14:19:32.000000 sheetfusion-1.0.6/src/sheetfusion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 14:19:32.000000 sheetfusion-1.0.6/src/sheetfusion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-05 14:19:32.000000 sheetfusion-1.0.6/src/sheetfusion.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-05 14:19:32.000000 sheetfusion-1.0.6/src/sheetfusion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-05 14:19:32.000000 sheetfusion-1.0.6/src/sheetfusion.egg-info/top_level.txt
```

### Comparing `sheetfusion-1.0.5/sheetfusion/main.py` & `sheetfusion-1.0.6/src/sheetfusion/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,83 +11,99 @@
 
 START_DT_STR = datetime.now().strftime(r"%Y%m%d_%H%M%S")
 SCRIPTDIR = os.getcwd()
 
 
 def main():
     console = Console()
-    logo = """                                                                                                                                        
-╔═╗╦ ╦╔═╗╔═╗╔╦╗╔═╗╦ ╦╔═╗╦╔═╗╔╗╔
-╚═╗╠═╣║╣ ║╣  ║ ╠╣ ║ ║╚═╗║║ ║║║║
-╚═╝╩ ╩╚═╝╚═╝ ╩ ╚  ╚═╝╚═╝╩╚═╝╝╚╝
-"""
+    logo = (
+        Path(__file__)
+        .parent.joinpath("assets")
+        .joinpath("ascii_logo.txt")
+        .read_text()
+    )
     console.print(f"[bold green1]{logo}[/bold green1]")
     try:
         console.print(
-            f"[bold green1]v{pkg_resources.get_distribution('sheetfusion').version}[bold green1]\n\n"
+            "[bold green1]"
+            f"v{pkg_resources.get_distribution('sheetfusion').version}"
+            "[bold green1]\n\n"
         )
     except pkg_resources.DistributionNotFound:
-        console.print(f"[bold green1]v0.0.0[bold green1]\n\n")
+        console.print("[bold green1]v0.0.0[bold green1]\n\n")
 
     args = parse_args()
 
     cover_sheets_file = Path(args.cover_sheets_file)
     if not cover_sheets_file.exists():
         console.print(
-            f"[bold red]Error: The file '{cover_sheets_file}' does not exist.[/bold red]"
+            "[bold red]Error:"
+            f" The file '{cover_sheets_file}' does not exist.[/bold red]"
         )
         return
 
     exam_file = Path(args.exam_file)
     if not exam_file.exists():
         console.print(
-            f"[bold red]Error: The file '{exam_file}' does not exist.[/bold red]"
+            "[bold red]Error:"
+            f" The file '{exam_file}' does not exist.[/bold red]"
         )
         return
 
     output_dir = Path(args.output_dir)
     if not output_dir.exists():
-        info_message = f"[bold cyan]Info:[/bold cyan] [bold white]The directory '{output_dir}' does not exist. Creating it now.[/bold white]"
+        info_message = (
+            "[bold cyan]Info:[/bold cyan]"
+            f" [bold white]The directory '{output_dir}' does not exist."
+            " Creating it now.[/bold white]"
+        )
         console.print(info_message)
         try:
             os.makedirs(output_dir)
         except Exception as e:
             console.print(
-                f"[bold red]Error: Failed to create the directory '{output_dir}'[/bold red]"
+                "[bold red]Error:"
+                f"Failed to create the directory '{output_dir}'[/bold red]"
             )
             console.print(e)
             return
 
-    with TitledProgress(
-        title=f"start: [green]{START_DT_STR}[/green]"
-    ) as progress, open(cover_sheets_file, "rb") as covers, open(
-        exam_file, "rb"
-    ) as exam:
+    with (
+        TitledProgress(
+            title=f"start: [green]{START_DT_STR}[/green]"
+        ) as progress,
+        open(cover_sheets_file, "rb") as covers,
+        open(exam_file, "rb") as exam,
+    ):
         console = progress.console
         cover_reader = PyPDF3.PdfFileReader(covers)
         exam_reader = PyPDF3.PdfFileReader(exam)
 
         n_exams = cover_reader.numPages
         n_exam_pages = exam_reader.numPages
 
-        bar = "-" * 50  # Adjust the number based on your desired width
+        bar = "-" * 50
 
         progress.print(f"[bold cyan]{bar}[/bold cyan]")
         progress.print(
-            f"[bold blue]cover_sheets_file:[/bold blue] [white]{cover_sheets_file}[/white]"
+            f"[bold blue]cover_sheets_file:[/bold blue]"
+            f" [white]{cover_sheets_file}[/white]"
+        )
+        progress.print(
+            "[bold blue]exam_file:[/bold blue]" f" [white]{exam_file}[/white]"
         )
-        progress.print(f"[bold blue]exam_file:[/bold blue] [white]{exam_file}[/white]")
         progress.print(
             f"[bold blue]output_dir:[/bold blue] [white]{output_dir}[/white]"
         )
         progress.print(
             f"[bold blue]number of exams:[/bold blue] [white]{n_exams}[/white]"
         )
         progress.print(
-            f"[bold blue]number of exam pages:[/bold blue] [white]{n_exam_pages}[/white]"
+            "[bold blue]number of exam pages:[/bold blue]"
+            f" [white]{n_exam_pages}[/white]"
         )
         progress.print(f"[bold cyan]{bar}[/bold cyan]")
         print("\n")
 
         all_exams_task = progress.add_task(
             f"All Exam - total = {n_exams} exams", total=n_exams
         )
@@ -104,15 +120,17 @@
             for j in range(exam_reader.numPages):
                 writer.addPage(exam_reader.getPage(j))
                 progress.update(this_exam_task, advance=1)
 
             write_path = output_dir / f"{i+1:0{n_leading_zeros}d}.pdf"
             if write_path.exists() and not args.overwrite:
                 console.print(
-                    f"[bold red]Warning:[/bold red] [white]The file '{write_path}' already exists. Skipping.[white]"
+                    "[bold red]Warning:[/bold red]"
+                    f" [white]The file '{write_path}' already exists."
+                    " Skipping.[white]"
                 )
                 progress.update(all_exams_task, advance=1)
                 progress.remove_task(this_exam_task)
                 continue
             with open(write_path, "wb") as output_pdf:
                 writer.write(output_pdf)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `sheetfusion-1.0.5/sheetfusion/args/parser.py` & `sheetfusion-1.0.6/src/sheetfusion/args/parser.py`

 * *Files identical despite different names*

### Comparing `sheetfusion-1.0.5/sheetfusion/utils/progress.py` & `sheetfusion-1.0.6/src/sheetfusion/utils/progress.py`

 * *Files identical despite different names*

### Comparing `sheetfusion-1.0.5/LICENSE` & `sheetfusion-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sheetfusion-1.0.5/README.md` & `sheetfusion-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `sheetfusion-1.0.5/pyproject.toml` & `sheetfusion-1.0.6/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,28 @@
 [build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
-
-[tool.hatch.build.targets.wheel]
-packages = ["sheetfusion"]
-exclude = ["__pycache__/*"]
-
-[tool.hatch.build.targets.sdist]
-packages = ["sheetfusion"]
-exclude = ["__pycache__/*"]
+requires = ["setuptools>=64", "setuptools_scm>=8"]
+build-backend = "setuptools.build_meta"
 
 [project]
 name = "sheetfusion"
-version = "1.0.5"
 authors = [{ name = "Mohammad Znz", email = "s.mohammad.znz@gmail.com" }]
 description = ""
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
 ]
 dependencies = ["PyPDF3~=1.0.6", "rich~=13.7.0", "setuptools~=69.0.2"]
+dynamic = ["version"]
 
 
 [project.urls]
 "Homepage" = "https://github.com/SMZ70/SheetFusion"
 "Bug Tracker" = "https://github.com/SMZ70/SheetFusion/issues"
 
 [project.scripts]
 sheetfusion = "sheetfusion:main"
+
+[tool.setuptools_scm]
+version_file = "src/sheetfusion/_version.py"
```

### Comparing `sheetfusion-1.0.5/PKG-INFO` & `sheetfusion-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: sheetfusion
-Version: 1.0.5
+Version: 1.0.6
+Author-email: Mohammad Znz <s.mohammad.znz@gmail.com>
 Project-URL: Homepage, https://github.com/SMZ70/SheetFusion
 Project-URL: Bug Tracker, https://github.com/SMZ70/SheetFusion/issues
-Author-email: Mohammad Znz <s.mohammad.znz@gmail.com>
-License-File: LICENSE
+Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
-Requires-Dist: pypdf3~=1.0.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: PyPDF3~=1.0.6
 Requires-Dist: rich~=13.7.0
 Requires-Dist: setuptools~=69.0.2
-Description-Content-Type: text/markdown
 
 [python]: https://img.shields.io/badge/-Python-3776AB?logo=python&logoColor=white
 [version]: https://img.shields.io/badge/Version-1.0.5-blue
 
 ![python][python]
 ![version][version]
```

