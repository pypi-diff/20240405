# Comparing `tmp/sphinx-translation-button-1.0.8.tar.gz` & `tmp/sphinx-translation-button-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-translation-button-1.0.8.tar", last modified: Fri Mar 29 20:49:21 2024, max compression
+gzip compressed data, was "sphinx-translation-button-1.0.9.tar", last modified: Fri Apr  5 14:56:24 2024, max compression
```

## Comparing `sphinx-translation-button-1.0.8.tar` & `sphinx-translation-button-1.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 20:49:21.044143 sphinx-translation-button-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-29 20:49:16.000000 sphinx-translation-button-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-03-29 20:49:21.044143 sphinx-translation-button-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-29 20:49:16.000000 sphinx-translation-button-1.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-03-29 20:49:16.000000 sphinx-translation-button-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 20:49:21.044143 sphinx-translation-button-1.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 20:49:21.044143 sphinx-translation-button-1.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 20:49:21.044143 sphinx-translation-button-1.0.8/src/sphinx-translation-button/
--rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-03-29 20:49:16.000000 sphinx-translation-button-1.0.8/src/sphinx-translation-button/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 20:49:21.044143 sphinx-translation-button-1.0.8/src/sphinx-translation-button/static/
--rw-r--r--   0 runner    (1001) docker     (127)     4840 2024-03-29 20:49:16.000000 sphinx-translation-button-1.0.8/src/sphinx-translation-button/static/package_translation_button.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 20:49:21.044143 sphinx-translation-button-1.0.8/src/sphinx_translation_button.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-03-29 20:49:21.000000 sphinx-translation-button-1.0.8/src/sphinx_translation_button.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-03-29 20:49:21.000000 sphinx-translation-button-1.0.8/src/sphinx_translation_button.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 20:49:21.000000 sphinx-translation-button-1.0.8/src/sphinx_translation_button.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-29 20:49:21.000000 sphinx-translation-button-1.0.8/src/sphinx_translation_button.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-29 20:49:21.000000 sphinx-translation-button-1.0.8/src/sphinx_translation_button.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:56:24.542926 sphinx-translation-button-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-05 14:56:19.000000 sphinx-translation-button-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-05 14:56:24.538926 sphinx-translation-button-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-05 14:56:19.000000 sphinx-translation-button-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-05 14:56:19.000000 sphinx-translation-button-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 14:56:24.542926 sphinx-translation-button-1.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:56:24.538926 sphinx-translation-button-1.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:56:24.538926 sphinx-translation-button-1.0.9/src/sphinx-translation-button/
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-05 14:56:19.000000 sphinx-translation-button-1.0.9/src/sphinx-translation-button/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:56:24.538926 sphinx-translation-button-1.0.9/src/sphinx-translation-button/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     5075 2024-04-05 14:56:19.000000 sphinx-translation-button-1.0.9/src/sphinx-translation-button/static/package_translation_button.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:56:24.538926 sphinx-translation-button-1.0.9/src/sphinx_translation_button.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-05 14:56:24.000000 sphinx-translation-button-1.0.9/src/sphinx_translation_button.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-05 14:56:24.000000 sphinx-translation-button-1.0.9/src/sphinx_translation_button.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 14:56:24.000000 sphinx-translation-button-1.0.9/src/sphinx_translation_button.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-05 14:56:24.000000 sphinx-translation-button-1.0.9/src/sphinx_translation_button.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-05 14:56:24.000000 sphinx-translation-button-1.0.9/src/sphinx_translation_button.egg-info/top_level.txt
```

### Comparing `sphinx-translation-button-1.0.8/src/sphinx-translation-button/__init__.py` & `sphinx-translation-button-1.0.9/src/sphinx-translation-button/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,19 +39,23 @@
 
         print("[sphinx-translation-button] copied files to _static directory.")
         
 def createVariable(file_name: str) -> str:
     # Read yaml file
     with open(file_name, 'r') as file:
         data = yaml.load(file, Loader=yaml.FullLoader)
-        languages = data['languages'] if 'languages' in data else print("[sphinx-translation-button] build failed due to missing languages in _config.yml. Please add languages to _config.yml.")
+        languages = data['languages'] if 'languages' in data else print('\033[91m' + " [sphinx-translation-button] build failed due to missing languages in _config.yml. Please add languages to _config.yml. "+ '\033[0m')
+
+    # check against first language
+    [print('\033[91m' + " [sphinx-translation-button] Not all languages contain all necessery arguments "+ '\033[0m') for language in languages if len(language) != len(languages[0])] 
     
     # Compose result_languages using list comprehension and join
     result_languages = f"let _languages = [{', '.join([f'{language}' for language in languages])}]"
     print("[sphinx-translation-button] adding languages : ", languages)
+    
     return result_languages + "\n\n"
 
    
 
     
 
 def setup(app: Sphinx) -> dict[str, str]:
```

### Comparing `sphinx-translation-button-1.0.8/src/sphinx-translation-button/static/package_translation_button.js` & `sphinx-translation-button-1.0.9/src/sphinx-translation-button/static/package_translation_button.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -9,23 +9,30 @@
 }
 
 
 // MAIN => hook into the DOM and add the buttons
 document.addEventListener('DOMContentLoaded', () => addLanguageSwitch(_button_data, _languages))
 
 const addLanguageSwitch = (button_data, languages) => {
+
+    // Process link to prevent breaking
+    if (languages[0].length == 2) languages = languages.map(([language, code]) => [language, code, ""]);
     console.log("[sphinx-translation-button] languages specified: ", languages)
+
     // properly append items to button_data
-    button_data.items = languages.map(([language, code]) => ({
+    button_data.items = languages.map(([language, code, link]) => ({
         "label": language,
         "onclick": () => {
             console.log("[sphinx-translation-button] adding ", language, " with code ", code)
-            // Check current language
-            let currentLanguageCode = languages.find(([language, code]) => window.location.pathname.includes(`/${code}/`))?.[1] || null;
-            currentLanguageCode != null && (window.location.pathname = window.location.pathname.replace(`/${currentLanguageCode}/`, `/${code}/`));
+            if (link != "") {
+                window.location.href = 'link'
+            } else {
+                let currentLanguageCode = languages.find(([language, code]) => window.location.pathname.includes(`/${code}/`))?.[1] || null;
+                currentLanguageCode != null && (window.location.pathname = window.location.pathname.replace(`/${currentLanguageCode}/`, `/${code}/`));
+            }
         }
     }))
     addDropdown(button_data)
 }
 
 let addDropdown = (button) => {
     // Create a new container for full element
```

