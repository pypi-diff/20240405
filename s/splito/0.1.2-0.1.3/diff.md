# Comparing `tmp/splito-0.1.2.tar.gz` & `tmp/splito-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splito-0.1.2.tar", last modified: Sat Dec  9 12:00:11 2023, max compression
+gzip compressed data, was "splito-0.1.3.tar", last modified: Fri Apr  5 15:28:42 2024, max compression
```

## Comparing `splito-0.1.2.tar` & `splito-0.1.3.tar`

### file list

```diff
@@ -1,79 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 12:00:11.287621 splito-0.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 12:00:11.279621 splito-0.1.2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-09 11:56:51.000000 splito-0.1.2/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)     5202 2023-12-09 11:56:51.000000 splito-0.1.2/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      627 2023-12-09 11:56:51.000000 splito-0.1.2/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 12:00:11.279621 splito-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      916 2023-12-09 11:56:51.000000 splito-0.1.2/.github/workflows/code-check.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-09 11:56:51.000000 splito-0.1.2/.github/workflows/doc.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3764 2023-12-09 11:56:51.000000 splito-0.1.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2023-12-09 11:56:51.000000 splito-0.1.2/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2023-12-09 11:56:51.000000 splito-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11506 2023-12-09 11:56:51.000000 splito-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3916 2023-12-09 12:00:11.287621 splito-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2023-12-09 11:56:51.000000 splito-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 12:00:11.279621 splito-0.1.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 12:00:11.279621 splito-0.1.2/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-09 11:56:51.000000 splito-0.1.2/docs/api/plot.md
--rw-r--r--   0 runner    (1001) docker     (127)      131 2023-12-09 11:56:51.000000 splito-0.1.2/docs/api/simpd.md
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-09 11:56:51.000000 splito-0.1.2/docs/api/splito.md
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-12-09 11:56:51.000000 splito-0.1.2/docs/api/utils.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 12:00:11.275621 splito-0.1.2/docs/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 12:00:11.279621 splito-0.1.2/docs/assets/css/
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2023-12-09 11:56:51.000000 splito-0.1.2/docs/assets/css/custom-splito.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 12:00:11.279621 splito-0.1.2/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)      856 2023-12-09 11:56:51.000000 splito-0.1.2/docs/images/logo-black.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2023-12-09 11:56:51.000000 splito-0.1.2/docs/images/logo-white.svg
--rw-r--r--   0 runner    (1001) docker     (127)      984 2023-12-09 11:56:51.000000 splito-0.1.2/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 12:00:11.283621 splito-0.1.2/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)     7439 2023-12-09 11:56:51.000000 splito-0.1.2/docs/tutorials/MOOD_Protocol.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   182769 2023-12-09 11:56:51.000000 splito-0.1.2/docs/tutorials/MPO_Splitters.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   347736 2023-12-09 11:56:51.000000 splito-0.1.2/docs/tutorials/Other_Splitters.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   291548 2023-12-09 11:56:51.000000 splito-0.1.2/docs/tutorials/Structure_based_Splitters.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   195174 2023-12-09 11:56:51.000000 splito-0.1.2/docs/tutorials/The_Basics.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      758 2023-12-09 11:56:51.000000 splito-0.1.2/docs/tutorials/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2023-12-09 11:56:51.000000 splito-0.1.2/env.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2023-12-09 11:56:51.000000 splito-0.1.2/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2023-12-09 11:56:51.000000 splito-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-09 12:00:11.287621 splito-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 12:00:11.283621 splito-0.1.2/splito/
--rw-r--r--   0 runner    (1001) docker     (127)      605 2023-12-09 11:56:51.000000 splito-0.1.2/splito/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6364 2023-12-09 11:56:51.000000 splito-0.1.2/splito/_distance_split_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6436 2023-12-09 11:56:51.000000 splito-0.1.2/splito/_distribution_split.py
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2023-12-09 11:56:51.000000 splito-0.1.2/splito/_kmeans_split.py
--rw-r--r--   0 runner    (1001) docker     (127)     2158 2023-12-09 11:56:51.000000 splito-0.1.2/splito/_max_dissimilarity_split.py
--rw-r--r--   0 runner    (1001) docker     (127)     2220 2023-12-09 11:56:51.000000 splito-0.1.2/splito/_min_max_split.py
--rw-r--r--   0 runner    (1001) docker     (127)     2635 2023-12-09 11:56:51.000000 splito-0.1.2/splito/_molecular_weight.py
--rw-r--r--   0 runner    (1001) docker     (127)    12728 2023-12-09 11:56:51.000000 splito-0.1.2/splito/_mood_split.py
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2023-12-09 11:56:51.000000 splito-0.1.2/splito/_perimeter_split.py
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2023-12-09 11:56:51.000000 splito-0.1.2/splito/_scaffold_split.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2023-12-09 11:56:51.000000 splito-0.1.2/splito/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 12:00:11.287621 splito-0.1.2/splito/simpd/
--rw-r--r--   0 runner    (1001) docker     (127)      430 2023-12-09 11:56:51.000000 splito-0.1.2/splito/simpd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2023-12-09 11:56:51.000000 splito-0.1.2/splito/simpd/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3583 2023-12-09 11:56:51.000000 splito-0.1.2/splito/simpd/clusters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2023-12-09 11:56:51.000000 splito-0.1.2/splito/simpd/descriptors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2023-12-09 11:56:51.000000 splito-0.1.2/splito/simpd/distance.py
--rw-r--r--   0 runner    (1001) docker     (127)     2943 2023-12-09 11:56:51.000000 splito-0.1.2/splito/simpd/ga.py
--rw-r--r--   0 runner    (1001) docker     (127)     3062 2023-12-09 11:56:51.000000 splito-0.1.2/splito/simpd/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     5314 2023-12-09 11:56:51.000000 splito-0.1.2/splito/simpd/problem.py
--rw-r--r--   0 runner    (1001) docker     (127)     7014 2023-12-09 11:56:51.000000 splito-0.1.2/splito/simpd/simpd.py
--rw-r--r--   0 runner    (1001) docker     (127)     7413 2023-12-09 11:56:51.000000 splito-0.1.2/splito/simpd/splitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2754 2023-12-09 11:56:51.000000 splito-0.1.2/splito/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 12:00:11.283621 splito-0.1.2/splito.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3916 2023-12-09 12:00:11.000000 splito-0.1.2/splito.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2023-12-09 12:00:11.000000 splito-0.1.2/splito.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-09 12:00:11.000000 splito-0.1.2/splito.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       94 2023-12-09 12:00:11.000000 splito-0.1.2/splito.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-12-09 12:00:11.000000 splito-0.1.2/splito.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 12:00:11.287621 splito-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      675 2023-12-09 11:56:51.000000 splito-0.1.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2023-12-09 11:56:51.000000 splito-0.1.2/tests/test_distribution_split.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2023-12-09 11:56:51.000000 splito-0.1.2/tests/test_kmeans_split.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2023-12-09 11:56:51.000000 splito-0.1.2/tests/test_max_dissimilarity_split.py
--rw-r--r--   0 runner    (1001) docker     (127)      388 2023-12-09 11:56:51.000000 splito-0.1.2/tests/test_min_max_split.py
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2023-12-09 11:56:51.000000 splito-0.1.2/tests/test_mood_split.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2023-12-09 11:56:51.000000 splito-0.1.2/tests/test_mw_split.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2023-12-09 11:56:51.000000 splito-0.1.2/tests/test_perimeter_split.py
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2023-12-09 11:56:51.000000 splito-0.1.2/tests/test_scaffold_split.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2023-12-09 11:56:51.000000 splito-0.1.2/tests/test_simpd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:28:42.519451 splito-0.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:28:42.507451 splito-0.1.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 15:25:11.000000 splito-0.1.3/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-04-05 15:25:11.000000 splito-0.1.3/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-05 15:25:11.000000 splito-0.1.3/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:28:42.507451 splito-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-05 15:25:11.000000 splito-0.1.3/.github/workflows/code-check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-05 15:25:11.000000 splito-0.1.3/.github/workflows/doc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-04-05 15:25:11.000000 splito-0.1.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-05 15:25:11.000000 splito-0.1.3/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-05 15:25:11.000000 splito-0.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    11506 2024-04-05 15:25:11.000000 splito-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-04-05 15:28:42.519451 splito-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-04-05 15:25:11.000000 splito-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:28:42.507451 splito-0.1.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:28:42.511451 splito-0.1.3/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-05 15:25:11.000000 splito-0.1.3/docs/api/plot.md
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-05 15:25:11.000000 splito-0.1.3/docs/api/simpd.md
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-05 15:25:11.000000 splito-0.1.3/docs/api/splito.md
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-05 15:25:11.000000 splito-0.1.3/docs/api/utils.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:28:42.507451 splito-0.1.3/docs/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:28:42.511451 splito-0.1.3/docs/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-05 15:25:11.000000 splito-0.1.3/docs/assets/css/custom-splito.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:28:42.511451 splito-0.1.3/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-05 15:25:11.000000 splito-0.1.3/docs/images/logo-black.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-04-05 15:25:11.000000 splito-0.1.3/docs/images/logo-white.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-05 15:25:11.000000 splito-0.1.3/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:28:42.511451 splito-0.1.3/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)     7439 2024-04-05 15:25:11.000000 splito-0.1.3/docs/tutorials/MOOD_Protocol.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   182769 2024-04-05 15:25:11.000000 splito-0.1.3/docs/tutorials/MPO_Splitters.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   347736 2024-04-05 15:25:11.000000 splito-0.1.3/docs/tutorials/Other_Splitters.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   291548 2024-04-05 15:25:11.000000 splito-0.1.3/docs/tutorials/Structure_based_Splitters.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   195174 2024-04-05 15:25:11.000000 splito-0.1.3/docs/tutorials/The_Basics.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-05 15:25:11.000000 splito-0.1.3/docs/tutorials/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-05 15:25:11.000000 splito-0.1.3/env.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-04-05 15:25:11.000000 splito-0.1.3/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-04-05 15:25:11.000000 splito-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 15:28:42.519451 splito-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:28:42.515451 splito-0.1.3/splito/
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-05 15:25:11.000000 splito-0.1.3/splito/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-04-05 15:25:11.000000 splito-0.1.3/splito/_distance_split_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6436 2024-04-05 15:25:11.000000 splito-0.1.3/splito/_distribution_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-05 15:25:11.000000 splito-0.1.3/splito/_kmeans_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-04-05 15:25:11.000000 splito-0.1.3/splito/_max_dissimilarity_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-04-05 15:25:11.000000 splito-0.1.3/splito/_min_max_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-05 15:25:11.000000 splito-0.1.3/splito/_molecular_weight.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12728 2024-04-05 15:25:11.000000 splito-0.1.3/splito/_mood_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-05 15:25:11.000000 splito-0.1.3/splito/_perimeter_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-05 15:25:11.000000 splito-0.1.3/splito/_scaffold_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-04-05 15:25:11.000000 splito-0.1.3/splito/_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-05 15:25:11.000000 splito-0.1.3/splito/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:28:42.515451 splito-0.1.3/splito/simpd/
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-05 15:25:11.000000 splito-0.1.3/splito/simpd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-05 15:25:11.000000 splito-0.1.3/splito/simpd/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-04-05 15:25:11.000000 splito-0.1.3/splito/simpd/clusters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-05 15:25:11.000000 splito-0.1.3/splito/simpd/descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-05 15:25:11.000000 splito-0.1.3/splito/simpd/distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-04-05 15:25:11.000000 splito-0.1.3/splito/simpd/ga.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-04-05 15:25:11.000000 splito-0.1.3/splito/simpd/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-04-05 15:25:11.000000 splito-0.1.3/splito/simpd/problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7014 2024-04-05 15:25:11.000000 splito-0.1.3/splito/simpd/simpd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7413 2024-04-05 15:25:11.000000 splito-0.1.3/splito/simpd/splitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-04-05 15:25:11.000000 splito-0.1.3/splito/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:28:42.519451 splito-0.1.3/splito.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-04-05 15:28:42.000000 splito-0.1.3/splito.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-05 15:28:42.000000 splito-0.1.3/splito.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 15:28:42.000000 splito-0.1.3/splito.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-05 15:28:42.000000 splito-0.1.3/splito.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-05 15:28:42.000000 splito-0.1.3/splito.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:28:42.519451 splito-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-05 15:25:11.000000 splito-0.1.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-05 15:25:11.000000 splito-0.1.3/tests/test_distribution_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-05 15:25:11.000000 splito-0.1.3/tests/test_kmeans_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-05 15:25:11.000000 splito-0.1.3/tests/test_max_dissimilarity_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-05 15:25:11.000000 splito-0.1.3/tests/test_min_max_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-05 15:25:11.000000 splito-0.1.3/tests/test_mood_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-05 15:25:11.000000 splito-0.1.3/tests/test_mw_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-05 15:25:11.000000 splito-0.1.3/tests/test_perimeter_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-05 15:25:11.000000 splito-0.1.3/tests/test_scaffold_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-05 15:25:11.000000 splito-0.1.3/tests/test_simpd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-05 15:25:11.000000 splito-0.1.3/tests/test_split.py
```

### Comparing `splito-0.1.2/.github/CODE_OF_CONDUCT.md` & `splito-0.1.3/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `splito-0.1.2/.github/PULL_REQUEST_TEMPLATE.md` & `splito-0.1.3/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `splito-0.1.2/.github/workflows/code-check.yml` & `splito-0.1.3/.github/workflows/code-check.yml`

 * *Files identical despite different names*

### Comparing `splito-0.1.2/.github/workflows/doc.yml` & `splito-0.1.3/.github/workflows/doc.yml`

 * *Files identical despite different names*

### Comparing `splito-0.1.2/.github/workflows/release.yml` & `splito-0.1.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `splito-0.1.2/.github/workflows/test.yml` & `splito-0.1.3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `splito-0.1.2/.gitignore` & `splito-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `splito-0.1.2/LICENSE` & `splito-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `splito-0.1.2/PKG-INFO` & `splito-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splito
-Version: 0.1.2
+Version: 0.1.3
 Summary: Machine Learning dataset splitting for life sciences.
 Author-email: Lu Zhu <lu@valencediscovery.com>, Hadrien Mary <hadrien@valencediscovery.com>, Cas Wognum <cas@valencediscovery.com>
 Project-URL: Source Code, https://github.com/datamol-io/splito
 Project-URL: Bug Tracker, https://github.com/datamol-io/splito/issues
 Project-URL: Documentation, https://splito-docs.datamol.io/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `splito-0.1.2/README.md` & `splito-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `splito-0.1.2/docs/assets/css/custom-splito.css` & `splito-0.1.3/docs/assets/css/custom-splito.css`

 * *Files identical despite different names*

