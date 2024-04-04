# Comparing `tmp/not1mm-24.4.2.1.tar.gz` & `tmp/not1mm-24.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "not1mm-24.4.2.1.tar", last modified: Wed Apr  3 04:02:05 2024, max compression
+gzip compressed data, was "not1mm-24.4.4.tar", last modified: Thu Apr  4 21:12:48 2024, max compression
```

## Comparing `not1mm-24.4.2.1.tar` & `not1mm-24.4.4.tar`

### file list

```diff
@@ -1,158 +1,158 @@
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-04-03 04:02:05.797761 not1mm-24.4.2.1/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/LICENSE
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    26568 2024-04-03 04:02:05.796761 not1mm-24.4.2.1/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    25495 2024-04-03 03:45:43.000000 not1mm-24.4.2.1/README.md
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-04-03 04:02:05.653759 not1mm-24.4.2.1/not1mm/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   119800 2024-04-03 03:28:39.000000 not1mm-24.4.2.1/not1mm/__main__.py
--rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    34318 2024-04-03 01:43:15.000000 not1mm-24.4.2.1/not1mm/bandmap.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10465 2024-04-03 03:04:54.000000 not1mm-24.4.2.1/not1mm/checkwindow.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-04-03 04:02:05.690759 not1mm-24.4.2.1/not1mm/data/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/JetBrainsMono-Regular.ttf
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   366478 2024-04-02 17:57:36.000000 not1mm-24.4.2.1/not1mm/data/MASTER.SCP
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2067 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/about.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      224 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/alpha bravo charlie delta.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     7125 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/bandmap.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      387 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/check.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4614 2024-04-02 19:15:08.000000 not1mm-24.4.2.1/not1mm/data/checkwindow.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51643 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/configuration.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    89307 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/contests.sql
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)  4790698 2024-04-02 16:11:52.000000 not1mm-24.4.2.1/not1mm/data/cty.json
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      451 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/cwmacros.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      116 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/donors.html
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    27404 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/editcontact.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2689 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/editmacro.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      474 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/greendot.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      205 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/k6gte-not1mm.desktop
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     6076 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/k6gte.not1mm-128.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1526 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/k6gte.not1mm-32.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2925 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/k6gte.not1mm-64.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1436 2024-04-01 23:54:49.000000 not1mm-24.4.2.1/not1mm/data/logwindow.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1610 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/logwindowx.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    54070 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/main.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    21823 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/new_contest.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    23273 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/not1mm.html
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2247 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/opon.ui
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-04-03 04:02:05.754760 not1mm-24.4.2.1/not1mm/data/phonetics/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42590 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/phonetics/0.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    30248 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/phonetics/1.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    29584 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/phonetics/2.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32072 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/phonetics/3.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43052 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/phonetics/4.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51976 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/phonetics/5.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58634 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/phonetics/6.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49154 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/phonetics/7.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32842 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/phonetics/73.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35636 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/phonetics/8.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    39592 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/phonetics/9.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46800 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/phonetics/a.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    44594 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/phonetics/again.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    40976 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/phonetics/b.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46746 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/phonetics/c.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    62558 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/phonetics/contest.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    92498 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/phonetics/cq.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52524 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/phonetics/d.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    45700 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/phonetics/e.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    53438 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/phonetics/f.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42766 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/phonetics/g.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50040 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/phonetics/h.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46372 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/phonetics/i.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43434 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/phonetics/j.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49066 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/phonetics/k.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   185562 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/phonetics/k6gte.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43154 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/phonetics/l.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    54352 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/phonetics/m.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56798 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/phonetics/mynumber.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52204 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/phonetics/n.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   154544 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/phonetics/nil.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47440 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/phonetics/o.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    38300 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/phonetics/p.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    55288 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/phonetics/q.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47432 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/phonetics/r.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46122 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/phonetics/roger.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    60698 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/phonetics/s.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    70424 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/phonetics/space.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58196 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/phonetics/t.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56320 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/phonetics/thankyou.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    94980 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/phonetics/thankyouqrz.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    65922 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/phonetics/u.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50142 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/phonetics/v.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    37638 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/phonetics/w.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    61870 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/phonetics/x.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56524 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/phonetics/y.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46510 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/phonetics/yourcall.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51768 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/phonetics/z.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1600 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/pickcontest.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1234 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/radio_green.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1258 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/radio_grey.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      957 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/radio_red.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      565 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/reddot.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    40028 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/settings.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      470 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/data/ssbmacros.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1986 2024-04-03 01:54:51.000000 not1mm-24.4.2.1/not1mm/data/vfo.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1652 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/fsutils.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-04-03 04:02:05.773760 not1mm-24.4.2.1/not1mm/lib/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/lib/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      416 2024-04-02 16:43:54.000000 not1mm-24.4.2.1/not1mm/lib/about.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15127 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/lib/cat_interface.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3126 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/lib/cwinterface.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42480 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/lib/database.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      353 2024-04-02 16:43:38.000000 not1mm-24.4.2.1/not1mm/lib/edit_contact.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      517 2024-04-02 16:43:30.000000 not1mm-24.4.2.1/not1mm/lib/edit_macro.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      359 2024-04-02 16:43:21.000000 not1mm-24.4.2.1/not1mm/lib/edit_opon.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1965 2024-04-02 16:43:09.000000 not1mm-24.4.2.1/not1mm/lib/edit_station.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10978 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/lib/ham_utility.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13952 2024-04-03 03:28:34.000000 not1mm-24.4.2.1/not1mm/lib/lookup.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3249 2024-04-02 17:02:22.000000 not1mm-24.4.2.1/not1mm/lib/multicast.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5712 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/lib/n1mm.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      350 2024-04-02 16:42:23.000000 not1mm-24.4.2.1/not1mm/lib/new_contest.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     8605 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/lib/plugin_common.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      359 2024-04-02 16:41:42.000000 not1mm-24.4.2.1/not1mm/lib/select_contest.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     8877 2024-04-02 16:41:49.000000 not1mm-24.4.2.1/not1mm/lib/settings.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2334 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/lib/super_check_partial.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       49 2024-04-03 03:41:42.000000 not1mm-24.4.2.1/not1mm/lib/version.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1286 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/lib/versiontest.py
--rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    44900 2024-04-03 01:43:18.000000 not1mm-24.4.2.1/not1mm/logwindow.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-04-03 04:02:05.795760 not1mm-24.4.2.1/not1mm/plugins/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10834 2024-04-02 16:04:28.000000 not1mm-24.4.2.1/not1mm/plugins/10_10_fall_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10839 2024-04-02 16:04:01.000000 not1mm-24.4.2.1/not1mm/plugins/10_10_spring_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10848 2024-04-02 16:06:56.000000 not1mm-24.4.2.1/not1mm/plugins/10_10_summer_phone.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10851 2024-04-02 16:06:46.000000 not1mm-24.4.2.1/not1mm/plugins/10_10_winter_phone.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2024-03-31 16:17:00.000000 not1mm-24.4.2.1/not1mm/plugins/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13643 2024-04-02 16:06:37.000000 not1mm-24.4.2.1/not1mm/plugins/arrl_10m.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13688 2024-04-02 16:06:29.000000 not1mm-24.4.2.1/not1mm/plugins/arrl_dx_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13691 2024-04-02 16:06:19.000000 not1mm-24.4.2.1/not1mm/plugins/arrl_dx_ssb.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10026 2024-04-02 03:37:09.000000 not1mm-24.4.2.1/not1mm/plugins/arrl_field_day.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     7974 2024-04-02 16:06:03.000000 not1mm-24.4.2.1/not1mm/plugins/arrl_rtty_ru.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13141 2024-04-02 17:50:55.000000 not1mm-24.4.2.1/not1mm/plugins/arrl_ss_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13147 2024-04-02 17:50:42.000000 not1mm-24.4.2.1/not1mm/plugins/arrl_ss_phone.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12438 2024-04-02 16:05:30.000000 not1mm-24.4.2.1/not1mm/plugins/arrl_vhf_jan.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11457 2024-04-02 16:05:17.000000 not1mm-24.4.2.1/not1mm/plugins/arrl_vhf_jun.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11457 2024-04-02 16:05:08.000000 not1mm-24.4.2.1/not1mm/plugins/arrl_vhf_sep.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11869 2024-04-02 16:08:42.000000 not1mm-24.4.2.1/not1mm/plugins/canada_day.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14018 2024-04-02 16:08:29.000000 not1mm-24.4.2.1/not1mm/plugins/cq_160_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14061 2024-04-02 16:08:22.000000 not1mm-24.4.2.1/not1mm/plugins/cq_160_ssb.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12378 2024-04-02 16:08:13.000000 not1mm-24.4.2.1/not1mm/plugins/cq_wpx_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12466 2024-04-02 16:08:05.000000 not1mm-24.4.2.1/not1mm/plugins/cq_wpx_ssb.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11083 2024-04-02 16:07:53.000000 not1mm-24.4.2.1/not1mm/plugins/cq_ww_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11088 2024-04-02 16:07:44.000000 not1mm-24.4.2.1/not1mm/plugins/cq_ww_ssb.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11976 2024-04-02 16:07:34.000000 not1mm-24.4.2.1/not1mm/plugins/cwt.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3369 2024-04-02 16:10:31.000000 not1mm-24.4.2.1/not1mm/plugins/general_logging.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11433 2024-04-02 16:10:23.000000 not1mm-24.4.2.1/not1mm/plugins/iaru_hf.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11049 2024-04-02 16:10:11.000000 not1mm-24.4.2.1/not1mm/plugins/jidx_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11051 2024-04-02 16:10:00.000000 not1mm-24.4.2.1/not1mm/plugins/jidx_ph.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11472 2024-04-02 16:09:51.000000 not1mm-24.4.2.1/not1mm/plugins/naqp_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11477 2024-04-02 16:09:43.000000 not1mm-24.4.2.1/not1mm/plugins/naqp_ssb.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12278 2024-04-02 16:09:34.000000 not1mm-24.4.2.1/not1mm/plugins/phone_weekly_test.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10546 2024-04-02 16:09:20.000000 not1mm-24.4.2.1/not1mm/plugins/stew_perry_topband.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10212 2024-04-02 16:09:08.000000 not1mm-24.4.2.1/not1mm/plugins/winter_field_day.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12430 2024-04-03 03:06:08.000000 not1mm-24.4.2.1/not1mm/vfo.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-04-03 04:02:05.795760 not1mm-24.4.2.1/not1mm.egg-info/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    26568 2024-04-03 04:02:05.000000 not1mm-24.4.2.1/not1mm.egg-info/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4079 2024-04-03 04:02:05.000000 not1mm-24.4.2.1/not1mm.egg-info/SOURCES.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2024-04-03 04:02:05.000000 not1mm-24.4.2.1/not1mm.egg-info/dependency_links.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       47 2024-04-03 04:02:05.000000 not1mm-24.4.2.1/not1mm.egg-info/entry_points.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      131 2024-04-03 04:02:05.000000 not1mm-24.4.2.1/not1mm.egg-info/requires.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       25 2024-04-03 04:02:05.000000 not1mm-24.4.2.1/not1mm.egg-info/top_level.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1427 2024-04-03 03:43:07.000000 not1mm-24.4.2.1/pyproject.toml
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2024-04-03 04:02:05.797761 not1mm-24.4.2.1/setup.cfg
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-04-04 21:12:48.932111 not1mm-24.4.4/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2024-03-31 16:17:00.000000 not1mm-24.4.4/LICENSE
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    26633 2024-04-04 21:12:48.932111 not1mm-24.4.4/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    25562 2024-04-04 20:04:08.000000 not1mm-24.4.4/README.md
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-04-04 21:12:48.811109 not1mm-24.4.4/not1mm/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   119858 2024-04-04 21:11:03.000000 not1mm-24.4.4/not1mm/__main__.py
+-rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    34318 2024-04-03 01:43:15.000000 not1mm-24.4.4/not1mm/bandmap.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10465 2024-04-03 03:04:54.000000 not1mm-24.4.4/not1mm/checkwindow.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-04-04 21:12:48.836110 not1mm-24.4.4/not1mm/data/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/JetBrainsMono-Regular.ttf
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   366478 2024-04-02 17:57:36.000000 not1mm-24.4.4/not1mm/data/MASTER.SCP
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2067 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/about.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      224 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/alpha bravo charlie delta.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     7125 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/bandmap.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      387 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/check.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4614 2024-04-02 19:15:08.000000 not1mm-24.4.4/not1mm/data/checkwindow.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51643 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/configuration.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    89307 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/contests.sql
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)  4790698 2024-04-02 16:11:52.000000 not1mm-24.4.4/not1mm/data/cty.json
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      451 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/cwmacros.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      116 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/donors.html
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    27404 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/editcontact.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2689 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/editmacro.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      474 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/greendot.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      205 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/k6gte-not1mm.desktop
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     6076 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/k6gte.not1mm-128.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1526 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/k6gte.not1mm-32.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2925 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/k6gte.not1mm-64.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1436 2024-04-01 23:54:49.000000 not1mm-24.4.4/not1mm/data/logwindow.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1610 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/logwindowx.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    54070 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/main.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    21823 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/new_contest.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    23273 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/not1mm.html
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2247 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/opon.ui
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-04-04 21:12:48.902110 not1mm-24.4.4/not1mm/data/phonetics/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42590 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/phonetics/0.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    30248 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/phonetics/1.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    29584 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/phonetics/2.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32072 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/phonetics/3.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43052 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/phonetics/4.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51976 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/phonetics/5.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58634 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/phonetics/6.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49154 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/phonetics/7.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32842 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/phonetics/73.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35636 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/phonetics/8.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    39592 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/phonetics/9.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46800 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/phonetics/a.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    44594 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/phonetics/again.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    40976 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/phonetics/b.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46746 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/phonetics/c.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    62558 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/phonetics/contest.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    92498 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/phonetics/cq.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52524 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/phonetics/d.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    45700 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/phonetics/e.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    53438 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/phonetics/f.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42766 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/phonetics/g.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50040 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/phonetics/h.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46372 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/phonetics/i.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43434 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/phonetics/j.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49066 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/phonetics/k.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   185562 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/phonetics/k6gte.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43154 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/phonetics/l.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    54352 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/phonetics/m.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56798 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/phonetics/mynumber.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52204 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/phonetics/n.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   154544 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/phonetics/nil.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47440 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/phonetics/o.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    38300 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/phonetics/p.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    55288 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/phonetics/q.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47432 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/phonetics/r.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46122 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/phonetics/roger.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    60698 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/phonetics/s.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    70424 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/phonetics/space.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58196 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/phonetics/t.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56320 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/phonetics/thankyou.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    94980 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/phonetics/thankyouqrz.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    65922 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/phonetics/u.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50142 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/phonetics/v.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    37638 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/phonetics/w.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    61870 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/phonetics/x.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56524 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/phonetics/y.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46510 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/phonetics/yourcall.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51768 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/phonetics/z.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1600 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/pickcontest.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1234 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/radio_green.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1258 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/radio_grey.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      957 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/radio_red.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      565 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/reddot.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    40028 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/settings.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      470 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/data/ssbmacros.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1986 2024-04-03 01:54:51.000000 not1mm-24.4.4/not1mm/data/vfo.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1652 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/fsutils.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-04-04 21:12:48.914111 not1mm-24.4.4/not1mm/lib/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/lib/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      416 2024-04-02 16:43:54.000000 not1mm-24.4.4/not1mm/lib/about.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15127 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/lib/cat_interface.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3126 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/lib/cwinterface.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42480 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/lib/database.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      353 2024-04-02 16:43:38.000000 not1mm-24.4.4/not1mm/lib/edit_contact.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      517 2024-04-02 16:43:30.000000 not1mm-24.4.4/not1mm/lib/edit_macro.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      359 2024-04-02 16:43:21.000000 not1mm-24.4.4/not1mm/lib/edit_opon.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1965 2024-04-02 16:43:09.000000 not1mm-24.4.4/not1mm/lib/edit_station.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10978 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/lib/ham_utility.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13952 2024-04-03 03:28:34.000000 not1mm-24.4.4/not1mm/lib/lookup.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3249 2024-04-02 17:02:22.000000 not1mm-24.4.4/not1mm/lib/multicast.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5712 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/lib/n1mm.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      816 2024-04-04 17:56:24.000000 not1mm-24.4.4/not1mm/lib/new_contest.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     8605 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/lib/plugin_common.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      359 2024-04-02 16:41:42.000000 not1mm-24.4.4/not1mm/lib/select_contest.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     8877 2024-04-02 16:41:49.000000 not1mm-24.4.4/not1mm/lib/settings.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2334 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/lib/super_check_partial.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       47 2024-04-04 20:02:17.000000 not1mm-24.4.4/not1mm/lib/version.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1286 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/lib/versiontest.py
+-rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    44900 2024-04-03 20:01:58.000000 not1mm-24.4.4/not1mm/logwindow.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-04-04 21:12:48.929111 not1mm-24.4.4/not1mm/plugins/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10873 2024-04-04 18:50:36.000000 not1mm-24.4.4/not1mm/plugins/10_10_fall_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10878 2024-04-04 18:58:51.000000 not1mm-24.4.4/not1mm/plugins/10_10_spring_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10887 2024-04-04 18:58:54.000000 not1mm-24.4.4/not1mm/plugins/10_10_summer_phone.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10890 2024-04-04 18:58:56.000000 not1mm-24.4.4/not1mm/plugins/10_10_winter_phone.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2024-03-31 16:17:00.000000 not1mm-24.4.4/not1mm/plugins/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13677 2024-04-04 19:07:30.000000 not1mm-24.4.4/not1mm/plugins/arrl_10m.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13722 2024-04-04 19:09:51.000000 not1mm-24.4.4/not1mm/plugins/arrl_dx_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13725 2024-04-04 19:10:06.000000 not1mm-24.4.4/not1mm/plugins/arrl_dx_ssb.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10052 2024-04-04 18:11:53.000000 not1mm-24.4.4/not1mm/plugins/arrl_field_day.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     7994 2024-04-04 19:10:45.000000 not1mm-24.4.4/not1mm/plugins/arrl_rtty_ru.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12989 2024-04-04 20:51:30.000000 not1mm-24.4.4/not1mm/plugins/arrl_ss_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12977 2024-04-04 20:53:34.000000 not1mm-24.4.4/not1mm/plugins/arrl_ss_phone.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12481 2024-04-04 19:17:41.000000 not1mm-24.4.4/not1mm/plugins/arrl_vhf_jan.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11500 2024-04-04 19:18:17.000000 not1mm-24.4.4/not1mm/plugins/arrl_vhf_jun.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11500 2024-04-04 19:18:29.000000 not1mm-24.4.4/not1mm/plugins/arrl_vhf_sep.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11907 2024-04-04 19:23:16.000000 not1mm-24.4.4/not1mm/plugins/canada_day.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14059 2024-04-04 19:27:40.000000 not1mm-24.4.4/not1mm/plugins/cq_160_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14102 2024-04-04 19:27:52.000000 not1mm-24.4.4/not1mm/plugins/cq_160_ssb.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12399 2024-04-04 19:29:11.000000 not1mm-24.4.4/not1mm/plugins/cq_wpx_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12487 2024-04-04 19:29:08.000000 not1mm-24.4.4/not1mm/plugins/cq_wpx_ssb.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11114 2024-04-04 19:31:31.000000 not1mm-24.4.4/not1mm/plugins/cq_ww_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11119 2024-04-04 19:31:27.000000 not1mm-24.4.4/not1mm/plugins/cq_ww_ssb.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12020 2024-04-04 19:46:16.000000 not1mm-24.4.4/not1mm/plugins/cwt.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3387 2024-04-04 17:53:54.000000 not1mm-24.4.4/not1mm/plugins/general_logging.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11461 2024-04-04 19:46:13.000000 not1mm-24.4.4/not1mm/plugins/iaru_hf.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11090 2024-04-04 19:47:46.000000 not1mm-24.4.4/not1mm/plugins/jidx_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11092 2024-04-04 19:47:59.000000 not1mm-24.4.4/not1mm/plugins/jidx_ph.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11510 2024-04-04 19:50:33.000000 not1mm-24.4.4/not1mm/plugins/naqp_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11515 2024-04-04 19:50:44.000000 not1mm-24.4.4/not1mm/plugins/naqp_ssb.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12316 2024-04-04 19:51:26.000000 not1mm-24.4.4/not1mm/plugins/phone_weekly_test.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10588 2024-04-04 19:52:18.000000 not1mm-24.4.4/not1mm/plugins/stew_perry_topband.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10238 2024-04-04 18:05:44.000000 not1mm-24.4.4/not1mm/plugins/winter_field_day.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12467 2024-04-03 15:03:49.000000 not1mm-24.4.4/not1mm/vfo.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-04-04 21:12:48.930111 not1mm-24.4.4/not1mm.egg-info/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    26633 2024-04-04 21:12:48.000000 not1mm-24.4.4/not1mm.egg-info/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4079 2024-04-04 21:12:48.000000 not1mm-24.4.4/not1mm.egg-info/SOURCES.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2024-04-04 21:12:48.000000 not1mm-24.4.4/not1mm.egg-info/dependency_links.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       47 2024-04-04 21:12:48.000000 not1mm-24.4.4/not1mm.egg-info/entry_points.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      131 2024-04-04 21:12:48.000000 not1mm-24.4.4/not1mm.egg-info/requires.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       25 2024-04-04 21:12:48.000000 not1mm-24.4.4/not1mm.egg-info/top_level.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1425 2024-04-04 20:02:17.000000 not1mm-24.4.4/pyproject.toml
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2024-04-04 21:12:48.932111 not1mm-24.4.4/setup.cfg
```

### Comparing `not1mm-24.4.2.1/LICENSE` & `not1mm-24.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/PKG-INFO` & `not1mm-24.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: not1mm
-Version: 24.4.2.1
+Version: 24.4.4
 Summary: NOT1MM Logger
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/not1mm
 Project-URL: Bug Tracker, https://github.com/mbridak/not1mm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -173,14 +173,15 @@
 - Phone Weekly Test
 - RAC Canada Day
 - Stew Perry Topband
 - Winter Field Day
 
 ## Recent Changes
 
