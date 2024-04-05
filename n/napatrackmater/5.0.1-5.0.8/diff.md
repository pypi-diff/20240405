# Comparing `tmp/napatrackmater-5.0.1.tar.gz` & `tmp/napatrackmater-5.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napatrackmater-5.0.1.tar", last modified: Mon Mar 25 10:23:49 2024, max compression
+gzip compressed data, was "napatrackmater-5.0.8.tar", last modified: Fri Apr  5 21:37:31 2024, max compression
```

## Comparing `napatrackmater-5.0.1.tar` & `napatrackmater-5.0.8.tar`

### file list

```diff
@@ -1,281 +1,281 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.316784 napatrackmater-5.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.272784 napatrackmater-5.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.288784 napatrackmater-5.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9639 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/MASTER.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.288784 napatrackmater-5.0.1/Notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)    13692 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/Notebooks/Track_vector.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4463 2024-03-25 10:23:49.316784 napatrackmater-5.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.284784 napatrackmater-5.0.1/_build/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.288784 napatrackmater-5.0.1/_build/.doctrees/
--rw-r--r--   0 runner    (1001) docker     (127)    33531 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/.doctrees/MASTER.doctree
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.288784 napatrackmater-5.0.1/_build/.doctrees/Notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)    29083 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/.doctrees/Notebooks/Track_vector.doctree
--rw-r--r--   0 runner    (1001) docker     (127)    11990 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/.doctrees/README.doctree
--rw-r--r--   0 runner    (1001) docker     (127)    36454 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/.doctrees/environment.pickle
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.288784 napatrackmater-5.0.1/_build/html/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/.buildinfo
--rw-r--r--   0 runner    (1001) docker     (127)    29915 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/MASTER.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.288784 napatrackmater-5.0.1/_build/html/Notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)    66062 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/Notebooks/Track_vector.html
--rw-r--r--   0 runner    (1001) docker     (127)    18885 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/README.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.288784 napatrackmater-5.0.1/_build/html/_images/
--rw-r--r--   0 runner    (1001) docker     (127)    20293 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_images/ClusterDistributionPlot_time_point_97.png
--rw-r--r--   0 runner    (1001) docker     (127)    29672 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_images/ClusterNearnessPlot_time_point_97.png
--rw-r--r--   0 runner    (1001) docker     (127)   162373 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_images/ClusterPlot_time_point_97.png
--rw-r--r--   0 runner    (1001) docker     (127)    61613 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_images/FeatureMatrixPlot_time_point_97.png
--rw-r--r--   0 runner    (1001) docker     (127)    66872 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_images/QuadrantDistributionPlot_time_point_97.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.292784 napatrackmater-5.0.1/_build/html/_sources/
--rw-r--r--   0 runner    (1001) docker     (127)     9639 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_sources/MASTER.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.292784 napatrackmater-5.0.1/_build/html/_sources/Notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)    13692 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_sources/Notebooks/Track_vector.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_sources/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.292784 napatrackmater-5.0.1/_build/html/_sphinx_design_static/
--rw-r--r--   0 runner    (1001) docker     (127)    48417 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_sphinx_design_static/design-style.4045f2051d55cab465a707391d5b2007.min.css
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_sphinx_design_static/design-tabs.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.296784 napatrackmater-5.0.1/_build/html/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    14692 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/basic.css
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/check-solid.svg
--rw-r--r--   0 runner    (1001) docker     (127)     9031 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/clipboard.min.js
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/copy-button.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/copybutton.css
--rw-r--r--   0 runner    (1001) docker     (127)     8467 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/copybutton.js
--rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/copybutton_funcs.js
--rw-r--r--   0 runner    (1001) docker     (127)    48417 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/design-style.4045f2051d55cab465a707391d5b2007.min.css
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/design-tabs.js
--rw-r--r--   0 runner    (1001) docker     (127)    10766 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/doctools.js
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/documentation_options.js
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/file.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.296784 napatrackmater-5.0.1/_build/html/_static/images/
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/images/logo_binder.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7601 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/images/logo_colab.png
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/images/logo_deepnote.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/images/logo_jupyterhub.svg
--rw-r--r--   0 runner    (1001) docker     (127)   287630 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/jquery-3.5.1.js
--rw-r--r--   0 runner    (1001) docker     (127)    89476 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/jquery.js
--rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/kapoorlablogo.png
--rw-r--r--   0 runner    (1001) docker     (127)    10854 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/language_data.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.284784 napatrackmater-5.0.1/_build/html/_static/locales/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.276784 napatrackmater-5.0.1/_build/html/_static/locales/ar/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.296784 napatrackmater-5.0.1/_build/html/_static/locales/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/locales/ar/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.276784 napatrackmater-5.0.1/_build/html/_static/locales/bg/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.296784 napatrackmater-5.0.1/_build/html/_static/locales/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/locales/bg/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.276784 napatrackmater-5.0.1/_build/html/_static/locales/bn/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.296784 napatrackmater-5.0.1/_build/html/_static/locales/bn/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/locales/bn/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.276784 napatrackmater-5.0.1/_build/html/_static/locales/ca/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.296784 napatrackmater-5.0.1/_build/html/_static/locales/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/locales/ca/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.276784 napatrackmater-5.0.1/_build/html/_static/locales/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.296784 napatrackmater-5.0.1/_build/html/_static/locales/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/locales/cs/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.276784 napatrackmater-5.0.1/_build/html/_static/locales/da/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.296784 napatrackmater-5.0.1/_build/html/_static/locales/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/locales/da/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.276784 napatrackmater-5.0.1/_build/html/_static/locales/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.296784 napatrackmater-5.0.1/_build/html/_static/locales/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/locales/de/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.276784 napatrackmater-5.0.1/_build/html/_static/locales/el/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.296784 napatrackmater-5.0.1/_build/html/_static/locales/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/locales/el/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.276784 napatrackmater-5.0.1/_build/html/_static/locales/eo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.296784 napatrackmater-5.0.1/_build/html/_static/locales/eo/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/locales/eo/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.276784 napatrackmater-5.0.1/_build/html/_static/locales/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.300784 napatrackmater-5.0.1/_build/html/_static/locales/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/locales/es/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.276784 napatrackmater-5.0.1/_build/html/_static/locales/et/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.300784 napatrackmater-5.0.1/_build/html/_static/locales/et/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/locales/et/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.276784 napatrackmater-5.0.1/_build/html/_static/locales/fi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.300784 napatrackmater-5.0.1/_build/html/_static/locales/fi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/locales/fi/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.276784 napatrackmater-5.0.1/_build/html/_static/locales/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.300784 napatrackmater-5.0.1/_build/html/_static/locales/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/locales/fr/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.276784 napatrackmater-5.0.1/_build/html/_static/locales/hr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.300784 napatrackmater-5.0.1/_build/html/_static/locales/hr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/locales/hr/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.276784 napatrackmater-5.0.1/_build/html/_static/locales/id/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.300784 napatrackmater-5.0.1/_build/html/_static/locales/id/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/locales/id/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.276784 napatrackmater-5.0.1/_build/html/_static/locales/it/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.300784 napatrackmater-5.0.1/_build/html/_static/locales/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/locales/it/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.276784 napatrackmater-5.0.1/_build/html/_static/locales/iw/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.300784 napatrackmater-5.0.1/_build/html/_static/locales/iw/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/locales/iw/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.276784 napatrackmater-5.0.1/_build/html/_static/locales/ja/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.300784 napatrackmater-5.0.1/_build/html/_static/locales/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/locales/ja/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.276784 napatrackmater-5.0.1/_build/html/_static/locales/ko/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.300784 napatrackmater-5.0.1/_build/html/_static/locales/ko/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/locales/ko/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.276784 napatrackmater-5.0.1/_build/html/_static/locales/lt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.300784 napatrackmater-5.0.1/_build/html/_static/locales/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/locales/lt/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.280784 napatrackmater-5.0.1/_build/html/_static/locales/lv/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.300784 napatrackmater-5.0.1/_build/html/_static/locales/lv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/locales/lv/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.280784 napatrackmater-5.0.1/_build/html/_static/locales/ml/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.300784 napatrackmater-5.0.1/_build/html/_static/locales/ml/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/locales/ml/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.280784 napatrackmater-5.0.1/_build/html/_static/locales/mr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.300784 napatrackmater-5.0.1/_build/html/_static/locales/mr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/locales/mr/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.280784 napatrackmater-5.0.1/_build/html/_static/locales/ms/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.300784 napatrackmater-5.0.1/_build/html/_static/locales/ms/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/locales/ms/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.280784 napatrackmater-5.0.1/_build/html/_static/locales/nl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.300784 napatrackmater-5.0.1/_build/html/_static/locales/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/locales/nl/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.280784 napatrackmater-5.0.1/_build/html/_static/locales/no/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.300784 napatrackmater-5.0.1/_build/html/_static/locales/no/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/locales/no/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.280784 napatrackmater-5.0.1/_build/html/_static/locales/pl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.300784 napatrackmater-5.0.1/_build/html/_static/locales/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/locales/pl/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.280784 napatrackmater-5.0.1/_build/html/_static/locales/pt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.300784 napatrackmater-5.0.1/_build/html/_static/locales/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/locales/pt/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.280784 napatrackmater-5.0.1/_build/html/_static/locales/ro/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.300784 napatrackmater-5.0.1/_build/html/_static/locales/ro/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/locales/ro/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.280784 napatrackmater-5.0.1/_build/html/_static/locales/ru/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.300784 napatrackmater-5.0.1/_build/html/_static/locales/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/locales/ru/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.280784 napatrackmater-5.0.1/_build/html/_static/locales/sk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.300784 napatrackmater-5.0.1/_build/html/_static/locales/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/locales/sk/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.280784 napatrackmater-5.0.1/_build/html/_static/locales/sl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.300784 napatrackmater-5.0.1/_build/html/_static/locales/sl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/locales/sl/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.280784 napatrackmater-5.0.1/_build/html/_static/locales/sr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.300784 napatrackmater-5.0.1/_build/html/_static/locales/sr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/locales/sr/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.280784 napatrackmater-5.0.1/_build/html/_static/locales/sv/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.300784 napatrackmater-5.0.1/_build/html/_static/locales/sv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/locales/sv/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.280784 napatrackmater-5.0.1/_build/html/_static/locales/ta/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.304784 napatrackmater-5.0.1/_build/html/_static/locales/ta/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/locales/ta/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.280784 napatrackmater-5.0.1/_build/html/_static/locales/te/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.304784 napatrackmater-5.0.1/_build/html/_static/locales/te/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/locales/te/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.280784 napatrackmater-5.0.1/_build/html/_static/locales/tg/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.304784 napatrackmater-5.0.1/_build/html/_static/locales/tg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/locales/tg/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.280784 napatrackmater-5.0.1/_build/html/_static/locales/th/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.304784 napatrackmater-5.0.1/_build/html/_static/locales/th/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/locales/th/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.280784 napatrackmater-5.0.1/_build/html/_static/locales/tl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.304784 napatrackmater-5.0.1/_build/html/_static/locales/tl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/locales/tl/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.280784 napatrackmater-5.0.1/_build/html/_static/locales/tr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.304784 napatrackmater-5.0.1/_build/html/_static/locales/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/locales/tr/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.280784 napatrackmater-5.0.1/_build/html/_static/locales/uk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.304784 napatrackmater-5.0.1/_build/html/_static/locales/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/locales/uk/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.284784 napatrackmater-5.0.1/_build/html/_static/locales/ur/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.304784 napatrackmater-5.0.1/_build/html/_static/locales/ur/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/locales/ur/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.284784 napatrackmater-5.0.1/_build/html/_static/locales/vi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.304784 napatrackmater-5.0.1/_build/html/_static/locales/vi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/locales/vi/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.284784 napatrackmater-5.0.1/_build/html/_static/locales/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.304784 napatrackmater-5.0.1/_build/html/_static/locales/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.284784 napatrackmater-5.0.1/_build/html/_static/locales/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.304784 napatrackmater-5.0.1/_build/html/_static/locales/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.po
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/minus.png
--rw-r--r--   0 runner    (1001) docker     (127)    39364 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/plus.png
--rw-r--r--   0 runner    (1001) docker     (127)    12757 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/pygments.css
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/sbt-webpack-macros.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.304784 napatrackmater-5.0.1/_build/html/_static/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)    80813 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/scripts/bootstrap.js
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/scripts/bootstrap.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)   335757 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/scripts/bootstrap.js.map
--rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/scripts/pydata-sphinx-theme.js
--rw-r--r--   0 runner    (1001) docker     (127)    19648 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/scripts/pydata-sphinx-theme.js.map
--rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/scripts/sphinx-book-theme.js
--rw-r--r--   0 runner    (1001) docker     (127)    13066 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/scripts/sphinx-book-theme.js.map
--rw-r--r--   0 runner    (1001) docker     (127)    16634 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/searchtools.js
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/sphinx-thebe.css
--rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/sphinx-thebe.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.308784 napatrackmater-5.0.1/_build/html/_static/styles/
--rw-r--r--   0 runner    (1001) docker     (127)   176654 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/styles/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)    63341 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/styles/pydata-sphinx-theme.css
--rw-r--r--   0 runner    (1001) docker     (127)    13841 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/styles/sphinx-book-theme.css
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/styles/theme.css
--rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/togglebutton.css
--rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/togglebutton.js
--rw-r--r--   0 runner    (1001) docker     (127)    68420 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/underscore-1.13.1.js
--rw-r--r--   0 runner    (1001) docker     (127)    19530 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/underscore.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.284784 napatrackmater-5.0.1/_build/html/_static/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.284784 napatrackmater-5.0.1/_build/html/_static/vendor/fontawesome/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.308784 napatrackmater-5.0.1/_build/html/_static/vendor/fontawesome/6.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     7427 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/vendor/fontawesome/6.1.2/LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.308784 napatrackmater-5.0.1/_build/html/_static/vendor/fontawesome/6.1.2/css/
--rw-r--r--   0 runner    (1001) docker     (127)   101691 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/vendor/fontawesome/6.1.2/css/all.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.308784 napatrackmater-5.0.1/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/
--rw-r--r--   0 runner    (1001) docker     (127)   181264 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   105112 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    60236 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    24028 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   389948 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   154840 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    10084 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/_static/webpack-macros.html
--rw-r--r--   0 runner    (1001) docker     (127)    11198 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/genindex.html
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/objects.inv
--rw-r--r--   0 runner    (1001) docker     (127)    12010 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/search.html
--rw-r--r--   0 runner    (1001) docker     (127)     7816 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/html/searchindex.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.284784 napatrackmater-5.0.1/_build/jupyter_execute/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.308784 napatrackmater-5.0.1/_build/jupyter_execute/Notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)    17500 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_build/jupyter_execute/Notebooks/Track_vector.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/_toc.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.312784 napatrackmater-5.0.1/images/
--rw-r--r--   0 runner    (1001) docker     (127)    20293 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/images/ClusterDistributionPlot_time_point_97.png
--rw-r--r--   0 runner    (1001) docker     (127)    29672 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/images/ClusterNearnessPlot_time_point_97.png
--rw-r--r--   0 runner    (1001) docker     (127)   162373 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/images/ClusterPlot_time_point_97.png
--rw-r--r--   0 runner    (1001) docker     (127)    61613 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/images/FeatureMatrixPlot_time_point_97.png
--rw-r--r--   0 runner    (1001) docker     (127)    66872 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/images/QuadrantDistributionPlot_time_point_97.png
--rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/images/kapoorlablogo.png
--rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/images/kapoorlogo.png
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-03-25 10:23:49.316784 napatrackmater-5.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.284784 napatrackmater-5.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.312784 napatrackmater-5.0.1/src/napatrackmater/
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/src/napatrackmater/CloudAutoEncoder.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/src/napatrackmater/DeepEmbeddedClustering.py
--rw-r--r--   0 runner    (1001) docker     (127)   123805 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/src/napatrackmater/Trackmate.py
--rw-r--r--   0 runner    (1001) docker     (127)   113055 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/src/napatrackmater/Trackvector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/src/napatrackmater/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/src/napatrackmater/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    25353 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/src/napatrackmater/clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/src/napatrackmater/fast_radius_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)    13035 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/src/napatrackmater/fate_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     6603 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/src/napatrackmater/pretrained.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:23:49.312784 napatrackmater-5.0.1/src/napatrackmater.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4463 2024-03-25 10:23:49.000000 napatrackmater-5.0.1/src/napatrackmater.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-03-25 10:23:49.000000 napatrackmater-5.0.1/src/napatrackmater.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 10:23:49.000000 napatrackmater-5.0.1/src/napatrackmater.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-03-25 10:23:49.000000 napatrackmater-5.0.1/src/napatrackmater.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-25 10:23:49.000000 napatrackmater-5.0.1/src/napatrackmater.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-03-25 10:23:37.000000 napatrackmater-5.0.1/update_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.384440 napatrackmater-5.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.340440 napatrackmater-5.0.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.356440 napatrackmater-5.0.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9639 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/MASTER.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.356440 napatrackmater-5.0.8/Notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)    13692 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/Notebooks/Track_vector.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4463 2024-04-05 21:37:31.384440 napatrackmater-5.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.352440 napatrackmater-5.0.8/_build/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.356440 napatrackmater-5.0.8/_build/.doctrees/
+-rw-r--r--   0 runner    (1001) docker     (127)    33531 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/.doctrees/MASTER.doctree
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.356440 napatrackmater-5.0.8/_build/.doctrees/Notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)    29083 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/.doctrees/Notebooks/Track_vector.doctree
+-rw-r--r--   0 runner    (1001) docker     (127)    11990 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/.doctrees/README.doctree
+-rw-r--r--   0 runner    (1001) docker     (127)    36454 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/.doctrees/environment.pickle
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.356440 napatrackmater-5.0.8/_build/html/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/.buildinfo
+-rw-r--r--   0 runner    (1001) docker     (127)    29915 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/MASTER.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.356440 napatrackmater-5.0.8/_build/html/Notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)    66062 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/Notebooks/Track_vector.html
+-rw-r--r--   0 runner    (1001) docker     (127)    18885 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/README.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.360440 napatrackmater-5.0.8/_build/html/_images/
+-rw-r--r--   0 runner    (1001) docker     (127)    20293 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_images/ClusterDistributionPlot_time_point_97.png
+-rw-r--r--   0 runner    (1001) docker     (127)    29672 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_images/ClusterNearnessPlot_time_point_97.png
+-rw-r--r--   0 runner    (1001) docker     (127)   162373 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_images/ClusterPlot_time_point_97.png
+-rw-r--r--   0 runner    (1001) docker     (127)    61613 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_images/FeatureMatrixPlot_time_point_97.png
+-rw-r--r--   0 runner    (1001) docker     (127)    66872 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_images/QuadrantDistributionPlot_time_point_97.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.360440 napatrackmater-5.0.8/_build/html/_sources/
+-rw-r--r--   0 runner    (1001) docker     (127)     9639 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_sources/MASTER.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.360440 napatrackmater-5.0.8/_build/html/_sources/Notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)    13692 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_sources/Notebooks/Track_vector.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_sources/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.360440 napatrackmater-5.0.8/_build/html/_sphinx_design_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    48417 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_sphinx_design_static/design-style.4045f2051d55cab465a707391d5b2007.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_sphinx_design_static/design-tabs.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.364440 napatrackmater-5.0.8/_build/html/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    14692 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/basic.css
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/check-solid.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     9031 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/clipboard.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/copy-button.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/copybutton.css
+-rw-r--r--   0 runner    (1001) docker     (127)     8467 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/copybutton.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/copybutton_funcs.js
+-rw-r--r--   0 runner    (1001) docker     (127)    48417 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/design-style.4045f2051d55cab465a707391d5b2007.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/design-tabs.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10766 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/doctools.js
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/documentation_options.js
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/file.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.364440 napatrackmater-5.0.8/_build/html/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/images/logo_binder.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7601 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/images/logo_colab.png
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/images/logo_deepnote.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/images/logo_jupyterhub.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   287630 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/jquery-3.5.1.js
+-rw-r--r--   0 runner    (1001) docker     (127)    89476 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/jquery.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/kapoorlablogo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10854 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/language_data.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.352440 napatrackmater-5.0.8/_build/html/_static/locales/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.340440 napatrackmater-5.0.8/_build/html/_static/locales/ar/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.364440 napatrackmater-5.0.8/_build/html/_static/locales/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/locales/ar/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.340440 napatrackmater-5.0.8/_build/html/_static/locales/bg/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.364440 napatrackmater-5.0.8/_build/html/_static/locales/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/locales/bg/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.340440 napatrackmater-5.0.8/_build/html/_static/locales/bn/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.364440 napatrackmater-5.0.8/_build/html/_static/locales/bn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/locales/bn/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.344440 napatrackmater-5.0.8/_build/html/_static/locales/ca/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.364440 napatrackmater-5.0.8/_build/html/_static/locales/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/locales/ca/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.344440 napatrackmater-5.0.8/_build/html/_static/locales/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.364440 napatrackmater-5.0.8/_build/html/_static/locales/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/locales/cs/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.344440 napatrackmater-5.0.8/_build/html/_static/locales/da/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.364440 napatrackmater-5.0.8/_build/html/_static/locales/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/locales/da/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.344440 napatrackmater-5.0.8/_build/html/_static/locales/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.368440 napatrackmater-5.0.8/_build/html/_static/locales/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/locales/de/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.344440 napatrackmater-5.0.8/_build/html/_static/locales/el/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.368440 napatrackmater-5.0.8/_build/html/_static/locales/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/locales/el/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.344440 napatrackmater-5.0.8/_build/html/_static/locales/eo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.368440 napatrackmater-5.0.8/_build/html/_static/locales/eo/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/locales/eo/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.344440 napatrackmater-5.0.8/_build/html/_static/locales/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.368440 napatrackmater-5.0.8/_build/html/_static/locales/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/locales/es/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.344440 napatrackmater-5.0.8/_build/html/_static/locales/et/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.368440 napatrackmater-5.0.8/_build/html/_static/locales/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/locales/et/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.344440 napatrackmater-5.0.8/_build/html/_static/locales/fi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.368440 napatrackmater-5.0.8/_build/html/_static/locales/fi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/locales/fi/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.344440 napatrackmater-5.0.8/_build/html/_static/locales/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.368440 napatrackmater-5.0.8/_build/html/_static/locales/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/locales/fr/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.344440 napatrackmater-5.0.8/_build/html/_static/locales/hr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.368440 napatrackmater-5.0.8/_build/html/_static/locales/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/locales/hr/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.344440 napatrackmater-5.0.8/_build/html/_static/locales/id/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.368440 napatrackmater-5.0.8/_build/html/_static/locales/id/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/locales/id/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.344440 napatrackmater-5.0.8/_build/html/_static/locales/it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.368440 napatrackmater-5.0.8/_build/html/_static/locales/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/locales/it/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.344440 napatrackmater-5.0.8/_build/html/_static/locales/iw/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.368440 napatrackmater-5.0.8/_build/html/_static/locales/iw/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/locales/iw/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.344440 napatrackmater-5.0.8/_build/html/_static/locales/ja/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.368440 napatrackmater-5.0.8/_build/html/_static/locales/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/locales/ja/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.344440 napatrackmater-5.0.8/_build/html/_static/locales/ko/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.368440 napatrackmater-5.0.8/_build/html/_static/locales/ko/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/locales/ko/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.344440 napatrackmater-5.0.8/_build/html/_static/locales/lt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.368440 napatrackmater-5.0.8/_build/html/_static/locales/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/locales/lt/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.344440 napatrackmater-5.0.8/_build/html/_static/locales/lv/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.368440 napatrackmater-5.0.8/_build/html/_static/locales/lv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/locales/lv/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.344440 napatrackmater-5.0.8/_build/html/_static/locales/ml/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.368440 napatrackmater-5.0.8/_build/html/_static/locales/ml/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/locales/ml/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.348440 napatrackmater-5.0.8/_build/html/_static/locales/mr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.368440 napatrackmater-5.0.8/_build/html/_static/locales/mr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/locales/mr/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.348440 napatrackmater-5.0.8/_build/html/_static/locales/ms/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.368440 napatrackmater-5.0.8/_build/html/_static/locales/ms/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/locales/ms/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.348440 napatrackmater-5.0.8/_build/html/_static/locales/nl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.368440 napatrackmater-5.0.8/_build/html/_static/locales/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/locales/nl/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.348440 napatrackmater-5.0.8/_build/html/_static/locales/no/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.368440 napatrackmater-5.0.8/_build/html/_static/locales/no/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/locales/no/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.348440 napatrackmater-5.0.8/_build/html/_static/locales/pl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.368440 napatrackmater-5.0.8/_build/html/_static/locales/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/locales/pl/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.348440 napatrackmater-5.0.8/_build/html/_static/locales/pt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.368440 napatrackmater-5.0.8/_build/html/_static/locales/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/locales/pt/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.348440 napatrackmater-5.0.8/_build/html/_static/locales/ro/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.368440 napatrackmater-5.0.8/_build/html/_static/locales/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/locales/ro/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.348440 napatrackmater-5.0.8/_build/html/_static/locales/ru/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.368440 napatrackmater-5.0.8/_build/html/_static/locales/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/locales/ru/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.348440 napatrackmater-5.0.8/_build/html/_static/locales/sk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.368440 napatrackmater-5.0.8/_build/html/_static/locales/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/locales/sk/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.348440 napatrackmater-5.0.8/_build/html/_static/locales/sl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.368440 napatrackmater-5.0.8/_build/html/_static/locales/sl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/locales/sl/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.348440 napatrackmater-5.0.8/_build/html/_static/locales/sr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.372440 napatrackmater-5.0.8/_build/html/_static/locales/sr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/locales/sr/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.348440 napatrackmater-5.0.8/_build/html/_static/locales/sv/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.372440 napatrackmater-5.0.8/_build/html/_static/locales/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/locales/sv/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.348440 napatrackmater-5.0.8/_build/html/_static/locales/ta/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.372440 napatrackmater-5.0.8/_build/html/_static/locales/ta/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/locales/ta/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.348440 napatrackmater-5.0.8/_build/html/_static/locales/te/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.372440 napatrackmater-5.0.8/_build/html/_static/locales/te/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/locales/te/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.348440 napatrackmater-5.0.8/_build/html/_static/locales/tg/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.372440 napatrackmater-5.0.8/_build/html/_static/locales/tg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/locales/tg/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.348440 napatrackmater-5.0.8/_build/html/_static/locales/th/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.372440 napatrackmater-5.0.8/_build/html/_static/locales/th/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/locales/th/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.348440 napatrackmater-5.0.8/_build/html/_static/locales/tl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.372440 napatrackmater-5.0.8/_build/html/_static/locales/tl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/locales/tl/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.348440 napatrackmater-5.0.8/_build/html/_static/locales/tr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.372440 napatrackmater-5.0.8/_build/html/_static/locales/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/locales/tr/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.352440 napatrackmater-5.0.8/_build/html/_static/locales/uk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.372440 napatrackmater-5.0.8/_build/html/_static/locales/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/locales/uk/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.352440 napatrackmater-5.0.8/_build/html/_static/locales/ur/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.372440 napatrackmater-5.0.8/_build/html/_static/locales/ur/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/locales/ur/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.352440 napatrackmater-5.0.8/_build/html/_static/locales/vi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.372440 napatrackmater-5.0.8/_build/html/_static/locales/vi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/locales/vi/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.352440 napatrackmater-5.0.8/_build/html/_static/locales/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.372440 napatrackmater-5.0.8/_build/html/_static/locales/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.352440 napatrackmater-5.0.8/_build/html/_static/locales/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.372440 napatrackmater-5.0.8/_build/html/_static/locales/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.po
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/minus.png
+-rw-r--r--   0 runner    (1001) docker     (127)    39364 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/plus.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12757 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/pygments.css
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/sbt-webpack-macros.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.372440 napatrackmater-5.0.8/_build/html/_static/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)    80813 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/scripts/bootstrap.js
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/scripts/bootstrap.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   335757 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/scripts/bootstrap.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/scripts/pydata-sphinx-theme.js
+-rw-r--r--   0 runner    (1001) docker     (127)    19648 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/scripts/pydata-sphinx-theme.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/scripts/sphinx-book-theme.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13066 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/scripts/sphinx-book-theme.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)    16634 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/searchtools.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/sphinx-thebe.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/sphinx-thebe.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.376440 napatrackmater-5.0.8/_build/html/_static/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)   176654 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/styles/bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (127)    63341 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/styles/pydata-sphinx-theme.css
+-rw-r--r--   0 runner    (1001) docker     (127)    13841 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/styles/sphinx-book-theme.css
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/styles/theme.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/togglebutton.css
+-rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/togglebutton.js
+-rw-r--r--   0 runner    (1001) docker     (127)    68420 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/underscore-1.13.1.js
+-rw-r--r--   0 runner    (1001) docker     (127)    19530 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/underscore.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.352440 napatrackmater-5.0.8/_build/html/_static/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.352440 napatrackmater-5.0.8/_build/html/_static/vendor/fontawesome/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.376440 napatrackmater-5.0.8/_build/html/_static/vendor/fontawesome/6.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     7427 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/vendor/fontawesome/6.1.2/LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.376440 napatrackmater-5.0.8/_build/html/_static/vendor/fontawesome/6.1.2/css/
+-rw-r--r--   0 runner    (1001) docker     (127)   101691 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/vendor/fontawesome/6.1.2/css/all.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.376440 napatrackmater-5.0.8/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/
+-rw-r--r--   0 runner    (1001) docker     (127)   181264 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   105112 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    60236 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    24028 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   389948 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   154840 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    10084 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/_static/webpack-macros.html
+-rw-r--r--   0 runner    (1001) docker     (127)    11198 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/genindex.html
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/objects.inv
+-rw-r--r--   0 runner    (1001) docker     (127)    12010 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/search.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7816 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/html/searchindex.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.352440 napatrackmater-5.0.8/_build/jupyter_execute/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.376440 napatrackmater-5.0.8/_build/jupyter_execute/Notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)    17500 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_build/jupyter_execute/Notebooks/Track_vector.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/_toc.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.380440 napatrackmater-5.0.8/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    20293 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/images/ClusterDistributionPlot_time_point_97.png
+-rw-r--r--   0 runner    (1001) docker     (127)    29672 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/images/ClusterNearnessPlot_time_point_97.png
+-rw-r--r--   0 runner    (1001) docker     (127)   162373 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/images/ClusterPlot_time_point_97.png
+-rw-r--r--   0 runner    (1001) docker     (127)    61613 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/images/FeatureMatrixPlot_time_point_97.png
+-rw-r--r--   0 runner    (1001) docker     (127)    66872 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/images/QuadrantDistributionPlot_time_point_97.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/images/kapoorlablogo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/images/kapoorlogo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-05 21:37:31.384440 napatrackmater-5.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.352440 napatrackmater-5.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.380440 napatrackmater-5.0.8/src/napatrackmater/
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/src/napatrackmater/CloudAutoEncoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/src/napatrackmater/DeepEmbeddedClustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)   135295 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/src/napatrackmater/Trackmate.py
+-rw-r--r--   0 runner    (1001) docker     (127)   110684 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/src/napatrackmater/Trackvector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/src/napatrackmater/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/src/napatrackmater/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24558 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/src/napatrackmater/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/src/napatrackmater/fast_radius_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13035 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/src/napatrackmater/fate_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6603 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/src/napatrackmater/pretrained.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:37:31.380440 napatrackmater-5.0.8/src/napatrackmater.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4463 2024-04-05 21:37:31.000000 napatrackmater-5.0.8/src/napatrackmater.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-04-05 21:37:31.000000 napatrackmater-5.0.8/src/napatrackmater.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 21:37:31.000000 napatrackmater-5.0.8/src/napatrackmater.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-05 21:37:31.000000 napatrackmater-5.0.8/src/napatrackmater.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-05 21:37:31.000000 napatrackmater-5.0.8/src/napatrackmater.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-05 21:37:20.000000 napatrackmater-5.0.8/update_version.py
```

### Comparing `napatrackmater-5.0.1/.github/workflows/deploy.yml` & `napatrackmater-5.0.8/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/.github/workflows/test_and_deploy.yml` & `napatrackmater-5.0.8/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/.gitignore` & `napatrackmater-5.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/.pre-commit-config.yaml` & `napatrackmater-5.0.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/.travis.yml` & `napatrackmater-5.0.8/.travis.yml`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/Dockerfile` & `napatrackmater-5.0.8/Dockerfile`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/LICENSE` & `napatrackmater-5.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/MASTER.md` & `napatrackmater-5.0.8/MASTER.md`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/Notebooks/Track_vector.ipynb` & `napatrackmater-5.0.8/Notebooks/Track_vector.ipynb`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/PKG-INFO` & `napatrackmater-5.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 5.0.1
+Version: 5.0.8
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/Kapoorlabs-CAPED/napatrackmater
 Author: Varun Kapoor, Mari Tolonen, Jakub Sedzinski
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/napatrackmater/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/napatrackmater#README.md
```

### Comparing `napatrackmater-5.0.1/README.md` & `napatrackmater-5.0.8/README.md`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/.doctrees/MASTER.doctree` & `napatrackmater-5.0.8/_build/.doctrees/MASTER.doctree`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/.doctrees/Notebooks/Track_vector.doctree` & `napatrackmater-5.0.8/_build/.doctrees/Notebooks/Track_vector.doctree`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/.doctrees/README.doctree` & `napatrackmater-5.0.8/_build/.doctrees/README.doctree`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/.doctrees/environment.pickle` & `napatrackmater-5.0.8/_build/.doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/MASTER.html` & `napatrackmater-5.0.8/_build/html/MASTER.html`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/Notebooks/Track_vector.html` & `napatrackmater-5.0.8/_build/html/Notebooks/Track_vector.html`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/README.html` & `napatrackmater-5.0.8/_build/html/README.html`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_images/ClusterDistributionPlot_time_point_97.png` & `napatrackmater-5.0.8/_build/html/_images/ClusterDistributionPlot_time_point_97.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_images/ClusterNearnessPlot_time_point_97.png` & `napatrackmater-5.0.8/_build/html/_images/ClusterNearnessPlot_time_point_97.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_images/ClusterPlot_time_point_97.png` & `napatrackmater-5.0.8/_build/html/_images/ClusterPlot_time_point_97.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_images/FeatureMatrixPlot_time_point_97.png` & `napatrackmater-5.0.8/_build/html/_images/FeatureMatrixPlot_time_point_97.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_images/QuadrantDistributionPlot_time_point_97.png` & `napatrackmater-5.0.8/_build/html/_images/QuadrantDistributionPlot_time_point_97.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_sources/MASTER.md` & `napatrackmater-5.0.8/_build/html/_sources/MASTER.md`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_sources/Notebooks/Track_vector.ipynb` & `napatrackmater-5.0.8/_build/html/_sources/Notebooks/Track_vector.ipynb`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_sources/README.md` & `napatrackmater-5.0.8/_build/html/_sources/README.md`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_sphinx_design_static/design-style.4045f2051d55cab465a707391d5b2007.min.css` & `napatrackmater-5.0.8/_build/html/_sphinx_design_static/design-style.4045f2051d55cab465a707391d5b2007.min.css`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_sphinx_design_static/design-tabs.js` & `napatrackmater-5.0.8/_build/html/_sphinx_design_static/design-tabs.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/basic.css` & `napatrackmater-5.0.8/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/clipboard.min.js` & `napatrackmater-5.0.8/_build/html/_static/clipboard.min.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/copybutton.css` & `napatrackmater-5.0.8/_build/html/_static/copybutton.css`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/copybutton.js` & `napatrackmater-5.0.8/_build/html/_static/copybutton.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/copybutton_funcs.js` & `napatrackmater-5.0.8/_build/html/_static/copybutton_funcs.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/design-style.4045f2051d55cab465a707391d5b2007.min.css` & `napatrackmater-5.0.8/_build/html/_static/design-style.4045f2051d55cab465a707391d5b2007.min.css`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/design-tabs.js` & `napatrackmater-5.0.8/_build/html/_static/design-tabs.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/doctools.js` & `napatrackmater-5.0.8/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/images/logo_binder.svg` & `napatrackmater-5.0.8/_build/html/_static/images/logo_binder.svg`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/images/logo_colab.png` & `napatrackmater-5.0.8/_build/html/_static/images/logo_colab.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/images/logo_deepnote.svg` & `napatrackmater-5.0.8/_build/html/_static/images/logo_deepnote.svg`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/images/logo_jupyterhub.svg` & `napatrackmater-5.0.8/_build/html/_static/images/logo_jupyterhub.svg`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/jquery-3.5.1.js` & `napatrackmater-5.0.8/_build/html/_static/jquery-3.5.1.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/jquery.js` & `napatrackmater-5.0.8/_build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/kapoorlablogo.png` & `napatrackmater-5.0.8/_build/html/_static/kapoorlablogo.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/language_data.js` & `napatrackmater-5.0.8/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/locales/ar/LC_MESSAGES/booktheme.po` & `napatrackmater-5.0.8/_build/html/_static/locales/ar/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/locales/bg/LC_MESSAGES/booktheme.po` & `napatrackmater-5.0.8/_build/html/_static/locales/bg/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/locales/bn/LC_MESSAGES/booktheme.po` & `napatrackmater-5.0.8/_build/html/_static/locales/bn/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/locales/ca/LC_MESSAGES/booktheme.po` & `napatrackmater-5.0.8/_build/html/_static/locales/ca/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/locales/cs/LC_MESSAGES/booktheme.po` & `napatrackmater-5.0.8/_build/html/_static/locales/cs/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/locales/da/LC_MESSAGES/booktheme.po` & `napatrackmater-5.0.8/_build/html/_static/locales/da/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/locales/de/LC_MESSAGES/booktheme.po` & `napatrackmater-5.0.8/_build/html/_static/locales/de/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/locales/el/LC_MESSAGES/booktheme.po` & `napatrackmater-5.0.8/_build/html/_static/locales/el/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/locales/eo/LC_MESSAGES/booktheme.po` & `napatrackmater-5.0.8/_build/html/_static/locales/eo/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/locales/es/LC_MESSAGES/booktheme.po` & `napatrackmater-5.0.8/_build/html/_static/locales/es/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/locales/et/LC_MESSAGES/booktheme.po` & `napatrackmater-5.0.8/_build/html/_static/locales/et/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/locales/fi/LC_MESSAGES/booktheme.po` & `napatrackmater-5.0.8/_build/html/_static/locales/fi/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/locales/fr/LC_MESSAGES/booktheme.po` & `napatrackmater-5.0.8/_build/html/_static/locales/fr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/locales/hr/LC_MESSAGES/booktheme.po` & `napatrackmater-5.0.8/_build/html/_static/locales/hr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/locales/id/LC_MESSAGES/booktheme.po` & `napatrackmater-5.0.8/_build/html/_static/locales/id/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/locales/it/LC_MESSAGES/booktheme.po` & `napatrackmater-5.0.8/_build/html/_static/locales/it/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/locales/iw/LC_MESSAGES/booktheme.po` & `napatrackmater-5.0.8/_build/html/_static/locales/iw/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/locales/ja/LC_MESSAGES/booktheme.po` & `napatrackmater-5.0.8/_build/html/_static/locales/ja/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/locales/ko/LC_MESSAGES/booktheme.po` & `napatrackmater-5.0.8/_build/html/_static/locales/ko/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/locales/lt/LC_MESSAGES/booktheme.po` & `napatrackmater-5.0.8/_build/html/_static/locales/lt/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/locales/lv/LC_MESSAGES/booktheme.po` & `napatrackmater-5.0.8/_build/html/_static/locales/lv/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/locales/ml/LC_MESSAGES/booktheme.po` & `napatrackmater-5.0.8/_build/html/_static/locales/ml/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/locales/mr/LC_MESSAGES/booktheme.po` & `napatrackmater-5.0.8/_build/html/_static/locales/mr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/locales/ms/LC_MESSAGES/booktheme.po` & `napatrackmater-5.0.8/_build/html/_static/locales/ms/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/locales/nl/LC_MESSAGES/booktheme.po` & `napatrackmater-5.0.8/_build/html/_static/locales/nl/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/locales/no/LC_MESSAGES/booktheme.po` & `napatrackmater-5.0.8/_build/html/_static/locales/no/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/locales/pl/LC_MESSAGES/booktheme.po` & `napatrackmater-5.0.8/_build/html/_static/locales/pl/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/locales/pt/LC_MESSAGES/booktheme.po` & `napatrackmater-5.0.8/_build/html/_static/locales/pt/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/locales/ro/LC_MESSAGES/booktheme.po` & `napatrackmater-5.0.8/_build/html/_static/locales/ro/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/locales/ru/LC_MESSAGES/booktheme.po` & `napatrackmater-5.0.8/_build/html/_static/locales/ru/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/locales/sk/LC_MESSAGES/booktheme.po` & `napatrackmater-5.0.8/_build/html/_static/locales/sk/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/locales/sl/LC_MESSAGES/booktheme.po` & `napatrackmater-5.0.8/_build/html/_static/locales/sl/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/locales/sr/LC_MESSAGES/booktheme.po` & `napatrackmater-5.0.8/_build/html/_static/locales/sr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/locales/sv/LC_MESSAGES/booktheme.po` & `napatrackmater-5.0.8/_build/html/_static/locales/sv/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/locales/ta/LC_MESSAGES/booktheme.po` & `napatrackmater-5.0.8/_build/html/_static/locales/ta/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/locales/te/LC_MESSAGES/booktheme.po` & `napatrackmater-5.0.8/_build/html/_static/locales/te/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/locales/tg/LC_MESSAGES/booktheme.po` & `napatrackmater-5.0.8/_build/html/_static/locales/tg/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/locales/th/LC_MESSAGES/booktheme.po` & `napatrackmater-5.0.8/_build/html/_static/locales/th/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/locales/tl/LC_MESSAGES/booktheme.po` & `napatrackmater-5.0.8/_build/html/_static/locales/tl/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/locales/tr/LC_MESSAGES/booktheme.po` & `napatrackmater-5.0.8/_build/html/_static/locales/tr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/locales/uk/LC_MESSAGES/booktheme.po` & `napatrackmater-5.0.8/_build/html/_static/locales/uk/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/locales/ur/LC_MESSAGES/booktheme.po` & `napatrackmater-5.0.8/_build/html/_static/locales/ur/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/locales/vi/LC_MESSAGES/booktheme.po` & `napatrackmater-5.0.8/_build/html/_static/locales/vi/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.po` & `napatrackmater-5.0.8/_build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.po` & `napatrackmater-5.0.8/_build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css` & `napatrackmater-5.0.8/_build/html/_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/pygments.css` & `napatrackmater-5.0.8/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/scripts/bootstrap.js` & `napatrackmater-5.0.8/_build/html/_static/scripts/bootstrap.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/scripts/bootstrap.js.map` & `napatrackmater-5.0.8/_build/html/_static/scripts/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/scripts/pydata-sphinx-theme.js` & `napatrackmater-5.0.8/_build/html/_static/scripts/pydata-sphinx-theme.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/scripts/pydata-sphinx-theme.js.map` & `napatrackmater-5.0.8/_build/html/_static/scripts/pydata-sphinx-theme.js.map`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/scripts/sphinx-book-theme.js` & `napatrackmater-5.0.8/_build/html/_static/scripts/sphinx-book-theme.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/scripts/sphinx-book-theme.js.map` & `napatrackmater-5.0.8/_build/html/_static/scripts/sphinx-book-theme.js.map`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/searchtools.js` & `napatrackmater-5.0.8/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/sphinx-thebe.css` & `napatrackmater-5.0.8/_build/html/_static/sphinx-thebe.css`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/sphinx-thebe.js` & `napatrackmater-5.0.8/_build/html/_static/sphinx-thebe.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/styles/bootstrap.css` & `napatrackmater-5.0.8/_build/html/_static/styles/bootstrap.css`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/styles/pydata-sphinx-theme.css` & `napatrackmater-5.0.8/_build/html/_static/styles/pydata-sphinx-theme.css`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/styles/sphinx-book-theme.css` & `napatrackmater-5.0.8/_build/html/_static/styles/sphinx-book-theme.css`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/togglebutton.css` & `napatrackmater-5.0.8/_build/html/_static/togglebutton.css`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/togglebutton.js` & `napatrackmater-5.0.8/_build/html/_static/togglebutton.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/underscore-1.13.1.js` & `napatrackmater-5.0.8/_build/html/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/underscore.js` & `napatrackmater-5.0.8/_build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/vendor/fontawesome/6.1.2/LICENSE.txt` & `napatrackmater-5.0.8/_build/html/_static/vendor/fontawesome/6.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/vendor/fontawesome/6.1.2/css/all.min.css` & `napatrackmater-5.0.8/_build/html/_static/vendor/fontawesome/6.1.2/css/all.min.css`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf` & `napatrackmater-5.0.8/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2` & `napatrackmater-5.0.8/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf` & `napatrackmater-5.0.8/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2` & `napatrackmater-5.0.8/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf` & `napatrackmater-5.0.8/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2` & `napatrackmater-5.0.8/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf` & `napatrackmater-5.0.8/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2` & `napatrackmater-5.0.8/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/_static/webpack-macros.html` & `napatrackmater-5.0.8/_build/html/_static/webpack-macros.html`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/genindex.html` & `napatrackmater-5.0.8/_build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/search.html` & `napatrackmater-5.0.8/_build/html/search.html`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/html/searchindex.js` & `napatrackmater-5.0.8/_build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_build/jupyter_execute/Notebooks/Track_vector.ipynb` & `napatrackmater-5.0.8/_build/jupyter_execute/Notebooks/Track_vector.ipynb`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/_config.yml` & `napatrackmater-5.0.8/_config.yml`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/images/ClusterDistributionPlot_time_point_97.png` & `napatrackmater-5.0.8/images/ClusterDistributionPlot_time_point_97.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/images/ClusterNearnessPlot_time_point_97.png` & `napatrackmater-5.0.8/images/ClusterNearnessPlot_time_point_97.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/images/ClusterPlot_time_point_97.png` & `napatrackmater-5.0.8/images/ClusterPlot_time_point_97.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/images/FeatureMatrixPlot_time_point_97.png` & `napatrackmater-5.0.8/images/FeatureMatrixPlot_time_point_97.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/images/QuadrantDistributionPlot_time_point_97.png` & `napatrackmater-5.0.8/images/QuadrantDistributionPlot_time_point_97.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/images/kapoorlablogo.png` & `napatrackmater-5.0.8/images/kapoorlablogo.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/images/kapoorlogo.png` & `napatrackmater-5.0.8/images/kapoorlogo.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/setup.cfg` & `napatrackmater-5.0.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/src/napatrackmater/CloudAutoEncoder.py` & `napatrackmater-5.0.8/src/napatrackmater/CloudAutoEncoder.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/src/napatrackmater/DeepEmbeddedClustering.py` & `napatrackmater-5.0.8/src/napatrackmater/DeepEmbeddedClustering.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/src/napatrackmater/Trackmate.py` & `napatrackmater-5.0.8/src/napatrackmater/Trackmate.py`

 * *Files 6% similar despite different names*

```diff
@@ -172,24 +172,30 @@
         self.beforeid_key = "before_id"
         self.dividing_key = "dividing_normal"
         self.number_dividing_key = "number_dividing"
         self.distance_cell_mask_key = "distance_cell_mask"
         self.maskcentroid_x_key = "maskcentroid_x_key"
         self.maskcentroid_z_key = "maskcentroid_z_key"
         self.maskcentroid_y_key = "maskcentroid_y_key"