### Comparing `splito-0.1.2/docs/images/logo-black.svg` & `splito-0.1.3/docs/images/logo-black.svg`

 * *Files identical despite different names*

### Comparing `splito-0.1.2/docs/images/logo-white.svg` & `splito-0.1.3/docs/images/logo-white.svg`

 * *Files identical despite different names*

### Comparing `splito-0.1.2/docs/index.md` & `splito-0.1.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `splito-0.1.2/docs/tutorials/MOOD_Protocol.ipynb` & `splito-0.1.3/docs/tutorials/MOOD_Protocol.ipynb`

 * *Files identical despite different names*

### Comparing `splito-0.1.2/docs/tutorials/MPO_Splitters.ipynb` & `splito-0.1.3/docs/tutorials/MPO_Splitters.ipynb`

 * *Files identical despite different names*

### Comparing `splito-0.1.2/docs/tutorials/Other_Splitters.ipynb` & `splito-0.1.3/docs/tutorials/Other_Splitters.ipynb`

 * *Files identical despite different names*

### Comparing `splito-0.1.2/docs/tutorials/Structure_based_Splitters.ipynb` & `splito-0.1.3/docs/tutorials/Structure_based_Splitters.ipynb`

 * *Files identical despite different names*

### Comparing `splito-0.1.2/docs/tutorials/The_Basics.ipynb` & `splito-0.1.3/docs/tutorials/The_Basics.ipynb`

 * *Files identical despite different names*

