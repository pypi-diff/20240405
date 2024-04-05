# Comparing `tmp/cmocean-3.1.3.tar.gz` & `tmp/cmocean-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmocean-3.1.3.tar", last modified: Tue Jan 23 17:44:57 2024, max compression
+gzip compressed data, was "cmocean-4.0.1.tar", last modified: Fri Apr  5 21:39:13 2024, max compression
```

## Comparing `cmocean-3.1.3.tar` & `cmocean-4.0.1.tar`

### file list

```diff
@@ -1,96 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 17:44:57.881744 cmocean-3.1.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 17:44:57.861744 cmocean-3.1.3/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-01-23 17:44:52.000000 cmocean-3.1.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 17:44:57.861744 cmocean-3.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-01-23 17:44:52.000000 cmocean-3.1.3/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-01-23 17:44:52.000000 cmocean-3.1.3/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-01-23 17:44:52.000000 cmocean-3.1.3/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-01-23 17:44:52.000000 cmocean-3.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-01-23 17:44:52.000000 cmocean-3.1.3/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-01-23 17:44:52.000000 cmocean-3.1.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-01-23 17:44:52.000000 cmocean-3.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-01-23 17:44:57.881744 cmocean-3.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-01-23 17:44:52.000000 cmocean-3.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 17:44:57.861744 cmocean-3.1.3/ci/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-01-23 17:44:52.000000 cmocean-3.1.3/ci/environment-py3.10.yml
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-01-23 17:44:52.000000 cmocean-3.1.3/ci/environment-py3.8.yml
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-01-23 17:44:52.000000 cmocean-3.1.3/ci/environment-py3.9.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 17:44:57.861744 cmocean-3.1.3/cmocean/
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-01-23 17:44:52.000000 cmocean-3.1.3/cmocean/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-01-23 17:44:52.000000 cmocean-3.1.3/cmocean/cm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-01-23 17:44:52.000000 cmocean-3.1.3/cmocean/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5295 2024-01-23 17:44:52.000000 cmocean-3.1.3/cmocean/plots.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 17:44:57.869744 cmocean-3.1.3/cmocean/rgb/
--rw-r--r--   0 runner    (1001) docker     (127)    19200 2024-01-23 17:44:52.000000 cmocean-3.1.3/cmocean/rgb/algae-rgb.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13687 2024-01-23 17:44:52.000000 cmocean-3.1.3/cmocean/rgb/algae.py
--rw-r--r--   0 runner    (1001) docker     (127)    19200 2024-01-23 17:44:52.000000 cmocean-3.1.3/cmocean/rgb/amp-rgb.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13746 2024-01-23 17:44:52.000000 cmocean-3.1.3/cmocean/rgb/balance-blue.py
--rw-r--r--   0 runner    (1001) docker     (127)    13641 2024-01-23 17:44:52.000000 cmocean-3.1.3/cmocean/rgb/balance-red.py
--rw-r--r--   0 runner    (1001) docker     (127)    19200 2024-01-23 17:44:52.000000 cmocean-3.1.3/cmocean/rgb/balance-rgb.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13707 2024-01-23 17:44:52.000000 cmocean-3.1.3/cmocean/rgb/curl-pink.py
--rw-r--r--   0 runner    (1001) docker     (127)    38400 2024-01-23 17:44:52.000000 cmocean-3.1.3/cmocean/rgb/curl-rgb.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13668 2024-01-23 17:44:52.000000 cmocean-3.1.3/cmocean/rgb/curl-turquoise.py
--rw-r--r--   0 runner    (1001) docker     (127)    19200 2024-01-23 17:44:52.000000 cmocean-3.1.3/cmocean/rgb/deep-rgb.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13710 2024-01-23 17:44:52.000000 cmocean-3.1.3/cmocean/rgb/deep.py
--rw-r--r--   0 runner    (1001) docker     (127)    13698 2024-01-23 17:44:52.000000 cmocean-3.1.3/cmocean/rgb/delta-blue.py
--rw-r--r--   0 runner    (1001) docker     (127)    13740 2024-01-23 17:44:52.000000 cmocean-3.1.3/cmocean/rgb/delta-green.py
--rw-r--r--   0 runner    (1001) docker     (127)    38400 2024-01-23 17:44:52.000000 cmocean-3.1.3/cmocean/rgb/delta-rgb.txt
--rw-r--r--   0 runner    (1001) docker     (127)    19200 2024-01-23 17:44:52.000000 cmocean-3.1.3/cmocean/rgb/dense-rgb.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13693 2024-01-23 17:44:52.000000 cmocean-3.1.3/cmocean/rgb/dense.py
--rw-r--r--   0 runner    (1001) docker     (127)    19200 2024-01-23 17:44:52.000000 cmocean-3.1.3/cmocean/rgb/diff-rgb.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-01-23 17:44:52.000000 cmocean-3.1.3/cmocean/rgb/diff.jscm
--rw-r--r--   0 runner    (1001) docker     (127)    19200 2024-01-23 17:44:52.000000 cmocean-3.1.3/cmocean/rgb/gray-rgb.txt
--rw-r--r--   0 runner    (1001) docker     (127)    17393 2024-01-23 17:44:52.000000 cmocean-3.1.3/cmocean/rgb/gray.py
--rw-r--r--   0 runner    (1001) docker     (127)    19200 2024-01-23 17:44:52.000000 cmocean-3.1.3/cmocean/rgb/haline-rgb.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13698 2024-01-23 17:44:52.000000 cmocean-3.1.3/cmocean/rgb/haline.py
--rw-r--r--   0 runner    (1001) docker     (127)    19200 2024-01-23 17:44:52.000000 cmocean-3.1.3/cmocean/rgb/ice-rgb.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13796 2024-01-23 17:44:52.000000 cmocean-3.1.3/cmocean/rgb/ice.py
--rw-r--r--   0 runner    (1001) docker     (127)    19200 2024-01-23 17:44:52.000000 cmocean-3.1.3/cmocean/rgb/matter-rgb.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13688 2024-01-23 17:44:52.000000 cmocean-3.1.3/cmocean/rgb/matter.py
--rw-r--r--   0 runner    (1001) docker     (127)    19200 2024-01-23 17:44:52.000000 cmocean-3.1.3/cmocean/rgb/oxy-rgb.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13666 2024-01-23 17:44:52.000000 cmocean-3.1.3/cmocean/rgb/oxy.py
--rw-r--r--   0 runner    (1001) docker     (127)    19200 2024-01-23 17:44:52.000000 cmocean-3.1.3/cmocean/rgb/phase-rgb.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13873 2024-01-23 17:44:52.000000 cmocean-3.1.3/cmocean/rgb/phase.py
--rw-r--r--   0 runner    (1001) docker     (127)    19200 2024-01-23 17:44:52.000000 cmocean-3.1.3/cmocean/rgb/rain-rgb.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-01-23 17:44:52.000000 cmocean-3.1.3/cmocean/rgb/rain.jscm
--rw-r--r--   0 runner    (1001) docker     (127)    19200 2024-01-23 17:44:52.000000 cmocean-3.1.3/cmocean/rgb/solar-rgb.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13687 2024-01-23 17:44:52.000000 cmocean-3.1.3/cmocean/rgb/solar.py
--rw-r--r--   0 runner    (1001) docker     (127)    19200 2024-01-23 17:44:52.000000 cmocean-3.1.3/cmocean/rgb/speed-rgb.txt
--rw-r--r--   0 runner    (1001) docker     (127)    19200 2024-01-23 17:44:52.000000 cmocean-3.1.3/cmocean/rgb/tarn-rgb.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-01-23 17:44:52.000000 cmocean-3.1.3/cmocean/rgb/tarn.jscm
--rw-r--r--   0 runner    (1001) docker     (127)    19200 2024-01-23 17:44:52.000000 cmocean-3.1.3/cmocean/rgb/tempo-rgb.txt
--rw-r--r--   0 runner    (1001) docker     (127)    19200 2024-01-23 17:44:52.000000 cmocean-3.1.3/cmocean/rgb/thermal-rgb.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13692 2024-01-23 17:44:52.000000 cmocean-3.1.3/cmocean/rgb/thermal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-01-23 17:44:52.000000 cmocean-3.1.3/cmocean/rgb/topo-land.jscm
--rw-r--r--   0 runner    (1001) docker     (127)    19200 2024-01-23 17:44:52.000000 cmocean-3.1.3/cmocean/rgb/topo-rgb.txt
--rw-r--r--   0 runner    (1001) docker     (127)    19200 2024-01-23 17:44:52.000000 cmocean-3.1.3/cmocean/rgb/turbid-rgb.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13685 2024-01-23 17:44:52.000000 cmocean-3.1.3/cmocean/rgb/turbid.py
--rw-r--r--   0 runner    (1001) docker     (127)     9161 2024-01-23 17:44:52.000000 cmocean-3.1.3/cmocean/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 17:44:57.881744 cmocean-3.1.3/cmocean.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-01-23 17:44:57.000000 cmocean-3.1.3/cmocean.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-01-23 17:44:57.000000 cmocean-3.1.3/cmocean.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-23 17:44:57.000000 cmocean-3.1.3/cmocean.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-01-23 17:44:57.000000 cmocean-3.1.3/cmocean.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-23 17:44:57.000000 cmocean-3.1.3/cmocean.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 17:44:57.873744 cmocean-3.1.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     7527 2024-01-23 17:44:52.000000 cmocean-3.1.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     7255 2024-01-23 17:44:52.000000 cmocean-3.1.3/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 17:44:57.873744 cmocean-3.1.3/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-01-23 17:44:52.000000 cmocean-3.1.3/docs/source/cmocean.rst
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-01-23 17:44:52.000000 cmocean-3.1.3/docs/source/colormaps_viscm.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9380 2024-01-23 17:44:52.000000 cmocean-3.1.3/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    37020 2024-01-23 17:44:52.000000 cmocean-3.1.3/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-01-23 17:44:52.000000 cmocean-3.1.3/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-01-23 17:44:52.000000 cmocean-3.1.3/docs/whats_new.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 17:44:57.881744 cmocean-3.1.3/figures/
--rw-r--r--   0 runner    (1001) docker     (127)  1077424 2024-01-23 17:44:52.000000 cmocean-3.1.3/figures/MS08_L12.png
--rw-r--r--   0 runner    (1001) docker     (127)   919513 2024-01-23 17:44:52.000000 cmocean-3.1.3/figures/MS09_L05.png
--rw-r--r--   0 runner    (1001) docker     (127)  1084391 2024-01-23 17:44:52.000000 cmocean-3.1.3/figures/MS09_L10.png
--rw-r--r--   0 runner    (1001) docker     (127)  1172045 2024-01-23 17:44:52.000000 cmocean-3.1.3/figures/MS2_L10.png
--rw-r--r--   0 runner    (1001) docker     (127)  1148455 2024-01-23 17:44:52.000000 cmocean-3.1.3/figures/sample-data-regclimits.png
--rw-r--r--   0 runner    (1001) docker     (127)  1248342 2024-01-23 17:44:52.000000 cmocean-3.1.3/figures/sample-data-showfullcolors.png
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-23 17:44:52.000000 cmocean-3.1.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-01-23 17:44:57.881744 cmocean-3.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-01-23 17:44:52.000000 cmocean-3.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 17:44:57.881744 cmocean-3.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-01-23 17:44:52.000000 cmocean-3.1.3/tests/test_cmocean.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:39:13.687392 cmocean-4.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:39:13.659392 cmocean-4.0.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-05 21:39:08.000000 cmocean-4.0.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:39:13.659392 cmocean-4.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-05 21:39:08.000000 cmocean-4.0.1/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-05 21:39:08.000000 cmocean-4.0.1/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-05 21:39:08.000000 cmocean-4.0.1/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-05 21:39:08.000000 cmocean-4.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-05 21:39:08.000000 cmocean-4.0.1/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-05 21:39:08.000000 cmocean-4.0.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-05 21:39:08.000000 cmocean-4.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-04-05 21:39:13.687392 cmocean-4.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-04-05 21:39:08.000000 cmocean-4.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:39:13.659392 cmocean-4.0.1/ci/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-05 21:39:08.000000 cmocean-4.0.1/ci/environment-py3.10.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-05 21:39:08.000000 cmocean-4.0.1/ci/environment-py3.8.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-05 21:39:08.000000 cmocean-4.0.1/ci/environment-py3.9.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:39:13.663392 cmocean-4.0.1/cmocean/
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/cm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5315 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/plots.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:39:13.671392 cmocean-4.0.1/cmocean/rgb/
+-rw-r--r--   0 runner    (1001) docker     (127)    19200 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/algae-rgb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13687 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/algae.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19200 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/amp-rgb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13746 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/balance-blue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13641 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/balance-red.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19200 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/balance-rgb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13707 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/curl-pink.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38400 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/curl-rgb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13668 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/curl-turquoise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19200 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/deep-rgb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13710 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/deep.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13698 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/delta-blue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13740 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/delta-green.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38400 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/delta-rgb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    19200 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/dense-rgb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13693 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19200 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/diff-rgb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/diff.jscm
+-rw-r--r--   0 runner    (1001) docker     (127)    19200 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/gray-rgb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    17393 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/gray.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19200 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/haline-rgb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13698 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/haline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19200 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/ice-rgb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13796 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/ice.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:39:13.675392 cmocean-4.0.1/cmocean/rgb/inverted/
+-rw-r--r--   0 runner    (1001) docker     (127)    38400 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/inverted/algae_i-rgb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    38400 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/inverted/amp_i-rgb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    38400 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/inverted/balance_i-rgb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    38400 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/inverted/curl_i-rgb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    38400 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/inverted/deep_i-rgb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    38400 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/inverted/delta_i-rgb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    38400 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/inverted/dense_i-rgb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    38400 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/inverted/diff_i-rgb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    38400 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/inverted/gray_i-rgb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    38400 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/inverted/haline_i-rgb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    38400 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/inverted/ice_i-rgb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    38400 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/inverted/matter_i-rgb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    38400 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/inverted/oxy_i-rgb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    38400 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/inverted/phase_i-rgb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    38400 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/inverted/rain_i-rgb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    38400 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/inverted/solar_i-rgb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    38400 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/inverted/speed_i-rgb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    38400 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/inverted/tarn_i-rgb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    38400 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/inverted/tempo_i-rgb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    38400 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/inverted/thermal_i-rgb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    38400 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/inverted/topo_i-rgb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    38400 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/inverted/turbid_i-rgb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    19200 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/matter-rgb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13688 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/matter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19200 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/oxy-rgb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13666 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/oxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19200 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/phase-rgb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13873 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/phase.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19200 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/rain-rgb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/rain.jscm
+-rw-r--r--   0 runner    (1001) docker     (127)    19200 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/solar-rgb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13687 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/solar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19200 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/speed-rgb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    19200 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/tarn-rgb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/tarn.jscm
+-rw-r--r--   0 runner    (1001) docker     (127)    19200 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/tempo-rgb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    19200 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/thermal-rgb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13692 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/thermal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/topo-land.jscm
+-rw-r--r--   0 runner    (1001) docker     (127)    19200 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/topo-rgb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    19200 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/turbid-rgb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13685 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/rgb/turbid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9161 2024-04-05 21:39:08.000000 cmocean-4.0.1/cmocean/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:39:13.687392 cmocean-4.0.1/cmocean.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-04-05 21:39:13.000000 cmocean-4.0.1/cmocean.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-04-05 21:39:13.000000 cmocean-4.0.1/cmocean.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 21:39:13.000000 cmocean-4.0.1/cmocean.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-05 21:39:13.000000 cmocean-4.0.1/cmocean.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-05 21:39:13.000000 cmocean-4.0.1/cmocean.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:39:13.675392 cmocean-4.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7527 2024-04-05 21:39:08.000000 cmocean-4.0.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     7255 2024-04-05 21:39:08.000000 cmocean-4.0.1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:39:13.675392 cmocean-4.0.1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-05 21:39:08.000000 cmocean-4.0.1/docs/source/cmocean.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-05 21:39:08.000000 cmocean-4.0.1/docs/source/colormaps_viscm.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9380 2024-04-05 21:39:08.000000 cmocean-4.0.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37667 2024-04-05 21:39:08.000000 cmocean-4.0.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-05 21:39:08.000000 cmocean-4.0.1/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-05 21:39:08.000000 cmocean-4.0.1/docs/whats_new.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:39:13.683392 cmocean-4.0.1/figures/
+-rw-r--r--   0 runner    (1001) docker     (127)  1077424 2024-04-05 21:39:08.000000 cmocean-4.0.1/figures/MS08_L12.png
+-rw-r--r--   0 runner    (1001) docker     (127)   919513 2024-04-05 21:39:08.000000 cmocean-4.0.1/figures/MS09_L05.png
+-rw-r--r--   0 runner    (1001) docker     (127)  1084391 2024-04-05 21:39:08.000000 cmocean-4.0.1/figures/MS09_L10.png
+-rw-r--r--   0 runner    (1001) docker     (127)  1172045 2024-04-05 21:39:08.000000 cmocean-4.0.1/figures/MS2_L10.png
+-rw-r--r--   0 runner    (1001) docker     (127)  1148455 2024-04-05 21:39:08.000000 cmocean-4.0.1/figures/sample-data-regclimits.png
+-rw-r--r--   0 runner    (1001) docker     (127)  1248342 2024-04-05 21:39:08.000000 cmocean-4.0.1/figures/sample-data-showfullcolors.png
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-05 21:39:08.000000 cmocean-4.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-05 21:39:13.687392 cmocean-4.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-05 21:39:08.000000 cmocean-4.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:39:13.687392 cmocean-4.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-05 21:39:08.000000 cmocean-4.0.1/tests/test_cmocean.py
```

### Comparing `cmocean-3.1.3/.github/workflows/codeql.yml` & `cmocean-4.0.1/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `cmocean-3.1.3/.github/workflows/release.yaml` & `cmocean-4.0.1/.github/workflows/release.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     environment:
       name: pypi
       url: https://pypi.org/p/cmocean
     permissions:
       id-token: write  # IMPORTANT: this permission is mandatory for trusted publishing
     steps:
       - uses: actions/checkout@v4
-      - uses: actions/setup-python@v4
+      - uses: actions/setup-python@v5
       - name: Install dependencies
         run: |
           python -m pip install -U pip wheel setuptools setuptools-scm twine      
         # python -m pip install -U pip wheel "setuptools<66.0.0" setuptools-scm twine
       - name: Build distributions
         run: python setup.py sdist bdist_wheel
```

