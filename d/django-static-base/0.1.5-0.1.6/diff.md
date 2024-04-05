# Comparing `tmp/django-static-base-0.1.5.tar.gz` & `tmp/django-static-base-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-static-base-0.1.5.tar", last modified: Sun Jan 28 14:14:03 2024, max compression
+gzip compressed data, was "django-static-base-0.1.6.tar", last modified: Fri Apr  5 21:48:58 2024, max compression
```

## Comparing `django-static-base-0.1.5.tar` & `django-static-base-0.1.6.tar`

### file list

```diff
@@ -1,327 +1,320 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 14:14:03.809383 django-static-base-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-01-28 14:13:51.000000 django-static-base-0.1.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-01-28 14:13:51.000000 django-static-base-0.1.5/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-01-28 14:13:51.000000 django-static-base-0.1.5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-01-28 14:13:51.000000 django-static-base-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-01-28 14:13:51.000000 django-static-base-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5820 2024-01-28 14:14:03.809383 django-static-base-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-01-28 14:13:51.000000 django-static-base-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-01-28 14:13:51.000000 django-static-base-0.1.5/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-01-28 14:13:51.000000 django-static-base-0.1.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 14:14:03.737383 django-static-base-0.1.5/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-01-28 14:13:51.000000 django-static-base-0.1.5/requirements/dev.in
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-01-28 14:13:51.000000 django-static-base-0.1.5/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (127)    33489 2024-01-28 14:13:51.000000 django-static-base-0.1.5/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)    46362 2024-01-28 14:13:51.000000 django-static-base-0.1.5/requirements/py310-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-01-28 14:13:51.000000 django-static-base-0.1.5/requirements/py310-django32.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-01-28 14:13:51.000000 django-static-base-0.1.5/requirements/py310-django42.txt
--rw-r--r--   0 runner    (1001) docker     (127)    45933 2024-01-28 14:13:51.000000 django-static-base-0.1.5/requirements/py311-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-01-28 14:13:51.000000 django-static-base-0.1.5/requirements/py311-django32.txt
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-01-28 14:13:51.000000 django-static-base-0.1.5/requirements/py311-django42.txt
--rw-r--r--   0 runner    (1001) docker     (127)    46672 2024-01-28 14:13:51.000000 django-static-base-0.1.5/requirements/py38-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-01-28 14:13:51.000000 django-static-base-0.1.5/requirements/py38-django32.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-01-28 14:13:51.000000 django-static-base-0.1.5/requirements/py38-django42.txt
--rw-r--r--   0 runner    (1001) docker     (127)    46384 2024-01-28 14:13:51.000000 django-static-base-0.1.5/requirements/py39-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-01-28 14:13:51.000000 django-static-base-0.1.5/requirements/py39-django32.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-01-28 14:13:51.000000 django-static-base-0.1.5/requirements/py39-django42.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-28 14:13:51.000000 django-static-base-0.1.5/requirements/requirements.in
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-01-28 14:13:51.000000 django-static-base-0.1.5/runtests.py
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-01-28 14:14:03.809383 django-static-base-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-01-28 14:13:51.000000 django-static-base-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 14:14:03.729383 django-static-base-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 14:14:03.809383 django-static-base-0.1.5/src/django_static_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5820 2024-01-28 14:14:03.000000 django-static-base-0.1.5/src/django_static_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15938 2024-01-28 14:14:03.000000 django-static-base-0.1.5/src/django_static_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-28 14:14:03.000000 django-static-base-0.1.5/src/django_static_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-28 14:14:03.000000 django-static-base-0.1.5/src/django_static_base.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-01-28 14:14:03.000000 django-static-base-0.1.5/src/django_static_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-01-28 14:14:03.000000 django-static-base-0.1.5/src/django_static_base.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 14:14:03.737383 django-static-base-0.1.5/src/static_base/
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 14:14:03.729383 django-static-base-0.1.5/src/static_base/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 14:14:03.729383 django-static-base-0.1.5/src/static_base/static/base/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 14:14:03.749383 django-static-base-0.1.5/src/static_base/static/base/css/
--rw-r--r--   0 runner    (1001) docker     (127)    67473 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/bootstrap-grid.css
--rw-r--r--   0 runner    (1001) docker     (127)   163857 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/bootstrap-grid.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    50637 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/bootstrap-grid.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   115092 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/bootstrap-grid.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)     4785 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/bootstrap-reboot.css
--rw-r--r--   0 runner    (1001) docker     (127)    78155 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/bootstrap-reboot.css.map
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/bootstrap-reboot.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    33157 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/bootstrap-reboot.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)   200388 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)   515620 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/bootstrap.css.map
--rw-r--r--   0 runner    (1001) docker     (127)   162265 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   654594 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/bootstrap.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    17571 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/bootstrap5.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 14:14:03.753383 django-static-base-0.1.5/src/static_base/static/base/css/color/
--rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/color/aqua.css
--rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/color/blue.css
--rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/color/brown.css
--rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/color/forest.css
--rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/color/green.css
--rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/color/ice.css
--rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/color/navy.css
--rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/color/oasis.css
--rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/color/orange.css
--rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/color/pink.css
--rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/color/purple.css
--rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/color/red.css
--rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/color/salmon.css
--rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/color/sky.css
--rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/color/teal.css
--rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/color/yellow.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 14:14:03.753383 django-static-base-0.1.5/src/static_base/static/base/css/images/
--rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/images/loading.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 14:14:03.757383 django-static-base-0.1.5/src/static_base/static/base/css/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)    25949 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/plugins/aos.min.css
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/plugins/cocoen.min.css
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/plugins/cocoen.scss
--rw-r--r--   0 runner    (1001) docker     (127)    85494 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/plugins/cubeportfolio.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    15142 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/plugins/fotorama.css
--rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/plugins/jquery.smartmenus.bootstrap-4.css
--rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/plugins/justifiedGallery.min.css
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/plugins/lg-autoplay.css
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/plugins/lg-fullscreen.css
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/plugins/lg-pager.css
--rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/plugins/lg-share.css
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/plugins/lg-thumbnail.css
--rw-r--r--   0 runner    (1001) docker     (127)    39071 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/plugins/lg-transitions.css
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/plugins/lg-zoom.css
--rw-r--r--   0 runner    (1001) docker     (127)    34916 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/plugins/lightgallery-bundle.css
--rw-r--r--   0 runner    (1001) docker     (127)    29350 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/plugins/lightgallery-bundle.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    21528 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/plugins/lightgallery-bundle.min.old.css
--rw-r--r--   0 runner    (1001) docker     (127)    34916 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/plugins/lightgallery-bundle.old.css
--rw-r--r--   0 runner    (1001) docker     (127)    15550 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/plugins/lightgallery.css
--rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/plugins/render.css
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/plugins/sm-core-css.css
--rw-r--r--   0 runner    (1001) docker     (127)    19302 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/plugins/swiper-bundle.css
--rw-r--r--   0 runner    (1001) docker     (127)    16472 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/plugins/swiper-bundle.min.css
--rw-r--r--   0 runner    (1001) docker     (127)     5421 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/plugins/transitions.css
--rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/style-accordion.css
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/style-box.css
--rw-r--r--   0 runner    (1001) docker     (127)     9617 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/style-btn.css
--rw-r--r--   0 runner    (1001) docker     (127)     8802 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/style-color.css
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/style-cubeportfolio.css
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/style-dropdown.css
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/style-font-icons.css
--rw-r--r--   0 runner    (1001) docker     (127)     5866 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/style-forms.css
--rw-r--r--   0 runner    (1001) docker     (127)    11384 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/style-general.css
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/style-google-iframe.css
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/style-gototop.css
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/style-icon-profile.css
--rw-r--r--   0 runner    (1001) docker     (127)    10541 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/style-icon-social.css
--rw-r--r--   0 runner    (1001) docker     (127)     7063 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/style-inverse-text.css
--rw-r--r--   0 runner    (1001) docker     (127)     9570 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/style-lightgallery.css
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/style-list-group.css
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/style-list.css
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/style-loading.css
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/style-menu-ham.css
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/style-menu-mega.css
--rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/style-navbar.css
--rw-r--r--   0 runner    (1001) docker     (127)     8627 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/style-overlay.css
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/style-pricing.css
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/style-reset.css
--rw-r--r--   0 runner    (1001) docker     (127)    13011 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/style-responsive.css
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/style-scroll-animations.css
--rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/style-slider-revolution.css
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/style-sticky-header.css
--rw-r--r--   0 runner    (1001) docker     (127)     4656 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/style-swiper.css
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/style-tabs.css
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/style-tiles.css
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/style-widgets.css
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/style-wrapper-bg-image.css
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/style-wrapper-bg-video.css
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/css/style-wrapper-block-image.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 14:14:03.761383 django-static-base-0.1.5/src/static_base/static/base/js/
--rw-r--r--   0 runner    (1001) docker     (127)   230599 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/bootstrap.bundle.js
--rw-r--r--   0 runner    (1001) docker     (127)   426919 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/bootstrap.bundle.js.map
--rw-r--r--   0 runner    (1001) docker     (127)    83377 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/bootstrap.bundle.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   308872 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/bootstrap.bundle.min.js.map
--rw-r--r--   0 runner    (1001) docker     (127)   137714 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/bootstrap.js
--rw-r--r--   0 runner    (1001) docker     (127)   271785 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/bootstrap.js.map
--rw-r--r--   0 runner    (1001) docker     (127)    62564 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   185258 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/bootstrap.min.js.map
--rw-r--r--   0 runner    (1001) docker     (127)    13697 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/jquery.migrate.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    87533 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    70264 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/jquery.slim.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 14:14:03.777383 django-static-base-0.1.5/src/static_base/static/base/js/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)    14213 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/aos.min.js
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/cocoen-jquery.js
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/cocoen-jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/cocoen.js
--rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/cocoen.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/countdown.min.js
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/footerreveal.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    38913 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/fotorama.js
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/gototop.js
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/gototop.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     4946 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/headhesive.js
--rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/headhesive.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    34882 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/htmx.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     9965 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/imagesloaded.js
--rw-r--r--   0 runner    (1001) docker     (127)    12785 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/imagesloaded.pkgd.js
--rw-r--r--   0 runner    (1001) docker     (127)     5595 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/imagesloaded.pkgd.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/instantpage.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     6474 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/instastory.js
--rw-r--r--   0 runner    (1001) docker     (127)    52855 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/iscroll.js
--rw-r--r--   0 runner    (1001) docker     (127)    91397 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/isotope.pkgd.js
--rw-r--r--   0 runner    (1001) docker     (127)    35446 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/isotope.pkgd.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    46467 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/jquery.backstretch.js
--rw-r--r--   0 runner    (1001) docker     (127)    17491 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/jquery.backstretch.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    15108 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/jquery.collagePlus.js
--rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/jquery.collagePlus.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/jquery.counterup.js
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/jquery.counterup.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    12060 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/jquery.counterup.min.js.map
--rw-r--r--   0 runner    (1001) docker     (127)    81756 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/jquery.cubeportfolio.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/jquery.easing.js
--rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/jquery.easing.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/jquery.hmbrgr.js
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/jquery.hmbrgr.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    19309 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/jquery.justifiedGallery.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     8292 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/jquery.mousewheel.js
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/jquery.mousewheel.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     5915 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/jquery.smartmenus.bootstrap-4.js
--rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/jquery.smartmenus.bootstrap-4.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    45916 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/jquery.smartmenus.js
--rw-r--r--   0 runner    (1001) docker     (127)    24109 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/jquery.smartmenus.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    17947 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/jquery.waypoints.js
--rw-r--r--   0 runner    (1001) docker     (127)     9029 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/jquery.waypoints.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    19986 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/lazysizes.js
--rw-r--r--   0 runner    (1001) docker     (127)     7890 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/lazysizes.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/lg-autoplay.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     9222 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/lg-thumbnail.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    16351 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/lg-zoom.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    83995 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/lightgallery.js
--rw-r--r--   0 runner    (1001) docker     (127)    45246 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/lightgallery.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    18959 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/lightgallery.min.old.js
--rw-r--r--   0 runner    (1001) docker     (127)   119183 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/lightgallery.umd.js
--rw-r--r--   0 runner    (1001) docker     (127)    93750 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/localforage.js
--rw-r--r--   0 runner    (1001) docker     (127)    29704 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/localforage.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    44683 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/picturefill.js
--rw-r--r--   0 runner    (1001) docker     (127)    11808 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/picturefill.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    69293 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/popper.js
--rw-r--r--   0 runner    (1001) docker     (127)   152513 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/popper.js.map
--rw-r--r--   0 runner    (1001) docker     (127)    18795 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/popper.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   103396 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/popper.min.js.map
--rw-r--r--   0 runner    (1001) docker     (127)    15694 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/prettify.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    43146 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/progressbar.js
--rw-r--r--   0 runner    (1001) docker     (127)    29462 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/progressbar.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    37384 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/progressbar.min.js.map
--rw-r--r--   0 runner    (1001) docker     (127)   338840 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/swiper-bundle.js
--rw-r--r--   0 runner    (1001) docker     (127)   143571 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/swiper-bundle.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   540304 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/swiper-bundle.min.js.map
--rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/typer.js
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/whitespace.js
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/js/plugins/whitespace.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 14:14:03.781383 django-static-base-0.1.5/src/static_base/static/base/type/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 14:14:03.781383 django-static-base-0.1.5/src/static_base/static/base/type/elemis/
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/elemis/elemis.eot
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/elemis/elemis.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/elemis/elemis.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/elemis/elemis.woff
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/elemis/elemis.woff2
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/font-awesome.css
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/font-elemis.css
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/font-get-show.css
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/font-inclitodo.css
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/font-levorotary.css
--rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/font-montserrat.css
--rw-r--r--   0 runner    (1001) docker     (127)     8776 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/font-muli.css
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/font-rumpi.css
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/font-slimicons.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 14:14:03.785383 django-static-base-0.1.5/src/static_base/static/base/type/fontawesome/
--rw-r--r--   0 runner    (1001) docker     (127)   165742 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/fontawesome/fontawesome-webfont.eot
--rw-r--r--   0 runner    (1001) docker     (127)   443670 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/fontawesome/fontawesome-webfont.svg
--rw-r--r--   0 runner    (1001) docker     (127)   165548 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/fontawesome/fontawesome-webfont.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    98024 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/fontawesome/fontawesome-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (127)    77160 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/fontawesome/fontawesome-webfont.woff2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 14:14:03.785383 django-static-base-0.1.5/src/static_base/static/base/type/get_show/
--rw-r--r--   0 runner    (1001) docker     (127)   393288 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/get_show/Get Show.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    23800 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/get_show/GetShow.otf
--rw-r--r--   0 runner    (1001) docker     (127)    41872 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/get_show/GetShow.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    21272 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/get_show/GetShow.woff
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 14:14:03.729383 django-static-base-0.1.5/src/static_base/static/base/type/gstatic/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 14:14:03.729383 django-static-base-0.1.5/src/static_base/static/base/type/gstatic/s/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 14:14:03.729383 django-static-base-0.1.5/src/static_base/static/base/type/gstatic/s/muli/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 14:14:03.785383 django-static-base-0.1.5/src/static_base/static/base/type/gstatic/s/muli/v20/
--rw-r--r--   0 runner    (1001) docker     (127)    11572 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/gstatic/s/muli/v20/7Au-p_0qiz-afTf2IALT8kU.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    29512 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/gstatic/s/muli/v20/7Au-p_0qiz-afTf2IQLT8kU.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    32120 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/gstatic/s/muli/v20/7Au-p_0qiz-afTf2LwLT.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    10888 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/gstatic/s/muli/v20/7Auwp_0qiz-afT3GLRrX.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    31120 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/gstatic/s/muli/v20/7Auwp_0qiz-afTLGLQ.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    28508 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/gstatic/s/muli/v20/7Auwp_0qiz-afTzGLRrX.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   102971 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/icons.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 14:14:03.789383 django-static-base-0.1.5/src/static_base/static/base/type/inclitodo/
--rw-r--r--   0 runner    (1001) docker     (127)   165460 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/inclitodo/Inclitodo.otf
--rw-r--r--   0 runner    (1001) docker     (127)   203740 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/inclitodo/Inclitodo.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    69860 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/inclitodo/Inclitodo.woff
--rw-r--r--   0 runner    (1001) docker     (127)    54424 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/inclitodo/Inclitodo.woff2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 14:14:03.789383 django-static-base-0.1.5/src/static_base/static/base/type/levorotary/
--rw-r--r--   0 runner    (1001) docker     (127)   296056 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/levorotary/Levorotary.otf
--rw-r--r--   0 runner    (1001) docker     (127)    93900 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/levorotary/Levorotary.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    42968 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/levorotary/Levorotary.woff
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 14:14:03.789383 django-static-base-0.1.5/src/static_base/static/base/type/lg/
--rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/lg/lg.eot
--rw-r--r--   0 runner    (1001) docker     (127)    12835 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/lg/lg.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/lg/lg.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     4832 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/lg/lg.woff
--rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/lg/lg.woff2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 14:14:03.801383 django-static-base-0.1.5/src/static_base/static/base/type/montserrat/
--rw-r--r--   0 runner    (1001) docker     (127)    23516 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-Bold.eot
--rw-r--r--   0 runner    (1001) docker     (127)    23332 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    14084 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (127)    10012 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    36904 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-BoldItalic.eot
--rw-r--r--   0 runner    (1001) docker     (127)    36692 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-BoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    20856 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-BoldItalic.woff
--rw-r--r--   0 runner    (1001) docker     (127)    16276 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-BoldItalic.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    35132 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-Italic.eot
--rw-r--r--   0 runner    (1001) docker     (127)    34940 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    20516 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-Italic.woff
--rw-r--r--   0 runner    (1001) docker     (127)    15872 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-Italic.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    34528 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-Light.eot
--rw-r--r--   0 runner    (1001) docker     (127)    34324 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-Light.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    19916 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-Light.woff
--rw-r--r--   0 runner    (1001) docker     (127)    15604 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-Light.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    35576 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-LightItalic.eot
--rw-r--r--   0 runner    (1001) docker     (127)    35360 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-LightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    20740 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-LightItalic.woff
--rw-r--r--   0 runner    (1001) docker     (127)    16160 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-LightItalic.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    34928 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-Medium.eot
--rw-r--r--   0 runner    (1001) docker     (127)    34720 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-Medium.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    20044 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-Medium.woff
--rw-r--r--   0 runner    (1001) docker     (127)    15660 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-Medium.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    35900 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-MediumItalic.eot
--rw-r--r--   0 runner    (1001) docker     (127)    35680 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-MediumItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    20804 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-MediumItalic.woff
--rw-r--r--   0 runner    (1001) docker     (127)    16212 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-MediumItalic.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    23160 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-Regular.eot
--rw-r--r--   0 runner    (1001) docker     (127)    22964 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    14104 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (127)     9940 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    35080 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-SemiBold.eot
--rw-r--r--   0 runner    (1001) docker     (127)    34864 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-SemiBold.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    20128 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-SemiBold.woff
--rw-r--r--   0 runner    (1001) docker     (127)    15668 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-SemiBold.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    35860 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-SemiBoldItalic.eot
--rw-r--r--   0 runner    (1001) docker     (127)    35632 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-SemiBoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    20792 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-SemiBoldItalic.woff
--rw-r--r--   0 runner    (1001) docker     (127)    16200 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-SemiBoldItalic.woff2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 14:14:03.801383 django-static-base-0.1.5/src/static_base/static/base/type/rumpi/
--rw-r--r--   0 runner    (1001) docker     (127)   142144 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/rumpi/Rumpi.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    19352 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/rumpi/Rumpi.otf
--rw-r--r--   0 runner    (1001) docker     (127)    34488 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/rumpi/Rumpi.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    19740 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/rumpi/Rumpi.woff
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 14:14:03.805383 django-static-base-0.1.5/src/static_base/static/base/type/slimicons/
--rw-r--r--   0 runner    (1001) docker     (127)   507244 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/slimicons/Slimicons.eot
--rw-r--r--   0 runner    (1001) docker     (127)  2062337 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/slimicons/Slimicons.svg
--rw-r--r--   0 runner    (1001) docker     (127)   507072 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/slimicons/Slimicons.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   507148 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/slimicons/Slimicons.woff
--rw-r--r--   0 runner    (1001) docker     (127)   200076 2024-01-28 14:13:51.000000 django-static-base-0.1.5/src/static_base/static/base/type/slimicons/Slimicons.woff2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 14:14:03.809383 django-static-base-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-28 14:13:51.000000 django-static-base-0.1.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-01-28 14:13:51.000000 django-static-base-0.1.5/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-01-28 14:13:51.000000 django-static-base-0.1.5/tests/test_fake.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-01-28 14:13:51.000000 django-static-base-0.1.5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:48:58.674393 django-static-base-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-05 21:48:43.000000 django-static-base-0.1.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-05 21:48:43.000000 django-static-base-0.1.6/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-05 21:48:43.000000 django-static-base-0.1.6/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-05 21:48:43.000000 django-static-base-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-05 21:48:43.000000 django-static-base-0.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5820 2024-04-05 21:48:58.674393 django-static-base-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-04-05 21:48:43.000000 django-static-base-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-05 21:48:43.000000 django-static-base-0.1.6/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-05 21:48:43.000000 django-static-base-0.1.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:48:58.598393 django-static-base-0.1.6/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-05 21:48:43.000000 django-static-base-0.1.6/requirements/py310-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-05 21:48:43.000000 django-static-base-0.1.6/requirements/py310-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-05 21:48:43.000000 django-static-base-0.1.6/requirements/py311-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-05 21:48:43.000000 django-static-base-0.1.6/requirements/py311-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-04-05 21:48:43.000000 django-static-base-0.1.6/requirements/py38-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-05 21:48:43.000000 django-static-base-0.1.6/requirements/py38-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-04-05 21:48:43.000000 django-static-base-0.1.6/requirements/py39-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-05 21:48:43.000000 django-static-base-0.1.6/requirements/py39-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-05 21:48:43.000000 django-static-base-0.1.6/requirements/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-05 21:48:43.000000 django-static-base-0.1.6/runtests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-04-05 21:48:58.674393 django-static-base-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-05 21:48:43.000000 django-static-base-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:48:58.594393 django-static-base-0.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:48:58.670393 django-static-base-0.1.6/src/django_static_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5820 2024-04-05 21:48:58.000000 django-static-base-0.1.6/src/django_static_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15769 2024-04-05 21:48:58.000000 django-static-base-0.1.6/src/django_static_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 21:48:58.000000 django-static-base-0.1.6/src/django_static_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 21:48:58.000000 django-static-base-0.1.6/src/django_static_base.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-05 21:48:58.000000 django-static-base-0.1.6/src/django_static_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-05 21:48:58.000000 django-static-base-0.1.6/src/django_static_base.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:48:58.602393 django-static-base-0.1.6/src/static_base/
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:48:58.594393 django-static-base-0.1.6/src/static_base/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:48:58.594393 django-static-base-0.1.6/src/static_base/static/base/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:48:58.610393 django-static-base-0.1.6/src/static_base/static/base/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    67473 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/bootstrap-grid.css
+-rw-r--r--   0 runner    (1001) docker     (127)   163857 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/bootstrap-grid.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    50637 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/bootstrap-grid.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   115092 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/bootstrap-grid.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)     4785 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/bootstrap-reboot.css
+-rw-r--r--   0 runner    (1001) docker     (127)    78155 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/bootstrap-reboot.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/bootstrap-reboot.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    33157 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/bootstrap-reboot.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)   200388 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (127)   515620 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/bootstrap.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)   162265 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   654594 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/bootstrap.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    17571 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/bootstrap5.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:48:58.614393 django-static-base-0.1.6/src/static_base/static/base/css/color/
+-rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/color/aqua.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/color/blue.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/color/brown.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/color/forest.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/color/green.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/color/ice.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/color/navy.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/color/oasis.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/color/orange.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/color/pink.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/color/purple.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/color/red.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/color/salmon.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/color/sky.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/color/teal.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/color/yellow.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:48:58.614393 django-static-base-0.1.6/src/static_base/static/base/css/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/images/loading.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:48:58.618393 django-static-base-0.1.6/src/static_base/static/base/css/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)    25949 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/plugins/aos.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/plugins/cocoen.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/plugins/cocoen.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    85494 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/plugins/cubeportfolio.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    15142 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/plugins/fotorama.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/plugins/jquery.smartmenus.bootstrap-4.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/plugins/justifiedGallery.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/plugins/lg-autoplay.css
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/plugins/lg-fullscreen.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/plugins/lg-pager.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/plugins/lg-share.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/plugins/lg-thumbnail.css
+-rw-r--r--   0 runner    (1001) docker     (127)    39071 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/plugins/lg-transitions.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/plugins/lg-zoom.css
+-rw-r--r--   0 runner    (1001) docker     (127)    34916 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/plugins/lightgallery-bundle.css
+-rw-r--r--   0 runner    (1001) docker     (127)    29350 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/plugins/lightgallery-bundle.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    21528 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/plugins/lightgallery-bundle.min.old.css
+-rw-r--r--   0 runner    (1001) docker     (127)    34916 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/plugins/lightgallery-bundle.old.css
+-rw-r--r--   0 runner    (1001) docker     (127)    15550 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/plugins/lightgallery.css
+-rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/plugins/render.css
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/plugins/sm-core-css.css
+-rw-r--r--   0 runner    (1001) docker     (127)    19302 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/plugins/swiper-bundle.css
+-rw-r--r--   0 runner    (1001) docker     (127)    16472 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/plugins/swiper-bundle.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     5421 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/plugins/transitions.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/style-accordion.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/style-box.css
+-rw-r--r--   0 runner    (1001) docker     (127)     9617 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/style-btn.css
+-rw-r--r--   0 runner    (1001) docker     (127)     8802 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/style-color.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/style-cubeportfolio.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/style-dropdown.css
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/style-font-icons.css
+-rw-r--r--   0 runner    (1001) docker     (127)     5866 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/style-forms.css
+-rw-r--r--   0 runner    (1001) docker     (127)    11384 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/style-general.css
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/style-google-iframe.css
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/style-gototop.css
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/style-icon-profile.css
+-rw-r--r--   0 runner    (1001) docker     (127)    10541 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/style-icon-social.css
+-rw-r--r--   0 runner    (1001) docker     (127)     7063 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/style-inverse-text.css
+-rw-r--r--   0 runner    (1001) docker     (127)     9570 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/style-lightgallery.css
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/style-list-group.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/style-list.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/style-loading.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/style-menu-ham.css
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/style-menu-mega.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/style-navbar.css
+-rw-r--r--   0 runner    (1001) docker     (127)     8627 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/style-overlay.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/style-pricing.css
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/style-reset.css
+-rw-r--r--   0 runner    (1001) docker     (127)    13011 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/style-responsive.css
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/style-scroll-animations.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/style-slider-revolution.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/style-sticky-header.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4656 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/style-swiper.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/style-tabs.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/style-tiles.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/style-widgets.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/style-wrapper-bg-image.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/style-wrapper-bg-video.css
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/css/style-wrapper-block-image.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:48:58.626393 django-static-base-0.1.6/src/static_base/static/base/js/
+-rw-r--r--   0 runner    (1001) docker     (127)   230599 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/bootstrap.bundle.js
+-rw-r--r--   0 runner    (1001) docker     (127)   426919 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/bootstrap.bundle.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)    83377 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/bootstrap.bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   308872 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/bootstrap.bundle.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)   137714 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/bootstrap.js
+-rw-r--r--   0 runner    (1001) docker     (127)   271785 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/bootstrap.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)    62564 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   185258 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/bootstrap.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)    13697 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/jquery.migrate.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    87533 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    70264 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/jquery.slim.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:48:58.642393 django-static-base-0.1.6/src/static_base/static/base/js/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)    14213 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/aos.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/cocoen-jquery.js
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/cocoen-jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/cocoen.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/cocoen.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/countdown.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/footerreveal.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    38913 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/fotorama.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/gototop.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/gototop.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4946 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/headhesive.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/headhesive.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    34882 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/htmx.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9965 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/imagesloaded.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12785 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/imagesloaded.pkgd.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5595 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/imagesloaded.pkgd.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/instantpage.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6474 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/instastory.js
+-rw-r--r--   0 runner    (1001) docker     (127)    52855 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/iscroll.js
+-rw-r--r--   0 runner    (1001) docker     (127)    91397 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/isotope.pkgd.js
+-rw-r--r--   0 runner    (1001) docker     (127)    35446 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/isotope.pkgd.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    46467 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/jquery.backstretch.js
+-rw-r--r--   0 runner    (1001) docker     (127)    17491 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/jquery.backstretch.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15108 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/jquery.collagePlus.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/jquery.collagePlus.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/jquery.counterup.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/jquery.counterup.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12060 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/jquery.counterup.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)    81756 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/jquery.cubeportfolio.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/jquery.easing.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/jquery.easing.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/jquery.hmbrgr.js
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/jquery.hmbrgr.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    19309 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/jquery.justifiedGallery.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8292 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/jquery.mousewheel.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/jquery.mousewheel.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5915 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/jquery.smartmenus.bootstrap-4.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/jquery.smartmenus.bootstrap-4.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    45916 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/jquery.smartmenus.js
+-rw-r--r--   0 runner    (1001) docker     (127)    24109 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/jquery.smartmenus.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    17947 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/jquery.waypoints.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9029 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/jquery.waypoints.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    19986 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/lazysizes.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7890 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/lazysizes.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/lg-autoplay.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9222 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/lg-thumbnail.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    16351 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/lg-zoom.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    83995 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/lightgallery.js
+-rw-r--r--   0 runner    (1001) docker     (127)    45246 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/lightgallery.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    18959 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/lightgallery.min.old.js
+-rw-r--r--   0 runner    (1001) docker     (127)   119183 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/lightgallery.umd.js
+-rw-r--r--   0 runner    (1001) docker     (127)    93750 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/localforage.js
+-rw-r--r--   0 runner    (1001) docker     (127)    29704 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/localforage.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    44683 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/picturefill.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11808 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/picturefill.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    69293 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/popper.js
+-rw-r--r--   0 runner    (1001) docker     (127)   152513 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/popper.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)    18795 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/popper.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   103396 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/popper.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)    15694 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/prettify.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    43146 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/progressbar.js
+-rw-r--r--   0 runner    (1001) docker     (127)    29462 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/progressbar.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    37384 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/progressbar.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)   338840 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/swiper-bundle.js
+-rw-r--r--   0 runner    (1001) docker     (127)   143571 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/swiper-bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   540304 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/swiper-bundle.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/typer.js
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/whitespace.js
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/js/plugins/whitespace.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:48:58.642393 django-static-base-0.1.6/src/static_base/static/base/type/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:48:58.646393 django-static-base-0.1.6/src/static_base/static/base/type/elemis/
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/elemis/elemis.eot
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/elemis/elemis.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/elemis/elemis.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/elemis/elemis.woff
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/elemis/elemis.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/font-awesome.css
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/font-elemis.css
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/font-get-show.css
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/font-inclitodo.css
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/font-levorotary.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/font-montserrat.css
+-rw-r--r--   0 runner    (1001) docker     (127)     8776 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/font-muli.css
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/font-rumpi.css
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/font-slimicons.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:48:58.646393 django-static-base-0.1.6/src/static_base/static/base/type/fontawesome/
+-rw-r--r--   0 runner    (1001) docker     (127)   165742 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/fontawesome/fontawesome-webfont.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   443670 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/fontawesome/fontawesome-webfont.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   165548 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/fontawesome/fontawesome-webfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    98024 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/fontawesome/fontawesome-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    77160 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/fontawesome/fontawesome-webfont.woff2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:48:58.650393 django-static-base-0.1.6/src/static_base/static/base/type/get_show/
+-rw-r--r--   0 runner    (1001) docker     (127)   393288 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/get_show/Get Show.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    23800 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/get_show/GetShow.otf
+-rw-r--r--   0 runner    (1001) docker     (127)    41872 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/get_show/GetShow.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    21272 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/get_show/GetShow.woff
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:48:58.594393 django-static-base-0.1.6/src/static_base/static/base/type/gstatic/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:48:58.594393 django-static-base-0.1.6/src/static_base/static/base/type/gstatic/s/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:48:58.594393 django-static-base-0.1.6/src/static_base/static/base/type/gstatic/s/muli/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:48:58.650393 django-static-base-0.1.6/src/static_base/static/base/type/gstatic/s/muli/v20/
+-rw-r--r--   0 runner    (1001) docker     (127)    11572 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/gstatic/s/muli/v20/7Au-p_0qiz-afTf2IALT8kU.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    29512 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/gstatic/s/muli/v20/7Au-p_0qiz-afTf2IQLT8kU.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    32120 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/gstatic/s/muli/v20/7Au-p_0qiz-afTf2LwLT.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    10888 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/gstatic/s/muli/v20/7Auwp_0qiz-afT3GLRrX.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    31120 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/gstatic/s/muli/v20/7Auwp_0qiz-afTLGLQ.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    28508 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/gstatic/s/muli/v20/7Auwp_0qiz-afTzGLRrX.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   102971 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/icons.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:48:58.650393 django-static-base-0.1.6/src/static_base/static/base/type/inclitodo/
+-rw-r--r--   0 runner    (1001) docker     (127)   165460 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/inclitodo/Inclitodo.otf
+-rw-r--r--   0 runner    (1001) docker     (127)   203740 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/inclitodo/Inclitodo.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    69860 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/inclitodo/Inclitodo.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    54424 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/inclitodo/Inclitodo.woff2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:48:58.654393 django-static-base-0.1.6/src/static_base/static/base/type/levorotary/
+-rw-r--r--   0 runner    (1001) docker     (127)   296056 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/levorotary/Levorotary.otf
+-rw-r--r--   0 runner    (1001) docker     (127)    93900 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/levorotary/Levorotary.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    42968 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/levorotary/Levorotary.woff
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:48:58.654393 django-static-base-0.1.6/src/static_base/static/base/type/lg/
+-rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/lg/lg.eot
+-rw-r--r--   0 runner    (1001) docker     (127)    12835 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/lg/lg.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/lg/lg.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     4832 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/lg/lg.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/lg/lg.woff2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:48:58.662393 django-static-base-0.1.6/src/static_base/static/base/type/montserrat/
+-rw-r--r--   0 runner    (1001) docker     (127)    23516 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-Bold.eot
+-rw-r--r--   0 runner    (1001) docker     (127)    23332 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    14084 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    10012 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    36904 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-BoldItalic.eot
+-rw-r--r--   0 runner    (1001) docker     (127)    36692 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    20856 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-BoldItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    16276 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-BoldItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    35132 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-Italic.eot
+-rw-r--r--   0 runner    (1001) docker     (127)    34940 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    20516 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-Italic.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    15872 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-Italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    34528 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-Light.eot
+-rw-r--r--   0 runner    (1001) docker     (127)    34324 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-Light.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    19916 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-Light.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    15604 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-Light.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    35576 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-LightItalic.eot
+-rw-r--r--   0 runner    (1001) docker     (127)    35360 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-LightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    20740 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-LightItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    16160 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-LightItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    34928 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-Medium.eot
+-rw-r--r--   0 runner    (1001) docker     (127)    34720 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-Medium.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    20044 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-Medium.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    15660 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-Medium.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    35900 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-MediumItalic.eot
+-rw-r--r--   0 runner    (1001) docker     (127)    35680 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-MediumItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    20804 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-MediumItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    16212 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-MediumItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    23160 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-Regular.eot
+-rw-r--r--   0 runner    (1001) docker     (127)    22964 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    14104 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     9940 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    35080 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-SemiBold.eot
+-rw-r--r--   0 runner    (1001) docker     (127)    34864 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-SemiBold.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    20128 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-SemiBold.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    15668 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-SemiBold.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    35860 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-SemiBoldItalic.eot
+-rw-r--r--   0 runner    (1001) docker     (127)    35632 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-SemiBoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    20792 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-SemiBoldItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    16200 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-SemiBoldItalic.woff2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:48:58.662393 django-static-base-0.1.6/src/static_base/static/base/type/rumpi/
+-rw-r--r--   0 runner    (1001) docker     (127)   142144 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/rumpi/Rumpi.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    19352 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/rumpi/Rumpi.otf
+-rw-r--r--   0 runner    (1001) docker     (127)    34488 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/rumpi/Rumpi.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    19740 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/rumpi/Rumpi.woff
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:48:58.670393 django-static-base-0.1.6/src/static_base/static/base/type/slimicons/
+-rw-r--r--   0 runner    (1001) docker     (127)   507244 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/slimicons/Slimicons.eot
+-rw-r--r--   0 runner    (1001) docker     (127)  2062337 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/slimicons/Slimicons.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   507072 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/slimicons/Slimicons.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   507148 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/slimicons/Slimicons.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   200076 2024-04-05 21:48:43.000000 django-static-base-0.1.6/src/static_base/static/base/type/slimicons/Slimicons.woff2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:48:58.670393 django-static-base-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 21:48:43.000000 django-static-base-0.1.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-05 21:48:43.000000 django-static-base-0.1.6/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-05 21:48:43.000000 django-static-base-0.1.6/tests/test_fake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-05 21:48:43.000000 django-static-base-0.1.6/tox.ini
```

### Comparing `django-static-base-0.1.5/.pre-commit-config.yaml` & `django-static-base-0.1.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/LICENSE` & `django-static-base-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/PKG-INFO` & `django-static-base-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-static-base
-Version: 0.1.5
+Version: 0.1.6
 Summary: Django's application to serve up-to-date common static files (JQuery, Bootstrap, Plugins, ...) as "base" static directory
 Home-page: https://github.com/DLRSP/django-static-base
 Author: DLRSP
 Author-email: dlrsp.dev@gmail.com
 License: MIT License
 Project-URL: Documentation, https://dlrsp.github.io/django-static-base/
 Project-URL: Source, https://github.com/DLRSP/django-static-base
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-static-base Version: 0.1.5 Summary: Django's
+Metadata-Version: 2.1 Name: django-static-base Version: 0.1.6 Summary: Django's
 application to serve up-to-date common static files (JQuery, Bootstrap,
 Plugins, ...) as "base" static directory Home-page: https://github.com/DLRSP/
 django-static-base Author: DLRSP Author-email: dlrsp.dev@gmail.com License: MIT
 License Project-URL: Documentation, https://dlrsp.github.io/django-static-base/
 Project-URL: Source, https://github.com/DLRSP/django-static-base Project-URL:
 Tracker, https://github.com/DLRSP/django-static-base/issues Keywords: django
 Classifier: Development Status :: 4 - Beta Classifier: Environment :: Web
