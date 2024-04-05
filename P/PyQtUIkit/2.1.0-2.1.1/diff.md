# Comparing `tmp/PyQtUIkit-2.1.0.tar.gz` & `tmp/PyQtUIkit-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyQtUIkit-2.1.0.tar", last modified: Thu Apr  4 19:10:24 2024, max compression
+gzip compressed data, was "PyQtUIkit-2.1.1.tar", last modified: Thu Apr  4 20:50:29 2024, max compression
```

## Comparing `PyQtUIkit-2.1.0.tar` & `PyQtUIkit-2.1.1.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 19:10:24.468640 PyQtUIkit-2.1.0/
--rw-rw-rw-   0        0        0     1090 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/LICENSE
--rw-rw-rw-   0        0        0     2938 2024-04-04 19:10:24.468640 PyQtUIkit-2.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-04 19:10:24.421768 PyQtUIkit-2.1.0/PyQtUIkit/
--rw-rw-rw-   0        0        0       49 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/__init__.py
--rw-rw-rw-   0        0        0     3835 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/_icons.py
-drwxrwxrwx   0        0        0        0 2024-04-04 19:10:24.437391 PyQtUIkit-2.1.0/PyQtUIkit/builder/
--rw-rw-rw-   0        0        0     1116 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/builder/__init__.py
--rw-rw-rw-   0        0        0     1825 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/builder/builder_class.py
--rw-rw-rw-   0        0        0     1383 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/builder/builder_module.py
-drwxrwxrwx   0        0        0        0 2024-04-04 19:10:24.437391 PyQtUIkit-2.1.0/PyQtUIkit/core/
--rw-rw-rw-   0        0        0       84 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/core/__init__.py
--rw-rw-rw-   0        0        0       19 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/core/_version.py
--rw-rw-rw-   0        0        0     1503 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/core/font.py
--rw-rw-rw-   0        0        0     1019 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/core/icon.py
--rw-rw-rw-   0        0        0     4655 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/core/properties.py
-drwxrwxrwx   0        0        0        0 2024-04-04 19:10:24.453012 PyQtUIkit-2.1.0/PyQtUIkit/fonts/
--rw-rw-rw-   0        0        0   168060 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/fonts/Roboto-Black.ttf
--rw-rw-rw-   0        0        0   174108 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/fonts/Roboto-BlackItalic.ttf
--rw-rw-rw-   0        0        0   167336 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/fonts/Roboto-Bold.ttf
--rw-rw-rw-   0        0        0   171508 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/fonts/Roboto-BoldItalic.ttf
--rw-rw-rw-   0        0        0   170504 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/fonts/Roboto-Italic.ttf
--rw-rw-rw-   0        0        0   167000 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/fonts/Roboto-Light.ttf
--rw-rw-rw-   0        0        0   173172 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/fonts/Roboto-LightItalic.ttf
--rw-rw-rw-   0        0        0   168644 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/fonts/Roboto-Medium.ttf
--rw-rw-rw-   0        0        0   173416 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/fonts/Roboto-MediumItalic.ttf
--rw-rw-rw-   0        0        0   168260 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/fonts/Roboto-Regular.ttf
--rw-rw-rw-   0        0        0   168488 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/fonts/Roboto-Thin.ttf
--rw-rw-rw-   0        0        0   172860 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/fonts/Roboto-ThinItalic.ttf
--rw-rw-rw-   0        0        0    87392 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/fonts/RobotoMono-Bold.ttf
--rw-rw-rw-   0        0        0    94636 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf
--rw-rw-rw-   0        0        0    88248 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf
--rw-rw-rw-   0        0        0    94016 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf
--rw-rw-rw-   0        0        0    94372 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/fonts/RobotoMono-Italic.ttf
--rw-rw-rw-   0        0        0    87980 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/fonts/RobotoMono-Light.ttf
--rw-rw-rw-   0        0        0    94256 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf
--rw-rw-rw-   0        0        0    87172 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/fonts/RobotoMono-Medium.ttf
--rw-rw-rw-   0        0        0    94412 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf
--rw-rw-rw-   0        0        0    87236 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/fonts/RobotoMono-Regular.ttf
--rw-rw-rw-   0        0        0    87496 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf
--rw-rw-rw-   0        0        0    94508 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf
--rw-rw-rw-   0        0        0    88288 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/fonts/RobotoMono-Thin.ttf
--rw-rw-rw-   0        0        0    93588 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf
-drwxrwxrwx   0        0        0        0 2024-04-04 19:10:24.453012 PyQtUIkit-2.1.0/PyQtUIkit/themes/
--rw-rw-rw-   0        0        0     2180 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/themes/__init__.py
--rw-rw-rw-   0        0        0     5879 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/themes/builtin_themes.py
--rw-rw-rw-   0        0        0  1559097 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/themes/icons.py
--rw-rw-rw-   0        0        0     1346 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/themes/svg.py
--rw-rw-rw-   0        0        0     1402 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/themes/theme.py
-drwxrwxrwx   0        0        0        0 2024-04-04 19:10:24.468640 PyQtUIkit-2.1.0/PyQtUIkit/widgets/
--rw-rw-rw-   0        0        0     1505 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/widgets/__init__.py
--rw-rw-rw-   0        0        0     3515 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/widgets/_widget.py
--rw-rw-rw-   0        0        0     1359 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/widgets/application.py
--rw-rw-rw-   0        0        0     7833 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/widgets/button.py
--rw-rw-rw-   0        0        0     2785 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/widgets/checkbox.py
--rw-rw-rw-   0        0        0    10004 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/widgets/combo_box.py
--rw-rw-rw-   0        0        0     7013 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/widgets/dialog.py
--rw-rw-rw-   0        0        0     5807 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/widgets/flow_layout.py
--rw-rw-rw-   0        0        0     2505 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/widgets/group.py
--rw-rw-rw-   0        0        0     4293 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/widgets/hbox_layout.py
--rw-rw-rw-   0        0        0     1578 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/widgets/icon_widget.py
--rw-rw-rw-   0        0        0     1100 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/widgets/label.py
--rw-rw-rw-   0        0        0     1468 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/widgets/line_edit.py
--rw-rw-rw-   0        0        0     3448 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/widgets/list_widget.py
--rw-rw-rw-   0        0        0     1076 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/widgets/main_window.py
--rw-rw-rw-   0        0        0     3302 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/widgets/menu.py
--rw-rw-rw-   0        0        0     7076 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/widgets/navigation.py
--rw-rw-rw-   0        0        0     2504 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/widgets/progress_bar.py
--rw-rw-rw-   0        0        0     6683 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/widgets/radio.py
--rw-rw-rw-   0        0        0     3881 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/widgets/scroll_area.py
--rw-rw-rw-   0        0        0     1173 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/widgets/separator.py
--rw-rw-rw-   0        0        0     7507 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/widgets/spin_box.py
--rw-rw-rw-   0        0        0     3580 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/widgets/spinner.py
--rw-rw-rw-   0        0        0    13356 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/widgets/tab_bar.py
--rw-rw-rw-   0        0        0     1218 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/widgets/tabs.py
--rw-rw-rw-   0        0        0     2167 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/widgets/text_edit.py
--rw-rw-rw-   0        0        0     4465 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/widgets/toggle.py
--rw-rw-rw-   0        0        0    17249 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/widgets/tree_widget.py
--rw-rw-rw-   0        0        0     4620 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/widgets/vbox_layout.py
-drwxrwxrwx   0        0        0        0 2024-04-04 19:10:24.421768 PyQtUIkit-2.1.0/PyQtUIkit.egg-info/
--rw-rw-rw-   0        0        0     2938 2024-04-04 19:10:24.000000 PyQtUIkit-2.1.0/PyQtUIkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2507 2024-04-04 19:10:24.000000 PyQtUIkit-2.1.0/PyQtUIkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 19:10:24.000000 PyQtUIkit-2.1.0/PyQtUIkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2024-04-04 19:10:24.000000 PyQtUIkit-2.1.0/PyQtUIkit.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       26 2024-04-04 19:10:24.000000 PyQtUIkit-2.1.0/PyQtUIkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-04 19:10:24.000000 PyQtUIkit-2.1.0/PyQtUIkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-04 19:10:24.468640 PyQtUIkit-2.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1411 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 20:50:29.346984 PyQtUIkit-2.1.1/
+-rw-rw-rw-   0        0        0     1090 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/LICENSE
+-rw-rw-rw-   0        0        0     2938 2024-04-04 20:50:29.346984 PyQtUIkit-2.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-04 20:50:29.300119 PyQtUIkit-2.1.1/PyQtUIkit/
+-rw-rw-rw-   0        0        0       49 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/__init__.py
+-rw-rw-rw-   0        0        0     3835 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/_icons.py
+drwxrwxrwx   0        0        0        0 2024-04-04 20:50:29.315737 PyQtUIkit-2.1.1/PyQtUIkit/builder/
+-rw-rw-rw-   0        0        0     1116 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/builder/__init__.py
+-rw-rw-rw-   0        0        0     1825 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/builder/builder_class.py
+-rw-rw-rw-   0        0        0     1383 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/builder/builder_module.py
+drwxrwxrwx   0        0        0        0 2024-04-04 20:50:29.315737 PyQtUIkit-2.1.1/PyQtUIkit/core/
+-rw-rw-rw-   0        0        0       84 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/core/__init__.py
+-rw-rw-rw-   0        0        0       19 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/core/_version.py
+-rw-rw-rw-   0        0        0     1503 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/core/font.py
+-rw-rw-rw-   0        0        0     1019 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/core/icon.py
+-rw-rw-rw-   0        0        0     4655 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/core/properties.py
+drwxrwxrwx   0        0        0        0 2024-04-04 20:50:29.331364 PyQtUIkit-2.1.1/PyQtUIkit/fonts/
+-rw-rw-rw-   0        0        0   168060 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/fonts/Roboto-Black.ttf
+-rw-rw-rw-   0        0        0   174108 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/fonts/Roboto-BlackItalic.ttf
+-rw-rw-rw-   0        0        0   167336 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/fonts/Roboto-Bold.ttf
+-rw-rw-rw-   0        0        0   171508 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/fonts/Roboto-BoldItalic.ttf
+-rw-rw-rw-   0        0        0   170504 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/fonts/Roboto-Italic.ttf
+-rw-rw-rw-   0        0        0   167000 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/fonts/Roboto-Light.ttf
+-rw-rw-rw-   0        0        0   173172 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/fonts/Roboto-LightItalic.ttf
+-rw-rw-rw-   0        0        0   168644 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/fonts/Roboto-Medium.ttf
+-rw-rw-rw-   0        0        0   173416 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/fonts/Roboto-MediumItalic.ttf
+-rw-rw-rw-   0        0        0   168260 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/fonts/Roboto-Regular.ttf
+-rw-rw-rw-   0        0        0   168488 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/fonts/Roboto-Thin.ttf
+-rw-rw-rw-   0        0        0   172860 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/fonts/Roboto-ThinItalic.ttf
+-rw-rw-rw-   0        0        0    87392 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/fonts/RobotoMono-Bold.ttf
+-rw-rw-rw-   0        0        0    94636 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf
+-rw-rw-rw-   0        0        0    88248 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf
+-rw-rw-rw-   0        0        0    94016 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf
+-rw-rw-rw-   0        0        0    94372 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/fonts/RobotoMono-Italic.ttf
+-rw-rw-rw-   0        0        0    87980 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/fonts/RobotoMono-Light.ttf
+-rw-rw-rw-   0        0        0    94256 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf
+-rw-rw-rw-   0        0        0    87172 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/fonts/RobotoMono-Medium.ttf
+-rw-rw-rw-   0        0        0    94412 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf
+-rw-rw-rw-   0        0        0    87236 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/fonts/RobotoMono-Regular.ttf
+-rw-rw-rw-   0        0        0    87496 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf
+-rw-rw-rw-   0        0        0    94508 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf
+-rw-rw-rw-   0        0        0    88288 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/fonts/RobotoMono-Thin.ttf
+-rw-rw-rw-   0        0        0    93588 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf
+drwxrwxrwx   0        0        0        0 2024-04-04 20:50:29.331364 PyQtUIkit-2.1.1/PyQtUIkit/themes/
+-rw-rw-rw-   0        0        0     2180 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/themes/__init__.py
+-rw-rw-rw-   0        0        0     5879 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/themes/builtin_themes.py
+-rw-rw-rw-   0        0        0  1559097 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/themes/icons.py
+-rw-rw-rw-   0        0        0     1346 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/themes/svg.py
+-rw-rw-rw-   0        0        0     1402 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/themes/theme.py
+drwxrwxrwx   0        0        0        0 2024-04-04 20:50:29.346984 PyQtUIkit-2.1.1/PyQtUIkit/widgets/
+-rw-rw-rw-   0        0        0     1505 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/widgets/__init__.py
+-rw-rw-rw-   0        0        0     3515 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/widgets/_widget.py
+-rw-rw-rw-   0        0        0     1359 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/widgets/application.py
+-rw-rw-rw-   0        0        0     7833 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/widgets/button.py
+-rw-rw-rw-   0        0        0     2785 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/widgets/checkbox.py
+-rw-rw-rw-   0        0        0    10004 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/widgets/combo_box.py
+-rw-rw-rw-   0        0        0     7013 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/widgets/dialog.py
+-rw-rw-rw-   0        0        0     5807 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/widgets/flow_layout.py
+-rw-rw-rw-   0        0        0     2280 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/widgets/group.py
+-rw-rw-rw-   0        0        0     4293 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/widgets/hbox_layout.py
+-rw-rw-rw-   0        0        0     1578 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/widgets/icon_widget.py
+-rw-rw-rw-   0        0        0     1100 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/widgets/label.py
+-rw-rw-rw-   0        0        0     1487 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/widgets/line_edit.py
+-rw-rw-rw-   0        0        0     3448 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/widgets/list_widget.py
+-rw-rw-rw-   0        0        0     1076 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/widgets/main_window.py
+-rw-rw-rw-   0        0        0     3302 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/widgets/menu.py
+-rw-rw-rw-   0        0        0     7076 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/widgets/navigation.py
+-rw-rw-rw-   0        0        0     2504 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/widgets/progress_bar.py
+-rw-rw-rw-   0        0        0     6683 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/widgets/radio.py
+-rw-rw-rw-   0        0        0     3881 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/widgets/scroll_area.py
+-rw-rw-rw-   0        0        0     1173 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/widgets/separator.py
+-rw-rw-rw-   0        0        0     7533 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/widgets/spin_box.py
+-rw-rw-rw-   0        0        0     3580 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/widgets/spinner.py
+-rw-rw-rw-   0        0        0    13356 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/widgets/tab_bar.py
+-rw-rw-rw-   0        0        0     1218 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/widgets/tabs.py
+-rw-rw-rw-   0        0        0     2167 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/widgets/text_edit.py
+-rw-rw-rw-   0        0        0     4465 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/widgets/toggle.py
+-rw-rw-rw-   0        0        0    17249 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/widgets/tree_widget.py
+-rw-rw-rw-   0        0        0     4620 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/PyQtUIkit/widgets/vbox_layout.py
+drwxrwxrwx   0        0        0        0 2024-04-04 20:50:29.300119 PyQtUIkit-2.1.1/PyQtUIkit.egg-info/
+-rw-rw-rw-   0        0        0     2938 2024-04-04 20:50:29.000000 PyQtUIkit-2.1.1/PyQtUIkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2507 2024-04-04 20:50:29.000000 PyQtUIkit-2.1.1/PyQtUIkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 20:50:29.000000 PyQtUIkit-2.1.1/PyQtUIkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-04-04 20:50:29.000000 PyQtUIkit-2.1.1/PyQtUIkit.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       26 2024-04-04 20:50:29.000000 PyQtUIkit-2.1.1/PyQtUIkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-04 20:50:29.000000 PyQtUIkit-2.1.1/PyQtUIkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-04 20:50:29.346984 PyQtUIkit-2.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1411 2024-04-04 20:49:42.000000 PyQtUIkit-2.1.1/setup.py
```

### Comparing `PyQtUIkit-2.1.0/LICENSE` & `PyQtUIkit-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/PKG-INFO` & `PyQtUIkit-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQtUIkit
-Version: 2.1.0
+Version: 2.1.1
 Summary: A PyQtUIkit package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) [year] [fullname]
