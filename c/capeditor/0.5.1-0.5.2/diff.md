# Comparing `tmp/capeditor-0.5.1.tar.gz` & `tmp/capeditor-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "capeditor-0.5.1.tar", last modified: Thu Mar 21 12:43:22 2024, max compression
+gzip compressed data, was "capeditor-0.5.2.tar", last modified: Fri Apr  5 13:32:04 2024, max compression
```

## Comparing `capeditor-0.5.1.tar` & `capeditor-0.5.2.tar`

### file list

```diff
@@ -1,132 +1,139 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:43:22.609220 capeditor-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-21 12:43:13.000000 capeditor-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11480 2024-03-21 12:43:22.609220 capeditor-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10180 2024-03-21 12:43:13.000000 capeditor-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:43:22.589220 capeditor-0.5.1/capeditor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)    27371 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/cap_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:43:22.593220 capeditor-0.5.1/capeditor/forms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/forms/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     6749 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/forms/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:43:22.585220 capeditor-0.5.1/capeditor/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:43:22.585220 capeditor-0.5.1/capeditor/locale/am/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:43:22.593220 capeditor-0.5.1/capeditor/locale/am/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    23195 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/locale/am/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    29781 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/locale/am/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:43:22.585220 capeditor-0.5.1/capeditor/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:43:22.593220 capeditor-0.5.1/capeditor/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    22416 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    29076 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:43:22.585220 capeditor-0.5.1/capeditor/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:43:22.593220 capeditor-0.5.1/capeditor/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    18681 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    25400 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:43:22.585220 capeditor-0.5.1/capeditor/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:43:22.593220 capeditor-0.5.1/capeditor/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    19764 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    26537 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:43:22.585220 capeditor-0.5.1/capeditor/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:43:22.593220 capeditor-0.5.1/capeditor/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    19747 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    26511 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:43:22.585220 capeditor-0.5.1/capeditor/locale/sw/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:43:22.593220 capeditor-0.5.1/capeditor/locale/sw/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    19084 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/locale/sw/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    25818 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/locale/sw/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:43:22.593220 capeditor-0.5.1/capeditor/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/migrations/0002_alter_capsetting_options_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/migrations/0003_capsetting_logo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/migrations/0004_predefinedalertarea.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16162 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:43:22.597220 capeditor-0.5.1/capeditor/pubsub/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/pubsub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/pubsub/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3862 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/pubsub/mqtt.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/pubsub/publish.py
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/renderers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:43:22.597220 capeditor-0.5.1/capeditor/shareable/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/shareable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14809 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/shareable/png.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:43:22.585220 capeditor-0.5.1/capeditor/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:43:22.589220 capeditor-0.5.1/capeditor/static/capeditor/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:43:22.597220 capeditor-0.5.1/capeditor/static/capeditor/css/
--rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/static/capeditor/css/cap_detail_page.css
--rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/static/capeditor/css/mapbox-gl-draw.css
--rw-r--r--   0 runner    (1001) docker     (127)    70882 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/static/capeditor/css/maplibre-gl.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:43:22.597220 capeditor-0.5.1/capeditor/static/capeditor/css/widget/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/static/capeditor/css/widget/boundary-widget.css
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/static/capeditor/css/widget/circle-widget.css
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/static/capeditor/css/widget/polygon-draw-widget.css
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/static/capeditor/css/widget/polygon-widget.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:43:22.597220 capeditor-0.5.1/capeditor/static/capeditor/fonts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:43:22.601220 capeditor-0.5.1/capeditor/static/capeditor/fonts/Roboto/
--rw-r--r--   0 runner    (1001) docker     (127)    11560 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/static/capeditor/fonts/Roboto/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)   168060 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/static/capeditor/fonts/Roboto/Roboto-Black.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   174108 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/static/capeditor/fonts/Roboto/Roboto-BlackItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   167336 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/static/capeditor/fonts/Roboto/Roboto-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   171508 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/static/capeditor/fonts/Roboto/Roboto-BoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   170504 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/static/capeditor/fonts/Roboto/Roboto-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   167000 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/static/capeditor/fonts/Roboto/Roboto-Light.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   173172 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/static/capeditor/fonts/Roboto/Roboto-LightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   168644 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/static/capeditor/fonts/Roboto/Roboto-Medium.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   173416 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/static/capeditor/fonts/Roboto/Roboto-MediumItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   168260 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/static/capeditor/fonts/Roboto/Roboto-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   168488 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/static/capeditor/fonts/Roboto/Roboto-Thin.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   172860 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/static/capeditor/fonts/Roboto/Roboto-ThinItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/static/capeditor/fonts/mapbox-gl-draw.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:43:22.605220 capeditor-0.5.1/capeditor/static/capeditor/images/
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/static/capeditor/images/alert.png
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/static/capeditor/images/alert.svg
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/static/capeditor/images/area.png
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/static/capeditor/images/certainty.png
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/static/capeditor/images/extreme.png
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/static/capeditor/images/minor.png
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/static/capeditor/images/moderate.png
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/static/capeditor/images/severe.png
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/static/capeditor/images/urgency.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:43:22.605220 capeditor-0.5.1/capeditor/static/capeditor/js/
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/static/capeditor/js/cap_accordion.js
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/static/capeditor/js/conditional_fields.js
--rw-r--r--   0 runner    (1001) docker     (127)    79103 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/static/capeditor/js/mapbox-gl-draw.js
--rw-r--r--   0 runner    (1001) docker     (127)   704176 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/static/capeditor/js/maplibre-gl.js
--rw-r--r--   0 runner    (1001) docker     (127)   604610 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/static/capeditor/js/turf.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:43:22.609220 capeditor-0.5.1/capeditor/static/capeditor/js/widget/
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/static/capeditor/js/widget/boundary-polygon-widget-telepath.js
--rw-r--r--   0 runner    (1001) docker     (127)     8373 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/static/capeditor/js/widget/boundary-polygon-widget.js
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/static/capeditor/js/widget/circle-widget-telepath.js
--rw-r--r--   0 runner    (1001) docker     (127)     8217 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/static/capeditor/js/widget/circle-widget.js
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/static/capeditor/js/widget/hazard-event-type-widget.js
--rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/static/capeditor/js/widget/polygon-draw-widget.js
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/static/capeditor/js/widget/polygon-widget-telepath.js
--rw-r--r--   0 runner    (1001) docker     (127)    10643 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/static/capeditor/js/widget/polygon-widget.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:43:22.589220 capeditor-0.5.1/capeditor/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:43:22.609220 capeditor-0.5.1/capeditor/templates/capeditor/
--rw-r--r--   0 runner    (1001) docker     (127)    16700 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/templates/capeditor/cap_alert_page.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:43:22.609220 capeditor-0.5.1/capeditor/templates/capeditor/icons/
--rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/templates/capeditor/icons/cap-alert-full.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/templates/capeditor/icons/cap-alert.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:43:22.609220 capeditor-0.5.1/capeditor/templates/capeditor/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/templates/capeditor/widgets/boundary_polygon_widget.html
--rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/templates/capeditor/widgets/circle_widget.html
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/templates/capeditor/widgets/hazard_event_type_widget.html
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/templates/capeditor/widgets/polygon_draw_widget.html
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/templates/capeditor/widgets/polygon_widget.html
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-03-21 12:43:13.000000 capeditor-0.5.1/capeditor/wagtail_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:43:22.609220 capeditor-0.5.1/capeditor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11480 2024-03-21 12:43:22.000000 capeditor-0.5.1/capeditor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4256 2024-03-21 12:43:22.000000 capeditor-0.5.1/capeditor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 12:43:22.000000 capeditor-0.5.1/capeditor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-03-21 12:43:22.000000 capeditor-0.5.1/capeditor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-21 12:43:22.000000 capeditor-0.5.1/capeditor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-21 12:43:13.000000 capeditor-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-03-21 12:43:22.613220 capeditor-0.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.596223 capeditor-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-05 13:31:56.000000 capeditor-0.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11505 2024-04-05 13:32:04.596223 capeditor-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10180 2024-04-05 13:31:56.000000 capeditor-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.572223 capeditor-0.5.2/capeditor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28279 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/cap_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11628 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/caputils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.576223 capeditor-0.5.2/capeditor/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/forms/capimporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/forms/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6749 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/forms/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.568223 capeditor-0.5.2/capeditor/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.568223 capeditor-0.5.2/capeditor/locale/am/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.576223 capeditor-0.5.2/capeditor/locale/am/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    23195 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/locale/am/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    29781 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/locale/am/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.568223 capeditor-0.5.2/capeditor/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.576223 capeditor-0.5.2/capeditor/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    22416 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    29076 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.568223 capeditor-0.5.2/capeditor/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.576223 capeditor-0.5.2/capeditor/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    18681 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    25400 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.568223 capeditor-0.5.2/capeditor/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.576223 capeditor-0.5.2/capeditor/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    19764 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    26537 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.568223 capeditor-0.5.2/capeditor/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.576223 capeditor-0.5.2/capeditor/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    19747 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    26511 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.568223 capeditor-0.5.2/capeditor/locale/sw/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.580223 capeditor-0.5.2/capeditor/locale/sw/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    19084 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/locale/sw/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    25818 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/locale/sw/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.580223 capeditor-0.5.2/capeditor/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/migrations/0002_alter_capsetting_options_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/migrations/0003_capsetting_logo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/migrations/0004_predefinedalertarea.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16150 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.580223 capeditor-0.5.2/capeditor/pubsub/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/pubsub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/pubsub/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3862 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/pubsub/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/pubsub/publish.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/renderers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.580223 capeditor-0.5.2/capeditor/shareable/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/shareable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14809 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/shareable/png.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.568223 capeditor-0.5.2/capeditor/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.568223 capeditor-0.5.2/capeditor/static/capeditor/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.580223 capeditor-0.5.2/capeditor/static/capeditor/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/css/cap_detail_page.css
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/css/import_cap_preview.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/css/mapbox-gl-draw.css
+-rw-r--r--   0 runner    (1001) docker     (127)    70882 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/css/maplibre-gl.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.580223 capeditor-0.5.2/capeditor/static/capeditor/css/widget/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/css/widget/boundary-widget.css
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/css/widget/circle-widget.css
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/css/widget/polygon-draw-widget.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/css/widget/polygon-widget.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.584223 capeditor-0.5.2/capeditor/static/capeditor/fonts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.588223 capeditor-0.5.2/capeditor/static/capeditor/fonts/Roboto/
+-rw-r--r--   0 runner    (1001) docker     (127)    11560 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/fonts/Roboto/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   168060 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/fonts/Roboto/Roboto-Black.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   174108 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/fonts/Roboto/Roboto-BlackItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   167336 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/fonts/Roboto/Roboto-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   171508 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/fonts/Roboto/Roboto-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   170504 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/fonts/Roboto/Roboto-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   167000 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/fonts/Roboto/Roboto-Light.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   173172 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/fonts/Roboto/Roboto-LightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   168644 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/fonts/Roboto/Roboto-Medium.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   173416 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/fonts/Roboto/Roboto-MediumItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   168260 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/fonts/Roboto/Roboto-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   168488 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/fonts/Roboto/Roboto-Thin.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   172860 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/fonts/Roboto/Roboto-ThinItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/fonts/mapbox-gl-draw.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.588223 capeditor-0.5.2/capeditor/static/capeditor/images/
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/images/alert.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/images/alert.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/images/area.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/images/certainty.png
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/images/extreme.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/images/minor.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/images/moderate.png
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/images/severe.png
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/images/urgency.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.592223 capeditor-0.5.2/capeditor/static/capeditor/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/js/cap_accordion.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/js/conditional_fields.js
+-rw-r--r--   0 runner    (1001) docker     (127)    79103 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/js/mapbox-gl-draw.js
+-rw-r--r--   0 runner    (1001) docker     (127)   704176 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/js/maplibre-gl.js
+-rw-r--r--   0 runner    (1001) docker     (127)   604610 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/js/turf.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.592223 capeditor-0.5.2/capeditor/static/capeditor/js/widget/
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/js/widget/boundary-polygon-widget-telepath.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8373 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/js/widget/boundary-polygon-widget.js
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/js/widget/circle-widget-telepath.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8246 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/js/widget/circle-widget.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/js/widget/hazard-event-type-widget.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5328 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/js/widget/polygon-draw-widget.js
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/js/widget/polygon-widget-telepath.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11181 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/js/widget/polygon-widget.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.568223 capeditor-0.5.2/capeditor/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.596223 capeditor-0.5.2/capeditor/templates/capeditor/
+-rw-r--r--   0 runner    (1001) docker     (127)    17275 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/templates/capeditor/cap_alert_page.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.596223 capeditor-0.5.2/capeditor/templates/capeditor/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/templates/capeditor/icons/cap-alert-full.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/templates/capeditor/icons/cap-alert.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/templates/capeditor/load_cap_alert.html
+-rw-r--r--   0 runner    (1001) docker     (127)    20436 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/templates/capeditor/preview_cap_alert.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.596223 capeditor-0.5.2/capeditor/templates/capeditor/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/templates/capeditor/widgets/boundary_polygon_widget.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/templates/capeditor/widgets/circle_widget.html
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/templates/capeditor/widgets/hazard_event_type_widget.html
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/templates/capeditor/widgets/polygon_draw_widget.html
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/templates/capeditor/widgets/polygon_widget.html
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/wagtail_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.596223 capeditor-0.5.2/capeditor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11505 2024-04-05 13:32:04.000000 capeditor-0.5.2/capeditor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-04-05 13:32:04.000000 capeditor-0.5.2/capeditor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 13:32:04.000000 capeditor-0.5.2/capeditor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-05 13:32:04.000000 capeditor-0.5.2/capeditor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-05 13:32:04.000000 capeditor-0.5.2/capeditor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-05 13:31:56.000000 capeditor-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-05 13:32:04.596223 capeditor-0.5.2/setup.cfg
```

### Comparing `capeditor-0.5.1/PKG-INFO` & `capeditor-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capeditor
-Version: 0.5.1
+Version: 0.5.2
 Summary: Wagtail based CAP composer
 Home-page: https://github.com/wmo-raf/cap-composer
 Author: Grace Amondi, Erick Otenyo
 Author-email: miswa.grace@gmail.com, otenyo.erick@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
