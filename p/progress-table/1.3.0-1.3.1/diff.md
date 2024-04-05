# Comparing `tmp/progress-table-1.3.0.tar.gz` & `tmp/progress-table-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "progress-table-1.3.0.tar", last modified: Thu Apr  4 15:48:45 2024, max compression
+gzip compressed data, was "progress-table-1.3.1.tar", last modified: Fri Apr  5 20:03:00 2024, max compression
```

## Comparing `progress-table-1.3.0.tar` & `progress-table-1.3.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-04 15:48:45.159666 progress-table-1.3.0/
--rw-r--r--   0 gaha      (1000) gaha      (1000)     1052 2022-11-17 19:44:00.000000 progress-table-1.3.0/LICENSE.txt
--rw-r--r--   0 gaha      (1000) gaha      (1000)     4907 2024-04-04 15:48:45.159666 progress-table-1.3.0/PKG-INFO
--rw-r--r--   0 gaha      (1000) gaha      (1000)     4143 2024-03-12 12:06:20.000000 progress-table-1.3.0/README.md
-drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-04 15:48:45.156332 progress-table-1.3.0/progress_table/
--rw-r--r--   0 gaha      (1000) gaha      (1000)      287 2024-04-04 15:47:39.000000 progress-table-1.3.0/progress_table/__init__.py
-drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-04 15:48:45.159666 progress-table-1.3.0/progress_table/v0/
--rw-r--r--   0 gaha      (1000) gaha      (1000)       41 2024-04-04 15:47:39.000000 progress-table-1.3.0/progress_table/v0/__init__.py
--rw-r--r--   0 gaha      (1000) gaha      (1000)    23213 2024-04-04 15:47:39.000000 progress-table-1.3.0/progress_table/v0/progress_table.py
--rw-r--r--   0 gaha      (1000) gaha      (1000)     3028 2024-04-04 15:47:39.000000 progress-table-1.3.0/progress_table/v0/symbols.py
-drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-04 15:48:45.159666 progress-table-1.3.0/progress_table/v1/
--rw-r--r--   0 gaha      (1000) gaha      (1000)       41 2024-04-04 15:47:39.000000 progress-table-1.3.0/progress_table/v1/__init__.py
--rw-r--r--   0 gaha      (1000) gaha      (1000)    28478 2024-04-04 15:47:39.000000 progress-table-1.3.0/progress_table/v1/progress_table.py
--rw-r--r--   0 gaha      (1000) gaha      (1000)     3132 2024-04-04 15:47:39.000000 progress-table-1.3.0/progress_table/v1/styles.py
-drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-04 15:48:45.159666 progress-table-1.3.0/progress_table.egg-info/
--rw-r--r--   0 gaha      (1000) gaha      (1000)     4907 2024-04-04 15:48:44.000000 progress-table-1.3.0/progress_table.egg-info/PKG-INFO
--rw-r--r--   0 gaha      (1000) gaha      (1000)     4883 2024-03-12 12:10:39.000000 progress-table-1.3.0/progress_table.egg-info/PKG-INFO.sync-conflict-20240314-015933-NXTV2IO
--rw-r--r--   0 gaha      (1000) gaha      (1000)      531 2024-04-04 15:48:45.000000 progress-table-1.3.0/progress_table.egg-info/SOURCES.txt
--rw-r--r--   0 gaha      (1000) gaha      (1000)        1 2024-04-04 15:48:44.000000 progress-table-1.3.0/progress_table.egg-info/dependency_links.txt
--rw-r--r--   0 gaha      (1000) gaha      (1000)        9 2024-04-04 15:48:44.000000 progress-table-1.3.0/progress_table.egg-info/requires.txt
--rw-r--r--   0 gaha      (1000) gaha      (1000)       15 2024-04-04 15:48:44.000000 progress-table-1.3.0/progress_table.egg-info/top_level.txt
--rw-r--r--   0 gaha      (1000) gaha      (1000)      207 2024-03-11 20:11:56.000000 progress-table-1.3.0/pyproject.toml
--rw-r--r--   0 gaha      (1000) gaha      (1000)      110 2024-04-04 15:48:45.162999 progress-table-1.3.0/setup.cfg
--rw-r--r--   0 gaha      (1000) gaha      (1000)     1504 2024-04-04 15:47:39.000000 progress-table-1.3.0/setup.py
+drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-05 20:03:00.837732 progress-table-1.3.1/
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     1052 2022-11-17 19:44:00.000000 progress-table-1.3.1/LICENSE.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     4907 2024-04-05 20:03:00.837732 progress-table-1.3.1/PKG-INFO
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     4143 2024-03-12 12:06:20.000000 progress-table-1.3.1/README.md
+drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-05 20:03:00.834399 progress-table-1.3.1/progress_table/
+-rw-r--r--   0 gaha      (1000) gaha      (1000)      287 2024-04-05 20:02:34.000000 progress-table-1.3.1/progress_table/__init__.py
+drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-05 20:03:00.837732 progress-table-1.3.1/progress_table/v0/
+-rw-r--r--   0 gaha      (1000) gaha      (1000)       41 2024-04-05 19:18:13.000000 progress-table-1.3.1/progress_table/v0/__init__.py
+-rw-r--r--   0 gaha      (1000) gaha      (1000)    23444 2024-04-05 20:02:34.000000 progress-table-1.3.1/progress_table/v0/progress_table.py
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     3028 2024-04-04 15:47:39.000000 progress-table-1.3.1/progress_table/v0/symbols.py
+drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-05 20:03:00.837732 progress-table-1.3.1/progress_table/v1/
+-rw-r--r--   0 gaha      (1000) gaha      (1000)       41 2024-04-04 15:47:39.000000 progress-table-1.3.1/progress_table/v1/__init__.py
+-rw-r--r--   0 gaha      (1000) gaha      (1000)    29325 2024-04-05 20:02:34.000000 progress-table-1.3.1/progress_table/v1/progress_table.py
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     3132 2024-04-04 15:47:39.000000 progress-table-1.3.1/progress_table/v1/styles.py
+drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-05 20:03:00.837732 progress-table-1.3.1/progress_table.egg-info/
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     4907 2024-04-05 20:03:00.000000 progress-table-1.3.1/progress_table.egg-info/PKG-INFO
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     4883 2024-03-12 12:10:39.000000 progress-table-1.3.1/progress_table.egg-info/PKG-INFO.sync-conflict-20240314-015933-NXTV2IO
+-rw-r--r--   0 gaha      (1000) gaha      (1000)      531 2024-04-05 20:03:00.000000 progress-table-1.3.1/progress_table.egg-info/SOURCES.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1000)        1 2024-04-05 20:03:00.000000 progress-table-1.3.1/progress_table.egg-info/dependency_links.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1000)        9 2024-04-05 20:03:00.000000 progress-table-1.3.1/progress_table.egg-info/requires.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1000)       15 2024-04-05 20:03:00.000000 progress-table-1.3.1/progress_table.egg-info/top_level.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1000)      207 2024-03-11 20:11:56.000000 progress-table-1.3.1/pyproject.toml
+-rw-r--r--   0 gaha      (1000) gaha      (1000)      110 2024-04-05 20:03:00.837732 progress-table-1.3.1/setup.cfg
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     1504 2024-04-04 15:47:39.000000 progress-table-1.3.1/setup.py
```

### Comparing `progress-table-1.3.0/LICENSE.txt` & `progress-table-1.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `progress-table-1.3.0/PKG-INFO` & `progress-table-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: progress-table
-Version: 1.3.0
+Version: 1.3.1
 Summary: Display progress as a pretty table in the command line.
 Home-page: https://github.com/gahaalt/progress-table.git
 Author: Szymon Mikler
 Author-email: sjmikler@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `progress-table-1.3.0/README.md` & `progress-table-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `progress-table-1.3.0/progress_table/v0/progress_table.py` & `progress-table-1.3.1/progress_table/v0/progress_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 ALL_COLORS = [getattr(Fore, x) for x in ALL_COLOR_NAMES]
 ALL_STYLES = [getattr(Style, x) for x in ALL_STYLE_NAMES]
 ALL_COLORS_STYLES = ALL_COLORS + ALL_STYLES
 
 ITERATOR_LENGTH_UNKNOWN_WARNED_ONCE = False
 ITERATOR_LENGTH_CACHE: Dict[int, int] = {}
 
+DEPRECATION_PRINTED = False
+
 
 class ProgressTableV0:
     def __init__(
         self,
         columns: Tuple | List = (),
         refresh_rate: int = 10,
         num_decimal_places: int = 4,
@@ -78,14 +80,20 @@
                                    from being displayed. If False, the progress bar covers the current
                                    row, preventing the user from seeing values that are being updated
                                    until the progress bar finishes.
             table_style: Change the borders of the table. Cause KeyError to see all the available styles.
             file: Redirect the output to another stream. There can be multiple streams at once passed as
                   a list or a tuple. Defaults to sys.stdout.
         """
+        global DEPRECATION_PRINTED
+
+        if not DEPRECATION_PRINTED:
+            logging.warning("ProgressTableV0 is deprecated, use ProgressTableV1 instead")
+            DEPRECATION_PRINTED = True
+
         self.refresh_rate = refresh_rate
         self.default_width = default_column_width
         self.default_alignment = default_column_alignment
         self.default_show_throughput = default_show_throughput
         self.default_show_progress = default_show_progress
         self.print_row_on_update = print_row_on_update
         self.reprint_header_every_n_rows = reprint_header_every_n_rows
```