-        self.cellaxis_mask_key = "cellaxis_mask_key"
+        self.cell_axis_z_key = "cell_axis_z_key"
+        self.cell_axis_y_key = "cell_axis_y_key"
+        self.cell_axis_x_key = "cell_axis_x_key"
         self.cellid_key = "cell_id"
         self.acceleration_key = "acceleration"
         self.centroid_key = "centroid"
         self.eccentricity_comp_firstkey = "cloud_eccentricity_comp_first"
         self.eccentricity_comp_secondkey = "cloud_eccentricity_comp_second"
         self.eccentricity_comp_thirdkey = "cloud_eccentricity_comp_third"
         self.surface_area_key = "cloud_surfacearea"
-        self.radial_angle_key = "radial_angle_key"
-        self.motion_angle_key = "motion_angle"
+        self.radial_angle_z_key = "radial_angle_z_key"
+        self.radial_angle_y_key = "radial_angle_y_key"
+        self.radial_angle_x_key = "radial_angle_x_key"
+        self.motion_angle_z_key = "motion_angle_z"
+        self.motion_angle_y_key = "motion_angle_y"
+        self.motion_angle_x_key = "motion_angle_x"
         self.latent_shape_features_key = "latent_shape_features"
 
         self.mean_intensity_ch1_key = self.track_analysis_spot_keys[
             "mean_intensity_ch1"
         ]
         self.mean_intensity_ch2_key = self.track_analysis_spot_keys[
             "mean_intensity_ch2"
@@ -1083,18 +1089,24 @@
         current_tracklets,
         current_tracklets_properties,
     ):
 
         gen_id = int(float(all_dict_values[self.generationid_key]))
         speed = float(all_dict_values[self.speed_key])
         acceleration = float(all_dict_values[self.acceleration_key])
