# Comparing `tmp/ganga-8.7.4.tar.gz` & `tmp/ganga-8.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ganga-8.7.4.tar", last modified: Tue Mar 19 20:21:33 2024, max compression
+gzip compressed data, was "ganga-8.7.5.tar", last modified: Fri Apr  5 11:20:57 2024, max compression
```

## Comparing `ganga-8.7.4.tar` & `ganga-8.7.5.tar`

### file list

```diff
@@ -1,991 +1,991 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.067903 ganga-8.7.4/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-19 20:21:22.000000 ganga-8.7.4/LICENSE_GPL
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-03-19 20:21:22.000000 ganga-8.7.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-03-19 20:21:33.067903 ganga-8.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-03-19 20:21:22.000000 ganga-8.7.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:32.915904 ganga-8.7.4/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3667 2024-03-19 20:21:22.000000 ganga-8.7.4/bin/ganga
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:32.915904 ganga-8.7.4/doc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:32.915904 ganga-8.7.4/doc/API/
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/API/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:32.915904 ganga-8.7.4/doc/GPI/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/GPI/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7818 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:32.919904 ganga-8.7.4/doc/UserGuide/
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/UserGuide/Configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/UserGuide/GoogleOauth.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6683 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/UserGuide/InputAndOutputData.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8173 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/UserGuide/InstallAndBasicUsage.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5383 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/UserGuide/JobManipulation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/UserGuide/MiscellaneousFunctionality.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10662 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/UserGuide/PostProcessors.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/UserGuide/Queues.rst
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/UserGuide/RunningExecutables.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5973 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/UserGuide/Splitters.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/UserGuide/Tasks.rst
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/UserGuide/TutorialPlugin.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/UserGuide/UsingDifferentApplications.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/UserGuide/UsingDifferentBackends.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7927 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/UserGuide/Virtualization.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/UserGuide/WhatIsGanga.rst
--rw-r--r--   0 runner    (1001) docker     (127)   587157 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/UserGuide/first_job.gif
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/UserGuide/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    65215 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/UserGuide/start_terminal.gif
--rw-r--r--   0 runner    (1001) docker     (127)   515269 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/UserGuide/virtualization.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:32.923904 ganga-8.7.4/doc/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     7406 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)    20408 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/_static/logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     9971 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:32.923904 ganga-8.7.4/doc/dev/
--rw-r--r--   0 runner    (1001) docker     (127)     5643 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/dev/credentials.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9109 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/dev/index.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     7656 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/fill_gpi.py
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:32.895904 ganga-8.7.4/doc/journal/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:32.947904 ganga-8.7.4/doc/journal/CPC2007/
--rwxr-xr-x   0 runner    (1001) docker     (127)    55839 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/journal/CPC2007/GangaJob.pdf
--rwxr-xr-x   0 runner    (1001) docker     (127)   310914 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/journal/CPC2007/GangaOverview.pdf
--rwxr-xr-x   0 runner    (1001) docker     (127)   121579 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/journal/CPC2007/GangaPlugin.pdf
--rwxr-xr-x   0 runner    (1001) docker     (127)     1000 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/journal/CPC2007/README
--rwxr-xr-x   0 runner    (1001) docker     (127)   189776 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/journal/CPC2007/avianflu.pdf
--rwxr-xr-x   0 runner    (1001) docker     (127)   255272 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/journal/CPC2007/avianflu.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     7896 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/journal/CPC2007/camtology.tex
--rw-r--r--   0 runner    (1001) docker     (127)  5151013 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/journal/CPC2007/camtologyfigure.eps
--rwxr-xr-x   0 runner    (1001) docker     (127)   588084 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/journal/CPC2007/camtologyfigure.pdf
--rwxr-xr-x   0 runner    (1001) docker     (127)   106103 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/journal/CPC2007/camtologytech.pdf
--rwxr-xr-x   0 runner    (1001) docker     (127)    54997 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/journal/CPC2007/elsart.cls
--rwxr-xr-x   0 runner    (1001) docker     (127)    13301 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/journal/CPC2007/elsart1p.cls
--rwxr-xr-x   0 runner    (1001) docker     (127)    13505 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/journal/CPC2007/elsart3p.cls
--rwxr-xr-x   0 runner    (1001) docker     (127)    13426 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/journal/CPC2007/elsart5p.cls
--rw-r--r--   0 runner    (1001) docker     (127)  7395300 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/journal/CPC2007/ganga-GUI.eps
--rw-r--r--   0 runner    (1001) docker     (127)   127751 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/journal/CPC2007/ganga-GUI.png
--rw-r--r--   0 runner    (1001) docker     (127)   102543 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/journal/CPC2007/ganga-architecture.png
--rw-r--r--   0 runner    (1001) docker     (127)    56388 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/journal/CPC2007/ganga-architecture.svg
--rwxr-xr-x   0 runner    (1001) docker     (127)    98876 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/journal/CPC2007/ganga-diane-portal.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    87966 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/journal/CPC2007/ganga-diane-portal.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    31356 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/journal/CPC2007/ganga-diane-portal.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/journal/CPC2007/ganga-objects.dia
--rw-r--r--   0 runner    (1001) docker     (127)    66244 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/journal/CPC2007/ganga-objects.eps
--rw-r--r--   0 runner    (1001) docker     (127)    31406 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/journal/CPC2007/ganga-objects.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    75987 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/journal/CPC2007/ganga.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)    26228 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/journal/CPC2007/instructions-num.tex
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/journal/CPC2007/job-uml.dia
--rw-r--r--   0 runner    (1001) docker     (127)    18329 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/journal/CPC2007/job-uml.eps
--rw-r--r--   0 runner    (1001) docker     (127)    21022 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/journal/CPC2007/job-uml.png
--rw-r--r--   0 runner    (1001) docker     (127)   372567 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/journal/CPC2007/monitoring.eps
--rw-r--r--   0 runner    (1001) docker     (127)   116572 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/journal/CPC2007/monitoring.png
--rwxr-xr-x   0 runner    (1001) docker     (127)   136823 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/journal/CPC2007/monitoring.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:32.947904 ganga-8.7.4/doc/manuals/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1856 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:32.947904 ganga-8.7.4/doc/manuals/html/
--rwxr-xr-x   0 runner    (1001) docker     (127)      944 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/html/about.dat
--rwxr-xr-x   0 runner    (1001) docker     (127)     3409 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/html/about.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:32.947904 ganga-8.7.4/doc/manuals/html/icons/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1958 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/html/icons/blank.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)     1031 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/html/icons/blank.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      438 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/html/icons/contents.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      649 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/html/icons/contents.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      289 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/html/icons/index.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      529 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/html/icons/index.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      385 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/html/icons/modules.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      598 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/html/icons/modules.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      253 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/html/icons/next.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      511 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/html/icons/next.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      252 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/html/icons/previous.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      511 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/html/icons/previous.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      125 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/html/icons/pyfav.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      316 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/html/icons/up.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      577 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/html/icons/up.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     4443 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/html/index.html.in
--rwxr-xr-x   0 runner    (1001) docker     (127)     1324 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/html/stdabout.dat
--rwxr-xr-x   0 runner    (1001) docker     (127)     6041 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/html/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:32.951904 ganga-8.7.4/doc/manuals/perl/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2513 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/perl/SynopsisTable.pm
--rwxr-xr-x   0 runner    (1001) docker     (127)      405 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/perl/distutils.perl
--rwxr-xr-x   0 runner    (1001) docker     (127)      242 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/perl/howto.perl
--rwxr-xr-x   0 runner    (1001) docker     (127)      162 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/perl/isilo.perl
--rwxr-xr-x   0 runner    (1001) docker     (127)    24053 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/perl/l2hinit.perl
--rwxr-xr-x   0 runner    (1001) docker     (127)     1921 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/perl/ltxmarkup.perl
--rwxr-xr-x   0 runner    (1001) docker     (127)      465 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/perl/manual.perl
--rwxr-xr-x   0 runner    (1001) docker     (127)    62754 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/perl/python.perl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:32.951904 ganga-8.7.4/doc/manuals/script/
--rwxr-xr-x   0 runner    (1001) docker     (127)      279 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/script/fiximgpath.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1789 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/script/make-doc.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      469 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/script/makeincl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:32.895904 ganga-8.7.4/doc/manuals/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:32.951904 ganga-8.7.4/doc/manuals/src/DocMaker/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3935 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/DocMaker/DocMaker.tex
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:32.963904 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2239 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/Back.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     2410 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/Copy.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     2492 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/Delete.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     2147 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/Download.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     1847 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/Folder_AddDocument.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     1710 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/Folder_Generic.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     2000 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/Folder_New.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     2258 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/Folder_Remove.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     2297 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/Folder_RemoveDocument.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     2037 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/Folder_Rename.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     2241 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/Forward.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    23577 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/GUI_User_Manual.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     2490 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/General_Options.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     2509 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/Go.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     2504 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/Properties.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     2433 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/Refresh.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     2251 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/Save.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     4504 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/SaveAs_Template.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     1959 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/Search.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     2225 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/Stop.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     1210 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/ToolBtn_Kill.jpg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1328 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/ToolBtn_NewJob.jpg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1397 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/ToolBtn_Remove.jpg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1251 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/ToolBtn_Save.jpg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1328 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/ToolBtn_Submit.jpg
--rwxr-xr-x   0 runner    (1001) docker     (127)     2452 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/View_Doc.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     2583 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/Write.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     1007 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/browse.jpg
--rwxr-xr-x   0 runner    (1001) docker     (127)      948 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/files_16x16.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     1479 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/files_24x24.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      987 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/files_text_16x16.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     1701 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/files_text_24x24.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     1333 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/folder_24x24.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     1891 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/folder_32x32.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     1563 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/folder_down_24x24.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     2322 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/folder_down_32x32.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      956 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/gangagui-manual-chapter_1.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     3183 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/gangagui-manual-chapter_2.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)    10990 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/gangagui-manual-chapter_3.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     3829 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/gangagui-manual-chapter_4.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     3964 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/gangagui-manual-chapter_5.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)       29 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/gangagui-manual-chapter_6.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     2656 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/gangagui-manual-contents.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)   120641 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/gangagui_default-view_typical.jpg
--rwxr-xr-x   0 runner    (1001) docker     (127)     7028 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/genericjob_pic_1.jpg
--rwxr-xr-x   0 runner    (1001) docker     (127)    10096 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/genericjob_pic_2.jpg
--rwxr-xr-x   0 runner    (1001) docker     (127)    22429 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/genericjob_pic_3.jpg
--rwxr-xr-x   0 runner    (1001) docker     (127)    31848 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/genericjob_pic_4.jpg
--rwxr-xr-x   0 runner    (1001) docker     (127)    37895 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/guiconfig_pic_1.jpg
--rwxr-xr-x   0 runner    (1001) docker     (127)    10919 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/guiconfig_pic_2.jpg
--rwxr-xr-x   0 runner    (1001) docker     (127)     4417 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/guiconfig_pic_3.jpg
--rwxr-xr-x   0 runner    (1001) docker     (127)    25440 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/guiconfig_pic_4.jpg
--rwxr-xr-x   0 runner    (1001) docker     (127)     2776 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/help.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    23577 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/index.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)    41244 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/jobbuilder_pic_1.jpg
--rwxr-xr-x   0 runner    (1001) docker     (127)     5020 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/jobbuilder_pic_2.jpg
--rwxr-xr-x   0 runner    (1001) docker     (127)    11470 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/jobbuilder_pic_3.jpg
--rwxr-xr-x   0 runner    (1001) docker     (127)    11606 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/jobbuilder_pic_4.jpg
--rwxr-xr-x   0 runner    (1001) docker     (127)     9174 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/jobbuilder_pic_5.jpg
--rwxr-xr-x   0 runner    (1001) docker     (127)    24152 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/menubar_pic_1.jpg
--rwxr-xr-x   0 runner    (1001) docker     (127)     7218 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/menubar_pic_2.jpg
--rwxr-xr-x   0 runner    (1001) docker     (127)     9076 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/menubar_pic_3.jpg
--rwxr-xr-x   0 runner    (1001) docker     (127)    48083 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/monitoring_pic_1.jpg
--rwxr-xr-x   0 runner    (1001) docker     (127)    26786 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/monitoring_pic_2.jpg
--rwxr-xr-x   0 runner    (1001) docker     (127)    13686 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/monitoring_pic_3.jpg
--rwxr-xr-x   0 runner    (1001) docker     (127)     2140 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/monitoring_pic_4.jpg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1153 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/open.jpg
--rwxr-xr-x   0 runner    (1001) docker     (127)      993 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/preview.jpg
--rwxr-xr-x   0 runner    (1001) docker     (127)    62349 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/quickstart_pic_1.jpg
--rwxr-xr-x   0 runner    (1001) docker     (127)    33800 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/quickstart_pic_2.jpg
--rwxr-xr-x   0 runner    (1001) docker     (127)    17676 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/quickstart_pic_3.jpg
--rwxr-xr-x   0 runner    (1001) docker     (127)    29133 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/quickstart_pic_4.jpg
--rwxr-xr-x   0 runner    (1001) docker     (127)    26485 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/quickstart_pic_5.jpg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1254 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/retrieve.jpg
--rwxr-xr-x   0 runner    (1001) docker     (127)    54473 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/scriptor_pic_1.jpg
--rwxr-xr-x   0 runner    (1001) docker     (127)    46152 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/splitter_pic_1.jpg
--rwxr-xr-x   0 runner    (1001) docker     (127)    70724 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/splitter_pic_2.jpg
--rwxr-xr-x   0 runner    (1001) docker     (127)    27847 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GUI_User_Manual/toolbar.jpg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:32.963904 ganga-8.7.4/doc/manuals/src/GangaIntroduction/
--rwxr-xr-x   0 runner    (1001) docker     (127)    87638 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/GangaIntroduction/GangaIntroduction.tex
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:32.963904 ganga-8.7.4/doc/manuals/src/LHCb/
--rwxr-xr-x   0 runner    (1001) docker     (127)    31025 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/LHCb/LHCb.tex
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:32.963904 ganga-8.7.4/doc/manuals/src/dev_survival/
--rwxr-xr-x   0 runner    (1001) docker     (127)    11822 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/dev_survival/dev_survival.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)     1662 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/dev_survival/makegraph.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10107 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/dev_survival/transient-states.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)    11362 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/dev_survival/user-states.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:32.963904 ganga-8.7.4/doc/manuals/src/workbook/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:32.967904 ganga-8.7.4/doc/manuals/src/workbook/development/
--rwxr-xr-x   0 runner    (1001) docker     (127)       53 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/workbook/development/architecture.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)       63 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/workbook/development/cvs.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)       51 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/workbook/development/dashboard.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)       61 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/workbook/development/developer.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)      574 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/workbook/development/development.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)       53 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/workbook/development/documentation.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)       77 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/workbook/development/panels.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)       46 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/workbook/development/release.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)       59 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/workbook/development/submission.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)       40 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/workbook/development/test.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)       38 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/workbook/development/twiki.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)       68 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/workbook/development/webpages.tex
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:32.967904 ganga-8.7.4/doc/manuals/src/workbook/extension/
--rwxr-xr-x   0 runner    (1001) docker     (127)       54 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/workbook/extension/application.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)       45 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/workbook/extension/backend.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)       74 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/workbook/extension/connector.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)       45 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/workbook/extension/dataset.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)      442 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/workbook/extension/extension.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)       44 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/workbook/extension/logging.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)       43 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/workbook/extension/merger.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)       66 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/workbook/extension/parameters.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)       41 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/workbook/extension/plugins.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)       47 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/workbook/extension/splitter.tex
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:32.967904 ganga-8.7.4/doc/manuals/src/workbook/installation/
--rwxr-xr-x   0 runner    (1001) docker     (127)       51 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/workbook/installation/afs.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)      185 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/workbook/installation/installation.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)       45 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/workbook/installation/local.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)       44 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/workbook/installation/site.tex
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:32.967904 ganga-8.7.4/doc/manuals/src/workbook/introduction/
--rwxr-xr-x   0 runner    (1001) docker     (127)       59 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/workbook/introduction/functionality.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)      375 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/workbook/introduction/introduction.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)       37 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/workbook/introduction/license.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)       39 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/workbook/introduction/mail.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)       37 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/workbook/introduction/website.tex
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:32.971904 ganga-8.7.4/doc/manuals/src/workbook/usage/
--rwxr-xr-x   0 runner    (1001) docker     (127)       68 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/workbook/usage/bugs.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)       62 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/workbook/usage/configuration.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)       54 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/workbook/usage/credentials.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)       88 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/workbook/usage/gpi.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)       59 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/workbook/usage/gui.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)       40 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/workbook/usage/help.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)       38 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/workbook/usage/jobs.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)       36 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/workbook/usage/model.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)       48 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/workbook/usage/monitoring.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)       54 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/workbook/usage/operations.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)       46 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/workbook/usage/repository.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)       49 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/workbook/usage/scripts.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)       44 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/workbook/usage/startup.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)       74 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/workbook/usage/statistics.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)      628 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/workbook/usage/usage.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)       44 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/workbook/usage/workspace.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)     1004 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/src/workbook/workbook.tex
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:32.971904 ganga-8.7.4/doc/manuals/texinputs/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1331 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/texinputs/distutils.sty
--rwxr-xr-x   0 runner    (1001) docker     (127)    14699 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/texinputs/fancyhdr.sty
--rwxr-xr-x   0 runner    (1001) docker     (127)    10359 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/texinputs/fncychap.sty
--rwxr-xr-x   0 runner    (1001) docker     (127)     2797 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/texinputs/howto.cls
--rwxr-xr-x   0 runner    (1001) docker     (127)     1225 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/texinputs/ltxmarkup.sty
--rwxr-xr-x   0 runner    (1001) docker     (127)     4440 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/texinputs/manual.cls
--rwxr-xr-x   0 runner    (1001) docker     (127)      597 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/texinputs/pypaper.sty
--rwxr-xr-x   0 runner    (1001) docker     (127)      220 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/texinputs/python.ist
--rwxr-xr-x   0 runner    (1001) docker     (127)    40097 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/texinputs/python.sty
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:32.979904 ganga-8.7.4/doc/manuals/tools/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2182 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/tools/anno-api.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10526 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/tools/buildindex.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4233 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/tools/checkargs.pm
--rwxr-xr-x   0 runner    (1001) docker     (127)      661 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/tools/cklatex
--rwxr-xr-x   0 runner    (1001) docker     (127)     2154 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/tools/custlib.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2434 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/tools/cvsinfo.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4029 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/tools/findacks
--rwxr-xr-x   0 runner    (1001) docker     (127)     3660 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/tools/findcsyms
--rwxr-xr-x   0 runner    (1001) docker     (127)     1806 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/tools/findmodrefs
--rwxr-xr-x   0 runner    (1001) docker     (127)     3937 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/tools/findsyms
--rwxr-xr-x   0 runner    (1001) docker     (127)       86 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/tools/fix_hack
--rwxr-xr-x   0 runner    (1001) docker     (127)      107 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/tools/fix_libaux.sed
--rwxr-xr-x   0 runner    (1001) docker     (127)      441 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/tools/fixinfo.el
--rwxr-xr-x   0 runner    (1001) docker     (127)     2900 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/tools/getpagecounts
--rwxr-xr-x   0 runner    (1001) docker     (127)     1847 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/tools/getversioninfo
--rwxr-xr-x   0 runner    (1001) docker     (127)    58169 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/tools/html2texi.pl
--rwxr-xr-x   0 runner    (1001) docker     (127)     2301 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/tools/indfix.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      365 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/tools/keywords.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5283 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/tools/listmodules
--rwxr-xr-x   0 runner    (1001) docker     (127)     3438 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/tools/makesec.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     1739 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/tools/mkackshtml
--rwxr-xr-x   0 runner    (1001) docker     (127)    24033 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/tools/mkhowto
--rwxr-xr-x   0 runner    (1001) docker     (127)     1552 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/tools/mkinfo
--rwxr-xr-x   0 runner    (1001) docker     (127)     4819 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/tools/mkmodindex
--rwxr-xr-x   0 runner    (1001) docker     (127)     2338 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/tools/mkpkglist
--rwxr-xr-x   0 runner    (1001) docker     (127)     5884 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/tools/mksourcepkg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1944 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/tools/node2label.pl
--rwxr-xr-x   0 runner    (1001) docker     (127)    15832 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/tools/prechm.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1987 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/tools/push-docs.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)    31256 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/tools/py2texi.el
--rwxr-xr-x   0 runner    (1001) docker     (127)   786944 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/tools/python
--rwxr-xr-x   0 runner    (1001) docker     (127)     2316 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/tools/refcounts.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1366 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/tools/rewrite.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:32.983904 ganga-8.7.4/doc/manuals/tools/sgmlconv/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1298 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/tools/sgmlconv/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (127)     2387 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/tools/sgmlconv/README
--rwxr-xr-x   0 runner    (1001) docker     (127)    23495 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/tools/sgmlconv/conversion.xml
--rwxr-xr-x   0 runner    (1001) docker     (127)    37241 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/tools/sgmlconv/docfixer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7269 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/tools/sgmlconv/esis2sgml.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9228 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/tools/sgmlconv/esistools.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    19936 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/tools/sgmlconv/latex2esis.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1098 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/tools/sgmlconv/make.rules
--rwxr-xr-x   0 runner    (1001) docker     (127)     6704 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/tools/support.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3949 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/tools/toc2bkm.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2528 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/tools/undoc_symbols.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      713 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/tools/update-docs.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)       85 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/manuals/tools/whichlibs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:32.983904 ganga-8.7.4/doc/sysadmin/
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/sysadmin/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:32.983904 ganga-8.7.4/doc/work/
--rwxr-xr-x   0 runner    (1001) docker     (127)     5697 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/work/lifetime.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     6855 2024-03-19 20:21:22.000000 ganga-8.7.4/doc/work/splitting.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:32.983904 ganga-8.7.4/ganga/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:32.983904 ganga-8.7.4/ganga/GangaCore/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:32.983904 ganga-8.7.4/ganga/GangaCore/Core/
--rwxr-xr-x   0 runner    (1001) docker     (127)    10903 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Core/FileWorkspace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:32.987904 ganga-8.7.4/ganga/GangaCore/Core/GangaRepository/
--rw-r--r--   0 runner    (1001) docker     (127)    12780 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Core/GangaRepository/DStreamer.py
--rw-r--r--   0 runner    (1001) docker     (127)    25943 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Core/GangaRepository/DatabaseRegistry.py
--rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Core/GangaRepository/FixedLock.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11096 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Core/GangaRepository/GangaRepository.py
--rw-r--r--   0 runner    (1001) docker     (127)     9354 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Core/GangaRepository/GangaRepositoryCentral.py
--rw-r--r--   0 runner    (1001) docker     (127)    36640 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Core/GangaRepository/GangaRepositoryDatabase.py
--rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Core/GangaRepository/GangaRepositoryImmutableTransient.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    54032 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Core/GangaRepository/GangaRepositoryXML.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Core/GangaRepository/PickleStreamer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    27240 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Core/GangaRepository/Registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    35399 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Core/GangaRepository/SessionLock.py
--rw-r--r--   0 runner    (1001) docker     (127)    19363 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Core/GangaRepository/SubJobJsonList.py
--rw-r--r--   0 runner    (1001) docker     (127)    26908 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Core/GangaRepository/SubJobXMLList.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    17812 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Core/GangaRepository/VStreamer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1146 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Core/GangaRepository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21734 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Core/GangaRepository/container_controllers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Core/GangaRepository/migrate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:32.987904 ganga-8.7.4/ganga/GangaCore/Core/GangaThread/
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Core/GangaThread/GangaThread.py
--rw-r--r--   0 runner    (1001) docker     (127)    11080 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Core/GangaThread/GangaThreadPool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:32.987904 ganga-8.7.4/ganga/GangaCore/Core/GangaThread/MTRunner/
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Core/GangaThread/MTRunner/Algorithm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Core/GangaThread/MTRunner/Data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5549 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Core/GangaThread/MTRunner/MTRunner.py
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Core/GangaThread/MTRunner/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:32.987904 ganga-8.7.4/ganga/GangaCore/Core/GangaThread/WorkerThreads/
--rw-r--r--   0 runner    (1001) docker     (127)    16573 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Core/GangaThread/WorkerThreads/ThreadPoolQueueMonitor.py
--rw-r--r--   0 runner    (1001) docker     (127)    12615 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Core/GangaThread/WorkerThreads/WorkerThreadPool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Core/GangaThread/WorkerThreads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Core/GangaThread/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:32.987904 ganga-8.7.4/ganga/GangaCore/Core/InternalServices/
--rwxr-xr-x   0 runner    (1001) docker     (127)     9171 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Core/InternalServices/Coordinator.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5638 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Core/InternalServices/ShutdownManager.py
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Core/InternalServices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:32.987904 ganga-8.7.4/ganga/GangaCore/Core/MonitoringComponent/
--rwxr-xr-x   0 runner    (1001) docker     (127)    54951 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Core/MonitoringComponent/Local_GangaMC_Service.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4521 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Core/MonitoringComponent/Monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     9425 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Core/MonitoringComponent/MonitoringService.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       28 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Core/MonitoringComponent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:32.991904 ganga-8.7.4/ganga/GangaCore/Core/Sandbox/
--rwxr-xr-x   0 runner    (1001) docker     (127)     5281 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Core/Sandbox/Sandbox.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4265 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Core/Sandbox/WNSandbox.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      281 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Core/Sandbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Core/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6146 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Core/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:32.991904 ganga-8.7.4/ganga/GangaCore/GPI/
--rwxr-xr-x   0 runner    (1001) docker     (127)       28 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPI/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:32.991904 ganga-8.7.4/ganga/GangaCore/GPIDev/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:32.991904 ganga-8.7.4/ganga/GangaCore/GPIDev/Adapters/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1872 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Adapters/ApplicationRuntimeHandlers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5528 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Adapters/IApplication.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    21380 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Adapters/IBackend.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3412 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Adapters/IChecker.py
--rw-r--r--   0 runner    (1001) docker     (127)     9536 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Adapters/ICredentialInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Adapters/ICredentialRequirement.py
--rw-r--r--   0 runner    (1001) docker     (127)     9973 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Adapters/IGangaFile.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9100 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Adapters/IMerger.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3918 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Adapters/IMonitoringService.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6228 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Adapters/IPostProcessor.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10624 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Adapters/IPrepareApp.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2110 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Adapters/IRuntimeHandler.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3121 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Adapters/ISplitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Adapters/IVirtualization.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7579 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Adapters/StandardJobConfig.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      156 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:32.995904 ganga-8.7.4/ganga/GangaCore/GPIDev/Base/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4315 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Base/Filters.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    59985 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Base/Objects.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    53774 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Base/Proxy.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12619 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Base/VPrinter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5177 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Base/VPrinterOld.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      350 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:32.995904 ganga-8.7.4/ganga/GangaCore/GPIDev/Credentials/
--rw-r--r--   0 runner    (1001) docker     (127)     5718 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Credentials/AfsToken.py
--rw-r--r--   0 runner    (1001) docker     (127)    12949 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Credentials/CredentialStore.py
--rw-r--r--   0 runner    (1001) docker     (127)     7443 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Credentials/VomsProxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Credentials/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:32.995904 ganga-8.7.4/ganga/GangaCore/GPIDev/Credentials_old/
--rwxr-xr-x   0 runner    (1001) docker     (127)    20594 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Credentials_old/ICredential.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3369 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Credentials_old/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:32.995904 ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:32.995904 ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/Config/
--rwxr-xr-x   0 runner    (1001) docker     (127)    11717 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/Config/Config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       52 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/Config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:32.995904 ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/Dataset/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1063 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/Dataset/Dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5984 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/Dataset/GangaDataset.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       69 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/Dataset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:32.995904 ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/File/
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/File/Configure.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    17376 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/File/File.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2878 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/File/FileBuffer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/File/FileUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)    24411 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/File/GoogleFile.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11639 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/File/LocalFile.py
--rw-r--r--   0 runner    (1001) docker     (127)    26379 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/File/MassStorageFile.py
--rw-r--r--   0 runner    (1001) docker     (127)    12947 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/File/OutputFileManager.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3257 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/File/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:32.995904 ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/File/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/File/scripts/LCGSEFileWNScript.py.template
--rw-r--r--   0 runner    (1001) docker     (127)     4324 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/File/scripts/MassStorageFileWNScript.py.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:32.999904 ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/GangaList/
--rwxr-xr-x   0 runner    (1001) docker     (127)    26733 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/GangaList/GangaList.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       38 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/GangaList/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:32.999904 ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/Job/
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/Job/Error.py
--rwxr-xr-x   0 runner    (1001) docker     (127)   121942 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/Job/Job.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/Job/JobInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)    18975 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/Job/JobTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/Job/MetadataDict.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      231 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/Job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/Job/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:32.999904 ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/JobTree/
--rwxr-xr-x   0 runner    (1001) docker     (127)    15970 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/JobTree/JobTree.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      292 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/JobTree/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:32.999904 ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/Registry/
--rwxr-xr-x   0 runner    (1001) docker     (127)     8979 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/Registry/BoxRegistry.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14541 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/Registry/JobRegistry.py
--rw-r--r--   0 runner    (1001) docker     (127)    27539 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/Registry/PrepRegistry.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    21459 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/Registry/RegistrySlice.py
--rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/Registry/RegistrySliceProxy.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/Registry/RegistryUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4432 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/Registry/TransientRegistry.py
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/Registry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.003904 ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/Tasks/
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/Tasks/CoreTask.py
--rw-r--r--   0 runner    (1001) docker     (127)     7215 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/Tasks/CoreTransform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/Tasks/CoreUnit.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12904 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/Tasks/ITask.py
--rw-r--r--   0 runner    (1001) docker     (127)    28090 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/Tasks/ITransform.py
--rw-r--r--   0 runner    (1001) docker     (127)    19618 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/Tasks/IUnit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/Tasks/TaskChainInput.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/Tasks/TaskLocalCopy.py
--rw-r--r--   0 runner    (1001) docker     (127)    22780 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/Tasks/TaskRegistry.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      739 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/Tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/Tasks/common.py
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.003904 ganga-8.7.4/ganga/GangaCore/GPIDev/MonitoringServices/
--rwxr-xr-x   0 runner    (1001) docker     (127)    10221 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/MonitoringServices/Composite.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4801 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/MonitoringServices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.003904 ganga-8.7.4/ganga/GangaCore/GPIDev/Persistency/
--rwxr-xr-x   0 runner    (1001) docker     (127)     7887 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Persistency/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.003904 ganga-8.7.4/ganga/GangaCore/GPIDev/Schema/
--rwxr-xr-x   0 runner    (1001) docker     (127)    32271 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Schema/Schema.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      130 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/Schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/TypeCheck.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      106 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/GPIDev/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.003904 ganga-8.7.4/ganga/GangaCore/Lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.003904 ganga-8.7.4/ganga/GangaCore/Lib/Batch/
--rwxr-xr-x   0 runner    (1001) docker     (127)    25180 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Lib/Batch/Batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Lib/Batch/BatchScriptTemplate.py.template
--rwxr-xr-x   0 runner    (1001) docker     (127)      128 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Lib/Batch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.003904 ganga-8.7.4/ganga/GangaCore/Lib/Checkers/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2335 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Lib/Checkers/CustomChecker.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2822 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Lib/Checkers/FileChecker.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2099 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Lib/Checkers/MetaDataChecker.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6964 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Lib/Checkers/RootFileChecker.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      169 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Lib/Checkers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.003904 ganga-8.7.4/ganga/GangaCore/Lib/Condor/
--rwxr-xr-x   0 runner    (1001) docker     (127)    29396 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Lib/Condor/Condor.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4609 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Lib/Condor/CondorRequirements.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      566 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Lib/Condor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.003904 ganga-8.7.4/ganga/GangaCore/Lib/Executable/
--rwxr-xr-x   0 runner    (1001) docker     (127)    13956 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Lib/Executable/Executable.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      149 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Lib/Executable/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.007904 ganga-8.7.4/ganga/GangaCore/Lib/Interactive/
--rwxr-xr-x   0 runner    (1001) docker     (127)    11328 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Lib/Interactive/Interactive.py
--rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Lib/Interactive/InteractiveScriptTemplate.py.template
--rwxr-xr-x   0 runner    (1001) docker     (127)      530 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Lib/Interactive/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.007904 ganga-8.7.4/ganga/GangaCore/Lib/Localhost/
--rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Lib/Localhost/LocalHostExec.py.template
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Lib/Localhost/LocalHostExec_batch.py.template
--rwxr-xr-x   0 runner    (1001) docker     (127)    17498 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Lib/Localhost/Localhost.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       34 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Lib/Localhost/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.007904 ganga-8.7.4/ganga/GangaCore/Lib/Mergers/
--rwxr-xr-x   0 runner    (1001) docker     (127)    15780 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Lib/Mergers/Merger.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       44 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Lib/Mergers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.007904 ganga-8.7.4/ganga/GangaCore/Lib/Notebook/
--rwxr-xr-x   0 runner    (1001) docker     (127)     7136 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Lib/Notebook/Notebook.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       32 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Lib/Notebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Lib/Notebook/wrapperNotebookTemplate.py.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.007904 ganga-8.7.4/ganga/GangaCore/Lib/Notifier/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2823 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Lib/Notifier/Notifier.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       32 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Lib/Notifier/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.007904 ganga-8.7.4/ganga/GangaCore/Lib/Remote/
--rw-r--r--   0 runner    (1001) docker     (127)    32668 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Lib/Remote/Remote.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Lib/Remote/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.007904 ganga-8.7.4/ganga/GangaCore/Lib/Splitters/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4294 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Lib/Splitters/ArgSplitter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1628 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Lib/Splitters/DefaultSplitter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1466 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Lib/Splitters/ExeSplitter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2450 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Lib/Splitters/GangaDatasetSplitter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5491 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Lib/Splitters/GenericSplitter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      223 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Lib/Splitters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.007904 ganga-8.7.4/ganga/GangaCore/Lib/Virtualization/
--rw-r--r--   0 runner    (1001) docker     (127)     6491 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Lib/Virtualization/Apptainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4884 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Lib/Virtualization/Docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     6638 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Lib/Virtualization/Singularity.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Lib/Virtualization/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Lib/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6001 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/PACKAGE.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.011904 ganga-8.7.4/ganga/GangaCore/Runtime/
--rw-r--r--   0 runner    (1001) docker     (127)     4511 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Runtime/GPIFunctions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Runtime/GPIexport.py
--rw-r--r--   0 runner    (1001) docker     (127)    17289 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Runtime/GangaCompleter.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Runtime/HEAD_CONFIG.INI
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Runtime/IPythonMagic.py
--rw-r--r--   0 runner    (1001) docker     (127)    11576 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Runtime/Repository_runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Runtime/Workspace_runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    65064 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Runtime/bootstrap.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12710 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Runtime/eliza.py
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Runtime/ganga_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     7608 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Runtime/gangadoc.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Runtime/gangadoceval.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Runtime/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.015904 ganga-8.7.4/ganga/GangaCore/Utility/
--rw-r--r--   0 runner    (1001) docker     (127)     7348 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Utility/ColourText.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.015904 ganga-8.7.4/ganga/GangaCore/Utility/Config/
--rwxr-xr-x   0 runner    (1001) docker     (127)       51 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Utility/Config/A.ini
--rwxr-xr-x   0 runner    (1001) docker     (127)       68 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Utility/Config/B.ini
--rw-r--r--   0 runner    (1001) docker     (127)    43719 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Utility/Config/Config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       41 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Utility/Config/ConfigTest.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Utility/Config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Utility/Config/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Utility/Decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Utility/GridShell.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.015904 ganga-8.7.4/ganga/GangaCore/Utility/Plugin/
--rw-r--r--   0 runner    (1001) docker     (127)     4887 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Utility/Plugin/GangaPlugin.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Utility/Plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Utility/Profiling.py
--rw-r--r--   0 runner    (1001) docker     (127)    14300 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Utility/Runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     6993 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Utility/Setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    12520 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Utility/Shell.py
--rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Utility/Virtualization.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11319 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Utility/execute.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.015904 ganga-8.7.4/ganga/GangaCore/Utility/external/
--rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Utility/external/OrderedDict.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Utility/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26942 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Utility/feedback_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Utility/files.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.015904 ganga-8.7.4/ganga/GangaCore/Utility/logging/
--rw-r--r--   0 runner    (1001) docker     (127)    21901 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Utility/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Utility/logging/message_caching_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Utility/logging/test.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Utility/logic.py
--rw-r--r--   0 runner    (1001) docker     (127)     8018 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Utility/root.py
--rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Utility/stacktracer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Utility/strings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Utility/threads.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9868 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/Utility/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    51841 2024-03-19 20:21:31.000000 ganga-8.7.4/ganga/GangaCore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.015904 ganga-8.7.4/ganga/GangaCore/old_test/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.015904 ganga-8.7.4/ganga/GangaCore/old_test/Bugs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.015904 ganga-8.7.4/ganga/GangaCore/old_test/Bugs/Savannah10013/
--rwxr-xr-x   0 runner    (1001) docker     (127)       72 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/old_test/Bugs/Savannah10013/Savannah10013.ini
--rwxr-xr-x   0 runner    (1001) docker     (127)       92 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/old_test/Bugs/Savannah17638.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.015904 ganga-8.7.4/ganga/GangaCore/old_test/Bugs/Savannah23737/
--rwxr-xr-x   0 runner    (1001) docker     (127)       28 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/old_test/Bugs/Savannah23737/Savannah23737.ini
--rwxr-xr-x   0 runner    (1001) docker     (127)       31 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/old_test/Bugs/Savannah32201.ini
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/old_test/Bugs/Savannah36651.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.019904 ganga-8.7.4/ganga/GangaCore/old_test/GPI/
--rwxr-xr-x   0 runner    (1001) docker     (127)       44 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/old_test/GPI/BackendApplicationMatrix.ini
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/old_test/GPI/CompressOutput.ini
--rwxr-xr-x   0 runner    (1001) docker     (127)      115 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/old_test/GPI/ConfigFile.ini
--rwxr-xr-x   0 runner    (1001) docker     (127)      751 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/old_test/GPI/ConfigObject.ini
--rwxr-xr-x   0 runner    (1001) docker     (127)      625 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/old_test/GPI/ConfigUser.ini
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/old_test/GPI/LCG.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.019904 ganga-8.7.4/ganga/GangaCore/old_test/GPI/Mergers/
--rwxr-xr-x   0 runner    (1001) docker     (127)      418 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/old_test/GPI/Mergers/TestRootMerger.ini
--rwxr-xr-x   0 runner    (1001) docker     (127)      141 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/old_test/GPI/Mergers/TestTextMerger.ini
--rwxr-xr-x   0 runner    (1001) docker     (127)      140 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/old_test/GPI/Mergers/TestTextMergerGzip.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.019904 ganga-8.7.4/ganga/GangaCore/old_test/GPI/MigrationFramework/
--rwxr-xr-x   0 runner    (1001) docker     (127)       36 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/old_test/GPI/MigrationFramework/MigrationFramework.ini
--rwxr-xr-x   0 runner    (1001) docker     (127)       75 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/old_test/GPI/MigrationFramework/MigrationFramework.pass1.ini
--rwxr-xr-x   0 runner    (1001) docker     (127)       74 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/old_test/GPI/MigrationFramework/MigrationFramework.pass2.ini
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/old_test/GPI/MonTest.ini
--rwxr-xr-x   0 runner    (1001) docker     (127)       28 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/old_test/GPI/MonitoringServices.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.023904 ganga-8.7.4/ganga/GangaCore/old_test/GPI/OutputFiles/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesBatch.ini
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesBatchMultipleFilesForLCGUpload.ini
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesBatchMultipleFilesForMassStorageAndLCGUpload.ini
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesBatchMultipleFilesForMassStorageUpload.ini
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesCompressedBatch.ini
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesCompressedLocal.ini
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesInteractive.ini
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesInteractiveMultipleFilesForLCGUpload.ini
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesInteractiveMultipleFilesForPattern.ini
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesLCG.ini
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesLCGMultipleCompressedFilesForMassStorageAndLCGUpload.ini
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesLocal.ini
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesLocalMultipleFilesForLCGUpload.ini
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesLocalMultipleFilesForPattern.ini
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesMixedBatch.ini
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/old_test/GPI/RegistrySorting.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.023904 ganga-8.7.4/ganga/GangaCore/old_test/GPI/ResubmitSubjobs/
--rwxr-xr-x   0 runner    (1001) docker     (127)       28 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/old_test/GPI/ResubmitSubjobs/ResubmitSubjobs.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.023904 ganga-8.7.4/ganga/GangaCore/old_test/GPI/Root/
--rwxr-xr-x   0 runner    (1001) docker     (127)      299 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/old_test/GPI/Root/TestRoot.ini
--rwxr-xr-x   0 runner    (1001) docker     (127)       48 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/old_test/GPI/WorkspaceRemoval.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.023904 ganga-8.7.4/ganga/GangaCore/old_test/GPI/auto_resubmit/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/old_test/GPI/auto_resubmit/auto_resubmit.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.023904 ganga-8.7.4/ganga/GangaCore/old_test/Internals/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/old_test/Internals/TestGridProxyExpandSystemVars.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.023904 ganga-8.7.4/ganga/GangaCore/old_test/Performance/
--rwxr-xr-x   0 runner    (1001) docker     (127)      184 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/old_test/Performance/PerfStats.ini
--rwxr-xr-x   0 runner    (1001) docker     (127)      101 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/old_test/Performance/TimeJobs.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.023904 ganga-8.7.4/ganga/GangaCore/old_test/XMLRepository/
--rwxr-xr-x   0 runner    (1001) docker     (127)       47 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/old_test/XMLRepository/SpecialName.ini
--rwxr-xr-x   0 runner    (1001) docker     (127)      642 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/old_test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.023904 ganga-8.7.4/ganga/GangaCore/old_test/config/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1195 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/old_test/config/Schema.ini
--rwxr-xr-x   0 runner    (1001) docker     (127)      793 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/old_test/config/default.ini
--rwxr-xr-x   0 runner    (1001) docker     (127)      793 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/old_test/config/localxml.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:32.907904 ganga-8.7.4/ganga/GangaCore/test/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:32.907904 ganga-8.7.4/ganga/GangaCore/test/GPI/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.023904 ganga-8.7.4/ganga/GangaCore/test/GPI/Config/
--rwxr-xr-x   0 runner    (1001) docker     (127)       50 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/test/GPI/Config/A.ini
--rwxr-xr-x   0 runner    (1001) docker     (127)       54 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/test/GPI/Config/B.ini
--rwxr-xr-x   0 runner    (1001) docker     (127)       40 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/test/GPI/Config/ConfigTest.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.023904 ganga-8.7.4/ganga/GangaCore/test/GPI/Notebook/
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/test/GPI/Notebook/Test.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.023904 ganga-8.7.4/ganga/GangaCore/testlib/
--rw-r--r--   0 runner    (1001) docker     (127)    12196 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/testlib/GangaUnitTest.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/testlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/testlib/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/testlib/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/testlib/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/testlib/mark.py
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaCore/testlib/monitoring.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.023904 ganga-8.7.4/ganga/GangaDirac/
--rwxr-xr-x   0 runner    (1001) docker     (127)     7275 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaDirac/BOOT.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaDirac/Dirac.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.027904 ganga-8.7.4/ganga/GangaDirac/Lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.027904 ganga-8.7.4/ganga/GangaDirac/Lib/Backends/
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaDirac/Lib/Backends/Dirac.py
--rw-r--r--   0 runner    (1001) docker     (127)    75705 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaDirac/Lib/Backends/DiracBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     9633 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaDirac/Lib/Backends/DiracUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaDirac/Lib/Backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.027904 ganga-8.7.4/ganga/GangaDirac/Lib/Credentials/
--rw-r--r--   0 runner    (1001) docker     (127)     8772 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaDirac/Lib/Credentials/DiracProxy.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaDirac/Lib/Credentials/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.027904 ganga-8.7.4/ganga/GangaDirac/Lib/Files/
--rw-r--r--   0 runner    (1001) docker     (127)    39938 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaDirac/Lib/Files/DiracFile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaDirac/Lib/Files/WNInjectTemplate.py.template
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaDirac/Lib/Files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaDirac/Lib/Files/downloadScript.py.template
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaDirac/Lib/Files/uploadScript.py.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.027904 ganga-8.7.4/ganga/GangaDirac/Lib/RTHandlers/
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaDirac/Lib/RTHandlers/DiracRTHScript.py.template
--rw-r--r--   0 runner    (1001) docker     (127)     9914 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaDirac/Lib/RTHandlers/DiracRTHUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10397 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaDirac/Lib/RTHandlers/ExeDiracRTHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     7472 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaDirac/Lib/RTHandlers/RunTimeHandlerUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaDirac/Lib/RTHandlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.031904 ganga-8.7.4/ganga/GangaDirac/Lib/Server/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaDirac/Lib/Server/BlankCommands.py
--rw-r--r--   0 runner    (1001) docker     (127)    18388 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaDirac/Lib/Server/DiracCommands.py
--rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaDirac/Lib/Server/DiracDefinition.py
--rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaDirac/Lib/Server/DiracExecutorProcess.py
--rw-r--r--   0 runner    (1001) docker     (127)    20454 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaDirac/Lib/Server/DiracNewCommands.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2266 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaDirac/Lib/Server/DiracOldProcess.py
--rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaDirac/Lib/Server/DiracProcessManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaDirac/Lib/Server/InspectionClient.py
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaDirac/Lib/Server/InspectionServer.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaDirac/Lib/Server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.031904 ganga-8.7.4/ganga/GangaDirac/Lib/Splitters/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3253 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaDirac/Lib/Splitters/GangaSplitterUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)    24738 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaDirac/Lib/Splitters/OfflineGangaDiracSplitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaDirac/Lib/Splitters/SplitterUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaDirac/Lib/Splitters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.031904 ganga-8.7.4/ganga/GangaDirac/Lib/Utilities/
--rw-r--r--   0 runner    (1001) docker     (127)    12049 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaDirac/Lib/Utilities/DiracUtilities.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaDirac/Lib/Utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaDirac/Lib/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      665 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaDirac/PACKAGE.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9416 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaDirac/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:32.907904 ganga-8.7.4/ganga/GangaDirac/old_test/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:32.907904 ganga-8.7.4/ganga/GangaDirac/old_test/GPI/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.031904 ganga-8.7.4/ganga/GangaDirac/old_test/GPI/Files/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaDirac/old_test/GPI/Files/TestDiracFile.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:32.907904 ganga-8.7.4/ganga/GangaDirac/old_test/Lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.031904 ganga-8.7.4/ganga/GangaDirac/old_test/Lib/RTHandlers/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaDirac/old_test/Lib/RTHandlers/TestExeDiracRTHandler.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.031904 ganga-8.7.4/ganga/GangaGaudi/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaGaudi/Gaudi.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.031904 ganga-8.7.4/ganga/GangaGaudi/Lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.031904 ganga-8.7.4/ganga/GangaGaudi/Lib/Applications/
--rw-r--r--   0 runner    (1001) docker     (127)     5645 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaGaudi/Lib/Applications/CMTUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8152 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaGaudi/Lib/Applications/Gaudi.py
--rw-r--r--   0 runner    (1001) docker     (127)    11669 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaGaudi/Lib/Applications/GaudiBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     8147 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaGaudi/Lib/Applications/GaudiUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5305 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaGaudi/Lib/Applications/GaudiXMLSummary.py
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaGaudi/Lib/Applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaGaudi/Lib/Applications/cmakeUtils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.031904 ganga-8.7.4/ganga/GangaGaudi/Lib/Checkers/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2848 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaGaudi/Lib/Checkers/GaudiMetaDataChecker.py
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaGaudi/Lib/Checkers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.031904 ganga-8.7.4/ganga/GangaGaudi/Lib/Datasets/
--rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaGaudi/Lib/Datasets/GaudiDataset.py
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaGaudi/Lib/Datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.031904 ganga-8.7.4/ganga/GangaGaudi/Lib/RTHandlers/
--rw-r--r--   0 runner    (1001) docker     (127)     5599 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaGaudi/Lib/RTHandlers/GaudiDiracRunTimeHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaGaudi/Lib/RTHandlers/GaudiRunTimeHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaGaudi/Lib/RTHandlers/RunTimeHandlerUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaGaudi/Lib/RTHandlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.035904 ganga-8.7.4/ganga/GangaGaudi/Lib/Splitters/
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaGaudi/Lib/Splitters/GaudiInputDataSplitter.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaGaudi/Lib/Splitters/SplitterUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaGaudi/Lib/Splitters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.035904 ganga-8.7.4/ganga/GangaGaudi/Lib/XMLSummary/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaGaudi/Lib/XMLSummary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    64665 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaGaudi/Lib/XMLSummary/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    25090 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaGaudi/Lib/XMLSummary/summary.py
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaGaudi/Lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaGaudi/PACKAGE.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaGaudi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.035904 ganga-8.7.4/ganga/GangaLHCb/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4251 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/BOOT.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2067 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/LHCb.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.035904 ganga-8.7.4/ganga/GangaLHCb/Lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.039903 ganga-8.7.4/ganga/GangaLHCb/Lib/Applications/
--rw-r--r--   0 runner    (1001) docker     (127)    14127 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/Lib/Applications/AppsBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/Lib/Applications/AppsBaseUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8806 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/Lib/Applications/Bender.py
--rw-r--r--   0 runner    (1001) docker     (127)    24468 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/Lib/Applications/BenderBox.py
--rw-r--r--   0 runner    (1001) docker     (127)    13997 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/Lib/Applications/BenderScript.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3409 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/Lib/Applications/CMTscript.py
--rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/Lib/Applications/EnvironFunctions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/Lib/Applications/FileFunctions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    31734 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/Lib/Applications/GaudiExec.py
--rw-r--r--   0 runner    (1001) docker     (127)     7845 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/Lib/Applications/GaudiExecUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/Lib/Applications/GaudiPython.py
--rw-r--r--   0 runner    (1001) docker     (127)    12134 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/Lib/Applications/Ostap.py
--rw-r--r--   0 runner    (1001) docker     (127)    10481 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/Lib/Applications/PythonOptionsParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4796 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/Lib/Applications/PythonOptsCmakeParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/Lib/Applications/XMLPostProcessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/Lib/Applications/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.039903 ganga-8.7.4/ganga/GangaLHCb/Lib/Backends/
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/Lib/Backends/Bookkeeping.py
--rw-r--r--   0 runner    (1001) docker     (127)     5008 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/Lib/Backends/Dirac.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/Lib/Backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.039903 ganga-8.7.4/ganga/GangaLHCb/Lib/Checkers/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2862 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/Lib/Checkers/LHCbMetadataChecker.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/Lib/Checkers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.039903 ganga-8.7.4/ganga/GangaLHCb/Lib/Files/
--rw-r--r--   0 runner    (1001) docker     (127)     4419 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/Lib/Files/LogicalFile.py
--rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/Lib/Files/PhysicalFile.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/Lib/Files/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.039903 ganga-8.7.4/ganga/GangaLHCb/Lib/LHCbDataset/
--rw-r--r--   0 runner    (1001) docker     (127)    13473 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/Lib/LHCbDataset/BKQuery.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    19914 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/Lib/LHCbDataset/LHCbCompressedDataset.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    23063 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/Lib/LHCbDataset/LHCbDataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/Lib/LHCbDataset/LHCbDatasetUtils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      192 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/Lib/LHCbDataset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.039903 ganga-8.7.4/ganga/GangaLHCb/Lib/Mergers/
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/Lib/Mergers/CMTVersion.py
--rw-r--r--   0 runner    (1001) docker     (127)    11090 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/Lib/Mergers/GaudiExecMerger.py
--rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/Lib/Mergers/LHCbFileMerger.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/Lib/Mergers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.043904 ganga-8.7.4/ganga/GangaLHCb/Lib/RTHandlers/
--rw-r--r--   0 runner    (1001) docker     (127)    10771 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/Lib/RTHandlers/ExeDiracRTHandler.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    34964 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/Lib/RTHandlers/GaudiExecRTHandlers.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/Lib/RTHandlers/GaudiTemplate.py.template
--rw-r--r--   0 runner    (1001) docker     (127)    11732 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/Lib/RTHandlers/LHCbGaudiDiracRunTimeHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     6431 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/Lib/RTHandlers/LHCbGaudiRunTimeHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4345 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/Lib/RTHandlers/RTHUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/Lib/RTHandlers/WorkerScript.py.template
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/Lib/RTHandlers/XMLWorkerScript.py.template
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/Lib/RTHandlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.043904 ganga-8.7.4/ganga/GangaLHCb/Lib/Server/
--rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/Lib/Server/DiracLHCbCommands.py
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/Lib/Server/DiracLHCbDefinition.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/Lib/Server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.043904 ganga-8.7.4/ganga/GangaLHCb/Lib/Splitters/
--rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/Lib/Splitters/GaussSplitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/Lib/Splitters/LHCbSplitterUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/Lib/Splitters/OptionsFileSplitter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10998 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/Lib/Splitters/SplitByFiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     6235 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/Lib/Splitters/SplitFilesBySize.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/Lib/Splitters/TestSplitter.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/Lib/Splitters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.043904 ganga-8.7.4/ganga/GangaLHCb/Lib/Tasks/
--rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/Lib/Tasks/BKTestQuery.py
--rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/Lib/Tasks/LHCbTask.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/Lib/Tasks/LHCbTaskDummySplitter.py
--rw-r--r--   0 runner    (1001) docker     (127)    12584 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/Lib/Tasks/LHCbTransform.py
--rw-r--r--   0 runner    (1001) docker     (127)     4975 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/Lib/Tasks/LHCbUnit.py
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/Lib/Tasks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.043904 ganga-8.7.4/ganga/GangaLHCb/Lib/XMLSummary/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/Lib/XMLSummary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    64685 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/Lib/XMLSummary/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    25050 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/Lib/XMLSummary/summary.py
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/Lib/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      665 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/PACKAGE.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.043904 ganga-8.7.4/ganga/GangaLHCb/Utility/
--rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/Utility/LHCbDIRACenv.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/Utility/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8960 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.043904 ganga-8.7.4/ganga/GangaLHCb/testlib/
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaLHCb/testlib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.047904 ganga-8.7.4/ganga/GangaND280/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaND280/BOOT.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.047904 ganga-8.7.4/ganga/GangaND280/Highland/
--rw-r--r--   0 runner    (1001) docker     (127)     7061 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaND280/Highland/Highland.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       24 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaND280/Highland/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaND280/ND280.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.047904 ganga-8.7.4/ganga/GangaND280/ND280Checkers/
--rw-r--r--   0 runner    (1001) docker     (127)    19378 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaND280/ND280Checkers/ND280Checker.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       56 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaND280/ND280Checkers/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9075 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaND280/ND280Checkers/post_status.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.047904 ganga-8.7.4/ganga/GangaND280/ND280Control/
--rwxr-xr-x   0 runner    (1001) docker     (127)    27283 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaND280/ND280Control/ND280Configs.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaND280/ND280Control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8913 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaND280/ND280Control/runND280.py
--rw-r--r--   0 runner    (1001) docker     (127)     8252 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaND280/ND280Control/runND280CosMC.py
--rw-r--r--   0 runner    (1001) docker     (127)     9047 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaND280/ND280Control/runND280CtrlSmpl.py
--rw-r--r--   0 runner    (1001) docker     (127)     7472 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaND280/ND280Control/runND280Kin.py
--rw-r--r--   0 runner    (1001) docker     (127)     8519 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaND280/ND280Control/runND280RDP.py
--rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaND280/ND280Control/runND280SandMC.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.047904 ganga-8.7.4/ganga/GangaND280/ND280Dataset/
--rwxr-xr-x   0 runner    (1001) docker     (127)     8427 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaND280/ND280Dataset/ND280Dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       39 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaND280/ND280Dataset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.047904 ganga-8.7.4/ganga/GangaND280/ND280Executable/
--rw-r--r--   0 runner    (1001) docker     (127)     7662 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaND280/ND280Executable/ND280Executable.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       31 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaND280/ND280Executable/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.051904 ganga-8.7.4/ganga/GangaND280/ND280RecoValidation/
--rw-r--r--   0 runner    (1001) docker     (127)    10903 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaND280/ND280RecoValidation/RecoPlusVFT.py
--rw-r--r--   0 runner    (1001) docker     (127)    12950 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaND280/ND280RecoValidation/VFT_make_ana.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       92 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaND280/ND280RecoValidation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9922 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaND280/ND280RecoValidation/oaReconPlusoaAnalysis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.051904 ganga-8.7.4/ganga/GangaND280/ND280Skimmer/
--rw-r--r--   0 runner    (1001) docker     (127)     8638 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaND280/ND280Skimmer/ND280Skimmer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       28 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaND280/ND280Skimmer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.051904 ganga-8.7.4/ganga/GangaND280/ND280Splitter/
--rwxr-xr-x   0 runner    (1001) docker     (127)     8589 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaND280/ND280Splitter/ND280Splitter.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaND280/ND280Splitter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.051904 ganga-8.7.4/ganga/GangaND280/ND280TPCGasInteractions/
--rw-r--r--   0 runner    (1001) docker     (127)     9046 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaND280/ND280TPCGasInteractions/TRExPlusOAAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaND280/ND280TPCGasInteractions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaND280/PACKAGE.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.051904 ganga-8.7.4/ganga/GangaND280/Tasks/
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaND280/Tasks/ND280Task.py
--rw-r--r--   0 runner    (1001) docker     (127)     6520 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaND280/Tasks/ND280Transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaND280/Tasks/ND280Transform_CSVEvtList.py
--rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaND280/Tasks/ND280Unit.py
--rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaND280/Tasks/ND280Unit_CSVEvtList.py
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaND280/Tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaND280/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.055904 ganga-8.7.4/ganga/GangaRelease/
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaRelease/ReleaseNotes
--rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-7.0.0
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-7.0.1
--rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-7.0.2
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-7.0.3
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-7.0.4
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-7.1.0
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-7.1.1
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-7.1.10
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-7.1.11
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-7.1.12
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-7.1.13
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-7.1.14
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-7.1.15
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-7.1.2
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-7.1.3
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-7.1.4
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-7.1.5
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-7.1.6
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-7.1.7
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-7.1.8
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-7.1.9
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-8.0.0
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-8.0.1
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-8.0.2
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-8.0.3
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-8.1.0
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-8.2.0
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-8.2.1
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-8.2.2
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-8.2.3
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-8.2.4
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-8.3.0
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-8.3.1
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-8.3.2
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-8.3.3
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-19 20:21:31.000000 ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-8.7.4
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.055904 ganga-8.7.4/ganga/GangaRelease/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaRelease/tools/check-new-ganga.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaRelease/tools/ganga-cvmfs-install-dev.sh
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaRelease/tools/ganga-cvmfs-install.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.059903 ganga-8.7.4/ganga/GangaTest/
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaTest/BOOT.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.059903 ganga-8.7.4/ganga/GangaTest/Framework/
--rwxr-xr-x   0 runner    (1001) docker     (127)       34 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaTest/Framework/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18555 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaTest/Framework/driver.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    31840 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaTest/Framework/htmlizer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    47550 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaTest/Framework/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     9026 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaTest/Framework/runner.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11385 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaTest/Framework/tests.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4149 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaTest/Framework/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13506 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaTest/Framework/xmldifferencer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.059903 ganga-8.7.4/ganga/GangaTest/Lib/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4013 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaTest/Lib/CrashTest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.059903 ganga-8.7.4/ganga/GangaTest/Lib/GListApp/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2803 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaTest/Lib/GListApp/GListApp.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      485 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaTest/Lib/GListApp/PACKAGE.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       32 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaTest/Lib/GListApp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.059903 ganga-8.7.4/ganga/GangaTest/Lib/RTHandlers/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaTest/Lib/RTHandlers/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3277 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaTest/Lib/StoreTestFramework.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.059903 ganga-8.7.4/ganga/GangaTest/Lib/TFile/
--rwxr-xr-x   0 runner    (1001) docker     (127)      485 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaTest/Lib/TFile/PACKAGE.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1485 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaTest/Lib/TFile/TFile.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       26 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaTest/Lib/TFile/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.059903 ganga-8.7.4/ganga/GangaTest/Lib/TestApplication/
--rwxr-xr-x   0 runner    (1001) docker     (127)     5553 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaTest/Lib/TestApplication/TestApplication.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1283 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaTest/Lib/TestApplication/TestDataset.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      100 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaTest/Lib/TestApplication/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.063903 ganga-8.7.4/ganga/GangaTest/Lib/TestMonitoringService/
--rwxr-xr-x   0 runner    (1001) docker     (127)      865 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaTest/Lib/TestMonitoringService/TestMonitoringService.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       37 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaTest/Lib/TestMonitoringService/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaTest/Lib/TestObjects.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.063903 ganga-8.7.4/ganga/GangaTest/Lib/TestRemoteBackend/
--rw-r--r--   0 runner    (1001) docker     (127)    18622 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaTest/Lib/TestRemoteBackend/TestRemoteBackend.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaTest/Lib/TestRemoteBackend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaTest/Lib/TestRemoteBackend/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.063903 ganga-8.7.4/ganga/GangaTest/Lib/TestSubmitter/
--rwxr-xr-x   0 runner    (1001) docker     (127)      386 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaTest/Lib/TestSubmitter/TestConfig.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1219 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaTest/Lib/TestSubmitter/TestConfig2.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1363 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaTest/Lib/TestSubmitter/TestSplitter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3498 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaTest/Lib/TestSubmitter/TestSubmitter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      176 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaTest/Lib/TestSubmitter/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      325 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaTest/Lib/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      952 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaTest/PACKAGE.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.063903 ganga-8.7.4/ganga/GangaTest/TestGPIP/
--rwxr-xr-x   0 runner    (1001) docker     (127)      153 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaTest/TestGPIP/TestGPIP.ini
--rwxr-xr-x   0 runner    (1001) docker     (127)      448 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaTest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.063903 ganga-8.7.4/ganga/GangaTutorial/
--rwxr-xr-x   0 runner    (1001) docker     (127)      649 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaTutorial/BOOT.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.063903 ganga-8.7.4/ganga/GangaTutorial/Lib/
--rwxr-xr-x   0 runner    (1001) docker     (127)     6722 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaTutorial/Lib/PrimeFactorizer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2258 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaTutorial/Lib/PrimeFactorizerSplitter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2287 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaTutorial/Lib/PrimeTableDataset.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      103 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaTutorial/Lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.063903 ganga-8.7.4/ganga/GangaTutorial/Lib/primes/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaTutorial/Lib/primes/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3020 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaTutorial/Lib/primes/prime_factor.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2158 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaTutorial/Lib/primes/primes.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      894 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaTutorial/PACKAGE.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       45 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaTutorial/Tutorial.ini
--rwxr-xr-x   0 runner    (1001) docker     (127)      202 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/GangaTutorial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.063903 ganga-8.7.4/ganga/ganga/
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/ganga/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-19 20:21:22.000000 ganga-8.7.4/ganga/submit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:21:33.063903 ganga-8.7.4/ganga.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-03-19 20:21:32.000000 ganga-8.7.4/ganga.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    35759 2024-03-19 20:21:32.000000 ganga-8.7.4/ganga.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 20:21:32.000000 ganga-8.7.4/ganga.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-03-19 20:21:32.000000 ganga-8.7.4/ganga.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-19 20:21:32.000000 ganga-8.7.4/ganga.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-03-19 20:21:33.067903 ganga-8.7.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-03-19 20:21:31.000000 ganga-8.7.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.970208 ganga-8.7.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-05 11:20:46.000000 ganga-8.7.5/LICENSE_GPL
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-05 11:20:46.000000 ganga-8.7.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-05 11:20:57.970208 ganga-8.7.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-05 11:20:46.000000 ganga-8.7.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.822207 ganga-8.7.5/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3667 2024-04-05 11:20:46.000000 ganga-8.7.5/bin/ganga
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.822207 ganga-8.7.5/doc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.822207 ganga-8.7.5/doc/API/
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/API/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.822207 ganga-8.7.5/doc/GPI/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/GPI/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7818 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.826207 ganga-8.7.5/doc/UserGuide/
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/UserGuide/Configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/UserGuide/GoogleOauth.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6683 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/UserGuide/InputAndOutputData.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8173 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/UserGuide/InstallAndBasicUsage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5383 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/UserGuide/JobManipulation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/UserGuide/MiscellaneousFunctionality.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10662 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/UserGuide/PostProcessors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/UserGuide/Queues.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/UserGuide/RunningExecutables.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5973 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/UserGuide/Splitters.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/UserGuide/Tasks.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/UserGuide/TutorialPlugin.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/UserGuide/UsingDifferentApplications.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/UserGuide/UsingDifferentBackends.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7927 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/UserGuide/Virtualization.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/UserGuide/WhatIsGanga.rst
+-rw-r--r--   0 runner    (1001) docker     (127)   587157 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/UserGuide/first_job.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/UserGuide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    65215 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/UserGuide/start_terminal.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   515269 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/UserGuide/virtualization.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.826207 ganga-8.7.5/doc/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     7406 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    20408 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/_static/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     9971 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.826207 ganga-8.7.5/doc/dev/
+-rw-r--r--   0 runner    (1001) docker     (127)     5643 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/dev/credentials.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9109 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/dev/index.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7656 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/fill_gpi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.806207 ganga-8.7.5/doc/journal/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.850207 ganga-8.7.5/doc/journal/CPC2007/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    55839 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/journal/CPC2007/GangaJob.pdf
+-rwxr-xr-x   0 runner    (1001) docker     (127)   310914 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/journal/CPC2007/GangaOverview.pdf
+-rwxr-xr-x   0 runner    (1001) docker     (127)   121579 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/journal/CPC2007/GangaPlugin.pdf
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1000 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/journal/CPC2007/README
+-rwxr-xr-x   0 runner    (1001) docker     (127)   189776 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/journal/CPC2007/avianflu.pdf
+-rwxr-xr-x   0 runner    (1001) docker     (127)   255272 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/journal/CPC2007/avianflu.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7896 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/journal/CPC2007/camtology.tex
+-rw-r--r--   0 runner    (1001) docker     (127)  5151013 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/journal/CPC2007/camtologyfigure.eps
+-rwxr-xr-x   0 runner    (1001) docker     (127)   588084 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/journal/CPC2007/camtologyfigure.pdf
+-rwxr-xr-x   0 runner    (1001) docker     (127)   106103 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/journal/CPC2007/camtologytech.pdf
+-rwxr-xr-x   0 runner    (1001) docker     (127)    54997 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/journal/CPC2007/elsart.cls
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13301 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/journal/CPC2007/elsart1p.cls
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13505 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/journal/CPC2007/elsart3p.cls
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13426 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/journal/CPC2007/elsart5p.cls
+-rw-r--r--   0 runner    (1001) docker     (127)  7395300 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/journal/CPC2007/ganga-GUI.eps
+-rw-r--r--   0 runner    (1001) docker     (127)   127751 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/journal/CPC2007/ganga-GUI.png
+-rw-r--r--   0 runner    (1001) docker     (127)   102543 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/journal/CPC2007/ganga-architecture.png
+-rw-r--r--   0 runner    (1001) docker     (127)    56388 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/journal/CPC2007/ganga-architecture.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)    98876 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/journal/CPC2007/ganga-diane-portal.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    87966 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/journal/CPC2007/ganga-diane-portal.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    31356 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/journal/CPC2007/ganga-diane-portal.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/journal/CPC2007/ganga-objects.dia
+-rw-r--r--   0 runner    (1001) docker     (127)    66244 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/journal/CPC2007/ganga-objects.eps
+-rw-r--r--   0 runner    (1001) docker     (127)    31406 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/journal/CPC2007/ganga-objects.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    75987 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/journal/CPC2007/ganga.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)    26228 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/journal/CPC2007/instructions-num.tex
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/journal/CPC2007/job-uml.dia
+-rw-r--r--   0 runner    (1001) docker     (127)    18329 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/journal/CPC2007/job-uml.eps
+-rw-r--r--   0 runner    (1001) docker     (127)    21022 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/journal/CPC2007/job-uml.png
+-rw-r--r--   0 runner    (1001) docker     (127)   372567 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/journal/CPC2007/monitoring.eps
+-rw-r--r--   0 runner    (1001) docker     (127)   116572 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/journal/CPC2007/monitoring.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)   136823 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/journal/CPC2007/monitoring.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.850207 ganga-8.7.5/doc/manuals/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1856 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.850207 ganga-8.7.5/doc/manuals/html/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      944 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/html/about.dat
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3409 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/html/about.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.854207 ganga-8.7.5/doc/manuals/html/icons/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1958 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/html/icons/blank.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1031 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/html/icons/blank.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      438 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/html/icons/contents.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      649 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/html/icons/contents.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      289 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/html/icons/index.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      529 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/html/icons/index.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      385 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/html/icons/modules.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      598 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/html/icons/modules.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      253 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/html/icons/next.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      511 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/html/icons/next.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      252 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/html/icons/previous.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      511 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/html/icons/previous.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      125 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/html/icons/pyfav.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      316 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/html/icons/up.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      577 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/html/icons/up.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4443 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/html/index.html.in
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1324 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/html/stdabout.dat
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6041 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/html/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.854207 ganga-8.7.5/doc/manuals/perl/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2513 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/perl/SynopsisTable.pm
+-rwxr-xr-x   0 runner    (1001) docker     (127)      405 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/perl/distutils.perl
+-rwxr-xr-x   0 runner    (1001) docker     (127)      242 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/perl/howto.perl
+-rwxr-xr-x   0 runner    (1001) docker     (127)      162 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/perl/isilo.perl
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24053 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/perl/l2hinit.perl
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1921 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/perl/ltxmarkup.perl
+-rwxr-xr-x   0 runner    (1001) docker     (127)      465 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/perl/manual.perl
+-rwxr-xr-x   0 runner    (1001) docker     (127)    62754 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/perl/python.perl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.854207 ganga-8.7.5/doc/manuals/script/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      279 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/script/fiximgpath.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1789 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/script/make-doc.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      469 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/script/makeincl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.806207 ganga-8.7.5/doc/manuals/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.854207 ganga-8.7.5/doc/manuals/src/DocMaker/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3935 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/DocMaker/DocMaker.tex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.866207 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2239 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/Back.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2410 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/Copy.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2492 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/Delete.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2147 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/Download.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1847 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/Folder_AddDocument.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1710 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/Folder_Generic.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2000 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/Folder_New.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2258 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/Folder_Remove.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2297 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/Folder_RemoveDocument.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2037 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/Folder_Rename.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2241 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/Forward.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23577 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/GUI_User_Manual.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2490 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/General_Options.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2509 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/Go.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2504 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/Properties.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2433 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/Refresh.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2251 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/Save.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4504 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/SaveAs_Template.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1959 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/Search.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2225 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/Stop.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1210 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/ToolBtn_Kill.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1328 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/ToolBtn_NewJob.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1397 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/ToolBtn_Remove.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1251 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/ToolBtn_Save.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1328 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/ToolBtn_Submit.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2452 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/View_Doc.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2583 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/Write.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1007 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/browse.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      948 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/files_16x16.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1479 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/files_24x24.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      987 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/files_text_16x16.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1701 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/files_text_24x24.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1333 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/folder_24x24.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1891 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/folder_32x32.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1563 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/folder_down_24x24.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2322 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/folder_down_32x32.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      956 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/gangagui-manual-chapter_1.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3183 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/gangagui-manual-chapter_2.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10990 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/gangagui-manual-chapter_3.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3829 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/gangagui-manual-chapter_4.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3964 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/gangagui-manual-chapter_5.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)       29 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/gangagui-manual-chapter_6.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2656 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/gangagui-manual-contents.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)   120641 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/gangagui_default-view_typical.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7028 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/genericjob_pic_1.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10096 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/genericjob_pic_2.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22429 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/genericjob_pic_3.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (127)    31848 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/genericjob_pic_4.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (127)    37895 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/guiconfig_pic_1.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10919 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/guiconfig_pic_2.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4417 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/guiconfig_pic_3.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (127)    25440 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/guiconfig_pic_4.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2776 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/help.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23577 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/index.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)    41244 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/jobbuilder_pic_1.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5020 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/jobbuilder_pic_2.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11470 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/jobbuilder_pic_3.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11606 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/jobbuilder_pic_4.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9174 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/jobbuilder_pic_5.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24152 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/menubar_pic_1.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7218 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/menubar_pic_2.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9076 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/menubar_pic_3.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (127)    48083 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/monitoring_pic_1.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (127)    26786 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/monitoring_pic_2.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13686 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/monitoring_pic_3.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2140 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/monitoring_pic_4.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1153 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/open.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      993 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/preview.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (127)    62349 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/quickstart_pic_1.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (127)    33800 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/quickstart_pic_2.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17676 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/quickstart_pic_3.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (127)    29133 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/quickstart_pic_4.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (127)    26485 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/quickstart_pic_5.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1254 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/retrieve.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (127)    54473 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/scriptor_pic_1.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (127)    46152 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/splitter_pic_1.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (127)    70724 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/splitter_pic_2.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27847 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GUI_User_Manual/toolbar.jpg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.870207 ganga-8.7.5/doc/manuals/src/GangaIntroduction/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    87638 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/GangaIntroduction/GangaIntroduction.tex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.870207 ganga-8.7.5/doc/manuals/src/LHCb/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    31025 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/LHCb/LHCb.tex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.870207 ganga-8.7.5/doc/manuals/src/dev_survival/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11822 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/dev_survival/dev_survival.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1662 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/dev_survival/makegraph.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10107 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/dev_survival/transient-states.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11362 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/dev_survival/user-states.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.870207 ganga-8.7.5/doc/manuals/src/workbook/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.874207 ganga-8.7.5/doc/manuals/src/workbook/development/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       53 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/workbook/development/architecture.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)       63 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/workbook/development/cvs.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)       51 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/workbook/development/dashboard.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)       61 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/workbook/development/developer.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)      574 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/workbook/development/development.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)       53 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/workbook/development/documentation.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)       77 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/workbook/development/panels.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)       46 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/workbook/development/release.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)       59 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/workbook/development/submission.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)       40 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/workbook/development/test.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)       38 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/workbook/development/twiki.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)       68 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/workbook/development/webpages.tex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.874207 ganga-8.7.5/doc/manuals/src/workbook/extension/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       54 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/workbook/extension/application.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)       45 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/workbook/extension/backend.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)       74 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/workbook/extension/connector.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)       45 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/workbook/extension/dataset.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)      442 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/workbook/extension/extension.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)       44 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/workbook/extension/logging.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)       43 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/workbook/extension/merger.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)       66 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/workbook/extension/parameters.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)       41 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/workbook/extension/plugins.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)       47 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/workbook/extension/splitter.tex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.874207 ganga-8.7.5/doc/manuals/src/workbook/installation/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       51 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/workbook/installation/afs.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)      185 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/workbook/installation/installation.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)       45 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/workbook/installation/local.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)       44 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/workbook/installation/site.tex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.874207 ganga-8.7.5/doc/manuals/src/workbook/introduction/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       59 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/workbook/introduction/functionality.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)      375 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/workbook/introduction/introduction.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)       37 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/workbook/introduction/license.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)       39 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/workbook/introduction/mail.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)       37 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/workbook/introduction/website.tex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.878207 ganga-8.7.5/doc/manuals/src/workbook/usage/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       68 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/workbook/usage/bugs.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)       62 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/workbook/usage/configuration.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)       54 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/workbook/usage/credentials.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)       88 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/workbook/usage/gpi.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)       59 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/workbook/usage/gui.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)       40 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/workbook/usage/help.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)       38 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/workbook/usage/jobs.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)       36 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/workbook/usage/model.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)       48 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/workbook/usage/monitoring.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)       54 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/workbook/usage/operations.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)       46 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/workbook/usage/repository.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)       49 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/workbook/usage/scripts.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)       44 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/workbook/usage/startup.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)       74 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/workbook/usage/statistics.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)      628 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/workbook/usage/usage.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)       44 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/workbook/usage/workspace.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1004 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/src/workbook/workbook.tex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.882207 ganga-8.7.5/doc/manuals/texinputs/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1331 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/texinputs/distutils.sty
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14699 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/texinputs/fancyhdr.sty
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10359 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/texinputs/fncychap.sty
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2797 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/texinputs/howto.cls
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1225 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/texinputs/ltxmarkup.sty
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4440 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/texinputs/manual.cls
+-rwxr-xr-x   0 runner    (1001) docker     (127)      597 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/texinputs/pypaper.sty
+-rwxr-xr-x   0 runner    (1001) docker     (127)      220 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/texinputs/python.ist
+-rwxr-xr-x   0 runner    (1001) docker     (127)    40097 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/texinputs/python.sty
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.886207 ganga-8.7.5/doc/manuals/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2182 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/tools/anno-api.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10526 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/tools/buildindex.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4233 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/tools/checkargs.pm
+-rwxr-xr-x   0 runner    (1001) docker     (127)      661 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/tools/cklatex
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2154 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/tools/custlib.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2434 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/tools/cvsinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4029 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/tools/findacks
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3660 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/tools/findcsyms
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1806 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/tools/findmodrefs
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3937 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/tools/findsyms
+-rwxr-xr-x   0 runner    (1001) docker     (127)       86 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/tools/fix_hack
+-rwxr-xr-x   0 runner    (1001) docker     (127)      107 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/tools/fix_libaux.sed
+-rwxr-xr-x   0 runner    (1001) docker     (127)      441 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/tools/fixinfo.el
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2900 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/tools/getpagecounts
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1847 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/tools/getversioninfo
+-rwxr-xr-x   0 runner    (1001) docker     (127)    58169 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/tools/html2texi.pl
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2301 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/tools/indfix.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      365 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/tools/keywords.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5283 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/tools/listmodules
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3438 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/tools/makesec.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1739 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/tools/mkackshtml
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24033 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/tools/mkhowto
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1552 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/tools/mkinfo
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4819 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/tools/mkmodindex
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2338 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/tools/mkpkglist
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5884 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/tools/mksourcepkg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1944 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/tools/node2label.pl
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15832 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/tools/prechm.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1987 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/tools/push-docs.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)    31256 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/tools/py2texi.el
+-rwxr-xr-x   0 runner    (1001) docker     (127)   786944 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/tools/python
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2316 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/tools/refcounts.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1366 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/tools/rewrite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.890207 ganga-8.7.5/doc/manuals/tools/sgmlconv/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1298 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/tools/sgmlconv/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2387 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/tools/sgmlconv/README
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23495 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/tools/sgmlconv/conversion.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)    37241 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/tools/sgmlconv/docfixer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7269 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/tools/sgmlconv/esis2sgml.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9228 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/tools/sgmlconv/esistools.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19936 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/tools/sgmlconv/latex2esis.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1098 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/tools/sgmlconv/make.rules
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6704 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/tools/support.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3949 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/tools/toc2bkm.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2528 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/tools/undoc_symbols.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      713 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/tools/update-docs.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)       85 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/manuals/tools/whichlibs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.890207 ganga-8.7.5/doc/sysadmin/
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/sysadmin/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.890207 ganga-8.7.5/doc/work/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5697 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/work/lifetime.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6855 2024-04-05 11:20:46.000000 ganga-8.7.5/doc/work/splitting.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.890207 ganga-8.7.5/ganga/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.890207 ganga-8.7.5/ganga/GangaCore/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.890207 ganga-8.7.5/ganga/GangaCore/Core/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10903 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Core/FileWorkspace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.894207 ganga-8.7.5/ganga/GangaCore/Core/GangaRepository/
+-rw-r--r--   0 runner    (1001) docker     (127)    12780 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Core/GangaRepository/DStreamer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25943 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Core/GangaRepository/DatabaseRegistry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Core/GangaRepository/FixedLock.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11096 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Core/GangaRepository/GangaRepository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9354 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Core/GangaRepository/GangaRepositoryCentral.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36640 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Core/GangaRepository/GangaRepositoryDatabase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Core/GangaRepository/GangaRepositoryImmutableTransient.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    54032 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Core/GangaRepository/GangaRepositoryXML.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Core/GangaRepository/PickleStreamer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27240 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Core/GangaRepository/Registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35399 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Core/GangaRepository/SessionLock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19363 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Core/GangaRepository/SubJobJsonList.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26908 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Core/GangaRepository/SubJobXMLList.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17812 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Core/GangaRepository/VStreamer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1146 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Core/GangaRepository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21734 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Core/GangaRepository/container_controllers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Core/GangaRepository/migrate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.894207 ganga-8.7.5/ganga/GangaCore/Core/GangaThread/
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Core/GangaThread/GangaThread.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11080 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Core/GangaThread/GangaThreadPool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.894207 ganga-8.7.5/ganga/GangaCore/Core/GangaThread/MTRunner/
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Core/GangaThread/MTRunner/Algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Core/GangaThread/MTRunner/Data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5549 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Core/GangaThread/MTRunner/MTRunner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Core/GangaThread/MTRunner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.894207 ganga-8.7.5/ganga/GangaCore/Core/GangaThread/WorkerThreads/
+-rw-r--r--   0 runner    (1001) docker     (127)    16573 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Core/GangaThread/WorkerThreads/ThreadPoolQueueMonitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12615 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Core/GangaThread/WorkerThreads/WorkerThreadPool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Core/GangaThread/WorkerThreads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Core/GangaThread/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.894207 ganga-8.7.5/ganga/GangaCore/Core/InternalServices/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9171 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Core/InternalServices/Coordinator.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5638 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Core/InternalServices/ShutdownManager.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Core/InternalServices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.898208 ganga-8.7.5/ganga/GangaCore/Core/MonitoringComponent/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    54951 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Core/MonitoringComponent/Local_GangaMC_Service.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4521 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Core/MonitoringComponent/Monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9425 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Core/MonitoringComponent/MonitoringService.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       28 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Core/MonitoringComponent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.898208 ganga-8.7.5/ganga/GangaCore/Core/Sandbox/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5281 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Core/Sandbox/Sandbox.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4265 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Core/Sandbox/WNSandbox.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      281 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Core/Sandbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Core/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6146 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Core/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.898208 ganga-8.7.5/ganga/GangaCore/GPI/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       28 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPI/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.898208 ganga-8.7.5/ganga/GangaCore/GPIDev/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.898208 ganga-8.7.5/ganga/GangaCore/GPIDev/Adapters/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1872 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Adapters/ApplicationRuntimeHandlers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5528 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Adapters/IApplication.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21380 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Adapters/IBackend.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3412 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Adapters/IChecker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9536 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Adapters/ICredentialInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Adapters/ICredentialRequirement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9973 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Adapters/IGangaFile.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9100 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Adapters/IMerger.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3918 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Adapters/IMonitoringService.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6228 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Adapters/IPostProcessor.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10624 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Adapters/IPrepareApp.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2110 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Adapters/IRuntimeHandler.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3121 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Adapters/ISplitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Adapters/IVirtualization.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7579 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Adapters/StandardJobConfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      156 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.902207 ganga-8.7.5/ganga/GangaCore/GPIDev/Base/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4315 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Base/Filters.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    59985 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Base/Objects.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    53774 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Base/Proxy.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12619 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Base/VPrinter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5177 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Base/VPrinterOld.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      350 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.902207 ganga-8.7.5/ganga/GangaCore/GPIDev/Credentials/
+-rw-r--r--   0 runner    (1001) docker     (127)     5718 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Credentials/AfsToken.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12949 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Credentials/CredentialStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7443 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Credentials/VomsProxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Credentials/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.902207 ganga-8.7.5/ganga/GangaCore/GPIDev/Credentials_old/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20594 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Credentials_old/ICredential.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3369 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Credentials_old/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.902207 ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.902207 ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/Config/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11717 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/Config/Config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       52 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/Config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.902207 ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/Dataset/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1063 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/Dataset/Dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5984 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/Dataset/GangaDataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       69 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/Dataset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.906207 ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/File/
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/File/Configure.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17376 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/File/File.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2878 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/File/FileBuffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/File/FileUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24411 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/File/GoogleFile.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11639 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/File/LocalFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26379 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/File/MassStorageFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12947 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/File/OutputFileManager.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3257 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/File/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.906207 ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/File/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/File/scripts/LCGSEFileWNScript.py.template
+-rw-r--r--   0 runner    (1001) docker     (127)     4324 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/File/scripts/MassStorageFileWNScript.py.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.906207 ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/GangaList/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    26733 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/GangaList/GangaList.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       38 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/GangaList/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.906207 ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/Job/
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/Job/Error.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)   121942 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/Job/Job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/Job/JobInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18975 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/Job/JobTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/Job/MetadataDict.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      231 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/Job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/Job/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.906207 ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/JobTree/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15970 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/JobTree/JobTree.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      292 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/JobTree/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.906207 ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/Registry/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8979 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/Registry/BoxRegistry.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14541 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/Registry/JobRegistry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27539 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/Registry/PrepRegistry.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21459 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/Registry/RegistrySlice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/Registry/RegistrySliceProxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/Registry/RegistryUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4432 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/Registry/TransientRegistry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/Registry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.910207 ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/Tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/Tasks/CoreTask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7215 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/Tasks/CoreTransform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/Tasks/CoreUnit.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12904 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/Tasks/ITask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28090 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/Tasks/ITransform.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19618 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/Tasks/IUnit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/Tasks/TaskChainInput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/Tasks/TaskLocalCopy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22780 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/Tasks/TaskRegistry.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      739 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/Tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/Tasks/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.910207 ganga-8.7.5/ganga/GangaCore/GPIDev/MonitoringServices/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10221 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/MonitoringServices/Composite.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4801 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/MonitoringServices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.910207 ganga-8.7.5/ganga/GangaCore/GPIDev/Persistency/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7887 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Persistency/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.910207 ganga-8.7.5/ganga/GangaCore/GPIDev/Schema/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    32271 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Schema/Schema.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      130 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/Schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/TypeCheck.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      106 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/GPIDev/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.910207 ganga-8.7.5/ganga/GangaCore/Lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.910207 ganga-8.7.5/ganga/GangaCore/Lib/Batch/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    25180 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Lib/Batch/Batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Lib/Batch/BatchScriptTemplate.py.template
+-rwxr-xr-x   0 runner    (1001) docker     (127)      128 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Lib/Batch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.910207 ganga-8.7.5/ganga/GangaCore/Lib/Checkers/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2335 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Lib/Checkers/CustomChecker.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2822 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Lib/Checkers/FileChecker.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2099 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Lib/Checkers/MetaDataChecker.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6964 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Lib/Checkers/RootFileChecker.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      169 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Lib/Checkers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.914208 ganga-8.7.5/ganga/GangaCore/Lib/Condor/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    29396 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Lib/Condor/Condor.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4609 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Lib/Condor/CondorRequirements.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      566 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Lib/Condor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.914208 ganga-8.7.5/ganga/GangaCore/Lib/Executable/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13956 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Lib/Executable/Executable.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      149 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Lib/Executable/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.914208 ganga-8.7.5/ganga/GangaCore/Lib/Interactive/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11328 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Lib/Interactive/Interactive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Lib/Interactive/InteractiveScriptTemplate.py.template
+-rwxr-xr-x   0 runner    (1001) docker     (127)      530 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Lib/Interactive/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.914208 ganga-8.7.5/ganga/GangaCore/Lib/Localhost/
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Lib/Localhost/LocalHostExec.py.template
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Lib/Localhost/LocalHostExec_batch.py.template
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17498 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Lib/Localhost/Localhost.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       34 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Lib/Localhost/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.914208 ganga-8.7.5/ganga/GangaCore/Lib/Mergers/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15780 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Lib/Mergers/Merger.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       44 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Lib/Mergers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.914208 ganga-8.7.5/ganga/GangaCore/Lib/Notebook/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7136 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Lib/Notebook/Notebook.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       32 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Lib/Notebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Lib/Notebook/wrapperNotebookTemplate.py.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.914208 ganga-8.7.5/ganga/GangaCore/Lib/Notifier/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2823 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Lib/Notifier/Notifier.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       32 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Lib/Notifier/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.914208 ganga-8.7.5/ganga/GangaCore/Lib/Remote/
+-rw-r--r--   0 runner    (1001) docker     (127)    32668 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Lib/Remote/Remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Lib/Remote/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.918208 ganga-8.7.5/ganga/GangaCore/Lib/Splitters/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4294 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Lib/Splitters/ArgSplitter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1628 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Lib/Splitters/DefaultSplitter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1466 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Lib/Splitters/ExeSplitter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2450 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Lib/Splitters/GangaDatasetSplitter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5491 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Lib/Splitters/GenericSplitter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      223 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Lib/Splitters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.918208 ganga-8.7.5/ganga/GangaCore/Lib/Virtualization/
+-rw-r--r--   0 runner    (1001) docker     (127)     6491 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Lib/Virtualization/Apptainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4884 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Lib/Virtualization/Docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6638 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Lib/Virtualization/Singularity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Lib/Virtualization/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Lib/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6001 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/PACKAGE.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.918208 ganga-8.7.5/ganga/GangaCore/Runtime/
+-rw-r--r--   0 runner    (1001) docker     (127)     4511 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Runtime/GPIFunctions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Runtime/GPIexport.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17289 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Runtime/GangaCompleter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Runtime/HEAD_CONFIG.INI
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Runtime/IPythonMagic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11576 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Runtime/Repository_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Runtime/Workspace_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65064 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Runtime/bootstrap.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12710 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Runtime/eliza.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Runtime/ganga_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7608 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Runtime/gangadoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Runtime/gangadoceval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Runtime/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.922207 ganga-8.7.5/ganga/GangaCore/Utility/
+-rw-r--r--   0 runner    (1001) docker     (127)     7348 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Utility/ColourText.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.922207 ganga-8.7.5/ganga/GangaCore/Utility/Config/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       51 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Utility/Config/A.ini
+-rwxr-xr-x   0 runner    (1001) docker     (127)       68 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Utility/Config/B.ini
+-rw-r--r--   0 runner    (1001) docker     (127)    43719 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Utility/Config/Config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       41 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Utility/Config/ConfigTest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Utility/Config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Utility/Config/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Utility/Decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Utility/GridShell.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.922207 ganga-8.7.5/ganga/GangaCore/Utility/Plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)     4887 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Utility/Plugin/GangaPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Utility/Plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Utility/Profiling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14300 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Utility/Runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6993 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Utility/Setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12520 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Utility/Shell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Utility/Virtualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11319 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Utility/execute.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.922207 ganga-8.7.5/ganga/GangaCore/Utility/external/
+-rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Utility/external/OrderedDict.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Utility/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26942 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Utility/feedback_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Utility/files.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.922207 ganga-8.7.5/ganga/GangaCore/Utility/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)    21901 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Utility/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Utility/logging/message_caching_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Utility/logging/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Utility/logic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8018 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Utility/root.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Utility/stacktracer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Utility/strings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Utility/threads.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9868 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/Utility/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51841 2024-04-05 11:20:56.000000 ganga-8.7.5/ganga/GangaCore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.922207 ganga-8.7.5/ganga/GangaCore/old_test/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.922207 ganga-8.7.5/ganga/GangaCore/old_test/Bugs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.926207 ganga-8.7.5/ganga/GangaCore/old_test/Bugs/Savannah10013/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       72 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/old_test/Bugs/Savannah10013/Savannah10013.ini
+-rwxr-xr-x   0 runner    (1001) docker     (127)       92 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/old_test/Bugs/Savannah17638.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.926207 ganga-8.7.5/ganga/GangaCore/old_test/Bugs/Savannah23737/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       28 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/old_test/Bugs/Savannah23737/Savannah23737.ini
+-rwxr-xr-x   0 runner    (1001) docker     (127)       31 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/old_test/Bugs/Savannah32201.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/old_test/Bugs/Savannah36651.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.926207 ganga-8.7.5/ganga/GangaCore/old_test/GPI/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       44 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/old_test/GPI/BackendApplicationMatrix.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/old_test/GPI/CompressOutput.ini
+-rwxr-xr-x   0 runner    (1001) docker     (127)      115 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/old_test/GPI/ConfigFile.ini
+-rwxr-xr-x   0 runner    (1001) docker     (127)      751 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/old_test/GPI/ConfigObject.ini
+-rwxr-xr-x   0 runner    (1001) docker     (127)      625 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/old_test/GPI/ConfigUser.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/old_test/GPI/LCG.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.926207 ganga-8.7.5/ganga/GangaCore/old_test/GPI/Mergers/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      418 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/old_test/GPI/Mergers/TestRootMerger.ini
+-rwxr-xr-x   0 runner    (1001) docker     (127)      141 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/old_test/GPI/Mergers/TestTextMerger.ini
+-rwxr-xr-x   0 runner    (1001) docker     (127)      140 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/old_test/GPI/Mergers/TestTextMergerGzip.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.926207 ganga-8.7.5/ganga/GangaCore/old_test/GPI/MigrationFramework/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       36 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/old_test/GPI/MigrationFramework/MigrationFramework.ini
+-rwxr-xr-x   0 runner    (1001) docker     (127)       75 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/old_test/GPI/MigrationFramework/MigrationFramework.pass1.ini
+-rwxr-xr-x   0 runner    (1001) docker     (127)       74 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/old_test/GPI/MigrationFramework/MigrationFramework.pass2.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/old_test/GPI/MonTest.ini
+-rwxr-xr-x   0 runner    (1001) docker     (127)       28 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/old_test/GPI/MonitoringServices.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.930208 ganga-8.7.5/ganga/GangaCore/old_test/GPI/OutputFiles/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesBatch.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesBatchMultipleFilesForLCGUpload.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesBatchMultipleFilesForMassStorageAndLCGUpload.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesBatchMultipleFilesForMassStorageUpload.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesCompressedBatch.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesCompressedLocal.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesInteractive.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesInteractiveMultipleFilesForLCGUpload.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesInteractiveMultipleFilesForPattern.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesLCG.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesLCGMultipleCompressedFilesForMassStorageAndLCGUpload.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesLocal.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesLocalMultipleFilesForLCGUpload.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesLocalMultipleFilesForPattern.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesMixedBatch.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/old_test/GPI/RegistrySorting.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.930208 ganga-8.7.5/ganga/GangaCore/old_test/GPI/ResubmitSubjobs/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       28 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/old_test/GPI/ResubmitSubjobs/ResubmitSubjobs.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.930208 ganga-8.7.5/ganga/GangaCore/old_test/GPI/Root/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      299 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/old_test/GPI/Root/TestRoot.ini
+-rwxr-xr-x   0 runner    (1001) docker     (127)       48 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/old_test/GPI/WorkspaceRemoval.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.930208 ganga-8.7.5/ganga/GangaCore/old_test/GPI/auto_resubmit/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/old_test/GPI/auto_resubmit/auto_resubmit.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.930208 ganga-8.7.5/ganga/GangaCore/old_test/Internals/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/old_test/Internals/TestGridProxyExpandSystemVars.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.930208 ganga-8.7.5/ganga/GangaCore/old_test/Performance/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      184 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/old_test/Performance/PerfStats.ini
+-rwxr-xr-x   0 runner    (1001) docker     (127)      101 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/old_test/Performance/TimeJobs.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.930208 ganga-8.7.5/ganga/GangaCore/old_test/XMLRepository/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       47 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/old_test/XMLRepository/SpecialName.ini
+-rwxr-xr-x   0 runner    (1001) docker     (127)      642 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/old_test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.930208 ganga-8.7.5/ganga/GangaCore/old_test/config/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1195 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/old_test/config/Schema.ini
+-rwxr-xr-x   0 runner    (1001) docker     (127)      793 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/old_test/config/default.ini
+-rwxr-xr-x   0 runner    (1001) docker     (127)      793 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/old_test/config/localxml.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.814207 ganga-8.7.5/ganga/GangaCore/test/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.814207 ganga-8.7.5/ganga/GangaCore/test/GPI/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.930208 ganga-8.7.5/ganga/GangaCore/test/GPI/Config/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       50 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/test/GPI/Config/A.ini
+-rwxr-xr-x   0 runner    (1001) docker     (127)       54 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/test/GPI/Config/B.ini
+-rwxr-xr-x   0 runner    (1001) docker     (127)       40 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/test/GPI/Config/ConfigTest.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.930208 ganga-8.7.5/ganga/GangaCore/test/GPI/Notebook/
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/test/GPI/Notebook/Test.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.930208 ganga-8.7.5/ganga/GangaCore/testlib/
+-rw-r--r--   0 runner    (1001) docker     (127)    12196 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/testlib/GangaUnitTest.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/testlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/testlib/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/testlib/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/testlib/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/testlib/mark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaCore/testlib/monitoring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.934208 ganga-8.7.5/ganga/GangaDirac/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7275 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaDirac/BOOT.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaDirac/Dirac.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.934208 ganga-8.7.5/ganga/GangaDirac/Lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.934208 ganga-8.7.5/ganga/GangaDirac/Lib/Backends/
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaDirac/Lib/Backends/Dirac.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75705 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaDirac/Lib/Backends/DiracBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9633 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaDirac/Lib/Backends/DiracUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaDirac/Lib/Backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.934208 ganga-8.7.5/ganga/GangaDirac/Lib/Credentials/
+-rw-r--r--   0 runner    (1001) docker     (127)     8772 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaDirac/Lib/Credentials/DiracProxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaDirac/Lib/Credentials/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.934208 ganga-8.7.5/ganga/GangaDirac/Lib/Files/
+-rw-r--r--   0 runner    (1001) docker     (127)    39938 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaDirac/Lib/Files/DiracFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaDirac/Lib/Files/WNInjectTemplate.py.template
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaDirac/Lib/Files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaDirac/Lib/Files/downloadScript.py.template
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaDirac/Lib/Files/uploadScript.py.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.934208 ganga-8.7.5/ganga/GangaDirac/Lib/RTHandlers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaDirac/Lib/RTHandlers/DiracRTHScript.py.template
+-rw-r--r--   0 runner    (1001) docker     (127)     9914 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaDirac/Lib/RTHandlers/DiracRTHUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10397 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaDirac/Lib/RTHandlers/ExeDiracRTHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7472 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaDirac/Lib/RTHandlers/RunTimeHandlerUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaDirac/Lib/RTHandlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.938207 ganga-8.7.5/ganga/GangaDirac/Lib/Server/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaDirac/Lib/Server/BlankCommands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18388 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaDirac/Lib/Server/DiracCommands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaDirac/Lib/Server/DiracDefinition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaDirac/Lib/Server/DiracExecutorProcess.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20454 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaDirac/Lib/Server/DiracNewCommands.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2266 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaDirac/Lib/Server/DiracOldProcess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaDirac/Lib/Server/DiracProcessManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaDirac/Lib/Server/InspectionClient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaDirac/Lib/Server/InspectionServer.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaDirac/Lib/Server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.938207 ganga-8.7.5/ganga/GangaDirac/Lib/Splitters/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3253 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaDirac/Lib/Splitters/GangaSplitterUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24738 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaDirac/Lib/Splitters/OfflineGangaDiracSplitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaDirac/Lib/Splitters/SplitterUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaDirac/Lib/Splitters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.938207 ganga-8.7.5/ganga/GangaDirac/Lib/Utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)    12049 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaDirac/Lib/Utilities/DiracUtilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaDirac/Lib/Utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaDirac/Lib/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      665 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaDirac/PACKAGE.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9416 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaDirac/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.814207 ganga-8.7.5/ganga/GangaDirac/old_test/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.814207 ganga-8.7.5/ganga/GangaDirac/old_test/GPI/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.938207 ganga-8.7.5/ganga/GangaDirac/old_test/GPI/Files/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaDirac/old_test/GPI/Files/TestDiracFile.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.814207 ganga-8.7.5/ganga/GangaDirac/old_test/Lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.938207 ganga-8.7.5/ganga/GangaDirac/old_test/Lib/RTHandlers/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaDirac/old_test/Lib/RTHandlers/TestExeDiracRTHandler.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.938207 ganga-8.7.5/ganga/GangaGaudi/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaGaudi/Gaudi.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.938207 ganga-8.7.5/ganga/GangaGaudi/Lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.938207 ganga-8.7.5/ganga/GangaGaudi/Lib/Applications/
+-rw-r--r--   0 runner    (1001) docker     (127)     5645 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaGaudi/Lib/Applications/CMTUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8152 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaGaudi/Lib/Applications/Gaudi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11669 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaGaudi/Lib/Applications/GaudiBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8147 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaGaudi/Lib/Applications/GaudiUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5305 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaGaudi/Lib/Applications/GaudiXMLSummary.py
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaGaudi/Lib/Applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaGaudi/Lib/Applications/cmakeUtils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.938207 ganga-8.7.5/ganga/GangaGaudi/Lib/Checkers/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2848 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaGaudi/Lib/Checkers/GaudiMetaDataChecker.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaGaudi/Lib/Checkers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.938207 ganga-8.7.5/ganga/GangaGaudi/Lib/Datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaGaudi/Lib/Datasets/GaudiDataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaGaudi/Lib/Datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.942208 ganga-8.7.5/ganga/GangaGaudi/Lib/RTHandlers/
+-rw-r--r--   0 runner    (1001) docker     (127)     5599 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaGaudi/Lib/RTHandlers/GaudiDiracRunTimeHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaGaudi/Lib/RTHandlers/GaudiRunTimeHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaGaudi/Lib/RTHandlers/RunTimeHandlerUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaGaudi/Lib/RTHandlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.942208 ganga-8.7.5/ganga/GangaGaudi/Lib/Splitters/
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaGaudi/Lib/Splitters/GaudiInputDataSplitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaGaudi/Lib/Splitters/SplitterUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaGaudi/Lib/Splitters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.942208 ganga-8.7.5/ganga/GangaGaudi/Lib/XMLSummary/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaGaudi/Lib/XMLSummary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64665 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaGaudi/Lib/XMLSummary/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25090 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaGaudi/Lib/XMLSummary/summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaGaudi/Lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaGaudi/PACKAGE.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaGaudi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.942208 ganga-8.7.5/ganga/GangaLHCb/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4251 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/BOOT.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2067 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/LHCb.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.942208 ganga-8.7.5/ganga/GangaLHCb/Lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.946208 ganga-8.7.5/ganga/GangaLHCb/Lib/Applications/
+-rw-r--r--   0 runner    (1001) docker     (127)    14127 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/Lib/Applications/AppsBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/Lib/Applications/AppsBaseUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8806 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/Lib/Applications/Bender.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24468 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/Lib/Applications/BenderBox.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13997 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/Lib/Applications/BenderScript.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3409 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/Lib/Applications/CMTscript.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/Lib/Applications/EnvironFunctions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/Lib/Applications/FileFunctions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    31734 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/Lib/Applications/GaudiExec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7845 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/Lib/Applications/GaudiExecUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/Lib/Applications/GaudiPython.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12134 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/Lib/Applications/Ostap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10481 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/Lib/Applications/PythonOptionsParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4796 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/Lib/Applications/PythonOptsCmakeParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/Lib/Applications/XMLPostProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/Lib/Applications/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.946208 ganga-8.7.5/ganga/GangaLHCb/Lib/Backends/
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/Lib/Backends/Bookkeeping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5008 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/Lib/Backends/Dirac.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/Lib/Backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.946208 ganga-8.7.5/ganga/GangaLHCb/Lib/Checkers/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2862 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/Lib/Checkers/LHCbMetadataChecker.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/Lib/Checkers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.946208 ganga-8.7.5/ganga/GangaLHCb/Lib/Files/
+-rw-r--r--   0 runner    (1001) docker     (127)     4419 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/Lib/Files/LogicalFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/Lib/Files/PhysicalFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/Lib/Files/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.946208 ganga-8.7.5/ganga/GangaLHCb/Lib/LHCbDataset/
+-rw-r--r--   0 runner    (1001) docker     (127)    13473 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/Lib/LHCbDataset/BKQuery.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19914 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/Lib/LHCbDataset/LHCbCompressedDataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23063 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/Lib/LHCbDataset/LHCbDataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/Lib/LHCbDataset/LHCbDatasetUtils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      192 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/Lib/LHCbDataset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.946208 ganga-8.7.5/ganga/GangaLHCb/Lib/Mergers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/Lib/Mergers/CMTVersion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11090 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/Lib/Mergers/GaudiExecMerger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/Lib/Mergers/LHCbFileMerger.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/Lib/Mergers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.950208 ganga-8.7.5/ganga/GangaLHCb/Lib/RTHandlers/
+-rw-r--r--   0 runner    (1001) docker     (127)    10771 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/Lib/RTHandlers/ExeDiracRTHandler.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    35150 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/Lib/RTHandlers/GaudiExecRTHandlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/Lib/RTHandlers/GaudiTemplate.py.template
+-rw-r--r--   0 runner    (1001) docker     (127)    11732 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/Lib/RTHandlers/LHCbGaudiDiracRunTimeHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6431 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/Lib/RTHandlers/LHCbGaudiRunTimeHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4345 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/Lib/RTHandlers/RTHUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/Lib/RTHandlers/WorkerScript.py.template
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/Lib/RTHandlers/XMLWorkerScript.py.template
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/Lib/RTHandlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.950208 ganga-8.7.5/ganga/GangaLHCb/Lib/Server/
+-rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/Lib/Server/DiracLHCbCommands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/Lib/Server/DiracLHCbDefinition.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/Lib/Server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.950208 ganga-8.7.5/ganga/GangaLHCb/Lib/Splitters/
+-rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/Lib/Splitters/GaussSplitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/Lib/Splitters/LHCbSplitterUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/Lib/Splitters/OptionsFileSplitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10998 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/Lib/Splitters/SplitByFiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6235 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/Lib/Splitters/SplitFilesBySize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/Lib/Splitters/TestSplitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/Lib/Splitters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.950208 ganga-8.7.5/ganga/GangaLHCb/Lib/Tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/Lib/Tasks/BKTestQuery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/Lib/Tasks/LHCbTask.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/Lib/Tasks/LHCbTaskDummySplitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12584 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/Lib/Tasks/LHCbTransform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4975 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/Lib/Tasks/LHCbUnit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/Lib/Tasks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.950208 ganga-8.7.5/ganga/GangaLHCb/Lib/XMLSummary/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/Lib/XMLSummary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64685 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/Lib/XMLSummary/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25050 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/Lib/XMLSummary/summary.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/Lib/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      665 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/PACKAGE.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.950208 ganga-8.7.5/ganga/GangaLHCb/Utility/
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/Utility/LHCbDIRACenv.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/Utility/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8960 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.950208 ganga-8.7.5/ganga/GangaLHCb/testlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaLHCb/testlib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.950208 ganga-8.7.5/ganga/GangaND280/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaND280/BOOT.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.954208 ganga-8.7.5/ganga/GangaND280/Highland/
+-rw-r--r--   0 runner    (1001) docker     (127)     7061 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaND280/Highland/Highland.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       24 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaND280/Highland/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaND280/ND280.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.954208 ganga-8.7.5/ganga/GangaND280/ND280Checkers/
+-rw-r--r--   0 runner    (1001) docker     (127)    19378 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaND280/ND280Checkers/ND280Checker.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       56 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaND280/ND280Checkers/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9075 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaND280/ND280Checkers/post_status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.954208 ganga-8.7.5/ganga/GangaND280/ND280Control/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27283 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaND280/ND280Control/ND280Configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaND280/ND280Control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8913 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaND280/ND280Control/runND280.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8252 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaND280/ND280Control/runND280CosMC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9047 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaND280/ND280Control/runND280CtrlSmpl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7472 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaND280/ND280Control/runND280Kin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8519 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaND280/ND280Control/runND280RDP.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaND280/ND280Control/runND280SandMC.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.954208 ganga-8.7.5/ganga/GangaND280/ND280Dataset/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8427 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaND280/ND280Dataset/ND280Dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       39 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaND280/ND280Dataset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.954208 ganga-8.7.5/ganga/GangaND280/ND280Executable/
+-rw-r--r--   0 runner    (1001) docker     (127)     7662 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaND280/ND280Executable/ND280Executable.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       31 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaND280/ND280Executable/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.954208 ganga-8.7.5/ganga/GangaND280/ND280RecoValidation/
+-rw-r--r--   0 runner    (1001) docker     (127)    10903 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaND280/ND280RecoValidation/RecoPlusVFT.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12950 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaND280/ND280RecoValidation/VFT_make_ana.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       92 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaND280/ND280RecoValidation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9922 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaND280/ND280RecoValidation/oaReconPlusoaAnalysis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.954208 ganga-8.7.5/ganga/GangaND280/ND280Skimmer/
+-rw-r--r--   0 runner    (1001) docker     (127)     8638 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaND280/ND280Skimmer/ND280Skimmer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       28 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaND280/ND280Skimmer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.954208 ganga-8.7.5/ganga/GangaND280/ND280Splitter/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8589 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaND280/ND280Splitter/ND280Splitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaND280/ND280Splitter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.958208 ganga-8.7.5/ganga/GangaND280/ND280TPCGasInteractions/
+-rw-r--r--   0 runner    (1001) docker     (127)     9046 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaND280/ND280TPCGasInteractions/TRExPlusOAAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaND280/ND280TPCGasInteractions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaND280/PACKAGE.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.958208 ganga-8.7.5/ganga/GangaND280/Tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaND280/Tasks/ND280Task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6520 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaND280/Tasks/ND280Transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaND280/Tasks/ND280Transform_CSVEvtList.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaND280/Tasks/ND280Unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaND280/Tasks/ND280Unit_CSVEvtList.py
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaND280/Tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaND280/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.962208 ganga-8.7.5/ganga/GangaRelease/
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaRelease/ReleaseNotes
+-rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-7.0.0
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-7.0.1
+-rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-7.0.2
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-7.0.3
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-7.0.4
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-7.1.0
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-7.1.1
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-7.1.10
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-7.1.11
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-7.1.12
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-7.1.13
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-7.1.14
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-7.1.15
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-7.1.2
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-7.1.3
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-7.1.4
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-7.1.5
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-7.1.6
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-7.1.7
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-7.1.8
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-7.1.9
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-8.0.0
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-8.0.1
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-8.0.2
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-8.0.3
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-8.1.0
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-8.2.0
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-8.2.1
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-8.2.2
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-8.2.3
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-8.2.4
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-8.3.0
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-8.3.1
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-8.3.2
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-8.3.3
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-05 11:20:56.000000 ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-8.7.5
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.962208 ganga-8.7.5/ganga/GangaRelease/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaRelease/tools/check-new-ganga.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaRelease/tools/ganga-cvmfs-install-dev.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaRelease/tools/ganga-cvmfs-install.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.962208 ganga-8.7.5/ganga/GangaTest/
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaTest/BOOT.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.966208 ganga-8.7.5/ganga/GangaTest/Framework/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       34 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaTest/Framework/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18555 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaTest/Framework/driver.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    31840 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaTest/Framework/htmlizer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    47550 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaTest/Framework/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9026 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaTest/Framework/runner.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11385 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaTest/Framework/tests.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4149 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaTest/Framework/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13506 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaTest/Framework/xmldifferencer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.966208 ganga-8.7.5/ganga/GangaTest/Lib/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4013 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaTest/Lib/CrashTest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.966208 ganga-8.7.5/ganga/GangaTest/Lib/GListApp/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2803 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaTest/Lib/GListApp/GListApp.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      485 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaTest/Lib/GListApp/PACKAGE.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       32 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaTest/Lib/GListApp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.966208 ganga-8.7.5/ganga/GangaTest/Lib/RTHandlers/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaTest/Lib/RTHandlers/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3277 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaTest/Lib/StoreTestFramework.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.966208 ganga-8.7.5/ganga/GangaTest/Lib/TFile/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      485 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaTest/Lib/TFile/PACKAGE.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1485 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaTest/Lib/TFile/TFile.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       26 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaTest/Lib/TFile/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.966208 ganga-8.7.5/ganga/GangaTest/Lib/TestApplication/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5553 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaTest/Lib/TestApplication/TestApplication.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1283 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaTest/Lib/TestApplication/TestDataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      100 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaTest/Lib/TestApplication/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.966208 ganga-8.7.5/ganga/GangaTest/Lib/TestMonitoringService/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      865 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaTest/Lib/TestMonitoringService/TestMonitoringService.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       37 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaTest/Lib/TestMonitoringService/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaTest/Lib/TestObjects.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.966208 ganga-8.7.5/ganga/GangaTest/Lib/TestRemoteBackend/
+-rw-r--r--   0 runner    (1001) docker     (127)    18622 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaTest/Lib/TestRemoteBackend/TestRemoteBackend.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaTest/Lib/TestRemoteBackend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaTest/Lib/TestRemoteBackend/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.966208 ganga-8.7.5/ganga/GangaTest/Lib/TestSubmitter/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      386 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaTest/Lib/TestSubmitter/TestConfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1219 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaTest/Lib/TestSubmitter/TestConfig2.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1363 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaTest/Lib/TestSubmitter/TestSplitter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3498 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaTest/Lib/TestSubmitter/TestSubmitter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      176 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaTest/Lib/TestSubmitter/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      325 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaTest/Lib/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      952 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaTest/PACKAGE.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.966208 ganga-8.7.5/ganga/GangaTest/TestGPIP/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      153 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaTest/TestGPIP/TestGPIP.ini
+-rwxr-xr-x   0 runner    (1001) docker     (127)      448 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaTest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.970208 ganga-8.7.5/ganga/GangaTutorial/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      649 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaTutorial/BOOT.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.970208 ganga-8.7.5/ganga/GangaTutorial/Lib/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6722 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaTutorial/Lib/PrimeFactorizer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2258 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaTutorial/Lib/PrimeFactorizerSplitter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2287 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaTutorial/Lib/PrimeTableDataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      103 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaTutorial/Lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.970208 ganga-8.7.5/ganga/GangaTutorial/Lib/primes/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaTutorial/Lib/primes/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3020 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaTutorial/Lib/primes/prime_factor.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2158 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaTutorial/Lib/primes/primes.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      894 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaTutorial/PACKAGE.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       45 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaTutorial/Tutorial.ini
+-rwxr-xr-x   0 runner    (1001) docker     (127)      202 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/GangaTutorial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.970208 ganga-8.7.5/ganga/ganga/
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/ganga/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-05 11:20:46.000000 ganga-8.7.5/ganga/submit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:20:57.970208 ganga-8.7.5/ganga.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-05 11:20:57.000000 ganga-8.7.5/ganga.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    35759 2024-04-05 11:20:57.000000 ganga-8.7.5/ganga.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 11:20:57.000000 ganga-8.7.5/ganga.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-05 11:20:57.000000 ganga-8.7.5/ganga.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-05 11:20:57.000000 ganga-8.7.5/ganga.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-05 11:20:57.970208 ganga-8.7.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-04-05 11:20:56.000000 ganga-8.7.5/setup.py
```

### Comparing `ganga-8.7.4/LICENSE_GPL` & `ganga-8.7.5/LICENSE_GPL`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/PKG-INFO` & `ganga-8.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ganga
-Version: 8.7.4
+Version: 8.7.5
 Summary: Job management tool
 Home-page: https://github.com/ganga-devs/ganga
 Author: Ganga Developers
 Author-email: project-ganga-developers@cern.ch
 License: GPL v2
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `ganga-8.7.4/README.rst` & `ganga-8.7.5/README.rst`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/bin/ganga` & `ganga-8.7.5/bin/ganga`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/Makefile` & `ganga-8.7.5/doc/Makefile`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/UserGuide/Configuration.rst` & `ganga-8.7.5/doc/UserGuide/Configuration.rst`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/UserGuide/GoogleOauth.rst` & `ganga-8.7.5/doc/UserGuide/GoogleOauth.rst`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/UserGuide/InputAndOutputData.rst` & `ganga-8.7.5/doc/UserGuide/InputAndOutputData.rst`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/UserGuide/InstallAndBasicUsage.rst` & `ganga-8.7.5/doc/UserGuide/InstallAndBasicUsage.rst`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/UserGuide/JobManipulation.rst` & `ganga-8.7.5/doc/UserGuide/JobManipulation.rst`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/UserGuide/MiscellaneousFunctionality.rst` & `ganga-8.7.5/doc/UserGuide/MiscellaneousFunctionality.rst`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/UserGuide/PostProcessors.rst` & `ganga-8.7.5/doc/UserGuide/PostProcessors.rst`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/UserGuide/Queues.rst` & `ganga-8.7.5/doc/UserGuide/Queues.rst`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/UserGuide/RunningExecutables.rst` & `ganga-8.7.5/doc/UserGuide/RunningExecutables.rst`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/UserGuide/Splitters.rst` & `ganga-8.7.5/doc/UserGuide/Splitters.rst`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/UserGuide/Tasks.rst` & `ganga-8.7.5/doc/UserGuide/Tasks.rst`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/UserGuide/TutorialPlugin.rst` & `ganga-8.7.5/doc/UserGuide/TutorialPlugin.rst`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/UserGuide/UsingDifferentApplications.rst` & `ganga-8.7.5/doc/UserGuide/UsingDifferentApplications.rst`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/UserGuide/UsingDifferentBackends.rst` & `ganga-8.7.5/doc/UserGuide/UsingDifferentBackends.rst`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/UserGuide/Virtualization.rst` & `ganga-8.7.5/doc/UserGuide/Virtualization.rst`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/UserGuide/WhatIsGanga.rst` & `ganga-8.7.5/doc/UserGuide/WhatIsGanga.rst`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/UserGuide/first_job.gif` & `ganga-8.7.5/doc/UserGuide/first_job.gif`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/UserGuide/index.rst` & `ganga-8.7.5/doc/UserGuide/index.rst`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/UserGuide/start_terminal.gif` & `ganga-8.7.5/doc/UserGuide/start_terminal.gif`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/UserGuide/virtualization.gif` & `ganga-8.7.5/doc/UserGuide/virtualization.gif`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/_static/favicon.ico` & `ganga-8.7.5/doc/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/_static/logo.svg` & `ganga-8.7.5/doc/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/conf.py` & `ganga-8.7.5/doc/conf.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/dev/credentials.rst` & `ganga-8.7.5/doc/dev/credentials.rst`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/dev/index.rst` & `ganga-8.7.5/doc/dev/index.rst`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/fill_gpi.py` & `ganga-8.7.5/doc/fill_gpi.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/journal/CPC2007/GangaJob.pdf` & `ganga-8.7.5/doc/journal/CPC2007/GangaJob.pdf`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/journal/CPC2007/GangaOverview.pdf` & `ganga-8.7.5/doc/journal/CPC2007/GangaOverview.pdf`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/journal/CPC2007/GangaPlugin.pdf` & `ganga-8.7.5/doc/journal/CPC2007/GangaPlugin.pdf`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/journal/CPC2007/README` & `ganga-8.7.5/doc/journal/CPC2007/README`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/journal/CPC2007/avianflu.pdf` & `ganga-8.7.5/doc/journal/CPC2007/avianflu.pdf`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/journal/CPC2007/avianflu.png` & `ganga-8.7.5/doc/journal/CPC2007/avianflu.png`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/journal/CPC2007/camtology.tex` & `ganga-8.7.5/doc/journal/CPC2007/camtology.tex`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/journal/CPC2007/camtologyfigure.eps` & `ganga-8.7.5/doc/journal/CPC2007/camtologyfigure.eps`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/journal/CPC2007/camtologyfigure.pdf` & `ganga-8.7.5/doc/journal/CPC2007/camtologyfigure.pdf`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/journal/CPC2007/camtologytech.pdf` & `ganga-8.7.5/doc/journal/CPC2007/camtologytech.pdf`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/journal/CPC2007/elsart.cls` & `ganga-8.7.5/doc/journal/CPC2007/elsart.cls`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/journal/CPC2007/elsart1p.cls` & `ganga-8.7.5/doc/journal/CPC2007/elsart1p.cls`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/journal/CPC2007/elsart3p.cls` & `ganga-8.7.5/doc/journal/CPC2007/elsart3p.cls`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/journal/CPC2007/elsart5p.cls` & `ganga-8.7.5/doc/journal/CPC2007/elsart5p.cls`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/journal/CPC2007/ganga-GUI.eps` & `ganga-8.7.5/doc/journal/CPC2007/ganga-GUI.eps`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/journal/CPC2007/ganga-GUI.png` & `ganga-8.7.5/doc/journal/CPC2007/ganga-GUI.png`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/journal/CPC2007/ganga-architecture.png` & `ganga-8.7.5/doc/journal/CPC2007/ganga-architecture.png`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/journal/CPC2007/ganga-architecture.svg` & `ganga-8.7.5/doc/journal/CPC2007/ganga-architecture.svg`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/journal/CPC2007/ganga-diane-portal.pdf` & `ganga-8.7.5/doc/journal/CPC2007/ganga-diane-portal.pdf`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/journal/CPC2007/ganga-diane-portal.png` & `ganga-8.7.5/doc/journal/CPC2007/ganga-diane-portal.png`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/journal/CPC2007/ganga-diane-portal.svg` & `ganga-8.7.5/doc/journal/CPC2007/ganga-diane-portal.svg`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/journal/CPC2007/ganga-objects.dia` & `ganga-8.7.5/doc/journal/CPC2007/ganga-objects.dia`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/journal/CPC2007/ganga-objects.eps` & `ganga-8.7.5/doc/journal/CPC2007/ganga-objects.eps`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/journal/CPC2007/ganga-objects.png` & `ganga-8.7.5/doc/journal/CPC2007/ganga-objects.png`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/journal/CPC2007/ganga.tex` & `ganga-8.7.5/doc/journal/CPC2007/ganga.tex`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/journal/CPC2007/instructions-num.tex` & `ganga-8.7.5/doc/journal/CPC2007/instructions-num.tex`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/journal/CPC2007/job-uml.dia` & `ganga-8.7.5/doc/journal/CPC2007/job-uml.dia`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/journal/CPC2007/job-uml.eps` & `ganga-8.7.5/doc/journal/CPC2007/job-uml.eps`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/journal/CPC2007/job-uml.png` & `ganga-8.7.5/doc/journal/CPC2007/job-uml.png`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/journal/CPC2007/monitoring.eps` & `ganga-8.7.5/doc/journal/CPC2007/monitoring.eps`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/journal/CPC2007/monitoring.png` & `ganga-8.7.5/doc/journal/CPC2007/monitoring.png`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/journal/CPC2007/monitoring.svg` & `ganga-8.7.5/doc/journal/CPC2007/monitoring.svg`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/Makefile` & `ganga-8.7.5/doc/manuals/Makefile`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/html/about.dat` & `ganga-8.7.5/doc/manuals/html/about.dat`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/html/about.html` & `ganga-8.7.5/doc/manuals/html/about.html`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/html/icons/blank.gif` & `ganga-8.7.5/doc/manuals/html/icons/blank.gif`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/html/icons/blank.png` & `ganga-8.7.5/doc/manuals/html/icons/blank.png`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/html/icons/contents.png` & `ganga-8.7.5/doc/manuals/html/icons/contents.png`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/html/icons/index.png` & `ganga-8.7.5/doc/manuals/html/icons/index.png`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/html/icons/modules.png` & `ganga-8.7.5/doc/manuals/html/icons/modules.png`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/html/icons/up.png` & `ganga-8.7.5/doc/manuals/html/icons/up.png`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/html/index.html.in` & `ganga-8.7.5/doc/manuals/html/index.html.in`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/html/stdabout.dat` & `ganga-8.7.5/doc/manuals/html/stdabout.dat`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/html/style.css` & `ganga-8.7.5/doc/manuals/html/style.css`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/perl/SynopsisTable.pm` & `ganga-8.7.5/doc/manuals/perl/SynopsisTable.pm`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/perl/l2hinit.perl` & `ganga-8.7.5/doc/manuals/perl/l2hinit.perl`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/perl/ltxmarkup.perl` & `ganga-8.7.5/doc/manuals/perl/ltxmarkup.perl`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/perl/python.perl` & `ganga-8.7.5/doc/manuals/perl/python.perl`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/script/make-doc.py` & `ganga-8.7.5/doc/manuals/script/make-doc.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/DocMaker/DocMaker.tex` & `ganga-8.7.5/doc/manuals/src/DocMaker/DocMaker.tex`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/Back.png` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/Back.png`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/Copy.png` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/Copy.png`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/Delete.png` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/Delete.png`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/Download.png` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/Download.png`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/Folder_AddDocument.png` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/Folder_AddDocument.png`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/Folder_Generic.png` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/Folder_Generic.png`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/Folder_New.png` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/Folder_New.png`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/Folder_Remove.png` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/Folder_Remove.png`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/Folder_RemoveDocument.png` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/Folder_RemoveDocument.png`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/Folder_Rename.png` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/Folder_Rename.png`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/Forward.png` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/Forward.png`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/GUI_User_Manual.rst` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/GUI_User_Manual.rst`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/General_Options.png` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/General_Options.png`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/Go.png` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/Go.png`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/Properties.png` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/Properties.png`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/Refresh.png` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/Refresh.png`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/Save.png` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/Save.png`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/SaveAs_Template.png` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/SaveAs_Template.png`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/Search.png` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/Search.png`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/Stop.png` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/Stop.png`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/ToolBtn_Kill.jpg` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/ToolBtn_Kill.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/ToolBtn_NewJob.jpg` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/ToolBtn_NewJob.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/ToolBtn_Remove.jpg` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/ToolBtn_Remove.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/ToolBtn_Save.jpg` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/ToolBtn_Save.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/ToolBtn_Submit.jpg` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/ToolBtn_Submit.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/View_Doc.png` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/View_Doc.png`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/Write.png` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/Write.png`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/browse.jpg` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/browse.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/files_16x16.png` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/files_16x16.png`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/files_24x24.png` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/files_24x24.png`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/files_text_16x16.png` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/files_text_16x16.png`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/files_text_24x24.png` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/files_text_24x24.png`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/folder_24x24.png` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/folder_24x24.png`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/folder_32x32.png` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/folder_32x32.png`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/folder_down_24x24.png` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/folder_down_24x24.png`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/folder_down_32x32.png` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/folder_down_32x32.png`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/gangagui-manual-chapter_1.rst` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/gangagui-manual-chapter_1.rst`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/gangagui-manual-chapter_2.rst` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/gangagui-manual-chapter_2.rst`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/gangagui-manual-chapter_3.rst` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/gangagui-manual-chapter_3.rst`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/gangagui-manual-chapter_4.rst` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/gangagui-manual-chapter_4.rst`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/gangagui-manual-chapter_5.rst` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/gangagui-manual-chapter_5.rst`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/gangagui-manual-contents.rst` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/gangagui-manual-contents.rst`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/gangagui_default-view_typical.jpg` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/gangagui_default-view_typical.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/genericjob_pic_1.jpg` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/genericjob_pic_1.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/genericjob_pic_2.jpg` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/genericjob_pic_2.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/genericjob_pic_3.jpg` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/genericjob_pic_3.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/genericjob_pic_4.jpg` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/genericjob_pic_4.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/guiconfig_pic_1.jpg` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/guiconfig_pic_1.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/guiconfig_pic_2.jpg` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/guiconfig_pic_2.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/guiconfig_pic_3.jpg` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/guiconfig_pic_3.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/guiconfig_pic_4.jpg` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/guiconfig_pic_4.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/help.png` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/help.png`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/index.rst` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/index.rst`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/jobbuilder_pic_1.jpg` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/jobbuilder_pic_1.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/jobbuilder_pic_2.jpg` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/jobbuilder_pic_2.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/jobbuilder_pic_3.jpg` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/jobbuilder_pic_3.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/jobbuilder_pic_4.jpg` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/jobbuilder_pic_4.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/jobbuilder_pic_5.jpg` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/jobbuilder_pic_5.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/menubar_pic_1.jpg` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/menubar_pic_1.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/menubar_pic_2.jpg` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/menubar_pic_2.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/menubar_pic_3.jpg` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/menubar_pic_3.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/monitoring_pic_1.jpg` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/monitoring_pic_1.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/monitoring_pic_2.jpg` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/monitoring_pic_2.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/monitoring_pic_3.jpg` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/monitoring_pic_3.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/monitoring_pic_4.jpg` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/monitoring_pic_4.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/open.jpg` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/open.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/preview.jpg` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/preview.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/quickstart_pic_1.jpg` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/quickstart_pic_1.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/quickstart_pic_2.jpg` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/quickstart_pic_2.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/quickstart_pic_3.jpg` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/quickstart_pic_3.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/quickstart_pic_4.jpg` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/quickstart_pic_4.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/quickstart_pic_5.jpg` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/quickstart_pic_5.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/retrieve.jpg` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/retrieve.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/scriptor_pic_1.jpg` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/scriptor_pic_1.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/splitter_pic_1.jpg` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/splitter_pic_1.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/splitter_pic_2.jpg` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/splitter_pic_2.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GUI_User_Manual/toolbar.jpg` & `ganga-8.7.5/doc/manuals/src/GUI_User_Manual/toolbar.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/GangaIntroduction/GangaIntroduction.tex` & `ganga-8.7.5/doc/manuals/src/GangaIntroduction/GangaIntroduction.tex`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/LHCb/LHCb.tex` & `ganga-8.7.5/doc/manuals/src/LHCb/LHCb.tex`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/dev_survival/dev_survival.tex` & `ganga-8.7.5/doc/manuals/src/dev_survival/dev_survival.tex`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/dev_survival/makegraph.py` & `ganga-8.7.5/doc/manuals/src/dev_survival/makegraph.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/dev_survival/transient-states.gif` & `ganga-8.7.5/doc/manuals/src/dev_survival/transient-states.gif`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/dev_survival/user-states.gif` & `ganga-8.7.5/doc/manuals/src/dev_survival/user-states.gif`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/workbook/development/development.tex` & `ganga-8.7.5/doc/manuals/src/workbook/development/development.tex`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/workbook/usage/usage.tex` & `ganga-8.7.5/doc/manuals/src/workbook/usage/usage.tex`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/src/workbook/workbook.tex` & `ganga-8.7.5/doc/manuals/src/workbook/workbook.tex`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/texinputs/distutils.sty` & `ganga-8.7.5/doc/manuals/texinputs/distutils.sty`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/texinputs/fancyhdr.sty` & `ganga-8.7.5/doc/manuals/texinputs/fancyhdr.sty`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/texinputs/fncychap.sty` & `ganga-8.7.5/doc/manuals/texinputs/fncychap.sty`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/texinputs/howto.cls` & `ganga-8.7.5/doc/manuals/texinputs/howto.cls`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/texinputs/ltxmarkup.sty` & `ganga-8.7.5/doc/manuals/texinputs/ltxmarkup.sty`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/texinputs/manual.cls` & `ganga-8.7.5/doc/manuals/texinputs/manual.cls`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/texinputs/pypaper.sty` & `ganga-8.7.5/doc/manuals/texinputs/pypaper.sty`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/texinputs/python.sty` & `ganga-8.7.5/doc/manuals/texinputs/python.sty`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/tools/anno-api.py` & `ganga-8.7.5/doc/manuals/tools/anno-api.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/tools/buildindex.py` & `ganga-8.7.5/doc/manuals/tools/buildindex.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/tools/checkargs.pm` & `ganga-8.7.5/doc/manuals/tools/checkargs.pm`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/tools/cklatex` & `ganga-8.7.5/doc/manuals/tools/cklatex`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/tools/custlib.py` & `ganga-8.7.5/doc/manuals/tools/custlib.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/tools/cvsinfo.py` & `ganga-8.7.5/doc/manuals/tools/cvsinfo.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/tools/findacks` & `ganga-8.7.5/doc/manuals/tools/findacks`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/tools/findcsyms` & `ganga-8.7.5/doc/manuals/tools/findcsyms`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/tools/findmodrefs` & `ganga-8.7.5/doc/manuals/tools/findmodrefs`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/tools/findsyms` & `ganga-8.7.5/doc/manuals/tools/findsyms`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/tools/getpagecounts` & `ganga-8.7.5/doc/manuals/tools/getpagecounts`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/tools/getversioninfo` & `ganga-8.7.5/doc/manuals/tools/getversioninfo`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/tools/html2texi.pl` & `ganga-8.7.5/doc/manuals/tools/html2texi.pl`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/tools/indfix.py` & `ganga-8.7.5/doc/manuals/tools/indfix.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/tools/listmodules` & `ganga-8.7.5/doc/manuals/tools/listmodules`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/tools/makesec.sh` & `ganga-8.7.5/doc/manuals/tools/makesec.sh`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/tools/mkackshtml` & `ganga-8.7.5/doc/manuals/tools/mkackshtml`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/tools/mkhowto` & `ganga-8.7.5/doc/manuals/tools/mkhowto`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/tools/mkinfo` & `ganga-8.7.5/doc/manuals/tools/mkinfo`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/tools/mkmodindex` & `ganga-8.7.5/doc/manuals/tools/mkmodindex`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/tools/mkpkglist` & `ganga-8.7.5/doc/manuals/tools/mkpkglist`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/tools/mksourcepkg` & `ganga-8.7.5/doc/manuals/tools/mksourcepkg`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/tools/node2label.pl` & `ganga-8.7.5/doc/manuals/tools/node2label.pl`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/tools/prechm.py` & `ganga-8.7.5/doc/manuals/tools/prechm.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/tools/push-docs.sh` & `ganga-8.7.5/doc/manuals/tools/push-docs.sh`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/tools/py2texi.el` & `ganga-8.7.5/doc/manuals/tools/py2texi.el`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/tools/python` & `ganga-8.7.5/doc/manuals/tools/python`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/tools/refcounts.py` & `ganga-8.7.5/doc/manuals/tools/refcounts.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/tools/rewrite.py` & `ganga-8.7.5/doc/manuals/tools/rewrite.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/tools/sgmlconv/Makefile` & `ganga-8.7.5/doc/manuals/tools/sgmlconv/Makefile`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/tools/sgmlconv/README` & `ganga-8.7.5/doc/manuals/tools/sgmlconv/README`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/tools/sgmlconv/conversion.xml` & `ganga-8.7.5/doc/manuals/tools/sgmlconv/conversion.xml`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/tools/sgmlconv/docfixer.py` & `ganga-8.7.5/doc/manuals/tools/sgmlconv/docfixer.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/tools/sgmlconv/esis2sgml.py` & `ganga-8.7.5/doc/manuals/tools/sgmlconv/esis2sgml.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/tools/sgmlconv/esistools.py` & `ganga-8.7.5/doc/manuals/tools/sgmlconv/esistools.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/tools/sgmlconv/latex2esis.py` & `ganga-8.7.5/doc/manuals/tools/sgmlconv/latex2esis.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/tools/sgmlconv/make.rules` & `ganga-8.7.5/doc/manuals/tools/sgmlconv/make.rules`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/tools/support.py` & `ganga-8.7.5/doc/manuals/tools/support.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/tools/toc2bkm.py` & `ganga-8.7.5/doc/manuals/tools/toc2bkm.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/tools/undoc_symbols.py` & `ganga-8.7.5/doc/manuals/tools/undoc_symbols.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/manuals/tools/update-docs.sh` & `ganga-8.7.5/doc/manuals/tools/update-docs.sh`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/sysadmin/index.rst` & `ganga-8.7.5/doc/sysadmin/index.rst`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/work/lifetime.txt` & `ganga-8.7.5/doc/work/lifetime.txt`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/doc/work/splitting.txt` & `ganga-8.7.5/doc/work/splitting.txt`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Core/FileWorkspace.py` & `ganga-8.7.5/ganga/GangaCore/Core/FileWorkspace.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Core/GangaRepository/DStreamer.py` & `ganga-8.7.5/ganga/GangaCore/Core/GangaRepository/DStreamer.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Core/GangaRepository/DatabaseRegistry.py` & `ganga-8.7.5/ganga/GangaCore/Core/GangaRepository/DatabaseRegistry.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Core/GangaRepository/FixedLock.py` & `ganga-8.7.5/ganga/GangaCore/Core/GangaRepository/FixedLock.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Core/GangaRepository/GangaRepository.py` & `ganga-8.7.5/ganga/GangaCore/Core/GangaRepository/GangaRepository.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Core/GangaRepository/GangaRepositoryCentral.py` & `ganga-8.7.5/ganga/GangaCore/Core/GangaRepository/GangaRepositoryCentral.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Core/GangaRepository/GangaRepositoryDatabase.py` & `ganga-8.7.5/ganga/GangaCore/Core/GangaRepository/GangaRepositoryDatabase.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Core/GangaRepository/GangaRepositoryImmutableTransient.py` & `ganga-8.7.5/ganga/GangaCore/Core/GangaRepository/GangaRepositoryImmutableTransient.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Core/GangaRepository/GangaRepositoryXML.py` & `ganga-8.7.5/ganga/GangaCore/Core/GangaRepository/GangaRepositoryXML.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Core/GangaRepository/Registry.py` & `ganga-8.7.5/ganga/GangaCore/Core/GangaRepository/Registry.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Core/GangaRepository/SessionLock.py` & `ganga-8.7.5/ganga/GangaCore/Core/GangaRepository/SessionLock.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Core/GangaRepository/SubJobJsonList.py` & `ganga-8.7.5/ganga/GangaCore/Core/GangaRepository/SubJobJsonList.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Core/GangaRepository/SubJobXMLList.py` & `ganga-8.7.5/ganga/GangaCore/Core/GangaRepository/SubJobXMLList.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Core/GangaRepository/VStreamer.py` & `ganga-8.7.5/ganga/GangaCore/Core/GangaRepository/VStreamer.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Core/GangaRepository/__init__.py` & `ganga-8.7.5/ganga/GangaCore/Core/GangaRepository/__init__.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Core/GangaRepository/container_controllers.py` & `ganga-8.7.5/ganga/GangaCore/Core/GangaRepository/container_controllers.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Core/GangaRepository/migrate.py` & `ganga-8.7.5/ganga/GangaCore/Core/GangaRepository/migrate.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Core/GangaThread/GangaThread.py` & `ganga-8.7.5/ganga/GangaCore/Core/GangaThread/GangaThread.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Core/GangaThread/GangaThreadPool.py` & `ganga-8.7.5/ganga/GangaCore/Core/GangaThread/GangaThreadPool.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Core/GangaThread/MTRunner/Algorithm.py` & `ganga-8.7.5/ganga/GangaCore/Core/GangaThread/MTRunner/Algorithm.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Core/GangaThread/MTRunner/Data.py` & `ganga-8.7.5/ganga/GangaCore/Core/GangaThread/MTRunner/Data.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Core/GangaThread/MTRunner/MTRunner.py` & `ganga-8.7.5/ganga/GangaCore/Core/GangaThread/MTRunner/MTRunner.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Core/GangaThread/WorkerThreads/ThreadPoolQueueMonitor.py` & `ganga-8.7.5/ganga/GangaCore/Core/GangaThread/WorkerThreads/ThreadPoolQueueMonitor.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Core/GangaThread/WorkerThreads/WorkerThreadPool.py` & `ganga-8.7.5/ganga/GangaCore/Core/GangaThread/WorkerThreads/WorkerThreadPool.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Core/GangaThread/WorkerThreads/__init__.py` & `ganga-8.7.5/ganga/GangaCore/Core/GangaThread/WorkerThreads/__init__.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Core/InternalServices/Coordinator.py` & `ganga-8.7.5/ganga/GangaCore/Core/InternalServices/Coordinator.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Core/InternalServices/ShutdownManager.py` & `ganga-8.7.5/ganga/GangaCore/Core/InternalServices/ShutdownManager.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Core/MonitoringComponent/Local_GangaMC_Service.py` & `ganga-8.7.5/ganga/GangaCore/Core/MonitoringComponent/Local_GangaMC_Service.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Core/MonitoringComponent/Monitoring.py` & `ganga-8.7.5/ganga/GangaCore/Core/MonitoringComponent/Monitoring.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Core/MonitoringComponent/MonitoringService.py` & `ganga-8.7.5/ganga/GangaCore/Core/MonitoringComponent/MonitoringService.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Core/Sandbox/Sandbox.py` & `ganga-8.7.5/ganga/GangaCore/Core/Sandbox/Sandbox.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Core/Sandbox/WNSandbox.py` & `ganga-8.7.5/ganga/GangaCore/Core/Sandbox/WNSandbox.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Core/__init__.py` & `ganga-8.7.5/ganga/GangaCore/Core/__init__.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Core/exceptions.py` & `ganga-8.7.5/ganga/GangaCore/Core/exceptions.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/Adapters/ApplicationRuntimeHandlers.py` & `ganga-8.7.5/ganga/GangaCore/GPIDev/Adapters/ApplicationRuntimeHandlers.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/Adapters/IApplication.py` & `ganga-8.7.5/ganga/GangaCore/GPIDev/Adapters/IApplication.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/Adapters/IBackend.py` & `ganga-8.7.5/ganga/GangaCore/GPIDev/Adapters/IBackend.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/Adapters/IChecker.py` & `ganga-8.7.5/ganga/GangaCore/GPIDev/Adapters/IChecker.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/Adapters/ICredentialInfo.py` & `ganga-8.7.5/ganga/GangaCore/GPIDev/Adapters/ICredentialInfo.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/Adapters/ICredentialRequirement.py` & `ganga-8.7.5/ganga/GangaCore/GPIDev/Adapters/ICredentialRequirement.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/Adapters/IGangaFile.py` & `ganga-8.7.5/ganga/GangaCore/GPIDev/Adapters/IGangaFile.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/Adapters/IMerger.py` & `ganga-8.7.5/ganga/GangaCore/GPIDev/Adapters/IMerger.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/Adapters/IMonitoringService.py` & `ganga-8.7.5/ganga/GangaCore/GPIDev/Adapters/IMonitoringService.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/Adapters/IPostProcessor.py` & `ganga-8.7.5/ganga/GangaCore/GPIDev/Adapters/IPostProcessor.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/Adapters/IPrepareApp.py` & `ganga-8.7.5/ganga/GangaCore/GPIDev/Adapters/IPrepareApp.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/Adapters/IRuntimeHandler.py` & `ganga-8.7.5/ganga/GangaCore/GPIDev/Adapters/IRuntimeHandler.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/Adapters/ISplitter.py` & `ganga-8.7.5/ganga/GangaCore/GPIDev/Adapters/ISplitter.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/Adapters/IVirtualization.py` & `ganga-8.7.5/ganga/GangaCore/GPIDev/Adapters/IVirtualization.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/Adapters/StandardJobConfig.py` & `ganga-8.7.5/ganga/GangaCore/GPIDev/Adapters/StandardJobConfig.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/Base/Filters.py` & `ganga-8.7.5/ganga/GangaCore/GPIDev/Base/Filters.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/Base/Objects.py` & `ganga-8.7.5/ganga/GangaCore/GPIDev/Base/Objects.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/Base/Proxy.py` & `ganga-8.7.5/ganga/GangaCore/GPIDev/Base/Proxy.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/Base/VPrinter.py` & `ganga-8.7.5/ganga/GangaCore/GPIDev/Base/VPrinter.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/Base/VPrinterOld.py` & `ganga-8.7.5/ganga/GangaCore/GPIDev/Base/VPrinterOld.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/Credentials/AfsToken.py` & `ganga-8.7.5/ganga/GangaCore/GPIDev/Credentials/AfsToken.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/Credentials/CredentialStore.py` & `ganga-8.7.5/ganga/GangaCore/GPIDev/Credentials/CredentialStore.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/Credentials/VomsProxy.py` & `ganga-8.7.5/ganga/GangaCore/GPIDev/Credentials/VomsProxy.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/Credentials/__init__.py` & `ganga-8.7.5/ganga/GangaCore/GPIDev/Credentials/__init__.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/Credentials_old/ICredential.py` & `ganga-8.7.5/ganga/GangaCore/GPIDev/Credentials_old/ICredential.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/Credentials_old/__init__.py` & `ganga-8.7.5/ganga/GangaCore/GPIDev/Credentials_old/__init__.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/Config/Config.py` & `ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/Config/Config.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/Dataset/Dataset.py` & `ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/Dataset/Dataset.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/Dataset/GangaDataset.py` & `ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/Dataset/GangaDataset.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/File/File.py` & `ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/File/File.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/File/FileBuffer.py` & `ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/File/FileBuffer.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/File/FileUtils.py` & `ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/File/FileUtils.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/File/GoogleFile.py` & `ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/File/GoogleFile.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/File/LocalFile.py` & `ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/File/LocalFile.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/File/MassStorageFile.py` & `ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/File/MassStorageFile.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/File/OutputFileManager.py` & `ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/File/OutputFileManager.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/File/__init__.py` & `ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/File/__init__.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/File/scripts/LCGSEFileWNScript.py.template` & `ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/File/scripts/LCGSEFileWNScript.py.template`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/File/scripts/MassStorageFileWNScript.py.template` & `ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/File/scripts/MassStorageFileWNScript.py.template`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/GangaList/GangaList.py` & `ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/GangaList/GangaList.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/Job/Job.py` & `ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/Job/Job.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/Job/JobInfo.py` & `ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/Job/JobInfo.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/Job/JobTime.py` & `ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/Job/JobTime.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/Job/MetadataDict.py` & `ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/Job/MetadataDict.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/Job/utils.py` & `ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/Job/utils.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/JobTree/JobTree.py` & `ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/JobTree/JobTree.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/Registry/BoxRegistry.py` & `ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/Registry/BoxRegistry.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/Registry/JobRegistry.py` & `ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/Registry/JobRegistry.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/Registry/PrepRegistry.py` & `ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/Registry/PrepRegistry.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/Registry/RegistrySlice.py` & `ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/Registry/RegistrySlice.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/Registry/RegistrySliceProxy.py` & `ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/Registry/RegistrySliceProxy.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/Registry/TransientRegistry.py` & `ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/Registry/TransientRegistry.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/Tasks/CoreTransform.py` & `ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/Tasks/CoreTransform.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/Tasks/CoreUnit.py` & `ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/Tasks/CoreUnit.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/Tasks/ITask.py` & `ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/Tasks/ITask.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/Tasks/ITransform.py` & `ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/Tasks/ITransform.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/Tasks/IUnit.py` & `ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/Tasks/IUnit.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/Tasks/TaskChainInput.py` & `ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/Tasks/TaskChainInput.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/Tasks/TaskLocalCopy.py` & `ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/Tasks/TaskLocalCopy.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/Tasks/TaskRegistry.py` & `ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/Tasks/TaskRegistry.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/Tasks/__init__.py` & `ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/Tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/Lib/Tasks/common.py` & `ganga-8.7.5/ganga/GangaCore/GPIDev/Lib/Tasks/common.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/MonitoringServices/Composite.py` & `ganga-8.7.5/ganga/GangaCore/GPIDev/MonitoringServices/Composite.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/MonitoringServices/__init__.py` & `ganga-8.7.5/ganga/GangaCore/GPIDev/MonitoringServices/__init__.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/Persistency/__init__.py` & `ganga-8.7.5/ganga/GangaCore/GPIDev/Persistency/__init__.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/Schema/Schema.py` & `ganga-8.7.5/ganga/GangaCore/GPIDev/Schema/Schema.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/GPIDev/TypeCheck.py` & `ganga-8.7.5/ganga/GangaCore/GPIDev/TypeCheck.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Lib/Batch/Batch.py` & `ganga-8.7.5/ganga/GangaCore/Lib/Batch/Batch.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Lib/Batch/BatchScriptTemplate.py.template` & `ganga-8.7.5/ganga/GangaCore/Lib/Batch/BatchScriptTemplate.py.template`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env python2
+#!/usr/bin/env python3
 from __future__ import print_function
 
 import glob
 import mimetypes
 import os
 import shutil
 import subprocess