### Comparing `splito-0.1.2/docs/tutorials/utils.py` & `splito-0.1.3/docs/tutorials/utils.py`

 * *Files identical despite different names*

### Comparing `splito-0.1.2/env.yml` & `splito-0.1.3/env.yml`

 * *Files identical despite different names*

### Comparing `splito-0.1.2/mkdocs.yml` & `splito-0.1.3/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `splito-0.1.2/pyproject.toml` & `splito-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `splito-0.1.2/splito/__init__.py` & `splito-0.1.3/splito/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,22 @@
-from ._mood_split import MOODSplitter
+from ._distribution_split import StratifiedDistributionSplit
 from ._kmeans_split import KMeansSplit
-from ._perimeter_split import PerimeterSplit
 from ._max_dissimilarity_split import MaxDissimilaritySplit
-from ._scaffold_split import ScaffoldSplit
 from ._min_max_split import MolecularMinMaxSplit
 from ._molecular_weight import MolecularWeightSplit
-from ._distribution_split import StratifiedDistributionSplit
-
+from ._mood_split import MOODSplitter
+from ._perimeter_split import PerimeterSplit
+from ._scaffold_split import ScaffoldSplit
+from ._split import train_test_split, train_test_split_indices
 
 __all__ = [
     "MOODSplitter",
     "KMeansSplit",
     "PerimeterSplit",
     "MaxDissimilaritySplit",
     "ScaffoldSplit",
     "StratifiedDistributionSplit",
     "MolecularWeightSplit",
     "MolecularMinMaxSplit",
+    "train_test_split",
+    "train_test_split_indices",
 ]