-        motion_angle = float(all_dict_values[self.motion_angle_key])
-        radial_angle = float(all_dict_values[self.radial_angle_key])
+        motion_angle_z = float(all_dict_values[self.motion_angle_z_key])
+        motion_angle_y = float(all_dict_values[self.motion_angle_y_key])
+        motion_angle_x = float(all_dict_values[self.motion_angle_x_key])
+
+        radial_angle_z = float(all_dict_values[self.radial_angle_z_key])
+        radial_angle_y = float(all_dict_values[self.radial_angle_y_key])
+        radial_angle_x = float(all_dict_values[self.radial_angle_x_key])
+
         radius = float(all_dict_values[self.radius_key])
-        volume_pixels = int(float(all_dict_values[self.quality_key]))
+        radius_pixel = int(float(all_dict_values[self.quality_key]))
         total_intensity = float(all_dict_values[self.total_intensity_key])
 
         distance_cell_mask = float(all_dict_values[self.distance_cell_mask_key])
 
         track_displacement = float(all_dict_values[self.displacement_key])
         total_track_distance = float(all_dict_values[self.total_track_distance_key])
         max_track_distance = float(all_dict_values[self.max_distance_traveled_key])
@@ -1117,22 +1129,26 @@
             eccentricity_comp_second = float(
                 all_dict_values[self.eccentricity_comp_secondkey]
             )
             eccentricity_comp_third = float(
                 all_dict_values[self.eccentricity_comp_thirdkey]
             )
             surface_area = float(all_dict_values[self.surface_area_key])
