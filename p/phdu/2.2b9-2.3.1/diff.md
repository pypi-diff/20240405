# Comparing `tmp/phdu-2.2b9.tar.gz` & `tmp/phdu-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phdu-2.2b9.tar", last modified: Mon Feb 26 02:51:54 2024, max compression
+gzip compressed data, was "phdu-2.3.1.tar", last modified: Fri Apr  5 11:54:27 2024, max compression
```

## Comparing `phdu-2.2b9.tar` & `phdu-2.3.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2024-02-26 02:51:54.885492 phdu-2.2b9/
--rw-r--r--   0 userx     (1000) wheel      (998)    35149 2023-07-31 18:53:26.000000 phdu-2.2b9/LICENSE.md
--rw-r--r--   0 userx     (1000) wheel      (998)     2864 2024-02-26 02:51:54.885492 phdu-2.2b9/PKG-INFO
--rw-r--r--   0 userx     (1000) wheel      (998)     1771 2023-07-31 18:53:26.000000 phdu-2.2b9/README.md
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2024-02-26 02:51:54.878826 phdu-2.2b9/phdu/
--rw-r--r--   0 userx     (1000) wheel      (998)      590 2024-02-24 02:21:10.000000 phdu-2.2b9/phdu/__init__.py
--rw-r--r--   0 userx     (1000) wheel      (998)     1948 2023-09-21 17:52:42.000000 phdu-2.2b9/phdu/_helper.py
--rw-r--r--   0 userx     (1000) wheel      (998)     2484 2024-02-04 05:18:27.000000 phdu-2.2b9/phdu/analysis.py
--rw-r--r--   0 userx     (1000) wheel      (998)     3664 2023-10-17 21:07:41.000000 phdu-2.2b9/phdu/clustering.py
--rw-r--r--   0 userx     (1000) wheel      (998)     3319 2023-07-31 18:53:27.000000 phdu-2.2b9/phdu/decomposition.py
--rw-r--r--   0 userx     (1000) wheel      (998)     1333 2023-12-05 04:36:26.000000 phdu-2.2b9/phdu/geometry.py
--rw-r--r--   0 userx     (1000) wheel      (998)     3183 2024-01-23 06:00:25.000000 phdu-2.2b9/phdu/np_utils.py
--rw-r--r--   0 userx     (1000) wheel      (998)     5912 2023-07-31 18:53:27.000000 phdu-2.2b9/phdu/pd_utils.py
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2024-02-26 02:51:54.878826 phdu-2.2b9/phdu/plots/
--rw-r--r--   0 userx     (1000) wheel      (998)       66 2023-07-31 18:53:27.000000 phdu-2.2b9/phdu/plots/__init__.py
--rw-r--r--   0 userx     (1000) wheel      (998)        0 2023-07-31 18:53:27.000000 phdu-2.2b9/phdu/plots/_mpl.py
--rw-r--r--   0 userx     (1000) wheel      (998)     4011 2023-12-05 02:04:31.000000 phdu-2.2b9/phdu/plots/base.py
--rw-r--r--   0 userx     (1000) wheel      (998)    22345 2024-02-26 02:51:35.000000 phdu-2.2b9/phdu/plots/plotly_utils.py
--rw-r--r--   0 userx     (1000) wheel      (998)     3978 2023-07-31 18:53:27.000000 phdu-2.2b9/phdu/script_fmt.py
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2024-02-26 02:51:54.882159 phdu-2.2b9/phdu/stats/
--rw-r--r--   0 userx     (1000) wheel      (998)      157 2023-07-31 18:53:27.000000 phdu-2.2b9/phdu/stats/__init__.py
--rw-r--r--   0 userx     (1000) wheel      (998)     2526 2023-07-31 18:53:27.000000 phdu-2.2b9/phdu/stats/_integration.py
--rw-r--r--   0 userx     (1000) wheel      (998)      842 2023-07-31 18:53:27.000000 phdu-2.2b9/phdu/stats/_plots.py
--rw-r--r--   0 userx     (1000) wheel      (998)      343 2023-07-31 18:53:27.000000 phdu-2.2b9/phdu/stats/_preprocess.py
--rw-r--r--   0 userx     (1000) wheel      (998)    32282 2024-01-18 07:19:52.000000 phdu-2.2b9/phdu/stats/bootstrap.py
--rw-r--r--   0 userx     (1000) wheel      (998)     9411 2023-07-31 18:53:27.000000 phdu-2.2b9/phdu/stats/conf_interval.py
--rw-r--r--   0 userx     (1000) wheel      (998)      643 2023-07-31 18:53:27.000000 phdu-2.2b9/phdu/stats/corr.py
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2024-02-26 02:51:54.882159 phdu-2.2b9/phdu/stats/rtopy/
--rw-r--r--   0 userx     (1000) wheel      (998)       22 2023-07-31 18:53:27.000000 phdu-2.2b9/phdu/stats/rtopy/__init__.py
--rw-r--r--   0 userx     (1000) wheel      (998)     1306 2023-07-31 18:53:27.000000 phdu-2.2b9/phdu/stats/rtopy/_helper.py
--rw-r--r--   0 userx     (1000) wheel      (998)     4755 2023-07-31 18:53:27.000000 phdu-2.2b9/phdu/stats/rtopy/resample.py
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2024-02-26 02:51:54.882159 phdu-2.2b9/phdu/stats/test/
--rw-r--r--   0 userx     (1000) wheel      (998)       25 2023-07-31 18:53:27.000000 phdu-2.2b9/phdu/stats/test/__init__.py
--rw-r--r--   0 userx     (1000) wheel      (998)      279 2023-07-31 18:53:27.000000 phdu-2.2b9/phdu/stats/test/_adherence.py
--rw-r--r--   0 userx     (1000) wheel      (998)    16550 2023-07-31 18:53:27.000000 phdu-2.2b9/phdu/stats/test/permutation.py
--rw-r--r--   0 userx     (1000) wheel      (998)     4437 2024-02-24 02:19:42.000000 phdu-2.2b9/phdu/storage.py
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2024-02-26 02:51:54.878826 phdu-2.2b9/phdu.egg-info/
--rwxr-xr-x   0 userx     (1000) wheel      (998)     2864 2024-02-26 02:51:54.000000 phdu-2.2b9/phdu.egg-info/PKG-INFO
--rwxr-xr-x   0 userx     (1000) wheel      (998)      786 2024-02-26 02:51:54.000000 phdu-2.2b9/phdu.egg-info/SOURCES.txt
--rwxr-xr-x   0 userx     (1000) wheel      (998)        1 2024-02-26 02:51:54.000000 phdu-2.2b9/phdu.egg-info/dependency_links.txt
--rwxr-xr-x   0 userx     (1000) wheel      (998)      302 2024-02-26 02:51:54.000000 phdu-2.2b9/phdu.egg-info/requires.txt
--rwxr-xr-x   0 userx     (1000) wheel      (998)        5 2024-02-26 02:51:54.000000 phdu-2.2b9/phdu.egg-info/top_level.txt
--rw-r--r--   0 userx     (1000) wheel      (998)      106 2024-02-26 02:51:54.885492 phdu-2.2b9/setup.cfg
--rw-r--r--   0 userx     (1000) wheel      (998)     1660 2024-02-26 02:51:49.000000 phdu-2.2b9/setup.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-04-05 11:54:27.394115 phdu-2.3.1/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)    35149 2022-11-08 11:52:59.000000 phdu-2.3.1/LICENSE.md
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2864 2024-04-05 11:54:27.394115 phdu-2.3.1/PKG-INFO
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     1771 2023-03-07 15:21:19.000000 phdu-2.3.1/README.md
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-04-05 11:54:27.302110 phdu-2.3.1/phdu/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      590 2024-04-05 11:52:28.000000 phdu-2.3.1/phdu/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     1948 2023-10-04 09:21:45.000000 phdu-2.3.1/phdu/_helper.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2484 2024-04-05 11:52:28.000000 phdu-2.3.1/phdu/analysis.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     3664 2023-10-19 13:00:53.000000 phdu-2.3.1/phdu/clustering.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     3319 2023-03-14 10:06:15.000000 phdu-2.3.1/phdu/decomposition.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     1333 2024-04-05 11:52:28.000000 phdu-2.3.1/phdu/geometry.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     3183 2024-04-05 11:52:28.000000 phdu-2.3.1/phdu/np_utils.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     5912 2023-03-16 10:33:06.000000 phdu-2.3.1/phdu/pd_utils.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-04-05 11:54:27.334112 phdu-2.3.1/phdu/plots/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)       66 2022-11-08 18:00:13.000000 phdu-2.3.1/phdu/plots/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)        0 2022-11-08 08:30:49.000000 phdu-2.3.1/phdu/plots/_mpl.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     4011 2023-10-19 15:28:08.000000 phdu-2.3.1/phdu/plots/base.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)    22437 2024-04-05 11:53:26.000000 phdu-2.3.1/phdu/plots/plotly_utils.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     3978 2023-03-10 11:02:11.000000 phdu-2.3.1/phdu/script_fmt.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-04-05 11:54:27.362113 phdu-2.3.1/phdu/stats/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      157 2023-03-16 13:28:14.000000 phdu-2.3.1/phdu/stats/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2526 2023-02-15 09:17:23.000000 phdu-2.3.1/phdu/stats/_integration.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      842 2023-04-25 08:51:47.000000 phdu-2.3.1/phdu/stats/_plots.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      343 2022-11-08 15:54:46.000000 phdu-2.3.1/phdu/stats/_preprocess.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)    32282 2024-04-05 11:52:28.000000 phdu-2.3.1/phdu/stats/bootstrap.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     9411 2023-03-20 23:41:28.000000 phdu-2.3.1/phdu/stats/conf_interval.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      643 2023-03-16 13:27:55.000000 phdu-2.3.1/phdu/stats/corr.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-04-05 11:54:27.374114 phdu-2.3.1/phdu/stats/rtopy/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)       22 2022-11-08 08:30:50.000000 phdu-2.3.1/phdu/stats/rtopy/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     1306 2022-11-08 18:28:33.000000 phdu-2.3.1/phdu/stats/rtopy/_helper.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     4755 2022-11-08 16:42:50.000000 phdu-2.3.1/phdu/stats/rtopy/resample.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-04-05 11:54:27.390115 phdu-2.3.1/phdu/stats/test/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)       25 2022-11-08 11:59:20.000000 phdu-2.3.1/phdu/stats/test/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      279 2022-11-08 14:38:29.000000 phdu-2.3.1/phdu/stats/test/_adherence.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)    16550 2023-03-07 15:36:38.000000 phdu-2.3.1/phdu/stats/test/permutation.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     4437 2024-04-05 11:52:28.000000 phdu-2.3.1/phdu/storage.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-04-05 11:54:27.322111 phdu-2.3.1/phdu.egg-info/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2864 2024-04-05 11:54:27.000000 phdu-2.3.1/phdu.egg-info/PKG-INFO
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      786 2024-04-05 11:54:27.000000 phdu-2.3.1/phdu.egg-info/SOURCES.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)        1 2024-04-05 11:54:27.000000 phdu-2.3.1/phdu.egg-info/dependency_links.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      302 2024-04-05 11:54:27.000000 phdu-2.3.1/phdu.egg-info/requires.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)        5 2024-04-05 11:54:27.000000 phdu-2.3.1/phdu.egg-info/top_level.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      106 2024-04-05 11:54:27.398115 phdu-2.3.1/setup.cfg
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     1659 2024-04-05 11:54:03.000000 phdu-2.3.1/setup.py
```

### Comparing `phdu-2.2b9/LICENSE.md` & `phdu-2.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `phdu-2.2b9/PKG-INFO` & `phdu-2.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phdu
-Version: 2.2b9
+Version: 2.3.1
 Summary: Automatically store/load data in a tidy, efficient way. Includes functions for data visualization and analysis.
 Home-page: https://github.com/medinajorge/PhD-utils
 Download-URL: https://github.com/medinajorge/PhD-utils/archive/refs/tags/v1.5-beta.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: science,statistics,tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```

