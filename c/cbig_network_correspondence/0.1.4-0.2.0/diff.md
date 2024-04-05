# Comparing `tmp/cbig_network_correspondence-0.1.4.tar.gz` & `tmp/cbig_network_correspondence-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbig_network_correspondence-0.1.4.tar", max compression
+gzip compressed data, was "cbig_network_correspondence-0.2.0.tar", max compression
```

## Comparing `cbig_network_correspondence-0.1.4.tar` & `cbig_network_correspondence-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1097 2024-03-30 10:03:04.788386 cbig_network_correspondence-0.1.4/LICENCE
--rw-r--r--   0        0        0    16956 2024-03-30 10:03:04.788386 cbig_network_correspondence-0.1.4/README.md
--rw-r--r--   0        0        0     2406 2024-03-30 10:03:04.788386 cbig_network_correspondence-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1433 2024-03-30 10:03:04.788386 cbig_network_correspondence-0.1.4/src/cbig_network_correspondence/__init__.py
--rw-r--r--   0        0        0    30806 2024-03-30 10:03:04.788386 cbig_network_correspondence-0.1.4/src/cbig_network_correspondence/compute_overlap_with_atlases.py
--rw-r--r--   0        0        0     3176 2024-03-30 10:03:04.788386 cbig_network_correspondence-0.1.4/src/cbig_network_correspondence/grab_data_info.py
--rw-r--r--   0        0        0      429 2024-03-30 10:03:04.788386 cbig_network_correspondence-0.1.4/src/cbig_network_correspondence/load_example.py
--rw-r--r--   0        0        0        0 2024-03-30 10:03:04.788386 cbig_network_correspondence-0.1.4/src/cbig_network_correspondence/py.typed
--rw-r--r--   0        0        0    14090 2024-03-30 10:03:04.788386 cbig_network_correspondence-0.1.4/src/cbig_network_correspondence/visualize_overlap_lib.py
--rw-r--r--   0        0        0    23061 2024-03-30 10:03:04.792387 cbig_network_correspondence-0.1.4/src/cbig_network_correspondence/visualize_report_lib.py
--rw-r--r--   0        0        0    18511 1970-01-01 00:00:00.000000 cbig_network_correspondence-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1097 2024-04-05 09:11:48.853965 cbig_network_correspondence-0.2.0/LICENCE
+-rw-r--r--   0        0        0    17155 2024-04-05 09:11:48.853965 cbig_network_correspondence-0.2.0/README.md
+-rw-r--r--   0        0        0     2406 2024-04-05 09:11:48.869965 cbig_network_correspondence-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1433 2024-04-05 09:11:48.869965 cbig_network_correspondence-0.2.0/src/cbig_network_correspondence/__init__.py
+-rw-r--r--   0        0        0    30655 2024-04-05 09:11:48.869965 cbig_network_correspondence-0.2.0/src/cbig_network_correspondence/compute_overlap_with_atlases.py
+-rw-r--r--   0        0        0     3176 2024-04-05 09:11:48.869965 cbig_network_correspondence-0.2.0/src/cbig_network_correspondence/grab_data_info.py
+-rw-r--r--   0        0        0      429 2024-04-05 09:11:48.869965 cbig_network_correspondence-0.2.0/src/cbig_network_correspondence/load_example.py
+-rw-r--r--   0        0        0        0 2024-04-05 09:11:48.869965 cbig_network_correspondence-0.2.0/src/cbig_network_correspondence/py.typed
+-rw-r--r--   0        0        0    14090 2024-04-05 09:11:48.869965 cbig_network_correspondence-0.2.0/src/cbig_network_correspondence/visualize_overlap_lib.py
+-rw-r--r--   0        0        0    23371 2024-04-05 09:11:48.869965 cbig_network_correspondence-0.2.0/src/cbig_network_correspondence/visualize_report_lib.py
+-rw-r--r--   0        0        0    18710 1970-01-01 00:00:00.000000 cbig_network_correspondence-0.2.0/PKG-INFO
```

### Comparing `cbig_network_correspondence-0.1.4/LICENCE` & `cbig_network_correspondence-0.2.0/LICENCE`

 * *Files identical despite different names*

### Comparing `cbig_network_correspondence-0.1.4/README.md` & `cbig_network_correspondence-0.2.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,44 @@
+Metadata-Version: 2.1
+Name: cbig_network_correspondence
+Version: 0.2.0
+Summary: A toolbox for exploring network correspondence across atlases
+Home-page: https://rubykong.github.io/cbig_network_correspondence
+License: MIT
+Author: Ruby Kong
+Author-email: roo.cone@gmail.com
+Requires-Python: >=3.8.1,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Typing :: Typed
+Requires-Dist: brainspace (>=0.1.10,<0.2.0)
+Requires-Dist: colorcet (>=3.0.1,<4.0.0)
+Requires-Dist: gitpython (>=3.1.27,<4.0.0)
+Requires-Dist: natsort (>=8.3.1,<9.0.0)
+Requires-Dist: nibabel (>=5.0.1,<6.0.0)
+Requires-Dist: numpy (>=1.20.3,<2.0.0)
+Requires-Dist: pandas (>=1.3.2,<2.0.0)
+Requires-Dist: plottable (>=0.1.5,<0.2.0)
+Requires-Dist: regfusion (>=0.1.0,<0.2.0)
+Requires-Dist: scipy (>=1.9.0,<2.0.0)
+Requires-Dist: seaborn (>=0.11.2,<0.12.0)
+Project-URL: Repository, https://github.com/rubykong/cbig_network_correspondence
+Description-Content-Type: text/markdown
+
 # cbig_network_correspondence
 
 [![PyPI](https://img.shields.io/pypi/v/cbig_network_correspondence?style=flat-square)](https://pypi.python.org/pypi/cbig_network_correspondence/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/cbig_network_correspondence?style=flat-square)](https://pypi.python.org/pypi/cbig_network_correspondence/)
 [![PyPI - License](https://img.shields.io/pypi/l/cbig_network_correspondence?style=flat-square)](https://pypi.python.org/pypi/cbig_network_correspondence/)
 [![Coookiecutter - Wolt](https://img.shields.io/badge/cookiecutter-Wolt-00c2e8?style=flat-square&logo=cookiecutter&logoColor=D4AA00&link=https://github.com/woltapp/wolt-python-package-cookiecutter)](https://github.com/woltapp/wolt-python-package-cookiecutter)
 
@@ -16,309 +53,248 @@
 
 ---
 
 This toolbox was used to explore the network correspondence between networks across different atlases. 
 
 ## Installation
 
+To install:
+
 ```sh
 pip install cbig_network_correspondence
 ```
 
-## Usage
+To upgrade:
+
+```sh
+pip install --upgrade cbig_network_correspondence
+```
 
-This toolbox has the following functions:
 
-+ Compute and visualize network overlap between two existing alases
-+ Compute and visualize overlap between any metric data (e.g. task contrast map, probability map, other atlas) and an existing atlas
-+ Visualze the overlapping area between two atlases or a metric data and an atlas
+## Usage
 
-We will provide detailed usage of these function in the following sections.
+### Tutorial
+
+We provide a tutorial for how to use this toolbox. The tutorial is available in the Usage.ipynb notebook:
++ [`Usage.ipynb](https://github.com/rubykong/cbig_network_correspondence/blob/master/Usage.ipynb)
 
 ### Atlases we included
 
 Check this list for the atlases we have included. We use abbreviations for the atlases. Here we provide the decription for each atlas. If you want us to include your atlas, please contact me (roo.cone@gmail.com).
 
-![networkcorrespondence](https://github.com/rubykong/cbig_network_correspondence_data/assets/20438248/b430f2fe-4b78-49f2-9084-5a43d450dba1)
+| Abbreviation | Source                         | Description                                            |
+|--------------|--------------------------------|--------------------------------------------------------|
+| MG360J12     | Glasser2016; Ji2019            | Mattew Glasser2016 360-ROI with Ji2019 12 Cole-Anticevic networks |
+| HCPICA       | Smith2009; Smith2013           | HCP 25-node ICA maps                                   |
+| AL20         | Laird2011                      | Angela Laird2011 20-node ICA maps                      |
+| AS200K17     | Schaefer2018; Kong2021         | Alex Schaefer2018 200-ROI with Kong2021 17 networks    |
+| AS200Y17     | Schaefer2018; Yeo2011          | Alex Schaefer2018 200-ROI with Yeo2011 17 networks     |
+| AS400K17     | Schaefer2018; Kong2021         | Alex Schaefer2018 400-ROI with Kong2021 17 networks    |
+| AS400Y17     | Schaefer2018; Yeo2011          | Alex Schaefer2018 400-ROI with Yeo2011 17 networks     |
+| XS268_8      | Shen2013                       | Xilin Shen2013 268-ROI with 8 networks                 |
+| XS368_8      | Shen2013                       | Xilin Shen2013 368-ROI with 8 networks                 |
+| WS90_14      | Shirer2012                     | William Shirer2012 90-ROI 14 networks                  |
+| UKBICA       | Smith2009; Alfaro-Almagro2018  | UKBiobank 25-node ICA maps                             |
+| EG286_12     | Power2011; Gordon2016          | Evan Gordon2016 286-ROI with 12 networks               |
+| TL12         | Power2011; Laumann2015         | Tim Laumann2015 12 networks (Power2011)                |
+| EG17         | Power2011; Gordon2017          | Evan Gordon2017 17 networks                            |
+| TY7          | Yeo2011                        | Thomas Yeo 7 networks                                  |
+| TY17         | Yeo2011                        | Thomas Yeo 17 networks                                 |
+| XY200K17     | Yan2023; Kong2021              | Xiaoxuan Yan2023 200-ROI with Kong2021 17 networks     |
+| XY200Y17     | Yan2023; Yeo2011               | Xiaoxuan Yan2023 200-ROI with Yeo2011 17 networks      |
+| XY400K17     | Yan2023; Kong2021              | Xiaoxuan Yan2023 400-ROI with Kong2021 17 networks     |
+| XY400Y17     | Yan2023; Yeo2011               | Xiaoxuan Yan2023 400-ROI with Yeo2011 17 networks      |
+
 
 These atlases should be automatically downloaded when you install the toolbox. If you want to download the atlases manually, you can find the atlases here: https://github.com/rubykong/cbig_network_correspondence_data. The atlas data will be automatically downloaded in your python package directory: `cbig_network_correspondence/src/cbig_network_correspondence/data`.
 
-### Config file
 
-In this toolbox, the information for each atlas was constructed as config file. We have included the config files for each atlas. The config files will be automatically downloaded when you install the toolbox. If you want to check the config files manually, you can find the config files in your python package directory: `cbig_network_correspondence/src/cbig_network_correspondence/data/atlas_config`. If you want to use your own atlas, you can create your own config file, check next sections for details. 
+### Input data
+
+The toolbox can also explore the network correspondence of your own input data. The input data can be different format. We support input data in fs_LR_32k, fsaverage6, and FSLMNI2mm.
+
+#### Format
+
+Here are the formats we support:
+
+For data in fs_LR_32k or fsaverage6 space:
+
++ `.mat` file: The file should contain two variables starting with `lh` and `rh`. For example, the variable names could be `lh_data`, `rh_data` or `lh_labels`, `rh_labels`. Each variable should be a 32492x1 vector for `fs_LR_32k` space or a 40962x1 vector for `fsaverage6` space. 
+
++ `.npy` file: The file should contain a numpy array with shape (64984, 1) for `fs_LR_32k` space or (81924, 1) for `fsaverage6` space.
+
+For data in FSLMNI2mm space:
+
++ `.nii` or `.nii.gz` file: The file should be a nifti file with the same dimension as the FSL MNI152 2mm template.
+
+
+#### Pass in the data as ...
+
++ A single path to a single file
+  - `/data_dir/my_task_contrast_map.mat`
+  - `/data_dir/my_task_contrast_map.npy`
+  - `/data_dir/my_task_contrast_map.nii.gz`
+
++ A list of paths to multiple files
+  - `['/data_dir/my_task_contrast_map1.mat', '/data_dir/my_task_contrast_map2.mat']`
+  - `['/data_dir/my_task_contrast_map1.npy', '/data_dir/my_task_contrast_map2.npy']`
+  - `['/data_dir/my_task_contrast_map1.nii.gz', '/data_dir/my_task_contrast_map2.nii.gz']`
+
++ A directory contains the input files
+  - `/data_dir`
+  under this directory, the toolbox will search for the files containing the `Data_Name` in the config file (see the Config file section for more details). For example, if the `Data_Name` is `my_task_contrast_map`, the toolbox will search for the files containing `my_task_contrast_map` in the file name
+
++ A string indicating the name of a existing atlas
+  - `AS400Y17`
+  - `EG17`
+  - `TY17`
+
+#### Reference data space
+
+To explore the network correspondence between a given input data and existing atlases, the toolbox will use the input data as the reference data. The toolbox will use existing atlases in the same space as the input data. For example, if the input data is in `fs_LR_32k` space, the toolbox will use the existing atlases in `fs_LR_32k` space. If the input data is in `FSLMNI2mm` space, the toolbox will use the existing atlases in `FSLMNI2mm` space. 
+
+#### Reference data names
+
+User can specify the name for the given input data, if not, the toolbox will use the `Data_Name` in the config file as the reference data name. 
+
+Reference data names could be important for a multi-dimension input data. For example, if the input data is a set of task contrast maps, the user might want to specify the reference data names for each task contrast map. Otherwise, the toolbox will name each task contrast map as `<Data_Name>1`, `<Data_Name>2`, etc. 
+
+If the input data is the user's own atlas with K networks, the user should specify the reference data names for each network. Otherwise the toolbox will name each network as `<Data_Name>1`, `<Data_Name>2`, etc.
+
+#### Config file
+
+In this toolbox, the information for each atlas or input data is constructed as a config file. We have included the config files for existing atlases. The config files will be automatically downloaded when you install the toolbox. If you want to check the config files manually, you can find the config files in your python package directory: `cbig_network_correspondence/src/cbig_network_correspondence/data/atlas_config`. If you want to explore network correspondence of your own input data/atlas, you can create your own config file, check next sections for how to create a config file. 
 
 The config file should be a text file. 
 
 Here is an example of the config file for the Schaefer 400-ROI atlas with Yeo 17-network network assignemnt `AS400Y17`:
 ```
 [data_info]
 Data_Category: YeoLab
 Data_Name: AS400Y17
 Data_Space: fsaverage6
 Data_Type: Hard
 Data_NetworkAssignment: 1
 ```
 
-Here is an example of the config file for a example metric data `Exemplar1(pos)`:
+Here is an example of the config file for a example metric data `Example`:
 ```
 [data_info]
-Data_Name: Exemplar1(pos)
+Data_Name: Example
 Data_Space: FSLMNI2mm
 Data_Type: Metric
 Data_Threshold: [5,Inf]
 ```
 
 Here is the decription for the config file:
 
 + `Data_Category` [optional]
   
   We included it for existing atlases because some atlases were from the same lab. In this case, we put the some atlases into the same category. This is not necessary for your own atlas or your own metric data.
    
 + `Data_Name`
 
-  The name of the atlas or metric data.
+  The name of the atlas or metric data. If the input data is a set of files instead of a single file, user can pass in the directory to the files. The toolbox will search for the files containing the `Data_Name` in the file name. For example, if the `Data_Name` is `my_task_contrast_map`, the toolbox will search for the files containing `my_task_contrast_map` in the file name.
 
 + `Data_Space`
 
-  The space name of the space where the atlas/data is in. It can be a surface name or a volumetric space name. We currenly have atlases in the following spaces: `fs_LR_32k` surface space, `fsaverage6` surface space, `FSLMNI2mm` volumetric space, `LairdColin2mm` volumetric space, `ShenColin1mm` volumetric space.
+  The space name of the space where the atlas/data is in. It can be a surface name or a volumetric space name. We currenly have atlases in the following spaces: `fs_LR_32k` surface space, `fsaverage6` surface space, `FSLMNI2mm` volumetric space, `LairdColin2mm` volumetric space, `ShenColin1mm` volumetric space. If the user wants to explore the network correspondence of their own data, the data should be in `fs_LR_32k`, `fsaverage6`, or `FSLMNI2mm` space.
   
 + `Data_Type`
 
   The type of the atlas/data. We have two types of atlas: `Hard` and `Soft`. The `Hard` atlas is the atlas that each ROI is assigned to a specific network. The `Soft` atlas is the atlas that each ROI is assigned to a probability of belonging to each network. We also allow for a metric data such as task contrast maps or probability maps, in this case `Data_Type` should be `Metric`. 
 
 + `Data_NetworkAssignment` [optional]
 
   Sometimes the atlas has fine-grained ROIs and these ROIs were assigned to large-scale networks. For example, the Schaefer2018 400 ROIs were assigned to the Yeo 17-network atlas. In this case the user can provide a mapping between ROIs to networks, here you can find the mapping for some of the existing atlases: https://github.com/rubykong/cbig_network_correspondence_data/tree/master/network_assignment
 
 + `Data_Threshold` [optional]
 
   For soft parcellation and metric data, we will need to apply a threshold to binarize the data. The threshold should be set as `[lower bound, upper bound]`. If the upper bound is `Inf`, then the threshold will be applied as `>= lower bound`. If the lower bound is `-Inf`, then the threshold will be applied as `<= upper bound`. If the `Data_Type` is `Soft` or `Metric`, but the `Data_Threshold` is not provided, the toolbox will use a default threshold `[0, Inf]`. `Data_Threshold` is not necessary for `Hard` atlas.
 
-After importing the toolbox, here are the relevant commands. After decribing the commands, we provide examples for how to use this toolbox. We also provided a jupyter notebook for the examples: ExampleUsage.ipynb. Please note that the output figure path were hard-coded in the notebook, so you might need to change the output figure path to your own path.
+After importing the toolbox, here are the relevant commands. After decribing the commands, we provide examples for how to use this toolbox. We also provided a jupyter notebook for the usage examples: Usage.ipynb. 
 
-```python
-import cbig_network_correspondence as cnc
-```
-
-```
-overlap_mat = cnc.compute_overlap_with_atlases.load_overlap_atlases(ref_atlas_name, other_atlas_name)
 
-This function will load the pre-computed network overlap matrix between the reference atlas and the other atlas.
+### Usage scenarios
 
-Input:
-- ref_atlas_name: the name of the reference atlas
-- other_atlas_name: the name of the other atlas
+This toolbox has two main usage scenarios:
 
-Output:
-- overlap_mat: the network overlap matrix between the reference atlas and the other atlas
-```
-
-```
-cnc.visualize_overlap_lib.draw_overlap_mat(overlap_mat, ref_atlas_name, other_atlas_name, minv, maxv, outputfigfile)
+1. Use this toolbox to explore network correspondence between existing atlases.
+2. Provide users' own input data, and explore the network correspondence between the input data and existing atlases.
 
-This function will draw the network overlap matrix between the reference atlas and the other atlas. In this function, the user can pass in the loaded overlap matrix from cnc.compute_overlap_with_atlases.load_overlap_atlases.
+**We have provided detailed examples for each usage scenario in the Usage.ipynb notebook. Here we provide brief descriptions for inputs.**
 
-Input:
-- overlap_mat: the network overlap matrix between the reference atlas and the other atlas
-- ref_atlas_name: the name of the reference atlas
-- other_atlas_name: the name of the other atlas
-- minv: the minimum value of the colorbar
-- maxv: the maximum value of the colorbar
-- outputfigfile: the output figure file name
+#### 1. Explore network correspondence between existing atlases
 
-```
-```
-cnc.visualize_overlap_lib.draw_overlap_atlases(ref_atlas_name, other_atlas_name, minv, maxv, outputfigfile)
-
-This function will draw the network overlap matrix between the reference atlas and the other atlas. This function will automatically load the pre-computed network overlap matrix between the reference atlas and the other atlas.
-
-Input:
-- ref_atlas_name: the name of the reference atlas
-- other_atlas_name: the name of the other atlas
-- minv: the minimum value of the colorbar
-- maxv: the maximum value of the colorbar
-- outputfigfile: the output figure file name
-```
-
-```
-overlap_data = cnc.compute_overlap_with_atlases.obtain_overlap_atlases(ref_atlas_name, other_atlas_name, ref_network_name, other_network_name)
-
-This function generate the overlapping area between networks from two atlases. This is used for visualization purpose.
-
-Input:
-- ref_atlas_name: the name of the reference atlas
-- other_atlas_name: the name of the other atlas
-- ref_network_name: the name of the reference network
-- other_network_name: the name of the other network
-
-Note that you can find the network names for each atlas here:
-https://github.com/rubykong/cbig_network_correspondence_data/tree/master/network_names
-
-Output:
-- overlap_data: a numpy array in the same space as the reference atlas. The array contains three labels: 1, 2, 3.
-1 indicates the reference network, 2 indicates the other network, 3 indicates the overlapping area between the two networks.
-```
+![NCT_workflow1](https://github.com/rubykong/cbig_network_correspondence/assets/20438248/5046486c-b192-4aa4-90e4-825d962fc94c)
 
 ```
-cnc.visualize_overlap_lib.draw_overlap_map(data_space, overlap_data, outputfigfile, coords)
-
-This function visualize the overlapping area between networks from two atlases. The reference network will be colored in pink, the other network will be colored in blue, and the overlapping area will be colored in purple.
-
-Input:
-- data_space: the space of the data. It can be `fsaverage6`, `fs_LR_32k`, `FSLMNI2mm`, `LairdColin2mm`, `ShenColin1mm`
-- overlap_data: a numpy array in the same space as the reference atlas. The array contains three labels: 1, 2, 3. This is the output of cnc.compute_overlap_with_atlases.obtain_overlap_atlases
-- outputfigfile: the output figure file name
-- coords: [for volumetric data only] the coordinates of the point where the cut is performed. BY default, we use [-4, -31, 18].
-```
-
-
-```
-example = cnc.load_example
-
-This function find the path to the example config and example nifti image
-
-Output:
-- example_config: the path to the example config file
-- example_nii: the path to the example nifti image
-```
-
-```
-data_params = cnc.compute_overlap_with_atlases.DataParams(config_file, data_path)
-
-This function reads in the config information and the data path to construct the parameters for the data
-
-Input:
-- config_file: the path to the config file
-- data_path: the path to the data
-```
-
-```
-overlap_data = cnc.compute_overlap_with_atlases.obtain_overlap_data(data_params, atlas_name, network_name)
-
-This function generate the overlapping area between the binarized data and an existing atlas. This is used for visualization purpose. The calculation is done in the same space as the data.
-
-Input:
-- data_params: the parameters for the data. This is the output of the function cnc.compute_overlap_with_atlases.DataParams
-- atlas_name: the name of the atlas. For example, "MG360J12".
-- network_name: the name of the network from the atlas. For example, "Default".
-
-```
-
-### Compute and visualize network overlap between two existing alases
-
-In this toolbox, we computes the network overlap between any pair of existing atlases. We treat each atlas as the reference atlas, and projected other atlases to the same space as the reference atlas. Then we compute the network overlap between the reference atlas and the projected atlas.
-
-Here we provide examples if you want to check the network overlap matrix between the Glasser 2016 atlas with Ji2019 networks and the Yeo 17 networks, you can use the following code:
-
-```python
-import  cbig_network_correspondence as cnc
-
-# When Yeo 17-network atlas is the reference atlas, the Glasser2016 atlas will be projected to fsaverage6 surface space
-overlap_mat1 = cnc.compute_overlap_with_atlases.load_overlap_atlases("TY17", "MG360J12")
-
-# When Glasser2016 atlas atlas is the reference atlas, theYeo 17-network atlas will be projected to fs_LR_32k surface space
-overlap_mat2 = cnc.compute_overlap_with_atlases.load_overlap_atlases("MG360J12", "TY17")
-```
-
-If you want to visualize the network overlap matrix, you can use the following code:
+import cbig_network_correspondence as cnc
 
-```python
-cnc.visualize_overlap_lib.draw_overlap_mat(overlap_mat1, "TY17", "MG360J12", 0, 1, "<path_to_figure>/TY17_MG360J12")
-cnc.visualize_overlap_lib.draw_overlap_mat(overlap_mat2, "MG360J12", "TY17", 0, 1, "<path_to_figure>/MG360J12_TY17")
+cnc.compute_overlap_with_atlases.network_correspondence(reference_atlas, atlas_names_list, output_dir)
 ```
 
-The output figures will be save under the path `<path_to_figure>/TY17_MG360J12.png` and `<path_to_figure>/MG360J12_TY17.png`. Here are the corresponding figures. The left side are reference network names, the upper part are the other atlas network names
-
-+ `<path_to_figure>/TY17_MG360J12.png` 
-
-![image](https://user-images.githubusercontent.com/20438248/232752322-0fbe141f-3879-4c6d-9a04-1dd372753ea0.png)
++ `reference_atlas`: str
+  - The name of the reference atlas. The reference atlas should be one of the existing atlases. The toolbox will use the reference atlas to explore the network correspondence between the reference atlas and other atlases in the `atlas_names_list`.
++ `atlas_names_list`: list
+  - A list of the names of the atlases. The toolbox will explore the network correspondence between the reference atlas and the atlases in the `atlas_names_list`.
++ `output_dir`: str
+  - The directory to save the output figures and csv files.
 
-+ `<path_to_figure>/MG360J12_TY17.png`
+Note: network name should be the abbreviation of the atlas. For example, `AS400Y17` for the Schaefer 400-ROI atlas with Yeo 17-network network assignemnt.
 
-![image](https://user-images.githubusercontent.com/20438248/232752400-a162a152-043f-48e9-b45d-171bfea6b952.png)
+#### 2. Explore network correspondence between input data and existing atlases
 
+![NCT_workflow2](https://github.com/rubykong/cbig_network_correspondence/assets/20438248/55f9f944-246d-4146-b530-978b7e951ddd)
 
-However, if you have no interest to check the overlap matrix and just want to see the visualized network overlap between two atlases, you can use the following code:
-
-```python
-import  cbig_network_correspondence as cnc
-
-cnc.visualize_overlap_lib.draw_overlap_atlases("MG360J12", "TY17", 0, 1, "<path_to_figure>/MG360J12_TY17")
 ```
+import cbig_network_correspondence as cnc
 
-If you want to check the brain maps of the overlappping regions between two atlases, you can use the following code:
-
-+ To check the overlapping regions between the `Default` network from `MG360J12` atlas and the `DefaultA` network from `TY17` atlas:
-
-```python
-import  cbig_network_correspondence as cnc
-
-# When Yeo 17-network atlas is the reference atlas
-overlap_data = cnc.compute_overlap_with_atlases.obtain_overlap_atlases("TY17", "MG360J12", "DefaultA", "Default")
-# Yeo 17-network atlas is in fsaverage6 surface space
-cnc.visualize_overlap_lib.draw_overlap_map("fsaverage6", overlap_data, "<path_to_figures>/TY17_MG360J12_DefaultA_Default")
+# construct DataParams object based on the data file path and config
+ref_params = cnc.compute_overlap_with_atlases.DataParams(config, file_path)
 
-# When Glasser2016 atlas atlas is the reference atlas
-overlap_data = cnc.compute_overlap_with_atlases.obtain_overlap_atlases("MG360J12", "TY17", "Default", "DefaultA")
-# Glasser2016 atlas is in fs_LR_32k surface space
-cnc.visualize_overlap_lib.draw_overlap_map("fs_LR_32k", overlap_data, "<path_to_figures>/MG360J12_TY17_Default_DefaultA")
+# compute the overlap with atlases and save the results
+cnc.compute_overlap_with_atlases.network_correspondence(ref_params, atlas_names_list,output_dir,ref_data_names)
 
 ```
 
-Here are the results:
-![Overlap_surface](https://user-images.githubusercontent.com/20438248/232758349-ad5157cd-d6c2-4d4c-880c-7dda3a36fe0b.jpg)
++ `config`: str
+  - The path to the config file for the input data.
++ `file_path`: str/list
+  - The path to a single input data file
+  - A list of paths to multiple input data files
+  - A directory contains the input data files
++ `atlas_names_list`: list
+  - A list of the names of the atlases. The toolbox will explore the network correspondence between the input data and the atlases in the `atlas_names_list`.
++ `output_dir`: str
+  - The directory to save the output figures and csv files.
++ `ref_data_names`: str/list
+  - The name of the input data. If `ref_data_names` is not provided, the toolbox will use the `Data_Name` in the config file as the reference data name. If the input data is multi-dimension, each dimension will be named as `<Data_Name>1`, `<Data_Name>2`,... if the `ref_data_names` is not provided.
 
 
-### Compute and visualize overlap between any metric data and an existing atlas
+### Significance test
 
-In this toolbox, we also allow users to upload their own data and compute the network overlap between the data and an existing atlas. We treat the data as the reference, and projected the atlas to the same space as the reference data. For a metric data, we binarize the data use `Data_Threshold`, then we compute the network overlap between the binarized data and the projected atlas. Here we provide an example data to show you how to use this toolbox.
+The toolbox provides a significance test to test the significance of the network correspondence between the given input data and an existing atlas. The toolbox will use the spin-test (Gordon2017;Alexander-Bloch2018)to test the significance of the network correspondence. Specically, SpinPermutations from BrainSpace python package is used here. For data in FSLMNI2mm space, we project the data to the fsaverage6 space for the spin-test. 
 
-After importing the toolbox, here are the relevant commands. After decribing the commands, we provide examples for how to use this toolbox to compute and visualize the overlap between any metric data and an existing atlas.
 
-You can load the example data by using the following code:
+### Results
 
-```python
-import  cbig_network_correspondence as cnc
+NCT provides different types of plots to help the user explore/visualize the network correspondences. 
 
-example = cnc.load_example
-# the example config file
-print(example.example_config)
-# the path to the example data
-print(example.example_nii)
-# construct parameters for example data
-data_params = cnc.compute_overlap_with_atlases.DataParams(example.example_config, example.example_nii)
-```
-
-In this example, we will compute the overlap between thie example data and the Glasser2016 atlas. Since the example data is in FSLMNI2mm space, we will project the Glasser2016 atlas to FSLMNI2mm space and compute the overlap matrix.
-
-```python
-overlap_mat = cnc.compute_overlap_with_atlases.compute_overlap_data(data_params, "MG360J12")
-```
-
-After that, we can visualize the overlap matrix by using the following code:
-
-```python
-cnc.visualize_overlap_lib.draw_overlap_mat(overlap_mat, "Exampler1(pos)", "MG360J12", 0, 1, "<path_to_figures>/exampler1_pos_MG360J12")
-```
-
-Here is how the overlap matrix looks like:
-![image](https://user-images.githubusercontent.com/20438248/232759475-2eae4dad-0f7c-40d0-afe3-bd4731466542.png)
-
-Based on the visualized overlap matrix, we can notice that the example data overlapped the most with the `Default` network from Glasser2016. If we want to check the overlapping regions between the example data and the `Default` network from Glasser2016, we can use the following code:
++ Overlap Heatmap
+  - If input data has multiple dimensions, e.g., a atlas with K networks, a set of task contrast maps. For a specified list of existing atlases, the toolbox will provide heatmaps to show the overlap between the input data and the existing atlases. Each atlas will have a heatmap. If input data has K dimension, and the other atlas has N networks, the heatmap will be a KxN heatmap. Each row represents the overlap between the input data and an existing atlas. Each column represents the overlap between the input data and a network in the existing atlas. The color represents the overlap value. The asterisk indicates the significance of the overlap. 
 
-```python
-overlap_data = cnc.compute_overlap_with_atlases.obtain_overlap_data(data_params, 'MG360J12', 'Default')
-# By default we use coords=[-4, -31, 18] to visualize volumetric data, you can change it to any other coordinates
-cnc.visualize_overlap_lib.draw_overlap_map("FSLMNI2mm", overlap_data, "<path_to_figures>/example_MG360J12_Default", [-4, -31, 18])
-```
-
-Here is the result:
-![image](https://user-images.githubusercontent.com/20438248/232760522-f1327b70-2bc7-4b74-bdf2-30274146bfa6.png)
++ Network Clock
+  - If input data is single dimension, e.g., a task contrast map, a probability map. For a specified list of existing atlases, the toolbox will provide a network clock to show the overlap between the input data and the existing atlases. The network clock will show the overlap between the input data and all networks. Networks from the same atlas are grouped together and colored by the same color. Only the networks with significant overlap will be indicated by network name in the network clock. The clock ring represents the overlap value. The network font size represents the overlap value. 
 
++ Network Radar
+  - If input data is single dimension, e.g., a task contrast map, a probability map. For a specified list of existing atlases, the toolbox will provide a network radar to show the overlap between the input data and the existing atlases. Each atlas will have a radar map. The asterisk indicates the significance of the overlap.
 
++ Summary Table
+  - The toolbox will provide a summary table to show the exact overlap values and p-values of the overlap between the input data and the existing atlases. Summary tables will be saved as figures and csv files.
 
 ## Development
 
 * Clone this repository
 * Requirements:
   * [Poetry](https://python-poetry.org/)
   * Python 3.7+
@@ -333,7 +309,8 @@
 ```sh
 poetry shell
 ```
 
 ---
 
 This project was generated using the [wolt-python-package-cookiecutter](https://github.com/woltapp/wolt-python-package-cookiecutter) template.
+
```

### Comparing `cbig_network_correspondence-0.1.4/pyproject.toml` & `cbig_network_correspondence-0.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cbig_network_correspondence"
-version = "0.1.4"
+version = "0.2.0"
 description = "A toolbox for exploring network correspondence across atlases"
 authors = [
     "Ruby Kong <roo.cone@gmail.com>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `cbig_network_correspondence-0.1.4/src/cbig_network_correspondence/__init__.py` & `cbig_network_correspondence-0.2.0/src/cbig_network_correspondence/__init__.py`

 * *Files identical despite different names*

### Comparing `cbig_network_correspondence-0.1.4/src/cbig_network_correspondence/compute_overlap_with_atlases.py` & `cbig_network_correspondence-0.2.0/src/cbig_network_correspondence/compute_overlap_with_atlases.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,18 @@
         self.network_assign_path = NETWORK_ASSIGN_PATH
 
 
 def sort_files(data_path, filename):
     """
     Reads in files under the path and sort the files based on a natural order.
     """
-    if path.isdir(data_path):
+    if isinstance(data_path, list):
+        files_sorted_res = data_path
+        return files_sorted_res 
+    elif path.isdir(data_path):
         allfiles = listdir(data_path)
         files = []
         for eachfile in allfiles:
             if filename in eachfile:
                 files.append(eachfile)
         files_sorted = natsorted(files)
         files_sorted_res = [path.join(data_path, str(i)) for i in files_sorted]
@@ -250,15 +253,15 @@
         rh_data_fs = rh_data.get_fdata()
         #extract first 40962 elements from lh_data_fs and rh_data_fs
         lh_data_fs = lh_data_fs[:40962]
         rh_data_fs = rh_data_fs[:40962]
         data = np.concatenate((lh_data_fs, rh_data_fs), axis=0)
         data = np.squeeze(data)
         data = np.reshape(data, (data.shape[0], 1))
-        out_path = path.join(temp_path, 'input_data.npy')
+        out_path = path.join(temp_path, params.config.name + '.npy')
         np.save(out_path, data)
 
     elif params.config.type in ('Soft', 'Metric'):
         print('This is a soft parcellation or metric data.')
         data = []        
         params.data_sort_path = sort_files(params.data_path, params.config.name)
         out_path = path.dirname(params.data_sort_path[0])
@@ -275,15 +278,15 @@
             rh_data_fs = rh_data.get_fdata()
             #extract first 40962 elements from lh_data_fs and rh_data_fs
             lh_data_fs = lh_data_fs[:40962]
             rh_data_fs = rh_data_fs[:40962]
             curr_data = np.concatenate((lh_data_fs, rh_data_fs), axis=0)
             curr_data = np.squeeze(curr_data)
             curr_data = np.reshape(curr_data, (curr_data.shape[0], 1))
-            np.save(path.join(out_path, path.basename(curr_data_file) + '_input_data.npy'), curr_data)
+            np.save(path.join(out_path, path.basename(curr_data_file) + params.config.name + '.npy'), curr_data)
 
     return out_path
 
 def if_atlas_exist(atlas_name):
     atlas_list_file = open(ATLAS_LIST_PATH,"r", encoding="utf8")
     atlas_names = atlas_list_file.read().splitlines()
     if atlas_name in atlas_names:
@@ -672,18 +675,14 @@
     # for item inside overlap_mat_all.items(), key is the atlas name, value is the overlap matrix
     # the overlap matrix should be a 1xN matrix, where N is the number of networks in the atlas
     # throw error message if the matrix is not 1xN
     single_flag = True
     for key, value in overlap_mat_all.items():
         if value.shape[0] != 1:
             single_flag = False
-            if ref_networks is None:
-                print("ERROR! The overlap matrix for atlas " + key + " has multiple dimensions.")
-                print("Please provide the reference networks names to visualize network correspondence as heatmap.")
-                sys.exit(1)
     p_val = permute_overlap_data_all(ref_params, atlas_names_list)
 
     if single_flag:
         print("Single dimension data is provided. Visualize network correspondence as circular chart.")
         network_names = vis.construct_network_name_all(atlas_names_list)
         df1 = pd.DataFrame([(key, value) for key, values in overlap_mat_all.items() for value in values], columns=['group', 'dice'])
         #flatten df1
```

### Comparing `cbig_network_correspondence-0.1.4/src/cbig_network_correspondence/grab_data_info.py` & `cbig_network_correspondence-0.2.0/src/cbig_network_correspondence/grab_data_info.py`

 * *Files identical despite different names*

### Comparing `cbig_network_correspondence-0.1.4/src/cbig_network_correspondence/visualize_overlap_lib.py` & `cbig_network_correspondence-0.2.0/src/cbig_network_correspondence/visualize_overlap_lib.py`

 * *Files identical despite different names*

### Comparing `cbig_network_correspondence-0.1.4/src/cbig_network_correspondence/visualize_report_lib.py` & `cbig_network_correspondence-0.2.0/src/cbig_network_correspondence/visualize_report_lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -650,16 +650,22 @@
     # export to csv
     df.to_csv(out_dir + "/network_correspondence.csv")
 
 def report_atlas_network_correspondence(combined_data,ref_atlas_name,out_dir):
     # if directory doesn't exist, create it
     if not os.path.exists(out_dir):
         os.makedirs(out_dir)
-    vis.draw_overlap_mat_all(combined_data, ref_atlas_name, figfile=out_dir)
     reference_name = vis.construct_network_name(ref_atlas_name)
+    iter_data = iter(combined_data.items())
+    firstkey , firstvalue = next(iter_data)
+    data_dim = firstvalue['Dice'].shape[0]
+    # if reference_name length is 1, add index to reference_name
+    if len(reference_name) == 1:
+        reference_name = [reference_name[0] + str(i+1) for i in range(data_dim)]
+    vis.draw_overlap_mat_all(combined_data, reference_name, figfile=out_dir)
     #for each key in combined_data, generate a table_summary_plot
     for key in combined_data:
         curr_data = combined_data[key]
         curr_dice = curr_data['Dice']
         curr_pval = curr_data['P value']
         
         other_name = vis.construct_network_name(key)
```

### Comparing `cbig_network_correspondence-0.1.4/PKG-INFO` & `cbig_network_correspondence-0.2.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,44 +1,7 @@
-Metadata-Version: 2.1
-Name: cbig_network_correspondence
-Version: 0.1.4
-Summary: A toolbox for exploring network correspondence across atlases
-Home-page: https://rubykong.github.io/cbig_network_correspondence
-License: MIT
-Author: Ruby Kong
-Author-email: roo.cone@gmail.com
-Requires-Python: >=3.8.1,<4.0
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Typing :: Typed
-Requires-Dist: brainspace (>=0.1.10,<0.2.0)
-Requires-Dist: colorcet (>=3.0.1,<4.0.0)
-Requires-Dist: gitpython (>=3.1.27,<4.0.0)
-Requires-Dist: natsort (>=8.3.1,<9.0.0)
-Requires-Dist: nibabel (>=5.0.1,<6.0.0)
-Requires-Dist: numpy (>=1.20.3,<2.0.0)
-Requires-Dist: pandas (>=1.3.2,<2.0.0)
-Requires-Dist: plottable (>=0.1.5,<0.2.0)
-Requires-Dist: regfusion (>=0.1.0,<0.2.0)
-Requires-Dist: scipy (>=1.9.0,<2.0.0)
-Requires-Dist: seaborn (>=0.11.2,<0.12.0)
-Project-URL: Repository, https://github.com/rubykong/cbig_network_correspondence
-Description-Content-Type: text/markdown
-
 # cbig_network_correspondence
 
 [![PyPI](https://img.shields.io/pypi/v/cbig_network_correspondence?style=flat-square)](https://pypi.python.org/pypi/cbig_network_correspondence/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/cbig_network_correspondence?style=flat-square)](https://pypi.python.org/pypi/cbig_network_correspondence/)
 [![PyPI - License](https://img.shields.io/pypi/l/cbig_network_correspondence?style=flat-square)](https://pypi.python.org/pypi/cbig_network_correspondence/)
 [![Coookiecutter - Wolt](https://img.shields.io/badge/cookiecutter-Wolt-00c2e8?style=flat-square&logo=cookiecutter&logoColor=D4AA00&link=https://github.com/woltapp/wolt-python-package-cookiecutter)](https://github.com/woltapp/wolt-python-package-cookiecutter)
 
@@ -53,309 +16,248 @@
 
 ---
 
 This toolbox was used to explore the network correspondence between networks across different atlases. 
 
 ## Installation
 
+To install:
+
 ```sh
 pip install cbig_network_correspondence
 ```
 
-## Usage
+To upgrade:
+
+```sh
+pip install --upgrade cbig_network_correspondence
+```
 
-This toolbox has the following functions:
 
-+ Compute and visualize network overlap between two existing alases
-+ Compute and visualize overlap between any metric data (e.g. task contrast map, probability map, other atlas) and an existing atlas
-+ Visualze the overlapping area between two atlases or a metric data and an atlas
+## Usage
 
-We will provide detailed usage of these function in the following sections.
+### Tutorial
+
+We provide a tutorial for how to use this toolbox. The tutorial is available in the Usage.ipynb notebook:
++ [`Usage.ipynb](https://github.com/rubykong/cbig_network_correspondence/blob/master/Usage.ipynb)
 
 ### Atlases we included
 
 Check this list for the atlases we have included. We use abbreviations for the atlases. Here we provide the decription for each atlas. If you want us to include your atlas, please contact me (roo.cone@gmail.com).
 
-![networkcorrespondence](https://github.com/rubykong/cbig_network_correspondence_data/assets/20438248/b430f2fe-4b78-49f2-9084-5a43d450dba1)
+| Abbreviation | Source                         | Description                                            |
+|--------------|--------------------------------|--------------------------------------------------------|
+| MG360J12     | Glasser2016; Ji2019            | Mattew Glasser2016 360-ROI with Ji2019 12 Cole-Anticevic networks |
+| HCPICA       | Smith2009; Smith2013           | HCP 25-node ICA maps                                   |
+| AL20         | Laird2011                      | Angela Laird2011 20-node ICA maps                      |
+| AS200K17     | Schaefer2018; Kong2021         | Alex Schaefer2018 200-ROI with Kong2021 17 networks    |
+| AS200Y17     | Schaefer2018; Yeo2011          | Alex Schaefer2018 200-ROI with Yeo2011 17 networks     |
+| AS400K17     | Schaefer2018; Kong2021         | Alex Schaefer2018 400-ROI with Kong2021 17 networks    |
+| AS400Y17     | Schaefer2018; Yeo2011          | Alex Schaefer2018 400-ROI with Yeo2011 17 networks     |
+| XS268_8      | Shen2013                       | Xilin Shen2013 268-ROI with 8 networks                 |
+| XS368_8      | Shen2013                       | Xilin Shen2013 368-ROI with 8 networks                 |
+| WS90_14      | Shirer2012                     | William Shirer2012 90-ROI 14 networks                  |
+| UKBICA       | Smith2009; Alfaro-Almagro2018  | UKBiobank 25-node ICA maps                             |
+| EG286_12     | Power2011; Gordon2016          | Evan Gordon2016 286-ROI with 12 networks               |
+| TL12         | Power2011; Laumann2015         | Tim Laumann2015 12 networks (Power2011)                |
+| EG17         | Power2011; Gordon2017          | Evan Gordon2017 17 networks                            |
+| TY7          | Yeo2011                        | Thomas Yeo 7 networks                                  |
+| TY17         | Yeo2011                        | Thomas Yeo 17 networks                                 |
+| XY200K17     | Yan2023; Kong2021              | Xiaoxuan Yan2023 200-ROI with Kong2021 17 networks     |
+| XY200Y17     | Yan2023; Yeo2011               | Xiaoxuan Yan2023 200-ROI with Yeo2011 17 networks      |
+| XY400K17     | Yan2023; Kong2021              | Xiaoxuan Yan2023 400-ROI with Kong2021 17 networks     |
+| XY400Y17     | Yan2023; Yeo2011               | Xiaoxuan Yan2023 400-ROI with Yeo2011 17 networks      |
+
 
 These atlases should be automatically downloaded when you install the toolbox. If you want to download the atlases manually, you can find the atlases here: https://github.com/rubykong/cbig_network_correspondence_data. The atlas data will be automatically downloaded in your python package directory: `cbig_network_correspondence/src/cbig_network_correspondence/data`.
 
-### Config file
 
-In this toolbox, the information for each atlas was constructed as config file. We have included the config files for each atlas. The config files will be automatically downloaded when you install the toolbox. If you want to check the config files manually, you can find the config files in your python package directory: `cbig_network_correspondence/src/cbig_network_correspondence/data/atlas_config`. If you want to use your own atlas, you can create your own config file, check next sections for details. 
+### Input data
+
+The toolbox can also explore the network correspondence of your own input data. The input data can be different format. We support input data in fs_LR_32k, fsaverage6, and FSLMNI2mm.
+
+#### Format
+
+Here are the formats we support:
+
+For data in fs_LR_32k or fsaverage6 space:
+
++ `.mat` file: The file should contain two variables starting with `lh` and `rh`. For example, the variable names could be `lh_data`, `rh_data` or `lh_labels`, `rh_labels`. Each variable should be a 32492x1 vector for `fs_LR_32k` space or a 40962x1 vector for `fsaverage6` space. 
+
++ `.npy` file: The file should contain a numpy array with shape (64984, 1) for `fs_LR_32k` space or (81924, 1) for `fsaverage6` space.
+
+For data in FSLMNI2mm space:
+
++ `.nii` or `.nii.gz` file: The file should be a nifti file with the same dimension as the FSL MNI152 2mm template.
+
+
+#### Pass in the data as ...
+
++ A single path to a single file
+  - `/data_dir/my_task_contrast_map.mat`
+  - `/data_dir/my_task_contrast_map.npy`
+  - `/data_dir/my_task_contrast_map.nii.gz`
+
++ A list of paths to multiple files
+  - `['/data_dir/my_task_contrast_map1.mat', '/data_dir/my_task_contrast_map2.mat']`
+  - `['/data_dir/my_task_contrast_map1.npy', '/data_dir/my_task_contrast_map2.npy']`
+  - `['/data_dir/my_task_contrast_map1.nii.gz', '/data_dir/my_task_contrast_map2.nii.gz']`
+
++ A directory contains the input files
+  - `/data_dir`
+  under this directory, the toolbox will search for the files containing the `Data_Name` in the config file (see the Config file section for more details). For example, if the `Data_Name` is `my_task_contrast_map`, the toolbox will search for the files containing `my_task_contrast_map` in the file name
+
++ A string indicating the name of a existing atlas
+  - `AS400Y17`
+  - `EG17`
+  - `TY17`
+
+#### Reference data space
+
+To explore the network correspondence between a given input data and existing atlases, the toolbox will use the input data as the reference data. The toolbox will use existing atlases in the same space as the input data. For example, if the input data is in `fs_LR_32k` space, the toolbox will use the existing atlases in `fs_LR_32k` space. If the input data is in `FSLMNI2mm` space, the toolbox will use the existing atlases in `FSLMNI2mm` space. 
+
+#### Reference data names
+
+User can specify the name for the given input data, if not, the toolbox will use the `Data_Name` in the config file as the reference data name. 
+
+Reference data names could be important for a multi-dimension input data. For example, if the input data is a set of task contrast maps, the user might want to specify the reference data names for each task contrast map. Otherwise, the toolbox will name each task contrast map as `<Data_Name>1`, `<Data_Name>2`, etc. 
+
+If the input data is the user's own atlas with K networks, the user should specify the reference data names for each network. Otherwise the toolbox will name each network as `<Data_Name>1`, `<Data_Name>2`, etc.
+
+#### Config file
+
+In this toolbox, the information for each atlas or input data is constructed as a config file. We have included the config files for existing atlases. The config files will be automatically downloaded when you install the toolbox. If you want to check the config files manually, you can find the config files in your python package directory: `cbig_network_correspondence/src/cbig_network_correspondence/data/atlas_config`. If you want to explore network correspondence of your own input data/atlas, you can create your own config file, check next sections for how to create a config file. 
 
 The config file should be a text file. 
 
 Here is an example of the config file for the Schaefer 400-ROI atlas with Yeo 17-network network assignemnt `AS400Y17`:
 ```
 [data_info]
 Data_Category: YeoLab
 Data_Name: AS400Y17
 Data_Space: fsaverage6
 Data_Type: Hard
 Data_NetworkAssignment: 1
 ```
 
-Here is an example of the config file for a example metric data `Exemplar1(pos)`:
+Here is an example of the config file for a example metric data `Example`:
 ```
 [data_info]
-Data_Name: Exemplar1(pos)
+Data_Name: Example
 Data_Space: FSLMNI2mm
 Data_Type: Metric
 Data_Threshold: [5,Inf]
 ```
 
 Here is the decription for the config file:
 
 + `Data_Category` [optional]
   
   We included it for existing atlases because some atlases were from the same lab. In this case, we put the some atlases into the same category. This is not necessary for your own atlas or your own metric data.
    
 + `Data_Name`
 
-  The name of the atlas or metric data.
+  The name of the atlas or metric data. If the input data is a set of files instead of a single file, user can pass in the directory to the files. The toolbox will search for the files containing the `Data_Name` in the file name. For example, if the `Data_Name` is `my_task_contrast_map`, the toolbox will search for the files containing `my_task_contrast_map` in the file name.
 
 + `Data_Space`
 
-  The space name of the space where the atlas/data is in. It can be a surface name or a volumetric space name. We currenly have atlases in the following spaces: `fs_LR_32k` surface space, `fsaverage6` surface space, `FSLMNI2mm` volumetric space, `LairdColin2mm` volumetric space, `ShenColin1mm` volumetric space.
+  The space name of the space where the atlas/data is in. It can be a surface name or a volumetric space name. We currenly have atlases in the following spaces: `fs_LR_32k` surface space, `fsaverage6` surface space, `FSLMNI2mm` volumetric space, `LairdColin2mm` volumetric space, `ShenColin1mm` volumetric space. If the user wants to explore the network correspondence of their own data, the data should be in `fs_LR_32k`, `fsaverage6`, or `FSLMNI2mm` space.
   
 + `Data_Type`
 
   The type of the atlas/data. We have two types of atlas: `Hard` and `Soft`. The `Hard` atlas is the atlas that each ROI is assigned to a specific network. The `Soft` atlas is the atlas that each ROI is assigned to a probability of belonging to each network. We also allow for a metric data such as task contrast maps or probability maps, in this case `Data_Type` should be `Metric`. 
 
 + `Data_NetworkAssignment` [optional]
 
   Sometimes the atlas has fine-grained ROIs and these ROIs were assigned to large-scale networks. For example, the Schaefer2018 400 ROIs were assigned to the Yeo 17-network atlas. In this case the user can provide a mapping between ROIs to networks, here you can find the mapping for some of the existing atlases: https://github.com/rubykong/cbig_network_correspondence_data/tree/master/network_assignment
 
 + `Data_Threshold` [optional]
 
   For soft parcellation and metric data, we will need to apply a threshold to binarize the data. The threshold should be set as `[lower bound, upper bound]`. If the upper bound is `Inf`, then the threshold will be applied as `>= lower bound`. If the lower bound is `-Inf`, then the threshold will be applied as `<= upper bound`. If the `Data_Type` is `Soft` or `Metric`, but the `Data_Threshold` is not provided, the toolbox will use a default threshold `[0, Inf]`. `Data_Threshold` is not necessary for `Hard` atlas.
 
-After importing the toolbox, here are the relevant commands. After decribing the commands, we provide examples for how to use this toolbox. We also provided a jupyter notebook for the examples: ExampleUsage.ipynb. Please note that the output figure path were hard-coded in the notebook, so you might need to change the output figure path to your own path.
+After importing the toolbox, here are the relevant commands. After decribing the commands, we provide examples for how to use this toolbox. We also provided a jupyter notebook for the usage examples: Usage.ipynb. 
 
-```python
-import cbig_network_correspondence as cnc
-```
-
-```
-overlap_mat = cnc.compute_overlap_with_atlases.load_overlap_atlases(ref_atlas_name, other_atlas_name)
 
-This function will load the pre-computed network overlap matrix between the reference atlas and the other atlas.
+### Usage scenarios
 
-Input:
-- ref_atlas_name: the name of the reference atlas
-- other_atlas_name: the name of the other atlas
+This toolbox has two main usage scenarios:
 
-Output:
-- overlap_mat: the network overlap matrix between the reference atlas and the other atlas
-```
-
-```
-cnc.visualize_overlap_lib.draw_overlap_mat(overlap_mat, ref_atlas_name, other_atlas_name, minv, maxv, outputfigfile)
+1. Use this toolbox to explore network correspondence between existing atlases.
+2. Provide users' own input data, and explore the network correspondence between the input data and existing atlases.
 
-This function will draw the network overlap matrix between the reference atlas and the other atlas. In this function, the user can pass in the loaded overlap matrix from cnc.compute_overlap_with_atlases.load_overlap_atlases.
+**We have provided detailed examples for each usage scenario in the Usage.ipynb notebook. Here we provide brief descriptions for inputs.**
 
-Input:
-- overlap_mat: the network overlap matrix between the reference atlas and the other atlas
-- ref_atlas_name: the name of the reference atlas
-- other_atlas_name: the name of the other atlas
-- minv: the minimum value of the colorbar
-- maxv: the maximum value of the colorbar
-- outputfigfile: the output figure file name
+#### 1. Explore network correspondence between existing atlases
 
-```
-```
-cnc.visualize_overlap_lib.draw_overlap_atlases(ref_atlas_name, other_atlas_name, minv, maxv, outputfigfile)
-
-This function will draw the network overlap matrix between the reference atlas and the other atlas. This function will automatically load the pre-computed network overlap matrix between the reference atlas and the other atlas.
-
-Input:
-- ref_atlas_name: the name of the reference atlas
-- other_atlas_name: the name of the other atlas
-- minv: the minimum value of the colorbar
-- maxv: the maximum value of the colorbar
-- outputfigfile: the output figure file name
-```
-
-```
-overlap_data = cnc.compute_overlap_with_atlases.obtain_overlap_atlases(ref_atlas_name, other_atlas_name, ref_network_name, other_network_name)
-
-This function generate the overlapping area between networks from two atlases. This is used for visualization purpose.
-
-Input:
-- ref_atlas_name: the name of the reference atlas
-- other_atlas_name: the name of the other atlas
-- ref_network_name: the name of the reference network
-- other_network_name: the name of the other network
-
-Note that you can find the network names for each atlas here:
-https://github.com/rubykong/cbig_network_correspondence_data/tree/master/network_names
-
-Output:
-- overlap_data: a numpy array in the same space as the reference atlas. The array contains three labels: 1, 2, 3.
-1 indicates the reference network, 2 indicates the other network, 3 indicates the overlapping area between the two networks.
-```
+![NCT_workflow1](https://github.com/rubykong/cbig_network_correspondence/assets/20438248/5046486c-b192-4aa4-90e4-825d962fc94c)
 
 ```
-cnc.visualize_overlap_lib.draw_overlap_map(data_space, overlap_data, outputfigfile, coords)
-
-This function visualize the overlapping area between networks from two atlases. The reference network will be colored in pink, the other network will be colored in blue, and the overlapping area will be colored in purple.
-
-Input:
-- data_space: the space of the data. It can be `fsaverage6`, `fs_LR_32k`, `FSLMNI2mm`, `LairdColin2mm`, `ShenColin1mm`
-- overlap_data: a numpy array in the same space as the reference atlas. The array contains three labels: 1, 2, 3. This is the output of cnc.compute_overlap_with_atlases.obtain_overlap_atlases
-- outputfigfile: the output figure file name
-- coords: [for volumetric data only] the coordinates of the point where the cut is performed. BY default, we use [-4, -31, 18].
-```
-
-
-```
-example = cnc.load_example
-
-This function find the path to the example config and example nifti image
-
-Output:
-- example_config: the path to the example config file
-- example_nii: the path to the example nifti image
-```
-
-```
-data_params = cnc.compute_overlap_with_atlases.DataParams(config_file, data_path)
-
-This function reads in the config information and the data path to construct the parameters for the data
-
-Input:
-- config_file: the path to the config file
-- data_path: the path to the data
-```
-
-```
-overlap_data = cnc.compute_overlap_with_atlases.obtain_overlap_data(data_params, atlas_name, network_name)
-
-This function generate the overlapping area between the binarized data and an existing atlas. This is used for visualization purpose. The calculation is done in the same space as the data.
-
-Input:
-- data_params: the parameters for the data. This is the output of the function cnc.compute_overlap_with_atlases.DataParams
-- atlas_name: the name of the atlas. For example, "MG360J12".
-- network_name: the name of the network from the atlas. For example, "Default".
-
-```
-
-### Compute and visualize network overlap between two existing alases
-
-In this toolbox, we computes the network overlap between any pair of existing atlases. We treat each atlas as the reference atlas, and projected other atlases to the same space as the reference atlas. Then we compute the network overlap between the reference atlas and the projected atlas.
-
-Here we provide examples if you want to check the network overlap matrix between the Glasser 2016 atlas with Ji2019 networks and the Yeo 17 networks, you can use the following code:
-
-```python
-import  cbig_network_correspondence as cnc
-
-# When Yeo 17-network atlas is the reference atlas, the Glasser2016 atlas will be projected to fsaverage6 surface space
-overlap_mat1 = cnc.compute_overlap_with_atlases.load_overlap_atlases("TY17", "MG360J12")
-
-# When Glasser2016 atlas atlas is the reference atlas, theYeo 17-network atlas will be projected to fs_LR_32k surface space
-overlap_mat2 = cnc.compute_overlap_with_atlases.load_overlap_atlases("MG360J12", "TY17")
-```
-
-If you want to visualize the network overlap matrix, you can use the following code:
+import cbig_network_correspondence as cnc
 
-```python
-cnc.visualize_overlap_lib.draw_overlap_mat(overlap_mat1, "TY17", "MG360J12", 0, 1, "<path_to_figure>/TY17_MG360J12")
-cnc.visualize_overlap_lib.draw_overlap_mat(overlap_mat2, "MG360J12", "TY17", 0, 1, "<path_to_figure>/MG360J12_TY17")
+cnc.compute_overlap_with_atlases.network_correspondence(reference_atlas, atlas_names_list, output_dir)
 ```
 
-The output figures will be save under the path `<path_to_figure>/TY17_MG360J12.png` and `<path_to_figure>/MG360J12_TY17.png`. Here are the corresponding figures. The left side are reference network names, the upper part are the other atlas network names
-
-+ `<path_to_figure>/TY17_MG360J12.png` 
-
-![image](https://user-images.githubusercontent.com/20438248/232752322-0fbe141f-3879-4c6d-9a04-1dd372753ea0.png)
++ `reference_atlas`: str
+  - The name of the reference atlas. The reference atlas should be one of the existing atlases. The toolbox will use the reference atlas to explore the network correspondence between the reference atlas and other atlases in the `atlas_names_list`.
++ `atlas_names_list`: list
+  - A list of the names of the atlases. The toolbox will explore the network correspondence between the reference atlas and the atlases in the `atlas_names_list`.
++ `output_dir`: str
+  - The directory to save the output figures and csv files.
 
-+ `<path_to_figure>/MG360J12_TY17.png`
+Note: network name should be the abbreviation of the atlas. For example, `AS400Y17` for the Schaefer 400-ROI atlas with Yeo 17-network network assignemnt.
 
-![image](https://user-images.githubusercontent.com/20438248/232752400-a162a152-043f-48e9-b45d-171bfea6b952.png)
+#### 2. Explore network correspondence between input data and existing atlases
 
+![NCT_workflow2](https://github.com/rubykong/cbig_network_correspondence/assets/20438248/55f9f944-246d-4146-b530-978b7e951ddd)
 
-However, if you have no interest to check the overlap matrix and just want to see the visualized network overlap between two atlases, you can use the following code:
-
-```python
-import  cbig_network_correspondence as cnc
-
-cnc.visualize_overlap_lib.draw_overlap_atlases("MG360J12", "TY17", 0, 1, "<path_to_figure>/MG360J12_TY17")
 ```
+import cbig_network_correspondence as cnc
 
-If you want to check the brain maps of the overlappping regions between two atlases, you can use the following code:
-
-+ To check the overlapping regions between the `Default` network from `MG360J12` atlas and the `DefaultA` network from `TY17` atlas:
-
-```python
-import  cbig_network_correspondence as cnc
-
-# When Yeo 17-network atlas is the reference atlas
-overlap_data = cnc.compute_overlap_with_atlases.obtain_overlap_atlases("TY17", "MG360J12", "DefaultA", "Default")
-# Yeo 17-network atlas is in fsaverage6 surface space
-cnc.visualize_overlap_lib.draw_overlap_map("fsaverage6", overlap_data, "<path_to_figures>/TY17_MG360J12_DefaultA_Default")
+# construct DataParams object based on the data file path and config
+ref_params = cnc.compute_overlap_with_atlases.DataParams(config, file_path)
 
-# When Glasser2016 atlas atlas is the reference atlas
-overlap_data = cnc.compute_overlap_with_atlases.obtain_overlap_atlases("MG360J12", "TY17", "Default", "DefaultA")
-# Glasser2016 atlas is in fs_LR_32k surface space
-cnc.visualize_overlap_lib.draw_overlap_map("fs_LR_32k", overlap_data, "<path_to_figures>/MG360J12_TY17_Default_DefaultA")
+# compute the overlap with atlases and save the results
+cnc.compute_overlap_with_atlases.network_correspondence(ref_params, atlas_names_list,output_dir,ref_data_names)
 
 ```
 
-Here are the results:
-![Overlap_surface](https://user-images.githubusercontent.com/20438248/232758349-ad5157cd-d6c2-4d4c-880c-7dda3a36fe0b.jpg)
++ `config`: str
+  - The path to the config file for the input data.
++ `file_path`: str/list
+  - The path to a single input data file
+  - A list of paths to multiple input data files
+  - A directory contains the input data files
++ `atlas_names_list`: list
+  - A list of the names of the atlases. The toolbox will explore the network correspondence between the input data and the atlases in the `atlas_names_list`.
++ `output_dir`: str
+  - The directory to save the output figures and csv files.
++ `ref_data_names`: str/list
+  - The name of the input data. If `ref_data_names` is not provided, the toolbox will use the `Data_Name` in the config file as the reference data name. If the input data is multi-dimension, each dimension will be named as `<Data_Name>1`, `<Data_Name>2`,... if the `ref_data_names` is not provided.
 
 
-### Compute and visualize overlap between any metric data and an existing atlas
+### Significance test
 
-In this toolbox, we also allow users to upload their own data and compute the network overlap between the data and an existing atlas. We treat the data as the reference, and projected the atlas to the same space as the reference data. For a metric data, we binarize the data use `Data_Threshold`, then we compute the network overlap between the binarized data and the projected atlas. Here we provide an example data to show you how to use this toolbox.
+The toolbox provides a significance test to test the significance of the network correspondence between the given input data and an existing atlas. The toolbox will use the spin-test (Gordon2017;Alexander-Bloch2018)to test the significance of the network correspondence. Specically, SpinPermutations from BrainSpace python package is used here. For data in FSLMNI2mm space, we project the data to the fsaverage6 space for the spin-test. 
 
-After importing the toolbox, here are the relevant commands. After decribing the commands, we provide examples for how to use this toolbox to compute and visualize the overlap between any metric data and an existing atlas.
 
-You can load the example data by using the following code:
+### Results
 
-```python
-import  cbig_network_correspondence as cnc
+NCT provides different types of plots to help the user explore/visualize the network correspondences. 
 
-example = cnc.load_example
-# the example config file
-print(example.example_config)
-# the path to the example data
-print(example.example_nii)
-# construct parameters for example data
-data_params = cnc.compute_overlap_with_atlases.DataParams(example.example_config, example.example_nii)
-```
-
-In this example, we will compute the overlap between thie example data and the Glasser2016 atlas. Since the example data is in FSLMNI2mm space, we will project the Glasser2016 atlas to FSLMNI2mm space and compute the overlap matrix.
-
-```python
-overlap_mat = cnc.compute_overlap_with_atlases.compute_overlap_data(data_params, "MG360J12")
-```
-
-After that, we can visualize the overlap matrix by using the following code:
-
-```python
-cnc.visualize_overlap_lib.draw_overlap_mat(overlap_mat, "Exampler1(pos)", "MG360J12", 0, 1, "<path_to_figures>/exampler1_pos_MG360J12")
-```
-
-Here is how the overlap matrix looks like:
-![image](https://user-images.githubusercontent.com/20438248/232759475-2eae4dad-0f7c-40d0-afe3-bd4731466542.png)
-
-Based on the visualized overlap matrix, we can notice that the example data overlapped the most with the `Default` network from Glasser2016. If we want to check the overlapping regions between the example data and the `Default` network from Glasser2016, we can use the following code:
++ Overlap Heatmap
+  - If input data has multiple dimensions, e.g., a atlas with K networks, a set of task contrast maps. For a specified list of existing atlases, the toolbox will provide heatmaps to show the overlap between the input data and the existing atlases. Each atlas will have a heatmap. If input data has K dimension, and the other atlas has N networks, the heatmap will be a KxN heatmap. Each row represents the overlap between the input data and an existing atlas. Each column represents the overlap between the input data and a network in the existing atlas. The color represents the overlap value. The asterisk indicates the significance of the overlap. 
 
-```python
-overlap_data = cnc.compute_overlap_with_atlases.obtain_overlap_data(data_params, 'MG360J12', 'Default')
-# By default we use coords=[-4, -31, 18] to visualize volumetric data, you can change it to any other coordinates
-cnc.visualize_overlap_lib.draw_overlap_map("FSLMNI2mm", overlap_data, "<path_to_figures>/example_MG360J12_Default", [-4, -31, 18])
-```
-
-Here is the result:
-![image](https://user-images.githubusercontent.com/20438248/232760522-f1327b70-2bc7-4b74-bdf2-30274146bfa6.png)
++ Network Clock
+  - If input data is single dimension, e.g., a task contrast map, a probability map. For a specified list of existing atlases, the toolbox will provide a network clock to show the overlap between the input data and the existing atlases. The network clock will show the overlap between the input data and all networks. Networks from the same atlas are grouped together and colored by the same color. Only the networks with significant overlap will be indicated by network name in the network clock. The clock ring represents the overlap value. The network font size represents the overlap value. 
 
++ Network Radar
+  - If input data is single dimension, e.g., a task contrast map, a probability map. For a specified list of existing atlases, the toolbox will provide a network radar to show the overlap between the input data and the existing atlases. Each atlas will have a radar map. The asterisk indicates the significance of the overlap.
 
++ Summary Table
+  - The toolbox will provide a summary table to show the exact overlap values and p-values of the overlap between the input data and the existing atlases. Summary tables will be saved as figures and csv files.
 
 ## Development
 
 * Clone this repository
 * Requirements:
   * [Poetry](https://python-poetry.org/)
   * Python 3.7+
@@ -370,8 +272,7 @@
 ```sh
 poetry shell
 ```
 
 ---
 
 This project was generated using the [wolt-python-package-cookiecutter](https://github.com/woltapp/wolt-python-package-cookiecutter) template.
-
```

