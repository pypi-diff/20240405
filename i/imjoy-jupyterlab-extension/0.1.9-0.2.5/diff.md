# Comparing `tmp/imjoy-jupyterlab-extension-0.1.9.tar.gz` & `tmp/imjoy_jupyterlab_extension-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imjoy-jupyterlab-extension-0.1.9.tar", last modified: Tue Apr 26 18:57:33 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `imjoy-jupyterlab-extension-0.1.9.tar` & `imjoy_jupyterlab_extension-0.2.5.tar`

### file list

```diff
@@ -1,50 +1,49 @@
-drwxrwxr-x   0 weiouyang  (1002) weiouyang  (1002)        0 2022-04-26 18:57:33.738163 imjoy-jupyterlab-extension-0.1.9/
-drwxrwxr-x   0 weiouyang  (1002) weiouyang  (1002)        0 2022-04-26 18:57:33.734163 imjoy-jupyterlab-extension-0.1.9/.github/
-drwxrwxr-x   0 weiouyang  (1002) weiouyang  (1002)        0 2022-04-26 18:57:33.738163 imjoy-jupyterlab-extension-0.1.9/.github/workflows/
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     1424 2021-11-28 12:57:11.000000 imjoy-jupyterlab-extension-0.1.9/.github/workflows/build.yml
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     1451 2021-11-28 16:55:07.000000 imjoy-jupyterlab-extension-0.1.9/.gitignore
--rw-r--r--   0 weiouyang  (1002) weiouyang  (1002)    36864 2022-04-26 18:37:30.000000 imjoy-jupyterlab-extension-0.1.9/.jupyterlite.doit.db
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)      108 2021-11-28 12:57:11.000000 imjoy-jupyterlab-extension-0.1.9/.prettierignore
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)       79 2021-11-28 12:57:11.000000 imjoy-jupyterlab-extension-0.1.9/.prettierrc
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     1510 2021-11-28 12:57:11.000000 imjoy-jupyterlab-extension-0.1.9/LICENSE
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)      457 2021-11-28 12:57:11.000000 imjoy-jupyterlab-extension-0.1.9/MANIFEST.in
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     3128 2022-04-26 18:57:33.738163 imjoy-jupyterlab-extension-0.1.9/PKG-INFO
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     2081 2022-04-26 15:58:27.000000 imjoy-jupyterlab-extension-0.1.9/README.md
-drwxrwxr-x   0 weiouyang  (1002) weiouyang  (1002)        0 2022-04-26 18:57:33.738163 imjoy-jupyterlab-extension-0.1.9/binder/
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)      537 2021-11-28 12:57:11.000000 imjoy-jupyterlab-extension-0.1.9/binder/environment.yml
--rwxrwxr-x   0 weiouyang  (1002) weiouyang  (1002)     1280 2021-11-28 12:57:11.000000 imjoy-jupyterlab-extension-0.1.9/binder/postBuild
-drwxrwxr-x   0 weiouyang  (1002) weiouyang  (1002)        0 2022-04-26 18:57:33.738163 imjoy-jupyterlab-extension-0.1.9/imjoy-jupyterlab-extension/
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)      318 2021-11-28 12:57:11.000000 imjoy-jupyterlab-extension-0.1.9/imjoy-jupyterlab-extension/__init__.py
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)      441 2021-11-28 12:57:11.000000 imjoy-jupyterlab-extension-0.1.9/imjoy-jupyterlab-extension/_version.py
-drwxrwxr-x   0 weiouyang  (1002) weiouyang  (1002)        0 2022-04-26 18:57:33.738163 imjoy-jupyterlab-extension-0.1.9/imjoy-jupyterlab-extension/labextension/
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     2167 2022-04-26 18:57:33.000000 imjoy-jupyterlab-extension-0.1.9/imjoy-jupyterlab-extension/labextension/package.json
-drwxrwxr-x   0 weiouyang  (1002) weiouyang  (1002)        0 2022-04-26 18:57:33.738163 imjoy-jupyterlab-extension-0.1.9/imjoy-jupyterlab-extension/labextension/static/
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     7405 2022-04-26 18:57:33.000000 imjoy-jupyterlab-extension-0.1.9/imjoy-jupyterlab-extension/labextension/static/433.fcbb6360ae49aa4065ba.js
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     3385 2022-04-26 18:57:33.000000 imjoy-jupyterlab-extension-0.1.9/imjoy-jupyterlab-extension/labextension/static/747.08ecd031b9c0861222d4.js
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)   139369 2022-04-26 18:57:33.000000 imjoy-jupyterlab-extension-0.1.9/imjoy-jupyterlab-extension/labextension/static/942.c4b692e5941010f31829.js
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     3114 2022-04-26 18:57:33.000000 imjoy-jupyterlab-extension-0.1.9/imjoy-jupyterlab-extension/labextension/static/942.c4b692e5941010f31829.js.LICENSE.txt
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     6824 2022-04-26 18:57:33.000000 imjoy-jupyterlab-extension-0.1.9/imjoy-jupyterlab-extension/labextension/static/remoteEntry.05fe1fc8ad4851885deb.js
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)      169 2022-04-26 18:57:31.000000 imjoy-jupyterlab-extension-0.1.9/imjoy-jupyterlab-extension/labextension/static/style.js
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     2576 2022-04-26 18:57:33.000000 imjoy-jupyterlab-extension-0.1.9/imjoy-jupyterlab-extension/labextension/static/third-party-licenses.json
-drwxrwxr-x   0 weiouyang  (1002) weiouyang  (1002)        0 2022-04-26 18:57:33.738163 imjoy-jupyterlab-extension-0.1.9/imjoy_jupyterlab_extension.egg-info/
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     3128 2022-04-26 18:57:33.000000 imjoy-jupyterlab-extension-0.1.9/imjoy_jupyterlab_extension.egg-info/PKG-INFO
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     1281 2022-04-26 18:57:33.000000 imjoy-jupyterlab-extension-0.1.9/imjoy_jupyterlab_extension.egg-info/SOURCES.txt
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)        1 2022-04-26 18:57:33.000000 imjoy-jupyterlab-extension-0.1.9/imjoy_jupyterlab_extension.egg-info/dependency_links.txt
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)        1 2021-11-28 13:08:27.000000 imjoy-jupyterlab-extension-0.1.9/imjoy_jupyterlab_extension.egg-info/not-zip-safe
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)       16 2022-04-26 18:57:33.000000 imjoy-jupyterlab-extension-0.1.9/imjoy_jupyterlab_extension.egg-info/requires.txt
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)       27 2022-04-26 18:57:33.000000 imjoy-jupyterlab-extension-0.1.9/imjoy_jupyterlab_extension.egg-info/top_level.txt
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)      213 2021-11-28 12:57:11.000000 imjoy-jupyterlab-extension-0.1.9/install.json
-drwxrwxr-x   0 weiouyang  (1002) weiouyang  (1002)        0 2022-04-26 18:57:33.738163 imjoy-jupyterlab-extension-0.1.9/lib/
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     7214 2021-11-28 13:38:51.000000 imjoy-jupyterlab-extension-0.1.9/lib/comm-connection.js
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     9610 2022-04-26 18:56:33.000000 imjoy-jupyterlab-extension-0.1.9/lib/index.js
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)   264092 2022-04-26 18:56:48.000000 imjoy-jupyterlab-extension-0.1.9/package-lock.json
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     2025 2022-04-26 18:56:44.000000 imjoy-jupyterlab-extension-0.1.9/package.json
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)      165 2021-11-28 17:00:06.000000 imjoy-jupyterlab-extension-0.1.9/publish.sh
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)      145 2021-11-28 12:57:11.000000 imjoy-jupyterlab-extension-0.1.9/pyproject.toml
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)       38 2022-04-26 18:57:33.738163 imjoy-jupyterlab-extension-0.1.9/setup.cfg
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     2651 2021-11-28 17:00:36.000000 imjoy-jupyterlab-extension-0.1.9/setup.py
-drwxrwxr-x   0 weiouyang  (1002) weiouyang  (1002)        0 2022-04-26 18:57:33.738163 imjoy-jupyterlab-extension-0.1.9/style/
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)        0 2021-11-28 12:57:11.000000 imjoy-jupyterlab-extension-0.1.9/style/base.css
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)       25 2021-11-28 12:57:11.000000 imjoy-jupyterlab-extension-0.1.9/style/index.css
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)       21 2021-11-28 12:57:11.000000 imjoy-jupyterlab-extension-0.1.9/style/index.js
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)   240262 2021-11-28 13:09:16.000000 imjoy-jupyterlab-extension-0.1.9/yarn.lock
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.5/.copier-answers.yml
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.5/.prettierignore
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.5/.yarnrc.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.5/CHANGELOG.md
+-rw-r--r--   0        0        0     3935 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.5/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.5/babel.config.js
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.5/install.json
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.5/jest.config.js
+-rw-r--r--   0        0        0     6636 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.5/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.5/setup.py
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.5/tsconfig.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.5/tsconfig.test.json
+-rw-r--r--   0        0        0   390165 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.5/yarn.lock
+-rw-r--r--   0        0        0  4893937 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.5/docs/Screenshot 2023-11-14 at 11.14.19.png
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.5/imjoy_jupyterlab_extension/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.5/imjoy_jupyterlab_extension/_version.py
+-rw-r--r--   0        0        0    21040 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.5/imjoy_jupyterlab_extension/labextension/build_log.json
+-rw-r--r--   0        0        0     5880 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.5/imjoy_jupyterlab_extension/labextension/package.json
+-rw-r--r--   0        0        0    34362 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.5/imjoy_jupyterlab_extension/labextension/static/lib_index_js.9b49eabf628b7b47bd8a.js
+-rw-r--r--   0        0        0    49510 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.5/imjoy_jupyterlab_extension/labextension/static/lib_index_js.9b49eabf628b7b47bd8a.js.map
+-rw-r--r--   0        0        0    29891 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.5/imjoy_jupyterlab_extension/labextension/static/remoteEntry.255b911990d2e3135de9.js
+-rw-r--r--   0        0        0    28802 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.5/imjoy_jupyterlab_extension/labextension/static/remoteEntry.255b911990d2e3135de9.js.map
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.5/imjoy_jupyterlab_extension/labextension/static/style.js
+-rw-r--r--   0        0        0    19369 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.5/imjoy_jupyterlab_extension/labextension/static/style_index_js.4a04af2efb9bedd57803.js
+-rw-r--r--   0        0        0    14857 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.5/imjoy_jupyterlab_extension/labextension/static/style_index_js.4a04af2efb9bedd57803.js.map
+-rw-r--r--   0        0        0   187964 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.5/imjoy_jupyterlab_extension/labextension/static/vendors-node_modules_imjoy-core_dist_imjoy-loader_js-node_modules_imjoy-core_dist_imjoy-rpc_js.fa1a9cd9c57812bbe9b2.js
+-rw-r--r--   0        0        0   265384 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.5/imjoy_jupyterlab_extension/labextension/static/vendors-node_modules_imjoy-core_dist_imjoy-loader_js-node_modules_imjoy-core_dist_imjoy-rpc_js.fa1a9cd9c57812bbe9b2.js.map
+-rw-r--r--   0        0        0    57602 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.5/imjoy_jupyterlab_extension/labextension/static/vendors-node_modules_reflect-metadata_Reflect_js.91708819816796d39b60.js
+-rw-r--r--   0        0        0    65803 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.5/imjoy_jupyterlab_extension/labextension/static/vendors-node_modules_reflect-metadata_Reflect_js.91708819816796d39b60.js.map
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.5/scripts/publish.sh
+-rw-r--r--   0        0        0     7754 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.5/src/comm-connection.js
+-rw-r--r--   0        0        0    10204 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.5/src/imjoy-extension.js
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.5/src/index.ts
+-rw-r--r--   0        0        0     5995 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.5/src/utils.js
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.5/src/__tests__/imjoy-jupyterlab-extension.spec.ts
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.5/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.5/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.5/style/index.js
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.5/ui-tests/README.md
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.5/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.5/ui-tests/package.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.5/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.5/ui-tests/yarn.lock
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.5/ui-tests/tests/imjoy-jupyterlab-extension.spec.ts
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.5/.gitignore
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.5/LICENSE
+-rw-r--r--   0        0        0     3138 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.5/README.md
+-rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     6074 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.5/PKG-INFO
```

