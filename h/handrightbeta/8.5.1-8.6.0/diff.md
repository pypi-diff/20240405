# Comparing `tmp/handrightbeta-8.5.1.tar.gz` & `tmp/handrightbeta-8.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "handrightbeta-8.5.1.tar", last modified: Tue Oct  3 05:53:30 2023, max compression
+gzip compressed data, was "handrightbeta-8.6.0.tar", last modified: Fri Apr  5 14:59:18 2024, max compression
```

## Comparing `handrightbeta-8.5.1.tar` & `handrightbeta-8.6.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-10-03 05:53:30.299219 handrightbeta-8.5.1/
--rw-rw-rw-   0        0        0     1555 2023-08-31 14:02:32.000000 handrightbeta-8.5.1/LICENSE.txt
--rw-rw-rw-   0        0        0      137 2023-08-31 14:02:32.000000 handrightbeta-8.5.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2518 2023-10-03 05:53:30.299219 handrightbeta-8.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     1827 2023-08-31 14:02:32.000000 handrightbeta-8.5.1/README.md
-drwxrwxrwx   0        0        0        0 2023-10-03 05:53:30.279109 handrightbeta-8.5.1/handright/
--rw-rw-rw-   0        0        0     1096 2023-10-03 05:53:13.000000 handrightbeta-8.5.1/handright/__init__.py
--rw-rw-rw-   0        0        0    14573 2023-10-03 02:47:55.000000 handrightbeta-8.5.1/handright/_core.py
--rw-rw-rw-   0        0        0      146 2023-08-31 14:02:32.000000 handrightbeta-8.5.1/handright/_exceptions.py
--rw-rw-rw-   0        0        0    16145 2023-10-03 02:47:40.000000 handrightbeta-8.5.1/handright/_template.py
--rw-rw-rw-   0        0        0     3207 2023-08-31 14:02:32.000000 handrightbeta-8.5.1/handright/_util.py
-drwxrwxrwx   0        0        0        0 2023-10-03 05:53:30.281108 handrightbeta-8.5.1/handright/tests/
--rw-rw-rw-   0        0        0       17 2023-08-31 14:02:32.000000 handrightbeta-8.5.1/handright/tests/__init__.py
--rw-rw-rw-   0        0        0     2489 2023-08-31 14:02:32.000000 handrightbeta-8.5.1/handright/tests/test_util.py
-drwxrwxrwx   0        0        0        0 2023-10-03 05:53:30.298213 handrightbeta-8.5.1/handrightbeta.egg-info/
--rw-rw-rw-   0        0        0     2518 2023-10-03 05:53:29.000000 handrightbeta-8.5.1/handrightbeta.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      433 2023-10-03 05:53:30.000000 handrightbeta-8.5.1/handrightbeta.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-03 05:53:29.000000 handrightbeta-8.5.1/handrightbeta.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-10-03 05:53:29.000000 handrightbeta-8.5.1/handrightbeta.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-10-03 05:53:29.000000 handrightbeta-8.5.1/handrightbeta.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-09-05 14:20:55.000000 handrightbeta-8.5.1/handrightbeta.egg-info/zip-safe
--rw-rw-rw-   0        0        0       85 2023-10-03 05:53:30.300218 handrightbeta-8.5.1/setup.cfg
--rw-rw-rw-   0        0        0     1456 2023-10-03 02:47:40.000000 handrightbeta-8.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 14:59:18.253047 handrightbeta-8.6.0/
+-rw-rw-rw-   0        0        0     1555 2023-08-31 14:02:32.000000 handrightbeta-8.6.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      137 2023-08-31 14:02:32.000000 handrightbeta-8.6.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2518 2024-04-05 14:59:18.254048 handrightbeta-8.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1827 2023-08-31 14:02:32.000000 handrightbeta-8.6.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-05 14:59:18.221988 handrightbeta-8.6.0/handright/
+-rw-rw-rw-   0        0        0     1097 2024-04-05 14:57:05.000000 handrightbeta-8.6.0/handright/__init__.py
+-rw-rw-rw-   0        0        0    14878 2024-02-24 15:02:36.000000 handrightbeta-8.6.0/handright/_core.py
+-rw-rw-rw-   0        0        0      146 2023-08-31 14:02:32.000000 handrightbeta-8.6.0/handright/_exceptions.py
+-rw-rw-rw-   0        0        0    16145 2024-02-24 15:02:25.000000 handrightbeta-8.6.0/handright/_template.py
+-rw-rw-rw-   0        0        0     3207 2023-08-31 14:02:32.000000 handrightbeta-8.6.0/handright/_util.py
+drwxrwxrwx   0        0        0        0 2024-04-05 14:59:18.223987 handrightbeta-8.6.0/handright/tests/
+-rw-rw-rw-   0        0        0       17 2023-08-31 14:02:32.000000 handrightbeta-8.6.0/handright/tests/__init__.py
+-rw-rw-rw-   0        0        0     2489 2023-08-31 14:02:32.000000 handrightbeta-8.6.0/handright/tests/test_util.py
+drwxrwxrwx   0        0        0        0 2024-04-05 14:59:18.252048 handrightbeta-8.6.0/handrightbeta.egg-info/
+-rw-rw-rw-   0        0        0     2518 2024-04-05 14:59:17.000000 handrightbeta-8.6.0/handrightbeta.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      433 2024-04-05 14:59:18.000000 handrightbeta-8.6.0/handrightbeta.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 14:59:17.000000 handrightbeta-8.6.0/handrightbeta.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-04-05 14:59:17.000000 handrightbeta-8.6.0/handrightbeta.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-05 14:59:17.000000 handrightbeta-8.6.0/handrightbeta.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-09-05 14:20:55.000000 handrightbeta-8.6.0/handrightbeta.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       85 2024-04-05 14:59:18.259559 handrightbeta-8.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     1456 2024-02-24 15:02:25.000000 handrightbeta-8.6.0/setup.py
```

### Comparing `handrightbeta-8.5.1/LICENSE.txt` & `handrightbeta-8.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `handrightbeta-8.5.1/PKG-INFO` & `handrightbeta-8.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: handrightbeta
-Version: 8.5.1
+Version: 8.6.0
 Summary: A lightweight Python library for simulating Chinese handwriting
 Home-page: https://github.com/14790897/Handright
 Author: Chenghui Li (Gsllchb)
 Author-email: 14790897abc@gmail.com
 License: bsd-3-clause
 Keywords: simulating Chinese handwriting
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `handrightbeta-8.5.1/README.md` & `handrightbeta-8.6.0/README.md`

 * *Files identical despite different names*

### Comparing `handrightbeta-8.5.1/handright/__init__.py` & `handrightbeta-8.6.0/handright/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,17 +22,17 @@
 `Iterable` of Pillow `Image`, so the images can be shown, saved, or further
 processed.
 """
 from handright._core import handwrite
 from handright._exceptions import Error, LayoutError, BackgroundTooLargeError
 from handright._template import Template, Feature
 
-__version__ = "8.5.1"
+__version__ = "8.6.0"
 
 __all__ = (
     "handwrite",
     "Template",
     "Feature",
     "Error",
     "LayoutError",
-    "BackgroundTooLargeError"
+    "BackgroundTooLargeError",
 )
```

### Comparing `handrightbeta-8.5.1/handright/_core.py` & `handrightbeta-8.6.0/handright/_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,31 +59,28 @@
     if export_pdf:
         # 如果 export_pdf 为 True，则保存为 PDF
         images_list = list(images)  # 转换为列表以保存为 PDF
         pdf_bytes = io.BytesIO()
         first_image = images_list[0]
         remaining_images = images_list[1:]
         first_image.save(
-            pdf_bytes,
-            format="PDF",
-            save_all=True,
-            append_images=remaining_images
+            pdf_bytes, format="PDF", save_all=True, append_images=remaining_images
         )
-        
+
         if save_to_file:
             # 如果 save_to_file 为 True，则保存到文件
             pdf_bytes.seek(0)  # 将指针移动到流的开头
             with open(file_path, "wb") as f:
                 f.write(pdf_bytes.read())
             return None  # 保存到文件后，返回 None
         else:
             pdf_bytes.seek(0)
             return pdf_bytes  # 返回 PDF 的字节流
-        
-    return images 
+
+    return images
 
 
 def _draft(text, templates, seed=None) -> Iterator[Page]:
     text = _preprocess_text(text)
     template_iter = itertools.cycle(templates)
     num_iter = itertools.count()
     rand = random.Random(x=seed)
@@ -96,33 +93,33 @@
 
 
 def _preprocess_text(text: str) -> str:
     return text.replace(_CRLF, _LF).replace(_CR, _LF)
 
 
 def _check_template(page, tpl) -> None:
-    if page.height() < (tpl.get_top_margin() + tpl.get_line_spacing()
-                        + tpl.get_bottom_margin()):
+    if page.height() < (
+        tpl.get_top_margin() + tpl.get_line_spacing() + tpl.get_bottom_margin()
+    ):
         msg = "for (height < top_margin + line_spacing + bottom_margin)"
         raise LayoutError(msg)
     if tpl.get_font().size > tpl.get_line_spacing():
         msg = "for (font.size > line_spacing)"
         raise LayoutError(msg)
-    if page.width() < (tpl.get_left_margin() + tpl.get_font().size
-                       + tpl.get_right_margin()):
+    if page.width() < (
+        tpl.get_left_margin() + tpl.get_font().size + tpl.get_right_margin()
+    ):
         msg = "for (width < left_margin + font.size + right_margin)"
         raise LayoutError(msg)
     if tpl.get_word_spacing() <= -tpl.get_font().size // 2:
         msg = "for (word_spacing <= -font.size // 2)"
         raise LayoutError(msg)
 
 
-def _draw_page(
-        page, text, start: int, tpl: Template, rand: random.Random
-) -> int:
+def _draw_page(page, text, start: int, tpl: Template, rand: random.Random) -> int:
     _check_template(page, tpl)
 
     width = page.width()
     height = page.height()
     top_margin = tpl.get_top_margin()
     bottom_margin = tpl.get_bottom_margin()
     left_margin = tpl.get_left_margin()
@@ -133,104 +130,96 @@
     end_chars = tpl.get_end_chars()
 
     draw = page.draw()
     y = top_margin + line_spacing - font_size
     while y <= height - bottom_margin - font_size:
         x = left_margin
         while True:
-            if text[start] == _LF: #跳过换行符自己处理
+            if text[start] == _LF:  # 跳过换行符自己处理
                 start += 1
                 if start == len(text):
                     return start
                 break
-            if (x > width - right_margin - 2 * font_size
-                    and text[start] in start_chars):
+            if x > width - right_margin - 2 * font_size and text[start] in start_chars:
                 break
-            if (x > width - right_margin - font_size
-                    and text[start] not in end_chars):
+            if x > width - right_margin - font_size and text[start] not in end_chars:
                 break
-            
-             # 随机选择一个字符进行替换 9.1
+
+            # 随机选择一个字符进行替换 9.1
             if rand.random() < tpl.get_strikethrough_probability():
                 wrong_char_index = random.randint(0, len(text) - 1)
-                wrong_end_chars = end_chars + ' '
+                wrong_end_chars = end_chars + " "
                 # 检查字符是否在排除列表中
                 while text[wrong_char_index] in wrong_end_chars:
                     wrong_char_index = random.randint(0, len(text) - 1)
                 wrong_char = text[wrong_char_index]
-                
-                origin_x =x
+
+                origin_x = x
                 # 绘制错误的字（被划掉的字）
                 if Feature.GRID_LAYOUT in tpl.get_features():
                     x = _grid_layout(draw, x, y, wrong_char, tpl, rand)
                 else:
                     x = _flow_layout(draw, x, y, wrong_char, tpl, rand)
                 # 添加涂改标记（斜线）
                 _draw_strikethrough(draw, origin_x, y, tpl, rand)
-                
-            # 绘制正确的字            
+
+            # 绘制正确的字
             if Feature.GRID_LAYOUT in tpl.get_features():
                 x = _grid_layout(draw, x, y, text[start], tpl, rand)
             else:
                 x = _flow_layout(draw, x, y, text[start], tpl, rand)
             start += 1
             if start == len(text):
                 return start
         y += line_spacing
     return start
 
+
 def _draw_strikethrough(draw, x, y, tpl, rand):
     line_length = tpl.get_font().size * math.sqrt(2)
     length_sigma = tpl.get_strikethrough_length_sigma()
     angle_sigma = tpl.get_strikethrough_angle_sigma()
     width_sigma = tpl.get_strikethrough_width_sigma()
     line_width = tpl.get_strikethrough_width()
-    
-    start_x = x + 1/7*line_length
-    start_y = y + 1/7*line_length
+
+    start_x = x + 1 / 7 * line_length
+    start_y = y + 1 / 7 * line_length
     # 添加扰动
     actual_length = line_length + gauss(rand, 0, length_sigma)
     initial_angle = 45  # 初始角度设置为45度
     actual_angle = initial_angle + gauss(rand, 0, angle_sigma)
     actual_width = line_width + gauss(rand, 0, width_sigma)  # 假设基础宽度为5
-    
-    end_x = start_x + actual_length * math.cos(math.radians(actual_angle))*5/7
-    end_y = start_y + actual_length * math.sin(math.radians(actual_angle))*5/7
+
+    end_x = start_x + actual_length * math.cos(math.radians(actual_angle)) * 5 / 7
+    end_y = start_y + actual_length * math.sin(math.radians(actual_angle)) * 5 / 7
     draw.line((start_x, start_y, end_x, end_y), fill=_WHITE, width=int(actual_width))
 
-def _flow_layout(
-        draw, x, y, char, tpl: Template, rand: random.Random
-) -> float:
+
+def _flow_layout(draw, x, y, char, tpl: Template, rand: random.Random) -> float:
     xy = (round(x), round(gauss(rand, y, tpl.get_line_spacing_sigma())))
     font = _get_font(tpl, rand)
     offset = _draw_char(draw, char, xy, font)
-    x += gauss(
-        rand,
-        tpl.get_word_spacing() + offset,
-        tpl.get_word_spacing_sigma()
-    )
+    x += gauss(rand, tpl.get_word_spacing() + offset, tpl.get_word_spacing_sigma())
     return x
 
 
-def _grid_layout(
-        draw, x, y, char, tpl: Template, rand: random.Random
-) -> float:
-    xy = (round(gauss(rand, x, tpl.get_word_spacing_sigma())),
-          round(gauss(rand, y, tpl.get_line_spacing_sigma())))
+def _grid_layout(draw, x, y, char, tpl: Template, rand: random.Random) -> float:
+    xy = (
+        round(gauss(rand, x, tpl.get_word_spacing_sigma())),
+        round(gauss(rand, y, tpl.get_line_spacing_sigma())),
+    )
     font = _get_font(tpl, rand)
     _ = _draw_char(draw, char, xy, font)
-    x += tpl.get_word_spacing() + tpl.get_font().size#主要的区别在于这里的X它是固定的
+    x += tpl.get_word_spacing() + tpl.get_font().size  # 主要的区别在于这里的X它是固定的
     return x
 
 
 def _get_font(tpl: Template, rand: random.Random):
     font = tpl.get_font()
-    actual_font_size = max(round(
-        gauss(rand, font.size, tpl.get_font_size_sigma())
-    ), 0)
+    actual_font_size = max(round(gauss(rand, font.size, tpl.get_font_size_sigma())), 0)
     if actual_font_size != font.size:
         return font.font_variant(size=actual_font_size)
     return font
 
 
 def _draw_char(draw, char: str, xy: Tuple[int, int], font) -> int:
     """Draws a single char with the parameters and white color, and returns the
