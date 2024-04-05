# Comparing `tmp/sbn-92.tar.gz` & `tmp/sbn-94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sbn-92.tar", last modified: Sun Feb  4 11:50:20 2024, max compression
+gzip compressed data, was "sbn-94.tar", last modified: Fri Apr  5 13:12:56 2024, max compression
```

## Comparing `sbn-92.tar` & `sbn-94.tar`

### file list

```diff
@@ -1,90 +1,92 @@
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-02-04 11:50:20.610101 sbn-92/
--rw-r--r--   0 bart      (1000) bart      (1000)     3680 2024-02-04 11:50:20.610101 sbn-92/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)     3074 2024-02-04 04:23:22.000000 sbn-92/README.rst
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-02-04 11:50:20.598101 sbn-92/docs/
--rw-r--r--   0 bart      (1000) bart      (1000)   180711 2024-02-04 03:28:21.000000 sbn-92/docs/ECHAabilify.png
--rw-r--r--   0 bart      (1000) bart      (1000)   193757 2024-02-04 03:28:21.000000 sbn-92/docs/ECHAclozapine.png
--rw-r--r--   0 bart      (1000) bart      (1000)   197697 2024-02-04 03:28:21.000000 sbn-92/docs/ECHAhaldol.png
--rw-r--r--   0 bart      (1000) bart      (1000)   232313 2024-02-04 03:28:21.000000 sbn-92/docs/ECHAzyprexa.png
--rw-r--r--   0 bart      (1000) bart      (1000)   245670 2024-02-04 03:28:21.000000 sbn-92/docs/OTP1.png
--rw-r--r--   0 bart      (1000) bart      (1000)   238095 2024-02-04 03:28:21.000000 sbn-92/docs/OTP2.png
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-02-04 11:50:20.598101 sbn-92/docs/_static/
--rw-r--r--   0 bart      (1000) bart      (1000)     1001 2024-02-04 03:28:21.000000 sbn-92/docs/_static/sbn.css
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-02-04 11:50:20.598101 sbn-92/docs/_templates/
--rw-r--r--   0 bart      (1000) bart      (1000)      269 2024-02-04 03:28:21.000000 sbn-92/docs/_templates/base.rst
--rw-r--r--   0 bart      (1000) bart      (1000)      543 2024-02-04 03:28:21.000000 sbn-92/docs/_templates/class.rst
--rw-r--r--   0 bart      (1000) bart      (1000)      879 2024-02-04 03:28:21.000000 sbn-92/docs/_templates/mine.rst
--rw-r--r--   0 bart      (1000) bart      (1000)      879 2024-02-04 03:28:21.000000 sbn-92/docs/_templates/module.rst
--rw-r--r--   0 bart      (1000) bart      (1000)     1123 2024-02-04 06:14:43.000000 sbn-92/docs/about.rst
--rw-r--r--   0 bart      (1000) bart      (1000)   130021 2024-02-04 03:28:21.000000 sbn-92/docs/arrest.png
--rw-r--r--   0 bart      (1000) bart      (1000)   256520 2024-02-04 03:28:21.000000 sbn-92/docs/banner.png
--rw-r--r--   0 bart      (1000) bart      (1000)  1685507 2024-02-04 03:28:21.000000 sbn-92/docs/bevestigd.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)     3559 2024-02-04 05:19:20.000000 sbn-92/docs/conf.py
--rw-r--r--   0 bart      (1000) bart      (1000)      537 2024-02-04 03:29:40.000000 sbn-92/docs/evidence.rst
--rw-r--r--   0 bart      (1000) bart      (1000)    47740 2024-02-04 03:28:21.000000 sbn-92/docs/genocide.png
--rw-r--r--   0 bart      (1000) bart      (1000)      303 2024-02-04 03:29:49.000000 sbn-92/docs/guilty.rst
--rw-r--r--   0 bart      (1000) bart      (1000)     2068 2024-02-04 03:29:30.000000 sbn-92/docs/index.rst
--rw-r--r--   0 bart      (1000) bart      (1000)    69979 2024-02-04 03:28:21.000000 sbn-92/docs/informed.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)   228393 2024-02-04 03:28:21.000000 sbn-92/docs/kamer.png
--rw-r--r--   0 bart      (1000) bart      (1000)     3546 2024-02-04 03:29:57.000000 sbn-92/docs/manual.rst
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-02-04 11:50:20.602101 sbn-92/docs/pdf/
--rw-r--r--   0 bart      (1000) bart      (1000)   238330 2024-02-04 03:28:21.000000 sbn-92/docs/pdf/EM_T04_OTP-CR-117_19.pdf
--rw-r--r--   0 bart      (1000) bart      (1000)   236671 2024-02-04 03:28:21.000000 sbn-92/docs/pdf/EM_T07_OTP-CR-117_19_001.pdf
--rw-r--r--   0 bart      (1000) bart      (1000)    41559 2024-02-04 03:28:21.000000 sbn-92/docs/pdf/Kamer.pdf
--rw-r--r--   0 bart      (1000) bart      (1000)   323490 2024-02-04 03:28:21.000000 sbn-92/docs/pdf/Rome-Statute.pdf
--rw-r--r--   0 bart      (1000) bart      (1000)    50044 2024-02-04 03:28:21.000000 sbn-92/docs/pdf/bevestigd.pdf
--rw-r--r--   0 bart      (1000) bart      (1000)     2196 2024-02-04 03:44:59.000000 sbn-92/docs/request.rst
--rw-r--r--   0 bart      (1000) bart      (1000)   179869 2024-02-04 03:28:21.000000 sbn-92/docs/skull.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)   287102 2024-02-04 03:28:21.000000 sbn-92/docs/skull3.png
--rw-r--r--   0 bart      (1000) bart      (1000)     1288 2024-02-04 04:18:20.000000 sbn-92/docs/source.rst
--rw-r--r--   0 bart      (1000) bart      (1000)      176 2024-02-04 03:28:21.000000 sbn-92/docs/verbatim.rst
--rw-r--r--   0 bart      (1000) bart      (1000)   234877 2024-02-04 03:28:21.000000 sbn-92/docs/verbatim2.png
--rw-r--r--   0 bart      (1000) bart      (1000)    46476 2024-02-04 03:28:21.000000 sbn-92/docs/wallpaper.png
--rw-r--r--   0 bart      (1000) bart      (1000)     1120 2024-02-04 03:30:09.000000 sbn-92/docs/writings.rst
--rw-r--r--   0 bart      (1000) bart      (1000)     2110 2024-02-04 05:40:25.000000 sbn-92/pyproject.toml
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-02-04 11:50:20.602101 sbn-92/sbn/
--rw-r--r--   0 bart      (1000) bart      (1000)     1045 2024-02-04 03:28:21.000000 sbn-92/sbn/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1000)     3398 2024-02-04 05:42:19.000000 sbn-92/sbn/__main__.py
--rw-r--r--   0 bart      (1000) bart      (1000)      731 2024-02-04 03:28:21.000000 sbn-92/sbn/brokers.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1855 2024-02-04 03:28:21.000000 sbn-92/sbn/clients.py
--rw-r--r--   0 bart      (1000) bart      (1000)      725 2024-02-04 03:28:21.000000 sbn-92/sbn/command.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1470 2024-02-04 03:28:21.000000 sbn-92/sbn/excepts.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1865 2024-02-04 03:28:21.000000 sbn-92/sbn/handler.py
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-02-04 11:50:20.610101 sbn-92/sbn/modules/
--rw-r--r--   0 bart      (1000) bart      (1000)      465 2024-02-04 03:28:21.000000 sbn-92/sbn/modules/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1000)      186 2024-02-04 03:28:21.000000 sbn-92/sbn/modules/cmd.py
--rw-r--r--   0 bart      (1000) bart      (1000)      459 2024-02-04 03:28:21.000000 sbn-92/sbn/modules/err.py
--rw-r--r--   0 bart      (1000) bart      (1000)      299 2024-02-04 03:28:21.000000 sbn-92/sbn/modules/flt.py
--rw-r--r--   0 bart      (1000) bart      (1000)      704 2024-02-04 03:28:21.000000 sbn-92/sbn/modules/fnd.py
--rw-r--r--   0 bart      (1000) bart      (1000)    16076 2024-02-04 05:50:48.000000 sbn-92/sbn/modules/irc.py
--rw-r--r--   0 bart      (1000) bart      (1000)      607 2024-02-04 03:28:21.000000 sbn-92/sbn/modules/log.py
--rw-r--r--   0 bart      (1000) bart      (1000)     3091 2024-02-04 03:28:21.000000 sbn-92/sbn/modules/man.py
--rw-r--r--   0 bart      (1000) bart      (1000)     3468 2024-02-04 03:28:21.000000 sbn-92/sbn/modules/mbx.py
--rw-r--r--   0 bart      (1000) bart      (1000)    16880 2024-02-04 03:28:21.000000 sbn-92/sbn/modules/mdl.py
--rw-r--r--   0 bart      (1000) bart      (1000)      175 2024-02-04 03:28:21.000000 sbn-92/sbn/modules/mod.py
--rw-r--r--   0 bart      (1000) bart      (1000)      653 2024-02-04 03:28:21.000000 sbn-92/sbn/modules/mre.py
--rw-r--r--   0 bart      (1000) bart      (1000)      408 2024-02-04 03:28:21.000000 sbn-92/sbn/modules/pwd.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2349 2024-02-04 03:28:21.000000 sbn-92/sbn/modules/req.py
--rw-r--r--   0 bart      (1000) bart      (1000)     3094 2024-02-04 05:02:48.000000 sbn-92/sbn/modules/rme.py
--rw-r--r--   0 bart      (1000) bart      (1000)     7304 2024-02-04 03:28:21.000000 sbn-92/sbn/modules/rss.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2638 2024-02-04 03:28:21.000000 sbn-92/sbn/modules/rst.py
--rw-r--r--   0 bart      (1000) bart      (1000)      350 2024-02-04 03:28:21.000000 sbn-92/sbn/modules/slg.py
--rw-r--r--   0 bart      (1000) bart      (1000)      996 2024-02-04 03:28:21.000000 sbn-92/sbn/modules/tdo.py
--rw-r--r--   0 bart      (1000) bart      (1000)      984 2024-02-04 03:28:21.000000 sbn-92/sbn/modules/thr.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1924 2024-02-04 03:28:21.000000 sbn-92/sbn/modules/tmr.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2817 2024-02-04 03:28:21.000000 sbn-92/sbn/modules/udp.py
--rw-r--r--   0 bart      (1000) bart      (1000)     5742 2024-02-04 03:28:21.000000 sbn-92/sbn/modules/wsd.py
--rw-r--r--   0 bart      (1000) bart      (1000)     5304 2024-02-04 03:28:21.000000 sbn-92/sbn/objects.py
--rw-r--r--   0 bart      (1000) bart      (1000)     6101 2024-02-04 03:28:21.000000 sbn-92/sbn/parsers.py
--rw-r--r--   0 bart      (1000) bart      (1000)     3862 2024-02-04 03:28:21.000000 sbn-92/sbn/storage.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2884 2024-02-04 03:28:21.000000 sbn-92/sbn/threads.py
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-02-04 11:50:20.606101 sbn-92/sbn.egg-info/
--rw-r--r--   0 bart      (1000) bart      (1000)     3680 2024-02-04 11:50:20.000000 sbn-92/sbn.egg-info/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)     1539 2024-02-04 11:50:20.000000 sbn-92/sbn.egg-info/SOURCES.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-02-04 11:50:20.000000 sbn-92/sbn.egg-info/dependency_links.txt
--rw-r--r--   0 bart      (1000) bart      (1000)       74 2024-02-04 11:50:20.000000 sbn-92/sbn.egg-info/entry_points.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        7 2024-02-04 11:50:20.000000 sbn-92/sbn.egg-info/requires.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        4 2024-02-04 11:50:20.000000 sbn-92/sbn.egg-info/top_level.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-02-04 11:50:20.000000 sbn-92/sbn.egg-info/zip-safe
--rw-r--r--   0 bart      (1000) bart      (1000)       38 2024-02-04 11:50:20.610101 sbn-92/setup.cfg
--rw-r--r--   0 bart      (1000) bart      (1000)      211 2024-02-04 03:28:21.000000 sbn-92/setup.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-05 13:12:56.600584 sbn-94/
+-rw-r--r--   0 bart      (1000) bart      (1000)     2807 2024-04-05 13:01:11.000000 sbn-94/MANUAL.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)     2495 2024-04-05 13:12:56.600584 sbn-94/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)     1933 2024-04-05 12:58:23.000000 sbn-94/README.rst
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-05 13:12:56.592584 sbn-94/docs/
+-rw-r--r--   0 bart      (1000) bart      (1000)   180711 2024-04-05 12:12:33.000000 sbn-94/docs/ECHAabilify.png
+-rw-r--r--   0 bart      (1000) bart      (1000)   193757 2024-04-05 12:12:33.000000 sbn-94/docs/ECHAclozapine.png
+-rw-r--r--   0 bart      (1000) bart      (1000)   197697 2024-04-05 12:12:33.000000 sbn-94/docs/ECHAhaldol.png
+-rw-r--r--   0 bart      (1000) bart      (1000)   232313 2024-04-05 12:12:33.000000 sbn-94/docs/ECHAzyprexa.png
+-rw-r--r--   0 bart      (1000) bart      (1000)   245670 2024-04-05 12:12:33.000000 sbn-94/docs/OTP1.png
+-rw-r--r--   0 bart      (1000) bart      (1000)   238095 2024-04-05 12:12:33.000000 sbn-94/docs/OTP2.png
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-05 13:12:56.592584 sbn-94/docs/_static/
+-rw-r--r--   0 bart      (1000) bart      (1000)     1000 2024-04-05 12:12:33.000000 sbn-94/docs/_static/sbn.css
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-05 13:12:56.592584 sbn-94/docs/_templates/
+-rw-r--r--   0 bart      (1000) bart      (1000)      291 2024-04-05 12:12:33.000000 sbn-94/docs/_templates/base.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)      543 2024-04-05 12:12:33.000000 sbn-94/docs/_templates/class.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)      879 2024-04-05 12:12:33.000000 sbn-94/docs/_templates/mine.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)      879 2024-04-05 12:12:33.000000 sbn-94/docs/_templates/module.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)     1434 2024-04-05 12:12:33.000000 sbn-94/docs/about.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)   130021 2024-04-05 12:12:33.000000 sbn-94/docs/arrest.png
+-rw-r--r--   0 bart      (1000) bart      (1000)   256520 2024-04-05 12:12:33.000000 sbn-94/docs/banner.png
+-rw-r--r--   0 bart      (1000) bart      (1000)  1685507 2024-04-05 12:12:33.000000 sbn-94/docs/bevestigd.jpg
+-rw-r--r--   0 bart      (1000) bart      (1000)     3246 2024-04-05 12:12:33.000000 sbn-94/docs/conf.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      537 2024-04-05 12:12:33.000000 sbn-94/docs/evidence.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)    47740 2024-04-05 12:12:33.000000 sbn-94/docs/genocide.png
+-rw-r--r--   0 bart      (1000) bart      (1000)      303 2024-04-05 12:12:33.000000 sbn-94/docs/guilty.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)     2087 2024-04-05 13:11:33.000000 sbn-94/docs/index.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)    69979 2024-04-05 12:12:33.000000 sbn-94/docs/informed.jpg
+-rw-r--r--   0 bart      (1000) bart      (1000)   228393 2024-04-05 12:12:33.000000 sbn-94/docs/kamer.png
+-rw-r--r--   0 bart      (1000) bart      (1000)     3413 2024-04-05 13:00:34.000000 sbn-94/docs/manual.rst
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-05 13:12:56.596583 sbn-94/docs/pdf/
+-rw-r--r--   0 bart      (1000) bart      (1000)   238330 2024-04-05 12:12:33.000000 sbn-94/docs/pdf/EM_T04_OTP-CR-117_19.pdf
+-rw-r--r--   0 bart      (1000) bart      (1000)   236671 2024-04-05 12:12:33.000000 sbn-94/docs/pdf/EM_T07_OTP-CR-117_19_001.pdf
+-rw-r--r--   0 bart      (1000) bart      (1000)    41559 2024-04-05 12:12:33.000000 sbn-94/docs/pdf/Kamer.pdf
+-rw-r--r--   0 bart      (1000) bart      (1000)   323490 2024-04-05 12:12:33.000000 sbn-94/docs/pdf/Rome-Statute.pdf
+-rw-r--r--   0 bart      (1000) bart      (1000)    50044 2024-04-05 12:12:33.000000 sbn-94/docs/pdf/bevestigd.pdf
+-rw-r--r--   0 bart      (1000) bart      (1000)     2196 2024-04-05 12:12:33.000000 sbn-94/docs/request.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)   179869 2024-04-05 12:12:33.000000 sbn-94/docs/skull.jpg
+-rw-r--r--   0 bart      (1000) bart      (1000)   287102 2024-04-05 12:12:33.000000 sbn-94/docs/skull3.png
+-rw-r--r--   0 bart      (1000) bart      (1000)     1494 2024-04-05 12:55:42.000000 sbn-94/docs/source.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)      176 2024-04-05 12:12:33.000000 sbn-94/docs/verbatim.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)   234877 2024-04-05 12:12:33.000000 sbn-94/docs/verbatim2.png
+-rw-r--r--   0 bart      (1000) bart      (1000)    46476 2024-04-05 12:12:33.000000 sbn-94/docs/wallpaper.png
+-rw-r--r--   0 bart      (1000) bart      (1000)     1120 2024-04-05 12:12:33.000000 sbn-94/docs/writings.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)     2073 2024-04-05 13:05:17.000000 sbn-94/pyproject.toml
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-05 13:12:56.596583 sbn-94/sbn/
+-rw-r--r--   0 bart      (1000) bart      (1000)       84 2024-04-04 12:27:14.000000 sbn-94/sbn/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     3915 2024-04-04 13:15:53.000000 sbn-94/sbn/__main__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      904 2024-04-04 11:48:34.000000 sbn-94/sbn/broker.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1582 2024-04-04 12:05:43.000000 sbn-94/sbn/client.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      321 2024-04-04 11:47:18.000000 sbn-94/sbn/default.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1738 2024-04-04 13:39:07.000000 sbn-94/sbn/errors.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      865 2024-04-04 11:46:43.000000 sbn-94/sbn/event.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1608 2024-04-04 12:10:33.000000 sbn-94/sbn/handler.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1442 2024-04-05 11:15:28.000000 sbn-94/sbn/interface.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-05 13:12:56.600584 sbn-94/sbn/modules/
+-rw-r--r--   0 bart      (1000) bart      (1000)      436 2024-04-04 11:31:06.000000 sbn-94/sbn/modules/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      239 2024-04-05 11:22:25.000000 sbn-94/sbn/modules/cmd.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      254 2024-04-05 11:22:46.000000 sbn-94/sbn/modules/dbg.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      573 2024-04-05 11:23:11.000000 sbn-94/sbn/modules/err.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      424 2024-04-05 11:23:26.000000 sbn-94/sbn/modules/flt.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      826 2024-04-05 11:44:57.000000 sbn-94/sbn/modules/fnd.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    19015 2024-04-05 11:25:16.000000 sbn-94/sbn/modules/irc.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      841 2024-04-05 11:25:50.000000 sbn-94/sbn/modules/log.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2482 2024-04-05 11:27:00.000000 sbn-94/sbn/modules/mbx.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    16468 2024-04-05 11:28:55.000000 sbn-94/sbn/modules/mdl.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      264 2024-04-05 11:29:51.000000 sbn-94/sbn/modules/mod.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2428 2024-04-05 11:31:46.000000 sbn-94/sbn/modules/req.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    10937 2024-04-05 11:35:17.000000 sbn-94/sbn/modules/rss.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     3213 2024-04-05 11:36:34.000000 sbn-94/sbn/modules/rst.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1196 2024-04-05 11:37:54.000000 sbn-94/sbn/modules/tdo.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1082 2024-04-05 11:38:18.000000 sbn-94/sbn/modules/thr.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     5282 2024-04-05 11:42:28.000000 sbn-94/sbn/modules/tmr.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     3169 2024-04-05 11:42:03.000000 sbn-94/sbn/modules/udp.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     6154 2024-04-04 11:48:18.000000 sbn-94/sbn/object.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1814 2024-04-04 11:48:07.000000 sbn-94/sbn/parser.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     3435 2024-04-04 11:46:19.000000 sbn-94/sbn/persist.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      344 2024-04-04 11:47:29.000000 sbn-94/sbn/repeater.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2029 2024-04-04 12:10:16.000000 sbn-94/sbn/thread.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1151 2024-04-04 11:46:52.000000 sbn-94/sbn/timer.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1235 2024-04-04 11:47:07.000000 sbn-94/sbn/utils.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      779 2024-04-04 12:09:42.000000 sbn-94/sbn/workdir.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-05 13:12:56.596583 sbn-94/sbn.egg-info/
+-rw-r--r--   0 bart      (1000) bart      (1000)     2495 2024-04-05 13:12:56.000000 sbn-94/sbn.egg-info/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)     1536 2024-04-05 13:12:56.000000 sbn-94/sbn.egg-info/SOURCES.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-04-05 13:12:56.000000 sbn-94/sbn.egg-info/dependency_links.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)       45 2024-04-05 13:12:56.000000 sbn-94/sbn.egg-info/entry_points.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        7 2024-04-05 13:12:56.000000 sbn-94/sbn.egg-info/requires.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        4 2024-04-05 13:12:56.000000 sbn-94/sbn.egg-info/top_level.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-04-05 13:12:56.000000 sbn-94/sbn.egg-info/zip-safe
+-rw-r--r--   0 bart      (1000) bart      (1000)       38 2024-04-05 13:12:56.600584 sbn-94/setup.cfg
+-rw-r--r--   0 bart      (1000) bart      (1000)      192 2024-04-05 12:12:33.000000 sbn-94/setup.py
```

### Comparing `sbn-92/PKG-INFO` & `sbn-94/MANUAL.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,20 @@
-Metadata-Version: 2.1
-Name: sbn
-Version: 92
-Summary: Skull, Bones and Number (OTP-CR-117/19)
-Author-email: OTP-CR-117/19 <skullbonesandnumer@gmail.com>
-License: Public Domain
-Project-URL: home, https://pypi.org/project/sbn
-Project-URL: bugs, https://github.com/skullbonesandnumber/sbn/issues
-Project-URL: source, https://github.com/skullbonesandnumber/sbn
-Classifier: Development Status :: 3 - Alpha
-Classifier: License :: Public Domain
-Classifier: Operating System :: Unix
-Classifier: Programming Language :: Python
-Classifier: Topic :: Utilities
-Description-Content-Type: text/x-rst
-Provides-Extra: dev
-
 NAME
 
 ::
 
     SBN - Skull, Bones and Number (OTP-CR-117/19)
 
 
 SYNOPSIS
 
 ::
 
     sbn <cmd> [key=val] [key==val]