```

### Comparing `splito-0.1.2/splito/_distance_split_base.py` & `splito-0.1.3/splito/_distance_split_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,41 @@
 import abc
+from typing import Callable, Optional, Sequence, Union
 
-import numpy as np
 import datamol as dm
-
-from typing import Callable, Union, Optional, Sequence
-
+import numpy as np
+import pandas as pd
 from numpy.random import RandomState
 from sklearn.metrics import pairwise_distances
 from sklearn.model_selection import GroupShuffleSplit
 from sklearn.model_selection._split import _validate_shuffle_split  # noqa W0212
 from sklearn.utils.validation import _num_samples  # noqa W0212
 
 from .utils import get_kmeans_clusters
 
-
 # In case users provide a list of SMILES instead of features, we rely on ECFP4 and the tanimoto distance by default
 MOLECULE_DEFAULT_FEATURIZER = dict(name="ecfp", kwargs=dict(radius=2, nBits=2048))
 MOLECULE_DEFAULT_DISTANCE_METRIC = "jaccard"
 
 
+def guess_distance_metric(example):
+    """Guess the appropriate distance metric given an exemplary datapoint"""
+
+    # By default we use the Euclidean distance
+    metric = "euclidean"
+
+    # For binary vectors we use jaccard
+    if isinstance(example, pd.DataFrame):
+        example = example.values  # DataFrames would require all().all() otherwise
+    if ((example == 0) | (example == 1)).all():
+        metric = "jaccard"
+
+    return metric
+
+
 def convert_to_default_feats_if_smiles(
     X: Union[Sequence[str], np.ndarray], metric: str, n_jobs: Optional[int] = None
 ):
     """
     If the input is a sequence of strings, assumes this is a list of SMILES and converts it
     to a default set of ECFP4 features with the default Tanimoto distance metric.
     """
