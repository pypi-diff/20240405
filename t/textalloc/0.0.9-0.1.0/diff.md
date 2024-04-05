# Comparing `tmp/textalloc-0.0.9.tar.gz` & `tmp/textalloc-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textalloc-0.0.9.tar", last modified: Sun Jan 21 17:17:03 2024, max compression
+gzip compressed data, was "textalloc-0.1.0.tar", last modified: Fri Apr  5 17:42:09 2024, max compression
```

## Comparing `textalloc-0.0.9.tar` & `textalloc-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        0 2024-01-21 17:17:03.484213 textalloc-0.0.9/
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     1077 2023-02-14 19:18:58.000000 textalloc-0.0.9/LICENSE
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     7585 2024-01-21 17:17:03.472212 textalloc-0.0.9/PKG-INFO
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     6946 2024-01-21 17:10:51.000000 textalloc-0.0.9/README.md
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)      719 2024-01-21 17:14:08.000000 textalloc-0.0.9/pyproject.toml
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)       38 2024-01-21 17:17:03.486212 textalloc-0.0.9/setup.cfg
-drwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        0 2024-01-21 17:17:03.066242 textalloc-0.0.9/src/
-drwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        0 2024-01-21 17:17:03.252389 textalloc-0.0.9/src/textalloc/
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)    11907 2024-01-21 17:04:59.000000 textalloc-0.0.9/src/textalloc/__init__.py
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     6539 2024-01-21 17:01:52.000000 textalloc-0.0.9/src/textalloc/candidates.py
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     6697 2024-01-21 17:11:54.000000 textalloc-0.0.9/src/textalloc/non_overlapping_boxes.py
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     9916 2024-01-21 16:26:34.000000 textalloc-0.0.9/src/textalloc/overlap_functions.py
-drwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        0 2024-01-21 17:17:03.457290 textalloc-0.0.9/src/textalloc.egg-info/
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     7585 2024-01-21 17:17:02.000000 textalloc-0.0.9/src/textalloc.egg-info/PKG-INFO
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)      344 2024-01-21 17:17:03.000000 textalloc-0.0.9/src/textalloc.egg-info/SOURCES.txt
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        1 2024-01-21 17:17:02.000000 textalloc-0.0.9/src/textalloc.egg-info/dependency_links.txt
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)       22 2024-01-21 17:17:02.000000 textalloc-0.0.9/src/textalloc.egg-info/requires.txt
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)       10 2024-01-21 17:17:02.000000 textalloc-0.0.9/src/textalloc.egg-info/top_level.txt
+drwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        0 2024-04-05 17:42:08.994909 textalloc-0.1.0/
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     1077 2023-02-14 19:18:58.000000 textalloc-0.1.0/LICENSE
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     7971 2024-04-05 17:42:08.986910 textalloc-0.1.0/PKG-INFO
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     7308 2024-04-05 16:57:31.000000 textalloc-0.1.0/README.md
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)      741 2024-04-05 17:42:00.000000 textalloc-0.1.0/pyproject.toml
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)       38 2024-04-05 17:42:08.995909 textalloc-0.1.0/setup.cfg
+drwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        0 2024-04-05 17:42:08.706912 textalloc-0.1.0/src/
+drwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        0 2024-04-05 17:42:08.830909 textalloc-0.1.0/src/textalloc/
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)    15463 2024-04-05 17:35:06.000000 textalloc-0.1.0/src/textalloc/__init__.py
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     6539 2024-02-20 19:23:50.000000 textalloc-0.1.0/src/textalloc/candidates.py
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     9795 2024-04-05 17:35:17.000000 textalloc-0.1.0/src/textalloc/non_overlapping_boxes.py
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)    10042 2024-02-20 19:25:04.000000 textalloc-0.1.0/src/textalloc/overlap_functions.py
+drwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        0 2024-04-05 17:42:08.975912 textalloc-0.1.0/src/textalloc.egg-info/
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     7971 2024-04-05 17:42:08.000000 textalloc-0.1.0/src/textalloc.egg-info/PKG-INFO
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)      344 2024-04-05 17:42:08.000000 textalloc-0.1.0/src/textalloc.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        1 2024-04-05 17:42:08.000000 textalloc-0.1.0/src/textalloc.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)       49 2024-04-05 17:42:08.000000 textalloc-0.1.0/src/textalloc.egg-info/requires.txt
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)       10 2024-04-05 17:42:08.000000 textalloc-0.1.0/src/textalloc.egg-info/top_level.txt
```

### Comparing `textalloc-0.0.9/LICENSE` & `textalloc-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `textalloc-0.0.9/PKG-INFO` & `textalloc-0.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: textalloc
-Version: 0.0.9
+Version: 0.1.0
 Summary: Efficient Text Allocation in matplotlib using NumPy Broadcasting
 Author-email: Christoffer Kjellson <c.kjellson@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/ckjellson/textalloc
 Project-URL: Bug Tracker, https://github.com/ckjellson/textalloc/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: tqdm
+Requires-Dist: tqdm; python_version > "3.6"
 Requires-Dist: numpy
 Requires-Dist: matplotlib
 
 # textalloc - Efficient matplotlib Text Allocation
 
 plt.text|textalloc (2.1s)
 :-------------------------:|:-------------------------:
@@ -103,29 +103,35 @@
     Parameter for max distance from textbox to
     its plotted position.
     Given in proportion of x-ax dimensions (0-1)
 verbose: (bool), default False
     prints progress using tqdm.
 draw_lines: (bool), default True
     draws lines from original points to textboxes.
-linecolor: (str), default "r"
+linecolor: (Union[str, List[str]]), default "r"
     Color code of the lines between points and text-boxes.
 draw_all: (bool), default True
     Draws all texts after allocating as many as possible despite overlap.
 nbr_candidates: (int), default 200
     Sets the number of candidates used.
 linewidth: (float), default 1
     Width of line between textbox and it's origin.
 textcolor: (Union[str, List[str]]), default "k"
     Color code of the text.
 seed: (int), default 0
     Seeds order of text allocations.
 direction: (str), default None
     Sets the preferred direction of the boxes with options:
     (south, north, east, west, northeast, northwest, southeast, southwest).
+x_logscale_base: (int), default None
+    Base of x-axis log-scale, required if the scaling of the x-axis is "log"
+y_logscale_base: (int), default None
+    Base of y-axis log-scale, required if the scaling of the y-axis is "log"
+avoid_label_lines_overlap: (bool), default False
+    If set to True, avoids overlap for drawn lines to text labels.
 **kwargs: (), kwargs for the plt.text() call.
 ```
 # Implementation and speed
 
 The implementation aims to plot as many text-boxes as possible in the free space in the plot. There are three main steps of the algorithm:
 
 For each textbox to be plotted:
