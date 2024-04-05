# Comparing `tmp/inventree-kicad-plugin-1.3.9.tar.gz` & `tmp/inventree-kicad-plugin-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/inventree-kicad-plugin-1.3.9.tar", last modified: Fri Dec  8 22:48:24 2023, max compression
+gzip compressed data, was "dist/inventree-kicad-plugin-1.4.0.tar", last modified: Fri Apr  5 19:47:58 2024, max compression
```

## Comparing `inventree-kicad-plugin-1.3.9.tar` & `inventree-kicad-plugin-1.4.0.tar`

### file list

```diff
@@ -1,31 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 22:48:24.000000 inventree-kicad-plugin-1.3.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2023-12-08 22:48:15.000000 inventree-kicad-plugin-1.3.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       45 2023-12-08 22:48:15.000000 inventree-kicad-plugin-1.3.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7402 2023-12-08 22:48:24.000000 inventree-kicad-plugin-1.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7031 2023-12-08 22:48:15.000000 inventree-kicad-plugin-1.3.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 22:48:24.000000 inventree-kicad-plugin-1.3.9/inventree_kicad/
--rw-r--r--   0 runner    (1001) docker     (127)    13062 2023-12-08 22:48:15.000000 inventree-kicad-plugin-1.3.9/inventree_kicad/KiCadLibraryPlugin.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2023-12-08 22:48:15.000000 inventree-kicad-plugin-1.3.9/inventree_kicad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2023-12-08 22:48:15.000000 inventree-kicad-plugin-1.3.9/inventree_kicad/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 22:48:24.000000 inventree-kicad-plugin-1.3.9/inventree_kicad/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)      661 2023-12-08 22:48:15.000000 inventree-kicad-plugin-1.3.9/inventree_kicad/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      840 2023-12-08 22:48:15.000000 inventree-kicad-plugin-1.3.9/inventree_kicad/migrations/0002_auto_20230920_0115.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2023-12-08 22:48:15.000000 inventree-kicad-plugin-1.3.9/inventree_kicad/migrations/0003_selectedcategory_default_reference.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2023-12-08 22:48:15.000000 inventree-kicad-plugin-1.3.9/inventree_kicad/migrations/0004_alter_selectedcategory_options.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2023-12-08 22:48:15.000000 inventree-kicad-plugin-1.3.9/inventree_kicad/migrations/0005_selectedcategory_default_value_parameter_template.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-08 22:48:15.000000 inventree-kicad-plugin-1.3.9/inventree_kicad/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2023-12-08 22:48:15.000000 inventree-kicad-plugin-1.3.9/inventree_kicad/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    14468 2023-12-08 22:48:15.000000 inventree-kicad-plugin-1.3.9/inventree_kicad/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 22:48:24.000000 inventree-kicad-plugin-1.3.9/inventree_kicad/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 22:48:24.000000 inventree-kicad-plugin-1.3.9/inventree_kicad/templates/inventree_kicad/
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2023-12-08 22:48:15.000000 inventree-kicad-plugin-1.3.9/inventree_kicad/templates/inventree_kicad/kicad_bom_import.html
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-08 22:48:15.000000 inventree-kicad-plugin-1.3.9/inventree_kicad/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2023-12-08 22:48:15.000000 inventree-kicad-plugin-1.3.9/inventree_kicad/viewsets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 22:48:24.000000 inventree-kicad-plugin-1.3.9/inventree_kicad_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7402 2023-12-08 22:48:24.000000 inventree-kicad-plugin-1.3.9/inventree_kicad_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      905 2023-12-08 22:48:24.000000 inventree-kicad-plugin-1.3.9/inventree_kicad_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-08 22:48:24.000000 inventree-kicad-plugin-1.3.9/inventree_kicad_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2023-12-08 22:48:24.000000 inventree-kicad-plugin-1.3.9/inventree_kicad_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-12-08 22:48:24.000000 inventree-kicad-plugin-1.3.9/inventree_kicad_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      143 2023-12-08 22:48:24.000000 inventree-kicad-plugin-1.3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      974 2023-12-08 22:48:15.000000 inventree-kicad-plugin-1.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:47:58.000000 inventree-kicad-plugin-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-05 19:47:48.000000 inventree-kicad-plugin-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-05 19:47:48.000000 inventree-kicad-plugin-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9648 2024-04-05 19:47:58.000000 inventree-kicad-plugin-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9277 2024-04-05 19:47:48.000000 inventree-kicad-plugin-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:47:58.000000 inventree-kicad-plugin-1.4.0/inventree_kicad/
+-rw-r--r--   0 runner    (1001) docker     (127)    16219 2024-04-05 19:47:48.000000 inventree-kicad-plugin-1.4.0/inventree_kicad/KiCadLibraryPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-05 19:47:48.000000 inventree-kicad-plugin-1.4.0/inventree_kicad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-05 19:47:48.000000 inventree-kicad-plugin-1.4.0/inventree_kicad/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:47:58.000000 inventree-kicad-plugin-1.4.0/inventree_kicad/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-05 19:47:48.000000 inventree-kicad-plugin-1.4.0/inventree_kicad/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-05 19:47:48.000000 inventree-kicad-plugin-1.4.0/inventree_kicad/migrations/0002_auto_20230920_0115.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-05 19:47:48.000000 inventree-kicad-plugin-1.4.0/inventree_kicad/migrations/0003_selectedcategory_default_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-05 19:47:48.000000 inventree-kicad-plugin-1.4.0/inventree_kicad/migrations/0004_alter_selectedcategory_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-05 19:47:48.000000 inventree-kicad-plugin-1.4.0/inventree_kicad/migrations/0005_selectedcategory_default_value_parameter_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-05 19:47:48.000000 inventree-kicad-plugin-1.4.0/inventree_kicad/migrations/0006_progressindicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-05 19:47:48.000000 inventree-kicad-plugin-1.4.0/inventree_kicad/migrations/0007_auto_20231212_1720.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-05 19:47:48.000000 inventree-kicad-plugin-1.4.0/inventree_kicad/migrations/0008_alter_selectedcategory_footprint_parameter_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 19:47:48.000000 inventree-kicad-plugin-1.4.0/inventree_kicad/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-04-05 19:47:48.000000 inventree-kicad-plugin-1.4.0/inventree_kicad/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16506 2024-04-05 19:47:48.000000 inventree-kicad-plugin-1.4.0/inventree_kicad/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:47:58.000000 inventree-kicad-plugin-1.4.0/inventree_kicad/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:47:58.000000 inventree-kicad-plugin-1.4.0/inventree_kicad/templates/inventree_kicad/
+-rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-04-05 19:47:48.000000 inventree-kicad-plugin-1.4.0/inventree_kicad/templates/inventree_kicad/kicad_bom_import.html
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-05 19:47:48.000000 inventree-kicad-plugin-1.4.0/inventree_kicad/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-05 19:47:48.000000 inventree-kicad-plugin-1.4.0/inventree_kicad/viewsets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:47:58.000000 inventree-kicad-plugin-1.4.0/inventree_kicad_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9648 2024-04-05 19:47:58.000000 inventree-kicad-plugin-1.4.0/inventree_kicad_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-05 19:47:58.000000 inventree-kicad-plugin-1.4.0/inventree_kicad_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 19:47:58.000000 inventree-kicad-plugin-1.4.0/inventree_kicad_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-05 19:47:58.000000 inventree-kicad-plugin-1.4.0/inventree_kicad_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-05 19:47:58.000000 inventree-kicad-plugin-1.4.0/inventree_kicad_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-05 19:47:58.000000 inventree-kicad-plugin-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-05 19:47:48.000000 inventree-kicad-plugin-1.4.0/setup.py
```

### Comparing `inventree-kicad-plugin-1.3.9/LICENSE` & `inventree-kicad-plugin-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `inventree-kicad-plugin-1.3.9/PKG-INFO` & `inventree-kicad-plugin-1.4.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,127 +1,144 @@
-Metadata-Version: 2.1
-Name: inventree-kicad-plugin
-Version: 1.3.9
-Summary: KiCad HTTP library plugin for InvenTree
-Home-page: https://github.com/afkiwers/inventree_kicad
-Author: Andre Iwers
-Author-email: iwers11@gmail.com
-License: MIT
-Keywords: inventree kicad pcb schematic inventory
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # InvenTree KiCad - HTTP Library Plugin
 
-A KiCad Conform API endpoint plugin, designed for seamless integration with [InvenTree](https://inventree.org), empowers users to seamlessly incorporate InvenTree parts into KiCad's parts library tool. Please note that this plugin exclusively offers metadata and necessitates the presence of corresponding symbol and footprint libraries within the KiCad EDA environment.
+A KiCad Conform API endpoint plugin, designed for integration with [InvenTree](https://inventree.org), empowers users to seamlessly incorporate InvenTree parts into KiCad's parts library tool. Please note that this plugin exclusively offers metadata and necessitates the presence of corresponding symbol and footprint libraries within the KiCad EDA environment.
 
 As of the current stage of development, KiCad exclusively offers read-only access to parts through the HTTP lib interface.
 
+However, this plugin provides a metadata import tool to import changes made within KiCad. This enables users to add footprints, symbols and datasheets to individual parts during the schematic design process if not already available and re-import that information into InvenTree to have it available for the next time.
+
 ## Installing the Plugin
+
 There are several methods available for installing this plugin. To gain a comprehensive understanding of the installation process, please refer to the [InvenTree - Installing a Plugin Guide](https://docs.inventree.org/en/latest/extend/plugins/install/#installation-methods). Depending on your preferred approach, the following instructions will provide you with the necessary information.
 
 Prior to plugin installation, ensure that you've activated both **URL Integration** and **App Integration**. You can accomplish this by going to Settings → Plugin Settings → Plugins. Additionally, if you're operating within a Docker environment, be sure to enable **Check plugins on startup** as well.
 
 ![image](https://raw.githubusercontent.com/afkiwers/inventree_kicad/main/images/plugin_general_settings.png)
 
 ### Through GitHub
+
 Navigate to the **Plugin Settings** and click on the Install Plugin button. This will trigger a new window to appear, prompting you to enter the following information:
 
 - Package Name: inventree-kicad-plugin
-- Source URL: git+https://github.com/afkiwers/inventree-kicad-plugin
+- Source URL: <git+https://github.com/afkiwers/inventree_kicad>
 
 ![image](https://raw.githubusercontent.com/afkiwers/inventree_kicad/main/images/install_plugin_via_github_url.png)
 
 ### Through PiP
+
 The plugin can be found here: [inventree-kicad-plugin](https://pypi.org/project/inventree-kicad-plugin/).
 
 - Package Name: inventree-kicad-plugin
 
-![image](images/pip_install.png)
-
+![image](https://raw.githubusercontent.com/afkiwers/inventree_kicad/main/images/pip_install.png)
 
 **IMPORTANT**: Remember to restart your server and run the migrate command to implement the model changes required for this plugin. Failure to do so may result in the plugin encountering issues and not functioning correctly.
 
 ## Configure Plugin Settings
-After installing the plugin, head over to the Plugin Settings and activate it. Look for **KiCadLibraryPlugin** in the list of available plugins. Once activated, you'll be able to open the plugin and proceed with the setup process.
 
-![image](https://github.com/afkiwers/inventree_kicad/raw/main/images/admin_add_change_categories.png)
+After installing the plugin, head over to the Plugin Settings and activate it. Look for **KiCadLibraryPlugin** in the list of available plugins. 
+
+![image](https://raw.githubusercontent.com/afkiwers/inventree_kicad/main/images/plugin_settings.png)
+
+
+Once activated, you'll see a new plugin **KiCad Library Endpoint** on the left hand side. Click on it to open the plugin and proceed with the setup process.
+
+![image](https://raw.githubusercontent.com/afkiwers/inventree_kicad/main/images/new_plugin.png)
+
 
 ## Adding Categories to KiCad
+
 Navigate to the admin backend, and scroll down until you find the **INVENTREE_KICAD** section. Within this section, click on **KiCad Categories**.
 If the section is not visible, ensure you've enabled the "Enable URL integration" and "Enable app integration" options in the Plugin Settings and run a database migration.
 
-![image](https://github.com/afkiwers/inventree_kicad/raw/main/images/admin_model.png)
+![image](https://raw.githubusercontent.com/afkiwers/inventree_kicad/main/images/admin_model.png)
 
 Once opened the "KiCad Categories" model, you'll have the option to add new categories which, once added, will be visible in KiCad's Symbol Chooser dialog.
 
-![image](https://github.com/afkiwers/inventree_kicad/raw/main/images/admin_add_change_categories.png)
+![image](https://raw.githubusercontent.com/afkiwers/inventree_kicad/main/images/admin_add_change_categories.png)
 
 #### Default Settings for Categories
+
 The plugin allows you to set default values when the child part lacks specific details regarding the KiCad symbol, footprint, or reference. This feature is particularly useful when dealing with components such as resistors or capacitors, as they often share the same symbols, reducing the need for repetitive data entry.
 
-![image](https://github.com/afkiwers/inventree_kicad/raw/main/images/admin_add_category.png)
+![image](https://raw.githubusercontent.com/afkiwers/inventree_kicad/main/images/admin_add_category.png)
+
+#### Utilizing Footprint Parameter Mapping
+
+If you have existing Footprint/Package Type parameters assigned to your components and prefer not to define a separate KiCad Footprint Parameter for them, you can leverage the Footprint Parameter Mapping functionality to establish a connection to KiCad Footprint names. Simply incorporate the desired mappings into the KiCad category:
+
+![image](https://raw.githubusercontent.com/afkiwers/inventree_kicad/main/images/admin_footprint_mappings.png)
+
+Additionally, you can combine this with the per-category "Footprint Parameter Template" override to utilize a different parameter for mapping purposes.
+
+![image](https://raw.githubusercontent.com/afkiwers/inventree_kicad/main/images/admin_footprint_parameter_override.png)
 
 ## Creating User Access Tokens
-Head back to the admin backend and click on Tokens. Click on "ADD Token" to generate a token dedicated to a particular user. It is important to emphasize that it is highly advisable to create individual tokens for each user, rather than employing a single token for everyone.
 
-![image](https://github.com/afkiwers/inventree_kicad/raw/main/images/admin_tokens.png)
+Return to the administrative backend, navigate to the USER model, and access API Tokens. Select "ADD API Token" to generate a token designated for a specific user. It's crucial to highlight the importance of creating separate tokens for each user, rather than using a universal token for everyone.
+
+![image](https://raw.githubusercontent.com/afkiwers/inventree_kicad/main/images/admin_tokens.png)
+
+## KiCad HTTP Library File
 
-## KiCad Configuration files
-Below is an example config which should help you get started reasonably quickly. The only thing needed here is to replace **http://127.0.0.1:8000** with your server's InvenTree URL, and replace usertokendatastring with a valid token. Save it as a file with `.kicad_httplib` extension, as specified in the [preliminary KiCad docs](https://docs.kicad.org/master/en/eeschema/eeschema_advanced.html#http-libraries). To use it, add it as a symbol library inside KiCad.
+Below is an example config which should help you get started reasonably quickly. The only thing needed here is to replace **<http://127.0.0.1:8000>** with your server's InvenTree URL, and replace usertokendatastring with a valid token. Save it as a file with `.kicad_httplib` extension, as specified in the [preliminary KiCad docs](https://docs.kicad.org/master/en/eeschema/eeschema_advanced.html#http-libraries). To use it, add it as a symbol library inside KiCad.
 
 **Please Note**: The config file does not contain any part or category information. It merely tells KiCad what API to expect, what token to use and where to find it.
 
 ```json
 {
     "meta": {
         "version": 1.0
     },
     "name": "KiCad HTTP Library",
     "description": "A KiCad library sourced from a REST API",
     "source": {
         "type": "REST_API",
         "api_version": "v1",
         "root_url": "http://127.0.0.1:8000/plugin/kicad-library-plugin",
-        "token": "usertokendatastring"
+        "token": "usertokendatastring",
+        "timeout_parts_seconds": 60,
+        "timeout_categories_seconds": 6000
     }
 }
 ```
+
 ## Add the HTTP library to KiCad
 
-Inside KiCads project manager, navigate to `Preferences -> Manage Symbol Libraries` and click on it. Add a GLobal Library by pressing the folder in the bottom left corner.
-![image](/images/add_symbol_lib.png)
+Inside KiCad's project manager, navigate to `Preferences -> Manage Symbol Libraries` and click on it. Add a GLobal Library by pressing the folder in the bottom left corner.
+![image](https://raw.githubusercontent.com/afkiwers/inventree_kicad/main/images/add_symbol_lib.png)
 
 When choosing the `.kicad_httplib` file, KiCad will automatically detect that it is a HTTP lib file and only a Nickname needs to be set.
 
 It's recommended to put a **#** as prefix to make sure it is at the top of the list. Otherwise one might end up scrolling a lot.
 
-## Use in KiCad
+## Display Stock Information in KiCad
+If activated KiCad will show stock data inside the symbol chooser. The data will be updated whenever the set category timeout expires ([`timeout_categories_seconds`](#kicad-http-library-file)). 
 
-Once everything has been configured properly, KiCad should be able to display all the categories and parts using the Symbol Picker. 
+![image](https://raw.githubusercontent.com/afkiwers/inventree_kicad/main/images/stock_data_settings.png)
 
-Inside the schematic, one can either use the shortcut and press **A** or navigate to the ribbon at the top and press `Place -> Add Symbol`.
+Users have the option to determine the presentation style of stock data through the **Stock Count Display Format** as shown above. In this setting, {0} represents the item description, while {1} represents the stock information as a numerical value. Using those placeholders, users can customize how this data is merged and showcased according to their preferences. An example of how this would look is shown below. 
 
-![image](/images/eeschema_open_chooser.png)
+**Please Note:** The stock information is not transferred into the schematic. It is only visible inside the symbol chooser!
 
-The Symbol Chooser should open up and display the parts sourced from InvenTree.
+![image](https://raw.githubusercontent.com/afkiwers/inventree_kicad/main/images/stock_data.png)
 
-![image](/images/symbol_chooser.png)
 
-## Importing Metadata from Previous Projects
-Since KiCad does not offer a way to push information back to the server, InvenTree needs to have all that metadata such as footprints and symbols added manually. This can be very tedious, especially when there are thousands of parts.
+## Use in KiCad
+
+Once everything has been configured properly, KiCad should be able to display all the categories and parts using the Symbol Picker.
 
-This plugin's import tool uses KiCads intermediate file which is created whenever there is a BOM export. This file contains all the project's data which is needed.
+Inside the schematic, one can either use the shortcut and press **A** or navigate to the ribbon at the top and press `Place -> Add Symbol`.
 
-![image](/images/kicad_meta_data_import.png) 
+![image](https://raw.githubusercontent.com/afkiwers/inventree_kicad/main/images/eeschema_open_chooser.png)
 
-## FAQ
+The Symbol Chooser should open up and display the parts sourced from InvenTree.
 
-### Why does this Plugin need the App Mixin?
+![image](https://raw.githubusercontent.com/afkiwers/inventree_kicad/main/images/symbol_chooser.png)
 
-This plugin uses the App Mixin to add a custom model to the database to manage the selected categories. Otherwise, KiCad symbol chooser would be cluttered with every single category (See [Categories](#adding-categories-to-kicad))
+## Importing Metadata from Previous Projects
 
-### Why does this Plugin need the Url Mixin?
+Since KiCad does not offer a way to push information back to the server, InvenTree needs to have all that metadata such as footprints and symbols added manually. This can be very tedious, especially when there are thousands of parts.
 
-This plugin uses the Url Mixin to expose custom API endpoints which are conform with KiCads REST API requirements.
+This plugin's import tool uses KiCad's intermediate file which is created whenever there is a BOM export. This file contains all the project's data which is needed.
 
+![image](https://raw.githubusercontent.com/afkiwers/inventree_kicad/main/images/kicad_meta_data_import.png)
```