### Comparing `imjoy-jupyterlab-extension-0.1.9/.gitignore` & `imjoy_jupyterlab_extension-0.2.5/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,23 @@
 *.bundle.*
+lib/
 node_modules/
+*.log
+.eslintcache
+.stylelintcache
 *.egg-info/
 .ipynb_checkpoints
-*.ipynb
 *.tsbuildinfo
-imjoy-jupyterlab-extension/labextension
+imjoy_jupyterlab_extension/labextension
+# Version file is handled by hatchling
+imjoy_jupyterlab_extension/_version.py
+
+# Integration tests
+ui-tests/test-results/
+ui-tests/playwright-report/
 
 # Created by https://www.gitignore.io/api/python
 # Edit at https://www.gitignore.io/?templates=python
 
 ### Python ###
 # Byte-compiled / optimized / DLL files
 __pycache__/
@@ -22,14 +31,15 @@
 .Python
 build/
 develop-eggs/
 dist/
 downloads/
 eggs/
 .eggs/
+lib/
 lib64/
 parts/
 sdist/
 var/
 wheels/
 pip-wheel-metadata/
 share/python-wheels/
@@ -51,14 +61,15 @@
 htmlcov/
 .tox/
 .nox/
 .coverage
 .coverage.*
 .cache
 nosetests.xml