@@ -42,15 +55,15 @@
 
 class DistanceSplitBase(GroupShuffleSplit, abc.ABC):
     """Base class for any splitter that splits the data based on the distance matrix."""
 
     def __init__(
         self,
         n_splits=10,
-        metric: Union[str, Callable] = "euclidean",
+        metric: Optional[Union[str, Callable]] = None,
         n_jobs: Optional[int] = None,
         test_size: Optional[Union[float, int]] = None,
         train_size: Optional[Union[float, int]] = None,
         random_state: Optional[Union[int, RandomState]] = None,
     ):
         super().__init__(
             n_splits=n_splits,
@@ -104,18 +117,20 @@
             default_test_size=self._default_test_size,
         )
 
         base_seed = self.random_state
         if base_seed is None:
             base_seed = 0
 
-        for i in range(self.n_splits):
-            # Convert to ECFP4 if X is a list of smiles
-            X, self._metric = convert_to_default_feats_if_smiles(X, self._metric, n_jobs=self._n_jobs)
+        # Convert to ECFP4 if X is a list of smiles
+        X, self._metric = convert_to_default_feats_if_smiles(X, self._metric, n_jobs=self._n_jobs)
+        if self._metric is None:
+            self._metric = guess_distance_metric(X[0])
 
+        for i in range(self.n_splits):
             # Possibly group the data to improve computation efficiency
             groups = self.reduce(X, base_seed + i)
 
             # Compute the distance matrix
             unique_groups, group_indices, group_counts = np.unique(
                 groups, return_inverse=True, return_counts=True, axis=0
             )