### Comparing `progress-table-1.3.0/progress_table/v0/symbols.py` & `progress-table-1.3.1/progress_table/v0/symbols.py`

 * *Files identical despite different names*

### Comparing `progress-table-1.3.0/progress_table/v1/progress_table.py` & `progress-table-1.3.1/progress_table/v1/progress_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,15 +215,15 @@
         self.column_names: list[str] = []  # Names serve as keys for column configs
 
         # We are storing row configs
         self.row_colors: dict[str, str] = {}
         self.finished_rows: list[dict[str, Any]] = []
 
         self._new_row: dict[str, Any] = {}
-        self.new_row_cumulated_weight: dict[str, int] = {}
+        self._new_row_cumulated_weight: dict[str, int] = {}
         self.files = (file,) if not isinstance(file, (list, tuple)) else file
 
         self.previous_header_counter = 0
         assert reprint_header_every_n_rows > 0, "Reprint header every n rows has to be positive!"
         self.reprint_header_every_n_rows = reprint_header_every_n_rows
 
         # Various flags for table flow
@@ -284,35 +284,43 @@
         # Columns might be added later - in this case we need to reprint header
         self._request_header = True
         self._is_table_opened = False
 
         # Initialize color for the column in the new row
         self._prepare_row_color_dict()
 
