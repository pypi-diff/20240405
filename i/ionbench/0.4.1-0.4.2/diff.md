# Comparing `tmp/ionbench-0.4.1.tar.gz` & `tmp/ionbench-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ionbench-0.4.1.tar", last modified: Thu Apr  4 15:23:52 2024, max compression
+gzip compressed data, was "ionbench-0.4.2.tar", last modified: Fri Apr  5 15:58:00 2024, max compression
```

## Comparing `ionbench-0.4.1.tar` & `ionbench-0.4.2.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 15:23:52.557291 ionbench-0.4.1/
--rw-rw-rw-   0        0        0     1491 2023-09-15 08:58:40.000000 ionbench-0.4.1/LICENSE.txt
--rw-rw-rw-   0        0        0     5369 2024-04-04 15:23:52.551955 ionbench-0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     4404 2024-03-04 14:35:22.000000 ionbench-0.4.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-04 15:23:51.208842 ionbench-0.4.1/ionbench/
--rw-rw-rw-   0        0        0     2060 2024-02-19 17:13:07.000000 ionbench-0.4.1/ionbench/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 15:23:51.305537 ionbench-0.4.1/ionbench/benchmarker/
--rw-rw-rw-   0        0        0       48 2024-02-19 17:32:13.000000 ionbench-0.4.1/ionbench/benchmarker/__init__.py
--rw-rw-rw-   0        0        0    38265 2024-04-04 14:59:14.000000 ionbench-0.4.1/ionbench/benchmarker/benchmarker.py
-drwxrwxrwx   0        0        0        0 2024-04-04 15:23:51.139294 ionbench-0.4.1/ionbench/data/
-drwxrwxrwx   0        0        0        0 2024-04-04 15:23:51.378336 ionbench-0.4.1/ionbench/data/loewe2016/
--rw-rw-rw-   0        0        0     1902 2024-03-26 11:30:58.000000 ionbench-0.4.1/ionbench/data/loewe2016/courtemanche-1998-ikr.mmt
--rw-rw-rw-   0        0        0     2929 2024-03-25 13:04:48.000000 ionbench-0.4.1/ionbench/data/loewe2016/courtemanche-1998-ikur.mmt
--rw-rw-rw-   0        0        0   468578 2024-03-26 11:58:01.000000 ionbench-0.4.1/ionbench/data/loewe2016/ikr.csv
--rw-rw-rw-   0        0        0   483972 2024-03-26 10:27:20.000000 ionbench-0.4.1/ionbench/data/loewe2016/ikur.csv
-drwxrwxrwx   0        0        0        0 2024-04-04 15:23:51.401142 ionbench-0.4.1/ionbench/data/moreno2016/
--rw-rw-rw-   0        0        0      947 2024-01-31 11:58:14.000000 ionbench-0.4.1/ionbench/data/moreno2016/ina.csv
--rw-rw-rw-   0        0        0     2786 2024-02-20 17:22:01.000000 ionbench-0.4.1/ionbench/data/moreno2016/moreno2016.mmt
-drwxrwxrwx   0        0        0        0 2024-04-04 15:23:51.471706 ionbench-0.4.1/ionbench/data/staircase/
--rw-rw-rw-   0        0        0      838 2024-03-06 13:55:41.000000 ionbench-0.4.1/ionbench/data/staircase/beattie-2017-ikr-hh.mmt
--rw-rw-rw-   0        0        0   647878 2024-03-06 14:25:28.000000 ionbench-0.4.1/ionbench/data/staircase/dataHH.csv
--rw-rw-rw-   0        0        0   658551 2024-03-06 14:30:35.000000 ionbench-0.4.1/ionbench/data/staircase/dataMM.csv
--rw-rw-rw-   0        0        0     2254 2024-03-06 14:29:18.000000 ionbench-0.4.1/ionbench/data/staircase/fink-2008-ikr-mm.mmt
--rw-rw-rw-   0        0        0     1142 2024-03-06 14:06:01.000000 ionbench-0.4.1/ionbench/data/staircase/staircase-pace.mmt
-drwxrwxrwx   0        0        0        0 2024-04-04 15:23:51.492538 ionbench-0.4.1/ionbench/data/test/
--rw-rw-rw-   0        0        0      440 2023-11-23 15:28:16.000000 ionbench-0.4.1/ionbench/data/test/data.csv
-drwxrwxrwx   0        0        0        0 2024-04-04 15:23:51.528603 ionbench-0.4.1/ionbench/modification/
--rw-rw-rw-   0        0        0       50 2023-10-17 16:49:57.000000 ionbench-0.4.1/ionbench/modification/__init__.py
--rw-rw-rw-   0        0        0    16367 2024-03-21 12:50:48.000000 ionbench-0.4.1/ionbench/modification/modification.py
-drwxrwxrwx   0        0        0        0 2024-04-04 15:23:51.543301 ionbench-0.4.1/ionbench/optimisers/
--rw-rw-rw-   0        0        0      153 2023-10-26 10:28:33.000000 ionbench-0.4.1/ionbench/optimisers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 15:23:51.930328 ionbench-0.4.1/ionbench/optimisers/external_optimisers/
--rw-rw-rw-   0        0        0     5624 2024-03-21 12:57:10.000000 ionbench-0.4.1/ionbench/optimisers/external_optimisers/DE_Zhou2009.py
--rw-rw-rw-   0        0        0     2932 2024-03-21 12:57:09.000000 ionbench-0.4.1/ionbench/optimisers/external_optimisers/GA_Bot2012.py
--rw-rw-rw-   0        0        0     5153 2024-03-21 12:57:09.000000 ionbench-0.4.1/ionbench/optimisers/external_optimisers/GA_Cairns2017.py
--rw-rw-rw-   0        0        0     3726 2024-03-21 12:57:09.000000 ionbench-0.4.1/ionbench/optimisers/external_optimisers/GA_Gurkiewicz2007a.py
--rw-rw-rw-   0        0        0     3385 2024-03-21 12:57:09.000000 ionbench-0.4.1/ionbench/optimisers/external_optimisers/GA_Gurkiewicz2007b.py
--rw-rw-rw-   0        0        0     3223 2024-03-21 15:12:02.000000 ionbench-0.4.1/ionbench/optimisers/external_optimisers/GA_Smirnov2020.py
--rw-rw-rw-   0        0        0     2267 2024-03-25 15:28:47.000000 ionbench-0.4.1/ionbench/optimisers/external_optimisers/NMPSO_Clausen2020.py
--rw-rw-rw-   0        0        0    10669 2024-03-26 10:17:05.000000 ionbench-0.4.1/ionbench/optimisers/external_optimisers/NMPSO_Liu2011.py
--rw-rw-rw-   0        0        0     7970 2024-03-25 15:17:59.000000 ionbench-0.4.1/ionbench/optimisers/external_optimisers/PSOTRR_Loewe2016.py
--rw-rw-rw-   0        0        0     5530 2024-03-25 15:17:58.000000 ionbench-0.4.1/ionbench/optimisers/external_optimisers/PSO_Loewe2016.py
--rw-rw-rw-   0        0        0    10097 2024-03-21 13:12:06.000000 ionbench-0.4.1/ionbench/optimisers/external_optimisers/SA_Vanier1999.py
--rw-rw-rw-   0        0        0     4293 2024-03-21 13:12:06.000000 ionbench-0.4.1/ionbench/optimisers/external_optimisers/SPSA_Spall1998.py
--rw-rw-rw-   0        0        0     1491 2023-11-14 17:57:37.000000 ionbench-0.4.1/ionbench/optimisers/external_optimisers/__init__.py
--rw-rw-rw-   0        0        0    15056 2024-03-28 15:05:33.000000 ionbench-0.4.1/ionbench/optimisers/external_optimisers/curvilinearGD_Dokos2004.py
--rw-rw-rw-   0        0        0     8595 2024-03-25 15:17:59.000000 ionbench-0.4.1/ionbench/optimisers/external_optimisers/hybridPSOTRRTRR_Loewe2016.py
--rw-rw-rw-   0        0        0     7612 2024-03-25 15:17:58.000000 ionbench-0.4.1/ionbench/optimisers/external_optimisers/hybridPSOTRR_Loewe2016.py
--rw-rw-rw-   0        0        0     5125 2024-03-21 13:03:27.000000 ionbench-0.4.1/ionbench/optimisers/external_optimisers/patternSearch_Kohjitani2022.py
--rw-rw-rw-   0        0        0     9131 2024-03-25 15:33:26.000000 ionbench-0.4.1/ionbench/optimisers/external_optimisers/ppso_Chen2012.py
--rw-rw-rw-   0        0        0     6752 2024-03-25 15:52:04.000000 ionbench-0.4.1/ionbench/optimisers/external_optimisers/pso_Cabo2022.py
--rw-rw-rw-   0        0        0     4418 2024-03-26 10:13:34.000000 ionbench-0.4.1/ionbench/optimisers/external_optimisers/pso_Seemann2009.py
--rw-rw-rw-   0        0        0     2183 2024-03-21 15:19:01.000000 ionbench-0.4.1/ionbench/optimisers/external_optimisers/randomSearch_Vanier1999.py
--rw-rw-rw-   0        0        0     2685 2024-03-21 13:11:58.000000 ionbench-0.4.1/ionbench/optimisers/external_optimisers/stochasticSearch_Vanier1999.py
-drwxrwxrwx   0        0        0        0 2024-04-04 15:23:52.020763 ionbench-0.4.1/ionbench/optimisers/pints_optimisers/
--rw-rw-rw-   0        0        0      311 2023-08-23 14:25:17.000000 ionbench-0.4.1/ionbench/optimisers/pints_optimisers/__init__.py
--rw-rw-rw-   0        0        0     1937 2024-03-21 16:56:40.000000 ionbench-0.4.1/ionbench/optimisers/pints_optimisers/cmaes_pints.py
--rw-rw-rw-   0        0        0     1638 2024-03-21 16:56:40.000000 ionbench-0.4.1/ionbench/optimisers/pints_optimisers/nelderMead_pints.py
--rw-rw-rw-   0        0        0     1611 2024-03-21 16:56:40.000000 ionbench-0.4.1/ionbench/optimisers/pints_optimisers/pso_pints.py
--rw-rw-rw-   0        0        0     1623 2024-03-21 16:56:40.000000 ionbench-0.4.1/ionbench/optimisers/pints_optimisers/snes_pints.py
--rw-rw-rw-   0        0        0     1625 2024-03-21 16:56:40.000000 ionbench-0.4.1/ionbench/optimisers/pints_optimisers/xnes_pints.py
-drwxrwxrwx   0        0        0        0 2024-04-04 15:23:52.120826 ionbench-0.4.1/ionbench/optimisers/scipy_optimisers/
--rw-rw-rw-   0        0        0      397 2023-11-14 13:29:40.000000 ionbench-0.4.1/ionbench/optimisers/scipy_optimisers/__init__.py
--rw-rw-rw-   0        0        0     2312 2024-03-21 13:11:58.000000 ionbench-0.4.1/ionbench/optimisers/scipy_optimisers/conjugateGD_scipy.py
--rw-rw-rw-   0        0        0     1770 2024-03-28 14:52:14.000000 ionbench-0.4.1/ionbench/optimisers/scipy_optimisers/lm_scipy.py
--rw-rw-rw-   0        0        0     2900 2024-03-21 16:55:00.000000 ionbench-0.4.1/ionbench/optimisers/scipy_optimisers/nelderMead_scipy.py
--rw-rw-rw-   0        0        0     2905 2024-03-21 16:55:01.000000 ionbench-0.4.1/ionbench/optimisers/scipy_optimisers/powell_scipy.py
--rw-rw-rw-   0        0        0     2320 2024-03-21 16:55:01.000000 ionbench-0.4.1/ionbench/optimisers/scipy_optimisers/slsqp_scipy.py
--rw-rw-rw-   0        0        0     2009 2024-03-28 14:52:14.000000 ionbench-0.4.1/ionbench/optimisers/scipy_optimisers/trustRegionReflective_scipy.py
-drwxrwxrwx   0        0        0        0 2024-04-04 15:23:52.187777 ionbench-0.4.1/ionbench/problems/
--rw-rw-rw-   0        0        0      160 2023-11-23 15:25:37.000000 ionbench-0.4.1/ionbench/problems/__init__.py
--rw-rw-rw-   0        0        0     8195 2024-03-28 13:37:02.000000 ionbench-0.4.1/ionbench/problems/loewe2016.py
--rw-rw-rw-   0        0        0    17417 2024-03-28 13:37:02.000000 ionbench-0.4.1/ionbench/problems/moreno2016.py
--rw-rw-rw-   0        0        0     9604 2024-03-28 13:37:02.000000 ionbench-0.4.1/ionbench/problems/staircase.py
--rw-rw-rw-   0        0        0     5839 2024-03-21 12:50:42.000000 ionbench-0.4.1/ionbench/problems/test.py
-drwxrwxrwx   0        0        0        0 2024-04-04 15:23:52.212627 ionbench-0.4.1/ionbench/tracker/
--rw-rw-rw-   0        0        0       40 2024-02-19 17:33:47.000000 ionbench-0.4.1/ionbench/tracker/__init__.py
--rw-rw-rw-   0        0        0    16857 2024-03-28 13:43:43.000000 ionbench-0.4.1/ionbench/tracker/tracker.py
-drwxrwxrwx   0        0        0        0 2024-04-04 15:23:52.259804 ionbench-0.4.1/ionbench/uncertainty/
--rw-rw-rw-   0        0        0       91 2023-09-08 12:44:51.000000 ionbench-0.4.1/ionbench/uncertainty/__init__.py
--rw-rw-rw-   0        0        0     7060 2024-03-21 12:36:02.000000 ionbench-0.4.1/ionbench/uncertainty/fim.py
--rw-rw-rw-   0        0        0    12104 2024-03-27 11:54:37.000000 ionbench-0.4.1/ionbench/uncertainty/profile_likelihood.py
-drwxrwxrwx   0        0        0        0 2024-04-04 15:23:52.456807 ionbench-0.4.1/ionbench/utils/
--rw-rw-rw-   0        0        0      259 2024-03-22 14:22:36.000000 ionbench-0.4.1/ionbench/utils/__init__.py
--rw-rw-rw-   0        0        0     7768 2024-03-21 12:50:42.000000 ionbench-0.4.1/ionbench/utils/autodiff.py
--rw-rw-rw-   0        0        0     1590 2024-03-20 15:36:43.000000 ionbench-0.4.1/ionbench/utils/cache.py
--rw-rw-rw-   0        0        0     4805 2024-03-28 13:55:01.000000 ionbench-0.4.1/ionbench/utils/classes_pints.py
--rw-rw-rw-   0        0        0     1516 2024-02-12 13:34:30.000000 ionbench-0.4.1/ionbench/utils/multistart.py
--rw-rw-rw-   0        0        0     2544 2024-03-26 09:47:49.000000 ionbench-0.4.1/ionbench/utils/particle_optimisers.py
--rw-rw-rw-   0        0        0     7625 2024-03-25 15:28:47.000000 ionbench-0.4.1/ionbench/utils/population_optimisers.py
--rw-rw-rw-   0        0        0     2460 2024-04-04 08:48:53.000000 ionbench-0.4.1/ionbench/utils/scipy_setup.py
-drwxrwxrwx   0        0        0        0 2024-04-04 15:23:52.543711 ionbench-0.4.1/ionbench.egg-info/
--rw-rw-rw-   0        0        0     5369 2024-04-04 15:23:50.000000 ionbench-0.4.1/ionbench.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3565 2024-04-04 15:23:51.000000 ionbench-0.4.1/ionbench.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 15:23:50.000000 ionbench-0.4.1/ionbench.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       94 2024-04-04 15:23:50.000000 ionbench-0.4.1/ionbench.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-04 15:23:50.000000 ionbench-0.4.1/ionbench.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-04 15:23:52.558336 ionbench-0.4.1/setup.cfg
--rw-rw-rw-   0        0        0     8469 2024-04-04 15:02:07.000000 ionbench-0.4.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-04 15:23:52.533715 ionbench-0.4.1/test/
--rw-rw-rw-   0        0        0     5403 2024-03-08 13:55:46.000000 ionbench-0.4.1/test/test_modifications.py
--rw-rw-rw-   0        0        0      542 2024-03-05 15:24:03.000000 ionbench-0.4.1/test/test_multistart.py
--rw-rw-rw-   0        0        0     2052 2024-03-26 10:22:59.000000 ionbench-0.4.1/test/test_optimisers.py
--rw-rw-rw-   0        0        0    29511 2024-03-28 14:36:40.000000 ionbench-0.4.1/test/test_problems.py
--rw-rw-rw-   0        0        0      773 2024-02-20 17:03:12.000000 ionbench-0.4.1/test/test_uncertainty.py
+drwxrwxrwx   0        0        0        0 2024-04-05 15:58:00.267327 ionbench-0.4.2/
+-rw-rw-rw-   0        0        0     1491 2023-09-15 08:58:40.000000 ionbench-0.4.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     5369 2024-04-05 15:58:00.257357 ionbench-0.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4404 2024-03-04 14:35:22.000000 ionbench-0.4.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-05 15:57:58.398327 ionbench-0.4.2/ionbench/
+-rw-rw-rw-   0        0        0     2060 2024-02-19 17:13:07.000000 ionbench-0.4.2/ionbench/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 15:57:58.547619 ionbench-0.4.2/ionbench/benchmarker/
+-rw-rw-rw-   0        0        0       48 2024-02-19 17:32:13.000000 ionbench-0.4.2/ionbench/benchmarker/__init__.py
+-rw-rw-rw-   0        0        0    38265 2024-04-04 14:59:14.000000 ionbench-0.4.2/ionbench/benchmarker/benchmarker.py
+drwxrwxrwx   0        0        0        0 2024-04-05 15:57:58.309470 ionbench-0.4.2/ionbench/data/
+drwxrwxrwx   0        0        0        0 2024-04-05 15:57:58.643812 ionbench-0.4.2/ionbench/data/loewe2016/
+-rw-rw-rw-   0        0        0     1902 2024-03-26 11:30:58.000000 ionbench-0.4.2/ionbench/data/loewe2016/courtemanche-1998-ikr.mmt
+-rw-rw-rw-   0        0        0     2929 2024-03-25 13:04:48.000000 ionbench-0.4.2/ionbench/data/loewe2016/courtemanche-1998-ikur.mmt
+-rw-rw-rw-   0        0        0   468578 2024-03-26 11:58:01.000000 ionbench-0.4.2/ionbench/data/loewe2016/ikr.csv
+-rw-rw-rw-   0        0        0   483972 2024-03-26 10:27:20.000000 ionbench-0.4.2/ionbench/data/loewe2016/ikur.csv
+drwxrwxrwx   0        0        0        0 2024-04-05 15:57:58.697722 ionbench-0.4.2/ionbench/data/moreno2016/
+-rw-rw-rw-   0        0        0      947 2024-01-31 11:58:14.000000 ionbench-0.4.2/ionbench/data/moreno2016/ina.csv
+-rw-rw-rw-   0        0        0     2786 2024-02-20 17:22:01.000000 ionbench-0.4.2/ionbench/data/moreno2016/moreno2016.mmt
+drwxrwxrwx   0        0        0        0 2024-04-05 15:57:58.772463 ionbench-0.4.2/ionbench/data/staircase/
+-rw-rw-rw-   0        0        0      838 2024-03-06 13:55:41.000000 ionbench-0.4.2/ionbench/data/staircase/beattie-2017-ikr-hh.mmt
+-rw-rw-rw-   0        0        0   647878 2024-03-06 14:25:28.000000 ionbench-0.4.2/ionbench/data/staircase/dataHH.csv
+-rw-rw-rw-   0        0        0   658551 2024-03-06 14:30:35.000000 ionbench-0.4.2/ionbench/data/staircase/dataMM.csv
+-rw-rw-rw-   0        0        0     2254 2024-03-06 14:29:18.000000 ionbench-0.4.2/ionbench/data/staircase/fink-2008-ikr-mm.mmt
+-rw-rw-rw-   0        0        0     1142 2024-03-06 14:06:01.000000 ionbench-0.4.2/ionbench/data/staircase/staircase-pace.mmt
+drwxrwxrwx   0        0        0        0 2024-04-05 15:57:58.792975 ionbench-0.4.2/ionbench/data/test/
+-rw-rw-rw-   0        0        0      440 2023-11-23 15:28:16.000000 ionbench-0.4.2/ionbench/data/test/data.csv
+drwxrwxrwx   0        0        0        0 2024-04-05 15:57:58.839650 ionbench-0.4.2/ionbench/modification/
+-rw-rw-rw-   0        0        0       50 2023-10-17 16:49:57.000000 ionbench-0.4.2/ionbench/modification/__init__.py
+-rw-rw-rw-   0        0        0    16367 2024-03-21 12:50:48.000000 ionbench-0.4.2/ionbench/modification/modification.py
+drwxrwxrwx   0        0        0        0 2024-04-05 15:57:58.865497 ionbench-0.4.2/ionbench/optimisers/
+-rw-rw-rw-   0        0        0      153 2023-10-26 10:28:33.000000 ionbench-0.4.2/ionbench/optimisers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 15:57:59.382740 ionbench-0.4.2/ionbench/optimisers/external_optimisers/
+-rw-rw-rw-   0        0        0     5632 2024-04-05 09:00:28.000000 ionbench-0.4.2/ionbench/optimisers/external_optimisers/DE_Zhou2009.py
+-rw-rw-rw-   0        0        0     2932 2024-03-21 12:57:09.000000 ionbench-0.4.2/ionbench/optimisers/external_optimisers/GA_Bot2012.py
+-rw-rw-rw-   0        0        0     5153 2024-03-21 12:57:09.000000 ionbench-0.4.2/ionbench/optimisers/external_optimisers/GA_Cairns2017.py
+-rw-rw-rw-   0        0        0     3726 2024-03-21 12:57:09.000000 ionbench-0.4.2/ionbench/optimisers/external_optimisers/GA_Gurkiewicz2007a.py
+-rw-rw-rw-   0        0        0     3385 2024-03-21 12:57:09.000000 ionbench-0.4.2/ionbench/optimisers/external_optimisers/GA_Gurkiewicz2007b.py
+-rw-rw-rw-   0        0        0     3223 2024-03-21 15:12:02.000000 ionbench-0.4.2/ionbench/optimisers/external_optimisers/GA_Smirnov2020.py
+-rw-rw-rw-   0        0        0     2267 2024-03-25 15:28:47.000000 ionbench-0.4.2/ionbench/optimisers/external_optimisers/NMPSO_Clausen2020.py
+-rw-rw-rw-   0        0        0    10669 2024-03-26 10:17:05.000000 ionbench-0.4.2/ionbench/optimisers/external_optimisers/NMPSO_Liu2011.py
+-rw-rw-rw-   0        0        0     7970 2024-03-25 15:17:59.000000 ionbench-0.4.2/ionbench/optimisers/external_optimisers/PSOTRR_Loewe2016.py
+-rw-rw-rw-   0        0        0     5530 2024-03-25 15:17:58.000000 ionbench-0.4.2/ionbench/optimisers/external_optimisers/PSO_Loewe2016.py
+-rw-rw-rw-   0        0        0    10097 2024-03-21 13:12:06.000000 ionbench-0.4.2/ionbench/optimisers/external_optimisers/SA_Vanier1999.py
+-rw-rw-rw-   0        0        0     4293 2024-03-21 13:12:06.000000 ionbench-0.4.2/ionbench/optimisers/external_optimisers/SPSA_Spall1998.py
+-rw-rw-rw-   0        0        0     1491 2023-11-14 17:57:37.000000 ionbench-0.4.2/ionbench/optimisers/external_optimisers/__init__.py
+-rw-rw-rw-   0        0        0    15056 2024-03-28 15:05:33.000000 ionbench-0.4.2/ionbench/optimisers/external_optimisers/curvilinearGD_Dokos2004.py
+-rw-rw-rw-   0        0        0     8595 2024-03-25 15:17:59.000000 ionbench-0.4.2/ionbench/optimisers/external_optimisers/hybridPSOTRRTRR_Loewe2016.py
+-rw-rw-rw-   0        0        0     7612 2024-03-25 15:17:58.000000 ionbench-0.4.2/ionbench/optimisers/external_optimisers/hybridPSOTRR_Loewe2016.py
+-rw-rw-rw-   0        0        0     5125 2024-03-21 13:03:27.000000 ionbench-0.4.2/ionbench/optimisers/external_optimisers/patternSearch_Kohjitani2022.py
+-rw-rw-rw-   0        0        0     9131 2024-03-25 15:33:26.000000 ionbench-0.4.2/ionbench/optimisers/external_optimisers/ppso_Chen2012.py
+-rw-rw-rw-   0        0        0     6680 2024-04-05 09:00:28.000000 ionbench-0.4.2/ionbench/optimisers/external_optimisers/pso_Cabo2022.py
+-rw-rw-rw-   0        0        0     4418 2024-03-26 10:13:34.000000 ionbench-0.4.2/ionbench/optimisers/external_optimisers/pso_Seemann2009.py
+-rw-rw-rw-   0        0        0     2183 2024-03-21 15:19:01.000000 ionbench-0.4.2/ionbench/optimisers/external_optimisers/randomSearch_Vanier1999.py
+-rw-rw-rw-   0        0        0     3221 2024-04-05 12:40:19.000000 ionbench-0.4.2/ionbench/optimisers/external_optimisers/stochasticSearch_Vanier1999.py
+drwxrwxrwx   0        0        0        0 2024-04-05 15:57:59.521098 ionbench-0.4.2/ionbench/optimisers/pints_optimisers/
+-rw-rw-rw-   0        0        0      311 2023-08-23 14:25:17.000000 ionbench-0.4.2/ionbench/optimisers/pints_optimisers/__init__.py
+-rw-rw-rw-   0        0        0     1937 2024-03-21 16:56:40.000000 ionbench-0.4.2/ionbench/optimisers/pints_optimisers/cmaes_pints.py
+-rw-rw-rw-   0        0        0     1638 2024-03-21 16:56:40.000000 ionbench-0.4.2/ionbench/optimisers/pints_optimisers/nelderMead_pints.py
+-rw-rw-rw-   0        0        0     1611 2024-03-21 16:56:40.000000 ionbench-0.4.2/ionbench/optimisers/pints_optimisers/pso_pints.py
+-rw-rw-rw-   0        0        0     1623 2024-03-21 16:56:40.000000 ionbench-0.4.2/ionbench/optimisers/pints_optimisers/snes_pints.py
+-rw-rw-rw-   0        0        0     1625 2024-03-21 16:56:40.000000 ionbench-0.4.2/ionbench/optimisers/pints_optimisers/xnes_pints.py
+drwxrwxrwx   0        0        0        0 2024-04-05 15:57:59.677281 ionbench-0.4.2/ionbench/optimisers/scipy_optimisers/
+-rw-rw-rw-   0        0        0      397 2023-11-14 13:29:40.000000 ionbench-0.4.2/ionbench/optimisers/scipy_optimisers/__init__.py
+-rw-rw-rw-   0        0        0     2312 2024-03-21 13:11:58.000000 ionbench-0.4.2/ionbench/optimisers/scipy_optimisers/conjugateGD_scipy.py
+-rw-rw-rw-   0        0        0     1770 2024-03-28 14:52:14.000000 ionbench-0.4.2/ionbench/optimisers/scipy_optimisers/lm_scipy.py
+-rw-rw-rw-   0        0        0     2900 2024-03-21 16:55:00.000000 ionbench-0.4.2/ionbench/optimisers/scipy_optimisers/nelderMead_scipy.py
+-rw-rw-rw-   0        0        0     2905 2024-03-21 16:55:01.000000 ionbench-0.4.2/ionbench/optimisers/scipy_optimisers/powell_scipy.py
+-rw-rw-rw-   0        0        0     2320 2024-03-21 16:55:01.000000 ionbench-0.4.2/ionbench/optimisers/scipy_optimisers/slsqp_scipy.py
+-rw-rw-rw-   0        0        0     2009 2024-03-28 14:52:14.000000 ionbench-0.4.2/ionbench/optimisers/scipy_optimisers/trustRegionReflective_scipy.py
+drwxrwxrwx   0        0        0        0 2024-04-05 15:57:59.790619 ionbench-0.4.2/ionbench/problems/
+-rw-rw-rw-   0        0        0      160 2023-11-23 15:25:37.000000 ionbench-0.4.2/ionbench/problems/__init__.py
+-rw-rw-rw-   0        0        0     8195 2024-03-28 13:37:02.000000 ionbench-0.4.2/ionbench/problems/loewe2016.py
+-rw-rw-rw-   0        0        0    17417 2024-03-28 13:37:02.000000 ionbench-0.4.2/ionbench/problems/moreno2016.py
+-rw-rw-rw-   0        0        0     9604 2024-03-28 13:37:02.000000 ionbench-0.4.2/ionbench/problems/staircase.py
+-rw-rw-rw-   0        0        0     5839 2024-03-21 12:50:42.000000 ionbench-0.4.2/ionbench/problems/test.py
+drwxrwxrwx   0        0        0        0 2024-04-05 15:57:59.826542 ionbench-0.4.2/ionbench/tracker/
+-rw-rw-rw-   0        0        0       40 2024-02-19 17:33:47.000000 ionbench-0.4.2/ionbench/tracker/__init__.py
+-rw-rw-rw-   0        0        0    16883 2024-04-05 09:42:13.000000 ionbench-0.4.2/ionbench/tracker/tracker.py
+drwxrwxrwx   0        0        0        0 2024-04-05 15:57:59.897269 ionbench-0.4.2/ionbench/uncertainty/
+-rw-rw-rw-   0        0        0       91 2023-09-08 12:44:51.000000 ionbench-0.4.2/ionbench/uncertainty/__init__.py
+-rw-rw-rw-   0        0        0     7060 2024-03-21 12:36:02.000000 ionbench-0.4.2/ionbench/uncertainty/fim.py
+-rw-rw-rw-   0        0        0    12104 2024-03-27 11:54:37.000000 ionbench-0.4.2/ionbench/uncertainty/profile_likelihood.py
+drwxrwxrwx   0        0        0        0 2024-04-05 15:58:00.121371 ionbench-0.4.2/ionbench/utils/
+-rw-rw-rw-   0        0        0      259 2024-03-22 14:22:36.000000 ionbench-0.4.2/ionbench/utils/__init__.py
+-rw-rw-rw-   0        0        0     7768 2024-03-21 12:50:42.000000 ionbench-0.4.2/ionbench/utils/autodiff.py
+-rw-rw-rw-   0        0        0     1590 2024-03-20 15:36:43.000000 ionbench-0.4.2/ionbench/utils/cache.py
+-rw-rw-rw-   0        0        0     4897 2024-04-05 08:53:05.000000 ionbench-0.4.2/ionbench/utils/classes_pints.py
+-rw-rw-rw-   0        0        0     1516 2024-02-12 13:34:30.000000 ionbench-0.4.2/ionbench/utils/multistart.py
+-rw-rw-rw-   0        0        0     2544 2024-03-26 09:47:49.000000 ionbench-0.4.2/ionbench/utils/particle_optimisers.py
+-rw-rw-rw-   0        0        0     7625 2024-03-25 15:28:47.000000 ionbench-0.4.2/ionbench/utils/population_optimisers.py
+-rw-rw-rw-   0        0        0     2460 2024-04-05 15:06:52.000000 ionbench-0.4.2/ionbench/utils/scipy_setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 15:58:00.243783 ionbench-0.4.2/ionbench.egg-info/
+-rw-rw-rw-   0        0        0     5369 2024-04-05 15:57:58.000000 ionbench-0.4.2/ionbench.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3565 2024-04-05 15:57:58.000000 ionbench-0.4.2/ionbench.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 15:57:58.000000 ionbench-0.4.2/ionbench.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2024-04-05 15:57:58.000000 ionbench-0.4.2/ionbench.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-05 15:57:58.000000 ionbench-0.4.2/ionbench.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-05 15:58:00.269474 ionbench-0.4.2/setup.cfg
+-rw-rw-rw-   0        0        0     8469 2024-04-05 15:47:35.000000 ionbench-0.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 15:58:00.230158 ionbench-0.4.2/test/
+-rw-rw-rw-   0        0        0     5403 2024-03-08 13:55:46.000000 ionbench-0.4.2/test/test_modifications.py
+-rw-rw-rw-   0        0        0      542 2024-03-05 15:24:03.000000 ionbench-0.4.2/test/test_multistart.py
+-rw-rw-rw-   0        0        0     2052 2024-03-26 10:22:59.000000 ionbench-0.4.2/test/test_optimisers.py
+-rw-rw-rw-   0        0        0    29511 2024-03-28 14:36:40.000000 ionbench-0.4.2/test/test_problems.py
+-rw-rw-rw-   0        0        0      773 2024-02-20 17:03:12.000000 ionbench-0.4.2/test/test_uncertainty.py
```

### Comparing `ionbench-0.4.1/LICENSE.txt` & `ionbench-0.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.1/PKG-INFO` & `ionbench-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ionbench
-Version: 0.4.1
+Version: 0.4.2
 Summary: A benchmarking tool for comparing different parameter optimization algorithms for ion channel models
 Home-page: https://github.com/CardiacModelling/ionbench
 Author: Matt J. Owen
 Author-email: matt.owen@nottingham.ac.uk
 Project-URL: Bug Reports, https://github.com/CardiacModelling/ionbench/issues
 Project-URL: Source, https://github.com/CardiacModelling/ionbench
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ionbench-0.4.1/README.md` & `ionbench-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.1/ionbench/__init__.py` & `ionbench-0.4.2/ionbench/__init__.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.1/ionbench/benchmarker/benchmarker.py` & `ionbench-0.4.2/ionbench/benchmarker/benchmarker.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.1/ionbench/data/loewe2016/courtemanche-1998-ikr.mmt` & `ionbench-0.4.2/ionbench/data/loewe2016/courtemanche-1998-ikr.mmt`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.1/ionbench/data/loewe2016/courtemanche-1998-ikur.mmt` & `ionbench-0.4.2/ionbench/data/loewe2016/courtemanche-1998-ikur.mmt`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.1/ionbench/data/loewe2016/ikr.csv` & `ionbench-0.4.2/ionbench/data/loewe2016/ikr.csv`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.1/ionbench/data/loewe2016/ikur.csv` & `ionbench-0.4.2/ionbench/data/loewe2016/ikur.csv`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.1/ionbench/data/moreno2016/ina.csv` & `ionbench-0.4.2/ionbench/data/moreno2016/ina.csv`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.1/ionbench/data/moreno2016/moreno2016.mmt` & `ionbench-0.4.2/ionbench/data/moreno2016/moreno2016.mmt`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.1/ionbench/data/staircase/beattie-2017-ikr-hh.mmt` & `ionbench-0.4.2/ionbench/data/staircase/beattie-2017-ikr-hh.mmt`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.1/ionbench/data/staircase/dataHH.csv` & `ionbench-0.4.2/ionbench/data/staircase/dataHH.csv`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.1/ionbench/data/staircase/dataMM.csv` & `ionbench-0.4.2/ionbench/data/staircase/dataMM.csv`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.1/ionbench/data/staircase/fink-2008-ikr-mm.mmt` & `ionbench-0.4.2/ionbench/data/staircase/fink-2008-ikr-mm.mmt`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.1/ionbench/data/staircase/staircase-pace.mmt` & `ionbench-0.4.2/ionbench/data/staircase/staircase-pace.mmt`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.1/ionbench/modification/modification.py` & `ionbench-0.4.2/ionbench/modification/modification.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.1/ionbench/optimisers/external_optimisers/DE_Zhou2009.py` & `ionbench-0.4.2/ionbench/optimisers/external_optimisers/DE_Zhou2009.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,17 +60,17 @@
     # Generate initial population
     pop = [None] * popSize
     for i in range(popSize):
         pop[i] = Individual()
         pop[i].find_cost()
 
     for gen in range(nGens):
-        print('----------------')
-        print(f'Generation {gen} of {nGens}')
         if debug:
+            print('----------------')
+            print(f'Generation {gen} of {nGens}')
             costMean = 0
             for p in pop:
                 costMean += p.cost / popSize
             print(f'Average cost is {costMean}')
         if gen > 0 and gen % 1000 == 0:
             # Run lm on each point
             if debug:
```

