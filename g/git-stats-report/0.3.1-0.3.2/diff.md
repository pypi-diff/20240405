# Comparing `tmp/git-stats-report-0.3.1.tar.gz` & `tmp/git-stats-report-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git-stats-report-0.3.1.tar", last modified: Thu Apr  4 05:22:59 2024, max compression
+gzip compressed data, was "git-stats-report-0.3.2.tar", last modified: Thu Apr  4 23:55:25 2024, max compression
```

## Comparing `git-stats-report-0.3.1.tar` & `git-stats-report-0.3.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:22:59.130883 git-stats-report-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-04 05:22:48.000000 git-stats-report-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-04 05:22:48.000000 git-stats-report-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-04-04 05:22:59.130883 git-stats-report-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-04 05:22:48.000000 git-stats-report-0.3.1/Pipfile
--rw-r--r--   0 runner    (1001) docker     (127)     5313 2024-04-04 05:22:48.000000 git-stats-report-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:22:59.126883 git-stats-report-0.3.1/git_stats_report/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-04 05:22:48.000000 git-stats-report-0.3.1/git_stats_report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-04 05:22:48.000000 git-stats-report-0.3.1/git_stats_report/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-04 05:22:48.000000 git-stats-report-0.3.1/git_stats_report/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-04-04 05:22:48.000000 git-stats-report-0.3.1/git_stats_report/git_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-04 05:22:48.000000 git-stats-report-0.3.1/git_stats_report/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 05:22:48.000000 git-stats-report-0.3.1/git_stats_report/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:22:59.130883 git-stats-report-0.3.1/git_stats_report/strategy/
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-04 05:22:48.000000 git-stats-report-0.3.1/git_stats_report/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-04 05:22:48.000000 git-stats-report-0.3.1/git_stats_report/strategy/from_date.py
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-04 05:22:48.000000 git-stats-report-0.3.1/git_stats_report/strategy/from_latest_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-04 05:22:48.000000 git-stats-report-0.3.1/git_stats_report/strategy/strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-04 05:22:48.000000 git-stats-report-0.3.1/git_stats_report/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:22:59.130883 git-stats-report-0.3.1/git_stats_report.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-04-04 05:22:59.000000 git-stats-report-0.3.1/git_stats_report.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-04 05:22:59.000000 git-stats-report-0.3.1/git_stats_report.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 05:22:59.000000 git-stats-report-0.3.1/git_stats_report.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-04 05:22:59.000000 git-stats-report-0.3.1/git_stats_report.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-04 05:22:59.000000 git-stats-report-0.3.1/git_stats_report.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-04 05:22:59.000000 git-stats-report-0.3.1/git_stats_report.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9489 2024-04-04 05:22:48.000000 git-stats-report-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 05:22:59.130883 git-stats-report-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:55:25.000931 git-stats-report-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-04 23:55:16.000000 git-stats-report-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-04 23:55:16.000000 git-stats-report-0.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7039 2024-04-04 23:55:25.000931 git-stats-report-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-04 23:55:16.000000 git-stats-report-0.3.2/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (127)     5940 2024-04-04 23:55:16.000000 git-stats-report-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:55:25.000931 git-stats-report-0.3.2/git_stats_report/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-04 23:55:16.000000 git-stats-report-0.3.2/git_stats_report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-04 23:55:16.000000 git-stats-report-0.3.2/git_stats_report/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-04 23:55:16.000000 git-stats-report-0.3.2/git_stats_report/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-04-04 23:55:16.000000 git-stats-report-0.3.2/git_stats_report/git_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-04 23:55:16.000000 git-stats-report-0.3.2/git_stats_report/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:55:16.000000 git-stats-report-0.3.2/git_stats_report/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:55:25.000931 git-stats-report-0.3.2/git_stats_report/strategy/
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-04 23:55:16.000000 git-stats-report-0.3.2/git_stats_report/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-04 23:55:16.000000 git-stats-report-0.3.2/git_stats_report/strategy/from_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-04 23:55:16.000000 git-stats-report-0.3.2/git_stats_report/strategy/from_latest_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-04 23:55:16.000000 git-stats-report-0.3.2/git_stats_report/strategy/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-04 23:55:16.000000 git-stats-report-0.3.2/git_stats_report/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:55:25.000931 git-stats-report-0.3.2/git_stats_report.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7039 2024-04-04 23:55:24.000000 git-stats-report-0.3.2/git_stats_report.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-04 23:55:24.000000 git-stats-report-0.3.2/git_stats_report.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 23:55:24.000000 git-stats-report-0.3.2/git_stats_report.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-04 23:55:24.000000 git-stats-report-0.3.2/git_stats_report.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-04 23:55:24.000000 git-stats-report-0.3.2/git_stats_report.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-04 23:55:24.000000 git-stats-report-0.3.2/git_stats_report.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9489 2024-04-04 23:55:16.000000 git-stats-report-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 23:55:25.000931 git-stats-report-0.3.2/setup.cfg
```

### Comparing `git-stats-report-0.3.1/LICENSE` & `git-stats-report-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `git-stats-report-0.3.1/PKG-INFO` & `git-stats-report-0.3.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-stats-report
-Version: 0.3.1
+Version: 0.3.2
 Author-email: Juan José Farina <juanjosefarina.jjf@gmail.com>, "Ezequiel L. Castaño" <castanoezequielleonardo@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/JuanJFarina/git-stats-report
 Project-URL: documentation, https://github.com/JuanJFarina/git-stats-report
 Project-URL: repository, https://github.com/JuanJFarina/git-stats-report
 Project-URL: changelog, https://github.com/JuanJFarina/git-stats-report/blob/master/CHANGELOG.md
 Classifier: Development Status :: 4 - Beta
@@ -40,29 +40,49 @@
 ```shell
 git-stats-report --help
 ```
 
 git-stats-report can be used in different ways, the most straightforward one is:
 
 ```shell