### Comparing `cmocean-3.1.3/.github/workflows/test.yaml` & `cmocean-4.0.1/.github/workflows/test.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,14 @@
         run: |
           python -m pip install -e . --no-deps --force-reinstall
       - name: Run Tests
         shell: bash -l {0}
         run: |
           pytest --cov=./ --cov-report=xml
       - name: Upload code coverage to Codecov
-        uses: codecov/codecov-action@v3
+        uses: codecov/codecov-action@v4
         with:
           file: ./coverage.xml
           flags: unittests
           env_vars: OS,PYTHON
           name: codecov-umbrella
           fail_ci_if_error: false
```

### Comparing `cmocean-3.1.3/.travis.yml` & `cmocean-4.0.1/.travis.yml`

 * *Files identical despite different names*

### Comparing `cmocean-3.1.3/LICENSE.txt` & `cmocean-4.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cmocean-3.1.3/PKG-INFO` & `cmocean-4.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmocean
-Version: 3.1.3
+Version: 4.0.1
 Summary: Colormaps for Oceanography
 Home-page: https://github.com/matplotlib/cmocean
 Author: Kristen Thyng
 Author-email: kthyng@gmail.com
 Keywords: colormaps,oceanography,plotting,visualization
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.8
```

### Comparing `cmocean-3.1.3/README.md` & `cmocean-4.0.1/README.md`

 * *Files identical despite different names*

### Comparing `cmocean-3.1.3/cmocean/cm.py` & `cmocean-4.0.1/cmocean/cm.py`

 * *Files 11% similar despite different names*

```diff
@@ -56,9 +56,29 @@
     reg_map = colors.ListedColormap(rgb_with_alpha, N=rgb.shape[0])
     _register_cmap(reg_map, name=f'cmo.{cmapname}')
 
     # Register the reversed map
     reg_map_r = colors.ListedColormap(rgb_with_alpha[::-1,:], N=rgb.shape[0])
     _register_cmap(reg_map_r, name=f'cmo.{cmapname}_r')
 