### Comparing `ionbench-0.4.1/ionbench/optimisers/external_optimisers/GA_Bot2012.py` & `ionbench-0.4.2/ionbench/optimisers/external_optimisers/GA_Bot2012.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.1/ionbench/optimisers/external_optimisers/GA_Cairns2017.py` & `ionbench-0.4.2/ionbench/optimisers/external_optimisers/GA_Cairns2017.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.1/ionbench/optimisers/external_optimisers/GA_Gurkiewicz2007a.py` & `ionbench-0.4.2/ionbench/optimisers/external_optimisers/GA_Gurkiewicz2007a.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.1/ionbench/optimisers/external_optimisers/GA_Gurkiewicz2007b.py` & `ionbench-0.4.2/ionbench/optimisers/external_optimisers/GA_Gurkiewicz2007b.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.1/ionbench/optimisers/external_optimisers/GA_Smirnov2020.py` & `ionbench-0.4.2/ionbench/optimisers/external_optimisers/GA_Smirnov2020.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.1/ionbench/optimisers/external_optimisers/NMPSO_Clausen2020.py` & `ionbench-0.4.2/ionbench/optimisers/external_optimisers/NMPSO_Clausen2020.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.1/ionbench/optimisers/external_optimisers/NMPSO_Liu2011.py` & `ionbench-0.4.2/ionbench/optimisers/external_optimisers/NMPSO_Liu2011.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.1/ionbench/optimisers/external_optimisers/PSOTRR_Loewe2016.py` & `ionbench-0.4.2/ionbench/optimisers/external_optimisers/PSOTRR_Loewe2016.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.1/ionbench/optimisers/external_optimisers/PSO_Loewe2016.py` & `ionbench-0.4.2/ionbench/optimisers/external_optimisers/PSO_Loewe2016.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.1/ionbench/optimisers/external_optimisers/SA_Vanier1999.py` & `ionbench-0.4.2/ionbench/optimisers/external_optimisers/SA_Vanier1999.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.1/ionbench/optimisers/external_optimisers/SPSA_Spall1998.py` & `ionbench-0.4.2/ionbench/optimisers/external_optimisers/SPSA_Spall1998.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.1/ionbench/optimisers/external_optimisers/__init__.py` & `ionbench-0.4.2/ionbench/optimisers/external_optimisers/__init__.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.1/ionbench/optimisers/external_optimisers/curvilinearGD_Dokos2004.py` & `ionbench-0.4.2/ionbench/optimisers/external_optimisers/curvilinearGD_Dokos2004.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.1/ionbench/optimisers/external_optimisers/hybridPSOTRRTRR_Loewe2016.py` & `ionbench-0.4.2/ionbench/optimisers/external_optimisers/hybridPSOTRRTRR_Loewe2016.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.1/ionbench/optimisers/external_optimisers/hybridPSOTRR_Loewe2016.py` & `ionbench-0.4.2/ionbench/optimisers/external_optimisers/hybridPSOTRR_Loewe2016.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.1/ionbench/optimisers/external_optimisers/patternSearch_Kohjitani2022.py` & `ionbench-0.4.2/ionbench/optimisers/external_optimisers/patternSearch_Kohjitani2022.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.1/ionbench/optimisers/external_optimisers/ppso_Chen2012.py` & `ionbench-0.4.2/ionbench/optimisers/external_optimisers/ppso_Chen2012.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.1/ionbench/optimisers/external_optimisers/pso_Cabo2022.py` & `ionbench-0.4.2/ionbench/optimisers/external_optimisers/pso_Cabo2022.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,16 +64,14 @@
             """
             for i in range(len(self.position)):
                 if self.position[i] < 0:
                     self.position[i] = 0
                     self.velocity[i] = 0
                 elif self.position[i] > 1:
                     self.position[i] = 1
-                    print(self.velocity)
-                    print(i)
                     self.velocity[i] = 0
 
     # noinspection PyShadowingNames
     def best_in_ring(particleList):
         """
         Finds the best cost and position in the ring topology for each particle. Returns the positions of the best neighbouring particle that each particle can see.