```

### Comparing `splito-0.1.2/splito/_distribution_split.py` & `splito-0.1.3/splito/_distribution_split.py`

 * *Files identical despite different names*

### Comparing `splito-0.1.2/splito/_kmeans_split.py` & `splito-0.1.3/splito/_kmeans_split.py`

 * *Files identical despite different names*

### Comparing `splito-0.1.2/splito/_max_dissimilarity_split.py` & `splito-0.1.3/splito/_max_dissimilarity_split.py`

 * *Files identical despite different names*

### Comparing `splito-0.1.2/splito/_min_max_split.py` & `splito-0.1.3/splito/_min_max_split.py`

 * *Files identical despite different names*

### Comparing `splito-0.1.2/splito/_molecular_weight.py` & `splito-0.1.3/splito/_molecular_weight.py`

 * *Files identical despite different names*

### Comparing `splito-0.1.2/splito/_mood_split.py` & `splito-0.1.3/splito/_mood_split.py`

 * *Files identical despite different names*

### Comparing `splito-0.1.2/splito/_perimeter_split.py` & `splito-0.1.3/splito/_perimeter_split.py`

 * *Files identical despite different names*

### Comparing `splito-0.1.2/splito/_scaffold_split.py` & `splito-0.1.3/splito/_scaffold_split.py`

 * *Files identical despite different names*

### Comparing `splito-0.1.2/splito/plot.py` & `splito-0.1.3/splito/plot.py`

 * *Files identical despite different names*

### Comparing `splito-0.1.2/splito/simpd/callbacks.py` & `splito-0.1.3/splito/simpd/callbacks.py`

 * *Files identical despite different names*

### Comparing `splito-0.1.2/splito/simpd/clusters.py` & `splito-0.1.3/splito/simpd/clusters.py`

 * *Files identical despite different names*

### Comparing `splito-0.1.2/splito/simpd/descriptors.py` & `splito-0.1.3/splito/simpd/descriptors.py`

 * *Files identical despite different names*

### Comparing `splito-0.1.2/splito/simpd/distance.py` & `splito-0.1.3/splito/simpd/distance.py`

 * *Files identical despite different names*

### Comparing `splito-0.1.2/splito/simpd/ga.py` & `splito-0.1.3/splito/simpd/ga.py`

 * *Files identical despite different names*

### Comparing `splito-0.1.2/splito/simpd/preprocess.py` & `splito-0.1.3/splito/simpd/preprocess.py`

 * *Files identical despite different names*

### Comparing `splito-0.1.2/splito/simpd/problem.py` & `splito-0.1.3/splito/simpd/problem.py`

 * *Files identical despite different names*

### Comparing `splito-0.1.2/splito/simpd/simpd.py` & `splito-0.1.3/splito/simpd/simpd.py`

 * *Files identical despite different names*

### Comparing `splito-0.1.2/splito/simpd/splitter.py` & `splito-0.1.3/splito/simpd/splitter.py`

 * *Files identical despite different names*

### Comparing `splito-0.1.2/splito/utils.py` & `splito-0.1.3/splito/utils.py`

 * *Files identical despite different names*

### Comparing `splito-0.1.2/splito.egg-info/PKG-INFO` & `splito-0.1.3/splito.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splito
-Version: 0.1.2
+Version: 0.1.3
 Summary: Machine Learning dataset splitting for life sciences.
 Author-email: Lu Zhu <lu@valencediscovery.com>, Hadrien Mary <hadrien@valencediscovery.com>, Cas Wognum <cas@valencediscovery.com>
 Project-URL: Source Code, https://github.com/datamol-io/splito
 Project-URL: Bug Tracker, https://github.com/datamol-io/splito/issues
 Project-URL: Documentation, https://splito-docs.datamol.io/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `splito-0.1.2/splito.egg-info/SOURCES.txt` & `splito-0.1.3/splito.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 splito/_kmeans_split.py
 splito/_max_dissimilarity_split.py
 splito/_min_max_split.py
 splito/_molecular_weight.py
 splito/_mood_split.py
 splito/_perimeter_split.py
 splito/_scaffold_split.py
+splito/_split.py
 splito/plot.py
 splito/utils.py
 splito.egg-info/PKG-INFO
 splito.egg-info/SOURCES.txt
 splito.egg-info/dependency_links.txt
 splito.egg-info/requires.txt
 splito.egg-info/top_level.txt
@@ -57,8 +58,9 @@
 tests/test_kmeans_split.py
 tests/test_max_dissimilarity_split.py
 tests/test_min_max_split.py
 tests/test_mood_split.py
 tests/test_mw_split.py
 tests/test_perimeter_split.py
 tests/test_scaffold_split.py