### Comparing `phdu-2.2b9/README.md` & `phdu-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `phdu-2.2b9/phdu/__init__.py` & `phdu-2.3.1/phdu/__init__.py`

 * *Files identical despite different names*

### Comparing `phdu-2.2b9/phdu/_helper.py` & `phdu-2.3.1/phdu/_helper.py`

 * *Files identical despite different names*

### Comparing `phdu-2.2b9/phdu/analysis.py` & `phdu-2.3.1/phdu/analysis.py`

 * *Files identical despite different names*

### Comparing `phdu-2.2b9/phdu/clustering.py` & `phdu-2.3.1/phdu/clustering.py`

 * *Files identical despite different names*

### Comparing `phdu-2.2b9/phdu/decomposition.py` & `phdu-2.3.1/phdu/decomposition.py`

 * *Files identical despite different names*

### Comparing `phdu-2.2b9/phdu/geometry.py` & `phdu-2.3.1/phdu/geometry.py`

 * *Files identical despite different names*

### Comparing `phdu-2.2b9/phdu/np_utils.py` & `phdu-2.3.1/phdu/np_utils.py`

 * *Files identical despite different names*

### Comparing `phdu-2.2b9/phdu/pd_utils.py` & `phdu-2.3.1/phdu/pd_utils.py`

 * *Files identical despite different names*

