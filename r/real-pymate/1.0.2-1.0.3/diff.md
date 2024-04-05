# Comparing `tmp/real_pymate-1.0.2.tar.gz` & `tmp/real_pymate-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "real_pymate-1.0.2.tar", last modified: Wed Apr  3 13:55:02 2024, max compression
+gzip compressed data, was "real_pymate-1.0.3.tar", last modified: Fri Apr  5 21:27:10 2024, max compression
```

## Comparing `real_pymate-1.0.2.tar` & `real_pymate-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 13:55:02.273428 real_pymate-1.0.2/
--rw-rw-rw-   0        0        0     1091 2024-03-31 20:35:08.000000 real_pymate-1.0.2/LICENSE
--rw-rw-rw-   0        0        0    25663 2024-04-03 13:55:02.270053 real_pymate-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0    25243 2024-04-03 13:50:04.000000 real_pymate-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-03 13:55:02.246935 real_pymate-1.0.2/pyMate/
--rw-rw-rw-   0        0        0    16473 2024-03-30 20:51:47.000000 real_pymate-1.0.2/pyMate/Clyde.py
--rw-rw-rw-   0        0        0    11748 2024-03-31 07:47:15.000000 real_pymate-1.0.2/pyMate/Gordo.py
--rw-rw-rw-   0        0        0     2916 2024-04-03 12:16:00.000000 real_pymate-1.0.2/pyMate/Zaius.py
--rw-rw-rw-   0        0        0        0 2024-04-01 06:37:29.000000 real_pymate-1.0.2/pyMate/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 13:55:02.266512 real_pymate-1.0.2/real_pymate.egg-info/
--rw-rw-rw-   0        0        0    25663 2024-04-03 13:55:02.000000 real_pymate-1.0.2/real_pymate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2024-04-03 13:55:02.000000 real_pymate-1.0.2/real_pymate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 13:55:02.000000 real_pymate-1.0.2/real_pymate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-03 13:55:02.000000 real_pymate-1.0.2/real_pymate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-03 13:55:02.273428 real_pymate-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      628 2024-04-03 11:06:57.000000 real_pymate-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-03 13:55:02.262765 real_pymate-1.0.2/test/
--rw-rw-rw-   0        0        0     1854 2024-03-23 20:11:15.000000 real_pymate-1.0.2/test/test_ephys_tools.py
--rw-rw-rw-   0        0        0     1439 2024-03-03 08:52:32.000000 real_pymate-1.0.2/test/test_fmri_tools.py
+drwxrwxrwx   0        0        0        0 2024-04-05 21:27:10.100570 real_pymate-1.0.3/
+-rw-rw-rw-   0        0        0     1091 2024-03-31 20:35:08.000000 real_pymate-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0    26359 2024-04-05 21:27:10.099241 real_pymate-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0    25939 2024-04-05 21:23:22.000000 real_pymate-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-05 21:27:10.086923 real_pymate-1.0.3/pyMate/
+-rw-rw-rw-   0        0        0    16473 2024-03-30 20:51:47.000000 real_pymate-1.0.3/pyMate/Clyde.py
+-rw-rw-rw-   0        0        0    11748 2024-03-31 07:47:15.000000 real_pymate-1.0.3/pyMate/Gordo.py
+-rw-rw-rw-   0        0        0     5876 2024-04-05 21:13:13.000000 real_pymate-1.0.3/pyMate/Zaius.py
+-rw-rw-rw-   0        0        0        0 2024-04-01 06:37:29.000000 real_pymate-1.0.3/pyMate/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 21:27:10.097733 real_pymate-1.0.3/real_pymate.egg-info/
+-rw-rw-rw-   0        0        0    26359 2024-04-05 21:27:10.000000 real_pymate-1.0.3/real_pymate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2024-04-05 21:27:10.000000 real_pymate-1.0.3/real_pymate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 21:27:10.000000 real_pymate-1.0.3/real_pymate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-05 21:27:10.000000 real_pymate-1.0.3/real_pymate.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-05 21:27:10.100570 real_pymate-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      628 2024-04-03 14:09:14.000000 real_pymate-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 21:27:10.094689 real_pymate-1.0.3/test/
+-rw-rw-rw-   0        0        0     1854 2024-03-23 20:11:15.000000 real_pymate-1.0.3/test/test_ephys_tools.py
+-rw-rw-rw-   0        0        0     1439 2024-03-03 08:52:32.000000 real_pymate-1.0.3/test/test_fmri_tools.py
```

### Comparing `real_pymate-1.0.2/LICENSE` & `real_pymate-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `real_pymate-1.0.2/PKG-INFO` & `real_pymate-1.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: real_pymate
-Version: 1.0.2
+Version: 1.0.3
 Summary: Framework to process primate fMRI and electrophysiological data
 Home-page: https://github.com/akcarsten/pyMate
 Author: Carsten Klein
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -49,17 +49,17 @@
     - [Plot LFP time course and power spectrum](#plot-lfp-time-course-and-power-spectrum)
     - [Plot LFP Time Course and Mark Detected Peaks](#plot-lfp-time-course-and-mark-detected-peaks)
     - [Plot mean Time-Frequency Power Spectrum](#plot-mean-time-frequency-power-spectrum)
     - [Plot Power Spectra of Detected Events](#plot-power-spectra-of-detected-events)
     - [Plot Cluster Time-Frequency Power Spectrum and LFP traces](#plot-cluster-time-frequency-power-spectrum-and-lfp-traces)
 - [Zaius](#zaius)
   - [Bruker Data to Nifti format](#bruker-data-to-nifti-format)
+  - [Matlab files to HDF5](#matlab-files-to-hdf5)
   - [DGZ files to csv](#dgz-files-to-csv)
   - [ADFX files to HDF5](#adfx-files-to-hdf5)
-  - [Matlab files to HDF5](#matlab-files-to-hdf5)
 
 ## Main Features
 - **[Gordo](#gordo)**: Toolkit to process fMRI data. Named after Gordo, a squirrel monkey, who traveled to space in 1958.
 - **[Clyde](#clyde)**: Toolkit to process e-phys data. Named after Clyde, a character in Clint Eastwood movies, played 
 by an Orangutan named Manis.
 - **[Zaius](#zaius)** Various tools to convert fringe data formats into more common data structures. Named after 
 Dr. Zaius, the minister of science in the Planet of the Apes movies.
@@ -411,26 +411,43 @@
 Bruker data to Nifti format. However, the package is no longer maintained and might not be able to convert 
 all Bruker data formats. 
 The [source code is available on GitHub](https://github.com/neurolabusc/Bru2Nii?tab=readme-ov-file).
 2) **[Bruker2nifti](https://github.com/SebastianoF/bruker2nifti)**: Is Python package that also provides a command line
 and a graphical user interface to convert Bruker data to Nifti format. The package is currently actively maintained. 
 The [Zaius](#zaius) module provides a wrapper function to use this package.
 
-The following otlines the intended usage:
+The following outlines the intended usage:
 ```python
 from pyMate.Zaius import ConvertBruker
 
 
 study_folder = r'c:\your\folder\structure\great_study\great_subject'
 target_folder = r'c:\your\folder\structure\great_study\converted_data'