@@ -27,14 +27,15 @@
 Requires-Dist: wagtail-humanitarian-icons>=2.0.0
 Requires-Dist: wagtail-modelchooser>=4.0.1
 Requires-Dist: paho-mqtt
 Requires-Dist: cairosvg
 Requires-Dist: geopandas
 Requires-Dist: matplotlib
 Requires-Dist: cartopy
+Requires-Dist: xmltodict
 
 # CAP Composer  <img style="float: right;" height="40" src="images/caplogo.jpeg" markdown="1">
 
 [![Upload Python Package](https://github.com/wmo-raf/cap-composer/actions/workflows/publish.yml/badge.svg)](https://github.com/wmo-raf/cap-composer/actions/workflows/publish.yml)
 
 A [Wagtail](https://wagtail.io/) based Common Alerting Protocol (CAP) Warning Composer. This is a web-based tool for
 creating and managing CAP alerts. It is designed to be used by meteorological and hydrological services, disaster
```

### Comparing `capeditor-0.5.1/README.md` & `capeditor-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/blocks.py` & `capeditor-0.5.2/capeditor/blocks.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from shapely.geometry import shape
 from wagtail import blocks
 from wagtail.blocks import FieldBlock, StructValue
 from wagtail.documents.blocks import DocumentChooserBlock
 from wagtail.models import Site
 from wagtailmodelchooser.blocks import ModelChooserBlock
 
-from .forms.fields import PolygonField, MultiPolygonField, BoundaryMultiPolygonField
+from .forms.fields import PolygonField, MultiPolygonField, BoundaryMultiPolygonField, PolygonOrMultiPolygonField
 from .forms.widgets import CircleWidget
 from .utils import file_path_mime
 
 
 class BoundaryFieldBlock(FieldBlock):
     def __init__(self, required=True, help_text=None, srid=4326, **kwargs):
         self.field_options = {
@@ -54,14 +54,34 @@
 
     def value_from_form(self, value):
         if isinstance(value, GEOSGeometry):
             value = value.json
         return value
 
 
+class PolygonOrMultiPolygonFieldBlock(FieldBlock):
+    def __init__(self, required=True, help_text=None, srid=4326, **kwargs):
+        self.field_options = {
+            "required": required,
+            "help_text": help_text,
+            "srid": srid
+        }
+
+        super().__init__(**kwargs)
+
+    @cached_property
+    def field(self):
+        return PolygonOrMultiPolygonField(**self.field_options)
+
+    def value_from_form(self, value):
+        if isinstance(value, GEOSGeometry):
+            value = value.json
+        return value
+
+
 class PolygonFieldBlock(FieldBlock):
     def __init__(self, required=True, help_text=None, srid=4326, **kwargs):
         self.field_options = {
             "required": required,
             "help_text": help_text,
             "srid": srid
         }
@@ -170,19 +190,14 @@
         return area_data
 
     @cached_property
     def geojson(self):
         polygon = self.get("boundary")
         return json.loads(polygon)
 
-    # @cached_property
-    # def aread_desc(self):
-    #     area_desc = self.get("areaDesc")
-    #     return json.loads(polygon)
-
 
 class AlertAreaBoundaryBlock(blocks.StructBlock):
     class Meta:
         value_class = AlertAreaBoundaryStructValue
 
     ADMIN_LEVEL_CHOICES = (
         (0, _("Level 0")),
@@ -205,23 +220,33 @@
                                help_text=_("The maximum altitude of the affected area of the alert message."
                                            "MUST NOT be used except in combination with the altitude element. "))
 
 
 class AlertAreaPolygonStructValue(StructValue):
     @cached_property
     def area(self):
-        polygon_geojson_str = self.get("polygon")
-        polygon_geojson_dict = json.loads(polygon_geojson_str)
+        geom_geojson_str = self.get("polygon")
+        geom_geojson_dict = json.loads(geom_geojson_str)
+        geom_shape = shape(geom_geojson_dict)
+
+        polygons = []
+
+        if isinstance(geom_shape, Polygon):
+            polygons.append(geom_shape)
+        else:
+            polygons = list(geom_shape.geoms)
 
-        polygon = shape(polygon_geojson_dict)
-        coords = " ".join(["{},{}".format(y, x) for x, y in list(polygon.exterior.coords)])
+        polygons_data = []
+        for polygon in polygons:
+            coords = " ".join(["{},{}".format(y, x) for x, y in list(polygon.exterior.reverse().coords)])
+            polygons_data.append(coords)
 
         area_data = {
             "areaDesc": self.get("areaDesc"),
-            "polygon": coords,
+            "polygons": polygons_data
         }
 
         if self.get("altitude"):
             area_data.update({"altitude": self.get("altitude")})
             if self.get("ceiling"):
                 area_data.update({"ceiling": self.get("ceiling")})
 
@@ -235,17 +260,18 @@
 
 class AlertAreaPolygonBlock(blocks.StructBlock):
     class Meta:
         value_class = AlertAreaPolygonStructValue
 
     areaDesc = blocks.TextBlock(label=_("Affected areas / Regions"),
                                 help_text=_("The text describing the affected area of the alert message"))
-    polygon = PolygonFieldBlock(label=_("Polygon"),
-                                help_text=_("The paired values of points defining a polygon that delineates "
-                                            "the affected area of the alert message"))
+    polygon = PolygonOrMultiPolygonFieldBlock(label=_("Polygon"),
+                                              help_text=_(
+                                                  "The paired values of points defining a polygon that delineates "
+                                                  "the affected area of the alert message"))
     altitude = blocks.CharBlock(max_length=100, required=False, label=_("Altitude"),
                                 help_text=_("The specific or minimum altitude of the affected "
                                             "area of the alert message"))
     ceiling = blocks.CharBlock(max_length=100, required=False, label=_("Ceiling"),
                                help_text=_("The maximum altitude of the affected area of the alert message."
                                            "MUST NOT be used except in combination with the altitude element. "))
 
@@ -572,15 +598,15 @@
         ('Security', _("Law enforcement, military, homeland and local/private security")),
         ('Rescue', _("Rescue and recovery")),
         ('Fire', _("Fire suppression and rescue")),
         ('Health', _("Medical and public health")),
         ('Env', _("Pollution and other environmental")),
         ('Transport', _("Public and private transportation")),
         ('Infra', _("Utility, telecommunication, other non-transport infrastructure")),
-        ('Cbrne', _("Chemical, Biological, Radiological, Nuclear or High-Yield Explosive threat or attack")),
+        ('CBRNE', _("Chemical, Biological, Radiological, Nuclear or High-Yield Explosive threat or attack")),
         ('Other', _("Other events")),
     )
 
     URGENCY_CHOICES = (
         ('Immediate', _("Immediate - Responsive action SHOULD be taken immediately")),
         ('Expected', _("Expected - Responsive action SHOULD be taken soon (within next hour)")),
         ('Future', _("Future - Responsive action SHOULD be taken in the near future")),
@@ -603,17 +629,18 @@
         ('Unlikely', _("Unlikely - Not expected to occur (percentage ~ 0)")),
         ('Unknown', _("Unknown - Certainty unknown")),
     )
     event = blocks.ChoiceBlock(choices=get_hazard_types, label=_("Event"),
                                help_text=_("The text denoting the type of the subject event of the alert message. You "
                                            "can define hazards events monitored by your institution from CAP settings"))
 
-    category = blocks.ChoiceBlock(choices=CATEGORY_CHOICES, default="Met", label=_("Category"),
-                                  help_text=_("The code denoting the category of the subject"
-                                              " event of the alert message"))
+    category = blocks.MultipleChoiceBlock(choices=CATEGORY_CHOICES, default="Met", label=_("Category"),
+                                          help_text=_("The code denoting the category of the subject"
+                                                      " event of the alert message"),
+                                          widget=forms.CheckboxSelectMultiple)
     language = blocks.ChoiceBlock(choices=LANGUAGE_CHOICES, default="en", required=False, label=_("Language"),
                                   help_text=_("The code denoting the language of the alert message"), )
 
     urgency = blocks.ChoiceBlock(choices=URGENCY_CHOICES, label=_("Urgency"),
                                  help_text=_("The code denoting the urgency of the subject "
                                              "event of the alert message"))
     severity = blocks.ChoiceBlock(choices=SEVERITY_CHOICES, label=_("Severity"),
```

### Comparing `capeditor-0.5.1/capeditor/cap_settings.py` & `capeditor-0.5.2/capeditor/cap_settings.py`

 * *Files 15% similar despite different names*

```diff
@@ -57,14 +57,32 @@
         ], heading=_("Audience Types")),
         ObjectList([
             InlinePanel("predefined_alert_areas", heading=_("Predefined Alert Areas"), label=_("Area"),
                         help_text=_("Predefined areas for alerts")),
         ], heading=_("Predefined Areas"), classname="map-resize-trigger"),
     ])
 
