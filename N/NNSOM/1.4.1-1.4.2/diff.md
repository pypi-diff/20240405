# Comparing `tmp/nnsom-1.4.1.tar.gz` & `tmp/nnsom-1.4.2.tar.gz`

## Comparing `nnsom-1.4.1.tar` & `nnsom-1.4.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    59021 2020-02-02 00:00:00.000000 nnsom-1.4.1/src/NNSOM/plots.py
--rw-r--r--   0        0        0    10365 2020-02-02 00:00:00.000000 nnsom-1.4.1/src/NNSOM/som.py
--rw-r--r--   0        0        0    20699 2020-02-02 00:00:00.000000 nnsom-1.4.1/src/NNSOM/utils.py
--rw-r--r--   0        0        0    16144 2020-02-02 00:00:00.000000 nnsom-1.4.1/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nnsom-1.4.1/LICENSE
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nnsom-1.4.1/README.md
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 nnsom-1.4.1/pyproject.toml
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 nnsom-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0    76901 2020-02-02 00:00:00.000000 nnsom-1.4.2/src/NNSOM/plots.py
+-rw-r--r--   0        0        0    10365 2020-02-02 00:00:00.000000 nnsom-1.4.2/src/NNSOM/som.py
+-rw-r--r--   0        0        0    22430 2020-02-02 00:00:00.000000 nnsom-1.4.2/src/NNSOM/utils.py
+-rw-r--r--   0        0        0    16144 2020-02-02 00:00:00.000000 nnsom-1.4.2/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nnsom-1.4.2/LICENSE
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nnsom-1.4.2/README.md
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 nnsom-1.4.2/pyproject.toml
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 nnsom-1.4.2/PKG-INFO
```

### Comparing `nnsom-1.4.1/src/NNSOM/plots.py` & `nnsom-1.4.2/src/NNSOM/plots.py`

 * *Files 18% similar despite different names*

```diff
@@ -168,15 +168,15 @@
             )
 
         # Get rid of extra white space on sides
         plt.tight_layout()
 
         return fig, ax, patches, text
 
-    def hit_hist(self, x, textFlag, mouse_click=False, connect_pick_event=True, **kwargs):
+    def hit_hist(self, x, textFlag=True, mouse_click=False, connect_pick_event=True, **kwargs):
         """ Generate Hit Histogram
 
         Parameters
         ----------
         x: array-like
             The input data to be clustered
         textFlag: bool
@@ -342,15 +342,15 @@
             ticktext.append('%.2f' % (dmax * ticklab[i]))
 
         cbar.ax.set_yticklabels(ticktext)
 
         # Get rid of extra white space on sides
         fig.tight_layout()
 
-        return fig, patches, text, cbar
+        return fig, ax, patches, text, cbar
 
     def cmplx_hit_hist(self, x, clust, perc, ind_missClass, ind21, ind12, mouse_click=False, **kwargs):
         """ Generates a complex hit histogram.
         It indicates what the majority class in each cluster is, and how many specific class occur in each cluster.
 
         Args:
             x: array-like
@@ -474,17 +474,14 @@
                 patches[neuron][0]._facecolor = cmap1(color1_idx)
                 patches[neuron][0]._linewidth = edge_width[neuron]
                 patches[neuron][0]._edgecolor = cmap2(color2_idx)
 
         # Get rid of extra white space on sides
         plt.tight_layout()
 