-study_name = 'CM032.Aw1'
+study_name = 'great_study'
 
 bru2nifti = ConvertBruker(study_folder=study_folder,
                           target_folder=target_folder,
                           study_name=study_name)
 
 bru2nifti.convert_2_nifti()
 ```
 
+#### Matlab files to HDF5
+Electro-physiological data that is acquired parallel to fMRI data contains large artifacts. Typically this data was
+cleaned with a default Matlab toolbox from the AGLO lab. Therefore the output format is a .mat file. To enable  working
+with this cleaned data in Python the [Zaius](#zaius) module provides the _ConvertMatFile_ class which converts these
+Matlab files into the HDF5 format.
+
+The following outlines the intended usage:
+```Python
+from pyMate.Zaius import ConvertMatFile
+
+
+mat_file_folder = r'D:\cleaned\matlab\ephys\data'
+target_folder = r'C:\lets\store\the\converted\data\here'
+
+converter = ConvertMatFile(mat_file_folder, target_folder)
+converter.convert()
+```
+
 #### DGZ files to csv
 #### ADFX files to HDF5 
-#### Matlab files to HDF5
```

### Comparing `real_pymate-1.0.2/README.md` & `real_pymate-1.0.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -37,17 +37,17 @@
     - [Plot LFP time course and power spectrum](#plot-lfp-time-course-and-power-spectrum)
     - [Plot LFP Time Course and Mark Detected Peaks](#plot-lfp-time-course-and-mark-detected-peaks)
     - [Plot mean Time-Frequency Power Spectrum](#plot-mean-time-frequency-power-spectrum)
     - [Plot Power Spectra of Detected Events](#plot-power-spectra-of-detected-events)
     - [Plot Cluster Time-Frequency Power Spectrum and LFP traces](#plot-cluster-time-frequency-power-spectrum-and-lfp-traces)
 - [Zaius](#zaius)
   - [Bruker Data to Nifti format](#bruker-data-to-nifti-format)
+  - [Matlab files to HDF5](#matlab-files-to-hdf5)
   - [DGZ files to csv](#dgz-files-to-csv)
   - [ADFX files to HDF5](#adfx-files-to-hdf5)
-  - [Matlab files to HDF5](#matlab-files-to-hdf5)
 
 ## Main Features
 - **[Gordo](#gordo)**: Toolkit to process fMRI data. Named after Gordo, a squirrel monkey, who traveled to space in 1958.
 - **[Clyde](#clyde)**: Toolkit to process e-phys data. Named after Clyde, a character in Clint Eastwood movies, played 
 by an Orangutan named Manis.
 - **[Zaius](#zaius)** Various tools to convert fringe data formats into more common data structures. Named after 
 Dr. Zaius, the minister of science in the Planet of the Apes movies.
@@ -399,26 +399,43 @@
 Bruker data to Nifti format. However, the package is no longer maintained and might not be able to convert 
 all Bruker data formats. 
 The [source code is available on GitHub](https://github.com/neurolabusc/Bru2Nii?tab=readme-ov-file).
 2) **[Bruker2nifti](https://github.com/SebastianoF/bruker2nifti)**: Is Python package that also provides a command line
 and a graphical user interface to convert Bruker data to Nifti format. The package is currently actively maintained. 
 The [Zaius](#zaius) module provides a wrapper function to use this package.
 
-The following otlines the intended usage:
+The following outlines the intended usage:
 ```python
 from pyMate.Zaius import ConvertBruker
 
 
 study_folder = r'c:\your\folder\structure\great_study\great_subject'
 target_folder = r'c:\your\folder\structure\great_study\converted_data'
-study_name = 'CM032.Aw1'
+study_name = 'great_study'
 
 bru2nifti = ConvertBruker(study_folder=study_folder,
                           target_folder=target_folder,
                           study_name=study_name)
 
 bru2nifti.convert_2_nifti()
 ```
 
+#### Matlab files to HDF5
+Electro-physiological data that is acquired parallel to fMRI data contains large artifacts. Typically this data was
+cleaned with a default Matlab toolbox from the AGLO lab. Therefore the output format is a .mat file. To enable  working
+with this cleaned data in Python the [Zaius](#zaius) module provides the _ConvertMatFile_ class which converts these
+Matlab files into the HDF5 format.
+
+The following outlines the intended usage:
+```Python
+from pyMate.Zaius import ConvertMatFile
+
+
+mat_file_folder = r'D:\cleaned\matlab\ephys\data'
+target_folder = r'C:\lets\store\the\converted\data\here'
+
+converter = ConvertMatFile(mat_file_folder, target_folder)
+converter.convert()
+```
+
 #### DGZ files to csv
-#### ADFX files to HDF5 
-#### Matlab files to HDF5
+#### ADFX files to HDF5
```

### Comparing `real_pymate-1.0.2/pyMate/Clyde.py` & `real_pymate-1.0.3/pyMate/Clyde.py`

 * *Files identical despite different names*

### Comparing `real_pymate-1.0.2/pyMate/Gordo.py` & `real_pymate-1.0.3/pyMate/Gordo.py`

 * *Files identical despite different names*

### Comparing `real_pymate-1.0.2/real_pymate.egg-info/PKG-INFO` & `real_pymate-1.0.3/real_pymate.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: real_pymate
-Version: 1.0.2
+Version: 1.0.3
 Summary: Framework to process primate fMRI and electrophysiological data
 Home-page: https://github.com/akcarsten/pyMate
 Author: Carsten Klein
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -49,17 +49,17 @@
     - [Plot LFP time course and power spectrum](#plot-lfp-time-course-and-power-spectrum)
     - [Plot LFP Time Course and Mark Detected Peaks](#plot-lfp-time-course-and-mark-detected-peaks)
     - [Plot mean Time-Frequency Power Spectrum](#plot-mean-time-frequency-power-spectrum)
     - [Plot Power Spectra of Detected Events](#plot-power-spectra-of-detected-events)
     - [Plot Cluster Time-Frequency Power Spectrum and LFP traces](#plot-cluster-time-frequency-power-spectrum-and-lfp-traces)
 - [Zaius](#zaius)
   - [Bruker Data to Nifti format](#bruker-data-to-nifti-format)
+  - [Matlab files to HDF5](#matlab-files-to-hdf5)
   - [DGZ files to csv](#dgz-files-to-csv)
   - [ADFX files to HDF5](#adfx-files-to-hdf5)
-  - [Matlab files to HDF5](#matlab-files-to-hdf5)
 
 ## Main Features
 - **[Gordo](#gordo)**: Toolkit to process fMRI data. Named after Gordo, a squirrel monkey, who traveled to space in 1958.
 - **[Clyde](#clyde)**: Toolkit to process e-phys data. Named after Clyde, a character in Clint Eastwood movies, played 
 by an Orangutan named Manis.
 - **[Zaius](#zaius)** Various tools to convert fringe data formats into more common data structures. Named after 
 Dr. Zaius, the minister of science in the Planet of the Apes movies.
@@ -411,26 +411,43 @@
 Bruker data to Nifti format. However, the package is no longer maintained and might not be able to convert 
 all Bruker data formats. 
 The [source code is available on GitHub](https://github.com/neurolabusc/Bru2Nii?tab=readme-ov-file).
 2) **[Bruker2nifti](https://github.com/SebastianoF/bruker2nifti)**: Is Python package that also provides a command line
 and a graphical user interface to convert Bruker data to Nifti format. The package is currently actively maintained. 
 The [Zaius](#zaius) module provides a wrapper function to use this package.
 
-The following otlines the intended usage:
+The following outlines the intended usage:
 ```python
 from pyMate.Zaius import ConvertBruker
 
 
 study_folder = r'c:\your\folder\structure\great_study\great_subject'
 target_folder = r'c:\your\folder\structure\great_study\converted_data'
-study_name = 'CM032.Aw1'
+study_name = 'great_study'
 
 bru2nifti = ConvertBruker(study_folder=study_folder,
                           target_folder=target_folder,
                           study_name=study_name)
 
 bru2nifti.convert_2_nifti()
 ```
 
+#### Matlab files to HDF5
+Electro-physiological data that is acquired parallel to fMRI data contains large artifacts. Typically this data was
+cleaned with a default Matlab toolbox from the AGLO lab. Therefore the output format is a .mat file. To enable  working
+with this cleaned data in Python the [Zaius](#zaius) module provides the _ConvertMatFile_ class which converts these
+Matlab files into the HDF5 format.
+
+The following outlines the intended usage:
+```Python
+from pyMate.Zaius import ConvertMatFile
+
+
+mat_file_folder = r'D:\cleaned\matlab\ephys\data'
+target_folder = r'C:\lets\store\the\converted\data\here'
+
+converter = ConvertMatFile(mat_file_folder, target_folder)
+converter.convert()
+```
+
 #### DGZ files to csv
 #### ADFX files to HDF5 
-#### Matlab files to HDF5
```

### Comparing `real_pymate-1.0.2/setup.py` & `real_pymate-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="real_pymate",
-    version="1.0.2",
+    version="1.0.3",
     url="https://github.com/akcarsten/pyMate",
     author="Carsten Klein",
     description="Framework to process primate fMRI and electrophysiological data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `real_pymate-1.0.2/test/test_ephys_tools.py` & `real_pymate-1.0.3/test/test_ephys_tools.py`

 * *Files identical despite different names*

### Comparing `real_pymate-1.0.2/test/test_fmri_tools.py` & `real_pymate-1.0.3/test/test_fmri_tools.py`

 * *Files identical despite different names*

