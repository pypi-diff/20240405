# Comparing `tmp/emgflow-0.0.1.tar.gz` & `tmp/emgflow-1.0.0.tar.gz`

## Comparing `emgflow-0.0.1.tar` & `emgflow-1.0.0.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     7042 2020-02-02 00:00:00.000000 emgflow-0.0.1/src/EMGFlow/OutlierFinder.py
--rw-r--r--   0        0        0     9754 2020-02-02 00:00:00.000000 emgflow-0.0.1/src/EMGFlow/PlotSignals.py
--rw-r--r--   0        0        0    45878 2020-02-02 00:00:00.000000 emgflow-0.0.1/src/EMGFlow/SignalFilterer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 emgflow-0.0.1/src/EMGFlow/__init__.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 emgflow-0.0.1/.gitignore
--rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 emgflow-0.0.1/LICENSE
--rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 emgflow-0.0.1/README.md
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 emgflow-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 emgflow-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     6069 2020-02-02 00:00:00.000000 emgflow-1.0.0/src/EMGFlow/OutlierFinder.py
+-rw-r--r--   0        0        0     8863 2020-02-02 00:00:00.000000 emgflow-1.0.0/src/EMGFlow/PlotSignals.py
+-rw-r--r--   0        0        0    49356 2020-02-02 00:00:00.000000 emgflow-1.0.0/src/EMGFlow/SignalFilterer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 emgflow-1.0.0/src/EMGFlow/__init__.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 emgflow-1.0.0/.gitignore
+-rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 emgflow-1.0.0/README.md
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 emgflow-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 emgflow-1.0.0/PKG-INFO
```

### Comparing `emgflow-0.0.1/src/EMGFlow/OutlierFinder.py` & `emgflow-1.0.0/src/EMGFlow/OutlierFinder.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-import neurokit2 as nk
 import pandas as pd
 import numpy as np
 import scipy.optimize
 import os
 import re
 from scipy.signal import argrelextrema
 from tqdm import tqdm
 
-from SignalFilterer import MapFiles
-from PlotSignals import PlotSpectrum
+from SignalFilterer import MapFiles, EMG2PSD
 
 #
 # =============================================================================
 #
 
 """
 A collection of functions for finding outliers while testing
@@ -109,15 +107,15 @@
             
             # Set to false
             isOutlier = False
             
             # Iterate over columns
             for i in range(len(cols)):
                 col = cols[i]
-                psd = nk.signal_psd(data[col], sampling_rate=sampling_rate)
+                psd = EMG2PSD(data[col], sampling_rate=sampling_rate)
                 psd = ZoomIn(psd, 20, 450)
                 
                 n = 200     # Width of band to check for local maxima in PSD
                 
                 # Create column containing local maxima
                 psd['max'] = psd.iloc[argrelextrema(psd['Power'].values, np.greater_equal, order=n)[0]]['Power']
                 
@@ -150,30 +148,8 @@
                     isOutlier = True
             
             # If any columns has an outlier, mark as an outlier
             if isOutlier:
                 # print('\tOutlier detected...')
                 outliers[file] = filedirs[file]
                 
-    return outliers
-
-#
-# =============================================================================
-#
-
-"""
-if __name__ == '__main__':
-    
-    raw_path = 'C:/Users/willi/Documents/UOIT/UOIT-Thesis/Data/01_Raw/'
-    notch_path = 'C:/Users/willi/Documents/UOIT/UOIT-Thesis/Data/02_Notch/'
-    notch_s_path = 'C:/Users/willi/Documents/UOIT/UOIT-Thesis/Data/02_Notch_Special/'
-    bandpass_path = 'C:/Users/willi/Documents/UOIT/UOIT-Thesis/Data/03_Bandpass/'
-    smooth_path = 'C:/Users/willi/Documents/UOIT/UOIT-Thesis/Data/04_Smooth/'
-    feature_path = 'C:/Users/willi/Documents/UOIT/UOIT-Thesis/Data/05_Feature/'
-    plot_path = 'C:/Users/willi/Documents/UOIT/UOIT-Thesis/Data/00_Plot/New/'
-    
-    sampling_rate = 2000
-    
-    outliers = DetectOutliers(notch_path, sampling_rate, 15, cols=['EMG_zyg', 'EMG_cor'])
-    
-    PlotSpectrum(outliers, plot_path, sampling_rate, cols=['EMG_zyg', 'EMG_cor'])
-"""  
+    return outliers
```

### Comparing `emgflow-0.0.1/src/EMGFlow/SignalFilterer.py` & `emgflow-1.0.0/src/EMGFlow/SignalFilterer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import scipy
 import pandas as pd
 import numpy as np
-import neurokit2 as nk
 import os
 import re
 import cv2
 from tqdm import tqdm
 
 #
 # =============================================================================
@@ -15,14 +14,74 @@
 A collection of functions for filtering Signals.
 """
 
 #
 # =============================================================================
 #
 
