# Comparing `tmp/Metage2Metabo-1.6.0.tar.gz` & `tmp/Metage2Metabo-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Metage2Metabo-1.6.0.tar", last modified: Fri Mar  1 12:50:56 2024, max compression
+gzip compressed data, was "Metage2Metabo-1.6.1.tar", last modified: Fri Apr  5 08:04:22 2024, max compression
```

## Comparing `Metage2Metabo-1.6.0.tar` & `Metage2Metabo-1.6.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 12:50:56.615286 Metage2Metabo-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     7662 2024-03-01 12:50:06.000000 Metage2Metabo-1.6.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 12:50:56.615286 Metage2Metabo-1.6.0/Metage2Metabo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19781 2024-03-01 12:50:56.000000 Metage2Metabo-1.6.0/Metage2Metabo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-03-01 12:50:56.000000 Metage2Metabo-1.6.0/Metage2Metabo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 12:50:56.000000 Metage2Metabo-1.6.0/Metage2Metabo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-01 12:50:56.000000 Metage2Metabo-1.6.0/Metage2Metabo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-01 12:50:56.000000 Metage2Metabo-1.6.0/Metage2Metabo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-01 12:50:56.000000 Metage2Metabo-1.6.0/Metage2Metabo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    19781 2024-03-01 12:50:56.615286 Metage2Metabo-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19212 2024-03-01 12:50:06.000000 Metage2Metabo-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 12:50:56.603287 Metage2Metabo-1.6.0/metage2metabo/
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-03-01 12:50:06.000000 Metage2Metabo-1.6.0/metage2metabo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23628 2024-03-01 12:50:06.000000 Metage2Metabo-1.6.0/metage2metabo/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15296 2024-03-01 12:50:06.000000 Metage2Metabo-1.6.0/metage2metabo/__main_analysis__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 12:50:56.603287 Metage2Metabo-1.6.0/metage2metabo/m2m/
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-03-01 12:50:06.000000 Metage2Metabo-1.6.0/metage2metabo/m2m/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-03-01 12:50:06.000000 Metage2Metabo-1.6.0/metage2metabo/m2m/community_addedvalue.py
--rw-r--r--   0 runner    (1001) docker     (127)     8736 2024-03-01 12:50:06.000000 Metage2Metabo-1.6.0/metage2metabo/m2m/community_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)    11802 2024-03-01 12:50:06.000000 Metage2Metabo-1.6.0/metage2metabo/m2m/individual_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)    13774 2024-03-01 12:50:06.000000 Metage2Metabo-1.6.0/metage2metabo/m2m/m2m_workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     6208 2024-03-01 12:50:06.000000 Metage2Metabo-1.6.0/metage2metabo/m2m/minimal_community.py
--rw-r--r--   0 runner    (1001) docker     (127)    21603 2024-03-01 12:50:06.000000 Metage2Metabo-1.6.0/metage2metabo/m2m/reconstruction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 12:50:56.607287 Metage2Metabo-1.6.0/metage2metabo/m2m_analysis/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-01 12:50:06.000000 Metage2Metabo-1.6.0/metage2metabo/m2m_analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8537 2024-03-01 12:50:06.000000 Metage2Metabo-1.6.0/metage2metabo/m2m_analysis/enumeration.py
--rw-r--r--   0 runner    (1001) docker     (127)    35906 2024-03-01 12:50:06.000000 Metage2Metabo-1.6.0/metage2metabo/m2m_analysis/graph_compression.py
--rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-03-01 12:50:06.000000 Metage2Metabo-1.6.0/metage2metabo/m2m_analysis/m2m_analysis_workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    10933 2024-03-01 12:50:06.000000 Metage2Metabo-1.6.0/metage2metabo/m2m_analysis/solution_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-03-01 12:50:06.000000 Metage2Metabo-1.6.0/metage2metabo/m2m_analysis/taxonomy.py
--rw-r--r--   0 runner    (1001) docker     (127)     7370 2024-03-01 12:50:06.000000 Metage2Metabo-1.6.0/metage2metabo/sbml_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     5504 2024-03-01 12:50:06.000000 Metage2Metabo-1.6.0/metage2metabo/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 12:50:56.607287 Metage2Metabo-1.6.0/metage2metabo/workflow_data/
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-03-01 12:50:06.000000 Metage2Metabo-1.6.0/metage2metabo/workflow_data/seeds_workflow.sbml
--rwxr-xr-x   0 runner    (1001) docker     (127)  4782536 2024-03-01 12:50:06.000000 Metage2Metabo-1.6.0/metage2metabo/workflow_data/workflow_genomes.tar.gz
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-03-01 12:50:06.000000 Metage2Metabo-1.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-01 12:50:56.615286 Metage2Metabo-1.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 12:50:56.615286 Metage2Metabo-1.6.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     6511 2024-03-01 12:50:06.000000 Metage2Metabo-1.6.0/test/test_m2m_addedvalue.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9943 2024-03-01 12:50:06.000000 Metage2Metabo-1.6.0/test/test_m2m_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-03-01 12:50:06.000000 Metage2Metabo-1.6.0/test/test_m2m_cscope.py
--rw-r--r--   0 runner    (1001) docker     (127)    21498 2024-03-01 12:50:06.000000 Metage2Metabo-1.6.0/test/test_m2m_iscope.py
--rw-r--r--   0 runner    (1001) docker     (127)    19290 2024-03-01 12:50:06.000000 Metage2Metabo-1.6.0/test/test_m2m_metacom.py
--rw-r--r--   0 runner    (1001) docker     (127)     6282 2024-03-01 12:50:06.000000 Metage2Metabo-1.6.0/test/test_m2m_mincom.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2415 2024-03-01 12:50:06.000000 Metage2Metabo-1.6.0/test/test_m2m_recon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-03-01 12:50:06.000000 Metage2Metabo-1.6.0/test/test_sbml_management.py
--rw-r--r--   0 runner    (1001) docker     (127)    13049 2024-03-01 12:50:06.000000 Metage2Metabo-1.6.0/test/test_tiny_toy_metacom.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:04:22.026137 Metage2Metabo-1.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     7662 2024-04-05 08:03:38.000000 Metage2Metabo-1.6.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:04:22.026137 Metage2Metabo-1.6.1/Metage2Metabo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19766 2024-04-05 08:04:22.000000 Metage2Metabo-1.6.1/Metage2Metabo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-05 08:04:22.000000 Metage2Metabo-1.6.1/Metage2Metabo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 08:04:22.000000 Metage2Metabo-1.6.1/Metage2Metabo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-05 08:04:22.000000 Metage2Metabo-1.6.1/Metage2Metabo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-05 08:04:22.000000 Metage2Metabo-1.6.1/Metage2Metabo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-05 08:04:22.000000 Metage2Metabo-1.6.1/Metage2Metabo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    19766 2024-04-05 08:04:22.026137 Metage2Metabo-1.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19197 2024-04-05 08:03:38.000000 Metage2Metabo-1.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:04:22.014137 Metage2Metabo-1.6.1/metage2metabo/
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-05 08:03:38.000000 Metage2Metabo-1.6.1/metage2metabo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23628 2024-04-05 08:03:38.000000 Metage2Metabo-1.6.1/metage2metabo/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15294 2024-04-05 08:03:38.000000 Metage2Metabo-1.6.1/metage2metabo/__main_analysis__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:04:22.014137 Metage2Metabo-1.6.1/metage2metabo/m2m/
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-05 08:03:38.000000 Metage2Metabo-1.6.1/metage2metabo/m2m/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-04-05 08:03:38.000000 Metage2Metabo-1.6.1/metage2metabo/m2m/community_addedvalue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9043 2024-04-05 08:03:38.000000 Metage2Metabo-1.6.1/metage2metabo/m2m/community_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11802 2024-04-05 08:03:38.000000 Metage2Metabo-1.6.1/metage2metabo/m2m/individual_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13774 2024-04-05 08:03:38.000000 Metage2Metabo-1.6.1/metage2metabo/m2m/m2m_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6208 2024-04-05 08:03:38.000000 Metage2Metabo-1.6.1/metage2metabo/m2m/minimal_community.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21603 2024-04-05 08:03:38.000000 Metage2Metabo-1.6.1/metage2metabo/m2m/reconstruction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:04:22.018137 Metage2Metabo-1.6.1/metage2metabo/m2m_analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-05 08:03:38.000000 Metage2Metabo-1.6.1/metage2metabo/m2m_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8537 2024-04-05 08:03:38.000000 Metage2Metabo-1.6.1/metage2metabo/m2m_analysis/enumeration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35906 2024-04-05 08:03:38.000000 Metage2Metabo-1.6.1/metage2metabo/m2m_analysis/graph_compression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-04-05 08:03:38.000000 Metage2Metabo-1.6.1/metage2metabo/m2m_analysis/m2m_analysis_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10933 2024-04-05 08:03:38.000000 Metage2Metabo-1.6.1/metage2metabo/m2m_analysis/solution_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-04-05 08:03:38.000000 Metage2Metabo-1.6.1/metage2metabo/m2m_analysis/taxonomy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7370 2024-04-05 08:03:38.000000 Metage2Metabo-1.6.1/metage2metabo/sbml_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5504 2024-04-05 08:03:38.000000 Metage2Metabo-1.6.1/metage2metabo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:04:22.018137 Metage2Metabo-1.6.1/metage2metabo/workflow_data/
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-04-05 08:03:38.000000 Metage2Metabo-1.6.1/metage2metabo/workflow_data/seeds_workflow.sbml
+-rwxr-xr-x   0 runner    (1001) docker     (127)  4782536 2024-04-05 08:03:38.000000 Metage2Metabo-1.6.1/metage2metabo/workflow_data/workflow_genomes.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-05 08:03:38.000000 Metage2Metabo-1.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 08:04:22.026137 Metage2Metabo-1.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:04:22.026137 Metage2Metabo-1.6.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     6511 2024-04-05 08:03:39.000000 Metage2Metabo-1.6.1/test/test_m2m_addedvalue.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9943 2024-04-05 08:03:39.000000 Metage2Metabo-1.6.1/test/test_m2m_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-04-05 08:03:39.000000 Metage2Metabo-1.6.1/test/test_m2m_cscope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21498 2024-04-05 08:03:39.000000 Metage2Metabo-1.6.1/test/test_m2m_iscope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19290 2024-04-05 08:03:39.000000 Metage2Metabo-1.6.1/test/test_m2m_metacom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6282 2024-04-05 08:03:39.000000 Metage2Metabo-1.6.1/test/test_m2m_mincom.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2415 2024-04-05 08:03:39.000000 Metage2Metabo-1.6.1/test/test_m2m_recon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-05 08:03:39.000000 Metage2Metabo-1.6.1/test/test_sbml_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13543 2024-04-05 08:03:39.000000 Metage2Metabo-1.6.1/test/test_tiny_toy_metacom.py
```

### Comparing `Metage2Metabo-1.6.0/LICENSE` & `Metage2Metabo-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Metage2Metabo-1.6.0/Metage2Metabo.egg-info/PKG-INFO` & `Metage2Metabo-1.6.1/Metage2Metabo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: Metage2Metabo
-Version: 1.6.0
+Version: 1.6.1
 Summary: Automatic reconstruction of draft metabolic networks with Pathway Tools and graph-based metabolic analysis
 Author-email: AuReMe <gem-aureme@inria.fr>
 License: LGPL-3.0-or-later
 Project-URL: Homepage, https://github.com/aureme/metage2metabo
 Project-URL: Changelog, https://github.com/aureme/metage2metabo/blob/main/CHANGELOG.md
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: miscoto
 Requires-Dist: menetools
 Requires-Dist: mpwt
 Requires-Dist: padmet
 