-    def add_columns(self, iterable, **kwds):
+    def add_columns(self, *columns, **kwds):
         """Add multiple columns to the table."""
-        for column in iterable:
+        for column in columns:
             self.add_column(column, **kwds)
 
-    def update(self, key, value, *, weight=1):
-        """Update value in the current row."""
+    def update(self, key, value, *, weight=1, **column_kwds):
+        """Update value in the current row. This is extends capabilities of __setitem__.
+
+        Args:
+            key: Name of the column.
+            value: Value to be set.
+            weight: Weight of the value. This is used for aggregation.
+            column_kwds: Additional arguments for the column. They will be only used for column creation.
+                         If column already exists, they will have no effect.
+        """
         if key not in self.column_names:
             if self._is_table_opened:
                 logging.info("Closing table (new column added to opened table)")
-                self.close(close_pbars=False)
+                self.close(close_pbars=False, close_row=False)
 
-            self.add_column(key)
+            self.add_column(key, **column_kwds)
 
         # Set default values for new rows
         self._new_row.setdefault(key, 0)
-        self.new_row_cumulated_weight.setdefault(key, 0)
+        self._new_row_cumulated_weight.setdefault(key, 0)
 
         fn = self.column_aggregates[key]
-        self._new_row[key] = fn(value, self._new_row[key], self.new_row_cumulated_weight[key])
-        self.new_row_cumulated_weight[key] += weight
+        self._new_row[key] = fn(value, self._new_row[key], self._new_row_cumulated_weight[key])
+        self._new_row_cumulated_weight[key] += weight
 
         t0 = time.time()
         td = t0 - self._last_time_row_printed
         if self._is_table_opened:
             if self.print_row_on_update and td > 1 / self.refresh_rate:
                 self._last_time_row_printed = t0
                 self._display_new_row_or_pbar()