```

### Comparing `textalloc-0.0.9/README.md` & `textalloc-0.1.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -85,29 +85,35 @@
     Parameter for max distance from textbox to
     its plotted position.
     Given in proportion of x-ax dimensions (0-1)
 verbose: (bool), default False
     prints progress using tqdm.
 draw_lines: (bool), default True
     draws lines from original points to textboxes.
-linecolor: (str), default "r"
+linecolor: (Union[str, List[str]]), default "r"
     Color code of the lines between points and text-boxes.
 draw_all: (bool), default True
     Draws all texts after allocating as many as possible despite overlap.
 nbr_candidates: (int), default 200
     Sets the number of candidates used.
 linewidth: (float), default 1
     Width of line between textbox and it's origin.
 textcolor: (Union[str, List[str]]), default "k"
     Color code of the text.
 seed: (int), default 0
     Seeds order of text allocations.
 direction: (str), default None
     Sets the preferred direction of the boxes with options:
     (south, north, east, west, northeast, northwest, southeast, southwest).
+x_logscale_base: (int), default None
+    Base of x-axis log-scale, required if the scaling of the x-axis is "log"
+y_logscale_base: (int), default None
+    Base of y-axis log-scale, required if the scaling of the y-axis is "log"
+avoid_label_lines_overlap: (bool), default False
+    If set to True, avoids overlap for drawn lines to text labels.
 **kwargs: (), kwargs for the plt.text() call.
 ```
 # Implementation and speed
 
 The implementation aims to plot as many text-boxes as possible in the free space in the plot. There are three main steps of the algorithm:
 
 For each textbox to be plotted:
```