```

### Comparing `ionbench-0.4.1/ionbench/optimisers/external_optimisers/pso_Seemann2009.py` & `ionbench-0.4.2/ionbench/optimisers/external_optimisers/pso_Seemann2009.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.1/ionbench/optimisers/external_optimisers/randomSearch_Vanier1999.py` & `ionbench-0.4.2/ionbench/optimisers/external_optimisers/randomSearch_Vanier1999.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.1/ionbench/optimisers/external_optimisers/stochasticSearch_Vanier1999.py` & `ionbench-0.4.2/ionbench/optimisers/external_optimisers/stochasticSearch_Vanier1999.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+"""
+The module provides the stochastic search algorithm from Vanier et al. 1999.
+This algorithm was previously described in Foster et al. 1993.
+We use the hyperparameters given by Vanier et al. 1999.
+Note that while Vanier et al. 1999 describes the variance as decreasing linearly, we use a geometric decrease as described in Foster et al. 1993.
+"""
 import numpy as np
 import ionbench
 
 
 # noinspection PyShadowingNames
 def run(bm, x0=None, varInit=0.5, varMin=0.05, varCont=0.95, maxIter=1000, debug=False):
     """
@@ -32,22 +38,24 @@
     """
     cost_func = ionbench.utils.cache.get_cached_cost(bm)
 
     if x0 is None:
         # sample initial point
         x0 = bm.sample()
     var = varInit
