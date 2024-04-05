# Comparing `tmp/geodynamic-0.0.1.tar.gz` & `tmp/geodynamic-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geodynamic-0.0.1.tar", last modified: Fri Apr  5 12:49:56 2024, max compression
+gzip compressed data, was "geodynamic-0.0.2.tar", last modified: Fri Apr  5 15:04:12 2024, max compression
```

## Comparing `geodynamic-0.0.1.tar` & `geodynamic-0.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-05 12:49:56.154961 geodynamic-0.0.1/
--rw-r--r--   0 mac        (501) staff       (20)       18 2024-04-05 12:40:59.000000 geodynamic-0.0.1/LICENSE.txt
--rw-r--r--   0 mac        (501) staff       (20)      953 2024-04-05 12:49:56.154860 geodynamic-0.0.1/PKG-INFO
--rw-------   0 mac        (501) staff       (20)      272 2024-04-05 12:38:51.000000 geodynamic-0.0.1/README.md
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-05 12:49:56.147813 geodynamic-0.0.1/geodynamic/
--rw-------   0 mac        (501) staff       (20)        0 2024-04-05 11:31:09.000000 geodynamic-0.0.1/geodynamic/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-05 12:49:56.151261 geodynamic-0.0.1/geodynamic/geo/
--rw-------   0 mac        (501) staff       (20)        0 2023-12-28 13:25:09.000000 geodynamic-0.0.1/geodynamic/geo/__init__.py
--rw-------   0 mac        (501) staff       (20)    10257 2024-02-21 13:25:22.000000 geodynamic-0.0.1/geodynamic/geo/construction.py
--rw-------   0 mac        (501) staff       (20)    23251 2024-03-01 12:40:39.000000 geodynamic-0.0.1/geodynamic/geo/lib_commands.py
--rw-------   0 mac        (501) staff       (20)    12689 2024-03-01 18:21:15.000000 geodynamic-0.0.1/geodynamic/geo/lib_elements.py
--rw-------   0 mac        (501) staff       (20)     1752 2024-01-22 09:44:40.000000 geodynamic-0.0.1/geodynamic/geo/lib_vars.py
--rw-------   0 mac        (501) staff       (20)    25136 2024-04-05 12:18:45.000000 geodynamic-0.0.1/geodynamic/manim_dynamic.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-05 12:49:56.153784 geodynamic-0.0.1/geodynamic/parsers/
--rw-------   0 mac        (501) staff       (20)        0 2023-12-28 13:25:33.000000 geodynamic-0.0.1/geodynamic/parsers/__init__.py
--rw-------   0 mac        (501) staff       (20)    13622 2024-04-05 11:51:36.000000 geodynamic-0.0.1/geodynamic/parsers/ggb_generator.py
--rw-------   0 mac        (501) staff       (20)     4295 2024-04-05 11:52:01.000000 geodynamic-0.0.1/geodynamic/parsers/ggb_parser.py
--rw-------   0 mac        (501) staff       (20)     3344 2024-04-05 11:52:04.000000 geodynamic-0.0.1/geodynamic/parsers/short_parser.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-05 12:49:56.154476 geodynamic-0.0.1/geodynamic.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)      953 2024-04-05 12:49:56.000000 geodynamic-0.0.1/geodynamic.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      542 2024-04-05 12:49:56.000000 geodynamic-0.0.1/geodynamic.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2024-04-05 12:49:56.000000 geodynamic-0.0.1/geodynamic.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)       70 2024-04-05 12:49:56.000000 geodynamic-0.0.1/geodynamic.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)       11 2024-04-05 12:49:56.000000 geodynamic-0.0.1/geodynamic.egg-info/top_level.txt
--rw-r--r--   0 mac        (501) staff       (20)       38 2024-04-05 12:49:56.155459 geodynamic-0.0.1/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)      961 2024-04-05 12:49:30.000000 geodynamic-0.0.1/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-05 15:04:12.316134 geodynamic-0.0.2/
+-rw-r--r--   0 mac        (501) staff       (20)       18 2024-04-05 12:40:59.000000 geodynamic-0.0.2/LICENSE.txt
+-rw-r--r--   0 mac        (501) staff       (20)      953 2024-04-05 15:04:12.315837 geodynamic-0.0.2/PKG-INFO
+-rw-------   0 mac        (501) staff       (20)      272 2024-04-05 12:38:51.000000 geodynamic-0.0.2/README.md
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-05 15:04:12.307218 geodynamic-0.0.2/geodynamic/
+-rw-------   0 mac        (501) staff       (20)        0 2024-04-05 11:31:09.000000 geodynamic-0.0.2/geodynamic/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-05 15:04:12.311744 geodynamic-0.0.2/geodynamic/geo/
+-rw-------   0 mac        (501) staff       (20)        0 2023-12-28 13:25:09.000000 geodynamic-0.0.2/geodynamic/geo/__init__.py
+-rw-------   0 mac        (501) staff       (20)    10257 2024-02-21 13:25:22.000000 geodynamic-0.0.2/geodynamic/geo/construction.py
+-rw-------   0 mac        (501) staff       (20)    23251 2024-03-01 12:40:39.000000 geodynamic-0.0.2/geodynamic/geo/lib_commands.py
+-rw-------   0 mac        (501) staff       (20)    12689 2024-03-01 18:21:15.000000 geodynamic-0.0.2/geodynamic/geo/lib_elements.py
+-rw-------   0 mac        (501) staff       (20)     1752 2024-01-22 09:44:40.000000 geodynamic-0.0.2/geodynamic/geo/lib_vars.py
+-rw-------   0 mac        (501) staff       (20)    25110 2024-04-05 14:53:52.000000 geodynamic-0.0.2/geodynamic/manim_dynamic.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-05 15:04:12.314370 geodynamic-0.0.2/geodynamic/parsers/
+-rw-------   0 mac        (501) staff       (20)        0 2023-12-28 13:25:33.000000 geodynamic-0.0.2/geodynamic/parsers/__init__.py
+-rw-------   0 mac        (501) staff       (20)    13622 2024-04-05 11:51:36.000000 geodynamic-0.0.2/geodynamic/parsers/ggb_generator.py
+-rw-------   0 mac        (501) staff       (20)     5939 2024-04-05 14:57:27.000000 geodynamic-0.0.2/geodynamic/parsers/ggb_parser.py
+-rw-------   0 mac        (501) staff       (20)     3344 2024-04-05 11:52:04.000000 geodynamic-0.0.2/geodynamic/parsers/short_parser.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-05 15:04:12.315021 geodynamic-0.0.2/geodynamic.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)      953 2024-04-05 15:04:12.000000 geodynamic-0.0.2/geodynamic.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      542 2024-04-05 15:04:12.000000 geodynamic-0.0.2/geodynamic.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2024-04-05 15:04:12.000000 geodynamic-0.0.2/geodynamic.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)       70 2024-04-05 15:04:12.000000 geodynamic-0.0.2/geodynamic.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)       11 2024-04-05 15:04:12.000000 geodynamic-0.0.2/geodynamic.egg-info/top_level.txt
+-rw-r--r--   0 mac        (501) staff       (20)       38 2024-04-05 15:04:12.317354 geodynamic-0.0.2/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)      961 2024-04-05 15:03:53.000000 geodynamic-0.0.2/setup.py
```

### Comparing `geodynamic-0.0.1/PKG-INFO` & `geodynamic-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geodynamic
-Version: 0.0.1
+Version: 0.0.2
 Summary: Geometric tools for parsing GeoGebra construction, proccess with manim animation and export to SVG
 Home-page: https://gitlab.mathem.ru/
 Author: ivaleo
 Author-email: ivaleotion@gmail.com
 Keywords: geometry dynamic geogebra manim animation svg python
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `geodynamic-0.0.1/geodynamic/geo/construction.py` & `geodynamic-0.0.2/geodynamic/geo/construction.py`

 * *Files identical despite different names*