### Comparing `textalloc-0.0.9/src/textalloc/candidates.py` & `textalloc-0.1.0/src/textalloc/candidates.py`

 * *Files identical despite different names*

### Comparing `textalloc-0.0.9/src/textalloc/non_overlapping_boxes.py` & `textalloc-0.1.0/src/textalloc/non_overlapping_boxes.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,15 +3,21 @@
 from textalloc.candidates import generate_candidates
 from textalloc.overlap_functions import (
     non_overlapping_with_points,
     non_overlapping_with_lines,
     non_overlapping_with_boxes,
     inside_plot,
 )
-from tqdm import tqdm
+
+try:
+    from tqdm import tqdm
+except ImportError:
+
+    def tqdm(iterator, *args, **kwargs):
+        return iterator
 
 
 def get_non_overlapping_boxes(
     original_boxes: list,
     xlims: Tuple[float, float],
     ylims: Tuple[float, float],
     aspect_ratio: float,
@@ -23,14 +29,16 @@
     draw_all: bool,
     scatter_xy: np.ndarray,
     lines_xyxy: np.ndarray,
     scatter_sizes: np.ndarray,
     scatter_plot_bbs: np.ndarray,
     text_scatter_sizes: np.ndarray,
     direction: str,
+    draw_lines: bool,
+    avoid_label_lines_overlap: bool,
 ) -> Tuple[List[Tuple[float, float, float, float, str, int]], List[int]]:
     """Finds boxes that do not have an overlap with any other objects.
 
     Args:
         original_boxes (np.ndarray): original boxes containing texts.
         xlims (Tuple[float, float]): x-limits of plot gotten from ax.get_ylim()
         ylims (Tuple[float, float]): y-limits of plot gotten from ax.get_ylim()
@@ -43,14 +51,16 @@
         draw_all (bool): Draws all texts after allocating as many as possible despit overlap.
         scatter_xy (np.ndarray): 2d array of scattered points in plot.
         lines_xyxy (np.ndarray): 2d array of line segments in plot.
         scatter_sizes (array-like): array of object sizes with centers in scatter_xy.
         scatter_plot_bbs (np.ndarray): boxes extracted from scatter plot.
         text_scatter_sizes (array-like): array of object sizes with centers in text objects.
         direction (str): set preferred direction of the boxes.
+        draw_lines (bool): draws lines from original points to textboxes.
+        avoid_label_lines_overlap (bool): If True, avoids overlap with lines drawn between text labels and locations.
 
     Returns:
         Tuple[List[Tuple[float, float, float, float, str, int]], List[int]]: data of non-overlapping boxes and indices of overlapping boxes.
     """
     xmin_bound, xmax_bound = xlims
     ymin_bound, ymax_bound = ylims
     xdiff = xmax_bound - xmin_bound
@@ -88,14 +98,34 @@
             ymindistance,
             xmaxdistance,
             ymaxdistance,
             nbr_candidates,
             text_scatter_size,
             direction,
         )