+    @property
+    def contact_list(self):
+        contacts = []
+        for contact_block in self.contacts:
+            contact = contact_block.value.get("contact")
+            if contact:
+                contacts.append(contact)
+        return contacts
+
+    @property
+    def audience_list(self):
+        audiences = []
+        for audience_block in self.audience_types:
+            audience = audience_block.value.get("audience")
+            if audience:
+                audiences.append(audience)
+        return audiences
+
 
 class HazardEventTypes(Orderable):
     setting = ParentalKey(CapSetting, on_delete=models.PROTECT, related_name="hazard_event_types")
     is_in_wmo_event_types_list = models.BooleanField(default=True,
                                                      verbose_name=_("Select from WMO list of Hazards Event Types"))
     event = models.CharField(max_length=255, unique=True, verbose_name=_("Hazard"), help_text=_("Name of Hazard"))
     icon = models.CharField(max_length=255, null=True, blank=True, verbose_name=_("Icon"), help_text=_("Matching icon"))
@@ -115,7 +133,19 @@
 
 
 def get_default_sender():
     cap_setting = get_cap_setting()
     if cap_setting and cap_setting.sender:
         return cap_setting.sender
     return None
+
+
+def get_cap_contact_list(request):
+    cap_settings = CapSetting.for_request(request)
+    contacts_list = cap_settings.contact_list
+    return contacts_list
+
+
+def get_cap_audience_list(request):
+    cap_settings = CapSetting.for_request(request)
+    audience_list = cap_settings.audience_list
+    return audience_list
```

### Comparing `capeditor-0.5.1/capeditor/constants.py` & `capeditor-0.5.2/capeditor/constants.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/forms/widgets.py` & `capeditor-0.5.2/capeditor/forms/widgets.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/locale/am/LC_MESSAGES/django.mo` & `capeditor-0.5.2/capeditor/locale/am/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/locale/am/LC_MESSAGES/django.po` & `capeditor-0.5.2/capeditor/locale/am/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/locale/ar/LC_MESSAGES/django.mo` & `capeditor-0.5.2/capeditor/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/locale/ar/LC_MESSAGES/django.po` & `capeditor-0.5.2/capeditor/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/locale/en/LC_MESSAGES/django.mo` & `capeditor-0.5.2/capeditor/locale/en/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/locale/en/LC_MESSAGES/django.po` & `capeditor-0.5.2/capeditor/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/locale/es/LC_MESSAGES/django.mo` & `capeditor-0.5.2/capeditor/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/locale/es/LC_MESSAGES/django.po` & `capeditor-0.5.2/capeditor/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/locale/fr/LC_MESSAGES/django.mo` & `capeditor-0.5.2/capeditor/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/locale/fr/LC_MESSAGES/django.po` & `capeditor-0.5.2/capeditor/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/locale/sw/LC_MESSAGES/django.mo` & `capeditor-0.5.2/capeditor/locale/sw/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/locale/sw/LC_MESSAGES/django.po` & `capeditor-0.5.2/capeditor/locale/sw/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/migrations/0001_initial.py` & `capeditor-0.5.2/capeditor/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/migrations/0002_alter_capsetting_options_and_more.py` & `capeditor-0.5.2/capeditor/migrations/0002_alter_capsetting_options_and_more.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/migrations/0003_capsetting_logo.py` & `capeditor-0.5.2/capeditor/migrations/0003_capsetting_logo.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/migrations/0004_predefinedalertarea.py` & `capeditor-0.5.2/capeditor/migrations/0004_predefinedalertarea.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/models.py` & `capeditor-0.5.2/capeditor/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import json
 import os
 import uuid
 
 from adminboundarymanager.models import AdminBoundarySettings
 from django.conf import settings
 from django.utils import timezone
 from django.utils.functional import cached_property