```

### Comparing `ganga-8.7.4/ganga/GangaCore/Lib/Checkers/CustomChecker.py` & `ganga-8.7.5/ganga/GangaCore/Lib/Checkers/CustomChecker.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Lib/Checkers/FileChecker.py` & `ganga-8.7.5/ganga/GangaCore/Lib/Checkers/FileChecker.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Lib/Checkers/MetaDataChecker.py` & `ganga-8.7.5/ganga/GangaCore/Lib/Checkers/MetaDataChecker.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Lib/Checkers/RootFileChecker.py` & `ganga-8.7.5/ganga/GangaCore/Lib/Checkers/RootFileChecker.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Lib/Condor/Condor.py` & `ganga-8.7.5/ganga/GangaCore/Lib/Condor/Condor.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Lib/Condor/CondorRequirements.py` & `ganga-8.7.5/ganga/GangaCore/Lib/Condor/CondorRequirements.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Lib/Condor/__init__.py` & `ganga-8.7.5/ganga/GangaCore/Lib/Condor/__init__.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Lib/Executable/Executable.py` & `ganga-8.7.5/ganga/GangaCore/Lib/Executable/Executable.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Lib/Interactive/Interactive.py` & `ganga-8.7.5/ganga/GangaCore/Lib/Interactive/Interactive.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Lib/Interactive/InteractiveScriptTemplate.py.template` & `ganga-8.7.5/ganga/GangaCore/Lib/Interactive/InteractiveScriptTemplate.py.template`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Lib/Interactive/__init__.py` & `ganga-8.7.5/ganga/GangaCore/Lib/Interactive/__init__.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Lib/Localhost/LocalHostExec.py.template` & `ganga-8.7.5/ganga/GangaCore/Lib/Localhost/LocalHostExec.py.template`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Lib/Localhost/LocalHostExec_batch.py.template` & `ganga-8.7.5/ganga/GangaCore/Lib/Localhost/LocalHostExec_batch.py.template`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Lib/Localhost/Localhost.py` & `ganga-8.7.5/ganga/GangaCore/Lib/Localhost/Localhost.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Lib/Mergers/Merger.py` & `ganga-8.7.5/ganga/GangaCore/Lib/Mergers/Merger.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Lib/Notebook/Notebook.py` & `ganga-8.7.5/ganga/GangaCore/Lib/Notebook/Notebook.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
                 preparable=1,
                 defvalue=None,
                 typelist=[None, int],
                 doc="Timeout in seconds for executing a notebook. If None, the default value will be taken.",
             ),
             'kernel': SimpleItem(
                 preparable=1,
-                defvalue='python2',
+                defvalue='python3',
                 doc="The kernel to use for the notebook execution. \
                 Depending on configuration, python3, Root and R might be available.",
             ),
             'regexp': SimpleItem(
                 preparable=1,
                 defvalue=[r'.+\.ipynb$'],
                 typelist=["str"],
```