+    # Load inverted cmaps
+    rgb_i = np.loadtxt(os.path.join(datadir, 'inverted', cmapname + '_i-rgb.txt'))
+    cmap_d[cmapname + '_i'] = tools.cmap(rgb_i, N=256)
+    cmap_d[cmapname + '_i'].name = cmapname + '_i'
+    cmap_d[cmapname + '_r_i'] = tools.cmap(rgb_i[::-1, :], N=256)
+    cmap_d[cmapname + '_r_i'].name = cmapname + '_r_i'
+    rgb_with_alpha = np.zeros((rgb_i.shape[0],4))
+    rgb_with_alpha[:,:3] = rgb_i
+    rgb_with_alpha[:,3]  = 1.  #set alpha channel to 1
+
+    # Register inverted cmaps
+    reg_map_i = colors.ListedColormap(rgb_with_alpha, N=rgb_i.shape[0])
+    _register_cmap(reg_map_i, name=f'cmo.{cmapname}_i')
+    reg_map_r_i = colors.ListedColormap(rgb_with_alpha[::-1,:], N=rgb_i.shape[0])
+    _register_cmap(reg_map_r_i, name=f'cmo.{cmapname}_r_i')
+
+    # order shouldn't matter
+    cmap_d[cmapname + '_i_r'] = cmap_d[cmapname + '_r_i']
+    _register_cmap(reg_map_r_i, name=f'cmo.{cmapname}_i_r')
+
 # make colormaps available to call
 locals().update(cmap_d)
