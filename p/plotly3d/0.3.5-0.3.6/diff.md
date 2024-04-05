# Comparing `tmp/plotly3d-0.3.5.tar.gz` & `tmp/plotly3d-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plotly3d-0.3.5.tar", last modified: Fri Apr  5 06:08:20 2024, max compression
+gzip compressed data, was "plotly3d-0.3.6.tar", last modified: Fri Apr  5 06:11:51 2024, max compression
```

## Comparing `plotly3d-0.3.5.tar` & `plotly3d-0.3.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-05 06:08:20.523818 plotly3d-0.3.5/
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)     1058 2024-03-31 02:54:34.000000 plotly3d-0.3.5/LICENSE
--rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)      310 2024-04-05 06:08:20.523049 plotly3d-0.3.5/PKG-INFO
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)      100 2024-04-01 03:31:03.000000 plotly3d-0.3.5/README.md
-drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-05 06:08:20.517948 plotly3d-0.3.5/plotly3d/
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-02 02:59:03.000000 plotly3d-0.3.5/plotly3d/__init__.py
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)     9559 2024-04-05 06:08:02.000000 plotly3d-0.3.5/plotly3d/plot.py
-drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-05 06:08:20.521989 plotly3d-0.3.5/plotly3d.egg-info/
--rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)      310 2024-04-05 06:08:20.518802 plotly3d-0.3.5/plotly3d.egg-info/PKG-INFO
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)      223 2024-04-05 06:08:20.519847 plotly3d-0.3.5/plotly3d.egg-info/SOURCES.txt
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        1 2024-04-05 06:08:20.520537 plotly3d-0.3.5/plotly3d.egg-info/dependency_links.txt
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)       33 2024-04-05 06:08:20.521651 plotly3d-0.3.5/plotly3d.egg-info/requires.txt
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        9 2024-04-05 06:08:20.522338 plotly3d-0.3.5/plotly3d.egg-info/top_level.txt
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)       38 2024-04-05 06:08:20.524084 plotly3d-0.3.5/setup.cfg
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)      404 2024-04-05 06:08:12.000000 plotly3d-0.3.5/setup.py
+drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-05 06:11:51.837043 plotly3d-0.3.6/
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)     1058 2024-03-31 02:54:34.000000 plotly3d-0.3.6/LICENSE
+-rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)      310 2024-04-05 06:11:51.836245 plotly3d-0.3.6/PKG-INFO
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)      100 2024-04-01 03:31:03.000000 plotly3d-0.3.6/README.md
+drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-05 06:11:51.830865 plotly3d-0.3.6/plotly3d/
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-02 02:59:03.000000 plotly3d-0.3.6/plotly3d/__init__.py
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)     9514 2024-04-05 06:11:38.000000 plotly3d-0.3.6/plotly3d/plot.py
+drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-05 06:11:51.835170 plotly3d-0.3.6/plotly3d.egg-info/
+-rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)      310 2024-04-05 06:11:51.831986 plotly3d-0.3.6/plotly3d.egg-info/PKG-INFO
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)      223 2024-04-05 06:11:51.832913 plotly3d-0.3.6/plotly3d.egg-info/SOURCES.txt
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        1 2024-04-05 06:11:51.834017 plotly3d-0.3.6/plotly3d.egg-info/dependency_links.txt
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)       33 2024-04-05 06:11:51.834836 plotly3d-0.3.6/plotly3d.egg-info/requires.txt
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        9 2024-04-05 06:11:51.835525 plotly3d-0.3.6/plotly3d.egg-info/top_level.txt
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)       38 2024-04-05 06:11:51.837315 plotly3d-0.3.6/setup.cfg
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)      404 2024-04-05 06:11:49.000000 plotly3d-0.3.6/setup.py
```

### Comparing `plotly3d-0.3.5/LICENSE` & `plotly3d-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `plotly3d-0.3.5/plotly3d/plot.py` & `plotly3d-0.3.6/plotly3d/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     filename = kwargs.get('filename', None)
     xtitle = kwargs.get('xtitle', 'X')
     ytitle = kwargs.get('ytitle', 'Y')
     ztitle = kwargs.get('ztitle', 'Z')
     force_continuous = kwargs.get('force_continuous', False)
     rescale = kwargs.get('rescale', True)
     legend = kwargs.get('legend', True)
-    colorscale = kwargs.get('colorscale', 'Viridis')
+    # colorscale = kwargs.get('colorscale', 'Viridis')
     fig = kwargs.get('fig', go.Figure())
     points = np.asarray(points)
     colors = np.asarray(colors) if colors is not None else None
     if rescale:
         if scaler is None:
             scaler = MinMaxScaler()
             scaler.fit(points)
@@ -93,15 +93,14 @@
             fig.add_trace(plot_func(
                 x=points_s[:, 0],
                 y=points_s[:, 1],
                 mode='markers',
                 marker=dict(size=s, color=colors, colorscale='Viridis', opacity=alpha, colorbar=dict(title='Color Scale')),
             ))
     
-    fig.data[0].marker.colorscale = colorscale
     if is_3d:
         fig.update_layout(
             title=title,
             scene=dict(xaxis_title=xtitle, yaxis_title=ytitle, zaxis_title=ztitle),
             showlegend=legend
         )
     else:
```