-[![PyPI version](https://img.shields.io/pypi/v/metage2metabo.svg)](https://pypi.org/project/Metage2Metabo/) [![GitHub license](https://img.shields.io/github/license/AuReMe/metage2metabo.svg)](https://github.com/AuReMe/metage2metabo/blob/master/LICENSE) [![Actions Status](https://github.com/AuReMe/metage2metabo/actions/workflows/pythonpackage.yml/badge.svg)](https://github.com/AuReMe/metage2metabo/actions/workflows/pythonpackage.yml) [![Documentation Status](https://readthedocs.org/projects/metage2metabo/badge/?version=latest)](https://metage2metabo.readthedocs.io/en/latest/?badge=latest) [![](https://img.shields.io/badge/doi-10.7554/eLife.61968-blueviolet.svg)](https://doi.org/10.7554/eLife.61968)
+[![PyPI version](https://img.shields.io/pypi/v/metage2metabo.svg)](https://pypi.org/project/Metage2Metabo/) [![GitHub license](https://img.shields.io/github/license/AuReMe/metage2metabo.svg)](https://github.com/AuReMe/metage2metabo/blob/main/LICENSE) [![Actions Status](https://github.com/AuReMe/metage2metabo/actions/workflows/pythonpackage.yml/badge.svg)](https://github.com/AuReMe/metage2metabo/actions/workflows/pythonpackage.yml) [![Documentation Status](https://readthedocs.org/projects/metage2metabo/badge/?version=latest)](https://metage2metabo.readthedocs.io/en/latest/?badge=latest) [![](https://img.shields.io/badge/doi-10.7554/eLife.61968-blueviolet.svg)](https://doi.org/10.7554/eLife.61968)
 
 # M2M - metage2metabo
 Metage2metabo is a Python3 (Python >= 3.8, tested with 3.8 and 3.9) tool to perform graph-based metabolic analysis starting from annotated genomes (**reference genomes or metagenome-assembled genomes**). It uses *Pathway Tools* in a automatic and parallel way to **reconstruct metabolic networks** for a large number of genomes. The obtained metabolic networks are then **analyzed individually and collectively** in order to get the **added value of metabolic cooperation in microbiota over individual metabolism** and to **identify and screen interesting organisms** among all.
 
 
 m2m can be used as a whole workflow (``` m2m workflow ```, ``` m2m metacom ```) or steps can be performed individually (``` m2m recon ``` , ``` m2m iscope ``` , ``` m2m cscope ```, ``` m2m addedvalue ```, ``` m2m mincom ```, ``` m2m seeds ```).
 
@@ -66,23 +66,23 @@
 * an *initiation rule*: producibility is initiated by the presence of nutrients, called *seeds*. 
 
 A metabolite that is producible from a set of nutrients is described as being "in the scope of the seeds".
 The computation is made using logic solvers (Answer Set Programming). The present modelling ignores the stoichiometry of reactions (2A + B --> C is considered equivalent to A + B --> C), and is therefore suited to non-curated or draft metabolic networks, as the ones built using M2M with the PathoLogic software of [Pathway Tools](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5036846/pdf/bbv079.pdf) handled by [Mpwt](https://github.com/AuReMe/mpwt). Many works have relied on network expansion to study organisms ([here](http://doi.wiley.com/10.1111/tpj.12627), [here](https://dx.plos.org/10.1371/journal.pcbi.1000049) or [there](http://dx.plos.org/10.1371/journal.pcbi.1005276)) and communities ([here](https://academic.oup.com/bioinformatics/article/34/17/i934/5093211), [here](https://bmcgenomics.biomedcentral.com/articles/10.1186/s12864-018-4786-7), or [here](https://www.ncbi.nlm.nih.gov/pubmed/18546499)). It has been [compared](http://www.ncbi.nlm.nih.gov/pubmed/19425125), [combined](https://www.cambridge.org/core/product/identifier/S1471068418000455/type/journal_article) to steady-state modelling (Flux Balance Analysis).
 
 ## License
 
-This project is licensed under the GNU Lesser General Public License - see the [LICENSE.md](https://github.com/AuReMe/metage2metabo/blob/master/LICENSE) file for details.
+This project is licensed under the GNU Lesser General Public License - see the [LICENSE.md](https://github.com/AuReMe/metage2metabo/blob/main/LICENSE) file for details.
 
 ## Documentation
 
 A more detailled documentation is available at: [https://metage2metabo.readthedocs.io](https://metage2metabo.readthedocs.io/en/latest/).
 
 ## Technologies
 
-Python 3 (Python 3.8 and 3.9 is tested). M2M uses a certain number of Python dependencies. An example of all these dependencies working for Ubuntu 18.04 is available in [requirements.txt](https://github.com/AuReMe/metage2metabo/blob/master/requirements.txt).
+Python 3 (Python 3.8 and 3.9 are tested). M2M uses a certain number of Python dependencies. An example of all these dependencies working for Ubuntu 18.04 is available in [requirements.txt](https://github.com/AuReMe/metage2metabo/blob/main/requirements.txt).
 They can be installed with:
 ````sh
 pip install -r requirements.txt --no-cache-dir
 ````
 In particular, m2m relies on:
 * [mpwt](https://github.com/AuReMe/mpwt) to automatize metabolic network reconstruction with Pathway Tools
 * [padmet](https://github.com/AuReMe/padmet) to manage metabolic networks
@@ -130,15 +130,15 @@
         ````sh
         echo 'export PATH="$PATH:your/install/directory/pathway-tools:"' >> ~/.bashrc
         ````
         Then source the bashrc file:
         ````sh
         source ~/.bashrc
 
-* [Oog Power Graph Command line tool](https://github.com/AuReMe/metage2metabo/tree/master/external_dependencies/Oog_CommandLineTool2012) to create a svg file from the compressed graph at the end of m2m_analysis. This tool is a jar file (``Oog.jar``) so Java is needed to use it.
+* [Oog Power Graph Command line tool](https://github.com/AuReMe/metage2metabo/tree/main/external_dependencies/Oog_CommandLineTool2012) to create a svg file from the compressed graph at the end of m2m_analysis. This tool is a jar file (``Oog.jar``) so Java is needed to use it.
 
 ## Installation
 
 Developed and tested on Linux (Ubuntu, Fedora, Debian) and MacOs (version 10.14) with Python3.8.
 
 Continuous Integration using GitHub Actions with Python3.8 and Python3.9 on ubuntu-latest, macos-latest and windows-latest ([corresponding virtual environment](https://docs.github.com/en/free-pro-team@latest/actions/reference/specifications-for-github-hosted-runners#supported-runners-and-hardware-resources)).
 
@@ -221,15 +221,15 @@
 
   {enum,graph,powergraph,workflow}
     enum                enumeration using miscoto
     graph               graph creation with enumeration solution
     powergraph          powergraph creation and visualization
     workflow            whole workflow
 
-Optional: Oog.jar file (https://github.com/AuReMe/metage2metabo/tree/master/external_dependencies) for powergraph svg creation.
+Optional: Oog.jar file (https://github.com/AuReMe/metage2metabo/tree/main/external_dependencies) for powergraph svg creation.
 ````
 
 ## Release Notes
 
 Changes between version are listed on the [release page](https://github.com/AuReMe/metage2metabo/releases).
 
 ## Additional features
@@ -284,17 +284,17 @@
 - ``ete3`` for taxonomic information used in power graphs:
 
 Huerta-Cepas J, Serra F, Bork P. ETE 3: Reconstruction, Analysis, and Visualization of Phylogenomic Data. Molecular Biology and Evolution 2016;33:1635–1638. [https://doi.org/10.1093/molbev/msw046](https://doi.org/10.1093/molbev/msw046).
 
 
 ## Article data
 
-Data used to create figures and tables are listed in the [article_data](https://github.com/AuReMe/metage2metabo/tree/master/article_data) folder, it contains:
+Data used to create figures and tables are listed in the [article_data](https://github.com/AuReMe/metage2metabo/tree/main/article_data) folder, it contains:
 
-- [gsmn_characteristics](https://github.com/AuReMe/metage2metabo/tree/master/article_data/gsmn_characteristics): scripts and tables to show the characteristics of draft metabolic networks created by M2M for gut, rumen and diabetes dataset.
-- [diabetes_study](https://github.com/AuReMe/metage2metabo/tree/master/article_data/diabetes_study): scripts and tables to create the figures of the diabetes analyses in the article.
+- [gsmn_characteristics](https://github.com/AuReMe/metage2metabo/tree/main/article_data/gsmn_characteristics): scripts and tables to show the characteristics of draft metabolic networks created by M2M for gut, rumen and diabetes dataset.
+- [diabetes_study](https://github.com/AuReMe/metage2metabo/tree/main/article_data/diabetes_study): scripts and tables to create the figures of the diabetes analyses in the article.
 
 ## Authors
 [Clémence Frioux](https://cfrioux.github.io/) and [Arnaud Belcour](https://arnaudbelcour.github.io/blog/), `Univ Bordeaux, Inria, INRAE, Bordeaux, France`, `Univ Grenoble Alpes, Inria, Grenoble, France` and `Univ Rennes, Inria, CNRS, IRISA, Rennes, France`.
 
 ## Acknowledgement
 People of Pathway Tools (SRI International) for their help integrating Pathway Tools with command line and multiprocessing in the [mpwt](https://github.com/AuReMe/mpwt) package, used in M2M.
```

### Comparing `Metage2Metabo-1.6.0/Metage2Metabo.egg-info/SOURCES.txt` & `Metage2Metabo-1.6.1/Metage2Metabo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Metage2Metabo-1.6.0/PKG-INFO` & `Metage2Metabo-1.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: Metage2Metabo
-Version: 1.6.0
+Version: 1.6.1
 Summary: Automatic reconstruction of draft metabolic networks with Pathway Tools and graph-based metabolic analysis
 Author-email: AuReMe <gem-aureme@inria.fr>
 License: LGPL-3.0-or-later
 Project-URL: Homepage, https://github.com/aureme/metage2metabo
 Project-URL: Changelog, https://github.com/aureme/metage2metabo/blob/main/CHANGELOG.md
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: miscoto
 Requires-Dist: menetools
 Requires-Dist: mpwt
 Requires-Dist: padmet
 
-[![PyPI version](https://img.shields.io/pypi/v/metage2metabo.svg)](https://pypi.org/project/Metage2Metabo/) [![GitHub license](https://img.shields.io/github/license/AuReMe/metage2metabo.svg)](https://github.com/AuReMe/metage2metabo/blob/master/LICENSE) [![Actions Status](https://github.com/AuReMe/metage2metabo/actions/workflows/pythonpackage.yml/badge.svg)](https://github.com/AuReMe/metage2metabo/actions/workflows/pythonpackage.yml) [![Documentation Status](https://readthedocs.org/projects/metage2metabo/badge/?version=latest)](https://metage2metabo.readthedocs.io/en/latest/?badge=latest) [![](https://img.shields.io/badge/doi-10.7554/eLife.61968-blueviolet.svg)](https://doi.org/10.7554/eLife.61968)
+[![PyPI version](https://img.shields.io/pypi/v/metage2metabo.svg)](https://pypi.org/project/Metage2Metabo/) [![GitHub license](https://img.shields.io/github/license/AuReMe/metage2metabo.svg)](https://github.com/AuReMe/metage2metabo/blob/main/LICENSE) [![Actions Status](https://github.com/AuReMe/metage2metabo/actions/workflows/pythonpackage.yml/badge.svg)](https://github.com/AuReMe/metage2metabo/actions/workflows/pythonpackage.yml) [![Documentation Status](https://readthedocs.org/projects/metage2metabo/badge/?version=latest)](https://metage2metabo.readthedocs.io/en/latest/?badge=latest) [![](https://img.shields.io/badge/doi-10.7554/eLife.61968-blueviolet.svg)](https://doi.org/10.7554/eLife.61968)
 
 # M2M - metage2metabo
 Metage2metabo is a Python3 (Python >= 3.8, tested with 3.8 and 3.9) tool to perform graph-based metabolic analysis starting from annotated genomes (**reference genomes or metagenome-assembled genomes**). It uses *Pathway Tools* in a automatic and parallel way to **reconstruct metabolic networks** for a large number of genomes. The obtained metabolic networks are then **analyzed individually and collectively** in order to get the **added value of metabolic cooperation in microbiota over individual metabolism** and to **identify and screen interesting organisms** among all.
 
 
 m2m can be used as a whole workflow (``` m2m workflow ```, ``` m2m metacom ```) or steps can be performed individually (``` m2m recon ``` , ``` m2m iscope ``` , ``` m2m cscope ```, ``` m2m addedvalue ```, ``` m2m mincom ```, ``` m2m seeds ```).
 
@@ -66,23 +66,23 @@
 * an *initiation rule*: producibility is initiated by the presence of nutrients, called *seeds*. 
 
 A metabolite that is producible from a set of nutrients is described as being "in the scope of the seeds".
 The computation is made using logic solvers (Answer Set Programming). The present modelling ignores the stoichiometry of reactions (2A + B --> C is considered equivalent to A + B --> C), and is therefore suited to non-curated or draft metabolic networks, as the ones built using M2M with the PathoLogic software of [Pathway Tools](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5036846/pdf/bbv079.pdf) handled by [Mpwt](https://github.com/AuReMe/mpwt). Many works have relied on network expansion to study organisms ([here](http://doi.wiley.com/10.1111/tpj.12627), [here](https://dx.plos.org/10.1371/journal.pcbi.1000049) or [there](http://dx.plos.org/10.1371/journal.pcbi.1005276)) and communities ([here](https://academic.oup.com/bioinformatics/article/34/17/i934/5093211), [here](https://bmcgenomics.biomedcentral.com/articles/10.1186/s12864-018-4786-7), or [here](https://www.ncbi.nlm.nih.gov/pubmed/18546499)). It has been [compared](http://www.ncbi.nlm.nih.gov/pubmed/19425125), [combined](https://www.cambridge.org/core/product/identifier/S1471068418000455/type/journal_article) to steady-state modelling (Flux Balance Analysis).
 
 ## License
 
-This project is licensed under the GNU Lesser General Public License - see the [LICENSE.md](https://github.com/AuReMe/metage2metabo/blob/master/LICENSE) file for details.
+This project is licensed under the GNU Lesser General Public License - see the [LICENSE.md](https://github.com/AuReMe/metage2metabo/blob/main/LICENSE) file for details.
 
 ## Documentation
 
 A more detailled documentation is available at: [https://metage2metabo.readthedocs.io](https://metage2metabo.readthedocs.io/en/latest/).
 
 ## Technologies
 
-Python 3 (Python 3.8 and 3.9 is tested). M2M uses a certain number of Python dependencies. An example of all these dependencies working for Ubuntu 18.04 is available in [requirements.txt](https://github.com/AuReMe/metage2metabo/blob/master/requirements.txt).
+Python 3 (Python 3.8 and 3.9 are tested). M2M uses a certain number of Python dependencies. An example of all these dependencies working for Ubuntu 18.04 is available in [requirements.txt](https://github.com/AuReMe/metage2metabo/blob/main/requirements.txt).
 They can be installed with:
 ````sh
 pip install -r requirements.txt --no-cache-dir
 ````
 In particular, m2m relies on:
 * [mpwt](https://github.com/AuReMe/mpwt) to automatize metabolic network reconstruction with Pathway Tools
 * [padmet](https://github.com/AuReMe/padmet) to manage metabolic networks
@@ -130,15 +130,15 @@
         ````sh
         echo 'export PATH="$PATH:your/install/directory/pathway-tools:"' >> ~/.bashrc
         ````
         Then source the bashrc file:
         ````sh
         source ~/.bashrc
 
-* [Oog Power Graph Command line tool](https://github.com/AuReMe/metage2metabo/tree/master/external_dependencies/Oog_CommandLineTool2012) to create a svg file from the compressed graph at the end of m2m_analysis. This tool is a jar file (``Oog.jar``) so Java is needed to use it.
+* [Oog Power Graph Command line tool](https://github.com/AuReMe/metage2metabo/tree/main/external_dependencies/Oog_CommandLineTool2012) to create a svg file from the compressed graph at the end of m2m_analysis. This tool is a jar file (``Oog.jar``) so Java is needed to use it.
 
 ## Installation
 
 Developed and tested on Linux (Ubuntu, Fedora, Debian) and MacOs (version 10.14) with Python3.8.
 
 Continuous Integration using GitHub Actions with Python3.8 and Python3.9 on ubuntu-latest, macos-latest and windows-latest ([corresponding virtual environment](https://docs.github.com/en/free-pro-team@latest/actions/reference/specifications-for-github-hosted-runners#supported-runners-and-hardware-resources)).
 
@@ -221,15 +221,15 @@
 
   {enum,graph,powergraph,workflow}
     enum                enumeration using miscoto
     graph               graph creation with enumeration solution
     powergraph          powergraph creation and visualization
     workflow            whole workflow
 
-Optional: Oog.jar file (https://github.com/AuReMe/metage2metabo/tree/master/external_dependencies) for powergraph svg creation.
+Optional: Oog.jar file (https://github.com/AuReMe/metage2metabo/tree/main/external_dependencies) for powergraph svg creation.
 ````
 
 ## Release Notes
 
 Changes between version are listed on the [release page](https://github.com/AuReMe/metage2metabo/releases).
 
 ## Additional features
@@ -284,17 +284,17 @@
 - ``ete3`` for taxonomic information used in power graphs:
 
 Huerta-Cepas J, Serra F, Bork P. ETE 3: Reconstruction, Analysis, and Visualization of Phylogenomic Data. Molecular Biology and Evolution 2016;33:1635–1638. [https://doi.org/10.1093/molbev/msw046](https://doi.org/10.1093/molbev/msw046).
 
 
 ## Article data
 
-Data used to create figures and tables are listed in the [article_data](https://github.com/AuReMe/metage2metabo/tree/master/article_data) folder, it contains:
+Data used to create figures and tables are listed in the [article_data](https://github.com/AuReMe/metage2metabo/tree/main/article_data) folder, it contains:
 
-- [gsmn_characteristics](https://github.com/AuReMe/metage2metabo/tree/master/article_data/gsmn_characteristics): scripts and tables to show the characteristics of draft metabolic networks created by M2M for gut, rumen and diabetes dataset.
-- [diabetes_study](https://github.com/AuReMe/metage2metabo/tree/master/article_data/diabetes_study): scripts and tables to create the figures of the diabetes analyses in the article.
+- [gsmn_characteristics](https://github.com/AuReMe/metage2metabo/tree/main/article_data/gsmn_characteristics): scripts and tables to show the characteristics of draft metabolic networks created by M2M for gut, rumen and diabetes dataset.
+- [diabetes_study](https://github.com/AuReMe/metage2metabo/tree/main/article_data/diabetes_study): scripts and tables to create the figures of the diabetes analyses in the article.
 
 ## Authors
 [Clémence Frioux](https://cfrioux.github.io/) and [Arnaud Belcour](https://arnaudbelcour.github.io/blog/), `Univ Bordeaux, Inria, INRAE, Bordeaux, France`, `Univ Grenoble Alpes, Inria, Grenoble, France` and `Univ Rennes, Inria, CNRS, IRISA, Rennes, France`.
 
 ## Acknowledgement
 People of Pathway Tools (SRI International) for their help integrating Pathway Tools with command line and multiprocessing in the [mpwt](https://github.com/AuReMe/mpwt) package, used in M2M.
```

### Comparing `Metage2Metabo-1.6.0/README.md` & `Metage2Metabo-1.6.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![PyPI version](https://img.shields.io/pypi/v/metage2metabo.svg)](https://pypi.org/project/Metage2Metabo/) [![GitHub license](https://img.shields.io/github/license/AuReMe/metage2metabo.svg)](https://github.com/AuReMe/metage2metabo/blob/master/LICENSE) [![Actions Status](https://github.com/AuReMe/metage2metabo/actions/workflows/pythonpackage.yml/badge.svg)](https://github.com/AuReMe/metage2metabo/actions/workflows/pythonpackage.yml) [![Documentation Status](https://readthedocs.org/projects/metage2metabo/badge/?version=latest)](https://metage2metabo.readthedocs.io/en/latest/?badge=latest) [![](https://img.shields.io/badge/doi-10.7554/eLife.61968-blueviolet.svg)](https://doi.org/10.7554/eLife.61968)
+[![PyPI version](https://img.shields.io/pypi/v/metage2metabo.svg)](https://pypi.org/project/Metage2Metabo/) [![GitHub license](https://img.shields.io/github/license/AuReMe/metage2metabo.svg)](https://github.com/AuReMe/metage2metabo/blob/main/LICENSE) [![Actions Status](https://github.com/AuReMe/metage2metabo/actions/workflows/pythonpackage.yml/badge.svg)](https://github.com/AuReMe/metage2metabo/actions/workflows/pythonpackage.yml) [![Documentation Status](https://readthedocs.org/projects/metage2metabo/badge/?version=latest)](https://metage2metabo.readthedocs.io/en/latest/?badge=latest) [![](https://img.shields.io/badge/doi-10.7554/eLife.61968-blueviolet.svg)](https://doi.org/10.7554/eLife.61968)
 
 # M2M - metage2metabo
 Metage2metabo is a Python3 (Python >= 3.8, tested with 3.8 and 3.9) tool to perform graph-based metabolic analysis starting from annotated genomes (**reference genomes or metagenome-assembled genomes**). It uses *Pathway Tools* in a automatic and parallel way to **reconstruct metabolic networks** for a large number of genomes. The obtained metabolic networks are then **analyzed individually and collectively** in order to get the **added value of metabolic cooperation in microbiota over individual metabolism** and to **identify and screen interesting organisms** among all.
 
 
 m2m can be used as a whole workflow (``` m2m workflow ```, ``` m2m metacom ```) or steps can be performed individually (``` m2m recon ``` , ``` m2m iscope ``` , ``` m2m cscope ```, ``` m2m addedvalue ```, ``` m2m mincom ```, ``` m2m seeds ```).
 
@@ -50,23 +50,23 @@
 * an *initiation rule*: producibility is initiated by the presence of nutrients, called *seeds*. 
 
 A metabolite that is producible from a set of nutrients is described as being "in the scope of the seeds".
 The computation is made using logic solvers (Answer Set Programming). The present modelling ignores the stoichiometry of reactions (2A + B --> C is considered equivalent to A + B --> C), and is therefore suited to non-curated or draft metabolic networks, as the ones built using M2M with the PathoLogic software of [Pathway Tools](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5036846/pdf/bbv079.pdf) handled by [Mpwt](https://github.com/AuReMe/mpwt). Many works have relied on network expansion to study organisms ([here](http://doi.wiley.com/10.1111/tpj.12627), [here](https://dx.plos.org/10.1371/journal.pcbi.1000049) or [there](http://dx.plos.org/10.1371/journal.pcbi.1005276)) and communities ([here](https://academic.oup.com/bioinformatics/article/34/17/i934/5093211), [here](https://bmcgenomics.biomedcentral.com/articles/10.1186/s12864-018-4786-7), or [here](https://www.ncbi.nlm.nih.gov/pubmed/18546499)). It has been [compared](http://www.ncbi.nlm.nih.gov/pubmed/19425125), [combined](https://www.cambridge.org/core/product/identifier/S1471068418000455/type/journal_article) to steady-state modelling (Flux Balance Analysis).
 
 ## License
 
-This project is licensed under the GNU Lesser General Public License - see the [LICENSE.md](https://github.com/AuReMe/metage2metabo/blob/master/LICENSE) file for details.
+This project is licensed under the GNU Lesser General Public License - see the [LICENSE.md](https://github.com/AuReMe/metage2metabo/blob/main/LICENSE) file for details.
 
 ## Documentation
 
 A more detailled documentation is available at: [https://metage2metabo.readthedocs.io](https://metage2metabo.readthedocs.io/en/latest/).
 
 ## Technologies
 
-Python 3 (Python 3.8 and 3.9 is tested). M2M uses a certain number of Python dependencies. An example of all these dependencies working for Ubuntu 18.04 is available in [requirements.txt](https://github.com/AuReMe/metage2metabo/blob/master/requirements.txt).
+Python 3 (Python 3.8 and 3.9 are tested). M2M uses a certain number of Python dependencies. An example of all these dependencies working for Ubuntu 18.04 is available in [requirements.txt](https://github.com/AuReMe/metage2metabo/blob/main/requirements.txt).
 They can be installed with:
 ````sh
 pip install -r requirements.txt --no-cache-dir
 ````
 In particular, m2m relies on:
 * [mpwt](https://github.com/AuReMe/mpwt) to automatize metabolic network reconstruction with Pathway Tools
 * [padmet](https://github.com/AuReMe/padmet) to manage metabolic networks
@@ -114,15 +114,15 @@
         ````sh
         echo 'export PATH="$PATH:your/install/directory/pathway-tools:"' >> ~/.bashrc
         ````
         Then source the bashrc file:
         ````sh
         source ~/.bashrc
 
-* [Oog Power Graph Command line tool](https://github.com/AuReMe/metage2metabo/tree/master/external_dependencies/Oog_CommandLineTool2012) to create a svg file from the compressed graph at the end of m2m_analysis. This tool is a jar file (``Oog.jar``) so Java is needed to use it.
+* [Oog Power Graph Command line tool](https://github.com/AuReMe/metage2metabo/tree/main/external_dependencies/Oog_CommandLineTool2012) to create a svg file from the compressed graph at the end of m2m_analysis. This tool is a jar file (``Oog.jar``) so Java is needed to use it.
 
 ## Installation
 
 Developed and tested on Linux (Ubuntu, Fedora, Debian) and MacOs (version 10.14) with Python3.8.
 
 Continuous Integration using GitHub Actions with Python3.8 and Python3.9 on ubuntu-latest, macos-latest and windows-latest ([corresponding virtual environment](https://docs.github.com/en/free-pro-team@latest/actions/reference/specifications-for-github-hosted-runners#supported-runners-and-hardware-resources)).
 
@@ -205,15 +205,15 @@
 
   {enum,graph,powergraph,workflow}
     enum                enumeration using miscoto
     graph               graph creation with enumeration solution
     powergraph          powergraph creation and visualization
     workflow            whole workflow
 
-Optional: Oog.jar file (https://github.com/AuReMe/metage2metabo/tree/master/external_dependencies) for powergraph svg creation.
+Optional: Oog.jar file (https://github.com/AuReMe/metage2metabo/tree/main/external_dependencies) for powergraph svg creation.
 ````
 
 ## Release Notes
 
 Changes between version are listed on the [release page](https://github.com/AuReMe/metage2metabo/releases).
 
 ## Additional features
@@ -268,17 +268,17 @@
 - ``ete3`` for taxonomic information used in power graphs:
 
 Huerta-Cepas J, Serra F, Bork P. ETE 3: Reconstruction, Analysis, and Visualization of Phylogenomic Data. Molecular Biology and Evolution 2016;33:1635–1638. [https://doi.org/10.1093/molbev/msw046](https://doi.org/10.1093/molbev/msw046).
 
 
 ## Article data
 
-Data used to create figures and tables are listed in the [article_data](https://github.com/AuReMe/metage2metabo/tree/master/article_data) folder, it contains:
+Data used to create figures and tables are listed in the [article_data](https://github.com/AuReMe/metage2metabo/tree/main/article_data) folder, it contains:
 
-- [gsmn_characteristics](https://github.com/AuReMe/metage2metabo/tree/master/article_data/gsmn_characteristics): scripts and tables to show the characteristics of draft metabolic networks created by M2M for gut, rumen and diabetes dataset.
-- [diabetes_study](https://github.com/AuReMe/metage2metabo/tree/master/article_data/diabetes_study): scripts and tables to create the figures of the diabetes analyses in the article.
+- [gsmn_characteristics](https://github.com/AuReMe/metage2metabo/tree/main/article_data/gsmn_characteristics): scripts and tables to show the characteristics of draft metabolic networks created by M2M for gut, rumen and diabetes dataset.
+- [diabetes_study](https://github.com/AuReMe/metage2metabo/tree/main/article_data/diabetes_study): scripts and tables to create the figures of the diabetes analyses in the article.
 
 ## Authors
 [Clémence Frioux](https://cfrioux.github.io/) and [Arnaud Belcour](https://arnaudbelcour.github.io/blog/), `Univ Bordeaux, Inria, INRAE, Bordeaux, France`, `Univ Grenoble Alpes, Inria, Grenoble, France` and `Univ Rennes, Inria, CNRS, IRISA, Rennes, France`.
 
 ## Acknowledgement
 People of Pathway Tools (SRI International) for their help integrating Pathway Tools with command line and multiprocessing in the [mpwt](https://github.com/AuReMe/mpwt) package, used in M2M.
```

### Comparing `Metage2Metabo-1.6.0/metage2metabo/__init__.py` & `Metage2Metabo-1.6.1/metage2metabo/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,10 +8,10 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Lesser General Public License for more details.
 
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>
 
-__version__ = '1.6.0'
+__version__ = '1.6.1'
 """ version of the package
 """
```

### Comparing `Metage2Metabo-1.6.0/metage2metabo/__main__.py` & `Metage2Metabo-1.6.1/metage2metabo/__main__.py`

 * *Files identical despite different names*

### Comparing `Metage2Metabo-1.6.0/metage2metabo/__main_analysis__.py` & `Metage2Metabo-1.6.1/metage2metabo/__main_analysis__.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 metage2metabo is free software: you are free to change and redistribute it.
 There is NO WARRANTY, to the extent permitted by law.\n
 """
 MESSAGE = """
 Detection of key species among communities.
 """
 REQUIRES = """
-Optional: Oog.jar file (https://github.com/AuReMe/metage2metabo/tree/master/external_dependencies) for powergraph svg creation.
+Optional: Oog.jar file (https://github.com/AuReMe/metage2metabo/tree/main/external_dependencies) for powergraph svg creation.
 """
 
 logger = logging.getLogger()
 logger.setLevel(logging.DEBUG)
 
 # Check ASP binaries.
 if not which('clingo'):
```

### Comparing `Metage2Metabo-1.6.0/metage2metabo/m2m/__init__.py` & `Metage2Metabo-1.6.1/metage2metabo/m2m/__init__.py`

 * *Files identical despite different names*

### Comparing `Metage2Metabo-1.6.0/metage2metabo/m2m/community_addedvalue.py` & `Metage2Metabo-1.6.1/metage2metabo/m2m/community_addedvalue.py`

 * *Files identical despite different names*

### Comparing `Metage2Metabo-1.6.0/metage2metabo/m2m/community_scope.py` & `Metage2Metabo-1.6.1/metage2metabo/m2m/community_scope.py`

 * *Files 4% similar despite different names*

```diff
@@ -130,14 +130,19 @@
         sys.exit(1)
 
     # Remove keys "host_prodtargets", "host_scope", "comhost_scope" and "host_unprodtargets" if there is no host:
     if host_mn is not None:
         scopes_results = run_scopes(lp_instance_file=instance)
         com_scope_dict = {}
         com_scope_dict['com_scope'] = scopes_results['com_scope']
+        com_scope_dict['host_prodtargets'] = scopes_results['host_prodtargets']
+        com_scope_dict['host_scope'] = scopes_results['host_scope']
+        com_scope_dict['comhost_scope'] = scopes_results['comhost_scope']
+        com_scope_dict['host_unprodtargets'] = scopes_results['host_unprodtargets']
+
         contributions_of_microbes = None
         logger.info('The computation of the community scope with a host is of limited functionality. It will not highlight the contribution of each microbe to the community scope. Additionally, the producibility of seeds by the microbes will not be computed. Consider running the community scope without a host (i.e. all metabolic networks, including the host, in the same directory) to get the full functionality of the community scope. \n')
         with open(com_scopes_path, 'w') as dumpfile:
             json.dump(com_scope_dict, dumpfile, indent=4, sort_keys=True)
         logger.info(f'Community scope for all metabolic networks available in {com_scopes_path}.\n')
         microbiota_scope = set(com_scope_dict['com_scope'])
     else:
```

### Comparing `Metage2Metabo-1.6.0/metage2metabo/m2m/individual_scope.py` & `Metage2Metabo-1.6.1/metage2metabo/m2m/individual_scope.py`

 * *Files identical despite different names*

### Comparing `Metage2Metabo-1.6.0/metage2metabo/m2m/m2m_workflow.py` & `Metage2Metabo-1.6.1/metage2metabo/m2m/m2m_workflow.py`

 * *Files identical despite different names*

### Comparing `Metage2Metabo-1.6.0/metage2metabo/m2m/minimal_community.py` & `Metage2Metabo-1.6.1/metage2metabo/m2m/minimal_community.py`

 * *Files identical despite different names*

### Comparing `Metage2Metabo-1.6.0/metage2metabo/m2m/reconstruction.py` & `Metage2Metabo-1.6.1/metage2metabo/m2m/reconstruction.py`

 * *Files identical despite different names*

### Comparing `Metage2Metabo-1.6.0/metage2metabo/m2m_analysis/__init__.py` & `Metage2Metabo-1.6.1/metage2metabo/m2m_analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `Metage2Metabo-1.6.0/metage2metabo/m2m_analysis/enumeration.py` & `Metage2Metabo-1.6.1/metage2metabo/m2m_analysis/enumeration.py`

 * *Files identical despite different names*

### Comparing `Metage2Metabo-1.6.0/metage2metabo/m2m_analysis/graph_compression.py` & `Metage2Metabo-1.6.1/metage2metabo/m2m_analysis/graph_compression.py`

 * *Files identical despite different names*

### Comparing `Metage2Metabo-1.6.0/metage2metabo/m2m_analysis/m2m_analysis_workflow.py` & `Metage2Metabo-1.6.1/metage2metabo/m2m_analysis/m2m_analysis_workflow.py`

 * *Files identical despite different names*

### Comparing `Metage2Metabo-1.6.0/metage2metabo/m2m_analysis/solution_graph.py` & `Metage2Metabo-1.6.1/metage2metabo/m2m_analysis/solution_graph.py`

 * *Files identical despite different names*

### Comparing `Metage2Metabo-1.6.0/metage2metabo/m2m_analysis/taxonomy.py` & `Metage2Metabo-1.6.1/metage2metabo/m2m_analysis/taxonomy.py`

 * *Files identical despite different names*

### Comparing `Metage2Metabo-1.6.0/metage2metabo/sbml_management.py` & `Metage2Metabo-1.6.1/metage2metabo/sbml_management.py`

 * *Files identical despite different names*

### Comparing `Metage2Metabo-1.6.0/metage2metabo/utils.py` & `Metage2Metabo-1.6.1/metage2metabo/utils.py`

 * *Files identical despite different names*

### Comparing `Metage2Metabo-1.6.0/metage2metabo/workflow_data/seeds_workflow.sbml` & `Metage2Metabo-1.6.1/metage2metabo/workflow_data/seeds_workflow.sbml`

 * *Files identical despite different names*

### Comparing `Metage2Metabo-1.6.0/metage2metabo/workflow_data/workflow_genomes.tar.gz` & `Metage2Metabo-1.6.1/metage2metabo/workflow_data/workflow_genomes.tar.gz`

 * *Files identical despite different names*

### Comparing `Metage2Metabo-1.6.0/pyproject.toml` & `Metage2Metabo-1.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Metage2Metabo-1.6.0/test/test_m2m_addedvalue.py` & `Metage2Metabo-1.6.1/test/test_m2m_addedvalue.py`

 * *Files identical despite different names*

### Comparing `Metage2Metabo-1.6.0/test/test_m2m_analysis.py` & `Metage2Metabo-1.6.1/test/test_m2m_analysis.py`

 * *Files identical despite different names*

### Comparing `Metage2Metabo-1.6.0/test/test_m2m_cscope.py` & `Metage2Metabo-1.6.1/test/test_m2m_cscope.py`

 * *Files identical despite different names*

### Comparing `Metage2Metabo-1.6.0/test/test_m2m_iscope.py` & `Metage2Metabo-1.6.1/test/test_m2m_iscope.py`

 * *Files identical despite different names*

### Comparing `Metage2Metabo-1.6.0/test/test_m2m_metacom.py` & `Metage2Metabo-1.6.1/test/test_m2m_metacom.py`

 * *Files identical despite different names*

### Comparing `Metage2Metabo-1.6.0/test/test_m2m_mincom.py` & `Metage2Metabo-1.6.1/test/test_m2m_mincom.py`

 * *Files identical despite different names*

### Comparing `Metage2Metabo-1.6.0/test/test_m2m_recon.py` & `Metage2Metabo-1.6.1/test/test_m2m_recon.py`

 * *Files identical despite different names*

### Comparing `Metage2Metabo-1.6.0/test/test_sbml_management.py` & `Metage2Metabo-1.6.1/test/test_sbml_management.py`

 * *Files identical despite different names*

### Comparing `Metage2Metabo-1.6.0/test/test_tiny_toy_metacom.py` & `Metage2Metabo-1.6.1/test/test_tiny_toy_metacom.py`

 * *Files 2% similar despite different names*

```diff
@@ -518,14 +518,24 @@
     # ensure the bacteria in union are ok
     assert set(mincom['union_bacteria']) == UNION_MINCOM
     # ensure the bacteria in intersection are ok
     assert set(mincom['inter_bacteria']) == INTERSECTION_MINCOM
     # ensure the newly producible targets are ok
     assert set(mincom['producible']) == PROD_TARGETS
 
+    comm_scopes_file = os.path.join(*[respath, 'community_analysis', 'comm_scopes.json'])
+    with open(comm_scopes_file, 'r') as json_cdata:
+        comm_scopes = json.load(json_cdata)
+
+    # Check host keys in comm_scopes json.
+    assert len(comm_scopes['com_scope']) == 13
+    assert set(comm_scopes['host_unprodtargets']) == set(['M_F_c', 'M_H_c', 'M_foo_c', 'M_C_c'])
+    # Host scope = old behavior, seed in scope.
+    assert set(comm_scopes['host_scope']) == set(['M_S1_c', 'M_S2_c'])
+
     # clean
     # Due to unstable behaviour of os.unlink on Windows, do not delete the file.
     # Refer to: https://github.com/python/cpython/issues/109608
     if sys.platform != 'win32':
         shutil.rmtree(respath)
```