-tests/test_simpd.py
+tests/test_simpd.py
+tests/test_split.py
```

### Comparing `splito-0.1.2/tests/test_distribution_split.py` & `splito-0.1.3/tests/test_distribution_split.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import pytest
 
 from splito import StratifiedDistributionSplit
 from splito._distribution_split import Clustering1D
 
 
 @pytest.mark.parametrize("algorithm", list(Clustering1D))
-def test_splits_stratified_distribution(dataset_smiles, dataset_targets, algorithm):
+def test_splits_stratified_distribution(test_dataset_smiles, test_dataset_targets, algorithm):
     splitter = StratifiedDistributionSplit(algorithm=algorithm, n_splits=2)
 
-    for train_ind, test_ind in splitter.split(dataset_smiles, y=dataset_targets):
-        assert len(train_ind) + len(test_ind) == len(dataset_targets)
+    for train_ind, test_ind in splitter.split(test_dataset_smiles, y=test_dataset_targets):
+        assert len(train_ind) + len(test_ind) == len(test_dataset_targets)
         assert len(set(train_ind).intersection(set(test_ind))) == 0
         assert len(train_ind) > 0 and len(test_ind) > 0
 
         # TODO (cwognum): Add more specialized tests
```

### Comparing `splito-0.1.2/tests/test_kmeans_split.py` & `splito-0.1.3/tests/test_kmeans_split.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import numpy as np
 
 from splito import KMeansSplit
 
 
-def test_splits_kmeans_default_feats(dataset_smiles):
+def test_splits_kmeans_default_feats(test_dataset_smiles):
     splitter = KMeansSplit(n_splits=2)
 
-    for train_ind, test_ind in splitter.split(dataset_smiles):
-        assert len(train_ind) + len(test_ind) == len(dataset_smiles)
+    for train_ind, test_ind in splitter.split(test_dataset_smiles):
+        assert len(train_ind) + len(test_ind) == len(test_dataset_smiles)
         assert len(set(train_ind).intersection(set(test_ind))) == 0
         assert len(train_ind) > 0 and len(test_ind) > 0
         assert splitter._cluster_metric == "jaccard"
 
 
 def test_splits_kmeans():
     X = np.random.random((100, 100))
```

### Comparing `splito-0.1.2/tests/test_max_dissimilarity_split.py` & `splito-0.1.3/tests/test_max_dissimilarity_split.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import numpy as np
 
 from splito import MaxDissimilaritySplit
 
 
-def test_splits_max_dissimilar_default_feats(dataset_smiles):
+def test_splits_max_dissimilar_default_feats(test_dataset_smiles):
     splitter = MaxDissimilaritySplit(n_splits=2)
 
-    for train_ind, test_ind in splitter.split(dataset_smiles):
-        assert len(train_ind) + len(test_ind) == len(dataset_smiles)
+    for train_ind, test_ind in splitter.split(test_dataset_smiles):
+        assert len(train_ind) + len(test_ind) == len(test_dataset_smiles)
         assert len(set(train_ind).intersection(set(test_ind))) == 0
         assert len(train_ind) > 0 and len(test_ind) > 0
 
 
 def test_splits_max_dissimilar():
     X = np.random.random((100, 100))
     splitter = MaxDissimilaritySplit(n_splits=2, metric="euclidean")
```

### Comparing `splito-0.1.2/tests/test_mw_split.py` & `splito-0.1.3/tests/test_mw_split.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,25 @@
-import pytest
 import datamol as dm
+import pytest
+
 from splito import MolecularWeightSplit
 
 
 @pytest.mark.parametrize("generalize_to_larger", [True, False])
-def test_splits_molecular_weight(dataset_smiles, generalize_to_larger):
+def test_splits_molecular_weight(test_dataset_smiles, generalize_to_larger):
     splitter = MolecularWeightSplit(generalize_to_larger=generalize_to_larger, n_splits=2)
 
-    for train_ind, test_ind in splitter.split(dataset_smiles):
-        assert len(train_ind) + len(test_ind) == len(dataset_smiles)
+    for train_ind, test_ind in splitter.split(test_dataset_smiles):
+        assert len(train_ind) + len(test_ind) == len(test_dataset_smiles)
         assert len(set(train_ind).intersection(set(test_ind))) == 0
         assert len(train_ind) > len(test_ind)
         assert len(train_ind) > 0 and len(test_ind) > 0
 
