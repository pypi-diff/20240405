# Comparing `tmp/tvb-ext-unicore-1.2.0.tar.gz` & `tmp/tvb-ext-unicore-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tvb-ext-unicore-1.2.0.tar", last modified: Mon Jul 17 11:41:37 2023, max compression
+gzip compressed data, was "tvb-ext-unicore-2.0.0.tar", last modified: Fri Apr  5 20:11:34 2024, max compression
```

## Comparing `tvb-ext-unicore-1.2.0.tar` & `tvb-ext-unicore-2.0.0.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:41:37.489169 tvb-ext-unicore-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    35181 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-07-17 11:41:37.489169 tvb-ext-unicore-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4852 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/RELEASE.md
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/babel.config.js
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/install.json
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/jest.config.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:41:37.473169 tvb-ext-unicore-1.2.0/jupyter-config/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:41:37.481169 tvb-ext-unicore-1.2.0/jupyter-config/nb-config/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/jupyter-config/nb-config/tvbextunicore.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:41:37.481169 tvb-ext-unicore-1.2.0/jupyter-config/server-config/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/jupyter-config/server-config/tvbextunicore.json
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/package.json
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 11:41:37.489169 tvb-ext-unicore-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/sonar-project.properties
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:41:37.481169 tvb-ext-unicore-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:41:37.485169 tvb-ext-unicore-1.2.0/src/__tests__/
--rw-r--r--   0 runner    (1001) docker     (123)     9892 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/src/__tests__/JobOutputFiles.test.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/src/__tests__/ModalComponent.test.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/src/__tests__/PaginationComponent.test.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/src/__tests__/SideButton.test.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/src/__tests__/UnicoreJobsTable.test.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/src/__tests__/UnicoreSites.test.tsx
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/src/__tests__/constants.tests.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     6093 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/src/__tests__/pyunicoreWidget.test.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/src/__tests__/utils.test.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:41:37.485169 tvb-ext-unicore-1.2.0/src/components/
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/src/components/CheckBoxToggle.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     7972 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/src/components/JobOutputFiles.tsx
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/src/components/ModalComponent.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/src/components/PaginationComponent.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/src/components/SideButton.ts
--rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/src/components/UnicoreJobsTable.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/src/components/UnicoreSites.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/src/constants.ts
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/src/globals.d.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/src/handler.ts
--rw-r--r--   0 runner    (1001) docker     (123)     6812 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/src/index.ts
--rw-r--r--   0 runner    (1001) docker     (123)    11617 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/src/pyunicoreWidget.tsx
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/src/utils.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:41:37.485169 tvb-ext-unicore-1.2.0/style/
--rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/style/base.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:41:37.485169 tvb-ext-unicore-1.2.0/style/icons/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/style/icons/logo-unicore.svg
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/style/index.css
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/style/index.js
--rw-r--r--   0 runner    (1001) docker     (123)    13727 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/style/variables.css
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/tsconfig.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:41:37.485169 tvb-ext-unicore-1.2.0/tvb_ext_unicore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-07-17 11:41:37.000000 tvb-ext-unicore-1.2.0/tvb_ext_unicore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-17 11:41:37.000000 tvb-ext-unicore-1.2.0/tvb_ext_unicore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 11:41:37.000000 tvb-ext-unicore-1.2.0/tvb_ext_unicore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 11:40:55.000000 tvb-ext-unicore-1.2.0/tvb_ext_unicore.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-17 11:41:37.000000 tvb-ext-unicore-1.2.0/tvb_ext_unicore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-17 11:41:37.000000 tvb-ext-unicore-1.2.0/tvb_ext_unicore.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:41:37.489169 tvb-ext-unicore-1.2.0/tvbextunicore/
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/tvbextunicore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/tvbextunicore/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/tvbextunicore/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/tvbextunicore/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:41:37.489169 tvb-ext-unicore-1.2.0/tvbextunicore/labextension/
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-07-17 11:41:37.000000 tvb-ext-unicore-1.2.0/tvbextunicore/labextension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:41:37.489169 tvb-ext-unicore-1.2.0/tvbextunicore/labextension/static/
--rw-r--r--   0 runner    (1001) docker     (123)     9777 2023-07-17 11:41:37.000000 tvb-ext-unicore-1.2.0/tvbextunicore/labextension/static/747.c26c9bf4f7bddc1ea1c7.js
--rw-r--r--   0 runner    (1001) docker     (123)    17540 2023-07-17 11:41:37.000000 tvb-ext-unicore-1.2.0/tvbextunicore/labextension/static/774.f5b7ad80ab759770978c.js
--rw-r--r--   0 runner    (1001) docker     (123)     7022 2023-07-17 11:41:37.000000 tvb-ext-unicore-1.2.0/tvbextunicore/labextension/static/remoteEntry.c6b3242597cbbe03a95e.js
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-17 11:41:35.000000 tvb-ext-unicore-1.2.0/tvbextunicore/labextension/static/style.js
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-07-17 11:41:37.000000 tvb-ext-unicore-1.2.0/tvbextunicore/labextension/static/third-party-licenses.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:41:37.489169 tvb-ext-unicore-1.2.0/tvbextunicore/logger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/tvbextunicore/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/tvbextunicore/logger/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/tvbextunicore/logger/logging.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:41:37.489169 tvb-ext-unicore-1.2.0/tvbextunicore/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/tvbextunicore/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7416 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/tvbextunicore/tests/test_unicore_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:41:37.489169 tvb-ext-unicore-1.2.0/tvbextunicore/unicore_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/tvbextunicore/unicore_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/tvbextunicore/unicore_wrapper/job_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     7030 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/tvbextunicore/unicore_wrapper/unicore_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/tvbextunicore/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   372706 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/yarn.lock
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:11:34.143064 tvb-ext-unicore-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-05 20:10:20.000000 tvb-ext-unicore-2.0.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-05 20:10:20.000000 tvb-ext-unicore-2.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35186 2024-04-05 20:10:20.000000 tvb-ext-unicore-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-05 20:10:20.000000 tvb-ext-unicore-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6097 2024-04-05 20:11:34.143064 tvb-ext-unicore-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5011 2024-04-05 20:10:20.000000 tvb-ext-unicore-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-05 20:10:20.000000 tvb-ext-unicore-2.0.0/RELEASE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-05 20:10:20.000000 tvb-ext-unicore-2.0.0/babel.config.js
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-05 20:10:20.000000 tvb-ext-unicore-2.0.0/install.json
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-05 20:10:20.000000 tvb-ext-unicore-2.0.0/jest.config.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:11:34.119063 tvb-ext-unicore-2.0.0/jupyter-config/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:11:34.127064 tvb-ext-unicore-2.0.0/jupyter-config/nb-config/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-05 20:10:20.000000 tvb-ext-unicore-2.0.0/jupyter-config/nb-config/tvbextunicore.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:11:34.127064 tvb-ext-unicore-2.0.0/jupyter-config/server-config/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-05 20:10:20.000000 tvb-ext-unicore-2.0.0/jupyter-config/server-config/tvbextunicore.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-05 20:10:20.000000 tvb-ext-unicore-2.0.0/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-05 20:10:20.000000 tvb-ext-unicore-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 20:11:34.143064 tvb-ext-unicore-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-04-05 20:10:20.000000 tvb-ext-unicore-2.0.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-05 20:10:20.000000 tvb-ext-unicore-2.0.0/sonar-project.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:11:34.127064 tvb-ext-unicore-2.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:11:34.127064 tvb-ext-unicore-2.0.0/src/__tests__/
+-rw-r--r--   0 runner    (1001) docker     (127)     9892 2024-04-05 20:10:20.000000 tvb-ext-unicore-2.0.0/src/__tests__/JobOutputFiles.test.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-05 20:10:20.000000 tvb-ext-unicore-2.0.0/src/__tests__/ModalComponent.test.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-04-05 20:10:20.000000 tvb-ext-unicore-2.0.0/src/__tests__/PaginationComponent.test.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-04-05 20:10:20.000000 tvb-ext-unicore-2.0.0/src/__tests__/SideButton.test.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     6124 2024-04-05 20:10:20.000000 tvb-ext-unicore-2.0.0/src/__tests__/UnicoreJobsTable.test.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-04-05 20:10:20.000000 tvb-ext-unicore-2.0.0/src/__tests__/UnicoreSites.test.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-05 20:10:20.000000 tvb-ext-unicore-2.0.0/src/__tests__/constants.tests.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     6093 2024-04-05 20:10:20.000000 tvb-ext-unicore-2.0.0/src/__tests__/pyunicoreWidget.test.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-05 20:10:20.000000 tvb-ext-unicore-2.0.0/src/__tests__/utils.test.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:11:34.131064 tvb-ext-unicore-2.0.0/src/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-05 20:10:20.000000 tvb-ext-unicore-2.0.0/src/components/CheckBoxToggle.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     8164 2024-04-05 20:10:20.000000 tvb-ext-unicore-2.0.0/src/components/JobOutputFiles.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-05 20:10:20.000000 tvb-ext-unicore-2.0.0/src/components/ModalComponent.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-05 20:10:20.000000 tvb-ext-unicore-2.0.0/src/components/PaginationComponent.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-04-05 20:10:20.000000 tvb-ext-unicore-2.0.0/src/components/SideButton.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     5545 2024-04-05 20:10:20.000000 tvb-ext-unicore-2.0.0/src/components/UnicoreJobsTable.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-05 20:10:20.000000 tvb-ext-unicore-2.0.0/src/components/UnicoreSites.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-05 20:10:20.000000 tvb-ext-unicore-2.0.0/src/constants.ts
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-05 20:10:20.000000 tvb-ext-unicore-2.0.0/src/globals.d.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-04-05 20:10:20.000000 tvb-ext-unicore-2.0.0/src/handler.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     6812 2024-04-05 20:10:20.000000 tvb-ext-unicore-2.0.0/src/index.ts
+-rw-r--r--   0 runner    (1001) docker     (127)    11760 2024-04-05 20:10:20.000000 tvb-ext-unicore-2.0.0/src/pyunicoreWidget.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-05 20:10:20.000000 tvb-ext-unicore-2.0.0/src/utils.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:11:34.139064 tvb-ext-unicore-2.0.0/style/
+-rw-r--r--   0 runner    (1001) docker     (127)     6186 2024-04-05 20:10:20.000000 tvb-ext-unicore-2.0.0/style/base.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:11:34.139064 tvb-ext-unicore-2.0.0/style/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-05 20:10:20.000000 tvb-ext-unicore-2.0.0/style/icons/logo-unicore.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-05 20:10:20.000000 tvb-ext-unicore-2.0.0/style/index.css
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-05 20:10:20.000000 tvb-ext-unicore-2.0.0/style/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13727 2024-04-05 20:10:20.000000 tvb-ext-unicore-2.0.0/style/variables.css
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-05 20:10:20.000000 tvb-ext-unicore-2.0.0/tsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:11:34.143064 tvb-ext-unicore-2.0.0/tvb_ext_unicore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6097 2024-04-05 20:11:34.000000 tvb-ext-unicore-2.0.0/tvb_ext_unicore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-05 20:11:34.000000 tvb-ext-unicore-2.0.0/tvb_ext_unicore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 20:11:34.000000 tvb-ext-unicore-2.0.0/tvb_ext_unicore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 20:10:53.000000 tvb-ext-unicore-2.0.0/tvb_ext_unicore.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-05 20:11:34.000000 tvb-ext-unicore-2.0.0/tvb_ext_unicore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-05 20:11:34.000000 tvb-ext-unicore-2.0.0/tvb_ext_unicore.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:11:34.139064 tvb-ext-unicore-2.0.0/tvbextunicore/
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-05 20:10:20.000000 tvb-ext-unicore-2.0.0/tvbextunicore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-05 20:10:20.000000 tvb-ext-unicore-2.0.0/tvbextunicore/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-05 20:10:20.000000 tvb-ext-unicore-2.0.0/tvbextunicore/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5284 2024-04-05 20:10:20.000000 tvb-ext-unicore-2.0.0/tvbextunicore/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:11:34.139064 tvb-ext-unicore-2.0.0/tvbextunicore/labextension/
+-rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-04-05 20:11:33.000000 tvb-ext-unicore-2.0.0/tvbextunicore/labextension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:11:34.139064 tvb-ext-unicore-2.0.0/tvbextunicore/labextension/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     9865 2024-04-05 20:11:33.000000 tvb-ext-unicore-2.0.0/tvbextunicore/labextension/static/747.0bb902cd31ab1b8a32cc.js
+-rw-r--r--   0 runner    (1001) docker     (127)    17484 2024-04-05 20:11:33.000000 tvb-ext-unicore-2.0.0/tvbextunicore/labextension/static/774.96299c03c320cee66d47.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7018 2024-04-05 20:11:33.000000 tvb-ext-unicore-2.0.0/tvbextunicore/labextension/static/remoteEntry.15eb2e0bc97996deb062.js
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-05 20:11:32.000000 tvb-ext-unicore-2.0.0/tvbextunicore/labextension/static/style.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-05 20:11:33.000000 tvb-ext-unicore-2.0.0/tvbextunicore/labextension/static/third-party-licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:11:34.143064 tvb-ext-unicore-2.0.0/tvbextunicore/logger/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 20:10:20.000000 tvb-ext-unicore-2.0.0/tvbextunicore/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-05 20:10:20.000000 tvb-ext-unicore-2.0.0/tvbextunicore/logger/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-05 20:10:20.000000 tvb-ext-unicore-2.0.0/tvbextunicore/logger/logging.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:11:34.143064 tvb-ext-unicore-2.0.0/tvbextunicore/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 20:10:20.000000 tvb-ext-unicore-2.0.0/tvbextunicore/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7416 2024-04-05 20:10:20.000000 tvb-ext-unicore-2.0.0/tvbextunicore/tests/test_unicore_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:11:34.143064 tvb-ext-unicore-2.0.0/tvbextunicore/unicore_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 20:10:20.000000 tvb-ext-unicore-2.0.0/tvbextunicore/unicore_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-04-05 20:10:20.000000 tvb-ext-unicore-2.0.0/tvbextunicore/unicore_wrapper/job_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7132 2024-04-05 20:10:20.000000 tvb-ext-unicore-2.0.0/tvbextunicore/unicore_wrapper/unicore_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-05 20:10:20.000000 tvb-ext-unicore-2.0.0/tvbextunicore/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)   372706 2024-04-05 20:10:20.000000 tvb-ext-unicore-2.0.0/yarn.lock
```

### Comparing `tvb-ext-unicore-1.2.0/LICENSE` & `tvb-ext-unicore-2.0.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 GNU General Public License v3.0 or later
 -------------------------------------------------------------------
 TVB-EXT-UNICORE
 