-    sbn [-a] [-c] [-d] [-h] [-v]
+    sbn [-a] [-c] [-d] [-v]
 
 
 DESCRIPTION
 
 ::
 
     SBN holds evidence that king netherlands is doing a genocide, a
@@ -67,18 +50,15 @@
     $
 
     see list of commands
 
     $ sbn cmd
     cfg,cmd,mre,now,pwd
 
-    the cfg command configures irc
-
     $ sbn cfg
-    channel=#sbn commands=True nick=sbn port=6667 server=localhost
 
     start a console
 
     $ sbn -c 
     >
 
     use -v for verbose
@@ -132,21 +112,17 @@
 
 
 COMMANDS
 
 
 ::
 
-    cfg - irc configuration
     cmd - commands
-    mre - displays cached output
     now - show genocide stats
-    pwd - sasl nickserv name/pass
     req - reconsider
-    wsd - show wisdom
 
 
 SYSTEMD
 
 
 ::
 
@@ -160,19 +136,19 @@
     After=network-online.target
 
     [Service]
     Type=simple
     User=<user>
     Group=<user>
     WorkingDirectory=/home/<user>/.sbn
-    ExecStart=/home/<user>/.local/pipx/venvs/sbn/bin/sbnd
+    ExecStart=/home/<user>/.local/pipx/venvs/sbn/bin/sbn -d
     RemainAfterExit=yes
 
     [Install]
-    WantedBy=multi-user.target
+    WantedBy=default.target
 
 
     then run this
 
     $ mkdir ~/.sbn
     $ sudo systemctl enable sbn --now
 
@@ -181,24 +157,23 @@
 
 FILES
 
 ::
 
     ~/.sbn
     ~/.local/bin/sbn
-    ~/.local/bin/sbnd
     ~/.local/pipx/venvs/sbn/
 
 
 AUTHOR
 
 
 ::
 
-    OTP-CR-117/19 <skullbonesandnumber@gmail.com>
+    Bart Thate <bthate@dds.nl>
 
 
 COPYRIGHT
 
 
 ::
```

### Comparing `sbn-92/docs/ECHAabilify.png` & `sbn-94/docs/ECHAabilify.png`

 * *Files identical despite different names*

### Comparing `sbn-92/docs/ECHAclozapine.png` & `sbn-94/docs/ECHAclozapine.png`

 * *Files identical despite different names*

### Comparing `sbn-92/docs/ECHAhaldol.png` & `sbn-94/docs/ECHAhaldol.png`

 * *Files identical despite different names*

### Comparing `sbn-92/docs/ECHAzyprexa.png` & `sbn-94/docs/ECHAzyprexa.png`

 * *Files identical despite different names*

### Comparing `sbn-92/docs/OTP1.png` & `sbn-94/docs/OTP1.png`

 * *Files identical despite different names*

### Comparing `sbn-92/docs/OTP2.png` & `sbn-94/docs/OTP2.png`

 * *Files identical despite different names*

### Comparing `sbn-92/docs/_static/sbn.css` & `sbn-94/docs/_static/sbn.css`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 body {
     font-family: 'Lucida Grande', 'Lucida Sans Unicode', 'Geneva',
                  'Verdana', sans-serif;
     font-size: 113%;
     background-color: #fff;
     color: #555;
     margin: 30px;
-    padding: 00px;
+    padding: 0px;
 }
 
 
 i {
     font-family: 'Lucida Grande', 'Lucida Sans Unicode', 'Geneva',
                  'Verdana', sans-serif;
     font-size: 90%;
```

### Comparing `sbn-92/docs/_templates/class.rst` & `sbn-94/docs/_templates/class.rst`

 * *Files identical despite different names*

### Comparing `sbn-92/docs/_templates/mine.rst` & `sbn-94/docs/_templates/mine.rst`

 * *Files identical despite different names*

### Comparing `sbn-92/docs/_templates/module.rst` & `sbn-94/docs/_templates/module.rst`

 * *Files identical despite different names*

### Comparing `sbn-92/docs/about.rst` & `sbn-94/docs/about.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,27 @@
 .. _about:
 
 
 .. raw:: html
 
+    <center>
+    <i>
+    By law, with the use of poison,
+    killing, torturing, castrating, destroying,
+    in whole or in part,
+    all elderly and all handicapped (Wzd), all criminals (Wfz)
+    and all psychiatric patients (WvGGZ)
+    here in the Netherlands
+    </i>
+    </center>
+    <br>
+
+
+.. raw:: html
+
     <br><br>
 
 .. title:: About
 
 
 In 2018 i informed the king of the netherlands that what he calls
 medicine in his "care" laws are not medicine but poison. Proof of