### Comparing `geodynamic-0.0.1/geodynamic/geo/lib_commands.py` & `geodynamic-0.0.2/geodynamic/geo/lib_commands.py`

 * *Files identical despite different names*

### Comparing `geodynamic-0.0.1/geodynamic/geo/lib_elements.py` & `geodynamic-0.0.2/geodynamic/geo/lib_elements.py`

 * *Files identical despite different names*

### Comparing `geodynamic-0.0.1/geodynamic/geo/lib_vars.py` & `geodynamic-0.0.2/geodynamic/geo/lib_vars.py`

 * *Files identical despite different names*

### Comparing `geodynamic-0.0.1/geodynamic/manim_dynamic.py` & `geodynamic-0.0.2/geodynamic/manim_dynamic.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,18 +92,20 @@
         return self.geo.element(name)
     
     def addGeoElement(self, elem, show = False):
         mobj = CreateMObject(elem, z_auto = True)
         self.obj[elem.name] = mobj
         if mobj is not None:
             self.add(mobj)
+            #print('Visible', elem.name, elem.visible)
             if (not show) | (not elem.visible): mobj.set_opacity(0)
 
     def addAllGeometry(self, show = False):
-        for el in self.geo.elements: el.visible = False
+        if not show:
+            for el in self.geo.elements: el.visible = False
         element_types = [
             [geo.Polygon],
             [geo.Angle],
             [geo.Circle, geo.Arc, geo.Segment],
             [geo.Point]
         ]
 