+"""
+    Creates a PSD graph of a Signal. Uses the Welch method, meaning it can be
+    used as a Long Term Average Spectrum (LTAS).
+
+    Parameters
+    ----------
+    Signal : DataFrame
+        A Pandas DataFrame containing a 'Time' column, and additional columns for signal data.
+    sampling_rate : float
+        Sampling rate of the Signal.
+    normalize : bool, optional
+        If True, will normalize the result. If False, will not. The default is True.
+
+    Returns
+    -------
+    psd : DataFrame
+        A DataFrame containing a 'Frequency' and 'Power' column. The Power column
+        indicates the intensity of each frequency in the Signal provided. Results
+        will be normalized if 'normalize' is set to True.
+"""
+def EMG2PSD(Signal, sr=1000, normalize=True):
+    # Initial parameters
+    Signal = Signal - np.mean(Signal)
+    N = len(Signal)
+    
+    # Calculate minimum frequency given sampling rate
+    min_frequency = (2 * sr) / (N / 2)
+    
+    # Calculate window size givern sampling rate
+    nperseg = int((2 / min_frequency) * sr)
+    nfft = nperseg * 2
+    
+    # Apply welch method with hanning window
+    frequency, power = scipy.signal.welch(
+        Signal,
+        fs=sr,
+        scaling='density',
+        detrend=False,
+        nfft=nfft,
+        average='mean',
+        nperseg=nperseg,
+        window='hann'
+    )
+    
+    # Normalize if set to true
+    if normalize is True:
+        power /= np.max(power)
+        
+    # Create dataframe of results
+    psd = pd.DataFrame({'Frequency': frequency, 'Power': power})
+    # Filter given 
+    psd = psd.loc[np.logical_and(psd['Frequency'] >= min_frequency,
+                                   psd['Frequency'] <= np.inf)]
+    
+    return psd
+
+#
+# =============================================================================
+#
+
 
 def MapFiles(in_path, file_ext='csv', expression=None):
     """
     Generate a dictionary of file names and locations from the subfiles of a folder.
     
     Parameters
     ----------
@@ -81,25 +140,79 @@
     # User provided a path to a folder
     if type(fileObj) is str:
         if not os.path.isabs(fileObj):
             fileObj = os.path.abspath(fileObj) + '\\'
         filedirs = MapFiles(in_path=fileObj, file_ext=file_ext, expression=expression)
     # User provided a processed file directory
     elif type(fileObj) is dict:
-        filedirs = fileObj
+        # If expression is provided, filters the dictionary
+        # for all entries matching it
+        fd = fileObj.copy()
+        if expression != None:
+            for file in fd:
+                if not (re.match(expression, fd[file])):
+                    del fd[file]
+        filedirs = fd
     # Provided file location format is unsupported
     else:
         raise Exception("Unsupported file location format:", type(fileObj))
     
     return filedirs
 
 #
 # =============================================================================
 #
 
+
+def MapFilesFuse(filedirs, names):
+    """
+    Generate a dictionary of file names and locations from different forms of input.
+
+    Parameters
+    ----------
+    filedirs : dict list
+        List of file location directories
+    names : str
+        List of names to use for file directory columns. Same order as file directories.
+
+    Raises
+    ------
+    Exception
+        If an unsupported file location format is provided, an exception is raised.
+
+    Returns
+    -------
+    filedirs : pd.DataFrame
+        A DataFrame of file names, and their locations in each file directory.
+    
+    """
+    
+    data = []
+    # Assumes all files listed in first file directory
+    # exists in the others
+    for file in filedirs[0].keys():
+        # Create row
+        row = [file, file]
+        for i, filedir in enumerate(filedirs):
+            if file not in filedir:
+                # Raise exception if file does not exist
+                raise Exception('File ' + file + ' does not exist in file directory ' + names[i])
+            row.append(filedir[file])
+        # Add row to data frame
+        data.append(row)
+    # Create data frame
+    df = pd.DataFrame(data, columns=['ID', 'File'] + names)
+    df.set_index('ID',inplace=True)
+    
+    return df
+
+#
+# =============================================================================
+#
+
 def ApplyNotchFilters(Signal, col, sampling_rate, notch_vals):
     """
     Apply a list of notch filters for given frequencies and Q-factors to a column of the provided data.
 
     Parameters
     ----------
     Signal : DataFrame