-            cell_axis_mask = float(all_dict_values[self.cellaxis_mask_key])
+            cell_axis_z = float(all_dict_values[self.cell_axis_z_key])
+            cell_axis_y = float(all_dict_values[self.cell_axis_y_key])
+            cell_axis_x = float(all_dict_values[self.cell_axis_x_key])
 
         else:
             eccentricity_comp_first = -1
             eccentricity_comp_second = -1
             eccentricity_comp_third = -1
             surface_area = -1
-            cell_axis_mask = -1
+            cell_axis_z = -1
+            cell_axis_y = -1
+            cell_axis_x = -1
 
         frame_spot_centroid = (
             t,
             round(z) / self.zcalibration,
             round(y) / self.ycalibration,
             round(x) / self.xcalibration,
         )
@@ -1155,26 +1171,32 @@
 
             value_array = current_tracklets_properties[current_track_id]
             current_value_list = [
                 t,
                 int(float(unique_id)),
                 gen_id,
                 radius,
-                volume_pixels,
+                radius_pixel,
                 eccentricity_comp_first,
                 eccentricity_comp_second,
                 eccentricity_comp_third,
                 surface_area,
                 total_intensity,
                 speed,
-                motion_angle,
+                motion_angle_z,
+                motion_angle_y,
+                motion_angle_x,
                 acceleration,
                 distance_cell_mask,
-                radial_angle,
-                cell_axis_mask,
+                radial_angle_z,
+                radial_angle_y,
+                radial_angle_x,
+                cell_axis_z,
+                cell_axis_y,
+                cell_axis_x,
                 track_displacement,
                 total_track_distance,
                 max_track_distance,
                 track_duration,
             ]
 
             if compute_with_latent_features:
@@ -1207,26 +1229,32 @@
             current_tracklets[current_track_id] = current_tracklet_array
 
             current_value_list = [
                 t,
                 int(float(unique_id)),
                 gen_id,
                 radius,
-                volume_pixels,
+                radius_pixel,
                 eccentricity_comp_first,
                 eccentricity_comp_second,
                 eccentricity_comp_third,
                 surface_area,
                 total_intensity,
                 speed,
-                motion_angle,
+                motion_angle_z,
+                motion_angle_y,
+                motion_angle_x,
                 acceleration,
                 distance_cell_mask,
-                radial_angle,
-                cell_axis_mask,
+                radial_angle_z,
+                radial_angle_y,
+                radial_angle_x,
+                cell_axis_z,
+                cell_axis_y,
+                cell_axis_x,
                 track_displacement,
                 total_track_distance,
                 max_track_distance,
                 track_duration,
             ]
             if compute_with_latent_features:
                 current_value_list.extend(latent_shape_features)
@@ -1264,22 +1292,36 @@
                     self.distance_cell_mask_key: (
                         float(Spotobject.get(self.distance_cell_mask_key))
                     ),
                     self.uniqueid_key: str(Spotobject.get(self.uniqueid_key)),
                     self.trackletid_key: str(Spotobject.get(self.trackletid_key)),
                     self.generationid_key: str(Spotobject.get(self.generationid_key)),
                     self.trackid_key: str(Spotobject.get(self.trackid_key)),
-                    self.motion_angle_key: (
-                        float(Spotobject.get(self.motion_angle_key))
+                    self.motion_angle_z_key: (
+                        float(Spotobject.get(self.motion_angle_z_key))
+                    ),
+                    self.motion_angle_y_key: (
+                        float(Spotobject.get(self.motion_angle_y_key))
+                    ),
+                    self.motion_angle_x_key: (
+                        float(Spotobject.get(self.motion_angle_x_key))
                     ),
                     self.speed_key: (float(Spotobject.get(self.speed_key))),
                     self.acceleration_key: (
                         float(Spotobject.get(self.acceleration_key))
                     ),
-                    self.radial_angle_key: float(Spotobject.get(self.radial_angle_key)),
+                    self.radial_angle_z_key: float(
+                        Spotobject.get(self.radial_angle_z_key)
+                    ),
+                    self.radial_angle_y_key: float(
+                        Spotobject.get(self.radial_angle_y_key)
+                    ),
+                    self.radial_angle_x_key: float(
+                        Spotobject.get(self.radial_angle_x_key)
+                    ),
                 }
                 if self.surface_area_key in Spotobject.keys():
                     self.unique_spot_properties[int(cell_id)].update(
                         {
                             self.eccentricity_comp_firstkey: float(
                                 Spotobject.get(self.eccentricity_comp_firstkey)
                             ),
@@ -1288,16 +1330,22 @@
                             ),
                             self.eccentricity_comp_thirdkey: float(
                                 Spotobject.get(self.eccentricity_comp_thirdkey)
                             ),
                             self.surface_area_key: float(
                                 Spotobject.get(self.surface_area_key)
                             ),
-                            self.cellaxis_mask_key: float(
-                                Spotobject.get(self.cellaxis_mask_key)
+                            self.cell_axis_z_key: float(
+                                Spotobject.get(self.cell_axis_z_key)
+                            ),
+                            self.cell_axis_y_key: float(
+                                Spotobject.get(self.cell_axis_y_key)
+                            ),
+                            self.cell_axis_x_key: float(
+                                Spotobject.get(self.cell_axis_x_key)
                             ),
                         }
                     )
 
             elif self.uniqueid_key not in Spotobject.keys():
 
                 if self.detectorchannel == 1:
@@ -1778,24 +1826,26 @@
             )
 
             cluster_eval._compute_latent_features()
 
             (
                 timed_latent_features,
                 output_cluster_centroids,
-                output_largest_eigenvalues,
+                output_eigenvalues,
             ) = cluster_eval.timed_latent_features[time_key]
 