-        print(cmap1)
-        print(cmap2)
-
         return fig, ax, patches, text
 
     def plt_nc(self, mouse_click=False, connect_pick_event=True, **kwargs):
         """ Generates neighborhood connection map.
         The gray hexagons represent cluster centers.
 
         Args:
@@ -784,14 +781,16 @@
         cbar.ax.set_yticklabels(ticktext)
 
         if mouse_click and connect_pick_event:
             fig.canvas.mpl_connect(
                 'pick_event', lambda event: self.onpick(event, hexagons, hexagon_to_neuron, **kwargs)
             )
 
+        plt.tight_layout()
+
         return fig, ax, patches, cbar
 
     def setup_axes(self):
         # Setup figure, axes and sub-axes for plots
         pos = self.pos
         numNeurons = self.numNeurons
 
@@ -1296,14 +1295,415 @@
                     color = plt.cm.viridis(norm(feature_weights[j]))  # Choose colormap as viridis
                     inverted_color = tuple(
                         1 - np.array(color[:3]))  # Invert the color to make darker colors represent larger weights
                     ax.fill(pos[0, j] + shapex, pos[1, j] + shapey, facecolor=inverted_color, edgecolor=(0.8, 0.8, 0.8))
 
         plt.show()
 
+    # Generic Plot Function
+    def plot(self, plot_type, data_dict=None, ind=None, target_class=None, use_add_1darray=False,
+             use_add_2darray=False, **kwargs):
+        """ Generic Plot Function.
+        It generates a plot based on the plot type and data provides.
+
+        Parameters
+        ----------
+        plot_type : str
+            The type of plot to be generated:
+            ["top", "top_num", "hit_hist", "gray_hist",
+            "color_hist", "complex_hist", "nc", "neuron_dist",
+            "simple_grid", "stem", "pie", "wgts", "pie", "hist",
+            "box", "violin", "scatter", "component_positions",
+            "component_planes"]
+
+        data_dict: dict (optional)
+            A dictionary containing the data to be plotted.
+            The key is prefixed with the data type and the value is the data itself.
+            {"original_data", "input_data", "target", "clust","cat_1darray", "cat_2darray",
+            "num_1darray"}
+
+        ind : int, str or array-like (optional)
+            The indices of the data to be plotted.
+
+        target_class: int (optional)
+            The target class to be plotted.
+
+        use_add_1darray: bool (optional)
+            If true, the additional array to be used.
+
+        use_add_2darray: bool (optional)
+            If true, the additional 2D array to be used.
+
+        **kwargs : dict
+            Additional arguments to be passed to the interactive plot function.
+        """
+        # Plot Types allowed
+        plot_types = ["top", "top_num",
+                      "hit_hist", "gray_hist", "color_hist", "complex_hist",
+                      "neuron_connection", "neuron_dist",
+                      "simple_grid",
+                      "stem", "pie", "wgts", "hist", "box", "violin", "scatter",
+                      "component_positions", "component_planes"]
+
+        # Validate the plot type
+        if plot_type not in plot_types:
+            raise ValueError(f"Invalid plot type: {plot_type}")
+
+        # Validate the data_dict
+        if data_dict is None and plot_type not in ["top", "top_num",
+                                                   "neuron_connection",
+                                                   "neuron_dist", "wgts"]:
+            raise ValueError("data_dict is required for this plot type.")
+
+        # Validate the plot function
+        plot_functions = {
+            "top": self.plt_top,
+            "top_num": self.plt_top_num,
+            "hit_hist": self.hit_hist,
+            "gray_hist": self.gray_hist,
+            "color_hist": self.color_hist,
+            "complex_hist": self.custom_cmplx_hit_hist,
+            "neuron_connection": self.plt_nc,
+            "neuron_dist": self.neuron_dist_plot,
+            "simple_grid": self.simple_grid,
+            "stem": self.plt_stem,
+            "pie": self.plt_pie,
+            "wgts": self.plt_wgts,
+            "hist": self.plt_histogram,
+            "box": self.plt_boxplot,
+            "violin": self.plt_violin_plot,
+            "scatter": self.plt_scatter,
+            "component_positions": self.component_positions,
+            "component_planes": self.component_planes
+        }
+
+        # Assign the plot function
+        selected_plot = plot_functions.get(plot_type)
+
+        # Error Handling if the plot function recieve the appropriate arguments
+        def validate_data_dict(keys):
+            for key in keys:
+                if key not in data_dict:
+                    raise ValueError(f"{key} is required for this plot type.")
+
+        # ======== Topology, Neuron Connection, Neuron Distance, and Weight Plot ==========
+        if plot_type in ["top", "top_num", "neuron_connection", "neuron_dist", "wgts"]:
+            # Call the plot function
+            return selected_plot(**kwargs)
+
+        # ======== Components Plane Family ==========
+        # Need to be modified
+        elif plot_type in ['component_positions', 'component_planes']:
+            # Error Handling if the data_dict have the scaled input data X
+            validate_data_dict(["input_data"])
+            # Data Preparation
+            x_scaled = data_dict['input_data']
+            # Invoke Function
+            return selected_plot(x_scaled)
+
+        # =====================  Hit Histogram Family =====================
+        elif plot_type in ['hit_hist', 'gray_hist', 'color_hist', 'complex_hist']:
+            # Validate the data_dict have the scaled input data
+            validate_data_dict(["input_data"])
+
+            # Extract input data
+            x = data_dict['input_data']
+
+            if plot_type in ['hit_hist']:
+                # Invoke the function
+                return selected_plot(x, True, **kwargs)
+
+            elif plot_type in ['gray_hist']:
+                if use_add_1darray:  # Check if user want to use additional 1D array
+
+                    # Validate the data_dict have the additional 1D array and original data
+                    validate_data_dict(["cat_1darray", "original_data"])
+
+                    # Validate the length of additional 1D array is equal to number of neuron or length of original data.
+                    if len(data_dict['cat_1darray']) != self.numNeurons and len(data_dict['cat_1darray']) != len(
+                            data_dict['original_data']):
+                        raise ValueError(
+                            "The additional 1D array must have the same length as the clust data or original data.")
+
+                    # If the length of additional 1D array is equal to the length of clust data just extract data
+                    elif len(data_dict['cat_1darray']) == self.numNeurons:
+                        perc = data_dict['cat_1darray']
+
+                    # If the length of additional 1D array is equal to the length of original data then preprocess the data
+                    elif len(data_dict['cat_1darray']) == len(data_dict['original_data']):
+
+                        # Validate the data_dict have the clust data
+                        validate_data_dict(["clust"])
+
+                        if target_class is None:
+                            raise ValueError("The target class is required. Eg. target_class = 1")
+
+                        # Preprocess and extract the data
+                        perc = get_perc_cluster(data_dict['cat_1darray'], target_class, data_dict['clust'])
+
+                else:
+                    # Error Handling if the target data not provided
+                    validate_data_dict(["target", "clust"])
+
+                    # Validate the data_dict have the clust data
+                    if target_class is None:
+                        raise ValueError("The target class is required. Eg. target_class = 1")
+
+                    perc = get_perc_cluster(data_dict['target'], target_class, data_dict['clust'])
+
+                # Invoke the gray hist function
+                return selected_plot(x, perc, **kwargs)
+
+            elif plot_type in ['color_hist']:
+                # Check if user want to use additional 1D array
+                if use_add_1darray:
+                    # Check if the additional 1D array and original data are provided
+                    validate_data_dict(["num_1darray", "original_data"])
+
+                    num_feature = data_dict['num_1darray']
+                    original_data_size = len(data_dict['original_data'])
+
+                    if len(num_feature) != original_data_size and len(num_feature) != self.numNeurons:
+                        raise ValueError(
+                            "The additional 1D array must have the same length as the clust data or original data.")
+
+                    elif len(num_feature) == original_data_size:
+                        # Check if the clust data is provided
+                        validate_data_dict(["clust"])
+
+                        clust = data_dict['clust']
+                        avg = get_cluster_avg(num_feature, clust)
+
+                    elif len(num_feature) == self.numNeurons:
+
+                        avg = num_feature
+
+                else:
+                    # Error Handling if the original data and clust are provided
+                    validate_data_dict(["original_data", "clust"])
+
+                    if ind is None:
+                        raise ValueError(
+                            "The indices is required for this plot type. Which numerical feature in the original data you want to plot? Eg. ind = 0")
+
+                    feature = data_dict['original_data'][:, ind]
+
+                    avg = get_cluster_avg(feature, data_dict['clust'])
+
+                return selected_plot(x, avg, **kwargs)
+
+            elif plot_type in ['complex_hist']:
+                if use_add_2darray:
+                    # Validate the data_dict have the additional 2D array
+                    validate_data_dict(["cat_2darray"])
+
+                    cat_2darray = data_dict['cat_2darray']
+
+                    if cat_2darray.shape[0] != self.numNeurons:
+                        raise ValueError(
+                            "The additional 2D array must have the same length as the number of neurons.")
+
+                    # Validate the additional 2D array have 3 features
+                    if cat_2darray.shape[1] != 3:
+                        raise ValueError(
+                            "The additional 2D array must have 3 features. E.g. [numNeurons, [face_labels, edge_labels, edge_widths]]")
+
+                    # Extract Data
+                    face_labels = cat_2darray[:, 0]
+                    edge_labels = cat_2darray[:, 1]
+                    edge_widths = cat_2darray[:, 2]
+
+                else:
+                    # Error Handling if the target and clust data not provided
+                    validate_data_dict(["target", "clust"])
+                    # Error Handling if the target class not provided
+                    if target_class is None:
+                        raise ValueError("The target class is required")
+
+                    # Generate Data
+                    target = data_dict['target']
+                    clust = data_dict['clust']
+
+                    face_labels = majority_class_cluster(target, clust)
+                    edge_labels = closest_class_cluster(target, clust)
+                    target_ind = np.where(target == target_class)[0]
+                    edge_widths = get_edge_widths(target_ind, clust)
+
+                return selected_plot(x, face_labels, edge_labels, edge_widths, **kwargs)
+
+        # ===================== Simple Grid =====================
+        elif plot_type in ['simple_grid']:
+            # Validate the data_dict have the original data
+            validate_data_dict(["original_data"])
+
+            original_data = data_dict['original_data']
+
+            # Check if there're additional variables
+            if use_add_1darray:
+                # Error Handling if the additional 1D arrays and clust not provided
+                validate_data_dict(["cat_1darray", "num_1darray", "clust"])
+
+                cat_feature = data_dict['cat_1darray']
+                num_feature = data_dict['num_1darray']
+                clust = data_dict['clust']
+
+                # ================================
+                # Extract avg from num_1darray
+                # potential input of num_1darray
+                # 1. the specific column of the original data
+                # 2. the pre-processes 1-d array with average value for each cluster
+                # ================================
+                # Validate the length of additional 1D array is equal to the number of neuron or length of original data.
+                if len(num_feature) != self.numNeurons and len(num_feature) != len(original_data):
+                    raise ValueError(
+                        "The additional 1D array must have the same length as the clust data or original data.")
+                elif len(num_feature) == self.numNeurons:
+                    avg = num_feature
+                elif len(num_feature) == len(original_data):
+                    avg = get_cluster_avg(num_feature, clust)
+
+                # ===============================
+                # Extract sizes from cat_1darray
+                # potential input of cat_1darray
+                # 1. The specific feature of the original data (e.g. the specific column) <- it'requres target class
+                # 2. The specific feature of the pre-processes 1-d array with magnitude for each cluster (e.g. percentage)
+                # ===============================
+                if len(cat_feature) != self.numNeurons and len(cat_feature) != len(original_data):
+                    raise ValueError(
+                        "The additional 1D array must have the same length as the clust data or original data.")
+
+                elif len(cat_feature) == self.numNeurons:
+                    sizes = cat_feature
+
+                elif len(cat_feature) == len(original_data):
+                    if target_class is None:
+                        raise ValueError("The target class is required")
+                    sizes = get_perc_cluster(cat_feature, target_class, clust)
+
+            else:
+                # Error Handling if the target and clust data not provided
+                validate_data_dict(["clust", "target"])
+
+                if ind is None:
+                    raise ValueError("The indices is required for this plot type.")
+
+                if target_class is None:
+                    raise ValueError("The target class is required")
+
+                clust = data_dict['clust']
+
+                # Extract avg from the original data
+                num_feature = original_data[:, ind]
+                avg = get_cluster_avg(num_feature, clust)
+
+                # Extract size from the target
+                target = data_dict['target']
+                sizes = get_perc_cluster(target, target_class, clust)
+
+            return selected_plot(avg, sizes, **kwargs)
+
+        # ===================== Basic Plot Family =====================
+        elif plot_type in ['stem', 'pie']:
+            # Error Handling if the clust data not provided
+            validate_data_dict(["target", "clust"])
+
+            # Extract Information
+            clust = data_dict['clust']
+
+            # If the user wanna plot input data
+            if use_add_2darray:
+                # Error Handling if the additional 2D array not provided
+                validate_data_dict(["cat_2darray"])
+
+                # Error Handling if additional vategorical variable has correct length
+                if len(data_dict["cat_2darray"]) != len(clust):
+                    raise ValueError("The additional categorical data must have the same length as the clust data.")
+
+                #  Get Additional Data
+                sizes = data_dict['cat_2darray']
+
+            else:
+                target = data_dict['target']
+                sizes = count_classes_in_cluster(target, clust)
+
+            if plot_type == 'pie':
+
+                # =============================================
+                # It needs to handle scale (need to implement)
+                # =============================================
+
+                # Call the pie plot
+                return selected_plot(sizes, **kwargs)
+
+            elif plot_type == 'stem':
+                # Extract Align
+                if use_add_1darray:
+                    align = [i for i in range(sizes.shape[1])]
+                else:
+                    align = [i for i in range(len(np.unique(target)))]
+                # Call the stem plot
+                return selected_plot(align, sizes, **kwargs)
+
+        elif plot_type in ['hist']:
+            # Error Handling if the index not provided
+            if ind is None:
+                raise ValueError("The indices is required for this plot type.")
+
+            # Error Handling if the original data not provided
+            validate_data_dict(["original_data", "clust"])
+
+            # Extract the feature from the original data
+            clust = data_dict['clust']
+            feature = data_dict['original_data'][:, ind]
+
+            x = get_cluster_array(feature, clust)
+
+            return selected_plot(x, **kwargs)
+
+        elif plot_type in ['scatter']:
+            # Error Handling if the index not provided
+            if ind is None:
+                raise ValueError("The indices is required for this plot type.")
+
+            if len(ind) != 2:
+                raise ValueError("The indices must contain exactly two elements. Eg. [0, 1]")
+
+            # Error Handling if the original data and clust not provided
+            validate_data_dict(["original_data", "clust"])
+
+            # Extract the feature from the original data
+            x = data_dict['original_data'][:, ind[0]]
+            y = data_dict['original_data'][:, ind[1]]
+            clust = data_dict['clust']
+            x = get_cluster_array(x, clust)
+            y = get_cluster_array(y, clust)
+
+            # Call the scatter plot function
+            return selected_plot(x, y, **kwargs)
+
+        elif plot_type in ['box', 'violin']:
+            # Error Handling if the original data not provided
+            validate_data_dict(["original_data", "clust"])
+
+            # Extract the feature from the original data
+            clust = data_dict['clust']
+
+            if ind is None:  # Extract All data
+                data = data_dict['original_data']
+                x = get_cluster_data(data, clust)
+            elif isinstance(ind, int):  # index just have 1 index
+                data = data_dict['original_data'][:, ind]
+                x = get_cluster_array(data, clust)
+            elif isinstance(ind, (list, np.ndarray)):  # index have multiple indices
+                data = data_dict['original_data'][:, ind]
+                x = get_cluster_data(data, clust)
+
+            # Call the box plot and violin function
+            return selected_plot(x, **kwargs)
+
     # Interactive Functionality
     def onpick(self, event, hexagons, hexagon_to_neuron, **kwargs):
         """
         Interactive Plot Function
         Args:
             event: event
                 a mouse click event