@@ -292,34 +281,33 @@
     assert left >= 0 and upper >= 0
     # reserve 0xFFFFFFFF as _STROKE_END
     if right >= _MAX_INT16_VALUE or lower >= _MAX_INT16_VALUE:
         msg = "the width or height of backgrounds can not exceed {}".format(
             _MAX_INT16_VALUE - 1
         )
         raise BackgroundTooLargeError(msg)
-    strokes = NumericOrderedSet(
-        _UNSIGNED_INT32_TYPECODE,
-        privileged=_STROKE_END
-    )
+    strokes = NumericOrderedSet(_UNSIGNED_INT32_TYPECODE, privileged=_STROKE_END)
     for y in range(upper, lower):
         for x in range(left, right):
             if bitmap[x, y] and strokes.add(_xy(x, y)):
                 _extract_stroke(bitmap, (x, y), strokes, bbox)
                 strokes.add_privileged()
     return strokes
 
 
 def _extract_stroke(
-        bitmap, start: Tuple[int, int], strokes, bbox: Tuple[int, int, int, int]
+    bitmap, start: Tuple[int, int], strokes, bbox: Tuple[int, int, int, int]
 ) -> None:
     """Helper function of _extract_strokes() which uses depth first search to
     find the pixels of a glyph. 修改了传入的 strokes 参数"""
     left, upper, right, lower = bbox