```

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/_icons.py` & `PyQtUIkit-2.1.1/PyQtUIkit/_icons.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/builder/__init__.py` & `PyQtUIkit-2.1.1/PyQtUIkit/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/builder/builder_class.py` & `PyQtUIkit-2.1.1/PyQtUIkit/builder/builder_class.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/builder/builder_module.py` & `PyQtUIkit-2.1.1/PyQtUIkit/builder/builder_module.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/core/font.py` & `PyQtUIkit-2.1.1/PyQtUIkit/core/font.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/core/icon.py` & `PyQtUIkit-2.1.1/PyQtUIkit/core/icon.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/core/properties.py` & `PyQtUIkit-2.1.1/PyQtUIkit/core/properties.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/fonts/Roboto-Black.ttf` & `PyQtUIkit-2.1.1/PyQtUIkit/fonts/Roboto-Black.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/fonts/Roboto-BlackItalic.ttf` & `PyQtUIkit-2.1.1/PyQtUIkit/fonts/Roboto-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/fonts/Roboto-Bold.ttf` & `PyQtUIkit-2.1.1/PyQtUIkit/fonts/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/fonts/Roboto-BoldItalic.ttf` & `PyQtUIkit-2.1.1/PyQtUIkit/fonts/Roboto-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/fonts/Roboto-Italic.ttf` & `PyQtUIkit-2.1.1/PyQtUIkit/fonts/Roboto-Italic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/fonts/Roboto-Light.ttf` & `PyQtUIkit-2.1.1/PyQtUIkit/fonts/Roboto-Light.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/fonts/Roboto-LightItalic.ttf` & `PyQtUIkit-2.1.1/PyQtUIkit/fonts/Roboto-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/fonts/Roboto-Medium.ttf` & `PyQtUIkit-2.1.1/PyQtUIkit/fonts/Roboto-Medium.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/fonts/Roboto-MediumItalic.ttf` & `PyQtUIkit-2.1.1/PyQtUIkit/fonts/Roboto-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/fonts/Roboto-Regular.ttf` & `PyQtUIkit-2.1.1/PyQtUIkit/fonts/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/fonts/Roboto-Thin.ttf` & `PyQtUIkit-2.1.1/PyQtUIkit/fonts/Roboto-Thin.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/fonts/Roboto-ThinItalic.ttf` & `PyQtUIkit-2.1.1/PyQtUIkit/fonts/Roboto-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/fonts/RobotoMono-Bold.ttf` & `PyQtUIkit-2.1.1/PyQtUIkit/fonts/RobotoMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf` & `PyQtUIkit-2.1.1/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf` & `PyQtUIkit-2.1.1/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf` & `PyQtUIkit-2.1.1/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/fonts/RobotoMono-Italic.ttf` & `PyQtUIkit-2.1.1/PyQtUIkit/fonts/RobotoMono-Italic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/fonts/RobotoMono-Light.ttf` & `PyQtUIkit-2.1.1/PyQtUIkit/fonts/RobotoMono-Light.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf` & `PyQtUIkit-2.1.1/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/fonts/RobotoMono-Medium.ttf` & `PyQtUIkit-2.1.1/PyQtUIkit/fonts/RobotoMono-Medium.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf` & `PyQtUIkit-2.1.1/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/fonts/RobotoMono-Regular.ttf` & `PyQtUIkit-2.1.1/PyQtUIkit/fonts/RobotoMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf` & `PyQtUIkit-2.1.1/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf` & `PyQtUIkit-2.1.1/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/fonts/RobotoMono-Thin.ttf` & `PyQtUIkit-2.1.1/PyQtUIkit/fonts/RobotoMono-Thin.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf` & `PyQtUIkit-2.1.1/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/themes/__init__.py` & `PyQtUIkit-2.1.1/PyQtUIkit/themes/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/themes/builtin_themes.py` & `PyQtUIkit-2.1.1/PyQtUIkit/themes/builtin_themes.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/themes/icons.py` & `PyQtUIkit-2.1.1/PyQtUIkit/themes/icons.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/themes/svg.py` & `PyQtUIkit-2.1.1/PyQtUIkit/themes/svg.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/themes/theme.py` & `PyQtUIkit-2.1.1/PyQtUIkit/themes/theme.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/widgets/__init__.py` & `PyQtUIkit-2.1.1/PyQtUIkit/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/widgets/_widget.py` & `PyQtUIkit-2.1.1/PyQtUIkit/widgets/_widget.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/widgets/application.py` & `PyQtUIkit-2.1.1/PyQtUIkit/widgets/application.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/widgets/button.py` & `PyQtUIkit-2.1.1/PyQtUIkit/widgets/button.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/widgets/checkbox.py` & `PyQtUIkit-2.1.1/PyQtUIkit/widgets/checkbox.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/widgets/combo_box.py` & `PyQtUIkit-2.1.1/PyQtUIkit/widgets/combo_box.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/widgets/dialog.py` & `PyQtUIkit-2.1.1/PyQtUIkit/widgets/dialog.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/widgets/flow_layout.py` & `PyQtUIkit-2.1.1/PyQtUIkit/widgets/flow_layout.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/widgets/group.py` & `PyQtUIkit-2.1.1/PyQtUIkit/widgets/group.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,18 +29,15 @@
     def clear(self):
         super().clear()
         self.__group.clear()
 
     def _apply_theme(self):
         self.setFixedHeight(self.height + self.contentsMargins().top() + self.contentsMargins().bottom())
         for item in self.__group:
-            if isinstance(item, KitIconButton):
-                item.size = self.height
-            else:
-                item.setFixedHeight(self.height)
+            item.setFixedHeight(self.height)
             item.border = self.border
             item.radius = self.radius
         super()._apply_theme()
 
 
 class KitVGroup(KitVBoxLayout):
     width = IntProperty('width', 150)
@@ -57,14 +54,11 @@
     def addItem(self, item: (QWidget, _KitGroupItem)):
         super().addWidget(item)
         self.__group.add_item(item)
 
     def _apply_theme(self):
         self.setFixedWidth(self.width + self.contentsMargins().left() + self.contentsMargins().right())
         for item in self.__group:
-            if isinstance(item, KitIconButton):
-                item.size = self.width
-            else:
-                item.setFixedWidth(self.width)
+            item.setFixedWidth(self.width)
             item.border = self.border
             item.radius = self.radius
         super()._apply_theme()
```

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/widgets/hbox_layout.py` & `PyQtUIkit-2.1.1/PyQtUIkit/widgets/hbox_layout.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/widgets/icon_widget.py` & `PyQtUIkit-2.1.1/PyQtUIkit/widgets/icon_widget.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/widgets/label.py` & `PyQtUIkit-2.1.1/PyQtUIkit/widgets/label.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/widgets/line_edit.py` & `PyQtUIkit-2.1.1/PyQtUIkit/widgets/line_edit.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,14 +21,15 @@
         self.setFont(self.font.get(self.font_size))
         self.setStyleSheet(f"""
 QLineEdit {{
     color: {self.main_palette.text};
     background-color: {self.main_palette.main};
     border: {self.border}px solid {self.border_palette.main};
     {self._border_radius_css()}
+    padding: 2px;
 }}
 QLineEdit:hover {{
     border: {self.border}px solid {self.border_palette.hover};
     background-color: {self.main_palette.hover};
 }}
 QLineEdit:focus {{
     border: {self.border}px solid {self.border_palette.selected};
```

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/widgets/list_widget.py` & `PyQtUIkit-2.1.1/PyQtUIkit/widgets/list_widget.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/widgets/main_window.py` & `PyQtUIkit-2.1.1/PyQtUIkit/widgets/main_window.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/widgets/menu.py` & `PyQtUIkit-2.1.1/PyQtUIkit/widgets/menu.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/widgets/navigation.py` & `PyQtUIkit-2.1.1/PyQtUIkit/widgets/navigation.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/widgets/progress_bar.py` & `PyQtUIkit-2.1.1/PyQtUIkit/widgets/progress_bar.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/widgets/radio.py` & `PyQtUIkit-2.1.1/PyQtUIkit/widgets/radio.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/widgets/scroll_area.py` & `PyQtUIkit-2.1.1/PyQtUIkit/widgets/scroll_area.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/widgets/separator.py` & `PyQtUIkit-2.1.1/PyQtUIkit/widgets/separator.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/widgets/spin_box.py` & `PyQtUIkit-2.1.1/PyQtUIkit/widgets/spin_box.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,27 +7,27 @@
 
 class KitSpinBox(QWidget, _KitGroupItem):
     border = IntProperty('border', 1)
     radius = IntProperty('radius', 4)
 
     valueChanged = pyqtSignal(object)
     valueEdited = pyqtSignal(object)
-    editingFinished = pyqtSignal()
 
     font = FontProperty('font')
     font_size = EnumProperty('font_size', KitFont.Size, KitFont.Size.MEDIUM)
 
     def __init__(self, func=int):
         super().__init__()
         self._min = 0
         self._max = 100
         self._step = 1
         self._func = func
         self._last_text = '0'
         self._last_pos = 0
+        self._value_changed = False
         self.setMaximumHeight(24)
 
         main_layout = QHBoxLayout()
         main_layout.setSpacing(0)
         main_layout.setContentsMargins(0, 0, 0, 0)
         self.setLayout(main_layout)
 
@@ -52,15 +52,21 @@
 
         self._button_down = QPushButton()
         self._button_down.setCursor(Qt.CursorShape.PointingHandCursor)
         # self._button_down.setFixedWidth(20)
         self._button_down.clicked.connect(self._decrease)
         buttons_layout.addWidget(self._button_down)
 
-    def _on_text_edited(self, manually=True):
+    def _on_text_edited(self):
+        value = 0 if not self._last_text else self._func(self._last_text)
+        self._fix_value()
+        if value != self.value:
+            self._value_changed = True
+
+    def _fix_value(self):
         text = self._line_edit.text()
         try:
             value = 0 if text in ['', '+', '-'] else self._func(text)
         except ValueError:
             pos = self._last_pos
             self._line_edit.setText(self._last_text)
             self._last_pos = pos
@@ -71,58 +77,54 @@
                 self._line_edit.setText(self._last_text)
             elif text and value > self._max:
                 self._last_text = str(self._max)
                 self._line_edit.setText(self._last_text)
             else:
                 self._last_text = text
             self.valueChanged.emit(value)
-            if manually:
-                self.valueEdited.emit(value)
             self._last_pos = self._line_edit.cursorPosition()
 
     def _on_cursor_moved(self):
         self._last_pos = self._line_edit.cursorPosition()
 
     def _on_editing_finished(self):
         text = self._line_edit.text()
         if not text:
             self._line_edit.setText('0')
             self._on_text_edited()
-        self.editingFinished.emit()
+        if self._value_changed:
+            self.valueEdited.emit(self.value)
+            self._value_changed = False
 
     def _decrease(self):
         self.setValue(round(self.value - self._step, 2))
-        self.valueChanged.emit(self.value)
-        # self._line_edit.selectAll()
-        # self._line_edit.setFocus()
-        self.editingFinished.emit()
+        self.valueEdited.emit(self.value)
+        self._value_changed = False
 
     def _increase(self):
         self.setValue(round(self.value + self._step, 2))
-        self.valueChanged.emit(self.value)
-        # self._line_edit.selectAll()
-        # self._line_edit.setFocus()
-        self.editingFinished.emit()
+        self.valueEdited.emit(self.value)
+        self._value_changed = False
 
     def setRange(self, minimum, maximum):
         self._min = minimum
         self._max = maximum
-        self._on_text_edited(False)
+        self._on_text_edited()
 
     def setMinimum(self, minimum):
         self._min = minimum
-        self._on_text_edited(False)
+        self._on_text_edited()
 
     def setMaximum(self, maximum):
         self._max = maximum
-        self._on_text_edited(False)
+        self._on_text_edited()
 
     def setValue(self, value):
         self._line_edit.setText(str(value))
-        self._on_text_edited(False)
+        self._on_text_edited()
 
     def getValue(self):
         if not self._line_edit.text():
             return 0
         return self._func(self._line_edit.text())
 
     def _apply_theme(self):
```

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/widgets/spinner.py` & `PyQtUIkit-2.1.1/PyQtUIkit/widgets/spinner.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/widgets/tab_bar.py` & `PyQtUIkit-2.1.1/PyQtUIkit/widgets/tab_bar.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/widgets/tabs.py` & `PyQtUIkit-2.1.1/PyQtUIkit/widgets/tabs.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/widgets/text_edit.py` & `PyQtUIkit-2.1.1/PyQtUIkit/widgets/text_edit.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/widgets/toggle.py` & `PyQtUIkit-2.1.1/PyQtUIkit/widgets/toggle.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/widgets/tree_widget.py` & `PyQtUIkit-2.1.1/PyQtUIkit/widgets/tree_widget.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit/widgets/vbox_layout.py` & `PyQtUIkit-2.1.1/PyQtUIkit/widgets/vbox_layout.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit.egg-info/PKG-INFO` & `PyQtUIkit-2.1.1/PyQtUIkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQtUIkit
-Version: 2.1.0
+Version: 2.1.1
 Summary: A PyQtUIkit package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) [year] [fullname]
```

### Comparing `PyQtUIkit-2.1.0/PyQtUIkit.egg-info/SOURCES.txt` & `PyQtUIkit-2.1.1/PyQtUIkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.1.0/setup.py` & `PyQtUIkit-2.1.1/setup.py`

 * *Files identical despite different names*