```

### Comparing `cmocean-3.1.3/cmocean/data.py` & `cmocean-4.0.1/cmocean/data.py`

 * *Files identical despite different names*

### Comparing `cmocean-3.1.3/cmocean/plots.py` & `cmocean-4.0.1/cmocean/plots.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     dc = 1.
     x = np.linspace(0.0, 1.0, 256)
     locs = []  # locations for text labels
 
     fig = plt.figure(figsize=(16, 5))
     ax = fig.add_subplot(111)
     fig.subplots_adjust(left=0.03, right=0.97)
-    ax.set_xlim(-0.1, len(cm.cmap_d)/2. + 0.1)
+    ax.set_xlim(-0.1, len(cm.cmap_d)/5. + 0.1)
     ax.set_ylim(0, 100)
     ax.set_xlabel('Lightness for each colormap', fontsize=14)
 
     for j, cmapname in enumerate(cm.cmapnames):
 
         if '_r' in cmapname:  # skip reversed versions for plot
             continue
@@ -71,20 +71,20 @@
 
     from colorspacious import cspace_converter
 
     gradient = np.linspace(0, 1, 256)
     gradient = np.vstack((gradient, gradient))
     x = np.linspace(0.0, 1.0, 256)
 
-    fig, axes = plt.subplots(nrows=int(len(cm.cmap_d)/2), ncols=1, figsize=(6, 12))
+    fig, axes = plt.subplots(nrows=int(len(cm.cmap_d)/5), ncols=1, figsize=(6, 12))
     fig.subplots_adjust(top=0.99, bottom=0.01, left=0.2, right=0.99, wspace=0.05)
 
     for ax, cmapname in zip(axes, cm.cmapnames):
 