-    stack = [start, ]
-    while stack:#白色是1，為true
+    stack = [
+        start,
+    ]
+    while stack:  # 白色是1，為true
         x, y = stack.pop()
         if y - 1 >= upper and bitmap[x, y - 1] and strokes.add(_xy(x, y - 1)):
             stack.append((x, y - 1))
         if y + 1 < lower and bitmap[x, y + 1] and strokes.add(_xy(x, y + 1)):
             stack.append((x, y + 1))
         if x - 1 >= left and bitmap[x - 1, y] and strokes.add(_xy(x - 1, y)):
             stack.append((x - 1, y))
@@ -348,56 +336,77 @@
         max_x = max(x, max_x)
         min_y = min(y, min_y)
         max_y = max(y, max_y)
         stroke.append((x, y))
 
 
 def _draw_stroke(
-        bitmap,
-        stroke: Sequence[Tuple[int, int]],
-        tpl: Template,
-        center: Tuple[float, float],
-        rand
+    bitmap,
+    stroke: Sequence[Tuple[int, int]],
+    tpl: Template,
+    center: Tuple[float, float],
+    rand,
 ) -> None:
     dx = gauss(rand, 0, tpl.get_perturb_x_sigma())
     dy = gauss(rand, 0, tpl.get_perturb_y_sigma())
     theta = gauss(rand, 0, tpl.get_perturb_theta_sigma())