```

### Comparing `nnsom-1.4.1/src/NNSOM/som.py` & `nnsom-1.4.2/src/NNSOM/som.py`

 * *Files identical despite different names*

### Comparing `nnsom-1.4.1/src/NNSOM/utils.py` & `nnsom-1.4.2/src/NNSOM/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -254,14 +254,39 @@
             cluster_array[i] = feature[cluster_indices]
         else:
             cluster_array[i] = np.array([])  # Store an empty array if the cluster is empty
 
     return cluster_array
 
 
+def get_cluster_avg(feature, clust):
+    """
+    Returns the average value of a feature for each cluster.
+
+    Parameters
+    ----------
+    feature : array-like
+        Feature array.
+    clust : list
+        A list of cluster arrays, each containing indices sorted by distances.
+
+    Returns
+    -------
+    cluster_avg : numpy array
+        A cluster array with the average value of the feature for each cluster.
+    """
+    cluster_array = get_cluster_array(feature, clust)
+    cluster_avg = np.zeros(len(cluster_array))
+    for i in range(len(cluster_array)):
+        if len(cluster_array[i]) > 0:
+            cluster_avg[i] = np.mean(cluster_array[i])
+
+    return cluster_avg
+
+
 def closest_class_cluster(cat_feature, clust):
     """
     Returns the cluster array with the closest class for each cluster.
 
     Paramters
     ----------
     cat_feature : array-like
@@ -572,15 +597,15 @@
         A tuple (min_value, max_value) where min_value is the minimum value
         in the data, and max_value is the maximum value.
     """
     flat_list = flatten(data)
     return min(flat_list), max(flat_list)
 
 