@@ -527,17 +529,14 @@
             m = (p1 + p2) / 2
             arr = []
 
             if dash: arr.append(DashedLine([p1[0], p1[1], 0], [p2[0], p2[1], 0], 
                             color = col_s, stroke_opacity = op_s, stroke_width = lw, dash_length = 0.17, dashed_ratio = dash).set_z_index(zz))
             else: arr.append(Line([p1[0], p1[1], 0], [p2[0], p2[1], 0], 
                             color = col_s, stroke_opacity = op_s, stroke_width = lw).set_z_index(zz))
-            
-            #if dash: 
-            #    arr[0] = DashedVMobject(arr[0], dashed_ratio = dash)
 
             if 'lines' in elem.style:
                 num = elem.style['lines']
                 dn = elem.data.n * style.strich_len / 2
                 v = (p2 - p1) / np.linalg.norm(p2 - p1)
                 line = Line([m[0] + dn[0], m[1] + dn[1], 0], [m[0] - dn[0], m[1] - dn[1], 0],
                             color = col_s, stroke_width = lw, stroke_opacity = op_s).set_z_index(zz)
```

### Comparing `geodynamic-0.0.1/geodynamic/parsers/ggb_generator.py` & `geodynamic-0.0.2/geodynamic/parsers/ggb_generator.py`

 * *Files identical despite different names*

### Comparing `geodynamic-0.0.1/geodynamic/parsers/ggb_parser.py` & `geodynamic-0.0.2/geodynamic/parsers/ggb_parser.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 from ..geo.lib_commands import Command
 from ..geo.lib_vars import *
 
 temp_path = os.path.join(os.getcwd(), "temp")
 
 #--------------------------------------------------------------------------
 
+def rgb_to_hex(r, g, b):
+    return '#{:02x}{:02x}{:02x}'.format(r, g, b)
+
 def get_constr_xelem(ggb_path: str): # -> XElement:
     try:    
         os.mkdir(temp_path)
     except FileExistsError:
         pass
     shutil.copyfile(ggb_path, os.path.join(temp_path, "temp.ggb"))
     
@@ -45,28 +48,50 @@
                 style[name] = {}
 
                 elem = xelem.find("decoration")
                 if elem is not None: 
                     style[name]['lines'] = int(elem.attrib['type'])
                     if xelem.attrib['type'] == 'angle':
                         style[name]['lines'] += 1
