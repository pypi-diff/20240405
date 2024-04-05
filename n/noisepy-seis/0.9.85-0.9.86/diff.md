# Comparing `tmp/noisepy_seis-0.9.85.tar.gz` & `tmp/noisepy_seis-0.9.86.tar.gz`

## Comparing `noisepy_seis-0.9.85.tar` & `noisepy_seis-0.9.86.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0     9692 2020-02-02 00:00:00.000000 noisepy_seis-0.9.85/src/noisepy/functions_2019/S0B_to_ASDF_2019.py
--rw-r--r--   0        0        0    18752 2020-02-02 00:00:00.000000 noisepy_seis-0.9.85/src/noisepy/functions_2019/noise_module.py
--rw-r--r--   0        0        0    13312 2020-02-02 00:00:00.000000 noisepy_seis-0.9.85/src/noisepy/monitoring/esyn_utils.py
--rw-r--r--   0        0        0    50445 2020-02-02 00:00:00.000000 noisepy_seis-0.9.85/src/noisepy/monitoring/monitoring_utils.py
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 noisepy_seis-0.9.85/src/noisepy/seis/__init__.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 noisepy_seis-0.9.85/src/noisepy/seis/_version.py
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 noisepy_seis-0.9.85/src/noisepy/seis/constants.py
--rw-r--r--   0        0        0    20170 2020-02-02 00:00:00.000000 noisepy_seis-0.9.85/src/noisepy/seis/correlate.py
--rw-r--r--   0        0        0    11389 2020-02-02 00:00:00.000000 noisepy_seis-0.9.85/src/noisepy/seis/fdsn_download.py
--rw-r--r--   0        0        0    11900 2020-02-02 00:00:00.000000 noisepy_seis-0.9.85/src/noisepy/seis/main.py
--rw-r--r--   0        0        0    47901 2020-02-02 00:00:00.000000 noisepy_seis-0.9.85/src/noisepy/seis/noise_module.py
--rw-r--r--   0        0        0     4730 2020-02-02 00:00:00.000000 noisepy_seis-0.9.85/src/noisepy/seis/scheduler.py
--rw-r--r--   0        0        0    13880 2020-02-02 00:00:00.000000 noisepy_seis-0.9.85/src/noisepy/seis/stack.py
--rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 noisepy_seis-0.9.85/src/noisepy/seis/application_modules/dispersion_analysis.py
--rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 noisepy_seis-0.9.85/.gitignore
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 noisepy_seis-0.9.85/LICENSE
--rw-r--r--   0        0        0     8345 2020-02-02 00:00:00.000000 noisepy_seis-0.9.85/README.md
--rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 noisepy_seis-0.9.85/pyproject.toml
--rw-r--r--   0        0        0    11367 2020-02-02 00:00:00.000000 noisepy_seis-0.9.85/PKG-INFO
+-rw-r--r--   0        0        0     9692 2020-02-02 00:00:00.000000 noisepy_seis-0.9.86/src/noisepy/functions_2019/S0B_to_ASDF_2019.py
+-rw-r--r--   0        0        0    18752 2020-02-02 00:00:00.000000 noisepy_seis-0.9.86/src/noisepy/functions_2019/noise_module.py
+-rw-r--r--   0        0        0     5062 2020-02-02 00:00:00.000000 noisepy_seis-0.9.86/src/noisepy/monitoring/esyn_plotting.py
+-rw-r--r--   0        0        0    12439 2020-02-02 00:00:00.000000 noisepy_seis-0.9.86/src/noisepy/monitoring/esyn_utils.py
+-rw-r--r--   0        0        0    50445 2020-02-02 00:00:00.000000 noisepy_seis-0.9.86/src/noisepy/monitoring/monitoring_utils.py
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 noisepy_seis-0.9.86/src/noisepy/seis/__init__.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 noisepy_seis-0.9.86/src/noisepy/seis/_version.py
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 noisepy_seis-0.9.86/src/noisepy/seis/constants.py
+-rw-r--r--   0        0        0    20170 2020-02-02 00:00:00.000000 noisepy_seis-0.9.86/src/noisepy/seis/correlate.py
+-rw-r--r--   0        0        0    11389 2020-02-02 00:00:00.000000 noisepy_seis-0.9.86/src/noisepy/seis/fdsn_download.py
+-rw-r--r--   0        0        0    11894 2020-02-02 00:00:00.000000 noisepy_seis-0.9.86/src/noisepy/seis/main.py
+-rw-r--r--   0        0        0    47935 2020-02-02 00:00:00.000000 noisepy_seis-0.9.86/src/noisepy/seis/noise_module.py
+-rw-r--r--   0        0        0     4730 2020-02-02 00:00:00.000000 noisepy_seis-0.9.86/src/noisepy/seis/scheduler.py
+-rw-r--r--   0        0        0    13880 2020-02-02 00:00:00.000000 noisepy_seis-0.9.86/src/noisepy/seis/stack.py
+-rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 noisepy_seis-0.9.86/src/noisepy/seis/application_modules/dispersion_analysis.py
+-rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 noisepy_seis-0.9.86/.gitignore
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 noisepy_seis-0.9.86/LICENSE
+-rw-r--r--   0        0        0     8345 2020-02-02 00:00:00.000000 noisepy_seis-0.9.86/README.md
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 noisepy_seis-0.9.86/pyproject.toml
+-rw-r--r--   0        0        0    11396 2020-02-02 00:00:00.000000 noisepy_seis-0.9.86/PKG-INFO
```

### Comparing `noisepy_seis-0.9.85/src/noisepy/functions_2019/S0B_to_ASDF_2019.py` & `noisepy_seis-0.9.86/src/noisepy/functions_2019/S0B_to_ASDF_2019.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.85/src/noisepy/functions_2019/noise_module.py` & `noisepy_seis-0.9.86/src/noisepy/functions_2019/noise_module.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.85/src/noisepy/monitoring/esyn_utils.py` & `noisepy_seis-0.9.86/src/noisepy/monitoring/esyn_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,47 +1,24 @@
 import logging
 import math
 from typing import Tuple
 
 import numpy as np