-Copyright (C) 2022 TVB Widgets Team
+Copyright (C) 2022-2024 TVB Widgets Team
 
 This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 
 This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 
 A copy of the GNU General Public License is put bellow. For more details see <https://www.gnu.org/licenses/>.
```

### Comparing `tvb-ext-unicore-1.2.0/MANIFEST.in` & `tvb-ext-unicore-2.0.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `tvb-ext-unicore-1.2.0/PKG-INFO` & `tvb-ext-unicore-2.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tvb-ext-unicore
-Version: 1.2.0
+Version: 2.0.0
 Summary: TVB Widgets - A Unicore Lab extension
 Home-page: https://github.com/the-virtual-brain/tvb-ext-unicore
 Author: TVB Widgets Team
 Author-email: tvb.admin@thevirtualbrain.org
 License: GPL-3.0-or-later
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
@@ -20,14 +20,16 @@
 Classifier: Framework :: Jupyter :: JupyterLab
 Classifier: Framework :: Jupyter :: JupyterLab :: 3
 Classifier: Framework :: Jupyter :: JupyterLab :: Extensions
 Classifier: Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: jupyter_server
+Requires-Dist: pyunicore>=1.0
 
 # tvb-ext-unicore
 
 [![Github Actions Status](https://github.com/the-virtual-brain/tvb-ext-unicore/workflows/Build/badge.svg)](https://github.com/the-virtual-brain/tvb-ext-unicore/actions/workflows/build.yml) [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=the-virtual-brain_tvb-ext-unicore&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=the-virtual-brain_tvb-ext-unicore) [![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=the-virtual-brain_tvb-ext-unicore&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=the-virtual-brain_tvb-ext-unicore)
  [![Lines of Code](https://sonarcloud.io/api/project_badges/measure?project=the-virtual-brain_tvb-ext-unicore&metric=ncloc)](https://sonarcloud.io/summary/new_code?id=the-virtual-brain_tvb-ext-unicore)
 
 
@@ -149,7 +151,9 @@
 In development mode, you will also need to remove the symlink created by `jupyter labextension develop`
 command. To find its location, you can run `jupyter labextension list` to figure out where the `labextensions`
 folder is located. Then you can remove the symlink named `tvb-ext-unicore` within that folder.
 
 ### Acknowledgments
 
 This project has received funding from the European Union’s Horizon 2020 Framework Programme for Research and Innovation under the Specific Grant Agreement No. 945539 (Human Brain Project SGA3).
+
+This project has received funding from the European Union’s Horizon Europe Programme under the Specific Grant Agreement No. 101147319 (EBRAINS 2.0 Project).
```

### Comparing `tvb-ext-unicore-1.2.0/README.md` & `tvb-ext-unicore-2.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -122,7 +122,9 @@
 In development mode, you will also need to remove the symlink created by `jupyter labextension develop`
 command. To find its location, you can run `jupyter labextension list` to figure out where the `labextensions`
 folder is located. Then you can remove the symlink named `tvb-ext-unicore` within that folder.
 
 ### Acknowledgments
 
 This project has received funding from the European Union’s Horizon 2020 Framework Programme for Research and Innovation under the Specific Grant Agreement No. 945539 (Human Brain Project SGA3).
+
+This project has received funding from the European Union’s Horizon Europe Programme under the Specific Grant Agreement No. 101147319 (EBRAINS 2.0 Project).
```

### Comparing `tvb-ext-unicore-1.2.0/RELEASE.md` & `tvb-ext-unicore-2.0.0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `tvb-ext-unicore-1.2.0/jest.config.js` & `tvb-ext-unicore-2.0.0/jest.config.js`

 * *Files identical despite different names*

### Comparing `tvb-ext-unicore-1.2.0/package.json` & `tvb-ext-unicore-2.0.0/package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9642857142857143%*

 * *Differences: {"'bugs'": "{'url': 'https://tvb-projects.atlassian.net/'}", "'version'": "'2.0.0'"}*

```diff
@@ -1,14 +1,14 @@
 {
     "author": {
         "email": "tvb.admin@thevirtualbrain.org",
         "name": "TVB Widgets Team"
     },
     "bugs": {
-        "url": "https://req.thevirtualbrain.org/"
+        "url": "https://tvb-projects.atlassian.net/"
     },
     "dependencies": {
         "@jupyterlab/application": "^3.2.9",
         "@jupyterlab/apputils": "^3.3.0",
         "@jupyterlab/console": "^3.3.0",
         "@jupyterlab/coreutils": "^5.1.0",
         "@jupyterlab/services": "^6.1.0",
@@ -100,9 +100,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "1.2.0"
+    "version": "2.0.0"
 }
```

### Comparing `tvb-ext-unicore-1.2.0/pyproject.toml` & `tvb-ext-unicore-2.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tvb-ext-unicore-1.2.0/setup.py` & `tvb-ext-unicore-2.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # "TheVirtualBrain - Widgets" package
 #
-# (c) 2022-2023, TVB Widgets Team
+# (c) 2022-2024, TVB Widgets Team
 #
 
 import json
 import sys
 import setuptools
 from pathlib import Path
 