### Comparing `ganga-8.7.4/ganga/GangaCore/Lib/Notebook/wrapperNotebookTemplate.py.template` & `ganga-8.7.5/ganga/GangaCore/Lib/Notebook/wrapperNotebookTemplate.py.template`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Lib/Notifier/Notifier.py` & `ganga-8.7.5/ganga/GangaCore/Lib/Notifier/Notifier.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Lib/Remote/Remote.py` & `ganga-8.7.5/ganga/GangaCore/Lib/Remote/Remote.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Lib/Splitters/ArgSplitter.py` & `ganga-8.7.5/ganga/GangaCore/Lib/Splitters/ArgSplitter.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Lib/Splitters/DefaultSplitter.py` & `ganga-8.7.5/ganga/GangaCore/Lib/Splitters/DefaultSplitter.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Lib/Splitters/ExeSplitter.py` & `ganga-8.7.5/ganga/GangaCore/Lib/Splitters/ExeSplitter.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Lib/Splitters/GangaDatasetSplitter.py` & `ganga-8.7.5/ganga/GangaCore/Lib/Splitters/GangaDatasetSplitter.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Lib/Splitters/GenericSplitter.py` & `ganga-8.7.5/ganga/GangaCore/Lib/Splitters/GenericSplitter.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Lib/Virtualization/Apptainer.py` & `ganga-8.7.5/ganga/GangaCore/Lib/Virtualization/Apptainer.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Lib/Virtualization/Docker.py` & `ganga-8.7.5/ganga/GangaCore/Lib/Virtualization/Docker.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Lib/Virtualization/Singularity.py` & `ganga-8.7.5/ganga/GangaCore/Lib/Virtualization/Singularity.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/PACKAGE.py` & `ganga-8.7.5/ganga/GangaCore/PACKAGE.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Runtime/GPIFunctions.py` & `ganga-8.7.5/ganga/GangaCore/Runtime/GPIFunctions.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Runtime/GPIexport.py` & `ganga-8.7.5/ganga/GangaCore/Runtime/GPIexport.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Runtime/GangaCompleter.py` & `ganga-8.7.5/ganga/GangaCore/Runtime/GangaCompleter.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Runtime/HEAD_CONFIG.INI` & `ganga-8.7.5/ganga/GangaCore/Runtime/HEAD_CONFIG.INI`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Runtime/IPythonMagic.py` & `ganga-8.7.5/ganga/GangaCore/Runtime/IPythonMagic.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Runtime/Repository_runtime.py` & `ganga-8.7.5/ganga/GangaCore/Runtime/Repository_runtime.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Runtime/__init__.py` & `ganga-8.7.5/ganga/GangaCore/Runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Runtime/bootstrap.py` & `ganga-8.7.5/ganga/GangaCore/Runtime/bootstrap.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Runtime/eliza.py` & `ganga-8.7.5/ganga/GangaCore/Runtime/eliza.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Runtime/ganga_extension.py` & `ganga-8.7.5/ganga/GangaCore/Runtime/ganga_extension.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Runtime/gangadoc.py` & `ganga-8.7.5/ganga/GangaCore/Runtime/gangadoc.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Runtime/plugins.py` & `ganga-8.7.5/ganga/GangaCore/Runtime/plugins.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Utility/ColourText.py` & `ganga-8.7.5/ganga/GangaCore/Utility/ColourText.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Utility/Config/Config.py` & `ganga-8.7.5/ganga/GangaCore/Utility/Config/Config.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Utility/Config/__init__.py` & `ganga-8.7.5/ganga/GangaCore/Utility/Config/__init__.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Utility/Config/tests.py` & `ganga-8.7.5/ganga/GangaCore/Utility/Config/tests.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Utility/Decorators.py` & `ganga-8.7.5/ganga/GangaCore/Utility/Decorators.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Utility/GridShell.py` & `ganga-8.7.5/ganga/GangaCore/Utility/GridShell.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Utility/Plugin/GangaPlugin.py` & `ganga-8.7.5/ganga/GangaCore/Utility/Plugin/GangaPlugin.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Utility/Profiling.py` & `ganga-8.7.5/ganga/GangaCore/Utility/Profiling.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Utility/Runtime.py` & `ganga-8.7.5/ganga/GangaCore/Utility/Runtime.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Utility/Setup.py` & `ganga-8.7.5/ganga/GangaCore/Utility/Setup.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Utility/Shell.py` & `ganga-8.7.5/ganga/GangaCore/Utility/Shell.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Utility/Virtualization.py` & `ganga-8.7.5/ganga/GangaCore/Utility/Virtualization.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Utility/execute.py` & `ganga-8.7.5/ganga/GangaCore/Utility/execute.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Utility/external/OrderedDict.py` & `ganga-8.7.5/ganga/GangaCore/Utility/external/OrderedDict.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Utility/feedback_report.py` & `ganga-8.7.5/ganga/GangaCore/Utility/feedback_report.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Utility/files.py` & `ganga-8.7.5/ganga/GangaCore/Utility/files.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Utility/logging/__init__.py` & `ganga-8.7.5/ganga/GangaCore/Utility/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Utility/logging/test.py` & `ganga-8.7.5/ganga/GangaCore/Utility/logging/test.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Utility/root.py` & `ganga-8.7.5/ganga/GangaCore/Utility/root.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Utility/stacktracer.py` & `ganga-8.7.5/ganga/GangaCore/Utility/stacktracer.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Utility/strings.py` & `ganga-8.7.5/ganga/GangaCore/Utility/strings.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Utility/threads.py` & `ganga-8.7.5/ganga/GangaCore/Utility/threads.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/Utility/util.py` & `ganga-8.7.5/ganga/GangaCore/Utility/util.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/__init__.py` & `ganga-8.7.5/ganga/GangaCore/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         return lcg_release_areas['cvmfs']
     else:
         return ''
 
 
 # ------------------------------------------------
 # store Ganga version based on new git tag for this file