-import pyasdf
 
 ### -----
 # These scripts are aim to perform the 2-D radiative transfer equation
 # for scalar waves (Shang and Gao 1988; Sato 1993),
 # assuming of isotropic scattering and source radiation in infinite medium
 # to calculate synthesized energy densities Esyn.
 ### -----
 
 logger = logging.getLogger(__name__)
 
 
 ### -----
-def read_pyasdf(sfile: str, ccomp: str) -> Tuple[float, float, np.ndarray, np.ndarray]:
-    # useful parameters from each asdf file
-    with pyasdf.ASDFDataSet(sfile, mode="r") as ds:
-        alist = ds.auxiliary_data.list()
-        try:
-            dt = ds.auxiliary_data[alist[0]][ccomp].parameters["dt"]
-            dist = ds.auxiliary_data[alist[0]][ccomp].parameters["dist"]
-            logger.info(f"working on {sfile} (comp: {ccomp}) that is {dist} km apart. dt: {dt}")
-            # read stacked data
-            sdata = ds.auxiliary_data[alist[0]][ccomp].data[:]
-
-            # time domain variables
-            npts = sdata.size
-            tvec = np.arange(-npts // 2 + 1, npts // 2 + 1) * dt
-            return dist, dt, tvec, sdata
-
-        except Exception:
-            logger.warning(f"continue! no {ccomp} component exist")
-            return None
-
-
-### -----
 # Function that Calculate Mean Square
 def msValue(arr: np.ndarray) -> np.ndarray:
     """
     # Mean-squared value calculation
     ----------------------------------------------
     Input:
         arr:  Input time series
@@ -248,15 +225,15 @@
             # plot_fitting_curves(mean_free,y,fmsv_mean[aa][0][:],Eobs_temp[nfree],Esyn_temp[nfree],fname[aa],vdist[aa],twindow)
         # logger.info(f"mean_free: {mean_free}, intrinsic_b {intrinsic_b}, SSR:{SSR_temp}")
         SSR_final = SSR_final / (np.min(SSR_final[:][:]))
 
     return SSR_final, mfpx, intby
 
 
-def get_optimal(fnum: int, para) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
+def get_optimal_Esyn(fnum: int, para) -> Tuple[np.ndarray, np.ndarray, np.ndarray, np.ndarray]:
     """
     # Getting the optimal value from the grid searching results (the SSR output from the get_SSR)
     # Return with the optimal value of mean free path, intrinsic absorption parameter
     # and the optimal fit of synthetic energy density function
     ----------------------------------------------
     Parameters:
         fb: the number of used frequency band
```

### Comparing `noisepy_seis-0.9.85/src/noisepy/monitoring/monitoring_utils.py` & `noisepy_seis-0.9.86/src/noisepy/monitoring/monitoring_utils.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.85/src/noisepy/seis/__init__.py` & `noisepy_seis-0.9.86/src/noisepy/seis/__init__.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.85/src/noisepy/seis/correlate.py` & `noisepy_seis-0.9.86/src/noisepy/seis/correlate.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.85/src/noisepy/seis/fdsn_download.py` & `noisepy_seis-0.9.86/src/noisepy/seis/fdsn_download.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.85/src/noisepy/seis/main.py` & `noisepy_seis-0.9.86/src/noisepy/seis/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from noisepy.seis.io.channel_filter_store import (
     LocationChannelFilterStore,
     channel_filter,
 )
 from noisepy.seis.io.channelcatalog import CSVChannelCatalog, XMLStationChannelCatalog
 from noisepy.seis.io.datatypes import ConfigParameters
 from noisepy.seis.io.numpystore import NumpyCCStore, NumpyStackStore
-from noisepy.seis.io.scedc_s3store import SCEDCS3DataStore
+from noisepy.seis.io.s3store import SCEDCS3DataStore
 from noisepy.seis.io.utils import fs_join, get_filesystem, io_retry
 from noisepy.seis.io.zarrstore import ZarrCCStore, ZarrStackStore
 
 from . import __version__
 from .constants import CONFIG_FILE, STATION_FILE
 from .correlate import cross_correlate
 from .fdsn_download import download
```

### Comparing `noisepy_seis-0.9.85/src/noisepy/seis/noise_module.py` & `noisepy_seis-0.9.86/src/noisepy/seis/noise_module.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,16 +160,14 @@
         # when starttimes are between sampling points
         fric = st[0].stats.starttime.microsecond % (delta * 1e6)
         if fric > 1e-4:
             st[0].data = segment_interpolate(np.float32(st[0].data), float(fric / (delta * 1e6)))
             # --reset the time to remove the discrepancy---
             st[0].stats.starttime -= fric * 1e-6
 
-    # remove traces of too small length
-
     # options to remove instrument response
     if rm_resp != RmResp.NO:
         if rm_resp != RmResp.INV:
             if (respdir is None) or (not os.path.isdir(respdir)):
                 raise ValueError("response file folder not found! abort!")
 
         if rm_resp == RmResp.INV:
@@ -184,34 +182,34 @@
                     st[0].attach_response(inv)
                     st[0].remove_response(output=rm_resp_out, pre_filt=pre_filt, water_level=60)
                 except Exception as e:
                     logger.warning("Failed to remove response from %s. Returning empty stream. %s" % (st[0], e))
                     st = []
                     return st
 
-        elif rm_resp == RmResp.SPECTRUM:
+        elif rm_resp == RmResp.SPECTRUM:  # TODO: to be implement
             logger.info("remove response using spectrum")
             specfile = glob.glob(os.path.join(respdir, "*" + station + "*"))
             if len(specfile) == 0:
                 raise ValueError("no response sepctrum found for %s" % station)
             st = resp_spectrum(st, specfile[0], samp_freq, pre_filt)
 
-        elif rm_resp == RmResp.RESP:
+        elif rm_resp == RmResp.RESP:  # TODO: to be implement
             logger.info("remove response using RESP files")
             resp = glob.glob(os.path.join(respdir, "RESP." + station + "*"))
             if len(resp) == 0:
                 raise ValueError("no RESP files found for %s" % station)
             seedresp = {
                 "filename": resp[0],
                 "date": starttime,
                 "units": "DIS",
             }
             st.simulate(paz_remove=None, pre_filt=pre_filt, seedresp=seedresp)
 
-        elif rm_resp == RmResp.POLES_ZEROS:
+        elif rm_resp == RmResp.POLES_ZEROS:  # TODO: to be implement
             logger.info("remove response using poles and zeros")
             paz_sts = glob.glob(os.path.join(respdir, "*" + station + "*"))
             if len(paz_sts) == 0:
                 raise ValueError("no poleszeros found for %s" % station)
             st.simulate(paz_remove=paz_sts[0], pre_filt=pre_filt)
 
         else:
```

### Comparing `noisepy_seis-0.9.85/src/noisepy/seis/scheduler.py` & `noisepy_seis-0.9.86/src/noisepy/seis/scheduler.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.85/src/noisepy/seis/stack.py` & `noisepy_seis-0.9.86/src/noisepy/seis/stack.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.85/src/noisepy/seis/application_modules/dispersion_analysis.py` & `noisepy_seis-0.9.86/src/noisepy/seis/application_modules/dispersion_analysis.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.85/.gitignore` & `noisepy_seis-0.9.86/.gitignore`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
+# noisepy-seis-io / dev
+src/noisepy/seis/io
+
 # C extensions
 *.so
 
 # Distribution / packaging
 .Python
 build/
 develop-eggs/
@@ -170,11 +173,12 @@
 
 # Temp locations for tutorials
 tutorials/get_started_data/
 tutorials/scedc_data/
 tutorials/ncedc_data/
 tutorials/cli/tmpdata
 tutorials/pnw_data
+tutorials/composite_data
 
 # Jupyterbook
 _build/
 log.txt
```

### Comparing `noisepy_seis-0.9.85/LICENSE` & `noisepy_seis-0.9.86/LICENSE`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.85/README.md` & `noisepy_seis-0.9.86/README.md`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.85/pyproject.toml` & `noisepy_seis-0.9.86/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,16 @@
     "s3fs==2023.4.0,<2024.0.0",
     "zarr==2.14.2",
     "aiobotocore==2.5.2", # "2.5.3 is broken"
     "pydantic==2.3.0",
     "PyYAML==6.0",
     "pydantic-yaml==1.0",
     "psutil>=5.9.5,<6.0.0",
-    "noisepy-seis-io>=0.1.11",
+    "noisepy-seis-io>=0.1.13",
+    "scipy==1.12.0"
 ]
 
 
 [project.urls]
 Homepage = "https://github.com/noisepy/NoisePy"
 
 [tool.hatch.version]