-    
+
     ink_depth_sigma = tpl.get_ink_depth_sigma()
     original_fill = tpl.get_fill()
     # 添加随机扰动
     ink_depth_rand = gauss(rand, 0, ink_depth_sigma)
     if isinstance(original_fill, int):
         # 如果 original_fill 是一个整数
         rand_fill = max(0, min(100, int(original_fill + ink_depth_rand)))
     elif isinstance(original_fill, tuple):
-        # 如果 original_fill 是一个三元组（假设是 RGB 值）
-        rand_fill = tuple(max(0, min(100, int(channel + ink_depth_rand))) for channel in original_fill)
-    # print('rand_fill',rand_fill)
-            
+        if len(original_fill) == 3:
+            # 如果 original_fill 是一个三元组（假设是 RGB 值）
+            rand_fill = tuple(
+                max(0, min(255, int(channel + ink_depth_rand)))
+                for channel in original_fill
+            )
+        elif len(original_fill) == 4:
+            # 如果 original_fill 是一个四元组（假设是 RGBA 值）
+            # 保持 Alpha 通道不变
+            rand_fill = tuple(
+                (
+                    max(0, min(255, int(channel + ink_depth_rand)))
+                    if i < 3
+                    else original_fill[3]
+                )
+                for i, channel in enumerate(original_fill)
+            )
+
+    # 打印结果以验证
+    # print('rand_fill', rand_fill)
+
     for x, y in stroke:
         new_x, new_y = _rotate(center, x, y, theta)
         new_x = round(new_x + dx)
         new_y = round(new_y + dy)
         width, height = tpl.get_size()
         if 0 <= new_x < width and 0 <= new_y < height:
             bitmap[new_x, new_y] = rand_fill
 
 
 def _rotate(
-        center: Tuple[float, float], x: float, y: float, theta: float
+    center: Tuple[float, float], x: float, y: float, theta: float
 ) -> Tuple[float, float]:
     if theta == 0:
         return x, y
