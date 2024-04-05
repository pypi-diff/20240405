# Comparing `tmp/GalSim-2.5.0.tar.gz` & `tmp/GalSim-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GalSim-2.5.0.tar", last modified: Mon Oct 16 20:55:17 2023, max compression
+gzip compressed data, was "GalSim-2.5.1.tar", last modified: Thu Nov  2 02:09:41 2023, max compression
```

## Comparing `GalSim-2.5.0.tar` & `GalSim-2.5.1.tar`

### file list

```diff
@@ -1,769 +1,769 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 20:55:17.380813 GalSim-2.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     4516 2023-10-16 20:54:09.000000 GalSim-2.5.0/CHANGELOG.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 20:55:17.124816 GalSim-2.5.0/GalSim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10310 2023-10-16 20:55:16.000000 GalSim-2.5.0/GalSim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    24094 2023-10-16 20:55:17.000000 GalSim-2.5.0/GalSim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-16 20:55:16.000000 GalSim-2.5.0/GalSim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      109 2023-10-16 20:55:16.000000 GalSim-2.5.0/GalSim.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-16 20:55:16.000000 GalSim-2.5.0/GalSim.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       64 2023-10-16 20:55:16.000000 GalSim-2.5.0/GalSim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-10-16 20:55:16.000000 GalSim-2.5.0/GalSim.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2023-10-16 20:54:09.000000 GalSim-2.5.0/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2023-10-16 20:54:09.000000 GalSim-2.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      240 2023-10-16 20:54:09.000000 GalSim-2.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10310 2023-10-16 20:55:17.380813 GalSim-2.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9796 2023-10-16 20:54:09.000000 GalSim-2.5.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 20:55:17.144816 GalSim-2.5.0/galsim/
--rw-r--r--   0 runner    (1001) docker     (127)     6370 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/_pyfits.py
--rw-r--r--   0 runner    (1001) docker     (127)    11884 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    10442 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/airy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/angle.py
--rw-r--r--   0 runner    (1001) docker     (127)    33296 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/bandpass.py
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/bessel.py
--rw-r--r--   0 runner    (1001) docker     (127)    18607 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/bounds.py
--rw-r--r--   0 runner    (1001) docker     (127)     8837 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/box.py
--rw-r--r--   0 runner    (1001) docker     (127)    23094 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)    11816 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/cdmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)      860 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/celestial.py
--rw-r--r--   0 runner    (1001) docker     (127)   177903 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/chromatic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 20:55:17.152816 GalSim-2.5.0/galsim/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6942 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/config/bandpass.py
--rw-r--r--   0 runner    (1001) docker     (127)    23329 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/config/extra.py
--rw-r--r--   0 runner    (1001) docker     (127)     3118 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/config/extra_badpix.py
--rw-r--r--   0 runner    (1001) docker     (127)     6416 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/config/extra_psf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5390 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/config/extra_truth.py
--rw-r--r--   0 runner    (1001) docker     (127)     4155 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/config/extra_weight.py
--rw-r--r--   0 runner    (1001) docker     (127)    25714 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/config/gsobject.py
--rw-r--r--   0 runner    (1001) docker     (127)    26118 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/config/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     9108 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/config/image_scattered.py
--rw-r--r--   0 runner    (1001) docker     (127)    11091 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/config/image_tiled.py
--rw-r--r--   0 runner    (1001) docker     (127)    32708 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/config/input.py
--rw-r--r--   0 runner    (1001) docker     (127)     7363 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/config/input_cosmos.py
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/config/input_fitsheader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/config/input_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     4163 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/config/input_nfw.py
--rw-r--r--   0 runner    (1001) docker     (127)    12494 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/config/input_powerspectrum.py
--rw-r--r--   0 runner    (1001) docker     (127)     5448 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/config/input_real.py
--rw-r--r--   0 runner    (1001) docker     (127)    28896 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/config/noise.py
--rw-r--r--   0 runner    (1001) docker     (127)    24343 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/config/output.py
--rw-r--r--   0 runner    (1001) docker     (127)     5595 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/config/output_datacube.py
--rw-r--r--   0 runner    (1001) docker     (127)     3475 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/config/output_multifits.py
--rw-r--r--   0 runner    (1001) docker     (127)    11659 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/config/photon_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)    13833 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/config/process.py
--rw-r--r--   0 runner    (1001) docker     (127)     7260 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/config/sed.py
--rw-r--r--   0 runner    (1001) docker     (127)     8437 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/config/sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)    56378 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/config/stamp.py
--rw-r--r--   0 runner    (1001) docker     (127)     7797 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/config/stamp_ring.py
--rw-r--r--   0 runner    (1001) docker     (127)    46057 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/config/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    34861 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/config/value.py
--rw-r--r--   0 runner    (1001) docker     (127)     8143 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/config/value_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)    10997 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/config/value_random.py
--rw-r--r--   0 runner    (1001) docker     (127)    12661 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/config/wcs.py
--rw-r--r--   0 runner    (1001) docker     (127)    40905 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/convolve.py
--rw-r--r--   0 runner    (1001) docker     (127)    88081 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/correlatednoise.py
--rw-r--r--   0 runner    (1001) docker     (127)     7407 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/dcr.py
--rw-r--r--   0 runner    (1001) docker     (127)     3171 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/deltafunction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 20:55:17.156816 GalSim-2.5.0/galsim/deprecated/
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/deprecated/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/deprecated/correlatednoise.py
--rw-r--r--   0 runner    (1001) docker     (127)     2772 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/deprecated/integ.py
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/deprecated/randwalk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 20:55:17.156816 GalSim-2.5.0/galsim/des/
--rw-r--r--   0 runner    (1001) docker     (127)      871 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/des/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26420 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/des/des_meds.py
--rw-r--r--   0 runner    (1001) docker     (127)    17509 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/des/des_psfex.py
--rw-r--r--   0 runner    (1001) docker     (127)     9656 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/des/des_shapelet.py
--rw-r--r--   0 runner    (1001) docker     (127)    17521 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/detectors.py
--rw-r--r--   0 runner    (1001) docker     (127)    21051 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/download_cosmos.py
--rw-r--r--   0 runner    (1001) docker     (127)    18816 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     6122 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/exponential.py
--rw-r--r--   0 runner    (1001) docker     (127)    10811 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/fft.py
--rw-r--r--   0 runner    (1001) docker     (127)    65426 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/fits.py
--rw-r--r--   0 runner    (1001) docker     (127)    83625 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/fitswcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7721 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/fouriersqrt.py
--rw-r--r--   0 runner    (1001) docker     (127)    50015 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/galaxy_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     6856 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)   131545 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/gsobject.py
--rw-r--r--   0 runner    (1001) docker     (127)    14402 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/gsparams.py
--rw-r--r--   0 runner    (1001) docker     (127)    42279 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/hsm.py
--rw-r--r--   0 runner    (1001) docker     (127)    83850 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    21169 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/inclined.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 20:55:17.160816 GalSim-2.5.0/galsim/include/
--rw-r--r--   0 runner    (1001) docker     (127)     2590 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/GalSim.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 20:55:17.160816 GalSim-2.5.0/galsim/include/fftw3/
--rw-r--r--   0 runner    (1001) docker     (127)    16123 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/fftw3/fftw3.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 20:55:17.180815 GalSim-2.5.0/galsim/include/galsim/
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/BinomFact.h
--rw-r--r--   0 runner    (1001) docker     (127)    17940 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/Bounds.h
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/CDModel.h
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/CorrelatedNoise.h
--rw-r--r--   0 runner    (1001) docker     (127)     9273 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/GSParams.h
--rw-r--r--   0 runner    (1001) docker     (127)    31400 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/Image.h
--rw-r--r--   0 runner    (1001) docker     (127)    21782 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/ImageArith.h
--rw-r--r--   0 runner    (1001) docker     (127)    20810 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/Interpolant.h
--rw-r--r--   0 runner    (1001) docker     (127)     8403 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/LRUCache.h
--rw-r--r--   0 runner    (1001) docker     (127)    15876 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/Laguerre.h
--rw-r--r--   0 runner    (1001) docker     (127)    12225 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/OneDimensionalDeviate.h
--rw-r--r--   0 runner    (1001) docker     (127)    11797 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/PhotonArray.h
--rw-r--r--   0 runner    (1001) docker     (127)     3924 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/Polygon.h
--rw-r--r--   0 runner    (1001) docker     (127)    16757 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/ProbabilityTree.h
--rw-r--r--   0 runner    (1001) docker     (127)    34396 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/Random.h
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/RealGalaxy.h
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/SBAdd.h
--rw-r--r--   0 runner    (1001) docker     (127)     9374 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/SBAddImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)     3046 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/SBAiry.h
--rw-r--r--   0 runner    (1001) docker     (127)    12047 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/SBAiryImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)     3535 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/SBBox.h
--rw-r--r--   0 runner    (1001) docker     (127)     9712 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/SBBoxImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)     6744 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/SBConvolve.h
--rw-r--r--   0 runner    (1001) docker     (127)    13052 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/SBConvolveImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/SBDeconvolve.h
--rw-r--r--   0 runner    (1001) docker     (127)     4086 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/SBDeconvolveImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/SBDeltaFunction.h
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/SBDeltaFunctionImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)     2609 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/SBExponential.h
--rw-r--r--   0 runner    (1001) docker     (127)     8093 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/SBExponentialImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/SBFourierSqrt.h
--rw-r--r--   0 runner    (1001) docker     (127)     3820 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/SBFourierSqrtImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/SBGaussian.h
--rw-r--r--   0 runner    (1001) docker     (127)     5739 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/SBGaussianImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)     3244 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/SBInclinedExponential.h
--rw-r--r--   0 runner    (1001) docker     (127)     6140 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/SBInclinedExponentialImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)     4212 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/SBInclinedSersic.h
--rw-r--r--   0 runner    (1001) docker     (127)     6245 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/SBInclinedSersicImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)     7185 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/SBInterpolatedImage.h
--rw-r--r--   0 runner    (1001) docker     (127)    11555 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/SBInterpolatedImageImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)     2808 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/SBKolmogorov.h
--rw-r--r--   0 runner    (1001) docker     (127)     7989 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/SBKolmogorovImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/SBMoffat.h
--rw-r--r--   0 runner    (1001) docker     (127)     8095 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/SBMoffatImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)    16789 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/SBProfile.h
--rw-r--r--   0 runner    (1001) docker     (127)     9531 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/SBProfileImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/SBSecondKick.h
--rw-r--r--   0 runner    (1001) docker     (127)     3981 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/SBSecondKickImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)     6056 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/SBSersic.h
--rw-r--r--   0 runner    (1001) docker     (127)    11563 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/SBSersicImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)     2308 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/SBShapelet.h
--rw-r--r--   0 runner    (1001) docker     (127)     4971 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/SBShapeletImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)     3813 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/SBSpergel.h
--rw-r--r--   0 runner    (1001) docker     (127)     9598 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/SBSpergelImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)     3132 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/SBTransform.h
--rw-r--r--   0 runner    (1001) docker     (127)    10313 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/SBTransformImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/SBVonKarman.h
--rw-r--r--   0 runner    (1001) docker     (127)     5998 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/SBVonKarmanImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)    12343 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/Silicon.h
--rw-r--r--   0 runner    (1001) docker     (127)    16801 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/Solve.h
--rw-r--r--   0 runner    (1001) docker     (127)     8138 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/Std.h
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/Stopwatch.h
--rw-r--r--   0 runner    (1001) docker     (127)     6072 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/Table.h
--rw-r--r--   0 runner    (1001) docker     (127)      965 2023-10-16 20:55:16.000000 GalSim-2.5.0/galsim/include/galsim/Version.h
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/WCS.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 20:55:17.180815 GalSim-2.5.0/galsim/include/galsim/boost1_48_0/
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/boost1_48_0/LICENSE_1_0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/boost1_48_0/README
--rw-r--r--   0 runner    (1001) docker     (127)     4118 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/boost1_48_0/assert.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 20:55:17.180815 GalSim-2.5.0/galsim/include/galsim/boost1_48_0/config/
--rw-r--r--   0 runner    (1001) docker     (127)    21149 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/boost1_48_0/config/suffix.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/boost1_48_0/current_function.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 20:55:17.184815 GalSim-2.5.0/galsim/include/galsim/boost1_48_0/random/
--rw-r--r--   0 runner    (1001) docker     (127)    12400 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/boost1_48_0/random/binomial_distribution.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6388 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/boost1_48_0/random/chi_squared_distribution.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 20:55:17.188815 GalSim-2.5.0/galsim/include/galsim/boost1_48_0/random/detail/
--rw-r--r--   0 runner    (1001) docker     (127)      929 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/boost1_48_0/random/detail/generator_seed_seq.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2950 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/boost1_48_0/random/detail/ptr_helper.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5418 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/boost1_48_0/random/detail/seed.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2420 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/boost1_48_0/random/detail/signed_unsigned_tools.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5728 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/boost1_48_0/random/exponential_distribution.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     9414 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/boost1_48_0/random/gamma_distribution.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    19903 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/boost1_48_0/random/mersenne_twister.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7472 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/boost1_48_0/random/normal_distribution.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    10295 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/boost1_48_0/random/poisson_distribution.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7982 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/boost1_48_0/random/uniform_01.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8594 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/boost1_48_0/random/uniform_real_distribution.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5679 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/boost1_48_0/random/weibull_distribution.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 20:55:17.192815 GalSim-2.5.0/galsim/include/galsim/fmath/
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/fmath/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      419 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/fmath/README
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/fmath/avx2.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    11454 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/fmath/bench.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/fmath/bench.sln
--rw-r--r--   0 runner    (1001) docker     (127)     7420 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/fmath/bench.vcproj
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/fmath/ck.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    37235 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/fmath/fastexp.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    23954 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/fmath/fmath.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 20:55:17.116816 GalSim-2.5.0/galsim/include/galsim/fmath/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 20:55:17.192815 GalSim-2.5.0/galsim/include/galsim/fmath/include/cybozu/
--rw-r--r--   0 runner    (1001) docker     (127)     3896 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/fmath/include/cybozu/benchmark.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/fmath/include/cybozu/inttype.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/fmath/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)     5899 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/fmath/readme.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 20:55:17.192815 GalSim-2.5.0/galsim/include/galsim/hsm/
--rw-r--r--   0 runner    (1001) docker     (127)    28148 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/hsm/PSFCorr.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 20:55:17.192815 GalSim-2.5.0/galsim/include/galsim/integ/
--rw-r--r--   0 runner    (1001) docker     (127)    42773 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/integ/Int.h
--rw-r--r--   0 runner    (1001) docker     (127)    12112 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/integ/IntGKPData1.h
--rw-r--r--   0 runner    (1001) docker     (127)    17415 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/integ/IntGKPData10.h
--rw-r--r--   0 runner    (1001) docker     (127)    32193 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/integ/MoreFunctional.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 20:55:17.196815 GalSim-2.5.0/galsim/include/galsim/math/
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/math/Angle.h
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/math/Bessel.h
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/math/Gamma.h
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/math/Hankel.h
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/math/Horner.h
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/math/Nan.h
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/math/Sinc.h
--rw-r--r--   0 runner    (1001) docker     (127)     8299 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/include/galsim/mmgr.h
--rw-r--r--   0 runner    (1001) docker     (127)    16748 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/integ.py
--rw-r--r--   0 runner    (1001) docker     (127)    24196 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/interpolant.py
--rw-r--r--   0 runner    (1001) docker     (127)    58093 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/interpolatedimage.py
--rw-r--r--   0 runner    (1001) docker     (127)    12961 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/knots.py
--rw-r--r--   0 runner    (1001) docker     (127)    13408 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/kolmogorov.py
--rw-r--r--   0 runner    (1001) docker     (127)    77477 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/lensing_ps.py
--rw-r--r--   0 runner    (1001) docker     (127)     9312 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/meta_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     9009 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/moffat.py
--rw-r--r--   0 runner    (1001) docker     (127)    20598 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/nfw_halo.py
--rw-r--r--   0 runner    (1001) docker     (127)    25981 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/noise.py
--rw-r--r--   0 runner    (1001) docker     (127)   107542 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/phase_psf.py
--rw-r--r--   0 runner    (1001) docker     (127)    62861 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/phase_screens.py
--rw-r--r--   0 runner    (1001) docker     (127)    55325 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/photon_array.py
--rw-r--r--   0 runner    (1001) docker     (127)    11746 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/position.py
--rw-r--r--   0 runner    (1001) docker     (127)    14511 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/pse.py
--rw-r--r--   0 runner    (1001) docker     (127)    39945 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/random.py
--rw-r--r--   0 runner    (1001) docker     (127)    70030 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/real.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 20:55:17.200815 GalSim-2.5.0/galsim/roman/
--rw-r--r--   0 runner    (1001) docker     (127)     4125 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/roman/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7113 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/roman/roman_backgrounds.py
--rw-r--r--   0 runner    (1001) docker     (127)     8082 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/roman/roman_bandpass.py
--rw-r--r--   0 runner    (1001) docker     (127)    12680 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/roman/roman_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    10748 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/roman/roman_detectors.py
--rw-r--r--   0 runner    (1001) docker     (127)    22797 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/roman/roman_psfs.py
--rw-r--r--   0 runner    (1001) docker     (127)    32871 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/roman/roman_wcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9875 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/second_kick.py
--rw-r--r--   0 runner    (1001) docker     (127)    56949 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/sed.py
--rw-r--r--   0 runner    (1001) docker     (127)    24844 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)    18752 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/sersic.py
--rw-r--r--   0 runner    (1001) docker     (127)    11563 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/shapelet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 20:55:17.200815 GalSim-2.5.0/galsim/share/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 20:55:17.204815 GalSim-2.5.0/galsim/share/SEDs/
--rw-r--r--   0 runner    (1001) docker     (127)    12280 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/SEDs/CWW_E_ext.sed
--rw-r--r--   0 runner    (1001) docker     (127)     7392 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/SEDs/CWW_E_ext_more.sed
--rw-r--r--   0 runner    (1001) docker     (127)    12021 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/SEDs/CWW_Im_ext.sed
--rw-r--r--   0 runner    (1001) docker     (127)     8017 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/SEDs/CWW_Im_ext_more.sed
--rw-r--r--   0 runner    (1001) docker     (127)    13010 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/SEDs/CWW_Sbc_ext.sed
--rw-r--r--   0 runner    (1001) docker     (127)     8460 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/SEDs/CWW_Sbc_ext_more.sed
--rw-r--r--   0 runner    (1001) docker     (127)    12932 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/SEDs/CWW_Scd_ext.sed
--rw-r--r--   0 runner    (1001) docker     (127)     8356 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/SEDs/CWW_Scd_ext_more.sed
--rw-r--r--   0 runner    (1001) docker     (127)      242 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/SEDs/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)   102422 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/SEDs/vega.txt
--rw-r--r--   0 runner    (1001) docker     (127)    57600 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/acs_I_unrot_sci_20_cf.fits
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 20:55:17.212815 GalSim-2.5.0/galsim/share/bandpasses/
--rw-r--r--   0 runner    (1001) docker     (127)     5885 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/bandpasses/ACS_wfc_F435W.dat
--rw-r--r--   0 runner    (1001) docker     (127)    11657 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/bandpasses/ACS_wfc_F606W.dat
--rw-r--r--   0 runner    (1001) docker     (127)     4611 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/bandpasses/ACS_wfc_F775W.dat
--rw-r--r--   0 runner    (1001) docker     (127)     8823 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/bandpasses/ACS_wfc_F814W.dat
--rw-r--r--   0 runner    (1001) docker     (127)     4093 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/bandpasses/ACS_wfc_F850LP.dat
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/bandpasses/LSST_g.dat
--rw-r--r--   0 runner    (1001) docker     (127)     3384 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/bandpasses/LSST_i.dat
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/bandpasses/LSST_r.dat
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/bandpasses/LSST_u.dat
--rw-r--r--   0 runner    (1001) docker     (127)     6036 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/bandpasses/LSST_y.dat
--rw-r--r--   0 runner    (1001) docker     (127)     3410 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/bandpasses/LSST_z.dat
--rw-r--r--   0 runner    (1001) docker     (127)      238 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/bandpasses/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/bandpasses/WFC3_ir_F105W.dat
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/bandpasses/WFC3_ir_F125W.dat
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/bandpasses/WFC3_ir_F160W.dat
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/bandpasses/WFC3_uvis_F275W.dat
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/bandpasses/WFC3_uvis_F336W.dat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 20:55:17.240815 GalSim-2.5.0/galsim/share/roman/
--rw-r--r--   0 runner    (1001) docker     (127)    72363 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_F184_SCA_1.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    72815 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_F184_SCA_10.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    71900 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_F184_SCA_11.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    71312 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_F184_SCA_12.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    73332 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_F184_SCA_13.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    73256 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_F184_SCA_14.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    72231 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_F184_SCA_15.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    75714 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_F184_SCA_16.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    73288 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_F184_SCA_17.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    72988 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_F184_SCA_18.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    72683 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_F184_SCA_2.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    71938 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_F184_SCA_3.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    72860 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_F184_SCA_4.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    72153 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_F184_SCA_5.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    71630 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_F184_SCA_6.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    76049 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_F184_SCA_7.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    73119 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_F184_SCA_8.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    72505 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_F184_SCA_9.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    74944 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_skinny_SCA_1.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    74222 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_skinny_SCA_10.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    73499 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_skinny_SCA_11.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    72953 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_skinny_SCA_12.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    77295 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_skinny_SCA_13.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    73917 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_skinny_SCA_14.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    73364 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_skinny_SCA_15.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    77941 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_skinny_SCA_16.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    78030 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_skinny_SCA_17.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    77598 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_skinny_SCA_18.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    74701 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_skinny_SCA_2.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    73506 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_skinny_SCA_3.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    78098 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_skinny_SCA_4.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    75183 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_skinny_SCA_5.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    73645 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_skinny_SCA_6.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    77605 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_skinny_SCA_7.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    77370 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_skinny_SCA_8.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    77167 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_skinny_SCA_9.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_03.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_04.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_05.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_06.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_07.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_08.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_09.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_10.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_11.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_12.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_13.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_14.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_15.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_16.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_17.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_18.txt
--rw-r--r--   0 runner    (1001) docker     (127)   204929 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/roman/Roman_SRR_WFC_Pupil_Mask_Longwave_2048_reformatted.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)   207326 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/roman/Roman_SRR_WFC_Pupil_Mask_Shortwave_2048_reformatted.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    53490 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/roman/Roman_effarea_20210614.txt
--rw-r--r--   0 runner    (1001) docker     (127)   206809 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/roman/roman_sky_backgrounds.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/roman/sca_positions_20210204.txt
--rw-r--r--   0 runner    (1001) docker     (127)    16920 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/roman/sip_20210204.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 20:55:17.248815 GalSim-2.5.0/galsim/share/sensors/
--rw-r--r--   0 runner    (1001) docker     (127)     5054 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/sensors/abs_length.dat
--rw-r--r--   0 runner    (1001) docker     (127)    10297 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/sensors/lsst_e2v_32.cfg
--rw-r--r--   0 runner    (1001) docker     (127)   812668 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/sensors/lsst_e2v_32.dat
--rw-r--r--   0 runner    (1001) docker     (127)    10060 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/sensors/lsst_e2v_50_32.cfg
--rw-r--r--   0 runner    (1001) docker     (127)   812668 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/sensors/lsst_e2v_50_32.dat
--rw-r--r--   0 runner    (1001) docker     (127)    10061 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/sensors/lsst_e2v_50_8.cfg
--rw-r--r--   0 runner    (1001) docker     (127)   221692 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/sensors/lsst_e2v_50_8.dat
--rw-r--r--   0 runner    (1001) docker     (127)    10296 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/sensors/lsst_e2v_8.cfg
--rw-r--r--   0 runner    (1001) docker     (127)   221692 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/sensors/lsst_e2v_8.dat
--rw-r--r--   0 runner    (1001) docker     (127)    10365 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/sensors/lsst_itl_32.cfg
--rw-r--r--   0 runner    (1001) docker     (127)   812668 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/sensors/lsst_itl_32.dat
--rw-r--r--   0 runner    (1001) docker     (127)    10374 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/sensors/lsst_itl_50_32.cfg
--rw-r--r--   0 runner    (1001) docker     (127)   812668 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/sensors/lsst_itl_50_32.dat
--rw-r--r--   0 runner    (1001) docker     (127)    10375 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/sensors/lsst_itl_50_8.cfg
--rw-r--r--   0 runner    (1001) docker     (127)   221692 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/sensors/lsst_itl_50_8.dat
--rw-r--r--   0 runner    (1001) docker     (127)    10365 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/sensors/lsst_itl_8.cfg
--rw-r--r--   0 runner    (1001) docker     (127)   221692 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/sensors/lsst_itl_8.dat
--rw-r--r--   0 runner    (1001) docker     (127)   122780 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/share/wfc_F814W.dat.gz
--rw-r--r--   0 runner    (1001) docker     (127)    17179 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/shear.py
--rw-r--r--   0 runner    (1001) docker     (127)    10472 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/spergel.py
--rw-r--r--   0 runner    (1001) docker     (127)    14283 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/sum.py
--rw-r--r--   0 runner    (1001) docker     (127)    52931 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/table.py
--rw-r--r--   0 runner    (1001) docker     (127)    26406 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/transform.py
--rw-r--r--   0 runner    (1001) docker     (127)    74404 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    13078 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/vonkarman.py
--rw-r--r--   0 runner    (1001) docker     (127)   121121 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/wcs.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/wfirst.py
--rw-r--r--   0 runner    (1001) docker     (127)    57604 2023-10-16 20:54:10.000000 GalSim-2.5.0/galsim/zernike.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 20:55:17.252815 GalSim-2.5.0/include/
--rw-r--r--   0 runner    (1001) docker     (127)     2590 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/GalSim.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 20:55:17.252815 GalSim-2.5.0/include/fftw3/
--rw-r--r--   0 runner    (1001) docker     (127)    16123 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/fftw3/fftw3.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 20:55:17.272814 GalSim-2.5.0/include/galsim/
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/BinomFact.h
--rw-r--r--   0 runner    (1001) docker     (127)    17940 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/Bounds.h
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/CDModel.h
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/CorrelatedNoise.h
--rw-r--r--   0 runner    (1001) docker     (127)     9273 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/GSParams.h
--rw-r--r--   0 runner    (1001) docker     (127)    31400 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/Image.h
--rw-r--r--   0 runner    (1001) docker     (127)    21782 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/ImageArith.h
--rw-r--r--   0 runner    (1001) docker     (127)    20810 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/Interpolant.h
--rw-r--r--   0 runner    (1001) docker     (127)     8403 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/LRUCache.h
--rw-r--r--   0 runner    (1001) docker     (127)    15876 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/Laguerre.h
--rw-r--r--   0 runner    (1001) docker     (127)    12225 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/OneDimensionalDeviate.h
--rw-r--r--   0 runner    (1001) docker     (127)    11797 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/PhotonArray.h
--rw-r--r--   0 runner    (1001) docker     (127)     3924 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/Polygon.h
--rw-r--r--   0 runner    (1001) docker     (127)    16757 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/ProbabilityTree.h
--rw-r--r--   0 runner    (1001) docker     (127)    34396 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/Random.h
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/RealGalaxy.h
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/SBAdd.h
--rw-r--r--   0 runner    (1001) docker     (127)     9374 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/SBAddImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)     3046 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/SBAiry.h
--rw-r--r--   0 runner    (1001) docker     (127)    12047 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/SBAiryImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)     3535 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/SBBox.h
--rw-r--r--   0 runner    (1001) docker     (127)     9712 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/SBBoxImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)     6744 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/SBConvolve.h
--rw-r--r--   0 runner    (1001) docker     (127)    13052 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/SBConvolveImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/SBDeconvolve.h
--rw-r--r--   0 runner    (1001) docker     (127)     4086 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/SBDeconvolveImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/SBDeltaFunction.h
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/SBDeltaFunctionImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)     2609 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/SBExponential.h
--rw-r--r--   0 runner    (1001) docker     (127)     8093 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/SBExponentialImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/SBFourierSqrt.h
--rw-r--r--   0 runner    (1001) docker     (127)     3820 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/SBFourierSqrtImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/SBGaussian.h
--rw-r--r--   0 runner    (1001) docker     (127)     5739 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/SBGaussianImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)     3244 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/SBInclinedExponential.h
--rw-r--r--   0 runner    (1001) docker     (127)     6140 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/SBInclinedExponentialImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)     4212 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/SBInclinedSersic.h
--rw-r--r--   0 runner    (1001) docker     (127)     6245 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/SBInclinedSersicImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)     7185 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/SBInterpolatedImage.h
--rw-r--r--   0 runner    (1001) docker     (127)    11555 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/SBInterpolatedImageImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)     2808 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/SBKolmogorov.h
--rw-r--r--   0 runner    (1001) docker     (127)     7989 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/SBKolmogorovImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/SBMoffat.h
--rw-r--r--   0 runner    (1001) docker     (127)     8095 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/SBMoffatImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)    16789 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/SBProfile.h
--rw-r--r--   0 runner    (1001) docker     (127)     9531 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/SBProfileImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/SBSecondKick.h
--rw-r--r--   0 runner    (1001) docker     (127)     3981 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/SBSecondKickImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)     6056 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/SBSersic.h
--rw-r--r--   0 runner    (1001) docker     (127)    11563 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/SBSersicImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)     2308 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/SBShapelet.h
--rw-r--r--   0 runner    (1001) docker     (127)     4971 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/SBShapeletImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)     3813 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/SBSpergel.h
--rw-r--r--   0 runner    (1001) docker     (127)     9598 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/SBSpergelImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)     3132 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/SBTransform.h
--rw-r--r--   0 runner    (1001) docker     (127)    10313 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/SBTransformImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/SBVonKarman.h
--rw-r--r--   0 runner    (1001) docker     (127)     5998 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/SBVonKarmanImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)    12343 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/Silicon.h
--rw-r--r--   0 runner    (1001) docker     (127)    16801 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/Solve.h
--rw-r--r--   0 runner    (1001) docker     (127)     8138 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/Std.h
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/Stopwatch.h
--rw-r--r--   0 runner    (1001) docker     (127)     6072 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/Table.h
--rw-r--r--   0 runner    (1001) docker     (127)      965 2023-10-16 20:55:16.000000 GalSim-2.5.0/include/galsim/Version.h
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/WCS.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 20:55:17.276814 GalSim-2.5.0/include/galsim/boost1_48_0/
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/boost1_48_0/LICENSE_1_0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/boost1_48_0/README
--rw-r--r--   0 runner    (1001) docker     (127)     4118 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/boost1_48_0/assert.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 20:55:17.276814 GalSim-2.5.0/include/galsim/boost1_48_0/config/
--rw-r--r--   0 runner    (1001) docker     (127)    21149 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/boost1_48_0/config/suffix.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/boost1_48_0/current_function.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 20:55:17.276814 GalSim-2.5.0/include/galsim/boost1_48_0/random/
--rw-r--r--   0 runner    (1001) docker     (127)    12400 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/boost1_48_0/random/binomial_distribution.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6388 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/boost1_48_0/random/chi_squared_distribution.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 20:55:17.280814 GalSim-2.5.0/include/galsim/boost1_48_0/random/detail/
--rw-r--r--   0 runner    (1001) docker     (127)      929 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/boost1_48_0/random/detail/generator_seed_seq.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2950 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/boost1_48_0/random/detail/ptr_helper.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5418 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/boost1_48_0/random/detail/seed.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2420 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/boost1_48_0/random/detail/signed_unsigned_tools.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5728 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/boost1_48_0/random/exponential_distribution.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     9414 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/boost1_48_0/random/gamma_distribution.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    19903 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/boost1_48_0/random/mersenne_twister.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7472 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/boost1_48_0/random/normal_distribution.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    10295 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/boost1_48_0/random/poisson_distribution.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7982 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/boost1_48_0/random/uniform_01.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8594 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/boost1_48_0/random/uniform_real_distribution.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5679 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/boost1_48_0/random/weibull_distribution.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 20:55:17.284814 GalSim-2.5.0/include/galsim/fmath/
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/fmath/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      419 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/fmath/README
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/fmath/avx2.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    11454 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/fmath/bench.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/fmath/bench.sln
--rw-r--r--   0 runner    (1001) docker     (127)     7420 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/fmath/bench.vcproj
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/fmath/ck.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    37235 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/fmath/fastexp.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    23954 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/fmath/fmath.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 20:55:17.120816 GalSim-2.5.0/include/galsim/fmath/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 20:55:17.284814 GalSim-2.5.0/include/galsim/fmath/include/cybozu/
--rw-r--r--   0 runner    (1001) docker     (127)     3896 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/fmath/include/cybozu/benchmark.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/fmath/include/cybozu/inttype.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/fmath/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)     5899 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/fmath/readme.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 20:55:17.284814 GalSim-2.5.0/include/galsim/hsm/
--rw-r--r--   0 runner    (1001) docker     (127)    28148 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/hsm/PSFCorr.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 20:55:17.284814 GalSim-2.5.0/include/galsim/integ/
--rw-r--r--   0 runner    (1001) docker     (127)    42773 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/integ/Int.h
--rw-r--r--   0 runner    (1001) docker     (127)    12112 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/integ/IntGKPData1.h
--rw-r--r--   0 runner    (1001) docker     (127)    17415 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/integ/IntGKPData10.h
--rw-r--r--   0 runner    (1001) docker     (127)    32193 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/integ/MoreFunctional.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 20:55:17.288814 GalSim-2.5.0/include/galsim/math/
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/math/Angle.h
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/math/Bessel.h
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/math/Gamma.h
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/math/Hankel.h
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/math/Horner.h
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/math/Nan.h
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/math/Sinc.h
--rw-r--r--   0 runner    (1001) docker     (127)     8299 2023-10-16 20:54:10.000000 GalSim-2.5.0/include/galsim/mmgr.h
--rw-r--r--   0 runner    (1001) docker     (127)       71 2023-10-16 20:54:10.000000 GalSim-2.5.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 20:55:17.300814 GalSim-2.5.0/pysrc/
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2023-10-16 20:54:10.000000 GalSim-2.5.0/pysrc/Bessel.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2023-10-16 20:54:10.000000 GalSim-2.5.0/pysrc/Bounds.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2023-10-16 20:54:10.000000 GalSim-2.5.0/pysrc/CDModel.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5454 2023-10-16 20:54:10.000000 GalSim-2.5.0/pysrc/HSM.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2023-10-16 20:54:10.000000 GalSim-2.5.0/pysrc/Horner.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3826 2023-10-16 20:54:10.000000 GalSim-2.5.0/pysrc/Image.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2892 2023-10-16 20:54:10.000000 GalSim-2.5.0/pysrc/Integ.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2023-10-16 20:54:10.000000 GalSim-2.5.0/pysrc/Interpolant.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2023-10-16 20:54:10.000000 GalSim-2.5.0/pysrc/PhotonArray.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2023-10-16 20:54:10.000000 GalSim-2.5.0/pysrc/PyBind11Helper.h
--rw-r--r--   0 runner    (1001) docker     (127)     5471 2023-10-16 20:54:10.000000 GalSim-2.5.0/pysrc/Random.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2023-10-16 20:54:10.000000 GalSim-2.5.0/pysrc/RealGalaxy.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2023-10-16 20:54:10.000000 GalSim-2.5.0/pysrc/SBAdd.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2023-10-16 20:54:10.000000 GalSim-2.5.0/pysrc/SBAiry.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2023-10-16 20:54:10.000000 GalSim-2.5.0/pysrc/SBBox.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2023-10-16 20:54:10.000000 GalSim-2.5.0/pysrc/SBConvolve.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2023-10-16 20:54:10.000000 GalSim-2.5.0/pysrc/SBDeconvolve.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2023-10-16 20:54:10.000000 GalSim-2.5.0/pysrc/SBDeltaFunction.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2023-10-16 20:54:10.000000 GalSim-2.5.0/pysrc/SBExponential.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2023-10-16 20:54:10.000000 GalSim-2.5.0/pysrc/SBFourierSqrt.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2023-10-16 20:54:10.000000 GalSim-2.5.0/pysrc/SBGaussian.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2023-10-16 20:54:10.000000 GalSim-2.5.0/pysrc/SBInclinedExponential.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2023-10-16 20:54:10.000000 GalSim-2.5.0/pysrc/SBInclinedSersic.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2023-10-16 20:54:10.000000 GalSim-2.5.0/pysrc/SBInterpolatedImage.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2023-10-16 20:54:10.000000 GalSim-2.5.0/pysrc/SBKolmogorov.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2023-10-16 20:54:10.000000 GalSim-2.5.0/pysrc/SBMoffat.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2023-10-16 20:54:10.000000 GalSim-2.5.0/pysrc/SBProfile.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2023-10-16 20:54:10.000000 GalSim-2.5.0/pysrc/SBSecondKick.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2023-10-16 20:54:10.000000 GalSim-2.5.0/pysrc/SBSersic.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2023-10-16 20:54:10.000000 GalSim-2.5.0/pysrc/SBShapelet.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2023-10-16 20:54:10.000000 GalSim-2.5.0/pysrc/SBSpergel.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2023-10-16 20:54:10.000000 GalSim-2.5.0/pysrc/SBTransform.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2023-10-16 20:54:10.000000 GalSim-2.5.0/pysrc/SBVonKarman.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2902 2023-10-16 20:54:10.000000 GalSim-2.5.0/pysrc/Silicon.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6730 2023-10-16 20:54:10.000000 GalSim-2.5.0/pysrc/Table.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6714 2023-10-16 20:54:10.000000 GalSim-2.5.0/pysrc/Utilities.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2023-10-16 20:54:10.000000 GalSim-2.5.0/pysrc/WCS.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4021 2023-10-16 20:54:10.000000 GalSim-2.5.0/pysrc/module.cpp
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-16 20:55:17.380813 GalSim-2.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    58359 2023-10-16 20:54:10.000000 GalSim-2.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 20:55:17.300814 GalSim-2.5.0/share/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 20:55:17.300814 GalSim-2.5.0/share/SEDs/
--rw-r--r--   0 runner    (1001) docker     (127)    12280 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/SEDs/CWW_E_ext.sed
--rw-r--r--   0 runner    (1001) docker     (127)     7392 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/SEDs/CWW_E_ext_more.sed
--rw-r--r--   0 runner    (1001) docker     (127)    12021 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/SEDs/CWW_Im_ext.sed
--rw-r--r--   0 runner    (1001) docker     (127)     8017 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/SEDs/CWW_Im_ext_more.sed
--rw-r--r--   0 runner    (1001) docker     (127)    13010 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/SEDs/CWW_Sbc_ext.sed
--rw-r--r--   0 runner    (1001) docker     (127)     8460 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/SEDs/CWW_Sbc_ext_more.sed
--rw-r--r--   0 runner    (1001) docker     (127)    12932 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/SEDs/CWW_Scd_ext.sed
--rw-r--r--   0 runner    (1001) docker     (127)     8356 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/SEDs/CWW_Scd_ext_more.sed
--rw-r--r--   0 runner    (1001) docker     (127)      242 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/SEDs/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)   102422 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/SEDs/vega.txt
--rw-r--r--   0 runner    (1001) docker     (127)    57600 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/acs_I_unrot_sci_20_cf.fits
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 20:55:17.308814 GalSim-2.5.0/share/bandpasses/
--rw-r--r--   0 runner    (1001) docker     (127)     5885 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/bandpasses/ACS_wfc_F435W.dat
--rw-r--r--   0 runner    (1001) docker     (127)    11657 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/bandpasses/ACS_wfc_F606W.dat
--rw-r--r--   0 runner    (1001) docker     (127)     4611 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/bandpasses/ACS_wfc_F775W.dat
--rw-r--r--   0 runner    (1001) docker     (127)     8823 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/bandpasses/ACS_wfc_F814W.dat
--rw-r--r--   0 runner    (1001) docker     (127)     4093 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/bandpasses/ACS_wfc_F850LP.dat
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/bandpasses/LSST_g.dat
--rw-r--r--   0 runner    (1001) docker     (127)     3384 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/bandpasses/LSST_i.dat
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/bandpasses/LSST_r.dat
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/bandpasses/LSST_u.dat
--rw-r--r--   0 runner    (1001) docker     (127)     6036 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/bandpasses/LSST_y.dat
--rw-r--r--   0 runner    (1001) docker     (127)     3410 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/bandpasses/LSST_z.dat
--rw-r--r--   0 runner    (1001) docker     (127)      238 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/bandpasses/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/bandpasses/WFC3_ir_F105W.dat
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/bandpasses/WFC3_ir_F125W.dat
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/bandpasses/WFC3_ir_F160W.dat
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/bandpasses/WFC3_uvis_F275W.dat
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/bandpasses/WFC3_uvis_F336W.dat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 20:55:17.328814 GalSim-2.5.0/share/roman/
--rw-r--r--   0 runner    (1001) docker     (127)    72363 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/roman/RST_WIM_Filter_F184_SCA_1.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    72815 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/roman/RST_WIM_Filter_F184_SCA_10.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    71900 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/roman/RST_WIM_Filter_F184_SCA_11.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    71312 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/roman/RST_WIM_Filter_F184_SCA_12.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    73332 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/roman/RST_WIM_Filter_F184_SCA_13.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    73256 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/roman/RST_WIM_Filter_F184_SCA_14.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    72231 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/roman/RST_WIM_Filter_F184_SCA_15.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    75714 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/roman/RST_WIM_Filter_F184_SCA_16.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    73288 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/roman/RST_WIM_Filter_F184_SCA_17.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    72988 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/roman/RST_WIM_Filter_F184_SCA_18.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    72683 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/roman/RST_WIM_Filter_F184_SCA_2.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    71938 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/roman/RST_WIM_Filter_F184_SCA_3.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    72860 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/roman/RST_WIM_Filter_F184_SCA_4.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    72153 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/roman/RST_WIM_Filter_F184_SCA_5.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    71630 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/roman/RST_WIM_Filter_F184_SCA_6.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    76049 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/roman/RST_WIM_Filter_F184_SCA_7.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    73119 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/roman/RST_WIM_Filter_F184_SCA_8.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    72505 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/roman/RST_WIM_Filter_F184_SCA_9.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    74944 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/roman/RST_WIM_Filter_skinny_SCA_1.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    74222 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/roman/RST_WIM_Filter_skinny_SCA_10.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    73499 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/roman/RST_WIM_Filter_skinny_SCA_11.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    72953 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/roman/RST_WIM_Filter_skinny_SCA_12.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    77295 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/roman/RST_WIM_Filter_skinny_SCA_13.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    73917 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/roman/RST_WIM_Filter_skinny_SCA_14.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    73364 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/roman/RST_WIM_Filter_skinny_SCA_15.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    77941 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/roman/RST_WIM_Filter_skinny_SCA_16.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    78030 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/roman/RST_WIM_Filter_skinny_SCA_17.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    77598 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/roman/RST_WIM_Filter_skinny_SCA_18.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    74701 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/roman/RST_WIM_Filter_skinny_SCA_2.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    73506 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/roman/RST_WIM_Filter_skinny_SCA_3.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    78098 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/roman/RST_WIM_Filter_skinny_SCA_4.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    75183 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/roman/RST_WIM_Filter_skinny_SCA_5.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    73645 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/roman/RST_WIM_Filter_skinny_SCA_6.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    77605 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/roman/RST_WIM_Filter_skinny_SCA_7.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    77370 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/roman/RST_WIM_Filter_skinny_SCA_8.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    77167 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/roman/RST_WIM_Filter_skinny_SCA_9.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_03.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_04.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_05.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_06.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_07.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_08.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_09.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_10.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_11.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_12.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_13.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_14.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_15.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_16.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_17.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_18.txt
--rw-r--r--   0 runner    (1001) docker     (127)   204929 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/roman/Roman_SRR_WFC_Pupil_Mask_Longwave_2048_reformatted.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)   207326 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/roman/Roman_SRR_WFC_Pupil_Mask_Shortwave_2048_reformatted.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    53490 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/roman/Roman_effarea_20210614.txt
--rw-r--r--   0 runner    (1001) docker     (127)   206809 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/roman/roman_sky_backgrounds.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/roman/sca_positions_20210204.txt
--rw-r--r--   0 runner    (1001) docker     (127)    16920 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/roman/sip_20210204.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 20:55:17.340813 GalSim-2.5.0/share/sensors/
--rw-r--r--   0 runner    (1001) docker     (127)     5054 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/sensors/abs_length.dat
--rw-r--r--   0 runner    (1001) docker     (127)    10297 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/sensors/lsst_e2v_32.cfg
--rw-r--r--   0 runner    (1001) docker     (127)   812668 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/sensors/lsst_e2v_32.dat
--rw-r--r--   0 runner    (1001) docker     (127)    10060 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/sensors/lsst_e2v_50_32.cfg
--rw-r--r--   0 runner    (1001) docker     (127)   812668 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/sensors/lsst_e2v_50_32.dat
--rw-r--r--   0 runner    (1001) docker     (127)    10061 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/sensors/lsst_e2v_50_8.cfg
--rw-r--r--   0 runner    (1001) docker     (127)   221692 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/sensors/lsst_e2v_50_8.dat
--rw-r--r--   0 runner    (1001) docker     (127)    10296 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/sensors/lsst_e2v_8.cfg
--rw-r--r--   0 runner    (1001) docker     (127)   221692 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/sensors/lsst_e2v_8.dat
--rw-r--r--   0 runner    (1001) docker     (127)    10365 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/sensors/lsst_itl_32.cfg
--rw-r--r--   0 runner    (1001) docker     (127)   812668 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/sensors/lsst_itl_32.dat
--rw-r--r--   0 runner    (1001) docker     (127)    10374 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/sensors/lsst_itl_50_32.cfg
--rw-r--r--   0 runner    (1001) docker     (127)   812668 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/sensors/lsst_itl_50_32.dat
--rw-r--r--   0 runner    (1001) docker     (127)    10375 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/sensors/lsst_itl_50_8.cfg
--rw-r--r--   0 runner    (1001) docker     (127)   221692 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/sensors/lsst_itl_50_8.dat
--rw-r--r--   0 runner    (1001) docker     (127)    10365 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/sensors/lsst_itl_8.cfg
--rw-r--r--   0 runner    (1001) docker     (127)   221692 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/sensors/lsst_itl_8.dat
--rw-r--r--   0 runner    (1001) docker     (127)   122780 2023-10-16 20:54:10.000000 GalSim-2.5.0/share/wfc_F814W.dat.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 20:55:17.352813 GalSim-2.5.0/src/
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2023-10-16 20:54:10.000000 GalSim-2.5.0/src/BinomFact.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4870 2023-10-16 20:54:10.000000 GalSim-2.5.0/src/CDModel.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2023-10-16 20:54:10.000000 GalSim-2.5.0/src/CorrelatedNoise.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5752 2023-10-16 20:54:10.000000 GalSim-2.5.0/src/GSParams.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    54447 2023-10-16 20:54:10.000000 GalSim-2.5.0/src/Image.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2023-10-16 20:54:10.000000 GalSim-2.5.0/src/Image.inst
--rw-r--r--   0 runner    (1001) docker     (127)    35052 2023-10-16 20:54:10.000000 GalSim-2.5.0/src/Interpolant.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    19072 2023-10-16 20:54:10.000000 GalSim-2.5.0/src/Laguerre.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    22231 2023-10-16 20:54:10.000000 GalSim-2.5.0/src/OneDimensionalDeviate.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8020 2023-10-16 20:54:10.000000 GalSim-2.5.0/src/PhotonArray.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6426 2023-10-16 20:54:10.000000 GalSim-2.5.0/src/Polygon.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    27173 2023-10-16 20:54:10.000000 GalSim-2.5.0/src/Random.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7380 2023-10-16 20:54:10.000000 GalSim-2.5.0/src/RealGalaxy.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    15670 2023-10-16 20:54:10.000000 GalSim-2.5.0/src/RealSpaceConvolve.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    10263 2023-10-16 20:54:10.000000 GalSim-2.5.0/src/SBAdd.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    16980 2023-10-16 20:54:10.000000 GalSim-2.5.0/src/SBAiry.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    17398 2023-10-16 20:54:10.000000 GalSim-2.5.0/src/SBBox.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    19001 2023-10-16 20:54:10.000000 GalSim-2.5.0/src/SBConvolve.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6731 2023-10-16 20:54:10.000000 GalSim-2.5.0/src/SBDeconvolve.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3028 2023-10-16 20:54:10.000000 GalSim-2.5.0/src/SBDeltaFunction.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    25768 2023-10-16 20:54:10.000000 GalSim-2.5.0/src/SBExponential.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4759 2023-10-16 20:54:10.000000 GalSim-2.5.0/src/SBFourierSqrt.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    12029 2023-10-16 20:54:10.000000 GalSim-2.5.0/src/SBGaussian.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    14238 2023-10-16 20:54:10.000000 GalSim-2.5.0/src/SBInclinedExponential.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    15106 2023-10-16 20:54:10.000000 GalSim-2.5.0/src/SBInclinedSersic.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    62389 2023-10-16 20:54:10.000000 GalSim-2.5.0/src/SBInterpolatedImage.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    18274 2023-10-16 20:54:10.000000 GalSim-2.5.0/src/SBKolmogorov.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    25486 2023-10-16 20:54:10.000000 GalSim-2.5.0/src/SBMoffat.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    24029 2023-10-16 20:54:10.000000 GalSim-2.5.0/src/SBProfile.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    16498 2023-10-16 20:54:10.000000 GalSim-2.5.0/src/SBSecondKick.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    33842 2023-10-16 20:54:10.000000 GalSim-2.5.0/src/SBSersic.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    13511 2023-10-16 20:54:10.000000 GalSim-2.5.0/src/SBShapelet.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    29887 2023-10-16 20:54:10.000000 GalSim-2.5.0/src/SBSpergel.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    44809 2023-10-16 20:54:10.000000 GalSim-2.5.0/src/SBTransform.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    20081 2023-10-16 20:54:10.000000 GalSim-2.5.0/src/SBVonKarman.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    70745 2023-10-16 20:54:10.000000 GalSim-2.5.0/src/Silicon.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    53187 2023-10-16 20:54:10.000000 GalSim-2.5.0/src/Table.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2023-10-16 20:54:10.000000 GalSim-2.5.0/src/Version.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    12132 2023-10-16 20:54:10.000000 GalSim-2.5.0/src/WCS.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 20:55:17.352813 GalSim-2.5.0/src/hsm/
--rw-r--r--   0 runner    (1001) docker     (127)    78969 2023-10-16 20:54:10.000000 GalSim-2.5.0/src/hsm/PSFCorr.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 20:55:17.356813 GalSim-2.5.0/src/math/
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2023-10-16 20:54:10.000000 GalSim-2.5.0/src/math/Angle.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6683 2023-10-16 20:54:10.000000 GalSim-2.5.0/src/math/Bessel.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    43843 2023-10-16 20:54:10.000000 GalSim-2.5.0/src/math/BesselI.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    74848 2023-10-16 20:54:10.000000 GalSim-2.5.0/src/math/BesselJ.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    45424 2023-10-16 20:54:10.000000 GalSim-2.5.0/src/math/BesselK.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6312 2023-10-16 20:54:10.000000 GalSim-2.5.0/src/math/BesselRoots.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    63931 2023-10-16 20:54:10.000000 GalSim-2.5.0/src/math/BesselY.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    24658 2023-10-16 20:54:10.000000 GalSim-2.5.0/src/math/Gamma.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     9825 2023-10-16 20:54:10.000000 GalSim-2.5.0/src/math/Hankel.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4557 2023-10-16 20:54:10.000000 GalSim-2.5.0/src/math/Horner.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2023-10-16 20:54:10.000000 GalSim-2.5.0/src/math/Nan.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     9748 2023-10-16 20:54:10.000000 GalSim-2.5.0/src/math/Sinc.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    73348 2023-10-16 20:54:10.000000 GalSim-2.5.0/src/mmgr.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 20:55:17.376813 GalSim-2.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    12631 2023-10-16 20:54:11.000000 GalSim-2.5.0/tests/test_airy.py
--rw-r--r--   0 runner    (1001) docker     (127)    20158 2023-10-16 20:54:11.000000 GalSim-2.5.0/tests/test_bandpass.py
--rw-r--r--   0 runner    (1001) docker     (127)    18529 2023-10-16 20:54:11.000000 GalSim-2.5.0/tests/test_bessel.py
--rw-r--r--   0 runner    (1001) docker     (127)    15067 2023-10-16 20:54:11.000000 GalSim-2.5.0/tests/test_box.py
--rw-r--r--   0 runner    (1001) docker     (127)    18703 2023-10-16 20:54:11.000000 GalSim-2.5.0/tests/test_calc.py
--rw-r--r--   0 runner    (1001) docker     (127)    14455 2023-10-16 20:54:11.000000 GalSim-2.5.0/tests/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)    16370 2023-10-16 20:54:11.000000 GalSim-2.5.0/tests/test_cdmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)    37474 2023-10-16 20:54:11.000000 GalSim-2.5.0/tests/test_celestial.py
--rw-r--r--   0 runner    (1001) docker     (127)   153562 2023-10-16 20:54:11.000000 GalSim-2.5.0/tests/test_chromatic.py
--rw-r--r--   0 runner    (1001) docker     (127)    91493 2023-10-16 20:54:11.000000 GalSim-2.5.0/tests/test_config_gsobject.py
--rw-r--r--   0 runner    (1001) docker     (127)   138579 2023-10-16 20:54:11.000000 GalSim-2.5.0/tests/test_config_image.py
--rw-r--r--   0 runner    (1001) docker     (127)    17439 2023-10-16 20:54:11.000000 GalSim-2.5.0/tests/test_config_input.py
--rw-r--r--   0 runner    (1001) docker     (127)    34185 2023-10-16 20:54:11.000000 GalSim-2.5.0/tests/test_config_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)    73746 2023-10-16 20:54:11.000000 GalSim-2.5.0/tests/test_config_output.py
--rw-r--r--   0 runner    (1001) docker     (127)    88975 2023-10-16 20:54:11.000000 GalSim-2.5.0/tests/test_config_value.py
--rw-r--r--   0 runner    (1001) docker     (127)    44767 2023-10-16 20:54:11.000000 GalSim-2.5.0/tests/test_convolve.py
--rw-r--r--   0 runner    (1001) docker     (127)    69505 2023-10-16 20:54:11.000000 GalSim-2.5.0/tests/test_correlatednoise.py
--rw-r--r--   0 runner    (1001) docker     (127)     8020 2023-10-16 20:54:11.000000 GalSim-2.5.0/tests/test_deltafunction.py
--rw-r--r--   0 runner    (1001) docker     (127)    27443 2023-10-16 20:54:11.000000 GalSim-2.5.0/tests/test_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)    34166 2023-10-16 20:54:11.000000 GalSim-2.5.0/tests/test_des.py
--rw-r--r--   0 runner    (1001) docker     (127)    22196 2023-10-16 20:54:11.000000 GalSim-2.5.0/tests/test_detectors.py
--rw-r--r--   0 runner    (1001) docker     (127)    26046 2023-10-16 20:54:11.000000 GalSim-2.5.0/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (127)    86539 2023-10-16 20:54:11.000000 GalSim-2.5.0/tests/test_draw.py
--rw-r--r--   0 runner    (1001) docker     (127)     9229 2023-10-16 20:54:11.000000 GalSim-2.5.0/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    10716 2023-10-16 20:54:11.000000 GalSim-2.5.0/tests/test_exponential.py
--rw-r--r--   0 runner    (1001) docker     (127)    10407 2023-10-16 20:54:11.000000 GalSim-2.5.0/tests/test_fitsheader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4445 2023-10-16 20:54:11.000000 GalSim-2.5.0/tests/test_fouriersqrt.py
--rw-r--r--   0 runner    (1001) docker     (127)    20703 2023-10-16 20:54:11.000000 GalSim-2.5.0/tests/test_galaxy_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)    18408 2023-10-16 20:54:11.000000 GalSim-2.5.0/tests/test_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)    51280 2023-10-16 20:54:11.000000 GalSim-2.5.0/tests/test_hsm.py
--rw-r--r--   0 runner    (1001) docker     (127)   168100 2023-10-16 20:54:11.000000 GalSim-2.5.0/tests/test_image.py
--rw-r--r--   0 runner    (1001) docker     (127)    29539 2023-10-16 20:54:11.000000 GalSim-2.5.0/tests/test_inclined.py
--rw-r--r--   0 runner    (1001) docker     (127)    14962 2023-10-16 20:54:11.000000 GalSim-2.5.0/tests/test_integ.py
--rw-r--r--   0 runner    (1001) docker     (127)    85965 2023-10-16 20:54:11.000000 GalSim-2.5.0/tests/test_interpolatedimage.py
--rw-r--r--   0 runner    (1001) docker     (127)    14275 2023-10-16 20:54:11.000000 GalSim-2.5.0/tests/test_knots.py
--rw-r--r--   0 runner    (1001) docker     (127)    18435 2023-10-16 20:54:11.000000 GalSim-2.5.0/tests/test_kolmogorov.py
--rw-r--r--   0 runner    (1001) docker     (127)    78648 2023-10-16 20:54:11.000000 GalSim-2.5.0/tests/test_lensing.py
--rw-r--r--   0 runner    (1001) docker     (127)    12085 2023-10-16 20:54:11.000000 GalSim-2.5.0/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)    20983 2023-10-16 20:54:11.000000 GalSim-2.5.0/tests/test_metacal.py
--rw-r--r--   0 runner    (1001) docker     (127)    25068 2023-10-16 20:54:11.000000 GalSim-2.5.0/tests/test_moffat.py
--rw-r--r--   0 runner    (1001) docker     (127)    35496 2023-10-16 20:54:11.000000 GalSim-2.5.0/tests/test_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)    48379 2023-10-16 20:54:11.000000 GalSim-2.5.0/tests/test_optics.py
--rw-r--r--   0 runner    (1001) docker     (127)    65379 2023-10-16 20:54:11.000000 GalSim-2.5.0/tests/test_phase_psf.py
--rw-r--r--   0 runner    (1001) docker     (127)    71865 2023-10-16 20:54:11.000000 GalSim-2.5.0/tests/test_photon_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     9321 2023-10-16 20:54:11.000000 GalSim-2.5.0/tests/test_pse.py
--rw-r--r--   0 runner    (1001) docker     (127)    80378 2023-10-16 20:54:11.000000 GalSim-2.5.0/tests/test_random.py
--rw-r--r--   0 runner    (1001) docker     (127)    43941 2023-10-16 20:54:11.000000 GalSim-2.5.0/tests/test_real.py
--rw-r--r--   0 runner    (1001) docker     (127)    67201 2023-10-16 20:54:11.000000 GalSim-2.5.0/tests/test_roman.py
--rw-r--r--   0 runner    (1001) docker     (127)    13305 2023-10-16 20:54:11.000000 GalSim-2.5.0/tests/test_second_kick.py
--rw-r--r--   0 runner    (1001) docker     (127)    55409 2023-10-16 20:54:11.000000 GalSim-2.5.0/tests/test_sed.py
--rw-r--r--   0 runner    (1001) docker     (127)    59459 2023-10-16 20:54:11.000000 GalSim-2.5.0/tests/test_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)    27331 2023-10-16 20:54:11.000000 GalSim-2.5.0/tests/test_sersic.py
--rw-r--r--   0 runner    (1001) docker     (127)    16575 2023-10-16 20:54:11.000000 GalSim-2.5.0/tests/test_shapelet.py
--rw-r--r--   0 runner    (1001) docker     (127)    13439 2023-10-16 20:54:11.000000 GalSim-2.5.0/tests/test_shear.py
--rw-r--r--   0 runner    (1001) docker     (127)     4231 2023-10-16 20:54:11.000000 GalSim-2.5.0/tests/test_shear_position.py
--rw-r--r--   0 runner    (1001) docker     (127)    15117 2023-10-16 20:54:11.000000 GalSim-2.5.0/tests/test_spergel.py
--rw-r--r--   0 runner    (1001) docker     (127)    14630 2023-10-16 20:54:11.000000 GalSim-2.5.0/tests/test_sum.py
--rw-r--r--   0 runner    (1001) docker     (127)    52841 2023-10-16 20:54:11.000000 GalSim-2.5.0/tests/test_table.py
--rw-r--r--   0 runner    (1001) docker     (127)    47931 2023-10-16 20:54:11.000000 GalSim-2.5.0/tests/test_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)    62197 2023-10-16 20:54:11.000000 GalSim-2.5.0/tests/test_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    15824 2023-10-16 20:54:11.000000 GalSim-2.5.0/tests/test_vonkarman.py
--rw-r--r--   0 runner    (1001) docker     (127)   152082 2023-10-16 20:54:11.000000 GalSim-2.5.0/tests/test_wcs.py
--rw-r--r--   0 runner    (1001) docker     (127)    53232 2023-10-16 20:54:11.000000 GalSim-2.5.0/tests/test_zernike.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 02:09:41.683256 GalSim-2.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     5698 2023-11-02 02:08:36.000000 GalSim-2.5.1/CHANGELOG.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 02:09:41.487252 GalSim-2.5.1/GalSim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10310 2023-11-02 02:09:41.000000 GalSim-2.5.1/GalSim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    24094 2023-11-02 02:09:41.000000 GalSim-2.5.1/GalSim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-02 02:09:41.000000 GalSim-2.5.1/GalSim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2023-11-02 02:09:41.000000 GalSim-2.5.1/GalSim.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-02 02:09:41.000000 GalSim-2.5.1/GalSim.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2023-11-02 02:09:41.000000 GalSim-2.5.1/GalSim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2023-11-02 02:09:41.000000 GalSim-2.5.1/GalSim.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2023-11-02 02:08:36.000000 GalSim-2.5.1/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2023-11-02 02:08:36.000000 GalSim-2.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2023-11-02 02:08:36.000000 GalSim-2.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10310 2023-11-02 02:09:41.683256 GalSim-2.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9796 2023-11-02 02:08:36.000000 GalSim-2.5.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 02:09:41.499252 GalSim-2.5.1/galsim/
+-rw-r--r--   0 runner    (1001) docker     (127)     6370 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/_pyfits.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11884 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10442 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/airy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/angle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33902 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/bandpass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/bessel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18607 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/bounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8837 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/box.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23094 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11816 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/cdmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/celestial.py
+-rw-r--r--   0 runner    (1001) docker     (127)   179905 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/chromatic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 02:09:41.507253 GalSim-2.5.1/galsim/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6942 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/config/bandpass.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23329 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/config/extra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3118 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/config/extra_badpix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6416 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/config/extra_psf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5390 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/config/extra_truth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4155 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/config/extra_weight.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25714 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/config/gsobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26118 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/config/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9108 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/config/image_scattered.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11091 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/config/image_tiled.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32708 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/config/input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7363 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/config/input_cosmos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/config/input_fitsheader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/config/input_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4163 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/config/input_nfw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12494 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/config/input_powerspectrum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5448 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/config/input_real.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28896 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/config/noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24343 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/config/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5595 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/config/output_datacube.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3475 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/config/output_multifits.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11659 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/config/photon_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13833 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/config/process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7260 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/config/sed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8437 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/config/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56378 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/config/stamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7797 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/config/stamp_ring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46057 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/config/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34861 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/config/value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8143 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/config/value_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10997 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/config/value_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12661 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/config/wcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40905 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/convolve.py
+-rw-r--r--   0 runner    (1001) docker     (127)    88081 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/correlatednoise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7407 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/dcr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3171 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/deltafunction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 02:09:41.507253 GalSim-2.5.1/galsim/deprecated/
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/deprecated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/deprecated/correlatednoise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/deprecated/integ.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/deprecated/randwalk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 02:09:41.507253 GalSim-2.5.1/galsim/des/
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/des/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26420 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/des/des_meds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17509 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/des/des_psfex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9656 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/des/des_shapelet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17521 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/detectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21051 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/download_cosmos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18816 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6122 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/exponential.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10811 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/fft.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65426 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/fits.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83625 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/fitswcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7721 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/fouriersqrt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50015 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/galaxy_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6856 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)   131545 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/gsobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14402 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/gsparams.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42279 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/hsm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83850 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21169 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/inclined.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 02:09:41.507253 GalSim-2.5.1/galsim/include/
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/GalSim.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 02:09:41.507253 GalSim-2.5.1/galsim/include/fftw3/
+-rw-r--r--   0 runner    (1001) docker     (127)    16123 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/fftw3/fftw3.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 02:09:41.515253 GalSim-2.5.1/galsim/include/galsim/
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/BinomFact.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17940 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/Bounds.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/CDModel.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/CorrelatedNoise.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9273 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/GSParams.h
+-rw-r--r--   0 runner    (1001) docker     (127)    31400 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/Image.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21782 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/ImageArith.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20810 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/Interpolant.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8403 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/LRUCache.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15876 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/Laguerre.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12225 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/OneDimensionalDeviate.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11797 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/PhotonArray.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3924 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/Polygon.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16757 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/ProbabilityTree.h
+-rw-r--r--   0 runner    (1001) docker     (127)    34396 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/Random.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/RealGalaxy.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/SBAdd.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9374 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/SBAddImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3046 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/SBAiry.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12047 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/SBAiryImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3535 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/SBBox.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9712 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/SBBoxImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6744 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/SBConvolve.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13052 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/SBConvolveImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/SBDeconvolve.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/SBDeconvolveImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/SBDeltaFunction.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/SBDeltaFunctionImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2609 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/SBExponential.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8093 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/SBExponentialImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/SBFourierSqrt.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3820 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/SBFourierSqrtImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/SBGaussian.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5739 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/SBGaussianImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3244 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/SBInclinedExponential.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6140 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/SBInclinedExponentialImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4212 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/SBInclinedSersic.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6245 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/SBInclinedSersicImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7185 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/SBInterpolatedImage.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11555 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/SBInterpolatedImageImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/SBKolmogorov.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7989 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/SBKolmogorovImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/SBMoffat.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8095 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/SBMoffatImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16789 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/SBProfile.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9531 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/SBProfileImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/SBSecondKick.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3981 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/SBSecondKickImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6056 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/SBSersic.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11563 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/SBSersicImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2308 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/SBShapelet.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4971 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/SBShapeletImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3813 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/SBSpergel.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9598 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/SBSpergelImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/SBTransform.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10313 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/SBTransformImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/SBVonKarman.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5998 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/SBVonKarmanImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12343 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/Silicon.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16801 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/Solve.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8138 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/Std.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/Stopwatch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6072 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/Table.h
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2023-11-02 02:09:41.000000 GalSim-2.5.1/galsim/include/galsim/Version.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/WCS.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 02:09:41.515253 GalSim-2.5.1/galsim/include/galsim/boost1_48_0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/boost1_48_0/LICENSE_1_0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/boost1_48_0/README
+-rw-r--r--   0 runner    (1001) docker     (127)     4118 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/boost1_48_0/assert.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 02:09:41.515253 GalSim-2.5.1/galsim/include/galsim/boost1_48_0/config/
+-rw-r--r--   0 runner    (1001) docker     (127)    21149 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/boost1_48_0/config/suffix.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/boost1_48_0/current_function.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 02:09:41.519253 GalSim-2.5.1/galsim/include/galsim/boost1_48_0/random/
+-rw-r--r--   0 runner    (1001) docker     (127)    12400 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/boost1_48_0/random/binomial_distribution.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6388 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/boost1_48_0/random/chi_squared_distribution.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 02:09:41.519253 GalSim-2.5.1/galsim/include/galsim/boost1_48_0/random/detail/
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/boost1_48_0/random/detail/generator_seed_seq.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/boost1_48_0/random/detail/ptr_helper.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5418 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/boost1_48_0/random/detail/seed.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2420 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/boost1_48_0/random/detail/signed_unsigned_tools.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5728 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/boost1_48_0/random/exponential_distribution.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9414 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/boost1_48_0/random/gamma_distribution.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    19903 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/boost1_48_0/random/mersenne_twister.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7472 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/boost1_48_0/random/normal_distribution.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10295 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/boost1_48_0/random/poisson_distribution.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7982 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/boost1_48_0/random/uniform_01.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8594 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/boost1_48_0/random/uniform_real_distribution.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5679 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/boost1_48_0/random/weibull_distribution.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 02:09:41.519253 GalSim-2.5.1/galsim/include/galsim/fmath/
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/fmath/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/fmath/README
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/fmath/avx2.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11454 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/fmath/bench.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/fmath/bench.sln
+-rw-r--r--   0 runner    (1001) docker     (127)     7420 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/fmath/bench.vcproj
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/fmath/ck.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    37235 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/fmath/fastexp.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    23954 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/fmath/fmath.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 02:09:41.483252 GalSim-2.5.1/galsim/include/galsim/fmath/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 02:09:41.519253 GalSim-2.5.1/galsim/include/galsim/fmath/include/cybozu/
+-rw-r--r--   0 runner    (1001) docker     (127)     3896 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/fmath/include/cybozu/benchmark.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/fmath/include/cybozu/inttype.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/fmath/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5899 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/fmath/readme.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 02:09:41.523253 GalSim-2.5.1/galsim/include/galsim/hsm/
+-rw-r--r--   0 runner    (1001) docker     (127)    28148 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/hsm/PSFCorr.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 02:09:41.523253 GalSim-2.5.1/galsim/include/galsim/integ/
+-rw-r--r--   0 runner    (1001) docker     (127)    42773 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/integ/Int.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12112 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/integ/IntGKPData1.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17415 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/integ/IntGKPData10.h
+-rw-r--r--   0 runner    (1001) docker     (127)    32193 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/integ/MoreFunctional.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 02:09:41.523253 GalSim-2.5.1/galsim/include/galsim/math/
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/math/Angle.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/math/Bessel.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/math/Gamma.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/math/Hankel.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/math/Horner.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/math/Nan.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/math/Sinc.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8299 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/include/galsim/mmgr.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16748 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/integ.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24196 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/interpolant.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58093 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/interpolatedimage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12961 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/knots.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13408 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/kolmogorov.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77477 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/lensing_ps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9312 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/meta_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9009 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/moffat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20598 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/nfw_halo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25981 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)   107542 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/phase_psf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62882 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/phase_screens.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59412 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/photon_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11746 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/position.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14511 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/pse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40353 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70048 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/real.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 02:09:41.523253 GalSim-2.5.1/galsim/roman/
+-rw-r--r--   0 runner    (1001) docker     (127)     4125 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/roman/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7113 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/roman/roman_backgrounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8082 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/roman/roman_bandpass.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12680 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/roman/roman_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10748 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/roman/roman_detectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22797 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/roman/roman_psfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32871 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/roman/roman_wcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9875 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/second_kick.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59974 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/sed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24844 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18752 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/sersic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11563 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/shapelet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 02:09:41.523253 GalSim-2.5.1/galsim/share/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 02:09:41.527253 GalSim-2.5.1/galsim/share/SEDs/
+-rw-r--r--   0 runner    (1001) docker     (127)    12280 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/SEDs/CWW_E_ext.sed
+-rw-r--r--   0 runner    (1001) docker     (127)     7392 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/SEDs/CWW_E_ext_more.sed
+-rw-r--r--   0 runner    (1001) docker     (127)    12021 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/SEDs/CWW_Im_ext.sed
+-rw-r--r--   0 runner    (1001) docker     (127)     8017 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/SEDs/CWW_Im_ext_more.sed
+-rw-r--r--   0 runner    (1001) docker     (127)    13010 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/SEDs/CWW_Sbc_ext.sed
+-rw-r--r--   0 runner    (1001) docker     (127)     8460 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/SEDs/CWW_Sbc_ext_more.sed
+-rw-r--r--   0 runner    (1001) docker     (127)    12932 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/SEDs/CWW_Scd_ext.sed
+-rw-r--r--   0 runner    (1001) docker     (127)     8356 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/SEDs/CWW_Scd_ext_more.sed
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/SEDs/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   102422 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/SEDs/vega.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    57600 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/acs_I_unrot_sci_20_cf.fits
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 02:09:41.531253 GalSim-2.5.1/galsim/share/bandpasses/
+-rw-r--r--   0 runner    (1001) docker     (127)     5885 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/bandpasses/ACS_wfc_F435W.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    11657 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/bandpasses/ACS_wfc_F606W.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     4611 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/bandpasses/ACS_wfc_F775W.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     8823 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/bandpasses/ACS_wfc_F814W.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     4093 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/bandpasses/ACS_wfc_F850LP.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/bandpasses/LSST_g.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     3384 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/bandpasses/LSST_i.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/bandpasses/LSST_r.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/bandpasses/LSST_u.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     6036 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/bandpasses/LSST_y.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     3410 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/bandpasses/LSST_z.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/bandpasses/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/bandpasses/WFC3_ir_F105W.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/bandpasses/WFC3_ir_F125W.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/bandpasses/WFC3_ir_F160W.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/bandpasses/WFC3_uvis_F275W.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/bandpasses/WFC3_uvis_F336W.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 02:09:41.555254 GalSim-2.5.1/galsim/share/roman/
+-rw-r--r--   0 runner    (1001) docker     (127)    72363 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_F184_SCA_1.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    72815 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_F184_SCA_10.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    71900 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_F184_SCA_11.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    71312 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_F184_SCA_12.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    73332 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_F184_SCA_13.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    73256 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_F184_SCA_14.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    72231 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_F184_SCA_15.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    75714 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_F184_SCA_16.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    73288 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_F184_SCA_17.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    72988 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_F184_SCA_18.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    72683 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_F184_SCA_2.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    71938 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_F184_SCA_3.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    72860 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_F184_SCA_4.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    72153 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_F184_SCA_5.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    71630 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_F184_SCA_6.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    76049 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_F184_SCA_7.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    73119 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_F184_SCA_8.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    72505 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_F184_SCA_9.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    74944 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_skinny_SCA_1.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    74222 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_skinny_SCA_10.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    73499 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_skinny_SCA_11.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    72953 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_skinny_SCA_12.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    77295 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_skinny_SCA_13.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    73917 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_skinny_SCA_14.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    73364 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_skinny_SCA_15.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    77941 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_skinny_SCA_16.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    78030 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_skinny_SCA_17.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    77598 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_skinny_SCA_18.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    74701 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_skinny_SCA_2.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    73506 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_skinny_SCA_3.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    78098 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_skinny_SCA_4.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    75183 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_skinny_SCA_5.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    73645 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_skinny_SCA_6.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    77605 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_skinny_SCA_7.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    77370 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_skinny_SCA_8.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    77167 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_skinny_SCA_9.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_03.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_04.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_05.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_06.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_07.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_08.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_09.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_10.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_11.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_12.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_13.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_14.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_15.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_16.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_17.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_18.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   204929 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/roman/Roman_SRR_WFC_Pupil_Mask_Longwave_2048_reformatted.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   207326 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/roman/Roman_SRR_WFC_Pupil_Mask_Shortwave_2048_reformatted.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    53490 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/roman/Roman_effarea_20210614.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   206809 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/roman/roman_sky_backgrounds.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/roman/sca_positions_20210204.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16920 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/roman/sip_20210204.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 02:09:41.567254 GalSim-2.5.1/galsim/share/sensors/
+-rw-r--r--   0 runner    (1001) docker     (127)     5054 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/sensors/abs_length.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    10297 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/sensors/lsst_e2v_32.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)   812668 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/sensors/lsst_e2v_32.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    10060 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/sensors/lsst_e2v_50_32.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)   812668 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/sensors/lsst_e2v_50_32.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    10061 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/sensors/lsst_e2v_50_8.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)   221692 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/sensors/lsst_e2v_50_8.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    10296 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/sensors/lsst_e2v_8.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)   221692 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/sensors/lsst_e2v_8.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    10365 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/sensors/lsst_itl_32.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)   812668 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/sensors/lsst_itl_32.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    10374 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/sensors/lsst_itl_50_32.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)   812668 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/sensors/lsst_itl_50_32.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    10375 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/sensors/lsst_itl_50_8.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)   221692 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/sensors/lsst_itl_50_8.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    10365 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/sensors/lsst_itl_8.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)   221692 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/sensors/lsst_itl_8.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   122780 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/share/wfc_F814W.dat.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    17179 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/shear.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10472 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/spergel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13794 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/sum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53306 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26406 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)    76831 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/vonkarman.py
+-rw-r--r--   0 runner    (1001) docker     (127)   121121 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/wcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/wfirst.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57604 2023-11-02 02:08:37.000000 GalSim-2.5.1/galsim/zernike.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 02:09:41.571254 GalSim-2.5.1/include/
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/GalSim.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 02:09:41.571254 GalSim-2.5.1/include/fftw3/
+-rw-r--r--   0 runner    (1001) docker     (127)    16123 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/fftw3/fftw3.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 02:09:41.603254 GalSim-2.5.1/include/galsim/
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/BinomFact.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17940 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/Bounds.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/CDModel.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/CorrelatedNoise.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9273 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/GSParams.h
+-rw-r--r--   0 runner    (1001) docker     (127)    31400 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/Image.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21782 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/ImageArith.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20810 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/Interpolant.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8403 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/LRUCache.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15876 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/Laguerre.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12225 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/OneDimensionalDeviate.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11797 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/PhotonArray.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3924 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/Polygon.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16757 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/ProbabilityTree.h
+-rw-r--r--   0 runner    (1001) docker     (127)    34396 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/Random.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/RealGalaxy.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/SBAdd.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9374 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/SBAddImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3046 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/SBAiry.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12047 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/SBAiryImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3535 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/SBBox.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9712 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/SBBoxImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6744 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/SBConvolve.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13052 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/SBConvolveImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/SBDeconvolve.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/SBDeconvolveImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/SBDeltaFunction.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/SBDeltaFunctionImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2609 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/SBExponential.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8093 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/SBExponentialImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/SBFourierSqrt.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3820 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/SBFourierSqrtImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/SBGaussian.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5739 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/SBGaussianImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3244 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/SBInclinedExponential.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6140 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/SBInclinedExponentialImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4212 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/SBInclinedSersic.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6245 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/SBInclinedSersicImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7185 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/SBInterpolatedImage.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11555 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/SBInterpolatedImageImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/SBKolmogorov.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7989 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/SBKolmogorovImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/SBMoffat.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8095 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/SBMoffatImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16789 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/SBProfile.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9531 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/SBProfileImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/SBSecondKick.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3981 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/SBSecondKickImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6056 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/SBSersic.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11563 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/SBSersicImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2308 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/SBShapelet.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4971 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/SBShapeletImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3813 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/SBSpergel.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9598 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/SBSpergelImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/SBTransform.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10313 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/SBTransformImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/SBVonKarman.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5998 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/SBVonKarmanImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12343 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/Silicon.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16801 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/Solve.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8138 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/Std.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/Stopwatch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6072 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/Table.h
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2023-11-02 02:09:41.000000 GalSim-2.5.1/include/galsim/Version.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/WCS.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 02:09:41.607255 GalSim-2.5.1/include/galsim/boost1_48_0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/boost1_48_0/LICENSE_1_0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/boost1_48_0/README
+-rw-r--r--   0 runner    (1001) docker     (127)     4118 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/boost1_48_0/assert.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 02:09:41.607255 GalSim-2.5.1/include/galsim/boost1_48_0/config/
+-rw-r--r--   0 runner    (1001) docker     (127)    21149 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/boost1_48_0/config/suffix.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/boost1_48_0/current_function.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 02:09:41.611255 GalSim-2.5.1/include/galsim/boost1_48_0/random/
+-rw-r--r--   0 runner    (1001) docker     (127)    12400 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/boost1_48_0/random/binomial_distribution.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6388 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/boost1_48_0/random/chi_squared_distribution.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 02:09:41.611255 GalSim-2.5.1/include/galsim/boost1_48_0/random/detail/
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/boost1_48_0/random/detail/generator_seed_seq.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/boost1_48_0/random/detail/ptr_helper.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5418 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/boost1_48_0/random/detail/seed.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2420 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/boost1_48_0/random/detail/signed_unsigned_tools.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5728 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/boost1_48_0/random/exponential_distribution.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9414 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/boost1_48_0/random/gamma_distribution.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    19903 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/boost1_48_0/random/mersenne_twister.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7472 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/boost1_48_0/random/normal_distribution.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10295 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/boost1_48_0/random/poisson_distribution.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7982 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/boost1_48_0/random/uniform_01.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8594 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/boost1_48_0/random/uniform_real_distribution.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5679 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/boost1_48_0/random/weibull_distribution.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 02:09:41.619255 GalSim-2.5.1/include/galsim/fmath/
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/fmath/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/fmath/README
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/fmath/avx2.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11454 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/fmath/bench.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/fmath/bench.sln
+-rw-r--r--   0 runner    (1001) docker     (127)     7420 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/fmath/bench.vcproj
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/fmath/ck.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    37235 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/fmath/fastexp.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    23954 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/fmath/fmath.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 02:09:41.487252 GalSim-2.5.1/include/galsim/fmath/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 02:09:41.619255 GalSim-2.5.1/include/galsim/fmath/include/cybozu/
+-rw-r--r--   0 runner    (1001) docker     (127)     3896 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/fmath/include/cybozu/benchmark.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/fmath/include/cybozu/inttype.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/fmath/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5899 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/fmath/readme.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 02:09:41.619255 GalSim-2.5.1/include/galsim/hsm/
+-rw-r--r--   0 runner    (1001) docker     (127)    28148 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/hsm/PSFCorr.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 02:09:41.619255 GalSim-2.5.1/include/galsim/integ/
+-rw-r--r--   0 runner    (1001) docker     (127)    42773 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/integ/Int.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12112 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/integ/IntGKPData1.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17415 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/integ/IntGKPData10.h
+-rw-r--r--   0 runner    (1001) docker     (127)    32193 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/integ/MoreFunctional.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 02:09:41.623255 GalSim-2.5.1/include/galsim/math/
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/math/Angle.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/math/Bessel.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/math/Gamma.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/math/Hankel.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/math/Horner.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/math/Nan.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/math/Sinc.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8299 2023-11-02 02:08:37.000000 GalSim-2.5.1/include/galsim/mmgr.h
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2023-11-02 02:08:37.000000 GalSim-2.5.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 02:09:41.631255 GalSim-2.5.1/pysrc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2023-11-02 02:08:37.000000 GalSim-2.5.1/pysrc/Bessel.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2023-11-02 02:08:37.000000 GalSim-2.5.1/pysrc/Bounds.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2023-11-02 02:08:37.000000 GalSim-2.5.1/pysrc/CDModel.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5454 2023-11-02 02:08:37.000000 GalSim-2.5.1/pysrc/HSM.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2023-11-02 02:08:37.000000 GalSim-2.5.1/pysrc/Horner.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3826 2023-11-02 02:08:37.000000 GalSim-2.5.1/pysrc/Image.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2892 2023-11-02 02:08:37.000000 GalSim-2.5.1/pysrc/Integ.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2023-11-02 02:08:37.000000 GalSim-2.5.1/pysrc/Interpolant.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2023-11-02 02:08:37.000000 GalSim-2.5.1/pysrc/PhotonArray.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2023-11-02 02:08:37.000000 GalSim-2.5.1/pysrc/PyBind11Helper.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5471 2023-11-02 02:08:37.000000 GalSim-2.5.1/pysrc/Random.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2023-11-02 02:08:37.000000 GalSim-2.5.1/pysrc/RealGalaxy.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2023-11-02 02:08:37.000000 GalSim-2.5.1/pysrc/SBAdd.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2023-11-02 02:08:37.000000 GalSim-2.5.1/pysrc/SBAiry.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2023-11-02 02:08:37.000000 GalSim-2.5.1/pysrc/SBBox.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2023-11-02 02:08:37.000000 GalSim-2.5.1/pysrc/SBConvolve.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2023-11-02 02:08:37.000000 GalSim-2.5.1/pysrc/SBDeconvolve.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2023-11-02 02:08:37.000000 GalSim-2.5.1/pysrc/SBDeltaFunction.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2023-11-02 02:08:37.000000 GalSim-2.5.1/pysrc/SBExponential.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2023-11-02 02:08:37.000000 GalSim-2.5.1/pysrc/SBFourierSqrt.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2023-11-02 02:08:37.000000 GalSim-2.5.1/pysrc/SBGaussian.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2023-11-02 02:08:37.000000 GalSim-2.5.1/pysrc/SBInclinedExponential.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2023-11-02 02:08:37.000000 GalSim-2.5.1/pysrc/SBInclinedSersic.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2023-11-02 02:08:37.000000 GalSim-2.5.1/pysrc/SBInterpolatedImage.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2023-11-02 02:08:37.000000 GalSim-2.5.1/pysrc/SBKolmogorov.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2023-11-02 02:08:37.000000 GalSim-2.5.1/pysrc/SBMoffat.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2908 2023-11-02 02:08:37.000000 GalSim-2.5.1/pysrc/SBProfile.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2023-11-02 02:08:37.000000 GalSim-2.5.1/pysrc/SBSecondKick.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2023-11-02 02:08:37.000000 GalSim-2.5.1/pysrc/SBSersic.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2023-11-02 02:08:37.000000 GalSim-2.5.1/pysrc/SBShapelet.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2023-11-02 02:08:37.000000 GalSim-2.5.1/pysrc/SBSpergel.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2023-11-02 02:08:37.000000 GalSim-2.5.1/pysrc/SBTransform.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2023-11-02 02:08:37.000000 GalSim-2.5.1/pysrc/SBVonKarman.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2023-11-02 02:08:37.000000 GalSim-2.5.1/pysrc/Silicon.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6730 2023-11-02 02:08:37.000000 GalSim-2.5.1/pysrc/Table.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6714 2023-11-02 02:08:37.000000 GalSim-2.5.1/pysrc/Utilities.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2023-11-02 02:08:37.000000 GalSim-2.5.1/pysrc/WCS.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4021 2023-11-02 02:08:37.000000 GalSim-2.5.1/pysrc/module.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-02 02:09:41.683256 GalSim-2.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    58359 2023-11-02 02:08:37.000000 GalSim-2.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 02:09:41.635255 GalSim-2.5.1/share/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 02:09:41.635255 GalSim-2.5.1/share/SEDs/
+-rw-r--r--   0 runner    (1001) docker     (127)    12280 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/SEDs/CWW_E_ext.sed
+-rw-r--r--   0 runner    (1001) docker     (127)     7392 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/SEDs/CWW_E_ext_more.sed
+-rw-r--r--   0 runner    (1001) docker     (127)    12021 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/SEDs/CWW_Im_ext.sed
+-rw-r--r--   0 runner    (1001) docker     (127)     8017 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/SEDs/CWW_Im_ext_more.sed
+-rw-r--r--   0 runner    (1001) docker     (127)    13010 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/SEDs/CWW_Sbc_ext.sed
+-rw-r--r--   0 runner    (1001) docker     (127)     8460 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/SEDs/CWW_Sbc_ext_more.sed
+-rw-r--r--   0 runner    (1001) docker     (127)    12932 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/SEDs/CWW_Scd_ext.sed
+-rw-r--r--   0 runner    (1001) docker     (127)     8356 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/SEDs/CWW_Scd_ext_more.sed
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/SEDs/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   102422 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/SEDs/vega.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    57600 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/acs_I_unrot_sci_20_cf.fits
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 02:09:41.639255 GalSim-2.5.1/share/bandpasses/
+-rw-r--r--   0 runner    (1001) docker     (127)     5885 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/bandpasses/ACS_wfc_F435W.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    11657 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/bandpasses/ACS_wfc_F606W.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     4611 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/bandpasses/ACS_wfc_F775W.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     8823 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/bandpasses/ACS_wfc_F814W.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     4093 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/bandpasses/ACS_wfc_F850LP.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/bandpasses/LSST_g.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     3384 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/bandpasses/LSST_i.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/bandpasses/LSST_r.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/bandpasses/LSST_u.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     6036 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/bandpasses/LSST_y.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     3410 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/bandpasses/LSST_z.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/bandpasses/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/bandpasses/WFC3_ir_F105W.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/bandpasses/WFC3_ir_F125W.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/bandpasses/WFC3_ir_F160W.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/bandpasses/WFC3_uvis_F275W.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/bandpasses/WFC3_uvis_F336W.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 02:09:41.651255 GalSim-2.5.1/share/roman/
+-rw-r--r--   0 runner    (1001) docker     (127)    72363 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/roman/RST_WIM_Filter_F184_SCA_1.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    72815 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/roman/RST_WIM_Filter_F184_SCA_10.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    71900 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/roman/RST_WIM_Filter_F184_SCA_11.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    71312 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/roman/RST_WIM_Filter_F184_SCA_12.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    73332 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/roman/RST_WIM_Filter_F184_SCA_13.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    73256 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/roman/RST_WIM_Filter_F184_SCA_14.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    72231 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/roman/RST_WIM_Filter_F184_SCA_15.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    75714 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/roman/RST_WIM_Filter_F184_SCA_16.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    73288 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/roman/RST_WIM_Filter_F184_SCA_17.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    72988 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/roman/RST_WIM_Filter_F184_SCA_18.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    72683 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/roman/RST_WIM_Filter_F184_SCA_2.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    71938 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/roman/RST_WIM_Filter_F184_SCA_3.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    72860 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/roman/RST_WIM_Filter_F184_SCA_4.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    72153 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/roman/RST_WIM_Filter_F184_SCA_5.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    71630 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/roman/RST_WIM_Filter_F184_SCA_6.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    76049 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/roman/RST_WIM_Filter_F184_SCA_7.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    73119 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/roman/RST_WIM_Filter_F184_SCA_8.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    72505 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/roman/RST_WIM_Filter_F184_SCA_9.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    74944 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/roman/RST_WIM_Filter_skinny_SCA_1.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    74222 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/roman/RST_WIM_Filter_skinny_SCA_10.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    73499 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/roman/RST_WIM_Filter_skinny_SCA_11.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    72953 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/roman/RST_WIM_Filter_skinny_SCA_12.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    77295 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/roman/RST_WIM_Filter_skinny_SCA_13.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    73917 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/roman/RST_WIM_Filter_skinny_SCA_14.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    73364 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/roman/RST_WIM_Filter_skinny_SCA_15.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    77941 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/roman/RST_WIM_Filter_skinny_SCA_16.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    78030 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/roman/RST_WIM_Filter_skinny_SCA_17.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    77598 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/roman/RST_WIM_Filter_skinny_SCA_18.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    74701 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/roman/RST_WIM_Filter_skinny_SCA_2.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    73506 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/roman/RST_WIM_Filter_skinny_SCA_3.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    78098 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/roman/RST_WIM_Filter_skinny_SCA_4.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    75183 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/roman/RST_WIM_Filter_skinny_SCA_5.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    73645 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/roman/RST_WIM_Filter_skinny_SCA_6.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    77605 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/roman/RST_WIM_Filter_skinny_SCA_7.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    77370 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/roman/RST_WIM_Filter_skinny_SCA_8.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    77167 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/roman/RST_WIM_Filter_skinny_SCA_9.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_03.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_04.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_05.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_06.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_07.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_08.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_09.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_10.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_11.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_12.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_13.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_14.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_15.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_16.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_17.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_18.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   204929 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/roman/Roman_SRR_WFC_Pupil_Mask_Longwave_2048_reformatted.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   207326 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/roman/Roman_SRR_WFC_Pupil_Mask_Shortwave_2048_reformatted.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    53490 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/roman/Roman_effarea_20210614.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   206809 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/roman/roman_sky_backgrounds.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/roman/sca_positions_20210204.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16920 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/roman/sip_20210204.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 02:09:41.659256 GalSim-2.5.1/share/sensors/
+-rw-r--r--   0 runner    (1001) docker     (127)     5054 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/sensors/abs_length.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    10297 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/sensors/lsst_e2v_32.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)   812668 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/sensors/lsst_e2v_32.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    10060 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/sensors/lsst_e2v_50_32.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)   812668 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/sensors/lsst_e2v_50_32.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    10061 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/sensors/lsst_e2v_50_8.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)   221692 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/sensors/lsst_e2v_50_8.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    10296 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/sensors/lsst_e2v_8.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)   221692 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/sensors/lsst_e2v_8.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    10365 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/sensors/lsst_itl_32.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)   812668 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/sensors/lsst_itl_32.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    10374 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/sensors/lsst_itl_50_32.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)   812668 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/sensors/lsst_itl_50_32.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    10375 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/sensors/lsst_itl_50_8.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)   221692 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/sensors/lsst_itl_50_8.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    10365 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/sensors/lsst_itl_8.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)   221692 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/sensors/lsst_itl_8.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   122780 2023-11-02 02:08:37.000000 GalSim-2.5.1/share/wfc_F814W.dat.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 02:09:41.667256 GalSim-2.5.1/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2023-11-02 02:08:37.000000 GalSim-2.5.1/src/BinomFact.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4870 2023-11-02 02:08:37.000000 GalSim-2.5.1/src/CDModel.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2023-11-02 02:08:37.000000 GalSim-2.5.1/src/CorrelatedNoise.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5752 2023-11-02 02:08:37.000000 GalSim-2.5.1/src/GSParams.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    54447 2023-11-02 02:08:37.000000 GalSim-2.5.1/src/Image.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2023-11-02 02:08:37.000000 GalSim-2.5.1/src/Image.inst
+-rw-r--r--   0 runner    (1001) docker     (127)    35052 2023-11-02 02:08:37.000000 GalSim-2.5.1/src/Interpolant.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    19072 2023-11-02 02:08:37.000000 GalSim-2.5.1/src/Laguerre.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    22231 2023-11-02 02:08:37.000000 GalSim-2.5.1/src/OneDimensionalDeviate.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8020 2023-11-02 02:08:37.000000 GalSim-2.5.1/src/PhotonArray.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6426 2023-11-02 02:08:37.000000 GalSim-2.5.1/src/Polygon.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    27173 2023-11-02 02:08:37.000000 GalSim-2.5.1/src/Random.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7380 2023-11-02 02:08:37.000000 GalSim-2.5.1/src/RealGalaxy.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    15670 2023-11-02 02:08:37.000000 GalSim-2.5.1/src/RealSpaceConvolve.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10263 2023-11-02 02:08:37.000000 GalSim-2.5.1/src/SBAdd.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    16980 2023-11-02 02:08:37.000000 GalSim-2.5.1/src/SBAiry.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    17398 2023-11-02 02:08:37.000000 GalSim-2.5.1/src/SBBox.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    19001 2023-11-02 02:08:37.000000 GalSim-2.5.1/src/SBConvolve.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6731 2023-11-02 02:08:37.000000 GalSim-2.5.1/src/SBDeconvolve.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3028 2023-11-02 02:08:37.000000 GalSim-2.5.1/src/SBDeltaFunction.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    25768 2023-11-02 02:08:37.000000 GalSim-2.5.1/src/SBExponential.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4759 2023-11-02 02:08:37.000000 GalSim-2.5.1/src/SBFourierSqrt.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12029 2023-11-02 02:08:37.000000 GalSim-2.5.1/src/SBGaussian.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    14238 2023-11-02 02:08:37.000000 GalSim-2.5.1/src/SBInclinedExponential.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    15106 2023-11-02 02:08:37.000000 GalSim-2.5.1/src/SBInclinedSersic.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    62389 2023-11-02 02:08:37.000000 GalSim-2.5.1/src/SBInterpolatedImage.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    18274 2023-11-02 02:08:37.000000 GalSim-2.5.1/src/SBKolmogorov.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    25486 2023-11-02 02:08:37.000000 GalSim-2.5.1/src/SBMoffat.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    24029 2023-11-02 02:08:37.000000 GalSim-2.5.1/src/SBProfile.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    16498 2023-11-02 02:08:37.000000 GalSim-2.5.1/src/SBSecondKick.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    33842 2023-11-02 02:08:37.000000 GalSim-2.5.1/src/SBSersic.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13511 2023-11-02 02:08:37.000000 GalSim-2.5.1/src/SBShapelet.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    29887 2023-11-02 02:08:37.000000 GalSim-2.5.1/src/SBSpergel.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    44809 2023-11-02 02:08:37.000000 GalSim-2.5.1/src/SBTransform.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    20081 2023-11-02 02:08:37.000000 GalSim-2.5.1/src/SBVonKarman.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    70507 2023-11-02 02:08:37.000000 GalSim-2.5.1/src/Silicon.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    53187 2023-11-02 02:08:37.000000 GalSim-2.5.1/src/Table.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2023-11-02 02:08:37.000000 GalSim-2.5.1/src/Version.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12132 2023-11-02 02:08:37.000000 GalSim-2.5.1/src/WCS.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 02:09:41.667256 GalSim-2.5.1/src/hsm/
+-rw-r--r--   0 runner    (1001) docker     (127)    78969 2023-11-02 02:08:37.000000 GalSim-2.5.1/src/hsm/PSFCorr.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 02:09:41.667256 GalSim-2.5.1/src/math/
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2023-11-02 02:08:37.000000 GalSim-2.5.1/src/math/Angle.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6683 2023-11-02 02:08:37.000000 GalSim-2.5.1/src/math/Bessel.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    43843 2023-11-02 02:08:37.000000 GalSim-2.5.1/src/math/BesselI.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    74848 2023-11-02 02:08:37.000000 GalSim-2.5.1/src/math/BesselJ.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    45424 2023-11-02 02:08:37.000000 GalSim-2.5.1/src/math/BesselK.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6312 2023-11-02 02:08:37.000000 GalSim-2.5.1/src/math/BesselRoots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    63931 2023-11-02 02:08:37.000000 GalSim-2.5.1/src/math/BesselY.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    24658 2023-11-02 02:08:37.000000 GalSim-2.5.1/src/math/Gamma.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9825 2023-11-02 02:08:37.000000 GalSim-2.5.1/src/math/Hankel.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4557 2023-11-02 02:08:37.000000 GalSim-2.5.1/src/math/Horner.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2023-11-02 02:08:37.000000 GalSim-2.5.1/src/math/Nan.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9748 2023-11-02 02:08:37.000000 GalSim-2.5.1/src/math/Sinc.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    73348 2023-11-02 02:08:37.000000 GalSim-2.5.1/src/mmgr.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 02:09:41.683256 GalSim-2.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    12631 2023-11-02 02:08:37.000000 GalSim-2.5.1/tests/test_airy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20750 2023-11-02 02:08:37.000000 GalSim-2.5.1/tests/test_bandpass.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18529 2023-11-02 02:08:37.000000 GalSim-2.5.1/tests/test_bessel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15067 2023-11-02 02:08:37.000000 GalSim-2.5.1/tests/test_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18703 2023-11-02 02:08:37.000000 GalSim-2.5.1/tests/test_calc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14455 2023-11-02 02:08:37.000000 GalSim-2.5.1/tests/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16370 2023-11-02 02:08:37.000000 GalSim-2.5.1/tests/test_cdmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37474 2023-11-02 02:08:37.000000 GalSim-2.5.1/tests/test_celestial.py
+-rw-r--r--   0 runner    (1001) docker     (127)   154183 2023-11-02 02:08:37.000000 GalSim-2.5.1/tests/test_chromatic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91493 2023-11-02 02:08:37.000000 GalSim-2.5.1/tests/test_config_gsobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)   138579 2023-11-02 02:08:37.000000 GalSim-2.5.1/tests/test_config_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17439 2023-11-02 02:08:37.000000 GalSim-2.5.1/tests/test_config_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34185 2023-11-02 02:08:37.000000 GalSim-2.5.1/tests/test_config_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73746 2023-11-02 02:08:37.000000 GalSim-2.5.1/tests/test_config_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)    88975 2023-11-02 02:08:37.000000 GalSim-2.5.1/tests/test_config_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44767 2023-11-02 02:08:37.000000 GalSim-2.5.1/tests/test_convolve.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69505 2023-11-02 02:08:37.000000 GalSim-2.5.1/tests/test_correlatednoise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8020 2023-11-02 02:08:37.000000 GalSim-2.5.1/tests/test_deltafunction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32195 2023-11-02 02:08:37.000000 GalSim-2.5.1/tests/test_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34166 2023-11-02 02:08:37.000000 GalSim-2.5.1/tests/test_des.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22196 2023-11-02 02:08:37.000000 GalSim-2.5.1/tests/test_detectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26046 2023-11-02 02:08:37.000000 GalSim-2.5.1/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86539 2023-11-02 02:08:37.000000 GalSim-2.5.1/tests/test_draw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9229 2023-11-02 02:08:37.000000 GalSim-2.5.1/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10716 2023-11-02 02:08:37.000000 GalSim-2.5.1/tests/test_exponential.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10407 2023-11-02 02:08:37.000000 GalSim-2.5.1/tests/test_fitsheader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4445 2023-11-02 02:08:37.000000 GalSim-2.5.1/tests/test_fouriersqrt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20703 2023-11-02 02:08:37.000000 GalSim-2.5.1/tests/test_galaxy_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18408 2023-11-02 02:08:37.000000 GalSim-2.5.1/tests/test_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51280 2023-11-02 02:08:37.000000 GalSim-2.5.1/tests/test_hsm.py
+-rw-r--r--   0 runner    (1001) docker     (127)   168100 2023-11-02 02:08:37.000000 GalSim-2.5.1/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29539 2023-11-02 02:08:37.000000 GalSim-2.5.1/tests/test_inclined.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14962 2023-11-02 02:08:37.000000 GalSim-2.5.1/tests/test_integ.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85965 2023-11-02 02:08:37.000000 GalSim-2.5.1/tests/test_interpolatedimage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14275 2023-11-02 02:08:37.000000 GalSim-2.5.1/tests/test_knots.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18435 2023-11-02 02:08:37.000000 GalSim-2.5.1/tests/test_kolmogorov.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78648 2023-11-02 02:08:37.000000 GalSim-2.5.1/tests/test_lensing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12085 2023-11-02 02:08:37.000000 GalSim-2.5.1/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20983 2023-11-02 02:08:37.000000 GalSim-2.5.1/tests/test_metacal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25068 2023-11-02 02:08:37.000000 GalSim-2.5.1/tests/test_moffat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35496 2023-11-02 02:08:37.000000 GalSim-2.5.1/tests/test_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48379 2023-11-02 02:08:37.000000 GalSim-2.5.1/tests/test_optics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65379 2023-11-02 02:08:37.000000 GalSim-2.5.1/tests/test_phase_psf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72381 2023-11-02 02:08:37.000000 GalSim-2.5.1/tests/test_photon_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9321 2023-11-02 02:08:37.000000 GalSim-2.5.1/tests/test_pse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81608 2023-11-02 02:08:37.000000 GalSim-2.5.1/tests/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43941 2023-11-02 02:08:37.000000 GalSim-2.5.1/tests/test_real.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67201 2023-11-02 02:08:37.000000 GalSim-2.5.1/tests/test_roman.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13305 2023-11-02 02:08:37.000000 GalSim-2.5.1/tests/test_second_kick.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58842 2023-11-02 02:08:37.000000 GalSim-2.5.1/tests/test_sed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60777 2023-11-02 02:08:37.000000 GalSim-2.5.1/tests/test_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27331 2023-11-02 02:08:37.000000 GalSim-2.5.1/tests/test_sersic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16575 2023-11-02 02:08:37.000000 GalSim-2.5.1/tests/test_shapelet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13439 2023-11-02 02:08:37.000000 GalSim-2.5.1/tests/test_shear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4231 2023-11-02 02:08:37.000000 GalSim-2.5.1/tests/test_shear_position.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15117 2023-11-02 02:08:37.000000 GalSim-2.5.1/tests/test_spergel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14630 2023-11-02 02:08:37.000000 GalSim-2.5.1/tests/test_sum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53035 2023-11-02 02:08:37.000000 GalSim-2.5.1/tests/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47931 2023-11-02 02:08:37.000000 GalSim-2.5.1/tests/test_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62197 2023-11-02 02:08:37.000000 GalSim-2.5.1/tests/test_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15824 2023-11-02 02:08:37.000000 GalSim-2.5.1/tests/test_vonkarman.py
+-rw-r--r--   0 runner    (1001) docker     (127)   152082 2023-11-02 02:08:37.000000 GalSim-2.5.1/tests/test_wcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53232 2023-11-02 02:08:37.000000 GalSim-2.5.1/tests/test_zernike.py
```

### Comparing `GalSim-2.5.0/CHANGELOG.rst` & `GalSim-2.5.1/CHANGELOG.rst`

 * *Files 24% similar despite different names*

```diff
@@ -78,7 +78,30 @@
   rather than raising an exception. (#1227)
 - Changed the SED class to correctly broadcast over waves when the SED is constant. (#1228, #1235)
 - Fixed some errors when drawing ChromaticTransformation objects with photon shooting. (#1229)
 - Fixed the flux drawn by ChromaticConvolution with photon shooting when poisson_flux=True. (#1229)
 - Fixed a slight inaccuracy in the FFT phase shifts for single-precision images. (#1231, #1234)
 - Fixed a bug that prevented a convolution of two PhaseScreenPSF objects from being drawn with
   photon shooting. (#1242)
+
+
+Changes from v2.5.0 to v2.5.1
+=============================
+
+- Fixed an incompatibility with Python 3.12 that we had missed.
+- Fixed a bug in the SED class normalization when using astropy.units for flux_type.  Thanks
+  to Sid Mau for finding and fixing this bug. (#1254, #1256)
+- Fixed a bug in the `EmissionLine.atRedshift` method. (#1257)
+- Added interpolant option to `SED` and `Bandpass` classes to use when reading from a file.
+  (#1257)
+- Improved the behavior of SEDs when using spline interpolant. (#1187, #1257)
+- No longer pickle the SED of chromatic objects when the SED is a derived value. (#1257)
+- Added interpolant option to `galsim.trapz`. (#1257)
+- Added clip_neg option to `DistDeviate` class. (#1257)
+- Fixed a bug in `SiliconSensor` if the image is outside the range where tree rings are defined.
+  (#1258)
+- Implemented algorith for `ChromaticSum` to be used as a photon_op. (#1259)
+- Added `PhotonArray.copyFrom` method. (#1259)
+- Deprecated `PhotonArray.setCorrelated` and `PhotonArray.isCorrelated`, since they are not
+  necessary anymore. (#1259)
+- Deprecated `PhotonArray.assignAt` in favor of the more flexible `PhotonArray.copyFrom`
+  method. (#1259)
```

### Comparing `GalSim-2.5.0/GalSim.egg-info/PKG-INFO` & `GalSim-2.5.1/GalSim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: GalSim
-Version: 2.5.0
+Version: 2.5.1
 Summary: The modular galaxy image simulation toolkit
 Home-page: https://github.com/GalSim-developers/GalSim
-Download-URL: https://github.com/GalSim-developers/GalSim/releases/tag/v2.5.0.zip
+Download-URL: https://github.com/GalSim-developers/GalSim/releases/tag/v2.5.1.zip
 Author: GalSim Developers (point of contact: Mike Jarvis)
 Author-email: michael@jarvis.net
 License: BSD License
 License-File: LICENSE
 Requires-Dist: setuptools>=38
 Requires-Dist: pybind11>=2.2
 Requires-Dist: numpy>=1.17
```

### Comparing `GalSim-2.5.0/GalSim.egg-info/SOURCES.txt` & `GalSim-2.5.1/GalSim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/INSTALL.rst` & `GalSim-2.5.1/INSTALL.rst`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/LICENSE` & `GalSim-2.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/PKG-INFO` & `GalSim-2.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: GalSim
-Version: 2.5.0
+Version: 2.5.1
 Summary: The modular galaxy image simulation toolkit
 Home-page: https://github.com/GalSim-developers/GalSim
-Download-URL: https://github.com/GalSim-developers/GalSim/releases/tag/v2.5.0.zip
+Download-URL: https://github.com/GalSim-developers/GalSim/releases/tag/v2.5.1.zip
 Author: GalSim Developers (point of contact: Mike Jarvis)
 Author-email: michael@jarvis.net
 License: BSD License
 License-File: LICENSE
 Requires-Dist: setuptools>=38
 Requires-Dist: pybind11>=2.2
 Requires-Dist: numpy>=1.17
```

### Comparing `GalSim-2.5.0/README.rst` & `GalSim-2.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/__init__.py` & `GalSim-2.5.1/galsim/__init__.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/__main__.py` & `GalSim-2.5.1/galsim/__main__.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/_pyfits.py` & `GalSim-2.5.1/galsim/_pyfits.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/_utilities.py` & `GalSim-2.5.1/galsim/_utilities.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/_version.py` & `GalSim-2.5.1/galsim/_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,9 +11,9 @@
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions, and the disclaimer given in the accompanying LICENSE
 #    file.
 # 2. Redistributions in binary form must reproduce the above copyright notice,
 #    this list of conditions, and the disclaimer given in the documentation
 #    and/or other materials provided with the distribution.
 #
-__version__ = '2.5.0'
+__version__ = '2.5.1'
 __version_info__ = tuple(map(lambda x:int(x.split('-')[0]), __version__.split('.')))[:3]
```

### Comparing `GalSim-2.5.0/galsim/airy.py` & `GalSim-2.5.1/galsim/airy.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/angle.py` & `GalSim-2.5.1/galsim/angle.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/bandpass.py` & `GalSim-2.5.1/galsim/bandpass.py`

 * *Files 3% similar despite different names*

```diff
@@ -101,31 +101,33 @@
         blue_limit:     Hard cut off of bandpass on the blue side. [default: None, but required
                         if throughput is not a `LookupTable` or file.  See above.]
         red_limit:      Hard cut off of bandpass on the red side. [default: None, but required
                         if throughput is not a `LookupTable` or file.  See above.]
         zeropoint:      Set the zero-point for this Bandpass.  Here, this can only be a float
                         value.  See the method `withZeropoint` for other options for how to
                         set this using a particular spectrum (AB, Vega, etc.) [default: None]
+        interpolant:    If reading from a file, what interpolant to use. [default: 'linear']
     """
     def __init__(self, throughput, wave_type, blue_limit=None, red_limit=None,
-                 zeropoint=None, _wave_list=None, _tp=None):
+                 zeropoint=None, interpolant='linear', _wave_list=None, _tp=None):
         # Note that `_wave_list` acts as a private construction variable that overrides the way that
         # `wave_list` is normally constructed (see `Bandpass.__mul__` below)
 
         self._orig_tp = throughput  # Save this for pickling.
         self._tp = _tp              # This will normally become orig_tp turned into an actual
                                     # function (see _initialize_tp()), although in some cases,
                                     # it can be supplied directly as a constructor argument.
 
         if blue_limit is not None and red_limit is not None and blue_limit >= red_limit:
             raise GalSimRangeError("blue_limit must be less than red_limit",
                                    blue_limit, None, red_limit)
         self.blue_limit = blue_limit # These may change as we go through this.
         self.red_limit = red_limit
         self.zeropoint = zeropoint
+        self.interpolant = interpolant
 
         # Parse the various options for wave_type
         if isinstance(wave_type, str):
             if wave_type.lower() in ('nm', 'nanometer', 'nanometers'):
                 self.wave_type = 'nm'
                 self.wave_factor = 1.
             elif wave_type.lower() in ('a', 'ang', 'angstrom', 'angstroms'):
@@ -218,15 +220,15 @@
         # The function cannot be pickled, so will need to do this in setstate as well as init.
 
         if self._tp is not None:
             pass
         elif isinstance(self._orig_tp, basestring):
             isfile, filename = utilities.check_share_file(self._orig_tp, 'bandpasses')
             if isfile:
-                self._tp = LookupTable.from_file(filename, interpolant='linear')
+                self._tp = LookupTable.from_file(filename, interpolant=self.interpolant)
             else:
                 if self.blue_limit is None or self.red_limit is None:
                     raise GalSimIncompatibleValuesError(
                         "red_limit and blue_limit are required if throughput is not a LookupTable.",
                         blue_limit=None, red_limit=None, throughput=self._orig_tp)
                 test_wave = self.blue_limit
                 try:
@@ -429,16 +431,17 @@
             zeropoint = 2.5 * np.log10(flux)
 
         # Should be a float now (or maybe an int).  If not, raise an exception.
         if not isinstance(zeropoint, (float, int)):
             raise TypeError(
                    "Don't know how to handle zeropoint of type: {0}".format(type(zeropoint)))
 
-        return Bandpass(self._orig_tp, self.wave_type, self.blue_limit, self.red_limit, zeropoint,
-                        self.wave_list, self._tp)
+        return Bandpass(self._orig_tp, self.wave_type, self.blue_limit, self.red_limit,
+                        zeropoint=zeropoint, interpolant=self.interpolant,
+                        _wave_list=self.wave_list, _tp=self._tp)
 
     def truncate(self, blue_limit=None, red_limit=None, relative_throughput=None,
                  preserve_zp='auto'):
         """Return a bandpass with its wavelength range truncated.
 
         This function truncate the range of the bandpass either explicitly (with ``blue_limit`` or
         ``red_limit`` or both) or automatically, just trimming off leading and trailing wavelength
@@ -524,17 +527,19 @@
         elif relative_throughput is not None:
             raise GalSimIncompatibleValuesError(
                 "Can only truncate with relative_throughput argument if throughput is "
                 "a LookupTable", relative_throughput=relative_throughput, throughput=self._orig_tp)
 
         if preserve_zp:
             return Bandpass(self._orig_tp, self.wave_type, blue_limit, red_limit,
-                            _wave_list=wave_list, _tp=self._tp, zeropoint=self.zeropoint)
+                            zeropoint=self.zeropoint, interpolant=self.interpolant,
+                            _wave_list=wave_list, _tp=self._tp)
         else:
             return Bandpass(self._orig_tp, self.wave_type, blue_limit, red_limit,
+                            interpolant=self.interpolant,
                             _wave_list=wave_list, _tp=self._tp)
 
     def thin(self, rel_err=1.e-4, trim_zeros=True, preserve_range=True, fast_search=True,
              preserve_zp=True):
         """Thin out the internal wavelengths of a `Bandpass` that uses a `LookupTable`.
 
         If the bandpass was initialized with a `LookupTable` or from a file (which internally
@@ -582,19 +587,22 @@
 
         Returns:
             the thinned `Bandpass`.
         """
         if len(self.wave_list) > 0:
             x = self.wave_list
             f = self(x)
+            interpolant = (self.interpolant if not isinstance(self._tp, LookupTable)
+                           else self._tp.interpolant)
             newx, newf = utilities.thin_tabulated_values(x, f, rel_err=rel_err,
                                                          trim_zeros=trim_zeros,
                                                          preserve_range=preserve_range,
-                                                         fast_search=fast_search)
-            tp = _LookupTable(newx, newf, 'linear')
+                                                         fast_search=fast_search,
+                                                         interpolant=interpolant)
+            tp = _LookupTable(newx, newf, interpolant)
             blue_limit = np.min(newx)
             red_limit = np.max(newx)
             wave_list = np.array(newx)
             if preserve_zp:
                 return Bandpass(tp, 'nm', blue_limit, red_limit, _wave_list=wave_list,
                                 zeropoint=self.zeropoint)
             else:
@@ -618,17 +626,17 @@
         if not hasattr(self, '_hash'):
             self._hash = hash(("galsim.Bandpass", self._orig_tp, self.blue_limit, self.red_limit,
                                self.wave_factor, self.zeropoint, tuple(self.wave_list)))
         return self._hash
 
     def __repr__(self):
         return ('galsim.Bandpass(%r, wave_type=%r, blue_limit=%r, red_limit=%r, zeropoint=%r, '
-                                 '_wave_list=array(%r))')%(
-                self._orig_tp, self.wave_type, self.blue_limit, self.red_limit, self.zeropoint,
-                self.wave_list.tolist())
+                'interpolant=%r, _wave_list=array(%r))')%(
+                    self._orig_tp, self.wave_type, self.blue_limit, self.red_limit,
+                    self.zeropoint, self.interpolant, self.wave_list.tolist())
 
     def __str__(self):
         orig_tp = repr(self._orig_tp)
         if len(orig_tp) > 80:
             orig_tp = str(self._orig_tp)
         return 'galsim.Bandpass(%s)'%self._orig_tp
```

### Comparing `GalSim-2.5.0/galsim/bessel.py` & `GalSim-2.5.1/galsim/bessel.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/bounds.py` & `GalSim-2.5.1/galsim/bounds.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/box.py` & `GalSim-2.5.1/galsim/box.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/catalog.py` & `GalSim-2.5.1/galsim/catalog.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/cdmodel.py` & `GalSim-2.5.1/galsim/cdmodel.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/celestial.py` & `GalSim-2.5.1/galsim/celestial.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/chromatic.py` & `GalSim-2.5.1/galsim/chromatic.py`

 * *Files 2% similar despite different names*

```diff
@@ -611,20 +611,15 @@
                             bundle in case the operator needs this information.  [default: None]
             rng:            A random number generator to use to effect the convolution.
                             [default: None]
         """
         if not photon_array.hasAllocatedWavelengths():
             raise GalSimError("Using ChromaticObject as a PhotonOp requires wavelengths be set")
         p1 = PhotonArray(len(photon_array))
-        p1._wave = photon_array._wave
-        if photon_array.hasAllocatedPupil():
-            p1._pupil_u = photon_array._pupil_u
-            p1._pupil_v = photon_array._pupil_v
-        if photon_array.hasAllocatedTimes():
-            p1._time = photon_array._time
+        p1._copyFrom(photon_array, slice(None), slice(None), do_xy=False, do_flux=False)
         obj = local_wcs.toImage(self) if local_wcs is not None else self
         rng = BaseDeviate(rng)
         obj._shoot(p1, rng)
         photon_array.convolve(p1, rng)
 
     # Make op* and op*= work to adjust the flux of the object
     def __mul__(self, flux_ratio):
@@ -1384,20 +1379,20 @@
         UniformDeviate(rng).generate(u)
         use_k = k - (u<f0).astype(int)  # The second term is either 0 or 1.
 
         # Draw photons from the saved profiles according to when we have selected to use each one.
         for kk, obj in enumerate(self.objs):
             use = (use_k == kk)  # True for each photon where this is the object to shoot from
             temp = PhotonArray(np.sum(use))
+            temp._copyFrom(photons, slice(None), use, do_xy=False, do_flux=False)
             obj._shoot(temp, rng)
-            photons.x[use] = temp.x
-            photons.y[use] = temp.y
             # It will have tried to shoot the right total flux.  But that's not correct.
             # Rescale it down by the fraction of the total flux we actually want in this set.
-            photons.flux[use] = temp.flux * (len(temp)/len(photons))
+            temp.scaleFlux(len(temp)/len(photons))
+            photons._copyFrom(temp, use, slice(None))
 
     def _get_interp_image(self, bandpass, image=None, integrator='quadratic',
                           _flux_ratio=None, **kwargs):
         if integrator == 'quadratic':
             rule = integ.quadRule
         elif integrator == 'trapezoidal':
             rule = integ.trapzRule
@@ -1891,14 +1886,22 @@
             s += '.shift(%s,%s)'%(self._offset[0],self._offset[1])
         if self._flux_ratio != 1.:
             s += '.withScaledFlux(%s)'%self._flux_ratio
         if self._redshift is not None:
             s += '.atRedshift(%s)'%(self._redshift)
         return s
 
+    def __getstate__(self):
+        d = self.__dict__.copy()
+        d.pop('sed',None)
+        return d
+
+    def __setstate__(self, d):
+        self.__dict__ = d
+
     def _getTransformations(self, wave):
         if hasattr(self._jac, '__call__'):
             jac = self._jac(wave)
         else:
             jac = self._jac
         if hasattr(self._offset, '__call__'):
             offset = self._offset(wave)
@@ -2080,14 +2083,22 @@
                 'gsparams=%r, propagate_gsparams=%r)')%(
             self.original, self._flux_ratio,
             self._gsparams, self._propagate_gsparams)
 
     def __str__(self):
         return str(self.original) + ' * ' + str(self.sed)
 
+    def __getstate__(self):
+        d = self.__dict__.copy()
+        d.pop('sed',None)
+        return d
+
+    def __setstate__(self, d):
+        self.__dict__ = d
+
     def _getTransformations(self, wave):
         flux_ratio = self._flux_ratio(wave)
         return self._jac, self._offset, flux_ratio
 
     def _shoot(self, photons, rng):
         self._original._shoot(photons, rng)
         wave = photons.wavelength
@@ -2265,28 +2276,61 @@
         return 'galsim.ChromaticSum(%r, gsparams=%r, propagate_gsparams=%r)'%(
                 self.obj_list, self._gsparams, self._propagate_gsparams)
 
     def __str__(self):
         str_list = [ str(obj) for obj in self.obj_list ]
         return 'galsim.ChromaticSum([%s])'%', '.join(str_list)
 
+    def __getstate__(self):
+        d = self.__dict__.copy()
+        d.pop('sed',None)
+        return d
+
+    def __setstate__(self, d):
+        self.__dict__ = d
+
     def evaluateAtWavelength(self, wave):
         """Evaluate this chromatic object at a particular wavelength ``wave``.
 
         Parameters:
             wave:   Wavelength in nanometers.
 
         Returns:
             the monochromatic object at the given wavelength.
         """
         return Add([obj.evaluateAtWavelength(wave) for obj in self.obj_list],
                    gsparams=self._gsparams, propagate_gsparams=self._propagate_gsparams)
 
     def _shoot(self, photons, rng):
-        raise GalSimNotImplementedError("ChromaticSum cannot be used as a PhotonOp")
+        w = photons.wavelength
+
+        # We probabilistically choose a component for each photon based on the
+        # relative flux density of that component for the given wavelength.
+        comp_flux = np.array([obj.sed(w) for obj in self._obj_list])
+        total_flux = np.sum(comp_flux, axis=0)
+
+        prob = comp_flux / total_flux
+        cdf = np.cumsum(prob, axis=0)
+
+        u = np.empty(len(photons))
+        UniformDeviate(rng).generate(u)
+        use_k = np.sum((u >= cdf), axis=0)
+        n = len(self._obj_list)
+        use_k[use_k==n] = n-1  # This shouldn't be possible, but maybe with numerical rounding...
+
+        # Draw photons from the components.
+        for kk, obj in enumerate(self._obj_list):
+            use = (use_k == kk)  # True for each photon where this is the object to shoot from
+            this_n = np.sum(use)
+            if this_n == 0:
+                continue
+            temp = PhotonArray(this_n)
+            temp._copyFrom(photons, slice(None), use, do_xy=False, do_flux=False)
+            obj._shoot(temp, rng)
+            photons._copyFrom(temp, use, slice(None))
 
     def drawImage(self, bandpass, image=None, integrator='quadratic', **kwargs):
         """Slightly optimized draw method for `ChromaticSum` instances.
 
         Draws each summand individually and add resulting images together.  This might waste time if
         two or more summands are separable and have the same `SED`, and another summand with a
         different `SED` is also added, in which case the summands should be added together first and
@@ -2576,14 +2620,22 @@
         return 'galsim.ChromaticConvolution(%r, gsparams=%r, propagate_gsparams=%r)'%(
                 self.obj_list, self._gsparams, self._propagate_gsparams)
 
     def __str__(self):
         str_list = [ str(obj) for obj in self.obj_list ]
         return 'galsim.ChromaticConvolution([%s])'%', '.join(str_list)
 
+    def __getstate__(self):
+        d = self.__dict__.copy()
+        d.pop('sed',None)
+        return d
+
+    def __setstate__(self, d):
+        self.__dict__ = d
+
     def _approxWavelength(self, wave):
         # If any of the components prefer a different wavelength, use that for all.
         achrom_objs = []
         for k, obj in enumerate(self.obj_list):
             new_wave, aobj = obj._approxWavelength(wave)
             if new_wave != wave:
                 # Break the loop and use evaluateAtWavelength for everything else.
@@ -2981,14 +3033,22 @@
         return ('galsim.ChromaticAutoConvolution(%r, real_space=%r, gsparams=%r, '
                 'propagate_gsparams=%r)')%(
                 self._obj, self._real_space, self.gsparams, self._propagate_gsparams)
 
     def __str__(self):
         return 'galsim.ChromaticAutoConvolution(%s)'%self._obj
 
+    def __getstate__(self):
+        d = self.__dict__.copy()
+        d.pop('sed',None)
+        return d
+
+    def __setstate__(self, d):
+        self.__dict__ = d
+
     def evaluateAtWavelength(self, wave):
         """Evaluate this chromatic object at a particular wavelength ``wave``.
 
         Parameters:
             wave:   Wavelength in nanometers.
 
         Returns:
@@ -3078,14 +3138,22 @@
         return ('galsim.ChromaticAutoCorrelation(%r, real_space=%r, gsparams=%r, '
                 'propagate_gsparams=%r)')%(
                 self._obj, self._real_space, self.gsparams, self._propagate_gsparams)
 
     def __str__(self):
         return 'galsim.ChromaticAutoCorrelation(%s)'%self._obj
 
+    def __getstate__(self):
+        d = self.__dict__.copy()
+        d.pop('sed',None)
+        return d
+
+    def __setstate__(self, d):
+        self.__dict__ = d
+
     def evaluateAtWavelength(self, wave):
         """Evaluate this chromatic object at a particular wavelength ``wave``.
 
         Parameters:
             wave:   Wavelength in nanometers.
 
         Returns:
@@ -3488,26 +3556,29 @@
             assert not np.any(use_p1 & use_p2)
             assert not np.any(use_p2 & use_p3)
             assert not np.any(use_p1 & use_p3)
 
             temp1 = PhotonArray(np.sum(use_p1))
             temp2 = PhotonArray(np.sum(use_p2))
             temp3 = PhotonArray(np.sum(use_p3))
+            temp1._copyFrom(photons, slice(None), use_p1, do_xy=False, do_flux=False)
+            temp2._copyFrom(photons, slice(None), use_p2, do_xy=False, do_flux=False)
+            temp3._copyFrom(photons, slice(None), use_p3, do_xy=False, do_flux=False)
             prof1._shoot(temp1, rng)
             prof2._shoot(temp2, rng)
             prof3._shoot(temp3, rng)
-            photons.x[use_p1] = temp1.x * (w[use_p1] / wave1)
-            photons.y[use_p1] = temp1.y * (w[use_p1] / wave1)
-            photons.flux[use_p1] = temp1.flux * (len(temp1)/len(photons))
-            photons.x[use_p2] = temp2.x * (w[use_p2] / wave2)
-            photons.y[use_p2] = temp2.y * (w[use_p2] / wave2)
-            photons.flux[use_p2] = temp2.flux * (len(temp2)/len(photons))
-            photons.x[use_p3] = temp3.x * (w[use_p3] / wave3)
-            photons.y[use_p3] = temp3.y * (w[use_p3] / wave3)
-            photons.flux[use_p3] = temp3.flux * (len(temp3)/len(photons))
+            temp1.scaleXY(w[use_p1]/wave1)
+            temp1.scaleFlux(len(temp1)/len(photons))
+            temp2.scaleXY(w[use_p2]/wave2)
+            temp2.scaleFlux(len(temp2)/len(photons))
+            temp3.scaleXY(w[use_p3]/wave3)
+            temp3.scaleFlux(len(temp3)/len(photons))
+            photons._copyFrom(temp1, use_p1, slice(None))
+            photons._copyFrom(temp2, use_p2, slice(None))
+            photons._copyFrom(temp3, use_p3, slice(None))
 
 
 class ChromaticAiry(ChromaticObject):
     """A subclass of `ChromaticObject` meant to represent chromatic Airy profiles.
 
     For more information about the basics of Airy profiles, please see `galsim.Airy`.
```

### Comparing `GalSim-2.5.0/galsim/config/__init__.py` & `GalSim-2.5.1/galsim/config/__init__.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/config/bandpass.py` & `GalSim-2.5.1/galsim/config/bandpass.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/config/extra.py` & `GalSim-2.5.1/galsim/config/extra.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/config/extra_badpix.py` & `GalSim-2.5.1/galsim/config/extra_badpix.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/config/extra_psf.py` & `GalSim-2.5.1/galsim/config/extra_psf.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/config/extra_truth.py` & `GalSim-2.5.1/galsim/config/extra_truth.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/config/extra_weight.py` & `GalSim-2.5.1/galsim/config/extra_weight.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/config/gsobject.py` & `GalSim-2.5.1/galsim/config/gsobject.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/config/image.py` & `GalSim-2.5.1/galsim/config/image.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/config/image_scattered.py` & `GalSim-2.5.1/galsim/config/image_scattered.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/config/image_tiled.py` & `GalSim-2.5.1/galsim/config/image_tiled.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/config/input.py` & `GalSim-2.5.1/galsim/config/input.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/config/input_cosmos.py` & `GalSim-2.5.1/galsim/config/input_cosmos.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/config/input_fitsheader.py` & `GalSim-2.5.1/galsim/config/input_fitsheader.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/config/input_image.py` & `GalSim-2.5.1/galsim/config/input_image.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/config/input_nfw.py` & `GalSim-2.5.1/galsim/config/input_nfw.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/config/input_powerspectrum.py` & `GalSim-2.5.1/galsim/config/input_powerspectrum.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/config/input_real.py` & `GalSim-2.5.1/galsim/config/input_real.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/config/noise.py` & `GalSim-2.5.1/galsim/config/noise.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/config/output.py` & `GalSim-2.5.1/galsim/config/output.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/config/output_datacube.py` & `GalSim-2.5.1/galsim/config/output_datacube.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/config/output_multifits.py` & `GalSim-2.5.1/galsim/config/output_multifits.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/config/photon_ops.py` & `GalSim-2.5.1/galsim/config/photon_ops.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/config/process.py` & `GalSim-2.5.1/galsim/config/process.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/config/sed.py` & `GalSim-2.5.1/galsim/config/sed.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/config/sensor.py` & `GalSim-2.5.1/galsim/config/sensor.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/config/stamp.py` & `GalSim-2.5.1/galsim/config/stamp.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/config/stamp_ring.py` & `GalSim-2.5.1/galsim/config/stamp_ring.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/config/util.py` & `GalSim-2.5.1/galsim/config/util.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/config/value.py` & `GalSim-2.5.1/galsim/config/value.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/config/value_eval.py` & `GalSim-2.5.1/galsim/config/value_eval.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/config/value_random.py` & `GalSim-2.5.1/galsim/config/value_random.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/config/wcs.py` & `GalSim-2.5.1/galsim/config/wcs.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/convolve.py` & `GalSim-2.5.1/galsim/convolve.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/correlatednoise.py` & `GalSim-2.5.1/galsim/correlatednoise.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/dcr.py` & `GalSim-2.5.1/galsim/dcr.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/deltafunction.py` & `GalSim-2.5.1/galsim/deltafunction.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/deprecated/__init__.py` & `GalSim-2.5.1/galsim/deprecated/__init__.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/deprecated/correlatednoise.py` & `GalSim-2.5.1/galsim/deprecated/correlatednoise.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/deprecated/integ.py` & `GalSim-2.5.1/galsim/deprecated/integ.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/deprecated/randwalk.py` & `GalSim-2.5.1/galsim/deprecated/randwalk.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/des/__init__.py` & `GalSim-2.5.1/galsim/des/__init__.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/des/des_meds.py` & `GalSim-2.5.1/galsim/des/des_meds.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/des/des_psfex.py` & `GalSim-2.5.1/galsim/des/des_psfex.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/des/des_shapelet.py` & `GalSim-2.5.1/galsim/des/des_shapelet.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/detectors.py` & `GalSim-2.5.1/galsim/detectors.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/download_cosmos.py` & `GalSim-2.5.1/galsim/download_cosmos.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/errors.py` & `GalSim-2.5.1/galsim/errors.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/exponential.py` & `GalSim-2.5.1/galsim/exponential.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/fft.py` & `GalSim-2.5.1/galsim/fft.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/fits.py` & `GalSim-2.5.1/galsim/fits.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/fitswcs.py` & `GalSim-2.5.1/galsim/fitswcs.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/fouriersqrt.py` & `GalSim-2.5.1/galsim/fouriersqrt.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/galaxy_sample.py` & `GalSim-2.5.1/galsim/galaxy_sample.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/gaussian.py` & `GalSim-2.5.1/galsim/gaussian.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/gsobject.py` & `GalSim-2.5.1/galsim/gsobject.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/gsparams.py` & `GalSim-2.5.1/galsim/gsparams.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/hsm.py` & `GalSim-2.5.1/galsim/hsm.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/image.py` & `GalSim-2.5.1/galsim/image.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/inclined.py` & `GalSim-2.5.1/galsim/inclined.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/GalSim.h` & `GalSim-2.5.1/galsim/include/GalSim.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/fftw3/fftw3.h` & `GalSim-2.5.1/galsim/include/fftw3/fftw3.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/BinomFact.h` & `GalSim-2.5.1/galsim/include/galsim/BinomFact.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/Bounds.h` & `GalSim-2.5.1/galsim/include/galsim/Bounds.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/CDModel.h` & `GalSim-2.5.1/galsim/include/galsim/CDModel.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/CorrelatedNoise.h` & `GalSim-2.5.1/galsim/include/galsim/CorrelatedNoise.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/GSParams.h` & `GalSim-2.5.1/galsim/include/galsim/GSParams.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/Image.h` & `GalSim-2.5.1/galsim/include/galsim/Image.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/ImageArith.h` & `GalSim-2.5.1/galsim/include/galsim/ImageArith.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/Interpolant.h` & `GalSim-2.5.1/galsim/include/galsim/Interpolant.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/LRUCache.h` & `GalSim-2.5.1/galsim/include/galsim/LRUCache.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/Laguerre.h` & `GalSim-2.5.1/galsim/include/galsim/Laguerre.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/OneDimensionalDeviate.h` & `GalSim-2.5.1/galsim/include/galsim/OneDimensionalDeviate.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/PhotonArray.h` & `GalSim-2.5.1/galsim/include/galsim/PhotonArray.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/Polygon.h` & `GalSim-2.5.1/galsim/include/galsim/Polygon.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/ProbabilityTree.h` & `GalSim-2.5.1/galsim/include/galsim/ProbabilityTree.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/Random.h` & `GalSim-2.5.1/galsim/include/galsim/Random.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/RealGalaxy.h` & `GalSim-2.5.1/galsim/include/galsim/RealGalaxy.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/SBAdd.h` & `GalSim-2.5.1/galsim/include/galsim/SBAdd.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/SBAddImpl.h` & `GalSim-2.5.1/galsim/include/galsim/SBAddImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/SBAiry.h` & `GalSim-2.5.1/galsim/include/galsim/SBAiry.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/SBAiryImpl.h` & `GalSim-2.5.1/galsim/include/galsim/SBAiryImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/SBBox.h` & `GalSim-2.5.1/galsim/include/galsim/SBBox.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/SBBoxImpl.h` & `GalSim-2.5.1/galsim/include/galsim/SBBoxImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/SBConvolve.h` & `GalSim-2.5.1/galsim/include/galsim/SBConvolve.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/SBConvolveImpl.h` & `GalSim-2.5.1/galsim/include/galsim/SBConvolveImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/SBDeconvolve.h` & `GalSim-2.5.1/galsim/include/galsim/SBDeconvolve.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/SBDeconvolveImpl.h` & `GalSim-2.5.1/galsim/include/galsim/SBDeconvolveImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/SBDeltaFunction.h` & `GalSim-2.5.1/galsim/include/galsim/SBDeltaFunction.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/SBDeltaFunctionImpl.h` & `GalSim-2.5.1/galsim/include/galsim/SBDeltaFunctionImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/SBExponential.h` & `GalSim-2.5.1/galsim/include/galsim/SBExponential.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/SBExponentialImpl.h` & `GalSim-2.5.1/galsim/include/galsim/SBExponentialImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/SBFourierSqrt.h` & `GalSim-2.5.1/galsim/include/galsim/SBFourierSqrt.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/SBFourierSqrtImpl.h` & `GalSim-2.5.1/galsim/include/galsim/SBFourierSqrtImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/SBGaussian.h` & `GalSim-2.5.1/galsim/include/galsim/SBGaussian.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/SBGaussianImpl.h` & `GalSim-2.5.1/galsim/include/galsim/SBGaussianImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/SBInclinedExponential.h` & `GalSim-2.5.1/galsim/include/galsim/SBInclinedExponential.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/SBInclinedExponentialImpl.h` & `GalSim-2.5.1/galsim/include/galsim/SBInclinedExponentialImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/SBInclinedSersic.h` & `GalSim-2.5.1/galsim/include/galsim/SBInclinedSersic.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/SBInclinedSersicImpl.h` & `GalSim-2.5.1/galsim/include/galsim/SBInclinedSersicImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/SBInterpolatedImage.h` & `GalSim-2.5.1/galsim/include/galsim/SBInterpolatedImage.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/SBInterpolatedImageImpl.h` & `GalSim-2.5.1/galsim/include/galsim/SBInterpolatedImageImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/SBKolmogorov.h` & `GalSim-2.5.1/galsim/include/galsim/SBKolmogorov.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/SBKolmogorovImpl.h` & `GalSim-2.5.1/galsim/include/galsim/SBKolmogorovImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/SBMoffat.h` & `GalSim-2.5.1/galsim/include/galsim/SBMoffat.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/SBMoffatImpl.h` & `GalSim-2.5.1/galsim/include/galsim/SBMoffatImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/SBProfile.h` & `GalSim-2.5.1/galsim/include/galsim/SBProfile.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/SBProfileImpl.h` & `GalSim-2.5.1/galsim/include/galsim/SBProfileImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/SBSecondKick.h` & `GalSim-2.5.1/galsim/include/galsim/SBSecondKick.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/SBSecondKickImpl.h` & `GalSim-2.5.1/galsim/include/galsim/SBSecondKickImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/SBSersic.h` & `GalSim-2.5.1/galsim/include/galsim/SBSersic.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/SBSersicImpl.h` & `GalSim-2.5.1/galsim/include/galsim/SBSersicImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/SBShapelet.h` & `GalSim-2.5.1/galsim/include/galsim/SBShapelet.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/SBShapeletImpl.h` & `GalSim-2.5.1/galsim/include/galsim/SBShapeletImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/SBSpergel.h` & `GalSim-2.5.1/galsim/include/galsim/SBSpergel.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/SBSpergelImpl.h` & `GalSim-2.5.1/galsim/include/galsim/SBSpergelImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/SBTransform.h` & `GalSim-2.5.1/galsim/include/galsim/SBTransform.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/SBTransformImpl.h` & `GalSim-2.5.1/galsim/include/galsim/SBTransformImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/SBVonKarman.h` & `GalSim-2.5.1/galsim/include/galsim/SBVonKarman.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/SBVonKarmanImpl.h` & `GalSim-2.5.1/galsim/include/galsim/SBVonKarmanImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/Silicon.h` & `GalSim-2.5.1/galsim/include/galsim/Silicon.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/Solve.h` & `GalSim-2.5.1/galsim/include/galsim/Solve.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/Std.h` & `GalSim-2.5.1/galsim/include/galsim/Std.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/Stopwatch.h` & `GalSim-2.5.1/galsim/include/galsim/Stopwatch.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/Table.h` & `GalSim-2.5.1/galsim/include/galsim/Table.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/Version.h` & `GalSim-2.5.1/galsim/include/galsim/Version.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 // This file is auto-generated by setup.py.  Do not edit.
 #define GALSIM_MAJOR 2
 #define GALSIM_MINOR 5
-#define GALSIM_REVISION 0
+#define GALSIM_REVISION 1
 
 #include <string>
 #include <sstream>
 
 #if defined(__GNUC__)
 #define PUBLIC_API __attribute__ ((visibility ("default")))
 #else
```

### Comparing `GalSim-2.5.0/galsim/include/galsim/WCS.h` & `GalSim-2.5.1/galsim/include/galsim/WCS.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/boost1_48_0/LICENSE_1_0.txt` & `GalSim-2.5.1/galsim/include/galsim/boost1_48_0/LICENSE_1_0.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/boost1_48_0/README` & `GalSim-2.5.1/galsim/include/galsim/boost1_48_0/README`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/boost1_48_0/assert.hpp` & `GalSim-2.5.1/galsim/include/galsim/boost1_48_0/assert.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/boost1_48_0/config/suffix.hpp` & `GalSim-2.5.1/galsim/include/galsim/boost1_48_0/config/suffix.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/boost1_48_0/current_function.hpp` & `GalSim-2.5.1/galsim/include/galsim/boost1_48_0/current_function.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/boost1_48_0/random/binomial_distribution.hpp` & `GalSim-2.5.1/galsim/include/galsim/boost1_48_0/random/binomial_distribution.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/boost1_48_0/random/chi_squared_distribution.hpp` & `GalSim-2.5.1/galsim/include/galsim/boost1_48_0/random/chi_squared_distribution.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/boost1_48_0/random/detail/generator_seed_seq.hpp` & `GalSim-2.5.1/galsim/include/galsim/boost1_48_0/random/detail/generator_seed_seq.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/boost1_48_0/random/detail/ptr_helper.hpp` & `GalSim-2.5.1/galsim/include/galsim/boost1_48_0/random/detail/ptr_helper.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/boost1_48_0/random/detail/seed.hpp` & `GalSim-2.5.1/galsim/include/galsim/boost1_48_0/random/detail/seed.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/boost1_48_0/random/detail/signed_unsigned_tools.hpp` & `GalSim-2.5.1/galsim/include/galsim/boost1_48_0/random/detail/signed_unsigned_tools.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/boost1_48_0/random/exponential_distribution.hpp` & `GalSim-2.5.1/galsim/include/galsim/boost1_48_0/random/exponential_distribution.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/boost1_48_0/random/gamma_distribution.hpp` & `GalSim-2.5.1/galsim/include/galsim/boost1_48_0/random/gamma_distribution.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/boost1_48_0/random/mersenne_twister.hpp` & `GalSim-2.5.1/galsim/include/galsim/boost1_48_0/random/mersenne_twister.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/boost1_48_0/random/normal_distribution.hpp` & `GalSim-2.5.1/galsim/include/galsim/boost1_48_0/random/normal_distribution.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/boost1_48_0/random/poisson_distribution.hpp` & `GalSim-2.5.1/galsim/include/galsim/boost1_48_0/random/poisson_distribution.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/boost1_48_0/random/uniform_01.hpp` & `GalSim-2.5.1/galsim/include/galsim/boost1_48_0/random/uniform_01.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/boost1_48_0/random/uniform_real_distribution.hpp` & `GalSim-2.5.1/galsim/include/galsim/boost1_48_0/random/uniform_real_distribution.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/boost1_48_0/random/weibull_distribution.hpp` & `GalSim-2.5.1/galsim/include/galsim/boost1_48_0/random/weibull_distribution.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/fmath/Makefile` & `GalSim-2.5.1/galsim/include/galsim/fmath/Makefile`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/fmath/avx2.cpp` & `GalSim-2.5.1/galsim/include/galsim/fmath/avx2.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/fmath/bench.cpp` & `GalSim-2.5.1/galsim/include/galsim/fmath/bench.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/fmath/bench.sln` & `GalSim-2.5.1/galsim/include/galsim/fmath/bench.sln`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/fmath/bench.vcproj` & `GalSim-2.5.1/galsim/include/galsim/fmath/bench.vcproj`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/fmath/ck.cpp` & `GalSim-2.5.1/galsim/include/galsim/fmath/ck.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/fmath/fastexp.cpp` & `GalSim-2.5.1/galsim/include/galsim/fmath/fastexp.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/fmath/fmath.hpp` & `GalSim-2.5.1/galsim/include/galsim/fmath/fmath.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/fmath/include/cybozu/benchmark.hpp` & `GalSim-2.5.1/galsim/include/galsim/fmath/include/cybozu/benchmark.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/fmath/include/cybozu/inttype.hpp` & `GalSim-2.5.1/galsim/include/galsim/fmath/include/cybozu/inttype.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/fmath/readme.md` & `GalSim-2.5.1/galsim/include/galsim/fmath/readme.md`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/fmath/readme.txt` & `GalSim-2.5.1/galsim/include/galsim/fmath/readme.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/hsm/PSFCorr.h` & `GalSim-2.5.1/galsim/include/galsim/hsm/PSFCorr.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/integ/Int.h` & `GalSim-2.5.1/galsim/include/galsim/integ/Int.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/integ/IntGKPData1.h` & `GalSim-2.5.1/galsim/include/galsim/integ/IntGKPData1.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/integ/IntGKPData10.h` & `GalSim-2.5.1/galsim/include/galsim/integ/IntGKPData10.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/integ/MoreFunctional.h` & `GalSim-2.5.1/galsim/include/galsim/integ/MoreFunctional.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/math/Angle.h` & `GalSim-2.5.1/galsim/include/galsim/math/Angle.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/math/Bessel.h` & `GalSim-2.5.1/galsim/include/galsim/math/Bessel.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/math/Gamma.h` & `GalSim-2.5.1/galsim/include/galsim/math/Gamma.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/math/Hankel.h` & `GalSim-2.5.1/galsim/include/galsim/math/Hankel.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/math/Horner.h` & `GalSim-2.5.1/galsim/include/galsim/math/Horner.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/math/Nan.h` & `GalSim-2.5.1/galsim/include/galsim/math/Nan.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/math/Sinc.h` & `GalSim-2.5.1/galsim/include/galsim/math/Sinc.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/include/galsim/mmgr.h` & `GalSim-2.5.1/galsim/include/galsim/mmgr.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/integ.py` & `GalSim-2.5.1/galsim/integ.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/interpolant.py` & `GalSim-2.5.1/galsim/interpolant.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/interpolatedimage.py` & `GalSim-2.5.1/galsim/interpolatedimage.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/knots.py` & `GalSim-2.5.1/galsim/knots.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/kolmogorov.py` & `GalSim-2.5.1/galsim/kolmogorov.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/lensing_ps.py` & `GalSim-2.5.1/galsim/lensing_ps.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/main.py` & `GalSim-2.5.1/galsim/main.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/meta_data.py` & `GalSim-2.5.1/galsim/meta_data.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/moffat.py` & `GalSim-2.5.1/galsim/moffat.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/nfw_halo.py` & `GalSim-2.5.1/galsim/nfw_halo.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/noise.py` & `GalSim-2.5.1/galsim/noise.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/phase_psf.py` & `GalSim-2.5.1/galsim/phase_psf.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/phase_screens.py` & `GalSim-2.5.1/galsim/phase_screens.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 # From https://stackoverflow.com/questions/71282555/acquire-a-multiprocessing-lock-in-a-with-statement-if-non-blocking-or-with-timeo
 @contextmanager
 def acquire_lock(lock, block=True, timeout=None):
     held = lock.acquire(block=block, timeout=timeout)
     try:
         yield held
     finally:
-        if held:
+        if held:  # pragma: no branch
             lock.release()
 
 
 class AtmosphericScreen:
     """ An atmospheric phase screen that can drift in the wind and evolves ("boils") over time.  The
     initial phases and fractional phase updates are drawn from a von Karman power spectrum, which is
     defined by a Fried parameter that effectively sets the amplitude of the turbulence, and an outer
```

### Comparing `GalSim-2.5.0/galsim/photon_array.py` & `GalSim-2.5.1/galsim/photon_array.py`

 * *Files 4% similar despite different names*

```diff
@@ -201,15 +201,21 @@
         ret._flux = flux
         ret._dxdz = dxdz
         ret._dydz = dydz
         ret._wave = wavelength
         ret._pupil_u = pupil_u
         ret._pupil_v = pupil_v
         ret._time = time
-        ret._is_corr = is_corr
+        ret._is_corr = False
+        if is_corr:
+            from .deprecated import depr
+            depr('is_corr=True', 2.5, '',
+                "We don't think this is necessary anymore.  If you have a use case that "
+                "requires it, please open an issue.")
+            ret._is_corr = is_corr
         return ret
 
     def size(self):
         """Return the size of the photon array.  Equivalent to ``len(self)``.
         """
         return len(self._x)
 
@@ -396,19 +402,27 @@
         """
         if self._time is None:
             self._time = np.zeros_like(self._x)
 
     def isCorrelated(self):
         """Returns whether the photons are correlated
         """
+        from .deprecated import depr
+        depr('isCorrelated', 2.5, '',
+                "We don't think this is necessary anymore.  If you have a use case that "
+                "requires it, please open an issue.")
         return self._is_corr
 
     def setCorrelated(self, is_corr=True):
         """Set whether the photons are correlated
         """
+        from .deprecated import depr
+        depr('setCorrelated', 2.5, '',
+                "We don't think this is necessary anymore.  If you have a use case that "
+                "requires it, please open an issue.")
         self._is_corr = is_corr
         self.__dict__.pop('_pa', None)
 
     def getTotalFlux(self):
         """Return the total flux of all the photons.
         """
         return self.flux.sum()
@@ -436,36 +450,99 @@
             scale:      The factor by which to scale the positions.
         """
         self._x *= scale
         self._y *= scale
 
     def assignAt(self, istart, rhs):
         """Assign the contents of another `PhotonArray` to this one starting at istart.
+
+        Parameters:
+            istart:     The first index at which to insert new values.
+            rhs:        The other `PhotonArray` from which to get the values.
         """
+        from .deprecated import depr
+        depr("PhotonArray.assignAt", 2.5, "copyFrom(rhs, slice(istart, istart+rhs.size()))")
         if istart + rhs.size() > self.size():
             raise GalSimValueError(
                 "The given rhs does not fit into this array starting at %d"%istart, rhs)
         s = slice(istart, istart + rhs.size())
-        self.x[s] = rhs.x
-        self.y[s] = rhs.y
-        self.flux[s] = rhs.flux
-        if rhs.hasAllocatedAngles():
+        self._copyFrom(rhs, s, slice(None))
+
+    def copyFrom(self, rhs, target_indices=slice(None), source_indices=slice(None),
+                 do_xy=True, do_flux=True, do_other=True):
+        """Copy some contents of another `PhotonArray` to some elements of this one.
+
+        Specifically each element of rhs[source_indices] is mapped to self[target_indices].
+        The values s1 and s2 may be slices, list of indices, or anything else that is a valid
+        key for a numpy array.
+
+        Parameters:
+            rhs:            The `PhotonArray` from which to get values.
+            target_indices: The indices at which to assign values in the current PhotonArray (self).
+                            [default: slice(None)]
+            source_indices: The indices from which to get values from the PhotonArray, ``rhs``.
+                            [default: slice(None)]
+            do_xy:          Whether to include copying the x and y arrays. [default: True]
+            do_flux:        Whether to include copying the flux array. [default: True]
+            do_other:       Whether to include copying the other arrays (angles, wavelength,
+                            pupil positions, time). [default: True]
+        """
+        try:
+            a1 = self.flux[target_indices]
+            # Numpy is flexible about allowing slices outside the range of the array.
+            # Rather than try to check all possible ways the indices can be invalid, we
+            # just make sure that at least some elements come back from the numpy call.
+            n1 = len(np.atleast_1d(a1))
+            assert n1 > 0
+        except (IndexError, AssertionError):
+            raise GalSimValueError("target_indices is invalid for the target PhotonArray",
+                                   target_indices)
+        try:
+            a2 = rhs.flux[source_indices]
+            n2 = len(np.atleast_1d(a2))
+            assert n2 > 0
+        except (IndexError, AssertionError) as e:
+            raise GalSimValueError("source_indices is invalid for the source PhotonArray",
+                                   source_indices)
+        if n1 != n2:
+            raise GalSimIncompatibleValuesError(
+                "target_indices and source_indices do not reference the same number of elements"
+                "in their respective PhotonArrays ({} and {} respectively)".format(n1, n2),
+                dict(target_indices=target_indices, source_indices=source_indices))
+
+        self._copyFrom(rhs, target_indices, source_indices, do_xy, do_flux, do_other)
+
+    def _copyFrom(self, rhs, target_indices, source_indices, do_xy=True, do_flux=True,
+                  do_other=True):
+        """Equivalent to self.copyFrom(rhs, target_indices, source_indices), but without any
+        checks that the indices are valid.
+        """
+        # Aliases for notational convenience.
+        s1 = target_indices
+        s2 = source_indices
+
+        if do_xy:
+            self.x[s1] = rhs.x[s2]
+            self.y[s1] = rhs.y[s2]
+        if do_flux:
+            self.flux[s1] = rhs.flux[s2]
+        if do_other and rhs.hasAllocatedAngles():
             self.allocateAngles()
-            self.dxdz[s] = rhs.dxdz
-            self.dydz[s] = rhs.dydz
-        if rhs.hasAllocatedWavelengths():
+            self.dxdz[s1] = rhs.dxdz[s2]
+            self.dydz[s1] = rhs.dydz[s2]
+        if do_other and rhs.hasAllocatedWavelengths():
             self.allocateWavelengths()
-            self.wavelength[s] = rhs.wavelength
-        if rhs.hasAllocatedPupil():
+            self.wavelength[s1] = rhs.wavelength[s2]
+        if do_other and rhs.hasAllocatedPupil():
             self.allocatePupil()
-            self.pupil_u[s] = rhs.pupil_u
-            self.pupil_v[s] = rhs.pupil_v
-        if rhs.hasAllocatedTimes():
+            self.pupil_u[s1] = rhs.pupil_u[s2]
+            self.pupil_v[s1] = rhs.pupil_v[s2]
+        if do_other and rhs.hasAllocatedTimes():
             self.allocateTimes()
-            self.time[s] = rhs.time
+            self.time[s1] = rhs.time[s2]
 
     def convolve(self, rhs, rng=None):
         """Convolve this `PhotonArray` with another.
 
         ..note::
 
             If both self and rhs have wavelengths, angles, pupil coordinates or times assigned,
```

### Comparing `GalSim-2.5.0/galsim/position.py` & `GalSim-2.5.1/galsim/position.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/pse.py` & `GalSim-2.5.1/galsim/pse.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/random.py` & `GalSim-2.5.1/galsim/random.py`

 * *Files 1% similar despite different names*

```diff
@@ -765,17 +765,19 @@
                         passed in any other case) [default: None]
         interpolant:    Type of interpolation used for interpolating a file (causes an error if
                         passed alongside a callable function).  Options are given in the
                         documentation for `LookupTable`. [default: 'linear']
         npoints:        Number of points DistDeviate should create for its internal interpolation
                         tables. [default: 256, unless the function is a non-log `LookupTable`, in
                         which case it uses the table's x values]
+        clip_neg:       Clip any negative input values to zero. [default: False; an error will
+                        be raised if any negative probabilities are found.]
     """
     def __init__(self, seed=None, function=None, x_min=None,
-                 x_max=None, interpolant=None, npoints=None):
+                 x_max=None, interpolant=None, npoints=None, clip_neg=False):
 
         # Set up the PRNG
         self._rng_type = _galsim.UniformDeviateImpl
         self._rng_args = ()
         self.reset(seed)
 
         # Basic input checking and setups
@@ -819,15 +821,15 @@
             if not hasattr(function, '__call__'):
                 raise TypeError('function must be a callable function or a string')
             if interpolant:
                 raise GalSimIncompatibleValuesError(
                     "Cannot provide an interpolant with a callable function argument",
                     interpolant=interpolant, function=function)
             if isinstance(function, LookupTable):
-                if x_min or x_max:
+                if (x_min not in (None, function.x_min)) or (x_max not in (None, function.x_max)):
                     raise GalSimIncompatibleValuesError(
                         "Cannot provide x_min or x_max with a LookupTable function",
                         function=function, x_min=x_min, x_max=x_max)
                 x_min = function.x_min
                 x_max = function.x_max
             else:
                 if x_min is None or x_max is None:
@@ -855,15 +857,19 @@
             xarray = x_min+(1.*x_max-x_min)/(npoints-1)*np.array(range(npoints),float)
             # Integrate over the range of x in case the function is doing something weird here.
             pdf = [0.] + [integ.int1d(function, xarray[i], xarray[i+1])
                           for i in range(npoints - 1)]
             pdf = np.array(pdf)
 
         # Check that the probability is nonnegative
-        if not np.all(pdf >= 0.):
+        if clip_neg:
+            # Write it this way so nan -> 0 as well as negative values.
+            w = np.where(~(pdf >= 0))
+            pdf[w] = 0.
+        elif not np.all(pdf >= 0.):
             raise GalSimValueError('Negative probability found in DistDeviate.',function)
 
         # Compute the cumulative distribution function = int(pdf(x),x)
         cdf = np.cumsum(pdf)
 
         # Quietly renormalize the probability if it wasn't already normalized
         totalprobability = cdf[-1]
```

### Comparing `GalSim-2.5.0/galsim/real.py` & `GalSim-2.5.1/galsim/real.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from multiprocessing import Lock
 
 from . import _galsim
 from .gsobject import GSObject
 from .gsparams import GSParams
 from .position import PositionD
 from .bounds import BoundsI
-from .utilities import lazy_property, doc_inherit, convert_interpolant
+from .utilities import lazy_property, doc_inherit, convert_interpolant, merge_sorted
 from .interpolant import Quintic
 from .interpolatedimage import InterpolatedImage, _InterpolatedKImage
 from .convolve import Convolve, Deconvolve
 from .image import Image, ImageCD
 from .correlatednoise import UncorrelatedNoise, BaseCorrelatedNoise, CovarianceSpectrum
 from .errors import GalSimError, GalSimValueError, GalSimIncompatibleValuesError
 from .errors import GalSimIndexError
@@ -1287,15 +1287,15 @@
         ChromaticSum.__init__(self, obj_list)
 
     @staticmethod
     def _poly_SEDs(bands):
         # Use polynomial SEDs by default; up to the number of bands provided.
         waves = []
         for bp in bands:
-            waves = np.union1d(waves, bp.wave_list)
+            waves = merge_sorted([waves, bp.wave_list])
         SEDs = []
         for i in range(len(bands)):
             SEDs.append(
                     SED(LookupTable(waves, waves**i, interpolant='linear'), 'nm', 'fphotons')
                     .withFlux(1.0, bands[0]))
         return SEDs
```

### Comparing `GalSim-2.5.0/galsim/roman/__init__.py` & `GalSim-2.5.1/galsim/roman/__init__.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/roman/roman_backgrounds.py` & `GalSim-2.5.1/galsim/roman/roman_backgrounds.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/roman/roman_bandpass.py` & `GalSim-2.5.1/galsim/roman/roman_bandpass.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/roman/roman_config.py` & `GalSim-2.5.1/galsim/roman/roman_config.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/roman/roman_detectors.py` & `GalSim-2.5.1/galsim/roman/roman_detectors.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/roman/roman_psfs.py` & `GalSim-2.5.1/galsim/roman/roman_psfs.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/roman/roman_wcs.py` & `GalSim-2.5.1/galsim/roman/roman_wcs.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/second_kick.py` & `GalSim-2.5.1/galsim/second_kick.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/sed.py` & `GalSim-2.5.1/galsim/sed.py`

 * *Files 3% similar despite different names*

```diff
@@ -105,59 +105,44 @@
     interpolation should take place in the native units of the input ``spec``, and subsequently flux
     density converted to photons/cm^2/s/nm afterwards.  Generally, the former option is faster, but
     may be less accurate since interpolation and dimensionality conversion do not commute.  One
     consequence of using ``fast=True`` is that __call__ can not accept an ``astropy.units.Quantity``
     in this case.
 
     Parameters:
-        spec:        Function defining the z=0 spectrum at each wavelength.  See above for
-                     valid options for this parameter.
-        wave_type:   String or astropy.unit specifying units for wavelength input to ``spec``.
-        flux_type:   String or astropy.unit specifying what type of spectral density or
-                     dimensionless normalization ``spec`` represents.  See above for valid options
-                     for this parameter.
-        redshift:    Optionally shift the spectrum to the given redshift. [default: 0]
-        fast:        Convert units on initialization instead of on __call__. [default: True]
+        spec:           Function defining the z=0 spectrum at each wavelength.  See above for
+                        valid options for this parameter.
+        wave_type:      String or astropy.unit specifying units for wavelength input to ``spec``.
+        flux_type:      String or astropy.unit specifying what type of spectral density or
+                        dimensionless normalization ``spec`` represents.  See above for valid
+                        options for this parameter.
+        redshift:       Optionally shift the spectrum to the given redshift. [default: 0]
+        fast:           Convert units on initialization instead of on __call__. [default: True]
+        interpolant:    If reading from a file, what interpolant to use. [default: 'linear']
     """
     # We'll use these multiple times below, and they are ridiculously slow to construct,
     # so just make them once at the class level.
     _fphotons_base = units.astrophys.photon/(units.s * units.cm**2)
     _flambda_base = units.erg/(units.s * units.cm**2)
     _fphotons = _fphotons_base / units.nm
     _flambda = _flambda_base / units.nm
     _fnu = units.erg / (units.s * units.Hz * units.cm**2)
     _spec_nm = units.spectral_density(1*units.nm)
     _c = constants.c.to('nm/s').value
     _h = constants.h.to('erg s').value
     _dimensionless = units.dimensionless_unscaled
+    _bolo_max_wave = 1.e30  # What we use as "infinity" for bolometric flux calculations.
 
-    def __init__(self, spec, wave_type, flux_type, redshift=0., fast=True,
+    def __init__(self, spec, wave_type, flux_type, redshift=0., fast=True, interpolant='linear',
                  _blue_limit=0.0, _red_limit=np.inf, _wave_list=None):
         self._flux_type = flux_type  # Need to save the original for repr
+        self.interpolant = interpolant
+
         # Parse the various options for wave_type
-        if isinstance(wave_type, str):
-            if wave_type.lower() in ('nm', 'nanometer', 'nanometers'):
-                self.wave_type = 'nm'
-                self.wave_factor = 1.
-            elif wave_type.lower() in ('a', 'ang', 'angstrom', 'angstroms'):
-                self.wave_type = 'Angstrom'
-                self.wave_factor = 10.
-            else:
-                raise GalSimValueError("Unknown wave_type", wave_type, ('nm', 'Angstrom'))
-        else:
-            self.wave_type = wave_type
-            try:
-                self.wave_factor = (1*units.nm).to(self.wave_type).value
-                if self.wave_factor == 1.:
-                    self.wave_type = 'nm'
-                elif abs(self.wave_factor-10.) < 2.e-15:  # This doesn't come out exactly 10.
-                    self.wave_type = 'Angstrom'
-                    self.wave_factor = 10.
-            except units.UnitConversionError:
-                self.wave_factor = None
+        self.wave_type, self.wave_factor = self._parse_wave_type(wave_type)
 
         # Parse the various options for flux_type
         self.flux_factor = None
         if isinstance(flux_type, str):
             if flux_type.lower() == 'flambda':
                 self.flux_type = 'flambda'
                 self.spectral = True
@@ -231,14 +216,37 @@
             self.blue_limit = 0.0
             self.red_limit = np.inf
             self.wave_list = np.array([], dtype=float)
 
         # Define the appropriate functions to call
         self._setup_funcs()
 
+    @staticmethod
+    def _parse_wave_type(wave_type):
+        # Parse the various options for wave_type.
+        # Returns wave_type, wave_factor
+        if isinstance(wave_type, str):
+            if wave_type.lower() in ('nm', 'nanometer', 'nanometers'):
+                return 'nm', 1.
+            elif wave_type.lower() in ('a', 'ang', 'angstrom', 'angstroms'):
+                return 'Angstrom', 10.
+            else:
+                raise GalSimValueError("Unknown wave_type", wave_type, ('nm', 'Angstrom'))
+        else:
+            try:
+                wave_factor = (1*units.nm).to(wave_type).value
+                if wave_factor == 1.:
+                    return 'nm', 1.
+                elif abs(wave_factor-10.) < 2.e-15:  # This doesn't come out exactly 10.
+                    return 'Angstrom', 10.
+                else:
+                    return units.Unit(wave_type), wave_factor
+            except units.UnitConversionError:
+                return units.Unit(wave_type), None
+
     def _setup_funcs(self):
         # Set up the various functions we use to do the right calculation based on which
         # wave type and/or flux type we have for _spec.
         # The astropy unit functions are horribly slow, so we want to avoid them as much as
         # possible.  If the wave_type and flux_type are one of the simpler (and most common)
         # types, then we have custom functions that do the necessary conversions directly.
         if self.wave_factor == 1:
@@ -312,15 +320,15 @@
             if not self.dimensionless:
                 raise GalSimSEDError("Attempt to set spectral SED using float or integer.", self)
             self._const = True
             self._spec = lambda w: float(self._orig_spec)
         elif isinstance(self._orig_spec, basestring):
             isfile, filename = utilities.check_share_file(self._orig_spec, 'SEDs')
             if isfile:
-                self._spec = LookupTable.from_file(filename, interpolant='linear')
+                self._spec = LookupTable.from_file(filename, interpolant=self.interpolant)
             else:
                 # If a constant function is input as a string (e.g. '1'), then we want to
                 # make sure it is flagged as a const SED.
                 try:
                     float(self._orig_spec)
                 except ValueError:
                     pass
@@ -409,15 +417,16 @@
                     return WeakMethod(self._rest_nm_to_dimensionless)
             else:
                 x = self.wave_list / (1.0 + self.redshift)
                 if self.spectral:
                     f = self._rest_nm_to_photons(x)
                 else:
                     f = self._rest_nm_to_dimensionless(x)
-                return _LookupTable(x, f, interpolant='linear')
+                interp = self._spec.interpolant if isinstance(self._spec, LookupTable) else 'linear'
+                return _LookupTable(x, f, interpolant=interp)
 
     def _call_fast(self, wave):
         """Return either flux in photons / sec / cm^2 / nm, or dimensionless normalization.
 
         Assumes that self._spec has already been transformed to accept correct wavelength units and
         yield correct flux units.
 
@@ -488,50 +497,69 @@
         # should always give us the right net redshift to use.
         redshift = self.redshift + other.redshift
 
         fast = self.fast and other.fast
 
         wave_list, blue_limit, red_limit = utilities.combine_wave_list(self, other)
         if fast:
-            zfactor1 = (1.+redshift) / (1.+self.redshift)
-            zfactor2 = (1.+redshift) / (1.+other.redshift)
-            spec = lambda w: self._fast_spec(w * zfactor1) * other._fast_spec(w * zfactor2)
+            if (isinstance(self._fast_spec, LookupTable)
+                    and not self._fast_spec.x_log
+                    and not self._fast_spec.f_log):
+                x = wave_list / (1.0 + self.redshift)
+                # Add in 500 uniformly spaced values to help improve accuracy.
+                x = utilities.merge_sorted([x, np.linspace(x[0], x[-1], 500)])
+                zfactor2 = (1.+redshift) / (1.+other.redshift)
+                f = self._fast_spec(x) * other._fast_spec(x*zfactor2)
+                spec = _LookupTable(x, f, self._fast_spec.interpolant)
+            elif (isinstance(other._fast_spec, LookupTable)
+                    and not other._fast_spec.x_log
+                    and not other._fast_spec.f_log):
+                x = wave_list / (1.0 + other.redshift)
+                x = utilities.merge_sorted([x, np.linspace(x[0], x[-1], 500)])
+                zfactor1 = (1.+redshift) / (1.+other.redshift)
+                f = self._fast_spec(x*zfactor1) * other._fast_spec(x)
+                spec = _LookupTable(x, f, other._fast_spec.interpolant)
+            else:
+                zfactor1 = (1.+redshift) / (1.+self.redshift)
+                zfactor2 = (1.+redshift) / (1.+other.redshift)
+                spec = lambda w: self._fast_spec(w * zfactor1) * other._fast_spec(w * zfactor2)
         else:
             spec = lambda w: self(w * (1.+redshift)) * other(w * (1.+redshift))
         spectral = self.spectral or other.spectral
         flux_type = 'fphotons' if spectral else '1'
         return SED(spec, 'nm', flux_type, redshift=redshift, fast=fast,
                    _blue_limit=blue_limit, _red_limit=red_limit, _wave_list=wave_list)
 
     def _mul_bandpass(self, other):
         """Equivalent to self * other when other is a Bandpass"""
         wave_list, blue_limit, red_limit = utilities.combine_wave_list(self, other)
         zfactor = (1.0+self.redshift) / other.wave_factor
         if self.fast:
             if (isinstance(self._fast_spec, LookupTable)
-                and not self._fast_spec.x_log
-                and not self._fast_spec.f_log
-                and self._fast_spec.interpolant == 'linear'):
+                    and not self._fast_spec.x_log
+                    and not self._fast_spec.f_log):
                 x = wave_list / (1.0 + self.redshift)
+                # Add in 500 uniformly spaced values to help improve accuracy.
+                x = utilities.merge_sorted([x, np.linspace(x[0], x[-1], 500)])
                 f = self._fast_spec(x) * other._tp(x*zfactor)
-                spec = _LookupTable(x, f, 'linear')
+                spec = _LookupTable(x, f, self._fast_spec.interpolant)
             else:
                 spec = lambda w: self._fast_spec(w) * other._tp(w*zfactor)
         else:
             spec = lambda w: self(w*(1.0+self.redshift)) * other._tp(w*zfactor)
         return SED(spec, 'nm', 'fphotons', redshift=self.redshift, fast=self.fast,
                    _blue_limit=blue_limit, _red_limit=red_limit, _wave_list=wave_list)
 
 
     def _mul_scalar(self, other, spectral):
         """Equivalent to self * other when other is a scalar"""
         # If other is a scalar and self._spec a LookupTable, then remake that LookupTable.
         if isinstance(self._spec, LookupTable):
             wave_type = self.wave_type
-            flux_type = self.flux_type
+            flux_type = self._flux_type
             x = self._spec.getArgs()
             f = np.array(self._spec.getVals()) * other
             spec = _LookupTable(x, f, x_log=self._spec.x_log, f_log=self._spec.f_log,
                                 interpolant=self._spec.interpolant)
         elif self._const and not spectral:
             spec = self._spec(42.0) * other
             wave_type = 'nm'
@@ -671,14 +699,16 @@
                 and not other._fast_spec.x_log
                 and not self._fast_spec.f_log
                 and not other._fast_spec.f_log
                 and self._fast_spec.interpolant == 'linear'
                 and other._fast_spec.interpolant == 'linear'):
             x = wave_list / (1.0 + self.redshift)
             f = self._fast_spec(x) + other._fast_spec(x)
+            # Note: adding splines doesn't quite work at full precision, so only do this for
+            # linear interpolants.
             spec = _LookupTable(x, f, interpolant='linear')
         else:
             spec = lambda w: self(w*(1.0+self.redshift)) + other(w*(1.0+self.redshift))
 
         return SED(spec, wave_type='nm', flux_type=flux_type,
                    redshift=self.redshift, fast=self.fast, _wave_list=wave_list,
                    _blue_limit=blue_limit, _red_limit=red_limit)
@@ -786,15 +816,15 @@
 
         Returns:
             the flux through the bandpass.
         """
         if self.dimensionless:
             raise GalSimSEDError("Cannot calculate flux of dimensionless SED.", self)
         if bandpass is None: # compute bolometric flux
-            bandpass = Bandpass(lambda w: 1., 'nm', blue_limit=0., red_limit=1e100)
+            bandpass = Bandpass(lambda w: 1., 'nm', blue_limit=0., red_limit=SED._bolo_max_wave)
         if len(bandpass.wave_list) > 0 or len(self.wave_list) > 0:
             slop = 1e-6 # nm
             if (self.blue_limit > bandpass.blue_limit + slop
                     or self.red_limit < bandpass.red_limit - slop):
                 raise GalSimRangeError("Bandpass is not completely within defined wavelength "
                                        "range for this SED.",
                                        (bandpass.blue_limit, bandpass.red_limit),
@@ -809,16 +839,18 @@
                 return self._fast_spec.integrate_product(bandpass._tp, wmin, wmax, wf) * ff
             else:
                 w, _, _ = utilities.combine_wave_list(self, bandpass)
                 if not self.fast and self.flux_type != 'fphotons':
                     # When not fast, the SED definition is not linear between the wave_list
                     # points, so this can be slightly inaccurate if the waves are too far apart.
                     # Add in 100 uniformly spaced points to achieve relative accurace ~few e-6.
-                    w = np.union1d(w, np.linspace(w[0], w[-1], 100))
-                return _LookupTable(w,bandpass(w),'linear').integrate_product(self)
+                    w = utilities.merge_sorted([w, np.linspace(w[0], w[-1], 100)])
+                interpolant = (bandpass._tp.interpolant if hasattr(bandpass._tp, 'interpolant')
+                                else 'linear')
+                return _LookupTable(w, bandpass(w), interpolant).integrate_product(self)
         else:
             return integ.int1d(lambda w: bandpass(w)*self(w),
                                bandpass.blue_limit, bandpass.red_limit)
 
     def calculateMagnitude(self, bandpass):
         """Return the `SED` magnitude through a `Bandpass` ``bandpass``.
 
@@ -873,19 +905,22 @@
             the thinned `SED`.
         """
         if len(self.wave_list) > 0:
             rest_wave_native = self._get_rest_native_waves(self.wave_list)
             spec_native = self._spec(rest_wave_native)
 
             # Note that this is thinning in native units, not nm and photons/nm.
+            interpolant = (self.interpolant if not isinstance(self._spec, LookupTable)
+                           else self._spec.interpolant)
             newx, newf = utilities.thin_tabulated_values(
                     rest_wave_native, spec_native, rel_err=rel_err,
-                    trim_zeros=trim_zeros, preserve_range=preserve_range, fast_search=fast_search)
+                    trim_zeros=trim_zeros, preserve_range=preserve_range,
+                    fast_search=fast_search, interpolant=interpolant)
 
-            newspec = _LookupTable(newx, newf, interpolant='linear')
+            newspec = _LookupTable(newx, newf, interpolant=interpolant)
             return SED(newspec, self.wave_type, self.flux_type, redshift=self.redshift,
                        fast=self.fast)
         else:
             return self
 
     def calculateDCRMomentShifts(self, bandpass, **kwargs):
         """Calculates shifts in first and second moments of PSF due to differential chromatic
@@ -928,15 +963,17 @@
                 raise (TypeError("Got unexpected keyword in calculateDCRMomentShifts: {0}"
                                  .format(kw)))
 
         # Now actually start calculating things.
         flux = self.calculateFlux(bandpass)
         if len(self.wave_list) > 0 or len(bandpass.wave_list) > 0:
             w, _, _ = utilities.combine_wave_list(self, bandpass)
-            bp = _LookupTable(w,bandpass(w),'linear')
+            interpolant = (bandpass._tp.interpolant if hasattr(bandpass._tp, 'interpolant')
+                            else 'linear')
+            bp = _LookupTable(w, bandpass(w), interpolant)
             R = lambda w: dcr.get_refraction(w, zenith_angle, **kwargs)
             Rbar = bp.integrate_product(lambda w: self(w) * R(w)) / flux
             V = bp.integrate_product(lambda w: self(w) * (R(w)-Rbar)**2) / flux
         else:
             weight = lambda w: bandpass(w) * self(w)
             Rbar_kernel = lambda w: dcr.get_refraction(w, zenith_angle, **kwargs)
             Rbar = integ.int1d(lambda w: weight(w) * Rbar_kernel(w),
@@ -975,16 +1012,18 @@
             # With three things multiplied together, we can't rely on integrate_product
             # being completely accurate if the waves are spaced too far apart, especially with
             # a power law being one of the factors.
             # So make sure to include a uniform density of points along with the native sed and
             # bandpass points. The error goes like dx**3, so 100 points should give relative
             # errors of order ~few e-6.
             w, _, _ = utilities.combine_wave_list([self, bandpass])
-            w = np.union1d(w, np.linspace(w[0], w[-1], 100))
-            bp = _LookupTable(w,bandpass(w),'linear')
+            w = utilities.merge_sorted([w, np.linspace(w[0], w[-1], 100)])
+            interpolant = (bandpass._tp.interpolant if hasattr(bandpass._tp, 'interpolant')
+                            else 'linear')
+            bp = _LookupTable(w, bandpass(w), interpolant)
             return bp.integrate_product(lambda w: self(w) * (w/base_wavelength)**(2*alpha)) / flux
         else:
             weight = lambda w: bandpass(w) * self(w)
             kernel = lambda w: (w/base_wavelength)**(2*alpha)
             return integ.int1d(lambda w: weight(w) * kernel(w),
                                bandpass.blue_limit, bandpass.red_limit) / flux
 
@@ -1013,21 +1052,18 @@
             dev = self._cache_deviate[key]
         else:
             if bandpass is None:
                 sed = self
             else:
                 sed = self._mul_bandpass(bandpass)
 
-            if isinstance(sed._fast_spec, LookupTable):
-                dev = DistDeviate(function=sed._fast_spec, npoints=npoints)
-            else:
-                xmin = sed.blue_limit / (1.+self.redshift)
-                xmax = sed.red_limit / (1.+self.redshift)
-                dev = DistDeviate(function=sed._fast_spec, x_min=xmin, x_max=xmax,
-                                  npoints=npoints)
+            xmin = sed.blue_limit / (1.+self.redshift)
+            xmax = sed.red_limit / (1.+self.redshift)
+            dev = DistDeviate(function=sed._fast_spec, x_min=xmin, x_max=xmax,
+                              npoints=npoints, clip_neg=True)
             self._cache_deviate[key] = dev
 
         # Reset the deviate explicitly
         if rng is not None: dev.reset(rng)
 
         ret = np.empty(nphotons)
         dev.generate(ret)
@@ -1063,18 +1099,18 @@
         if not hasattr(self, '_hash'):
             self._hash = hash(("galsim.SED", self._orig_spec, self.wave_type, self.flux_type,
                                self.redshift, self.fast, self.blue_limit, self.red_limit,
                                tuple(self.wave_list)))
         return self._hash
 
     def __repr__(self):
-        outstr = ('galsim.SED(%r, wave_type=%r, flux_type=%r, redshift=%r, fast=%r,'
-                  ' _wave_list=%r, _blue_limit=%r, _red_limit=%s)')%(
+        outstr = ('galsim.SED(%r, wave_type=%r, flux_type=%r, redshift=%r, fast=%r, '
+                  'interpolant=%r, _wave_list=%r, _blue_limit=%r, _red_limit=%s)')%(
                       self._orig_spec, self.wave_type, self._flux_type, self.redshift, self.fast,
-                      self.wave_list, self.blue_limit,
+                      self.interpolant, self.wave_list, self.blue_limit,
                       "float('inf')" if self.red_limit == np.inf else repr(self.red_limit))
         return outstr
 
     def __str__(self):
         orig_spec = repr(self._orig_spec)
         if len(orig_spec) > 80:
             orig_spec = str(self._orig_spec)
@@ -1108,32 +1144,44 @@
         wavelength:    The wavelength of the line.
         fwhm:          The full-width-half-max of the line.  [default: 1.0]
         flux:          The integrated flux of the line.  [default: 1.0]
         wave_type:     The units of ``wavelength`` and ``fwhm`` above.  See SED
                        constructor for options.  [default: 'nm']
         flux_type:     The units of flux used for this SED.  See SED constructor
                        for options.  [default: 'fphotons']
+        max_wave       The maximum wavelength to use in the LookupTable for the SED.
+                       [default: {}; must be > wavelength+fwhm]
         **kwargs:      Any additional keyword arguments to pass to the `SED`
                        constructor.
-    """
+    """.format(SED._bolo_max_wave)
     def __init__(
         self,
         wavelength,
         fwhm=1.0,
         flux=1.0,
         wave_type='nm',
         flux_type='fphotons',
+        max_wave=SED._bolo_max_wave,
         **kwargs
     ):
         self.wavelength = wavelength
         self.fwhm = fwhm
         self.flux = flux
+        _, wave_factor = SED._parse_wave_type(wave_type)
+        if wave_factor is None:
+            raise GalSimValueError("wave_type must be a distance unit", wave_type)
+        assert max_wave > wavelength + fwhm
+
+        w = wavelength
+        # Some operations can turn a 0 into 1.e-15, which can lead to large errors
+        # when integrating from w+fwhm to max_wave.  So add a second set of 0's at
+        # w +- 2*fwhm to make sure it's exactly 0 for most of the range.
         spec = LookupTable(
-            [0.0, wavelength-fwhm, wavelength, wavelength+fwhm, np.inf],
-            [0, 0, flux/fwhm, 0, 0],
+            [0.0, w-2*fwhm, w-fwhm, w, w+fwhm, w+2*fwhm, max_wave*wave_factor],
+            [0, 0, 0, flux/fwhm, 0, 0, 0],
             interpolant='linear'
         )
         super().__init__(
             spec,
             wave_type=wave_type,
             flux_type=flux_type,
             **kwargs
@@ -1148,18 +1196,17 @@
         Returns:
             the redshifted `EmissionLine`.
         """
         if redshift == self.redshift:
             return self
         if redshift <= -1:
             raise GalSimRangeError("Invalid redshift", redshift, -1.)
-        zfactor = (1.0 + redshift) / (1.0 + self.redshift)
         return EmissionLine(
-            self.wavelength * zfactor,
-            self.fwhm * zfactor,
+            self.wavelength,
+            self.fwhm,
             flux=self.flux,
             wave_type=self.wave_type,
             flux_type=self.flux_type,
             redshift=redshift,
             fast=self.fast
         )
```

### Comparing `GalSim-2.5.0/galsim/sensor.py` & `GalSim-2.5.1/galsim/sensor.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/sersic.py` & `GalSim-2.5.1/galsim/sersic.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/shapelet.py` & `GalSim-2.5.1/galsim/shapelet.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/SEDs/CWW_E_ext.sed` & `GalSim-2.5.1/galsim/share/SEDs/CWW_E_ext.sed`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/SEDs/CWW_E_ext_more.sed` & `GalSim-2.5.1/galsim/share/SEDs/CWW_E_ext_more.sed`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/SEDs/CWW_Im_ext.sed` & `GalSim-2.5.1/galsim/share/SEDs/CWW_Im_ext.sed`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/SEDs/CWW_Im_ext_more.sed` & `GalSim-2.5.1/galsim/share/SEDs/CWW_Im_ext_more.sed`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/SEDs/CWW_Sbc_ext.sed` & `GalSim-2.5.1/galsim/share/SEDs/CWW_Sbc_ext.sed`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/SEDs/CWW_Sbc_ext_more.sed` & `GalSim-2.5.1/galsim/share/SEDs/CWW_Sbc_ext_more.sed`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/SEDs/CWW_Scd_ext.sed` & `GalSim-2.5.1/galsim/share/SEDs/CWW_Scd_ext.sed`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/SEDs/CWW_Scd_ext_more.sed` & `GalSim-2.5.1/galsim/share/SEDs/CWW_Scd_ext_more.sed`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/SEDs/vega.txt` & `GalSim-2.5.1/galsim/share/SEDs/vega.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/acs_I_unrot_sci_20_cf.fits` & `GalSim-2.5.1/galsim/share/acs_I_unrot_sci_20_cf.fits`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/bandpasses/ACS_wfc_F435W.dat` & `GalSim-2.5.1/galsim/share/bandpasses/ACS_wfc_F435W.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/bandpasses/ACS_wfc_F606W.dat` & `GalSim-2.5.1/galsim/share/bandpasses/ACS_wfc_F606W.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/bandpasses/ACS_wfc_F775W.dat` & `GalSim-2.5.1/galsim/share/bandpasses/ACS_wfc_F775W.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/bandpasses/ACS_wfc_F814W.dat` & `GalSim-2.5.1/galsim/share/bandpasses/ACS_wfc_F814W.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/bandpasses/ACS_wfc_F850LP.dat` & `GalSim-2.5.1/galsim/share/bandpasses/ACS_wfc_F850LP.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/bandpasses/LSST_g.dat` & `GalSim-2.5.1/galsim/share/bandpasses/LSST_g.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/bandpasses/LSST_i.dat` & `GalSim-2.5.1/galsim/share/bandpasses/LSST_i.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/bandpasses/LSST_r.dat` & `GalSim-2.5.1/galsim/share/bandpasses/LSST_r.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/bandpasses/LSST_u.dat` & `GalSim-2.5.1/galsim/share/bandpasses/LSST_u.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/bandpasses/LSST_y.dat` & `GalSim-2.5.1/galsim/share/bandpasses/LSST_y.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/bandpasses/LSST_z.dat` & `GalSim-2.5.1/galsim/share/bandpasses/LSST_z.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/bandpasses/WFC3_ir_F105W.dat` & `GalSim-2.5.1/galsim/share/bandpasses/WFC3_ir_F105W.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/bandpasses/WFC3_ir_F125W.dat` & `GalSim-2.5.1/galsim/share/bandpasses/WFC3_ir_F125W.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/bandpasses/WFC3_ir_F160W.dat` & `GalSim-2.5.1/galsim/share/bandpasses/WFC3_ir_F160W.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/bandpasses/WFC3_uvis_F275W.dat` & `GalSim-2.5.1/galsim/share/bandpasses/WFC3_uvis_F275W.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/bandpasses/WFC3_uvis_F336W.dat` & `GalSim-2.5.1/galsim/share/bandpasses/WFC3_uvis_F336W.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_F184_SCA_1.fits.gz` & `GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_F184_SCA_1.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_F184_SCA_10.fits.gz` & `GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_F184_SCA_10.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_F184_SCA_11.fits.gz` & `GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_F184_SCA_11.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_F184_SCA_12.fits.gz` & `GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_F184_SCA_12.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_F184_SCA_13.fits.gz` & `GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_F184_SCA_13.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_F184_SCA_14.fits.gz` & `GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_F184_SCA_14.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_F184_SCA_15.fits.gz` & `GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_F184_SCA_15.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_F184_SCA_16.fits.gz` & `GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_F184_SCA_16.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_F184_SCA_17.fits.gz` & `GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_F184_SCA_17.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_F184_SCA_18.fits.gz` & `GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_F184_SCA_18.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_F184_SCA_2.fits.gz` & `GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_F184_SCA_2.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_F184_SCA_3.fits.gz` & `GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_F184_SCA_3.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_F184_SCA_4.fits.gz` & `GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_F184_SCA_4.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_F184_SCA_5.fits.gz` & `GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_F184_SCA_5.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_F184_SCA_6.fits.gz` & `GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_F184_SCA_6.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_F184_SCA_7.fits.gz` & `GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_F184_SCA_7.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_F184_SCA_8.fits.gz` & `GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_F184_SCA_8.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_F184_SCA_9.fits.gz` & `GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_F184_SCA_9.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_skinny_SCA_1.fits.gz` & `GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_skinny_SCA_1.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_skinny_SCA_10.fits.gz` & `GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_skinny_SCA_10.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_skinny_SCA_11.fits.gz` & `GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_skinny_SCA_11.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_skinny_SCA_12.fits.gz` & `GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_skinny_SCA_12.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_skinny_SCA_13.fits.gz` & `GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_skinny_SCA_13.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_skinny_SCA_14.fits.gz` & `GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_skinny_SCA_14.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_skinny_SCA_15.fits.gz` & `GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_skinny_SCA_15.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_skinny_SCA_16.fits.gz` & `GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_skinny_SCA_16.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_skinny_SCA_17.fits.gz` & `GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_skinny_SCA_17.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_skinny_SCA_18.fits.gz` & `GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_skinny_SCA_18.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_skinny_SCA_2.fits.gz` & `GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_skinny_SCA_2.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_skinny_SCA_3.fits.gz` & `GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_skinny_SCA_3.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_skinny_SCA_4.fits.gz` & `GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_skinny_SCA_4.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_skinny_SCA_5.fits.gz` & `GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_skinny_SCA_5.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_skinny_SCA_6.fits.gz` & `GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_skinny_SCA_6.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_skinny_SCA_7.fits.gz` & `GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_skinny_SCA_7.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_skinny_SCA_8.fits.gz` & `GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_skinny_SCA_8.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/roman/RST_WIM_Filter_skinny_SCA_9.fits.gz` & `GalSim-2.5.1/galsim/share/roman/RST_WIM_Filter_skinny_SCA_9.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_01.txt` & `GalSim-2.5.1/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_01.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_02.txt` & `GalSim-2.5.1/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_02.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_03.txt` & `GalSim-2.5.1/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_03.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_04.txt` & `GalSim-2.5.1/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_04.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_05.txt` & `GalSim-2.5.1/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_05.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_06.txt` & `GalSim-2.5.1/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_06.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_07.txt` & `GalSim-2.5.1/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_07.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_08.txt` & `GalSim-2.5.1/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_08.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_09.txt` & `GalSim-2.5.1/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_09.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_10.txt` & `GalSim-2.5.1/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_10.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_11.txt` & `GalSim-2.5.1/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_11.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_12.txt` & `GalSim-2.5.1/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_12.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_13.txt` & `GalSim-2.5.1/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_13.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_14.txt` & `GalSim-2.5.1/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_14.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_15.txt` & `GalSim-2.5.1/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_15.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_16.txt` & `GalSim-2.5.1/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_16.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_17.txt` & `GalSim-2.5.1/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_17.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_18.txt` & `GalSim-2.5.1/galsim/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_18.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/roman/Roman_SRR_WFC_Pupil_Mask_Longwave_2048_reformatted.fits.gz` & `GalSim-2.5.1/galsim/share/roman/Roman_SRR_WFC_Pupil_Mask_Longwave_2048_reformatted.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/roman/Roman_SRR_WFC_Pupil_Mask_Shortwave_2048_reformatted.fits.gz` & `GalSim-2.5.1/galsim/share/roman/Roman_SRR_WFC_Pupil_Mask_Shortwave_2048_reformatted.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/roman/Roman_effarea_20210614.txt` & `GalSim-2.5.1/galsim/share/roman/Roman_effarea_20210614.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/roman/roman_sky_backgrounds.txt` & `GalSim-2.5.1/galsim/share/roman/roman_sky_backgrounds.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/roman/sca_positions_20210204.txt` & `GalSim-2.5.1/galsim/share/roman/sca_positions_20210204.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/roman/sip_20210204.txt` & `GalSim-2.5.1/galsim/share/roman/sip_20210204.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/sensors/abs_length.dat` & `GalSim-2.5.1/galsim/share/sensors/abs_length.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/sensors/lsst_e2v_32.cfg` & `GalSim-2.5.1/galsim/share/sensors/lsst_e2v_32.cfg`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/sensors/lsst_e2v_32.dat` & `GalSim-2.5.1/galsim/share/sensors/lsst_e2v_32.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/sensors/lsst_e2v_50_32.cfg` & `GalSim-2.5.1/galsim/share/sensors/lsst_e2v_50_32.cfg`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/sensors/lsst_e2v_50_32.dat` & `GalSim-2.5.1/galsim/share/sensors/lsst_e2v_50_32.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/sensors/lsst_e2v_50_8.cfg` & `GalSim-2.5.1/galsim/share/sensors/lsst_e2v_50_8.cfg`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/sensors/lsst_e2v_50_8.dat` & `GalSim-2.5.1/galsim/share/sensors/lsst_e2v_50_8.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/sensors/lsst_e2v_8.cfg` & `GalSim-2.5.1/galsim/share/sensors/lsst_e2v_8.cfg`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/sensors/lsst_e2v_8.dat` & `GalSim-2.5.1/galsim/share/sensors/lsst_e2v_8.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/sensors/lsst_itl_32.cfg` & `GalSim-2.5.1/galsim/share/sensors/lsst_itl_32.cfg`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/sensors/lsst_itl_32.dat` & `GalSim-2.5.1/galsim/share/sensors/lsst_itl_32.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/sensors/lsst_itl_50_32.cfg` & `GalSim-2.5.1/galsim/share/sensors/lsst_itl_50_32.cfg`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/sensors/lsst_itl_50_32.dat` & `GalSim-2.5.1/galsim/share/sensors/lsst_itl_50_32.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/sensors/lsst_itl_50_8.cfg` & `GalSim-2.5.1/galsim/share/sensors/lsst_itl_50_8.cfg`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/sensors/lsst_itl_50_8.dat` & `GalSim-2.5.1/galsim/share/sensors/lsst_itl_50_8.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/sensors/lsst_itl_8.cfg` & `GalSim-2.5.1/galsim/share/sensors/lsst_itl_8.cfg`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/sensors/lsst_itl_8.dat` & `GalSim-2.5.1/galsim/share/sensors/lsst_itl_8.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/share/wfc_F814W.dat.gz` & `GalSim-2.5.1/galsim/share/wfc_F814W.dat.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/shear.py` & `GalSim-2.5.1/galsim/shear.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/spergel.py` & `GalSim-2.5.1/galsim/spergel.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/sum.py` & `GalSim-2.5.1/galsim/sum.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 import copy
 
 from .gsparams import GSParams
 from .gsobject import GSObject
 from .utilities import lazy_property
 from . import _galsim
 from .photon_array import PhotonArray
-from .random import BinomialDeviate
+from .random import UniformDeviate
 from . import chromatic as chrom
 
 
 def Add(*args, **kwargs):
     """A function for adding 2 or more `GSObject` or `ChromaticObject` instances.
 
     This function will inspect its input arguments to decide if a `Sum` object or a
@@ -306,47 +306,41 @@
         if len(self.obj_list) > 1:
             im1 = image.copy()
             for obj in self.obj_list[1:]:
                 obj._drawReal(im1, jac, offset, flux_scaling)
                 image += im1
 
     def _shoot(self, photons, rng):
-        remainingAbsoluteFlux = self.positive_flux + self.negative_flux
-        fluxPerPhoton = remainingAbsoluteFlux / len(photons)
-
-        remainingN = len(photons)
-        istart = 0  # The location in the photons array where we assign the component arrays.
-
-        # Get photons from each summand, using BinomialDeviate to randomize
-        # the distribution of photons among summands
-        for i, obj in enumerate(self.obj_list):
-            thisAbsoluteFlux = obj.positive_flux + obj.negative_flux
-
-            # How many photons to shoot from this summand?
-            thisN = remainingN  # All of what's left, if this is the last summand...
-            if i < len(self.obj_list)-1:
-                # otherwise, allocate a randomized fraction of the remaining photons to summand.
-                bd = BinomialDeviate(rng, remainingN, thisAbsoluteFlux/remainingAbsoluteFlux)
-                thisN = int(bd())
-            if thisN > 0:
-                thisPA = obj.shoot(thisN, rng)
-                # Now rescale the photon fluxes so that they are each nominally fluxPerPhoton
-                # whereas the shoot() routine would have made them each nominally
-                # thisAbsoluteFlux/thisN
-                thisPA.scaleFlux(fluxPerPhoton*thisN/thisAbsoluteFlux)
-                photons.assignAt(istart, thisPA)
-                istart += thisN
-            remainingN -= thisN
-            remainingAbsoluteFlux -= thisAbsoluteFlux
-        #assert remainingN == 0
-        #assert np.isclose(remainingAbsoluteFlux, 0.0)
-
-        # This process produces correlated photons, so mark the resulting array as such.
-        if len(self.obj_list) > 1:
-            photons.setCorrelated()
+        # We probabilistically choose a component for each photon based on the
+        # relative flux density of that component for the given wavelength.
+        comp_flux = np.array([obj.positive_flux + obj.negative_flux for obj in self._obj_list])
+        total_flux = np.sum(comp_flux)
+
+        prob = comp_flux / total_flux
+        cdf = np.cumsum(prob)
+
+        u = np.empty(len(photons))
+        UniformDeviate(rng).generate(u)
+        use_k = np.sum((u >= cdf[:,None]), axis=0)
+        n = len(self._obj_list)
+        use_k[use_k==n] = n-1  # This shouldn't be possible, but maybe with numerical rounding...
+
+        fluxPerPhoton = total_flux / len(photons)
+
+        # Shoot the corresponding photons from each component.
+        for kk, obj in enumerate(self.obj_list):
+            use = (use_k == kk)  # True for each photon where this is the object to shoot from
+            this_n = np.sum(use)
+            if this_n == 0:
+                continue
+            temp = PhotonArray(this_n)
+            temp._copyFrom(photons, slice(None), use, do_xy=False, do_flux=False)
+            obj._shoot(temp, rng)
+            temp.flux = fluxPerPhoton
+            photons._copyFrom(temp, use, slice(None))
 
     def _drawKImage(self, image, jac=None):
         self.obj_list[0]._drawKImage(image, jac)
         if len(self.obj_list) > 1:
             im1 = image.copy()
             for obj in self.obj_list[1:]:
                 obj._drawKImage(im1, jac)
```

### Comparing `GalSim-2.5.0/galsim/table.py` & `GalSim-2.5.1/galsim/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -340,14 +340,15 @@
                         means to use self.x_max]
             x_factor:   Optionally scale the x values of f by this factor when doing the integral.
                         I.e. Find :math:`\int f(x x_\mathrm{factor}) g(x) dx`. [default: 1]
 
         Returns:
             an estimate of the integral
         """
+        from .utilities import merge_sorted
         if self.x_log:
             raise GalSimNotImplementedError("log x spacing not implemented yet.")
         if self.f_log:
             raise GalSimNotImplementedError("log f values not implemented yet.")
         if not isinstance(self.interpolant, basestring):
             raise GalSimNotImplementedError(
                 "Integration with interpolant=%s is not implemented."%(self.interpolant))
@@ -368,15 +369,15 @@
             x_min = max(x_min, g.x_min)
             x_max = min(x_max, g.x_max)
             if x_min >= x_max:
                 return 0.
         else:
             gx = self.x / x_factor
             gx = gx[(gx >= x_min) & (gx <= x_max)]
-            gx = np.union1d(gx, [x_min, x_max])
+            gx = merge_sorted([gx, [x_min, x_max]])
             # Let this raise an appropriate error if g is not a valid function over this domain.
             gf = g(gx)
             # If g is a constant function (like lambda wave: 1), then this doesn't return
             # an array.  Make it one.
             try:
                 len(gf)
             except TypeError:
@@ -386,19 +387,21 @@
             g = _LookupTable(gx, gf, 'linear')
 
         return self._tab.integrate_product(g._tab, float(x_min), float(x_max), float(x_factor))
 
     def _check_range(self, x):
         slop = (self.x_max - self.x_min) * 1.e-6
         if np.min(x,initial=self.x_min) < self.x_min - slop:
+            xx = np.array(x)
             raise GalSimRangeError("x value(s) below the range of the LookupTable.",
-                                   x, self.x_min, self.x_max)
+                                   xx[xx<self.x_min], self.x_min, self.x_max) from None
         if np.max(x,initial=self.x_max) > self.x_max + slop:  # pragma: no branch
+            xx = np.array(x)
             raise GalSimRangeError("x value(s) above the range of the LookupTable.",
-                                   x, self.x_min, self.x_max)
+                                   xx[xx>self.x_max], self.x_min, self.x_max) from None
 
     def getArgs(self):
         return self.x
 
     def getVals(self):
         return self.f
 
@@ -548,29 +551,31 @@
     if interpolant in ('nearest', 'linear', 'ceil', 'floor', 'spline'):
         ret._interp1d = None
     else:
         ret._interp1d = convert_interpolant(interpolant)
     return ret
 
 
-def trapz(f, x):
+def trapz(f, x, interpolant='linear'):
     """Integrate f(x) using the trapezoidal rule.
 
     Equivalent to np.trapz(f,x) for 1d array inputs.  Intended as a drop-in replacement,
     which is usually faster.
 
     Parameters:
-        f:      The ordinates of the function to integrate.
-        x:      The abscissae of the function to integrate.
+        f:              The ordinates of the function to integrate.
+        x:              The abscissae of the function to integrate.
+        interpolant:    The interpolant to use between the tabulated points.  [default: 'linear',
+                        which matches the behavior of np.trapz]
 
     Returns:
         Estimate of the integral.
     """
     if len(x) >= 2:
-        return _LookupTable(x,f,'linear').integrate()
+        return _LookupTable(x, f, interpolant=interpolant).integrate()
     else:
         return 0.
 
 
 class LookupTable2D:
     """
     LookupTable2D represents a 2-dimensional lookup table to store function values that may be slow
```

### Comparing `GalSim-2.5.0/galsim/transform.py` & `GalSim-2.5.1/galsim/transform.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/utilities.py` & `GalSim-2.5.1/galsim/utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 from . import _galsim
 from .errors import GalSimError, GalSimValueError, GalSimIncompatibleValuesError, GalSimRangeError
 from .errors import galsim_warn
 from .position import Position, PositionD, PositionI, _PositionD, _PositionI
 from .angle import AngleUnit, arcsec
 from .image import Image
-from .table import trapz, LookupTable2D
+from .table import trapz, _LookupTable, LookupTable2D
 from .wcs import JacobianWCS, PixelScale
 from .position import _PositionD
 from .random import BaseDeviate, UniformDeviate
 from . import meta_data
 
 # A couple things are documented as galsim.utilties.* functions, but live in other files.
 # Bring them into scope here.
@@ -219,40 +219,66 @@
         # Note that for the next two lines, pos *must* be a list, not a tuple.  Assignments to
         # elements of tuples is not allowed.
         pos[0] *= scale
         pos[1] *= scale
 
     return pos
 
-def _lin_approx_err(x, f, i):
+def _spline_approx_err(x, f, left, right, splitpoints, i):
+    # For splines, we can't just do the integral over a small range, since the spline slopes
+    # are all wrong.  Rather we compute a spline function with the current splitpoints and
+    # just the single point in the trial region and recompute a spline function with that.
+    # Then we can compute the total error from that approximation.
+    # (For the error integral, we still use linear.)
+
+    indices = sorted(splitpoints + [i])
+    new_tab = _LookupTable(x[indices], f[indices], 'spline')
+
+    xleft, xright = x[left:i+1], x[i:right+1]
+    fleft, fright = f[left:i+1], f[i:right+1]
+    f2left = new_tab(xleft)
+    f2right = new_tab(xright)
+    return trapz(np.abs(fleft-f2left), xleft), trapz(np.abs(fright-f2right), xright)
+
+def _spline_approx_split(x, f, left, right, splitpoints):
+    r"""Split a tabulated function into a two-part piecewise spline approximation by exactly
+    minimizing \int abs(f(x) - approx(x)) dx.  Operates in O(N^2) time.
+    """
+    errs = [_spline_approx_err(x, f, left, right, splitpoints, i) for i in range(left+1, right)]
+    i = np.argmin(np.sum(errs, axis=1))
+    return i+left+1, errs[i]
+
+def _lin_approx_err(x, f, left, right, i):
     r"""Error as \int abs(f(x) - approx(x)) when using ith data point to make piecewise linear
     approximation.
     """
-    xleft, xright = x[:i+1], x[i:]
-    fleft, fright = f[:i+1], f[i:]
+    xleft, xright = x[left:i+1], x[i:right+1]
+    fleft, fright = f[left:i+1], f[i:right+1]
     xi, fi = x[i], f[i]
-    mleft = (fi-f[0])/(xi-x[0])
-    mright = (f[-1]-fi)/(x[-1]-xi)
-    f2left = f[0]+mleft*(xleft-x[0])
+    mleft = (fi-f[left])/(xi-x[left])
+    mright = (f[right]-fi)/(x[right]-xi)
+    f2left = f[left]+mleft*(xleft-x[left])
     f2right = fi+mright*(xright-xi)
     return trapz(np.abs(fleft-f2left), xleft), trapz(np.abs(fright-f2right), xright)
 
-def _exact_lin_approx_split(x, f):
+def _exact_lin_approx_split(x, f, left, right, splitpoints):
     r"""Split a tabulated function into a two-part piecewise linear approximation by exactly
     minimizing \int abs(f(x) - approx(x)) dx.  Operates in O(N^2) time.
     """
-    errs = [_lin_approx_err(x, f, i) for i in range(1, len(x)-1)]
+    errs = [_lin_approx_err(x, f, left, right, i) for i in range(left+1, right)]
     i = np.argmin(np.sum(errs, axis=1))
-    return i+1, errs[i]
+    return i+left+1, errs[i]
 
-def _lin_approx_split(x, f):
+def _lin_approx_split(x, f, left, right, splitpoints):
     r"""Split a tabulated function into a two-part piecewise linear approximation by approximately
     minimizing \int abs(f(x) - approx(x)) dx.  Chooses the split point by exactly minimizing
     \int (f(x) - approx(x))^2 dx in O(N) time.
     """
+    x = x[left:right+1]
+    f = f[left:right+1]
     dx = x[2:] - x[:-2]
     # Error contribution on the left.
     ff0 = f[1:-1]-f[0]  # Only need to search between j=1..(N-1)
     xx0 = x[1:-1]-x[0]
     mleft = ff0/xx0  # slope
     errleft = (np.cumsum(dx*ff0**2)
                - 2*mleft*np.cumsum(dx*ff0*xx0)
@@ -265,18 +291,18 @@
     errright = (np.cumsum(dx*ffN**2)
                 - 2*mright*np.cumsum(dx*ffN*xxN)
                 + mright**2*np.cumsum(dx*xxN**2))
     errright = errright[::-1]
 
     # Get absolute error for the found point.
     i = np.argmin(errleft+errright)
-    return i+1, _lin_approx_err(x, f, i+1)
+    return i+left+1, _lin_approx_err(x, f, 0, len(x)-1, i+1)
 
 def thin_tabulated_values(x, f, rel_err=1.e-4, trim_zeros=True, preserve_range=True,
-                          fast_search=True):
+                          fast_search=True, interpolant='linear'):
     """
     Remove items from a set of tabulated f(x) values so that the error in the integral is still
     accurate to a given relative accuracy.
 
     The input ``x`` and ``f`` values can be lists, NumPy arrays, or really anything that can be
     converted to a NumPy array.  The new lists will be output as numpy arrays.
 
@@ -295,19 +321,25 @@
                         significant? (False)  [default: True]
         fast_search:    If set to True, then the underlying algorithm will use a relatively fast
                         O(N) algorithm to select points to include in the thinned approximation.
                         If set to False, then a slower O(N^2) algorithm will be used.  We have
                         found that the slower algorithm tends to yield a thinned representation
                         that retains fewer samples while still meeting the relative error
                         requirement.  [default: True]
+        interpolant:    The interpolant to assume for the tabulated values. [default: 'linear']
 
     Returns:
         a tuple of lists (x_new, y_new) with the thinned tabulation.
     """
-    split_fn = _lin_approx_split if fast_search else _exact_lin_approx_split
+    if interpolant == 'spline':
+        split_fn = _spline_approx_split
+    elif fast_search:
+        split_fn = _lin_approx_split
+    else:
+        split_fn = _exact_lin_approx_split
 
     x = np.asarray(x, dtype=float)
     f = np.asarray(f, dtype=float)
 
     # Check for valid inputs
     if len(x) != len(f):
         raise GalSimIncompatibleValuesError("len(x) != len(f)", x=x, f=f)
@@ -317,29 +349,29 @@
         raise GalSimValueError("input x is not sorted.", x)
 
     # Check for trivial noop.
     if len(x) <= 2:
         # Nothing to do
         return x,f
 
-    total_integ = trapz(abs(f), x)
+    total_integ = trapz(abs(f), x, interpolant)
     if total_integ == 0:
         return np.array([ x[0], x[-1] ]), np.array([ f[0], f[-1] ])
     thresh = total_integ * rel_err
 
     if trim_zeros:
         first = max(f.nonzero()[0][0]-1, 0)  # -1 to keep one non-redundant zero.
         last = min(f.nonzero()[0][-1]+1, len(x)-1)  # +1 to keep one non-redundant zero.
         x, f = x[first:last+1], f[first:last+1]
 
-    x_range = x[-1] - x[0]
     if not preserve_range:
         # Remove values from the front that integrate to less than thresh.
         err_integ1 = 0.5 * (abs(f[0]) + abs(f[1])) * (x[1] - x[0])
         k0 = 0
+        x_range = x[-1] - x[0]
         while k0 < len(x)-2 and err_integ1 < thresh * (x[k0+1]-x[0]) / x_range:
             k0 = k0+1
             err_integ1 += 0.5 * (abs(f[k0]) + abs(f[k0+1])) * (x[k0+1] - x[k0])
         # Now the integral from 0 to k0+1 (inclusive) is a bit too large.
         # That means k0 is the largest value we can use that will work as the starting value.
 
         # Remove values from the back that integrate to less than thresh.
@@ -348,38 +380,55 @@
         while k1 > k0 and err_integ2 < thresh * (x[-1]-x[k1-1]) / x_range:
             k1 = k1-1
             err_integ2 += 0.5 * (abs(f[k1-1]) + abs(f[k1])) * (x[k1] - x[k1-1])
         # Now the integral from k1-1 to len(x)-1 (inclusive) is a bit too large.
         # That means k1 is the smallest value we can use that will work as the ending value.
 
         # Subtract the error so far from thresh
-        thresh -= trapz(abs(f[:k0]),x[:k0]) + trapz(abs(f[k1:]),x[k1:])
+        if interpolant == 'spline':
+            new_integ = trapz(abs(f[k0:k1+1]),x[k0:k1+1], interpolant='spline')
+            thresh -= np.abs(new_integ-total_integ)
+        else:
+            thresh -= trapz(abs(f[:k0]),x[:k0]) + trapz(abs(f[k1:]),x[k1:])
 
         x = x[k0:k1+1]  # +1 since end of range is given as one-past-the-end.
         f = f[k0:k1+1]
 
-        # And update x_range for the new values
-        x_range = x[-1] - x[0]
-
     # Check again for noop after trimming endpoints.
     if len(x) <= 2:
         return x,f
 
     # Thin interior points.  Start with no interior points and then greedily add them back in one at
     # a time until relative error goal is met.
     # Use a heap to track:
     heap = [(-2*thresh,  # -err; initialize large enough to trigger while loop below.
              0,          # first index of interval
              len(x)-1)]  # last index of interval
-    while (-sum(h[0] for h in heap) > thresh):
+    splitpoints = [0,len(x)-1]
+    while len(heap) > 0:
         _, left, right = heapq.heappop(heap)
-        i, (errleft, errright) = split_fn(x[left:right+1], f[left:right+1])
-        heapq.heappush(heap, (-errleft, left, i+left))
-        heapq.heappush(heap, (-errright, i+left, right))
-    splitpoints = sorted([0]+[h[2] for h in heap])
+        i, (errleft, errright) = split_fn(x, f, left, right, splitpoints)
+        splitpoints.append(i)
+        if i > left+1:
+            heapq.heappush(heap, (-errleft, left, i))
+        if right > i+1:
+            heapq.heappush(heap, (-errright, i, right))
+        if interpolant != 'spline':
+            # This is a sufficient stopping criterion for linear
+            if (-sum(h[0] for h in heap) < thresh):
+                break
+        else:
+            # For spline, we also need to recompute the total integral to make sure
+            # that the realized total error is less than thresh.
+            if (-sum(h[0] for h in heap) < thresh):
+                splitpoints = sorted(splitpoints)
+                current_integ = trapz(f[splitpoints], x[splitpoints], interpolant)
+                if np.abs(current_integ - total_integ) < thresh:
+                    break
+    splitpoints = sorted(splitpoints)
     return x[splitpoints], f[splitpoints]
 
 def old_thin_tabulated_values(x, f, rel_err=1.e-4, preserve_range=False): # pragma: no cover
     """
     Remove items from a set of tabulated f(x) values so that the error in the integral is still
     accurate to a given relative accuracy.
```

### Comparing `GalSim-2.5.0/galsim/vonkarman.py` & `GalSim-2.5.1/galsim/vonkarman.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/wcs.py` & `GalSim-2.5.1/galsim/wcs.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/wfirst.py` & `GalSim-2.5.1/galsim/wfirst.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/galsim/zernike.py` & `GalSim-2.5.1/galsim/zernike.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/GalSim.h` & `GalSim-2.5.1/include/GalSim.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/fftw3/fftw3.h` & `GalSim-2.5.1/include/fftw3/fftw3.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/BinomFact.h` & `GalSim-2.5.1/include/galsim/BinomFact.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/Bounds.h` & `GalSim-2.5.1/include/galsim/Bounds.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/CDModel.h` & `GalSim-2.5.1/include/galsim/CDModel.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/CorrelatedNoise.h` & `GalSim-2.5.1/include/galsim/CorrelatedNoise.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/GSParams.h` & `GalSim-2.5.1/include/galsim/GSParams.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/Image.h` & `GalSim-2.5.1/include/galsim/Image.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/ImageArith.h` & `GalSim-2.5.1/include/galsim/ImageArith.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/Interpolant.h` & `GalSim-2.5.1/include/galsim/Interpolant.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/LRUCache.h` & `GalSim-2.5.1/include/galsim/LRUCache.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/Laguerre.h` & `GalSim-2.5.1/include/galsim/Laguerre.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/OneDimensionalDeviate.h` & `GalSim-2.5.1/include/galsim/OneDimensionalDeviate.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/PhotonArray.h` & `GalSim-2.5.1/include/galsim/PhotonArray.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/Polygon.h` & `GalSim-2.5.1/include/galsim/Polygon.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/ProbabilityTree.h` & `GalSim-2.5.1/include/galsim/ProbabilityTree.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/Random.h` & `GalSim-2.5.1/include/galsim/Random.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/RealGalaxy.h` & `GalSim-2.5.1/include/galsim/RealGalaxy.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/SBAdd.h` & `GalSim-2.5.1/include/galsim/SBAdd.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/SBAddImpl.h` & `GalSim-2.5.1/include/galsim/SBAddImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/SBAiry.h` & `GalSim-2.5.1/include/galsim/SBAiry.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/SBAiryImpl.h` & `GalSim-2.5.1/include/galsim/SBAiryImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/SBBox.h` & `GalSim-2.5.1/include/galsim/SBBox.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/SBBoxImpl.h` & `GalSim-2.5.1/include/galsim/SBBoxImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/SBConvolve.h` & `GalSim-2.5.1/include/galsim/SBConvolve.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/SBConvolveImpl.h` & `GalSim-2.5.1/include/galsim/SBConvolveImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/SBDeconvolve.h` & `GalSim-2.5.1/include/galsim/SBDeconvolve.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/SBDeconvolveImpl.h` & `GalSim-2.5.1/include/galsim/SBDeconvolveImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/SBDeltaFunction.h` & `GalSim-2.5.1/include/galsim/SBDeltaFunction.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/SBDeltaFunctionImpl.h` & `GalSim-2.5.1/include/galsim/SBDeltaFunctionImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/SBExponential.h` & `GalSim-2.5.1/include/galsim/SBExponential.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/SBExponentialImpl.h` & `GalSim-2.5.1/include/galsim/SBExponentialImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/SBFourierSqrt.h` & `GalSim-2.5.1/include/galsim/SBFourierSqrt.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/SBFourierSqrtImpl.h` & `GalSim-2.5.1/include/galsim/SBFourierSqrtImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/SBGaussian.h` & `GalSim-2.5.1/include/galsim/SBGaussian.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/SBGaussianImpl.h` & `GalSim-2.5.1/include/galsim/SBGaussianImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/SBInclinedExponential.h` & `GalSim-2.5.1/include/galsim/SBInclinedExponential.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/SBInclinedExponentialImpl.h` & `GalSim-2.5.1/include/galsim/SBInclinedExponentialImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/SBInclinedSersic.h` & `GalSim-2.5.1/include/galsim/SBInclinedSersic.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/SBInclinedSersicImpl.h` & `GalSim-2.5.1/include/galsim/SBInclinedSersicImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/SBInterpolatedImage.h` & `GalSim-2.5.1/include/galsim/SBInterpolatedImage.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/SBInterpolatedImageImpl.h` & `GalSim-2.5.1/include/galsim/SBInterpolatedImageImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/SBKolmogorov.h` & `GalSim-2.5.1/include/galsim/SBKolmogorov.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/SBKolmogorovImpl.h` & `GalSim-2.5.1/include/galsim/SBKolmogorovImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/SBMoffat.h` & `GalSim-2.5.1/include/galsim/SBMoffat.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/SBMoffatImpl.h` & `GalSim-2.5.1/include/galsim/SBMoffatImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/SBProfile.h` & `GalSim-2.5.1/include/galsim/SBProfile.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/SBProfileImpl.h` & `GalSim-2.5.1/include/galsim/SBProfileImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/SBSecondKick.h` & `GalSim-2.5.1/include/galsim/SBSecondKick.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/SBSecondKickImpl.h` & `GalSim-2.5.1/include/galsim/SBSecondKickImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/SBSersic.h` & `GalSim-2.5.1/include/galsim/SBSersic.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/SBSersicImpl.h` & `GalSim-2.5.1/include/galsim/SBSersicImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/SBShapelet.h` & `GalSim-2.5.1/include/galsim/SBShapelet.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/SBShapeletImpl.h` & `GalSim-2.5.1/include/galsim/SBShapeletImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/SBSpergel.h` & `GalSim-2.5.1/include/galsim/SBSpergel.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/SBSpergelImpl.h` & `GalSim-2.5.1/include/galsim/SBSpergelImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/SBTransform.h` & `GalSim-2.5.1/include/galsim/SBTransform.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/SBTransformImpl.h` & `GalSim-2.5.1/include/galsim/SBTransformImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/SBVonKarman.h` & `GalSim-2.5.1/include/galsim/SBVonKarman.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/SBVonKarmanImpl.h` & `GalSim-2.5.1/include/galsim/SBVonKarmanImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/Silicon.h` & `GalSim-2.5.1/include/galsim/Silicon.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/Solve.h` & `GalSim-2.5.1/include/galsim/Solve.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/Std.h` & `GalSim-2.5.1/include/galsim/Std.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/Stopwatch.h` & `GalSim-2.5.1/include/galsim/Stopwatch.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/Table.h` & `GalSim-2.5.1/include/galsim/Table.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/Version.h` & `GalSim-2.5.1/include/galsim/Version.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 // This file is auto-generated by setup.py.  Do not edit.
 #define GALSIM_MAJOR 2
 #define GALSIM_MINOR 5
-#define GALSIM_REVISION 0
+#define GALSIM_REVISION 1
 
 #include <string>
 #include <sstream>
 
 #if defined(__GNUC__)
 #define PUBLIC_API __attribute__ ((visibility ("default")))
 #else
```

### Comparing `GalSim-2.5.0/include/galsim/WCS.h` & `GalSim-2.5.1/include/galsim/WCS.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/boost1_48_0/LICENSE_1_0.txt` & `GalSim-2.5.1/include/galsim/boost1_48_0/LICENSE_1_0.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/boost1_48_0/README` & `GalSim-2.5.1/include/galsim/boost1_48_0/README`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/boost1_48_0/assert.hpp` & `GalSim-2.5.1/include/galsim/boost1_48_0/assert.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/boost1_48_0/config/suffix.hpp` & `GalSim-2.5.1/include/galsim/boost1_48_0/config/suffix.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/boost1_48_0/current_function.hpp` & `GalSim-2.5.1/include/galsim/boost1_48_0/current_function.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/boost1_48_0/random/binomial_distribution.hpp` & `GalSim-2.5.1/include/galsim/boost1_48_0/random/binomial_distribution.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/boost1_48_0/random/chi_squared_distribution.hpp` & `GalSim-2.5.1/include/galsim/boost1_48_0/random/chi_squared_distribution.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/boost1_48_0/random/detail/generator_seed_seq.hpp` & `GalSim-2.5.1/include/galsim/boost1_48_0/random/detail/generator_seed_seq.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/boost1_48_0/random/detail/ptr_helper.hpp` & `GalSim-2.5.1/include/galsim/boost1_48_0/random/detail/ptr_helper.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/boost1_48_0/random/detail/seed.hpp` & `GalSim-2.5.1/include/galsim/boost1_48_0/random/detail/seed.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/boost1_48_0/random/detail/signed_unsigned_tools.hpp` & `GalSim-2.5.1/include/galsim/boost1_48_0/random/detail/signed_unsigned_tools.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/boost1_48_0/random/exponential_distribution.hpp` & `GalSim-2.5.1/include/galsim/boost1_48_0/random/exponential_distribution.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/boost1_48_0/random/gamma_distribution.hpp` & `GalSim-2.5.1/include/galsim/boost1_48_0/random/gamma_distribution.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/boost1_48_0/random/mersenne_twister.hpp` & `GalSim-2.5.1/include/galsim/boost1_48_0/random/mersenne_twister.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/boost1_48_0/random/normal_distribution.hpp` & `GalSim-2.5.1/include/galsim/boost1_48_0/random/normal_distribution.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/boost1_48_0/random/poisson_distribution.hpp` & `GalSim-2.5.1/include/galsim/boost1_48_0/random/poisson_distribution.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/boost1_48_0/random/uniform_01.hpp` & `GalSim-2.5.1/include/galsim/boost1_48_0/random/uniform_01.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/boost1_48_0/random/uniform_real_distribution.hpp` & `GalSim-2.5.1/include/galsim/boost1_48_0/random/uniform_real_distribution.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/boost1_48_0/random/weibull_distribution.hpp` & `GalSim-2.5.1/include/galsim/boost1_48_0/random/weibull_distribution.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/fmath/Makefile` & `GalSim-2.5.1/include/galsim/fmath/Makefile`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/fmath/avx2.cpp` & `GalSim-2.5.1/include/galsim/fmath/avx2.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/fmath/bench.cpp` & `GalSim-2.5.1/include/galsim/fmath/bench.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/fmath/bench.sln` & `GalSim-2.5.1/include/galsim/fmath/bench.sln`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/fmath/bench.vcproj` & `GalSim-2.5.1/include/galsim/fmath/bench.vcproj`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/fmath/ck.cpp` & `GalSim-2.5.1/include/galsim/fmath/ck.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/fmath/fastexp.cpp` & `GalSim-2.5.1/include/galsim/fmath/fastexp.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/fmath/fmath.hpp` & `GalSim-2.5.1/include/galsim/fmath/fmath.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/fmath/include/cybozu/benchmark.hpp` & `GalSim-2.5.1/include/galsim/fmath/include/cybozu/benchmark.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/fmath/include/cybozu/inttype.hpp` & `GalSim-2.5.1/include/galsim/fmath/include/cybozu/inttype.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/fmath/readme.md` & `GalSim-2.5.1/include/galsim/fmath/readme.md`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/fmath/readme.txt` & `GalSim-2.5.1/include/galsim/fmath/readme.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/hsm/PSFCorr.h` & `GalSim-2.5.1/include/galsim/hsm/PSFCorr.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/integ/Int.h` & `GalSim-2.5.1/include/galsim/integ/Int.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/integ/IntGKPData1.h` & `GalSim-2.5.1/include/galsim/integ/IntGKPData1.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/integ/IntGKPData10.h` & `GalSim-2.5.1/include/galsim/integ/IntGKPData10.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/integ/MoreFunctional.h` & `GalSim-2.5.1/include/galsim/integ/MoreFunctional.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/math/Angle.h` & `GalSim-2.5.1/include/galsim/math/Angle.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/math/Bessel.h` & `GalSim-2.5.1/include/galsim/math/Bessel.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/math/Gamma.h` & `GalSim-2.5.1/include/galsim/math/Gamma.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/math/Hankel.h` & `GalSim-2.5.1/include/galsim/math/Hankel.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/math/Horner.h` & `GalSim-2.5.1/include/galsim/math/Horner.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/math/Nan.h` & `GalSim-2.5.1/include/galsim/math/Nan.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/math/Sinc.h` & `GalSim-2.5.1/include/galsim/math/Sinc.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/include/galsim/mmgr.h` & `GalSim-2.5.1/include/galsim/mmgr.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/pysrc/Bessel.cpp` & `GalSim-2.5.1/pysrc/Bessel.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/pysrc/Bounds.cpp` & `GalSim-2.5.1/pysrc/Bounds.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/pysrc/CDModel.cpp` & `GalSim-2.5.1/pysrc/CDModel.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/pysrc/HSM.cpp` & `GalSim-2.5.1/pysrc/HSM.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/pysrc/Horner.cpp` & `GalSim-2.5.1/pysrc/Horner.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/pysrc/Image.cpp` & `GalSim-2.5.1/pysrc/Image.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/pysrc/Integ.cpp` & `GalSim-2.5.1/pysrc/Integ.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/pysrc/Interpolant.cpp` & `GalSim-2.5.1/pysrc/Interpolant.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/pysrc/PhotonArray.cpp` & `GalSim-2.5.1/pysrc/PhotonArray.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/pysrc/PyBind11Helper.h` & `GalSim-2.5.1/pysrc/PyBind11Helper.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/pysrc/Random.cpp` & `GalSim-2.5.1/pysrc/Random.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/pysrc/RealGalaxy.cpp` & `GalSim-2.5.1/pysrc/RealGalaxy.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/pysrc/SBAdd.cpp` & `GalSim-2.5.1/pysrc/SBAdd.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/pysrc/SBAiry.cpp` & `GalSim-2.5.1/pysrc/SBAiry.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/pysrc/SBBox.cpp` & `GalSim-2.5.1/pysrc/SBBox.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/pysrc/SBConvolve.cpp` & `GalSim-2.5.1/pysrc/SBConvolve.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/pysrc/SBDeconvolve.cpp` & `GalSim-2.5.1/pysrc/SBDeconvolve.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/pysrc/SBDeltaFunction.cpp` & `GalSim-2.5.1/pysrc/SBDeltaFunction.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/pysrc/SBExponential.cpp` & `GalSim-2.5.1/pysrc/SBExponential.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/pysrc/SBFourierSqrt.cpp` & `GalSim-2.5.1/pysrc/SBFourierSqrt.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/pysrc/SBGaussian.cpp` & `GalSim-2.5.1/pysrc/SBGaussian.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/pysrc/SBInclinedExponential.cpp` & `GalSim-2.5.1/pysrc/SBInclinedExponential.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/pysrc/SBInclinedSersic.cpp` & `GalSim-2.5.1/pysrc/SBInclinedSersic.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/pysrc/SBInterpolatedImage.cpp` & `GalSim-2.5.1/pysrc/SBInterpolatedImage.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/pysrc/SBKolmogorov.cpp` & `GalSim-2.5.1/pysrc/SBKolmogorov.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/pysrc/SBMoffat.cpp` & `GalSim-2.5.1/pysrc/SBMoffat.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/pysrc/SBProfile.cpp` & `GalSim-2.5.1/pysrc/SBProfile.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/pysrc/SBSecondKick.cpp` & `GalSim-2.5.1/pysrc/SBSecondKick.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/pysrc/SBSersic.cpp` & `GalSim-2.5.1/pysrc/SBSersic.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/pysrc/SBShapelet.cpp` & `GalSim-2.5.1/pysrc/SBShapelet.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/pysrc/SBSpergel.cpp` & `GalSim-2.5.1/pysrc/SBSpergel.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/pysrc/SBTransform.cpp` & `GalSim-2.5.1/pysrc/SBTransform.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/pysrc/SBVonKarman.cpp` & `GalSim-2.5.1/pysrc/SBVonKarman.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/pysrc/Silicon.cpp` & `GalSim-2.5.1/pysrc/Silicon.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/pysrc/Table.cpp` & `GalSim-2.5.1/pysrc/Table.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/pysrc/Utilities.cpp` & `GalSim-2.5.1/pysrc/Utilities.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/pysrc/WCS.cpp` & `GalSim-2.5.1/pysrc/WCS.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/pysrc/module.cpp` & `GalSim-2.5.1/pysrc/module.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/setup.py` & `GalSim-2.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/SEDs/CWW_E_ext.sed` & `GalSim-2.5.1/share/SEDs/CWW_E_ext.sed`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/SEDs/CWW_E_ext_more.sed` & `GalSim-2.5.1/share/SEDs/CWW_E_ext_more.sed`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/SEDs/CWW_Im_ext.sed` & `GalSim-2.5.1/share/SEDs/CWW_Im_ext.sed`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/SEDs/CWW_Im_ext_more.sed` & `GalSim-2.5.1/share/SEDs/CWW_Im_ext_more.sed`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/SEDs/CWW_Sbc_ext.sed` & `GalSim-2.5.1/share/SEDs/CWW_Sbc_ext.sed`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/SEDs/CWW_Sbc_ext_more.sed` & `GalSim-2.5.1/share/SEDs/CWW_Sbc_ext_more.sed`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/SEDs/CWW_Scd_ext.sed` & `GalSim-2.5.1/share/SEDs/CWW_Scd_ext.sed`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/SEDs/CWW_Scd_ext_more.sed` & `GalSim-2.5.1/share/SEDs/CWW_Scd_ext_more.sed`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/SEDs/vega.txt` & `GalSim-2.5.1/share/SEDs/vega.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/acs_I_unrot_sci_20_cf.fits` & `GalSim-2.5.1/share/acs_I_unrot_sci_20_cf.fits`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/bandpasses/ACS_wfc_F435W.dat` & `GalSim-2.5.1/share/bandpasses/ACS_wfc_F435W.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/bandpasses/ACS_wfc_F606W.dat` & `GalSim-2.5.1/share/bandpasses/ACS_wfc_F606W.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/bandpasses/ACS_wfc_F775W.dat` & `GalSim-2.5.1/share/bandpasses/ACS_wfc_F775W.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/bandpasses/ACS_wfc_F814W.dat` & `GalSim-2.5.1/share/bandpasses/ACS_wfc_F814W.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/bandpasses/ACS_wfc_F850LP.dat` & `GalSim-2.5.1/share/bandpasses/ACS_wfc_F850LP.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/bandpasses/LSST_g.dat` & `GalSim-2.5.1/share/bandpasses/LSST_g.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/bandpasses/LSST_i.dat` & `GalSim-2.5.1/share/bandpasses/LSST_i.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/bandpasses/LSST_r.dat` & `GalSim-2.5.1/share/bandpasses/LSST_r.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/bandpasses/LSST_u.dat` & `GalSim-2.5.1/share/bandpasses/LSST_u.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/bandpasses/LSST_y.dat` & `GalSim-2.5.1/share/bandpasses/LSST_y.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/bandpasses/LSST_z.dat` & `GalSim-2.5.1/share/bandpasses/LSST_z.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/bandpasses/WFC3_ir_F105W.dat` & `GalSim-2.5.1/share/bandpasses/WFC3_ir_F105W.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/bandpasses/WFC3_ir_F125W.dat` & `GalSim-2.5.1/share/bandpasses/WFC3_ir_F125W.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/bandpasses/WFC3_ir_F160W.dat` & `GalSim-2.5.1/share/bandpasses/WFC3_ir_F160W.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/bandpasses/WFC3_uvis_F275W.dat` & `GalSim-2.5.1/share/bandpasses/WFC3_uvis_F275W.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/bandpasses/WFC3_uvis_F336W.dat` & `GalSim-2.5.1/share/bandpasses/WFC3_uvis_F336W.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/roman/RST_WIM_Filter_F184_SCA_1.fits.gz` & `GalSim-2.5.1/share/roman/RST_WIM_Filter_F184_SCA_1.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/roman/RST_WIM_Filter_F184_SCA_10.fits.gz` & `GalSim-2.5.1/share/roman/RST_WIM_Filter_F184_SCA_10.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/roman/RST_WIM_Filter_F184_SCA_11.fits.gz` & `GalSim-2.5.1/share/roman/RST_WIM_Filter_F184_SCA_11.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/roman/RST_WIM_Filter_F184_SCA_12.fits.gz` & `GalSim-2.5.1/share/roman/RST_WIM_Filter_F184_SCA_12.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/roman/RST_WIM_Filter_F184_SCA_13.fits.gz` & `GalSim-2.5.1/share/roman/RST_WIM_Filter_F184_SCA_13.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/roman/RST_WIM_Filter_F184_SCA_14.fits.gz` & `GalSim-2.5.1/share/roman/RST_WIM_Filter_F184_SCA_14.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/roman/RST_WIM_Filter_F184_SCA_15.fits.gz` & `GalSim-2.5.1/share/roman/RST_WIM_Filter_F184_SCA_15.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/roman/RST_WIM_Filter_F184_SCA_16.fits.gz` & `GalSim-2.5.1/share/roman/RST_WIM_Filter_F184_SCA_16.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/roman/RST_WIM_Filter_F184_SCA_17.fits.gz` & `GalSim-2.5.1/share/roman/RST_WIM_Filter_F184_SCA_17.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/roman/RST_WIM_Filter_F184_SCA_18.fits.gz` & `GalSim-2.5.1/share/roman/RST_WIM_Filter_F184_SCA_18.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/roman/RST_WIM_Filter_F184_SCA_2.fits.gz` & `GalSim-2.5.1/share/roman/RST_WIM_Filter_F184_SCA_2.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/roman/RST_WIM_Filter_F184_SCA_3.fits.gz` & `GalSim-2.5.1/share/roman/RST_WIM_Filter_F184_SCA_3.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/roman/RST_WIM_Filter_F184_SCA_4.fits.gz` & `GalSim-2.5.1/share/roman/RST_WIM_Filter_F184_SCA_4.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/roman/RST_WIM_Filter_F184_SCA_5.fits.gz` & `GalSim-2.5.1/share/roman/RST_WIM_Filter_F184_SCA_5.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/roman/RST_WIM_Filter_F184_SCA_6.fits.gz` & `GalSim-2.5.1/share/roman/RST_WIM_Filter_F184_SCA_6.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/roman/RST_WIM_Filter_F184_SCA_7.fits.gz` & `GalSim-2.5.1/share/roman/RST_WIM_Filter_F184_SCA_7.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/roman/RST_WIM_Filter_F184_SCA_8.fits.gz` & `GalSim-2.5.1/share/roman/RST_WIM_Filter_F184_SCA_8.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/roman/RST_WIM_Filter_F184_SCA_9.fits.gz` & `GalSim-2.5.1/share/roman/RST_WIM_Filter_F184_SCA_9.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/roman/RST_WIM_Filter_skinny_SCA_1.fits.gz` & `GalSim-2.5.1/share/roman/RST_WIM_Filter_skinny_SCA_1.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/roman/RST_WIM_Filter_skinny_SCA_10.fits.gz` & `GalSim-2.5.1/share/roman/RST_WIM_Filter_skinny_SCA_10.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/roman/RST_WIM_Filter_skinny_SCA_11.fits.gz` & `GalSim-2.5.1/share/roman/RST_WIM_Filter_skinny_SCA_11.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/roman/RST_WIM_Filter_skinny_SCA_12.fits.gz` & `GalSim-2.5.1/share/roman/RST_WIM_Filter_skinny_SCA_12.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/roman/RST_WIM_Filter_skinny_SCA_13.fits.gz` & `GalSim-2.5.1/share/roman/RST_WIM_Filter_skinny_SCA_13.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/roman/RST_WIM_Filter_skinny_SCA_14.fits.gz` & `GalSim-2.5.1/share/roman/RST_WIM_Filter_skinny_SCA_14.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/roman/RST_WIM_Filter_skinny_SCA_15.fits.gz` & `GalSim-2.5.1/share/roman/RST_WIM_Filter_skinny_SCA_15.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/roman/RST_WIM_Filter_skinny_SCA_16.fits.gz` & `GalSim-2.5.1/share/roman/RST_WIM_Filter_skinny_SCA_16.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/roman/RST_WIM_Filter_skinny_SCA_17.fits.gz` & `GalSim-2.5.1/share/roman/RST_WIM_Filter_skinny_SCA_17.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/roman/RST_WIM_Filter_skinny_SCA_18.fits.gz` & `GalSim-2.5.1/share/roman/RST_WIM_Filter_skinny_SCA_18.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/roman/RST_WIM_Filter_skinny_SCA_2.fits.gz` & `GalSim-2.5.1/share/roman/RST_WIM_Filter_skinny_SCA_2.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/roman/RST_WIM_Filter_skinny_SCA_3.fits.gz` & `GalSim-2.5.1/share/roman/RST_WIM_Filter_skinny_SCA_3.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/roman/RST_WIM_Filter_skinny_SCA_4.fits.gz` & `GalSim-2.5.1/share/roman/RST_WIM_Filter_skinny_SCA_4.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/roman/RST_WIM_Filter_skinny_SCA_5.fits.gz` & `GalSim-2.5.1/share/roman/RST_WIM_Filter_skinny_SCA_5.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/roman/RST_WIM_Filter_skinny_SCA_6.fits.gz` & `GalSim-2.5.1/share/roman/RST_WIM_Filter_skinny_SCA_6.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/roman/RST_WIM_Filter_skinny_SCA_7.fits.gz` & `GalSim-2.5.1/share/roman/RST_WIM_Filter_skinny_SCA_7.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/roman/RST_WIM_Filter_skinny_SCA_8.fits.gz` & `GalSim-2.5.1/share/roman/RST_WIM_Filter_skinny_SCA_8.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/roman/RST_WIM_Filter_skinny_SCA_9.fits.gz` & `GalSim-2.5.1/share/roman/RST_WIM_Filter_skinny_SCA_9.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_01.txt` & `GalSim-2.5.1/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_01.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_02.txt` & `GalSim-2.5.1/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_02.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_03.txt` & `GalSim-2.5.1/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_03.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_04.txt` & `GalSim-2.5.1/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_04.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_05.txt` & `GalSim-2.5.1/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_05.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_06.txt` & `GalSim-2.5.1/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_06.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_07.txt` & `GalSim-2.5.1/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_07.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_08.txt` & `GalSim-2.5.1/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_08.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_09.txt` & `GalSim-2.5.1/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_09.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_10.txt` & `GalSim-2.5.1/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_10.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_11.txt` & `GalSim-2.5.1/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_11.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_12.txt` & `GalSim-2.5.1/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_12.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_13.txt` & `GalSim-2.5.1/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_13.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_14.txt` & `GalSim-2.5.1/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_14.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_15.txt` & `GalSim-2.5.1/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_15.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_16.txt` & `GalSim-2.5.1/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_16.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_17.txt` & `GalSim-2.5.1/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_17.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_18.txt` & `GalSim-2.5.1/share/roman/Roman_Cycle-9_WFI_zim_zernikes_082623_18.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/roman/Roman_SRR_WFC_Pupil_Mask_Longwave_2048_reformatted.fits.gz` & `GalSim-2.5.1/share/roman/Roman_SRR_WFC_Pupil_Mask_Longwave_2048_reformatted.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/roman/Roman_SRR_WFC_Pupil_Mask_Shortwave_2048_reformatted.fits.gz` & `GalSim-2.5.1/share/roman/Roman_SRR_WFC_Pupil_Mask_Shortwave_2048_reformatted.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/roman/Roman_effarea_20210614.txt` & `GalSim-2.5.1/share/roman/Roman_effarea_20210614.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/roman/roman_sky_backgrounds.txt` & `GalSim-2.5.1/share/roman/roman_sky_backgrounds.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/roman/sca_positions_20210204.txt` & `GalSim-2.5.1/share/roman/sca_positions_20210204.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/roman/sip_20210204.txt` & `GalSim-2.5.1/share/roman/sip_20210204.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/sensors/abs_length.dat` & `GalSim-2.5.1/share/sensors/abs_length.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/sensors/lsst_e2v_32.cfg` & `GalSim-2.5.1/share/sensors/lsst_e2v_32.cfg`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/sensors/lsst_e2v_32.dat` & `GalSim-2.5.1/share/sensors/lsst_e2v_32.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/sensors/lsst_e2v_50_32.cfg` & `GalSim-2.5.1/share/sensors/lsst_e2v_50_32.cfg`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/sensors/lsst_e2v_50_32.dat` & `GalSim-2.5.1/share/sensors/lsst_e2v_50_32.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/sensors/lsst_e2v_50_8.cfg` & `GalSim-2.5.1/share/sensors/lsst_e2v_50_8.cfg`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/sensors/lsst_e2v_50_8.dat` & `GalSim-2.5.1/share/sensors/lsst_e2v_50_8.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/sensors/lsst_e2v_8.cfg` & `GalSim-2.5.1/share/sensors/lsst_e2v_8.cfg`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/sensors/lsst_e2v_8.dat` & `GalSim-2.5.1/share/sensors/lsst_e2v_8.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/sensors/lsst_itl_32.cfg` & `GalSim-2.5.1/share/sensors/lsst_itl_32.cfg`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/sensors/lsst_itl_32.dat` & `GalSim-2.5.1/share/sensors/lsst_itl_32.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/sensors/lsst_itl_50_32.cfg` & `GalSim-2.5.1/share/sensors/lsst_itl_50_32.cfg`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/sensors/lsst_itl_50_32.dat` & `GalSim-2.5.1/share/sensors/lsst_itl_50_32.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/sensors/lsst_itl_50_8.cfg` & `GalSim-2.5.1/share/sensors/lsst_itl_50_8.cfg`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/sensors/lsst_itl_50_8.dat` & `GalSim-2.5.1/share/sensors/lsst_itl_50_8.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/sensors/lsst_itl_8.cfg` & `GalSim-2.5.1/share/sensors/lsst_itl_8.cfg`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/sensors/lsst_itl_8.dat` & `GalSim-2.5.1/share/sensors/lsst_itl_8.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/share/wfc_F814W.dat.gz` & `GalSim-2.5.1/share/wfc_F814W.dat.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/src/BinomFact.cpp` & `GalSim-2.5.1/src/BinomFact.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/src/CDModel.cpp` & `GalSim-2.5.1/src/CDModel.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/src/CorrelatedNoise.cpp` & `GalSim-2.5.1/src/CorrelatedNoise.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/src/GSParams.cpp` & `GalSim-2.5.1/src/GSParams.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/src/Image.cpp` & `GalSim-2.5.1/src/Image.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/src/Image.inst` & `GalSim-2.5.1/src/Image.inst`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/src/Interpolant.cpp` & `GalSim-2.5.1/src/Interpolant.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/src/Laguerre.cpp` & `GalSim-2.5.1/src/Laguerre.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/src/OneDimensionalDeviate.cpp` & `GalSim-2.5.1/src/OneDimensionalDeviate.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/src/PhotonArray.cpp` & `GalSim-2.5.1/src/PhotonArray.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/src/Polygon.cpp` & `GalSim-2.5.1/src/Polygon.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/src/Random.cpp` & `GalSim-2.5.1/src/Random.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/src/RealGalaxy.cpp` & `GalSim-2.5.1/src/RealGalaxy.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/src/RealSpaceConvolve.cpp` & `GalSim-2.5.1/src/RealSpaceConvolve.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/src/SBAdd.cpp` & `GalSim-2.5.1/src/SBAdd.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/src/SBAiry.cpp` & `GalSim-2.5.1/src/SBAiry.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/src/SBBox.cpp` & `GalSim-2.5.1/src/SBBox.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/src/SBConvolve.cpp` & `GalSim-2.5.1/src/SBConvolve.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/src/SBDeconvolve.cpp` & `GalSim-2.5.1/src/SBDeconvolve.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/src/SBDeltaFunction.cpp` & `GalSim-2.5.1/src/SBDeltaFunction.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/src/SBExponential.cpp` & `GalSim-2.5.1/src/SBExponential.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/src/SBFourierSqrt.cpp` & `GalSim-2.5.1/src/SBFourierSqrt.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/src/SBGaussian.cpp` & `GalSim-2.5.1/src/SBGaussian.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/src/SBInclinedExponential.cpp` & `GalSim-2.5.1/src/SBInclinedExponential.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/src/SBInclinedSersic.cpp` & `GalSim-2.5.1/src/SBInclinedSersic.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/src/SBInterpolatedImage.cpp` & `GalSim-2.5.1/src/SBInterpolatedImage.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/src/SBKolmogorov.cpp` & `GalSim-2.5.1/src/SBKolmogorov.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/src/SBMoffat.cpp` & `GalSim-2.5.1/src/SBMoffat.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/src/SBProfile.cpp` & `GalSim-2.5.1/src/SBProfile.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/src/SBSecondKick.cpp` & `GalSim-2.5.1/src/SBSecondKick.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/src/SBSersic.cpp` & `GalSim-2.5.1/src/SBSersic.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/src/SBShapelet.cpp` & `GalSim-2.5.1/src/SBShapelet.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/src/SBSpergel.cpp` & `GalSim-2.5.1/src/SBSpergel.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/src/SBTransform.cpp` & `GalSim-2.5.1/src/SBTransform.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/src/SBVonKarman.cpp` & `GalSim-2.5.1/src/SBVonKarman.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/src/Silicon.cpp` & `GalSim-2.5.1/src/Silicon.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -538,25 +538,24 @@
     }
 
     // This version of calculateTreeRingDistortion only distorts a polygon.
     // Used in the no-flux pixel area calculation.
     void Silicon::calculateTreeRingDistortion(int i, int j, Position<int> orig_center,
                                               Polygon& poly) const
     {
-        double shift = 0.0;
         for (int n=0; n<_nv; n++) {
             xdbg<<"i,j,n = "<<i<<','<<j<<','<<n<<": x,y = "<<
                 poly[n].x <<"  "<< poly[n].y<<std::endl;
             double tx = (double)i + poly[n].x - _treeRingCenter.x + (double)orig_center.x;
             double ty = (double)j + poly[n].y - _treeRingCenter.y + (double)orig_center.y;
             xdbg<<"tx,ty = "<<tx<<','<<ty<<std::endl;
             double r = sqrt(tx * tx + ty * ty);
-            shift = _tr_radial_table.lookup(r);
-            xdbg<<"r = "<<r<<", shift = "<<shift<<std::endl;
-            if (r > 0) {
+            if (r > 0 && r < _tr_radial_table.argMax()) {
+                double shift = _tr_radial_table.lookup(r);
+                xdbg<<"r = "<<r<<", shift = "<<shift<<std::endl;
                 // Shifts are along the radial vector in direction of the doping gradient
                 double dx = shift * tx / r;
                 double dy = shift * ty / r;
                 xdbg<<"dx,dy = "<<dx<<','<<dy<<std::endl;
                 poly[n].x = double(poly[n].x) + dx;
                 poly[n].y = double(poly[n].y) + dy;
                 xdbg<<"    x,y => "<<poly[n].x <<"  "<< poly[n].y;
@@ -564,40 +563,42 @@
         }
     }
 
     // This version updates the linear boundary
     void Silicon::calculateTreeRingDistortion(int i, int j, Position<int> orig_center,
                                               int nx, int ny, int i1, int j1)
     {
-        iteratePixelBoundary(i - i1, j - j1, nx, ny, [&](int n, Position<float>& pt, bool rhs, bool top) {
-                             Position<double> p = pt;
-
-                             // only do bottom and left points unless we're on top/right edge
-                             if ((rhs) && ((i - i1) < (nx - 1))) return;
-                             if ((top) && ((j - j1) < (ny - 1))) return;
-
-                             if (rhs) p.x += 1.0;
-                             if (top) p.y += 1.0;
-                             //xdbg<<"x,y = "<<p.x<<','<<p.y<<std::endl;
-
-                             double tx = (double)i + p.x - _treeRingCenter.x + (double)orig_center.x;
-                             double ty = (double)j + p.y - _treeRingCenter.y + (double)orig_center.y;
-                             //xdbg<<"tx,ty = "<<tx<<','<<ty<<std::endl;
-                             double r = sqrt(tx * tx + ty * ty);
-                             if (r > 0) {
-                                double shift = _tr_radial_table.lookup(r);
-                                //xdbg<<"r = "<<r<<", shift = "<<shift<<std::endl;
-                                // Shifts are along the radial vector in direction of the doping gradient
-                                double dx = shift * tx / r;
-                                double dy = shift * ty / r;
-                                //xdbg<<"dx,dy = "<<dx<<','<<dy<<std::endl;
-                                pt.x += dx;
-                                pt.y += dy;
-                             }
-        });
+        iteratePixelBoundary(
+            i-i1, j-j1, nx, ny, [&](int n, Position<float>& pt, bool rhs, bool top) {
+                Position<double> p = pt;
+
+                // only do bottom and left points unless we're on top/right edge
+                if ((rhs) && ((i - i1) < (nx - 1))) return;
+                if ((top) && ((j - j1) < (ny - 1))) return;
+
+                if (rhs) p.x += 1.0;
+                if (top) p.y += 1.0;
+                //xdbg<<"x,y = "<<p.x<<','<<p.y<<std::endl;
+
+                double tx = (double)i + p.x - _treeRingCenter.x + (double)orig_center.x;
+                double ty = (double)j + p.y - _treeRingCenter.y + (double)orig_center.y;
+                //xdbg<<"tx,ty = "<<tx<<','<<ty<<std::endl;
+                double r = sqrt(tx * tx + ty * ty);
+                if (r > 0 && r < _tr_radial_table.argMax()) {
+                    double shift = _tr_radial_table.lookup(r);
+                    //xdbg<<"r = "<<r<<", shift = "<<shift<<std::endl;
+                    // Shifts are along the radial vector in direction of the doping gradient
+                    double dx = shift * tx / r;
+                    double dy = shift * ty / r;
+                    //xdbg<<"dx,dy = "<<dx<<','<<dy<<std::endl;
+                    pt.x += dx;
+                    pt.y += dy;
+                }
+            }
+        );
     }
 
     template <typename T>
     void Silicon::addTreeRingDistortions(ImageView<T> target, Position<int> orig_center)
     {
         if (_tr_radial_table.size() == 2) {
             //dbg<<"Trivial radial table\n";
@@ -641,21 +642,24 @@
     // Scales a linear pixel boundary into a polygon object.
     void Silicon::scaleBoundsToPoly(int i, int j, int nx, int ny,
                                     const Polygon& emptypoly, Polygon& result,
                                     double factor) const
     {
         result = emptypoly;
 
-        iteratePixelBoundary(i, j, nx, ny, [&](int n, const Position<float>& pt, bool rhs, bool top) {
-                             Position<double> p = pt;
-                             if (rhs) p.x += 1.0;
-                             if (top) p.y += 1.0;
-                             result[n].x += (p.x - emptypoly[n].x) * factor;
-                             result[n].y += (p.y - emptypoly[n].y) * factor;
-                             });
+        iteratePixelBoundary(
+            i, j, nx, ny,
+            [&](int n, const Position<float>& pt, bool rhs, bool top) {
+                Position<double> p = pt;
+                if (rhs) p.x += 1.0;
+                if (top) p.y += 1.0;
+                result[n].x += (p.x - emptypoly[n].x) * factor;
+                result[n].y += (p.y - emptypoly[n].y) * factor;
+            }
+        );
 
         result.updateBounds();
     }
 
     bool Silicon::insidePixel(int ix, int iy, double x, double y, double zconv,
                               Bounds<int>& targetBounds, bool* off_edge,
                               int emptypolySize,
```

### Comparing `GalSim-2.5.0/src/Table.cpp` & `GalSim-2.5.1/src/Table.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/src/Version.cpp` & `GalSim-2.5.1/src/Version.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/src/WCS.cpp` & `GalSim-2.5.1/src/WCS.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/src/hsm/PSFCorr.cpp` & `GalSim-2.5.1/src/hsm/PSFCorr.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/src/math/Angle.cpp` & `GalSim-2.5.1/src/math/Angle.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/src/math/Bessel.cpp` & `GalSim-2.5.1/src/math/Bessel.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/src/math/BesselI.cpp` & `GalSim-2.5.1/src/math/BesselI.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/src/math/BesselJ.cpp` & `GalSim-2.5.1/src/math/BesselJ.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/src/math/BesselK.cpp` & `GalSim-2.5.1/src/math/BesselK.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/src/math/BesselRoots.cpp` & `GalSim-2.5.1/src/math/BesselRoots.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/src/math/BesselY.cpp` & `GalSim-2.5.1/src/math/BesselY.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/src/math/Gamma.cpp` & `GalSim-2.5.1/src/math/Gamma.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/src/math/Hankel.cpp` & `GalSim-2.5.1/src/math/Hankel.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/src/math/Horner.cpp` & `GalSim-2.5.1/src/math/Horner.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/src/math/Nan.cpp` & `GalSim-2.5.1/src/math/Nan.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/src/math/Sinc.cpp` & `GalSim-2.5.1/src/math/Sinc.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/src/mmgr.cpp` & `GalSim-2.5.1/src/mmgr.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/tests/test_airy.py` & `GalSim-2.5.1/tests/test_airy.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/tests/test_bandpass.py` & `GalSim-2.5.1/tests/test_bandpass.py`

 * *Files 0% similar despite different names*

```diff
@@ -265,14 +265,20 @@
                                    err_msg="Bandpass.red_limit doesn't respect wave_type")
     np.testing.assert_approx_equal(a0.blue_limit, a1.blue_limit*10,
                                    err_msg="Bandpass.blue_limit doesn't respect wave_type")
     np.testing.assert_approx_equal(a0.effective_wavelength, a1.effective_wavelength*10,
                                    err_msg="Bandpass.effective_wavelength doesn't respect"
                                            +" wave_type")
 
+    # Spline interpolation changes the effective wavelength slightly, but not much.
+    a2 = galsim.Bandpass('LSST_r.dat', wave_type='nm', interpolant='spline')
+    np.testing.assert_equal(a2.red_limit, a0.red_limit)
+    np.testing.assert_equal(a2.blue_limit, a0.blue_limit)
+    np.testing.assert_allclose(a2.effective_wavelength, a0.effective_wavelength, rtol=1.e-3)
+
     b0 = galsim.Bandpass(galsim.LookupTable([1,2,3,4,5], [1,2,3,4,5]), wave_type='nm')
     b1 = galsim.Bandpass(galsim.LookupTable([10,20,30,40,50], [1,2,3,4,5]), wave_type='ang')
     np.testing.assert_approx_equal(b0.red_limit, b1.red_limit,
                                    err_msg="Bandpass.red_limit doesn't respect wave_type")
     np.testing.assert_approx_equal(b0.blue_limit, b1.blue_limit,
                                    err_msg="Bandpass.blue_limit doesn't respect wave_type")
     np.testing.assert_approx_equal(b0.effective_wavelength, b1.effective_wavelength,
@@ -309,36 +315,40 @@
            galsim.Bandpass(throughput=lt, wave_type='nm').withZeropoint(None)
 
 
 @timer
 def test_thin():
     """Test that bandpass thinning works with the requested accuracy."""
     s = galsim.SED('1', wave_type='nm', flux_type='fphotons')
-    bp = galsim.Bandpass(os.path.join(datapath, 'LSST_r.dat'), 'nm')
-    flux = s.calculateFlux(bp)
-    print("Original number of bandpass samples = ",len(bp.wave_list))
-    for err in [1.e-2, 1.e-3, 1.e-4, 1.e-5]:
-        print("Test err = ",err)
-        thin_bp = bp.thin(rel_err=err, preserve_range=True, fast_search=False)
-        thin_flux = s.calculateFlux(thin_bp)
-        thin_err = (flux-thin_flux)/flux
-        print("num samples with preserve_range = True, fast_search = False: ",len(thin_bp.wave_list))
-        print("realized error = ",(flux-thin_flux)/flux)
-        thin_bp = bp.thin(rel_err=err, preserve_range=True)
-        thin_flux = s.calculateFlux(thin_bp)
-        thin_err = (flux-thin_flux)/flux
-        print("num samples with preserve_range = True: ",len(thin_bp.wave_list))
-        print("realized error = ",(flux-thin_flux)/flux)
-        assert np.abs(thin_err) < err, "Thinned bandpass failed accuracy goal, preserving range."
-        thin_bp = bp.thin(rel_err=err, preserve_range=False)
-        thin_flux = s.calculateFlux(thin_bp)
-        thin_err = (flux-thin_flux)/flux
-        print("num samples with preserve_range = False: ",len(thin_bp.wave_list))
-        print("realized error = ",(flux-thin_flux)/flux)
-        assert np.abs(thin_err) < err, "Thinned bandpass failed accuracy goal, w/ range shrinkage."
+    bp1 = galsim.Bandpass(os.path.join(datapath, 'LSST_r.dat'), 'nm')
+    bp2 = galsim.Bandpass(os.path.join(datapath, 'LSST_r.dat'), 'nm', interpolant='spline')
+
+    for bp in [bp1, bp2]:
+        flux = s.calculateFlux(bp)
+        print("Original number of bandpass samples = ",len(bp.wave_list))
+        for err in [1.e-2, 1.e-3, 1.e-4, 1.e-5]:
+            print("Test err = ",err)
+            thin_bp = bp.thin(rel_err=err, preserve_range=True, fast_search=False)
+            thin_flux = s.calculateFlux(thin_bp)
+            thin_err = (flux-thin_flux)/flux
+            print("num samples with preserve_range = True, fast_search = False: ",
+                  len(thin_bp.wave_list))
+            print("realized error = ",(flux-thin_flux)/flux)
+            thin_bp = bp.thin(rel_err=err, preserve_range=True)
+            thin_flux = s.calculateFlux(thin_bp)
+            thin_err = (flux-thin_flux)/flux
+            print("num samples with preserve_range = True: ",len(thin_bp.wave_list))
+            print("realized error = ",(flux-thin_flux)/flux)
+            assert np.abs(thin_err) < err, "Thinned bandpass failed accuracy goal, preserving range."
+            thin_bp = bp.thin(rel_err=err, preserve_range=False)
+            thin_flux = s.calculateFlux(thin_bp)
+            thin_err = (flux-thin_flux)/flux
+            print("num samples with preserve_range = False: ",len(thin_bp.wave_list))
+            print("realized error = ",(flux-thin_flux)/flux)
+            assert np.abs(thin_err) < err, "Thinned bandpass failed accuracy goal, w/ range shrinkage."
 
 
 @timer
 def test_zp():
     """Check that the zero points are maintained in an appropriate way when thinning, truncating."""
     # Make a bandpass and set an AB zeropoint.
     bp = galsim.Bandpass(os.path.join(datapath, 'LSST_r.dat'), 'nm')
```

### Comparing `GalSim-2.5.0/tests/test_bessel.py` & `GalSim-2.5.1/tests/test_bessel.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/tests/test_box.py` & `GalSim-2.5.1/tests/test_box.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/tests/test_calc.py` & `GalSim-2.5.1/tests/test_calc.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/tests/test_catalog.py` & `GalSim-2.5.1/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/tests/test_cdmodel.py` & `GalSim-2.5.1/tests/test_cdmodel.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/tests/test_celestial.py` & `GalSim-2.5.1/tests/test_celestial.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/tests/test_chromatic.py` & `GalSim-2.5.1/tests/test_chromatic.py`

 * *Files 0% similar despite different names*

```diff
@@ -2222,18 +2222,30 @@
     psf6 = galsim.ChromaticOpticalPSF(lam=bandpass.effective_wavelength, diam=diam,
                                       aberrations=aberrations, obscuration=obscuration,
                                       nstruts=6, geometric_shooting=False)
 
     # 7. InterpolatedChromaticObject
     psf7 = psf6.interpolate(waves=[500, 700, 1000])
 
-    for psf in [psf1, psf2, psf3, psf4, psf5, psf6, psf7]:
+    # 8. ChromaticSum
+    # Most useful as a way to linearly interpolate between two (or more) values, so do that.
+    ab1 = np.array([0,0,0,0, 0.008, -0.005, -0.005, -0.002])
+    ab2 = np.array([0,0,0,0, 0.003, 0.003, -0.007, -0.001])
+    psf8a = galsim.ChromaticOpticalPSF(lam=bandpass.effective_wavelength, diam=diam,
+                                       aberrations=ab1, obscuration=obscuration,
+                                       geometric_shooting=True)
+    psf8b = galsim.ChromaticOpticalPSF(lam=bandpass.effective_wavelength, diam=diam,
+                                       aberrations=ab2, obscuration=obscuration,
+                                       nstruts=6, geometric_shooting=True)
+    psf8 = 0.7 * psf8a + 0.3 * psf8b
+
+    for psf in [psf1, psf2, psf3, psf4, psf5, psf6, psf7, psf8]:
         print('psf = ',psf)
         atol = 4.e-4
-        if psf in [psf5, psf6, psf7]:
+        if psf in [psf5, psf6, psf7, psf8]:
             atol = 6e-4   # OpticalPSF doesn't match quite as well as the others.
         rng = galsim.BaseDeviate(1234)
 
         # First draw with FFT
         obj = galsim.Convolve(gal, psf)
         pixel_scale = 0.01
         im1 = galsim.ImageD(100, 100, scale=pixel_scale)
@@ -2613,15 +2625,15 @@
     check_pickle(chrom)
 
     scaling = galsim.SED(lambda w: w**1.03, 'nm', '1')
     chrom = galsim.Transform(gsobj * bulge_SED, offset=(0.1, 0.3), flux_ratio=scaling)
     assert isinstance(chrom, galsim.ChromaticTransformation)
     assert not isinstance(chrom, galsim.SimpleChromaticTransformation)
     check_chromatic_invariant(chrom)
-    np.testing.assert_allclose(chrom.sed(waves), flux * bulge_SED(waves) * waves**1.03)
+    np.testing.assert_allclose(chrom.sed(waves), flux * bulge_SED(waves) * waves**1.03, rtol=1.e-4)
     # Not picklable, but run str, repr
     str(chrom)
     repr(chrom)
 
     # ChromaticOpticalPSF
     chrom_opt = galsim.ChromaticOpticalPSF(lam=500.0, diam=2.0, tip=2.0, tilt=3.0, defocus=0.2,
                                            scale_unit='arcmin')
@@ -2644,15 +2656,14 @@
     #       unpicklable user input should be picklable.
     #       e.g. autoconv2 has no hope.  But there are a few check_pickle calls that are commented
     #       out that we should probably try to make work.  A job for another day, though...
     #check_pickle(chrom_sum_noSED)
     repr(chrom_sum_noSED)
     str(chrom_sum_noSED)
     assert_raises(galsim.GalSimError, chrom_sum_noSED.applyTo, p1)
-    assert_raises(galsim.GalSimNotImplementedError, chrom_sum_noSED.applyTo, p2)
 
     chrom = gsobj * bulge_SED
     chrom_sum_SED = chrom + chrom  # used to be considered separable, but not anymore.
     check_chromatic_invariant(chrom_sum_SED)
     np.testing.assert_allclose(chrom_sum_SED.sed(waves), 2*flux*bulge_SED(waves))
     check_pickle(chrom_sum_SED)
     assert not chrom_sum_SED.separable
@@ -2661,15 +2672,14 @@
     chrom2 = gsobj2 * disk_SED
     chrom_sum_SED2 = chrom + chrom2
     check_chromatic_invariant(chrom_sum_SED2)
     np.testing.assert_allclose(chrom_sum_SED2.sed(waves), flux*bulge_SED(waves) + disk_SED(waves))
     check_pickle(chrom_sum_SED2)
     assert not chrom_sum_SED2.separable
     assert_raises(galsim.GalSimError, chrom_sum_SED.applyTo, p1)
-    assert_raises(galsim.GalSimNotImplementedError, chrom_sum_SED.applyTo, p2)
 
     # ChromaticConvolution
     conv1 = galsim.Convolve(chrom, chrom_airy)  # SEDed
     check_chromatic_invariant(conv1)
     np.testing.assert_allclose(conv1.sed(waves), flux*bulge_SED(waves))
     check_pickle(conv1)
 
@@ -3195,15 +3205,15 @@
     psf = galsim.ChromaticObject(
         galsim.Gaussian(fwhm=1)
     ).withScaledFlux(lambda w: (w/500)**1.3)
     obj = galsim.Convolve(psf, star).withFlux(flux, bandpass)
     img = obj.drawImage(bandpass, nx=25, ny=25, scale=0.2, method='phot', rng=rng,
                         poisson_flux=False)
     print(img.added_flux)
-    np.testing.assert_allclose(img.added_flux, flux)
+    np.testing.assert_allclose(img.added_flux, flux, rtol=1.e-6)
     img = obj.drawImage(bandpass, nx=25, ny=25, scale=0.2, method='phot', rng=rng)
     print(img.added_flux)
     assert abs(img.added_flux - flux) > 0.1
 
 
 if __name__ == "__main__":
     testfns = [v for k, v in vars().items() if k[:5] == 'test_' and callable(v)]
```

### Comparing `GalSim-2.5.0/tests/test_config_gsobject.py` & `GalSim-2.5.1/tests/test_config_gsobject.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/tests/test_config_image.py` & `GalSim-2.5.1/tests/test_config_image.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/tests/test_config_input.py` & `GalSim-2.5.1/tests/test_config_input.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/tests/test_config_noise.py` & `GalSim-2.5.1/tests/test_config_noise.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/tests/test_config_output.py` & `GalSim-2.5.1/tests/test_config_output.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/tests/test_config_value.py` & `GalSim-2.5.1/tests/test_config_value.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/tests/test_convolve.py` & `GalSim-2.5.1/tests/test_convolve.py`

 * *Files 0% similar despite different names*

```diff
@@ -674,15 +674,15 @@
 
 @timer
 def test_autocorrelate():
     """Test that auto-correlation works the same as convolution with the mirror image of itself.
 
     (See the Signal processing Section of http://en.wikipedia.org/wiki/Autocorrelation)
     """
-    dx = 0.7
+    dx = 0.8
     myImg1 = galsim.ImageF(80,80, scale=dx)
     myImg1.setCenter(0,0)
     myImg2 = galsim.ImageF(80,80, scale=dx)
     myImg2.setCenter(0,0)
 
     # Use a function that is NOT two-fold rotationally symmetric, e.g. two different flux Gaussians
     obj1 = galsim.Gaussian(sigma=3., flux=4).shift(-0.2, -0.4)
```

### Comparing `GalSim-2.5.0/tests/test_correlatednoise.py` & `GalSim-2.5.1/tests/test_correlatednoise.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/tests/test_deltafunction.py` & `GalSim-2.5.1/tests/test_deltafunction.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/tests/test_deprecated.py` & `GalSim-2.5.1/tests/test_deprecated.py`

 * *Files 13% similar despite different names*

```diff
@@ -599,14 +599,46 @@
     v[:] = 10.0
     np.testing.assert_array_equal(photon_array.pupil_u, 0.0)
     np.testing.assert_array_equal(photon_array.pupil_v, 10.0)
     u = photon_array.pupil_u
     u[:] = 6.0
     np.testing.assert_array_equal(photon_array.pupil_u, 6.0)
 
+    # Check assignAt
+    pa1 = galsim.PhotonArray(50)
+    pa1.x = photon_array.x[:50]
+    for i in range(50):
+        pa1.y[i] = photon_array.y[i]
+    pa1.flux[0:50] = photon_array.flux[:50]
+    pa1.dxdz = photon_array.dxdz[:50]
+    pa1.dydz = photon_array.dydz[:50]
+    pa1.pupil_u = photon_array.pupil_u[:50]
+    pa1.pupil_v = photon_array.pupil_v[:50]
+    pa2 = galsim.PhotonArray(100)
+    check_dep(pa2.assignAt, 0, pa1)
+    check_dep(pa2.assignAt, 50, pa1)
+    np.testing.assert_almost_equal(pa2.x[:50], pa1.x)
+    np.testing.assert_almost_equal(pa2.y[:50], pa1.y)
+    np.testing.assert_almost_equal(pa2.flux[:50], pa1.flux)
+    np.testing.assert_almost_equal(pa2.dxdz[:50], pa1.dxdz)
+    np.testing.assert_almost_equal(pa2.dydz[:50], pa1.dydz)
+    np.testing.assert_almost_equal(pa2.pupil_u[:50], pa1.pupil_u)
+    np.testing.assert_almost_equal(pa2.pupil_v[:50], pa1.pupil_v)
+    np.testing.assert_almost_equal(pa2.x[50:], pa1.x)
+    np.testing.assert_almost_equal(pa2.y[50:], pa1.y)
+    np.testing.assert_almost_equal(pa2.flux[50:], pa1.flux)
+    np.testing.assert_almost_equal(pa2.dxdz[50:], pa1.dxdz)
+    np.testing.assert_almost_equal(pa2.dydz[50:], pa1.dydz)
+    np.testing.assert_almost_equal(pa2.pupil_u[50:], pa1.pupil_u)
+    np.testing.assert_almost_equal(pa2.pupil_v[50:], pa1.pupil_v)
+
+    # Error if it doesn't fit.
+    with assert_raises(ValueError):
+        check_dep(pa2.assignAt, 90, pa1)
+
 @timer
 def test_chromatic_flux():
     # This is based on a snippet of test_chromatic_flux in test_chromatic.py.
 
     bulge_SED = galsim.SED('CWW_E_ext.sed', wave_type='ang', flux_type='flambda')
     star = galsim.Gaussian(fwhm=1e-8) * bulge_SED
     mono_PSF = galsim.Gaussian(half_light_radius=0.8)
@@ -664,12 +696,99 @@
     config['bandpass'] = bp
     psf1 = check_dep(galsim.config.BuildGSObject, config, 'psf')[0]
     psf2 = check_dep(galsim.roman.getPSF, SCA=4, bandpass='W149', pupil_bin=8, wavelength=985.)
     print('psf1 = ',str(psf1))
     print('psf2 = ',str(psf2))
     assert psf1 == psf2
 
+@timer
+def test_photon_array_correlated():
+
+    # This is part of test_convolve in test_photon_array.py
+    nphotons = 1000
+    obj = galsim.Gaussian(flux=1.7, sigma=2.3)
+    rng = galsim.UniformDeviate(1234)
+    pa1 = obj.shoot(nphotons, rng)
+    rng2 = rng.duplicate()  # Save this state.
+    pa2 = obj.shoot(nphotons, rng)
+
+    # If not correlated then convolve is deterministic
+    conv_x = pa1.x + pa2.x
+    conv_y = pa1.y + pa2.y
+    conv_flux = pa1.flux * pa2.flux * nphotons
+
+    np.testing.assert_allclose(np.sum(pa1.flux), 1.7)
+    np.testing.assert_allclose(np.sum(pa2.flux), 1.7)
+    np.testing.assert_allclose(np.sum(conv_flux), 1.7*1.7)
+
+    np.testing.assert_allclose(np.sum(pa1.x**2)/nphotons, 2.3**2, rtol=0.1)
+    np.testing.assert_allclose(np.sum(pa2.x**2)/nphotons, 2.3**2, rtol=0.1)
+    np.testing.assert_allclose(np.sum(conv_x**2)/nphotons, 2.*2.3**2, rtol=0.1)
+
+    np.testing.assert_allclose(np.sum(pa1.y**2)/nphotons, 2.3**2, rtol=0.1)
+    np.testing.assert_allclose(np.sum(pa2.y**2)/nphotons, 2.3**2, rtol=0.1)
+    np.testing.assert_allclose(np.sum(conv_y**2)/nphotons, 2.*2.3**2, rtol=0.1)
+
+    pa3 = galsim.PhotonArray(nphotons)
+    pa3.copyFrom(pa1)  # copy from pa1
+    pa3.convolve(pa2)
+    np.testing.assert_allclose(pa3.x, conv_x)
+    np.testing.assert_allclose(pa3.y, conv_y)
+    np.testing.assert_allclose(pa3.flux, conv_flux)
+
+    # If one of them is correlated, it is still deterministic.
+    pa3.copyFrom(pa1)
+    check_dep(pa3.setCorrelated)
+    pa3.convolve(pa2)
+    np.testing.assert_allclose(pa3.x, conv_x)
+    np.testing.assert_allclose(pa3.y, conv_y)
+    np.testing.assert_allclose(pa3.flux, conv_flux)
+
+    pa3.copyFrom(pa1)
+    check_dep(pa3.setCorrelated, False)
+    check_dep(pa2.setCorrelated)
+    pa3.convolve(pa2)
+    np.testing.assert_allclose(pa3.x, conv_x)
+    np.testing.assert_allclose(pa3.y, conv_y)
+    np.testing.assert_allclose(pa3.flux, conv_flux)
+
+    # But if both are correlated, then it's not this simple.
+    pa3.copyFrom(pa1)
+    check_dep(pa3.setCorrelated)
+    assert check_dep(pa3.isCorrelated)
+    assert check_dep(pa2.isCorrelated)
+    pa3.convolve(pa2)
+    with assert_raises(AssertionError):
+        np.testing.assert_allclose(pa3.x, conv_x)
+    with assert_raises(AssertionError):
+        np.testing.assert_allclose(pa3.y, conv_y)
+    np.testing.assert_allclose(np.sum(pa3.flux), 1.7*1.7)
+    np.testing.assert_allclose(np.sum(pa3.x**2)/nphotons, 2*2.3**2, rtol=0.1)
+    np.testing.assert_allclose(np.sum(pa3.y**2)/nphotons, 2*2.3**2, rtol=0.1)
+
+    # Can also effect the convolution by treating the psf as a PhotonOp
+    pa3.copyFrom(pa1)
+    check_dep(pa3.setCorrelated)
+    obj.applyTo(pa3, rng=rng2)
+    np.testing.assert_allclose(pa3.x, conv_x)
+    np.testing.assert_allclose(pa3.y, conv_y)
+    np.testing.assert_allclose(pa3.flux, conv_flux)
+
+    # Check the is_corr flag gets set
+    assert not check_dep(pa1.isCorrelated)
+    pa3 = check_dep(galsim.PhotonArray.fromArrays, pa1.x, pa1.y, pa1.flux, is_corr=True)
+    assert check_dep(pa3.isCorrelated)
+
+    # Check toggling is_corr
+    assert not check_dep(pa1.isCorrelated)
+    check_dep(pa1.setCorrelated)
+    assert check_dep(pa1.isCorrelated)
+    check_dep(pa1.setCorrelated, False)
+    assert not check_dep(pa1.isCorrelated)
+    check_dep(pa1.setCorrelated, True)
+    assert check_dep(pa1.isCorrelated)
+
 
 if __name__ == "__main__":
     testfns = [v for k, v in vars().items() if k[:5] == 'test_' and callable(v)]
     for testfn in testfns:
         testfn()
```

### Comparing `GalSim-2.5.0/tests/test_des.py` & `GalSim-2.5.1/tests/test_des.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/tests/test_detectors.py` & `GalSim-2.5.1/tests/test_detectors.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/tests/test_download.py` & `GalSim-2.5.1/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/tests/test_draw.py` & `GalSim-2.5.1/tests/test_draw.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/tests/test_errors.py` & `GalSim-2.5.1/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/tests/test_exponential.py` & `GalSim-2.5.1/tests/test_exponential.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/tests/test_fitsheader.py` & `GalSim-2.5.1/tests/test_fitsheader.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/tests/test_fouriersqrt.py` & `GalSim-2.5.1/tests/test_fouriersqrt.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/tests/test_galaxy_sample.py` & `GalSim-2.5.1/tests/test_galaxy_sample.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/tests/test_gaussian.py` & `GalSim-2.5.1/tests/test_gaussian.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/tests/test_hsm.py` & `GalSim-2.5.1/tests/test_hsm.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/tests/test_image.py` & `GalSim-2.5.1/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/tests/test_inclined.py` & `GalSim-2.5.1/tests/test_inclined.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/tests/test_integ.py` & `GalSim-2.5.1/tests/test_integ.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/tests/test_interpolatedimage.py` & `GalSim-2.5.1/tests/test_interpolatedimage.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/tests/test_knots.py` & `GalSim-2.5.1/tests/test_knots.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/tests/test_kolmogorov.py` & `GalSim-2.5.1/tests/test_kolmogorov.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/tests/test_lensing.py` & `GalSim-2.5.1/tests/test_lensing.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/tests/test_main.py` & `GalSim-2.5.1/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/tests/test_metacal.py` & `GalSim-2.5.1/tests/test_metacal.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/tests/test_moffat.py` & `GalSim-2.5.1/tests/test_moffat.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/tests/test_noise.py` & `GalSim-2.5.1/tests/test_noise.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/tests/test_optics.py` & `GalSim-2.5.1/tests/test_optics.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/tests/test_phase_psf.py` & `GalSim-2.5.1/tests/test_phase_psf.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/tests/test_photon_array.py` & `GalSim-2.5.1/tests/test_photon_array.py`

 * *Files 4% similar despite different names*

```diff
@@ -162,24 +162,14 @@
     np.testing.assert_array_equal(photon_array.dxdz, 0.23)
     np.testing.assert_array_equal(photon_array.dydz, 0.88)
     np.testing.assert_array_equal(photon_array.wavelength, 912)
     np.testing.assert_array_equal(photon_array.pupil_u, 6.0)
     np.testing.assert_array_equal(photon_array.pupil_v, 0.0)
     np.testing.assert_array_equal(photon_array.time, 0.0)
 
-
-    # Check toggling is_corr
-    assert not photon_array.isCorrelated()
-    photon_array.setCorrelated()
-    assert photon_array.isCorrelated()
-    photon_array.setCorrelated(False)
-    assert not photon_array.isCorrelated()
-    photon_array.setCorrelated(True)
-    assert photon_array.isCorrelated()
-
     # Check rescaling the total flux
     flux = photon_array.flux.sum()
     np.testing.assert_almost_equal(photon_array.getTotalFlux(), flux)
     photon_array.scaleFlux(17)
     np.testing.assert_almost_equal(photon_array.getTotalFlux(), 17*flux)
     photon_array.setTotalFlux(199)
     np.testing.assert_almost_equal(photon_array.getTotalFlux(), 199)
@@ -213,39 +203,89 @@
     np.testing.assert_almost_equal(pa1.dxdz, photon_array.dxdz[:50])
     np.testing.assert_almost_equal(pa1.dydz, photon_array.dydz[:50])
     np.testing.assert_almost_equal(pa1.wavelength, photon_array.wavelength[:50])
     np.testing.assert_almost_equal(pa1.pupil_u, photon_array.pupil_u[:50])
     np.testing.assert_almost_equal(pa1.pupil_v, photon_array.pupil_v[:50])
     np.testing.assert_almost_equal(pa1.time, photon_array.time[:50])
 
-    # Check assignAt
+    # Check copyFrom
     pa2 = galsim.PhotonArray(100)
-    pa2.assignAt(0, pa1)
-    pa2.assignAt(50, pa1)
-    np.testing.assert_almost_equal(pa2.x[:50], pa1.x)
-    np.testing.assert_almost_equal(pa2.y[:50], pa1.y)
-    np.testing.assert_almost_equal(pa2.flux[:50], pa1.flux)
-    np.testing.assert_almost_equal(pa2.dxdz[:50], pa1.dxdz)
-    np.testing.assert_almost_equal(pa2.dydz[:50], pa1.dydz)
-    np.testing.assert_almost_equal(pa2.wavelength[:50], pa1.wavelength)
-    np.testing.assert_almost_equal(pa2.pupil_u[:50], pa1.pupil_u)
-    np.testing.assert_almost_equal(pa2.pupil_v[:50], pa1.pupil_v)
-    np.testing.assert_almost_equal(pa2.time[:50], pa1.time)
-    np.testing.assert_almost_equal(pa2.x[50:], pa1.x)
-    np.testing.assert_almost_equal(pa2.y[50:], pa1.y)
-    np.testing.assert_almost_equal(pa2.flux[50:], pa1.flux)
-    np.testing.assert_almost_equal(pa2.dxdz[50:], pa1.dxdz)
-    np.testing.assert_almost_equal(pa2.dydz[50:], pa1.dydz)
-    np.testing.assert_almost_equal(pa2.wavelength[50:], pa1.wavelength)
-    np.testing.assert_almost_equal(pa2.pupil_u[50:], pa1.pupil_u)
-    np.testing.assert_almost_equal(pa2.pupil_v[50:], pa1.pupil_v)
-    np.testing.assert_almost_equal(pa2.time[50:], pa1.time)
-
-    # Error if it doesn't fit.
-    assert_raises(ValueError, pa2.assignAt, 90, pa1)
+    pa2.copyFrom(pa1, slice(0,50))
+    pa2.copyFrom(pa1, target_indices=slice(50,100), source_indices=slice(49,None,-1))
+    np.testing.assert_array_equal(pa2.x[:50], pa1.x)
+    np.testing.assert_array_equal(pa2.y[:50], pa1.y)
+    np.testing.assert_array_equal(pa2.flux[:50], pa1.flux)
+    np.testing.assert_array_equal(pa2.dxdz[:50], pa1.dxdz)
+    np.testing.assert_array_equal(pa2.dydz[:50], pa1.dydz)
+    np.testing.assert_array_equal(pa2.wavelength[:50], pa1.wavelength)
+    np.testing.assert_array_equal(pa2.pupil_u[:50], pa1.pupil_u)
+    np.testing.assert_array_equal(pa2.pupil_v[:50], pa1.pupil_v)
+    np.testing.assert_array_equal(pa2.time[:50], pa1.time)
+    np.testing.assert_array_equal(pa2.x[50:], pa1.x[::-1])
+    np.testing.assert_array_equal(pa2.y[50:], pa1.y[::-1])
+    np.testing.assert_array_equal(pa2.flux[50:], pa1.flux[::-1])
+    np.testing.assert_array_equal(pa2.dxdz[50:], pa1.dxdz[::-1])
+    np.testing.assert_array_equal(pa2.dydz[50:], pa1.dydz[::-1])
+    np.testing.assert_array_equal(pa2.wavelength[50:], pa1.wavelength[::-1])
+    np.testing.assert_array_equal(pa2.pupil_u[50:], pa1.pupil_u[::-1])
+    np.testing.assert_array_equal(pa2.pupil_v[50:], pa1.pupil_v[::-1])
+    np.testing.assert_array_equal(pa2.time[50:], pa1.time[::-1])
+
+    # Can copy a single photon if desired.
+    pa2.copyFrom(pa1, 17, 20)
+    assert pa2.flux[17] == pa1.flux[20]
+    assert pa2.x[17] == pa1.x[20]
+    assert pa2.time[17] == pa1.time[20]
+
+    # Can choose not to copy flux
+    pa2.flux[27] = -1
+    pa2.copyFrom(pa1, 27, 10, do_flux=False)
+    assert pa2.flux[27] != pa1.flux[10]
+    assert pa2.x[27] == pa1.x[10]
+    assert pa2.time[27] == pa1.time[10]
+
+    # ... or positions
+    pa2.copyFrom(pa1, 37, 8, do_xy=False)
+    assert pa2.flux[37] == pa1.flux[8]
+    assert pa2.x[37] != pa1.x[8]
+    assert pa2.y[37] != pa1.y[8]
+    assert pa2.time[37] == pa1.time[8]
+
+    # ... or the other arrays
+    pa2.dxdz[47] = pa2.dydz[47] = pa2.wavelength[47] = -1
+    pa2.pupil_u[47] = pa2.pupil_v[47] = pa2.time[47] = -1
+    pa2.copyFrom(pa1, 47, 18, do_other=False)
+    assert pa2.flux[47] == pa1.flux[18]
+    assert pa2.x[47] == pa1.x[18]
+    assert pa2.y[47] == pa1.y[18]
+    assert pa2.dxdz[47] != pa1.dxdz[18]
+    assert pa2.dydz[47] != pa1.dydz[18]
+    assert pa2.wavelength[47] != pa1.wavelength[18]
+    assert pa2.pupil_u[47] != pa1.pupil_u[18]
+    assert pa2.pupil_v[47] != pa1.pupil_v[18]
+    assert pa2.time[47] != pa1.time[18]
+
+    # Can also use complicated numpy expressions for indexing.
+    nleft = np.sum(pa1.x < 0)
+    pa2.copyFrom(pa1, slice(nleft), (pa1.x<0))
+    assert np.all(pa2.x[:nleft] < 0)
+    np.testing.assert_array_equal(pa2.x[:nleft], pa1.x[pa1.x<0])
+    np.testing.assert_array_equal(pa2.y[:nleft], pa1.y[pa1.x<0])
+    pa2.copyFrom(pa1, slice(nleft,50), np.where(pa1.x>=0))
+    assert np.all(pa2.x[nleft:50] > 0)
+    np.testing.assert_array_equal(pa2.x[nleft:50], pa1.x[pa1.x>=0])
+    np.testing.assert_array_equal(pa2.y[nleft:50], pa1.y[pa1.x>=0])
+
+    # Error if indices are invalid
+    assert_raises(ValueError, pa2.copyFrom, pa1, slice(50,None), slice(50,None))
+    assert_raises(ValueError, pa2.copyFrom, pa1, 100, 0)
+    assert_raises(ValueError, pa2.copyFrom, pa1, 0, slice(None))
+    assert_raises(ValueError, pa2.copyFrom, pa1)
+    assert_raises(ValueError, pa2.copyFrom, pa1, slice(None), pa1.x<0)
+    assert_raises(ValueError, pa2.copyFrom, pa1, slice(None), np.where(pa1.x<0))
 
     # Test some trivial usage of makeFromImage
     zero = galsim.Image(4,4,init_value=0)
     photons = galsim.PhotonArray.makeFromImage(zero)
     print('photons = ',photons)
     assert len(photons) == 16
     np.testing.assert_array_equal(photons.flux, 0.)
@@ -278,15 +318,15 @@
 
     obj = galsim.Gaussian(flux=1.7, sigma=2.3)
     rng = galsim.UniformDeviate(1234)
     pa1 = obj.shoot(nphotons, rng)
     rng2 = rng.duplicate()  # Save this state.
     pa2 = obj.shoot(nphotons, rng)
 
-    # If not correlated then convolve is deterministic
+    # Check that convolve is deterministic
     conv_x = pa1.x + pa2.x
     conv_y = pa1.y + pa2.y
     conv_flux = pa1.flux * pa2.flux * nphotons
 
     np.testing.assert_allclose(np.sum(pa1.flux), 1.7)
     np.testing.assert_allclose(np.sum(pa2.flux), 1.7)
     np.testing.assert_allclose(np.sum(conv_flux), 1.7*1.7)
@@ -296,53 +336,22 @@
     np.testing.assert_allclose(np.sum(conv_x**2)/nphotons, 2.*2.3**2, rtol=0.01)
 
     np.testing.assert_allclose(np.sum(pa1.y**2)/nphotons, 2.3**2, rtol=0.01)
     np.testing.assert_allclose(np.sum(pa2.y**2)/nphotons, 2.3**2, rtol=0.01)
     np.testing.assert_allclose(np.sum(conv_y**2)/nphotons, 2.*2.3**2, rtol=0.01)
 
     pa3 = galsim.PhotonArray(nphotons)
-    pa3.assignAt(0, pa1)  # copy from pa1
-    pa3.convolve(pa2)
-    np.testing.assert_allclose(pa3.x, conv_x)
-    np.testing.assert_allclose(pa3.y, conv_y)
-    np.testing.assert_allclose(pa3.flux, conv_flux)
-
-    # If one of them is correlated, it is still deterministic.
-    pa3.assignAt(0, pa1)
-    pa3.setCorrelated()
+    pa3.copyFrom(pa1)  # copy from pa1
     pa3.convolve(pa2)
     np.testing.assert_allclose(pa3.x, conv_x)
     np.testing.assert_allclose(pa3.y, conv_y)
     np.testing.assert_allclose(pa3.flux, conv_flux)
 
-    pa3.assignAt(0, pa1)
-    pa3.setCorrelated(False)
-    pa2.setCorrelated()
-    pa3.convolve(pa2)
-    np.testing.assert_allclose(pa3.x, conv_x)
-    np.testing.assert_allclose(pa3.y, conv_y)
-    np.testing.assert_allclose(pa3.flux, conv_flux)
-
-    # But if both are correlated, then it's not this simple.
-    pa3.assignAt(0, pa1)
-    pa3.setCorrelated()
-    assert pa3.isCorrelated()
-    assert pa2.isCorrelated()
-    pa3.convolve(pa2)
-    with assert_raises(AssertionError):
-        np.testing.assert_allclose(pa3.x, conv_x)
-    with assert_raises(AssertionError):
-        np.testing.assert_allclose(pa3.y, conv_y)
-    np.testing.assert_allclose(np.sum(pa3.flux), 1.7*1.7)
-    np.testing.assert_allclose(np.sum(pa3.x**2)/nphotons, 2*2.3**2, rtol=0.01)
-    np.testing.assert_allclose(np.sum(pa3.y**2)/nphotons, 2*2.3**2, rtol=0.01)
-
     # Can also effect the convolution by treating the psf as a PhotonOp
-    pa3.assignAt(0, pa1)
-    pa3.setCorrelated()
+    pa3.copyFrom(pa1)
     obj.applyTo(pa3, rng=rng2)
     np.testing.assert_allclose(pa3.x, conv_x)
     np.testing.assert_allclose(pa3.y, conv_y)
     np.testing.assert_allclose(pa3.flux, conv_flux)
 
     # Error to have different lengths
     pa4 = galsim.PhotonArray(50, pa1.x[:50], pa1.y[:50], pa1.flux[:50])
@@ -1532,19 +1541,14 @@
     np.testing.assert_array_equal(pa_2.dxdz, pa_batch.dxdz[Nsplit:])
     np.testing.assert_array_equal(pa_2.dydz, pa_batch.dydz[Nsplit:])
     np.testing.assert_array_equal(pa_2.wavelength, pa_batch.wavelength[Nsplit:])
     np.testing.assert_array_equal(pa_2.pupil_u, pa_batch.pupil_u[Nsplit:])
     np.testing.assert_array_equal(pa_2.pupil_v, pa_batch.pupil_v[Nsplit:])
     np.testing.assert_array_equal(pa_2.time, pa_batch.time[Nsplit:])
 
-    # Check the is_corr flag gets set
-    assert not pa_batch.isCorrelated()
-    pa_batch = galsim.PhotonArray.fromArrays(x, y, flux, dxdz, dydz, wavelength, is_corr=True)
-    assert pa_batch.isCorrelated()
-
     # Check some invalid inputs are caught
     with np.testing.assert_raises(TypeError):
         galsim.PhotonArray.fromArrays(list(x), y, flux, dxdz, dydz, wavelength)
     with np.testing.assert_raises(TypeError):
         galsim.PhotonArray.fromArrays(np.empty(1000, dtype=int), y, flux, dxdz, dydz, wavelength)
     with np.testing.assert_raises(ValueError):
         galsim.PhotonArray.fromArrays(x[:10], y, flux, dxdz, dydz, wavelength)
```

### Comparing `GalSim-2.5.0/tests/test_pse.py` & `GalSim-2.5.1/tests/test_pse.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/tests/test_random.py` & `GalSim-2.5.1/tests/test_random.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 #    and/or other materials provided with the distribution.
 #
 
 import numpy as np
 import os
 import sys
 import math
+import warnings
 
 import galsim
 from galsim_test_helpers import *
 from galsim.utilities import single_threaded
 
 
 #
@@ -1753,14 +1754,40 @@
     d.seed(testseed)
     test_array = np.empty(3)
     d.generate(test_array)
     np.testing.assert_array_almost_equal(
             test_array, np.array(dLookupTableResult), precision,
             err_msg='Wrong DistDeviate random number sequence from generate.')
 
+    # Test clip_neg
+    # Same values as d, but with some negative values, where it had zeros.
+    x = [0.0, 1.0, 1.000000001, 1.5, 2, 2.5, 2.999999999, 3.0, 4.0]
+    f = [0.1, 0.1, 0.0, -0.2, -0.3, -0.2, 0.0    , 0.1, 0.1]
+    tab2 = galsim.LookupTable(x=x, f=f, interpolant='linear')
+    d2 = galsim.DistDeviate(testseed, function=tab2, clip_neg=True)
+    test_array2 = np.empty(3)
+    d2.generate(test_array2)
+    np.testing.assert_array_almost_equal(test_array2, test_array)
+
+    # Without clip_neg, it raises an error
+    with assert_raises(galsim.GalSimValueError):
+        galsim.DistDeviate(testseed, function=tab2)
+    with assert_raises(galsim.GalSimValueError):
+        galsim.DistDeviate(testseed, function=tab2, clip_neg=False)
+
+    # Also works to cleanup NaN values
+    with warnings.catch_warnings():
+        warnings.filterwarnings("ignore", category=RuntimeWarning)
+        f = [0.1, 0.1, 0.0, -0.2, np.sqrt(-0.3), -0.2, 0.0    , 0.1, 0.1]
+    tab3 = galsim.LookupTable(x=x, f=f, interpolant='linear')
+    d3 = galsim.DistDeviate(testseed, function=tab3, clip_neg=True)
+    test_array3 = np.empty(3)
+    d3.generate(test_array3)
+    np.testing.assert_array_almost_equal(test_array3, test_array)
+
     # Test filling an image
     d.seed(testseed)
     testimage = galsim.ImageD(np.zeros((3, 1)))
     testimage.addNoise(galsim.DeviateNoise(d))
     np.testing.assert_array_almost_equal(
             testimage.array.flatten(), np.array(dLookupTableResult), precision,
             err_msg='Wrong DistDeviate random number sequence generated when applied to image.')
```

### Comparing `GalSim-2.5.0/tests/test_real.py` & `GalSim-2.5.1/tests/test_real.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/tests/test_roman.py` & `GalSim-2.5.1/tests/test_roman.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/tests/test_second_kick.py` & `GalSim-2.5.1/tests/test_second_kick.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/tests/test_sed.py` & `GalSim-2.5.1/tests/test_sed.py`

 * *Files 2% similar despite different names*

```diff
@@ -283,26 +283,32 @@
         if sed is sed0: check_pickle(d)
 
         # SED multiplied by dimensionless, constant SED
         e = galsim.SED(2.0, 'nm', '1')
         f = a*e
         np.testing.assert_almost_equal(f(x), a(x) * e(x), 10,
                                        err_msg="Found wrong value in SED.__mul__")
-        f = e*a
-        np.testing.assert_almost_equal(f(x), e(x) * a(x), 10,
+        f2 = e*a
+        np.testing.assert_almost_equal(f2(x), e(x) * a(x), 10,
                                        err_msg="Found wrong value in SED.__mul__")
+        if sed is sed0:
+            check_pickle(f)
+            check_pickle(f2)
 
         # SED multiplied by dimensionless, non-constant SED
         g = galsim.SED('wave', 'nm', '1')
         h = a*g
         np.testing.assert_almost_equal(h(x), a(x) * g(x), 10,
                                        err_msg="Found wrong value in SED.__mul__")
         h2 = g*a
         np.testing.assert_almost_equal(h2(x), g(x) * a(x), 10,
                                        err_msg="Found wrong value in SED.__mul__")
+        if sed is sed0:
+            check_pickle(h)
+            check_pickle(h2)
 
         assert_raises(TypeError, a.__mul__, 'invalid')
 
 
     sed1 = galsim.SED('1', 'nm', 'fphotons', redshift=1)
     sed2 = galsim.SED('2', 'nm', 'fphotons', redshift=2)
     sed3 = galsim.SED('3', 'nm', '1')
@@ -509,16 +515,17 @@
 def test_SED_withFlux():
     """ Check that setting the flux works.
     """
     rband = galsim.Bandpass(os.path.join(bppath, 'LSST_r.dat'), 'nm')
     for z in [0, 0.2, 0.4]:
         for fast in [True, False]:
             for sed in [
-                galsim.SED(os.path.join(sedpath, 'CWW_E_ext.sed'), wave_type='ang',
-                           flux_type='flambda', fast=fast),
+                galsim.SED('CWW_E_ext.sed', wave_type='ang', flux_type='flambda', fast=fast),
+                galsim.SED('CWW_E_ext.sed', wave_type='ang', flux_type='flambda', fast=fast,
+                           interpolant='spline'),
                 galsim.SED('wave', wave_type='nm', flux_type='fphotons'),
                 galsim.EmissionLine(620.0, 1.0) + 2*galsim.EmissionLine(450.0, 0.5)
             ]:
                 if z != 0:
                     sed = sed.atRedshift(z)
                 sed = sed.withFlux(1.0, rband)
                 np.testing.assert_array_almost_equal(
@@ -569,16 +576,15 @@
 
 
 @timer
 def test_SED_withFluxDensity():
     """ Check that setting the flux density works.
     """
 
-    a0 = galsim.SED(os.path.join(sedpath, 'CWW_E_ext.sed'), wave_type='ang',
-                    flux_type='flambda')
+    a0 = galsim.SED('CWW_E_ext.sed', wave_type='ang', flux_type='flambda')
     for z in [0, 0.2, 0.4]:
         a = a0.atRedshift(z)
         a = a.withFluxDensity(1.0, 500)
         np.testing.assert_array_almost_equal(
                 a(500), 1.0, 5, "Setting SED flux density failed.")
         a = a.withFluxDensity(2.0, 5000*units.AA)
         np.testing.assert_array_almost_equal(
@@ -720,14 +726,29 @@
     print('z=0 disk in HST V band: flux = ',flux0, t1-t0)
     print('z=1 disk in HST V band: flux = ',flux1, t2-t1)
 
     # Regression tests
     np.testing.assert_allclose(flux0, 2.993792e+15, rtol=1.e-4)
     np.testing.assert_allclose(flux1, 4.395954e+14, rtol=1.e-4)
 
+    # With spline, it's almost the same, but slightly different of course.
+    sed = galsim.SED('CWW_Sbc_ext.sed', 'nm', 'flambda', interpolant='spline')
+    bp = galsim.Bandpass('ACS_wfc_F606W.dat', 'nm', interpolant='spline')
+    t0 = time.time()
+    flux0 = sed.calculateFlux(bp)
+    t1 = time.time()
+    flux1 = sed.atRedshift(1).calculateFlux(bp)
+    t2 = time.time()
+    print('z=0 disk in HST V band: flux = ',flux0, t1-t0)
+    print('z=1 disk in HST V band: flux = ',flux1, t2-t1)
+
+    # Regression tests
+    np.testing.assert_allclose(flux0, 3.023368e+15, rtol=1.e-4)
+    np.testing.assert_allclose(flux1, 4.303569e+14, rtol=1.e-4)
+
 
 @timer
 def test_SED_calculateDCRMomentShifts():
     # compute some moment shifts
     sed = galsim.SED(os.path.join(sedpath, 'CWW_E_ext.sed'), 'nm', 'flambda')
     bandpass = galsim.Bandpass(os.path.join(bppath, 'LSST_r.dat'), 'nm')
     Rbar, V = sed.calculateDCRMomentShifts(bandpass, zenith_angle=45*galsim.degrees)
@@ -845,15 +866,15 @@
     out = sed.sampleWavelength(3,None,rng=rng, npoints=256)
     np.testing.assert_array_almost_equal(out,test0,8,"Failed to pass 'UniformDeviate'.")
 
     out = sed.sampleWavelength(3,bandpass,rng=seed, npoints=256)
     np.testing.assert_equal(len(sed._cache_deviate),2,"Creating new SED deviate failed.")
 
     test1 = np.array([ 4.16227593,  4.6166918 ,  2.95075946])
-    np.testing.assert_array_almost_equal(out,test1,8,"Unexpected SED sample values.")
+    np.testing.assert_array_almost_equal(out,test1,5,"Unexpected SED sample values.")
 
     out = sed.sampleWavelength(1e3,bandpass,rng=seed,npoints=256)
     np.testing.assert_equal(len(sed._cache_deviate),2,"Unexpected number of SED deviates.")
     np.testing.assert_equal(len(out),1e3,"Unexpected number of SED samples.")
 
     np.testing.assert_equal(np.sum(out > sedbp.red_limit),0,
                             "SED sample outside of function bounds.")
@@ -1012,38 +1033,50 @@
             galsim.EmissionLine(500.0, 1.0),
         ]
     check_all_diff(seds)
 
 
 @timer
 def test_thin():
-    s = galsim.SED(os.path.join(sedpath, 'CWW_E_ext.sed'), wave_type='ang', flux_type='flambda',
-                   fast=False)
-    bp = galsim.Bandpass('1', 'nm', blue_limit=s.blue_limit, red_limit=s.red_limit)
-    flux = s.calculateFlux(bp)
-    print("Original number of SED samples = ",len(s.wave_list))
-    for err in [1.e-2, 1.e-3, 1.e-4, 1.e-5]:
-        print("Test err = ",err)
-        thin_s = s.thin(rel_err=err, preserve_range=True, fast_search=False)
-        thin_flux = thin_s.calculateFlux(bp)
-        thin_err = (flux-thin_flux)/flux
-        print("num samples with preserve_range = True, fast_search = False: ",len(thin_s.wave_list))
-        print("realized error = ",(flux-thin_flux)/flux)
-        thin_s = s.thin(rel_err=err, preserve_range=True)
-        thin_flux = thin_s.calculateFlux(bp)
-        thin_err = (flux-thin_flux)/flux
-        print("num samples with preserve_range = True: ",len(thin_s.wave_list))
-        print("realized error = ",(flux-thin_flux)/flux)
-        assert np.abs(thin_err) < err, "Thinned SED failed accuracy goal, preserving range."
-        thin_s = s.thin(rel_err=err, preserve_range=False)
-        thin_flux = thin_s.calculateFlux(bp.truncate(thin_s.blue_limit, thin_s.red_limit))
-        thin_err = (flux-thin_flux)/flux
-        print("num samples with preserve_range = False: ",len(thin_s.wave_list))
-        print("realized error = ",(flux-thin_flux)/flux)
-        assert np.abs(thin_err) < err, "Thinned SED failed accuracy goal, w/ range shrinkage."
+    for interpolant in ['linear', 'nearest', 'spline']:
+        s = galsim.SED('CWW_E_ext.sed', wave_type='ang', flux_type='flambda',
+                       fast=False, interpolant=interpolant)
+        bp = galsim.Bandpass('1', 'nm', blue_limit=s.blue_limit, red_limit=s.red_limit)
+        flux = s.calculateFlux(bp)
+        print("Original number of SED samples = ",len(s.wave_list))
+        for err in [1.e-2, 1.e-3, 1.e-4, 1.e-5]:
+            print("Test err = ",err)
+            thin_s = s.thin(rel_err=err, preserve_range=True, fast_search=False)
+            thin_flux = thin_s.calculateFlux(bp)
+            thin_err = (flux-thin_flux)/flux
+            print("num samples with preserve_range = True, fast_search = False: ",
+                  len(thin_s.wave_list))
+            print("realized error = ",(flux-thin_flux)/flux)
+            thin_s = s.thin(rel_err=err, preserve_range=True)
+            thin_flux = thin_s.calculateFlux(bp)
+            thin_err = (flux-thin_flux)/flux
+            print("num samples with preserve_range = True: ",len(thin_s.wave_list))
+            print("realized error = ",(flux-thin_flux)/flux)
+            print('true flux = ',flux)
+            print('thinned flux = ',thin_flux)
+            print('err = ',thin_err)
+            # The thinning algorithm guarantees a relative error of err for bolometric flux,
+            # but not for any arbitrary bandpass.  When the target error is very small, it can
+            # miss by a bit, especially for spline.  So test it with a little looser tolerance
+            # than the target.
+            test_err = err*4 if err <= 1.e-5 else err
+            assert np.abs(thin_err) < test_err,\
+                "Thinned SED failed accuracy goal, preserving range."
+            thin_s = s.thin(rel_err=err, preserve_range=False)
+            thin_flux = thin_s.calculateFlux(bp.truncate(thin_s.blue_limit, thin_s.red_limit))
+            thin_err = (flux-thin_flux)/flux
+            print("num samples with preserve_range = False: ",len(thin_s.wave_list))
+            print("realized error = ",(flux-thin_flux)/flux)
+            assert np.abs(thin_err) < test_err,\
+                "Thinned SED failed accuracy goal, w/ range shrinkage."
 
     assert_raises(ValueError, s.thin, rel_err=-0.5)
     assert_raises(ValueError, s.thin, rel_err=1.5)
     # These errors aren't accessible from the SED or Bandpass calls.
     assert_raises(ValueError, galsim.utilities.thin_tabulated_values,
                   s.wave_list[3:], s._spec.getVals())
     assert_raises(ValueError, galsim.utilities.thin_tabulated_values,
@@ -1151,16 +1184,18 @@
     for wavelength, fwhm in [
         (500.0, 1.0),
         (650.0, 0.3),
         (700.0, 4.3)
     ]:
         for sed in [
             galsim.EmissionLine(wavelength, fwhm),
-            galsim.EmissionLine(wavelength*10, fwhm*10, wave_type='ang')
+            galsim.EmissionLine(wavelength*10, fwhm*10, wave_type='ang'),
+            galsim.EmissionLine(wavelength*1.e-9, fwhm*1.e-9, wave_type=units.m),
         ]:
+            print(sed)
             np.testing.assert_allclose(sed.calculateFlux(None), 1.0)
             np.testing.assert_allclose((sed*2).calculateFlux(None), 2.0)
             np.testing.assert_allclose((3*sed).calculateFlux(None), 3.0)
             np.testing.assert_allclose((sed/2).calculateFlux(None), 0.5)
             np.testing.assert_allclose(sed(wavelength), 1./fwhm)
             np.testing.assert_allclose(sed(wavelength+fwhm), 0.0, rtol=0, atol=1e-11)
             np.testing.assert_allclose(sed(wavelength-fwhm), 0.0, rtol=0, atol=1e-11)
@@ -1176,17 +1211,63 @@
             with np.testing.assert_raises(galsim.GalSimIncompatibleValuesError):
                 sed * spectral
             with np.testing.assert_raises(galsim.GalSimSEDError):
                 sed / spectral
             with np.testing.assert_raises(galsim.GalSimSEDError):
                 spectral / sed
 
-            sed = sed.atRedshift(1.1)
-            assert sed is sed.atRedshift(1.1)
+            z = 1.1
+            sed = sed.atRedshift(z)
+            assert sed is sed.atRedshift(z)
+            np.testing.assert_allclose(sed.calculateFlux(None), (1+z))
+            np.testing.assert_allclose(sed(wavelength*(1+z)), 1/fwhm)
+
             with np.testing.assert_raises(galsim.GalSimRangeError):
                 sed.atRedshift(-2.0)
+        with np.testing.assert_raises(galsim.GalSimValueError):
+            galsim.EmissionLine(wavelength, fwhm, wave_type=units.Hz),
+
+
+@timer
+def test_flux_type_calculateFlux():
+    sed1 = galsim.SED(
+        galsim.LookupTable([1,2,3,4,5], [1.1, 1.9, 1.4, 1.8, 2.0]),
+        wave_type='nm', flux_type='flambda'
+    )
+    sed2 = galsim.SED(
+        galsim.LookupTable([1,2,3,4,5], [1.1, 1.9, 1.4, 1.8, 2.0]),
+        wave_type='nm', flux_type='fnu'
+    )
+    sed3 = galsim.SED(
+        galsim.LookupTable([1,2,3,4,5], [1.1, 1.9, 1.4, 1.8, 2.0]),
+        wave_type='nm', flux_type='fphotons'
+    )
+    sed4 = galsim.SED(
+        galsim.LookupTable([1,2,3,4,5], [1.1, 1.9, 1.4, 1.8, 2.0]),
+        wave_type="nm", flux_type=units.Lsun / units.Hz / units.Mpc**2
+    )
+    flat_sed = galsim.SED(
+        '1',
+        wave_type="nm", flux_type="1"
+    )
+    bp = galsim.Bandpass(galsim.LookupTable([2,4], [1,2]), wave_type='nm')
+    exp_gal = galsim.Exponential(half_light_radius=0.5, flux=1)
+
+    for sed in [sed1, sed2, sed3, sed4]:
+        flux1 = sed.calculateFlux(bp)
+        flux2 = (1 * sed).calculateFlux(bp)
+        flux3 = (exp_gal * sed).calculateFlux(bp)
+        flux4 = (flat_sed * sed).calculateFlux(bp)
+        print('flux = {}, {}, {}'.format(flux1, flux2, flux3))
+        wave = np.linspace(bp.blue_limit, bp.red_limit, 10000)
+        f = sed(wave) * bp(wave)
+        flux5 = np.trapz(f, wave)
+        np.testing.assert_allclose(flux1, flux2)
+        np.testing.assert_allclose(flux1, flux3)
+        np.testing.assert_allclose(flux1, flux4)
+        np.testing.assert_allclose(flux1, flux5)
 
 
 if __name__ == "__main__":
     testfns = [v for k, v in vars().items() if k[:5] == 'test_' and callable(v)]
     for testfn in testfns:
         testfn()
```

### Comparing `GalSim-2.5.0/tests/test_sensor.py` & `GalSim-2.5.1/tests/test_sensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -883,14 +883,39 @@
                                    treering_center=galsim.PositionD(1,1))
     im.fill(0)
     areas8 = sensor8.calculate_pixel_areas(im)
     print('min/max area1 = ',np.min(areas8.array),np.max(areas8.array))
     # Mostly checking that there aren't any nan's here from division by 0.
     assert np.min(areas8.array) > 0
 
+    # Also check that things behave sensibly if the stamp is outside the arg range of
+    # the treering function
+    # tr6 has a max radius of 2000.
+    im.setCenter(2000,2000)
+    obj.drawImage(im, method='phot', sensor=sensor6, rng=rng6)
+    print('im.sum = ',im.array.sum(), im.added_flux)
+    np.testing.assert_allclose(im.array.sum(), im.added_flux)
+    np.testing.assert_allclose(im.array.sum(), init_flux, rtol=1.e-2)
+
+    areas6a = sensor6.calculate_pixel_areas(im, use_flux=True)
+    assert np.min(areas6a.array) > 0
+    print('areas6a = ',areas6a.array)
+    areas6b = sensor6.calculate_pixel_areas(im, use_flux=False)
+    assert np.min(areas6b.array) > 0
+    # When the stamp is outside the range of the treering function, the areas will be
+    # identical for the use_flux=False case.
+    print('areas6b = ',areas6b.array)
+    print('min, max = ',areas6b.array.min(), areas6b.array.max())
+    assert np.all(areas6b.array == areas6b.array[0,0])
+    # But not when use_flux=True
+    assert not np.all(areas6a.array == areas6a.array[0,0])
+    print('mean, std when use_flux=True: ', np.mean(areas6a.array), np.std(areas6a.array))
+    np.testing.assert_allclose(np.mean(areas6a.array), np.mean(areas6b.array),
+                               rtol=np.std(areas6a.array)/np.sqrt(np.prod(areas6b.array.shape))*3)
+
 
 @timer
 def test_resume():
     """Test that the resume option for accumulate works properly.
     """
     # Note: This test is based on a script devel/lsst/treering_skybg_check.py
```

### Comparing `GalSim-2.5.0/tests/test_sersic.py` & `GalSim-2.5.1/tests/test_sersic.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/tests/test_shapelet.py` & `GalSim-2.5.1/tests/test_shapelet.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/tests/test_shear.py` & `GalSim-2.5.1/tests/test_shear.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/tests/test_shear_position.py` & `GalSim-2.5.1/tests/test_shear_position.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/tests/test_spergel.py` & `GalSim-2.5.1/tests/test_spergel.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/tests/test_sum.py` & `GalSim-2.5.1/tests/test_sum.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/tests/test_table.py` & `GalSim-2.5.1/tests/test_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -1082,32 +1082,36 @@
     t4 = time.time()
     ans5 = galsim._LookupTable(x,y,'nearest').integrate()
     t5 = time.time()
     ans6 = galsim.trapz(y,x)
     t6 = time.time()
     ans7 = np.trapz(y,x)
     t7 = time.time()
+    ans8 = galsim.trapz(y,x, interpolant='spline')
+    t8 = time.time()
     # Amazingly, LookupTable(linear) is more than 2x faster than np.trapz, and equally accurate.
     # Spline is a bit slower, but about 2x more accurate.
     # Floor and ceil are slightly faster still, but not nearly as accurate.
     print('           integration time       answer - Pi')
     print('linear         %.6f          %.6e'%(t1-t0,ans1-np.pi))
     print('spline         %.6f          %.6e'%(t2-t1,ans2-np.pi))
     print('floor          %.6f          %.6e'%(t3-t2,ans3-np.pi))
     print('ceil           %.6f          %.6e'%(t4-t3,ans4-np.pi))
     print('nearest        %.6f          %.6e'%(t5-t4,ans5-np.pi))
     print('trapz          %.6f          %.6e'%(t6-t5,ans6-np.pi))
     print('np.trapz       %.6f          %.6e'%(t7-t6,ans7-np.pi))
+    print('trapz(spline)  %.6f          %.6e'%(t8-t7,ans8-np.pi))
     np.testing.assert_allclose(ans1, np.pi, atol=2.e-9)
     np.testing.assert_allclose(ans2, np.pi, atol=1.e-9)
     np.testing.assert_allclose(ans3, np.pi, atol=3.e-6)
     np.testing.assert_allclose(ans4, np.pi, atol=3.e-6)
     np.testing.assert_allclose(ans5, np.pi, atol=2.e-9)
     np.testing.assert_allclose(ans6, np.pi, atol=2.e-9)
     np.testing.assert_allclose(ans7, np.pi, atol=2.e-9)
+    np.testing.assert_allclose(ans8, np.pi, atol=1.e-9)
 
     # Check errors
     with assert_raises(NotImplementedError):
         galsim.LookupTable([1,2,3,4], [5,5,8,1], x_log=True).integrate()
     with assert_raises(NotImplementedError):
         galsim.LookupTable([1,2,3,4], [5,5,8,1], f_log=True).integrate()
     with assert_raises(NotImplementedError):
```

### Comparing `GalSim-2.5.0/tests/test_transforms.py` & `GalSim-2.5.1/tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/tests/test_utilities.py` & `GalSim-2.5.1/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/tests/test_vonkarman.py` & `GalSim-2.5.1/tests/test_vonkarman.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/tests/test_wcs.py` & `GalSim-2.5.1/tests/test_wcs.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.5.0/tests/test_zernike.py` & `GalSim-2.5.1/tests/test_zernike.py`

 * *Files identical despite different names*