@@ -331,15 +339,15 @@
         return self._new_row[key]
 
     def reorder_columns(self, *column_names):
         if all(x == y for x, y in zip(column_names, self.column_names)):
             return
 
         logging.info("Closing table (reordering columns)")
-        self.close(close_pbars=False)
+        self.close(close_pbars=False, close_row=False)
 
         assert isinstance(column_names, (List, Tuple))
         assert all([x in self.column_names for x in column_names]), f"Columns {column_names} not in {self.column_names}"
         self.column_names = list(column_names)
         self.column_widths = {k: self.column_widths[k] for k in column_names}
         self.column_colors = {k: self.column_colors[k] for k in column_names}
         self.column_alignments = {k: self.column_alignments[k] for k in column_names}
@@ -440,15 +448,16 @@
 
     def _display_new_row(self):
         row_str = self._get_row_str(coloring=True)
         self._print(row_str, end="\r")
 
     def _display_new_row_or_pbar(self):
         if self._active_pbars.get(0, None) is not None:
-            self._active_pbars[0].display()  # Level 0 pbar is embedded into the row, if it exists we want to display it instead of a row
+            # Level 0 pbar is embedded into the row, if it exists we want to display it instead of a row
+            self._active_pbars[0].display()
         else:
             self._display_new_row()
 
     @typing.no_type_check
     def _prepare_row_color_dict(self, color: ColorFormat | Dict[str, ColorFormat] = None):
         color = color or self.row_color or {}
         if isinstance(color, ColorFormatTuple):
@@ -462,14 +471,17 @@
         """End the current row."""
         if header or self._request_header or self.previous_header_counter >= self.reprint_header_every_n_rows:
             self.print_header()
             split = False
         if split or self._request_splitter:
             self._print_splitter()
 
+        # Reset aggregated values!
+        self._new_row_cumulated_weight = {}
+
         self._prepare_row_color_dict(color)
         self._display_new_row()
         self._print()  # Insert a newline
         self._prepare_row_color_dict()
         self.previous_header_counter += 1
 
         # Reset the new row
@@ -544,25 +556,27 @@
     def pbar(
         self,
         iterable: Iterable | int | None = None,
         *range_args,
         level=None,
         total=None,
         refresh_rate=None,
+        description="",
         show_throughput=None,
         show_progress=None,
     ):
         """Create iterable progress bar object.
 
         Args:
             iterable: Iterable to iterate over. If None, it will be created from as range(iterable, *range_args).
             range_args: Optional arguments for range function.
             level: Level of the progress bar. If not provided, it will be set automatically.
             total: Total number of iterations. If not provided, it will be calculated from the length of the iterable.
             refresh_rate: The maximal number of times per second the progress bar will be refreshed.
+            description: Custom description of the progress bar that will be shown as prefix.
             show_throughput: If True, the throughput will be displayed.
             show_progress: If True, the progress will be displayed.
         """
         if isinstance(iterable, int):
             iterable = range(iterable, *range_args)
 
         level = level if level is not None else (len(self._active_pbars) + 1 - self.embedded_progress_bar)
