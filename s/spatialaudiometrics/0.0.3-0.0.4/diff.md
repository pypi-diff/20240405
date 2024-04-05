# Comparing `tmp/spatialaudiometrics-0.0.3.tar.gz` & `tmp/spatialaudiometrics-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spatialaudiometrics-0.0.3.tar", last modified: Wed Apr  3 14:12:40 2024, max compression
+gzip compressed data, was "spatialaudiometrics-0.0.4.tar", last modified: Fri Apr  5 10:22:28 2024, max compression
```

## Comparing `spatialaudiometrics-0.0.3.tar` & `spatialaudiometrics-0.0.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 14:12:40.518863 spatialaudiometrics-0.0.3/
--rw-rw-rw-   0        0        0    35821 2024-03-20 09:59:16.000000 spatialaudiometrics-0.0.3/LICENSE
--rw-rw-rw-   0        0        0       69 2024-04-03 08:31:29.000000 spatialaudiometrics-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0    44001 2024-04-03 14:12:40.517866 spatialaudiometrics-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1116 2024-04-03 08:31:29.000000 spatialaudiometrics-0.0.3/README.md
--rw-rw-rw-   0        0        0     1417 2024-04-03 14:11:32.000000 spatialaudiometrics-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-03 14:12:40.518863 spatialaudiometrics-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-03 14:12:40.504901 spatialaudiometrics-0.0.3/spatialaudiometrics/
--rw-rw-rw-   0        0        0        0 2024-03-20 09:59:17.000000 spatialaudiometrics-0.0.3/spatialaudiometrics/__init__.py
--rw-rw-rw-   0        0        0     3268 2024-03-20 09:59:17.000000 spatialaudiometrics-0.0.3/spatialaudiometrics/angular_metrics.py
--rw-rw-rw-   0        0        0    60165 2024-03-20 09:59:17.000000 spatialaudiometrics-0.0.3/spatialaudiometrics/example_data_1.csv
--rw-rw-rw-   0        0        0  2833739 2023-10-23 10:30:19.000000 spatialaudiometrics-0.0.3/spatialaudiometrics/example_sofa_1.sofa
--rw-rw-rw-   0        0        0  2838236 2023-11-07 09:18:47.000000 spatialaudiometrics-0.0.3/spatialaudiometrics/example_sofa_2.sofa
--rw-rw-rw-   0        0        0     6024 2024-04-03 11:37:57.000000 spatialaudiometrics-0.0.3/spatialaudiometrics/hrtf_metrics.py
--rw-rw-rw-   0        0        0     2182 2024-04-03 09:09:17.000000 spatialaudiometrics-0.0.3/spatialaudiometrics/lap_challenge.py
--rw-rw-rw-   0        0        0     5922 2024-04-03 08:54:17.000000 spatialaudiometrics-0.0.3/spatialaudiometrics/load_data.py
--rw-rw-rw-   0        0        0     6240 2024-03-20 10:48:46.000000 spatialaudiometrics-0.0.3/spatialaudiometrics/localisation_metrics.py
--rw-rw-rw-   0        0        0     1401 2024-04-03 09:01:23.000000 spatialaudiometrics-0.0.3/spatialaudiometrics/signal_processing.py
--rw-rw-rw-   0        0        0     7462 2024-03-20 09:59:17.000000 spatialaudiometrics-0.0.3/spatialaudiometrics/statistics.py
--rw-rw-rw-   0        0        0    13819 2024-04-03 14:01:00.000000 spatialaudiometrics-0.0.3/spatialaudiometrics/visualisation.py
-drwxrwxrwx   0        0        0        0 2024-04-03 14:12:40.515871 spatialaudiometrics-0.0.3/spatialaudiometrics.egg-info/
--rw-rw-rw-   0        0        0    44001 2024-04-03 14:12:40.000000 spatialaudiometrics-0.0.3/spatialaudiometrics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      710 2024-04-03 14:12:40.000000 spatialaudiometrics-0.0.3/spatialaudiometrics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 14:12:40.000000 spatialaudiometrics-0.0.3/spatialaudiometrics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      611 2024-04-03 14:12:40.000000 spatialaudiometrics-0.0.3/spatialaudiometrics.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-04-03 14:12:40.000000 spatialaudiometrics-0.0.3/spatialaudiometrics.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 10:22:28.465641 spatialaudiometrics-0.0.4/
+-rw-rw-rw-   0        0        0    35821 2024-03-20 09:59:16.000000 spatialaudiometrics-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0       69 2024-04-03 08:31:29.000000 spatialaudiometrics-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0    44002 2024-04-05 10:22:28.463645 spatialaudiometrics-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1117 2024-04-03 14:15:08.000000 spatialaudiometrics-0.0.4/README.md
+-rw-rw-rw-   0        0        0     1417 2024-04-05 10:22:14.000000 spatialaudiometrics-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-05 10:22:28.465641 spatialaudiometrics-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-05 10:22:28.452675 spatialaudiometrics-0.0.4/spatialaudiometrics/
+-rw-rw-rw-   0        0        0        0 2024-03-20 09:59:17.000000 spatialaudiometrics-0.0.4/spatialaudiometrics/__init__.py
+-rw-rw-rw-   0        0        0     3268 2024-03-20 09:59:17.000000 spatialaudiometrics-0.0.4/spatialaudiometrics/angular_metrics.py
+-rw-rw-rw-   0        0        0    60165 2024-03-20 09:59:17.000000 spatialaudiometrics-0.0.4/spatialaudiometrics/example_data_1.csv
+-rw-rw-rw-   0        0        0  2833739 2023-10-23 10:30:19.000000 spatialaudiometrics-0.0.4/spatialaudiometrics/example_sofa_1.sofa
+-rw-rw-rw-   0        0        0  2838236 2023-11-07 09:18:47.000000 spatialaudiometrics-0.0.4/spatialaudiometrics/example_sofa_2.sofa
+-rw-rw-rw-   0        0        0     6024 2024-04-03 11:37:57.000000 spatialaudiometrics-0.0.4/spatialaudiometrics/hrtf_metrics.py
+-rw-rw-rw-   0        0        0     2180 2024-04-05 10:19:02.000000 spatialaudiometrics-0.0.4/spatialaudiometrics/lap_challenge.py
+-rw-rw-rw-   0        0        0     5922 2024-04-03 08:54:17.000000 spatialaudiometrics-0.0.4/spatialaudiometrics/load_data.py
+-rw-rw-rw-   0        0        0     6240 2024-03-20 10:48:46.000000 spatialaudiometrics-0.0.4/spatialaudiometrics/localisation_metrics.py
+-rw-rw-rw-   0        0        0     1401 2024-04-03 09:01:23.000000 spatialaudiometrics-0.0.4/spatialaudiometrics/signal_processing.py
+-rw-rw-rw-   0        0        0     7462 2024-03-20 09:59:17.000000 spatialaudiometrics-0.0.4/spatialaudiometrics/statistics.py
+-rw-rw-rw-   0        0        0    15808 2024-04-05 09:22:06.000000 spatialaudiometrics-0.0.4/spatialaudiometrics/visualisation.py
+drwxrwxrwx   0        0        0        0 2024-04-05 10:22:28.462688 spatialaudiometrics-0.0.4/spatialaudiometrics.egg-info/
+-rw-rw-rw-   0        0        0    44002 2024-04-05 10:22:28.000000 spatialaudiometrics-0.0.4/spatialaudiometrics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      710 2024-04-05 10:22:28.000000 spatialaudiometrics-0.0.4/spatialaudiometrics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 10:22:28.000000 spatialaudiometrics-0.0.4/spatialaudiometrics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      611 2024-04-05 10:22:28.000000 spatialaudiometrics-0.0.4/spatialaudiometrics.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-04-05 10:22:28.000000 spatialaudiometrics-0.0.4/spatialaudiometrics.egg-info/top_level.txt
```

### Comparing `spatialaudiometrics-0.0.3/LICENSE` & `spatialaudiometrics-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `spatialaudiometrics-0.0.3/PKG-INFO` & `spatialaudiometrics-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spatialaudiometrics
-Version: 0.0.3
+Version: 0.0.4
 Summary: For calculating spatial audio metrics
 Author-email: "Katarina C. Poole" <katarina.poole@imperial.ac.uk>
 Maintainer-email: "Katarina C. Poole" <katarina.poole@imperial.ac.uk>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -720,15 +720,15 @@
 Requires-Dist: urllib3>=2.2.1
 
 # Spatial-Audio-Metrics
 Spatial Audio Metrics (SAM) is a Python toolbox to analyse spatial audio and spatial audio perceptual experiments.
 It is still underdevelopment so more functionality will be added
 
 # Documentation
-Detailed coumentation of the Spatial Audio Metrics can be found here: <https://spatial-audio-metrics.readthedocs.io>
+Detailed documentation of the Spatial Audio Metrics can be found here: <https://spatial-audio-metrics.readthedocs.io>
 
 # Installation
 You can install the package using pip:
 'pip install spatialaudiometrics'
 
 # License
 Copyright (C) 2024  Katarina C. Poole
```