@@ -54,15 +54,15 @@
     license=pkg_json["license"],
     license_file="LICENSE",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     install_requires=[
         "jupyter_server",
-        "pyunicore >= 0.11.1"
+        "pyunicore >= 1.0"
     ],
     zip_safe=False,
     include_package_data=True,
     python_requires=">=3.6",
     platforms="Linux, Mac OS X, Windows",
     keywords=["Jupyter", "JupyterLab", "JupyterLab3"],
     classifiers=[
```

### Comparing `tvb-ext-unicore-1.2.0/sonar-project.properties` & `tvb-ext-unicore-2.0.0/sonar-project.properties`

 * *Files identical despite different names*

### Comparing `tvb-ext-unicore-1.2.0/src/__tests__/JobOutputFiles.test.tsx` & `tvb-ext-unicore-2.0.0/src/__tests__/JobOutputFiles.test.tsx`

 * *Files identical despite different names*

### Comparing `tvb-ext-unicore-1.2.0/src/__tests__/ModalComponent.test.tsx` & `tvb-ext-unicore-2.0.0/src/__tests__/ModalComponent.test.tsx`

 * *Files identical despite different names*

### Comparing `tvb-ext-unicore-1.2.0/src/__tests__/PaginationComponent.test.tsx` & `tvb-ext-unicore-2.0.0/src/__tests__/PaginationComponent.test.tsx`

 * *Files identical despite different names*

### Comparing `tvb-ext-unicore-1.2.0/src/__tests__/SideButton.test.tsx` & `tvb-ext-unicore-2.0.0/src/__tests__/SideButton.test.tsx`

 * *Files identical despite different names*

### Comparing `tvb-ext-unicore-1.2.0/src/__tests__/UnicoreJobsTable.test.tsx` & `tvb-ext-unicore-2.0.0/src/__tests__/UnicoreJobsTable.test.tsx`

 * *Files identical despite different names*

### Comparing `tvb-ext-unicore-1.2.0/src/__tests__/UnicoreSites.test.tsx` & `tvb-ext-unicore-2.0.0/src/__tests__/UnicoreSites.test.tsx`

 * *Files identical despite different names*

### Comparing `tvb-ext-unicore-1.2.0/src/__tests__/constants.tests.tsx` & `tvb-ext-unicore-2.0.0/src/__tests__/constants.tests.tsx`

 * *Files identical despite different names*

### Comparing `tvb-ext-unicore-1.2.0/src/__tests__/pyunicoreWidget.test.tsx` & `tvb-ext-unicore-2.0.0/src/__tests__/pyunicoreWidget.test.tsx`

 * *Files identical despite different names*

### Comparing `tvb-ext-unicore-1.2.0/src/__tests__/utils.test.ts` & `tvb-ext-unicore-2.0.0/src/__tests__/utils.test.ts`

 * *Files identical despite different names*

### Comparing `tvb-ext-unicore-1.2.0/src/components/CheckBoxToggle.tsx` & `tvb-ext-unicore-2.0.0/src/components/CheckBoxToggle.tsx`

 * *Files identical despite different names*

### Comparing `tvb-ext-unicore-1.2.0/src/components/JobOutputFiles.tsx` & `tvb-ext-unicore-2.0.0/src/components/JobOutputFiles.tsx`

 * *Files 2% similar despite different names*

```diff
@@ -249,14 +249,20 @@
               <span className={'unicoreLoading'} />
             </div>
           ) : (
             <i
               data-testid={'download-file'}
               className={'fa fa-download clickableIcon'}
               onClick={() => downloadToCurrentPath(output)}
+              onKeyDown={event => {
+                if (event.key === 'Enter') {
+                  downloadToCurrentPath(output);
+                }
+              }}
+              tabIndex={0}
             />
           )}
         </>
       )}
     </div>
   );
 };
```

### Comparing `tvb-ext-unicore-1.2.0/src/components/ModalComponent.tsx` & `tvb-ext-unicore-2.0.0/src/components/ModalComponent.tsx`

 * *Files identical despite different names*

### Comparing `tvb-ext-unicore-1.2.0/src/components/PaginationComponent.tsx` & `tvb-ext-unicore-2.0.0/src/components/PaginationComponent.tsx`

 * *Files identical despite different names*

### Comparing `tvb-ext-unicore-1.2.0/src/components/SideButton.ts` & `tvb-ext-unicore-2.0.0/src/components/SideButton.ts`

 * *Files identical despite different names*

### Comparing `tvb-ext-unicore-1.2.0/src/components/UnicoreJobsTable.tsx` & `tvb-ext-unicore-2.0.0/src/components/UnicoreJobsTable.tsx`

 * *Files identical despite different names*

### Comparing `tvb-ext-unicore-1.2.0/src/components/UnicoreSites.tsx` & `tvb-ext-unicore-2.0.0/src/components/UnicoreSites.tsx`

 * *Files identical despite different names*

### Comparing `tvb-ext-unicore-1.2.0/src/constants.ts` & `tvb-ext-unicore-2.0.0/src/constants.ts`

 * *Files identical despite different names*

### Comparing `tvb-ext-unicore-1.2.0/src/handler.ts` & `tvb-ext-unicore-2.0.0/src/handler.ts`

 * *Files identical despite different names*

### Comparing `tvb-ext-unicore-1.2.0/src/index.ts` & `tvb-ext-unicore-2.0.0/src/index.ts`

 * *Files identical despite different names*

### Comparing `tvb-ext-unicore-1.2.0/src/pyunicoreWidget.tsx` & `tvb-ext-unicore-2.0.0/src/pyunicoreWidget.tsx`

 * *Files 14% similar despite different names*

```diff
@@ -168,105 +168,106 @@
 
   /**
    * method to fetch data from api and toggle pagination buttons, sites, loading wheel,
    * before and after data loads
    * @protected
    */
   protected async getData(): Promise<void> {
-    this.setState({
-      ...this.state,
+    this.setState(prevState => ({
+      ...prevState,
       loading: true,
       renderLeftArrow: false,
       renderRightArrow: false,
       disableSitesSelection: true
-    });
+    }));
     const data = await requestAPI<any>(this._getEndpoint());
 
-    this.setState({
-      ...this.state,
+    this.setState(prevState => ({
+      ...prevState,
       jobs: data.jobs,
       message: data.message,
       loading: false,
       lastUpdate: new Date(),
-      renderLeftArrow: this.state.page > 1,
-      renderRightArrow: data.jobs.length >= this.state.itemsPerPage,
+      renderLeftArrow: prevState.page > 1,
+      renderRightArrow: data.jobs.length >= prevState.itemsPerPage,
       disableSitesSelection: false,
       isRefresh: false
-    });
+    }));
 
     return data;
   }
 
   /**
    * Main function that triggers an update of the jobs from current site
    * @param ignoreRefreshRate - if true will ignore how much time has passed since last update
    */
   private _triggerUpdate = (ignoreRefreshRate = false): void => {
     if (this.state.site === NO_SITE) {
       return;
     }
     if (ignoreRefreshRate) {
-      this.setState({ ...this.state, isRefresh: true });
+      this.setState(prevState => ({ ...prevState, isRefresh: true }));
       return;
     } else if (!this.state.autoReload) {
       return;
     }
     const now = new Date().valueOf();
     const previous = this.state.lastUpdate.valueOf();
     const diff = now - previous;
     if (diff >= this.state.reloadRate && !this.state.loading) {
-      this.setState({ ...this.state, isRefresh: true });
+      this.setState(prevState => ({ ...prevState, isRefresh: true }));
     }
   };
 
   /**
    * helper method to set page state from a child component
    * @param page
    * @protected
    */
   protected setPageState(page: number): void {
-    this.setState({ ...this.state, page: page });
+    this.setState(prevState => ({ ...prevState, page: page }));
   }
 
   /**
    * helper method to set modal visibility from modal component
    * @param visible
    * @protected
    */
   protected setModalSateVisible(visible: boolean): void {
-    this.setState({
-      ...this.state,
+    this.setState(prevState => ({
+      ...prevState,
       loading: false,
       renderLeftArrow: true,
       renderRightArrow: true,
       disableSitesSelection: false,
-      modalState: { ...this.state.modalState, visible: visible }
-    });
+      modalState: { ...prevState.modalState, visible: visible }
+    }));
   }
   /**
    * helper method to set site state from a child component
    * @param site
    * @protected
    */
   protected setSiteState(site: string): void {
     // reset the page to 1 when changing site
-    let jobs = this.state.jobs;
-    if (site === NO_SITE) {
-      jobs = [];
-    }
-    this.setState({ ...this.state, page: 1, site: site, jobs: jobs });
+    this.setState(prevState => ({
+      ...prevState,
+      page: 1,
+      site: site,
+      jobs: site === NO_SITE ? [] : prevState.jobs
+    }));
   }
 
   /**
    * Method to set state of auto update functionality
    * @param active - active state of the reload functionality
    * @protected
    */
   protected setAutoReload(active: boolean): void {
-    this.setState({ ...this.state, autoReload: active });
+    this.setState(prevState => ({ ...prevState, autoReload: active }));
   }
 
   /**
    * if page or site changed reload data
    * @param _prevProps
    * @param prevState
    */
@@ -277,43 +278,43 @@
     if (
       ((this.state.isRefresh && !prevState.isRefresh) ||
         prevState.page !== this.state.page ||
         prevState.site !== this.state.site) &&
       this.state.sites.length > 0
     ) {
       if (this.state.site === NO_SITE) {
-        this.setState({
-          ...this.state,
+        this.setState(prevState => ({
+          ...prevState,
           loading: false,
           disableSitesSelection: false,
           jobs: [],
           renderLeftArrow: false,
           renderRightArrow: false,
           isRefresh: false
-        });
+        }));
         return;
       }
       this.getData().catch(this.catchError);
     }
   }
 
   /**
    * helper function to catch an error and update the state to show modal with error
    * @param reason
    * @private
    */
   private catchError(reason?: any): void {
-    this.setState({
-      ...this.state,
+    this.setState(prevState => ({
+      ...prevState,
       modalState: {
-        ...this.state.modalState,
+        ...prevState.modalState,
         visible: true,
         message: reason
       }
-    });
+    }));
   }
   /**
    * clear interval to avoid unnecessary reloads
    */
   componentWillUnmount(): void {
     clearInterval(this.state.updateIntervalId);
   }