-    x0_cost = bm.cost(x0)
+    x0_cost = cost_func(x0)
     if debug:
         print(f'Starting cost is {x0_cost}')
     for i in range(maxIter):
-
-        trial = x0 + np.random.normal(loc=0, scale=np.sqrt(x0 * var))
+        trial = x0 + np.random.normal(loc=np.zeros(bm.n_parameters()), scale=np.sqrt(var))*(bm.input_parameter_space(bm.ub)-bm.input_parameter_space(bm.lb))
+        trial = bm.clamp_parameters(trial)
         trial_cost = cost_func(trial)
         if debug:
+            print(x0)
+            print(trial)
             print(f'var: {var}, trial cost: {trial_cost}')
         if trial_cost < x0_cost:
             x0 = trial
             x0_cost = trial_cost
             if debug:
                 print('Found improvement')
         var *= varCont
```

### Comparing `ionbench-0.4.1/ionbench/optimisers/pints_optimisers/cmaes_pints.py` & `ionbench-0.4.2/ionbench/optimisers/pints_optimisers/cmaes_pints.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.1/ionbench/optimisers/pints_optimisers/nelderMead_pints.py` & `ionbench-0.4.2/ionbench/optimisers/pints_optimisers/nelderMead_pints.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.1/ionbench/optimisers/pints_optimisers/pso_pints.py` & `ionbench-0.4.2/ionbench/optimisers/pints_optimisers/pso_pints.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.1/ionbench/optimisers/pints_optimisers/snes_pints.py` & `ionbench-0.4.2/ionbench/optimisers/pints_optimisers/snes_pints.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.1/ionbench/optimisers/pints_optimisers/xnes_pints.py` & `ionbench-0.4.2/ionbench/optimisers/pints_optimisers/xnes_pints.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.1/ionbench/optimisers/scipy_optimisers/conjugateGD_scipy.py` & `ionbench-0.4.2/ionbench/optimisers/scipy_optimisers/conjugateGD_scipy.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.1/ionbench/optimisers/scipy_optimisers/lm_scipy.py` & `ionbench-0.4.2/ionbench/optimisers/scipy_optimisers/lm_scipy.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.1/ionbench/optimisers/scipy_optimisers/nelderMead_scipy.py` & `ionbench-0.4.2/ionbench/optimisers/scipy_optimisers/nelderMead_scipy.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.1/ionbench/optimisers/scipy_optimisers/powell_scipy.py` & `ionbench-0.4.2/ionbench/optimisers/scipy_optimisers/powell_scipy.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.1/ionbench/optimisers/scipy_optimisers/slsqp_scipy.py` & `ionbench-0.4.2/ionbench/optimisers/scipy_optimisers/slsqp_scipy.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.1/ionbench/optimisers/scipy_optimisers/trustRegionReflective_scipy.py` & `ionbench-0.4.2/ionbench/optimisers/scipy_optimisers/trustRegionReflective_scipy.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.1/ionbench/problems/loewe2016.py` & `ionbench-0.4.2/ionbench/problems/loewe2016.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.1/ionbench/problems/moreno2016.py` & `ionbench-0.4.2/ionbench/problems/moreno2016.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.1/ionbench/problems/staircase.py` & `ionbench-0.4.2/ionbench/problems/staircase.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.1/ionbench/problems/test.py` & `ionbench-0.4.2/ionbench/problems/test.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.1/ionbench/tracker/tracker.py` & `ionbench-0.4.2/ionbench/tracker/tracker.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,14 +140,15 @@
                 plt.ylim(np.min(c[c < 1e5]), np.max(c[c < 1e5]))
             except ValueError:
                 # All points out of bounds
                 pass
             plt.xlabel('Model solves')
             plt.ylabel('RMSE cost')
             plt.title(title)
