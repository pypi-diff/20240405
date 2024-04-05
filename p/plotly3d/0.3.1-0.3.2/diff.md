# Comparing `tmp/plotly3d-0.3.1.tar.gz` & `tmp/plotly3d-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plotly3d-0.3.1.tar", last modified: Tue Apr  2 03:33:16 2024, max compression
+gzip compressed data, was "plotly3d-0.3.2.tar", last modified: Fri Apr  5 06:01:39 2024, max compression
```

## Comparing `plotly3d-0.3.1.tar` & `plotly3d-0.3.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-02 03:33:16.498439 plotly3d-0.3.1/
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)     1058 2024-03-31 02:54:34.000000 plotly3d-0.3.1/LICENSE
--rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)      310 2024-04-02 03:33:16.497616 plotly3d-0.3.1/PKG-INFO
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)      100 2024-04-01 03:31:03.000000 plotly3d-0.3.1/README.md
-drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-02 03:33:16.487494 plotly3d-0.3.1/plotly3d/
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-02 02:59:03.000000 plotly3d-0.3.1/plotly3d/__init__.py
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)     9413 2024-04-02 03:32:03.000000 plotly3d-0.3.1/plotly3d/plot.py
-drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-02 03:33:16.496659 plotly3d-0.3.1/plotly3d.egg-info/
--rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)      310 2024-04-02 03:33:16.494567 plotly3d-0.3.1/plotly3d.egg-info/PKG-INFO
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)      223 2024-04-02 03:33:16.495301 plotly3d-0.3.1/plotly3d.egg-info/SOURCES.txt
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        1 2024-04-02 03:33:16.495783 plotly3d-0.3.1/plotly3d.egg-info/dependency_links.txt
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)       33 2024-04-02 03:33:16.496291 plotly3d-0.3.1/plotly3d.egg-info/requires.txt
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        9 2024-04-02 03:33:16.496730 plotly3d-0.3.1/plotly3d.egg-info/top_level.txt
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)       38 2024-04-02 03:33:16.498515 plotly3d-0.3.1/setup.cfg
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)      404 2024-04-02 03:32:36.000000 plotly3d-0.3.1/setup.py
+drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-05 06:01:39.530812 plotly3d-0.3.2/
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)     1058 2024-03-31 02:54:34.000000 plotly3d-0.3.2/LICENSE
+-rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)      310 2024-04-05 06:01:39.529662 plotly3d-0.3.2/PKG-INFO
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)      100 2024-04-01 03:31:03.000000 plotly3d-0.3.2/README.md
+drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-05 06:01:39.522851 plotly3d-0.3.2/plotly3d/
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-02 02:59:03.000000 plotly3d-0.3.2/plotly3d/__init__.py
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)     9557 2024-04-05 06:01:04.000000 plotly3d-0.3.2/plotly3d/plot.py
+drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-05 06:01:39.528090 plotly3d-0.3.2/plotly3d.egg-info/
+-rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)      310 2024-04-05 06:01:38.000000 plotly3d-0.3.2/plotly3d.egg-info/PKG-INFO
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)      223 2024-04-05 06:01:38.000000 plotly3d-0.3.2/plotly3d.egg-info/SOURCES.txt
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        1 2024-04-05 06:01:38.000000 plotly3d-0.3.2/plotly3d.egg-info/dependency_links.txt
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)       33 2024-04-05 06:01:38.000000 plotly3d-0.3.2/plotly3d.egg-info/requires.txt
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        9 2024-04-05 06:01:38.000000 plotly3d-0.3.2/plotly3d.egg-info/top_level.txt
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)       38 2024-04-05 06:01:39.530953 plotly3d-0.3.2/setup.cfg
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)      404 2024-04-05 06:01:13.000000 plotly3d-0.3.2/setup.py
```

### Comparing `plotly3d-0.3.1/LICENSE` & `plotly3d-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `plotly3d-0.3.1/plotly3d/plot.py` & `plotly3d-0.3.2/plotly3d/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,16 @@
     title = kwargs.get('title', 'Plot')
     filename = kwargs.get('filename', None)
     xtitle = kwargs.get('xtitle', 'X')
     ytitle = kwargs.get('ytitle', 'Y')
     ztitle = kwargs.get('ztitle', 'Z')
     force_continuous = kwargs.get('force_continuous', False)
     rescale = kwargs.get('rescale', True)
+    legend = kwargs.get('legend', True)
+    colorscale = kwargs.get('colorscale', 'Viridis')
 
     points = np.asarray(points)
     colors = np.asarray(colors) if colors is not None else None
     if rescale:
         if scaler is None:
             scaler = MinMaxScaler()
             scaler.fit(points)
@@ -97,22 +99,23 @@
                 marker=dict(size=s, color=colors, colorscale='Viridis', opacity=alpha, colorbar=dict(title='Color Scale')),
             ))
 
     if is_3d:
         fig.update_layout(
             title=title,
             scene=dict(xaxis_title=xtitle, yaxis_title=ytitle, zaxis_title=ztitle),
-            showlegend=True
+            showlegend=legend
         )
     else:
         fig.update_layout(
             title=title,
             xaxis_title=xtitle, yaxis_title=ytitle,
-            showlegend=True
+            showlegend=legend
         )
+    fig.data[0].marker.colorscale = colorscale
     if filename is not None:
         fig.write_html(filename)
 
     return fig
 
 # for compatability with previous versions
 plot_3d = scatter
```

