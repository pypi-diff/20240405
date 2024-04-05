# Comparing `tmp/GeoHD-0.1.4.tar.gz` & `tmp/GeoHD-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GeoHD-0.1.4.tar", last modified: Tue Apr  2 18:02:24 2024, max compression
+gzip compressed data, was "GeoHD-0.1.5.tar", last modified: Fri Apr  5 18:55:29 2024, max compression
```

## Comparing `GeoHD-0.1.4.tar` & `GeoHD-0.1.5.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 18:02:24.598187 GeoHD-0.1.4/
-drwxrwxrwx   0        0        0        0 2024-04-02 18:02:24.590257 GeoHD-0.1.4/GeoHD/
--rw-rw-rw-   0        0        0     8637 2024-04-01 18:15:13.000000 GeoHD-0.1.4/GeoHD/AKDE.py
--rw-rw-rw-   0        0        0      140 2024-04-01 18:26:55.000000 GeoHD-0.1.4/GeoHD/__init__.py
--rw-rw-rw-   0        0        0     4915 2024-04-01 16:22:54.000000 GeoHD-0.1.4/GeoHD/analyze.py
--rw-rw-rw-   0        0        0     4355 2024-04-02 14:23:48.000000 GeoHD-0.1.4/GeoHD/process.py
--rw-rw-rw-   0        0        0     7367 2024-04-02 18:00:56.000000 GeoHD-0.1.4/GeoHD/utils.py
--rw-rw-rw-   0        0        0     2912 2024-04-02 08:36:03.000000 GeoHD-0.1.4/GeoHD/visualize.py
-drwxrwxrwx   0        0        0        0 2024-04-02 18:02:24.596244 GeoHD-0.1.4/GeoHD.egg-info/
--rw-rw-rw-   0        0        0      386 2024-04-02 18:02:24.000000 GeoHD-0.1.4/GeoHD.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2024-04-02 18:02:24.000000 GeoHD-0.1.4/GeoHD.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 18:02:24.000000 GeoHD-0.1.4/GeoHD.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-04-02 18:02:24.000000 GeoHD-0.1.4/GeoHD.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-02 18:02:24.000000 GeoHD-0.1.4/GeoHD.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35182 2024-04-01 18:46:45.000000 GeoHD-0.1.4/LICENSE
--rw-rw-rw-   0        0        0      386 2024-04-02 18:02:24.597246 GeoHD-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     3965 2024-04-02 16:29:01.000000 GeoHD-0.1.4/README.md
--rw-rw-rw-   0        0        0       42 2024-04-02 18:02:24.598187 GeoHD-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      469 2024-04-02 18:01:46.000000 GeoHD-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-02 18:02:24.595240 GeoHD-0.1.4/test/
--rw-rw-rw-   0        0        0        0 2024-04-01 18:50:35.000000 GeoHD-0.1.4/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 18:55:29.963652 GeoHD-0.1.5/
+drwxrwxrwx   0        0        0        0 2024-04-05 18:55:29.955590 GeoHD-0.1.5/GeoHD/
+-rw-rw-rw-   0        0        0     8637 2024-04-01 18:15:13.000000 GeoHD-0.1.5/GeoHD/AKDE.py
+-rw-rw-rw-   0        0        0      161 2024-04-05 18:06:35.000000 GeoHD-0.1.5/GeoHD/__init__.py
+-rw-rw-rw-   0        0        0     4915 2024-04-01 16:22:54.000000 GeoHD-0.1.5/GeoHD/analyze.py
+-rw-rw-rw-   0        0        0     4358 2024-04-05 18:26:40.000000 GeoHD-0.1.5/GeoHD/process.py
+-rw-rw-rw-   0        0        0     7367 2024-04-02 18:00:56.000000 GeoHD-0.1.5/GeoHD/utils.py
+-rw-rw-rw-   0        0        0     2912 2024-04-05 18:31:26.000000 GeoHD-0.1.5/GeoHD/visualize.py
+-rw-rw-rw-   0        0        0     9599 2024-04-05 18:21:57.000000 GeoHD-0.1.5/GeoHD/zone.py
+drwxrwxrwx   0        0        0        0 2024-04-05 18:55:29.961645 GeoHD-0.1.5/GeoHD.egg-info/
+-rw-rw-rw-   0        0        0      405 2024-04-05 18:55:29.000000 GeoHD-0.1.5/GeoHD.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      301 2024-04-05 18:55:29.000000 GeoHD-0.1.5/GeoHD.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 18:55:29.000000 GeoHD-0.1.5/GeoHD.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-04-05 18:55:29.000000 GeoHD-0.1.5/GeoHD.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-05 18:55:29.000000 GeoHD-0.1.5/GeoHD.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35182 2024-04-01 18:46:45.000000 GeoHD-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0      405 2024-04-05 18:55:29.962649 GeoHD-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4768 2024-04-05 18:54:02.000000 GeoHD-0.1.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-05 18:55:29.963995 GeoHD-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      484 2024-04-05 18:54:02.000000 GeoHD-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 18:55:29.961110 GeoHD-0.1.5/test/
+-rw-rw-rw-   0        0        0        0 2024-04-01 18:50:35.000000 GeoHD-0.1.5/test/__init__.py
```

### Comparing `GeoHD-0.1.4/GeoHD/AKDE.py` & `GeoHD-0.1.5/GeoHD/AKDE.py`

 * *Files identical despite different names*

### Comparing `GeoHD-0.1.4/GeoHD/analyze.py` & `GeoHD-0.1.5/GeoHD/analyze.py`

 * *Files identical despite different names*

### Comparing `GeoHD-0.1.4/GeoHD/process.py` & `GeoHD-0.1.5/GeoHD/process.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         np.arange(xmin, xmax, pixel_size),
         np.arange(ymin, ymax, pixel_size)
     )
     xy = np.vstack([x.ravel(), y.ravel()])
     z = kde(xy).reshape(x.shape)
     return z
 