+            plt.show()
 
         # Cost plot
         plot_costs(self.costs, 'Evaluated Cost')
         plot_costs(self.bestCosts, 'Best Costs')
 
         # Plot cost and grad times
         plot_times(self.costTimes, 'cost')
@@ -218,16 +219,16 @@
 
         """
         i = self.when_converged(threshold)
         if i is None:
             print('Convergence reason:              Optimiser terminated early.')
             i = len(self.bestCosts) - 1
         else:
-            print('Convergence reason:              ' + 'Cost threshold' if self.cost_threshold(threshold,
-                                                                                                i) else 'Cost unchanged')
+            print('Convergence reason:              ' + ('Cost threshold' if self.cost_threshold(threshold,
+                                                                                                i) else 'Cost unchanged'))
         print('Cost evaluations at convergence: ' + str(self.modelSolves[i]))
         print('Grad evaluations at convergence: ' + str(self.gradSolves[i]))
         print('Best cost at convergence:        {0:.6f}'.format(self.bestCosts[i]))
         costTime, gradTime = self.total_solve_time(i)
         print('Model solve time at convergence: {0:.6f}'.format(costTime))
         print('Grad solve time at convergence:  {0:.6f}'.format(gradTime))
```

### Comparing `ionbench-0.4.1/ionbench/uncertainty/fim.py` & `ionbench-0.4.2/ionbench/uncertainty/fim.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.1/ionbench/uncertainty/profile_likelihood.py` & `ionbench-0.4.2/ionbench/uncertainty/profile_likelihood.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.1/ionbench/utils/autodiff.py` & `ionbench-0.4.2/ionbench/utils/autodiff.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.1/ionbench/utils/cache.py` & `ionbench-0.4.2/ionbench/utils/cache.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.1/ionbench/utils/classes_pints.py` & `ionbench-0.4.2/ionbench/utils/classes_pints.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,19 @@
         A Pints model containing the benchmarker.
     opt : pints.OptimisationController
         An optimisation controller to run the pints optimisation on.
     """
     if x0 is None:
         x0 = bm.sample()
     model = Model(bm)