-_gangaVersion = '8.7.4'
+_gangaVersion = '8.7.5'
 _development = False
 
 # store a path to Ganga libraries
 _gangaPythonPath = os.path.dirname(os.path.dirname(__file__))
 
 
 # grab the hostname
```

### Comparing `ganga-8.7.4/ganga/GangaCore/old_test/GPI/ConfigObject.ini` & `ganga-8.7.5/ganga/GangaCore/old_test/GPI/ConfigObject.ini`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/old_test/GPI/ConfigUser.ini` & `ganga-8.7.5/ganga/GangaCore/old_test/GPI/ConfigUser.ini`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesBatchMultipleFilesForLCGUpload.ini` & `ganga-8.7.5/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesBatchMultipleFilesForLCGUpload.ini`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesInteractiveMultipleFilesForPattern.ini` & `ganga-8.7.5/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesInteractiveMultipleFilesForPattern.ini`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesLCG.ini` & `ganga-8.7.5/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesLCG.ini`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesLocal.ini` & `ganga-8.7.5/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesLocal.ini`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesLocalMultipleFilesForLCGUpload.ini` & `ganga-8.7.5/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesLocalMultipleFilesForLCGUpload.ini`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesLocalMultipleFilesForPattern.ini` & `ganga-8.7.5/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesLocalMultipleFilesForPattern.ini`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesMixedBatch.ini` & `ganga-8.7.5/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesMixedBatch.ini`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/old_test/__init__.py` & `ganga-8.7.5/ganga/GangaCore/old_test/__init__.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/old_test/config/Schema.ini` & `ganga-8.7.5/ganga/GangaCore/old_test/config/Schema.ini`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/old_test/config/default.ini` & `ganga-8.7.5/ganga/GangaCore/old_test/config/default.ini`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/old_test/config/localxml.ini` & `ganga-8.7.5/ganga/GangaCore/old_test/config/localxml.ini`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/test/GPI/Notebook/Test.ipynb` & `ganga-8.7.5/ganga/GangaCore/test/GPI/Notebook/Test.ipynb`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9925595238095238%*

 * *Differences: {"'metadata'": "{'kernelspec': {'name': 'python3'}, 'language_info': {'pygments_lexer': "*

 * *               "'ipython3'}}"}*

```diff
@@ -24,25 +24,25 @@
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 2",
             "language": "python",