-def process_shapefile(input_file_path, bandwidth=0.2, pixel_size=50):
+def process_shapefile(input_file_path, bandwidth=0.2, pixel_size=0.001):
     """
     Process a shapefile to generate a kernel density estimation raster.
 
     Parameters:
         input_file_path (str): Path to the input shapefile.
         bandwidth (float): Bandwidth for kernel density estimation. Default is 0.2.
         pixel_size (float): Pixel size for density raster. Default is 50.
@@ -81,15 +81,15 @@
     Parameters:
         smoothed_density (numpy.ndarray): Smoothed density raster array.
         xmin (float): Minimum x-coordinate of the bounding box.
         ymin (float): Minimum y-coordinate of the bounding box.
         xmax (float): Maximum x-coordinate of the bounding box.
         ymax (float): Maximum y-coordinate of the bounding box.
     """
-    plt.figure(figsize=(8, 8))
+    plt.figure(figsize=(6, 6))
     plt.imshow(smoothed_density, extent=[xmin, xmax, ymin, ymax], origin='lower', cmap='Purples')
     plt.colorbar(label='Density')
     plt.xlabel('Longitude')
     plt.ylabel('Latitude')
     plt.title('Kernel Density Estimation')
     plt.show()
```

### Comparing `GeoHD-0.1.4/GeoHD/utils.py` & `GeoHD-0.1.5/GeoHD/utils.py`

 * *Files identical despite different names*

### Comparing `GeoHD-0.1.4/GeoHD/visualize.py` & `GeoHD-0.1.5/GeoHD/visualize.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     points_gdf = gpd.read_file(file_path)
 
     # Display the first few rows of the point data
     print("First few rows of point data:")
     print(points_gdf.head())
 
     # Create a new figure and axis for plotting