### Comparing `spatialaudiometrics-0.0.3/README.md` & `spatialaudiometrics-0.0.4/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Spatial-Audio-Metrics
 Spatial Audio Metrics (SAM) is a Python toolbox to analyse spatial audio and spatial audio perceptual experiments.
 It is still underdevelopment so more functionality will be added
 
 # Documentation
-Detailed coumentation of the Spatial Audio Metrics can be found here: <https://spatial-audio-metrics.readthedocs.io>
+Detailed documentation of the Spatial Audio Metrics can be found here: <https://spatial-audio-metrics.readthedocs.io>
 
 # Installation
 You can install the package using pip:
 'pip install spatialaudiometrics'
 
 # License
 Copyright (C) 2024  Katarina C. Poole
```

### Comparing `spatialaudiometrics-0.0.3/pyproject.toml` & `spatialaudiometrics-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>54",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "spatialaudiometrics"
-version = "0.0.3"
+version = "0.0.4"
 
 dependencies = [
 "alabaster>=0.7.16",
 "Babel>=2.14.0",
 "certifi>=2024.2.2",
 "cftime>=1.6.3",
 "charset-normalizer>=3.3.2",
```

### Comparing `spatialaudiometrics-0.0.3/spatialaudiometrics/angular_metrics.py` & `spatialaudiometrics-0.0.4/spatialaudiometrics/angular_metrics.py`

 * *Files identical despite different names*

### Comparing `spatialaudiometrics-0.0.3/spatialaudiometrics/example_data_1.csv` & `spatialaudiometrics-0.0.4/spatialaudiometrics/example_data_1.csv`

 * *Files identical despite different names*

### Comparing `spatialaudiometrics-0.0.3/spatialaudiometrics/example_sofa_1.sofa` & `spatialaudiometrics-0.0.4/spatialaudiometrics/example_sofa_1.sofa`

 * *Files identical despite different names*

### Comparing `spatialaudiometrics-0.0.3/spatialaudiometrics/example_sofa_2.sofa` & `spatialaudiometrics-0.0.4/spatialaudiometrics/example_sofa_2.sofa`

 * *Files identical despite different names*

### Comparing `spatialaudiometrics-0.0.3/spatialaudiometrics/hrtf_metrics.py` & `spatialaudiometrics-0.0.4/spatialaudiometrics/hrtf_metrics.py`

 * *Files identical despite different names*

### Comparing `spatialaudiometrics-0.0.3/spatialaudiometrics/lap_challenge.py` & `spatialaudiometrics-0.0.4/spatialaudiometrics/lap_challenge.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 from spatialaudiometrics import hrtf_metrics as hf
 
 class Parameters:
     '''
     Parameters derived from A. Hoggs dataset
     '''
     itd_threshold = 31.6
-    ild_threshold = 4.37
-    lsd_threshold = 7.36
+    ild_threshold = 4.4
+    lsd_threshold = 7.4
     
 def calculate_task_two_metrics(original_hrtf_path,upsampled_hrtf_path):
     '''
     Function that calculates all the metrics for the lab challenge
     
     :param original_hrtf_path: full path of the original sofa file
     :param upsampled_hrtf_path: full path of the upsampled sofa file
```

### Comparing `spatialaudiometrics-0.0.3/spatialaudiometrics/load_data.py` & `spatialaudiometrics-0.0.4/spatialaudiometrics/load_data.py`

 * *Files identical despite different names*

### Comparing `spatialaudiometrics-0.0.3/spatialaudiometrics/localisation_metrics.py` & `spatialaudiometrics-0.0.4/spatialaudiometrics/localisation_metrics.py`

 * *Files identical despite different names*

### Comparing `spatialaudiometrics-0.0.3/spatialaudiometrics/signal_processing.py` & `spatialaudiometrics-0.0.4/spatialaudiometrics/signal_processing.py`

 * *Files identical despite different names*

### Comparing `spatialaudiometrics-0.0.3/spatialaudiometrics/statistics.py` & `spatialaudiometrics-0.0.4/spatialaudiometrics/statistics.py`

 * *Files identical despite different names*

### Comparing `spatialaudiometrics-0.0.3/spatialaudiometrics/visualisation.py` & `spatialaudiometrics-0.0.4/spatialaudiometrics/visualisation.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,19 @@
 Functions for visualising data
 '''
 import seaborn as sns
 import numpy as np
 import matplotlib
 import matplotlib.pyplot as plt
 from spatialaudiometrics import hrtf_metrics as hf
+from spatialaudiometrics import angular_metrics as am
 from mpl_toolkits.axes_grid1.inset_locator import inset_axes
 from matplotlib.cm import ScalarMappable
+import matplotlib.animation as animation
+
 
 class FigSize:
     '''
     Size of figure
     '''
     # optimimum size for thesis and gives a bit of space at the bottom for the beginning of a figure legend
     # Using this for now until i find better heights and widths 
@@ -279,24 +282,24 @@
     sns.scatterplot(x = hrtf.locs[:,0], y = hrtf.locs[:,1], hue = itd_us, hue_norm=(-huemax,huemax), ax = axes, palette = "vlag")
     axes.set_ylabel('Elevation (°)')
     axes.set_xlabel('Azimuth (°); -> counterclockwise')
     axes.set_title('ITD at all locations')
     finish_axes(axes)
     add_colourbar_on_side(-huemax,huemax,"vlag", axes, 'ITD (µs)')
     show()
-    
+
 def plot_ild_overview(hrtf):
     '''
     Plots the ILD at elevation 0 and also the ild by each location
     '''
     ild                     = hf.ild_estimator_rms(hrtf.hrir)
     idx                     = np.where(hrtf.locs[:,1] == 0)[0]
     sort_idx                = np.argsort(hrtf.locs[idx,0])
     idx                     = idx[sort_idx]
-    
+
     fig,gs  = create_fig(fig_size=(16,6))
     axes    = fig.add_subplot(gs[0:12,0:4], projection = 'polar')
     axes.plot(np.deg2rad(hrtf.locs[idx,0]),np.abs(ild[idx]))
     axes.set_theta_zero_location("N")
     #axes.set_rticks([200,400,600,800])
     axes.set_title('Absolute ILD (dB)')
 
@@ -305,23 +308,70 @@
     sns.scatterplot(x = hrtf.locs[:,0], y = hrtf.locs[:,1], hue = ild, hue_norm=(-huemax,huemax), ax = axes, palette = "vlag")
     axes.set_ylabel('Elevation (°)')
     axes.set_xlabel('Azimuth (°); -> counterclockwise')
     axes.set_title('ILD at all locations')
     finish_axes(axes)
     add_colourbar_on_side(-huemax,huemax,"vlag", axes, 'ILD (dB)')
     show()
-    
+
 def add_colourbar_on_side(hue_min,hue_max,colourmap,axes,axes_label):
     '''
     Adds a colourbar on the side of the plot
     
     :param hue_min: the minimum hue value used
     :param hu_max: the maximum hie value used
     :param colourmap: the colourmap used
     :param axes: the axes you want to generate it on the side of
     :param axes_label: the label you want to attach to the colourbar     
     '''
     norm    = plt.Normalize(hue_min,hue_max)
     sm      = plt.cm.ScalarMappable(cmap = colourmap, norm = norm)
     sm.set_array([])
     cbar    = axes.figure.colorbar(sm, ax = axes)
-    cbar.set_label(axes_label, rotation = 90)
+    cbar.set_label(axes_label, rotation = 90)
+
+def plot_source_locations(locs):
+    '''
+    Plots the source locations on a 3d plot.
+    
+    :param locations: numpy array where each row is a location, col 1 = azimuth, col 2 = elevation, col 3 = distance. Can easily just use hrtf.locs
+    '''
+    # Plot the locations used
+    fig,gs = create_fig(fig_size=(10,10))
+    x,y,z = am.polar2cartesian(locs[:,0], locs[:,1], locs[:,2])
+    dist = max(abs(z))
+    axes = fig.add_subplot(gs[0:12,0:12],projection='3d')
+    axes.scatter(x,y,z,s = 100)
+    axes.set_xlabel('X')
+    axes.set_ylabel('Y')
+    axes.set_title('Source locations')
+    axes.set_ylim(-dist,dist)
+    axes.set_xlim(-dist,dist)
+    axes.set_zlim(-dist,dist)
+    axes.set_aspect('equal')
+    # Annotate
+    x,y,z = am.polar2cartesian(0, 0, locs[0,2])
+    axes.text(x,y,z,  'Front', size=14, zorder=1, color = 'k')
+    x,y,z = am.polar2cartesian(90, 0, locs[0,2])
+    axes.text(x,y,z,  'Left', size=14, zorder=1, color = 'k')
+    x,y,z = am.polar2cartesian(270, 0, locs[0,2])
+    axes.text(x,y,z,  'Right', size=14, zorder=1, color = 'k')
+    finish_axes(axes)
+    show()
+    return fig, axes
+
+def create_source_location_gif(fig,axes,save_filename,dpi = 120):
+    '''
+    Creates a gif that rotates around the azimuth 
+    
+    :param fig: matplotlib figure handles
+    :param axes: matplotlib ax handle you want to rotate
+    :param save_filename: filename including path of where you want to save the file (include .gif)
+    :param dpi: dpi settings for animation, higher value = better quality but longer rendering time
+    '''
+    def rotate(angle):
+        axes.view_init(azim=angle)
+
+    print("Making animation...")
+    rot_animation = animation.FuncAnimation(fig, rotate, frames=np.arange(0, 362, 2), interval=100)
+    rot_animation.save(save_filename, dpi=dpi, writer='pillow')
+    print("Saved animation at: " + save_filename)
```

### Comparing `spatialaudiometrics-0.0.3/spatialaudiometrics.egg-info/PKG-INFO` & `spatialaudiometrics-0.0.4/spatialaudiometrics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spatialaudiometrics
-Version: 0.0.3
+Version: 0.0.4
 Summary: For calculating spatial audio metrics
 Author-email: "Katarina C. Poole" <katarina.poole@imperial.ac.uk>
 Maintainer-email: "Katarina C. Poole" <katarina.poole@imperial.ac.uk>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -720,15 +720,15 @@
 Requires-Dist: urllib3>=2.2.1
 
 # Spatial-Audio-Metrics
 Spatial Audio Metrics (SAM) is a Python toolbox to analyse spatial audio and spatial audio perceptual experiments.
 It is still underdevelopment so more functionality will be added
 
 # Documentation
-Detailed coumentation of the Spatial Audio Metrics can be found here: <https://spatial-audio-metrics.readthedocs.io>
+Detailed documentation of the Spatial Audio Metrics can be found here: <https://spatial-audio-metrics.readthedocs.io>
 
 # Installation
 You can install the package using pip:
 'pip install spatialaudiometrics'
 
 # License
 Copyright (C) 2024  Katarina C. Poole
```

### Comparing `spatialaudiometrics-0.0.3/spatialaudiometrics.egg-info/SOURCES.txt` & `spatialaudiometrics-0.0.4/spatialaudiometrics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spatialaudiometrics-0.0.3/spatialaudiometrics.egg-info/requires.txt` & `spatialaudiometrics-0.0.4/spatialaudiometrics.egg-info/requires.txt`

 * *Files identical despite different names*