-        if '_r' in cmapname:  # skip reversed versions for plot
+        if '_r' in cmapname or '_i' in cmapname:  # skip reversed versions for plot
             continue
 
         cmap = cm.cmap_d[cmapname]  # get the colormap instance
 
         rgb = cmap(x)[np.newaxis, :, :3]
 
         # Find a good conversion to grayscale
```

### Comparing `cmocean-3.1.3/cmocean/rgb/algae-rgb.txt` & `cmocean-4.0.1/cmocean/rgb/algae-rgb.txt`

 * *Files identical despite different names*

### Comparing `cmocean-3.1.3/cmocean/rgb/algae.py` & `cmocean-4.0.1/cmocean/rgb/algae.py`

 * *Files identical despite different names*

### Comparing `cmocean-3.1.3/cmocean/rgb/amp-rgb.txt` & `cmocean-4.0.1/cmocean/rgb/amp-rgb.txt`

 * *Files identical despite different names*

### Comparing `cmocean-3.1.3/cmocean/rgb/balance-blue.py` & `cmocean-4.0.1/cmocean/rgb/balance-blue.py`

 * *Files identical despite different names*

### Comparing `cmocean-3.1.3/cmocean/rgb/balance-red.py` & `cmocean-4.0.1/cmocean/rgb/balance-red.py`

 * *Files identical despite different names*

### Comparing `cmocean-3.1.3/cmocean/rgb/balance-rgb.txt` & `cmocean-4.0.1/cmocean/rgb/balance-rgb.txt`

 * *Files identical despite different names*

### Comparing `cmocean-3.1.3/cmocean/rgb/curl-pink.py` & `cmocean-4.0.1/cmocean/rgb/curl-pink.py`

 * *Files identical despite different names*

### Comparing `cmocean-3.1.3/cmocean/rgb/curl-rgb.txt` & `cmocean-4.0.1/cmocean/rgb/curl-rgb.txt`

 * *Files identical despite different names*

### Comparing `cmocean-3.1.3/cmocean/rgb/curl-turquoise.py` & `cmocean-4.0.1/cmocean/rgb/curl-turquoise.py`

 * *Files identical despite different names*

### Comparing `cmocean-3.1.3/cmocean/rgb/deep-rgb.txt` & `cmocean-4.0.1/cmocean/rgb/deep-rgb.txt`

 * *Files identical despite different names*

### Comparing `cmocean-3.1.3/cmocean/rgb/deep.py` & `cmocean-4.0.1/cmocean/rgb/deep.py`

 * *Files identical despite different names*

### Comparing `cmocean-3.1.3/cmocean/rgb/delta-blue.py` & `cmocean-4.0.1/cmocean/rgb/delta-blue.py`

 * *Files identical despite different names*

### Comparing `cmocean-3.1.3/cmocean/rgb/delta-green.py` & `cmocean-4.0.1/cmocean/rgb/delta-green.py`

 * *Files identical despite different names*

### Comparing `cmocean-3.1.3/cmocean/rgb/delta-rgb.txt` & `cmocean-4.0.1/cmocean/rgb/delta-rgb.txt`

 * *Files identical despite different names*

### Comparing `cmocean-3.1.3/cmocean/rgb/dense-rgb.txt` & `cmocean-4.0.1/cmocean/rgb/dense-rgb.txt`

 * *Files identical despite different names*

### Comparing `cmocean-3.1.3/cmocean/rgb/dense.py` & `cmocean-4.0.1/cmocean/rgb/dense.py`

 * *Files identical despite different names*

### Comparing `cmocean-3.1.3/cmocean/rgb/diff-rgb.txt` & `cmocean-4.0.1/cmocean/rgb/diff-rgb.txt`

 * *Files identical despite different names*

### Comparing `cmocean-3.1.3/cmocean/rgb/diff.jscm` & `cmocean-4.0.1/cmocean/rgb/diff.jscm`

 * *Files identical despite different names*

### Comparing `cmocean-3.1.3/cmocean/rgb/gray-rgb.txt` & `cmocean-4.0.1/cmocean/rgb/gray-rgb.txt`

 * *Files identical despite different names*

### Comparing `cmocean-3.1.3/cmocean/rgb/gray.py` & `cmocean-4.0.1/cmocean/rgb/gray.py`

 * *Files identical despite different names*

### Comparing `cmocean-3.1.3/cmocean/rgb/haline-rgb.txt` & `cmocean-4.0.1/cmocean/rgb/haline-rgb.txt`

 * *Files identical despite different names*

### Comparing `cmocean-3.1.3/cmocean/rgb/haline.py` & `cmocean-4.0.1/cmocean/rgb/haline.py`

 * *Files identical despite different names*

### Comparing `cmocean-3.1.3/cmocean/rgb/ice-rgb.txt` & `cmocean-4.0.1/cmocean/rgb/ice-rgb.txt`

 * *Files identical despite different names*

### Comparing `cmocean-3.1.3/cmocean/rgb/ice.py` & `cmocean-4.0.1/cmocean/rgb/ice.py`

 * *Files identical despite different names*

### Comparing `cmocean-3.1.3/cmocean/rgb/matter-rgb.txt` & `cmocean-4.0.1/cmocean/rgb/matter-rgb.txt`

 * *Files identical despite different names*

### Comparing `cmocean-3.1.3/cmocean/rgb/matter.py` & `cmocean-4.0.1/cmocean/rgb/matter.py`

 * *Files identical despite different names*

### Comparing `cmocean-3.1.3/cmocean/rgb/oxy-rgb.txt` & `cmocean-4.0.1/cmocean/rgb/oxy-rgb.txt`

 * *Files identical despite different names*

### Comparing `cmocean-3.1.3/cmocean/rgb/oxy.py` & `cmocean-4.0.1/cmocean/rgb/oxy.py`

 * *Files identical despite different names*

### Comparing `cmocean-3.1.3/cmocean/rgb/phase-rgb.txt` & `cmocean-4.0.1/cmocean/rgb/phase-rgb.txt`

 * *Files identical despite different names*

### Comparing `cmocean-3.1.3/cmocean/rgb/phase.py` & `cmocean-4.0.1/cmocean/rgb/phase.py`

 * *Files identical despite different names*

### Comparing `cmocean-3.1.3/cmocean/rgb/rain-rgb.txt` & `cmocean-4.0.1/cmocean/rgb/rain-rgb.txt`

 * *Files identical despite different names*

### Comparing `cmocean-3.1.3/cmocean/rgb/rain.jscm` & `cmocean-4.0.1/cmocean/rgb/rain.jscm`

 * *Files identical despite different names*

### Comparing `cmocean-3.1.3/cmocean/rgb/solar-rgb.txt` & `cmocean-4.0.1/cmocean/rgb/solar-rgb.txt`

 * *Files identical despite different names*

### Comparing `cmocean-3.1.3/cmocean/rgb/solar.py` & `cmocean-4.0.1/cmocean/rgb/solar.py`

 * *Files identical despite different names*

### Comparing `cmocean-3.1.3/cmocean/rgb/speed-rgb.txt` & `cmocean-4.0.1/cmocean/rgb/speed-rgb.txt`

 * *Files identical despite different names*

### Comparing `cmocean-3.1.3/cmocean/rgb/tarn-rgb.txt` & `cmocean-4.0.1/cmocean/rgb/tarn-rgb.txt`

 * *Files identical despite different names*

### Comparing `cmocean-3.1.3/cmocean/rgb/tarn.jscm` & `cmocean-4.0.1/cmocean/rgb/tarn.jscm`

 * *Files identical despite different names*

### Comparing `cmocean-3.1.3/cmocean/rgb/tempo-rgb.txt` & `cmocean-4.0.1/cmocean/rgb/tempo-rgb.txt`

 * *Files identical despite different names*

### Comparing `cmocean-3.1.3/cmocean/rgb/thermal-rgb.txt` & `cmocean-4.0.1/cmocean/rgb/thermal-rgb.txt`

 * *Files identical despite different names*

### Comparing `cmocean-3.1.3/cmocean/rgb/thermal.py` & `cmocean-4.0.1/cmocean/rgb/thermal.py`

 * *Files identical despite different names*

### Comparing `cmocean-3.1.3/cmocean/rgb/topo-land.jscm` & `cmocean-4.0.1/cmocean/rgb/topo-land.jscm`

 * *Files identical despite different names*

### Comparing `cmocean-3.1.3/cmocean/rgb/topo-rgb.txt` & `cmocean-4.0.1/cmocean/rgb/topo-rgb.txt`

 * *Files identical despite different names*

### Comparing `cmocean-3.1.3/cmocean/rgb/turbid-rgb.txt` & `cmocean-4.0.1/cmocean/rgb/turbid-rgb.txt`

 * *Files identical despite different names*

### Comparing `cmocean-3.1.3/cmocean/rgb/turbid.py` & `cmocean-4.0.1/cmocean/rgb/turbid.py`

 * *Files identical despite different names*

### Comparing `cmocean-3.1.3/cmocean/tools.py` & `cmocean-4.0.1/cmocean/tools.py`

 * *Files identical despite different names*

### Comparing `cmocean-3.1.3/cmocean.egg-info/PKG-INFO` & `cmocean-4.0.1/cmocean.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmocean
-Version: 3.1.3
+Version: 4.0.1
 Summary: Colormaps for Oceanography
 Home-page: https://github.com/matplotlib/cmocean
 Author: Kristen Thyng
 Author-email: kthyng@gmail.com
 Keywords: colormaps,oceanography,plotting,visualization
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.8
```

### Comparing `cmocean-3.1.3/docs/Makefile` & `cmocean-4.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cmocean-3.1.3/docs/make.bat` & `cmocean-4.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cmocean-3.1.3/docs/source/cmocean.rst` & `cmocean-4.0.1/docs/source/cmocean.rst`

 * *Files identical despite different names*

### Comparing `cmocean-3.1.3/docs/source/conf.py` & `cmocean-4.0.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `cmocean-3.1.3/docs/source/index.rst` & `cmocean-4.0.1/docs/source/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -129,14 +129,30 @@
    fig = plt.figure(figsize=(8, 3))
    ax = fig.add_subplot(1, 2, 1)
    cmocean.plots.test(cmocean.cm.gray, ax=ax)
    ax = fig.add_subplot(1, 2, 2)
    cmocean.plots.test(cmocean.cm.gray_r, ax=ax)
    fig.tight_layout()
 
+Inverted lightness versions of all colormaps are available by appending "_i" to the colormap name. This is particularly useful for diverging colormaps used on light backgrounds:
+
+.. plot::
+   :include-source:
+
+   import cmocean
+   import matplotlib.pyplot as plt
+
+   fig = plt.figure(figsize=(8, 3))
+   ax = fig.add_subplot(1, 2, 1)
+   cmocean.plots.test(cmocean.cm.balance, ax=ax)
+   ax = fig.add_subplot(1, 2, 2)
+   cmocean.plots.test(cmocean.cm.balance_i, ax=ax)
+   fig.tight_layout()
+
+Reversed and inverted lightness versions of all colormaps are available by appending "_r_i" or "_i_r" to the colormap name, e.g., ``cmocean.cm.balance_i_r``.
 
 You can lighten a colormap using an alpha value below 1 with the `cmocean.tools.lighten()` function so that you can overlay contours and other lines that are more easily visible:
 
 .. plot::
    :include-source:
 
    import cmocean
```