```

### Comparing `sbn-92/docs/arrest.png` & `sbn-94/docs/arrest.png`

 * *Files identical despite different names*

### Comparing `sbn-92/docs/banner.png` & `sbn-94/docs/banner.png`

 * *Files identical despite different names*

### Comparing `sbn-92/docs/bevestigd.jpg` & `sbn-94/docs/bevestigd.jpg`

 * *Files identical despite different names*

### Comparing `sbn-92/docs/conf.py` & `sbn-94/docs/conf.py`

 * *Files 13% similar despite different names*

```diff
@@ -109,42 +109,25 @@
 intersphinx_cache_limit = 1
 
 
 rst_prolog = '''.. image:: genocide.png
     :width: 100%
     :height: 2.6cm
     :target: index.html
-
-
-.. raw:: html
-
-    <center>
-    <i>
-    By law, with the use of poison,
-    killing, torturing, castrating, destroying,
-    in whole or in part,
-    all elderly and all handicapped (Wzd), all criminals (Wfz)
-    and all psychiatric patients (WvGGZ)
-    here in the Netherlands
-    </i>
-    </center>
-    <br>
-
-
 '''
 
 rst_epilog = '''.. raw:: html
 
     <br>
     <br>
     <br>
     <center>
     <b>
 
-:ref:`about <about>` - :ref:`writings <writings>` - :ref:`reconsider <reconsider>` - :ref:`evidence <evidence>` - :ref:`guilty <guilty>`
+:ref:`about <about>` - :ref:`writings <writings>` - :ref:`evidence <evidence>` - :ref:`guilty <guilty>` - :ref:`reconsider <reconsider>`
 
 
 .. raw:: html
 
     </b>
     </center>
```

### Comparing `sbn-92/docs/evidence.rst` & `sbn-94/docs/evidence.rst`

 * *Files identical despite different names*

### Comparing `sbn-92/docs/genocide.png` & `sbn-94/docs/genocide.png`

 * *Files identical despite different names*

### Comparing `sbn-92/docs/index.rst` & `sbn-94/docs/index.rst`

 * *Files 6% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 .. title:: Reconsider
 
 
 | **Information and Evidence Unit**
 | **Office of the Prosecutor**
 | **Post Office Box 19519**
 | **2500 CM The Hague**
-| **The Netherlands**
+| **The Netherlands** 
 |
 
-Hello Office of the Prosecutor,
+Hello Office of the Prosecutor, ``OTP-CR-117/19``
 
 i write you in the context of communications and claims under art.15 of 
 the Rome Statute. i want to inform the prosecutor that the king of the 
 netherlands and his government are commiting 3 of the 5 crimes defined 
 in the Rome Statute.
 
 The dutch government has introduced three new forced care laws, the Wfz
```

### Comparing `sbn-92/docs/informed.jpg` & `sbn-94/docs/informed.jpg`

 * *Files identical despite different names*

### Comparing `sbn-92/docs/kamer.png` & `sbn-94/docs/kamer.png`

 * *Files identical despite different names*

### Comparing `sbn-92/docs/manual.rst` & `sbn-94/docs/manual.rst`

 * *Files 4% similar despite different names*

```diff
@@ -144,21 +144,18 @@
         $ sbn nme <url> <name>
 
 
 **COMMANDS**
 
     ::
 
-        cfg - irc configuration
         cmd - commands
-        mre - displays cached output
+        mod - show modules
         now - show genocide stats
-        pwd - sasl nickserv name/pass
         req - reconsider
-        wsd - show wisdom
 
 
 **SYSTEMD**
 
     save the following it in /etc/systems/system/sbn.service
     and replace "<user>" with the user running pipx
 
@@ -170,19 +167,19 @@
         After=network-online.target
 
         [Service]
         Type=simple
         User=<user>
         Group=<user>
         WorkingDirectory=/home/<user>/.sbn
-        ExecStart=/home/<user>/.local/pipx/venvs/sbn/bin/sbnd
+        ExecStart=/home/<user>/.local/pipx/venvs/sbn/bin/sbn -d
         RemainAfterExit=yes
 
         [Install]
-        WantedBy=multi-user.target
+        WantedBy=default.target
 
 
     then run this
 
     ::
 
         $ mkdir ~/.sbn
@@ -193,15 +190,14 @@
 
 **FILES**
 
     ::
 
         ~/.sbn
         ~/.local/bin/sbn
-        ~/.local/bin/sbnd
         ~/.local/pipx/venvs/sbn/
 
 
 **SOURCE**
 
 
    source code is :ref:`here <source>`
```

### Comparing `sbn-92/docs/pdf/EM_T04_OTP-CR-117_19.pdf` & `sbn-94/docs/pdf/EM_T04_OTP-CR-117_19.pdf`

 * *Files identical despite different names*

### Comparing `sbn-92/docs/pdf/EM_T07_OTP-CR-117_19_001.pdf` & `sbn-94/docs/pdf/EM_T07_OTP-CR-117_19_001.pdf`

 * *Files identical despite different names*

### Comparing `sbn-92/docs/pdf/Kamer.pdf` & `sbn-94/docs/pdf/Kamer.pdf`

 * *Files identical despite different names*

### Comparing `sbn-92/docs/pdf/Rome-Statute.pdf` & `sbn-94/docs/pdf/Rome-Statute.pdf`

 * *Files identical despite different names*

### Comparing `sbn-92/docs/pdf/bevestigd.pdf` & `sbn-94/docs/pdf/bevestigd.pdf`

 * *Files identical despite different names*

### Comparing `sbn-92/docs/request.rst` & `sbn-94/docs/request.rst`

 * *Files identical despite different names*

### Comparing `sbn-92/docs/skull.jpg` & `sbn-94/docs/skull.jpg`

 * *Files identical despite different names*

### Comparing `sbn-92/docs/skull3.png` & `sbn-94/docs/skull3.png`

 * *Files identical despite different names*

### Comparing `sbn-92/docs/verbatim2.png` & `sbn-94/docs/verbatim2.png`

 * *Files identical despite different names*

### Comparing `sbn-92/docs/wallpaper.png` & `sbn-94/docs/wallpaper.png`

 * *Files identical despite different names*

### Comparing `sbn-92/docs/writings.rst` & `sbn-94/docs/writings.rst`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 .. raw:: html
 
     <br>
 
 .. title:: Writings
 
 
-**Email 1**
+**EMAIL 1**
 
 
 |
 | **From**: Bart Thate <bthate@dds.nl>
 | **To**: otp.informationdesk@icc-cpi.int
 | **Subject**: Information that the king of the netherlands is aware that the medicine administered with the use of new defines laws are proven to be poison and is commiting 3 of 5 genocide crimes on parts of the population here in the netherlands
 | **Message-ID**: <e49d02a2-6a8e-ad64-6c8d-9abd45cf5c0e@dds.nl>
@@ -33,15 +33,15 @@
 
 
 .. raw:: html
 
     <br><br>
 
 
-**Email 2**
+**EMAIL 2**
 
 
 |
 | **From:** Bart Thate <bthate@dds.nl>
 | **To:** OTP InformationDesk <OTP.InformationDesk@icc-cpi.int>
 | **Subject:** Request to reconsider OTP-CR-117/19
 | **Message-ID:** <33777b52-6be9-72b2-f756-d5482d32f03d@dds.nl>
```

### Comparing `sbn-92/pyproject.toml` & `sbn-94/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 requires = ["setuptools>=43.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "sbn"
 description = "Skull, Bones and Number (OTP-CR-117/19)"
-version = "92"
+version = "94"
 authors = [
-    {name = "OTP-CR-117/19", email = "skullbonesandnumer@gmail.com" },
+    {name = "Bart Thate", email = "bthate@dds.nl" },
 ]
 readme = "README.rst"
 license = { text="Public Domain"}
 classifiers=[
     'Development Status :: 3 - Alpha',
     'License :: Public Domain',
     'Operating System :: Unix',
@@ -20,34 +20,35 @@
     'Topic :: Utilities'
 ]
 
 [project.optional-dependencies]
 dev = []
 
 [project.scripts]
-sbn = "sbn.__main__:wrapped"
-sbnd = "sbn.__main__:daemoned"
+"sbn" = "sbn.__main__:wrapped"
 
 
 [project.urls]
 "home" = "https://pypi.org/project/sbn"
-"bugs" = "https://github.com/skullbonesandnumber/sbn/issues"
-"source" = "https://github.com/skullbonesandnumber/sbn"
+"bugs" = "https://github.com/bthate/sbn/issues"
+"source" = "https://github.com/bthate/sbn"
 
 
 [tool.setuptools]
 packages = [
    "sbn",
    "sbn.modules"
 ]
 zip-safe = true
 
 
 [tool.setuptools.data-files]
 "share/doc/sbn" = [
+    "README.rst",
+    "MANUAL.rst",
     "docs/about.rst",
     "docs/arrest.png",
     "docs/conf.py",
     "docs/ECHAhaldol.png",
     "docs/evidence.rst",
     "docs/genocide.png",
     "docs/informed.jpg",
```

### Comparing `sbn-92/sbn/__main__.py` & `sbn-94/sbn/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,86 +1,83 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,R,W0212,W0611,W0613,E0401
+# pylint: disable=C,R,W0105,W0212
+# ruff: noqa: E402
 
 
-"runtime"
+"main"
 
 
 import getpass
-import inspect
 import os
 import pwd
-import readline
 import sys
 import termios
 import time
-import _thread
-
-
-from . import Client, Command, Default, Error, Event, Object, Storage
-from . import cdir, cmnd, debug, forever, launch, parse_command, spl, scan
-
 
-def __dir__():
-    return (
-        'Cfg',
-        'Console',
-        'daemon',
-        'daemoned',
-        'main',
-        'privileges',
-        'wrap',
-        'wrapped'
-    )
 
+from .client  import Client, cmnd
+from .default import Default
+from .errors  import Errors,debug
+from .event   import Event
+from .object  import cdir
+from .parser  import parse_cmd
+from .utils   import spl
+from .workdir import Workdir
+
+
+from . import modules
+
+Cfg          = Default()
+Cfg.mod      = "cmd,mod"
+Cfg.name     = sys.argv[0].split(os.sep)[-2]
+Cfg.dir      = os.path.expanduser(f"~/.{Cfg.name}")
+Cfg.pidfile  = os.path.join(Cfg.wd, f"{Cfg.name}.pid")
+Workdir.workdir = Cfg.dir
 
-__all__ = __dir__()
 
-
-Cfg         = Default()
-Cfg.name    = __file__.split(os.sep)[-2]
-Cfg.wd      = os.path.expanduser(f"~/.{Cfg.name}")
-Cfg.pidfile = os.path.join(Cfg.wd, f"{Cfg.name}.pid")
-Cfg.user    = getpass.getuser()
-Storage.wd  = Cfg.wd
-
-
-from sbn import modules
+dte = time.ctime(time.time()).replace("  ", " ")
+ext = os._exit 
 
 
 class Console(Client):
 
+    "Console"
+
     def announce(self, txt):
-        pass
+        "blind announce"
 
     def callback(self, evt):
+        "run and wait for callback to finish."
         Client.callback(self, evt)
-        evt.wait()
+        evt.wait(5.0)
 
     def poll(self):
+        "reconstruct event from input."
         evt = Event()
         evt.orig = object.__repr__(self)
         evt.txt = input("> ")
         evt.type = "command"
         return evt
 
-    def say(self, channel, txt):
+    def say(self, _channel, txt):
+        "say text in channel."
         txt = txt.encode('utf-8', 'replace').decode()
         print(txt)
 
 
 def daemon(pidfile, verbose=False):
+    "fork into the background."
     pid = os.fork()
     if pid != 0:
-        os._exit(0)
+        ext(0)
     os.setsid()
     pid2 = os.fork()
     if pid2 != 0:
-        os._exit(0)
+        ext(0)
     if not verbose:
         with open('/dev/null', 'r', encoding="utf-8") as sis:
             os.dup2(sis.fileno(), sys.stdin.fileno())
         with open('/dev/null', 'a+', encoding="utf-8") as sos:
             os.dup2(sos.fileno(), sys.stdout.fileno())
         with open('/dev/null', 'a+', encoding="utf-8") as ses:
             os.dup2(ses.fileno(), sys.stderr.fileno())
@@ -89,68 +86,88 @@
     if os.path.exists(pidfile):
         os.unlink(pidfile)
     cdir(os.path.dirname(pidfile))
     with open(pidfile, "w", encoding="utf-8") as fds:
         fds.write(str(os.getpid()))
 
 
-def daemoned():
-    Cfg.mod = ",".join(modules.__dir__())
-    daemon(Cfg.pidfile)
-    privileges(Cfg.user)
-    scan(modules, Cfg.mod, True)
-    forever()
+def init(pkg, modstr, disable=""):
+    "start inits in modules."
+    mds = []
+    for modname in spl(modstr):
+        if modname in spl(disable):
+            continue
+        module = getattr(pkg, modname, None)
+        if not module:
+            continue
+        if "init" in dir(module):
+            module.init()
+            mds.append(module)
+    return mds
 
 
 def privileges(username):
+    "lower privileges."
     pwnam = pwd.getpwnam(username)
     os.setgid(pwnam.pw_gid)
     os.setuid(pwnam.pw_uid)
 
 
 def wrap(func):
+    "restore terminal"
     old2 = None
     try:
         old2 = termios.tcgetattr(sys.stdin.fileno())
     except termios.error:
         pass
     try:
         func()
     except (KeyboardInterrupt, EOFError):
         print("")
     finally:
         if old2:
             termios.tcsetattr(sys.stdin.fileno(), termios.TCSADRAIN, old2)
 
 
+"runtime"
+
+
 def main():
-    Storage.skel()
-    parse_command(Cfg, " ".join(sys.argv[1:]))
-    if "x" in Cfg.opts:
-        Cfg.mod += ",cmd,flt,man,mod,mre,pwd,req,thr"
-    else:
-        Cfg.mod = ",".join(modules.__dir__())
+    "main code"
+    Workdir.skel()
+    Errors.enable(print)
+    parse_cmd(Cfg, " ".join(sys.argv[1:]))
+    result = None
+    if 'a' in Cfg.opts:
+        Cfg.mod = "," + ",".join(modules.__dir__())
     if "v" in Cfg.opts:
-        dte = time.ctime(time.time()).replace("  ", " ")
         debug(f"{Cfg.name.upper()} {Cfg.opts.upper()} started {dte}")
-    if "d" in Cfg.opts:
-        daemoned()
-    csl = Console()
     if "h" in Cfg.opts:
-        scan(modules, Cfg.mod)
-        cmnd("man")
-    if "c" in Cfg.opts:
-        scan(modules, Cfg.mod, True, Cfg.sets.dis, True)
+        print(__doc__)
+        return result
+    if "d" in Cfg.opts:
+        Cfg.mod = ",".join(modules.__dir__())
+        Cfg.user = getpass.getuser()
+        daemon(Cfg.pidfile, "v" in Cfg.opts)
+        privileges(Cfg.user)
+        init(modules, Cfg.mod)
+        while 1:
+            time.sleep(1.0)
+    elif "c" in Cfg.opts:
+        init(modules, Cfg.mod)
+        csl = Console()
         csl.start()
-        forever()
-    if Cfg.otxt:
-        scan(modules, Cfg.mod)
-        return cmnd(Cfg.otxt)
+        while 1:
+            time.sleep(1.0)
+    elif Cfg.otxt:
+        cmnd(Cfg.otxt, print)
+    return result
 
 
 def wrapped():
+    "wrapped code"
     wrap(main)
-    Error.show()
+    Errors.show()
 
 
 if __name__ == "__main__":
     wrapped()
```

### Comparing `sbn-92/sbn/excepts.py` & `sbn-94/sbn/errors.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,73 +1,87 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,R,W0125,E0402
+# pylint: disable=C,R,W0105,E1102
 
 
-"deferred exception handling"
+"errors"
 
 
 import io
 import traceback
 
 
-from .objects import Object
+class Errors:
 
-
-def __dir__():
-    return (
-        'Error',
-        'debug'
-    )
-
-
-__all__ = __dir__()
-
-
-class Error(Object):
+    "Errors"
 
     errors = []
     filter = []
-    output = print
+    output = None
     shown  = []
 
     @staticmethod
     def add(exc):
+        "add an exception"
         excp = exc.with_traceback(exc.__traceback__)
-        Error.errors.append(excp)
+        Errors.errors.append(excp)
+
+    @staticmethod
+    def enable(out):
+        "enable output"
+        Errors.output = out
 
     @staticmethod
     def format(exc):
+        "format an exception"
         res = ""
         stream = io.StringIO(
                              traceback.print_exception(
                                                        type(exc),
                                                        exc,
                                                        exc.__traceback__
                                                       )
                             )
         for line in stream.readlines():
             res += line + "\n"
         return res
 
     @staticmethod
-    def handle(exc):
-        if Error.output:
-            txt = str(Error.format(exc))
-            Error.output(txt)
+    def out(exc):
+        "check if output function is set."
+        if Errors.output is None:
+            return
+        txt = str(Errors.format(exc))
+        Errors.output(txt)
 
     @staticmethod
     def show():
-        for exc in Error.errors:
-            Error.handle(exc)
+        "show exceptions"
+        for exc in Errors.errors:
+            Errors.out(exc)
 
     @staticmethod
     def skip(txt):
-        for skp in Error.filter:
+        "check for skipping exceptions"
+        for skp in Errors.filter:
             if skp in str(txt):
                 return True
         return False
 
 
 def debug(txt):
-    if Error.output and not Error.skip(txt):
-        Error.output(txt)
+    "debug text"
+    if Errors.output and not Errors.skip(txt):
+        Errors.output(txt)
+
+
+"interface"
+
+
+def __dir__():
+    return (
+        'Errors',
+        'debug'
+    )
+
+
+__all__ = __dir__()
```

### Comparing `sbn-92/sbn/handler.py` & `sbn-94/sbn/handler.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,94 +1,80 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,R,W0212,E0402
+# pylint: disable=C,R,W0105,W0212,W0718
 
 
-"event handler"
+"handler"
 
 
 import queue
 import threading
 import _thread
 
 
-from .brokers import Fleet
-from .objects import Default, Object
-from .threads import launch
+from .errors  import Errors
+from .object  import Object
+from .thread  import launch
 
 
-def __dir__():
-    return (
-        'Event',
-        'Handler'
-   ) 
+class Handler:
 
-
-__all__ = __dir__()
-
-
-class Handler(Object):
+    "Handler"
 
     def __init__(self):
-        Object.__init__(self)
-        self.cbs      = Object()
+        self.cbs = Object()
         self.queue    = queue.Queue()
         self.stopped  = threading.Event()
+        self.threaded = True
 
     def callback(self, evt):
+        "call callback based on event type."
         func = getattr(self.cbs, evt.type, None)
-        if not func:
-            evt.ready()
-            return
-        evt._thr = launch(func, evt)
- 
+        if func:
+            if self.threaded:
+                evt._thr = launch(func, evt)
+            else:
+                func(evt)
+
     def loop(self):
+        "proces events until interrupted."
         while not self.stopped.is_set():
             try:
-                self.callback(self.poll())
+                evt = self.poll()
+                self.callback(evt)
             except (KeyboardInterrupt, EOFError):
                 _thread.interrupt_main()
+            except Exception as ex:
+                Errors.add(ex)
+                evt.ready()
 
     def poll(self):
+        "function to return event."
         return self.queue.get()
 
     def put(self, evt):
+        "put event into the queue."
         self.queue.put_nowait(evt)
 
     def register(self, typ, cbs):
+        "register callback for a type."
         setattr(self.cbs, typ, cbs)
 
     def start(self):
+        "start the event loop."
         launch(self.loop)
 
     def stop(self):
+        "stop the event loop."
         self.stopped.set()
 
 
-class Event(Default):
+"interface"
 
-    def __init__(self):
-        Default.__init__(self)
-        self._ready  = threading.Event()
-        self._thr    = None
-        self.done    = False
-        self.orig    = None
-        self.result  = []
-        self.txt     = ""
-
-    def ready(self):
-        self._ready.set()
-
-    def reply(self, txt):
-        self.result.append(txt)
-
-    def show(self):
-        for txt in self.result:
-            bot = Fleet.byorig(self.orig) or Fleet.first()
-            if bot:
-                bot.say(self.channel, txt)
-
-    def wait(self):
-        if self._thr:
-            self._thr.join()
-        self._ready.wait()
-        return self.result
+
+def __dir__():
+    return (
+        'Handler',
+    )
+
+
+__all__ = __dir__()
```

### Comparing `sbn-92/sbn/modules/irc.py` & `sbn-94/sbn/modules/irc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,69 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,R,W0105,W0612,W0718,E0402
+# pylint: disable=C,R,W0105,W0718
+# ruff: noqa: F841
 
 
 "internet relay chat"
 
 
+import base64
 import os
 import queue
 import socket
 import ssl
 import textwrap
 import threading
 import time
 import _thread
 
 
-from .. import Default, Object, edit, fmt, keys
-from .. import Client, Command, Error, Event
-from .. import byorig, debug, last, launch, sync
+from ..broker  import Broker
+from ..client  import Client
+from ..default import Default
+from ..event   import Event
+from ..errors  import Errors, debug
+from ..object  import Object, edit, fmt, keys
+from ..persist import Persist, last, sync
+from ..thread  import launch
 
 
-Error.filter = ["PING", "PONG", "PRIVMSG"]
-
-
-NAME = __file__.split(os.sep)[-3]
+NAME    = __file__.split(os.sep)[-3]
+get     = Broker.get
+saylock = _thread.allocate_lock()
 
 
-saylock = _thread.allocate_lock()
+Errors.filter = ["PING", "PONG", "PRIVMSG"]
 
 
 def init():
+    "initialize a irc bot."
     irc = IRC()
     irc.start()
     irc.events.joined.wait()
     return irc
 
 
+def shutdown():
+    "shutdown irc bot."
+    for bot in Broker.all():
+        if "irc" not in type(bot):
+            continue
+        debug(f"IRC stopping {repr(bot)}")
+        bot.state.pongcheck = True
+        bot.state.keeprunning = False
+        bot.events.connected.clear()
+        bot.stop()
+
+
 class Config(Default):
 
+    "Config"
+
     channel = f'#{NAME}'
     commands = True
     control = '!'
     edited = time.time()
     nick = NAME
     port = 6667
     realname = NAME
@@ -61,16 +82,21 @@
         self.nick = self.nick or Config.nick
         self.port = self.port or Config.port
         self.realname = self.realname or Config.realname
         self.server = self.server or Config.server
         self.username = self.username or Config.username
 
 
+Persist.add(Config)
+
+
 class TextWrap(textwrap.TextWrapper):
 
+    "TextWrap"
+
     def __init__(self):
         super().__init__()
         self.break_long_words = False
         self.drop_whitespace = False
         self.fix_sentence_endings = True
         self.replace_whitespace = True
         self.tabsize = 4
@@ -78,47 +104,54 @@
 
 
 wrapper = TextWrap()
 
 
 class Output():
 
+    "Output"
+
     cache = Object()
 
     def __init__(self):
         self.dostop = threading.Event()
         self.oqueue = queue.Queue()
 
     def dosay(self, channel, txt):
+        "overload this."
         raise NotImplementedError
 
     @staticmethod
     def extend(channel, txtlist):
+        "add list of txt to channel cache."
         if channel not in Output.cache:
             Output.cache[channel] = []
         chanlist = getattr(Output.cache, channel)
         chanlist.extend(txtlist)
 
     @staticmethod
     def gettxt(channel):
+        "return text from channel cache."
         txt = None
         try:
             che = getattr(Output.cache, channel, None)
             if che:
                 txt = che.pop(0)
         except (KeyError, IndexError):
             pass
         return txt
 
     def oput(self, channel, txt):
+        "put text to output queue."
         if channel and channel not in dir(Output.cache):
             setattr(Output.cache, channel, [])
         self.oqueue.put_nowait((channel, txt))
 
     def out(self):
+        "output loop."
         while not self.dostop.is_set():
             (channel, txt) = self.oqueue.get()
             if channel is None and txt is None:
                 break
             if self.dostop.is_set():
                 break
             txtlist = wrapper.wrap(txt)
@@ -133,34 +166,39 @@
             _nr = -1
             for txt in txtlist:
                 _nr += 1
                 self.dosay(channel, txt)
 
     @staticmethod
     def size(chan):
+        "return size of channel cache."
         if chan in Output.cache:
             return len(getattr(Output.cache, chan, []))
         return 0
 
 
 class IRC(Client, Output):
 
+    "IRC"
+
     def __init__(self):
         Client.__init__(self)
         Output.__init__(self)
         self.buffer = []
         self.cfg = Config()
+        self.channels = []
         self.events = Default()
         self.events.authed = threading.Event()
         self.events.connected = threading.Event()
         self.events.joined = threading.Event()
         self.events.ready = threading.Event()
-        self.channels = []
         self.sock = None
         self.state = Default()
+        self.state.dostop = False
+        self.state.error = ""
         self.state.keeprunning = False
         self.state.lastline = ""
         self.state.nrconnect = 0
         self.state.nrsend = 0
         self.zelf = ''
         self.register('903', cb_h903)
         self.register('904', cb_h903)
@@ -168,20 +206,23 @@
         self.register('CAP', cb_cap)
         self.register('ERROR', cb_error)
         self.register('LOG', cb_log)
         self.register('NOTICE', cb_notice)
         self.register('PRIVMSG', cb_privmsg)
         self.register('QUIT', cb_quit)
         self.register("366", cb_ready)
+        Broker.add(self)
 
     def announce(self, txt):
+        "announce on all channels."
         for channel in self.channels:
             self.oput(channel, txt)
 
-    def command(self, cmd, *args):
+    def docommand(self, cmd, *args):
+        "send command to server."
         with saylock:
             if not args:
                 self.raw(cmd)
             elif len(args) == 1:
                 self.raw(f'{cmd.upper()} {args[0]}')
             elif len(args) == 2:
                 txt = ' '.join(args[1:])
@@ -190,14 +231,15 @@
                 txt = ' '.join(args[2:])
                 self.raw("{cmd.upper()} {args[0]} {args[1]} :{txt}")
             if (time.time() - self.state.last) < 5.0:
                 time.sleep(5.0)
             self.state.last = time.time()
 
     def connect(self, server, port=6667):
+        "connect to server."
         self.state.nrconnect += 1
         self.events.connected.clear()
         if self.cfg.password:
             debug("using SASL")
             self.cfg.sasl = True
             self.cfg.port = "6697"
             ctx = ssl.SSLContext(ssl.PROTOCOL_TLS)
@@ -216,101 +258,112 @@
             self.sock.setblocking(True)
             self.sock.settimeout(180.0)
             self.events.connected.set()
             return True
         return False
 
     def direct(self, txt):
+        "send text directly on the socket."
         with saylock:
             self.raw(txt)
             time.sleep(2.0)
 
     def disconnect(self):
+        "disconnect from server."
         try:
             self.sock.shutdown(2)
         except (
                 ssl.SSLError,
                 OSError,
                 BrokenPipeError
-               ) as ex:
+               ) as _ex:
             pass
         except Exception as ex:
-            Error.errors.append(ex)
+            Errors.add(ex)
 
     def doconnect(self, server, nck, port=6667):
+        "loop until connected."
         while 1:
             try:
                 if self.connect(server, port):
                     break
             except (
                     ssl.SSLError,
                     OSError,
                     ConnectionResetError
                    ) as ex:
-                self.state.errors = str(ex)
+                self.state.error = str(ex)
                 debug(str(ex))
             debug(f"sleeping {self.cfg.sleep} seconds")
             time.sleep(self.cfg.sleep)
         self.logon(server, nck)
 
     def event(self, txt):
+        "create an event."
         evt = self.parsing(txt)
         cmd = evt.command
         if cmd == 'PING':
             self.state.pongcheck = True
-            self.command('PONG', evt.txt or '')
+            self.docommand('PONG', evt.txt or '')
         elif cmd == 'PONG':
             self.state.pongcheck = False
         if cmd == '001':
             self.state.needconnect = False
             if self.cfg.servermodes:
-                self.command(f'MODE {self.cfg.nick} {self.cfg.servermodes}')
+                self.docommand(f'MODE {self.cfg.nick} {self.cfg.servermodes}')
             self.zelf = evt.args[-1]
         elif cmd == "376":
             self.joinall()
         elif cmd == '002':
             self.state.host = evt.args[2][:-1]
         elif cmd == '366':
-            self.state.errors = []
+            self.state.error = ""
             self.events.joined.set()
         elif cmd == '433':
-            self.state.errors = txt
+            self.state.error = txt
             nck = self.cfg.nick + '_'
-            self.command('NICK', nck)
+            self.docommand('NICK', nck)
         return evt
 
     def joinall(self):
+        "join all channels."
         for channel in self.channels:
-            self.command('JOIN', channel)
+            self.docommand('JOIN', channel)
 
     def keep(self):
+        "keep alive."
         while not self.stopped.is_set():
+            if self.state.stopkeep:
+                self.state.stopkeep = False
+                break
             self.events.connected.wait()
             self.events.authed.wait()
             self.state.keeprunning = True
             time.sleep(self.cfg.sleep)
             self.state.pongcheck = True
-            self.command('PING', self.cfg.server)
+            self.docommand('PING', self.cfg.server)
             if self.state.pongcheck:
                 debug("failed pongcheck, restarting")
                 self.state.pongcheck = False
                 self.state.keeprunning = False
                 self.events.connected.clear()
                 self.stop()
                 init()
                 break
 
     def logon(self, server, nck):
+        "log onto server,"
         self.events.connected.wait()
         self.events.authed.wait()
         self.direct(f'NICK {nck}')
         self.direct(f'USER {nck} {server} {server} {nck}')
 
 
     def parsing(self, txt):
+        "parse text into an event."
         rawstr = str(txt)
         rawstr = rawstr.replace('\u0001', '')
         rawstr = rawstr.replace('\001', '')
         debug(txt)
         obj = Event()
         obj.args = []
         obj.rawstr = rawstr
@@ -364,14 +417,15 @@
             obj.rest = " ".join(obj.args)
         obj.orig = object.__repr__(self)
         obj.txt = obj.txt.strip()
         obj.type = obj.command
         return obj
 
     def poll(self):
+        "poll for event."
         self.events.connected.wait()
         if not self.buffer:
             try:
                 self.some()
             except BlockingIOError as ex:
                 time.sleep(1.0)
                 return self.event(str(ex))
@@ -379,26 +433,27 @@
                     OSError,
                     socket.timeout,
                     ssl.SSLError,
                     ssl.SSLZeroReturnError,
                     ConnectionResetError,
                     BrokenPipeError
                    ) as ex:
-                Error.add(ex)
+                Errors.add(ex)
                 self.stop()
                 debug("handler stopped")
                 evt = self.event(str(ex))
                 return evt
         try:
             txt = self.buffer.pop(0)
         except IndexError:
             txt = ""
         return self.event(txt)
 
     def raw(self, txt):
+        "send raw text."
         txt = txt.rstrip()
         debug(txt)
         txt = txt[:500]
         txt += '\r\n'
         txt = bytes(txt, 'utf-8')
         if self.sock:
             try:
@@ -406,173 +461,239 @@
             except (
                     OSError,
                     ssl.SSLError,
                     ssl.SSLZeroReturnError,
                     ConnectionResetError,
                     BrokenPipeError
                    ) as ex:
-                Error.errors.append(ex)
+                Errors.add(ex)
                 self.stop()
                 return
         self.state.last = time.time()
         self.state.nrsend += 1
 
     def reconnect(self):
+        "reconnect to server."
         debug(f"reconnecting to {self.cfg.server}")
         try:
             self.disconnect()
         except (ssl.SSLError, OSError):
             pass
         self.events.connected.clear()
         self.events.joined.clear()
         self.doconnect(self.cfg.server, self.cfg.nick, int(self.cfg.port))
 
     def dosay(self, channel, txt):
+        "method for output cache."
         self.events.joined.wait()
         txt = str(txt).replace('\n', '')
         txt = txt.replace('  ', ' ')
-        self.command('PRIVMSG', channel, txt)
+        self.docommand('PRIVMSG', channel, txt)
 
     def say(self, channel, txt):
+        "say text on channel."
         self.oput(channel, txt)
 
     def some(self):
+        "parse part of input text."
         self.events.connected.wait()
         if not self.sock:
             return
         inbytes = self.sock.recv(512)
         txt = str(inbytes, 'utf-8')
         if txt == '':
             raise ConnectionResetError
         self.state.lastline += txt
         splitted = self.state.lastline.split('\r\n')
         for line in splitted[:-1]:
             self.buffer.append(line)
         self.state.lastline = splitted[-1]
 
     def start(self):
+        "start bot."
         last(self.cfg)
         if self.cfg.channel not in self.channels:
             self.channels.append(self.cfg.channel)
         self.events.connected.clear()
         self.events.joined.clear()
         launch(Output.out, self)
-        Client.start(self)
+        launch(Client.start, self)
         launch(
                self.doconnect,
                self.cfg.server or "localhost",
                self.cfg.nick,
                int(self.cfg.port or '6667')
               )
         if not self.state.keeprunning:
             launch(self.keep)
 
     def stop(self):
+        "stop bot."
+        self.state.stopkeep = True
         self.disconnect()
         self.dostop.set()
         self.oput(None, None)
         Client.stop(self)
 
     def wait(self):
+        "wait for ready."
         self.events.ready.wait()
 
 
+"callbacks"
+
+
 def cb_auth(evt):
-    bot = byorig(evt.orig)
-    bot.command(f'AUTHENTICATE {bot.cfg.password}')
+    "auth callback."
+    bot = get(evt.orig)
+    bot.docommand(f'AUTHENTICATE {bot.cfg.password}')
 
 
 def cb_cap(evt):
-    bot = byorig(evt.orig)
+    "capabilities callback."
+    bot = get(evt.orig)
     if bot.cfg.password and 'ACK' in evt.arguments:
         bot.direct('AUTHENTICATE PLAIN')
     else:
         bot.direct('CAP REQ :sasl')
 
 
 def cb_error(evt):
-    bot = byorig(evt.orig)
+    "error callback."
+    bot = get(evt.orig)
+    if not bot.state.nrerror:
+        bot.state.nrerror = 0
     bot.state.nrerror += 1
-    bot.state.errors.append(evt.txt)
+    bot.state.error = evt.txt
     debug(evt.txt)
 
 
 def cb_h903(evt):
-    bot = byorig(evt.orig)
+    "auth succeded callback."
+    bot = get(evt.orig)
     bot.direct('CAP END')
     bot.events.authed.set()
 
 
 def cb_h904(evt):
-    bot = byorig(evt.orig)
+    "auth succeded callback."
+    bot = get(evt.orig)
     bot.direct('CAP END')
     bot.events.authed.set()
 
 
 def cb_kill(evt):
-    pass
+    "got killed callback."
 
 
 def cb_log(evt):
-    pass
+    "log callback."
 
 
 def cb_ready(evt):
-    bot = byorig(evt.orig)
+    "bot is ready callback."
+    bot = get(evt.orig)
     if bot:
         bot.events.ready.set()
 
 
 def cb_001(evt):
-    bot = byorig(evt.orig)
+    "first line received callback."
+    bot = get(evt.orig)
     bot.logon()
 
 
 def cb_notice(evt):
-    bot = byorig(evt.orig)
+    "notice callback."
+    bot = get(evt.orig)
     if evt.txt.startswith('VERSION'):
         txt = f'\001VERSION {NAME.upper()} 140 - {bot.cfg.username}\001'
-        bot.command('NOTICE', evt.channel, txt)
+        bot.docommand('NOTICE', evt.channel, txt)
 
 
 def cb_privmsg(evt):
-    bot = byorig(evt.orig)
+    "privmsg callback."
+    bot = get(evt.orig)
     if not bot.cfg.commands:
         return
     if evt.txt:
         if evt.txt[0] in ['!',]:
             evt.txt = evt.txt[1:]
         elif evt.txt.startswith(f'{bot.cfg.nick}:'):
             evt.txt = evt.txt[len(bot.cfg.nick)+1:]
         else:
             return
         if evt.txt:
             evt.txt = evt.txt[0].lower() + evt.txt[1:]
         debug(f"command from {evt.origin}: {evt.txt}")
-        Command.handle(evt)
+        bot.command(evt)
 
 
 def cb_quit(evt):
-    bot = byorig(evt.orig)
+    "quit callback."
+    bot = get(evt.orig)
     debug(f"quit from {bot.cfg.server}")
     if evt.orig and evt.orig in bot.zelf:
         bot.stop()
 
 
 "commands"
 
 
 def cfg(event):
+    "configure command."
     config = Config()
     path = last(config)
     if not event.sets:
         event.reply(
                     fmt(
                         config,
                         keys(config),
                         skip='control,password,realname,sleep,username'.split(",")
                        )
                    )
     else:
         edit(config, event.sets)
         sync(config, path)
         event.reply('ok')
+
+
+def mre(event):
+    "show from output cache."
+    if not event.channel:
+        event.reply('channel is not set.')
+        return
+    bot = Broker.get(event.orig)
+    if 'cache' not in dir(bot):
+        event.reply('bot is missing cache')
+        return
+    if event.channel not in bot.cache:
+        event.reply(f'no output in {event.channel} cache.')
+        return
+    for _x in range(3):
+        txt = bot.gettxt(event.channel)
+        if txt:
+            bot.say(event.channel, txt)
+    size = bot.size(event.channel)
+    event.reply(f'{size} more in cache')
+
+
+def pwd(event):
+    "create a base64 password."
+    if len(event.args) != 2:
+        event.reply('pwd <nick> <password>')
+        return
+    arg1 = event.args[0]
+    arg2 = event.args[1]
+    txt = f'\x00{arg1}\x00{arg2}'
+    enc = txt.encode('ascii')
+    base = base64.b64encode(enc)
+    dcd = base.decode('ascii')
+    event.reply(dcd)
+
+
+"register"
+
+
+Client.add(cfg)
+Client.add(mre)
+Client.add(pwd)
```

### Comparing `sbn-92/sbn/modules/log.py` & `sbn-94/sbn/modules/log.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,53 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=R,C,E0402
+# pylint: disable=C,R,W0105
 
 
 "log text"
 
 
 import time
 
 
-from .. import Object, find, fntime, laps, sync
+from ..client  import Client
+from ..object  import Object
+from ..persist import Persist, find, fntime, sync
+from ..utils   import laps
 
 
 class Log(Object):
 
+    "Log"
+
     def __init__(self):
-        super().__init__()
+        Object.__init__()
         self.txt = ''
 
+    def __yo__(self):
+        pass
+
+    def __yoyo__(self):
+        pass
+
 
 def log(event):
+    "log text."
     if not event.rest:
         nmr = 0
         for fnm, obj in find('log'):
             lap = laps(time.time() - fntime(fnm))
             event.reply(f'{nmr} {obj.txt} {lap}')
             nmr += 1
         if not nmr:
             event.reply('no log')
         return
     obj = Log()
     obj.txt = event.rest
     sync(obj)
     event.reply('ok')
+
+
+"register"
+
+Client.add(log)
+Persist.add(Log)
```

### Comparing `sbn-92/sbn/modules/mdl.py` & `sbn-94/sbn/modules/mdl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,48 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,R,W0613,E0402
+# pylint: disable=C,R,W0105
 
 
 "genocide model of the netherlands"
 
 
 import datetime
 import time
 
 
-from .. import Object, construct, keys
-from .. import Event, Fleet, Repeater, laps, launch
+from ..broker   import Broker
+from ..client   import Client
+from ..event    import Event
+from ..object   import Object, construct, keys
+from ..repeater import Repeater
+from ..thread   import launch
+from ..utils    import laps
 
 
 def __dir__():
     return (
             'init',
             'now'
-           ) 
+           )
 
 
 def init():
+    "start genocide model."
     for key in keys(oorzaken):
         val = getattr(oorzaken, key, None)
         if val and int(val) > 10000:
             evt = Event()
             evt.txt = ""
             evt.rest = key
             sec = seconds(val)
             repeater = Repeater(sec, cbstats, evt, thrname=aliases.get(key))
             repeater.start()
     launch(daily, name="daily")
-    
+
 
 DAY = 24*60*60
 YEAR = 365*DAY
 SOURCE = "https://github.com/bthate/genocide"
 STARTDATE = "2020-01-01 00:00:00"
 STARTTIME = time.mktime(time.strptime(STARTDATE, "%Y-%m-%d %H:%M:%S"))
 
@@ -273,123 +279,130 @@
 
 
 oorzaak = Object()
 construct(oorzaak, zip(oor, aantal))
 oorzaken = Object()
 
 
-
 def getalias(txt):
+    "teturn matching alias."
+    result = None
     for key, value in aliases.items():
         if txt.lower() in key.lower():
-            return value
+            result = value
+            break
+    return result
 
 
 def getday():
+    "return timestamp of current day."
     day = datetime.datetime.now()
     day = day.replace(hour=0, minute=0, second=0, microsecond=0)
     return day.timestamp()
 
 
 def getnr(name):
+    "return number of deaths by name."
     for k in keys(oorzaken):
         if name.lower() in k.lower():
             return int(getattr(oorzaken, k))
     return 0
 
 
 def seconds(nrs):
+    "calculate sedconds"
     if not nrs:
         return nrs
     return 60*60*24*365 / float(nrs)
 
 
 
 def iswanted(k, line):
+    "see whether an item is wanted."
     for word in line:
         if word in k:
             return True
     return False
 
 
 def daily():
+    "run a callback daily."
     while 1:
         time.sleep(24*60*60)
-        evt = Event()
-        cbnow(evt)
+        cbnow(Event())
 
 
 def hourly():
+    "run a callback hourly."
     while 1:
         time.sleep(60*60)
-        evt = Event()
-        cbnow(evt)
+        cbnow(Event())
 
 
 def cbnow(evt):
+    "check status now callback."
+    if not evt:
+        evt = Event()
     delta = time.time() - STARTTIME
     txt = laps(delta) + " "
     for name in sorted(keys(oorzaken), key=lambda x: seconds(getnr(x))):
         needed = seconds(getnr(name))
         if needed > 60*60:
             continue
         nrtimes = int(delta/needed)
-        txt += "%s: %s " % (getalias(name), nrtimes)
+        txt += f"{getalias(name)}: {nrtimes}"
     txt += " http://genocide.rtfd.io"
-    for bot in Fleet.objs:
+    for bot in Broker.all():
         if "announce" in dir(bot):
             bot.announce(txt)
 
 
 def cbstats(evt):
+    "callback showing stats."
     name = evt.rest or "Psych"
     needed = seconds(getnr(name))
     if needed:
         delta = time.time() - STARTTIME
-        nrtimes = int(delta/needed)
-        nryear = int(YEAR/needed)
-        nrday = int(DAY/needed)
+        nrt = int(delta/needed)
+        nry = int(YEAR/needed)
+        nrd = int(DAY/needed)
         delta2 = time.time() - getday()
-        thisday = int(delta2/needed)
-        txt = "patient #%s died from %s (%s/%s) every %s (%s/year)" % (
-                                                               nrtimes,
-                                                               getalias(name),
-                                                               thisday,
-                                                               nrday,
-                                                               laps(needed),
-                                                               nryear,
-                                                              )
-        for bot in Fleet.objs:
+        this = int(delta2/needed)
+        txt = f"#{nrt} died from {getalias(name)} ({this}/{nrd}) every {laps(needed)} ({nry}/year)"
+        for bot in Broker.all():
             bot.announce(txt)
 
 
 def now(event):
+    "showing number of psychiatric patients victims."
     name = event.rest or "Psych"
     needed = seconds(getnr(name))
     if needed:
         delta = time.time() - STARTTIME
         txt = laps(delta) + " "
-        nrtimes = int(delta/needed)
-        nryear = int(YEAR/needed)
-        nrday = int(DAY/needed)
-        thisday = int(DAY % needed)
-        txt += "patient #%s died from %s (%s/%s/%s) every %s" % (
-                                                                 nrtimes,
-                                                                 getalias(name),
-                                                                 thisday,
-                                                                 nrday,
-                                                                 nryear,
-                                                                 laps(needed)
-                                                                )
+        nrt = int(delta/needed)
+        nrd = int(DAY/needed)
+        this = int(DAY % needed)
+        txt = f"#{nrt} died from {getalias(name)} ({this}/{nrd}) every {laps(needed)}"
         event.reply(txt)
     else:
         event.reply("not needed")
 
 
+"register"
+
+
+Client.add(now)
+
+
+"runtime"
+
+
 def boot():
+    "format model data."
     _nr = -1
     for key in keys(oorzaak):
         _nr += 1
         if _nr == 0:
             continue
         if key.startswith('"'):
             key = key[1:]
```

### Comparing `sbn-92/sbn/modules/req.py` & `sbn-94/sbn/modules/req.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C0115,C0116
+# pylint: disable=C.R,W0105
 
 
 """| **Information and Evidence Unit**
 | **Office of the Prosecutor**
 | **Post Office Box 19519**
 | **2500 CM The Hague**
 | **The Netherlands**
@@ -75,9 +75,19 @@
 
 
 (1) provided are the confirmation letters of both the chamber and the king.
 (2) your reference: OTP-CR-117/19
 """
 
 
+from ..client import Client
+
+
 def req(event):
+    "show request."
     event.reply(__doc__)
+
+
+"register"
+
+
+Client.add(req)
```

### Comparing `sbn-92/sbn/modules/rst.py` & `sbn-94/sbn/modules/rst.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,111 +1,141 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,R,W0612,W0613
+# pylint: disable=C,R,W0105
 
 
-""" rest interface. """
+"rest"
 
 
 import os
 import sys
 import time
 
 
 from http.server import HTTPServer, BaseHTTPRequestHandler
 
 
-from .. import Default, Object
-from .. import Error, Storage, debug, launch
-
-
-def init():
-    rest = REST((Config.hostname, int(Config.port)), RESTHandler)
-    launch(rest.start)
-    return rest
-
-
-def html(txt):
-    return """<!doctype html>
-<html>
-   %s
-</html>
-""" % txt
+from ..default import Default
+from ..errors  import Errors, debug
+from ..object  import Object
+from ..persist import Persist, Workdir
+from ..thread  import launch
 
 
 class Config(Default):
 
+    "Config"
+
     hostname = "localhost"
     port     = 10102
 
+    def __bla__(self):
+        pass
+
+    def __blabla__(self):
+        pass
+
 
 class REST(HTTPServer, Object):
 
+    "REST"
+
     allow_reuse_address = True
     daemon_thread = True
 
     def __init__(self, *args, **kwargs):
         HTTPServer.__init__(self, *args, **kwargs)
         Object.__init__(self)
         self.host = args[0]
         self._last = time.time()
         self._starttime = time.time()
         self._status = "start"
 
     def exit(self):
+        "shutdown server."
         self._status = ""
         time.sleep(0.2)
         self.shutdown()
 
-    def start(self): 
+    def start(self):
+        "start server/"
         self._status = "ok"
         self.serve_forever()
 
     def request(self):
+        "handler request."
         self._last = time.time()
 
     def error(self, request, addr):
-        exctype, excvalue, tb = sys.exc_info()
+        "handle error."
+        exctype, excvalue, _tb = sys.exc_info()
         exc = exctype(excvalue)
-        Error.add(exc)
-        debug('%s %s' % (addr, excvalue))
+        Errors.add(exc)
+        if request:
+            debug(f'{addr} {excvalue}')
 
 
 class RESTHandler(BaseHTTPRequestHandler):
 
+    "RESTHandler"
+
     def setup(self):
+        "setup request."
         BaseHTTPRequestHandler.setup(self)
         self._ip = self.client_address[0]
         self._size = 0
 
     def send(self, txt):
+        "send text."
         self.wfile.write(bytes(txt, "utf-8"))
         self.wfile.flush()
 
     def write_header(self, htype='text/plain'):
+        "write a header."
         self.send_response(200)
-        self.send_header('Content-type', '%s; charset=%s ' % (htype, "utf-8"))
+        self.send_header('Content-type', f'{htype}; charset="utf-8"')
         self.send_header('Server', "1")
         self.end_headers()
 
-    def do_GET(self):
+    def do_GET(self): # pylint: disable=C0103
+        "handle GET."
         if self.path == "/":
             self.write_header("text/html")
             txt = ""
-            for fnm in Storage.fns():
+            for fnm in Persist.fns():
                 txt += f'<a href="http://{Config.hostname}:{Config.port}/{fnm}">{fnm}</a>\n'
             self.send(html(txt.strip()))
             return
-        fnm = Storage.wd + os.sep + "store" + os.sep + self.path
+        fnm = Workdir.workdir + os.sep + "store" + os.sep + self.path
         try:
-            f = open(fnm, "r", encoding="utf-8")
-            txt = f.read()
-            f.close()
-            self.write_header("txt/plain")
-            self.send(html(txt))
+            with open(fnm, "r", encoding="utf-8") as file:
+                txt = file.read()
+                self.write_header("txt/plain")
+                self.send(html(txt))
         except (TypeError, FileNotFoundError, IsADirectoryError) as ex:
             self.send_response(404)
-            Error.add(ex)
+            Errors.add(ex)
             self.end_headers()
 
     def log(self, code):
-        debug('%s code %s path %s' % (self.address_string(), code, self.path))
+        "log access."
+        debug(f"{self.address_string()} code {code} path {self.path}")
+
+
+def html(txt):
+    "html template."
+    return f"<!doctype html><html>{txt}</html>"
+
+
+"runtime"
+
+
+def init():
+    "start object server."
+    result = None
+    try:
+        result = REST((Config.hostname, int(Config.port)), RESTHandler)
+    except OSError:
+        pass
+    if result:
+        launch(result.start)
+    return result
```

### Comparing `sbn-92/sbn/modules/thr.py` & `sbn-94/sbn/modules/thr.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C0116,W0105,E0402,E0401,E0611
+# pylint: disable=C,R,W0105
 
 
 "show running threads"
 
 
 import threading
 import time
 
 
-from .. import Object, laps, update
+from ..client  import Client
+from ..object  import Object, update
+from ..utils   import laps
 
 
 STARTTIME = time.time()
 
 
 def thr(event):
+    "show running threads."
     result = []
     for thread in sorted(threading.enumerate(), key=lambda x: x.name):
         if str(thread).startswith('<_'):
             continue
         obj = Object()
         update(obj, vars(thread))
         if getattr(obj, 'sleep', None):
@@ -34,7 +37,13 @@
     for uptime, txt in sorted(result, key=lambda x: x[1]):
         lap = laps(uptime)
         res.append(f'{txt}/{lap}')
     if res:
         event.reply(' '.join(res))
     else:
         event.reply('no threads')
+
+
+"initialize"
+
+
+Client.add(thr)
```

### Comparing `sbn-92/sbn/modules/udp.py` & `sbn-94/sbn/modules/udp.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,57 +1,71 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C0115,C0116,W0105,E0402,R0903
+# pylint: disable=C,R,W0105
 
 
 "udp to irc relay"
 
 
 import select
 import socket
 import sys
 import threading
 import time
 
 
-from .. import Fleet, Object, launch
+from dataclasses import dataclass
+
+
+from ..broker import Broker
+from ..client import Client
+from ..object import Object
+from ..thread import launch
 
 
 def init():
+    "start udp to irc relay."
     udpd = UDP()
     udpd.start()
     return udpd
 
 
+@dataclass
 class Cfg(Object):
 
+    "Cfg"
+
     addr = ""
     host = "localhost"
     port = 5500
 
 
 class UDP(Object):
 
+    "UDP"
+
     def __init__(self):
         Object.__init__(self)
         self.stopped = False
         self._sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
         self._sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
         self._sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEPORT, 1)
         self._sock.setblocking(1)
         self._starttime = time.time()
         self.ready = threading.Event()
 
     def output(self, txt, addr=None):
+        "output to fleet."
         if addr:
             Cfg.addr = addr
-        for bot in Fleet.objs:
+        for bot in Broker.all():
             bot.announce(txt.replace("\00", ""))
 
     def loop(self):
+        "udp input loop."
         try:
             self._sock.bind((Cfg.host, Cfg.port))
         except socket.gaierror:
             return
         self.ready.set()
         while not self.stopped:
             (txt, addr) = self._sock.recvfrom(64000)
@@ -59,31 +73,38 @@
                 break
             data = str(txt.rstrip(), "utf-8")
             if not data:
                 break
             self.output(data, addr)
 
     def exit(self):
+        "stop relay."
         self.stopped = True
         self._sock.settimeout(0.01)
         self._sock.sendto(
                           bytes("exit", "utf-8"),
                           (Cfg.host, Cfg.port)
                          )
 
     def start(self):
+        "start relay."
         launch(self.loop)
 
 
 def toudp(host, port, txt):
+    "send udp packet to bot."
     sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
     sock.sendto(bytes(txt.strip(), "utf-8"), (host, port))
 
 
+"commands"
+
+
 def udp(event):
+    "send udp command."
     if event.rest:
         toudp(Cfg.host, Cfg.port, event.rest)
         event.reply(f"{len(event.rest)} characters sent")
         return
     if not select.select(
                          [sys.stdin, ],
                          [],
@@ -109,7 +130,13 @@
             if not txt:
                 stop = True
                 break
             size += len(txt)
             toudp(Cfg.host, Cfg.port, txt)
         if stop:
             break
+
+
+"register"
+
+
+Client.add(udp)
```

### Comparing `sbn-92/sbn/objects.py` & `sbn-94/sbn/object.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,178 +1,57 @@
 # This file is placed in the Public Domain.
 #
 # pylint: disable=C,R,W0105
 
 
-"a clean namespace"
+"object"
 
 
-import pathlib
 import json
 import os
+import pathlib
 import _thread
 
 
-def __dir__():
-    return (
-        'Default',
-        'Object',
-        'cdir',
-        'construct',
-        'edit',
-        'fmt',
-        'fqn',
-        'items',
-        'keys',
-        'read',
-        'update',
-        'values',
-        'write'
-    )
-
-
-__all__ = __dir__()
-
-
-lock = _thread.allocate_lock()
-
-
-def cdir(pth) -> None:
-    if os.path.exists(pth):
-        return
-    pth = pathlib.Path(pth)
-    os.makedirs(pth, exist_ok=True)
+disklock = _thread.allocate_lock()
 
 
 class Object:
 
+    "Object"
+
     def __contains__(self, key):
         return key in dir(self)
 
     def __iter__(self):
         return iter(self.__dict__)
 
     def __len__(self):
         return len(self.__dict__)
 
-    def __repr__(self):
-        return dumps(self)
-
     def __str__(self):
         return str(self.__dict__)
 
 
-class Default(Object):
-
-    __slots__ = ("__default__",)
-
-    def __init__(self):
-        Object.__init__(self)
-        self.__default__ = ""
-
-    def __getattr__(self, key):
-        return self.__dict__.get(key, self.__default__)
-
-
-class ObjectDecoder(json.JSONDecoder):
-
-    def decode(self, s, _w=None):
-        val = json.JSONDecoder.decode(self, s)
-        if not val:
-            val = {}
-        return hook(val)
-
-    def raw_decode(self, s, idx=0):
-        return json.JSONDecoder.raw_decode(self, s, idx)
-
-
-def hook(objdict, typ=None):
-    if typ:
-        obj = typ()
-    else:
-        obj = Object()
-    construct(obj, objdict)
-    return obj
-
-
-def load(fpt, *args, **kw):
-    kw["cls"] = ObjectDecoder
-    kw["object_hook"] = hook
-    return json.load(fpt, *args, **kw)
-
-
-def loads(string, *args, **kw):
-    kw["cls"] = ObjectDecoder
-    kw["object_hook"] = hook
-    return json.loads(string, *args, **kw)
-
-
-class ObjectEncoder(json.JSONEncoder):
-
-    def default(self, o):
-        if isinstance(o, dict):
-            return o.items()
-        if isinstance(o, Object):
-            return vars(o)
-        if isinstance(o, list):
-            return iter(o)
-        if isinstance(
-                      o,
-                      (
-                       type(str),
-                       type(True),
-                       type(False),
-                       type(int),
-                       type(float)
-                      )
-                     ):
-            return o
-        try:
-            return json.JSONEncoder.default(self, o)
-        except TypeError:
-            return object.__repr__(o)
-
-    def encode(self, o) -> str:
-        return json.JSONEncoder.encode(self, o)
-
-    def iterencode(
-                   self,
-                   o,
-                   _one_shot=False
-                  ):
-        return json.JSONEncoder.iterencode(self, o, _one_shot)
-
-
-def dump(*args, **kw) -> None:
-    kw["cls"] = ObjectEncoder
-    return json.dump(*args, **kw)
-
-
-def dumps(*args, **kw) -> str:
-    kw["cls"] = ObjectEncoder
-    return json.dumps(*args, **kw)
-
-
-"methods"
-
-
 def construct(obj, *args, **kwargs):
+    "construct an object from provided arguments."
     if args:
         val = args[0]
         if isinstance(val, zip):
             update(obj, dict(val))
         elif isinstance(val, dict):
             update(obj, val)
         elif isinstance(val, Object):
             update(obj, vars(val))
     if kwargs:
         update(obj, kwargs)
 
 
 def edit(obj, setter, skip=False):
+    "edit an object from provided dict/dict-like."
     for key, val in items(setter):
         if skip and val == "":
             continue
         try:
             setattr(obj, key, int(val))
             continue
         except ValueError:
@@ -187,14 +66,15 @@
         elif val in ["False", "false"]:
             setattr(obj, key, False)
         else:
             setattr(obj, key, val)
 
 
 def fmt(obj, args=None, skip=None, plain=False):
+    "format an object to a printable string."
     if args is None:
         args = keys(obj)
     if skip is None:
         skip = []
     txt = ""
     for key in args:
         if key.startswith("__"):
@@ -205,52 +85,196 @@
         if value is None:
             continue
         if plain:
             txt += f"{value} "
         elif isinstance(value, str) and len(value.split()) >= 2:
             txt += f'{key}="{value}" '
         else:
-            txt += f'{key}={value} '
+            txt += f"{key}={value} "
     return txt.strip()
 
 
 def fqn(obj):
+    "return full qualified name of an object."
     kin = str(type(obj)).split()[-1][1:-2]
     if kin == "type":
         kin = obj.__name__
     return kin
 
 
 def items(obj):
+    "return the items of an object."
     if isinstance(obj, type({})):
         return obj.items()
     return obj.__dict__.items()
 
 
 def keys(obj):
+    "return keys of an object."
     if isinstance(obj, type({})):
         return obj.keys()
     return list(obj.__dict__.keys())
 
 
 def read(obj, pth):
-    with lock:
+    "read an object from file path."
+    with disklock:
         with open(pth, 'r', encoding='utf-8') as ofile:
             update(obj, load(ofile))
 
 
+def search(obj, selector):
+    "check if object matches provided values."
+    res = False
+    if not selector:
+        return True
+    for key, value in items(selector):
+        val = getattr(obj, key, None)
+        if str(value).lower() in str(val).lower():
+            res = True
+        else:
+            res = False
+            break
+    return res
+
+
 def update(obj, data, empty=True):
+    "update an object."
     for key, value in items(data):
         if empty and not value:
             continue
         setattr(obj, key, value)
 
 
 def values(obj):
+    "return values of an object."
     return obj.__dict__.values()
 
 
 def write(obj, pth):
-    with lock:
+    "write an object to disk."
+    with disklock:
         cdir(os.path.dirname(pth))
         with open(pth, 'w', encoding='utf-8') as ofile:
-            dump(obj, ofile)
+            dump(obj, ofile, indent=4)
+
+
+class ObjectDecoder(json.JSONDecoder):
+
+    "ObjectDecoder"
+
+    def __init__(self, *args, **kwargs):
+        json.JSONDecoder.__init__(self, *args, **kwargs)
+
+    def decode(self, s, _w=None):
+        "decoding string to object."
+        val = json.JSONDecoder.decode(self, s)
+        if not val:
+            val = {}
+        return hook(val)
+
+    def raw_decode(self, s, idx=0):
+        "decode partial string to object."
+        return json.JSONDecoder.raw_decode(self, s, idx)
+
+
+def hook(objdict, typ=None):
+    "construct object from dict."
+    if typ:
+        obj = typ()
+    else:
+        obj = Object()
+    construct(obj, objdict)
+    return obj
+
+
+def load(fpt, *args, **kw):
+    "load object from file."
+    kw["cls"] = ObjectDecoder
+    kw["object_hook"] = hook
+    return json.load(fpt, *args, **kw)
+
+
+def loads(string, *args, **kw):
+    "load object from string."
+    kw["cls"] = ObjectDecoder
+    kw["object_hook"] = hook
+    return json.loads(string, *args, **kw)
+
+
+class ObjectEncoder(json.JSONEncoder):
+
+    "ObjectEncoder"
+
+    def __init__(self, *args, **kwargs):
+        json.JSONEncoder.__init__(self, *args, **kwargs)
+
+    def default(self, o):
+        "return stringable value."
+        if isinstance(o, dict):
+            return o.items()
+        if isinstance(o, Object):
+            return vars(o)
+        if isinstance(o, list):
+            return iter(o)
+        if isinstance(o, (type(str), type(True), type(False), type(int), type(float))):
+            return o
+        try:
+            return json.JSONEncoder.default(self, o)
+        except TypeError:
+            return o.__dict__
+
+    def encode(self, o) -> str:
+        "encode object to string."
+        return json.JSONEncoder.encode(self, o)
+
+    def iterencode(self, o, _one_shot=False):
+        "loop over object to encode to string."
+        return json.JSONEncoder.iterencode(self, o, _one_shot)
+
+
+def dump(*args, **kw):
+    "dump object to file."
+    kw["cls"] = ObjectEncoder
+    return json.dump(*args, **kw)
+
+
+def dumps(*args, **kw):
+    "dump object to string."
+    kw["cls"] = ObjectEncoder
+    return json.dumps(*args, **kw)
+
+
+def cdir(pth):
+    "create directory."
+    if os.path.exists(pth):
+        return
+    pth = pathlib.Path(pth)
+    os.makedirs(pth, exist_ok=True)
+
+
+"interface"
+
+
+def __dir__():
+    return (
+        'Object',
+        'construct',
+        'dump',
+        'dumps',
+        'edit',
+        'fmt',
+        'fqn',
+        'hook',
+        'items',
+        'keys',
+        'load',
+        'loads',
+        'read',
+        'search',
+        'update',
+        'values',
+        'write'
+    )
+
+
+__all__ = __dir__()
```

### Comparing `sbn-92/sbn/parsers.py` & `sbn-94/sbn/modules/tmr.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,31 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,R,W0718,W0702,E0402
+# pylint: disable=C,R,W0105
 
 
-"parsing text"
+"timer"
 
 
 import datetime
-import os
 import re
 import time as ttime
 
 
-from .objects import Default
+from ..broker  import Broker
+from ..client  import Client
+from ..event   import Event
+from ..object  import update
+from ..persist import Persist, find, sync
+from ..thread  import launch
+from ..timer   import Timer
+from ..utils   import laps
 
 
-def __dir__():
-    return (
-        'NoDate',
-        'fntime',
-        'get_day',
-        'get_hour',
-        'get_time',
-        'laps',
-        'parse_command',
-        'parse_time',
-        'spl',
-        'today',
-        'to_day'
-    )
-
-
-__all__ = __dir__()
-
-
-bdmonths = [
+MONTHS = [
     'Bo',
     'Jan',
     'Feb',
     'Mar',
     'Apr',
     'May',
     'Jun',
@@ -47,69 +34,67 @@
     'Sep',
     'Oct',
     'Nov',
     'Dec'
 ]
 
 
-year_formats = [
+FORMATS = [
     "%Y-%m-%d",
     "%d-%m-%Y",
     "%d-%m",
     "%m-%d",
 ]
 
 
 class NoDate(Exception):
 
-    pass
+    "NoDate"
 
 
 def extract_date(daystr):
-    for fmt in year_formats:
+    "extract date from string."
+    res = None
+    for fmt in FORMATS:
         try:
             res = ttime.mktime(ttime.strptime(daystr, fmt))
-        except:
+            break
+        except ValueError:
             res = None
-        if res:
-            return res
-
-
-def fntime(daystr):
-    daystr = daystr.replace('_', ':')
-    datestr = ' '.join(daystr.split(os.sep)[-2:])
-    if '.' in datestr:
-        datestr, rest = datestr.rsplit('.', 1)
-    else:
-        rest = ''
-    timed = ttime.mktime(ttime.strptime(datestr, '%Y-%m-%d %H:%M:%S'))
-    if rest:
-        timed += float('.' + rest)
-    return timed
+    return res
 
 
 def get_day(daystr):
+    "return day from string."
+    day = None
+    month = None
+    yea = None
     try:
         ymdre = re.search(r'(\d+)-(\d+)-(\d+)', daystr)
-        (day, month, yea) = ymdre.groups()
-    except:
+        if ymdre:
+            (day, month, yea) = ymdre.groups()
+    except ValueError:
         try:
             ymre = re.search(r'(\d+)-(\d+)', daystr)
-            (day, month) = ymre.groups()
-            yea = ttime.strftime("%Y", ttime.localtime())
+            if ymre:
+                (day, month) = ymre.groups()
+                yea = ttime.strftime("%Y", ttime.localtime())
         except Exception as ex:
             raise NoDate(daystr) from ex
-    day = int(day)
-    month = int(month)
-    yea = int(yea)
-    date = "%s %s %s" % (day, bdmonths[month], yea)
-    return ttime.mktime(ttime.strptime(date, r"%d %b %Y"))
+    if day:
+        day = int(day)
+        month = int(month)
+        yea = int(yea)
+        date = f"{day} {MONTHS[month]} {yea}"
+        return ttime.mktime(ttime.strptime(date, r"%d %b %Y"))
+    raise NoDate(daystr)
 
 
 def get_hour(daystr):
+    "return hour from string."
     try:
         hmsre = re.search(r'(\d+):(\d+):(\d+)', str(daystr))
         hours = 60 * 60 * (int(hmsre.group(1)))
         hoursmin = hours  + int(hmsre.group(2)) * 60
         hmsres = hoursmin + int(hmsre.group(3))
     except AttributeError:
         pass
@@ -123,117 +108,27 @@
         return 0
     except ValueError:
         return 0
     return hmsres
 
 
 def get_time(txt):
+    "parse full time string."
     try:
         target = get_day(txt)
     except NoDate:
         target = to_day(today())
     hour =  get_hour(txt)
     if hour:
         target += hour
     return target
 
 
-def laps(seconds, short=True):
-    txt = ""
-    nsec = float(seconds)
-    if nsec < 1:
-        return f"{nsec:.2f}s"
-    yea = 365*24*60*60
-    week = 7*24*60*60
-    nday = 24*60*60
-    hour = 60*60
-    minute = 60
-    yeas = int(nsec/yea)
-    nsec -= yeas*yea
-    weeks = int(nsec/week)
-    nsec -= weeks*week
-    nrdays = int(nsec/nday)
-    nsec -= nrdays*nday
-    hours = int(nsec/hour)
-    nsec -= hours*hour
-    minutes = int(nsec/minute)
-    nsec -= int(minute*minutes)
-    sec = int(nsec)
-    if yeas:
-        txt += f"{yeas}y"
-    if weeks:
-        nrdays += weeks * 7
-    if nrdays:
-        txt += f"{nrdays}d"
-    if short and txt:
-        return txt.strip()
-    if hours:
-        txt += f"{hours}h"
-    if minutes:
-        txt += f"{minutes}m"
-    if sec:
-        txt += f"{sec}s"
-    txt = txt.strip()
-    return txt
-
-
-def parse_command(obj, txt=None):
-    args = []
-    obj.args    = obj.args or []
-    obj.cmd     = obj.cmd or ""
-    obj.gets    = obj.gets or Default()
-    obj.hasmods = obj.hasmod or False
-    obj.index   = None
-    obj.mod     = obj.mod or ""
-    obj.opts    = obj.opts or ""
-    obj.result  = obj.reult or []
-    obj.sets    = obj.sets or Default()
-    obj.txt     = txt or obj.txt or ""
-    obj.otxt    = obj.txt
-    _nr = -1
-    for spli in obj.otxt.split():
-        if spli.startswith("-"):
-            try:
-                obj.index = int(spli[1:])
-            except ValueError:
-                obj.opts += spli[1:]
-            continue
-        if "==" in spli:
-            key, value = spli.split("==", maxsplit=1)
-            if key in obj.gets:
-                val = getattr(obj.gets, key)
-                value = val + "," + value
-            setattr(obj.gets, key, value)
-            continue
-        if "=" in spli:
-            key, value = spli.split("=", maxsplit=1)
-            if key == "mod":
-                obj.hasmods = True
-                if obj.mod:
-                    obj.mod += f",{value}"
-                else:
-                    obj.mod = value
-                continue
-            setattr(obj.sets, key, value)
-            continue
-        _nr += 1
-        if _nr == 0:
-            obj.cmd = spli
-            continue
-        args.append(spli)
-    if args:
-        obj.args = args
-        obj.txt  = obj.cmd or ""
-        obj.rest = " ".join(obj.args)
-        obj.txt  = obj.cmd + " " + obj.rest
-    else:
-        obj.txt = obj.cmd or ""
-
-
 def parse_time(txt):
+    "parse time from string."
     seconds = 0
     target = 0
     txt = str(txt)
     for word in txt.split():
         if word.startswith("+"):
             seconds = int(word[1:])
             return ttime.time() + seconds
@@ -247,33 +142,103 @@
             target = to_day(today())
         hour =  get_hour(txt)
         if hour:
             target += hour
     return target
 
 
-def spl(txt):
-    try:
-        res = txt.split(',')
-    except (TypeError, ValueError):
-        res = txt
-    return [x for x in res if x]
-
-
 def to_day(daystr):
+    "parse day from string."
     previous = ""
     line = ""
     daystr = str(daystr)
+    res = None
     for word in daystr.split():
         line = previous + " " + word
         previous = word
         try:
             res = extract_date(line.strip())
+            break
         except ValueError:
             res = None
-        if res:
-            return res
         line = ""
+    return res
 
 
 def today():
+    "return date."
     return str(datetime.datetime.today()).split()[0]
+
+
+"commands"
+
+
+def tmr(event):
+    "add a timer."
+    result = ""
+    if not event.rest:
+        nmr = 0
+        for _fn, obj in find('timer'):
+            lap = float(obj.time) - ttime.time()
+            if lap > 0:
+                event.reply(f'{nmr} {obj.txt} {laps(lap)}')
+                nmr += 1
+        return result
+    seconds = 0
+    line = ""
+    for word in event.args:
+        if word.startswith("+"):
+            try:
+                seconds = int(word[1:])
+            except (ValueError, IndexError):
+                event.reply(f"{seconds} is not an integer")
+                return result
+        else:
+            line += word + " "
+    if seconds:
+        target = ttime.time() + seconds
+    else:
+        try:
+            target = get_day(event.rest)
+        except NoDate:
+            target = to_day(today())
+        hour =  get_hour(event.rest)
+        if hour:
+            target += hour
+    if not target or ttime.time() > target:
+        event.reply("already passed given time.")
+        return result
+    event.time = target
+    diff = target - ttime.time()
+    event.reply("ok " +  laps(diff))
+    event.result = []
+    event.result.append(event.rest)
+    timer = Timer(diff, event.show, thrname=event.cmd)
+    update(timer, event)
+    sync(timer)
+    launch(timer.start)
+    return result
+
+
+"runtime"
+
+
+def init():
+    "start timers."
+    for _fn, obj in find("timer"):
+        if "time" not in obj:
+            continue
+        diff = float(obj.time) - ttime.time()
+        if diff > 0:
+            bot = Broker.first()
+            evt = Event()
+            update(evt, obj)
+            evt.orig = object.__repr__(bot)
+            timer = Timer(diff, evt.show)
+            launch(timer.start)
+
+
+"register"
+
+
+Client.add(tmr)
+Persist.add(Timer)
```

### Comparing `sbn-92/sbn/storage.py` & `sbn-94/sbn/persist.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,168 +1,147 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,R,W0105,E0402
+# pylint: disable=C,R,W0105
 
 
-"directory of objects"
+"persist"
 
 
 import datetime
 import os
 import time
 
 
-from .objects import Default, Object, cdir, fqn, items, read, update, write
-from .parsers import spl
+from .default import Default
+from .object  import Object, fqn, read, search, update, write
+from .workdir import Workdir
 
 
-def __dir__():
-    return (
-        'Storage',
-        'fetch',
-        'find',
-        'fntime',
-        'ident',
-        'last',
-        'search',
-        'sync'
-    )
+class Persist(Object):
 
+    "Persist"
 
-__all__ = __dir__()
-
-
-class Storage(Object):
-
-    classes = {}
-    wd = ""
+    classes = Object()
 
     @staticmethod
     def add(clz):
-        if not clz:
-            return
+        "add class to whitelist."
         name = str(clz).split()[1][1:-2]
-        Storage.classes[name] = clz
+        setattr(Persist.classes, name, clz)
 
     @staticmethod
     def fns(mtc=""):
+        "show list of files."
         dname = ''
-        pth = Storage.store(mtc)
+        pth = Workdir.store(mtc)
         for rootdir, dirs, _files in os.walk(pth, topdown=False):
             if dirs:
                 for dname in sorted(dirs):
                     if dname.count('-') == 2:
                         ddd = os.path.join(rootdir, dname)
                         fls = sorted(os.listdir(ddd))
                         for fll in fls:
-                            yield strip(os.path.join(ddd, fll))
+                            yield Workdir.strip(os.path.join(ddd, fll))
 
     @staticmethod
     def long(name):
+        "match from single name to long name."
         split = name.split(".")[-1].lower()
         res = name
-        for named in Storage.classes:
+        for named in Persist.classes:
             if split in named.split(".")[-1].lower():
                 res = named
                 break
         if "." not in res:
-            for fnm in Storage.types():
+            for fnm in Workdir.types():
                 claz = fnm.split(".")[-1]
                 if fnm == claz.lower():
                     res = fnm
         return res
 
-    @staticmethod
-    def skel():
-        cdir(os.path.join(Storage.wd, "store", ""))
-
-    @staticmethod
-    def store(pth=""):
-        return os.path.join(Storage.wd, "store", pth)
-
-    @staticmethod
-    def types():
-        return os.listdir(Storage.store())
-
-
-def find(mtc, selector=None, index=None, deleted=False):
-    clz = Storage.long(mtc)
-    nr = -1
-    for fnm in sorted(Storage.fns(clz), key=fntime):
-        obj = Default()
-        fetch(obj, fnm)
-        if not deleted and '__deleted__' in obj:
-            continue
-        if selector and not search(obj, selector):
-            continue
-        nr += 1
-        if index is not None and nr != int(index):
-            continue
-        yield (fnm, obj)
-
 
 def fntime(daystr):
+    "convert file name to it's saved time."
     daystr = daystr.replace('_', ':')
     datestr = ' '.join(daystr.split(os.sep)[-2:])
     if '.' in datestr:
         datestr, rest = datestr.rsplit('.', 1)
     else:
         rest = ''
     timed = time.mktime(time.strptime(datestr, '%Y-%m-%d %H:%M:%S'))
     if rest:
         timed += float('.' + rest)
     return timed
 
 
-def strip(pth, nmr=3):
-    return os.sep.join(pth.split(os.sep)[-nmr:])
+def find(mtc, selector=None, index=None, deleted=False):
+    "find object matching the selector dict."
+    clz = Persist.long(mtc)
+    nrs = -1
+    for fnm in sorted(Persist.fns(clz), key=fntime):
+        obj = Default()
+        fetch(obj, fnm)
+        if not deleted and '__deleted__' in obj:
+            continue
+        if selector and not search(obj, selector):
+            continue
+        nrs += 1
+        if index is not None and nrs != int(index):
+            continue
+        yield (fnm, obj)
+
+
+def fetch(obj, pth):
+    "read object from disk."
+    pth2 = Workdir.store(pth)
+    read(obj, pth2)
+    return Workdir.strip(pth)
 
 
 def ident(obj):
+    "return an id for an object."
     return os.path.join(
                         fqn(obj),
                         os.path.join(*str(datetime.datetime.now()).split())
                        )
 
-def fetch(obj, pth):
-    pth2 = Storage.store(pth)
-    read(obj, pth2)
-    return strip(pth)
-
 
 def last(obj, selector=None):
+    "return last object saved."
     if selector is None:
         selector = {}
     result = sorted(
                     find(fqn(obj), selector),
                     key=lambda x: fntime(x[0])
                    )
+    res = None
     if result:
         inp = result[-1]
         update(obj, inp[-1])
-        return inp[0]
-
-
-def search(obj, selector):
-    res = False
-    if not selector:
-        return True
-    for key, value in items(selector):
-        if key not in obj:
-            res = False
-            break
-        for vval in spl(str(value)):
-            val = getattr(obj, key, None)
-            if str(vval).lower() in str(val).lower():
-                res = True
-            else:
-                res = False
-                break
+        res = inp[0]
     return res
 
-
 def sync(obj, pth=None):
+    "sync object to disk."
     if pth is None:
         pth = ident(obj)
-    pth2 = Storage.store(pth)
+    pth2 = Workdir.store(pth)
     write(obj, pth2)
     return pth
+
+
+"interface"
+
+
+def __dir__():
+    return (
+        'Persist',
+        'fetch',
+        'fntime',
+        'find',
+        'last',
+        'ident',
+        'sync',
+    )
+
+
+__all__ = __dir__()
```

### Comparing `sbn-92/sbn/threads.py` & `sbn-94/sbn/thread.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,28 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,R,W0718,E0402
+# pylint: disable=C,R,W0105,W0718
 
 
-"threads"
+"thread"
 
 
 import queue
 import threading
 import time
 import types
 
 
-from .excepts import Error
-from .objects import Object
-
-
-def __dir__():
-    return (
-       'Repeater',
-       'Thread',
-       'Timer',
-       'launch',
-       'name',
-    )
-
-
-__all__ = __dir__()
+from .errors import Errors
 
 
 class Thread(threading.Thread):
 
+    "Thread"
+
     def __init__(self, func, thrname, *args, daemon=True, **kwargs):
         super().__init__(None, self.run, thrname, (), {}, daemon=daemon)
         self._result   = None
         self.name      = thrname or name(func)
         self.queue     = queue.Queue()
         self.sleep     = None
         self.starttime = time.time()
@@ -43,81 +31,59 @@
     def __iter__(self):
         return self
 
     def __next__(self):
         for k in dir(self):
             yield k
 
-    def join(self, timeout=None):
+    def join(self, timeout=1.0):
+        "join this thread."
         super().join(timeout)
         return self._result
 
     def run(self):
+        "run this thread's payload."
         func, args = self.queue.get()
         try:
             self._result = func(*args)
-        except Exception as exc:
-            Error.add(exc)
-            if args and "ready" in dir(args[0]):
+        except Exception as ex:
+            Errors.add(ex)
+            if args and "Event" in str(type(args[0])):
                 args[0].ready()
 
 
-class Timer(Object):
-
-    def __init__(self, sleep, func, *args, thrname=None):
-        Object.__init__(self)
-        self.args  = args
-        self.func  = func
-        self.sleep = sleep
-        self.name  = thrname or str(self.func).split()[2]
-        self.state = {}
-        self.timer = None
-
-    def run(self):
-        self.state["latest"] = time.time()
-        launch(self.func, *self.args)
-
-    def start(self):
-        timer = threading.Timer(self.sleep, self.run)
-        timer.name   = self.name
-        timer.daemon = True
-        timer.sleep  = self.sleep
-        timer.state  = self.state
-        timer.func   = self.func
-        timer.state["starttime"] = time.time()
-        timer.state["latest"]    = time.time()
-        timer.start()
-        self.timer   = timer
-
-    def stop(self):
-        if self.timer:
-            self.timer.cancel()
-
-
-class Repeater(Timer):
-
-    def run(self):
-        thr = launch(self.start)
-        super().run()
-        return thr
-
-
 def launch(func, *args, **kwargs):
+    "launch a thread."
     nme = kwargs.get("name", name(func))
     thread = Thread(func, nme, *args, **kwargs)
     thread.start()
     return thread
 
 
 def name(obj):
+    "return a full qualified name of an object/function/module."
     typ = type(obj)
     if isinstance(typ, types.ModuleType):
         return obj.__name__
     if '__self__' in dir(obj):
         return f'{obj.__self__.__class__.__name__}.{obj.__name__}'
     if '__class__' in dir(obj) and '__name__' in dir(obj):
         return f'{obj.__class__.__name__}.{obj.__name__}'
     if '__class__' in dir(obj):
         return f"{obj.__class__.__module__}.{obj.__class__.__name__}"
     if '__name__' in dir(obj):
         return f'{obj.__class__.__name__}.{obj.__name__}'
     return None
+
+
+"interface"
+
+
+def __dir__():
+    return (
+        'Thread',
+        'launch',
+        'name'
+    )
+
+
+__all__ = __dir__()
```

### Comparing `sbn-92/sbn.egg-info/SOURCES.txt` & `sbn-94/sbn.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+MANUAL.rst
 README.rst
 pyproject.toml
 setup.py
 docs/ECHAabilify.png
 docs/ECHAclozapine.png
 docs/ECHAhaldol.png
 docs/ECHAzyprexa.png
@@ -35,46 +36,47 @@
 docs/pdf/EM_T04_OTP-CR-117_19.pdf
 docs/pdf/EM_T07_OTP-CR-117_19_001.pdf
 docs/pdf/Kamer.pdf
 docs/pdf/Rome-Statute.pdf
 docs/pdf/bevestigd.pdf
 sbn/__init__.py
 sbn/__main__.py
-sbn/brokers.py
-sbn/clients.py
-sbn/command.py
-sbn/excepts.py
+sbn/broker.py
+sbn/client.py
+sbn/default.py
+sbn/errors.py
+sbn/event.py
 sbn/handler.py
-sbn/objects.py
-sbn/parsers.py
-sbn/storage.py
-sbn/threads.py
+sbn/interface.py
+sbn/object.py
+sbn/parser.py
+sbn/persist.py
+sbn/repeater.py
+sbn/thread.py
+sbn/timer.py
+sbn/utils.py
+sbn/workdir.py
 sbn.egg-info/PKG-INFO
 sbn.egg-info/SOURCES.txt
 sbn.egg-info/dependency_links.txt
 sbn.egg-info/entry_points.txt
 sbn.egg-info/requires.txt
 sbn.egg-info/top_level.txt
 sbn.egg-info/zip-safe
 sbn/modules/__init__.py
 sbn/modules/cmd.py
+sbn/modules/dbg.py
 sbn/modules/err.py
 sbn/modules/flt.py
 sbn/modules/fnd.py
 sbn/modules/irc.py
 sbn/modules/log.py
-sbn/modules/man.py
 sbn/modules/mbx.py
 sbn/modules/mdl.py
 sbn/modules/mod.py
-sbn/modules/mre.py
-sbn/modules/pwd.py
 sbn/modules/req.py
-sbn/modules/rme.py
 sbn/modules/rss.py
 sbn/modules/rst.py
-sbn/modules/slg.py
 sbn/modules/tdo.py
 sbn/modules/thr.py
 sbn/modules/tmr.py
-sbn/modules/udp.py
-sbn/modules/wsd.py
+sbn/modules/udp.py
```