+        # If overlap with drawn lines should be avoided, create cand_lines.
+        cand_lines = None
+        if avoid_label_lines_overlap:
+            for i_ in range(candidates.shape[0]):
+                x_near, y_near = find_nearest_point_on_box(
+                    candidates[i_, 0],
+                    candidates[i_, 1],
+                    w,
+                    h,
+                    x_original,
+                    y_original,
+                )
+                if x_near is None:
+                    x_near = x_original
+                    y_near = y_original
+                new_line = np.array([[x_near, y_near, x_original, y_original]])
+                if cand_lines is None:
+                    cand_lines = new_line
+                else:
+                    cand_lines = np.vstack([cand_lines, new_line])
 
         # Check for overlapping
         if scatter_xy is None and scatter_plot_bbs is None:
             non_op = np.zeros((candidates.shape[0],)) == 0
         elif scatter_plot_bbs is None:
             non_op = non_overlapping_with_points(
                 scatter_xy,
@@ -115,21 +145,32 @@
                 lines_xyxy, candidates, xmargin, ymargin
             )
         if box_arr.shape[0] == 0:
             non_orec = np.zeros((candidates.shape[0],)) == 0
         else:
             non_orec = non_overlapping_with_boxes(box_arr, candidates, xmargin, ymargin)
         inside = inside_plot(xmin_bound, ymin_bound, xmax_bound, ymax_bound, candidates)
+        if cand_lines is None or box_arr.shape[0] == 0:
+            non_oll = np.zeros((candidates.shape[0],)) == 0
+        else:
+            non_oll = non_overlapping_with_lines(
+                cand_lines, box_arr, xmargin, ymargin, axis=0
+            )
 
         # Validate
         ok_candidates = np.where(
             np.bitwise_and(
-                non_ol, np.bitwise_and(non_op, np.bitwise_and(non_orec, inside))
+                non_ol,
+                np.bitwise_and(
+                    non_op,
+                    np.bitwise_and(non_orec, np.bitwise_and(inside, non_oll)),
+                ),
             )
         )[0]
+        best_candidate = None
         if len(ok_candidates) > 0:
             best_candidate = candidates[ok_candidates[0], :]
             box_arr = np.vstack(
                 [
                     box_arr,
                     np.array(
                         [
@@ -165,8 +206,59 @@
                     non_overlapping_boxes.append(
                         (best_candidate[0], best_candidate[1], w, h, s, i)
                     )
                 else:
                     overlapping_boxes_inds.append(i)
             else:
                 overlapping_boxes_inds.append(i)
+        if draw_lines and avoid_label_lines_overlap and best_candidate is not None:
+            x_near, y_near = find_nearest_point_on_box(
+                best_candidate[0], best_candidate[1], w, h, x_original, y_original
+            )
+            if x_near is not None:
+                new_line = np.array([[x_near, y_near, x_original, y_original]])
+                if lines_xyxy is None:
+                    lines_xyxy = new_line
+                else:
+                    lines_xyxy = np.vstack([lines_xyxy, new_line])
     return non_overlapping_boxes, overlapping_boxes_inds
+
+
+def find_nearest_point_on_box(
+    xmin: float, ymin: float, w: float, h: float, x: float, y: float
+) -> Tuple[float, float]:
+    """Finds nearest point on box from point.
+    Returns None,None if point inside box
+
+    Args:
+        xmin (float): xmin of box
+        ymin (float): ymin of box
+        w (float): width of box
+        h (float): height of box
+        x (float): x-coordinate of point
+        y (float): y-coordinate of point
+
+    Returns:
+        Tuple[float, float]: x,y coordinate of nearest point
+    """
+    xmax = xmin + w
+    ymax = ymin + h
+    if x < xmin:
+        if y < ymin:
+            return xmin, ymin
+        elif y > ymax:
+            return xmin, ymax
+        else:
+            return xmin, y
+    elif x > xmax:
+        if y < ymin:
+            return xmax, ymin
+        elif y > ymax:
+            return xmax, ymax
+        else:
+            return xmax, y
+    else:
+        if y < ymin:
+            return x, ymin
+        elif y > ymax:
+            return x, ymax
+    return None, None
```

### Comparing `textalloc-0.0.9/src/textalloc/overlap_functions.py` & `textalloc-0.1.0/src/textalloc/overlap_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,23 +54,28 @@
                 ),
                 axis=1,
             )
         )
 
 
 def non_overlapping_with_lines(
-    lines_xyxy: np.ndarray, candidates: np.ndarray, xmargin: float, ymargin: float
+    lines_xyxy: np.ndarray,
+    candidates: np.ndarray,
+    xmargin: float,
+    ymargin: float,
+    axis: int = 1,
 ) -> np.ndarray:
     """Finds candidates not overlapping with lines
 
     Args:
         lines_xyxy (np.ndarray): line segments
         candidates (np.ndarray): candidate boxes
         xmargin (float): fraction of the x-dimension to use as margins for text boxes
         ymargin (float): fraction of the y-dimension to use as margins for text boxes
+        axis (int): If axis set to 0, performs the opposite comparison (lines to boxes)
 
     Returns:
         np.ndarray: Boolean array of shape (K,) with True for non-overlapping candidates with lines.
     """
     non_intersecting = np.invert(
         np.any(
             np.bitwise_or(
@@ -119,15 +124,15 @@
                                 ]
                             ),
                             lines_xyxy,
                         ),
                     ),
                 ),
             ),