```

### Comparing `capeditor-0.5.1/capeditor/pubsub/base.py` & `capeditor-0.5.2/capeditor/pubsub/base.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/pubsub/mqtt.py` & `capeditor-0.5.2/capeditor/pubsub/mqtt.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/pubsub/publish.py` & `capeditor-0.5.2/capeditor/pubsub/publish.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/renderers.py` & `capeditor-0.5.2/capeditor/renderers.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/serializers.py` & `capeditor-0.5.2/capeditor/serializers.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/shareable/png.py` & `capeditor-0.5.2/capeditor/shareable/png.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/static/capeditor/css/cap_detail_page.css` & `capeditor-0.5.2/capeditor/static/capeditor/css/cap_detail_page.css`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/static/capeditor/css/mapbox-gl-draw.css` & `capeditor-0.5.2/capeditor/static/capeditor/css/mapbox-gl-draw.css`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/static/capeditor/css/maplibre-gl.css` & `capeditor-0.5.2/capeditor/static/capeditor/css/maplibre-gl.css`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/static/capeditor/css/widget/circle-widget.css` & `capeditor-0.5.2/capeditor/static/capeditor/css/widget/circle-widget.css`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/static/capeditor/css/widget/polygon-widget.css` & `capeditor-0.5.2/capeditor/static/capeditor/css/widget/polygon-widget.css`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/static/capeditor/fonts/Roboto/LICENSE.txt` & `capeditor-0.5.2/capeditor/static/capeditor/fonts/Roboto/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/static/capeditor/fonts/Roboto/Roboto-Black.ttf` & `capeditor-0.5.2/capeditor/static/capeditor/fonts/Roboto/Roboto-Black.ttf`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/static/capeditor/fonts/Roboto/Roboto-BlackItalic.ttf` & `capeditor-0.5.2/capeditor/static/capeditor/fonts/Roboto/Roboto-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/static/capeditor/fonts/Roboto/Roboto-Bold.ttf` & `capeditor-0.5.2/capeditor/static/capeditor/fonts/Roboto/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/static/capeditor/fonts/Roboto/Roboto-BoldItalic.ttf` & `capeditor-0.5.2/capeditor/static/capeditor/fonts/Roboto/Roboto-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/static/capeditor/fonts/Roboto/Roboto-Italic.ttf` & `capeditor-0.5.2/capeditor/static/capeditor/fonts/Roboto/Roboto-Italic.ttf`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/static/capeditor/fonts/Roboto/Roboto-Light.ttf` & `capeditor-0.5.2/capeditor/static/capeditor/fonts/Roboto/Roboto-Light.ttf`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/static/capeditor/fonts/Roboto/Roboto-LightItalic.ttf` & `capeditor-0.5.2/capeditor/static/capeditor/fonts/Roboto/Roboto-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/static/capeditor/fonts/Roboto/Roboto-Medium.ttf` & `capeditor-0.5.2/capeditor/static/capeditor/fonts/Roboto/Roboto-Medium.ttf`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/static/capeditor/fonts/Roboto/Roboto-MediumItalic.ttf` & `capeditor-0.5.2/capeditor/static/capeditor/fonts/Roboto/Roboto-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/static/capeditor/fonts/Roboto/Roboto-Regular.ttf` & `capeditor-0.5.2/capeditor/static/capeditor/fonts/Roboto/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/static/capeditor/fonts/Roboto/Roboto-Thin.ttf` & `capeditor-0.5.2/capeditor/static/capeditor/fonts/Roboto/Roboto-Thin.ttf`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/static/capeditor/fonts/Roboto/Roboto-ThinItalic.ttf` & `capeditor-0.5.2/capeditor/static/capeditor/fonts/Roboto/Roboto-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/static/capeditor/fonts/mapbox-gl-draw.css` & `capeditor-0.5.2/capeditor/static/capeditor/fonts/mapbox-gl-draw.css`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/static/capeditor/images/alert.png` & `capeditor-0.5.2/capeditor/static/capeditor/images/alert.png`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/static/capeditor/images/alert.svg` & `capeditor-0.5.2/capeditor/static/capeditor/images/alert.svg`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/static/capeditor/images/area.png` & `capeditor-0.5.2/capeditor/static/capeditor/images/area.png`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/static/capeditor/images/certainty.png` & `capeditor-0.5.2/capeditor/static/capeditor/images/certainty.png`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/static/capeditor/images/extreme.png` & `capeditor-0.5.2/capeditor/static/capeditor/images/extreme.png`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/static/capeditor/images/minor.png` & `capeditor-0.5.2/capeditor/static/capeditor/images/minor.png`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/static/capeditor/images/moderate.png` & `capeditor-0.5.2/capeditor/static/capeditor/images/moderate.png`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/static/capeditor/images/severe.png` & `capeditor-0.5.2/capeditor/static/capeditor/images/severe.png`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/static/capeditor/js/cap_accordion.js` & `capeditor-0.5.2/capeditor/static/capeditor/js/cap_accordion.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/static/capeditor/js/conditional_fields.js` & `capeditor-0.5.2/capeditor/static/capeditor/js/conditional_fields.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/static/capeditor/js/mapbox-gl-draw.js` & `capeditor-0.5.2/capeditor/static/capeditor/js/mapbox-gl-draw.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/static/capeditor/js/maplibre-gl.js` & `capeditor-0.5.2/capeditor/static/capeditor/js/maplibre-gl.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/static/capeditor/js/turf.min.js` & `capeditor-0.5.2/capeditor/static/capeditor/js/turf.min.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/static/capeditor/js/widget/boundary-polygon-widget-telepath.js` & `capeditor-0.5.2/capeditor/static/capeditor/js/widget/boundary-polygon-widget-telepath.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/static/capeditor/js/widget/boundary-polygon-widget.js` & `capeditor-0.5.2/capeditor/static/capeditor/js/widget/boundary-polygon-widget.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/static/capeditor/js/widget/circle-widget-telepath.js` & `capeditor-0.5.2/capeditor/static/capeditor/js/widget/circle-widget-telepath.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/static/capeditor/js/widget/circle-widget.js` & `capeditor-0.5.2/capeditor/static/capeditor/js/widget/circle-widget.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -297,14 +297,16 @@
         this.setState("")
     }
 }
 
 CircleWidget.prototype.initFromState = function() {
     const circeValue = this.getState()
 
+    console.log(circeValue)
+
     if (circeValue) {
         const {
             lon,
             lat,
             radius
         } = this.parseCircleValue(circeValue) || {}
```