### Comparing `inventree-kicad-plugin-1.3.9/README.md` & `inventree-kicad-plugin-1.4.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,114 +1,157 @@
+Metadata-Version: 2.1
+Name: inventree-kicad-plugin
+Version: 1.4.0
+Summary: KiCad HTTP library plugin for InvenTree
+Home-page: https://github.com/afkiwers/inventree_kicad
+Author: Andre Iwers
+Author-email: iwers11@gmail.com
+License: MIT
+Keywords: inventree kicad pcb schematic inventory
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # InvenTree KiCad - HTTP Library Plugin
 
-A KiCad Conform API endpoint plugin, designed for seamless integration with [InvenTree](https://inventree.org), empowers users to seamlessly incorporate InvenTree parts into KiCad's parts library tool. Please note that this plugin exclusively offers metadata and necessitates the presence of corresponding symbol and footprint libraries within the KiCad EDA environment.
+A KiCad Conform API endpoint plugin, designed for integration with [InvenTree](https://inventree.org), empowers users to seamlessly incorporate InvenTree parts into KiCad's parts library tool. Please note that this plugin exclusively offers metadata and necessitates the presence of corresponding symbol and footprint libraries within the KiCad EDA environment.
 
 As of the current stage of development, KiCad exclusively offers read-only access to parts through the HTTP lib interface.
 
+However, this plugin provides a metadata import tool to import changes made within KiCad. This enables users to add footprints, symbols and datasheets to individual parts during the schematic design process if not already available and re-import that information into InvenTree to have it available for the next time.
+
 ## Installing the Plugin
+
 There are several methods available for installing this plugin. To gain a comprehensive understanding of the installation process, please refer to the [InvenTree - Installing a Plugin Guide](https://docs.inventree.org/en/latest/extend/plugins/install/#installation-methods). Depending on your preferred approach, the following instructions will provide you with the necessary information.
 
 Prior to plugin installation, ensure that you've activated both **URL Integration** and **App Integration**. You can accomplish this by going to Settings → Plugin Settings → Plugins. Additionally, if you're operating within a Docker environment, be sure to enable **Check plugins on startup** as well.
 
 ![image](https://raw.githubusercontent.com/afkiwers/inventree_kicad/main/images/plugin_general_settings.png)
 
 ### Through GitHub
+
 Navigate to the **Plugin Settings** and click on the Install Plugin button. This will trigger a new window to appear, prompting you to enter the following information:
 
 - Package Name: inventree-kicad-plugin
-- Source URL: git+https://github.com/afkiwers/inventree-kicad-plugin
+- Source URL: <git+https://github.com/afkiwers/inventree_kicad>
 
 ![image](https://raw.githubusercontent.com/afkiwers/inventree_kicad/main/images/install_plugin_via_github_url.png)
 
 ### Through PiP
+
 The plugin can be found here: [inventree-kicad-plugin](https://pypi.org/project/inventree-kicad-plugin/).
 
 - Package Name: inventree-kicad-plugin
 
-![image](images/pip_install.png)
-
+![image](https://raw.githubusercontent.com/afkiwers/inventree_kicad/main/images/pip_install.png)
 
 **IMPORTANT**: Remember to restart your server and run the migrate command to implement the model changes required for this plugin. Failure to do so may result in the plugin encountering issues and not functioning correctly.
 
 ## Configure Plugin Settings
-After installing the plugin, head over to the Plugin Settings and activate it. Look for **KiCadLibraryPlugin** in the list of available plugins. Once activated, you'll be able to open the plugin and proceed with the setup process.
 
-![image](https://github.com/afkiwers/inventree_kicad/raw/main/images/admin_add_change_categories.png)
+After installing the plugin, head over to the Plugin Settings and activate it. Look for **KiCadLibraryPlugin** in the list of available plugins. 
+
+![image](https://raw.githubusercontent.com/afkiwers/inventree_kicad/main/images/plugin_settings.png)
+
+
+Once activated, you'll see a new plugin **KiCad Library Endpoint** on the left hand side. Click on it to open the plugin and proceed with the setup process.
+
+![image](https://raw.githubusercontent.com/afkiwers/inventree_kicad/main/images/new_plugin.png)
+
 
 ## Adding Categories to KiCad
+
 Navigate to the admin backend, and scroll down until you find the **INVENTREE_KICAD** section. Within this section, click on **KiCad Categories**.
 If the section is not visible, ensure you've enabled the "Enable URL integration" and "Enable app integration" options in the Plugin Settings and run a database migration.
 
-![image](https://github.com/afkiwers/inventree_kicad/raw/main/images/admin_model.png)
+![image](https://raw.githubusercontent.com/afkiwers/inventree_kicad/main/images/admin_model.png)
 
 Once opened the "KiCad Categories" model, you'll have the option to add new categories which, once added, will be visible in KiCad's Symbol Chooser dialog.
 
-![image](https://github.com/afkiwers/inventree_kicad/raw/main/images/admin_add_change_categories.png)
+![image](https://raw.githubusercontent.com/afkiwers/inventree_kicad/main/images/admin_add_change_categories.png)
 
 #### Default Settings for Categories
+
 The plugin allows you to set default values when the child part lacks specific details regarding the KiCad symbol, footprint, or reference. This feature is particularly useful when dealing with components such as resistors or capacitors, as they often share the same symbols, reducing the need for repetitive data entry.
 
-![image](https://github.com/afkiwers/inventree_kicad/raw/main/images/admin_add_category.png)
+![image](https://raw.githubusercontent.com/afkiwers/inventree_kicad/main/images/admin_add_category.png)
+
+#### Utilizing Footprint Parameter Mapping
+
+If you have existing Footprint/Package Type parameters assigned to your components and prefer not to define a separate KiCad Footprint Parameter for them, you can leverage the Footprint Parameter Mapping functionality to establish a connection to KiCad Footprint names. Simply incorporate the desired mappings into the KiCad category:
+
+![image](https://raw.githubusercontent.com/afkiwers/inventree_kicad/main/images/admin_footprint_mappings.png)
+
+Additionally, you can combine this with the per-category "Footprint Parameter Template" override to utilize a different parameter for mapping purposes.
+
+![image](https://raw.githubusercontent.com/afkiwers/inventree_kicad/main/images/admin_footprint_parameter_override.png)
 
 ## Creating User Access Tokens
-Head back to the admin backend and click on Tokens. Click on "ADD Token" to generate a token dedicated to a particular user. It is important to emphasize that it is highly advisable to create individual tokens for each user, rather than employing a single token for everyone.
 
-![image](https://github.com/afkiwers/inventree_kicad/raw/main/images/admin_tokens.png)
+Return to the administrative backend, navigate to the USER model, and access API Tokens. Select "ADD API Token" to generate a token designated for a specific user. It's crucial to highlight the importance of creating separate tokens for each user, rather than using a universal token for everyone.
+
+![image](https://raw.githubusercontent.com/afkiwers/inventree_kicad/main/images/admin_tokens.png)
+
+## KiCad HTTP Library File
 
-## KiCad Configuration files
-Below is an example config which should help you get started reasonably quickly. The only thing needed here is to replace **http://127.0.0.1:8000** with your server's InvenTree URL, and replace usertokendatastring with a valid token. Save it as a file with `.kicad_httplib` extension, as specified in the [preliminary KiCad docs](https://docs.kicad.org/master/en/eeschema/eeschema_advanced.html#http-libraries). To use it, add it as a symbol library inside KiCad.
+Below is an example config which should help you get started reasonably quickly. The only thing needed here is to replace **<http://127.0.0.1:8000>** with your server's InvenTree URL, and replace usertokendatastring with a valid token. Save it as a file with `.kicad_httplib` extension, as specified in the [preliminary KiCad docs](https://docs.kicad.org/master/en/eeschema/eeschema_advanced.html#http-libraries). To use it, add it as a symbol library inside KiCad.
 
 **Please Note**: The config file does not contain any part or category information. It merely tells KiCad what API to expect, what token to use and where to find it.
 
 ```json
 {
     "meta": {
         "version": 1.0
     },
     "name": "KiCad HTTP Library",
     "description": "A KiCad library sourced from a REST API",
     "source": {
         "type": "REST_API",
         "api_version": "v1",
         "root_url": "http://127.0.0.1:8000/plugin/kicad-library-plugin",
-        "token": "usertokendatastring"
+        "token": "usertokendatastring",
+        "timeout_parts_seconds": 60,
+        "timeout_categories_seconds": 6000
     }
 }
 ```
+
 ## Add the HTTP library to KiCad
 
-Inside KiCads project manager, navigate to `Preferences -> Manage Symbol Libraries` and click on it. Add a GLobal Library by pressing the folder in the bottom left corner.
-![image](/images/add_symbol_lib.png)
+Inside KiCad's project manager, navigate to `Preferences -> Manage Symbol Libraries` and click on it. Add a GLobal Library by pressing the folder in the bottom left corner.
+![image](https://raw.githubusercontent.com/afkiwers/inventree_kicad/main/images/add_symbol_lib.png)
 
 When choosing the `.kicad_httplib` file, KiCad will automatically detect that it is a HTTP lib file and only a Nickname needs to be set.
 
 It's recommended to put a **#** as prefix to make sure it is at the top of the list. Otherwise one might end up scrolling a lot.
 
-## Use in KiCad
+## Display Stock Information in KiCad
+If activated KiCad will show stock data inside the symbol chooser. The data will be updated whenever the set category timeout expires ([`timeout_categories_seconds`](#kicad-http-library-file)). 
 
-Once everything has been configured properly, KiCad should be able to display all the categories and parts using the Symbol Picker. 
+![image](https://raw.githubusercontent.com/afkiwers/inventree_kicad/main/images/stock_data_settings.png)
 
-Inside the schematic, one can either use the shortcut and press **A** or navigate to the ribbon at the top and press `Place -> Add Symbol`.
+Users have the option to determine the presentation style of stock data through the **Stock Count Display Format** as shown above. In this setting, {0} represents the item description, while {1} represents the stock information as a numerical value. Using those placeholders, users can customize how this data is merged and showcased according to their preferences. An example of how this would look is shown below. 
 
-![image](/images/eeschema_open_chooser.png)
+**Please Note:** The stock information is not transferred into the schematic. It is only visible inside the symbol chooser!
 
-The Symbol Chooser should open up and display the parts sourced from InvenTree.
+![image](https://raw.githubusercontent.com/afkiwers/inventree_kicad/main/images/stock_data.png)
 
-![image](/images/symbol_chooser.png)
 
-## Importing Metadata from Previous Projects
-Since KiCad does not offer a way to push information back to the server, InvenTree needs to have all that metadata such as footprints and symbols added manually. This can be very tedious, especially when there are thousands of parts.
+## Use in KiCad
+
+Once everything has been configured properly, KiCad should be able to display all the categories and parts using the Symbol Picker.
 
-This plugin's import tool uses KiCads intermediate file which is created whenever there is a BOM export. This file contains all the project's data which is needed.
+Inside the schematic, one can either use the shortcut and press **A** or navigate to the ribbon at the top and press `Place -> Add Symbol`.
 
-![image](/images/kicad_meta_data_import.png) 
+![image](https://raw.githubusercontent.com/afkiwers/inventree_kicad/main/images/eeschema_open_chooser.png)
 
-## FAQ
+The Symbol Chooser should open up and display the parts sourced from InvenTree.
 
-### Why does this Plugin need the App Mixin?
+![image](https://raw.githubusercontent.com/afkiwers/inventree_kicad/main/images/symbol_chooser.png)
 
-This plugin uses the App Mixin to add a custom model to the database to manage the selected categories. Otherwise, KiCad symbol chooser would be cluttered with every single category (See [Categories](#adding-categories-to-kicad))
+## Importing Metadata from Previous Projects
 
-### Why does this Plugin need the Url Mixin?
+Since KiCad does not offer a way to push information back to the server, InvenTree needs to have all that metadata such as footprints and symbols added manually. This can be very tedious, especially when there are thousands of parts.
 
-This plugin uses the Url Mixin to expose custom API endpoints which are conform with KiCads REST API requirements.
+This plugin's import tool uses KiCad's intermediate file which is created whenever there is a BOM export. This file contains all the project's data which is needed.
 
+![image](https://raw.githubusercontent.com/afkiwers/inventree_kicad/main/images/kicad_meta_data_import.png)
```

### Comparing `inventree-kicad-plugin-1.3.9/inventree_kicad/KiCadLibraryPlugin.py` & `inventree-kicad-plugin-1.4.0/inventree_kicad/KiCadLibraryPlugin.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,32 +2,30 @@
 
 API endpoint for Kicad REST API library.
 
 This plugin supplies the endpoints and data needed for KiCad to display selected categories and their
 corresponding parts within the Kicad environment.
 
 """
-import datetime
-
 from django.core.validators import URLValidator
 
-from django.conf.urls import url
 from django.http import JsonResponse
 from django.template.loader import render_to_string
 from django.urls import include, re_path
 from django.utils.translation import gettext_lazy as _
 
 from InvenTree.helpers import str2bool
 from common.notifications import logger
 from part.models import Part, PartParameterTemplate, PartParameter, PartAttachment
 from plugin import InvenTreePlugin
 from plugin.base.integration.mixins import SettingsContentMixin
 from plugin.mixins import UrlsMixin, AppMixin, SettingsMixin
 import xml.etree.ElementTree as elementTree
 
+from .models import ProgressIndicator
 from .version import KICAD_PLUGIN_VERSION
 
 
 class KiCadLibraryPlugin(UrlsMixin, AppMixin, SettingsMixin, SettingsContentMixin, InvenTreePlugin):
     """Plugin for KiCad Library Endpoint.
     
     Provides a set of API endpoints which conform to the KiCad REST API specification.
@@ -39,42 +37,48 @@
 
     VERSION = KICAD_PLUGIN_VERSION
 
     TITLE = "KiCad Library Endpoint"
     SLUG = "kicad-library-plugin"
     NAME = "KiCadLibraryPlugin"
 
-    PUBLISH_DATE = datetime.date(2023, 9, 21)
-
     WEBSITE = "https://github.com/afkiwers"
 
     MIN_VERSION = '0.12.0'
 
     SETTINGS = {
         'KICAD_ENABLE_SUBCATEGORY': {
             'name': _('Enable Sub-Category Parts'),
             'description': _(
                 'When activated, the plugin will provide all components associated with this category, including those located within sub-categories'),
             'validator': bool,
             'default': True,
         },
-        'KICAD_INCLUDE_IPN': {
-            'name': _('Include IPN in part fields'),
+        'KICAD_ENABLE_STOCK_COUNT': {
+            'name': _('Display Available Stock'),
             'description': _(
-                'When activated, the IPN is included in the KiCad fields for a part'),
+                'When activated, the plugin will provide stock information which will be displayed as part of the top level description in KiCad'),
             'validator': bool,
             'default': False,
         },
-        'KICAD_META_DATA_IMPORT_ADD_DATASHEET': {
-            'name': _('Add datasheet if URL is valid'),
-            'description': _(
-                'When activated, the plugin will add the datasheet URL (comment will be \'datasheet\') to the '
-                'attachments.'),
-            'validator': bool,
-            'default': False,
+        'KICAD_ENABLE_STOCK_COUNT_FORMAT': {
+            'name': _('Stock Count Display Format'),
+            'description': _('This will be displayed after the part\'s description in KiCad (right column). Note: {1} contains the Stock information, {0} the description of the part.'),
+            'default': "[Stock: {1}] {0}"
+        },
+        'DEFAULT_FOR_MISSING_SYMBOL': {
+            'name': _('Backup KiCad Symbol'),
+            'description': _('This backup symbol will be used if none has been defined'),
+            'default': ""
+        },
+        'KICAD_INCLUDE_IPN': {
+            'name': _('Include IPN'),
+            'description': _('When activated, the IPN is included in the KiCad fields for a part'),
+            'choices': [('0', 'Do not Include'), ('False', 'Include but Hide in Schematic'), ('True', 'Include and Show in Schematic')],
+            'default': '0',
         },
         'KICAD_SYMBOL_PARAMETER': {
             'name': _('Symbol Parameter'),
             'description': _('The part parameter to use for the symbol name.'),
             'model': 'part.partparametertemplate',
         },
         'KICAD_FOOTPRINT_PARAMETER': {
@@ -104,19 +108,40 @@
             'model': 'part.partparametertemplate',
         },
         'KICAD_EXCLUDE_FROM_SIM_PARAMETER': {
             'name': _('Simulation Exclusion Parameter'),
             'description': _('The part parameter to use for to exclude it from the simulation.'),
             'model': 'part.partparametertemplate',
         },
-        'STAUTS_BAR_PROGRESS': {
-            'name': _('Status bar progress'),
-            'description': _('This is used to display a status bar to the user'),
-            'default': 0,
-            'hidden': True
+        'KICAD_META_DATA_IMPORT_ADD_DATASHEET': {
+            'name': _('[KiCad Metadata Import] Add datasheet if URL is valid'),
+            'description': _(
+                'When activated, the plugin will add the datasheet URL (comment will be \'datasheet\') to the '
+                'attachments.'),
+            'validator': bool,
+            'default': False,
+        },
+        'IMPORT_INVENTREE_ID_FALLBACK': {
+            'name': _('[KiCad Metadata Import] Match Against Part Name'),
+            'description': _(
+                'When activated, the import tool will use the part name as fallback if the ID does not return an existing part.'),
+            'validator': bool,
+            'default': False,
+        },
+        'IMPORT_INVENTREE_OVERRIDE_PARAS': {
+            'name': _('[KiCad Metadata Import] Override Parmeters'),
+            'description': _(
+                'When activated, the import tool will override existing KiCad parameters.'),
+            'validator': bool,
+            'default': False,
+        },
+        'IMPORT_INVENTREE_ID_IDENTIFIER': {
+            'name': _('[KiCad Metadata Import] Inventree Part ID Identifier'),
+            'description': _('This identifier specifies what key the import tool looks for to get the part ID'),
+            'default': "InvenTree"
         },
     }
 
     def get_settings_content(self, request):
         """Custom settings content for the plugin."""
 
         try:
@@ -152,24 +177,27 @@
                 re_path('categories(.json)?/?$', viewsets.CategoryList.as_view(), {'plugin': self},
                         name='kicad-category-list'),
 
                 # Anything else goes to the index view
                 re_path('^.*$', viewsets.Index.as_view(), name='kicad-index'),
             ])),
 
-            url(r'upload(?:\.(?P<format>json))?$', self.import_meta_data, name='meta_data_upload'),
-            url(r'progress_bar_status', self.get_import_progress, name='get_import_progress'),
+            re_path(r'upload(?:\.(?P<format>json))?$', self.import_meta_data, name='meta_data_upload'),
+            re_path(r'progress_bar_status', self.get_import_progress, name='get_import_progress'),
 
             # Anything else, redirect to our top-level v1 page
             re_path('^.*$', viewsets.Index.as_view(), name='kicad-index'),
         ]
 
     def get_import_progress(self, request):
+        progress = ProgressIndicator.objects.get_or_create(user=request.user)[0]
+
         return JsonResponse({
-            'value': self.get_setting('STAUTS_BAR_PROGRESS', None)
+            'value': progress.current_progress,
+            'file_name': progress.file_name
         }, status=200)
 
     def import_meta_data(self, request):  # noqa
 
         if request.FILES.get('file', False):
             file = request.FILES.get('file', False)
 
@@ -192,24 +220,28 @@
             tree = elementTree.parse(file)
             root = tree.getroot()
 
             # Grab the "components" list
             components = root.find('components')
             inventree_parts = set()
 
-            # reset progress bar
-            self.set_setting('STAUTS_BAR_PROGRESS', 0)
+            # get and reset user specific progress bar status
+            import_progress = ProgressIndicator.objects.get_or_create(user=request.user)[0]
+            import_progress.current_progress = 0
+            import_progress.file_name = file
 
             # we start at 0
             comp_cnt = len(components.findall('comp')) - 1
 
             # Iterate through all child components with the tag 'comp'
             for idx, comp in enumerate(components.findall('comp')):
 
-                self.set_setting('STAUTS_BAR_PROGRESS', int((idx / comp_cnt) * 100))
+                # update user specific progress bar status
+                import_progress.current_progress = int((idx / comp_cnt) * 100)
+                import_progress.save()
 
                 ref = comp.attrib.get('ref', None)
 
                 # Missing ref - continue
                 if not ref:
                     logger.debug('Missing ref, skipping')
                     continue
@@ -238,78 +270,103 @@
 
                 if not lib_name or not lib_part:
                     logger.debug('Missing lib_name or lib_part, skipping')
                     continue
 
                 symbol = f'{lib_name}:{lib_part}'
 
-                inventree_id = None
+                inventree_part_id = None
 
                 # check if there are fields, some parts may not have any like fiducials.
                 fields = comp.find('fields')
                 if not fields:
                     logger.debug('Missing fields skipping')
                     continue
 
+                # load the inventree ID identifier
+                inventree_id_identifier = self.get_setting('IMPORT_INVENTREE_ID_IDENTIFIER', None)
+
                 for field in fields:
-                    if str(field.attrib.get('name', '')).lower().startswith('inventree'):
-                        inventree_id = field.text
+                    if str(field.attrib.get('name', '')).lower().startswith(inventree_id_identifier.lower()):
+                        inventree_part_id = field.text
                         break
 
                 # Missing inventree_id, cannot continue
-                if not inventree_id:
-                    logger.debug('Missing inventree_id, skipping')
-                    continue
-
-                try:
-                    inventree_id = int(inventree_id)
-                except ValueError:
-                    logger.debug('InvenTree ID is not an integer, skipping')
+                if not inventree_part_id:
+                    logger.debug('Missing part id, skipping')
                     continue
 
                 # Already checked this one
-                if inventree_id in inventree_parts:
+                if inventree_part_id in inventree_parts:
                     continue
 
                 # add to our cache, we use this to not add the same data multiple times
-                inventree_parts.add(inventree_id)
+                inventree_parts.add(inventree_part_id)
 
+                # try load part from database
+                part = None
                 try:
-                    part = Part.objects.get(id=inventree_id)
+                    part = Part.objects.get(id=inventree_part_id)
+
                 except Part.DoesNotExist:
-                    logger.debug(f'Part ID: {inventree_id} does not belong to an existing part, skipping')
+                    invalid_part = True
+
+                    # try also the part name if user wants it
+                    if self.get_setting('IMPORT_INVENTREE_ID_FALLBACK', None):
+                        try:
+                            part = Part.objects.get(name=inventree_part_id)
+                            invalid_part = False
+
+                            # map actual id as we now know which part we are referencing
+                            inventree_part_id = part.id
+
+                        except Part.DoesNotExist:
+                            invalid_part = True
+
+                    if invalid_part:
+                        logger.debug(f'Part ID: {inventree_part_id} does not belong to an existing part, skipping')
+                        continue
+
+                except Exception as exp:
+                    logger.debug(f'Part ID: {inventree_part_id} caused uknown error {exp}')
                     continue
 
-                # find and/or add template and value
-                template = PartParameterTemplate.objects.get(id=kicad_reference_param_id)
-                parameter = PartParameter.objects.get_or_create(part=part, template=template)
-                parameter[0].data = ref
-                parameter[0].save()
-
-                template = PartParameterTemplate.objects.get(id=kicad_footprint_param_id)
-                parameter = PartParameter.objects.get_or_create(part=part, template=template)
-                parameter[0].data = footprint
-                parameter[0].save()
-
-                template = PartParameterTemplate.objects.get(id=kicad_symbol_param_id)
-                parameter = PartParameter.objects.get_or_create(part=part, template=template)
-                parameter[0].data = symbol
-                parameter[0].save()
+                t_ids = []
+                t_ids.append(kicad_reference_param_id)
+                t_ids.append(kicad_footprint_param_id)
+                t_ids.append(kicad_symbol_param_id)
+
+                t_id_values = []
+                t_id_values .append(ref)
+                t_id_values .append(footprint)
+                t_id_values .append(symbol)
+
+                for idx, t_id in enumerate(t_ids):
+                    # find and/or add template and value
+                    template = PartParameterTemplate.objects.get(id=t_id)
+                    parameter = PartParameter.objects.get_or_create(part=part, template=template)
+                    # Don't override
+                    if parameter[1] or self.get_setting('IMPORT_INVENTREE_OVERRIDE_PARAS', None):
+                        parameter[0].data = t_id_values[idx]
+                        parameter[0].save()
 
                 if datasheet and str2bool(self.get_setting('KICAD_META_DATA_IMPORT_ADD_DATASHEET', False)):
                     try:
                         URLValidator()(datasheet)
                     except Exception as e:
                         logger.debug(f'URL is invalid: {e}')
                         continue
 
+                    # only add a datasheet if there is not already one which is already called out to be one.
                     try:
                         # inventree is not happy with urls which are too long, so let's make sure that this
                         # doesn't prevent us from importing all the following parts.
-                        PartAttachment.objects.get_or_create(part_id=inventree_id, link=datasheet, comment='datasheet')
+                        part = PartAttachment.objects.filter(part_id=inventree_part_id, comment='Datasheet')
+                        if not part:
+                            part = PartAttachment.objects.create(part_id=inventree_part_id, link=datasheet, comment='Datasheet')
                     except Exception as exp:
                         logger.debug(exp)
                         pass
 
             return JsonResponse({}, status=200)
 
         return JsonResponse({'error': 'No file uploaded!'}, status=204)
```

### Comparing `inventree-kicad-plugin-1.3.9/inventree_kicad/migrations/0001_initial.py` & `inventree-kicad-plugin-1.4.0/inventree_kicad/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `inventree-kicad-plugin-1.3.9/inventree_kicad/migrations/0002_auto_20230920_0115.py` & `inventree-kicad-plugin-1.4.0/inventree_kicad/migrations/0002_auto_20230920_0115.py`

 * *Files identical despite different names*

### Comparing `inventree-kicad-plugin-1.3.9/inventree_kicad/migrations/0003_selectedcategory_default_reference.py` & `inventree-kicad-plugin-1.4.0/inventree_kicad/migrations/0003_selectedcategory_default_reference.py`

 * *Files identical despite different names*

### Comparing `inventree-kicad-plugin-1.3.9/inventree_kicad/migrations/0005_selectedcategory_default_value_parameter_template.py` & `inventree-kicad-plugin-1.4.0/inventree_kicad/migrations/0005_selectedcategory_default_value_parameter_template.py`

 * *Files identical despite different names*

### Comparing `inventree-kicad-plugin-1.3.9/inventree_kicad/serializers.py` & `inventree-kicad-plugin-1.4.0/inventree_kicad/serializers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,24 @@
+import logging
+
 from django.utils.translation import gettext_lazy as _
 
 from rest_framework import serializers
 from rest_framework.reverse import reverse_lazy
 
-from InvenTree.helpers import str2bool
+
 from InvenTree.helpers_model import construct_absolute_url
+from part.filters import annotate_total_stock
 from part.models import Part, PartCategory, PartParameter
+from InvenTree.helpers import str2bool, decimal2string
+
+from .models import SelectedCategory, FootprintParameterMapping
+
+
+logger = logging.getLogger('inventree')
 
 
 class KicadDetailedPartSerializer(serializers.ModelSerializer):
     """Custom model serializer for a single KiCad part instance"""
 
     def get_api_url(self):
         """Return the API url associated with this serializer"""
@@ -54,16 +63,14 @@
         If there are multiple possible associations, return the "deepest" one.
         """
 
         # Prevent duplicate lookups
         if hasattr(self, 'kicad_category'):
             return self.kicad_category
 
-        from .models import SelectedCategory
-
         # If the selcted part does not have a category, return None
         if not part.category:
             return None
 
         # Get the category tree for the selected part
         categories = part.category.get_ancestors(include_self=True)
 
@@ -128,19 +135,22 @@
             symbol = kicad_category.default_symbol
 
         # Find the symbol parameter value associated with this part instance
         template_id = self.plugin.get_setting('KICAD_SYMBOL_PARAMETER', None)
 
         symbol = self.get_parameter_value(part, template_id, backup_value=symbol)
 
+        if not symbol:
+            symbol = template_id = self.plugin.get_setting('DEFAULT_FOR_MISSING_SYMBOL', "")
+
         # KiCad does not like colons in their symbol names.
         # Check if there is more than one colon present, if so rebuild string and honour only the first
         # colon. Replace the other colons with underscores.
         cnt = symbol.count(':')
-        if cnt != 1:
+        if cnt != 1 and len(symbol) != 0:
             spilt_str = symbol.split(':')
             tmp_str = ""
 
             for iter, s in enumerate(spilt_str):
                 tmp_str += s
 
                 if iter < 1:
@@ -152,26 +162,42 @@
 
         return str(symbol)
 
     def get_footprint(self, part):
         """Return the footprint associated with this part.
 
         - First, check if the part has a footprint assigned (via parameter)
+        - Then, check if there is a valid footprint mapping
         - Otherwise, fallback to the default footprint for the KiCad Category
         """
 
         footprint = ""
+        footprint_mappings = None
+        template_id = None
 
         if kicad_category := self.get_kicad_category(part):
             footprint = kicad_category.default_footprint
+            footprint_mappings = FootprintParameterMapping.objects.filter(
+                kicad_category=kicad_category,
+            )
+            template = kicad_category.footprint_parameter_template
 
-        template_id = self.plugin.get_setting('KICAD_FOOTPRINT_PARAMETER', None)
+            if template:
+                template_id = kicad_category.footprint_parameter_template.id
+
+        if not template_id:
+            template_id = self.plugin.get_setting('KICAD_FOOTPRINT_PARAMETER', None)
 
         footprint = self.get_parameter_value(part, template_id, backup_value=footprint)
 
+        if footprint_mappings:
+            footprint_mapping = footprint_mappings.filter(parameter_value=footprint).first()
+            if footprint_mapping:
+                footprint = footprint_mapping.kicad_footprint
+
         return str(footprint)
 
     def get_datasheet(self, part):
         """Return the datasheet associated with this part.
 
         Here, we look at the attachments associated with the part,
         and return the first one which has a comment matching "datasheet"
@@ -253,18 +279,18 @@
             },
             'Part URL': {
                 'value': url,
                 'visible': 'False'
             }
         }
 
-        if str2bool(self.plugin.get_setting('KICAD_INCLUDE_IPN', False)):
+        if self.plugin.get_setting('KICAD_INCLUDE_IPN', '0') != '0':
             fields['IPN'] = {
                 'value': f'{part.IPN}',
-                'visible': 'False'
+                'visible': self.plugin.get_setting('KICAD_INCLUDE_IPN', 'False')
             }
 
         for parameter in part.parameters.all():
             # Exclude any which have already been used for default KiCad fields
             if str(parameter.template.pk) in excluded_templates:
                 continue
 
@@ -387,14 +413,52 @@
         """
 
         self.plugin = kwargs.pop('plugin')
         super().__init__(*args, **kwargs)
 
     id = serializers.CharField(source='pk', read_only=True)
 
+    description = serializers.SerializerMethodField('get_description')
+
+    def get_description(self, part):
+        """Custom name function.
+
+        This will allow users to display stock information
+        if they enable it.
+        """
+
+        if not hasattr(self, 'enable_stock_count'):
+            self.enable_stock_count = str2bool(self.plugin.get_setting('KICAD_ENABLE_STOCK_COUNT', False))
+        
+        if not hasattr(self, 'stock_count_format'):
+            self.stock_count_format = self.plugin.get_setting("KICAD_ENABLE_STOCK_COUNT_FORMAT", False)
+
+        description = part.description
+
+        # In-stock quantity should be annotated to the queryset
+        stock_count = getattr(part, 'in_stock', 0)
+
+        if self.enable_stock_count:
+            try:
+                description = self.stock_count_format.format(part.description, decimal2string(stock_count))
+            except Exception as e:
+                logger.exception("Failed to format stock count: %s", e)
+
+        return description
+
+    @staticmethod
+    def annotate_queryset(queryset):
+        """Add extra annotations to the queryset."""
+
+        queryset = queryset.annotate(
+            in_stock=annotate_total_stock(),
+        )
+
+        return queryset
+
 
 class KicadCategorySerializer(serializers.ModelSerializer):
     """Custom model serializer for a single KiCad category instance"""
 
     class Meta:
         """Metaclass defining serializer fields"""
         model = PartCategory
@@ -404,14 +468,8 @@
             'description'
         ]
 
     id = serializers.CharField(source='pk', read_only=True)
     name = serializers.SerializerMethodField('get_name')
 
     def get_name(self, category):
-        """Return the whether or not the part should be excluded from the sim.
-
-        If the part exclusion has been specified via parameter, return that.
-        Otherwise, simply return false
-        """
-
         return category.pathstring
```

### Comparing `inventree-kicad-plugin-1.3.9/inventree_kicad/templates/inventree_kicad/kicad_bom_import.html` & `inventree-kicad-plugin-1.4.0/inventree_kicad/templates/inventree_kicad/kicad_bom_import.html`

 * *Files 19% similar despite different names*

```diff
@@ -1,48 +1,63 @@
 {% load inventree_extras %}
 {% load i18n %}
 {% load static %}
 
 <script>
+    var exitTimer = false
+    const get_url = "{% url 'plugin:kicad-library-plugin:get_import_progress' %}"
+    var file_name = ""
 
-    window.onload = () => {
-        const get_url = "{% url 'plugin:kicad-library-plugin:get_import_progress' %}"
-
-        setInterval(startTimer, 250);
-
-        function startTimer() {
+    function startTimer() {
 
+        // Poll server for progress status
+        if (!exitTimer) {
             $.ajax({
                 url: get_url,
                 type: 'GET',
                 dataType: 'json',
                 success: function (res) {
-
                     document.getElementById("progress_bar").setAttribute("aria-valuenow", res.value);
                     document.getElementById("progress_bar").setAttribute("style", "width:" + res.value + "%;");
-
                     document.getElementById("progress_bar").innerText = res.value + "%";
+
+                    if (res.value === 100) {
+                        exitTimer = true;
+                        document.getElementById("btn_import").disabled = false;
+                    }
+
                 }
             });
         }
+
     }
 
     async function upload_csv() {
         var formData = new FormData();
 
         formData.append("file", fileupload.files[0]);
 
+        exitTimer = false;
+        setInterval(startTimer, 500);
+
         const cmd_url = "{% url 'plugin:kicad-library-plugin:meta_data_upload' %}"
 
-        document.getElementById("import_spinner").hidden = false;
         document.getElementById("progress_bar_container").hidden = false;
+        document.getElementById("btn_import").disabled = true;
+        document.getElementById("btn_import").setAttribute("class", "btn btn-outline-primary")
 
         inventreeFormDataUpload(url = cmd_url, data = formData).then(function (data) {
 
-            document.getElementById("import_spinner").hidden = true;
+            exitTimer = true;
+            document.getElementById("btn_import").setAttribute("class", "btn btn-primary")
+            document.getElementById("btn_import").disabled = false;
+
+            document.getElementById("progress_bar").setAttribute("aria-valuenow", 100);
+            document.getElementById("progress_bar").setAttribute("style", "width: 100%;");
+            document.getElementById("progress_bar").innerText = "100%";
 
             showMessage("Metadata has been processed!", {
                 style: 'success',
                 icon: 'fas fa-server icon-green',
                 details: '',
             });
         });
@@ -73,24 +88,14 @@
 </script>
 
 <div class="panel-heading">
     <h4>KiCad Metadata Import</h4>
 </div>
 
 <div class='panel-content'>
-    <div id="progress_bar_container" class="container mb-5 mt-5" hidden>
-
-        <div class="progress">
-            <div id="progress_bar" class="progress-bar" role="progressbar" style="width: 0;"
-                 aria-valuenow="0"
-                 aria-valuemin="0"
-                 aria-valuemax="100">
-            </div>
-        </div>
-    </div>
 
     <!-- Generic note for user -->
     <div class='alert alert-info alert-block'>
         <strong>Requirements for KiCad Metadata upload:</strong>
         <ul>
             <li>
                 Open the KiCad BOM export tool and use any of the generator scripts to export the part data.
@@ -102,23 +107,34 @@
             </li>
 
             <li>Each part must already exist in the database. If not, KiCad will return an error for that specific
                 part.
             </li>
         </ul>
     </div>
+
+    <div id="progress_bar_container" class="container mb-5 mt-5" hidden>
+
+        <div class="progress">
+            <div id="progress_bar" class="progress-bar" role="progressbar" style="width: 0;"
+                 aria-valuenow="0"
+                 aria-valuemin="0"
+                 aria-valuemax="100">
+            </div>
+        </div>
+    </div>
+
 </div>
 
 <form id="upload-form">
 
     <div class="mb-3">
         <label for="formFile" class="form-label">Please select an XML file</label>
         <input class="form-control" accept=".xml" type="file" id="fileupload" name="fileupload"
                onchange="submit_button_controller()">
     </div>
 
 </form>
 
 <button type="submit" class="btn btn-primary" onclick="upload_csv()" title='Import' id="btn_import" disabled>
     Import Metadata
-    <span class="spinner-border spinner-border-sm" id="import_spinner" hidden role="status" aria-hidden="true"></span>
 </button>
```

### Comparing `inventree-kicad-plugin-1.3.9/inventree_kicad/viewsets.py` & `inventree-kicad-plugin-1.4.0/inventree_kicad/viewsets.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from rest_framework import generics, permissions, response, views
 
 from InvenTree.helpers import str2bool
 from part.models import PartCategory, Part
 
 
+from inventree_kicad import serializers
+
+
 class Index(views.APIView):
     """Index view which provides a list of available endpoints"""
 
     permission_classes = [
         permissions.IsAuthenticated,
     ]
 
@@ -25,34 +28,30 @@
             }
         )
 
 
 class CategoryList(generics.ListAPIView):
     """List of available KiCad categories"""
 
-    from .serializers import KicadCategorySerializer
-
-    serializer_class = KicadCategorySerializer
+    serializer_class = serializers.KicadCategorySerializer
 
     def get_queryset(self):
         """Return only PartCategory objects which are mapped to a SelectedCategory"""
 
         from .models import SelectedCategory
 
         category_ids = SelectedCategory.objects.all().values_list('category_id', flat=True)
 
         return PartCategory.objects.filter(pk__in=category_ids)
 
 
 class PartsPreviewList(generics.ListAPIView):
     """Preview list for all parts in a given category"""
 
-    from .serializers import KicadPreviewPartSerializer
-
-    serializer_class = KicadPreviewPartSerializer
+    serializer_class = serializers.KicadPreviewPartSerializer
 
     def get_serializer(self, *args, **kwargs):
         """Add the parent plugin instance to the serializer contenxt"""
 
         kwargs['plugin'] = self.kwargs['plugin']
 
         return self.serializer_class(*args, **kwargs)
@@ -67,36 +66,39 @@
         category_id = self.kwargs.get('id', None)
 
         # Get a reference to the plugin instance
         plugin = self.kwargs['plugin']
 
         cascade = str2bool(plugin.get_setting('KICAD_ENABLE_SUBCATEGORY', False))
 
-        # Get the part category
-        try:
-            category = PartCategory.objects.get(id=category_id)
-        except PartCategory.DoesNotExist:
-            return Part.objects.all()
-        
-        if cascade:
-            return Part.objects.filter(category__in=category.get_descendants(include_self=True))
-        else:
-            return Part.objects.filter(category=category)
+        queryset = Part.objects.all()
+
+        category = PartCategory.objects.filter(id=category_id).first()
+
+        if category is not None:
+            if cascade:
+                queryset = queryset.filter(
+                    category__in=category.get_descendants(include_self=True)
+                )
+            else:
+                queryset = queryset.filter(category=category)
+
+        queryset = serializers.KicadPreviewPartSerializer.annotate_queryset(queryset)
+
+        return queryset
 
 
 class PartDetail(generics.RetrieveAPIView):
     """Detailed information endpoint for a single part instance.
     
     Here, the lookup id (pk) is the part id.
     The custom plugin serializer formats the data into a KiCad compatible format.
     """
 
-    from .serializers import KicadDetailedPartSerializer
-
-    serializer_class = KicadDetailedPartSerializer
+    serializer_class = serializers.KicadDetailedPartSerializer
     queryset = Part.objects.all()
 
     def get_queryset(self):
         """Prefetch related fields to speed up query"""
 
         queryset = super().get_queryset()
```

### Comparing `inventree-kicad-plugin-1.3.9/inventree_kicad_plugin.egg-info/SOURCES.txt` & `inventree-kicad-plugin-1.4.0/inventree_kicad_plugin.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 inventree_kicad/version.py
 inventree_kicad/viewsets.py
 inventree_kicad/migrations/0001_initial.py
 inventree_kicad/migrations/0002_auto_20230920_0115.py
 inventree_kicad/migrations/0003_selectedcategory_default_reference.py
 inventree_kicad/migrations/0004_alter_selectedcategory_options.py
 inventree_kicad/migrations/0005_selectedcategory_default_value_parameter_template.py
+inventree_kicad/migrations/0006_progressindicator.py
+inventree_kicad/migrations/0007_auto_20231212_1720.py
+inventree_kicad/migrations/0008_alter_selectedcategory_footprint_parameter_template.py
 inventree_kicad/migrations/__init__.py
 inventree_kicad/templates/inventree_kicad/kicad_bom_import.html
 inventree_kicad_plugin.egg-info/PKG-INFO
 inventree_kicad_plugin.egg-info/SOURCES.txt
 inventree_kicad_plugin.egg-info/dependency_links.txt
 inventree_kicad_plugin.egg-info/entry_points.txt
 inventree_kicad_plugin.egg-info/top_level.txt
```

### Comparing `inventree-kicad-plugin-1.3.9/setup.py` & `inventree-kicad-plugin-1.4.0/setup.py`

 * *Files identical despite different names*