-            output_latent_features = timed_latent_features
-            output_cluster_centroid = output_cluster_centroids
-            output_largest_eigenvalue = output_largest_eigenvalues
-            for i in range(len(output_latent_features)):
-                latent_feature_list = output_latent_features[i]
-                centroid = output_cluster_centroid[i]
-                quality = output_largest_eigenvalue[i]
+            for i in range(len(timed_latent_features)):
+                latent_feature_list = timed_latent_features[i]
+                centroid = output_cluster_centroids[i]
+                quality = math.pow(
+                    output_eigenvalues[i][0]
+                    * output_eigenvalues[i][1]
+                    * output_eigenvalues[i][2],
+                    1.0 / 3.0,
+                )
                 dist, index = tree.query(centroid)
 
                 if dist < quality:
                     closest_centroid = spot_centroids[index]
                     frame_spot_centroid = (
                         int(time_key),
                         closest_centroid[0],
@@ -1815,15 +1865,19 @@
             for (k, v) in self.root_spots.items():
                 self.root_spots[k] = self.unique_spot_properties[k]
 
     def _assign_cluster_class(self):
 
         self.axes = self.axes.replace("T", "")
 
-        for count, time_key in enumerate(self._timed_centroid.keys()):
+        for count, time_key in tqdm(
+            enumerate(self._timed_centroid.keys()),
+            desc="Getting point clouds",
+            unit="_time_frame",
+        ):
 
             tree, spot_centroids = self._timed_centroid[time_key]
             if self.progress_bar is not None:
                 self.progress_bar.label = "Autoencoder for refining point clouds"
                 self.progress_bar.range = (
                     0,
                     len(self._timed_centroid.keys()) + 1,
@@ -1850,39 +1904,42 @@
             cluster_eval._create_cluster_labels()
 
             timed_cluster_label = cluster_eval.timed_cluster_label
             (
                 output_labels,
                 output_cluster_centroid,
                 output_cloud_eccentricity,
-                output_largest_eigenvector,
-                output_largest_eigenvalue,
+                output_eigenvectors,
+                output_eigenvalues,
                 output_dimensions,
                 output_cloud_surface_area,
             ) = timed_cluster_label[time_key]
             scale_1 = 1
             scale_2 = 1
             scale_3 = 1
             for i in range(len(output_cluster_centroid)):
                 centroid = output_cluster_centroid[i]
-                quality = output_largest_eigenvalue[i]
+                quality = math.pow(
+                    output_eigenvalues[i][2]
+                    * output_eigenvalues[i][1]
+                    * output_eigenvalues[i][0],
+                    1.0 / 3.0,
+                )
                 eccentricity_comp_firstyz = output_cloud_eccentricity[i]
                 eccentricity_dimension = output_dimensions[i]
                 if not isinstance(eccentricity_dimension, int):
-                    scale = set_scale(
-                        eccentricity_dimension,
-                        self.xcalibration,
-                        self.ycalibration,
-                        self.zcalibration,
-                    )
-                    scale_1 = scale[0]
-                    scale_2 = scale[1]
-                    scale_3 = scale[2]
 
-                    cell_axis = output_largest_eigenvector[i]
+                    scale_1 = self.xcalibration
+                    scale_2 = self.ycalibration
+                    scale_3 = self.zcalibration
+
+                    cell_axis_x = output_eigenvectors[i][2]
+                    cell_axis_y = output_eigenvectors[i][1]
+                    cell_axis_z = output_eigenvectors[i][0]
+
                     surface_area = (
                         output_cloud_surface_area[i]
                         * self.zcalibration
                         * self.ycalibration
                         * self.xcalibration
                     )
                     dist, index = tree.query(centroid)
@@ -1896,29 +1953,37 @@
                             int(time_key),
                             closest_centroid[0],
                             closest_centroid[1],
                             closest_centroid[2],
                         )
                         closest_cell_id = self.unique_spot_centroid[frame_spot_centroid]
 
-                        cell_axis_mask = cell_angular_change(cell_axis)
+                        angle_cell_axis_x = cell_angular_change_x(cell_axis_x)
+                        angle_cell_axis_y = cell_angular_change_y(cell_axis_y)
+                        angle_cell_axis_z = cell_angular_change_z(cell_axis_z)
 
                         self.unique_spot_properties[int(closest_cell_id)].update(
-                            {self.cellaxis_mask_key: cell_axis_mask}
+                            {self.cell_axis_x_key: angle_cell_axis_x}
+                        )
+                        self.unique_spot_properties[int(closest_cell_id)].update(
+                            {self.cell_axis_y_key: angle_cell_axis_y}
+                        )
+                        self.unique_spot_properties[int(closest_cell_id)].update(
+                            {self.cell_axis_z_key: angle_cell_axis_z}
                         )
                         if (
                             self.unique_spot_properties[int(closest_cell_id)][
                                 self.radius_key
                             ]
                             > 0
                         ):
                             self.unique_spot_properties[int(closest_cell_id)].update(
                                 {
                                     self.eccentricity_comp_firstkey: eccentricity_comp_firstyz[
-                                        0
+                                        2
                                     ]
                                     * scale_1
                                 }
                             )
                             self.unique_spot_properties[int(closest_cell_id)].update(
                                 {
                                     self.eccentricity_comp_secondkey: eccentricity_comp_firstyz[
@@ -1927,15 +1992,15 @@
                                     * scale_2
                                 }
                             )
 
                             self.unique_spot_properties[int(closest_cell_id)].update(
                                 {
                                     self.eccentricity_comp_thirdkey: eccentricity_comp_firstyz[
-                                        2
+                                        0
                                     ]
                                     * scale_3
                                 }
                             )
 
                             self.unique_spot_properties[int(closest_cell_id)].update(
                                 {self.surface_area_key: surface_area}
@@ -1983,37 +2048,48 @@
             X = tracks[:, 4]
 
             time = tracklet_properties[:, 0]
             unique_ids = tracklet_properties[:, 1]
             unique_ids_set = set(unique_ids)
             # generation_ids = tracklet_properties[:, 2]
             radius = tracklet_properties[:, 3]
-            volume = tracklet_properties[:, 4]
+            radius_pixel = tracklet_properties[:, 4]
             eccentricity_comp_first = tracklet_properties[:, 5]
             eccentricity_comp_second = tracklet_properties[:, 6]
             eccentricity_comp_third = tracklet_properties[:, 7]
             surface_area = tracklet_properties[:, 8]
 
             intensity = tracklet_properties[:, 9]
             speed = tracklet_properties[:, 10]
-            motion_angle = tracklet_properties[:, 11]
-            acceleration = tracklet_properties[:, 12]
-            distance_cell_mask = tracklet_properties[:, 13]
-            radial_angle = tracklet_properties[:, 14]
-            cell_axis_mask = tracklet_properties[:, 15]
-            track_displacement = tracklet_properties[:, 16]
 
-            total_track_distance = tracklet_properties[:, 17]
+            motion_angle_z = tracklet_properties[:, 11]
+            motion_angle_y = tracklet_properties[:, 12]
+            motion_angle_x = tracklet_properties[:, 13]
+
+            acceleration = tracklet_properties[:, 14]
+            distance_cell_mask = tracklet_properties[:, 15]
 
-            max_track_distance = tracklet_properties[:, 18]
+            radial_angle_z = tracklet_properties[:, 16]
+            radial_angle_y = tracklet_properties[:, 17]
+            radial_angle_x = tracklet_properties[:, 18]
 
-            track_duration = tracklet_properties[:, 19]
+            cell_axis_z = tracklet_properties[:, 19]
+            cell_axis_y = tracklet_properties[:, 20]
+            cell_axis_x = tracklet_properties[:, 21]
 
-            if tracklet_properties.shape[1] > 20:
-                latent_shape_features = tracklet_properties[:, 20:]
+            track_displacement = tracklet_properties[:, 22]
+
+            total_track_distance = tracklet_properties[:, 23]
+
+            max_track_distance = tracklet_properties[:, 24]
+
+            track_duration = tracklet_properties[:, 25]
+
+            if tracklet_properties.shape[1] > 25:
+                latent_shape_features = tracklet_properties[:, 26:]
             else:
                 latent_shape_features = []
 
             unique_fft_properties_tracklet = {}
             unique_cluster_properties_tracklet = {}
             self.unique_fft_properties[track_id] = {}
             self.unique_cluster_properties[track_id] = {}
@@ -2032,43 +2108,53 @@
 
                 current_time = []
                 current_z = []
                 current_y = []
                 current_x = []
                 current_intensity = []
                 current_radius = []
-                current_volume = []
+                current_radius_pixel = []
                 current_speed = []
-                current_motion_angle = []
+                current_motion_angle_z = []
+                current_motion_angle_y = []
+                current_motion_angle_x = []
+
                 current_acceleration = []
                 current_distance_cell_mask = []
                 current_eccentricity_comp_first = []
                 current_eccentricity_comp_second = []
                 current_eccentricity_comp_third = []
                 current_surface_area = []
                 current_latent_shape_features = []
-                current_radial_angle = []
-                current_cell_axis_mask = []
+                current_radial_angle_z = []
+                current_radial_angle_y = []
+                current_radial_angle_x = []
+                current_cell_axis_z = []
+                current_cell_axis_y = []
+                current_cell_axis_x = []
                 current_track_displacement = []
                 current_total_track_distance = []
                 current_max_track_distance = []
                 current_track_duration = []
 
                 for j in range(time.shape[0]):
                     if current_unique_id == unique_ids[j]:
                         current_time.append(time[j])
                         current_z.append(Z[j])
                         current_y.append(Y[j])
                         current_x.append(X[j])
                         expanded_intensity[int(time[j])] = intensity[j]
                         current_intensity.append(intensity[j])
                         current_radius.append(radius[j])
-                        current_volume.append(volume[j])
+                        current_radius_pixel.append(radius_pixel[j])
                         current_speed.append(speed[j])
-                        current_motion_angle.append(motion_angle[j])
+                        current_motion_angle_z.append(motion_angle_z[j])
+                        current_motion_angle_y.append(motion_angle_y[j])
+                        current_motion_angle_x.append(motion_angle_x[j])
+
                         current_acceleration.append(acceleration[j])
                         current_distance_cell_mask.append(distance_cell_mask[j])
                         current_eccentricity_comp_first.append(
                             eccentricity_comp_first[j]
                         )
                         current_eccentricity_comp_second.append(
                             eccentricity_comp_second[j]
@@ -2078,26 +2164,34 @@
                         )
 
                         current_surface_area.append(surface_area[j])
                         if latent_shape_features != []:
                             current_latent_shape_features.append(
                                 latent_shape_features[j]
                             )
-                        current_radial_angle.append(radial_angle[j])
-                        current_cell_axis_mask.append(cell_axis_mask[j])
+                        current_radial_angle_z.append(radial_angle_z[j])
+                        current_radial_angle_y.append(radial_angle_y[j])
+                        current_radial_angle_x.append(radial_angle_x[j])
+
+                        current_cell_axis_z.append(cell_axis_z[j])
+                        current_cell_axis_y.append(cell_axis_y[j])
+                        current_cell_axis_x.append(cell_axis_x[j])
+
                         current_track_displacement.append(track_displacement[j])
                         current_total_track_distance.append(total_track_distance[j])
                         current_max_track_distance.append(max_track_distance[j])
                         current_track_duration.append(track_duration[j])
 
                 current_time = np.asarray(current_time, dtype=np.float32)
                 current_intensity = np.asarray(current_intensity, dtype=np.float32)
 
                 current_radius = np.asarray(current_radius, dtype=np.float32)
-                current_volume = np.asarray(current_volume, dtype=np.float32)
+                current_radius_pixel = np.asarray(
+                    current_radius_pixel, dtype=np.float32
+                )
                 current_eccentricity_comp_first = np.asarray(
                     current_eccentricity_comp_first, dtype=np.float32
                 )
                 current_eccentricity_comp_second = np.asarray(
                     current_eccentricity_comp_second, dtype=np.float32
                 )
                 current_eccentricity_comp_third = np.asarray(
@@ -2108,29 +2202,42 @@
                 )
 
                 current_latent_shape_features = np.asarray(
                     current_latent_shape_features, dtype=np.float32
                 )
 
                 current_speed = np.asarray(current_speed, dtype=np.float32)
-                current_motion_angle = np.asarray(
-                    current_motion_angle, dtype=np.float32
+                current_motion_angle_z = np.asarray(
+                    current_motion_angle_z, dtype=np.float32
+                )
+                current_motion_angle_y = np.asarray(
+                    current_motion_angle_y, dtype=np.float32
+                )
+                current_motion_angle_x = np.asarray(
+                    current_motion_angle_x, dtype=np.float32
                 )
                 current_acceleration = np.asarray(
                     current_acceleration, dtype=np.float32
                 )
                 current_distance_cell_mask = np.asarray(
                     current_distance_cell_mask, dtype=np.float32
                 )
-                current_radial_angle = np.asarray(
-                    current_radial_angle, dtype=np.float32
+                current_radial_angle_z = np.asarray(
+                    current_radial_angle_z, dtype=np.float32
                 )
-                current_cell_axis_mask = np.asarray(
-                    current_cell_axis_mask, dtype=np.float32
+                current_radial_angle_y = np.asarray(
+                    current_radial_angle_y, dtype=np.float32
                 )
+                current_radial_angle_x = np.asarray(
+                    current_radial_angle_x, dtype=np.float32
+                )
+
+                current_cell_axis_z = np.asarray(current_cell_axis_z, dtype=np.float32)
+                current_cell_axis_y = np.asarray(current_cell_axis_y, dtype=np.float32)
+                current_cell_axis_x = np.asarray(current_cell_axis_x, dtype=np.float32)
 
                 current_track_displacement = np.asarray(
                     current_track_displacement, dtype=np.float32
                 )
                 current_total_track_distance = np.asarray(
                     current_total_track_distance, dtype=np.float32
                 )
@@ -2157,29 +2264,35 @@
                 unique_cluster_properties_tracklet[current_unique_id] = current_time
                 unique_shape_properties_tracklet[current_unique_id] = (
                     current_time,
                     current_z,
                     current_y,
                     current_x,
                     current_radius,
-                    current_volume,
+                    current_radius_pixel,
                     current_eccentricity_comp_first,
                     current_eccentricity_comp_second,
                     current_eccentricity_comp_third,
                     current_surface_area,
                     current_latent_shape_features,
                 )
                 unique_dynamic_properties_tracklet[current_unique_id] = (
                     current_time,
                     current_speed,
-                    current_motion_angle,
+                    current_motion_angle_z,
+                    current_motion_angle_y,
+                    current_motion_angle_x,
                     current_acceleration,
                     current_distance_cell_mask,
-                    current_radial_angle,
-                    current_cell_axis_mask,
+                    current_radial_angle_z,
+                    current_radial_angle_y,
+                    current_radial_angle_x,
+                    current_cell_axis_z,
+                    current_cell_axis_y,
+                    current_cell_axis_x,
                     current_track_displacement,
                     current_total_track_distance,
                     current_max_track_distance,
                     current_track_duration,
                 )
                 self.unique_fft_properties[track_id].update(
                     {
@@ -2296,46 +2409,58 @@
 
         vec_cell = [
             float(self.unique_spot_properties[int(cell_id)][self.xposid_key]),
             float(self.unique_spot_properties[int(cell_id)][self.yposid_key]),
             float(self.unique_spot_properties[int(cell_id)][self.zposid_key]),
         ]
 
-        angle = angular_change(vec_mask, vec_cell)
-
-        self.unique_spot_properties[int(cell_id)].update({self.radial_angle_key: angle})
+        angle_x = angular_change_x(vec_mask, vec_cell)
+        angle_y = angular_change_y(vec_mask, vec_cell)
+        angle_z = angular_change_z(vec_mask, vec_cell)
 
+        self.unique_spot_properties[int(cell_id)].update(
+            {self.radial_angle_x_key: angle_x}
+        )
+        self.unique_spot_properties[int(cell_id)].update(
+            {self.radial_angle_y_key: angle_y}
+        )
+        self.unique_spot_properties[int(cell_id)].update(
+            {self.radial_angle_z_key: angle_z}
+        )
         unique_tracklet_ids.append(str(unique_id))
         self.unique_spot_properties[int(cell_id)].update(
             {self.uniqueid_key: str(unique_id)}
         )
         self.unique_spot_properties[int(cell_id)].update(
             {self.trackletid_key: str(tracklet_id)}
         )
         self.unique_spot_properties[int(cell_id)].update(
             {self.generationid_key: str(generation_id)}
         )
         self.unique_spot_properties[int(cell_id)].update(
             {self.trackid_key: str(track_id)}
         )
-        self.unique_spot_properties[int(cell_id)].update({self.motion_angle_key: 0.0})
+        self.unique_spot_properties[int(cell_id)].update({self.motion_angle_z_key: 0.0})
+        self.unique_spot_properties[int(cell_id)].update({self.motion_angle_y_key: 0.0})
+        self.unique_spot_properties[int(cell_id)].update({self.motion_angle_x_key: 0.0})
         self.unique_spot_properties[int(cell_id)].update({self.speed_key: 0.0})
         self.unique_spot_properties[int(cell_id)].update({self.acceleration_key: 0.0})
         self.unique_spot_properties[int(cell_id)].update(
             {self.eccentricity_comp_firstkey: -1}
         )
         self.unique_spot_properties[int(cell_id)].update(
             {self.eccentricity_comp_secondkey: -1}
         )
         self.unique_spot_properties[int(cell_id)].update(
             {self.eccentricity_comp_thirdkey: -1}
         )
         self.unique_spot_properties[int(cell_id)].update({self.surface_area_key: -1})
-        self.unique_spot_properties[int(cell_id)].update({self.cellaxis_mask_key: -1})
-
+        self.unique_spot_properties[int(cell_id)].update({self.cell_axis_z_key: -1})
+        self.unique_spot_properties[int(cell_id)].update({self.cell_axis_y_key: -1})
+        self.unique_spot_properties[int(cell_id)].update({self.cell_axis_x_key: -1})
         if source_id is not None:
             self.unique_spot_properties[int(cell_id)].update(
                 {self.beforeid_key: int(source_id)}
             )
             vec_1 = [
                 float(self.unique_spot_properties[int(cell_id)][self.xposid_key])
                 - float(self.unique_spot_properties[int(source_id)][self.xposid_key]),
@@ -2343,18 +2468,28 @@
                 - float(self.unique_spot_properties[int(source_id)][self.yposid_key]),
                 float(self.unique_spot_properties[int(cell_id)][self.zposid_key])
                 - float(self.unique_spot_properties[int(source_id)][self.zposid_key]),
             ]
             speed = np.sqrt(np.dot(vec_1, vec_1)) / self.tcalibration
             self.unique_spot_properties[int(cell_id)].update({self.speed_key: speed})
 
-            motion_angle = cell_angular_change(vec_1)
+            motion_angle_x = cell_angular_change_x(vec_1)
+            motion_angle_y = cell_angular_change_y(vec_1)
+            motion_angle_z = cell_angular_change_z(vec_1)
+
+            self.unique_spot_properties[int(cell_id)].update(
+                {self.motion_angle_x_key: motion_angle_x}
+            )
+
+            self.unique_spot_properties[int(cell_id)].update(
+                {self.motion_angle_y_key: motion_angle_y}
+            )
 
             self.unique_spot_properties[int(cell_id)].update(
-                {self.motion_angle_key: motion_angle}
+                {self.motion_angle_z_key: motion_angle_z}
             )
 
             if source_id in self.edge_source_lookup:
                 pre_source_id = self.edge_source_lookup[source_id]
 
                 vec_2 = [
                     float(self.unique_spot_properties[int(cell_id)][self.xposid_key])
@@ -2420,16 +2555,22 @@
 
         self.mitotic_mean_speed = []
         self.mitotic_var_speed = []
 
         self.mitotic_mean_acc = []
         self.mitotic_var_acc = []
 
-        self.mitotic_mean_directional_change = []
-        self.mitotic_var_directional_change = []
+        self.mitotic_mean_directional_change_z = []
+        self.mitotic_var_directional_change_z = []
+
+        self.mitotic_mean_directional_change_y = []
+        self.mitotic_var_directional_change_y = []
+
+        self.mitotic_mean_directional_change_x = []
+        self.mitotic_var_directional_change_x = []
 
         self.mitotic_mean_distance_cell_mask = []
         self.mitotic_var_distance_cell_mask = []
 
         self.non_mitotic_mean_disp_z = []
         self.non_mitotic_var_disp_z = []
 
@@ -2444,16 +2585,22 @@
 
         self.non_mitotic_mean_speed = []
         self.non_mitotic_var_speed = []
 
         self.non_mitotic_mean_acc = []
         self.non_mitotic_var_acc = []
 
-        self.non_mitotic_mean_directional_change = []
-        self.non_mitotic_var_directional_change = []
+        self.non_mitotic_mean_directional_change_z = []
+        self.non_mitotic_var_directional_change_z = []
+
+        self.non_mitotic_mean_directional_change_y = []
+        self.non_mitotic_var_directional_change_y = []
+
+        self.non_mitotic_mean_directional_change_x = []
+        self.non_mitotic_var_directional_change_x = []
 
         self.non_mitotic_mean_distance_cell_mask = []
         self.non_mitotic_var_distance_cell_mask = []
 
         self.all_mean_disp_z = []
         self.all_var_disp_z = []
 
@@ -2468,16 +2615,22 @@
 
         self.all_mean_speed = []
         self.all_var_speed = []
 
         self.all_mean_acc = []
         self.all_var_acc = []
 
-        self.all_mean_directional_change = []
-        self.all_var_directional_change = []
+        self.all_mean_directional_change_z = []
+        self.all_var_directional_change_z = []
+
+        self.all_mean_directional_change_y = []
+        self.all_var_directional_change_y = []
+
+        self.all_mean_directional_change_x = []
+        self.all_var_directional_change_x = []
 
         self.all_mean_distance_cell_mask = []
         self.all_var_distance_cell_mask = []
 
         all_spots_tracks = {}
         for (k, v) in self.unique_spot_properties.items():
 
@@ -2501,33 +2654,39 @@
     def _compute_temporal(self, i, all_spots_tracks):
         mitotic_disp_z = []
         mitotic_disp_y = []
         mitotic_disp_x = []
         mitotic_radius = []
         mitotic_speed = []
         mitotic_acc = []
-        mitotic_directional_change = []
+        mitotic_directional_change_z = []
+        mitotic_directional_change_y = []
+        mitotic_directional_change_x = []
         mitotic_distance_cell_mask = []
 
         non_mitotic_disp_z = []
         non_mitotic_disp_y = []
         non_mitotic_disp_x = []
         non_mitotic_radius = []
         non_mitotic_speed = []
         non_mitotic_acc = []
-        non_mitotic_directional_change = []
+        non_mitotic_directional_change_z = []
+        non_mitotic_directional_change_y = []
+        non_mitotic_directional_change_x = []
         non_mitotic_distance_cell_mask = []
 
         all_disp_z = []
         all_disp_y = []
         all_disp_x = []
         all_radius = []
         all_speed = []
         all_acc = []
-        all_directional_change = []
+        all_directional_change_z = []
+        all_directional_change_y = []
+        all_directional_change_x = []
         all_distance_cell_mask = []
 
         for (k, v) in all_spots_tracks.items():
 
             current_time = all_spots_tracks[k][self.frameid_key]
             mitotic = all_spots_tracks[k][self.dividing_key]
 
@@ -2538,16 +2697,22 @@
                     mitotic_disp_x.append(all_spots_tracks[k][self.xposid_key])
                     if all_spots_tracks[k][self.radius_key] > 0:
                         mitotic_radius.append(all_spots_tracks[k][self.radius_key])
                     else:
                         mitotic_radius.append(None)
                     mitotic_speed.append(all_spots_tracks[k][self.speed_key])
                     mitotic_acc.append(all_spots_tracks[k][self.acceleration_key])
-                    mitotic_directional_change.append(
-                        all_spots_tracks[k][self.motion_angle_key]
+                    mitotic_directional_change_z.append(
+                        all_spots_tracks[k][self.motion_angle_z_key]
+                    )
+                    mitotic_directional_change_y.append(
+                        all_spots_tracks[k][self.motion_angle_y_key]
+                    )
+                    mitotic_directional_change_x.append(
+                        all_spots_tracks[k][self.motion_angle_x_key]
                     )
                     mitotic_distance_cell_mask.append(
                         all_spots_tracks[k][self.distance_cell_mask_key]
                     )
 
                 if not mitotic:
                     non_mitotic_disp_z.append(all_spots_tracks[k][self.zposid_key])
@@ -2555,32 +2720,44 @@
                     non_mitotic_disp_x.append(all_spots_tracks[k][self.xposid_key])
                     if all_spots_tracks[k][self.radius_key] > 0:
                         non_mitotic_radius.append(all_spots_tracks[k][self.radius_key])
                     else:
                         non_mitotic_radius.append(None)
                     non_mitotic_speed.append(all_spots_tracks[k][self.speed_key])
                     non_mitotic_acc.append(all_spots_tracks[k][self.acceleration_key])
-                    non_mitotic_directional_change.append(
-                        all_spots_tracks[k][self.motion_angle_key]
+                    non_mitotic_directional_change_z.append(
+                        all_spots_tracks[k][self.motion_angle_z_key]
+                    )
+                    non_mitotic_directional_change_y.append(
+                        all_spots_tracks[k][self.motion_angle_y_key]
+                    )
+                    non_mitotic_directional_change_x.append(
+                        all_spots_tracks[k][self.motion_angle_x_key]
                     )
                     non_mitotic_distance_cell_mask.append(
                         all_spots_tracks[k][self.distance_cell_mask_key]
                     )
 
                 all_disp_z.append(all_spots_tracks[k][self.zposid_key])
                 all_disp_y.append(all_spots_tracks[k][self.yposid_key])
                 all_disp_x.append(all_spots_tracks[k][self.xposid_key])
                 if all_spots_tracks[k][self.radius_key] > 0:
                     all_radius.append(all_spots_tracks[k][self.radius_key])
                 else:
                     all_radius.append(None)
                 all_speed.append(all_spots_tracks[k][self.speed_key])
                 all_acc.append(all_spots_tracks[k][self.acceleration_key])
-                all_directional_change.append(
-                    all_spots_tracks[k][self.motion_angle_key]
+                all_directional_change_z.append(
+                    all_spots_tracks[k][self.motion_angle_z_key]
+                )
+                all_directional_change_y.append(
+                    all_spots_tracks[k][self.motion_angle_y_key]
+                )
+                all_directional_change_x.append(
+                    all_spots_tracks[k][self.motion_angle_x_key]
                 )
                 all_distance_cell_mask.append(
                     all_spots_tracks[k][self.distance_cell_mask_key]
                 )
 
         mitotic_disp_z = np.abs(np.diff(mitotic_disp_z))
         mitotic_disp_y = np.abs(np.diff(mitotic_disp_y))
@@ -2612,16 +2789,34 @@
 
         self.mitotic_mean_speed.append(np.mean(mitotic_speed))
         self.mitotic_var_speed.append(np.std(mitotic_speed))
 
         self.mitotic_mean_acc.append(np.mean(mitotic_acc))
         self.mitotic_var_acc.append(np.std(mitotic_acc))
 
-        self.mitotic_mean_directional_change.append(np.mean(mitotic_directional_change))
-        self.mitotic_var_directional_change.append(np.std(mitotic_directional_change))
+        self.mitotic_mean_directional_change_z.append(
+            np.mean(mitotic_directional_change_z)
+        )
+        self.mitotic_var_directional_change_z.append(
+            np.std(mitotic_directional_change_z)
+        )
+
+        self.mitotic_mean_directional_change_y.append(
+            np.mean(mitotic_directional_change_y)
+        )
+        self.mitotic_var_directional_change_y.append(
+            np.std(mitotic_directional_change_y)
+        )
+
+        self.mitotic_mean_directional_change_x.append(
+            np.mean(mitotic_directional_change_x)
+        )
+        self.mitotic_var_directional_change_x.append(
+            np.std(mitotic_directional_change_x)
+        )
 
         self.mitotic_mean_distance_cell_mask.append(np.mean(mitotic_distance_cell_mask))
         self.mitotic_var_distance_cell_mask.append(np.std(mitotic_distance_cell_mask))
 
         self.non_mitotic_mean_disp_z.append(np.mean(non_mitotic_disp_z))
         self.non_mitotic_var_disp_z.append(np.std(non_mitotic_disp_z))
 
@@ -2638,19 +2833,33 @@
 
         self.non_mitotic_mean_speed.append(np.mean(non_mitotic_speed))
         self.non_mitotic_var_speed.append(np.std(non_mitotic_speed))
 
         self.non_mitotic_mean_acc.append(np.mean(non_mitotic_acc))
         self.non_mitotic_var_acc.append(np.std(non_mitotic_acc))
 
-        self.non_mitotic_mean_directional_change.append(
-            np.mean(non_mitotic_directional_change)
+        self.non_mitotic_mean_directional_change_z.append(
+            np.mean(non_mitotic_directional_change_z)
+        )
+        self.non_mitotic_var_directional_change_z.append(
+            np.std(non_mitotic_directional_change_z)
+        )
+
+        self.non_mitotic_mean_directional_change_y.append(
+            np.mean(non_mitotic_directional_change_y)
         )
-        self.non_mitotic_var_directional_change.append(
-            np.std(non_mitotic_directional_change)
+        self.non_mitotic_var_directional_change_y.append(
+            np.std(non_mitotic_directional_change_y)
+        )
+
+        self.non_mitotic_mean_directional_change_x.append(
+            np.mean(non_mitotic_directional_change_x)
+        )
+        self.non_mitotic_var_directional_change_x.append(
+            np.std(non_mitotic_directional_change_x)
         )
 
         self.non_mitotic_mean_distance_cell_mask.append(
             np.mean(non_mitotic_distance_cell_mask)
         )
         self.non_mitotic_var_distance_cell_mask.append(
             np.std(non_mitotic_distance_cell_mask)
@@ -2672,16 +2881,22 @@
 
         self.all_mean_speed.append(np.mean(all_speed))
         self.all_var_speed.append(np.std(all_speed))
 
         self.all_mean_acc.append(np.mean(all_acc))
         self.all_var_acc.append(np.std(all_acc))
 
-        self.all_mean_directional_change.append(np.mean(all_directional_change))
-        self.all_var_directional_change.append(np.std(all_directional_change))
+        self.all_mean_directional_change_z.append(np.mean(all_directional_change_z))
+        self.all_var_directional_change_z.append(np.std(all_directional_change_z))
+
+        self.all_mean_directional_change_y.append(np.mean(all_directional_change_y))
+        self.all_var_directional_change_y.append(np.std(all_directional_change_y))
+
+        self.all_mean_directional_change_x.append(np.mean(all_directional_change_x))
+        self.all_var_directional_change_x.append(np.std(all_directional_change_x))
 
         self.all_mean_distance_cell_mask.append(np.mean(all_distance_cell_mask))
         self.all_var_distance_cell_mask.append(np.std(all_distance_cell_mask))
 
 
 def boundary_points(mask, xcalibration, ycalibration, zcalibration):
 
@@ -2699,15 +2914,15 @@
 
         for j in range(0, len(real_indices)):
 
             real_indices[j][0] = real_indices[j][0] * ycalibration
             real_indices[j][1] = real_indices[j][1] * xcalibration
 
         tree = spatial.cKDTree(real_indices)
-        # This object contains list of all the points for all the labels in the Mask image with the label id and volume of each label
+        # This object contains list of all the points for all the labels in the Mask image with the label id and radius_pixel of each label
         timed_mask[str(0)] = [tree, indices, regioncentroid]
 
     # TYX shaped object
     if ndim == 3:
 
         for i in tqdm(range(0, mask.shape[0])):
 
@@ -2889,42 +3104,98 @@
     return x * scale
 
 
 def prob_sigmoid(x):
     return 1 - math.exp(-x)
 
 
-def angular_change(vec_mask, vec_cell):
+def angular_change_z(vec_mask, vec_cell):
 
     vec = np.asarray(vec_cell) - np.asarray(vec_mask)
     vec = vec / np.linalg.norm(vec)
     num_dims = len(vec)
     unit_vector = np.zeros(num_dims)
     unit_vector[-1] = 1
     unit_vector = unit_vector / np.linalg.norm(unit_vector)
     theta = np.arccos(np.clip(np.dot(vec, unit_vector), -1.0, 1.0))
     angle = np.rad2deg(theta)
 
     return angle
 
 
-def cell_angular_change(vec_cell):
+def cell_angular_change_z(vec_cell):
 
     vec = np.asarray(vec_cell)
     vec = vec / np.linalg.norm(vec)
     num_dims = len(vec)
     unit_vector = np.zeros(num_dims)
     unit_vector[-1] = 1
     unit_vector = unit_vector / np.linalg.norm(unit_vector)
     theta = np.arccos(np.clip(np.dot(vec, unit_vector), -1.0, 1.0))
     angle = np.rad2deg(theta)
 
     return angle
 
 
+def angular_change_y(vec_mask, vec_cell):
+
+    vec = np.asarray(vec_cell) - np.asarray(vec_mask)
+    vec = vec / np.linalg.norm(vec)
+    num_dims = len(vec)
+    unit_vector = np.zeros(num_dims)
+    unit_vector[-2] = 1
+    unit_vector = unit_vector / np.linalg.norm(unit_vector)
+    theta = np.arccos(np.clip(np.dot(vec, unit_vector), -1.0, 1.0))
+    angle = np.rad2deg(theta)
+
+    return angle
+
+
+def cell_angular_change_y(vec_cell):
+
+    vec = np.asarray(vec_cell)
+    vec = vec / np.linalg.norm(vec)
+    num_dims = len(vec)
+    unit_vector = np.zeros(num_dims)
+    unit_vector[-2] = 1
+    unit_vector = unit_vector / np.linalg.norm(unit_vector)
+    theta = np.arccos(np.clip(np.dot(vec, unit_vector), -1.0, 1.0))
+    angle = np.rad2deg(theta)
+
+    return angle
+
+
+def angular_change_x(vec_mask, vec_cell):
+
+    vec = np.asarray(vec_cell) - np.asarray(vec_mask)
+    vec = vec / np.linalg.norm(vec)
+    num_dims = len(vec)
+    unit_vector = np.zeros(num_dims)
+    unit_vector[0] = 1
+    unit_vector = unit_vector / np.linalg.norm(unit_vector)
+    theta = np.arccos(np.clip(np.dot(vec, unit_vector), -1.0, 1.0))
+    angle = np.rad2deg(theta)
+
+    return angle
+
+
+def cell_angular_change_x(vec_cell):
+
+    vec = np.asarray(vec_cell)
+    vec = vec / np.linalg.norm(vec)
+    num_dims = len(vec)
+    unit_vector = np.zeros(num_dims)
+    unit_vector[0] = 1
+    unit_vector = unit_vector / np.linalg.norm(unit_vector)
+    theta = np.arccos(np.clip(np.dot(vec, unit_vector), -1.0, 1.0))
+    angle = np.rad2deg(theta)
+
+    return angle
+
+
 def check_and_update_mask(mask, image):
     if len(mask.shape) < len(image.shape):
         update_mask = np.zeros_like(image, dtype="uint8")
         for i in range(image.shape[0]):
             labeled_mask, num_features = measure.label(
                 mask[i], background=0, return_num=True
             )
@@ -2948,41 +3219,50 @@
 
 def get_feature_dict(unique_tracks_properties):
 
     features = {
         "time": np.asarray(unique_tracks_properties, dtype="float16")[:, 0],
         "generation": np.asarray(unique_tracks_properties, dtype="float16")[:, 2],
         "radius": np.asarray(unique_tracks_properties, dtype="float16")[:, 3],
-        "volume_pixels": np.asarray(unique_tracks_properties, dtype="float16")[:, 4],
+        "radius_pixel": np.asarray(unique_tracks_properties, dtype="float16")[:, 4],
         "eccentricity_comp_first": np.asarray(
             unique_tracks_properties, dtype="float16"
         )[:, 5],
         "eccentricity_comp_second": np.asarray(
             unique_tracks_properties, dtype="float16"
         )[:, 6],
-        "surface_area": np.asarray(unique_tracks_properties, dtype="float16")[:, 7],
-        "total_intensity": np.asarray(unique_tracks_properties, dtype="float16")[:, 8],
-        "speed": np.asarray(unique_tracks_properties, dtype="float16")[:, 9],
-        "motion_angle": np.asarray(unique_tracks_properties, dtype="float16")[:, 10],
-        "acceleration": np.asarray(unique_tracks_properties, dtype="float16")[:, 11],
+        "eccentricity_comp_third": np.asarray(
+            unique_tracks_properties, dtype="float16"
+        )[:, 7],
+        "surface_area": np.asarray(unique_tracks_properties, dtype="float16")[:, 8],
+        "total_intensity": np.asarray(unique_tracks_properties, dtype="float16")[:, 9],
+        "speed": np.asarray(unique_tracks_properties, dtype="float16")[:, 10],
+        "motion_angle_z": np.asarray(unique_tracks_properties, dtype="float16")[:, 11],
+        "motion_angle_y": np.asarray(unique_tracks_properties, dtype="float16")[:, 12],
+        "motion_angle_x": np.asarray(unique_tracks_properties, dtype="float16")[:, 13],
+        "acceleration": np.asarray(unique_tracks_properties, dtype="float16")[:, 14],
         "distance_cell_mask": np.asarray(unique_tracks_properties, dtype="float16")[
-            :, 12
+            :, 15
         ],
-        "radial_angle": np.asarray(unique_tracks_properties, dtype="float16")[:, 13],
-        "cell_axis_mask": np.asarray(unique_tracks_properties, dtype="float16")[:, 14],
+        "radial_angle_z": np.asarray(unique_tracks_properties, dtype="float16")[:, 16],
+        "radial_angle_y": np.asarray(unique_tracks_properties, dtype="float16")[:, 17],
+        "radial_angle_x": np.asarray(unique_tracks_properties, dtype="float16")[:, 18],
+        "cell_axis_z": np.asarray(unique_tracks_properties, dtype="float16")[:, 19],
+        "cell_axis_y": np.asarray(unique_tracks_properties, dtype="float16")[:, 20],
+        "cell_axis_x": np.asarray(unique_tracks_properties, dtype="float16")[:, 21],
         "track_displacement": np.asarray(unique_tracks_properties, dtype="float16")[
-            :, 15
+            :, 22
         ],
         "total_track_distance": np.asarray(unique_tracks_properties, dtype="float16")[
-            :, 16
+            :, 23
         ],
         "max_track_distance": np.asarray(unique_tracks_properties, dtype="float16")[
-            :, 17
+            :, 24
         ],
-        "track_duration": np.asarray(unique_tracks_properties, dtype="float16")[:, 18],
+        "track_duration": np.asarray(unique_tracks_properties, dtype="float16")[:, 25],
     }
 
     return features
 
 
 def set_scale(dimensions, x_calibration, y_calibration, z_calibration):
```

### Comparing `napatrackmater-5.0.1/src/napatrackmater/Trackvector.py` & `napatrackmater-5.0.8/src/napatrackmater/Trackvector.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,47 @@
 from torch.optim.lr_scheduler import MultiStepLR
 import matplotlib.pyplot as plt
 from typing import List, Union
 import torch.nn.init as init
 import random
 
 
+SHAPE_FEATURES = [
+    "Radius",
+    "Radius_Pixel",
+    "Eccentricity_Comp_First",
+    "Eccentricity_Comp_Second",
+    "Eccentricity_Comp_Third",
+    "Surface_Area",
+]
+
+DYNAMIC_FEATURES = [
+    "Speed",
+    "Motion_Angle_Z",
+    "Motion_Angle_Y",
+    "Motion_Angle_X",
+    "Acceleration",
+    "Distance_Cell_mask",
+    "Radial_Angle_Z",
+    "Radial_Angle_Y",
+    "Radial_Angle_X",
+    "Cell_Axis_Z",
+    "Cell_Axis_Y",
+    "Cell_Axis_X",
+]
+
+IDENTITY_FEATURES = ["Track ID", "t", "z", "y", "x", "Dividing", "Number_Dividing"]
+
+STATUS_FEATURES = ["Dividing", "Number_Dividing"]
+
+SHAPE_DYNAMIC_FEATURES = SHAPE_FEATURES + DYNAMIC_FEATURES
+
+ALL_FEATURES = IDENTITY_FEATURES + SHAPE_DYNAMIC_FEATURES
+
+
 class TrackVector(TrackMate):
     def __init__(
         self,
         master_xml_path: Path,
         viewer: napari.Viewer = None,
         image: np.ndarray = None,
         spot_csv_path: Path = None,
@@ -245,34 +278,40 @@
 
                 unique_dynamic_properties_tracklet = nested_unique_dynamic_properties[
                     current_unique_id
                 ]
                 (
                     current_time,
                     speed,
-                    motion_angle,
+                    motion_angle_z,
+                    motion_angle_y,
+                    motion_angle_x,
                     acceleration,
                     distance_cell_mask,
-                    radial_angle,
-                    cell_axis_mask,
+                    radial_angle_z,
+                    radial_angle_y,
+                    radial_angle_x,
+                    cell_axis_z,
+                    cell_axis_y,
+                    cell_axis_x,
                     _,
                     _,
                     _,
                     _,
                 ) = unique_dynamic_properties_tracklet
                 unique_shape_properties_tracklet = nested_unique_shape_properties[
                     current_unique_id
                 ]
                 (
                     current_time,
                     current_z,
                     current_y,
                     current_x,
                     radius,
-                    volume,
+                    radius_pixel,
                     eccentricity_comp_first,
                     eccentricity_comp_second,
                     eccentricity_comp_third,
                     surface_area,
                     latent_features,
                 ) = unique_shape_properties_tracklet
 
@@ -291,25 +330,31 @@
                         current_time,
                         current_z,
                         current_y,
                         current_x,
                         dividing_array,
                         number_dividing_array,
                         radius,
-                        volume,
+                        radius_pixel,
                         eccentricity_comp_first,
                         eccentricity_comp_second,
                         eccentricity_comp_third,
                         surface_area,
                         speed,
-                        motion_angle,
+                        motion_angle_z,
+                        motion_angle_y,
+                        motion_angle_x,
                         acceleration,
                         distance_cell_mask,
-                        radial_angle,
-                        cell_axis_mask,
+                        radial_angle_z,
+                        radial_angle_y,
+                        radial_angle_x,
+                        cell_axis_z,
+                        cell_axis_y,
+                        cell_axis_x,
                     ]
                     + (
                         [latent_features[i] for i in range(len(latent_features))]
                         if len(latent_features) > 0
                         else []
                     )
                 )
@@ -504,93 +549,86 @@
             tracklet_id = spot_properties[self.trackletid_key]
             number_times_divided = spot_properties[self.number_dividing_key]
             surface_area = spot_properties[self.surface_area_key]
             eccentricity_comp_first = spot_properties[self.eccentricity_comp_firstkey]
             eccentricity_comp_second = spot_properties[self.eccentricity_comp_secondkey]
             eccentricity_comp_third = spot_properties[self.eccentricity_comp_thirdkey]
             radius = spot_properties[self.radius_key]
-            volume = spot_properties[self.quality_key]
+            radius_pixel = spot_properties[self.quality_key]
             speed = spot_properties[self.speed_key]
 
-            motion_angle = spot_properties[self.motion_angle_key]
+            motion_angle_z = spot_properties[self.motion_angle_z_key]
+            motion_angle_y = spot_properties[self.motion_angle_y_key]
+            motion_angle_x = spot_properties[self.motion_angle_x_key]
             acceleration = spot_properties[self.acceleration_key]
             distance_cell_mask = spot_properties[self.distance_cell_mask_key]
-            radial_angle = spot_properties[self.radial_angle_key]
-            cell_axis_mask = spot_properties[self.cellaxis_mask_key]
+            radial_angle_z = spot_properties[self.radial_angle_z_key]
+            radial_angle_y = spot_properties[self.radial_angle_y_key]
+            radial_angle_x = spot_properties[self.radial_angle_x_key]
+            cell_axis_z = spot_properties[self.cell_axis_z_key]
+            cell_axis_y = spot_properties[self.cell_axis_y_key]
+            cell_axis_x = spot_properties[self.cell_axis_x_key]
 
             data = {
-                "Track ID": track_id,
-                "Unique ID": unique_id,
-                "Tracklet ID": tracklet_id,
-                "Number Times Divided": number_times_divided,
-                "Surface Area": surface_area,
-                "Eccentricity Comp First": eccentricity_comp_first,
-                "Eccentricity Comp Second": eccentricity_comp_second,
-                "Eccentricity Comp Third": eccentricity_comp_third,
+                "Track_ID": track_id,
+                "Unique_ID": unique_id,
+                "Tracklet_ID": tracklet_id,
+                "Number_Times_Divided": number_times_divided,
+                "Surface_Area": surface_area,
+                "Eccentricity_Comp_First": eccentricity_comp_first,
+                "Eccentricity_Comp_Second": eccentricity_comp_second,
+                "Eccentricity_Comp_Third": eccentricity_comp_third,
                 "Radius": radius,
-                "Volume": volume,
+                "Radius_Pixel": radius_pixel,
                 "Speed": speed,
-                "Motion Angle": motion_angle,
+                "Motion_Angle_Z": motion_angle_z,
+                "Motion_Angle_Y": motion_angle_y,
+                "Motion_Angle_X": motion_angle_x,
                 "Acceleration": acceleration,
-                "Distance Cell Mask": distance_cell_mask,
-                "Radial Angle": radial_angle,
-                "Cell Axis Mask": cell_axis_mask,
+                "Distance_Cell_Mask": distance_cell_mask,
+                "Radial_Angle_Z": radial_angle_z,
+                "Radial_Angle_Y": radial_angle_y,
+                "Radial_Angle_X": radial_angle_x,
+                "cell_axis_Z": cell_axis_z,
+                "cell_axis_Y": cell_axis_y,
+                "cell_axis_X": cell_axis_x,
             }
 
             all_split_data.append(data)
 
         np.save(f"{save_path}_data_at_mitosis_time.npy", all_split_data)
 
     def get_shape_dynamic_feature_dataframe(self):
 
         current_shape_dynamic_vectors = self.current_shape_dynamic_vectors
         global_shape_dynamic_dataframe = []
 
         for i in range(len(current_shape_dynamic_vectors)):
             vector_list = current_shape_dynamic_vectors[i]
-            initial_array = np.array(vector_list[:19])
-            latent_shape_features = np.array(vector_list[19:])
+            numel_features = len(ALL_FEATURES)
+            initial_array = np.array(vector_list[:numel_features])
+            latent_shape_features = np.array(vector_list[numel_features:])
             zipped_initial_array = list(zip(initial_array))
             data_frame_list = np.transpose(
                 np.asarray(
                     [zipped_initial_array[i] for i in range(len(zipped_initial_array))]
                 )[:, 0, :]
             )
 
             shape_dynamic_dataframe = pd.DataFrame(
                 data_frame_list,
-                columns=[
-                    "Track ID",
-                    "t",
-                    "z",
-                    "y",
-                    "x",
-                    "Dividing",
-                    "Number_Dividing",
-                    "Radius",
-                    "Volume",
-                    "Eccentricity Comp First",
-                    "Eccentricity Comp Second",
-                    "Eccentricity Comp Third",
-                    "Surface Area",
-                    "Speed",
-                    "Motion_Angle",
-                    "Acceleration",
-                    "Distance_Cell_mask",
-                    "Radial_Angle",
-                    "Cell_Axis_Mask",
-                ],
+                columns=ALL_FEATURES,
             )
 
             cols_to_replace = [
                 "Radius",
-                "Volume",
-                "Eccentricity Comp First",
-                "Eccentricity Comp Second",
-                "Eccentricity Comp Third",
+                "Radius_Pixel",
+                "Eccentricity_Comp_First",
+                "Eccentricity_Comp_Second",
+                "Eccentricity_Comp_Third",
                 "Surface Area",
             ]
             shape_dynamic_dataframe[cols_to_replace] = shape_dynamic_dataframe[
                 cols_to_replace
             ].apply(lambda x: np.where(x < 0, np.nan, x))
             if len(latent_shape_features) > 0:
                 new_columns = [
@@ -617,15 +655,15 @@
         ] = global_shape_dynamic_dataframe["Track ID"].map(
             self.tracklet_id_to_trackmate_id
         )
         trackmate_ids = global_shape_dynamic_dataframe["TrackMate Track ID"]
         track_duration_dict = {}
         for trackmate_id in trackmate_ids:
             track_properties = self.unique_track_properties[trackmate_id]
-            total_track_duration = track_properties[:, 18][0]
+            total_track_duration = track_properties[:, -1][0]
             track_duration_dict[trackmate_id] = int(total_track_duration)
         global_shape_dynamic_dataframe[
             "Track Duration"
         ] = global_shape_dynamic_dataframe["TrackMate Track ID"].map(
             track_duration_dict
         )
 
@@ -639,98 +677,23 @@
         return global_shape_dynamic_dataframe
 
 
 def _iterate_over_tracklets(
     track_data, training_tracklets, track_id, prediction=False, ignore_columns=[]
 ):
 
-    shape_dynamic_dataframe = track_data[
-        [
-            "Radius",
-            "Volume",
-            "Eccentricity Comp First",
-            "Eccentricity Comp Second",
-            "Eccentricity Comp Third",
-            "Surface Area",
-            "Speed",
-            "Motion_Angle",
-            "Acceleration",
-            "Distance_Cell_mask",
-            "Radial_Angle",
-            "Cell_Axis_Mask",
-        ]
-    ].copy()
+    shape_dynamic_dataframe = track_data[SHAPE_DYNAMIC_FEATURES].copy()
 
-    shape_dataframe = track_data[
-        [
-            "Radius",
-            "Volume",
-            "Eccentricity Comp First",
-            "Eccentricity Comp Second",
-            "Eccentricity Comp Third",
-            "Surface Area",
-        ]
-    ].copy()
+    shape_dataframe = track_data[SHAPE_FEATURES].copy()
 
-    dynamic_dataframe = track_data[
-        [
-            "Speed",
-            "Motion_Angle",
-            "Acceleration",
-            "Distance_Cell_mask",
-            "Radial_Angle",
-            "Cell_Axis_Mask",
-        ]
-    ].copy()
+    dynamic_dataframe = track_data[DYNAMIC_FEATURES].copy()
     if not prediction:
-        full_dataframe = track_data[
-            [
-                "Track ID",
-                "t",
-                "z",
-                "y",
-                "x",
-                "Dividing",
-                "Number_Dividing",
-                "Radius",
-                "Volume",
-                "Eccentricity Comp First",
-                "Eccentricity Comp Second",
-                "Eccentricity Comp Third",
-                "Surface Area",
-                "Speed",
-                "Motion_Angle",
-                "Acceleration",
-                "Distance_Cell_mask",
-                "Radial_Angle",
-                "Cell_Axis_Mask",
-            ]
-        ].copy()
+        full_dataframe = track_data[ALL_FEATURES].copy()
     else:
-        full_dataframe = track_data[
-            [
-                "Track ID",
-                "t",
-                "z",
-                "y",
-                "x",
-                "Radius",
-                "Volume",
-                "Eccentricity Comp First",
-                "Eccentricity Comp Second",
-                "Eccentricity Comp Third",
-                "Surface Area",
-                "Speed",
-                "Motion_Angle",
-                "Acceleration",
-                "Distance_Cell_mask",
-                "Radial_Angle",
-                "Cell_Axis_Mask",
-            ]
-        ].copy()
+        full_dataframe = track_data[ALL_FEATURES - STATUS_FEATURES].copy()
 
     if ignore_columns is not None:
         for column in ignore_columns:
             if column in full_dataframe.columns:
                 full_dataframe.drop(columns=[column], inplace=True)
             if column in shape_dynamic_dataframe.columns:
                 shape_dynamic_dataframe.drop(columns=[column], inplace=True)
@@ -1142,60 +1105,22 @@
 
 def create_gt_analysis_vectors_dict(global_shape_dynamic_dataframe: pd.DataFrame):
     gt_analysis_vectors = {}
     for track_id in global_shape_dynamic_dataframe["Track ID"].unique():
         track_data = global_shape_dynamic_dataframe[
             global_shape_dynamic_dataframe["Track ID"] == track_id
         ].sort_values(by="t")
-        shape_dynamic_dataframe = track_data[
-            [
-                "Radius",
-                "Volume",
-                "Eccentricity Comp First",
-                "Eccentricity Comp Second",
-                "Eccentricity Comp Third",
-                "Surface Area",
-                "Speed",
-                "Motion_Angle",
-                "Acceleration",
-                "Distance_Cell_mask",
-                "Radial_Angle",
-                "Cell_Axis_Mask",
-            ]
-        ]
+        shape_dynamic_dataframe = track_data[SHAPE_DYNAMIC_FEATURES]
         gt_dataframe = track_data[
             [
                 "Cluster",
             ]
         ]
 
-        full_dataframe = track_data[
-            [
-                "Track ID",
-                "t",
-                "z",
-                "y",
-                "x",
-                "Dividing",
-                "Number_Dividing",
-                "Radius",
-                "Volume",
-                "Eccentricity Comp First",
-                "Eccentricity Comp Second",
-                "Eccentricity Comp Third",
-                "Surface Area",
-                "Speed",
-                "Motion_Angle",
-                "Acceleration",
-                "Distance_Cell_mask",
-                "Radial_Angle",
-                "Cell_Axis_Mask",
-                "Cluster",
-            ]
-        ]
+        full_dataframe = track_data[ALL_FEATURES]
 
         latent_columns = [
             col
             for col in track_data.columns
             if col.startswith("latent_feature_number_")
         ]
         if latent_columns:
@@ -1938,48 +1863,19 @@
             dynamic_covariance_2d,
             analysis_track_ids,
         )
 
 
 def cell_fate_recipe(track_data):
 
-    dividing_shape_dynamic_dataframe = track_data[
-        [
-            "Radius",
-            "Eccentricity Comp First",
-            "Eccentricity Comp Second",
-            "Eccentricity Comp Third",
-            "Surface Area",
-            "Speed",
-            "Motion_Angle",
-            "Distance_Cell_mask",
-            "Radial_Angle",
-            "Cell_Axis_Mask",
-        ]
-    ].copy()
+    dividing_shape_dynamic_dataframe = track_data[SHAPE_DYNAMIC_FEATURES].copy()
 
-    dividing_shape_dataframe = track_data[
-        [
-            "Radius",
-            "Eccentricity Comp First",
-            "Eccentricity Comp Second",
-            "Eccentricity Comp Third",
-            "Surface Area",
-        ]
-    ].copy()
+    dividing_shape_dataframe = track_data[SHAPE_FEATURES].copy()
 
-    dividing_dynamic_dataframe = track_data[
-        [
-            "Speed",
-            "Motion_Angle",
-            "Distance_Cell_mask",
-            "Radial_Angle",
-            "Cell_Axis_Mask",
-        ]
-    ].copy()
+    dividing_dynamic_dataframe = track_data[DYNAMIC_FEATURES].copy()
 
     dividing_shape_dynamic_dataframe.dropna(inplace=True)
     dividing_shape_dataframe.dropna(inplace=True)
     dividing_dynamic_dataframe.dropna(inplace=True)
 
     dividing_shape_dynamic_dataframe_list = dividing_shape_dynamic_dataframe.to_dict(
         orient="records"
@@ -2000,25 +1896,24 @@
     )
     dividing_dynamic_track_array = np.array(
         [
             [item for item in record.values()]
             for record in dividing_dynamic_dataframe_list
         ]
     )
-    if (
-            dividing_shape_dynamic_track_array.shape[0] > 1 
-    ):
+    if dividing_shape_dynamic_track_array.shape[0] > 1:
         (
             dividing_covariance_shape_dynamic,
             dividing_eigenvectors_shape_dynamic,
         ) = compute_covariance_matrix(dividing_shape_dynamic_track_array)
 
-        dividing_covariance_shape, dividing_eigenvectors_shape = compute_covariance_matrix(
-            dividing_shape_track_array
-        )
+        (
+            dividing_covariance_shape,
+            dividing_eigenvectors_shape,
+        ) = compute_covariance_matrix(dividing_shape_track_array)
 
         (
             dividing_covariance_dynamic,
             dividing_eigenvectors_dynamic,
         ) = compute_covariance_matrix(dividing_dynamic_track_array)
 
         dividing_shape_dynamic_eigenvectors_3d = np.dstack(
@@ -2026,15 +1921,17 @@
         )
         dividing_shape_eigenvectors_3d = np.dstack(dividing_covariance_shape)
         dividing_dynamic_eigenvectors_3d = np.dstack(dividing_covariance_dynamic)
         dividing_shape_dynamic_eigenvectors_2d = (
             dividing_shape_dynamic_eigenvectors_3d.reshape(1, -1)
         )
         dividing_shape_eigenvectors_2d = dividing_shape_eigenvectors_3d.reshape(1, -1)
-        dividing_dynamic_eigenvectors_2d = dividing_dynamic_eigenvectors_3d.reshape(1, -1)
+        dividing_dynamic_eigenvectors_2d = dividing_dynamic_eigenvectors_3d.reshape(
+            1, -1
+        )
 
         dividing_shape_dynamic_covariance_2d = np.array(
             dividing_shape_dynamic_eigenvectors_2d
         )
         dividing_shape_covariance_2d = np.array(dividing_shape_eigenvectors_2d)
         dividing_dynamic_covariance_2d = np.array(dividing_dynamic_eigenvectors_2d)
```

### Comparing `napatrackmater-5.0.1/src/napatrackmater/__init__.py` & `napatrackmater-5.0.8/src/napatrackmater/__init__.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/src/napatrackmater/clustering.py` & `napatrackmater-5.0.8/src/napatrackmater/clustering.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,42 +10,40 @@
 from torch.utils.data import Dataset
 from torch.utils.data import DataLoader
 import tempfile
 from scipy.spatial import ConvexHull
 from scipy.spatial.qhull import QhullError
 from lightning import Trainer
 from typing import List
-from tqdm import tqdm
 
 
 class PointCloudDataset(Dataset):
     def __init__(self, clouds: List[PyntCloud], center=True, scale_z=1.0, scale_xy=1.0):
         self.clouds = clouds
         self.center = center
         self.scale_z = scale_z
         self.scale_xy = scale_xy
 
     def __len__(self):
         return len(self.clouds)
 
     def __getitem__(self, idx):
         point_cloud = self.clouds[idx]
-        mean = 0.0  
+        mean = 0.0
         point_cloud = torch.tensor(point_cloud.points.values).float()
 
         if self.center:
-            mean = torch.mean(point_cloud, 0).float()  
+            mean = torch.mean(point_cloud, 0).float()
 
         scale = torch.tensor([[self.scale_z, self.scale_xy, self.scale_xy]]).float()
         point_cloud = (point_cloud - mean) / scale
 
         return point_cloud
 
 
-
 class Clustering:
     def __init__(
         self,
         pretrainer: Trainer,
         accelerator: str,
         devices: List[int],
         label_image: np.ndarray,
@@ -93,30 +91,30 @@
                 self.min_size,
                 ndim,
                 self.compute_with_autoencoder,
             )
             (
                 latent_features,
                 cluster_centroids,
-                output_largest_eigenvalues,
+                output_eigenvalues,
             ) = _extract_latent_features(
                 self.model,
                 self.accelerator,
                 clouds,
                 marching_cube_points,
                 centroids,
                 self.batch_size,
                 self.scale_z,
                 self.scale_xy,
             )
 
             self.timed_latent_features[str(self.key)] = (
                 latent_features,
                 cluster_centroids,
-                output_largest_eigenvalues,
+                output_eigenvalues,
             )
 
         # ZYX image
         if ndim == 3 and "T" not in self.axes:
 
             labels, centroids, clouds, marching_cube_points = _label_cluster(
                 self.label_image,
@@ -126,60 +124,60 @@
                 self.compute_with_autoencoder,
             )
             if len(labels) > 1:
 
                 (
                     latent_features,
                     cluster_centroids,
-                    output_largest_eigenvalues,
+                    output_eigenvalues,
                 ) = _extract_latent_features(
                     self.model,
                     self.accelerator,
                     clouds,
                     marching_cube_points,
                     centroids,
                     self.batch_size,
                     self.scale_z,
                     self.scale_xy,
                 )
 
                 self.timed_latent_features[str(self.key)] = (
                     latent_features,
                     cluster_centroids,
-                    output_largest_eigenvalues,
+                    output_eigenvalues,
                 )
 
         # TYX
         if ndim == 3 and "T" in self.axes:
 
             for i in range(self.label_image.shape[0]):
                 (
                     latent_features,
                     cluster_centroids,
-                    output_largest_eigenvalues,
+                    output_eigenvalues,
                 ) = self._latent_computer(i, ndim - 1)
                 self.timed_latent_features[str(i)] = (
                     latent_features,
                     cluster_centroids,
-                    output_largest_eigenvalues,
+                    output_eigenvalues,
                 )
 
         # TZYX image
         if ndim == 4:
 
             for i in range(self.label_image.shape[0]):
                 (
                     latent_features,
                     cluster_centroids,
-                    output_largest_eigenvalues,
+                    output_eigenvalues,
                 ) = self._latent_computer(i, ndim)
                 self.timed_latent_features[str(i)] = (
                     latent_features,
                     cluster_centroids,
-                    output_largest_eigenvalues,
+                    output_eigenvalues,
                 )
 
     def _latent_computer(self, i, dim):
 
         xyz_label_image = self.label_image[i, :]
         labels, centroids, clouds, marching_cube_points = _label_cluster(
             xyz_label_image,
@@ -189,26 +187,26 @@
             self.compute_with_autoencoder,
         )
         if len(labels) > 1:
 
             (
                 latent_features,
                 cluster_centroids,
-                output_largest_eigenvalues,
+                output_eigenvalues,
             ) = _extract_latent_features(
                 self.model,
                 self.accelerator,
                 clouds,
                 marching_cube_points,
                 centroids,
                 self.batch_size,
                 self.scale_z,
                 self.scale_xy,
             )
-            return latent_features, cluster_centroids, output_largest_eigenvalues
+            return latent_features, cluster_centroids, output_eigenvalues
 
     def _create_cluster_labels(self):
 
         ndim = len(self.label_image.shape)
         if ndim == 2:
 
             labels, centroids, clouds, marching_cube_points = _label_cluster(
@@ -219,16 +217,16 @@
                 self.compute_with_autoencoder,
             )
 
             (
                 output_labels,
                 output_cluster_centroid,
                 output_cloud_eccentricity,
-                output_largest_eigenvector,
-                output_largest_eigenvalue,
+                output_eigenvectors,
+                output_eigenvalues,
                 output_dimensions,
                 output_cloud_surface_area,
             ) = _model_output(
                 self.model,
                 self.pretrainer,
                 marching_cube_points,
                 clouds,
@@ -239,16 +237,16 @@
                 self.scale_z,
                 self.scale_xy,
             )
             self.timed_cluster_label[str(self.key)] = [
                 output_labels,
                 output_cluster_centroid,
                 output_cloud_eccentricity,
-                output_largest_eigenvector,
-                output_largest_eigenvalue,
+                output_eigenvectors,
+                output_eigenvalues,
                 output_dimensions,
                 output_cloud_surface_area,
             ]
 
         # ZYX image
         if ndim == 3 and "T" not in self.axes:
 
@@ -261,16 +259,16 @@
             )
             if len(labels) > 1:
 
                 (
                     output_labels,
                     output_cluster_centroid,
                     output_cloud_eccentricity,
-                    output_largest_eigenvector,
-                    output_largest_eigenvalue,
+                    output_eigenvectors,
+                    output_eigenvalues,
                     output_dimensions,
                     output_cloud_surface_area,
                 ) = _model_output(
                     self.model,
                     self.pretrainer,
                     marching_cube_points,
                     clouds,
@@ -281,64 +279,64 @@
                     self.scale_z,
                     self.scale_xy,
                 )
                 self.timed_cluster_label[str(self.key)] = [
                     output_labels,
                     output_cluster_centroid,
                     output_cloud_eccentricity,
-                    output_largest_eigenvector,
-                    output_largest_eigenvalue,
+                    output_eigenvectors,
+                    output_eigenvalues,
                     output_dimensions,
                     output_cloud_surface_area,
                 ]
 
         # TYX
         if ndim == 3 and "T" in self.axes:
 
             for i in range(self.label_image.shape[0]):
                 self.count = self.count + 1
                 (
                     output_labels,
                     output_cluster_centroid,
                     output_cloud_eccentricity,
-                    output_largest_eigenvector,
-                    output_largest_eigenvalue,
+                    output_eigenvectors,
+                    output_eigenvalues,
                     output_dimensions,
                     output_cloud_surface_area,
                 ) = self._label_computer(i, ndim - 1)
                 self.timed_cluster_label[str(i)] = [
                     output_labels,
                     output_cluster_centroid,
                     output_cloud_eccentricity,
-                    output_largest_eigenvector,
-                    output_largest_eigenvalue,
+                    output_eigenvectors,
+                    output_eigenvalues,
                     output_dimensions,
                     output_cloud_surface_area,
                 ]
 
         # TZYX image
         if ndim == 4:
 
             for i in range(self.label_image.shape[0]):
                 self.count = self.count + 1
                 (
                     output_labels,
                     output_cluster_centroid,
                     output_cloud_eccentricity,
-                    output_largest_eigenvector,
-                    output_largest_eigenvalue,
+                    output_eigenvectors,
+                    output_eigenvalues,
                     output_dimensions,
                     output_cloud_surface_area,
                 ) = self._label_computer(i, ndim)
                 self.timed_cluster_label[str(i)] = [
                     output_labels,
                     output_cluster_centroid,
                     output_cloud_eccentricity,
-                    output_largest_eigenvector,
-                    output_largest_eigenvalue,
+                    output_eigenvectors,
+                    output_eigenvalues,
                     output_dimensions,
                     output_cloud_surface_area,
                 ]
 
     def _label_computer(self, i, dim):
 
         xyz_label_image = self.label_image[i, :]
@@ -351,16 +349,16 @@
         )
         if len(labels) > 1:
 
             (
                 output_labels,
                 output_cluster_centroid,
                 output_cloud_eccentricity,
-                output_largest_eigenvector,
-                output_largest_eigenvalue,
+                output_eigenvectors,
+                output_eigenvalues,
                 output_dimensions,
                 output_cloud_surface_area,
             ) = _model_output(
                 self.model,
                 self.pretrainer,
                 marching_cube_points,
                 clouds,
@@ -372,16 +370,16 @@
                 self.scale_xy,
             )
 
             return (
                 output_labels,
                 output_cluster_centroid,
                 output_cloud_eccentricity,
-                output_largest_eigenvector,
-                output_largest_eigenvalue,
+                output_eigenvectors,
+                output_eigenvalues,
                 output_dimensions,
                 output_cloud_surface_area,
             )
 
 
 def _extract_latent_features(
     model: AutoLightningModel,
@@ -401,30 +399,30 @@
     ]
 
     torch_model = model.network
     torch_model.eval()
     device = accelerator
     torch_model.to(device)
     latent_features = []
-    output_largest_eigenvalue = [
+    output_eigenvalues = [
         get_eccentricity(cloud_input)[2]
         if get_eccentricity(cloud_input) is not None
         else -1
         for cloud_input in marching_cube_points
     ]
 
     for batch in dataloader:
 
         with torch.no_grad():
             batch = batch.to(device).float()
             latent_representation_list = torch_model.encoder(batch)
             for latent_representation in latent_representation_list:
                 latent_features.append(latent_representation.cpu().numpy())
 
-    return latent_features, output_cluster_centroids, output_largest_eigenvalue
+    return latent_features, output_cluster_centroids, output_eigenvalues
 
 
 def _model_output(
     model: AutoLightningModel,
     pretrainer: Trainer,
     marching_cube_points,
     clouds,
@@ -436,16 +434,16 @@
     scale_xy: float = 1.0,
 ):
 
     output_labels = []
     output_cluster_centroid = []
     output_cloud_eccentricity = []
     output_cloud_surface_area = []
-    output_largest_eigenvector = []
-    output_largest_eigenvalue = []
+    output_eigenvectors = []
+    output_eigenvalues = []
     output_dimensions = []
     dataset = PointCloudDataset(clouds, scale_z=scale_z, scale_xy=scale_xy)
     dataloader = DataLoader(dataset, batch_size=batch_size)
 
     output_cluster_centroid = output_cluster_centroid + [
         tuple(centroid_input) for centroid_input in centroids
     ]
@@ -453,64 +451,62 @@
 
     if compute_with_autoencoder:
 
         model.eval()
 
         outputs_list = pretrainer.predict(model=model, dataloaders=dataloader)
 
-        for outputs in tqdm(outputs_list, desc="Autoencoder model", unit="batch"):
+        for outputs in outputs_list:
             output_cloud_eccentricity = output_cloud_eccentricity + [
                 tuple(get_eccentricity(cloud_input.detach().cpu().numpy()))[0]
                 for cloud_input in outputs
             ]
-            output_largest_eigenvector = output_largest_eigenvector + [
+            output_eigenvectors = output_eigenvectors + [
                 get_eccentricity(cloud_input.detach().cpu().numpy())[1]
                 for cloud_input in outputs
             ]
-            output_largest_eigenvalue = output_largest_eigenvalue + [
+            output_eigenvalues = output_eigenvalues + [
                 get_eccentricity(cloud_input.detach().cpu().numpy())[2]
                 for cloud_input in outputs
             ]
             output_dimensions = output_dimensions + [
                 get_eccentricity(cloud_input.detach().cpu().numpy())[3]
                 for cloud_input in outputs
             ]
             output_cloud_surface_area = output_cloud_surface_area + [
                 float(get_surface_area(cloud_input.detach().cpu().numpy()))
                 for cloud_input in outputs
             ]
 
     else:
 
-        for cloud_input in tqdm(
-            marching_cube_points, desc="Marching cubes", unit="cloud_input"
-        ):
+        for cloud_input in marching_cube_points:
             try:
                 ConvexHull(cloud_input)
 
                 output_cloud_eccentricity.append(
                     tuple(get_eccentricity(cloud_input))[0]
                 )
 
-                output_largest_eigenvector.append(get_eccentricity(cloud_input)[1])
-                output_largest_eigenvalue.append(get_eccentricity(cloud_input)[2])
+                output_eigenvectors.append(get_eccentricity(cloud_input)[1])
+                output_eigenvalues.append(get_eccentricity(cloud_input)[2])
                 output_dimensions.append(get_eccentricity(cloud_input)[3])
                 output_cloud_surface_area.append(float(get_surface_area(cloud_input)))
             except QhullError:
                 output_cloud_eccentricity.append(-1)
-                output_largest_eigenvector.append(-1)
-                output_largest_eigenvalue.append(-1)
+                output_eigenvectors.append(-1)
+                output_eigenvalues.append(-1)
                 output_dimensions.append(-1)
                 output_cloud_surface_area.append(-1)
     return (
         output_labels,
         output_cluster_centroid,
         output_cloud_eccentricity,
-        output_largest_eigenvector,
-        output_largest_eigenvalue,
+        output_eigenvectors,
+        output_eigenvalues,
         output_dimensions,
         output_cloud_surface_area,
     )
 
 
 def _label_cluster(label_image, num_points, min_size, ndim, compute_with_autoencoder):
 
@@ -543,15 +539,22 @@
                 centroids.append(centroid)
                 marching_cube_points.append(sample_points)
 
     return labels, centroids, clouds, marching_cube_points
 
 
 def get_label_centroid_cloud(
-    binary_image, num_points, ndim, label, centroid, min_size, compute_with_autoencoder, padding_size = 3
+    binary_image,
+    num_points,
+    ndim,
+    label,
+    centroid,
+    min_size,
+    compute_with_autoencoder,
+    padding_size=3,
 ):
 
     valid = []
 
     if min_size is not None:
         for j in range(len(min_size)):
             if binary_image.shape[j] >= min_size[j]:
@@ -561,25 +564,26 @@
     else:
         for j in range(len(binary_image.shape)):
             valid.append(True)
 
     if False not in valid:
 
         try:
-            
-            binary_image_padded = np.pad(binary_image, padding_size, mode='constant', constant_values=0)
+
+            binary_image_padded = np.pad(
+                binary_image, padding_size, mode="constant", constant_values=0
+            )
             vertices, faces, normals, values = marching_cubes(binary_image_padded)
         except Exception as e:
-            print(f'Zero padding not possible {e}')    
+            print(f"Zero padding not possible {e}")
             try:
                 vertices, faces, normals, values = marching_cubes(binary_image)
             except RuntimeError:
                 vertices = None
 
-        
         if vertices is not None:
             mesh_obj = trimesh.Trimesh(vertices=vertices, faces=faces)
             simple_clouds = np.asarray(mesh_obj.sample(num_points).data)
 
             if compute_with_autoencoder:
                 mesh_obj = trimesh.Trimesh(
                     vertices=vertices, faces=faces, process=False
@@ -623,39 +627,31 @@
     cloud = PyntCloud(pd.DataFrame(data=points, columns=["x", "y"]))
 
     return cloud
 
 
 def get_panda_cloud_xyz(points):
 
-    cloud = PyntCloud(pd.DataFrame(data=points, columns=["x", "y", "z"]))
+    cloud = PyntCloud(pd.DataFrame(data=points, columns=["z", "y", "x"]))
 
     return cloud
 
 
 def get_eccentricity(point_cloud):
-
-    # Compute the covariance matrix of the point cloud
     cov_mat = np.cov(point_cloud, rowvar=False)
 
-    # Compute the eigenvectors and eigenvalues of the covariance matrix
     eigenvalues, eigenvectors = np.linalg.eigh(cov_mat)
 
-    # Sort the eigenvectors in descending order of their corresponding eigenvalues
-    idx = eigenvalues.argsort()[::-1]
-    eigenvectors = eigenvectors[:, idx]
-    eigenvalues = eigenvalues[idx]
-    largest_eigen_vector = eigenvectors[:, idx[0]]
-    largest_eigen_value = eigenvalues[idx[0]]
     if np.any(eigenvalues < 0):
         return None
+    eigenvectors = eigenvectors[:, ::-1]
     eccentricities = np.sqrt(eigenvalues)
-    dimensions = idx
-
-    return eccentricities, largest_eigen_vector, largest_eigen_value, dimensions
+    dimensions = np.arange(len(eigenvalues))
+    # Z Y X
+    return eccentricities, eigenvectors, eigenvalues, dimensions
 
 
 def get_surface_area(point_cloud):
     # Compute the convex hull of the point cloud
     hull = ConvexHull(point_cloud)
 
     # Compute the areas of the triangles in the convex hull
```

### Comparing `napatrackmater-5.0.1/src/napatrackmater/fast_radius_regression.py` & `napatrackmater-5.0.8/src/napatrackmater/fast_radius_regression.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/src/napatrackmater/fate_mapping.py` & `napatrackmater-5.0.8/src/napatrackmater/fate_mapping.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/src/napatrackmater/pretrained.py` & `napatrackmater-5.0.8/src/napatrackmater/pretrained.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/src/napatrackmater.egg-info/PKG-INFO` & `napatrackmater-5.0.8/src/napatrackmater.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 5.0.1
+Version: 5.0.8
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/Kapoorlabs-CAPED/napatrackmater
 Author: Varun Kapoor, Mari Tolonen, Jakub Sedzinski
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/napatrackmater/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/napatrackmater#README.md
```

### Comparing `napatrackmater-5.0.1/src/napatrackmater.egg-info/SOURCES.txt` & `napatrackmater-5.0.8/src/napatrackmater.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.0.1/update_version.py` & `napatrackmater-5.0.8/update_version.py`

 * *Files identical despite different names*