### Comparing `cmocean-3.1.3/docs/whats_new.md` & `cmocean-4.0.1/docs/whats_new.md`

 * *Files identical despite different names*

### Comparing `cmocean-3.1.3/figures/MS08_L12.png` & `cmocean-4.0.1/figures/MS08_L12.png`

 * *Files identical despite different names*

### Comparing `cmocean-3.1.3/figures/MS09_L05.png` & `cmocean-4.0.1/figures/MS09_L05.png`

 * *Files identical despite different names*

### Comparing `cmocean-3.1.3/figures/MS09_L10.png` & `cmocean-4.0.1/figures/MS09_L10.png`

 * *Files identical despite different names*

### Comparing `cmocean-3.1.3/figures/MS2_L10.png` & `cmocean-4.0.1/figures/MS2_L10.png`

 * *Files identical despite different names*

### Comparing `cmocean-3.1.3/figures/sample-data-regclimits.png` & `cmocean-4.0.1/figures/sample-data-regclimits.png`

 * *Files identical despite different names*

### Comparing `cmocean-3.1.3/figures/sample-data-showfullcolors.png` & `cmocean-4.0.1/figures/sample-data-showfullcolors.png`

 * *Files identical despite different names*

### Comparing `cmocean-3.1.3/setup.py` & `cmocean-4.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     'plots':  ["colorspacious", "viscm"],
 }
 # # in case I add more later
 # extras_require['complete'] = sorted(set(sum(extras_require.values(), [])))
 
 setup(
     name = "cmocean",
-    version = "v3.1.3",
+    version = "v4.0.1",
     author = "Kristen Thyng",
     author_email = "kthyng@gmail.com",
     url = 'https://github.com/matplotlib/cmocean',
     # download_url = 'https://github.com/matplotlib/cmocean/tarball/2.0',
     description = ("Colormaps for Oceanography"),
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

### Comparing `cmocean-3.1.3/tests/test_cmocean.py` & `cmocean-4.0.1/tests/test_cmocean.py`

 * *Files identical despite different names*