-            "name": "python2"
+            "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 2
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
-            "pygments_lexer": "ipython2",
+            "pygments_lexer": "ipython3",
             "version": "2.7.12"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 0
 }
```

### Comparing `ganga-8.7.4/ganga/GangaCore/testlib/GangaUnitTest.py` & `ganga-8.7.5/ganga/GangaCore/testlib/GangaUnitTest.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/testlib/decorators.py` & `ganga-8.7.5/ganga/GangaCore/testlib/decorators.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/testlib/file_utils.py` & `ganga-8.7.5/ganga/GangaCore/testlib/file_utils.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/testlib/fixtures.py` & `ganga-8.7.5/ganga/GangaCore/testlib/fixtures.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/testlib/mark.py` & `ganga-8.7.5/ganga/GangaCore/testlib/mark.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaCore/testlib/monitoring.py` & `ganga-8.7.5/ganga/GangaCore/testlib/monitoring.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaDirac/BOOT.py` & `ganga-8.7.5/ganga/GangaDirac/BOOT.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaDirac/Dirac.ini` & `ganga-8.7.5/ganga/GangaDirac/Dirac.ini`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaDirac/Lib/Backends/Dirac.py` & `ganga-8.7.5/ganga/GangaDirac/Lib/Backends/Dirac.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaDirac/Lib/Backends/DiracBase.py` & `ganga-8.7.5/ganga/GangaDirac/Lib/Backends/DiracBase.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaDirac/Lib/Backends/DiracUtils.py` & `ganga-8.7.5/ganga/GangaDirac/Lib/Backends/DiracUtils.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaDirac/Lib/Credentials/DiracProxy.py` & `ganga-8.7.5/ganga/GangaDirac/Lib/Credentials/DiracProxy.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaDirac/Lib/Files/DiracFile.py` & `ganga-8.7.5/ganga/GangaDirac/Lib/Files/DiracFile.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaDirac/Lib/Files/WNInjectTemplate.py.template` & `ganga-8.7.5/ganga/GangaDirac/Lib/Files/WNInjectTemplate.py.template`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaDirac/Lib/Files/uploadScript.py.template` & `ganga-8.7.5/ganga/GangaDirac/Lib/Files/uploadScript.py.template`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaDirac/Lib/RTHandlers/DiracRTHScript.py.template` & `ganga-8.7.5/ganga/GangaDirac/Lib/RTHandlers/DiracRTHScript.py.template`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaDirac/Lib/RTHandlers/DiracRTHUtils.py` & `ganga-8.7.5/ganga/GangaDirac/Lib/RTHandlers/DiracRTHUtils.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaDirac/Lib/RTHandlers/ExeDiracRTHandler.py` & `ganga-8.7.5/ganga/GangaDirac/Lib/RTHandlers/ExeDiracRTHandler.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaDirac/Lib/RTHandlers/RunTimeHandlerUtils.py` & `ganga-8.7.5/ganga/GangaDirac/Lib/RTHandlers/RunTimeHandlerUtils.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaDirac/Lib/Server/DiracCommands.py` & `ganga-8.7.5/ganga/GangaDirac/Lib/Server/DiracCommands.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaDirac/Lib/Server/DiracDefinition.py` & `ganga-8.7.5/ganga/GangaDirac/Lib/Server/DiracDefinition.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaDirac/Lib/Server/DiracExecutorProcess.py` & `ganga-8.7.5/ganga/GangaDirac/Lib/Server/DiracExecutorProcess.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaDirac/Lib/Server/DiracNewCommands.py` & `ganga-8.7.5/ganga/GangaDirac/Lib/Server/DiracNewCommands.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaDirac/Lib/Server/DiracOldProcess.py` & `ganga-8.7.5/ganga/GangaDirac/Lib/Server/DiracOldProcess.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaDirac/Lib/Server/DiracProcessManager.py` & `ganga-8.7.5/ganga/GangaDirac/Lib/Server/DiracProcessManager.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaDirac/Lib/Server/InspectionClient.py` & `ganga-8.7.5/ganga/GangaDirac/Lib/Server/InspectionClient.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaDirac/Lib/Server/InspectionServer.py` & `ganga-8.7.5/ganga/GangaDirac/Lib/Server/InspectionServer.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaDirac/Lib/Splitters/GangaSplitterUtils.py` & `ganga-8.7.5/ganga/GangaDirac/Lib/Splitters/GangaSplitterUtils.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaDirac/Lib/Splitters/OfflineGangaDiracSplitter.py` & `ganga-8.7.5/ganga/GangaDirac/Lib/Splitters/OfflineGangaDiracSplitter.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaDirac/Lib/Splitters/SplitterUtils.py` & `ganga-8.7.5/ganga/GangaDirac/Lib/Splitters/SplitterUtils.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaDirac/Lib/Utilities/DiracUtilities.py` & `ganga-8.7.5/ganga/GangaDirac/Lib/Utilities/DiracUtilities.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaDirac/PACKAGE.py` & `ganga-8.7.5/ganga/GangaDirac/PACKAGE.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaDirac/__init__.py` & `ganga-8.7.5/ganga/GangaDirac/__init__.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaGaudi/Lib/Applications/CMTUtils.py` & `ganga-8.7.5/ganga/GangaGaudi/Lib/Applications/CMTUtils.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaGaudi/Lib/Applications/Gaudi.py` & `ganga-8.7.5/ganga/GangaGaudi/Lib/Applications/Gaudi.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaGaudi/Lib/Applications/GaudiBase.py` & `ganga-8.7.5/ganga/GangaGaudi/Lib/Applications/GaudiBase.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaGaudi/Lib/Applications/GaudiUtils.py` & `ganga-8.7.5/ganga/GangaGaudi/Lib/Applications/GaudiUtils.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaGaudi/Lib/Applications/GaudiXMLSummary.py` & `ganga-8.7.5/ganga/GangaGaudi/Lib/Applications/GaudiXMLSummary.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaGaudi/Lib/Applications/cmakeUtils.py` & `ganga-8.7.5/ganga/GangaGaudi/Lib/Applications/cmakeUtils.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaGaudi/Lib/Checkers/GaudiMetaDataChecker.py` & `ganga-8.7.5/ganga/GangaGaudi/Lib/Checkers/GaudiMetaDataChecker.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaGaudi/Lib/Datasets/GaudiDataset.py` & `ganga-8.7.5/ganga/GangaGaudi/Lib/Datasets/GaudiDataset.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaGaudi/Lib/RTHandlers/GaudiDiracRunTimeHandler.py` & `ganga-8.7.5/ganga/GangaGaudi/Lib/RTHandlers/GaudiDiracRunTimeHandler.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaGaudi/Lib/RTHandlers/GaudiRunTimeHandler.py` & `ganga-8.7.5/ganga/GangaGaudi/Lib/RTHandlers/GaudiRunTimeHandler.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaGaudi/Lib/Splitters/GaudiInputDataSplitter.py` & `ganga-8.7.5/ganga/GangaGaudi/Lib/Splitters/GaudiInputDataSplitter.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaGaudi/Lib/XMLSummary/schema.py` & `ganga-8.7.5/ganga/GangaGaudi/Lib/XMLSummary/schema.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaGaudi/Lib/XMLSummary/summary.py` & `ganga-8.7.5/ganga/GangaGaudi/Lib/XMLSummary/summary.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaGaudi/PACKAGE.py` & `ganga-8.7.5/ganga/GangaGaudi/PACKAGE.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaGaudi/__init__.py` & `ganga-8.7.5/ganga/GangaGaudi/__init__.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaLHCb/BOOT.py` & `ganga-8.7.5/ganga/GangaLHCb/BOOT.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaLHCb/LHCb.ini` & `ganga-8.7.5/ganga/GangaLHCb/LHCb.ini`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaLHCb/Lib/Applications/AppsBase.py` & `ganga-8.7.5/ganga/GangaLHCb/Lib/Applications/AppsBase.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaLHCb/Lib/Applications/AppsBaseUtils.py` & `ganga-8.7.5/ganga/GangaLHCb/Lib/Applications/AppsBaseUtils.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaLHCb/Lib/Applications/Bender.py` & `ganga-8.7.5/ganga/GangaLHCb/Lib/Applications/Bender.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaLHCb/Lib/Applications/BenderBox.py` & `ganga-8.7.5/ganga/GangaLHCb/Lib/Applications/BenderBox.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaLHCb/Lib/Applications/BenderScript.py` & `ganga-8.7.5/ganga/GangaLHCb/Lib/Applications/BenderScript.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaLHCb/Lib/Applications/CMTscript.py` & `ganga-8.7.5/ganga/GangaLHCb/Lib/Applications/CMTscript.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaLHCb/Lib/Applications/EnvironFunctions.py` & `ganga-8.7.5/ganga/GangaLHCb/Lib/Applications/EnvironFunctions.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaLHCb/Lib/Applications/FileFunctions.py` & `ganga-8.7.5/ganga/GangaLHCb/Lib/Applications/FileFunctions.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaLHCb/Lib/Applications/GaudiExec.py` & `ganga-8.7.5/ganga/GangaLHCb/Lib/Applications/GaudiExec.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaLHCb/Lib/Applications/GaudiExecUtils.py` & `ganga-8.7.5/ganga/GangaLHCb/Lib/Applications/GaudiExecUtils.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaLHCb/Lib/Applications/GaudiPython.py` & `ganga-8.7.5/ganga/GangaLHCb/Lib/Applications/GaudiPython.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaLHCb/Lib/Applications/Ostap.py` & `ganga-8.7.5/ganga/GangaLHCb/Lib/Applications/Ostap.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaLHCb/Lib/Applications/PythonOptionsParser.py` & `ganga-8.7.5/ganga/GangaLHCb/Lib/Applications/PythonOptionsParser.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaLHCb/Lib/Applications/PythonOptsCmakeParser.py` & `ganga-8.7.5/ganga/GangaLHCb/Lib/Applications/PythonOptsCmakeParser.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaLHCb/Lib/Applications/XMLPostProcessor.py` & `ganga-8.7.5/ganga/GangaLHCb/Lib/Applications/XMLPostProcessor.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaLHCb/Lib/Applications/__init__.py` & `ganga-8.7.5/ganga/GangaLHCb/Lib/Applications/__init__.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaLHCb/Lib/Backends/Bookkeeping.py` & `ganga-8.7.5/ganga/GangaLHCb/Lib/Backends/Bookkeeping.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaLHCb/Lib/Backends/Dirac.py` & `ganga-8.7.5/ganga/GangaLHCb/Lib/Backends/Dirac.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaLHCb/Lib/Checkers/LHCbMetadataChecker.py` & `ganga-8.7.5/ganga/GangaLHCb/Lib/Checkers/LHCbMetadataChecker.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaLHCb/Lib/Files/LogicalFile.py` & `ganga-8.7.5/ganga/GangaLHCb/Lib/Files/LogicalFile.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaLHCb/Lib/Files/PhysicalFile.py` & `ganga-8.7.5/ganga/GangaLHCb/Lib/Files/PhysicalFile.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaLHCb/Lib/LHCbDataset/BKQuery.py` & `ganga-8.7.5/ganga/GangaLHCb/Lib/LHCbDataset/BKQuery.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaLHCb/Lib/LHCbDataset/LHCbCompressedDataset.py` & `ganga-8.7.5/ganga/GangaLHCb/Lib/LHCbDataset/LHCbCompressedDataset.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaLHCb/Lib/LHCbDataset/LHCbDataset.py` & `ganga-8.7.5/ganga/GangaLHCb/Lib/LHCbDataset/LHCbDataset.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaLHCb/Lib/LHCbDataset/LHCbDatasetUtils.py` & `ganga-8.7.5/ganga/GangaLHCb/Lib/LHCbDataset/LHCbDatasetUtils.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaLHCb/Lib/Mergers/CMTVersion.py` & `ganga-8.7.5/ganga/GangaLHCb/Lib/Mergers/CMTVersion.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaLHCb/Lib/Mergers/GaudiExecMerger.py` & `ganga-8.7.5/ganga/GangaLHCb/Lib/Mergers/GaudiExecMerger.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaLHCb/Lib/Mergers/LHCbFileMerger.py` & `ganga-8.7.5/ganga/GangaLHCb/Lib/Mergers/LHCbFileMerger.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaLHCb/Lib/RTHandlers/ExeDiracRTHandler.py` & `ganga-8.7.5/ganga/GangaLHCb/Lib/RTHandlers/ExeDiracRTHandler.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,15 +163,15 @@
                                  outputbox=unique(outputsandbox))
 
 
 # \/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\#
 
 
 def exe_script_template():
-    script_template = """#!/usr/bin/env python2
+    script_template = """#!/usr/bin/env python3
 '''Script to run Executable application'''
 import sys, os
 import subprocess
 from os import system, environ, pathsep, getcwd, listdir, path
 
 runenv = environ.copy()
 if 'PATH' in runenv.keys():
```