-    problem = pints.SingleOutputProblem(model, np.arange(0, model.bm.T_MAX, model.bm.TIMESTEP), model.bm.DATA)
+    if 'moreno' in bm.NAME:
+        times = np.arange(len(bm.DATA))
+    else:
+        times = np.arange(0, bm.T_MAX, bm.TIMESTEP)
+    problem = pints.SingleOutputProblem(model, times, model.bm.DATA)
     error = pints.RootMeanSquaredError(problem)
     if bm.parametersBounded and not forceUnbounded:
         if bm.ratesBounded:
             boundaries = AdvancedBoundaries(bm)
         else:
             boundaries = pints.RectangularBoundaries(bm.input_parameter_space(bm.lb), bm.input_parameter_space(bm.ub))
         counter = 1
```

### Comparing `ionbench-0.4.1/ionbench/utils/multistart.py` & `ionbench-0.4.2/ionbench/utils/multistart.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.1/ionbench/utils/particle_optimisers.py` & `ionbench-0.4.2/ionbench/utils/particle_optimisers.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.1/ionbench/utils/population_optimisers.py` & `ionbench-0.4.2/ionbench/utils/population_optimisers.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.1/ionbench/utils/scipy_setup.py` & `ionbench-0.4.2/ionbench/utils/scipy_setup.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.1/ionbench.egg-info/PKG-INFO` & `ionbench-0.4.2/ionbench.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ionbench
-Version: 0.4.1
+Version: 0.4.2
 Summary: A benchmarking tool for comparing different parameter optimization algorithms for ion channel models
 Home-page: https://github.com/CardiacModelling/ionbench
 Author: Matt J. Owen
 Author-email: matt.owen@nottingham.ac.uk
 Project-URL: Bug Reports, https://github.com/CardiacModelling/ionbench/issues
 Project-URL: Source, https://github.com/CardiacModelling/ionbench
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ionbench-0.4.1/ionbench.egg-info/SOURCES.txt` & `ionbench-0.4.2/ionbench.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.1/setup.py` & `ionbench-0.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     name="ionbench",  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version="0.4.1",  # Required
+    version="0.4.2",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="A benchmarking tool for comparing different parameter optimization algorithms for ion channel models",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

### Comparing `ionbench-0.4.1/test/test_modifications.py` & `ionbench-0.4.2/test/test_modifications.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.1/test/test_multistart.py` & `ionbench-0.4.2/test/test_multistart.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.1/test/test_optimisers.py` & `ionbench-0.4.2/test/test_optimisers.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.1/test/test_problems.py` & `ionbench-0.4.2/test/test_problems.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.1/test/test_uncertainty.py` & `ionbench-0.4.2/test/test_uncertainty.py`

 * *Files identical despite different names*