+coverage/
 coverage.xml
 *.cover
 .hypothesis/
 .pytest_cache/
 
 # Translations
 *.mo
@@ -105,7 +116,10 @@
 # Pyre type checker
 .pyre/
 
 # End of https://www.gitignore.io/api/python
 
 # OSX files
 .DS_Store
+
+# Yarn cache
+.yarn/
```

### Comparing `imjoy-jupyterlab-extension-0.1.9/LICENSE` & `imjoy_jupyterlab_extension-0.2.5/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 BSD 3-Clause License
 
-Copyright (c) 2020, Wei Ouyang All rights reserved.
+Copyright (c) 2024, Wei Ouyang
+All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
-* Redistributions of source code must retain the above copyright notice, this
-  list of conditions and the following disclaimer.
+1. Redistributions of source code must retain the above copyright notice, this
+   list of conditions and the following disclaimer.
 
-* Redistributions in binary form must reproduce the above copyright notice,
-  this list of conditions and the following disclaimer in the documentation
-  and/or other materials provided with the distribution.
-
-* Neither the name of the copyright holder nor the names of its
-  contributors may be used to endorse or promote products derived from
-  this software without specific prior written permission.
+2. Redistributions in binary form must reproduce the above copyright notice,
+   this list of conditions and the following disclaimer in the documentation
+   and/or other materials provided with the distribution.
+
+3. Neither the name of the copyright holder nor the names of its
+   contributors may be used to endorse or promote products derived from
+   this software without specific prior written permission.
 
 THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
 AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
 IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
 DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