### Comparing `phdu-2.2b9/phdu/plots/base.py` & `phdu-2.3.1/phdu/plots/base.py`

 * *Files identical despite different names*

### Comparing `phdu-2.2b9/phdu/plots/plotly_utils.py` & `phdu-2.3.1/phdu/plots/plotly_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -303,27 +303,28 @@
 
     fig = get_figure(xaxis_title=label_fmt(x), yaxis_title=label_fmt(y_label))
     xaxis_ticktext = []
     for i, idx in enumerate(x_order):
         df_i = df[df[x] == idx]
         xaxis_ticktext.append(idx)
         for j, g in enumerate(group_order):
-            color_g = colors[g]
-            Xj = X0[i] + j*width
-            df_g = df_i[df_i[group] == g].iloc[0]
-            y = df_g.sample_stat
-            CI = df_g.CI.squeeze()
-            baseline = df_g[base]
-            error_up = np.clip(CI[1], *y_range) - y
-            error_down = y - np.clip(CI[0], *y_range)
-            # plot bars
-            fig.add_trace(go.Bar(x=[Xj], y=[y], name=label_fmt(g), marker=dict(color=color_g), width=width, showlegend=i == 0))
-            fig.add_trace(go.Bar(x=[Xj], y=[baseline], name=label_fmt(base), marker=dict(color='grey'), width=width, showlegend=baseline_in_legend and i == 0 and j == (num_groups-1)))
-            # plot error
-            fig.add_trace(go.Scatter(x=[Xj], y=[y], error_y=dict(type='data', array=[error_up], arrayminus=[error_down], color=color_gradient(color_g, 'black', 6)[1], width=4, thickness=3), mode='markers', marker=dict(color=color_g, size=0.5), showlegend=False))
+            if g in df_i[group].values:
+                color_g = colors[g]
+                Xj = X0[i] + j*width
+                df_g = df_i[df_i[group] == g].iloc[0]
+                y = df_g.sample_stat
+                CI = df_g.CI.squeeze()
+                baseline = df_g[base]
+                error_up = np.clip(CI[1], *y_range) - y
+                error_down = y - np.clip(CI[0], *y_range)
+                # plot bars
+                fig.add_trace(go.Bar(x=[Xj], y=[y], name=label_fmt(g), marker=dict(color=color_g), width=width, showlegend=i == 0))
+                fig.add_trace(go.Bar(x=[Xj], y=[baseline], name=label_fmt(base), marker=dict(color='grey'), width=width, showlegend=baseline_in_legend and i == 0 and j == (num_groups-1)))
+                # plot error
+                fig.add_trace(go.Scatter(x=[Xj], y=[y], error_y=dict(type='data', array=[error_up], arrayminus=[error_down], color=color_gradient(color_g, 'black', 6)[1], width=4, thickness=3), mode='markers', marker=dict(color=color_g, size=0.5), showlegend=False))
 
     fig.update_layout(yaxis_range=y_range, barmode='overlay',
                       xaxis=dict(tickvals=np.vstack((X, X0)).mean(axis=0),
                                  ticktext=xaxis_ticktext,
                                  tickangle=90),
                      legend=dict(orientation='h', yanchor='bottom', y=1.02, xanchor='right', x=1))
     return fig