```

### Comparing `noisepy_seis-0.9.85/PKG-INFO` & `noisepy_seis-0.9.86/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: noisepy-seis
-Version: 0.9.85
+Version: 0.9.86
 Summary: A High-performance Computing Python Package for Ambient Noise Analysis
 Project-URL: Homepage, https://github.com/noisepy/NoisePy
 Author-email: Marine Denolle <mdenolle@uw.edu>, Chengxin Jiang <Chengxin.Jiang1@anu.edu.au>, Yiyu Ni <niyiyu@uw.edu>
 License: MIT License
         
         Copyright (c) 2019 Marine Denolle & Chengxin Jiang
         
@@ -34,25 +34,26 @@
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: <3.11,>=3.9
 Requires-Dist: aiobotocore==2.5.2
 Requires-Dist: datetimerange<3.0.0,>=2.0.0
 Requires-Dist: diskcache<6.0.0,>=5.6.1
 Requires-Dist: fsspec<2024.0.0,>=2023.4.0
 Requires-Dist: h5py<4.0.0,>=3.8.0
-Requires-Dist: noisepy-seis-io>=0.1.11
+Requires-Dist: noisepy-seis-io>=0.1.13
 Requires-Dist: numba<1.0.0,>=0.57.0
 Requires-Dist: numpy<2.0.0,>=1.22.0
 Requires-Dist: pandas<2.0.0,>=1.5.3
 Requires-Dist: psutil<6.0.0,>=5.9.5
 Requires-Dist: pyasdf<1.0.0,>=0.7.5
 Requires-Dist: pycwt<1.0.0,>=0.3.0a22
 Requires-Dist: pydantic-yaml==1.0
 Requires-Dist: pydantic==2.3.0
 Requires-Dist: pyyaml==6.0
 Requires-Dist: s3fs<2024.0.0,==2023.4.0
+Requires-Dist: scipy==1.12.0
 Requires-Dist: zarr==2.14.2
 Provides-Extra: aws
 Requires-Dist: boto3<2.0.0,>=1.26.0; extra == 'aws'
 Provides-Extra: dev
 Requires-Dist: memory-profiler==0.61; extra == 'dev'
 Requires-Dist: pre-commit==3.3.3; extra == 'dev'
 Requires-Dist: pytest-cov==4.1.0; extra == 'dev'
```