### Comparing `ganga-8.7.4/ganga/GangaLHCb/Lib/RTHandlers/GaudiExecRTHandlers.py` & `ganga-8.7.5/ganga/GangaLHCb/Lib/RTHandlers/GaudiExecRTHandlers.py`

 * *Files 4% similar despite different names*

```diff
@@ -584,15 +584,14 @@
             raise ApplicationPrepareError("Failed to find a replica, aborting submit")
 
         # Check if the uploaded input already has replicas in case this is a copy of a job.
         if len(app.uploadedInput.locations) == 0:
             app.uploadedInput.getReplicas()
         if len(app.uploadedInput.locations) >= 2:
             logger.debug("Uploaded input archive already at two locations, not replicating again")
-            return
         else:
             replicateJobFile(app.uploadedInput)
 
         replicateJobFile(app.jobScriptArchive)
 
         return StandardJobConfig(inputbox=unique(inputsandbox), outputbox=unique(outputsandbox))
 
@@ -629,15 +628,16 @@
                 inputsandbox += ['LFN:' + file_.lfn]
             elif isinstance(file_, LocalFile):
                 if job.master is not None and file_ not in job.master.inputfiles:
                     shutil.copy(os.path.join(file_.localDir, file_.namePattern), app.getSharedPath())
                     inputsandbox += [os.path.join(app.getSharedPath(), file_.namePattern)]
             else:
                 logger.error(
-                    "Filetype: %s nor currently supported, please contact Ganga Devs if you require support for this with the DIRAC backend" %
+                    "Filetype: %s nor currently supported, "
+                    "please contact Ganga Devs if you require support for this with the DIRAC backend" %
                     getName(file_))
                 raise ApplicationConfigurationError("Unsupported filetype: %s with DIRAC backend" % getName(file_))
 
         master_job = job.master or job
 
         app.uploadedInput = master_job.application.uploadedInput
         app.jobScriptArchive = master_job.application.jobScriptArchive
@@ -712,15 +712,15 @@
         # NB
         # inputsandbox here isn't used by the DIRAC backend as we explicitly define the INPUT_SANDBOX here!
 
         # Return the output needed for the backend to submit this job
         return StandardJobConfig(dirac_script, inputbox=[], outputbox=[])
 
 
-#\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\#
+# \/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\#
 
 
 def gaudiRun_script_template():
     """
     Script to return the contents of the command to be executed on the worker node
     """
     script_template = """#!/usr/bin/env python3
@@ -774,15 +774,16 @@
 if __name__ == '__main__':
     '''
     Main section of code for the GaudiExec script run on the WN
     '''
     # Opening pleasantries
     print("Hello from GaudiExec")
     print("Arrived at workernode: %s" % getcwd())
-    print(r"#\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/#")
+    print(r"#\\/\\/\\/\\/\\/\\/\\/\\/\\/\\/\\/\\/\\/\\/\\/\\/\\/\\/\\/\\/\\/\\/\\/"
+            "\\/\\/\\/\\/\\/\\/\\/\\/\\/\\/\\/\\/\\/\\/\\/\\/\\/\\/\\/\\/\\/\\/\\/\\/#")
     print("")
 
     print("CWD: %s" % getcwd())
     print("Files found on WN: %s" % (listdir('.')))
 
     if 'LHCb_release_area' not in environ:
         environ['LHCb_release_area'] = '/cvmfs/lhcb.cern.ch/lib/lhcb/'
@@ -791,33 +792,36 @@
     # Extract any/_all_ (b/g)zip files on the WN
     extractAllTarFiles('.')
 
     print("Executing: %s" % '###COMMAND###'+' '+' '.join(sys.argv[1:]))
 
     # Execute the actual command on the WN
     # NB os.system caused the entire stream to be captured before being streamed in some cases
-    pipe = subprocess.Popen('###COMMAND###'+' '+' '.join(sys.argv[1:]), shell=True, stdin=subprocess.PIPE, stdout=subprocess.PIPE, universal_newlines=True, errors="replace")
+    pipe = subprocess.Popen('###COMMAND###'+' '+' '.join(sys.argv[1:]), shell=True,
+                            stdin=subprocess.PIPE, stdout=subprocess.PIPE,
+                            universal_newlines=True, errors="replace")
 
     # Flush the stdout/stderr as the process is running correctly
     flush_streams(pipe)
 
     # Wait for the process to finish executing
     pipe.wait()
 
     rc = pipe.returncode
 
     ###OUTPUTFILESINJECTEDCODE###
 
     # Final pleasantries
     print("")
-    print(r"#\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/#")
+    print(r"#\\/\\/\\/\\/\\/\\/\\/\\/\\/\\/\\/\\/\\/\\/\\/\\/\\/\\/\\/\\/\\/\\/\\/\\/\\/"
+            "\\/\\/\\/\\/\\/\\/\\/\\/\\/\\/\\/\\/\\/\\/\\/\\/\\/\\/\\/\\/\\/\\/#")
     print("Goodbye from GaudiExec")
 
     sys.exit(rc)
 """
     return script_template
 
-#\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\#
+# \/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\#
 
 
 from GangaCore.GPIDev.Adapters.ApplicationRuntimeHandlers import allHandlers
 allHandlers.add('GaudiExec', 'Dirac', GaudiExecDiracRTHandler)
```