-            axis=1,
+            axis=axis,
         )
     )
 
     non_inside = np.invert(
         np.any(
             np.bitwise_and(
                 candidates[:, 0][:, None] - xmargin < lines_xyxy[:, 0],
@@ -150,15 +155,15 @@
                                     ),
                                 ),
                             ),
                         ),
                     ),
                 ),
             ),
-            axis=1,
+            axis=axis,
         )
     )
     return np.bitwise_and(non_intersecting, non_inside)
 
 
 def line_intersect(cand_xyxy: np.ndarray, lines_xyxy: np.ndarray) -> np.ndarray:
     """Checks if line segments intersect for all line segments and candidates.
```

### Comparing `textalloc-0.0.9/src/textalloc.egg-info/PKG-INFO` & `textalloc-0.1.0/src/textalloc.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: textalloc
-Version: 0.0.9
+Version: 0.1.0
 Summary: Efficient Text Allocation in matplotlib using NumPy Broadcasting
 Author-email: Christoffer Kjellson <c.kjellson@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/ckjellson/textalloc
 Project-URL: Bug Tracker, https://github.com/ckjellson/textalloc/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: tqdm
+Requires-Dist: tqdm; python_version > "3.6"
 Requires-Dist: numpy
 Requires-Dist: matplotlib
 
 # textalloc - Efficient matplotlib Text Allocation
 
 plt.text|textalloc (2.1s)
 :-------------------------:|:-------------------------:
@@ -103,29 +103,35 @@
     Parameter for max distance from textbox to
     its plotted position.
     Given in proportion of x-ax dimensions (0-1)
 verbose: (bool), default False
     prints progress using tqdm.
 draw_lines: (bool), default True
     draws lines from original points to textboxes.
-linecolor: (str), default "r"
+linecolor: (Union[str, List[str]]), default "r"
     Color code of the lines between points and text-boxes.
 draw_all: (bool), default True
     Draws all texts after allocating as many as possible despite overlap.
 nbr_candidates: (int), default 200
     Sets the number of candidates used.
 linewidth: (float), default 1
     Width of line between textbox and it's origin.
 textcolor: (Union[str, List[str]]), default "k"
     Color code of the text.
 seed: (int), default 0
     Seeds order of text allocations.
 direction: (str), default None
     Sets the preferred direction of the boxes with options:
     (south, north, east, west, northeast, northwest, southeast, southwest).
+x_logscale_base: (int), default None
+    Base of x-axis log-scale, required if the scaling of the x-axis is "log"
+y_logscale_base: (int), default None
+    Base of y-axis log-scale, required if the scaling of the y-axis is "log"
+avoid_label_lines_overlap: (bool), default False
+    If set to True, avoids overlap for drawn lines to text labels.
 **kwargs: (), kwargs for the plt.text() call.
 ```
 # Implementation and speed
 
 The implementation aims to plot as many text-boxes as possible in the free space in the plot. There are three main steps of the algorithm:
 
 For each textbox to be plotted:
```