@@ -570,14 +584,15 @@
 
         pbar = TableProgressBar(
             iterable=iterable,
             table=self,
             total=total,
             level=level,
             refresh_rate=refresh_rate if refresh_rate is not None else self.refresh_rate,
+            description=description,
             show_throughput=show_throughput if show_throughput is not None else self.pbar_show_throughput,
             show_progress=show_progress if show_progress is not None else self.pbar_show_progress,
         )
         self._active_pbars[level] = pbar
 
         if len(self._active_pbars) > MAX_ACITVE_PBARS:
             raise ValueError("Too many active pbars, remember to .close() old pbars!")
@@ -585,25 +600,26 @@
 
     def __call__(self, *args, **kwds):
         """Creates iterable progress bar object using .pbar method and returns it."""
         return self.pbar(*args, **kwds)
 
 
 class TableProgressBar:
-    def __init__(self, iterable, *, table, total, level, refresh_rate, show_throughput, show_progress):
+    def __init__(self, iterable, *, table, total, level, refresh_rate, description, show_throughput, show_progress):
         self.iterable: Iterable | None = iterable
 
         self._step: int = 0
         self._total: int = total
         self._creation_time: float = time.perf_counter()
         self._last_refresh_time: float = -float("inf")
 
         self.level: int = level
         self.table: ProgressTableV1 = table
         self.refresh_rate: int = refresh_rate
+        self.description: str = description
         self.show_progress: bool = show_progress
         self.show_throughput: bool = show_throughput
         self._is_active: bool = True
 
     def display(self):
         assert self._is_active, "Progress bar was closed!"
 
@@ -614,21 +630,23 @@
         step = min(self._step, total) if total else self._step
 
         self._last_refresh_time = time.perf_counter()
         time_passed = self._last_refresh_time - self._creation_time
         throughput = self._step / time_passed if time_passed > 0 else 0.0
 
         inside_infobar = []
-        if self.show_throughput:
-            inside_infobar.append(f"{throughput: <.2f} it/s")
+        if self.description:
+            inside_infobar.append(self.description)
         if self.show_progress:
             if self._total:
                 inside_infobar.append(f"{self._step}/{self._total}")
             else:
                 inside_infobar.append(f"{self._step}")
+        if self.show_throughput:
+            inside_infobar.append(f"{throughput: <.2f} it/s")
         infobar = "[" + ", ".join(inside_infobar) + "] " if inside_infobar else ""
 
         pbar = ["\n" * self.level]
         if not is_embedded:
             tot_width = sum(self.table.column_widths.values()) + 3 * (len(self.table.column_widths) - 1) + 2
             if tot_width >= terminal_width - 1:
                 tot_width = terminal_width - 2
```

### Comparing `progress-table-1.3.0/progress_table/v1/styles.py` & `progress-table-1.3.1/progress_table/v1/styles.py`

 * *Files identical despite different names*

### Comparing `progress-table-1.3.0/progress_table.egg-info/PKG-INFO` & `progress-table-1.3.1/progress_table.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: progress-table
-Version: 1.3.0
+Version: 1.3.1
 Summary: Display progress as a pretty table in the command line.
 Home-page: https://github.com/gahaalt/progress-table.git
 Author: Szymon Mikler
 Author-email: sjmikler@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `progress-table-1.3.0/progress_table.egg-info/PKG-INFO.sync-conflict-20240314-015933-NXTV2IO` & `progress-table-1.3.1/progress_table.egg-info/PKG-INFO.sync-conflict-20240314-015933-NXTV2IO`

 * *Files identical despite different names*

### Comparing `progress-table-1.3.0/progress_table.egg-info/SOURCES.txt` & `progress-table-1.3.1/progress_table.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `progress-table-1.3.0/setup.py` & `progress-table-1.3.1/setup.py`

 * *Files identical despite different names*