-git-stats-report
+git-stats-report -s "4"
 ```
 
-This will return statistics for each contributor since the last merge commit
+This will return statistics for each contributor since four days ago. The -s flag accepts
+any number greater than 0
+
+Other use of git-stats-report is with the -st flag, which allows to change the default
+behaviour, SINCE_DAYS, to FROM_LATEST_TAG:
+
+```shell
+git-stats-report -st "FROM_LATEST_TAG"
+```
+
+This will return statistics for each contributor since the last generated tag. Using the
+-st flag, the -s flag is not needed.
+
+A last option is the -r flag, which will return the raw string with linebreaks:
+
+```shell
+git-stats-report -r -s "4"
+```
+
+The output will be more suitable in some cases, like in CI/CD pipelines if you want to
+store the report in a variable and print it somewhere else.
 
 ## Installation
 
 
 ### With Pipx
 
 Recommended instalation for CICD is through `pipx` with a pinned version:
 
 ```shell
 pip install pipx==1.2.0
-pipx run git-stats-report==0.2.0
+pipx run git-stats-report==0.3.2
 ```
 
 That command will create a virtual environment just for git-stats-report and return the
 report.
 
 ### With pip
```

### Comparing `git-stats-report-0.3.1/Pipfile` & `git-stats-report-0.3.2/Pipfile`

 * *Files identical despite different names*

### Comparing `git-stats-report-0.3.1/README.md` & `git-stats-report-0.3.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -15,29 +15,49 @@
 ```shell
 git-stats-report --help
 ```
 
 git-stats-report can be used in different ways, the most straightforward one is:
 
 ```shell
-git-stats-report
+git-stats-report -s "4"
 ```
 
-This will return statistics for each contributor since the last merge commit
+This will return statistics for each contributor since four days ago. The -s flag accepts
+any number greater than 0
+
+Other use of git-stats-report is with the -st flag, which allows to change the default
+behaviour, SINCE_DAYS, to FROM_LATEST_TAG:
+
+```shell
+git-stats-report -st "FROM_LATEST_TAG"
+```
+
+This will return statistics for each contributor since the last generated tag. Using the
+-st flag, the -s flag is not needed.
+
+A last option is the -r flag, which will return the raw string with linebreaks:
+
+```shell
+git-stats-report -r -s "4"
+```
+
+The output will be more suitable in some cases, like in CI/CD pipelines if you want to
+store the report in a variable and print it somewhere else.
 
 ## Installation
 
 
 ### With Pipx
 
 Recommended instalation for CICD is through `pipx` with a pinned version:
 
 ```shell
 pip install pipx==1.2.0
-pipx run git-stats-report==0.2.0
+pipx run git-stats-report==0.3.2
 ```
 
 That command will create a virtual environment just for git-stats-report and return the
 report.
 
 ### With pip