-def get_edge_width(indices, clust):
+def get_edge_widths(indices, clust):
     """ Calculate edge width for each cluster based on the number of indices in the cluster.
 
     Args:
         indices: 1-d array
             Array of indices for the specific class.
         clust: sequence of vectors
             A sequence of vectors, each containing the indices of elements in a cluster.
@@ -600,42 +625,66 @@
                 lwidth[i] = None
         else:
             lwidth[i] = None
 
     return lwidth
 
 
-def get_edge_color(clust, *args):
-    """ Calculate edge color for each cluster based on the number of indices in the cluster.
+def get_color_labels(clust, *listOfIndices):
+    """ Generates color label for each cluster based on indices of classes.
 
     Args:
         clust: sequence of vectors
             A sequence of vectors, each containing the indices of elements in a cluster.
 
         *args: 1-d array
             A list of indices where the specific class is present.
     """
+    # Validate if the user have provided at least one class indices
+    if len(listOfIndices) == 0:
+        raise ValueError('At least one class indices must be provided.')
+
+    # Validate if the arg is a list or numpy array and unpack them
+    numst = []
+    for arg in listOfIndices:
+        if not isinstance(arg, (list, np.ndarray)):
+            raise ValueError('The arguments must be a list or numpy array.')
+        else:
+            numst.append(arg)
 