@@ -325,19 +326,19 @@
     // TODO: Try to replace with setTimeout
     const updateIntervalId = setInterval(
       this._triggerUpdate,
       RELOAD_CHECK_RATE_MS
     );
     this.setState({ ...this.state, updateIntervalId: updateIntervalId });
     if (this.state.site === NO_SITE) {
-      this.setState({
-        ...this.state,
+      this.setState(prevState => ({
+        ...prevState,
         loading: false,
         disableSitesSelection: false
-      });
+      }));
       return;
     }
     if (this.state.sites.length <= 0) {
       return;
     }
     this.getData().catch(this.catchError);
   }
@@ -388,15 +389,15 @@
 
         <UnicoreJobsTable
           buttonSettings={this.state.buttonSettings}
           afterButtonSettingClick={this.getData}
           columns={this.state.tableFormat.cols}
           data={this.state.jobs}
           setMessageState={(message: string) => {
-            this.setState({ ...this.state, message: message });
+            this.setState(prevState => ({ ...prevState, message: message }));
           }}
           getKernel={this.props.getKernel}
           getJob={this.props.getJobCode}
           handleError={this.catchError}
           getFileBrowser={this.props.getFileBrowser}
         />
       </>
```

### Comparing `tvb-ext-unicore-1.2.0/src/utils.ts` & `tvb-ext-unicore-2.0.0/src/utils.ts`

 * *Files identical despite different names*

### Comparing `tvb-ext-unicore-1.2.0/style/base.css` & `tvb-ext-unicore-2.0.0/style/base.css`

 * *Files 5% similar despite different names*

```diff
@@ -303,10 +303,15 @@
     display: inline-block;
 }
 
 .clickableIcon {
     cursor: pointer;
 }
 
+.clickableIcon:focus {
+    outline: #2b2b2c solid 2px;
+    outline-offset: 2px;
+}
+
 i {
     color: var(--jp-content-font-color2);
 }
```

### Comparing `tvb-ext-unicore-1.2.0/style/icons/logo-unicore.svg` & `tvb-ext-unicore-2.0.0/style/icons/logo-unicore.svg`

 * *Files identical despite different names*

### Comparing `tvb-ext-unicore-1.2.0/style/variables.css` & `tvb-ext-unicore-2.0.0/style/variables.css`

 * *Files identical despite different names*

### Comparing `tvb-ext-unicore-1.2.0/tsconfig.json` & `tvb-ext-unicore-2.0.0/tsconfig.json`

 * *Files identical despite different names*

### Comparing `tvb-ext-unicore-1.2.0/tvb_ext_unicore.egg-info/PKG-INFO` & `tvb-ext-unicore-2.0.0/tvb_ext_unicore.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tvb-ext-unicore
-Version: 1.2.0
+Version: 2.0.0
 Summary: TVB Widgets - A Unicore Lab extension
 Home-page: https://github.com/the-virtual-brain/tvb-ext-unicore
 Author: TVB Widgets Team
 Author-email: tvb.admin@thevirtualbrain.org
 License: GPL-3.0-or-later
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
@@ -20,14 +20,16 @@
 Classifier: Framework :: Jupyter :: JupyterLab
 Classifier: Framework :: Jupyter :: JupyterLab :: 3
 Classifier: Framework :: Jupyter :: JupyterLab :: Extensions
 Classifier: Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: jupyter_server