-
-                #elem = xelem.find("labelOffset")
-                #if elem is not None: 
-                #    style[name]['offset'] = [float(elem.attrib['x']) / 100, -float(elem.attrib['y']) / 100]
-
-                show = xelem.find("show")
-                labelMode = xelem.find("labelMode")
-                caption = xelem.find("caption")
-                if show is not None: 
-                    style[name]['show_label'] = (show.attrib['label'] == 'true')
-                if labelMode is not None:
-                    if (labelMode.attrib['val'] == '3') & (caption is not None):
+                       
+                elem = xelem.find("show")
+                if elem is not None: 
+                    style[name]['show_element'] = (elem.attrib['object'] == 'true')
+                    style[name]['show_label'] = (elem.attrib['label'] == 'true')
+                
+                elem = xelem.find("labelMode")
+                if elem is not None:
+                    caption = xelem.find("caption")
+                    if (elem.attrib['val'] == '3') & (caption is not None):
                         style[name]['label'] = caption.attrib['val']
-
+                        
+                elem = xelem.find("labelOffset")
+                if elem is not None: 
+                    style[name]['offset'] = [float(elem.attrib['x']) / 100, -float(elem.attrib['y']) / 100]
+ 
+                elem = xelem.find("arcSize")
+                if elem is not None: 
+                    if xelem.attrib['type'] == 'angle':
+                        style[name]['r_offset'] = (float(elem.attrib['val']) - 30) / 30
+                        
+                elem = xelem.find("objColor")
+                if elem is not None:
+                    r, g, b, a = int(elem.attrib['r']), int(elem.attrib['g']), int(elem.attrib['b']), float(elem.attrib['alpha'])
+                    if xelem.attrib['type'] in ['angle', 'polygon', 'arc', 'circle']:
+                        style[name]['fill'] = rgb_to_hex(r, g, b)
+                        style[name]['fill_opacity'] = a
+                    lineStyle = xelem.find("lineStyle")
+                    if lineStyle is not None:
+                        thick, tt, op = lineStyle.attrib['thickness'], lineStyle.attrib['type'], float(lineStyle.attrib['opacity'])
+                        if xelem.attrib['type'] in ['angle', 'segment', 'arc', 'circle']:
+                            style[name]['stroke'] = rgb_to_hex(r, g, b)
+                            #style[name]['stroke_opacity'] = op / 255
+                            #style[name]['stroke_width'] = thick
+                            if int(tt) > 0: style[name]['stroke_dash'] = 0.65
+                        
         if xelems_left_to_pass:
             xelems_left_to_pass -= 1
             continue
 
         if xelem.tag == "expression":
             #xelems_left_to_pass = 1
             continue
@@ -104,14 +129,17 @@
 
     constr.rebuild(debug = debug)
 
     #styling elements
     for name in style:
         for key in style[name]:
             #print(f'STYLE >> {name} >> {key} = {style[name][key]}')
+            if key == 'show_element':
+                constr.element(name).visible = style[name][key]
+                continue
             constr.element(name).style[key] = style[name][key]
 
     return constr
 
 def load(ggb_path: str, debug = False): # -> Construction:
     constr_xelem = get_constr_xelem(ggb_path)
     constr = parse(constr_xelem, debug = debug)
```

### Comparing `geodynamic-0.0.1/geodynamic/parsers/short_parser.py` & `geodynamic-0.0.2/geodynamic/parsers/short_parser.py`

 * *Files identical despite different names*

### Comparing `geodynamic-0.0.1/geodynamic.egg-info/PKG-INFO` & `geodynamic-0.0.2/geodynamic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geodynamic
-Version: 0.0.1
+Version: 0.0.2
 Summary: Geometric tools for parsing GeoGebra construction, proccess with manim animation and export to SVG
 Home-page: https://gitlab.mathem.ru/
 Author: ivaleo
 Author-email: ivaleotion@gmail.com
 Keywords: geometry dynamic geogebra manim animation svg python
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `geodynamic-0.0.1/geodynamic.egg-info/SOURCES.txt` & `geodynamic-0.0.2/geodynamic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geodynamic-0.0.1/setup.py` & `geodynamic-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
 setup(
   name='geodynamic',
-  version='0.0.1',
+  version='0.0.2',
   author='ivaleo',
   author_email='ivaleotion@gmail.com',
   description='Geometric tools for parsing GeoGebra construction, proccess with manim animation and export to SVG',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://gitlab.mathem.ru/',
   packages=find_packages(),
```