### Comparing `ganga-8.7.4/ganga/GangaLHCb/Lib/RTHandlers/GaudiTemplate.py.template` & `ganga-8.7.5/ganga/GangaLHCb/Lib/RTHandlers/GaudiTemplate.py.template`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaLHCb/Lib/RTHandlers/LHCbGaudiDiracRunTimeHandler.py` & `ganga-8.7.5/ganga/GangaLHCb/Lib/RTHandlers/LHCbGaudiDiracRunTimeHandler.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaLHCb/Lib/RTHandlers/LHCbGaudiRunTimeHandler.py` & `ganga-8.7.5/ganga/GangaLHCb/Lib/RTHandlers/LHCbGaudiRunTimeHandler.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaLHCb/Lib/RTHandlers/RTHUtils.py` & `ganga-8.7.5/ganga/GangaLHCb/Lib/RTHandlers/RTHUtils.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaLHCb/Lib/RTHandlers/WorkerScript.py.template` & `ganga-8.7.5/ganga/GangaLHCb/Lib/RTHandlers/WorkerScript.py.template`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaLHCb/Lib/RTHandlers/XMLWorkerScript.py.template` & `ganga-8.7.5/ganga/GangaLHCb/Lib/RTHandlers/XMLWorkerScript.py.template`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaLHCb/Lib/Server/DiracLHCbCommands.py` & `ganga-8.7.5/ganga/GangaLHCb/Lib/Server/DiracLHCbCommands.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaLHCb/Lib/Server/DiracLHCbDefinition.py` & `ganga-8.7.5/ganga/GangaLHCb/Lib/Server/DiracLHCbDefinition.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaLHCb/Lib/Splitters/GaussSplitter.py` & `ganga-8.7.5/ganga/GangaLHCb/Lib/Splitters/GaussSplitter.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaLHCb/Lib/Splitters/LHCbSplitterUtils.py` & `ganga-8.7.5/ganga/GangaLHCb/Lib/Splitters/LHCbSplitterUtils.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaLHCb/Lib/Splitters/OptionsFileSplitter.py` & `ganga-8.7.5/ganga/GangaLHCb/Lib/Splitters/OptionsFileSplitter.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaLHCb/Lib/Splitters/SplitByFiles.py` & `ganga-8.7.5/ganga/GangaLHCb/Lib/Splitters/SplitByFiles.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaLHCb/Lib/Splitters/SplitFilesBySize.py` & `ganga-8.7.5/ganga/GangaLHCb/Lib/Splitters/SplitFilesBySize.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaLHCb/Lib/Splitters/TestSplitter.py` & `ganga-8.7.5/ganga/GangaLHCb/Lib/Splitters/TestSplitter.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaLHCb/Lib/Tasks/BKTestQuery.py` & `ganga-8.7.5/ganga/GangaLHCb/Lib/Tasks/BKTestQuery.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaLHCb/Lib/Tasks/LHCbTask.py` & `ganga-8.7.5/ganga/GangaLHCb/Lib/Tasks/LHCbTask.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaLHCb/Lib/Tasks/LHCbTaskDummySplitter.py` & `ganga-8.7.5/ganga/GangaLHCb/Lib/Tasks/LHCbTaskDummySplitter.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaLHCb/Lib/Tasks/LHCbTransform.py` & `ganga-8.7.5/ganga/GangaLHCb/Lib/Tasks/LHCbTransform.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaLHCb/Lib/Tasks/LHCbUnit.py` & `ganga-8.7.5/ganga/GangaLHCb/Lib/Tasks/LHCbUnit.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaLHCb/Lib/XMLSummary/schema.py` & `ganga-8.7.5/ganga/GangaLHCb/Lib/XMLSummary/schema.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaLHCb/Lib/XMLSummary/summary.py` & `ganga-8.7.5/ganga/GangaLHCb/Lib/XMLSummary/summary.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaLHCb/PACKAGE.py` & `ganga-8.7.5/ganga/GangaLHCb/PACKAGE.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaLHCb/Utility/LHCbDIRACenv.py` & `ganga-8.7.5/ganga/GangaLHCb/Utility/LHCbDIRACenv.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaLHCb/__init__.py` & `ganga-8.7.5/ganga/GangaLHCb/__init__.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaND280/Highland/Highland.py` & `ganga-8.7.5/ganga/GangaND280/Highland/Highland.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaND280/ND280Checkers/ND280Checker.py` & `ganga-8.7.5/ganga/GangaND280/ND280Checkers/ND280Checker.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaND280/ND280Checkers/post_status.py` & `ganga-8.7.5/ganga/GangaND280/ND280Checkers/post_status.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaND280/ND280Control/ND280Configs.py` & `ganga-8.7.5/ganga/GangaND280/ND280Control/ND280Configs.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaND280/ND280Control/runND280.py` & `ganga-8.7.5/ganga/GangaND280/ND280Control/runND280.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaND280/ND280Control/runND280CosMC.py` & `ganga-8.7.5/ganga/GangaND280/ND280Control/runND280CosMC.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaND280/ND280Control/runND280CtrlSmpl.py` & `ganga-8.7.5/ganga/GangaND280/ND280Control/runND280CtrlSmpl.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaND280/ND280Control/runND280Kin.py` & `ganga-8.7.5/ganga/GangaND280/ND280Control/runND280Kin.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaND280/ND280Control/runND280RDP.py` & `ganga-8.7.5/ganga/GangaND280/ND280Control/runND280RDP.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaND280/ND280Control/runND280SandMC.py` & `ganga-8.7.5/ganga/GangaND280/ND280Control/runND280SandMC.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaND280/ND280Dataset/ND280Dataset.py` & `ganga-8.7.5/ganga/GangaND280/ND280Dataset/ND280Dataset.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaND280/ND280Executable/ND280Executable.py` & `ganga-8.7.5/ganga/GangaND280/ND280Executable/ND280Executable.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaND280/ND280RecoValidation/RecoPlusVFT.py` & `ganga-8.7.5/ganga/GangaND280/ND280RecoValidation/RecoPlusVFT.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaND280/ND280RecoValidation/VFT_make_ana.py` & `ganga-8.7.5/ganga/GangaND280/ND280RecoValidation/VFT_make_ana.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaND280/ND280RecoValidation/oaReconPlusoaAnalysis.py` & `ganga-8.7.5/ganga/GangaND280/ND280RecoValidation/oaReconPlusoaAnalysis.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaND280/ND280Skimmer/ND280Skimmer.py` & `ganga-8.7.5/ganga/GangaND280/ND280Skimmer/ND280Skimmer.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaND280/ND280Splitter/ND280Splitter.py` & `ganga-8.7.5/ganga/GangaND280/ND280Splitter/ND280Splitter.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaND280/ND280TPCGasInteractions/TRExPlusOAAnalysis.py` & `ganga-8.7.5/ganga/GangaND280/ND280TPCGasInteractions/TRExPlusOAAnalysis.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaND280/PACKAGE.py` & `ganga-8.7.5/ganga/GangaND280/PACKAGE.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaND280/Tasks/ND280Task.py` & `ganga-8.7.5/ganga/GangaND280/Tasks/ND280Task.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaND280/Tasks/ND280Transform.py` & `ganga-8.7.5/ganga/GangaND280/Tasks/ND280Transform.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaND280/Tasks/ND280Transform_CSVEvtList.py` & `ganga-8.7.5/ganga/GangaND280/Tasks/ND280Transform_CSVEvtList.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaND280/Tasks/ND280Unit.py` & `ganga-8.7.5/ganga/GangaND280/Tasks/ND280Unit.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaND280/Tasks/ND280Unit_CSVEvtList.py` & `ganga-8.7.5/ganga/GangaND280/Tasks/ND280Unit_CSVEvtList.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaND280/__init__.py` & `ganga-8.7.5/ganga/GangaND280/__init__.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-7.0.0` & `ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-7.0.0`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-7.0.1` & `ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-7.0.1`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-7.0.2` & `ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-7.0.2`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-7.0.3` & `ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-7.0.3`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-7.0.4` & `ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-7.0.4`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-7.1.0` & `ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-7.1.0`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-7.1.1` & `ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-7.1.1`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-7.1.10` & `ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-7.1.10`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-7.1.11` & `ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-7.1.11`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-7.1.12` & `ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-7.1.12`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-7.1.13` & `ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-7.1.13`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-7.1.14` & `ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-7.1.14`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-7.1.15` & `ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-7.1.15`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-7.1.2` & `ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-7.1.2`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-7.1.3` & `ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-7.1.3`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-7.1.4` & `ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-7.1.4`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-7.1.5` & `ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-7.1.5`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-7.1.6` & `ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-7.1.6`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-7.1.7` & `ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-7.1.7`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-7.1.8` & `ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-7.1.8`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-7.1.9` & `ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-7.1.9`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-8.0.0` & `ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-8.0.0`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-8.0.1` & `ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-8.0.1`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-8.0.2` & `ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-8.0.2`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-8.0.3` & `ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-8.0.3`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-8.1.0` & `ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-8.1.0`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-8.2.0` & `ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-8.2.0`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-8.2.1` & `ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-8.2.1`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-8.2.2` & `ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-8.2.2`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-8.2.3` & `ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-8.2.3`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-8.2.4` & `ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-8.2.4`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-8.3.0` & `ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-8.3.0`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-8.3.1` & `ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-8.3.1`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-8.3.2` & `ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-8.3.2`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaRelease/ReleaseNotes-8.3.3` & `ganga-8.7.5/ganga/GangaRelease/ReleaseNotes-8.3.3`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaRelease/tools/check-new-ganga.py` & `ganga-8.7.5/ganga/GangaRelease/tools/check-new-ganga.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaRelease/tools/ganga-cvmfs-install-dev.sh` & `ganga-8.7.5/ganga/GangaRelease/tools/ganga-cvmfs-install-dev.sh`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaTest/BOOT.py` & `ganga-8.7.5/ganga/GangaTest/BOOT.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaTest/Framework/driver.py` & `ganga-8.7.5/ganga/GangaTest/Framework/driver.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaTest/Framework/htmlizer.py` & `ganga-8.7.5/ganga/GangaTest/Framework/htmlizer.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaTest/Framework/loader.py` & `ganga-8.7.5/ganga/GangaTest/Framework/loader.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaTest/Framework/runner.py` & `ganga-8.7.5/ganga/GangaTest/Framework/runner.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaTest/Framework/tests.py` & `ganga-8.7.5/ganga/GangaTest/Framework/tests.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaTest/Framework/utils.py` & `ganga-8.7.5/ganga/GangaTest/Framework/utils.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaTest/Framework/xmldifferencer.py` & `ganga-8.7.5/ganga/GangaTest/Framework/xmldifferencer.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaTest/Lib/CrashTest.py` & `ganga-8.7.5/ganga/GangaTest/Lib/CrashTest.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaTest/Lib/GListApp/GListApp.py` & `ganga-8.7.5/ganga/GangaTest/Lib/GListApp/GListApp.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaTest/Lib/StoreTestFramework.py` & `ganga-8.7.5/ganga/GangaTest/Lib/StoreTestFramework.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaTest/Lib/TFile/TFile.py` & `ganga-8.7.5/ganga/GangaTest/Lib/TFile/TFile.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaTest/Lib/TestApplication/TestApplication.py` & `ganga-8.7.5/ganga/GangaTest/Lib/TestApplication/TestApplication.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaTest/Lib/TestApplication/TestDataset.py` & `ganga-8.7.5/ganga/GangaTest/Lib/TestApplication/TestDataset.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaTest/Lib/TestMonitoringService/TestMonitoringService.py` & `ganga-8.7.5/ganga/GangaTest/Lib/TestMonitoringService/TestMonitoringService.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaTest/Lib/TestObjects.py` & `ganga-8.7.5/ganga/GangaTest/Lib/TestObjects.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaTest/Lib/TestRemoteBackend/TestRemoteBackend.py` & `ganga-8.7.5/ganga/GangaTest/Lib/TestRemoteBackend/TestRemoteBackend.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaTest/Lib/TestRemoteBackend/__init__.py` & `ganga-8.7.5/ganga/GangaTest/Lib/TestRemoteBackend/__init__.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaTest/Lib/TestRemoteBackend/server.py` & `ganga-8.7.5/ganga/GangaTest/Lib/TestRemoteBackend/server.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaTest/Lib/TestSubmitter/TestConfig2.py` & `ganga-8.7.5/ganga/GangaTest/Lib/TestSubmitter/TestConfig2.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaTest/Lib/TestSubmitter/TestSplitter.py` & `ganga-8.7.5/ganga/GangaTest/Lib/TestSubmitter/TestSplitter.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaTest/Lib/TestSubmitter/TestSubmitter.py` & `ganga-8.7.5/ganga/GangaTest/Lib/TestSubmitter/TestSubmitter.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaTest/PACKAGE.py` & `ganga-8.7.5/ganga/GangaTest/PACKAGE.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaTutorial/BOOT.py` & `ganga-8.7.5/ganga/GangaTutorial/BOOT.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaTutorial/Lib/PrimeFactorizer.py` & `ganga-8.7.5/ganga/GangaTutorial/Lib/PrimeFactorizer.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaTutorial/Lib/PrimeFactorizerSplitter.py` & `ganga-8.7.5/ganga/GangaTutorial/Lib/PrimeFactorizerSplitter.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaTutorial/Lib/PrimeTableDataset.py` & `ganga-8.7.5/ganga/GangaTutorial/Lib/PrimeTableDataset.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaTutorial/Lib/primes/prime_factor.py` & `ganga-8.7.5/ganga/GangaTutorial/Lib/primes/prime_factor.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaTutorial/Lib/primes/primes.py` & `ganga-8.7.5/ganga/GangaTutorial/Lib/primes/primes.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/GangaTutorial/PACKAGE.py` & `ganga-8.7.5/ganga/GangaTutorial/PACKAGE.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga/ganga/__init__.py` & `ganga-8.7.5/ganga/ganga/__init__.py`

 * *Files identical despite different names*