-    new_x = ((x - center[0]) * math.cos(theta)
-             + (y - center[1]) * math.sin(theta)
-             + center[0])
-    new_y = ((y - center[1]) * math.cos(theta)
-             - (x - center[0]) * math.sin(theta)
-             + center[1])
+    new_x = (
+        (x - center[0]) * math.cos(theta)
+        + (y - center[1]) * math.sin(theta)
+        + center[0]
+    )
+    new_y = (
+        (y - center[1]) * math.cos(theta)
+        - (x - center[0]) * math.sin(theta)
+        + center[1]
+    )
     return new_x, new_y
 
 
 def _xy(x: int, y: int) -> int:
     return (x << 16) | y
```

### Comparing `handrightbeta-8.5.1/handright/_template.py` & `handrightbeta-8.6.0/handright/_template.py`

 * *Files identical despite different names*

### Comparing `handrightbeta-8.5.1/handright/_util.py` & `handrightbeta-8.6.0/handright/_util.py`

 * *Files identical despite different names*

### Comparing `handrightbeta-8.5.1/handright/tests/test_util.py` & `handrightbeta-8.6.0/handright/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `handrightbeta-8.5.1/handrightbeta.egg-info/PKG-INFO` & `handrightbeta-8.6.0/handrightbeta.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: handrightbeta
-Version: 8.5.1
+Version: 8.6.0
 Summary: A lightweight Python library for simulating Chinese handwriting
 Home-page: https://github.com/14790897/Handright
 Author: Chenghui Li (Gsllchb)
 Author-email: 14790897abc@gmail.com
 License: bsd-3-clause
 Keywords: simulating Chinese handwriting
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `handrightbeta-8.5.1/setup.py` & `handrightbeta-8.6.0/setup.py`

 * *Files identical despite different names*