```

### Comparing `git-stats-report-0.3.1/git_stats_report/__main__.py` & `git-stats-report-0.3.2/git_stats_report/__main__.py`

 * *Files identical despite different names*

### Comparing `git-stats-report-0.3.1/git_stats_report/entrypoint.py` & `git-stats-report-0.3.2/git_stats_report/entrypoint.py`

 * *Files identical despite different names*

### Comparing `git-stats-report-0.3.1/git_stats_report/git_stats.py` & `git-stats-report-0.3.2/git_stats_report/git_stats.py`

 * *Files identical despite different names*

### Comparing `git-stats-report-0.3.1/git_stats_report/strategy/__init__.py` & `git-stats-report-0.3.2/git_stats_report/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `git-stats-report-0.3.1/git_stats_report/strategy/from_latest_tag.py` & `git-stats-report-0.3.2/git_stats_report/strategy/from_latest_tag.py`

 * *Files identical despite different names*

### Comparing `git-stats-report-0.3.1/git_stats_report/utils.py` & `git-stats-report-0.3.2/git_stats_report/utils.py`

 * *Files identical despite different names*

### Comparing `git-stats-report-0.3.1/git_stats_report.egg-info/PKG-INFO` & `git-stats-report-0.3.2/git_stats_report.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-stats-report
-Version: 0.3.1
+Version: 0.3.2
 Author-email: Juan José Farina <juanjosefarina.jjf@gmail.com>, "Ezequiel L. Castaño" <castanoezequielleonardo@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/JuanJFarina/git-stats-report
 Project-URL: documentation, https://github.com/JuanJFarina/git-stats-report
 Project-URL: repository, https://github.com/JuanJFarina/git-stats-report
 Project-URL: changelog, https://github.com/JuanJFarina/git-stats-report/blob/master/CHANGELOG.md
 Classifier: Development Status :: 4 - Beta
@@ -40,29 +40,49 @@
 ```shell
 git-stats-report --help
 ```
 
 git-stats-report can be used in different ways, the most straightforward one is:
 
 ```shell
-git-stats-report
+git-stats-report -s "4"
 ```
 
-This will return statistics for each contributor since the last merge commit
+This will return statistics for each contributor since four days ago. The -s flag accepts
+any number greater than 0
+
+Other use of git-stats-report is with the -st flag, which allows to change the default
+behaviour, SINCE_DAYS, to FROM_LATEST_TAG:
+
+```shell
+git-stats-report -st "FROM_LATEST_TAG"
+```
+
+This will return statistics for each contributor since the last generated tag. Using the
+-st flag, the -s flag is not needed.
+
+A last option is the -r flag, which will return the raw string with linebreaks:
+
+```shell
+git-stats-report -r -s "4"
+```
+
+The output will be more suitable in some cases, like in CI/CD pipelines if you want to
+store the report in a variable and print it somewhere else.
 
 ## Installation
 
 
 ### With Pipx
 
 Recommended instalation for CICD is through `pipx` with a pinned version:
 
 ```shell
 pip install pipx==1.2.0
-pipx run git-stats-report==0.2.0
+pipx run git-stats-report==0.3.2
 ```
 
 That command will create a virtual environment just for git-stats-report and return the
 report.
 
 ### With pip
```

### Comparing `git-stats-report-0.3.1/git_stats_report.egg-info/SOURCES.txt` & `git-stats-report-0.3.2/git_stats_report.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `git-stats-report-0.3.1/pyproject.toml` & `git-stats-report-0.3.2/pyproject.toml`

 * *Files identical despite different names*