@@ -653,27 +766,27 @@
     """
     
     # Separate Signal1 by div and find spectral flux
     if isinstance(diff, float):
         # Find column divider index
         diff_ind = int(len(Signal1[col]) * diff)
         # Take the PSD of each signal
-        psd1 = nk.signal_psd(Signal1[col][:diff_ind], sampling_rate=sr)
-        psd2 = nk.signal_psd(Signal1[col][diff_ind:], sampling_rate=sr)
+        psd1 = EMG2PSD(Signal1[col][:diff_ind], sampling_rate=sr)
+        psd2 = EMG2PSD(Signal1[col][diff_ind:], sampling_rate=sr)
         # Calculate the spectral flux
         flux = np.sum((psd1['Power'] - psd2['Power']) ** 2)
         
     # Find spectral flux of Signal1 by div
     elif isinstance(diff, pd.DataFrame):
         
         # If no second sampling rate, assume same sampling rate as first Signal
         if diff_sr == None: diff_sr = sr
         # Take the PSD of each signal
-        psd1 = nk.signal_psd(Signal1[col], sampling_rate=sr)
-        psd2 = nk.signal_psd(diff[col], sampling_rate=diff_sr)
+        psd1 = EMG2PSD(Signal1[col], sampling_rate=sr)
+        psd2 = EMG2PSD(diff[col], sampling_rate=diff_sr)
         # Calculate the spectral flux
         flux = np.sum((psd1['Power'] - psd2['Power']) ** 2)
     
     return flux
 
 #
 # =============================================================================
@@ -1423,15 +1536,15 @@
                 WL = CalcWL(data_s, col)
                 LOG = CalcLOG(data_s, col)
                 MFL = CalcMFL(data_s, col)
                 AP = CalcAP(data_s, col)
                 Spectral_Flux = CalcSpecFlux(data_s, 0.5, col, sampling_rate)
     
                 # Calculate spectral features
-                psd = nk.signal_psd(data_b[col], sampling_rate=sampling_rate)
+                psd = EMG2PSD(data_b[col], sampling_rate=sampling_rate)
                 Max_Freq = psd.iloc[psd['Power'].idxmax()]['Frequency']
                 Twitch_Ratio = CalcTwitchRatio(psd)
                 Twitch_Index = CalcTwitchIndex(psd)
                 Fast_Twitch_Slope, Slow_Twitch_Slope = CalcTwitchSlope(psd)
                 Spectral_Centroid = CalcSC(psd)
                 Spectral_Flatness = CalcSF(psd)
                 Spectral_Spread = CalcSS(psd)
```

### Comparing `emgflow-0.0.1/README.md` & `emgflow-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `emgflow-0.0.1/PKG-INFO` & `emgflow-1.0.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,23 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: EMGFlow
-Version: 0.0.1
+Version: 1.0.0
 Summary: A general EMG processing and feature extraction package.
+Author: Steven Livingstone
 Author-email: William Conley <william@cconley.ca>
-License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: opencv-python
+Requires-Dist: pandas
+Requires-Dist: scipy
+Requires-Dist: tqdm
 Description-Content-Type: text/markdown
 
 # EMGFlow
 
 The EMG Workflow Toolkit (EMGFlow) was created to provide a more streamlined way to perform the processing of EMG signals in Python. The package provides modules for different steps in inspection, preprocessing, and analysis.
 
 The EMGFlow package stands out among others as it does not follow a strict pipeline, allowing users to use what functions they need, rather than forcing users to follow a specific series of functions.
```