+- [24-4-4] Added per-contest echange hint when adding new contest.
 - [24-4-2] Migrated to PyQt6. I'm sure there are broken things.
 - [24-4-1-2] Added color text indicators to the Check Partial window. Poached the code from @kyleboyle. Thanks! Fixed the Log, VFO and Check Partial windows to be actual docking widgets. Refocus call field after double clicking on item in the check partial window.
 - [24-4-1] Removed some un-needed loops and widgets from the check window. Fixed docking to the left side.
 
 See [CHANGELOG.md](CHANGELOG.md) for prior changes.
 
 ## Flatpak
```

### Comparing `not1mm-24.4.2.1/README.md` & `not1mm-24.4.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -141,14 +141,15 @@
 - Phone Weekly Test
 - RAC Canada Day
 - Stew Perry Topband
 - Winter Field Day
 
 ## Recent Changes
 
+- [24-4-4] Added per-contest echange hint when adding new contest.
 - [24-4-2] Migrated to PyQt6. I'm sure there are broken things.
 - [24-4-1-2] Added color text indicators to the Check Partial window. Poached the code from @kyleboyle. Thanks! Fixed the Log, VFO and Check Partial windows to be actual docking widgets. Refocus call field after double clicking on item in the check partial window.
 - [24-4-1] Removed some un-needed loops and widgets from the check window. Fixed docking to the left side.
 
 See [CHANGELOG.md](CHANGELOG.md) for prior changes.
 
 ## Flatpak
```

### Comparing `not1mm-24.4.2.1/not1mm/__main__.py` & `not1mm-24.4.4/not1mm/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7055,434 +7055,438 @@
 0001b8e0: 6f5f 6669 6c65 0a20 2020 2020 2020 2020  o_file.         
 0001b8f0: 2020 2029 0a20 2020 2020 2020 2074 7279     ).        try
 0001b900: 3a0a 2020 2020 2020 2020 2020 2020 6673  :.            fs
 0001b910: 7574 696c 732e 6f70 656e 4669 6c65 5769  utils.openFileWi
 0001b920: 7468 4f53 2866 7375 7469 6c73 2e55 5345  thOS(fsutils.USE
 0001b930: 525f 4441 5441 5f50 4154 4820 2f20 6d61  R_DATA_PATH / ma
 0001b940: 6372 6f5f 6669 6c65 290a 2020 2020 2020  cro_file).      