+Requires-Dist: pyunicore>=1.0
 
 # tvb-ext-unicore
 
 [![Github Actions Status](https://github.com/the-virtual-brain/tvb-ext-unicore/workflows/Build/badge.svg)](https://github.com/the-virtual-brain/tvb-ext-unicore/actions/workflows/build.yml) [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=the-virtual-brain_tvb-ext-unicore&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=the-virtual-brain_tvb-ext-unicore) [![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=the-virtual-brain_tvb-ext-unicore&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=the-virtual-brain_tvb-ext-unicore)
  [![Lines of Code](https://sonarcloud.io/api/project_badges/measure?project=the-virtual-brain_tvb-ext-unicore&metric=ncloc)](https://sonarcloud.io/summary/new_code?id=the-virtual-brain_tvb-ext-unicore)
 
 
@@ -149,7 +151,9 @@
 In development mode, you will also need to remove the symlink created by `jupyter labextension develop`
 command. To find its location, you can run `jupyter labextension list` to figure out where the `labextensions`
 folder is located. Then you can remove the symlink named `tvb-ext-unicore` within that folder.
 
 ### Acknowledgments
 
 This project has received funding from the European Union’s Horizon 2020 Framework Programme for Research and Innovation under the Specific Grant Agreement No. 945539 (Human Brain Project SGA3).
+
+This project has received funding from the European Union’s Horizon Europe Programme under the Specific Grant Agreement No. 101147319 (EBRAINS 2.0 Project).
```

### Comparing `tvb-ext-unicore-1.2.0/tvb_ext_unicore.egg-info/SOURCES.txt` & `tvb-ext-unicore-2.0.0/tvb_ext_unicore.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -50,17 +50,17 @@
 tvb_ext_unicore.egg-info/top_level.txt
 tvbextunicore/__init__.py
 tvbextunicore/_version.py
 tvbextunicore/exceptions.py
 tvbextunicore/handlers.py
 tvbextunicore/utils.py
 tvbextunicore/labextension/package.json
-tvbextunicore/labextension/static/747.c26c9bf4f7bddc1ea1c7.js
-tvbextunicore/labextension/static/774.f5b7ad80ab759770978c.js
-tvbextunicore/labextension/static/remoteEntry.c6b3242597cbbe03a95e.js
+tvbextunicore/labextension/static/747.0bb902cd31ab1b8a32cc.js
+tvbextunicore/labextension/static/774.96299c03c320cee66d47.js
+tvbextunicore/labextension/static/remoteEntry.15eb2e0bc97996deb062.js
 tvbextunicore/labextension/static/style.js
 tvbextunicore/labextension/static/third-party-licenses.json
 tvbextunicore/logger/__init__.py
 tvbextunicore/logger/builder.py
 tvbextunicore/logger/logging.conf
 tvbextunicore/tests/__init__.py
 tvbextunicore/tests/test_unicore_wrapper.py
```

### Comparing `tvb-ext-unicore-1.2.0/tvbextunicore/__init__.py` & `tvb-ext-unicore-2.0.0/tvbextunicore/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-ext-unicore-1.2.0/tvbextunicore/_version.py` & `tvb-ext-unicore-2.0.0/tvbextunicore/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # "TheVirtualBrain - Widgets" package
 #
-# (c) 2022-2023, TVB Widgets Team
+# (c) 2022-2024, TVB Widgets Team
 #
 
 import json
 from pathlib import Path
 
 __all__ = ["__version__"]
```

### Comparing `tvb-ext-unicore-1.2.0/tvbextunicore/exceptions.py` & `tvb-ext-unicore-2.0.0/tvbextunicore/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # "TheVirtualBrain - Widgets" package
 #
-# (c) 2022-2023, TVB Widgets Team
+# (c) 2022-2024, TVB Widgets Team
 #
 
 class TVBExtUnicoreException(Exception):
 
     def __init__(self, message):
         super().__init__(message)
         self.message = str(message)
```

### Comparing `tvb-ext-unicore-1.2.0/tvbextunicore/handlers.py` & `tvb-ext-unicore-2.0.0/tvbextunicore/handlers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # "TheVirtualBrain - Widgets" package
 #
-# (c) 2022-2023, TVB Widgets Team
+# (c) 2022-2024, TVB Widgets Team
 #
 
 import os
 import json
 
 from jupyter_server.base.handlers import APIHandler
 from jupyter_server.utils import url_path_join
```

### Comparing `tvb-ext-unicore-1.2.0/tvbextunicore/labextension/package.json` & `tvb-ext-unicore-2.0.0/tvbextunicore/labextension/package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9637896825396824%*

 * *Differences: {"'bugs'": "{'url': 'https://tvb-projects.atlassian.net/'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.15eb2e0bc97996deb062.js'}}",*

 * * "'version'": "'2.0.0'"}*

```diff
@@ -1,14 +1,14 @@
 {
     "author": {
         "email": "tvb.admin@thevirtualbrain.org",
         "name": "TVB Widgets Team"
     },
     "bugs": {
-        "url": "https://req.thevirtualbrain.org/"
+        "url": "https://tvb-projects.atlassian.net/"
     },
     "dependencies": {
         "@jupyterlab/application": "^3.2.9",
         "@jupyterlab/apputils": "^3.3.0",
         "@jupyterlab/console": "^3.3.0",
         "@jupyterlab/coreutils": "^5.1.0",
         "@jupyterlab/services": "^6.1.0",
@@ -48,15 +48,15 @@
                 "jlpm"
             ]
         }
     },
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.c6b3242597cbbe03a95e.js",
+            "load": "static/remoteEntry.15eb2e0bc97996deb062.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "tvb-ext-unicore"
                 },
@@ -105,9 +105,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "1.2.0"
+    "version": "2.0.0"
 }
```

### Comparing `tvb-ext-unicore-1.2.0/tvbextunicore/labextension/static/747.c26c9bf4f7bddc1ea1c7.js` & `tvb-ext-unicore-2.0.0/tvbextunicore/labextension/static/747.0bb902cd31ab1b8a32cc.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -5,15 +5,15 @@
             r.d(e, {
                 Z: () => i
             });
             var o = r(645),
                 t = r.n(o)()((function(n) {
                     return n[1]
                 }));
-            t.push([n.id, ".tvb-pyunicoreWidget {\n    background-color: whitesmoke;\n    font-family: var(--jp-ui-font-family);\n    max-height: 100vh;\n    overflow-y: auto;\n    overflow-x: hidden;\n}\n\n.tvb-pyunicoreWidget > div {\n    margin-top: 0.2rem;\n}\n\n.tvb-pyunicoreWidget table {\n    width: 100%;\n    border: var(--jp-border-width) solid black;\n    border-collapse: collapse;\n    background-color: white;\n    color: black;\n    text-align: center;\n    vertical-align: middle;\n    overflow: hidden;\n}\n\n.tvb-pyunicoreWidget tr {\n    border-bottom: 1px solid black;\n}\n\n/* hint that table rows that aren't with details are clickable */\n.tvb-pyunicoreWidget tbody tr:not(.detailsRow) {\n    cursor: pointer;\n}\n.tvb-pyunicoreWidget tbody tr:not(.detailsRow):hover {\n    box-shadow: 0 0 7px 0 rgba(0, 0, 0, 0.2);\n}\n\n.tvb-pyunicoreWidget tbody tr:nth-child(even) {\n    background-color: whitesmoke;\n}\n\n.tvb-pyunicoreWidget td, th {\n    padding: 8px;\n}\n\n.tvb-pyunicoreWidget table, body {\n    font-family: var(--jp-ui-font-family);\n}\n\n.tvb-pyunicoreWidget thead {\n    background-color: lightgray;\n    text-transform: uppercase;\n}\n\n.tvb-pyunicoreWidget button {\n    padding: 8px 16px;\n    border: 1px solid black;\n    border-radius: 7px;\n    background-color: white;\n    color: black;\n}\n\n.tvb-pyunicoreWidget button:hover {\n    box-shadow: 0 12px 16px 0 rgba(0,0,0,0.24), 0 17px 50px 0 rgba(0,0,0,0.19);\n    cursor: pointer;\n}\n/**\ntop bar style\n */\n.unicoreTopBar {\n    display: flex;\n    flex-direction: row;\n    align-items: center;\n    justify-content: flex-start;\n    padding-bottom: 0.2rem;\n}\n/* end top bar */\n.lastUpdate {\n    margin-left: 1rem;\n}\n/**\ndetails section style\n */\n.tvb-pyunicoreWidget .detailsRow td {\n    column-span: all;\n    padding-top: 0;\n    padding-bottom: 0;\n    padding-right: 0;\n    width: 100%;\n}\n.tvb-pyunicoreWidget .detailsRow textarea {\n    width: 100%;\n    height: 10rem;\n    border: none;\n}\n/* end details section style */\n\n/**\nselection component (pyunicore sites)\n */\n.pyunicoreSites {\n    display: flex;\n    flex-direction: row;\n    margin: 0 1rem 0 0 ;\n}\n\n@-moz-keyframes spin {\n    from { -moz-transform: rotate(0deg); }\n    to { -moz-transform: rotate(360deg); }\n}\n@-webkit-keyframes spin {\n    from { -webkit-transform: rotate(0deg); }\n    to { -webkit-transform: rotate(360deg); }\n}\n@keyframes spin {\n    from {transform:rotate(0deg);}\n    to {transform:rotate(360deg);}\n}\n\n.spin {\n    -webkit-animation: spin 1s infinite linear;\n    animation: spin 0.5s infinite linear;\n}\n\n.pyunicoreSites .refreshBtn {\n    border: none;\n    padding: 5px;\n    background: none;\n}\n.pyunicoreSites div{\n    border: var(--jp-border-width) solid var(--jp-border-color1);\n    border-radius: 7px;\n    padding: 0.2rem;\n    display: flex;\n    align-items: center;\n    justify-content: center;\n}\n.pyunicoreSites select {\n    background-color: whitesmoke;\n    border: none;\n}\n.pyunicoreSites span {\n    text-transform: uppercase;\n    font-weight: bold;\n    margin-left: 1rem;\n}\n/* end selection style */\n\n/* modal styling */\n.unicoreModal {\n    position: absolute;\n    background-color: rgba(0,0,0,0.2);\n    width: 100%;\n    height: 100%;\n    z-index: 5;\n    top: 0;\n    left: 0;\n    display: flex;\n    align-items: center;\n    justify-content: center;\n}\n\n.unicoreModal > div {\n    width: 40%;\n    min-height: 5rem;\n    background-color: whitesmoke;\n    border-radius: 7px;\n    /*padding: 1rem;*/\n    box-shadow: 0 0 10px 0 rgba(185,185,185, .4);\n}\n.unicoreModal > div h3 {\n    padding: 0;\n    margin: 0;\n}\n\n.unicoreModal > div > div:first-child {\n    background-color: var(--jp-error-color1);\n    border-radius: 7px 7px 0 0;\n    color: whitesmoke;\n}\n.unicoreModal > div > div {\n    padding: 1rem;\n    margin: 0;\n}\n\n.unicoreModal button {\n    background-color: var(--jp-error-color1);\n    color: whitesmoke;\n    padding: 0.5rem 1rem;\n    border-radius: 7px;\n    border: none;\n    box-shadow: 0 0 7px 0 rgba(185,185,185, .4);\n    cursor: pointer;\n}\n\n.unicoreModal button:hover {\n    box-shadow: 0 0 14px 0 rgba(0,0,0, .4);\n}\n/* end modal style */\n\n/* loading animation */\n@keyframes circle{\n  0%{\n    transform:rotate(0deg);\n  }\n  100%{\n    transform:rotate(360deg);\n  }\n}\n.loadingRoot {\n    display: flex;\n    align-items: center;\n    justify-content: center;\n}\n\n\n.unicoreLoading {\n    width: 0.9rem;\n    height: 0.9rem;\n    display: inline-block;\n    border-radius: 50%;\n    border: 3px solid var(--jp-border-color1);\n    border-top: 3px solid var(--jp-cell-editor-active-border-color);\n    animation: circle 0.5s linear infinite;\n}\n\n.unicoreMessage {\n    color: var(--jp-error-color1);\n}\n\n.unicoreMessage-success {\n    color: var(--jp-success-color1);\n}\n\n.unicoreMessage-warning {\n    color: var(--jp-warn-color1);\n}\n\n/**\npagination style\n */\n.unicorePagination {\n    display: inline-block;\n    border: var(--jp-border-width) solid var(--jp-border-color1);\n    border-radius: 7px;\n    margin-right: 1rem;\n    /*margin-left: 0.5rem;*/\n}\n.unicorePagination div{\n    display: flex;\n    flex-direction: row;\n    align-items: center;\n    justify-content: center;\n}\n.unicorePagination > div div {\n    min-width: 1rem;\n    padding: 0.2rem;\n    height: 100%;\n}\n.unicorePagination button {\n    padding: 0;\n    border: none;\n    margin: 0;\n    display: flex;\n    align-items: center;\n    justify-content: center;\n    background-color: whitesmoke;\n    color: var(--jp-border-color1);\n}\n\nbutton:disabled,\nbutton[disabled]{\n    color: #ababab;\n    box-shadow: none;\n}\n\nbutton:disabled:hover,\nbutton[disabled]:hover {\n    box-shadow: none;\n    cursor: initial;\n}\n\n.currentPageContainer {\n    border-left: var(--jp-border-width) solid var(--jp-border-color1);\n    border-right: var(--jp-border-width) solid var(--jp-border-color1);\n    padding: 0 0.2rem;\n}\n\n\n/*----- output files -----*/\n.unicore-jobOutput {\n    display: flex;\n    flex-direction: row;\n    height: 1.3rem;\n    align-items: center;\n    margin: 0.1rem 0;\n}\n\n.outputFiles {\n    text-align: left;\n}\n\n.outputFileName {\n    margin: 0 0.5rem 0 0.2rem;\n    display: inline-block;\n}\n\n.clickableIcon {\n    cursor: pointer;\n}\n\ni {\n    color: var(--jp-content-font-color2);\n}", ""]);
+            t.push([n.id, ".tvb-pyunicoreWidget {\n    background-color: whitesmoke;\n    font-family: var(--jp-ui-font-family);\n    max-height: 100vh;\n    overflow-y: auto;\n    overflow-x: hidden;\n}\n\n.tvb-pyunicoreWidget > div {\n    margin-top: 0.2rem;\n}\n\n.tvb-pyunicoreWidget table {\n    width: 100%;\n    border: var(--jp-border-width) solid black;\n    border-collapse: collapse;\n    background-color: white;\n    color: black;\n    text-align: center;\n    vertical-align: middle;\n    overflow: hidden;\n}\n\n.tvb-pyunicoreWidget tr {\n    border-bottom: 1px solid black;\n}\n\n/* hint that table rows that aren't with details are clickable */\n.tvb-pyunicoreWidget tbody tr:not(.detailsRow) {\n    cursor: pointer;\n}\n.tvb-pyunicoreWidget tbody tr:not(.detailsRow):hover {\n    box-shadow: 0 0 7px 0 rgba(0, 0, 0, 0.2);\n}\n\n.tvb-pyunicoreWidget tbody tr:nth-child(even) {\n    background-color: whitesmoke;\n}\n\n.tvb-pyunicoreWidget td, th {\n    padding: 8px;\n}\n\n.tvb-pyunicoreWidget table, body {\n    font-family: var(--jp-ui-font-family);\n}\n\n.tvb-pyunicoreWidget thead {\n    background-color: lightgray;\n    text-transform: uppercase;\n}\n\n.tvb-pyunicoreWidget button {\n    padding: 8px 16px;\n    border: 1px solid black;\n    border-radius: 7px;\n    background-color: white;\n    color: black;\n}\n\n.tvb-pyunicoreWidget button:hover {\n    box-shadow: 0 12px 16px 0 rgba(0,0,0,0.24), 0 17px 50px 0 rgba(0,0,0,0.19);\n    cursor: pointer;\n}\n/**\ntop bar style\n */\n.unicoreTopBar {\n    display: flex;\n    flex-direction: row;\n    align-items: center;\n    justify-content: flex-start;\n    padding-bottom: 0.2rem;\n}\n/* end top bar */\n.lastUpdate {\n    margin-left: 1rem;\n}\n/**\ndetails section style\n */\n.tvb-pyunicoreWidget .detailsRow td {\n    column-span: all;\n    padding-top: 0;\n    padding-bottom: 0;\n    padding-right: 0;\n    width: 100%;\n}\n.tvb-pyunicoreWidget .detailsRow textarea {\n    width: 100%;\n    height: 10rem;\n    border: none;\n}\n/* end details section style */\n\n/**\nselection component (pyunicore sites)\n */\n.pyunicoreSites {\n    display: flex;\n    flex-direction: row;\n    margin: 0 1rem 0 0 ;\n}\n\n@-moz-keyframes spin {\n    from { -moz-transform: rotate(0deg); }\n    to { -moz-transform: rotate(360deg); }\n}\n@-webkit-keyframes spin {\n    from { -webkit-transform: rotate(0deg); }\n    to { -webkit-transform: rotate(360deg); }\n}\n@keyframes spin {\n    from {transform:rotate(0deg);}\n    to {transform:rotate(360deg);}\n}\n\n.spin {\n    -webkit-animation: spin 1s infinite linear;\n    animation: spin 0.5s infinite linear;\n}\n\n.pyunicoreSites .refreshBtn {\n    border: none;\n    padding: 5px;\n    background: none;\n}\n.pyunicoreSites div{\n    border: var(--jp-border-width) solid var(--jp-border-color1);\n    border-radius: 7px;\n    padding: 0.2rem;\n    display: flex;\n    align-items: center;\n    justify-content: center;\n}\n.pyunicoreSites select {\n    background-color: whitesmoke;\n    border: none;\n}\n.pyunicoreSites span {\n    text-transform: uppercase;\n    font-weight: bold;\n    margin-left: 1rem;\n}\n/* end selection style */\n\n/* modal styling */\n.unicoreModal {\n    position: absolute;\n    background-color: rgba(0,0,0,0.2);\n    width: 100%;\n    height: 100%;\n    z-index: 5;\n    top: 0;\n    left: 0;\n    display: flex;\n    align-items: center;\n    justify-content: center;\n}\n\n.unicoreModal > div {\n    width: 40%;\n    min-height: 5rem;\n    background-color: whitesmoke;\n    border-radius: 7px;\n    /*padding: 1rem;*/\n    box-shadow: 0 0 10px 0 rgba(185,185,185, .4);\n}\n.unicoreModal > div h3 {\n    padding: 0;\n    margin: 0;\n}\n\n.unicoreModal > div > div:first-child {\n    background-color: var(--jp-error-color1);\n    border-radius: 7px 7px 0 0;\n    color: whitesmoke;\n}\n.unicoreModal > div > div {\n    padding: 1rem;\n    margin: 0;\n}\n\n.unicoreModal button {\n    background-color: var(--jp-error-color1);\n    color: whitesmoke;\n    padding: 0.5rem 1rem;\n    border-radius: 7px;\n    border: none;\n    box-shadow: 0 0 7px 0 rgba(185,185,185, .4);\n    cursor: pointer;\n}\n\n.unicoreModal button:hover {\n    box-shadow: 0 0 14px 0 rgba(0,0,0, .4);\n}\n/* end modal style */\n\n/* loading animation */\n@keyframes circle{\n  0%{\n    transform:rotate(0deg);\n  }\n  100%{\n    transform:rotate(360deg);\n  }\n}\n.loadingRoot {\n    display: flex;\n    align-items: center;\n    justify-content: center;\n}\n\n\n.unicoreLoading {\n    width: 0.9rem;\n    height: 0.9rem;\n    display: inline-block;\n    border-radius: 50%;\n    border: 3px solid var(--jp-border-color1);\n    border-top: 3px solid var(--jp-cell-editor-active-border-color);\n    animation: circle 0.5s linear infinite;\n}\n\n.unicoreMessage {\n    color: var(--jp-error-color1);\n}\n\n.unicoreMessage-success {\n    color: var(--jp-success-color1);\n}\n\n.unicoreMessage-warning {\n    color: var(--jp-warn-color1);\n}\n\n/**\npagination style\n */\n.unicorePagination {\n    display: inline-block;\n    border: var(--jp-border-width) solid var(--jp-border-color1);\n    border-radius: 7px;\n    margin-right: 1rem;\n    /*margin-left: 0.5rem;*/\n}\n.unicorePagination div{\n    display: flex;\n    flex-direction: row;\n    align-items: center;\n    justify-content: center;\n}\n.unicorePagination > div div {\n    min-width: 1rem;\n    padding: 0.2rem;\n    height: 100%;\n}\n.unicorePagination button {\n    padding: 0;\n    border: none;\n    margin: 0;\n    display: flex;\n    align-items: center;\n    justify-content: center;\n    background-color: whitesmoke;\n    color: var(--jp-border-color1);\n}\n\nbutton:disabled,\nbutton[disabled]{\n    color: #ababab;\n    box-shadow: none;\n}\n\nbutton:disabled:hover,\nbutton[disabled]:hover {\n    box-shadow: none;\n    cursor: initial;\n}\n\n.currentPageContainer {\n    border-left: var(--jp-border-width) solid var(--jp-border-color1);\n    border-right: var(--jp-border-width) solid var(--jp-border-color1);\n    padding: 0 0.2rem;\n}\n\n\n/*----- output files -----*/\n.unicore-jobOutput {\n    display: flex;\n    flex-direction: row;\n    height: 1.3rem;\n    align-items: center;\n    margin: 0.1rem 0;\n}\n\n.outputFiles {\n    text-align: left;\n}\n\n.outputFileName {\n    margin: 0 0.5rem 0 0.2rem;\n    display: inline-block;\n}\n\n.clickableIcon {\n    cursor: pointer;\n}\n\n.clickableIcon:focus {\n    outline: #2b2b2c solid 2px;\n    outline-offset: 2px;\n}\n\ni {\n    color: var(--jp-content-font-color2);\n}", ""]);
             const i = t
         },
         645: n => {
             n.exports = function(n) {
                 var e = [];
                 return e.toString = function() {
                     return this.map((function(e) {
```

### Comparing `tvb-ext-unicore-1.2.0/tvbextunicore/labextension/static/774.f5b7ad80ab759770978c.js` & `tvb-ext-unicore-2.0.0/tvbextunicore/labextension/static/774.96299c03c320cee66d47.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,30 +1,30 @@
 "use strict";
 (self.webpackChunktvb_ext_unicore = self.webpackChunktvb_ext_unicore || []).push([
     [774], {
         774: (e, t, a) => {
             a.r(t), a.d(t, {
                 default: () => P
             });
-            var s = a(638),
-                n = a(303);
+            var s = a(271),
+                n = a(583);
             const i = "NONE",
                 r = "text/plain";
 
             function o(e) {
                 return `from tvbextunicore.unicore_wrapper import unicore_wrapper\nunicore = unicore_wrapper.UnicoreWrapper()\njob = unicore.get_job('${e}')\njob`
             }
-            var l = a(122),
-                c = a(127),
-                d = a(271),
+            var l = a(83),
+                c = a(854),
+                d = a(918),
                 u = a.n(d),
                 g = a(694),
                 m = a(526),
-                h = a(344),
-                b = a(139);
+                h = a(46),
+                b = a(582);
             async function p(e = "", t = {}) {
                 const a = b.ServerConnection.makeSettings(),
                     s = h.URLExt.join(a.baseUrl, "tvbextunicore", e);
                 let n;
                 console.log("req URL: ", s);
                 try {
                     n = await b.ServerConnection.makeRequest(s, t, a)
@@ -36,15 +36,15 @@
                     i = JSON.parse(i)
                 } catch (e) {
                     console.log("Not a JSON response body.", n)
                 }
                 if (!n.ok) throw new b.ServerConnection.ResponseError(n, i.message || i);
                 return i
             }
-            var S = a(918);
+            var S = a(156);
             const E = e => {
                     const [t, a] = (0, d.useState)(null), [s, n] = (0, d.useState)("");
                     return (0, d.useEffect)((() => {
                         p(`job_output?job_url=${encodeURIComponent(e.job_url)}`).then((e => a(e))).catch((e => {
                             console.log("err: ", e), n(e.message)
                         }))
                     }), []), u().createElement("tr", {
@@ -164,15 +164,19 @@
                     }, b.text), l ? u().createElement("div", {
                         className: "loadingRoot"
                     }, u().createElement("span", {
                         className: "unicoreLoading"
                     })) : u().createElement("i", {
                         "data-testid": "download-file",
                         className: "fa fa-download clickableIcon",
-                        onClick: () => f(t)
+                        onClick: () => f(t),
+                        onKeyDown: e => {
+                            "Enter" === e.key && f(t)
+                        },
+                        tabIndex: 0
                     })))
                 },
                 f = e => u().createElement("table", null, u().createElement(v, {
                     columns: e.columns
                 }), u().createElement(j, {
                     buttonSettings: e.buttonSettings,
                     columns: e.columns,
@@ -348,17 +352,17 @@
                         getFileBrowser: this.props.getFileBrowser
                     })
                 }
             }
             class x extends u().Component {
                 constructor(e) {
                     super(e), this._triggerUpdate = (e = !1) => {
-                        this.state.site !== i && (e || this.state.autoReload && (new Date).valueOf() - this.state.lastUpdate.valueOf() >= this.state.reloadRate && !this.state.loading) && this.setState(Object.assign(Object.assign({}, this.state), {
+                        this.state.site !== i && (e || this.state.autoReload && (new Date).valueOf() - this.state.lastUpdate.valueOf() >= this.state.reloadRate && !this.state.loading) && this.setState((e => Object.assign(Object.assign({}, e), {
                             isRefresh: !0
-                        }))
+                        })))
                     }, this.setPageState = this.setPageState.bind(this), this.setSiteState = this.setSiteState.bind(this), this.setModalSateVisible = this.setModalSateVisible.bind(this), this.getData = this.getData.bind(this), this.catchError = this.catchError.bind(this), this.setAutoReload = this.setAutoReload.bind(this);
                     const t = new Date;
                     this.state = {
                         jobs: [],
                         message: e.data.message,
                         site: e.defaultSite,
                         buttonSettings: e.buttonSettings,
@@ -383,93 +387,92 @@
                         updateIntervalId: 0
                     }
                 }
                 _getEndpoint() {
                     return `jobs?site=${this.state.site}&page=${this.state.page}`
                 }
                 async getData() {
-                    this.setState(Object.assign(Object.assign({}, this.state), {
+                    this.setState((e => Object.assign(Object.assign({}, e), {
                         loading: !0,
                         renderLeftArrow: !1,
                         renderRightArrow: !1,
                         disableSitesSelection: !0
-                    }));
+                    })));
                     const e = await p(this._getEndpoint());
-                    return this.setState(Object.assign(Object.assign({}, this.state), {
+                    return this.setState((t => Object.assign(Object.assign({}, t), {
                         jobs: e.jobs,
                         message: e.message,
                         loading: !1,
                         lastUpdate: new Date,
-                        renderLeftArrow: this.state.page > 1,
-                        renderRightArrow: e.jobs.length >= this.state.itemsPerPage,
+                        renderLeftArrow: t.page > 1,
+                        renderRightArrow: e.jobs.length >= t.itemsPerPage,
                         disableSitesSelection: !1,
                         isRefresh: !1
-                    })), e
+                    }))), e
                 }
                 setPageState(e) {
-                    this.setState(Object.assign(Object.assign({}, this.state), {
+                    this.setState((t => Object.assign(Object.assign({}, t), {
                         page: e
-                    }))
+                    })))
                 }
                 setModalSateVisible(e) {
-                    this.setState(Object.assign(Object.assign({}, this.state), {
+                    this.setState((t => Object.assign(Object.assign({}, t), {
                         loading: !1,
                         renderLeftArrow: !0,
                         renderRightArrow: !0,
                         disableSitesSelection: !1,
-                        modalState: Object.assign(Object.assign({}, this.state.modalState), {
+                        modalState: Object.assign(Object.assign({}, t.modalState), {
                             visible: e
                         })
-                    }))
+                    })))
                 }
                 setSiteState(e) {
-                    let t = this.state.jobs;
-                    e === i && (t = []), this.setState(Object.assign(Object.assign({}, this.state), {
+                    this.setState((t => Object.assign(Object.assign({}, t), {
                         page: 1,
                         site: e,
-                        jobs: t
-                    }))
+                        jobs: e === i ? [] : t.jobs
+                    })))
                 }
                 setAutoReload(e) {
-                    this.setState(Object.assign(Object.assign({}, this.state), {
+                    this.setState((t => Object.assign(Object.assign({}, t), {
                         autoReload: e
-                    }))
+                    })))
                 }
                 componentDidUpdate(e, t) {
                     if ((this.state.isRefresh && !t.isRefresh || t.page !== this.state.page || t.site !== this.state.site) && this.state.sites.length > 0) {
-                        if (this.state.site === i) return void this.setState(Object.assign(Object.assign({}, this.state), {
+                        if (this.state.site === i) return void this.setState((e => Object.assign(Object.assign({}, e), {
                             loading: !1,
                             disableSitesSelection: !1,
                             jobs: [],
                             renderLeftArrow: !1,
                             renderRightArrow: !1,
                             isRefresh: !1
-                        }));
+                        })));
                         this.getData().catch(this.catchError)
                     }
                 }
                 catchError(e) {
-                    this.setState(Object.assign(Object.assign({}, this.state), {
-                        modalState: Object.assign(Object.assign({}, this.state.modalState), {
+                    this.setState((t => Object.assign(Object.assign({}, t), {
+                        modalState: Object.assign(Object.assign({}, t.modalState), {
                             visible: !0,
                             message: e
                         })
-                    }))
+                    })))
                 }
                 componentWillUnmount() {
                     clearInterval(this.state.updateIntervalId)
                 }
                 componentDidMount() {
                     const e = setInterval(this._triggerUpdate, 1e4);
                     this.setState(Object.assign(Object.assign({}, this.state), {
                         updateIntervalId: e
-                    })), this.state.site !== i ? this.state.sites.length <= 0 || this.getData().catch(this.catchError) : this.setState(Object.assign(Object.assign({}, this.state), {
+                    })), this.state.site !== i ? this.state.sites.length <= 0 || this.getData().catch(this.catchError) : this.setState((e => Object.assign(Object.assign({}, e), {
                         loading: !1,
                         disableSitesSelection: !1
-                    }))
+                    })))
                 }
                 render() {
                     return u().createElement(u().Fragment, null, u().createElement(O, {
                         modalType: this.state.modalState.modalType,
                         message: this.state.modalState.message,
                         visible: this.state.modalState.visible,
                         setVisible: this.state.modalState.setVisible
@@ -498,26 +501,26 @@
                         className: "lastUpdate"
                     }, "Last update: ", this.state.lastUpdate.toLocaleTimeString()))), u().createElement(f, {
                         buttonSettings: this.state.buttonSettings,
                         afterButtonSettingClick: this.getData,
                         columns: this.state.tableFormat.cols,
                         data: this.state.jobs,
                         setMessageState: e => {
-                            this.setState(Object.assign(Object.assign({}, this.state), {
+                            this.setState((t => Object.assign(Object.assign({}, t), {
                                 message: e
-                            }))
+                            })))
                         },
                         getKernel: this.props.getKernel,
                         getJob: this.props.getJobCode,
                         handleError: this.catchError,
                         getFileBrowser: this.props.getFileBrowser
                     }))
                 }
             }
-            var F = a(543),
+            var F = a(219),
                 I = a(832);
             class B extends I.Widget {
                 constructor(e) {
                     super(e), this._labShell = e.labShell, this._command = e.command, this._commands = e.commandRegistry, this._area = e.area, this._shellOptions = e.shellOptions, this.title.icon = e.icon, this.title.caption = e.caption, this.id = e.id ? e.id : "tvb-ext-unicore-side-btn", this.title.className = this.id
                 }
                 addToLabShell() {
                     this._labShell.add(this, this._area, this._shellOptions)
@@ -532,15 +535,15 @@
                             break;
                         case "right":
                             this._labShell.collapseRight()
                     }
                     await this._commands.execute(this._command)
                 }
             }
-            var D = a(745);
+            var D = a(880);
             async function A(e) {
                 const t = {
                     resource_url: e
                 };
                 return p("jobs", {
                     method: "POST",
                     body: JSON.stringify(t)
```

### Comparing `tvb-ext-unicore-1.2.0/tvbextunicore/labextension/static/remoteEntry.c6b3242597cbbe03a95e.js` & `tvb-ext-unicore-2.0.0/tvbextunicore/labextension/static/remoteEntry.15eb2e0bc97996deb062.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, u, l, f, d, s, c, p, h, v = {
+    var e, r, t, n, o, a, i, u, l, f, s, d, p, c, h, v = {
             675: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(774).then((() => () => t(774))),
                         "./extension": () => t.e(774).then((() => () => t(774))),
                         "./style": () => t.e(747).then((() => () => t(747)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
@@ -43,49 +43,49 @@
         }), r
     }, g.d = (e, r) => {
         for (var t in r) g.o(r, t) && !g.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, g.f = {}, g.e = e => Promise.all(Object.keys(g.f).reduce(((r, t) => (g.f[t](e, r), r)), [])), g.u = e => e + "." + {
-        747: "c26c9bf4f7bddc1ea1c7",
-        774: "f5b7ad80ab759770978c"
+        747: "0bb902cd31ab1b8a32cc",
+        774: "96299c03c320cee66d47"
     } [e] + ".js?v=" + {
-        747: "c26c9bf4f7bddc1ea1c7",
-        774: "f5b7ad80ab759770978c"
+        747: "0bb902cd31ab1b8a32cc",
+        774: "96299c03c320cee66d47"
     } [e], g.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), g.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "tvb-ext-unicore:", g.l = (t, n, o, a) => {
         if (e[t]) e[t].push(n);
         else {
             var i, u;
             if (void 0 !== o)
                 for (var l = document.getElementsByTagName("script"), f = 0; f < l.length; f++) {
-                    var d = l[f];
-                    if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + o) {
-                        i = d;
+                    var s = l[f];
+                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + o) {
+                        i = s;
                         break
                     }
                 }
             i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, g.nc && i.setAttribute("nonce", g.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
-            var s = (r, n) => {
-                    i.onerror = i.onload = null, clearTimeout(c);
+            var d = (r, n) => {
+                    i.onerror = i.onload = null, clearTimeout(p);
                     var o = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
                 },
-                c = setTimeout(s.bind(null, void 0, {
+                p = setTimeout(d.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = s.bind(null, i.onerror), i.onload = s.bind(null, i.onload), u && document.head.appendChild(i)
+            i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), u && document.head.appendChild(i)
         }
     }, g.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -106,15 +106,15 @@
                     var o = a[e] = a[e] || {},
                         u = o[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (o[r] = {
                         get: () => g.e(774).then((() => () => g(774))),
                         from: i,
                         eager: !1
                     })
-                })("tvb-ext-unicore", "1.2.0"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("tvb-ext-unicore", "2.0.0"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         g.g.importScripts && (e = g.g.location + "");
         var r = g.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -163,87 +163,87 @@
     }, a = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 o = n < 0;
             o && (n = -n - 1);
             for (var i = 0, u = 1, l = !0;; u++, i++) {
-                var f, d, s = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (d = (typeof(f = r[i]))[0])) return !l || ("u" == s ? u > n && !o : "" == s != o);
-                if ("u" == d) {
-                    if (!l || "u" != s) return !1
+                var f, s, d = u < e.length ? (typeof e[u])[0] : "";
+                if (i >= r.length || "o" == (s = (typeof(f = r[i]))[0])) return !l || ("u" == d ? u > n && !o : "" == d != o);
+                if ("u" == s) {
+                    if (!l || "u" != d) return !1
                 } else if (l)
-                    if (s == d)
+                    if (d == s)
                         if (u <= n) {
                             if (f != e[u]) return !1
                         } else {
                             if (o ? f > e[u] : f < e[u]) return !1;
                             f != e[u] && (l = !1)
                         }
-                else if ("s" != s && "n" != s) {
+                else if ("s" != d && "n" != d) {
                     if (o || u <= n) return !1;
                     l = !1, u--
                 } else {
-                    if (u <= n || d < s != o) return !1;
+                    if (u <= n || s < d != o) return !1;
                     l = !1
-                } else "s" != s && "n" != s && (l = !1, u--)
+                } else "s" != d && "n" != d && (l = !1, u--)
             }
         }
-        var c = [],
-            p = c.pop.bind(c);
+        var p = [],
+            c = p.pop.bind(p);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
-            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? a(h, r) : !p())
+            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? a(h, r) : !c())
         }
-        return !!p()
+        return !!c()
     }, i = (e, r) => {
         var t = g.S[e];
         if (!t || !g.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
     }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", f = (e, r, t, n) => {
         var o = u(e, t);
-        return a(n, o) || "undefined" != typeof console && console.warn && console.warn(l(e, t, o, n)), d(e[t][o])
-    }, d = e => (e.loaded = 1, e.get()), s = (e => function(r, t, n, o) {
+        return a(n, o) || "undefined" != typeof console && console.warn && console.warn(l(e, t, o, n)), s(e[t][o])
+    }, s = e => (e.loaded = 1, e.get()), d = (e => function(r, t, n, o) {
         var a = g.I(r);
         return a && a.then ? a.then(e.bind(e, r, g.S[r], t, n, o)) : e(r, g.S[r], t, n)
-    })(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), c = {}, p = {
-        122: () => s("default", "@jupyterlab/filebrowser", [1, 3, 6, 5]),
-        127: () => s("default", "@jupyterlab/notebook", [1, 3, 6, 5]),
-        139: () => s("default", "@jupyterlab/services", [1, 6, 6, 5]),
-        271: () => s("default", "react", [1, 17, 0, 1]),
-        303: () => s("default", "@jupyterlab/apputils", [1, 3, 6, 5]),
-        344: () => s("default", "@jupyterlab/coreutils", [1, 5, 6, 5]),
-        526: () => s("default", "@lumino/coreutils", [1, 1, 11, 0]),
-        543: () => s("default", "@jupyterlab/console", [1, 3, 6, 5]),
-        638: () => s("default", "@jupyterlab/application", [1, 3, 6, 5]),
-        694: () => s("default", "@lumino/dragdrop", [1, 1, 13, 0]),
-        745: () => s("default", "@jupyterlab/ui-components", [1, 3, 6, 5]),
-        832: () => s("default", "@lumino/widgets", [1, 1, 37, 2]),
-        918: () => s("default", "@lumino/algorithm", [1, 1, 9, 0])
+    })(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), p = {}, c = {
+        46: () => d("default", "@jupyterlab/coreutils", [1, 5, 6, 7]),
+        83: () => d("default", "@jupyterlab/filebrowser", [1, 3, 6, 7]),
+        156: () => d("default", "@lumino/algorithm", [1, 1, 9, 0]),
+        219: () => d("default", "@jupyterlab/console", [1, 3, 6, 7]),
+        271: () => d("default", "@jupyterlab/application", [1, 3, 6, 7]),
+        526: () => d("default", "@lumino/coreutils", [1, 1, 11, 0]),
+        582: () => d("default", "@jupyterlab/services", [1, 6, 6, 7]),
+        583: () => d("default", "@jupyterlab/apputils", [1, 3, 6, 7]),
+        694: () => d("default", "@lumino/dragdrop", [1, 1, 13, 0]),
+        832: () => d("default", "@lumino/widgets", [1, 1, 37, 2]),
+        854: () => d("default", "@jupyterlab/notebook", [1, 3, 6, 7]),
+        880: () => d("default", "@jupyterlab/ui-components", [1, 3, 6, 7]),
+        918: () => d("default", "react", [1, 17, 0, 1])
     }, h = {
-        774: [122, 127, 139, 271, 303, 344, 526, 543, 638, 694, 745, 832, 918]
+        774: [46, 83, 156, 219, 271, 526, 582, 583, 694, 832, 854, 880, 918]
     }, g.f.consumes = (e, r) => {
         g.o(h, e) && h[e].forEach((e => {
-            if (g.o(c, e)) return r.push(c[e]);
+            if (g.o(p, e)) return r.push(p[e]);
             var t = r => {
-                    c[e] = 0, g.m[e] = t => {
+                    p[e] = 0, g.m[e] = t => {
                         delete g.c[e], t.exports = r()
                     }
                 },
                 n = r => {
-                    delete c[e], g.m[e] = t => {
+                    delete p[e], g.m[e] = t => {
                         throw delete g.c[e], r
                     }
                 };
             try {
-                var o = p[e]();
-                o.then ? r.push(c[e] = o.then(t).catch(n)) : t(o)
+                var o = c[e]();
+                o.then ? r.push(p[e] = o.then(t).catch(n)) : t(o)
             } catch (e) {
                 n(e)
             }
         }))
     }, (() => {
         var e = {
             899: 0
```

### Comparing `tvb-ext-unicore-1.2.0/tvbextunicore/labextension/static/third-party-licenses.json` & `tvb-ext-unicore-2.0.0/tvbextunicore/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `tvb-ext-unicore-1.2.0/tvbextunicore/logger/builder.py` & `tvb-ext-unicore-2.0.0/tvbextunicore/logger/builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # "TheVirtualBrain - Widgets" package
 #
-# (c) 2022-2023, TVB Widgets Team
+# (c) 2022-2024, TVB Widgets Team
 #
 
 import os
 import inspect
 import weakref
 import logging
 import logging.config
```

### Comparing `tvb-ext-unicore-1.2.0/tvbextunicore/logger/logging.conf` & `tvb-ext-unicore-2.0.0/tvbextunicore/logger/logging.conf`

 * *Files identical despite different names*

### Comparing `tvb-ext-unicore-1.2.0/tvbextunicore/tests/test_unicore_wrapper.py` & `tvb-ext-unicore-2.0.0/tvbextunicore/tests/test_unicore_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # "TheVirtualBrain - Widgets" package
 #
-# (c) 2022-2023, TVB Widgets Team
+# (c) 2022-2024, TVB Widgets Team
 #
 
 import json
 import os
 import pytest
 from datetime import datetime
```

### Comparing `tvb-ext-unicore-1.2.0/tvbextunicore/unicore_wrapper/job_dto.py` & `tvb-ext-unicore-2.0.0/tvbextunicore/unicore_wrapper/job_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # "TheVirtualBrain - Widgets" package
 #
-# (c) 2022-2023, TVB Widgets Team
+# (c) 2022-2024, TVB Widgets Team
 #
 
 from datetime import datetime
 
 NAME = 'name'
 MOUNT_POINT = 'mountPoint'
 TERMINATION_TIME = 'terminationTime'
```

### Comparing `tvb-ext-unicore-1.2.0/tvbextunicore/unicore_wrapper/unicore_wrapper.py` & `tvb-ext-unicore-2.0.0/tvbextunicore/unicore_wrapper/unicore_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 # -*- coding: utf-8 -*-
 #
 # "TheVirtualBrain - Widgets" package
 #
-# (c) 2022-2023, TVB Widgets Team
+# (c) 2022-2024, TVB Widgets Team
 #
 
 import os
-
 from pyunicore.client import _HBP_REGISTRY_URL
 import pyunicore.client as unicore_client
+from pyunicore.credentials import OIDCToken
 from requests.exceptions import ConnectionError
-
-from tvbextunicore.exceptions import TVBExtUnicoreException, ClientAuthException, \
-    SitesDownException, FileNotExistsException, JobRunningException
+from tvbextunicore.exceptions import TVBExtUnicoreException, ClientAuthException, SitesDownException
+from tvbextunicore.exceptions import FileNotExistsException, JobRunningException
 from tvbextunicore.logger.builder import get_logger
 from tvbextunicore.unicore_wrapper.job_dto import JobDTO
 
 LOGGER = get_logger(__name__)
 DOWNLOAD_MESSAGE = 'Downloaded successfully!'
 
 
 class UnicoreWrapper(object):
 
     def __init__(self):
-        token = self.__retrieve_token()
+        token = self.__retrieve_token_str()
+        token = OIDCToken(token)
         self.transport = self.__build_transport(token)
         self.registry = unicore_client.Registry(self.transport, _HBP_REGISTRY_URL)
 
-    def __retrieve_token(self):
+    def __retrieve_token_str(self):
         try:
             from clb_nb_utils import oauth as clb_oauth
             token = clb_oauth.get_token()
         except (ModuleNotFoundError, ConnectionError) as e:
             LOGGER.warning(f"Could not connect to EBRAINS to retrieve an auth token: {e}")
             LOGGER.info("Will try to use the auth token defined by environment variable CLB_AUTH...")
 
@@ -42,15 +42,15 @@
                                              "Collab, or define the CLB_AUTH environment variable!")
 
             LOGGER.info("Successfully retrieved the auth token from environment variable CLB_AUTH!")
         return token
 
     def __build_transport(self, token):
         # type: (str) -> unicore_client.Transport
-        transport = unicore_client.Transport(token, oidc=True)
+        transport = unicore_client.Transport(token)
         return transport
 
     def __build_client(self, site):
         # type: (dict) -> unicore_client.Client
         sites = self.registry.site_urls
         site_url = sites.get(site)
```

### Comparing `tvb-ext-unicore-1.2.0/tvbextunicore/utils.py` & `tvb-ext-unicore-2.0.0/tvbextunicore/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # "TheVirtualBrain - Widgets" package
 #
-# (c) 2022-2023, TVB Widgets Team
+# (c) 2022-2024, TVB Widgets Team
 #
 
 import json
 import enum
 from tvbextunicore.logger.builder import get_logger
 
 LOGGER = get_logger(__name__)
```

### Comparing `tvb-ext-unicore-1.2.0/yarn.lock` & `tvb-ext-unicore-2.0.0/yarn.lock`

 * *Files identical despite different names*