-    # unpack the args
-    numst = list(args)
+            # Initialize the color label array
+    color_labels = np.zeros(len(clust))
 
-    # Initialize the edge color array
-    edge_color = np.zeros(len(clust))
+    # When there is only one list provides,
+    # check if the cluster contains the indices of the class.
+    # If that class is majority in the cluster, assign 1, otherwise 0.
+    if len(numst) == 1:
+        indices = numst[0]
+        for i in range(len(clust)):
+            if len(clust[i]) != 0:
+                num_class = len(np.intersect1d(clust[i], indices))
+                if num_class > len(clust[i]) / 2:
+                    color_labels[i] = 1
+                else:
+                    color_labels[i] = 0
+            else:
+                color_labels[i] = None
 
-    # Detect the intersection of the cluster and each list of indices (class),
-    # and get the majority class in the cluster.
-    # Append the majority class to the edge color array.
-    for i in range(len(clust)):
-        if len(clust[i]) != 0:
-            intersection = [len(np.intersect1d(clust[i], numst[j])) for j in range(len(numst))]
-            edge_color[i] = np.argmax(intersection)
-        else:
-            edge_color[i] = None
+    else:
+        # Detect the intersection of the cluster and each list of indices (class),
+        # and get the majority class in the cluster.
+        # Append the majority class to the edge color array.
+        for i in range(len(clust)):
+            if len(clust[i]) != 0:
+                intersection = [len(np.intersect1d(clust[i], numst[j])) for j in range(len(numst))]
+                color_labels[i] = np.argmax(intersection)
+            else:
+                color_labels[i] = None
 