-    fig, ax = plt.subplots(figsize=(7, 7))
+    fig, ax = plt.subplots(figsize=(8, 8))
 
     # Plot the point data
     points_gdf.plot(ax=ax, markersize=20, color='red', marker='o', alpha=0.7)
 
     # Add a basemap using contextily
     ctx.add_basemap(ax, crs=points_gdf.crs.to_string(), source=ctx.providers.CartoDB.Positron)
```

### Comparing `GeoHD-0.1.4/LICENSE` & `GeoHD-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `GeoHD-0.1.4/README.md` & `GeoHD-0.1.5/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # GeoHD
 
 ![python](https://img.shields.io/badge/python-3.11-black)
-![GitHub release](https://img.shields.io/badge/release-v0.1.3-blue)
-![pypi](https://img.shields.io/badge/pypi-v0.1.3-orange)
+![GitHub release](https://img.shields.io/badge/release-v0.1.5-blue)
+![pypi](https://img.shields.io/badge/pypi-v0.1.5-orange)
 ![license](https://img.shields.io/badge/license-GNU%20AGPLv3-green)
 
 [**Getting Started**](#getting-started)
 | [**Issues**](#issues)
 | [**Contribute**](#contribute)
 | [**Citation**](#citation)
 | [**Authors**](#authors)
@@ -35,47 +35,77 @@
 
 Visualization of hotspots on real maps:
 
 ```python
 visualize_shapefile('data.shp', output_image_path='custom_image.png')
 ```
 
-![Visualization of hotspots on real maps](./doc/1.png)
+<p align="center">
+  <img src="./doc/1.png" width="400" height="300"/>
+</p>
+
 
 Analytic Plane Point Patterns: Ripley G, Ripley F, Ripley J, Ripley K, Ripley L, etc. through the plotting function.
 
 ```python
 plot_g_function('data.shp')
 ```
 
-![Analytic Plane Point Patterns](./doc/2.png)
+<p align="center">
+  <img src="./doc/2.png" width="400" height="300"/>
+</p>
+
+The study area was divided into a quadrilateral (hexagonal) grid and fast visualization was achieved based on the density of point data within the divided area.
+
+```python
+create_cell_zones(area_file, crash_file)
+create_hex_grid_zones(area_file, crash_file)
+create_cell_heatmap(area_file, crash_file)
+create_hexagonal_heatmap(area_file, crash_file)
+```
+
+<p align="center">
+  <img src="./doc/3.png" width="400" height="300"/>
+  <img src="./doc/4.png" width="400" height="300"/>
+</p>
+
+<p align="center">
+  <img src="./doc/5.png" width="400" height="300"/>
+  <img src="./doc/6.png" width="400" height="300"/>
+</p>
 
 Realization of kernel density analysis with fixed bandwidth:
 
 ```python
 density_raster = process_shapefile(input_file_path)
 plot_density_raster(density_raster,output_data_path, *gpd.read_file(input_file_path).total_bounds)
 ```
 
 Kernel density analysis for realizing adaptive bandwidth:
 
 ```python
 adaptiveKDE(shp_file,output_data_path)
 ```
 
-![AKDE](./doc/4.png)
+<p align="center">
+  <img src="./doc/8.png" width="400" height="300"/>
+</p>
+
 
 Hotspot Identification:
 
 ```python
 hotspots = extract_hotspots(density_data_path)
 visualize_hotspots(np.load(density_data_path), hotspots)
 ```
 
-![Hotspot](./doc/5.png)
+<p align="center">
+  <img src="./doc/9.png" width="400" height="300"/>
+</p>
+
 
 
 ## Issues
 
 If you encounter any **bugs** or **problems** with GeoHD, please create a post using our package [issue tracker](https://github.com/yan-yuchen/GeoHD/issues). Please provide a clear and concise description of the problem, with images or code-snippets where appropriate. We will do our best to address these problems as fast and efficiently as possible.
 
 ## Contribute
```

