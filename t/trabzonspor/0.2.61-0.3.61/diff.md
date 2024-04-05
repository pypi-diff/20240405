# Comparing `tmp/trabzonspor-0.2.61.tar.gz` & `tmp/trabzonspor-0.3.61.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trabzonspor-0.2.61.tar", max compression
+gzip compressed data, was "trabzonspor-0.3.61.tar", max compression
```

## Comparing `trabzonspor-0.2.61.tar` & `trabzonspor-0.3.61.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1071 2023-03-29 13:55:14.077715 trabzonspor-0.2.61/LICENSE.txt
--rw-r--r--   0        0        0      321 2023-03-29 13:55:14.077895 trabzonspor-0.2.61/README.md
--rw-r--r--   0        0        0     1347 2023-12-22 11:33:14.982508 trabzonspor-0.2.61/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-29 13:55:14.085813 trabzonspor-0.2.61/trabzonspor/__init__.py
--rw-r--r--   0        0        0     1037 2023-03-29 14:13:00.519180 trabzonspor-0.2.61/trabzonspor/cli.py
--rw-r--r--   0        0        0     5585 2023-04-10 08:54:59.823984 trabzonspor-0.2.61/trabzonspor/scrapper.py
--rw-r--r--   0        0        0     9719 2023-03-29 14:30:39.240396 trabzonspor-0.2.61/trabzonspor/screen.py
--rw-r--r--   0        0        0     1442 1970-01-01 00:00:00.000000 trabzonspor-0.2.61/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-04-05 13:26:53.465858 trabzonspor-0.3.61/LICENSE.txt
+-rw-r--r--   0        0        0      321 2023-03-29 13:55:14.077895 trabzonspor-0.3.61/README.md
+-rw-r--r--   0        0        0     1742 2024-04-05 13:21:04.272891 trabzonspor-0.3.61/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-29 13:55:14.085813 trabzonspor-0.3.61/trabzonspor/__init__.py
+-rw-r--r--   0        0        0     1037 2023-03-29 14:13:00.519180 trabzonspor-0.3.61/trabzonspor/cli.py
+-rw-r--r--   0        0        0     5585 2023-12-22 11:39:36.598926 trabzonspor-0.3.61/trabzonspor/scrapper.py
+-rw-r--r--   0        0        0     9768 2024-04-05 13:25:55.260179 trabzonspor-0.3.61/trabzonspor/screen.py
+-rw-r--r--   0        0        0     1543 1970-01-01 00:00:00.000000 trabzonspor-0.3.61/PKG-INFO
```

### Comparing `trabzonspor-0.2.61/LICENSE.txt` & `trabzonspor-0.3.61/LICENSE.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 MIT License
 
-Copyright (c) 2022 yarimdunya.com
+Copyright (c) 2022 omerfarukgul.com.tr
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `trabzonspor-0.2.61/trabzonspor/cli.py` & `trabzonspor-0.3.61/trabzonspor/cli.py`

 * *Files identical despite different names*

### Comparing `trabzonspor-0.2.61/trabzonspor/scrapper.py` & `trabzonspor-0.3.61/trabzonspor/scrapper.py`

 * *Files identical despite different names*

### Comparing `trabzonspor-0.2.61/trabzonspor/screen.py` & `trabzonspor-0.3.61/trabzonspor/screen.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,17 +55,17 @@
         for count, title in self.scrapper.cups:
             cups.add_row(count, " ", title)
         return Panel(Align.center(cups, vertical="middle"))
 
     @staticmethod
     def get_header_middle():
         logo = Group(
-            Align.center("[dark_red]Trabzon[/dark_red][dodger_blue1]spor[/dodger_blue1]\n"),
+            Align.center(":star:\n"),
+            Align.center("[dark_red]TRABZON[/dark_red][dodger_blue1]SPOR[/dodger_blue1]\n"),
             Align.center("1967"),
-
         )
         return Panel(Align.center(logo, vertical="middle"), style="bold", padding=1)
 
     def get_header_right(self):
         return Panel(Align.center(f"Kadro değeri\n[b]{self.scrapper.team_value}[/b]", vertical="middle"))
 
     def get_main_left_top(self):
@@ -73,15 +73,15 @@
         standings.add_column(header="#")
         standings.add_column(header="Kulüp")
         standings.add_column(header="Maçlar")
         standings.add_column(header="+/-")
         standings.add_column(header="Puan")
 
         for no, club, matches, average, points, highlight in self.scrapper.standings:
-            style = "u red on white" if highlight else None
+            style = "u dodger_blue1 on dark_red" if highlight else None
             standings.add_row(no, club, matches, average, points, style=style)
         return Panel(standings, title="[cyan][b]TABLO KESİTİ SÜPER LİG[/b][/cyan]", box=box.SQUARE)
 
     def get_main_left_bottom(self):
         truths = Table.grid(expand=True)
         truths.add_column()
         truths.add_column()
```

### Comparing `trabzonspor-0.2.61/PKG-INFO` & `trabzonspor-0.3.61/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 Metadata-Version: 2.1
 Name: trabzonspor
-Version: 0.2.61
+Version: 0.3.61
 Summary: trabzonspor cli!
 Home-page: https://github.com/ofaruk89/trabzonspor
 License: MIT
 Keywords: trabzonspor
 Author: Omer Faruk GUL
 Author-email: ofaruk89@gmail.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Dist: beautifulsoup4 (>=4.11.1,<5.0.0)
-Requires-Dist: requests (>=2.28.1,<3.0.0)
-Requires-Dist: rich (>=12.6.0,<13.0.0)
+Classifier: Programming Language :: Python :: 3.9
+Requires-Dist: beautifulsoup4 (>=4.12.3,<5.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: rich (>=13.7.0,<14.0.0)
 Project-URL: Repository, https://github.com/ofaruk89/trabzonspor
 Description-Content-Type: text/markdown
 
 # Trabzonspor
 
 TS CLI
```