-    return edge_color
+    return color_labels
 
 
 # Helper functions to create button objects in the interactive plot
 def create_buttons(fig, button_types):
     sidebar_width = 0.2
     button_config = calculate_button_positions(len(button_types), sidebar_width)
```

### Comparing `nnsom-1.4.1/.gitignore` & `nnsom-1.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `nnsom-1.4.1/pyproject.toml` & `nnsom-1.4.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 include = ["src/NNSOM/*.py"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/NNSOM"]
 
 [project]
 name = "NNSOM"
-version = "1.4.1"
+version = "1.4.2"
 description = "A SOM package"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 authors = [
   { name = "Dr. Hagan" },
   { name = "Dr. Amir Jafari", email = "amir.h.jafari@okstate.edu" },
```

### Comparing `nnsom-1.4.1/PKG-INFO` & `nnsom-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: NNSOM
-Version: 1.4.1
+Version: 1.4.2
 Summary: A SOM package
 Project-URL: Repository, https://github.com/amir-jafari/SOM
 Project-URL: Issues, https://github.com/amir-jafari/SOM/issues
 Author: Dr. Hagan, Lakshmi Sravya Chalapati, Ei Tanaka
 Author-email: "Dr. Amir Jafari" <amir.h.jafari@okstate.edu>
 Maintainer-email: "Dr. Amir Jafari" <amir.h.jafari@okstate.edu>
 License-File: LICENSE
```