```

### Comparing `imjoy-jupyterlab-extension-0.1.9/PKG-INFO` & `imjoy_jupyterlab_extension-0.2.5/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,106 +1,100 @@
-Metadata-Version: 2.1
-Name: imjoy-jupyterlab-extension
-Version: 0.1.9
-Summary: Run ImJoy plugins in JupyterLab
-Home-page: https://github.coimjoy-team/imjoy-jupyterlab-extension
-Author: Wei Ouyang
-Author-email: oeway007@gmail.com
-License: BSD-3-Clause
-Keywords: Jupyter,JupyterLab,JupyterLab3,ImJoy
-Platform: Linux
-Platform: Mac OS X
-Platform: Windows
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Framework :: Jupyter
-Classifier: Framework :: Jupyter :: JupyterLab
-Classifier: Framework :: Jupyter :: JupyterLab :: 3
-Classifier: Framework :: Jupyter :: JupyterLab :: Extensions
-Classifier: Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
+# ImJoy Jupyterlab Extension
+[![Github Actions Status](https://github.com/imjoy-team/imjoy-jupyterlab-extension/workflows/Build/badge.svg)](https://github.com/imjoy-team/imjoy-jupyterlab-extension/actions/workflows/build.yml)
 
-# imjoy-jupyterlab-extension
+Run ImJoy plugins in JupyterLab
+
+![screenshot of the imjoy jupyterlab extension](<./docs/Screenshot 2023-11-14 at 11.14.19.png>)
 
-![Github Actions Status](https://github.coimjoy-team/imjoy-jupyterlab-extension/workflows/Build/badge.svg)
 
-Run ImJoy plugins in JupyterLab
 
 ## Requirements
 
-* JupyterLab >= 3.0
+- JupyterLab >= 4.0.0
 
 ## Install
 
+To install the extension, execute:
+
 ```bash
 pip install imjoy-jupyterlab-extension
 ```
 
+## Uninstall
+
+To remove the extension, execute:
+
+```bash
+pip uninstall imjoy-jupyterlab-extension
+```
+
 ## Contributing
 
 ### Development install
 
 Note: You will need NodeJS to build the extension package.
 
 The `jlpm` command is JupyterLab's pinned version of
 [yarn](https://yarnpkg.com/) that is installed with JupyterLab. You may use
 `yarn` or `npm` in lieu of `jlpm` below.
 
 ```bash
 # Clone the repo to your local environment
 # Change directory to the imjoy-jupyterlab-extension directory
 # Install package in development mode
-pip install -e .
+pip install -e "."
 # Link your development version of the extension with JupyterLab
 jupyter labextension develop . --overwrite
 # Rebuild extension Typescript source after making changes
-jlpm run build
+jlpm build
 ```
 
 You can watch the source directory and run JupyterLab at the same time in different terminals to watch for changes in the extension's source and automatically rebuild the extension.
 
 ```bash
 # Watch the source directory in one terminal, automatically rebuilding when needed
-jlpm run watch
+jlpm watch
 # Run JupyterLab in another terminal
 jupyter lab
 ```
 
 With the watch command running, every saved change will immediately be built locally and available in your running JupyterLab. Refresh JupyterLab to load the change in your browser (you may need to wait several seconds for the extension to be rebuilt).
 
-By default, the `jlpm run build` command generates the source maps for this extension to make it easier to debug using the browser dev tools. To also generate source maps for the JupyterLab core extensions, you can run the following command:
+By default, the `jlpm build` command generates the source maps for this extension to make it easier to debug using the browser dev tools. To also generate source maps for the JupyterLab core extensions, you can run the following command:
 
 ```bash
 jupyter lab build --minimize=False
 ```
 
-### Uninstall
+### Development uninstall
 
 ```bash
 pip uninstall imjoy-jupyterlab-extension
 ```
 
-### Note 
-```
-npm run watch:labextension
-```
+In development mode, you will also need to remove the symlink created by `jupyter labextension develop`
+command. To find its location, you can run `jupyter labextension list` to figure out where the `labextensions`
+folder is located. Then you can remove the symlink named `imjoy-jupyterlab-extension` within that folder.
 
-```
-pip install jupyter_packaging
-npm run install:extension
-jupyter lab
-```
+### Testing the extension
 
-## Publish
+#### Frontend tests
 
-The setup.py script will rebuild the static files, therefore run:
-```
-sh publish.sh
+This extension is using [Jest](https://jestjs.io/) for JavaScript code testing.
+
+To execute them, execute:
+
+```sh
+jlpm
+jlpm test
 ```
 
+#### Integration tests
+
+This extension uses [Playwright](https://playwright.dev/docs/intro) for the integration tests (aka user level tests).
+More precisely, the JupyterLab helper [Galata](https://github.com/jupyterlab/jupyterlab/tree/master/galata) is used to handle testing the extension in JupyterLab.
+
+More information are provided within the [ui-tests](./ui-tests/README.md) README.
+
+### Packaging the extension
+
+See [RELEASE](RELEASE.md)
```

### Comparing `imjoy-jupyterlab-extension-0.1.9/lib/comm-connection.js` & `imjoy_jupyterlab_extension-0.2.5/src/comm-connection.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -228,10 +228,11 @@
 
     disconnect() {}
 
     emit(data) {
         data.peer_id = this._peer_id;
         const split = removeBuffers(data);
         split.state.__buffer_paths__ = split.buffer_paths;
-        this.comm.send(split.state, {}, {}, split.buffers);
+        // NOTE: updated for newer kernels, the send signature is different
+        this.comm.send(split.state, null, split.buffers);
     }
 }
```

### Comparing `imjoy-jupyterlab-extension-0.1.9/lib/index.js` & `imjoy_jupyterlab_extension-0.2.5/src/imjoy-extension.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,42 +1,40 @@
+/**
+ * Initialization data for the imjoy-jupyterlab-extension extension.
+ */
+
 import {
     loadImJoyBasicApp
 } from "imjoy-core/dist/imjoy-loader";
 import {
     setupRPC
 } from "imjoy-core/dist/imjoy-rpc";
 import {
-    IFileBrowserFactory
-} from '@jupyterlab/filebrowser';
-import {
-    ITranslator
-} from '@jupyterlab/translation';
+    githubUrlRaw,
+    convertZenodoFileUrl
+} from "./utils.js";
+import "reflect-metadata";
+
 import {
     showErrorMessage,
     Spinner
 } from '@jupyterlab/apputils';
 import {
     PathExt
 } from '@jupyterlab/coreutils';
 
 import {
-    ContentsManager
-} from '@jupyterlab/services';
-
-import {
     DisposableDelegate
 } from '@lumino/disposable';
 
 import {
     ToolbarButton
 } from '@jupyterlab/apputils';
 
-import {
-    version
-} from '../package.json';
+// import { version } from '../package.json';
 
 import {
     Connection
 } from './comm-connection.js';
 
 
 async function patchPyodideKernel(kernel) {
@@ -44,88 +42,88 @@
     // apply patch for pyolite to make sure we have the kernel id
     if (info.implementation === 'pyodide') {
         const kernel_patch = `
 import os
 import ipykernel
 import micropip
 import sys
-
 await micropip.install([ "imjoy-rpc"])
 import imjoy_rpc
-
 if 'imjoy' not in sys.modules:
     sys.modules['imjoy'] = sys.modules['imjoy_rpc']
-
 if 'IMJOY_RPC_CONNECTION' not in os.environ:
     os.environ['IMJOY_RPC_CONNECTION'] = 'jupyter'
-
 class Connect():
     def __init__(self, kernel_id):
         self.kernel_id = kernel_id
-
     def get_connection_file(self):
         return f"kernel-{self.kernel_id}.json"
-
 if not hasattr(ipykernel, 'connect'):
     ipykernel.connect = Connect("${kernel.id}")
 `;
         const future = kernel.requestExecute({
             code: kernel_patch
         });
         await future.done
         console.log('Pyodide kernel patch applied');
 
     }
 }
 
-async function parseURL(queryString, app, browser, trans) {
+export async function parseURL(queryString, app, browser, trans) {
     const urlParams = new URLSearchParams(queryString);
     const urls = urlParams.getAll("load");
     let lastFile = null;
     for (let url of urls) {
         let type = '';
         let blob;
         // fetch the file from the URL
         try {
+            if (url.includes("//zenodo.org/record")) {
+                url = await convertZenodoFileUrl(url);
+            } else {
+                url = await githubUrlRaw(url, ".ipynb") || url;
+            }
             const req = await fetch(url);
             blob = await req.blob();
             type = req.headers.get('Content-Type') ?? '';
+            // upload the content of the file to the server
+            try {
+                const name = PathExt.basename(url).split("?")[0];
+                const file = new File([blob], name, {
+                    type
+                });
+                const model = await browser.model.upload(file);
+                lastFile = model.path
+                console.log("File uploaded: " + model.path);
+            } catch (error) {
+                showErrorMessage(
+                    trans._p('showErrorMessage', 'Upload Error'),
+                    error
+                );
+            }
         } catch (reason) {
             if (reason.response && reason.response.status !== 200) {
                 reason.message = trans.__('Could not open URL: %1', url);
             }
             return showErrorMessage(trans.__('Cannot fetch'), reason);
         }
-        // upload the content of the file to the server
-        try {
-            const name = PathExt.basename(url).split("?")[0];
-            const file = new File([blob], name, {
-                type
-            });
-            const model = await browser.model.upload(file);
-            lastFile = model.path
-            console.log("File uploaded: " + model.path);
-        } catch (error) {
-            return showErrorMessage(
-                trans._p('showErrorMessage', 'Upload Error'),
-                error
-            );
-        }
     }
 
     let file2Open = urlParams.get("open")
     if (file2Open === "1") file2Open = lastFile;
     if (file2Open) {
-        app.commands.execute('docmanager:open', {
+        await app.commands.execute('docmanager:open', {
             path: file2Open
         });
     }
 }
-class ImjoyExtension {
-    constructor(jupyterBaseUrl) {
+
+export class ImjoyExtension {
+    constructor(jupyterBaseUrl, labApp, fileBrowser) {
         this.baseUrl = jupyterBaseUrl;
         const isIframe = window.self !== window.top;
         this.notebookHandlerPromise = new Promise((resolve, reject) => {
             this.resolveNotebookHandler = resolve;
             this.rejectNotebookHandler = reject;
         })
         // create an div with id= "window-container"
@@ -167,32 +165,68 @@
                     },
                 }
             }).then(async app => {
                 console.log(`ImJoy Basic App loaded!`)
                 imjoy = app.imjoy;
                 const kernelInfo = {}
                 if (isIframe) {
-                    const contents = new ContentsManager();
                     const api = await setupRPC({
-                        name: "ImJoy"
+                        name: "JupyterLite"
                     });
                     api.export({
                         setup() {},
-                        async saveContent(name, content) {
-                            await contents.save(name, content);
-                        },
-                        async openUrl(url, with_token) {
-                            if (with_token) {
-                                if (url.indexOf('?') === -1) {
-                                    url = url + '?token=' + contents.serverSettings.token;
-                                } else {
-                                    url = url + '&token=' + contents.serverSettings.token;
+                        run(ctx) {
+                            ctx = ctx || {}
+                            ctx.config = ctx.config || {}
+                            ctx.config.left_collapsed = ctx.config.left_collapsed === undefined ? true : false
+                            if (ctx.config.left_collapsed) {
+                                if (!labApp.shell.leftCollapsed) {
+                                    labApp.commands.execute('application:toggle-left-area');
                                 }
+                            } else {
+                                if (labApp.shell.leftCollapsed) {
+                                    labApp.commands.execute('application:toggle-left-area');
+                                }
+                            }
+                        },
+                        async fileExists(path) {
+                            try {
+                                await fileBrowser.model.manager.services.contents.get(path);
+                                return true;
+                            } catch (e) {
+                                return false;
+                            }
+                        },
+                        async getFile(path) {
+                            return await fileBrowser.model.manager.services.contents.get(path);
+                        },
+                        async removeFile(path) {
+                            return await fileBrowser.model.manager.deleteFile(path);
+                        },
+                        async loadFile(name, content, type) {
+                            const file = new File([content], name, {
+                                type
+                            });
+                            const model = await fileBrowser.model.upload(file);
+                            return model.path;
+                        },
+                        async openFile(path) {
+                            await labApp.commands.execute('docmanager:open', {
+                                path: path
+                            });
+                        },
+                        async closeLeft() {
+                            if (!labApp.shell.leftCollapsed) {
+                                labApp.commands.execute('application:toggle-left-area');
+                            }
+                        },
+                        async openLeft() {
+                            if (labApp.shell.leftCollapsed) {
+                                labApp.commands.execute('application:toggle-left-area');
                             }
-                            window.location.href = url;
                         }
                     })
                 }
 
                 async function connectPlugin(kernel_id) {
                     if (!kernelInfo[kernel_id]) {
                         console.warn('Kernel is not ready: ' + kernel_id);
@@ -293,49 +327,20 @@
     }
 
     /**
      * Create a new extension object.
      */
     createNew(panel, context) {
         const button = new ToolbarButton({
-            tooltip: `ImJoy JupyterLab Extension (version: ${version})`,
+            tooltip: `ImJoy JupyterLab Extension`, // (version: ${version})`,
         });
         panel.toolbar.insertItem(0, 'Run ImJoy Plugin', button);
 
         context.sessionContext.ready.then(async () => {
             const notebookHandler = await this.notebookHandlerPromise;
             notebookHandler(context.sessionContext, panel.node, button.node);
         });
         return new DisposableDelegate(() => {
             button.dispose();
         });
     }
-}
-
-
-export default {
-    id: 'imjoy-jupyterlab-extension',
-    requires: [IFileBrowserFactory, ITranslator],
-    autoStart: true,
-    activate: async function(app, factory, translator) {
-        const trans = translator.load('jupyterlab');
-        const {
-            defaultBrowser: browser
-        } = factory;
-        const jupyterBaseUrl =
-            app.serviceManager.settings.serverSettings.baseUrl;
-        app.docRegistry.addWidgetExtension(
-            'Notebook',
-            new ImjoyExtension(jupyterBaseUrl),
-        );
-        console.log(
-            'JupyterLab extension imjoy-jupyterlab-extension is activated!'
-        );
-        const currentLocation = new URL(window.location);
-        app.started.then(() => {
-            parseURL(window.location.search, app, browser, trans).finally(() => {
-                // restore location, since jupyterlab will force double slashes into single
-                window.history.pushState(null, '', currentLocation);
-            })
-        })
-    }
 }
```