-        train_mws = [dm.descriptors.mw(dm.to_mol(smi)) for smi in dataset_smiles[train_ind]]
+        train_mws = [dm.descriptors.mw(dm.to_mol(smi)) for smi in test_dataset_smiles[train_ind]]
         if generalize_to_larger:
-            assert all(dm.descriptors.mw(dm.to_mol(smi)) > max(train_mws) for smi in dataset_smiles[test_ind])
+            assert all(
+                dm.descriptors.mw(dm.to_mol(smi)) >= max(train_mws) for smi in test_dataset_smiles[test_ind]
+            )
         else:
-            assert all(dm.descriptors.mw(dm.to_mol(smi)) < min(train_mws) for smi in dataset_smiles[test_ind])
+            assert all(
+                dm.descriptors.mw(dm.to_mol(smi)) <= min(train_mws) for smi in test_dataset_smiles[test_ind]
+            )
```

### Comparing `splito-0.1.2/tests/test_perimeter_split.py` & `splito-0.1.3/tests/test_perimeter_split.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import numpy as np
 
 from splito import PerimeterSplit
 
 
-def test_splits_perimeter(dataset_smiles):
+def test_splits_perimeter(test_dataset_smiles):
     splitter = PerimeterSplit(n_splits=2)
 
-    for train_ind, test_ind in splitter.split(dataset_smiles):
-        assert len(train_ind) + len(test_ind) == len(dataset_smiles)
+    for train_ind, test_ind in splitter.split(test_dataset_smiles):
+        assert len(train_ind) + len(test_ind) == len(test_dataset_smiles)
         assert len(set(train_ind).intersection(set(test_ind))) == 0
         assert len(train_ind) > 0 and len(test_ind) > 0
         assert splitter._metric == "jaccard"
 
 
 def test_splits_perimeter_euclidean():
     X = np.random.random((100, 100))
```

### Comparing `splito-0.1.2/tests/test_scaffold_split.py` & `splito-0.1.3/tests/test_scaffold_split.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pytest
+
 from splito import ScaffoldSplit
 from splito._scaffold_split import get_scaffold
 
 
 def test_get_scaffold(manual_smiles):
     scf = [get_scaffold(smi, make_generic=False) for smi in manual_smiles]
     assert scf == [""] + ["c1ccccc1"] * 5 + ["O=c1[nH]c(=O)c2[nH]cnc2[nH]1"] * 2
@@ -10,17 +11,17 @@
 
 def test_get_scaffold_generic(manual_smiles):
     scf = [get_scaffold(smi, make_generic=True) for smi in manual_smiles]
     assert scf == [""] + ["*1:*:*:*:*:*:1"] * 5 + ["*=*1:*:*(=*):*2:*:*:*:*:2:*:1"] * 2
 
 
 @pytest.mark.parametrize("make_generic", [True, False])
-def test_splits_scaffold(dataset_smiles, make_generic):
-    splitter = ScaffoldSplit(dataset_smiles, n_splits=2, make_generic=make_generic)
-    for train_ind, test_ind in splitter.split(dataset_smiles):
-        assert len(train_ind) + len(test_ind) == len(dataset_smiles)
+def test_splits_scaffold(test_dataset_smiles, make_generic):
+    splitter = ScaffoldSplit(test_dataset_smiles, n_splits=2, make_generic=make_generic)
+    for train_ind, test_ind in splitter.split(test_dataset_smiles):
+        assert len(train_ind) + len(test_ind) == len(test_dataset_smiles)
         assert len(set(train_ind).intersection(set(test_ind))) == 0
         assert len(train_ind) > 0 and len(test_ind) > 0
 
-        train_scfs = set([get_scaffold(dataset_smiles[i], make_generic=make_generic) for i in train_ind])
-        test_scfs = [get_scaffold(dataset_smiles[i], make_generic=make_generic) for i in test_ind]
+        train_scfs = set([get_scaffold(test_dataset_smiles[i], make_generic=make_generic) for i in train_ind])
+        test_scfs = [get_scaffold(test_dataset_smiles[i], make_generic=make_generic) for i in test_ind]
         assert not any(test_scf in train_scfs for test_scf in test_scfs)
```

### Comparing `splito-0.1.2/tests/test_simpd.py` & `splito-0.1.3/tests/test_simpd.py`

 * *Files identical despite different names*