### Comparing `capeditor-0.5.1/capeditor/static/capeditor/js/widget/hazard-event-type-widget.js` & `capeditor-0.5.2/capeditor/static/capeditor/js/widget/hazard-event-type-widget.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/static/capeditor/js/widget/polygon-draw-widget.js` & `capeditor-0.5.2/capeditor/static/capeditor/js/widget/polygon-draw-widget.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -179,18 +179,14 @@
         if (featureCollection && featureCollection.features && !!featureCollection.features.length) {
             combinedFeatures = turf.combine(featureCollection)
         }
 
         if (combinedFeatures) {
             const feature = combinedFeatures.features[0]
 
-            if (feature.properties) {
-                delete feature.properties
-            }
-
             this.setValue(JSON.stringify(feature.geometry))
 
         } else {
             this.setValue("")
         }
     }
 }
```

### Comparing `capeditor-0.5.1/capeditor/static/capeditor/js/widget/polygon-widget-telepath.js` & `capeditor-0.5.2/capeditor/static/capeditor/js/widget/polygon-widget-telepath.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/static/capeditor/js/widget/polygon-widget.js` & `capeditor-0.5.2/capeditor/static/capeditor/js/widget/polygon-widget.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -264,20 +264,26 @@
 
     const $geomEditAction = $(".mapboxgl-draw-actions-btn")
 
     $geomEditAction.on("click", (e) => {
         e.preventDefault()
         const isSaveButton = e.target.classList.contains("mapboxgl-draw-actions-btn_save")
         if (isSaveButton) {
-            const FC = this.draw.getAll();
-            const feat = FC.features[0]
 
-            if (feat) {
-                const feature = feat.geometry
-                this.setDrawData(feature)
+            let combinedFeatures
+
+            const featureCollection = this.draw.getAll()
+            if (featureCollection && featureCollection.features && !!featureCollection.features.length) {
+                combinedFeatures = turf.combine(featureCollection)
+            }
+
+            if (combinedFeatures) {
+                const feature = combinedFeatures.features[0]
+
+                this.setDrawData(feature.geometry)
             } else {
                 this.setDrawData(null)
             }
 
         } else {
             this.map.setLayoutProperty("polygon", "visibility", "visible")
 
@@ -286,17 +292,26 @@
             this.draw.deleteAll();
 
             this.initDraw()
         }
     })
 
     this.map.on("draw.create", (e) => {
-        const feat = e.features[0]
-        const feature = feat.geometry
-        this.setDrawData(feature)
+        let combinedFeatures
+
+        const featureCollection = this.draw.getAll()
+        if (featureCollection && featureCollection.features && !!featureCollection.features.length) {
+            combinedFeatures = turf.combine(featureCollection)
+        }
+
+        if (combinedFeatures) {
+            const feature = combinedFeatures.features[0]
+
+            this.setDrawData(feature.geometry)
+        }
     });
 }
 
 
 PolygonWidget.prototype.clearDraw = function() {
     if (this.draw) {
         this.map.removeControl(this.draw)
@@ -311,29 +326,30 @@
     if (this.saveCancelControl) {
         this.map.removeControl(this.saveCancelControl)
         this.saveCancelControl = null
     }
 }
 
 
-PolygonWidget.prototype.setDrawData = function(feature) {
-    if (feature) {
-        const bbox = turf.bbox(feature)
+PolygonWidget.prototype.setDrawData = function(geometry) {
+    if (geometry) {
+        const bbox = turf.bbox(geometry)
         const bounds = [
             [bbox[0], bbox[1]],
             [bbox[2], bbox[3]]
         ]
 
-        this.setSourceData(feature)
+        this.setSourceData(geometry)
         this.map.setLayoutProperty("polygon", "visibility", "visible")
 
         this.map.fitBounds(bounds, {
             padding: 50
         })
-        const geomString = JSON.stringify(feature)
+        const geomString = JSON.stringify(geometry)
+
 
         this.setState(geomString)
     } else {
         this.setSourceData(null)
         this.setState("")
     }
```

### Comparing `capeditor-0.5.1/capeditor/templates/capeditor/cap_alert_page.html` & `capeditor-0.5.2/capeditor/templates/capeditor/cap_alert_page.html`

 * *Files 6% similar despite different names*

```diff
@@ -310,19 +310,32 @@
 
             // add layer
             map.addLayer({
                 'id': 'polygon',
                 'type': 'fill',
                 'source': 'polygon',
                 'layout': {},
-                'paint': {
-                    'fill-color': "red",
-                    'fill-opacity': 0.8,
+                paint: {
+                    "fill-color": [
+                        "case",
+                        ["==", ["get", "severity"], "Extreme"],
+                        "#d72f2a",
+                        ["==", ["get", "severity"], "Severe"],
+                        "#f89904",
+                        ["==", ["get", "severity"], "Moderate"],
+                        "#e4e616",
+                        ["==", ["get", "severity"], "Minor"],
+                        "#53ffff",
+                        ["==", ["get", "severity"], "Unknown"],
+                        "#3366ff",
+                        "black",
+                    ],
+                    "fill-opacity": 0.7,
                     "fill-outline-color": "#000",
-                }
+                },
             });
 
             // fit to bounds
             if (bounds) {
                 const bbox = [[bounds[0], bounds[1]], [bounds[2], bounds[3]]]
                 map.fitBounds(bbox, {padding: 20})
             }
```

### Comparing `capeditor-0.5.1/capeditor/templates/capeditor/icons/cap-alert-full.svg` & `capeditor-0.5.2/capeditor/templates/capeditor/icons/cap-alert-full.svg`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/templates/capeditor/icons/cap-alert.svg` & `capeditor-0.5.2/capeditor/templates/capeditor/icons/cap-alert.svg`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/templates/capeditor/widgets/circle_widget.html` & `capeditor-0.5.2/capeditor/templates/capeditor/widgets/circle_widget.html`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/templates/capeditor/widgets/hazard_event_type_widget.html` & `capeditor-0.5.2/capeditor/templates/capeditor/widgets/hazard_event_type_widget.html`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/templates/capeditor/widgets/polygon_draw_widget.html` & `capeditor-0.5.2/capeditor/templates/capeditor/widgets/polygon_draw_widget.html`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/utils.py` & `capeditor-0.5.2/capeditor/utils.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.1/capeditor/wagtail_hooks.py` & `capeditor-0.5.2/capeditor/wagtail_hooks.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 from django.shortcuts import redirect
 from django.template.response import TemplateResponse
 from django.templatetags.static import static
+from django.urls import path
 from django.utils.html import format_html
 from django.utils.translation import gettext as _
 from wagtail import hooks
 from wagtail.actions.copy_page import CopyPageAction
 from wagtail.admin import messages
 from wagtail.admin.forms.pages import CopyForm
 from wagtail.admin.utils import get_valid_next_url_from_request
 from wagtail.models import Page
 
+from capeditor.views import load_cap_alert, import_cap_alert
+
 
 @hooks.register("insert_editor_js")
 def insert_editor_js():
     return format_html(
         '<script src="{}"></script>', static("capeditor/js/conditional_fields.js"),
     )
 
@@ -22,14 +25,22 @@
 def register_icons(icons):
     return icons + [
         'capeditor/icons/cap-alert.svg',
         'capeditor/icons/cap-alert-full.svg',
     ]
 
 
+@hooks.register('register_admin_urls')
+def urlconf_stations():
+    return [
+        path('import-cap/', load_cap_alert, name='load_cap_alert'),
+        path('import-cap/import/', import_cap_alert, name='import_cap_alert'),
+    ]
+
+
 # @hooks.register("before_copy_page")
 def copy_cap_alert_page(request, page):
     if page.specific.__class__.__name__ == "CapAlertPage":
 
         # Parent page defaults to parent of source page
         parent_page = page.get_parent()
```

### Comparing `capeditor-0.5.1/capeditor.egg-info/PKG-INFO` & `capeditor-0.5.2/capeditor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capeditor
-Version: 0.5.1
+Version: 0.5.2
 Summary: Wagtail based CAP composer
 Home-page: https://github.com/wmo-raf/cap-composer
 Author: Grace Amondi, Erick Otenyo
 Author-email: miswa.grace@gmail.com, otenyo.erick@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
@@ -27,14 +27,15 @@
 Requires-Dist: wagtail-humanitarian-icons>=2.0.0
 Requires-Dist: wagtail-modelchooser>=4.0.1
 Requires-Dist: paho-mqtt
 Requires-Dist: cairosvg
 Requires-Dist: geopandas
 Requires-Dist: matplotlib
 Requires-Dist: cartopy
+Requires-Dist: xmltodict
 
 # CAP Composer  <img style="float: right;" height="40" src="images/caplogo.jpeg" markdown="1">
 
 [![Upload Python Package](https://github.com/wmo-raf/cap-composer/actions/workflows/publish.yml/badge.svg)](https://github.com/wmo-raf/cap-composer/actions/workflows/publish.yml)
 
 A [Wagtail](https://wagtail.io/) based Common Alerting Protocol (CAP) Warning Composer. This is a web-based tool for
 creating and managing CAP alerts. It is designed to be used by meteorological and hydrological services, disaster
```

### Comparing `capeditor-0.5.1/capeditor.egg-info/SOURCES.txt` & `capeditor-0.5.2/capeditor.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -3,27 +3,31 @@
 pyproject.toml
 setup.cfg
 capeditor/__init__.py
 capeditor/admin.py
 capeditor/apps.py
 capeditor/blocks.py
 capeditor/cap_settings.py
+capeditor/caputils.py
 capeditor/constants.py
+capeditor/errors.py
 capeditor/models.py
 capeditor/renderers.py
 capeditor/serializers.py
 capeditor/tests.py
 capeditor/utils.py
+capeditor/views.py
 capeditor/wagtail_hooks.py
 capeditor.egg-info/PKG-INFO
 capeditor.egg-info/SOURCES.txt
 capeditor.egg-info/dependency_links.txt
 capeditor.egg-info/requires.txt
 capeditor.egg-info/top_level.txt
 capeditor/forms/__init__.py
+capeditor/forms/capimporter.py
 capeditor/forms/fields.py
 capeditor/forms/widgets.py
 capeditor/locale/am/LC_MESSAGES/django.mo
 capeditor/locale/am/LC_MESSAGES/django.po
 capeditor/locale/ar/LC_MESSAGES/django.mo
 capeditor/locale/ar/LC_MESSAGES/django.po
 capeditor/locale/en/LC_MESSAGES/django.mo
@@ -42,14 +46,15 @@
 capeditor/pubsub/__init__.py
 capeditor/pubsub/base.py
 capeditor/pubsub/mqtt.py
 capeditor/pubsub/publish.py
 capeditor/shareable/__init__.py
 capeditor/shareable/png.py
 capeditor/static/capeditor/css/cap_detail_page.css
+capeditor/static/capeditor/css/import_cap_preview.css
 capeditor/static/capeditor/css/mapbox-gl-draw.css
 capeditor/static/capeditor/css/maplibre-gl.css
 capeditor/static/capeditor/css/widget/boundary-widget.css
 capeditor/static/capeditor/css/widget/circle-widget.css
 capeditor/static/capeditor/css/widget/polygon-draw-widget.css
 capeditor/static/capeditor/css/widget/polygon-widget.css
 capeditor/static/capeditor/fonts/mapbox-gl-draw.css
@@ -85,14 +90,16 @@
 capeditor/static/capeditor/js/widget/circle-widget-telepath.js
 capeditor/static/capeditor/js/widget/circle-widget.js
 capeditor/static/capeditor/js/widget/hazard-event-type-widget.js
 capeditor/static/capeditor/js/widget/polygon-draw-widget.js
 capeditor/static/capeditor/js/widget/polygon-widget-telepath.js
 capeditor/static/capeditor/js/widget/polygon-widget.js
 capeditor/templates/capeditor/cap_alert_page.html
+capeditor/templates/capeditor/load_cap_alert.html
+capeditor/templates/capeditor/preview_cap_alert.html
 capeditor/templates/capeditor/icons/cap-alert-full.svg
 capeditor/templates/capeditor/icons/cap-alert.svg
 capeditor/templates/capeditor/widgets/boundary_polygon_widget.html
 capeditor/templates/capeditor/widgets/circle_widget.html
 capeditor/templates/capeditor/widgets/hazard_event_type_widget.html
 capeditor/templates/capeditor/widgets/polygon_draw_widget.html
 capeditor/templates/capeditor/widgets/polygon_widget.html
```

### Comparing `capeditor-0.5.1/setup.cfg` & `capeditor-0.5.2/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = capeditor
-version = 0.5.1
+version = 0.5.2
 description = Wagtail based CAP composer
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/wmo-raf/cap-composer
 author = Grace Amondi, Erick Otenyo
 author_email = miswa.grace@gmail.com, otenyo.erick@gmail.com
 license = MIT
@@ -34,12 +34,13 @@
 	wagtail-humanitarian-icons>=2.0.0
 	wagtail-modelchooser>=4.0.1
 	paho-mqtt
 	cairosvg
 	geopandas
 	matplotlib
 	cartopy
+	xmltodict
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