-0001b950: 2020 6578 6365 7074 3a0a 2020 2020 2020    except:.      
-0001b960: 2020 2020 2020 6c6f 6767 6572 2e65 7863        logger.exc
-0001b970: 6570 7469 6f6e 280a 2020 2020 2020 2020  eption(.        
-0001b980: 2020 2020 2020 2020 6622 436f 756c 6420          f"Could 
-0001b990: 6e6f 7420 6f70 656e 2066 696c 6520 7b66  not open file {f
-0001b9a0: 7375 7469 6c73 2e55 5345 525f 4441 5441  sutils.USER_DATA
-0001b9b0: 5f50 4154 4820 2f20 6d61 6372 6f5f 6669  _PATH / macro_fi
-0001b9c0: 6c65 7d22 0a20 2020 2020 2020 2020 2020  le}".           
-0001b9d0: 2029 0a0a 2020 2020 6465 6620 7265 6164   )..    def read
-0001b9e0: 5f63 775f 6d61 6372 6f73 2873 656c 6629  _cw_macros(self)
-0001b9f0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-0001ba00: 2020 2222 220a 2020 2020 2020 2020 5265    """.        Re
-0001ba10: 6164 7320 696e 2074 6865 2043 5720 6d61  ads in the CW ma
-0001ba20: 6372 6f73 2c20 6669 7273 7473 2069 7420  cros, firsts it 
-0001ba30: 6368 6563 6b73 2074 6f20 7365 6520 6966  checks to see if
-0001ba40: 2074 6865 2066 696c 6520 6578 6973 7473   the file exists
-0001ba50: 2e20 4966 2069 7420 646f 6573 206e 6f74  . If it does not
-0001ba60: 2c0a 2020 2020 2020 2020 616e 6420 7468  ,.        and th
-0001ba70: 6973 2068 6173 2062 6565 6e20 7061 636b  is has been pack
-0001ba80: 6167 6564 2077 6974 6820 7079 696e 7374  aged with pyinst
-0001ba90: 616c 6c65 7220 6974 2077 696c 6c20 636f  aller it will co
-0001baa0: 7079 2074 6865 2064 6566 6175 6c74 2066  py the default f
-0001bab0: 696c 6520 6672 6f6d 2074 6865 0a20 2020  ile from the.   
-0001bac0: 2020 2020 2074 656d 7020 6469 7265 6374       temp direct
-0001bad0: 6f72 7920 7468 6973 2069 7320 7275 6e6e  ory this is runn
-0001bae0: 696e 6720 6672 6f6d 2e2e 2e20 496e 2074  ing from... In t
-0001baf0: 6865 6f72 792e 0a20 2020 2020 2020 2022  heory..        "
-0001bb00: 2222 0a0a 2020 2020 2020 2020 6966 2073  ""..        if s
-0001bb10: 656c 662e 7261 6469 6f5f 7374 6174 652e  elf.radio_state.
-0001bb20: 6765 7428 226d 6f64 6522 2920 3d3d 2022  get("mode") == "
-0001bb30: 4357 223a 0a20 2020 2020 2020 2020 2020  CW":.           
-0001bb40: 206d 6163 726f 5f66 696c 6520 3d20 2263   macro_file = "c
-0001bb50: 776d 6163 726f 732e 7478 7422 0a20 2020  wmacros.txt".   
-0001bb60: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0001bb70: 2020 2020 2020 206d 6163 726f 5f66 696c         macro_fil
-0001bb80: 6520 3d20 2273 7362 6d61 6372 6f73 2e74  e = "ssbmacros.t
-0001bb90: 7874 220a 0a20 2020 2020 2020 2069 6620  xt"..        if 
-0001bba0: 6e6f 7420 2866 7375 7469 6c73 2e55 5345  not (fsutils.USE
-0001bbb0: 525f 4441 5441 5f50 4154 4820 2f20 6d61  R_DATA_PATH / ma
-0001bbc0: 6372 6f5f 6669 6c65 292e 6578 6973 7473  cro_file).exists
-0001bbd0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-0001bbe0: 6c6f 6767 6572 2e64 6562 7567 2822 7265  logger.debug("re
-0001bbf0: 6164 5f63 775f 6d61 6372 6f73 3a20 636f  ad_cw_macros: co
-0001bc00: 7079 696e 6720 6465 6661 756c 7420 6d61  pying default ma
-0001bc10: 6372 6f20 6669 6c65 2e22 290a 2020 2020  cro file.").    
-0001bc20: 2020 2020 2020 2020 636f 7079 6669 6c65          copyfile
-0001bc30: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0001bc40: 2020 6673 7574 696c 732e 4150 505f 4441    fsutils.APP_DA
-0001bc50: 5441 5f50 4154 4820 2f20 6d61 6372 6f5f  TA_PATH / macro_
-0001bc60: 6669 6c65 2c20 6673 7574 696c 732e 5553  file, fsutils.US
-0001bc70: 4552 5f44 4154 415f 5041 5448 202f 206d  ER_DATA_PATH / m
-0001bc80: 6163 726f 5f66 696c 650a 2020 2020 2020  acro_file.      
-0001bc90: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-0001bca0: 7769 7468 206f 7065 6e28 0a20 2020 2020  with open(.     
-0001bcb0: 2020 2020 2020 2066 7375 7469 6c73 2e55         fsutils.U
-0001bcc0: 5345 525f 4441 5441 5f50 4154 4820 2f20  SER_DATA_PATH / 
-0001bcd0: 6d61 6372 6f5f 6669 6c65 2c20 2272 222c  macro_file, "r",
-0001bce0: 2065 6e63 6f64 696e 673d 2275 7466 2d38   encoding="utf-8
-0001bcf0: 220a 2020 2020 2020 2020 2920 6173 2066  ".        ) as f
-0001bd00: 696c 655f 6465 7363 7269 7074 6f72 3a0a  ile_descriptor:.
-0001bd10: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0001bd20: 6c69 6e65 2069 6e20 6669 6c65 5f64 6573  line in file_des
-0001bd30: 6372 6970 746f 723a 0a20 2020 2020 2020  criptor:.       
-0001bd40: 2020 2020 2020 2020 2074 7279 3a0a 2020           try:.  
-0001bd50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bd60: 2020 6d6f 6465 2c20 666b 6579 2c20 6275    mode, fkey, bu
-0001bd70: 7474 6f6e 6e61 6d65 2c20 6377 7465 7874  ttonname, cwtext
-0001bd80: 203d 206c 696e 652e 7370 6c69 7428 227c   = line.split("|
-0001bd90: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-0001bda0: 2020 2020 2020 2069 6620 6d6f 6465 2e73         if mode.s
-0001bdb0: 7472 6970 2829 2e75 7070 6572 2829 203d  trip().upper() =
-0001bdc0: 3d20 2252 2220 616e 6420 7365 6c66 2e70  = "R" and self.p
-0001bdd0: 7265 662e 6765 7428 2272 756e 5f73 7461  ref.get("run_sta
-0001bde0: 7465 2229 3a0a 2020 2020 2020 2020 2020  te"):.          
-0001bdf0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0001be00: 6c66 2e66 6b65 7973 5b66 6b65 792e 7374  lf.fkeys[fkey.st
-0001be10: 7269 7028 295d 203d 2028 6275 7474 6f6e  rip()] = (button
-0001be20: 6e61 6d65 2e73 7472 6970 2829 2c20 6377  name.strip(), cw
-0001be30: 7465 7874 2e73 7472 6970 2829 290a 2020  text.strip()).  
-0001be40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001be50: 2020 6966 206d 6f64 652e 7374 7269 7028    if mode.strip(
-0001be60: 292e 7570 7065 7228 2920 213d 2022 5222  ).upper() != "R"
-0001be70: 2061 6e64 206e 6f74 2073 656c 662e 7072   and not self.pr
-0001be80: 6566 2e67 6574 2822 7275 6e5f 7374 6174  ef.get("run_stat
-0001be90: 6522 293a 0a20 2020 2020 2020 2020 2020  e"):.           
-0001bea0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0001beb0: 662e 666b 6579 735b 666b 6579 2e73 7472  f.fkeys[fkey.str
-0001bec0: 6970 2829 5d20 3d20 2862 7574 746f 6e6e  ip()] = (buttonn
-0001bed0: 616d 652e 7374 7269 7028 292c 2063 7774  ame.strip(), cwt
-0001bee0: 6578 742e 7374 7269 7028 2929 0a20 2020  ext.strip()).   
-0001bef0: 2020 2020 2020 2020 2020 2020 2065 7863               exc
-0001bf00: 6570 7420 5661 6c75 6545 7272 6f72 2061  ept ValueError a
-0001bf10: 7320 6572 723a 0a20 2020 2020 2020 2020  s err:.         
-0001bf20: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
-0001bf30: 722e 696e 666f 2822 7265 6164 5f63 775f  r.info("read_cw_
-0001bf40: 6d61 6372 6f73 3a20 2573 222c 2065 7272  macros: %s", err
-0001bf50: 290a 2020 2020 2020 2020 6b65 7973 203d  ).        keys =
-0001bf60: 2073 656c 662e 666b 6579 732e 6b65 7973   self.fkeys.keys
-0001bf70: 2829 0a20 2020 2020 2020 2069 6620 2246  ().        if "F
-0001bf80: 3122 2069 6e20 6b65 7973 3a0a 2020 2020  1" in keys:.    
-0001bf90: 2020 2020 2020 2020 7365 6c66 2e46 312e          self.F1.
-0001bfa0: 7365 7454 6578 7428 6622 4631 3a20 7b73  setText(f"F1: {s
-0001bfb0: 656c 662e 666b 6579 735b 2746 3127 5d5b  elf.fkeys['F1'][
-0001bfc0: 305d 7d22 290a 2020 2020 2020 2020 2020  0]}").          
-0001bfd0: 2020 7365 6c66 2e46 312e 7365 7454 6f6f    self.F1.setToo
-0001bfe0: 6c54 6970 2873 656c 662e 666b 6579 735b  lTip(self.fkeys[
-0001bff0: 2246 3122 5d5b 315d 290a 2020 2020 2020  "F1"][1]).      
-0001c000: 2020 6966 2022 4632 2220 696e 206b 6579    if "F2" in key
-0001c010: 733a 0a20 2020 2020 2020 2020 2020 2073  s:.            s
-0001c020: 656c 662e 4632 2e73 6574 5465 7874 2866  elf.F2.setText(f
-0001c030: 2246 323a 207b 7365 6c66 2e66 6b65 7973  "F2: {self.fkeys
-0001c040: 5b27 4632 275d 5b30 5d7d 2229 0a20 2020  ['F2'][0]}").   
+0001b950: 2020 6578 6365 7074 2046 696c 654e 6f74    except FileNot
+0001b960: 466f 756e 6445 7272 6f72 207c 2050 6572  FoundError | Per
+0001b970: 6d69 7373 696f 6e45 7272 6f72 207c 204f  missionError | O
+0001b980: 5345 7272 6f72 2061 7320 6572 723a 0a20  SError as err:. 
+0001b990: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+0001b9a0: 722e 6372 6974 6963 616c 280a 2020 2020  r.critical(.    
+0001b9b0: 2020 2020 2020 2020 2020 2020 6622 436f              f"Co
+0001b9c0: 756c 6420 6e6f 7420 6f70 656e 2066 696c  uld not open fil
+0001b9d0: 6520 7b66 7375 7469 6c73 2e55 5345 525f  e {fsutils.USER_
+0001b9e0: 4441 5441 5f50 4154 4820 2f20 6d61 6372  DATA_PATH / macr
+0001b9f0: 6f5f 6669 6c65 7d20 7b65 7272 7d22 0a20  o_file} {err}". 
+0001ba00: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
+0001ba10: 2020 6465 6620 7265 6164 5f63 775f 6d61    def read_cw_ma
+0001ba20: 6372 6f73 2873 656c 6629 202d 3e20 4e6f  cros(self) -> No
+0001ba30: 6e65 3a0a 2020 2020 2020 2020 2222 220a  ne:.        """.
+0001ba40: 2020 2020 2020 2020 5265 6164 7320 696e          Reads in
+0001ba50: 2074 6865 2043 5720 6d61 6372 6f73 2c20   the CW macros, 
+0001ba60: 6669 7273 7473 2069 7420 6368 6563 6b73  firsts it checks
+0001ba70: 2074 6f20 7365 6520 6966 2074 6865 2066   to see if the f
+0001ba80: 696c 6520 6578 6973 7473 2e20 4966 2069  ile exists. If i
+0001ba90: 7420 646f 6573 206e 6f74 2c0a 2020 2020  t does not,.    
+0001baa0: 2020 2020 616e 6420 7468 6973 2068 6173      and this has
+0001bab0: 2062 6565 6e20 7061 636b 6167 6564 2077   been packaged w
+0001bac0: 6974 6820 7079 696e 7374 616c 6c65 7220  ith pyinstaller 
+0001bad0: 6974 2077 696c 6c20 636f 7079 2074 6865  it will copy the
+0001bae0: 2064 6566 6175 6c74 2066 696c 6520 6672   default file fr
+0001baf0: 6f6d 2074 6865 0a20 2020 2020 2020 2074  om the.        t
+0001bb00: 656d 7020 6469 7265 6374 6f72 7920 7468  emp directory th
+0001bb10: 6973 2069 7320 7275 6e6e 696e 6720 6672  is is running fr
+0001bb20: 6f6d 2e2e 2e20 496e 2074 6865 6f72 792e  om... In theory.
+0001bb30: 0a20 2020 2020 2020 2022 2222 0a0a 2020  .        """..  
+0001bb40: 2020 2020 2020 6966 2073 656c 662e 7261        if self.ra
+0001bb50: 6469 6f5f 7374 6174 652e 6765 7428 226d  dio_state.get("m
+0001bb60: 6f64 6522 2920 3d3d 2022 4357 223a 0a20  ode") == "CW":. 
+0001bb70: 2020 2020 2020 2020 2020 206d 6163 726f             macro
+0001bb80: 5f66 696c 6520 3d20 2263 776d 6163 726f  _file = "cwmacro
+0001bb90: 732e 7478 7422 0a20 2020 2020 2020 2065  s.txt".        e
+0001bba0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0001bbb0: 206d 6163 726f 5f66 696c 6520 3d20 2273   macro_file = "s
+0001bbc0: 7362 6d61 6372 6f73 2e74 7874 220a 0a20  sbmacros.txt".. 
+0001bbd0: 2020 2020 2020 2069 6620 6e6f 7420 2866         if not (f
+0001bbe0: 7375 7469 6c73 2e55 5345 525f 4441 5441  sutils.USER_DATA
+0001bbf0: 5f50 4154 4820 2f20 6d61 6372 6f5f 6669  _PATH / macro_fi
+0001bc00: 6c65 292e 6578 6973 7473 2829 3a0a 2020  le).exists():.  
+0001bc10: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
+0001bc20: 2e64 6562 7567 2822 7265 6164 5f63 775f  .debug("read_cw_
+0001bc30: 6d61 6372 6f73 3a20 636f 7079 696e 6720  macros: copying 
+0001bc40: 6465 6661 756c 7420 6d61 6372 6f20 6669  default macro fi
+0001bc50: 6c65 2e22 290a 2020 2020 2020 2020 2020  le.").          
+0001bc60: 2020 636f 7079 6669 6c65 280a 2020 2020    copyfile(.    
+0001bc70: 2020 2020 2020 2020 2020 2020 6673 7574              fsut
+0001bc80: 696c 732e 4150 505f 4441 5441 5f50 4154  ils.APP_DATA_PAT
+0001bc90: 4820 2f20 6d61 6372 6f5f 6669 6c65 2c20  H / macro_file, 
+0001bca0: 6673 7574 696c 732e 5553 4552 5f44 4154  fsutils.USER_DAT
+0001bcb0: 415f 5041 5448 202f 206d 6163 726f 5f66  A_PATH / macro_f
+0001bcc0: 696c 650a 2020 2020 2020 2020 2020 2020  ile.            
+0001bcd0: 290a 2020 2020 2020 2020 7769 7468 206f  ).        with o
+0001bce0: 7065 6e28 0a20 2020 2020 2020 2020 2020  pen(.           
+0001bcf0: 2066 7375 7469 6c73 2e55 5345 525f 4441   fsutils.USER_DA
+0001bd00: 5441 5f50 4154 4820 2f20 6d61 6372 6f5f  TA_PATH / macro_
+0001bd10: 6669 6c65 2c20 2272 222c 2065 6e63 6f64  file, "r", encod
+0001bd20: 696e 673d 2275 7466 2d38 220a 2020 2020  ing="utf-8".    
+0001bd30: 2020 2020 2920 6173 2066 696c 655f 6465      ) as file_de
+0001bd40: 7363 7269 7074 6f72 3a0a 2020 2020 2020  scriptor:.      
+0001bd50: 2020 2020 2020 666f 7220 6c69 6e65 2069        for line i
+0001bd60: 6e20 6669 6c65 5f64 6573 6372 6970 746f  n file_descripto
+0001bd70: 723a 0a20 2020 2020 2020 2020 2020 2020  r:.             
+0001bd80: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+0001bd90: 2020 2020 2020 2020 2020 2020 6d6f 6465              mode
+0001bda0: 2c20 666b 6579 2c20 6275 7474 6f6e 6e61  , fkey, buttonna
+0001bdb0: 6d65 2c20 6377 7465 7874 203d 206c 696e  me, cwtext = lin
+0001bdc0: 652e 7370 6c69 7428 227c 2229 0a20 2020  e.split("|").   
+0001bdd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bde0: 2069 6620 6d6f 6465 2e73 7472 6970 2829   if mode.strip()
+0001bdf0: 2e75 7070 6572 2829 203d 3d20 2252 2220  .upper() == "R" 
+0001be00: 616e 6420 7365 6c66 2e70 7265 662e 6765  and self.pref.ge
+0001be10: 7428 2272 756e 5f73 7461 7465 2229 3a0a  t("run_state"):.
+0001be20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001be30: 2020 2020 2020 2020 7365 6c66 2e66 6b65          self.fke
+0001be40: 7973 5b66 6b65 792e 7374 7269 7028 295d  ys[fkey.strip()]
+0001be50: 203d 2028 6275 7474 6f6e 6e61 6d65 2e73   = (buttonname.s
+0001be60: 7472 6970 2829 2c20 6377 7465 7874 2e73  trip(), cwtext.s
+0001be70: 7472 6970 2829 290a 2020 2020 2020 2020  trip()).        
+0001be80: 2020 2020 2020 2020 2020 2020 6966 206d              if m
+0001be90: 6f64 652e 7374 7269 7028 292e 7570 7065  ode.strip().uppe
+0001bea0: 7228 2920 213d 2022 5222 2061 6e64 206e  r() != "R" and n
+0001beb0: 6f74 2073 656c 662e 7072 6566 2e67 6574  ot self.pref.get
+0001bec0: 2822 7275 6e5f 7374 6174 6522 293a 0a20  ("run_state"):. 
+0001bed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bee0: 2020 2020 2020 2073 656c 662e 666b 6579         self.fkey
+0001bef0: 735b 666b 6579 2e73 7472 6970 2829 5d20  s[fkey.strip()] 
+0001bf00: 3d20 2862 7574 746f 6e6e 616d 652e 7374  = (buttonname.st
+0001bf10: 7269 7028 292c 2063 7774 6578 742e 7374  rip(), cwtext.st
+0001bf20: 7269 7028 2929 0a20 2020 2020 2020 2020  rip()).         
+0001bf30: 2020 2020 2020 2065 7863 6570 7420 5661         except Va
+0001bf40: 6c75 6545 7272 6f72 2061 7320 6572 723a  lueError as err:
+0001bf50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001bf60: 2020 2020 206c 6f67 6765 722e 696e 666f       logger.info
+0001bf70: 2822 7265 6164 5f63 775f 6d61 6372 6f73  ("read_cw_macros
+0001bf80: 3a20 2573 222c 2065 7272 290a 2020 2020  : %s", err).    
+0001bf90: 2020 2020 6b65 7973 203d 2073 656c 662e      keys = self.
+0001bfa0: 666b 6579 732e 6b65 7973 2829 0a20 2020  fkeys.keys().   
+0001bfb0: 2020 2020 2069 6620 2246 3122 2069 6e20       if "F1" in 
+0001bfc0: 6b65 7973 3a0a 2020 2020 2020 2020 2020  keys:.          
+0001bfd0: 2020 7365 6c66 2e46 312e 7365 7454 6578    self.F1.setTex
+0001bfe0: 7428 6622 4631 3a20 7b73 656c 662e 666b  t(f"F1: {self.fk
+0001bff0: 6579 735b 2746 3127 5d5b 305d 7d22 290a  eys['F1'][0]}").
+0001c000: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0001c010: 2e46 312e 7365 7454 6f6f 6c54 6970 2873  .F1.setToolTip(s
+0001c020: 656c 662e 666b 6579 735b 2246 3122 5d5b  elf.fkeys["F1"][
+0001c030: 315d 290a 2020 2020 2020 2020 6966 2022  1]).        if "
+0001c040: 4632 2220 696e 206b 6579 733a 0a20 2020  F2" in keys:.   
 0001c050: 2020 2020 2020 2020 2073 656c 662e 4632           self.F2
-0001c060: 2e73 6574 546f 6f6c 5469 7028 7365 6c66  .setToolTip(self
-0001c070: 2e66 6b65 7973 5b22 4632 225d 5b31 5d29  .fkeys["F2"][1])
-0001c080: 0a20 2020 2020 2020 2069 6620 2246 3322  .        if "F3"
-0001c090: 2069 6e20 6b65 7973 3a0a 2020 2020 2020   in keys:.      
-0001c0a0: 2020 2020 2020 7365 6c66 2e46 332e 7365        self.F3.se
-0001c0b0: 7454 6578 7428 6622 4633 3a20 7b73 656c  tText(f"F3: {sel
-0001c0c0: 662e 666b 6579 735b 2746 3327 5d5b 305d  f.fkeys['F3'][0]
-0001c0d0: 7d22 290a 2020 2020 2020 2020 2020 2020  }").            
-0001c0e0: 7365 6c66 2e46 332e 7365 7454 6f6f 6c54  self.F3.setToolT
-0001c0f0: 6970 2873 656c 662e 666b 6579 735b 2246  ip(self.fkeys["F
-0001c100: 3322 5d5b 315d 290a 2020 2020 2020 2020  3"][1]).        
-0001c110: 6966 2022 4634 2220 696e 206b 6579 733a  if "F4" in keys:
-0001c120: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0001c130: 662e 4634 2e73 6574 5465 7874 2866 2246  f.F4.setText(f"F
-0001c140: 343a 207b 7365 6c66 2e66 6b65 7973 5b27  4: {self.fkeys['
-0001c150: 4634 275d 5b30 5d7d 2229 0a20 2020 2020  F4'][0]}").     
+0001c060: 2e73 6574 5465 7874 2866 2246 323a 207b  .setText(f"F2: {
+0001c070: 7365 6c66 2e66 6b65 7973 5b27 4632 275d  self.fkeys['F2']
+0001c080: 5b30 5d7d 2229 0a20 2020 2020 2020 2020  [0]}").         
+0001c090: 2020 2073 656c 662e 4632 2e73 6574 546f     self.F2.setTo
+0001c0a0: 6f6c 5469 7028 7365 6c66 2e66 6b65 7973  olTip(self.fkeys
+0001c0b0: 5b22 4632 225d 5b31 5d29 0a20 2020 2020  ["F2"][1]).     
+0001c0c0: 2020 2069 6620 2246 3322 2069 6e20 6b65     if "F3" in ke
+0001c0d0: 7973 3a0a 2020 2020 2020 2020 2020 2020  ys:.            
+0001c0e0: 7365 6c66 2e46 332e 7365 7454 6578 7428  self.F3.setText(
+0001c0f0: 6622 4633 3a20 7b73 656c 662e 666b 6579  f"F3: {self.fkey
+0001c100: 735b 2746 3327 5d5b 305d 7d22 290a 2020  s['F3'][0]}").  
+0001c110: 2020 2020 2020 2020 2020 7365 6c66 2e46            self.F
+0001c120: 332e 7365 7454 6f6f 6c54 6970 2873 656c  3.setToolTip(sel
+0001c130: 662e 666b 6579 735b 2246 3322 5d5b 315d  f.fkeys["F3"][1]
+0001c140: 290a 2020 2020 2020 2020 6966 2022 4634  ).        if "F4
+0001c150: 2220 696e 206b 6579 733a 0a20 2020 2020  " in keys:.     
 0001c160: 2020 2020 2020 2073 656c 662e 4634 2e73         self.F4.s
-0001c170: 6574 546f 6f6c 5469 7028 7365 6c66 2e66  etToolTip(self.f
-0001c180: 6b65 7973 5b22 4634 225d 5b31 5d29 0a20  keys["F4"][1]). 
-0001c190: 2020 2020 2020 2069 6620 2246 3522 2069         if "F5" i
-0001c1a0: 6e20 6b65 7973 3a0a 2020 2020 2020 2020  n keys:.        
-0001c1b0: 2020 2020 7365 6c66 2e46 352e 7365 7454      self.F5.setT
-0001c1c0: 6578 7428 6622 4635 3a20 7b73 656c 662e  ext(f"F5: {self.
-0001c1d0: 666b 6579 735b 2746 3527 5d5b 305d 7d22  fkeys['F5'][0]}"
-0001c1e0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-0001c1f0: 6c66 2e46 352e 7365 7454 6f6f 6c54 6970  lf.F5.setToolTip
-0001c200: 2873 656c 662e 666b 6579 735b 2246 3522  (self.fkeys["F5"
-0001c210: 5d5b 315d 290a 2020 2020 2020 2020 6966  ][1]).        if
-0001c220: 2022 4636 2220 696e 206b 6579 733a 0a20   "F6" in keys:. 
-0001c230: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0001c240: 4636 2e73 6574 5465 7874 2866 2246 363a  F6.setText(f"F6:
-0001c250: 207b 7365 6c66 2e66 6b65 7973 5b27 4636   {self.fkeys['F6
-0001c260: 275d 5b30 5d7d 2229 0a20 2020 2020 2020  '][0]}").       
+0001c170: 6574 5465 7874 2866 2246 343a 207b 7365  etText(f"F4: {se
+0001c180: 6c66 2e66 6b65 7973 5b27 4634 275d 5b30  lf.fkeys['F4'][0
+0001c190: 5d7d 2229 0a20 2020 2020 2020 2020 2020  ]}").           
+0001c1a0: 2073 656c 662e 4634 2e73 6574 546f 6f6c   self.F4.setTool
+0001c1b0: 5469 7028 7365 6c66 2e66 6b65 7973 5b22  Tip(self.fkeys["
+0001c1c0: 4634 225d 5b31 5d29 0a20 2020 2020 2020  F4"][1]).       
+0001c1d0: 2069 6620 2246 3522 2069 6e20 6b65 7973   if "F5" in keys
+0001c1e0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0001c1f0: 6c66 2e46 352e 7365 7454 6578 7428 6622  lf.F5.setText(f"
+0001c200: 4635 3a20 7b73 656c 662e 666b 6579 735b  F5: {self.fkeys[
+0001c210: 2746 3527 5d5b 305d 7d22 290a 2020 2020  'F5'][0]}").    
+0001c220: 2020 2020 2020 2020 7365 6c66 2e46 352e          self.F5.
+0001c230: 7365 7454 6f6f 6c54 6970 2873 656c 662e  setToolTip(self.
+0001c240: 666b 6579 735b 2246 3522 5d5b 315d 290a  fkeys["F5"][1]).
+0001c250: 2020 2020 2020 2020 6966 2022 4636 2220          if "F6" 
+0001c260: 696e 206b 6579 733a 0a20 2020 2020 2020  in keys:.       
 0001c270: 2020 2020 2073 656c 662e 4636 2e73 6574       self.F6.set
-0001c280: 546f 6f6c 5469 7028 7365 6c66 2e66 6b65  ToolTip(self.fke
-0001c290: 7973 5b22 4636 225d 5b31 5d29 0a20 2020  ys["F6"][1]).   
-0001c2a0: 2020 2020 2069 6620 2246 3722 2069 6e20       if "F7" in 
-0001c2b0: 6b65 7973 3a0a 2020 2020 2020 2020 2020  keys:.          
-0001c2c0: 2020 7365 6c66 2e46 372e 7365 7454 6578    self.F7.setTex
-0001c2d0: 7428 6622 4637 3a20 7b73 656c 662e 666b  t(f"F7: {self.fk
-0001c2e0: 6579 735b 2746 3727 5d5b 305d 7d22 290a  eys['F7'][0]}").
+0001c280: 5465 7874 2866 2246 363a 207b 7365 6c66  Text(f"F6: {self
+0001c290: 2e66 6b65 7973 5b27 4636 275d 5b30 5d7d  .fkeys['F6'][0]}
+0001c2a0: 2229 0a20 2020 2020 2020 2020 2020 2073  ").            s
+0001c2b0: 656c 662e 4636 2e73 6574 546f 6f6c 5469  elf.F6.setToolTi
+0001c2c0: 7028 7365 6c66 2e66 6b65 7973 5b22 4636  p(self.fkeys["F6
+0001c2d0: 225d 5b31 5d29 0a20 2020 2020 2020 2069  "][1]).        i
+0001c2e0: 6620 2246 3722 2069 6e20 6b65 7973 3a0a  f "F7" in keys:.
 0001c2f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0001c300: 2e46 372e 7365 7454 6f6f 6c54 6970 2873  .F7.setToolTip(s
-0001c310: 656c 662e 666b 6579 735b 2246 3722 5d5b  elf.fkeys["F7"][
-0001c320: 315d 290a 2020 2020 2020 2020 6966 2022  1]).        if "
-0001c330: 4638 2220 696e 206b 6579 733a 0a20 2020  F8" in keys:.   
-0001c340: 2020 2020 2020 2020 2073 656c 662e 4638           self.F8
-0001c350: 2e73 6574 5465 7874 2866 2246 383a 207b  .setText(f"F8: {
-0001c360: 7365 6c66 2e66 6b65 7973 5b27 4638 275d  self.fkeys['F8']
-0001c370: 5b30 5d7d 2229 0a20 2020 2020 2020 2020  [0]}").         
-0001c380: 2020 2073 656c 662e 4638 2e73 6574 546f     self.F8.setTo
-0001c390: 6f6c 5469 7028 7365 6c66 2e66 6b65 7973  olTip(self.fkeys
-0001c3a0: 5b22 4638 225d 5b31 5d29 0a20 2020 2020  ["F8"][1]).     
-0001c3b0: 2020 2069 6620 2246 3922 2069 6e20 6b65     if "F9" in ke
-0001c3c0: 7973 3a0a 2020 2020 2020 2020 2020 2020  ys:.            
-0001c3d0: 7365 6c66 2e46 392e 7365 7454 6578 7428  self.F9.setText(
-0001c3e0: 6622 4639 3a20 7b73 656c 662e 666b 6579  f"F9: {self.fkey
-0001c3f0: 735b 2746 3927 5d5b 305d 7d22 290a 2020  s['F9'][0]}").  
+0001c300: 2e46 372e 7365 7454 6578 7428 6622 4637  .F7.setText(f"F7
+0001c310: 3a20 7b73 656c 662e 666b 6579 735b 2746  : {self.fkeys['F
+0001c320: 3727 5d5b 305d 7d22 290a 2020 2020 2020  7'][0]}").      
+0001c330: 2020 2020 2020 7365 6c66 2e46 372e 7365        self.F7.se
+0001c340: 7454 6f6f 6c54 6970 2873 656c 662e 666b  tToolTip(self.fk
+0001c350: 6579 735b 2246 3722 5d5b 315d 290a 2020  eys["F7"][1]).  
+0001c360: 2020 2020 2020 6966 2022 4638 2220 696e        if "F8" in
+0001c370: 206b 6579 733a 0a20 2020 2020 2020 2020   keys:.         
+0001c380: 2020 2073 656c 662e 4638 2e73 6574 5465     self.F8.setTe
+0001c390: 7874 2866 2246 383a 207b 7365 6c66 2e66  xt(f"F8: {self.f
+0001c3a0: 6b65 7973 5b27 4638 275d 5b30 5d7d 2229  keys['F8'][0]}")
+0001c3b0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0001c3c0: 662e 4638 2e73 6574 546f 6f6c 5469 7028  f.F8.setToolTip(
+0001c3d0: 7365 6c66 2e66 6b65 7973 5b22 4638 225d  self.fkeys["F8"]
+0001c3e0: 5b31 5d29 0a20 2020 2020 2020 2069 6620  [1]).        if 
+0001c3f0: 2246 3922 2069 6e20 6b65 7973 3a0a 2020  "F9" in keys:.  
 0001c400: 2020 2020 2020 2020 2020 7365 6c66 2e46            self.F
-0001c410: 392e 7365 7454 6f6f 6c54 6970 2873 656c  9.setToolTip(sel
-0001c420: 662e 666b 6579 735b 2246 3922 5d5b 315d  f.fkeys["F9"][1]
-0001c430: 290a 2020 2020 2020 2020 6966 2022 4631  ).        if "F1
-0001c440: 3022 2069 6e20 6b65 7973 3a0a 2020 2020  0" in keys:.    
-0001c450: 2020 2020 2020 2020 7365 6c66 2e46 3130          self.F10
-0001c460: 2e73 6574 5465 7874 2866 2246 3130 3a20  .setText(f"F10: 
-0001c470: 7b73 656c 662e 666b 6579 735b 2746 3130  {self.fkeys['F10
-0001c480: 275d 5b30 5d7d 2229 0a20 2020 2020 2020  '][0]}").       
-0001c490: 2020 2020 2073 656c 662e 4631 302e 7365       self.F10.se
-0001c4a0: 7454 6f6f 6c54 6970 2873 656c 662e 666b  tToolTip(self.fk
-0001c4b0: 6579 735b 2246 3130 225d 5b31 5d29 0a20  eys["F10"][1]). 
-0001c4c0: 2020 2020 2020 2069 6620 2246 3131 2220         if "F11" 
-0001c4d0: 696e 206b 6579 733a 0a20 2020 2020 2020  in keys:.       
-0001c4e0: 2020 2020 2073 656c 662e 4631 312e 7365       self.F11.se
-0001c4f0: 7454 6578 7428 6622 4631 313a 207b 7365  tText(f"F11: {se
-0001c500: 6c66 2e66 6b65 7973 5b27 4631 3127 5d5b  lf.fkeys['F11'][
-0001c510: 305d 7d22 290a 2020 2020 2020 2020 2020  0]}").          
-0001c520: 2020 7365 6c66 2e46 3131 2e73 6574 546f    self.F11.setTo
-0001c530: 6f6c 5469 7028 7365 6c66 2e66 6b65 7973  olTip(self.fkeys
-0001c540: 5b22 4631 3122 5d5b 315d 290a 2020 2020  ["F11"][1]).    
-0001c550: 2020 2020 6966 2022 4631 3222 2069 6e20      if "F12" in 
-0001c560: 6b65 7973 3a0a 2020 2020 2020 2020 2020  keys:.          
-0001c570: 2020 7365 6c66 2e46 3132 2e73 6574 5465    self.F12.setTe
-0001c580: 7874 2866 2246 3132 3a20 7b73 656c 662e  xt(f"F12: {self.
-0001c590: 666b 6579 735b 2746 3132 275d 5b30 5d7d  fkeys['F12'][0]}
-0001c5a0: 2229 0a20 2020 2020 2020 2020 2020 2073  ").            s
-0001c5b0: 656c 662e 4631 322e 7365 7454 6f6f 6c54  elf.F12.setToolT
-0001c5c0: 6970 2873 656c 662e 666b 6579 735b 2246  ip(self.fkeys["F
-0001c5d0: 3132 225d 5b31 5d29 0a0a 2020 2020 6465  12"][1])..    de
-0001c5e0: 6620 6765 6e65 7261 7465 5f61 6469 6628  f generate_adif(
-0001c5f0: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
-0001c600: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0001c610: 2020 2043 616c 6c73 2074 6865 2063 6f6e     Calls the con
-0001c620: 7465 7374 2041 4449 4620 6669 6c65 2067  test ADIF file g
-0001c630: 656e 6572 6174 6f72 2e0a 0a20 2020 2020  enerator...     
-0001c640: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
-0001c650: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
-0001c660: 0a20 2020 2020 2020 204e 6f6e 650a 0a20  .        None.. 
-0001c670: 2020 2020 2020 2052 6574 7572 6e73 0a20         Returns. 
-0001c680: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0a20         -------. 
-0001c690: 2020 2020 2020 204e 6f6e 650a 2020 2020         None.    
-0001c6a0: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
-0001c6b0: 2023 2068 7474 7073 3a2f 2f77 7777 2e61   # https://www.a
-0001c6c0: 6469 662e 6f72 672f 3331 352f 4144 4946  dif.org/315/ADIF
-0001c6d0: 5f33 3135 2e68 746d 0a20 2020 2020 2020  _315.htm.       
-0001c6e0: 206c 6f67 6765 722e 6465 6275 6728 222a   logger.debug("*
-0001c6f0: 2a2a 2a2a 2a41 4449 462a 2a2a 2a2a 2229  *****ADIF*****")
-0001c700: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
-0001c710: 6e74 6573 742e 6164 6966 2873 656c 6629  ntest.adif(self)
-0001c720: 0a0a 2020 2020 6465 6620 6765 6e65 7261  ..    def genera
-0001c730: 7465 5f63 6162 7269 6c6c 6f28 7365 6c66  te_cabrillo(self
-0001c740: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-0001c750: 2020 2022 2222 0a20 2020 2020 2020 2043     """.        C
-0001c760: 616c 6c73 2074 6865 2063 6f6e 7465 7374  alls the contest
-0001c770: 2043 6162 7269 6c6c 6f20 6669 6c65 2067   Cabrillo file g
-0001c780: 656e 6572 6174 6f72 2e20 4d61 7962 652e  enerator. Maybe.
-0001c790: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
-0001c7a0: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
-0001c7b0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-0001c7c0: 4e6f 6e65 0a0a 2020 2020 2020 2020 5265  None..        Re
-0001c7d0: 7475 726e 730a 2020 2020 2020 2020 2d2d  turns.        --
-0001c7e0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 4e6f  -----.        No
-0001c7f0: 6e65 0a20 2020 2020 2020 2022 2222 0a0a  ne.        """..
-0001c800: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
-0001c810: 6562 7567 2822 2a2a 2a2a 2a2a 4361 6272  ebug("******Cabr
-0001c820: 696c 6c6f 2a2a 2a2a 2a22 290a 2020 2020  illo*****").    
-0001c830: 2020 2020 7365 6c66 2e63 6f6e 7465 7374      self.contest
-0001c840: 2e63 6162 7269 6c6c 6f28 7365 6c66 290a  .cabrillo(self).
-0001c850: 0a0a 6465 6620 6c6f 6164 5f66 6f6e 7473  ..def load_fonts
-0001c860: 5f66 726f 6d5f 6469 7228 6469 7265 6374  _from_dir(direct
-0001c870: 6f72 793a 2073 7472 2920 2d3e 2073 6574  ory: str) -> set
-0001c880: 3a0a 2020 2020 2222 220a 2020 2020 5765  :.    """.    We
-0001c890: 6c6c 2069 7420 6c6f 6164 7320 666f 6e74  ll it loads font
-0001c8a0: 7320 6672 6f6d 2061 2064 6972 6563 746f  s from a directo
-0001c8b0: 7279 2e2e 2e0a 0a20 2020 2050 6172 616d  ry.....    Param
-0001c8c0: 6574 6572 730a 2020 2020 2d2d 2d2d 2d2d  eters.    ------
-0001c8d0: 2d2d 2d2d 0a20 2020 2064 6972 6563 746f  ----.    directo
-0001c8e0: 7279 203a 2073 7472 0a20 2020 2054 6865  ry : str.    The
-0001c8f0: 2064 6972 6563 746f 7279 2074 6f20 6c6f   directory to lo
-0001c900: 6164 2066 6f6e 7473 2066 726f 6d2e 0a0a  ad fonts from...
-0001c910: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
-0001c920: 2d2d 2d2d 2d2d 2d0a 2020 2020 7365 740a  -------.    set.
-0001c930: 2020 2020 4120 7365 7420 6f66 2066 6f6e      A set of fon
-0001c940: 7420 6661 6d69 6c69 6573 2069 6e73 7461  t families insta
-0001c950: 6c6c 6564 2069 6e20 7468 6520 6469 7265  lled in the dire
-0001c960: 6374 6f72 792e 0a20 2020 2022 2222 0a20  ctory..    """. 
-0001c970: 2020 2066 6f6e 745f 6661 6d69 6c69 6573     font_families
-0001c980: 203d 2073 6574 2829 0a20 2020 2066 6f72   = set().    for
-0001c990: 205f 6669 2069 6e20 5144 6972 2864 6972   _fi in QDir(dir
-0001c9a0: 6563 746f 7279 292e 656e 7472 7949 6e66  ectory).entryInf
-0001c9b0: 6f4c 6973 7428 5b22 2a2e 7474 6622 2c20  oList(["*.ttf", 
-0001c9c0: 222a 2e77 6f66 6622 2c20 222a 2e77 6f66  "*.woff", "*.wof
-0001c9d0: 6632 225d 293a 0a20 2020 2020 2020 205f  f2"]):.        _
-0001c9e0: 6964 203d 2051 466f 6e74 4461 7461 6261  id = QFontDataba
-0001c9f0: 7365 2e61 6464 4170 706c 6963 6174 696f  se.addApplicatio
-0001ca00: 6e46 6f6e 7428 5f66 692e 6162 736f 6c75  nFont(_fi.absolu
-0001ca10: 7465 4669 6c65 5061 7468 2829 290a 2020  teFilePath()).  
-0001ca20: 2020 2020 2020 666f 6e74 5f66 616d 696c        font_famil
-0001ca30: 6965 7320 7c3d 2073 6574 2851 466f 6e74  ies |= set(QFont
-0001ca40: 4461 7461 6261 7365 2e61 7070 6c69 6361  Database.applica
-0001ca50: 7469 6f6e 466f 6e74 4661 6d69 6c69 6573  tionFontFamilies
-0001ca60: 285f 6964 2929 0a20 2020 2072 6574 7572  (_id)).    retur
-0001ca70: 6e20 666f 6e74 5f66 616d 696c 6965 730a  n font_families.
-0001ca80: 0a0a 6465 6620 696e 7374 616c 6c5f 6963  ..def install_ic
-0001ca90: 6f6e 7328 2920 2d3e 204e 6f6e 653a 0a20  ons() -> None:. 
-0001caa0: 2020 2022 2222 496e 7374 616c 6c20 6963     """Install ic
-0001cab0: 6f6e 7322 2222 0a0a 2020 2020 6966 2073  ons"""..    if s
-0001cac0: 7973 2e70 6c61 7466 6f72 6d20 3d3d 2022  ys.platform == "
-0001cad0: 6c69 6e75 7822 3a0a 2020 2020 2020 2020  linux":.        
-0001cae0: 6f73 2e73 7973 7465 6d28 0a20 2020 2020  os.system(.     
-0001caf0: 2020 2020 2020 2022 7864 672d 6963 6f6e         "xdg-icon
-0001cb00: 2d72 6573 6f75 7263 6520 696e 7374 616c  -resource instal
-0001cb10: 6c20 2d2d 7369 7a65 2033 3220 2d2d 636f  l --size 32 --co
-0001cb20: 6e74 6578 7420 6170 7073 202d 2d6d 6f64  ntext apps --mod
-0001cb30: 6520 7573 6572 2022 0a20 2020 2020 2020  e user ".       
-0001cb40: 2020 2020 2066 227b 6673 7574 696c 732e       f"{fsutils.
-0001cb50: 4150 505f 4441 5441 5f50 4154 487d 2f6b  APP_DATA_PATH}/k
-0001cb60: 3667 7465 2e6e 6f74 316d 6d2d 3332 2e70  6gte.not1mm-32.p
-0001cb70: 6e67 206b 3667 7465 2d6e 6f74 316d 6d22  ng k6gte-not1mm"
-0001cb80: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-0001cb90: 2020 206f 732e 7379 7374 656d 280a 2020     os.system(.  
-0001cba0: 2020 2020 2020 2020 2020 2278 6467 2d69            "xdg-i
-0001cbb0: 636f 6e2d 7265 736f 7572 6365 2069 6e73  con-resource ins
-0001cbc0: 7461 6c6c 202d 2d73 697a 6520 3634 202d  tall --size 64 -
-0001cbd0: 2d63 6f6e 7465 7874 2061 7070 7320 2d2d  -context apps --
-0001cbe0: 6d6f 6465 2075 7365 7220 220a 2020 2020  mode user ".    
-0001cbf0: 2020 2020 2020 2020 6622 7b66 7375 7469          f"{fsuti
-0001cc00: 6c73 2e41 5050 5f44 4154 415f 5041 5448  ls.APP_DATA_PATH
-0001cc10: 7d2f 6b36 6774 652e 6e6f 7431 6d6d 2d36  }/k6gte.not1mm-6
-0001cc20: 342e 706e 6720 6b36 6774 652d 6e6f 7431  4.png k6gte-not1
-0001cc30: 6d6d 220a 2020 2020 2020 2020 290a 2020  mm".        ).  
-0001cc40: 2020 2020 2020 6f73 2e73 7973 7465 6d28        os.system(
-0001cc50: 0a20 2020 2020 2020 2020 2020 2022 7864  .            "xd
-0001cc60: 672d 6963 6f6e 2d72 6573 6f75 7263 6520  g-icon-resource 
-0001cc70: 696e 7374 616c 6c20 2d2d 7369 7a65 2031  install --size 1
-0001cc80: 3238 202d 2d63 6f6e 7465 7874 2061 7070  28 --context app
-0001cc90: 7320 2d2d 6d6f 6465 2075 7365 7220 220a  s --mode user ".
-0001cca0: 2020 2020 2020 2020 2020 2020 6622 7b66              f"{f
-0001ccb0: 7375 7469 6c73 2e41 5050 5f44 4154 415f  sutils.APP_DATA_
-0001ccc0: 5041 5448 7d2f 6b36 6774 652e 6e6f 7431  PATH}/k6gte.not1
-0001ccd0: 6d6d 2d31 3238 2e70 6e67 206b 3667 7465  mm-128.png k6gte
-0001cce0: 2d6e 6f74 316d 6d22 0a20 2020 2020 2020  -not1mm".       
-0001ccf0: 2029 0a20 2020 2020 2020 206f 732e 7379   ).        os.sy
-0001cd00: 7374 656d 280a 2020 2020 2020 2020 2020  stem(.          
-0001cd10: 2020 6622 7864 672d 6465 736b 746f 702d    f"xdg-desktop-
-0001cd20: 6d65 6e75 2069 6e73 7461 6c6c 207b 6673  menu install {fs
-0001cd30: 7574 696c 732e 4150 505f 4441 5441 5f50  utils.APP_DATA_P
-0001cd40: 4154 487d 2f6b 3667 7465 2d6e 6f74 316d  ATH}/k6gte-not1m
-0001cd50: 6d2e 6465 736b 746f 7022 0a20 2020 2020  m.desktop".     
-0001cd60: 2020 2029 0a0a 0a64 6566 2064 6f69 6d70     )...def doimp
-0001cd70: 286d 6f64 6e61 6d65 2920 2d3e 206f 626a  (modname) -> obj
-0001cd80: 6563 743a 0a20 2020 2022 2222 0a20 2020  ect:.    """.   
-0001cd90: 2049 6d70 6f72 7473 2061 206d 6f64 756c   Imports a modul
-0001cda0: 652e 0a0a 2020 2020 5061 7261 6d65 7465  e...    Paramete
-0001cdb0: 7273 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  rs.    ---------
-0001cdc0: 2d0a 2020 2020 6d6f 646e 616d 6520 3a20  -.    modname : 
-0001cdd0: 7374 720a 2020 2020 5468 6520 6e61 6d65  str.    The name
-0001cde0: 206f 6620 7468 6520 6d6f 6475 6c65 2074   of the module t
-0001cdf0: 6f20 696d 706f 7274 2e0a 0a20 2020 2052  o import...    R
-0001ce00: 6574 7572 6e73 0a20 2020 202d 2d2d 2d2d  eturns.    -----
-0001ce10: 2d2d 0a20 2020 206f 626a 6563 740a 2020  --.    object.  
-0001ce20: 2020 5468 6520 6d6f 6475 6c65 206f 626a    The module obj
-0001ce30: 6563 742e 0a20 2020 2022 2222 0a0a 2020  ect..    """..  
-0001ce40: 2020 6c6f 6767 6572 2e64 6562 7567 2822    logger.debug("
-0001ce50: 646f 696d 703a 2025 7322 2c20 6d6f 646e  doimp: %s", modn
-0001ce60: 616d 6529 0a20 2020 2072 6574 7572 6e20  ame).    return 
-0001ce70: 696d 706f 7274 6c69 622e 696d 706f 7274  importlib.import
-0001ce80: 5f6d 6f64 756c 6528 6622 6e6f 7431 6d6d  _module(f"not1mm
-0001ce90: 2e70 6c75 6769 6e73 2e7b 6d6f 646e 616d  .plugins.{modnam
-0001cea0: 657d 2229 0a0a 0a64 6566 2072 756e 2829  e}")...def run()
-0001ceb0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2222   -> None:.    ""
-0001cec0: 220a 2020 2020 4d61 696e 2045 6e74 7279  ".    Main Entry
-0001ced0: 0a20 2020 2022 2222 0a20 2020 206c 6f67  .    """.    log
-0001cee0: 6765 722e 6465 6275 6728 0a20 2020 2020  ger.debug(.     
-0001cef0: 2020 2066 2252 6573 6f6c 7665 6420 4f53     f"Resolved OS
-0001cf00: 2066 696c 6520 7379 7374 656d 2070 6174   file system pat
-0001cf10: 6873 3a20 4d4f 4455 4c45 5f50 4154 4820  hs: MODULE_PATH 
-0001cf20: 7b66 7375 7469 6c73 2e4d 4f44 554c 455f  {fsutils.MODULE_
-0001cf30: 5041 5448 7d2c 2055 5345 525f 4441 5441  PATH}, USER_DATA
-0001cf40: 5f50 4154 4820 7b66 7375 7469 6c73 2e55  _PATH {fsutils.U
-0001cf50: 5345 525f 4441 5441 5f50 4154 487d 2c20  SER_DATA_PATH}, 
-0001cf60: 434f 4e46 4947 5f50 4154 4820 7b66 7375  CONFIG_PATH {fsu
-0001cf70: 7469 6c73 2e43 4f4e 4649 475f 5041 5448  tils.CONFIG_PATH
-0001cf80: 7d22 0a20 2020 2029 0a20 2020 2069 6e73  }".    ).    ins
-0001cf90: 7461 6c6c 5f69 636f 6e73 2829 0a20 2020  tall_icons().   
-0001cfa0: 2074 696d 6572 2e73 7461 7274 2832 3530   timer.start(250
-0001cfb0: 290a 2020 2020 7379 732e 6578 6974 2861  ).    sys.exit(a
-0001cfc0: 7070 2e65 7865 6328 2929 0a0a 0a44 4542  pp.exec())...DEB
-0001cfd0: 5547 5f45 4e41 424c 4544 203d 2046 616c  UG_ENABLED = Fal
-0001cfe0: 7365 0a69 6620 5061 7468 2822 2e2f 6465  se.if Path("./de
-0001cff0: 6275 6722 292e 6578 6973 7473 2829 3a0a  bug").exists():.
-0001d000: 2020 2020 4445 4255 475f 454e 4142 4c45      DEBUG_ENABLE
-0001d010: 4420 3d20 5472 7565 0a0a 6c6f 6767 6572  D = True..logger
-0001d020: 203d 206c 6f67 6769 6e67 2e67 6574 4c6f   = logging.getLo
-0001d030: 6767 6572 2822 5f5f 6d61 696e 5f5f 2229  gger("__main__")
-0001d040: 0a0a 6c6f 6767 696e 672e 6261 7369 6343  ..logging.basicC
-0001d050: 6f6e 6669 6728 0a20 2020 206c 6576 656c  onfig(.    level
-0001d060: 3d6c 6f67 6769 6e67 2e44 4542 5547 2069  =logging.DEBUG i
-0001d070: 6620 4445 4255 475f 454e 4142 4c45 4420  f DEBUG_ENABLED 
-0001d080: 656c 7365 206c 6f67 6769 6e67 2e43 5249  else logging.CRI
-0001d090: 5449 4341 4c2c 0a20 2020 2066 6f72 6d61  TICAL,.    forma
-0001d0a0: 743d 225b 2528 6173 6374 696d 6529 735d  t="[%(asctime)s]
-0001d0b0: 2025 286c 6576 656c 6e61 6d65 2973 2025   %(levelname)s %
-0001d0c0: 286e 616d 6529 7320 2d20 2528 6675 6e63  (name)s - %(func
-0001d0d0: 4e61 6d65 2973 204c 696e 6520 2528 6c69  Name)s Line %(li
-0001d0e0: 6e65 6e6f 2964 3a20 2528 6d65 7373 6167  neno)d: %(messag
-0001d0f0: 6529 7322 2c0a 2020 2020 6861 6e64 6c65  e)s",.    handle
-0001d100: 7273 3d5b 0a20 2020 2020 2020 2052 6f74  rs=[.        Rot
-0001d110: 6174 696e 6746 696c 6548 616e 646c 6572  atingFileHandler
-0001d120: 2866 7375 7469 6c73 2e4c 4f47 5f46 494c  (fsutils.LOG_FIL
-0001d130: 452c 206d 6178 4279 7465 733d 3130 3439  E, maxBytes=1049
-0001d140: 3030 3030 2c20 6261 636b 7570 436f 756e  0000, backupCoun
-0001d150: 743d 3230 292c 0a20 2020 2020 2020 206c  t=20),.        l
-0001d160: 6f67 6769 6e67 2e53 7472 6561 6d48 616e  ogging.StreamHan
-0001d170: 646c 6572 2829 2c0a 2020 2020 5d2c 0a29  dler(),.    ],.)
-0001d180: 0a6c 6f67 6769 6e67 2e67 6574 4c6f 6767  .logging.getLogg
-0001d190: 6572 2822 5079 5174 352e 7569 632e 7569  er("PyQt5.uic.ui
-0001d1a0: 7061 7273 6572 2229 2e73 6574 4c65 7665  parser").setLeve
-0001d1b0: 6c28 2249 4e46 4f22 290a 6c6f 6767 696e  l("INFO").loggin
-0001d1c0: 672e 6765 744c 6f67 6765 7228 2250 7951  g.getLogger("PyQ
-0001d1d0: 7435 2e75 6963 2e70 726f 7065 7274 6965  t5.uic.propertie
-0001d1e0: 7322 292e 7365 744c 6576 656c 2822 494e  s").setLevel("IN
-0001d1f0: 464f 2229 0a61 7070 203d 2051 7457 6964  FO").app = QtWid
-0001d200: 6765 7473 2e51 4170 706c 6963 6174 696f  gets.QApplicatio
-0001d210: 6e28 7379 732e 6172 6776 290a 6661 6d69  n(sys.argv).fami
-0001d220: 6c69 6573 203d 206c 6f61 645f 666f 6e74  lies = load_font
-0001d230: 735f 6672 6f6d 5f64 6972 286f 732e 6673  s_from_dir(os.fs
-0001d240: 7061 7468 2866 7375 7469 6c73 2e41 5050  path(fsutils.APP
-0001d250: 5f44 4154 415f 5041 5448 2929 0a6c 6f67  _DATA_PATH)).log
-0001d260: 6765 722e 696e 666f 2866 2266 6f6e 7420  ger.info(f"font 
-0001d270: 6661 6d69 6c69 6573 207b 6661 6d69 6c69  families {famili
-0001d280: 6573 7d22 290a 7769 6e64 6f77 203d 204d  es}").window = M
-0001d290: 6169 6e57 696e 646f 7728 290a 6865 6967  ainWindow().heig
-0001d2a0: 6874 203d 2077 696e 646f 772e 7072 6566  ht = window.pref
-0001d2b0: 2e67 6574 2822 7769 6e64 6f77 5f68 6569  .get("window_hei
-0001d2c0: 6768 7422 2c20 3330 3029 0a77 6964 7468  ght", 300).width
-0001d2d0: 203d 2077 696e 646f 772e 7072 6566 2e67   = window.pref.g
-0001d2e0: 6574 2822 7769 6e64 6f77 5f77 6964 7468  et("window_width
-0001d2f0: 222c 2037 3030 290a 7820 3d20 7769 6e64  ", 700).x = wind
-0001d300: 6f77 2e70 7265 662e 6765 7428 2277 696e  ow.pref.get("win
-0001d310: 646f 775f 7822 2c20 2d31 290a 7920 3d20  dow_x", -1).y = 
-0001d320: 7769 6e64 6f77 2e70 7265 662e 6765 7428  window.pref.get(
-0001d330: 2277 696e 646f 775f 7922 2c20 2d31 290a  "window_y", -1).
-0001d340: 7769 6e64 6f77 2e73 6574 4765 6f6d 6574  window.setGeomet
-0001d350: 7279 2878 2c20 792c 2077 6964 7468 2c20  ry(x, y, width, 
-0001d360: 6865 6967 6874 290a 7769 6e64 6f77 2e63  height).window.c
-0001d370: 616c 6c73 6967 6e2e 7365 7446 6f63 7573  allsign.setFocus
-0001d380: 2829 0a77 696e 646f 772e 7368 6f77 2829  ().window.show()
-0001d390: 0a74 696d 6572 203d 2051 7443 6f72 652e  .timer = QtCore.
-0001d3a0: 5154 696d 6572 2829 0a74 696d 6572 2e74  QTimer().timer.t
-0001d3b0: 696d 656f 7574 2e63 6f6e 6e65 6374 2877  imeout.connect(w
-0001d3c0: 696e 646f 772e 706f 6c6c 5f72 6164 696f  indow.poll_radio
-0001d3d0: 290a 0a69 6620 5f5f 6e61 6d65 5f5f 203d  )..if __name__ =
-0001d3e0: 3d20 225f 5f6d 6169 6e5f 5f22 3a0a 2020  = "__main__":.  
-0001d3f0: 2020 7275 6e28 290a                        run().
+0001c410: 392e 7365 7454 6578 7428 6622 4639 3a20  9.setText(f"F9: 
+0001c420: 7b73 656c 662e 666b 6579 735b 2746 3927  {self.fkeys['F9'
+0001c430: 5d5b 305d 7d22 290a 2020 2020 2020 2020  ][0]}").        
+0001c440: 2020 2020 7365 6c66 2e46 392e 7365 7454      self.F9.setT
+0001c450: 6f6f 6c54 6970 2873 656c 662e 666b 6579  oolTip(self.fkey
+0001c460: 735b 2246 3922 5d5b 315d 290a 2020 2020  s["F9"][1]).    
+0001c470: 2020 2020 6966 2022 4631 3022 2069 6e20      if "F10" in 
+0001c480: 6b65 7973 3a0a 2020 2020 2020 2020 2020  keys:.          
+0001c490: 2020 7365 6c66 2e46 3130 2e73 6574 5465    self.F10.setTe
+0001c4a0: 7874 2866 2246 3130 3a20 7b73 656c 662e  xt(f"F10: {self.
+0001c4b0: 666b 6579 735b 2746 3130 275d 5b30 5d7d  fkeys['F10'][0]}
+0001c4c0: 2229 0a20 2020 2020 2020 2020 2020 2073  ").            s
+0001c4d0: 656c 662e 4631 302e 7365 7454 6f6f 6c54  elf.F10.setToolT
+0001c4e0: 6970 2873 656c 662e 666b 6579 735b 2246  ip(self.fkeys["F
+0001c4f0: 3130 225d 5b31 5d29 0a20 2020 2020 2020  10"][1]).       
+0001c500: 2069 6620 2246 3131 2220 696e 206b 6579   if "F11" in key
+0001c510: 733a 0a20 2020 2020 2020 2020 2020 2073  s:.            s
+0001c520: 656c 662e 4631 312e 7365 7454 6578 7428  elf.F11.setText(
+0001c530: 6622 4631 313a 207b 7365 6c66 2e66 6b65  f"F11: {self.fke
+0001c540: 7973 5b27 4631 3127 5d5b 305d 7d22 290a  ys['F11'][0]}").
+0001c550: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0001c560: 2e46 3131 2e73 6574 546f 6f6c 5469 7028  .F11.setToolTip(
+0001c570: 7365 6c66 2e66 6b65 7973 5b22 4631 3122  self.fkeys["F11"
+0001c580: 5d5b 315d 290a 2020 2020 2020 2020 6966  ][1]).        if
+0001c590: 2022 4631 3222 2069 6e20 6b65 7973 3a0a   "F12" in keys:.
+0001c5a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0001c5b0: 2e46 3132 2e73 6574 5465 7874 2866 2246  .F12.setText(f"F
+0001c5c0: 3132 3a20 7b73 656c 662e 666b 6579 735b  12: {self.fkeys[
+0001c5d0: 2746 3132 275d 5b30 5d7d 2229 0a20 2020  'F12'][0]}").   
+0001c5e0: 2020 2020 2020 2020 2073 656c 662e 4631           self.F1
+0001c5f0: 322e 7365 7454 6f6f 6c54 6970 2873 656c  2.setToolTip(sel
+0001c600: 662e 666b 6579 735b 2246 3132 225d 5b31  f.fkeys["F12"][1
+0001c610: 5d29 0a0a 2020 2020 6465 6620 6765 6e65  ])..    def gene
+0001c620: 7261 7465 5f61 6469 6628 7365 6c66 2920  rate_adif(self) 
+0001c630: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+0001c640: 2022 2222 0a20 2020 2020 2020 2043 616c   """.        Cal
+0001c650: 6c73 2074 6865 2063 6f6e 7465 7374 2041  ls the contest A
+0001c660: 4449 4620 6669 6c65 2067 656e 6572 6174  DIF file generat
+0001c670: 6f72 2e0a 0a20 2020 2020 2020 2050 6172  or...        Par
+0001c680: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
+0001c690: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
+0001c6a0: 2020 204e 6f6e 650a 0a20 2020 2020 2020     None..       
+0001c6b0: 2052 6574 7572 6e73 0a20 2020 2020 2020   Returns.       
+0001c6c0: 202d 2d2d 2d2d 2d2d 0a20 2020 2020 2020   -------.       
+0001c6d0: 204e 6f6e 650a 2020 2020 2020 2020 2222   None.        ""
+0001c6e0: 220a 0a20 2020 2020 2020 2023 2068 7474  "..        # htt
+0001c6f0: 7073 3a2f 2f77 7777 2e61 6469 662e 6f72  ps://www.adif.or
+0001c700: 672f 3331 352f 4144 4946 5f33 3135 2e68  g/315/ADIF_315.h
+0001c710: 746d 0a20 2020 2020 2020 206c 6f67 6765  tm.        logge
+0001c720: 722e 6465 6275 6728 222a 2a2a 2a2a 2a41  r.debug("******A
+0001c730: 4449 462a 2a2a 2a2a 2229 0a20 2020 2020  DIF*****").     
+0001c740: 2020 2073 656c 662e 636f 6e74 6573 742e     self.contest.
+0001c750: 6164 6966 2873 656c 6629 0a0a 2020 2020  adif(self)..    
+0001c760: 6465 6620 6765 6e65 7261 7465 5f63 6162  def generate_cab
+0001c770: 7269 6c6c 6f28 7365 6c66 2920 2d3e 204e  rillo(self) -> N
+0001c780: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
+0001c790: 0a20 2020 2020 2020 2043 616c 6c73 2074  .        Calls t
+0001c7a0: 6865 2063 6f6e 7465 7374 2043 6162 7269  he contest Cabri
+0001c7b0: 6c6c 6f20 6669 6c65 2067 656e 6572 6174  llo file generat
+0001c7c0: 6f72 2e20 4d61 7962 652e 0a0a 2020 2020  or. Maybe...    
+0001c7d0: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+0001c7e0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+0001c7f0: 2d0a 2020 2020 2020 2020 4e6f 6e65 0a0a  -.        None..
+0001c800: 2020 2020 2020 2020 5265 7475 726e 730a          Returns.
+0001c810: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
+0001c820: 2020 2020 2020 2020 4e6f 6e65 0a20 2020          None.   
+0001c830: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
+0001c840: 2020 6c6f 6767 6572 2e64 6562 7567 2822    logger.debug("
+0001c850: 2a2a 2a2a 2a2a 4361 6272 696c 6c6f 2a2a  ******Cabrillo**
+0001c860: 2a2a 2a22 290a 2020 2020 2020 2020 7365  ***").        se
+0001c870: 6c66 2e63 6f6e 7465 7374 2e63 6162 7269  lf.contest.cabri
+0001c880: 6c6c 6f28 7365 6c66 290a 0a0a 6465 6620  llo(self)...def 
+0001c890: 6c6f 6164 5f66 6f6e 7473 5f66 726f 6d5f  load_fonts_from_
+0001c8a0: 6469 7228 6469 7265 6374 6f72 793a 2073  dir(directory: s
+0001c8b0: 7472 2920 2d3e 2073 6574 3a0a 2020 2020  tr) -> set:.    
+0001c8c0: 2222 220a 2020 2020 5765 6c6c 2069 7420  """.    Well it 
+0001c8d0: 6c6f 6164 7320 666f 6e74 7320 6672 6f6d  loads fonts from
+0001c8e0: 2061 2064 6972 6563 746f 7279 2e2e 2e0a   a directory....
+0001c8f0: 0a20 2020 2050 6172 616d 6574 6572 730a  .    Parameters.
+0001c900: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+0001c910: 2020 2064 6972 6563 746f 7279 203a 2073     directory : s
+0001c920: 7472 0a20 2020 2054 6865 2064 6972 6563  tr.    The direc
+0001c930: 746f 7279 2074 6f20 6c6f 6164 2066 6f6e  tory to load fon
+0001c940: 7473 2066 726f 6d2e 0a0a 2020 2020 5265  ts from...    Re
+0001c950: 7475 726e 730a 2020 2020 2d2d 2d2d 2d2d  turns.    ------
+0001c960: 2d0a 2020 2020 7365 740a 2020 2020 4120  -.    set.    A 
+0001c970: 7365 7420 6f66 2066 6f6e 7420 6661 6d69  set of font fami
+0001c980: 6c69 6573 2069 6e73 7461 6c6c 6564 2069  lies installed i
+0001c990: 6e20 7468 6520 6469 7265 6374 6f72 792e  n the directory.
+0001c9a0: 0a20 2020 2022 2222 0a20 2020 2066 6f6e  .    """.    fon
+0001c9b0: 745f 6661 6d69 6c69 6573 203d 2073 6574  t_families = set
+0001c9c0: 2829 0a20 2020 2066 6f72 205f 6669 2069  ().    for _fi i
+0001c9d0: 6e20 5144 6972 2864 6972 6563 746f 7279  n QDir(directory
+0001c9e0: 292e 656e 7472 7949 6e66 6f4c 6973 7428  ).entryInfoList(
+0001c9f0: 5b22 2a2e 7474 6622 2c20 222a 2e77 6f66  ["*.ttf", "*.wof
+0001ca00: 6622 2c20 222a 2e77 6f66 6632 225d 293a  f", "*.woff2"]):
+0001ca10: 0a20 2020 2020 2020 205f 6964 203d 2051  .        _id = Q
+0001ca20: 466f 6e74 4461 7461 6261 7365 2e61 6464  FontDatabase.add
+0001ca30: 4170 706c 6963 6174 696f 6e46 6f6e 7428  ApplicationFont(
+0001ca40: 5f66 692e 6162 736f 6c75 7465 4669 6c65  _fi.absoluteFile
+0001ca50: 5061 7468 2829 290a 2020 2020 2020 2020  Path()).        
+0001ca60: 666f 6e74 5f66 616d 696c 6965 7320 7c3d  font_families |=
+0001ca70: 2073 6574 2851 466f 6e74 4461 7461 6261   set(QFontDataba
+0001ca80: 7365 2e61 7070 6c69 6361 7469 6f6e 466f  se.applicationFo
+0001ca90: 6e74 4661 6d69 6c69 6573 285f 6964 2929  ntFamilies(_id))
+0001caa0: 0a20 2020 2072 6574 7572 6e20 666f 6e74  .    return font
+0001cab0: 5f66 616d 696c 6965 730a 0a0a 6465 6620  _families...def 
+0001cac0: 696e 7374 616c 6c5f 6963 6f6e 7328 2920  install_icons() 
+0001cad0: 2d3e 204e 6f6e 653a 0a20 2020 2022 2222  -> None:.    """
+0001cae0: 496e 7374 616c 6c20 6963 6f6e 7322 2222  Install icons"""
+0001caf0: 0a0a 2020 2020 6966 2073 7973 2e70 6c61  ..    if sys.pla
+0001cb00: 7466 6f72 6d20 3d3d 2022 6c69 6e75 7822  tform == "linux"
+0001cb10: 3a0a 2020 2020 2020 2020 6f73 2e73 7973  :.        os.sys
+0001cb20: 7465 6d28 0a20 2020 2020 2020 2020 2020  tem(.           
+0001cb30: 2022 7864 672d 6963 6f6e 2d72 6573 6f75   "xdg-icon-resou
+0001cb40: 7263 6520 696e 7374 616c 6c20 2d2d 7369  rce install --si
+0001cb50: 7a65 2033 3220 2d2d 636f 6e74 6578 7420  ze 32 --context 
+0001cb60: 6170 7073 202d 2d6d 6f64 6520 7573 6572  apps --mode user
+0001cb70: 2022 0a20 2020 2020 2020 2020 2020 2066   ".            f
+0001cb80: 227b 6673 7574 696c 732e 4150 505f 4441  "{fsutils.APP_DA
+0001cb90: 5441 5f50 4154 487d 2f6b 3667 7465 2e6e  TA_PATH}/k6gte.n
+0001cba0: 6f74 316d 6d2d 3332 2e70 6e67 206b 3667  ot1mm-32.png k6g
+0001cbb0: 7465 2d6e 6f74 316d 6d22 0a20 2020 2020  te-not1mm".     
+0001cbc0: 2020 2029 0a20 2020 2020 2020 206f 732e     ).        os.
+0001cbd0: 7379 7374 656d 280a 2020 2020 2020 2020  system(.        
+0001cbe0: 2020 2020 2278 6467 2d69 636f 6e2d 7265      "xdg-icon-re
+0001cbf0: 736f 7572 6365 2069 6e73 7461 6c6c 202d  source install -
+0001cc00: 2d73 697a 6520 3634 202d 2d63 6f6e 7465  -size 64 --conte
+0001cc10: 7874 2061 7070 7320 2d2d 6d6f 6465 2075  xt apps --mode u
+0001cc20: 7365 7220 220a 2020 2020 2020 2020 2020  ser ".          
+0001cc30: 2020 6622 7b66 7375 7469 6c73 2e41 5050    f"{fsutils.APP
+0001cc40: 5f44 4154 415f 5041 5448 7d2f 6b36 6774  _DATA_PATH}/k6gt
+0001cc50: 652e 6e6f 7431 6d6d 2d36 342e 706e 6720  e.not1mm-64.png 
+0001cc60: 6b36 6774 652d 6e6f 7431 6d6d 220a 2020  k6gte-not1mm".  
+0001cc70: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0001cc80: 6f73 2e73 7973 7465 6d28 0a20 2020 2020  os.system(.     
+0001cc90: 2020 2020 2020 2022 7864 672d 6963 6f6e         "xdg-icon
+0001cca0: 2d72 6573 6f75 7263 6520 696e 7374 616c  -resource instal
+0001ccb0: 6c20 2d2d 7369 7a65 2031 3238 202d 2d63  l --size 128 --c
+0001ccc0: 6f6e 7465 7874 2061 7070 7320 2d2d 6d6f  ontext apps --mo
+0001ccd0: 6465 2075 7365 7220 220a 2020 2020 2020  de user ".      
+0001cce0: 2020 2020 2020 6622 7b66 7375 7469 6c73        f"{fsutils
+0001ccf0: 2e41 5050 5f44 4154 415f 5041 5448 7d2f  .APP_DATA_PATH}/
+0001cd00: 6b36 6774 652e 6e6f 7431 6d6d 2d31 3238  k6gte.not1mm-128
+0001cd10: 2e70 6e67 206b 3667 7465 2d6e 6f74 316d  .png k6gte-not1m
+0001cd20: 6d22 0a20 2020 2020 2020 2029 0a20 2020  m".        ).   
+0001cd30: 2020 2020 206f 732e 7379 7374 656d 280a       os.system(.
+0001cd40: 2020 2020 2020 2020 2020 2020 6622 7864              f"xd
+0001cd50: 672d 6465 736b 746f 702d 6d65 6e75 2069  g-desktop-menu i
+0001cd60: 6e73 7461 6c6c 207b 6673 7574 696c 732e  nstall {fsutils.
+0001cd70: 4150 505f 4441 5441 5f50 4154 487d 2f6b  APP_DATA_PATH}/k
+0001cd80: 3667 7465 2d6e 6f74 316d 6d2e 6465 736b  6gte-not1mm.desk
+0001cd90: 746f 7022 0a20 2020 2020 2020 2029 0a0a  top".        )..
+0001cda0: 0a64 6566 2064 6f69 6d70 286d 6f64 6e61  .def doimp(modna
+0001cdb0: 6d65 2920 2d3e 206f 626a 6563 743a 0a20  me) -> object:. 
+0001cdc0: 2020 2022 2222 0a20 2020 2049 6d70 6f72     """.    Impor
+0001cdd0: 7473 2061 206d 6f64 756c 652e 0a0a 2020  ts a module...  
+0001cde0: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
+0001cdf0: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
+0001ce00: 6d6f 646e 616d 6520 3a20 7374 720a 2020  modname : str.  
+0001ce10: 2020 5468 6520 6e61 6d65 206f 6620 7468    The name of th
+0001ce20: 6520 6d6f 6475 6c65 2074 6f20 696d 706f  e module to impo
+0001ce30: 7274 2e0a 0a20 2020 2052 6574 7572 6e73  rt...    Returns
+0001ce40: 0a20 2020 202d 2d2d 2d2d 2d2d 0a20 2020  .    -------.   
+0001ce50: 206f 626a 6563 740a 2020 2020 5468 6520   object.    The 
+0001ce60: 6d6f 6475 6c65 206f 626a 6563 742e 0a20  module object.. 
+0001ce70: 2020 2022 2222 0a0a 2020 2020 6c6f 6767     """..    logg
+0001ce80: 6572 2e64 6562 7567 2822 646f 696d 703a  er.debug("doimp:
+0001ce90: 2025 7322 2c20 6d6f 646e 616d 6529 0a20   %s", modname). 
+0001cea0: 2020 2072 6574 7572 6e20 696d 706f 7274     return import
+0001ceb0: 6c69 622e 696d 706f 7274 5f6d 6f64 756c  lib.import_modul
+0001cec0: 6528 6622 6e6f 7431 6d6d 2e70 6c75 6769  e(f"not1mm.plugi
+0001ced0: 6e73 2e7b 6d6f 646e 616d 657d 2229 0a0a  ns.{modname}")..
+0001cee0: 0a64 6566 2072 756e 2829 202d 3e20 4e6f  .def run() -> No
+0001cef0: 6e65 3a0a 2020 2020 2222 220a 2020 2020  ne:.    """.    
+0001cf00: 4d61 696e 2045 6e74 7279 0a20 2020 2022  Main Entry.    "
+0001cf10: 2222 0a20 2020 206c 6f67 6765 722e 6465  "".    logger.de
+0001cf20: 6275 6728 0a20 2020 2020 2020 2066 2252  bug(.        f"R
+0001cf30: 6573 6f6c 7665 6420 4f53 2066 696c 6520  esolved OS file 
+0001cf40: 7379 7374 656d 2070 6174 6873 3a20 4d4f  system paths: MO
+0001cf50: 4455 4c45 5f50 4154 4820 7b66 7375 7469  DULE_PATH {fsuti
+0001cf60: 6c73 2e4d 4f44 554c 455f 5041 5448 7d2c  ls.MODULE_PATH},
+0001cf70: 2055 5345 525f 4441 5441 5f50 4154 4820   USER_DATA_PATH 
+0001cf80: 7b66 7375 7469 6c73 2e55 5345 525f 4441  {fsutils.USER_DA
+0001cf90: 5441 5f50 4154 487d 2c20 434f 4e46 4947  TA_PATH}, CONFIG
+0001cfa0: 5f50 4154 4820 7b66 7375 7469 6c73 2e43  _PATH {fsutils.C
+0001cfb0: 4f4e 4649 475f 5041 5448 7d22 0a20 2020  ONFIG_PATH}".   
+0001cfc0: 2029 0a20 2020 2069 6e73 7461 6c6c 5f69   ).    install_i
+0001cfd0: 636f 6e73 2829 0a20 2020 2074 696d 6572  cons().    timer
+0001cfe0: 2e73 7461 7274 2832 3530 290a 2020 2020  .start(250).    
+0001cff0: 7379 732e 6578 6974 2861 7070 2e65 7865  sys.exit(app.exe
+0001d000: 6328 2929 0a0a 0a44 4542 5547 5f45 4e41  c())...DEBUG_ENA
+0001d010: 424c 4544 203d 2046 616c 7365 0a69 6620  BLED = False.if 
+0001d020: 5061 7468 2822 2e2f 6465 6275 6722 292e  Path("./debug").
+0001d030: 6578 6973 7473 2829 3a0a 2020 2020 4445  exists():.    DE
+0001d040: 4255 475f 454e 4142 4c45 4420 3d20 5472  BUG_ENABLED = Tr
+0001d050: 7565 0a0a 6c6f 6767 6572 203d 206c 6f67  ue..logger = log
+0001d060: 6769 6e67 2e67 6574 4c6f 6767 6572 2822  ging.getLogger("
+0001d070: 5f5f 6d61 696e 5f5f 2229 0a0a 6c6f 6767  __main__")..logg
+0001d080: 696e 672e 6261 7369 6343 6f6e 6669 6728  ing.basicConfig(
+0001d090: 0a20 2020 206c 6576 656c 3d6c 6f67 6769  .    level=loggi
+0001d0a0: 6e67 2e44 4542 5547 2069 6620 4445 4255  ng.DEBUG if DEBU
+0001d0b0: 475f 454e 4142 4c45 4420 656c 7365 206c  G_ENABLED else l
+0001d0c0: 6f67 6769 6e67 2e43 5249 5449 4341 4c2c  ogging.CRITICAL,
+0001d0d0: 0a20 2020 2066 6f72 6d61 743d 225b 2528  .    format="[%(
+0001d0e0: 6173 6374 696d 6529 735d 2025 286c 6576  asctime)s] %(lev
+0001d0f0: 656c 6e61 6d65 2973 2025 286e 616d 6529  elname)s %(name)
+0001d100: 7320 2d20 2528 6675 6e63 4e61 6d65 2973  s - %(funcName)s
+0001d110: 204c 696e 6520 2528 6c69 6e65 6e6f 2964   Line %(lineno)d
+0001d120: 3a20 2528 6d65 7373 6167 6529 7322 2c0a  : %(message)s",.
+0001d130: 2020 2020 6861 6e64 6c65 7273 3d5b 0a20      handlers=[. 
+0001d140: 2020 2020 2020 2052 6f74 6174 696e 6746         RotatingF
+0001d150: 696c 6548 616e 646c 6572 2866 7375 7469  ileHandler(fsuti
+0001d160: 6c73 2e4c 4f47 5f46 494c 452c 206d 6178  ls.LOG_FILE, max
+0001d170: 4279 7465 733d 3130 3439 3030 3030 2c20  Bytes=10490000, 
+0001d180: 6261 636b 7570 436f 756e 743d 3230 292c  backupCount=20),
+0001d190: 0a20 2020 2020 2020 206c 6f67 6769 6e67  .        logging
+0001d1a0: 2e53 7472 6561 6d48 616e 646c 6572 2829  .StreamHandler()
+0001d1b0: 2c0a 2020 2020 5d2c 0a29 0a6c 6f67 6769  ,.    ],.).loggi
+0001d1c0: 6e67 2e67 6574 4c6f 6767 6572 2822 5079  ng.getLogger("Py
+0001d1d0: 5174 352e 7569 632e 7569 7061 7273 6572  Qt5.uic.uiparser
+0001d1e0: 2229 2e73 6574 4c65 7665 6c28 2249 4e46  ").setLevel("INF
+0001d1f0: 4f22 290a 6c6f 6767 696e 672e 6765 744c  O").logging.getL
+0001d200: 6f67 6765 7228 2250 7951 7435 2e75 6963  ogger("PyQt5.uic
+0001d210: 2e70 726f 7065 7274 6965 7322 292e 7365  .properties").se
+0001d220: 744c 6576 656c 2822 494e 464f 2229 0a61  tLevel("INFO").a
+0001d230: 7070 203d 2051 7457 6964 6765 7473 2e51  pp = QtWidgets.Q
+0001d240: 4170 706c 6963 6174 696f 6e28 7379 732e  Application(sys.
+0001d250: 6172 6776 290a 6661 6d69 6c69 6573 203d  argv).families =
+0001d260: 206c 6f61 645f 666f 6e74 735f 6672 6f6d   load_fonts_from
+0001d270: 5f64 6972 286f 732e 6673 7061 7468 2866  _dir(os.fspath(f
+0001d280: 7375 7469 6c73 2e41 5050 5f44 4154 415f  sutils.APP_DATA_
+0001d290: 5041 5448 2929 0a6c 6f67 6765 722e 696e  PATH)).logger.in
+0001d2a0: 666f 2866 2266 6f6e 7420 6661 6d69 6c69  fo(f"font famili
+0001d2b0: 6573 207b 6661 6d69 6c69 6573 7d22 290a  es {families}").
+0001d2c0: 7769 6e64 6f77 203d 204d 6169 6e57 696e  window = MainWin
+0001d2d0: 646f 7728 290a 6865 6967 6874 203d 2077  dow().height = w
+0001d2e0: 696e 646f 772e 7072 6566 2e67 6574 2822  indow.pref.get("
+0001d2f0: 7769 6e64 6f77 5f68 6569 6768 7422 2c20  window_height", 
+0001d300: 3330 3029 0a77 6964 7468 203d 2077 696e  300).width = win
+0001d310: 646f 772e 7072 6566 2e67 6574 2822 7769  dow.pref.get("wi
+0001d320: 6e64 6f77 5f77 6964 7468 222c 2037 3030  ndow_width", 700
+0001d330: 290a 7820 3d20 7769 6e64 6f77 2e70 7265  ).x = window.pre
+0001d340: 662e 6765 7428 2277 696e 646f 775f 7822  f.get("window_x"
+0001d350: 2c20 2d31 290a 7920 3d20 7769 6e64 6f77  , -1).y = window
+0001d360: 2e70 7265 662e 6765 7428 2277 696e 646f  .pref.get("windo
+0001d370: 775f 7922 2c20 2d31 290a 7769 6e64 6f77  w_y", -1).window
+0001d380: 2e73 6574 4765 6f6d 6574 7279 2878 2c20  .setGeometry(x, 
+0001d390: 792c 2077 6964 7468 2c20 6865 6967 6874  y, width, height
+0001d3a0: 290a 7769 6e64 6f77 2e63 616c 6c73 6967  ).window.callsig
+0001d3b0: 6e2e 7365 7446 6f63 7573 2829 0a77 696e  n.setFocus().win
+0001d3c0: 646f 772e 7368 6f77 2829 0a74 696d 6572  dow.show().timer
+0001d3d0: 203d 2051 7443 6f72 652e 5154 696d 6572   = QtCore.QTimer
+0001d3e0: 2829 0a74 696d 6572 2e74 696d 656f 7574  ().timer.timeout
+0001d3f0: 2e63 6f6e 6e65 6374 2877 696e 646f 772e  .connect(window.
+0001d400: 706f 6c6c 5f72 6164 696f 290a 0a69 6620  poll_radio)..if 
+0001d410: 5f5f 6e61 6d65 5f5f 203d 3d20 225f 5f6d  __name__ == "__m
+0001d420: 6169 6e5f 5f22 3a0a 2020 2020 7275 6e28  ain__":.    run(
+0001d430: 290a                                     ).
```

### Comparing `not1mm-24.4.2.1/not1mm/bandmap.py` & `not1mm-24.4.4/not1mm/bandmap.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/checkwindow.py` & `not1mm-24.4.4/not1mm/checkwindow.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/JetBrainsMono-Regular.ttf` & `not1mm-24.4.4/not1mm/data/JetBrainsMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/MASTER.SCP` & `not1mm-24.4.4/not1mm/data/MASTER.SCP`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/about.ui` & `not1mm-24.4.4/not1mm/data/about.ui`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/bandmap.ui` & `not1mm-24.4.4/not1mm/data/bandmap.ui`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/checkwindow.ui` & `not1mm-24.4.4/not1mm/data/checkwindow.ui`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/configuration.ui` & `not1mm-24.4.4/not1mm/data/configuration.ui`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/contests.sql` & `not1mm-24.4.4/not1mm/data/contests.sql`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/cty.json` & `not1mm-24.4.4/not1mm/data/cty.json`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/editcontact.ui` & `not1mm-24.4.4/not1mm/data/editcontact.ui`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/editmacro.ui` & `not1mm-24.4.4/not1mm/data/editmacro.ui`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/k6gte.not1mm-128.png` & `not1mm-24.4.4/not1mm/data/k6gte.not1mm-128.png`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/k6gte.not1mm-32.png` & `not1mm-24.4.4/not1mm/data/k6gte.not1mm-32.png`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/k6gte.not1mm-64.png` & `not1mm-24.4.4/not1mm/data/k6gte.not1mm-64.png`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/logwindow.ui` & `not1mm-24.4.4/not1mm/data/logwindow.ui`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/logwindowx.ui` & `not1mm-24.4.4/not1mm/data/logwindowx.ui`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/main.ui` & `not1mm-24.4.4/not1mm/data/main.ui`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/new_contest.ui` & `not1mm-24.4.4/not1mm/data/new_contest.ui`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/not1mm.html` & `not1mm-24.4.4/not1mm/data/not1mm.html`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/opon.ui` & `not1mm-24.4.4/not1mm/data/opon.ui`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/phonetics/0.wav` & `not1mm-24.4.4/not1mm/data/phonetics/0.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/phonetics/1.wav` & `not1mm-24.4.4/not1mm/data/phonetics/1.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/phonetics/2.wav` & `not1mm-24.4.4/not1mm/data/phonetics/2.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/phonetics/3.wav` & `not1mm-24.4.4/not1mm/data/phonetics/3.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/phonetics/4.wav` & `not1mm-24.4.4/not1mm/data/phonetics/4.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/phonetics/5.wav` & `not1mm-24.4.4/not1mm/data/phonetics/5.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/phonetics/6.wav` & `not1mm-24.4.4/not1mm/data/phonetics/6.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/phonetics/7.wav` & `not1mm-24.4.4/not1mm/data/phonetics/7.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/phonetics/73.wav` & `not1mm-24.4.4/not1mm/data/phonetics/73.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/phonetics/8.wav` & `not1mm-24.4.4/not1mm/data/phonetics/8.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/phonetics/9.wav` & `not1mm-24.4.4/not1mm/data/phonetics/9.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/phonetics/a.wav` & `not1mm-24.4.4/not1mm/data/phonetics/a.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/phonetics/again.wav` & `not1mm-24.4.4/not1mm/data/phonetics/again.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/phonetics/b.wav` & `not1mm-24.4.4/not1mm/data/phonetics/b.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/phonetics/c.wav` & `not1mm-24.4.4/not1mm/data/phonetics/c.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/phonetics/contest.wav` & `not1mm-24.4.4/not1mm/data/phonetics/contest.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/phonetics/cq.wav` & `not1mm-24.4.4/not1mm/data/phonetics/cq.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/phonetics/d.wav` & `not1mm-24.4.4/not1mm/data/phonetics/d.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/phonetics/e.wav` & `not1mm-24.4.4/not1mm/data/phonetics/e.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/phonetics/f.wav` & `not1mm-24.4.4/not1mm/data/phonetics/f.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/phonetics/g.wav` & `not1mm-24.4.4/not1mm/data/phonetics/g.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/phonetics/h.wav` & `not1mm-24.4.4/not1mm/data/phonetics/h.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/phonetics/i.wav` & `not1mm-24.4.4/not1mm/data/phonetics/i.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/phonetics/j.wav` & `not1mm-24.4.4/not1mm/data/phonetics/j.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/phonetics/k.wav` & `not1mm-24.4.4/not1mm/data/phonetics/k.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/phonetics/k6gte.wav` & `not1mm-24.4.4/not1mm/data/phonetics/k6gte.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/phonetics/l.wav` & `not1mm-24.4.4/not1mm/data/phonetics/l.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/phonetics/m.wav` & `not1mm-24.4.4/not1mm/data/phonetics/m.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/phonetics/mynumber.wav` & `not1mm-24.4.4/not1mm/data/phonetics/mynumber.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/phonetics/n.wav` & `not1mm-24.4.4/not1mm/data/phonetics/n.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/phonetics/nil.wav` & `not1mm-24.4.4/not1mm/data/phonetics/nil.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/phonetics/o.wav` & `not1mm-24.4.4/not1mm/data/phonetics/o.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/phonetics/p.wav` & `not1mm-24.4.4/not1mm/data/phonetics/p.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/phonetics/q.wav` & `not1mm-24.4.4/not1mm/data/phonetics/q.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/phonetics/r.wav` & `not1mm-24.4.4/not1mm/data/phonetics/r.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/phonetics/roger.wav` & `not1mm-24.4.4/not1mm/data/phonetics/roger.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/phonetics/s.wav` & `not1mm-24.4.4/not1mm/data/phonetics/s.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/phonetics/space.wav` & `not1mm-24.4.4/not1mm/data/phonetics/space.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/phonetics/t.wav` & `not1mm-24.4.4/not1mm/data/phonetics/t.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/phonetics/thankyou.wav` & `not1mm-24.4.4/not1mm/data/phonetics/thankyou.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/phonetics/thankyouqrz.wav` & `not1mm-24.4.4/not1mm/data/phonetics/thankyouqrz.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/phonetics/u.wav` & `not1mm-24.4.4/not1mm/data/phonetics/u.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/phonetics/v.wav` & `not1mm-24.4.4/not1mm/data/phonetics/v.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/phonetics/w.wav` & `not1mm-24.4.4/not1mm/data/phonetics/w.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/phonetics/x.wav` & `not1mm-24.4.4/not1mm/data/phonetics/x.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/phonetics/y.wav` & `not1mm-24.4.4/not1mm/data/phonetics/y.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/phonetics/yourcall.wav` & `not1mm-24.4.4/not1mm/data/phonetics/yourcall.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/phonetics/z.wav` & `not1mm-24.4.4/not1mm/data/phonetics/z.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/pickcontest.ui` & `not1mm-24.4.4/not1mm/data/pickcontest.ui`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/radio_green.png` & `not1mm-24.4.4/not1mm/data/radio_green.png`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/radio_grey.png` & `not1mm-24.4.4/not1mm/data/radio_grey.png`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/radio_red.png` & `not1mm-24.4.4/not1mm/data/radio_red.png`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/reddot.png` & `not1mm-24.4.4/not1mm/data/reddot.png`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/settings.ui` & `not1mm-24.4.4/not1mm/data/settings.ui`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/data/vfo.ui` & `not1mm-24.4.4/not1mm/data/vfo.ui`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/fsutils.py` & `not1mm-24.4.4/not1mm/fsutils.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/lib/cat_interface.py` & `not1mm-24.4.4/not1mm/lib/cat_interface.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/lib/cwinterface.py` & `not1mm-24.4.4/not1mm/lib/cwinterface.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/lib/database.py` & `not1mm-24.4.4/not1mm/lib/database.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/lib/edit_macro.py` & `not1mm-24.4.4/not1mm/lib/edit_macro.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/lib/edit_station.py` & `not1mm-24.4.4/not1mm/lib/edit_station.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/lib/ham_utility.py` & `not1mm-24.4.4/not1mm/lib/ham_utility.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/lib/lookup.py` & `not1mm-24.4.4/not1mm/lib/lookup.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/lib/multicast.py` & `not1mm-24.4.4/not1mm/lib/multicast.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/lib/n1mm.py` & `not1mm-24.4.4/not1mm/lib/n1mm.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/lib/plugin_common.py` & `not1mm-24.4.4/not1mm/lib/plugin_common.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/lib/settings.py` & `not1mm-24.4.4/not1mm/lib/settings.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/lib/super_check_partial.py` & `not1mm-24.4.4/not1mm/lib/super_check_partial.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/lib/versiontest.py` & `not1mm-24.4.4/not1mm/lib/versiontest.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/logwindow.py` & `not1mm-24.4.4/not1mm/logwindow.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/not1mm/plugins/10_10_fall_cw.py` & `not1mm-24.4.4/not1mm/plugins/10_10_fall_cw.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 from PyQt6 import QtWidgets
 
 from not1mm.lib.plugin_common import gen_adif, get_points
 from not1mm.lib.version import __version__
 
 logger = logging.getLogger(__name__)
 
+EXCHANGE_HINT = "Name + 10-10# + SPC"
+
 name = "10 10 FALL CW"
 cabrillo_name = "10-10-FALL-CW"
 mode = "CW"  # CW SSB BOTH RTTY
 # columns = [0, 1, 2, 3, 4, 5, 6, 15]
 columns = [
     "YYYY-MM-DD HH:MM:SS",
     "Call",
```

### Comparing `not1mm-24.4.2.1/not1mm/plugins/10_10_spring_cw.py` & `not1mm-24.4.4/not1mm/plugins/10_10_spring_cw.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 from PyQt6 import QtWidgets
 from not1mm.lib.plugin_common import gen_adif, get_points
 from not1mm.lib.version import __version__
 
 logger = logging.getLogger(__name__)
 
+EXCHANGE_HINT = "Name + 10-10# + SPC"
+
 name = "10 10 SPRING CW"
 cabrillo_name = "10-10-SPRING-CW"
 mode = "CW"  # CW SSB BOTH RTTY
 # columns = [0, 1, 2, 3, 4, 5, 6, 15]
 columns = [
     "YYYY-MM-DD HH:MM:SS",
     "Call",
```

### Comparing `not1mm-24.4.2.1/not1mm/plugins/10_10_summer_phone.py` & `not1mm-24.4.4/not1mm/plugins/10_10_summer_phone.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from PyQt6 import QtWidgets
 
 from not1mm.lib.plugin_common import gen_adif, get_points
 from not1mm.lib.version import __version__
 
 logger = logging.getLogger(__name__)
 
+EXCHANGE_HINT = "Name + 10-10# + SPC"
+
 name = "10 10 SUMMER PHONE"
 cabrillo_name = "10-10-SUMMER-PHONE"
 mode = "SSB"  # CW SSB BOTH RTTY
 # columns = [0, 1, 2, 3, 4, 5, 6, 15]
 columns = [
     "YYYY-MM-DD HH:MM:SS",
     "Call",
```

### Comparing `not1mm-24.4.2.1/not1mm/plugins/10_10_winter_phone.py` & `not1mm-24.4.4/not1mm/plugins/10_10_winter_phone.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from PyQt6 import QtWidgets
 
 from not1mm.lib.plugin_common import gen_adif, get_points
 from not1mm.lib.version import __version__
 
 logger = logging.getLogger(__name__)
 
+EXCHANGE_HINT = "Name + 10-10# + SPC"
+
 name = "10 10 WINTER PHONE"
 cabrillo_name = "10-10-WINTER-PHONE"
 mode = "SSB"  # CW SSB BOTH RTTY
 # columns = [0, 1, 2, 3, 4, 5, 6, 15]
 columns = [
     "YYYY-MM-DD HH:MM:SS",
     "Call",
```

### Comparing `not1mm-24.4.2.1/not1mm/plugins/arrl_10m.py` & `not1mm-24.4.4/not1mm/plugins/arrl_10m.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,16 @@
 from PyQt6 import QtWidgets
 
 from not1mm.lib.plugin_common import gen_adif, get_points
 from not1mm.lib.version import __version__
 
 logger = logging.getLogger(__name__)
 
+EXCHANGE_HINT = "State/Province"
+
 name = "ARRL 10M"
 mode = "BOTH"  # CW SSB BOTH RTTY
 cabrillo_name = "ARRL-10"
 
 columns = [
     "YYYY-MM-DD HH:MM:SS",
     "Call",
```

### Comparing `not1mm-24.4.2.1/not1mm/plugins/arrl_dx_cw.py` & `not1mm-24.4.4/not1mm/plugins/arrl_dx_cw.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 from PyQt6 import QtWidgets
 
 from not1mm.lib.plugin_common import gen_adif, get_points
 from not1mm.lib.version import __version__
 
 logger = logging.getLogger(__name__)
 
+EXCHANGE_HINT = "State/Province"
+
 name = "ARRL DX CW"
 cabrillo_name = "ARRL-DX-CW"
 mode = "CW"  # CW SSB BOTH RTTY
 # columns = [0, 1, 2, 3, 4, 10, 11, 14, 15]
 columns = [
     "YYYY-MM-DD HH:MM:SS",
     "Call",
```

### Comparing `not1mm-24.4.2.1/not1mm/plugins/arrl_dx_ssb.py` & `not1mm-24.4.4/not1mm/plugins/arrl_dx_ssb.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 from PyQt6 import QtWidgets
 
 from not1mm.lib.plugin_common import gen_adif, get_points
 from not1mm.lib.version import __version__
 
 logger = logging.getLogger(__name__)
 
+EXCHANGE_HINT = "State/Province"
+
 name = "ARRL DX SSB"
 cabrillo_name = "ARRL-DX-SSB"
 mode = "SSB"  # CW SSB BOTH RTTY
 # columns = [0, 1, 2, 3, 4, 10, 11, 14, 15]
 columns = [
     "YYYY-MM-DD HH:MM:SS",
     "Call",
```

### Comparing `not1mm-24.4.2.1/not1mm/plugins/arrl_field_day.py` & `not1mm-24.4.4/not1mm/plugins/arrl_field_day.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 from PyQt6 import QtWidgets
 
 from not1mm.lib.plugin_common import gen_adif, get_points
 from not1mm.lib.version import __version__
 
 logger = logging.getLogger(__name__)
 
+EXCHANGE_HINT = "1D ORG"
+
 name = "ARRL Field Day"
 mode = "BOTH"  # CW SSB BOTH RTTY
 cabrillo_name = "ARRL-FD"
 
 columns = [
     "YYYY-MM-DD HH:MM:SS",
     "Call",
```

### Comparing `not1mm-24.4.2.1/not1mm/plugins/arrl_rtty_ru.py` & `not1mm-24.4.4/not1mm/plugins/arrl_rtty_ru.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 import datetime
 from decimal import Decimal
 from pathlib import Path
 
 from PyQt6 import QtWidgets
 
+EXCHANGE_HINT = ""
+
 name = "ARRL RTTY Round Up"
 cabrillo_name = "ARRL-RTTY"
 mode = "BOTH"  # CW SSB BOTH RTTY
 columns = [
     "YYYY-MM-DD HH:MM:SS",
     "Call",
     "Freq",
```

### Comparing `not1mm-24.4.2.1/not1mm/plugins/arrl_ss_cw.py` & `not1mm-24.4.4/not1mm/plugins/arrl_ss_cw.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from PyQt6 import QtWidgets
 
 from not1mm.lib.plugin_common import gen_adif
 from not1mm.lib.version import __version__
 
 logger = logging.getLogger(__name__)
 
+EXCHANGE_HINT = "Prec Call Check Section"
+
 name = "ARRL Sweepstakes CW"
 cabrillo_name = "ARRL-SS-CW"
 mode = "CW"  # CW SSB BOTH RTTY
 columns = [
     "YYYY-MM-DD HH:MM:SS",
     "Call",
     "Freq",
@@ -377,40 +379,35 @@
     ck = ""
     sec = ""
     call = self.callsign.text()
 
     for tokens in exchange.split():
         text = ""
         numb = ""
-        print(f"'{tokens}'")
         if tokens.isdigit():
-            print(f"{tokens} is digits")
             if sn == "":
                 sn = tokens
             else:
                 ck = tokens
             continue
         elif tokens.isalpha():
-            print(f"{tokens} is alpha")
             if len(tokens) == 1:
                 prec = tokens
             else:
                 sec = tokens
             continue
         elif tokens.isalnum():
-            print("isalnum")
             if tokens[:1].isalpha():
                 print(f"{tokens} is callsign")
                 call = tokens
                 continue
             for i, c in enumerate(tokens):
                 if c.isalpha():
                     text = tokens[i:]
                     numb = tokens[:i]
-                    print(f"{tokens[:i]} {tokens[i:]}")
                     break
             if len(text) == 1:
                 prec = text
                 sn = numb
             else:
                 sec = text
                 ck = numb
```

### Comparing `not1mm-24.4.2.1/not1mm/plugins/arrl_ss_phone.py` & `not1mm-24.4.4/not1mm/plugins/arrl_ss_phone.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from PyQt6 import QtWidgets
 
 from not1mm.lib.plugin_common import gen_adif
 from not1mm.lib.version import __version__
 
 logger = logging.getLogger(__name__)
 
+EXCHANGE_HINT = "Prec Call Check Section"
+
 name = "ARRL Sweepstakes Phone"
 cabrillo_name = "ARRL-SS-SSB"
 mode = "SSB"  # CW SSB BOTH RTTY
 columns = [
     "YYYY-MM-DD HH:MM:SS",
     "Call",
     "Freq",
@@ -379,38 +381,33 @@
     call = self.callsign.text()
 
     for tokens in exchange.split():
         text = ""
         numb = ""
         print(f"'{tokens}'")
         if tokens.isdigit():
-            print(f"{tokens} is digits")
             if sn == "":
                 sn = tokens
             else:
                 ck = tokens
             continue
         elif tokens.isalpha():
-            print(f"{tokens} is alpha")
             if len(tokens) == 1:
                 prec = tokens
             else:
                 sec = tokens
             continue
         elif tokens.isalnum():
-            print("isalnum")
             if tokens[:1].isalpha():
-                print(f"{tokens} is callsign")
                 call = tokens
                 continue
             for i, c in enumerate(tokens):
                 if c.isalpha():
                     text = tokens[i:]
                     numb = tokens[:i]
-                    print(f"{tokens[:i]} {tokens[i:]}")
                     break
             if len(text) == 1:
                 prec = text
                 sn = numb
             else:
                 sec = text
                 ck = numb
```

### Comparing `not1mm-24.4.2.1/not1mm/plugins/arrl_vhf_jan.py` & `not1mm-24.4.4/not1mm/plugins/arrl_vhf_jan.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,14 +44,16 @@
 from PyQt6 import QtWidgets
 
 from not1mm.lib.plugin_common import gen_adif, get_points
 from not1mm.lib.version import __version__
 
 logger = logging.getLogger(__name__)
 
+EXCHANGE_HINT = "4-character grid square"
+
 name = "ARRL VHF JAN"
 mode = "BOTH"  # CW SSB BOTH RTTY
 cabrillo_name = "ARRL-VHF-JAN"
 
 columns = [
     "YYYY-MM-DD HH:MM:SS",
     "Call",
```

### Comparing `not1mm-24.4.2.1/not1mm/plugins/arrl_vhf_jun.py` & `not1mm-24.4.4/not1mm/plugins/arrl_vhf_sep.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-"""ARRL Jun VHF"""
+"""ARRL Sep VHF"""
 
-# Cabrillo name:	ARRL-VHF-JUN
+# Cabrillo name:	ARRL-VHF-SEP
 # Cabrillo name aliases:	ARRL-VHF
 
 # pylint: disable=invalid-name, unused-argument, unused-variable, c-extension-no-member
 
 import datetime
 import logging
 
@@ -12,17 +12,19 @@
 from PyQt6 import QtWidgets
 
 from not1mm.lib.plugin_common import gen_adif, get_points
 from not1mm.lib.version import __version__
 
 logger = logging.getLogger(__name__)
 
-name = "ARRL VHF JUN"
+EXCHANGE_HINT = "4-character grid square"
+
+name = "ARRL VHF SEP"
 mode = "BOTH"  # CW SSB BOTH RTTY
-cabrillo_name = "ARRL-VHF-JUN"
+cabrillo_name = "ARRL-VHF-SEP"
 
 columns = [
     "YYYY-MM-DD HH:MM:SS",
     "Call",
     "Freq",
     "SentNr",
     "RcvNr",
@@ -131,16 +133,16 @@
 
 
 def points(self):
     """Calc point"""
 
     # QSO Points:	1 point per 50 or 144 MHz QSO
     # 2 points per 222 or 432 MHz QSO
-    # 4 points per 902 or 1296 MHz QSO
-    # 8 points per 2.3 GHz or higher QSO
+    # 3 points per 902 or 1296 MHz QSO
+    # 4 points per 2.3 GHz or higher QSO
 
     _band = self.contact.get("Band", "")
     if _band in ["50", "144"]:
         return 1
     if _band in ["222", "432"]:
         return 2
     if _band in ["902", "1296"]:
```

### Comparing `not1mm-24.4.2.1/not1mm/plugins/arrl_vhf_sep.py` & `not1mm-24.4.4/not1mm/plugins/arrl_vhf_jun.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-"""ARRL Sep VHF"""
+"""ARRL Jun VHF"""
 
-# Cabrillo name:	ARRL-VHF-SEP
+# Cabrillo name:	ARRL-VHF-JUN
 # Cabrillo name aliases:	ARRL-VHF
 
 # pylint: disable=invalid-name, unused-argument, unused-variable, c-extension-no-member
 
 import datetime
 import logging
 
@@ -12,17 +12,19 @@
 from PyQt6 import QtWidgets
 
 from not1mm.lib.plugin_common import gen_adif, get_points
 from not1mm.lib.version import __version__
 
 logger = logging.getLogger(__name__)
 
-name = "ARRL VHF SEP"
+EXCHANGE_HINT = "4-character grid square"
+
+name = "ARRL VHF JUN"
 mode = "BOTH"  # CW SSB BOTH RTTY
-cabrillo_name = "ARRL-VHF-SEP"
+cabrillo_name = "ARRL-VHF-JUN"
 
 columns = [
     "YYYY-MM-DD HH:MM:SS",
     "Call",
     "Freq",
     "SentNr",
     "RcvNr",
@@ -131,16 +133,16 @@
 
 
 def points(self):
     """Calc point"""
 
     # QSO Points:	1 point per 50 or 144 MHz QSO
     # 2 points per 222 or 432 MHz QSO
-    # 3 points per 902 or 1296 MHz QSO
-    # 4 points per 2.3 GHz or higher QSO
+    # 4 points per 902 or 1296 MHz QSO
+    # 8 points per 2.3 GHz or higher QSO
 
     _band = self.contact.get("Band", "")
     if _band in ["50", "144"]:
         return 1
     if _band in ["222", "432"]:
         return 2
     if _band in ["902", "1296"]:
```

### Comparing `not1mm-24.4.2.1/not1mm/plugins/canada_day.py` & `not1mm-24.4.4/not1mm/plugins/canada_day.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from PyQt6 import QtWidgets
 
 from not1mm.lib.plugin_common import gen_adif, get_points
 from not1mm.lib.version import __version__
 
 logger = logging.getLogger(__name__)
 
+EXCHANGE_HINT = "Province/Territory"
+
 name = "CANADA DAY"
 cabrillo_name = "CANADA-DAY"
 mode = "BOTH"  # CW SSB BOTH RTTY
 
 columns = [
     "YYYY-MM-DD HH:MM:SS",
     "Call",
```

### Comparing `not1mm-24.4.2.1/not1mm/plugins/cq_160_cw.py` & `not1mm-24.4.4/not1mm/plugins/cq_160_cw.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 from PyQt6 import QtWidgets
 
 from not1mm.lib.plugin_common import gen_adif
 from not1mm.lib.version import __version__
 
 logger = logging.getLogger(__name__)
 
+EXCHANGE_HINT = "ST/Prov or DX CQ Zone"
+
 name = "CQ 160 CW"
 cabrillo_name = "CQ-160-CW"
 mode = "CW"  # CW SSB BOTH RTTY
 
 columns = [
     "YYYY-MM-DD HH:MM:SS",
     "Call",
```

### Comparing `not1mm-24.4.2.1/not1mm/plugins/cq_160_ssb.py` & `not1mm-24.4.4/not1mm/plugins/cq_160_ssb.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 from PyQt6 import QtWidgets
 
 from not1mm.lib.plugin_common import gen_adif
 from not1mm.lib.version import __version__
 
 logger = logging.getLogger(__name__)
 
+EXCHANGE_HINT = "ST/Prov or DX CQ Zone"
+
 name = "CQ 160 SSB"
 cabrillo_name = "CQ-160-SSB"
 mode = "SSB"  # CW SSB BOTH RTTY
 
 columns = [
     "YYYY-MM-DD HH:MM:SS",
     "Call",
```

### Comparing `not1mm-24.4.2.1/not1mm/plugins/cq_wpx_cw.py` & `not1mm-24.4.4/not1mm/plugins/cq_wpx_cw.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from PyQt6 import QtWidgets
 
 from not1mm.lib.plugin_common import gen_adif, get_points
 from not1mm.lib.version import __version__
 
 logger = logging.getLogger(__name__)
 
+EXCHANGE_HINT = "#"
+
 name = "CQ WPX CW"
 cabrillo_name = "CQ-WPX-CW"
 mode = "CW"  # CW SSB BOTH RTTY
 # columns = [0, 1, 2, 3, 4, 5, 6, 9, 11, 15]
 columns = [
     "YYYY-MM-DD HH:MM:SS",
     "Call",
```

### Comparing `not1mm-24.4.2.1/not1mm/plugins/cq_wpx_ssb.py` & `not1mm-24.4.4/not1mm/plugins/cq_wpx_ssb.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from PyQt6 import QtWidgets
 
 from not1mm.lib.plugin_common import gen_adif, get_points
 from not1mm.lib.version import __version__
 
 logger = logging.getLogger(__name__)
 
+EXCHANGE_HINT = "#"
+
 name = "CQ WPX SSB"
 cabrillo_name = "CQ-WPX-SSB"
 mode = "SSB"  # CW SSB BOTH RTTY
 # columns = [0, 1, 2, 3, 4, 5, 6, 9, 11, 15]
 columns = [
     "YYYY-MM-DD HH:MM:SS",
     "Call",
```

### Comparing `not1mm-24.4.2.1/not1mm/plugins/cq_ww_cw.py` & `not1mm-24.4.4/not1mm/plugins/cq_ww_cw.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from PyQt6 import QtWidgets
 
 from not1mm.lib.plugin_common import gen_adif, get_points
 from not1mm.lib.version import __version__
 
 logger = logging.getLogger(__name__)
 
+EXCHANGE_HINT = "CQ Zone No."
+
 name = "CQ WW CW"
 cabrillo_name = "CQ-WW-CW"
 mode = "CW"  # CW SSB BOTH RTTY
 # columns = [0, 1, 2, 3, 4, 5, 6, 15]
 columns = [
     "YYYY-MM-DD HH:MM:SS",
     "Call",
```

### Comparing `not1mm-24.4.2.1/not1mm/plugins/cq_ww_ssb.py` & `not1mm-24.4.4/not1mm/plugins/cq_ww_ssb.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from PyQt6 import QtWidgets
 
 from not1mm.lib.plugin_common import gen_adif, get_points
 from not1mm.lib.version import __version__
 
 logger = logging.getLogger(__name__)
 
+EXCHANGE_HINT = "CQ Zone No."
+
 name = "CQ WW SSB"
 cabrillo_name = "CQ-WW-SSB"
 mode = "SSB"  # CW SSB BOTH RTTY
 # columns = [0, 1, 2, 3, 4, 5, 6, 15]
 columns = [
     "YYYY-MM-DD HH:MM:SS",
     "Call",
```

### Comparing `not1mm-24.4.2.1/not1mm/plugins/cwt.py` & `not1mm-24.4.4/not1mm/plugins/cwt.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 
 from PyQt6 import QtWidgets
 
 from not1mm.lib.plugin_common import gen_adif, get_points
 from not1mm.lib.version import __version__
 
 logger = logging.getLogger(__name__)
+
+EXCHANGE_HINT = "Name + Member No./'CWA'"
+
 name = "CWT"
 mode = "CW"  # CW SSB BOTH RTTY
 # columns = [0, 1, 2, 3, 4, 5, 6, 11, 15]
 columns = [
     "YYYY-MM-DD HH:MM:SS",
     "Call",
     "Freq",
```

### Comparing `not1mm-24.4.2.1/not1mm/plugins/general_logging.py` & `not1mm-24.4.4/not1mm/plugins/general_logging.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from PyQt6 import QtWidgets
 
 from not1mm.lib.plugin_common import gen_adif, get_points
 from not1mm.lib.version import __version__
 
 logger = logging.getLogger(__name__)
-
+EXCHANGE_HINT = ""
 name = "General Logging"
 cabrillo_name = "General-Logging"
 mode = "BOTH"  # CW SSB BOTH RTTY
 columns = [0, 1, 2, 3, 4, 16, 17]
 columns = [
     "YYYY-MM-DD HH:MM:SS",
     "Call",
```

### Comparing `not1mm-24.4.2.1/not1mm/plugins/iaru_hf.py` & `not1mm-24.4.4/not1mm/plugins/iaru_hf.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 from PyQt6 import QtWidgets
 
 from not1mm.lib.plugin_common import gen_adif, get_points
 from not1mm.lib.version import __version__
 
 logger = logging.getLogger(__name__)
 
+EXCHANGE_HINT = "ITU Zone"
+
 name = "IARU HF"
 cabrillo_name = "IARU-HF"
 mode = "BOTH"  # CW SSB BOTH RTTY
 
 columns = [
     "YYYY-MM-DD HH:MM:SS",
     "Call",
```

### Comparing `not1mm-24.4.2.1/not1mm/plugins/jidx_cw.py` & `not1mm-24.4.4/not1mm/plugins/jidx_cw.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from PyQt6 import QtWidgets
 
 from not1mm.lib.plugin_common import gen_adif, get_points
 from not1mm.lib.version import __version__
 
 logger = logging.getLogger(__name__)
 
+EXCHANGE_HINT = "Prefecture or CQ Zone"
+
 name = "JIDX CW"
 cabrillo_name = "JIDX-CW"
 mode = "CW"  # CW SSB BOTH RTTY
 # columns = [0, 1, 2, 3, 4, 5, 6, 11, 15]
 columns = [
     "YYYY-MM-DD HH:MM:SS",
     "Call",
```

### Comparing `not1mm-24.4.2.1/not1mm/plugins/jidx_ph.py` & `not1mm-24.4.4/not1mm/plugins/jidx_ph.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from PyQt6 import QtWidgets
 
 from not1mm.lib.plugin_common import gen_adif, get_points
 from not1mm.lib.version import __version__
 
 logger = logging.getLogger(__name__)
 
+EXCHANGE_HINT = "Prefecture or CQ Zone"
+
 name = "JIDX PH"
 cabrillo_name = "JIDX-PH"
 mode = "SSB"  # CW SSB BOTH RTTY
 # columns = [0, 1, 2, 3, 4, 5, 6, 11, 15]
 columns = [
     "YYYY-MM-DD HH:MM:SS",
     "Call",
```

### Comparing `not1mm-24.4.2.1/not1mm/plugins/naqp_cw.py` & `not1mm-24.4.4/not1mm/plugins/naqp_cw.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 from PyQt6 import QtWidgets
 
 from not1mm.lib.plugin_common import gen_adif, get_points
 from not1mm.lib.version import __version__
 
 logger = logging.getLogger(__name__)
 
+EXCHANGE_HINT = "Name or Name + SPC"
+
 name = "NAQP CW"
 cabrillo_name = "NAQP-CW"
 mode = "CW"  # CW SSB BOTH RTTY
 # columns = [0, 1, 2, 3, 4, 10, 11, 14, 15]
 columns = [
     "YYYY-MM-DD HH:MM:SS",
     "Call",
```

### Comparing `not1mm-24.4.2.1/not1mm/plugins/naqp_ssb.py` & `not1mm-24.4.4/not1mm/plugins/naqp_ssb.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 from PyQt6 import QtWidgets
 
 from not1mm.lib.plugin_common import gen_adif, get_points
 from not1mm.lib.version import __version__
 
 logger = logging.getLogger(__name__)
 
+EXCHANGE_HINT = "Name or Name + SPC"
+
 name = "NAQP SSB"
 cabrillo_name = "NAQP-SSB"
 mode = "SSB"  # CW SSB BOTH RTTY
 # columns = [0, 1, 2, 3, 4, 10, 11, 14, 15]
 columns = [
     "YYYY-MM-DD HH:MM:SS",
     "Call",
```

### Comparing `not1mm-24.4.2.1/not1mm/plugins/phone_weekly_test.py` & `not1mm-24.4.4/not1mm/plugins/phone_weekly_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,16 @@
 from PyQt6 import QtWidgets
 
 from not1mm.lib.plugin_common import gen_adif, get_points
 from not1mm.lib.version import __version__
 
 logger = logging.getLogger(__name__)
 
+EXCHANGE_HINT = "Name or Name + SPC"
+
 name = "PHONE WEEKLY TEST"
 cabrillo_name = "PHONE-WEEKLY-TEST"
 mode = "SSB"  # CW SSB BOTH RTTY
 # columns = [0, 1, 2, 3, 4, 10, 11, 14, 15]
 columns = [
     "YYYY-MM-DD HH:MM:SS",
     "Call",
```

### Comparing `not1mm-24.4.2.1/not1mm/plugins/stew_perry_topband.py` & `not1mm-24.4.4/not1mm/plugins/stew_perry_topband.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 from PyQt6 import QtWidgets
 from not1mm.lib.plugin_common import gen_adif, get_points
 from not1mm.lib.version import __version__
 from not1mm.lib.ham_utility import distance
 
 logger = logging.getLogger(__name__)
 
+EXCHANGE_HINT = "4-Character grid square"
 cabrillo_name = "STEW-PERRY"
 name = "Stew Perry Topband"
 
 mode = "CW"  # CW SSB BOTH RTTY
 
 columns = [
     "YYYY-MM-DD HH:MM:SS",
```

### Comparing `not1mm-24.4.2.1/not1mm/plugins/winter_field_day.py` & `not1mm-24.4.4/not1mm/plugins/winter_field_day.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from pathlib import Path
 from PyQt6 import QtWidgets
 from not1mm.lib.plugin_common import gen_adif, get_points
 from not1mm.lib.version import __version__
 
 logger = logging.getLogger(__name__)
 
+EXCHANGE_HINT = "1O ORG"
+
 cabrillo_name = "WFD"
 name = "Winter Field Day"
 # 1 once per contest, 2 work each band, 3 each band/mode, 4 no dupe checking
 mode = "BOTH"  # CW SSB BOTH RTTY
 columns = [
     "YYYY-MM-DD HH:MM:SS",
     "Call",
```

### Comparing `not1mm-24.4.2.1/not1mm/vfo.py` & `not1mm-24.4.4/not1mm/vfo.py`

 * *Files 0% similar despite different names*

```diff
@@ -324,13 +324,14 @@
         # app.processEvents()
 
     def show_message_box(self, message: str) -> None:
         """
         Display an alert box with the supplied message.
         """
         message_box = QtWidgets.QMessageBox()
-        message_box.setPalette(self.current_palette)
+        if self.current_palette:
+            message_box.setPalette(self.current_palette)
         message_box.setIcon(QtWidgets.QMessageBox.Icon.Information)
         message_box.setText(message)
         message_box.setWindowTitle("Information")
         message_box.setStandardButtons(QtWidgets.QMessageBox.StandardButton.Ok)
         _ = message_box.exec()
```

### Comparing `not1mm-24.4.2.1/not1mm.egg-info/PKG-INFO` & `not1mm-24.4.4/not1mm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: not1mm
-Version: 24.4.2.1
+Version: 24.4.4
 Summary: NOT1MM Logger
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/not1mm
 Project-URL: Bug Tracker, https://github.com/mbridak/not1mm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -173,14 +173,15 @@
 - Phone Weekly Test
 - RAC Canada Day
 - Stew Perry Topband
 - Winter Field Day
 
 ## Recent Changes
 
+- [24-4-4] Added per-contest echange hint when adding new contest.
 - [24-4-2] Migrated to PyQt6. I'm sure there are broken things.
 - [24-4-1-2] Added color text indicators to the Check Partial window. Poached the code from @kyleboyle. Thanks! Fixed the Log, VFO and Check Partial windows to be actual docking widgets. Refocus call field after double clicking on item in the check partial window.
 - [24-4-1] Removed some un-needed loops and widgets from the check window. Fixed docking to the left side.
 
 See [CHANGELOG.md](CHANGELOG.md) for prior changes.
 
 ## Flatpak
```

### Comparing `not1mm-24.4.2.1/not1mm.egg-info/SOURCES.txt` & `not1mm-24.4.4/not1mm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.2.1/pyproject.toml` & `not1mm-24.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "not1mm" 
-version = "24.4.2.1"
+version = "24.4.4"
 description = "NOT1MM Logger"
 readme = "README.md"
 requires-python = ">=3.9"
 authors = [
   { name="Michael Bridak", email="michael.bridak@gmail.com" },
 ]
 dependencies = [
```