```

### Comparing `phdu-2.2b9/phdu/script_fmt.py` & `phdu-2.3.1/phdu/script_fmt.py`

 * *Files identical despite different names*

### Comparing `phdu-2.2b9/phdu/stats/_integration.py` & `phdu-2.3.1/phdu/stats/_integration.py`

 * *Files identical despite different names*

### Comparing `phdu-2.2b9/phdu/stats/_plots.py` & `phdu-2.3.1/phdu/stats/_plots.py`

 * *Files identical despite different names*

### Comparing `phdu-2.2b9/phdu/stats/bootstrap.py` & `phdu-2.3.1/phdu/stats/bootstrap.py`

 * *Files identical despite different names*

### Comparing `phdu-2.2b9/phdu/stats/conf_interval.py` & `phdu-2.3.1/phdu/stats/conf_interval.py`

 * *Files identical despite different names*

### Comparing `phdu-2.2b9/phdu/stats/corr.py` & `phdu-2.3.1/phdu/stats/corr.py`

 * *Files identical despite different names*

### Comparing `phdu-2.2b9/phdu/stats/rtopy/_helper.py` & `phdu-2.3.1/phdu/stats/rtopy/_helper.py`

 * *Files identical despite different names*

### Comparing `phdu-2.2b9/phdu/stats/rtopy/resample.py` & `phdu-2.3.1/phdu/stats/rtopy/resample.py`

 * *Files identical despite different names*

### Comparing `phdu-2.2b9/phdu/stats/test/permutation.py` & `phdu-2.3.1/phdu/stats/test/permutation.py`

 * *Files identical despite different names*

### Comparing `phdu-2.2b9/phdu/storage.py` & `phdu-2.3.1/phdu/storage.py`

 * *Files identical despite different names*

### Comparing `phdu-2.2b9/phdu.egg-info/PKG-INFO` & `phdu-2.3.1/phdu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phdu
-Version: 2.2b9
+Version: 2.3.1
 Summary: Automatically store/load data in a tidy, efficient way. Includes functions for data visualization and analysis.
 Home-page: https://github.com/medinajorge/PhD-utils
 Download-URL: https://github.com/medinajorge/PhD-utils/archive/refs/tags/v1.5-beta.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: science,statistics,tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```

### Comparing `phdu-2.2b9/phdu.egg-info/SOURCES.txt` & `phdu-2.3.1/phdu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phdu-2.2b9/setup.py` & `phdu-2.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='phdu',
-    version='2.2.b9',
+    version='2.3.1',
     author="Jorge Medina Hernández",
     author_email='medinahdezjorge@gmail.com',
     packages=find_packages("."),
     url='https://github.com/medinajorge/PhD-utils',
     download_url='https://github.com/medinajorge/PhD-utils/archive/refs/tags/v1.5-beta.tar.gz',
     description="Automatically store/load data in a tidy, efficient way. Includes functions for data visualization and analysis.",
     long_description=open('README.md').read(),
```