### Comparing `ganga-8.7.4/ganga.egg-info/PKG-INFO` & `ganga-8.7.5/ganga.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ganga
-Version: 8.7.4
+Version: 8.7.5
 Summary: Job management tool
 Home-page: https://github.com/ganga-devs/ganga
 Author: Ganga Developers
 Author-email: project-ganga-developers@cern.ch
 License: GPL v2
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `ganga-8.7.4/ganga.egg-info/SOURCES.txt` & `ganga-8.7.5/ganga.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -766,15 +766,15 @@
 ganga/GangaRelease/ReleaseNotes-8.2.2
 ganga/GangaRelease/ReleaseNotes-8.2.3
 ganga/GangaRelease/ReleaseNotes-8.2.4
 ganga/GangaRelease/ReleaseNotes-8.3.0
 ganga/GangaRelease/ReleaseNotes-8.3.1
 ganga/GangaRelease/ReleaseNotes-8.3.2
 ganga/GangaRelease/ReleaseNotes-8.3.3
-ganga/GangaRelease/ReleaseNotes-8.7.4
+ganga/GangaRelease/ReleaseNotes-8.7.5
 ganga/GangaRelease/tools/check-new-ganga.py
 ganga/GangaRelease/tools/ganga-cvmfs-install-dev.sh
 ganga/GangaRelease/tools/ganga-cvmfs-install.sh
 ganga/GangaTest/BOOT.py
 ganga/GangaTest/PACKAGE.py
 ganga/GangaTest/__init__.py
 ganga/GangaTest/Framework/__init__.py
```

### Comparing `ganga-8.7.4/setup.py` & `ganga-8.7.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import Command
 import subprocess
 import os
 import sys
 
 file_path = os.path.dirname(os.path.realpath(__file__))
 
-_gangaVersion = '8.7.4'
+_gangaVersion = '8.7.5'
 
 
 def version():
     return _gangaVersion
 
 
 def readme():
```