```

### Comparing `django-static-base-0.1.5/README.md` & `django-static-base-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/mkdocs.yml` & `django-static-base-0.1.6/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/pyproject.toml` & `django-static-base-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     --strict-markers
     --ds=tests.settings
     """
 django_find_project = false
 
 # bump-my-version
 [tool.bumpversion]
-current_version = "0.1.5"
+current_version = "0.1.6"
 commit = true
 tag = true
 allow_dirty = true
 
 [[tool.bumpversion.files]]
 filename = "./setup.cfg"
```

### Comparing `django-static-base-0.1.5/requirements/py310-django32.txt` & `django-static-base-0.1.6/requirements/py311-django32.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    pip-compile --allow-unsafe --generate-hashes --output-file=requirements/py310-django32.txt requirements/requirements.in
+#    pip-compile --allow-unsafe --generate-hashes --output-file=requirements/py311-django32.txt requirements/requirements.in
 #
-asgiref==3.7.2 \
-    --hash=sha256:89b2ef2247e3b562a16eef663bc0e2e703ec6468e2fa8a5cd61cd449786d4f6e \
-    --hash=sha256:9e0ce3aa93a819ba5b45120216b23878cf6e8525eb3848653452b4192b92afed
+asgiref==3.8.1 \
+    --hash=sha256:3e1e3ecc849832fe52ccf2cb6686b7a55f82bb1d6aee72a58826471390335e47 \
+    --hash=sha256:c343bd80a0bec947a9860adb4c432ffa7db769836c64238fc34bdc3fec84d590
     # via django
-django==3.2.23 \
-    --hash=sha256:82968f3640e29ef4a773af2c28448f5f7a08d001c6ac05b32d02aeee6509508b \
-    --hash=sha256:d48608d5f62f2c1e260986835db089fa3b79d6f58510881d316b8d88345ae6e1
+django==3.2.25 \
+    --hash=sha256:7ca38a78654aee72378594d63e51636c04b8e28574f5505dff630895b5472777 \
+    --hash=sha256:a52ea7fcf280b16f7b739cec38fa6d3f8953a5456986944c3ca97e79882b4e38
     # via -r requirements/requirements.in
-pytz==2023.3.post1 \
-    --hash=sha256:7b4fddbeb94a1eba4b557da24f19fdf9db575192544270a9101d8509f9f43d7b \
-    --hash=sha256:ce42d816b81b68506614c11e8937d3aa9e41007ceb50bfdcb0749b921bf646c7
+pytz==2024.1 \
+    --hash=sha256:2a29735ea9c18baf14b448846bde5a48030ed267578472d8955cd0e7443a9812 \
+    --hash=sha256:328171f4e3623139da4983451950b28e95ac706e13f3f2630a879749e7a8b319
     # via django
 sqlparse==0.4.4 \
     --hash=sha256:5430a4fe2ac7d0f93e66f1efc6e1338a41884b7ddf2a350cedd20ccc4d9d28f3 \
     --hash=sha256:d446183e84b8349fa3061f0fe7f06ca94ba65b426946ffebe6e3e8295332420c
     # via django
-typing-extensions==4.9.0 \
-    --hash=sha256:23478f88c37f27d76ac8aee6c905017a143b0b1b886c3c9f66bc2fd94f9f5783 \
-    --hash=sha256:af72aea155e91adfc61c3ae9e0e342dbc0cba726d6cba4b6c72c1f34e47291cd
-    # via asgiref
```

### Comparing `django-static-base-0.1.5/requirements/py310-django42.txt` & `django-static-base-0.1.6/requirements/py311-django42.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    pip-compile --allow-unsafe --generate-hashes --output-file=requirements/py310-django42.txt requirements/requirements.in
+#    pip-compile --allow-unsafe --generate-hashes --output-file=requirements/py311-django42.txt requirements/requirements.in
 #
-asgiref==3.7.2 \
-    --hash=sha256:89b2ef2247e3b562a16eef663bc0e2e703ec6468e2fa8a5cd61cd449786d4f6e \
-    --hash=sha256:9e0ce3aa93a819ba5b45120216b23878cf6e8525eb3848653452b4192b92afed
+asgiref==3.8.1 \
+    --hash=sha256:3e1e3ecc849832fe52ccf2cb6686b7a55f82bb1d6aee72a58826471390335e47 \
+    --hash=sha256:c343bd80a0bec947a9860adb4c432ffa7db769836c64238fc34bdc3fec84d590
     # via django
-django==4.2.9 \
-    --hash=sha256:12498cc3cb8bc8038539fef9e90e95f507502436c1f0c3a673411324fa675d14 \
-    --hash=sha256:2cc2fc7d1708ada170ddd6c99f35cc25db664f165d3794bc7723f46b2f8c8984
+django==4.2.11 \
+    --hash=sha256:6e6ff3db2d8dd0c986b4eec8554c8e4f919b5c1ff62a5b4390c17aff2ed6e5c4 \
+    --hash=sha256:ddc24a0a8280a0430baa37aff11f28574720af05888c62b7cfe71d219f4599d3
     # via -r requirements/requirements.in
 sqlparse==0.4.4 \
     --hash=sha256:5430a4fe2ac7d0f93e66f1efc6e1338a41884b7ddf2a350cedd20ccc4d9d28f3 \
     --hash=sha256:d446183e84b8349fa3061f0fe7f06ca94ba65b426946ffebe6e3e8295332420c
     # via django
-typing-extensions==4.9.0 \
-    --hash=sha256:23478f88c37f27d76ac8aee6c905017a143b0b1b886c3c9f66bc2fd94f9f5783 \
-    --hash=sha256:af72aea155e91adfc61c3ae9e0e342dbc0cba726d6cba4b6c72c1f34e47291cd
-    # via asgiref
```

### Comparing `django-static-base-0.1.5/requirements/py311-django32.txt` & `django-static-base-0.1.6/requirements/py310-django32.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 #
-# This file is autogenerated by pip-compile with Python 3.11
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --allow-unsafe --generate-hashes --output-file=requirements/py311-django32.txt requirements/requirements.in
+#    pip-compile --allow-unsafe --generate-hashes --output-file=requirements/py310-django32.txt requirements/requirements.in
 #
-asgiref==3.7.2 \
-    --hash=sha256:89b2ef2247e3b562a16eef663bc0e2e703ec6468e2fa8a5cd61cd449786d4f6e \
-    --hash=sha256:9e0ce3aa93a819ba5b45120216b23878cf6e8525eb3848653452b4192b92afed
+asgiref==3.8.1 \
+    --hash=sha256:3e1e3ecc849832fe52ccf2cb6686b7a55f82bb1d6aee72a58826471390335e47 \
+    --hash=sha256:c343bd80a0bec947a9860adb4c432ffa7db769836c64238fc34bdc3fec84d590
     # via django
-django==3.2.23 \
-    --hash=sha256:82968f3640e29ef4a773af2c28448f5f7a08d001c6ac05b32d02aeee6509508b \
-    --hash=sha256:d48608d5f62f2c1e260986835db089fa3b79d6f58510881d316b8d88345ae6e1
+django==3.2.25 \
+    --hash=sha256:7ca38a78654aee72378594d63e51636c04b8e28574f5505dff630895b5472777 \
+    --hash=sha256:a52ea7fcf280b16f7b739cec38fa6d3f8953a5456986944c3ca97e79882b4e38
     # via -r requirements/requirements.in
-pytz==2023.3.post1 \
-    --hash=sha256:7b4fddbeb94a1eba4b557da24f19fdf9db575192544270a9101d8509f9f43d7b \
-    --hash=sha256:ce42d816b81b68506614c11e8937d3aa9e41007ceb50bfdcb0749b921bf646c7
+pytz==2024.1 \
+    --hash=sha256:2a29735ea9c18baf14b448846bde5a48030ed267578472d8955cd0e7443a9812 \
+    --hash=sha256:328171f4e3623139da4983451950b28e95ac706e13f3f2630a879749e7a8b319
     # via django
 sqlparse==0.4.4 \
     --hash=sha256:5430a4fe2ac7d0f93e66f1efc6e1338a41884b7ddf2a350cedd20ccc4d9d28f3 \
     --hash=sha256:d446183e84b8349fa3061f0fe7f06ca94ba65b426946ffebe6e3e8295332420c
     # via django
+typing-extensions==4.10.0 \
+    --hash=sha256:69b1a937c3a517342112fb4c6df7e72fc39a38e7891a5730ed4985b5214b5475 \
+    --hash=sha256:b0abd7c89e8fb96f98db18d86106ff1d90ab692004eb746cf6eda2682f91b3cb
+    # via asgiref
```

### Comparing `django-static-base-0.1.5/requirements/py38-django42.txt` & `django-static-base-0.1.6/requirements/py38-django42.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #
 # This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
 #    pip-compile --allow-unsafe --generate-hashes --output-file=requirements/py38-django42.txt requirements/requirements.in
 #
-asgiref==3.7.2 \
-    --hash=sha256:89b2ef2247e3b562a16eef663bc0e2e703ec6468e2fa8a5cd61cd449786d4f6e \
-    --hash=sha256:9e0ce3aa93a819ba5b45120216b23878cf6e8525eb3848653452b4192b92afed
+asgiref==3.8.1 \
+    --hash=sha256:3e1e3ecc849832fe52ccf2cb6686b7a55f82bb1d6aee72a58826471390335e47 \
+    --hash=sha256:c343bd80a0bec947a9860adb4c432ffa7db769836c64238fc34bdc3fec84d590
     # via django
 backports-zoneinfo==0.2.1 \
     --hash=sha256:17746bd546106fa389c51dbea67c8b7c8f0d14b5526a579ca6ccf5ed72c526cf \
     --hash=sha256:1b13e654a55cd45672cb54ed12148cd33628f672548f373963b0bff67b217328 \
     --hash=sha256:1c5742112073a563c81f786e77514969acb58649bcdf6cdf0b4ed31a348d4546 \
     --hash=sha256:4a0f800587060bf8880f954dbef70de6c11bbe59c673c3d818921f042f9954a6 \
     --hash=sha256:5c144945a7752ca544b4b78c8c41544cdfaf9786f25fe5ffb10e838e19a27570 \
@@ -22,19 +22,19 @@
     --hash=sha256:da6013fd84a690242c310d77ddb8441a559e9cb3d3d59ebac9aca1a57b2e18bc \
     --hash=sha256:e55b384612d93be96506932a786bbcde5a2db7a9e6a4bb4bffe8b733f5b9036b \
     --hash=sha256:e81b76cace8eda1fca50e345242ba977f9be6ae3945af8d46326d776b4cf78d1 \
     --hash=sha256:e8236383a20872c0cdf5a62b554b27538db7fa1bbec52429d8d106effbaeca08 \
     --hash=sha256:f04e857b59d9d1ccc39ce2da1021d196e47234873820cbeaad210724b1ee28ac \
     --hash=sha256:fadbfe37f74051d024037f223b8e001611eac868b5c5b06144ef4d8b799862f2
     # via django
-django==4.2.9 \
-    --hash=sha256:12498cc3cb8bc8038539fef9e90e95f507502436c1f0c3a673411324fa675d14 \
-    --hash=sha256:2cc2fc7d1708ada170ddd6c99f35cc25db664f165d3794bc7723f46b2f8c8984
+django==4.2.11 \
+    --hash=sha256:6e6ff3db2d8dd0c986b4eec8554c8e4f919b5c1ff62a5b4390c17aff2ed6e5c4 \
+    --hash=sha256:ddc24a0a8280a0430baa37aff11f28574720af05888c62b7cfe71d219f4599d3
     # via -r requirements/requirements.in
 sqlparse==0.4.4 \
     --hash=sha256:5430a4fe2ac7d0f93e66f1efc6e1338a41884b7ddf2a350cedd20ccc4d9d28f3 \
     --hash=sha256:d446183e84b8349fa3061f0fe7f06ca94ba65b426946ffebe6e3e8295332420c
     # via django
-typing-extensions==4.9.0 \
-    --hash=sha256:23478f88c37f27d76ac8aee6c905017a143b0b1b886c3c9f66bc2fd94f9f5783 \
-    --hash=sha256:af72aea155e91adfc61c3ae9e0e342dbc0cba726d6cba4b6c72c1f34e47291cd
+typing-extensions==4.10.0 \
+    --hash=sha256:69b1a937c3a517342112fb4c6df7e72fc39a38e7891a5730ed4985b5214b5475 \
+    --hash=sha256:b0abd7c89e8fb96f98db18d86106ff1d90ab692004eb746cf6eda2682f91b3cb
     # via asgiref
```

### Comparing `django-static-base-0.1.5/runtests.py` & `django-static-base-0.1.6/runtests.py`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/setup.cfg` & `django-static-base-0.1.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [bdist_wheel]
 universal = 1
 
 [metadata]
 name = django-static-base
-version = 0.1.5
+version = 0.1.6
 url = https://github.com/DLRSP/django-static-base
 project_urls = 
 	Documentation = https://dlrsp.github.io/django-static-base/
 	Source = https://github.com/DLRSP/django-static-base
 	Tracker = https://github.com/DLRSP/django-static-base/issues
 author = DLRSP
 author_email = dlrsp.dev@gmail.com
```

### Comparing `django-static-base-0.1.5/setup.py` & `django-static-base-0.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/django_static_base.egg-info/PKG-INFO` & `django-static-base-0.1.6/src/django_static_base.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-static-base
-Version: 0.1.5
+Version: 0.1.6
 Summary: Django's application to serve up-to-date common static files (JQuery, Bootstrap, Plugins, ...) as "base" static directory
 Home-page: https://github.com/DLRSP/django-static-base
 Author: DLRSP
 Author-email: dlrsp.dev@gmail.com
 License: MIT License
 Project-URL: Documentation, https://dlrsp.github.io/django-static-base/
 Project-URL: Source, https://github.com/DLRSP/django-static-base
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-static-base Version: 0.1.5 Summary: Django's
+Metadata-Version: 2.1 Name: django-static-base Version: 0.1.6 Summary: Django's
 application to serve up-to-date common static files (JQuery, Bootstrap,
 Plugins, ...) as "base" static directory Home-page: https://github.com/DLRSP/
 django-static-base Author: DLRSP Author-email: dlrsp.dev@gmail.com License: MIT
 License Project-URL: Documentation, https://dlrsp.github.io/django-static-base/
 Project-URL: Source, https://github.com/DLRSP/django-static-base Project-URL:
 Tracker, https://github.com/DLRSP/django-static-base/issues Keywords: django
 Classifier: Development Status :: 4 - Beta Classifier: Environment :: Web
```

### Comparing `django-static-base-0.1.5/src/django_static_base.egg-info/SOURCES.txt` & `django-static-base-0.1.6/src/django_static_base.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,27 +6,20 @@
 README.md
 mkdocs.yml
 pyproject.toml
 runtests.py
 setup.cfg
 setup.py
 tox.ini
-requirements/dev.in
-requirements/docs.in
-requirements/docs.txt
-requirements/py310-dev.txt
 requirements/py310-django32.txt
 requirements/py310-django42.txt
-requirements/py311-dev.txt
 requirements/py311-django32.txt
 requirements/py311-django42.txt
-requirements/py38-dev.txt
 requirements/py38-django32.txt
 requirements/py38-django42.txt
-requirements/py39-dev.txt
 requirements/py39-django32.txt
 requirements/py39-django42.txt
 requirements/requirements.in
 src/django_static_base.egg-info/PKG-INFO
 src/django_static_base.egg-info/SOURCES.txt
 src/django_static_base.egg-info/dependency_links.txt
 src/django_static_base.egg-info/not-zip-safe
```

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/bootstrap-grid.css` & `django-static-base-0.1.6/src/static_base/static/base/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/bootstrap-grid.css.map` & `django-static-base-0.1.6/src/static_base/static/base/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/bootstrap-grid.min.css` & `django-static-base-0.1.6/src/static_base/static/base/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/bootstrap-grid.min.css.map` & `django-static-base-0.1.6/src/static_base/static/base/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/bootstrap-reboot.css` & `django-static-base-0.1.6/src/static_base/static/base/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/bootstrap-reboot.css.map` & `django-static-base-0.1.6/src/static_base/static/base/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/bootstrap-reboot.min.css` & `django-static-base-0.1.6/src/static_base/static/base/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/bootstrap-reboot.min.css.map` & `django-static-base-0.1.6/src/static_base/static/base/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/bootstrap.css` & `django-static-base-0.1.6/src/static_base/static/base/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/bootstrap.css.map` & `django-static-base-0.1.6/src/static_base/static/base/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/bootstrap.min.css` & `django-static-base-0.1.6/src/static_base/static/base/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/bootstrap.min.css.map` & `django-static-base-0.1.6/src/static_base/static/base/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/bootstrap5.min.css` & `django-static-base-0.1.6/src/static_base/static/base/css/bootstrap5.min.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/color/aqua.css` & `django-static-base-0.1.6/src/static_base/static/base/css/color/aqua.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/color/blue.css` & `django-static-base-0.1.6/src/static_base/static/base/css/color/blue.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/color/brown.css` & `django-static-base-0.1.6/src/static_base/static/base/css/color/brown.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/color/forest.css` & `django-static-base-0.1.6/src/static_base/static/base/css/color/forest.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/color/green.css` & `django-static-base-0.1.6/src/static_base/static/base/css/color/green.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/color/ice.css` & `django-static-base-0.1.6/src/static_base/static/base/css/color/ice.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/color/navy.css` & `django-static-base-0.1.6/src/static_base/static/base/css/color/navy.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/color/oasis.css` & `django-static-base-0.1.6/src/static_base/static/base/css/color/oasis.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/color/orange.css` & `django-static-base-0.1.6/src/static_base/static/base/css/color/orange.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/color/pink.css` & `django-static-base-0.1.6/src/static_base/static/base/css/color/pink.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/color/purple.css` & `django-static-base-0.1.6/src/static_base/static/base/css/color/purple.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/color/red.css` & `django-static-base-0.1.6/src/static_base/static/base/css/color/red.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/color/salmon.css` & `django-static-base-0.1.6/src/static_base/static/base/css/color/salmon.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/color/sky.css` & `django-static-base-0.1.6/src/static_base/static/base/css/color/sky.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/color/teal.css` & `django-static-base-0.1.6/src/static_base/static/base/css/color/teal.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/color/yellow.css` & `django-static-base-0.1.6/src/static_base/static/base/css/color/yellow.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/images/loading.gif` & `django-static-base-0.1.6/src/static_base/static/base/css/images/loading.gif`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/plugins/aos.min.css` & `django-static-base-0.1.6/src/static_base/static/base/css/plugins/aos.min.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/plugins/cocoen.min.css` & `django-static-base-0.1.6/src/static_base/static/base/css/plugins/cocoen.min.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/plugins/cocoen.scss` & `django-static-base-0.1.6/src/static_base/static/base/css/plugins/cocoen.scss`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/plugins/cubeportfolio.min.css` & `django-static-base-0.1.6/src/static_base/static/base/css/plugins/cubeportfolio.min.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/plugins/fotorama.css` & `django-static-base-0.1.6/src/static_base/static/base/css/plugins/fotorama.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/plugins/jquery.smartmenus.bootstrap-4.css` & `django-static-base-0.1.6/src/static_base/static/base/css/plugins/jquery.smartmenus.bootstrap-4.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/plugins/justifiedGallery.min.css` & `django-static-base-0.1.6/src/static_base/static/base/css/plugins/justifiedGallery.min.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/plugins/lg-autoplay.css` & `django-static-base-0.1.6/src/static_base/static/base/css/plugins/lg-autoplay.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/plugins/lg-pager.css` & `django-static-base-0.1.6/src/static_base/static/base/css/plugins/lg-pager.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/plugins/lg-share.css` & `django-static-base-0.1.6/src/static_base/static/base/css/plugins/lg-share.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/plugins/lg-thumbnail.css` & `django-static-base-0.1.6/src/static_base/static/base/css/plugins/lg-thumbnail.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/plugins/lg-transitions.css` & `django-static-base-0.1.6/src/static_base/static/base/css/plugins/lg-transitions.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/plugins/lg-zoom.css` & `django-static-base-0.1.6/src/static_base/static/base/css/plugins/lg-zoom.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/plugins/lightgallery-bundle.css` & `django-static-base-0.1.6/src/static_base/static/base/css/plugins/lightgallery-bundle.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/plugins/lightgallery-bundle.min.css` & `django-static-base-0.1.6/src/static_base/static/base/css/plugins/lightgallery-bundle.min.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/plugins/lightgallery-bundle.min.old.css` & `django-static-base-0.1.6/src/static_base/static/base/css/plugins/lightgallery-bundle.min.old.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/plugins/lightgallery-bundle.old.css` & `django-static-base-0.1.6/src/static_base/static/base/css/plugins/lightgallery-bundle.old.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/plugins/lightgallery.css` & `django-static-base-0.1.6/src/static_base/static/base/css/plugins/lightgallery.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/plugins/render.css` & `django-static-base-0.1.6/src/static_base/static/base/css/plugins/render.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/plugins/sm-core-css.css` & `django-static-base-0.1.6/src/static_base/static/base/css/plugins/sm-core-css.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/plugins/swiper-bundle.css` & `django-static-base-0.1.6/src/static_base/static/base/css/plugins/swiper-bundle.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/plugins/swiper-bundle.min.css` & `django-static-base-0.1.6/src/static_base/static/base/css/plugins/swiper-bundle.min.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/plugins/transitions.css` & `django-static-base-0.1.6/src/static_base/static/base/css/plugins/transitions.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/style-accordion.css` & `django-static-base-0.1.6/src/static_base/static/base/css/style-accordion.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/style-box.css` & `django-static-base-0.1.6/src/static_base/static/base/css/style-box.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/style-btn.css` & `django-static-base-0.1.6/src/static_base/static/base/css/style-btn.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/style-color.css` & `django-static-base-0.1.6/src/static_base/static/base/css/style-color.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/style-cubeportfolio.css` & `django-static-base-0.1.6/src/static_base/static/base/css/style-cubeportfolio.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/style-dropdown.css` & `django-static-base-0.1.6/src/static_base/static/base/css/style-dropdown.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/style-font-icons.css` & `django-static-base-0.1.6/src/static_base/static/base/css/style-font-icons.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/style-forms.css` & `django-static-base-0.1.6/src/static_base/static/base/css/style-forms.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/style-general.css` & `django-static-base-0.1.6/src/static_base/static/base/css/style-general.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/style-gototop.css` & `django-static-base-0.1.6/src/static_base/static/base/css/style-gototop.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/style-icon-profile.css` & `django-static-base-0.1.6/src/static_base/static/base/css/style-icon-profile.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/style-icon-social.css` & `django-static-base-0.1.6/src/static_base/static/base/css/style-icon-social.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/style-inverse-text.css` & `django-static-base-0.1.6/src/static_base/static/base/css/style-inverse-text.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/style-lightgallery.css` & `django-static-base-0.1.6/src/static_base/static/base/css/style-lightgallery.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/style-list-group.css` & `django-static-base-0.1.6/src/static_base/static/base/css/style-list-group.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/style-list.css` & `django-static-base-0.1.6/src/static_base/static/base/css/style-list.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/style-loading.css` & `django-static-base-0.1.6/src/static_base/static/base/css/style-loading.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/style-menu-ham.css` & `django-static-base-0.1.6/src/static_base/static/base/css/style-menu-ham.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/style-navbar.css` & `django-static-base-0.1.6/src/static_base/static/base/css/style-navbar.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/style-overlay.css` & `django-static-base-0.1.6/src/static_base/static/base/css/style-overlay.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/style-pricing.css` & `django-static-base-0.1.6/src/static_base/static/base/css/style-pricing.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/style-reset.css` & `django-static-base-0.1.6/src/static_base/static/base/css/style-reset.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/style-responsive.css` & `django-static-base-0.1.6/src/static_base/static/base/css/style-responsive.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/style-scroll-animations.css` & `django-static-base-0.1.6/src/static_base/static/base/css/style-scroll-animations.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/style-slider-revolution.css` & `django-static-base-0.1.6/src/static_base/static/base/css/style-slider-revolution.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/style-sticky-header.css` & `django-static-base-0.1.6/src/static_base/static/base/css/style-sticky-header.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/style-swiper.css` & `django-static-base-0.1.6/src/static_base/static/base/css/style-swiper.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/style-tabs.css` & `django-static-base-0.1.6/src/static_base/static/base/css/style-tabs.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/style-tiles.css` & `django-static-base-0.1.6/src/static_base/static/base/css/style-tiles.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/style-widgets.css` & `django-static-base-0.1.6/src/static_base/static/base/css/style-widgets.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/style-wrapper-bg-image.css` & `django-static-base-0.1.6/src/static_base/static/base/css/style-wrapper-bg-image.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/style-wrapper-bg-video.css` & `django-static-base-0.1.6/src/static_base/static/base/css/style-wrapper-bg-video.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/css/style-wrapper-block-image.css` & `django-static-base-0.1.6/src/static_base/static/base/css/style-wrapper-block-image.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/bootstrap.bundle.js` & `django-static-base-0.1.6/src/static_base/static/base/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/bootstrap.bundle.js.map` & `django-static-base-0.1.6/src/static_base/static/base/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/bootstrap.bundle.min.js` & `django-static-base-0.1.6/src/static_base/static/base/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/bootstrap.bundle.min.js.map` & `django-static-base-0.1.6/src/static_base/static/base/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/bootstrap.js` & `django-static-base-0.1.6/src/static_base/static/base/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/bootstrap.js.map` & `django-static-base-0.1.6/src/static_base/static/base/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/bootstrap.min.js` & `django-static-base-0.1.6/src/static_base/static/base/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/bootstrap.min.js.map` & `django-static-base-0.1.6/src/static_base/static/base/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/jquery.migrate.min.js` & `django-static-base-0.1.6/src/static_base/static/base/js/jquery.migrate.min.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/jquery.min.js` & `django-static-base-0.1.6/src/static_base/static/base/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/jquery.slim.min.js` & `django-static-base-0.1.6/src/static_base/static/base/js/jquery.slim.min.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/aos.min.js` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/aos.min.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/cocoen-jquery.min.js` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/cocoen-jquery.min.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/cocoen.js` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/cocoen.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/cocoen.min.js` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/cocoen.min.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/countdown.min.js` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/countdown.min.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/footerreveal.min.js` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/footerreveal.min.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/fotorama.js` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/fotorama.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/gototop.js` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/gototop.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/gototop.min.js` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/gototop.min.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/headhesive.js` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/headhesive.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/headhesive.min.js` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/headhesive.min.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/htmx.min.js` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/htmx.min.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/imagesloaded.js` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/imagesloaded.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/imagesloaded.pkgd.js` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/imagesloaded.pkgd.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/imagesloaded.pkgd.min.js` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/imagesloaded.pkgd.min.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/instantpage.min.js` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/instantpage.min.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/instastory.js` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/instastory.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/iscroll.js` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/iscroll.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/isotope.pkgd.js` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/isotope.pkgd.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/isotope.pkgd.min.js` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/isotope.pkgd.min.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/jquery.backstretch.js` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/jquery.backstretch.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/jquery.backstretch.min.js` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/jquery.backstretch.min.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/jquery.collagePlus.js` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/jquery.collagePlus.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/jquery.collagePlus.min.js` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/jquery.collagePlus.min.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/jquery.counterup.js` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/jquery.counterup.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/jquery.counterup.min.js` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/jquery.counterup.min.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/jquery.counterup.min.js.map` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/jquery.counterup.min.js.map`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/jquery.cubeportfolio.min.js` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/jquery.cubeportfolio.min.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/jquery.easing.js` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/jquery.easing.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/jquery.easing.min.js` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/jquery.easing.min.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/jquery.hmbrgr.js` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/jquery.hmbrgr.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/jquery.hmbrgr.min.js` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/jquery.hmbrgr.min.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/jquery.justifiedGallery.min.js` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/jquery.justifiedGallery.min.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/jquery.mousewheel.js` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/jquery.mousewheel.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/jquery.mousewheel.min.js` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/jquery.mousewheel.min.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/jquery.smartmenus.bootstrap-4.js` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/jquery.smartmenus.bootstrap-4.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/jquery.smartmenus.bootstrap-4.min.js` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/jquery.smartmenus.bootstrap-4.min.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/jquery.smartmenus.js` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/jquery.smartmenus.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/jquery.smartmenus.min.js` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/jquery.smartmenus.min.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/jquery.waypoints.js` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/jquery.waypoints.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/jquery.waypoints.min.js` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/jquery.waypoints.min.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/lazysizes.js` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/lazysizes.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/lazysizes.min.js` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/lazysizes.min.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/lg-autoplay.min.js` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/lg-autoplay.min.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/lg-thumbnail.min.js` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/lg-thumbnail.min.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/lg-zoom.min.js` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/lg-zoom.min.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/lightgallery.js` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/lightgallery.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/lightgallery.min.js` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/lightgallery.min.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/lightgallery.min.old.js` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/lightgallery.min.old.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/lightgallery.umd.js` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/lightgallery.umd.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/localforage.js` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/localforage.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/localforage.min.js` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/localforage.min.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/picturefill.js` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/picturefill.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/picturefill.min.js` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/picturefill.min.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/popper.js` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/popper.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/popper.js.map` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/popper.js.map`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/popper.min.js` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/popper.min.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/popper.min.js.map` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/popper.min.js.map`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/prettify.min.js` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/prettify.min.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/progressbar.js` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/progressbar.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/progressbar.min.js` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/progressbar.min.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/progressbar.min.js.map` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/progressbar.min.js.map`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/swiper-bundle.js` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/swiper-bundle.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/swiper-bundle.min.js` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/swiper-bundle.min.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/swiper-bundle.min.js.map` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/swiper-bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/js/plugins/typer.js` & `django-static-base-0.1.6/src/static_base/static/base/js/plugins/typer.js`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/elemis/elemis.eot` & `django-static-base-0.1.6/src/static_base/static/base/type/elemis/elemis.eot`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/elemis/elemis.svg` & `django-static-base-0.1.6/src/static_base/static/base/type/elemis/elemis.svg`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/elemis/elemis.ttf` & `django-static-base-0.1.6/src/static_base/static/base/type/elemis/elemis.ttf`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/elemis/elemis.woff` & `django-static-base-0.1.6/src/static_base/static/base/type/elemis/elemis.woff`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/elemis/elemis.woff2` & `django-static-base-0.1.6/src/static_base/static/base/type/elemis/elemis.woff2`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/font-awesome.css` & `django-static-base-0.1.6/src/static_base/static/base/type/font-awesome.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/font-montserrat.css` & `django-static-base-0.1.6/src/static_base/static/base/type/font-montserrat.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/font-muli.css` & `django-static-base-0.1.6/src/static_base/static/base/type/font-muli.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/font-slimicons.css` & `django-static-base-0.1.6/src/static_base/static/base/type/font-slimicons.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/fontawesome/fontawesome-webfont.eot` & `django-static-base-0.1.6/src/static_base/static/base/type/fontawesome/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/fontawesome/fontawesome-webfont.svg` & `django-static-base-0.1.6/src/static_base/static/base/type/fontawesome/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/fontawesome/fontawesome-webfont.ttf` & `django-static-base-0.1.6/src/static_base/static/base/type/fontawesome/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/fontawesome/fontawesome-webfont.woff` & `django-static-base-0.1.6/src/static_base/static/base/type/fontawesome/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/fontawesome/fontawesome-webfont.woff2` & `django-static-base-0.1.6/src/static_base/static/base/type/fontawesome/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/get_show/Get Show.jpg` & `django-static-base-0.1.6/src/static_base/static/base/type/get_show/Get Show.jpg`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/get_show/GetShow.otf` & `django-static-base-0.1.6/src/static_base/static/base/type/get_show/GetShow.otf`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/get_show/GetShow.ttf` & `django-static-base-0.1.6/src/static_base/static/base/type/get_show/GetShow.ttf`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/get_show/GetShow.woff` & `django-static-base-0.1.6/src/static_base/static/base/type/get_show/GetShow.woff`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/gstatic/s/muli/v20/7Au-p_0qiz-afTf2IALT8kU.woff2` & `django-static-base-0.1.6/src/static_base/static/base/type/gstatic/s/muli/v20/7Au-p_0qiz-afTf2IALT8kU.woff2`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/gstatic/s/muli/v20/7Au-p_0qiz-afTf2IQLT8kU.woff2` & `django-static-base-0.1.6/src/static_base/static/base/type/gstatic/s/muli/v20/7Au-p_0qiz-afTf2IQLT8kU.woff2`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/gstatic/s/muli/v20/7Au-p_0qiz-afTf2LwLT.woff2` & `django-static-base-0.1.6/src/static_base/static/base/type/gstatic/s/muli/v20/7Au-p_0qiz-afTf2LwLT.woff2`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/gstatic/s/muli/v20/7Auwp_0qiz-afT3GLRrX.woff2` & `django-static-base-0.1.6/src/static_base/static/base/type/gstatic/s/muli/v20/7Auwp_0qiz-afT3GLRrX.woff2`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/gstatic/s/muli/v20/7Auwp_0qiz-afTLGLQ.woff2` & `django-static-base-0.1.6/src/static_base/static/base/type/gstatic/s/muli/v20/7Auwp_0qiz-afTLGLQ.woff2`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/gstatic/s/muli/v20/7Auwp_0qiz-afTzGLRrX.woff2` & `django-static-base-0.1.6/src/static_base/static/base/type/gstatic/s/muli/v20/7Auwp_0qiz-afTzGLRrX.woff2`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/icons.css` & `django-static-base-0.1.6/src/static_base/static/base/type/icons.css`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/inclitodo/Inclitodo.otf` & `django-static-base-0.1.6/src/static_base/static/base/type/inclitodo/Inclitodo.otf`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/inclitodo/Inclitodo.ttf` & `django-static-base-0.1.6/src/static_base/static/base/type/inclitodo/Inclitodo.ttf`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/inclitodo/Inclitodo.woff` & `django-static-base-0.1.6/src/static_base/static/base/type/inclitodo/Inclitodo.woff`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/inclitodo/Inclitodo.woff2` & `django-static-base-0.1.6/src/static_base/static/base/type/inclitodo/Inclitodo.woff2`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/levorotary/Levorotary.otf` & `django-static-base-0.1.6/src/static_base/static/base/type/levorotary/Levorotary.otf`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/levorotary/Levorotary.ttf` & `django-static-base-0.1.6/src/static_base/static/base/type/levorotary/Levorotary.ttf`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/levorotary/Levorotary.woff` & `django-static-base-0.1.6/src/static_base/static/base/type/levorotary/Levorotary.woff`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/lg/lg.eot` & `django-static-base-0.1.6/src/static_base/static/base/type/lg/lg.eot`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/lg/lg.svg` & `django-static-base-0.1.6/src/static_base/static/base/type/lg/lg.svg`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/lg/lg.ttf` & `django-static-base-0.1.6/src/static_base/static/base/type/lg/lg.ttf`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/lg/lg.woff` & `django-static-base-0.1.6/src/static_base/static/base/type/lg/lg.woff`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/lg/lg.woff2` & `django-static-base-0.1.6/src/static_base/static/base/type/lg/lg.woff2`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-Bold.eot` & `django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-Bold.eot`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-Bold.ttf` & `django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-Bold.ttf`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-Bold.woff` & `django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-Bold.woff`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-Bold.woff2` & `django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-Bold.woff2`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-BoldItalic.eot` & `django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-BoldItalic.eot`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-BoldItalic.ttf` & `django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-BoldItalic.woff` & `django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-BoldItalic.woff2` & `django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-Italic.eot` & `django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-Italic.eot`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-Italic.ttf` & `django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-Italic.ttf`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-Italic.woff` & `django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-Italic.woff`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-Italic.woff2` & `django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-Italic.woff2`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-Light.eot` & `django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-Light.eot`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-Light.ttf` & `django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-Light.ttf`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-Light.woff` & `django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-Light.woff`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-Light.woff2` & `django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-Light.woff2`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-LightItalic.eot` & `django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-LightItalic.eot`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-LightItalic.ttf` & `django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-LightItalic.woff` & `django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-LightItalic.woff`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-LightItalic.woff2` & `django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-LightItalic.woff2`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-Medium.eot` & `django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-Medium.eot`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-Medium.ttf` & `django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-Medium.ttf`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-Medium.woff` & `django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-Medium.woff`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-Medium.woff2` & `django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-Medium.woff2`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-MediumItalic.eot` & `django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-MediumItalic.eot`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-MediumItalic.ttf` & `django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-MediumItalic.woff` & `django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-MediumItalic.woff`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-MediumItalic.woff2` & `django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-MediumItalic.woff2`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-Regular.eot` & `django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-Regular.eot`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-Regular.ttf` & `django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-Regular.ttf`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-Regular.woff` & `django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-Regular.woff`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-Regular.woff2` & `django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-Regular.woff2`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-SemiBold.eot` & `django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-SemiBold.eot`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-SemiBold.ttf` & `django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-SemiBold.woff` & `django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-SemiBold.woff`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-SemiBold.woff2` & `django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-SemiBold.woff2`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-SemiBoldItalic.eot` & `django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-SemiBoldItalic.eot`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-SemiBoldItalic.ttf` & `django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-SemiBoldItalic.woff` & `django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-SemiBoldItalic.woff`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/montserrat/Montserrat-SemiBoldItalic.woff2` & `django-static-base-0.1.6/src/static_base/static/base/type/montserrat/Montserrat-SemiBoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/rumpi/Rumpi.jpg` & `django-static-base-0.1.6/src/static_base/static/base/type/rumpi/Rumpi.jpg`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/rumpi/Rumpi.otf` & `django-static-base-0.1.6/src/static_base/static/base/type/rumpi/Rumpi.otf`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/rumpi/Rumpi.ttf` & `django-static-base-0.1.6/src/static_base/static/base/type/rumpi/Rumpi.ttf`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/rumpi/Rumpi.woff` & `django-static-base-0.1.6/src/static_base/static/base/type/rumpi/Rumpi.woff`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/slimicons/Slimicons.eot` & `django-static-base-0.1.6/src/static_base/static/base/type/slimicons/Slimicons.eot`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/slimicons/Slimicons.svg` & `django-static-base-0.1.6/src/static_base/static/base/type/slimicons/Slimicons.svg`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/slimicons/Slimicons.ttf` & `django-static-base-0.1.6/src/static_base/static/base/type/slimicons/Slimicons.ttf`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/slimicons/Slimicons.woff` & `django-static-base-0.1.6/src/static_base/static/base/type/slimicons/Slimicons.woff`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/src/static_base/static/base/type/slimicons/Slimicons.woff2` & `django-static-base-0.1.6/src/static_base/static/base/type/slimicons/Slimicons.woff2`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/tests/settings.py` & `django-static-base-0.1.6/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-static-base-0.1.5/tests/test_fake.py` & `django-static-base-0.1.6/tests/test_fake.py`

 * *Files identical despite different names*

