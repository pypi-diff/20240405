# Comparing `tmp/pyguiadapter-0.2.8.tar.gz` & `tmp/pyguiadapter-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyguiadapter-0.2.8.tar", max compression
+gzip compressed data, was "pyguiadapter-0.2.9.tar", max compression
```

## Comparing `pyguiadapter-0.2.8.tar` & `pyguiadapter-0.2.9.tar`

### file list

```diff
@@ -1,245 +1,245 @@
--rw-r--r--   0        0        0    35821 2024-03-07 14:10:28.559603 pyguiadapter-0.2.8/License
--rw-r--r--   0        0        0        0 2024-03-17 02:32:55.457540 pyguiadapter-0.2.8/pyguiadapter/__init__.py
--rw-r--r--   0        0        0       53 2024-03-17 02:29:22.426087 pyguiadapter-0.2.8/pyguiadapter/adapter/__init__.py
--rw-r--r--   0        0        0     8327 2024-03-22 15:02:32.806769 pyguiadapter-0.2.8/pyguiadapter/adapter/adapter.py
--rw-r--r--   0        0        0     2840 2024-03-22 15:03:36.779855 pyguiadapter-0.2.8/pyguiadapter/adapter/bundle.py
--rw-r--r--   0        0        0      910 2024-03-17 02:30:34.866408 pyguiadapter-0.2.8/pyguiadapter/adapter/executor.py
--rw-r--r--   0        0        0     1985 2024-03-24 10:04:25.514442 pyguiadapter-0.2.8/pyguiadapter/commons.py
--rw-r--r--   0        0        0      212 2024-03-15 13:59:57.444102 pyguiadapter-0.2.8/pyguiadapter/exceptions.py
--rw-r--r--   0        0        0        0 2024-03-16 03:25:43.591074 pyguiadapter-0.2.8/pyguiadapter/interact/__init__.py
--rw-r--r--   0        0        0     5010 2024-03-21 10:36:00.956016 pyguiadapter-0.2.8/pyguiadapter/interact/ulogging.py
--rw-r--r--   0        0        0    12531 2024-03-22 15:12:24.013998 pyguiadapter-0.2.8/pyguiadapter/interact/upopup.py
--rw-r--r--   0        0        0      793 2024-03-19 13:00:20.549109 pyguiadapter-0.2.8/pyguiadapter/interact/uprint.py
--rw-r--r--   0        0        0      753 2024-03-09 14:42:49.269579 pyguiadapter-0.2.8/pyguiadapter/res/icons/abnormal.svg
--rw-r--r--   0        0        0      563 2024-03-09 14:42:49.301675 pyguiadapter-0.2.8/pyguiadapter/res/icons/acoustic.svg
--rw-r--r--   0        0        0      437 2024-03-09 14:42:49.334414 pyguiadapter-0.2.8/pyguiadapter/res/icons/activity-source.svg
--rw-r--r--   0        0        0      721 2024-03-09 14:42:49.367533 pyguiadapter-0.2.8/pyguiadapter/res/icons/add-computer.svg
--rw-r--r--   0        0        0     1074 2024-03-09 14:42:49.400158 pyguiadapter-0.2.8/pyguiadapter/res/icons/add-picture.svg
--rw-r--r--   0        0        0      556 2024-03-09 14:42:49.432714 pyguiadapter-0.2.8/pyguiadapter/res/icons/add-print.svg
--rw-r--r--   0        0        0      611 2024-03-09 14:42:49.462803 pyguiadapter-0.2.8/pyguiadapter/res/icons/add-user.svg
--rw-r--r--   0        0        0      820 2024-03-09 14:42:49.493344 pyguiadapter-0.2.8/pyguiadapter/res/icons/add-web.svg
--rw-r--r--   0        0        0      444 2024-03-09 14:42:49.525909 pyguiadapter-0.2.8/pyguiadapter/res/icons/airplay.svg
--rw-r--r--   0        0        0      744 2024-03-09 14:42:49.557957 pyguiadapter-0.2.8/pyguiadapter/res/icons/api-app.svg
--rw-r--r--   0        0        0      915 2024-03-09 14:42:49.595156 pyguiadapter-0.2.8/pyguiadapter/res/icons/application-effect.svg
--rw-r--r--   0        0        0      513 2024-03-09 14:42:49.627840 pyguiadapter-0.2.8/pyguiadapter/res/icons/application-one.svg
--rw-r--r--   0        0        0      471 2024-03-09 14:42:49.662047 pyguiadapter-0.2.8/pyguiadapter/res/icons/application-two.svg
--rw-r--r--   0        0        0      444 2024-03-09 14:42:49.695595 pyguiadapter-0.2.8/pyguiadapter/res/icons/area-map.svg
--rw-r--r--   0        0        0     1704 2024-03-09 14:42:49.730658 pyguiadapter-0.2.8/pyguiadapter/res/icons/arithmetic-buttons.svg
--rw-r--r--   0        0        0      886 2024-03-09 14:42:49.763713 pyguiadapter-0.2.8/pyguiadapter/res/icons/arithmetic-one.svg
--rw-r--r--   0        0        0     1051 2024-03-09 14:42:49.803740 pyguiadapter-0.2.8/pyguiadapter/res/icons/arrow-keys.svg
--rw-r--r--   0        0        0      510 2024-03-09 14:42:49.839218 pyguiadapter-0.2.8/pyguiadapter/res/icons/audio-file.svg
--rw-r--r--   0        0        0      806 2024-03-09 14:42:49.874542 pyguiadapter-0.2.8/pyguiadapter/res/icons/audit.svg
--rw-r--r--   0        0        0      503 2024-03-09 14:42:49.912111 pyguiadapter-0.2.8/pyguiadapter/res/icons/average.svg
--rw-r--r--   0        0        0      871 2024-03-09 14:42:49.953498 pyguiadapter-0.2.8/pyguiadapter/res/icons/bitcoin.svg
--rw-r--r--   0        0        0      753 2024-03-09 14:42:50.007926 pyguiadapter-0.2.8/pyguiadapter/res/icons/blackboard.svg
--rw-r--r--   0        0        0      633 2024-03-09 14:42:50.054525 pyguiadapter-0.2.8/pyguiadapter/res/icons/blocks-and-arrows.svg
--rw-r--r--   0        0        0      261 2024-03-09 14:42:50.096249 pyguiadapter-0.2.8/pyguiadapter/res/icons/bluetooth.svg
--rw-r--r--   0        0        0      794 2024-03-09 14:42:50.134304 pyguiadapter-0.2.8/pyguiadapter/res/icons/bookmark-three.svg
--rw-r--r--   0        0        0      981 2024-03-09 14:42:50.168174 pyguiadapter-0.2.8/pyguiadapter/res/icons/broadcast.svg
--rw-r--r--   0        0        0      993 2024-03-09 14:42:50.199705 pyguiadapter-0.2.8/pyguiadapter/res/icons/browser.svg
--rw-r--r--   0        0        0     1399 2024-03-09 14:42:50.232340 pyguiadapter-0.2.8/pyguiadapter/res/icons/bug.svg
--rw-r--r--   0        0        0      978 2024-03-09 14:42:50.265457 pyguiadapter-0.2.8/pyguiadapter/res/icons/bytedance-mini-app.svg
--rw-r--r--   0        0        0      334 2024-03-09 14:42:50.311121 pyguiadapter-0.2.8/pyguiadapter/res/icons/card-two.svg
--rw-r--r--   0        0        0      643 2024-03-09 14:42:50.383849 pyguiadapter-0.2.8/pyguiadapter/res/icons/carousel-video.svg
--rw-r--r--   0        0        0      849 2024-03-09 14:42:50.350168 pyguiadapter-0.2.8/pyguiadapter/res/icons/carousel.svg
--rw-r--r--   0        0        0      685 2024-03-09 14:42:50.414066 pyguiadapter-0.2.8/pyguiadapter/res/icons/cast-screen.svg
--rw-r--r--   0        0        0      472 2024-03-09 14:42:50.447609 pyguiadapter-0.2.8/pyguiadapter/res/icons/category-management.svg
--rw-r--r--   0        0        0      443 2024-03-09 14:42:50.478933 pyguiadapter-0.2.8/pyguiadapter/res/icons/caution.svg
--rw-r--r--   0        0        0     1016 2024-03-09 14:42:50.509609 pyguiadapter-0.2.8/pyguiadapter/res/icons/certificate.svg
--rw-r--r--   0        0        0      634 2024-03-09 14:42:50.540729 pyguiadapter-0.2.8/pyguiadapter/res/icons/check-one.svg
--rw-r--r--   0        0        0      697 2024-03-09 14:42:50.572289 pyguiadapter-0.2.8/pyguiadapter/res/icons/checklist.svg
--rw-r--r--   0        0        0     1023 2024-03-09 14:42:50.603351 pyguiadapter-0.2.8/pyguiadapter/res/icons/chip.svg
--rw-r--r--   0        0        0      519 2024-03-09 14:42:50.635463 pyguiadapter-0.2.8/pyguiadapter/res/icons/classroom.svg
--rw-r--r--   0        0        0      478 2024-03-09 14:42:50.667994 pyguiadapter-0.2.8/pyguiadapter/res/icons/clipboard.svg
--rw-r--r--   0        0        0      576 2024-03-09 14:42:50.700513 pyguiadapter-0.2.8/pyguiadapter/res/icons/close-one.svg
--rw-r--r--   0        0        0     1211 2024-03-09 14:42:50.732035 pyguiadapter-0.2.8/pyguiadapter/res/icons/cloud-storage.svg
--rw-r--r--   0        0        0      536 2024-03-09 14:42:50.795255 pyguiadapter-0.2.8/pyguiadapter/res/icons/code-brackets.svg
--rw-r--r--   0        0        0      547 2024-03-09 14:42:50.826965 pyguiadapter-0.2.8/pyguiadapter/res/icons/code-download.svg
--rw-r--r--   0        0        0      639 2024-03-09 14:42:50.860630 pyguiadapter-0.2.8/pyguiadapter/res/icons/code-laptop.svg
--rw-r--r--   0        0        0      346 2024-03-09 14:42:50.893306 pyguiadapter-0.2.8/pyguiadapter/res/icons/code-one.svg
--rw-r--r--   0        0        0      441 2024-03-09 14:42:50.764191 pyguiadapter-0.2.8/pyguiadapter/res/icons/code.svg
--rw-r--r--   0        0        0      831 2024-03-09 14:42:50.925357 pyguiadapter-0.2.8/pyguiadapter/res/icons/collect-computer.svg
--rw-r--r--   0        0        0      732 2024-03-09 14:42:50.958885 pyguiadapter-0.2.8/pyguiadapter/res/icons/collect-laptop.svg
--rw-r--r--   0        0        0     1181 2024-03-09 14:42:50.991576 pyguiadapter-0.2.8/pyguiadapter/res/icons/collect-picture.svg
--rw-r--r--   0        0        0     1118 2024-03-09 14:42:51.022102 pyguiadapter-0.2.8/pyguiadapter/res/icons/color-card.svg
--rw-r--r--   0        0        0     1289 2024-03-09 14:42:51.052795 pyguiadapter-0.2.8/pyguiadapter/res/icons/command.svg
--rw-r--r--   0        0        0      371 2024-03-09 14:42:51.119127 pyguiadapter-0.2.8/pyguiadapter/res/icons/comment-one.svg
--rw-r--r--   0        0        0      581 2024-03-09 14:42:51.085912 pyguiadapter-0.2.8/pyguiadapter/res/icons/comment.svg
--rw-r--r--   0        0        0      553 2024-03-09 14:42:51.153360 pyguiadapter-0.2.8/pyguiadapter/res/icons/comments.svg
--rw-r--r--   0        0        0      628 2024-03-09 14:42:51.186924 pyguiadapter-0.2.8/pyguiadapter/res/icons/communication.svg
--rw-r--r--   0        0        0      753 2024-03-09 14:42:51.219995 pyguiadapter-0.2.8/pyguiadapter/res/icons/compass.svg
--rw-r--r--   0        0        0     1110 2024-03-09 14:42:51.250504 pyguiadapter-0.2.8/pyguiadapter/res/icons/compression.svg
--rw-r--r--   0        0        0      556 2024-03-09 14:42:51.284109 pyguiadapter-0.2.8/pyguiadapter/res/icons/computer.svg
--rw-r--r--   0        0        0      447 2024-03-09 14:42:51.317638 pyguiadapter-0.2.8/pyguiadapter/res/icons/cones.svg
--rw-r--r--   0        0        0     1850 2024-03-09 14:42:51.350759 pyguiadapter-0.2.8/pyguiadapter/res/icons/connect.svg
--rw-r--r--   0        0        0      620 2024-03-09 14:42:51.382155 pyguiadapter-0.2.8/pyguiadapter/res/icons/copy-one.svg
--rw-r--r--   0        0        0      524 2024-03-09 14:42:51.414093 pyguiadapter-0.2.8/pyguiadapter/res/icons/copyright.svg
--rw-r--r--   0        0        0     2644 2024-03-09 14:42:51.445689 pyguiadapter-0.2.8/pyguiadapter/res/icons/cpu.svg
--rw-r--r--   0        0        0      516 2024-03-09 14:42:51.477786 pyguiadapter-0.2.8/pyguiadapter/res/icons/cross-ring-two.svg
--rw-r--r--   0        0        0      895 2024-03-09 14:42:51.510328 pyguiadapter-0.2.8/pyguiadapter/res/icons/cube-four.svg
--rw-r--r--   0        0        0      369 2024-03-09 14:42:51.543870 pyguiadapter-0.2.8/pyguiadapter/res/icons/curve-adjustment.svg
--rw-r--r--   0        0        0     1177 2024-03-09 14:42:51.576599 pyguiadapter-0.2.8/pyguiadapter/res/icons/cuvette.svg
--rw-r--r--   0        0        0     1199 2024-03-09 14:42:51.608710 pyguiadapter-0.2.8/pyguiadapter/res/icons/dashboard-one.svg
--rw-r--r--   0        0        0     1332 2024-03-09 14:42:51.643261 pyguiadapter-0.2.8/pyguiadapter/res/icons/dashboard-two.svg
--rw-r--r--   0        0        0     1221 2024-03-09 14:42:51.709446 pyguiadapter-0.2.8/pyguiadapter/res/icons/data-all.svg
--rw-r--r--   0        0        0     1239 2024-03-09 14:42:51.742529 pyguiadapter-0.2.8/pyguiadapter/res/icons/data-display.svg
--rw-r--r--   0        0        0     1255 2024-03-09 14:42:51.777672 pyguiadapter-0.2.8/pyguiadapter/res/icons/data-lock.svg
--rw-r--r--   0        0        0      829 2024-03-09 14:42:51.813216 pyguiadapter-0.2.8/pyguiadapter/res/icons/data-screen.svg
--rw-r--r--   0        0        0      833 2024-03-09 14:42:51.846297 pyguiadapter-0.2.8/pyguiadapter/res/icons/data-server.svg
--rw-r--r--   0        0        0     1448 2024-03-09 14:42:51.879954 pyguiadapter-0.2.8/pyguiadapter/res/icons/data-switching.svg
--rw-r--r--   0        0        0     1209 2024-03-09 14:42:51.911088 pyguiadapter-0.2.8/pyguiadapter/res/icons/data-user.svg
--rw-r--r--   0        0        0      794 2024-03-09 14:42:51.675906 pyguiadapter-0.2.8/pyguiadapter/res/icons/data.svg
--rw-r--r--   0        0        0     1588 2024-03-09 14:42:51.944604 pyguiadapter-0.2.8/pyguiadapter/res/icons/database-alert.svg
--rw-r--r--   0        0        0     1606 2024-03-09 14:42:51.977363 pyguiadapter-0.2.8/pyguiadapter/res/icons/database-code.svg
--rw-r--r--   0        0        0     1596 2024-03-09 14:42:52.007892 pyguiadapter-0.2.8/pyguiadapter/res/icons/database-config.svg
--rw-r--r--   0        0        0     1513 2024-03-09 14:42:52.040009 pyguiadapter-0.2.8/pyguiadapter/res/icons/database-download.svg
--rw-r--r--   0        0        0     1516 2024-03-09 14:42:52.074200 pyguiadapter-0.2.8/pyguiadapter/res/icons/database-enter.svg
--rw-r--r--   0        0        0     1528 2024-03-09 14:42:52.106242 pyguiadapter-0.2.8/pyguiadapter/res/icons/database-fail.svg
--rw-r--r--   0        0        0     1513 2024-03-09 14:42:52.137391 pyguiadapter-0.2.8/pyguiadapter/res/icons/database-first.svg
--rw-r--r--   0        0        0     1492 2024-03-09 14:42:52.170998 pyguiadapter-0.2.8/pyguiadapter/res/icons/database-forbid.svg
--rw-r--r--   0        0        0     1738 2024-03-09 14:42:52.201569 pyguiadapter-0.2.8/pyguiadapter/res/icons/database-lock.svg
--rw-r--r--   0        0        0     1195 2024-03-09 14:42:52.268001 pyguiadapter-0.2.8/pyguiadapter/res/icons/database-network-point.svg
--rw-r--r--   0        0        0     1770 2024-03-09 14:42:52.234122 pyguiadapter-0.2.8/pyguiadapter/res/icons/database-network.svg
--rw-r--r--   0        0        0     1637 2024-03-09 14:42:52.300547 pyguiadapter-0.2.8/pyguiadapter/res/icons/database-point.svg
--rw-r--r--   0        0        0     1390 2024-03-09 14:42:52.333068 pyguiadapter-0.2.8/pyguiadapter/res/icons/database-position.svg
--rw-r--r--   0        0        0     1504 2024-03-09 14:42:52.364241 pyguiadapter-0.2.8/pyguiadapter/res/icons/database-power.svg
--rw-r--r--   0        0        0     1528 2024-03-09 14:42:52.397951 pyguiadapter-0.2.8/pyguiadapter/res/icons/database-proportion.svg
--rw-r--r--   0        0        0     1908 2024-03-09 14:42:52.428304 pyguiadapter-0.2.8/pyguiadapter/res/icons/database-search.svg
--rw-r--r--   0        0        0     1542 2024-03-09 14:42:52.460505 pyguiadapter-0.2.8/pyguiadapter/res/icons/database-setting.svg
--rw-r--r--   0        0        0     1504 2024-03-09 14:42:52.494171 pyguiadapter-0.2.8/pyguiadapter/res/icons/database-success.svg
--rw-r--r--   0        0        0     1638 2024-03-09 14:42:52.525731 pyguiadapter-0.2.8/pyguiadapter/res/icons/database-sync.svg
--rw-r--r--   0        0        0     1492 2024-03-09 14:42:52.559018 pyguiadapter-0.2.8/pyguiadapter/res/icons/database-time.svg
--rw-r--r--   0        0        0      762 2024-03-09 14:42:52.591111 pyguiadapter-0.2.8/pyguiadapter/res/icons/date-comes-back.svg
--rw-r--r--   0        0        0      470 2024-03-09 14:42:52.624367 pyguiadapter-0.2.8/pyguiadapter/res/icons/diamond-one.svg
--rw-r--r--   0        0        0      470 2024-03-09 14:42:52.657545 pyguiadapter-0.2.8/pyguiadapter/res/icons/diamond-three.svg
--rw-r--r--   0        0        0      466 2024-03-09 14:42:52.689586 pyguiadapter-0.2.8/pyguiadapter/res/icons/diamond-two.svg
--rw-r--r--   0        0        0      855 2024-03-09 14:42:52.754775 pyguiadapter-0.2.8/pyguiadapter/res/icons/disk-one.svg
--rw-r--r--   0        0        0      533 2024-03-09 14:42:52.788667 pyguiadapter-0.2.8/pyguiadapter/res/icons/disk-two.svg
--rw-r--r--   0        0        0      599 2024-03-09 14:42:52.722118 pyguiadapter-0.2.8/pyguiadapter/res/icons/disk.svg
--rw-r--r--   0        0        0      646 2024-03-09 14:42:52.821412 pyguiadapter-0.2.8/pyguiadapter/res/icons/document-folder.svg
--rw-r--r--   0        0        0      957 2024-03-09 14:42:52.852474 pyguiadapter-0.2.8/pyguiadapter/res/icons/download-one.svg
--rw-r--r--   0        0        0      649 2024-03-09 14:42:52.884528 pyguiadapter-0.2.8/pyguiadapter/res/icons/download-three.svg
--rw-r--r--   0        0        0      730 2024-03-09 14:42:52.917857 pyguiadapter-0.2.8/pyguiadapter/res/icons/download-two.svg
--rw-r--r--   0        0        0      827 2024-03-09 14:42:52.952370 pyguiadapter-0.2.8/pyguiadapter/res/icons/download-web.svg
--rw-r--r--   0        0        0      500 2024-03-09 14:42:52.983983 pyguiadapter-0.2.8/pyguiadapter/res/icons/electrocardiogram.svg
--rw-r--r--   0        0        0      568 2024-03-09 14:42:53.017497 pyguiadapter-0.2.8/pyguiadapter/res/icons/email-down.svg
--rw-r--r--   0        0        0      567 2024-03-09 14:42:53.052087 pyguiadapter-0.2.8/pyguiadapter/res/icons/email-push.svg
--rw-r--r--   0        0        0      634 2024-03-09 14:42:53.117840 pyguiadapter-0.2.8/pyguiadapter/res/icons/experiment-one.svg
--rw-r--r--   0        0        0      731 2024-03-09 14:42:53.084199 pyguiadapter-0.2.8/pyguiadapter/res/icons/experiment.svg
--rw-r--r--   0        0        0      680 2024-03-09 14:42:53.152428 pyguiadapter-0.2.8/pyguiadapter/res/icons/figma-component.svg
--rw-r--r--   0        0        0      652 2024-03-09 14:42:53.185744 pyguiadapter-0.2.8/pyguiadapter/res/icons/file-addition.svg
--rw-r--r--   0        0        0      664 2024-03-09 14:42:53.217973 pyguiadapter-0.2.8/pyguiadapter/res/icons/file-code.svg
--rw-r--r--   0        0        0      856 2024-03-09 14:42:53.249496 pyguiadapter-0.2.8/pyguiadapter/res/icons/file-conversion.svg
--rw-r--r--   0        0        0      772 2024-03-09 14:42:53.281733 pyguiadapter-0.2.8/pyguiadapter/res/icons/file-display.svg
--rw-r--r--   0        0        0     1316 2024-03-09 14:42:53.313837 pyguiadapter-0.2.8/pyguiadapter/res/icons/file-pdf-one.svg
--rw-r--r--   0        0        0     1381 2024-03-09 14:42:53.347168 pyguiadapter-0.2.8/pyguiadapter/res/icons/file-ppt.svg
--rw-r--r--   0        0        0      658 2024-03-09 14:42:53.382365 pyguiadapter-0.2.8/pyguiadapter/res/icons/file-protection.svg
--rw-r--r--   0        0        0      652 2024-03-09 14:42:53.417579 pyguiadapter-0.2.8/pyguiadapter/res/icons/file-text.svg
--rw-r--r--   0        0        0      468 2024-03-09 14:42:53.455122 pyguiadapter-0.2.8/pyguiadapter/res/icons/file-word.svg
--rw-r--r--   0        0        0      931 2024-03-09 14:42:53.486147 pyguiadapter-0.2.8/pyguiadapter/res/icons/film.svg
--rw-r--r--   0        0        0      734 2024-03-09 14:42:53.517258 pyguiadapter-0.2.8/pyguiadapter/res/icons/flask.svg
--rw-r--r--   0        0        0      851 2024-03-09 14:42:53.549857 pyguiadapter-0.2.8/pyguiadapter/res/icons/game-handle.svg
--rw-r--r--   0        0        0      989 2024-03-09 14:42:53.581226 pyguiadapter-0.2.8/pyguiadapter/res/icons/help.svg
--rw-r--r--   0        0        0      545 2024-03-09 14:42:53.612330 pyguiadapter-0.2.8/pyguiadapter/res/icons/hexagon-one.svg
--rw-r--r--   0        0        0      794 2024-03-09 14:42:53.643884 pyguiadapter-0.2.8/pyguiadapter/res/icons/id-card-h.svg
--rw-r--r--   0        0        0      935 2024-03-09 14:42:53.676625 pyguiadapter-0.2.8/pyguiadapter/res/icons/info.svg
--rw-r--r--   0        0        0      696 2024-03-09 14:42:53.708204 pyguiadapter-0.2.8/pyguiadapter/res/icons/install.svg
--rw-r--r--   0        0        0    11551 2024-03-17 02:22:55.741177 pyguiadapter-0.2.8/pyguiadapter/res/icons/LICENSE.txt
--rw-r--r--   0        0        0      683 2024-03-09 14:42:53.741316 pyguiadapter-0.2.8/pyguiadapter/res/icons/many-to-many.svg
--rw-r--r--   0        0        0      602 2024-03-09 14:42:53.805746 pyguiadapter-0.2.8/pyguiadapter/res/icons/message-emoji.svg
--rw-r--r--   0        0        0      522 2024-03-09 14:42:53.840353 pyguiadapter-0.2.8/pyguiadapter/res/icons/message-one.svg
--rw-r--r--   0        0        0      763 2024-03-09 14:42:53.871762 pyguiadapter-0.2.8/pyguiadapter/res/icons/message-privacy.svg
--rw-r--r--   0        0        0      648 2024-03-09 14:42:53.905271 pyguiadapter-0.2.8/pyguiadapter/res/icons/message-search.svg
--rw-r--r--   0        0        0      679 2024-03-09 14:42:53.935786 pyguiadapter-0.2.8/pyguiadapter/res/icons/message-security.svg
--rw-r--r--   0        0        0      485 2024-03-09 14:42:53.970910 pyguiadapter-0.2.8/pyguiadapter/res/icons/message-sent.svg
--rw-r--r--   0        0        0      577 2024-03-09 14:42:54.004586 pyguiadapter-0.2.8/pyguiadapter/res/icons/message-success.svg
--rw-r--r--   0        0        0      550 2024-03-09 14:42:54.037266 pyguiadapter-0.2.8/pyguiadapter/res/icons/message-unread.svg
--rw-r--r--   0        0        0      738 2024-03-09 14:42:53.773734 pyguiadapter-0.2.8/pyguiadapter/res/icons/message.svg
--rw-r--r--   0        0        0      537 2024-03-09 14:42:54.071502 pyguiadapter-0.2.8/pyguiadapter/res/icons/mini-sd-card.svg
--rw-r--r--   0        0        0      521 2024-03-09 14:42:54.103643 pyguiadapter-0.2.8/pyguiadapter/res/icons/monitor.svg
--rw-r--r--   0        0        0     1053 2024-03-09 14:42:54.135574 pyguiadapter-0.2.8/pyguiadapter/res/icons/more-app.svg
--rw-r--r--   0        0        0      971 2024-03-09 14:42:54.204781 pyguiadapter-0.2.8/pyguiadapter/res/icons/movie-board.svg
--rw-r--r--   0        0        0     1213 2024-03-09 14:42:54.169203 pyguiadapter-0.2.8/pyguiadapter/res/icons/movie.svg
--rw-r--r--   0        0        0      995 2024-03-09 14:42:54.236957 pyguiadapter-0.2.8/pyguiadapter/res/icons/multi-function-knife.svg
--rw-r--r--   0        0        0      835 2024-03-09 14:42:54.270059 pyguiadapter-0.2.8/pyguiadapter/res/icons/notebook-one.svg
--rw-r--r--   0        0        0      626 2024-03-09 14:42:54.305013 pyguiadapter-0.2.8/pyguiadapter/res/icons/octagon.svg
--rw-r--r--   0        0        0      575 2024-03-09 14:42:54.338102 pyguiadapter-0.2.8/pyguiadapter/res/icons/online-meeting.svg
--rw-r--r--   0        0        0      227 2024-03-09 14:42:54.370839 pyguiadapter-0.2.8/pyguiadapter/res/icons/oval-one.svg
--rw-r--r--   0        0        0      537 2024-03-09 14:42:54.440082 pyguiadapter-0.2.8/pyguiadapter/res/icons/page-template.svg
--rw-r--r--   0        0        0      440 2024-03-09 14:42:54.403964 pyguiadapter-0.2.8/pyguiadapter/res/icons/page.svg
--rw-r--r--   0        0        0      412 2024-03-09 14:42:54.473151 pyguiadapter-0.2.8/pyguiadapter/res/icons/parallelogram.svg
--rw-r--r--   0        0        0      633 2024-03-09 14:42:54.508004 pyguiadapter-0.2.8/pyguiadapter/res/icons/pay-code.svg
--rw-r--r--   0        0        0      509 2024-03-09 14:42:54.540081 pyguiadapter-0.2.8/pyguiadapter/res/icons/pentagon-one.svg
--rw-r--r--   0        0        0      980 2024-03-09 14:42:54.573293 pyguiadapter-0.2.8/pyguiadapter/res/icons/people-plus-one.svg
--rw-r--r--   0        0        0     1040 2024-03-09 14:42:54.640249 pyguiadapter-0.2.8/pyguiadapter/res/icons/phone-incoming-one.svg
--rw-r--r--   0        0        0     1029 2024-03-09 14:42:54.606929 pyguiadapter-0.2.8/pyguiadapter/res/icons/phone-incoming.svg
--rw-r--r--   0        0        0     1083 2024-03-09 14:42:54.672454 pyguiadapter-0.2.8/pyguiadapter/res/icons/phone-missed.svg
--rw-r--r--   0        0        0     1015 2024-03-09 14:42:54.735192 pyguiadapter-0.2.8/pyguiadapter/res/icons/phone-outgoing-one.svg
--rw-r--r--   0        0        0     1008 2024-03-09 14:42:54.704958 pyguiadapter-0.2.8/pyguiadapter/res/icons/phone-outgoing.svg
--rw-r--r--   0        0        0      811 2024-03-09 14:42:54.769268 pyguiadapter-0.2.8/pyguiadapter/res/icons/phone-telephone.svg
--rw-r--r--   0        0        0      935 2024-03-09 14:42:54.800614 pyguiadapter-0.2.8/pyguiadapter/res/icons/phone-video-call.svg
--rw-r--r--   0        0        0      974 2024-03-09 14:42:54.832344 pyguiadapter-0.2.8/pyguiadapter/res/icons/platte.svg
--rw-r--r--   0        0        0      473 2024-03-09 14:42:54.868011 pyguiadapter-0.2.8/pyguiadapter/res/icons/play.svg
--rw-r--r--   0        0        0      434 2024-03-09 14:42:54.900949 pyguiadapter-0.2.8/pyguiadapter/res/icons/powerpoint.svg
--rw-r--r--   0        0        0      612 2024-03-09 14:42:54.933463 pyguiadapter-0.2.8/pyguiadapter/res/icons/ppt.svg
--rw-r--r--   0        0        0      427 2024-03-09 14:42:54.965026 pyguiadapter-0.2.8/pyguiadapter/res/icons/puzzle.svg
--rw-r--r--   0        0        0      364 2024-03-09 14:42:54.997189 pyguiadapter-0.2.8/pyguiadapter/res/icons/quadrilateral.svg
--rw-r--r--   0        0        0      783 2024-03-09 14:42:55.060859 pyguiadapter-0.2.8/pyguiadapter/res/icons/record-disc.svg
--rw-r--r--   0        0        0      880 2024-03-09 14:42:55.028755 pyguiadapter-0.2.8/pyguiadapter/res/icons/record.svg
--rw-r--r--   0        0        0      319 2024-03-09 14:42:55.123563 pyguiadapter-0.2.8/pyguiadapter/res/icons/rectangle-one.svg
--rw-r--r--   0        0        0      328 2024-03-09 14:42:55.156079 pyguiadapter-0.2.8/pyguiadapter/res/icons/rectangle-small.svg
--rw-r--r--   0        0        0      319 2024-03-09 14:42:55.092477 pyguiadapter-0.2.8/pyguiadapter/res/icons/rectangle.svg
--rw-r--r--   0        0        0      591 2024-03-09 16:01:09.963050 pyguiadapter-0.2.8/pyguiadapter/res/icons/rename.py
--rw-r--r--   0        0        0      425 2024-03-09 14:42:55.187919 pyguiadapter-0.2.8/pyguiadapter/res/icons/right-angle.svg
--rw-r--r--   0        0        0      217 2024-03-09 14:42:55.218332 pyguiadapter-0.2.8/pyguiadapter/res/icons/round.svg
--rw-r--r--   0        0        0      901 2024-03-09 14:42:55.250585 pyguiadapter-0.2.8/pyguiadapter/res/icons/rule-two.svg
--rw-r--r--   0        0        0      794 2024-03-09 14:42:55.314442 pyguiadapter-0.2.8/pyguiadapter/res/icons/ruler-one.svg
--rw-r--r--   0        0        0      926 2024-03-09 14:42:55.282289 pyguiadapter-0.2.8/pyguiadapter/res/icons/ruler.svg
--rw-r--r--   0        0        0      583 2024-03-09 14:42:55.344890 pyguiadapter-0.2.8/pyguiadapter/res/icons/sd-card.svg
--rw-r--r--   0        0        0     1259 2024-03-09 14:42:55.377061 pyguiadapter-0.2.8/pyguiadapter/res/icons/setting-computer.svg
--rw-r--r--   0        0        0     1148 2024-03-09 14:42:55.409597 pyguiadapter-0.2.8/pyguiadapter/res/icons/setting-laptop.svg
--rw-r--r--   0        0        0     1443 2024-03-09 14:42:55.444676 pyguiadapter-0.2.8/pyguiadapter/res/icons/setting-two.svg
--rw-r--r--   0        0        0      980 2024-03-09 14:42:55.477262 pyguiadapter-0.2.8/pyguiadapter/res/icons/share-one.svg
--rw-r--r--   0        0        0      328 2024-03-09 14:42:55.541521 pyguiadapter-0.2.8/pyguiadapter/res/icons/square-small.svg
--rw-r--r--   0        0        0      317 2024-03-09 14:42:55.509301 pyguiadapter-0.2.8/pyguiadapter/res/icons/square.svg
--rw-r--r--   0        0        0      954 2024-03-09 14:42:55.574211 pyguiadapter-0.2.8/pyguiadapter/res/icons/system.svg
--rw-r--r--   0        0        0      895 2024-03-09 14:42:55.606324 pyguiadapter-0.2.8/pyguiadapter/res/icons/table-file.svg
--rw-r--r--   0        0        0     1216 2024-03-09 14:42:55.637907 pyguiadapter-0.2.8/pyguiadapter/res/icons/tape.svg
--rw-r--r--   0        0        0      465 2024-03-09 14:42:55.669026 pyguiadapter-0.2.8/pyguiadapter/res/icons/terminal.svg
--rw-r--r--   0        0        0      751 2024-03-09 14:42:55.704103 pyguiadapter-0.2.8/pyguiadapter/res/icons/test-tube.svg
--rw-r--r--   0        0        0      724 2024-03-09 14:42:55.736266 pyguiadapter-0.2.8/pyguiadapter/res/icons/thermometer.svg
--rw-r--r--   0        0        0      425 2024-03-09 14:42:55.768900 pyguiadapter-0.2.8/pyguiadapter/res/icons/tips-one.svg
--rw-r--r--   0        0        0      510 2024-03-09 14:42:55.800445 pyguiadapter-0.2.8/pyguiadapter/res/icons/tool.svg
--rw-r--r--   0        0        0      587 2024-03-09 14:42:55.867211 pyguiadapter-0.2.8/pyguiadapter/res/icons/topic-discussion.svg
--rw-r--r--   0        0        0     1027 2024-03-09 14:42:55.835066 pyguiadapter-0.2.8/pyguiadapter/res/icons/topic.svg
--rw-r--r--   0        0        0      413 2024-03-09 14:42:55.900240 pyguiadapter-0.2.8/pyguiadapter/res/icons/trapezoid.svg
--rw-r--r--   0        0        0      831 2024-03-09 14:42:55.935077 pyguiadapter-0.2.8/pyguiadapter/res/icons/tree-list.svg
--rw-r--r--   0        0        0     1970 2024-03-09 14:42:55.998698 pyguiadapter-0.2.8/pyguiadapter/res/icons/triangle-ruler.svg
--rw-r--r--   0        0        0      468 2024-03-09 14:42:55.966416 pyguiadapter-0.2.8/pyguiadapter/res/icons/triangle.svg
--rw-r--r--   0        0        0      717 2024-03-09 14:42:56.029033 pyguiadapter-0.2.8/pyguiadapter/res/icons/vial.svg
--rw-r--r--   0        0        0     1823 2024-03-09 14:42:56.061697 pyguiadapter-0.2.8/pyguiadapter/res/icons/video.svg
--rw-r--r--   0        0        0      706 2024-03-09 14:42:56.093308 pyguiadapter-0.2.8/pyguiadapter/res/icons/view-grid-card.svg
--rw-r--r--   0        0        0      775 2024-03-09 14:42:56.123098 pyguiadapter-0.2.8/pyguiadapter/res/icons/view-grid-detail.svg
--rw-r--r--   0        0        0      887 2024-03-09 14:42:56.156703 pyguiadapter-0.2.8/pyguiadapter/res/icons/view-grid-list.svg
--rw-r--r--   0        0        0      642 2024-03-09 14:42:56.218845 pyguiadapter-0.2.8/pyguiadapter/res/icons/voice-input.svg
--rw-r--r--   0        0        0      903 2024-03-09 14:42:56.251446 pyguiadapter-0.2.8/pyguiadapter/res/icons/voice-message.svg
--rw-r--r--   0        0        0      685 2024-03-09 14:42:56.284535 pyguiadapter-0.2.8/pyguiadapter/res/icons/voice-one.svg
--rw-r--r--   0        0        0      508 2024-03-09 14:42:56.187304 pyguiadapter-0.2.8/pyguiadapter/res/icons/voice.svg
--rw-r--r--   0        0        0     1173 2024-03-09 14:42:56.317102 pyguiadapter-0.2.8/pyguiadapter/res/icons/weixin-mini-app.svg
--rw-r--r--   0        0        0      809 2024-03-09 14:42:56.349946 pyguiadapter-0.2.8/pyguiadapter/res/icons/wifi.svg
--rw-r--r--   0        0        0      976 2024-03-09 14:42:56.381588 pyguiadapter-0.2.8/pyguiadapter/res/icons/zip.svg
--rw-r--r--   0        0        0        0 2024-03-15 05:08:37.625966 pyguiadapter-0.2.8/pyguiadapter/ui/__init__.py
--rw-r--r--   0        0        0     1462 2024-03-22 14:55:24.908558 pyguiadapter-0.2.8/pyguiadapter/ui/config.py
--rw-r--r--   0        0        0        0 2024-03-15 11:37:47.907987 pyguiadapter-0.2.8/pyguiadapter/ui/generated/__init__.py
--rw-r--r--   0        0        0     6996 2024-03-22 12:51:51.481008 pyguiadapter-0.2.8/pyguiadapter/ui/generated/ui_execution_window.py
--rw-r--r--   0        0        0     2844 2024-03-22 12:51:51.656489 pyguiadapter-0.2.8/pyguiadapter/ui/generated/ui_initialization_window.py
--rw-r--r--   0        0        0     4413 2024-03-22 12:51:51.830703 pyguiadapter-0.2.8/pyguiadapter/ui/generated/ui_selection_window.py
--rw-r--r--   0        0        0     1460 2024-03-19 13:11:31.754220 pyguiadapter-0.2.8/pyguiadapter/ui/styles.py
--rw-r--r--   0        0        0     1109 2024-03-19 13:11:19.291844 pyguiadapter-0.2.8/pyguiadapter/ui/utils.py
--rw-r--r--   0        0        0        0 2024-03-15 12:09:31.827626 pyguiadapter-0.2.8/pyguiadapter/ui/window/__init__.py
--rw-r--r--   0        0        0    17385 2024-03-25 16:57:48.958090 pyguiadapter-0.2.8/pyguiadapter/ui/window/execution.py
--rw-r--r--   0        0        0     6185 2024-03-22 14:58:04.952081 pyguiadapter-0.2.8/pyguiadapter/ui/window/initialization.py
--rw-r--r--   0        0        0     8273 2024-03-22 14:56:06.155478 pyguiadapter-0.2.8/pyguiadapter/ui/window/selection.py
--rw-r--r--   0        0        0      688 2024-03-25 16:58:12.207592 pyguiadapter-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     8610 2024-03-24 02:40:52.393460 pyguiadapter-0.2.8/README.md
--rw-r--r--   0        0        0     9140 1970-01-01 00:00:00.000000 pyguiadapter-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0    35821 2024-03-07 14:10:28.559603 pyguiadapter-0.2.9/License
+-rw-r--r--   0        0        0        0 2024-03-17 02:32:55.457540 pyguiadapter-0.2.9/pyguiadapter/__init__.py
+-rw-r--r--   0        0        0       53 2024-03-17 02:29:22.426087 pyguiadapter-0.2.9/pyguiadapter/adapter/__init__.py
+-rw-r--r--   0        0        0     8327 2024-03-22 15:02:32.806769 pyguiadapter-0.2.9/pyguiadapter/adapter/adapter.py
+-rw-r--r--   0        0        0     2840 2024-03-22 15:03:36.779855 pyguiadapter-0.2.9/pyguiadapter/adapter/bundle.py
+-rw-r--r--   0        0        0      910 2024-03-17 02:30:34.866408 pyguiadapter-0.2.9/pyguiadapter/adapter/executor.py
+-rw-r--r--   0        0        0     1985 2024-03-24 10:04:25.514442 pyguiadapter-0.2.9/pyguiadapter/commons.py
+-rw-r--r--   0        0        0      212 2024-03-15 13:59:57.444102 pyguiadapter-0.2.9/pyguiadapter/exceptions.py
+-rw-r--r--   0        0        0        0 2024-03-16 03:25:43.591074 pyguiadapter-0.2.9/pyguiadapter/interact/__init__.py
+-rw-r--r--   0        0        0     5010 2024-03-21 10:36:00.956016 pyguiadapter-0.2.9/pyguiadapter/interact/ulogging.py
+-rw-r--r--   0        0        0    12531 2024-03-22 15:12:24.013998 pyguiadapter-0.2.9/pyguiadapter/interact/upopup.py
+-rw-r--r--   0        0        0      793 2024-03-19 13:00:20.549109 pyguiadapter-0.2.9/pyguiadapter/interact/uprint.py
+-rw-r--r--   0        0        0      753 2024-03-09 14:42:49.269579 pyguiadapter-0.2.9/pyguiadapter/res/icons/abnormal.svg
+-rw-r--r--   0        0        0      563 2024-03-09 14:42:49.301675 pyguiadapter-0.2.9/pyguiadapter/res/icons/acoustic.svg
+-rw-r--r--   0        0        0      437 2024-03-09 14:42:49.334414 pyguiadapter-0.2.9/pyguiadapter/res/icons/activity-source.svg
+-rw-r--r--   0        0        0      721 2024-03-09 14:42:49.367533 pyguiadapter-0.2.9/pyguiadapter/res/icons/add-computer.svg
+-rw-r--r--   0        0        0     1074 2024-03-09 14:42:49.400158 pyguiadapter-0.2.9/pyguiadapter/res/icons/add-picture.svg
+-rw-r--r--   0        0        0      556 2024-03-09 14:42:49.432714 pyguiadapter-0.2.9/pyguiadapter/res/icons/add-print.svg
+-rw-r--r--   0        0        0      611 2024-03-09 14:42:49.462803 pyguiadapter-0.2.9/pyguiadapter/res/icons/add-user.svg
+-rw-r--r--   0        0        0      820 2024-03-09 14:42:49.493344 pyguiadapter-0.2.9/pyguiadapter/res/icons/add-web.svg
+-rw-r--r--   0        0        0      444 2024-03-09 14:42:49.525909 pyguiadapter-0.2.9/pyguiadapter/res/icons/airplay.svg
+-rw-r--r--   0        0        0      744 2024-03-09 14:42:49.557957 pyguiadapter-0.2.9/pyguiadapter/res/icons/api-app.svg
+-rw-r--r--   0        0        0      915 2024-03-09 14:42:49.595156 pyguiadapter-0.2.9/pyguiadapter/res/icons/application-effect.svg
+-rw-r--r--   0        0        0      513 2024-03-09 14:42:49.627840 pyguiadapter-0.2.9/pyguiadapter/res/icons/application-one.svg
+-rw-r--r--   0        0        0      471 2024-03-09 14:42:49.662047 pyguiadapter-0.2.9/pyguiadapter/res/icons/application-two.svg
+-rw-r--r--   0        0        0      444 2024-03-09 14:42:49.695595 pyguiadapter-0.2.9/pyguiadapter/res/icons/area-map.svg
+-rw-r--r--   0        0        0     1704 2024-03-09 14:42:49.730658 pyguiadapter-0.2.9/pyguiadapter/res/icons/arithmetic-buttons.svg
+-rw-r--r--   0        0        0      886 2024-03-09 14:42:49.763713 pyguiadapter-0.2.9/pyguiadapter/res/icons/arithmetic-one.svg
+-rw-r--r--   0        0        0     1051 2024-03-09 14:42:49.803740 pyguiadapter-0.2.9/pyguiadapter/res/icons/arrow-keys.svg
+-rw-r--r--   0        0        0      510 2024-03-09 14:42:49.839218 pyguiadapter-0.2.9/pyguiadapter/res/icons/audio-file.svg
+-rw-r--r--   0        0        0      806 2024-03-09 14:42:49.874542 pyguiadapter-0.2.9/pyguiadapter/res/icons/audit.svg
+-rw-r--r--   0        0        0      503 2024-03-09 14:42:49.912111 pyguiadapter-0.2.9/pyguiadapter/res/icons/average.svg
+-rw-r--r--   0        0        0      871 2024-03-09 14:42:49.953498 pyguiadapter-0.2.9/pyguiadapter/res/icons/bitcoin.svg
+-rw-r--r--   0        0        0      753 2024-03-09 14:42:50.007926 pyguiadapter-0.2.9/pyguiadapter/res/icons/blackboard.svg
+-rw-r--r--   0        0        0      633 2024-03-09 14:42:50.054525 pyguiadapter-0.2.9/pyguiadapter/res/icons/blocks-and-arrows.svg
+-rw-r--r--   0        0        0      261 2024-03-09 14:42:50.096249 pyguiadapter-0.2.9/pyguiadapter/res/icons/bluetooth.svg
+-rw-r--r--   0        0        0      794 2024-03-09 14:42:50.134304 pyguiadapter-0.2.9/pyguiadapter/res/icons/bookmark-three.svg
+-rw-r--r--   0        0        0      981 2024-03-09 14:42:50.168174 pyguiadapter-0.2.9/pyguiadapter/res/icons/broadcast.svg
+-rw-r--r--   0        0        0      993 2024-03-09 14:42:50.199705 pyguiadapter-0.2.9/pyguiadapter/res/icons/browser.svg
+-rw-r--r--   0        0        0     1399 2024-03-09 14:42:50.232340 pyguiadapter-0.2.9/pyguiadapter/res/icons/bug.svg
+-rw-r--r--   0        0        0      978 2024-03-09 14:42:50.265457 pyguiadapter-0.2.9/pyguiadapter/res/icons/bytedance-mini-app.svg
+-rw-r--r--   0        0        0      334 2024-03-09 14:42:50.311121 pyguiadapter-0.2.9/pyguiadapter/res/icons/card-two.svg
+-rw-r--r--   0        0        0      643 2024-03-09 14:42:50.383849 pyguiadapter-0.2.9/pyguiadapter/res/icons/carousel-video.svg
+-rw-r--r--   0        0        0      849 2024-03-09 14:42:50.350168 pyguiadapter-0.2.9/pyguiadapter/res/icons/carousel.svg
+-rw-r--r--   0        0        0      685 2024-03-09 14:42:50.414066 pyguiadapter-0.2.9/pyguiadapter/res/icons/cast-screen.svg
+-rw-r--r--   0        0        0      472 2024-03-09 14:42:50.447609 pyguiadapter-0.2.9/pyguiadapter/res/icons/category-management.svg
+-rw-r--r--   0        0        0      443 2024-03-09 14:42:50.478933 pyguiadapter-0.2.9/pyguiadapter/res/icons/caution.svg
+-rw-r--r--   0        0        0     1016 2024-03-09 14:42:50.509609 pyguiadapter-0.2.9/pyguiadapter/res/icons/certificate.svg
+-rw-r--r--   0        0        0      634 2024-03-09 14:42:50.540729 pyguiadapter-0.2.9/pyguiadapter/res/icons/check-one.svg
+-rw-r--r--   0        0        0      697 2024-03-09 14:42:50.572289 pyguiadapter-0.2.9/pyguiadapter/res/icons/checklist.svg
+-rw-r--r--   0        0        0     1023 2024-03-09 14:42:50.603351 pyguiadapter-0.2.9/pyguiadapter/res/icons/chip.svg
+-rw-r--r--   0        0        0      519 2024-03-09 14:42:50.635463 pyguiadapter-0.2.9/pyguiadapter/res/icons/classroom.svg
+-rw-r--r--   0        0        0      478 2024-03-09 14:42:50.667994 pyguiadapter-0.2.9/pyguiadapter/res/icons/clipboard.svg
+-rw-r--r--   0        0        0      576 2024-03-09 14:42:50.700513 pyguiadapter-0.2.9/pyguiadapter/res/icons/close-one.svg
+-rw-r--r--   0        0        0     1211 2024-03-09 14:42:50.732035 pyguiadapter-0.2.9/pyguiadapter/res/icons/cloud-storage.svg
+-rw-r--r--   0        0        0      536 2024-03-09 14:42:50.795255 pyguiadapter-0.2.9/pyguiadapter/res/icons/code-brackets.svg
+-rw-r--r--   0        0        0      547 2024-03-09 14:42:50.826965 pyguiadapter-0.2.9/pyguiadapter/res/icons/code-download.svg
+-rw-r--r--   0        0        0      639 2024-03-09 14:42:50.860630 pyguiadapter-0.2.9/pyguiadapter/res/icons/code-laptop.svg
+-rw-r--r--   0        0        0      346 2024-03-09 14:42:50.893306 pyguiadapter-0.2.9/pyguiadapter/res/icons/code-one.svg
+-rw-r--r--   0        0        0      441 2024-03-09 14:42:50.764191 pyguiadapter-0.2.9/pyguiadapter/res/icons/code.svg
+-rw-r--r--   0        0        0      831 2024-03-09 14:42:50.925357 pyguiadapter-0.2.9/pyguiadapter/res/icons/collect-computer.svg
+-rw-r--r--   0        0        0      732 2024-03-09 14:42:50.958885 pyguiadapter-0.2.9/pyguiadapter/res/icons/collect-laptop.svg
+-rw-r--r--   0        0        0     1181 2024-03-09 14:42:50.991576 pyguiadapter-0.2.9/pyguiadapter/res/icons/collect-picture.svg
+-rw-r--r--   0        0        0     1118 2024-03-09 14:42:51.022102 pyguiadapter-0.2.9/pyguiadapter/res/icons/color-card.svg
+-rw-r--r--   0        0        0     1289 2024-03-09 14:42:51.052795 pyguiadapter-0.2.9/pyguiadapter/res/icons/command.svg
+-rw-r--r--   0        0        0      371 2024-03-09 14:42:51.119127 pyguiadapter-0.2.9/pyguiadapter/res/icons/comment-one.svg
+-rw-r--r--   0        0        0      581 2024-03-09 14:42:51.085912 pyguiadapter-0.2.9/pyguiadapter/res/icons/comment.svg
+-rw-r--r--   0        0        0      553 2024-03-09 14:42:51.153360 pyguiadapter-0.2.9/pyguiadapter/res/icons/comments.svg
+-rw-r--r--   0        0        0      628 2024-03-09 14:42:51.186924 pyguiadapter-0.2.9/pyguiadapter/res/icons/communication.svg
+-rw-r--r--   0        0        0      753 2024-03-09 14:42:51.219995 pyguiadapter-0.2.9/pyguiadapter/res/icons/compass.svg
+-rw-r--r--   0        0        0     1110 2024-03-09 14:42:51.250504 pyguiadapter-0.2.9/pyguiadapter/res/icons/compression.svg
+-rw-r--r--   0        0        0      556 2024-03-09 14:42:51.284109 pyguiadapter-0.2.9/pyguiadapter/res/icons/computer.svg
+-rw-r--r--   0        0        0      447 2024-03-09 14:42:51.317638 pyguiadapter-0.2.9/pyguiadapter/res/icons/cones.svg
+-rw-r--r--   0        0        0     1850 2024-03-09 14:42:51.350759 pyguiadapter-0.2.9/pyguiadapter/res/icons/connect.svg
+-rw-r--r--   0        0        0      620 2024-03-09 14:42:51.382155 pyguiadapter-0.2.9/pyguiadapter/res/icons/copy-one.svg
+-rw-r--r--   0        0        0      524 2024-03-09 14:42:51.414093 pyguiadapter-0.2.9/pyguiadapter/res/icons/copyright.svg
+-rw-r--r--   0        0        0     2644 2024-03-09 14:42:51.445689 pyguiadapter-0.2.9/pyguiadapter/res/icons/cpu.svg
+-rw-r--r--   0        0        0      516 2024-03-09 14:42:51.477786 pyguiadapter-0.2.9/pyguiadapter/res/icons/cross-ring-two.svg
+-rw-r--r--   0        0        0      895 2024-03-09 14:42:51.510328 pyguiadapter-0.2.9/pyguiadapter/res/icons/cube-four.svg
+-rw-r--r--   0        0        0      369 2024-03-09 14:42:51.543870 pyguiadapter-0.2.9/pyguiadapter/res/icons/curve-adjustment.svg
+-rw-r--r--   0        0        0     1177 2024-03-09 14:42:51.576599 pyguiadapter-0.2.9/pyguiadapter/res/icons/cuvette.svg
+-rw-r--r--   0        0        0     1199 2024-03-09 14:42:51.608710 pyguiadapter-0.2.9/pyguiadapter/res/icons/dashboard-one.svg
+-rw-r--r--   0        0        0     1332 2024-03-09 14:42:51.643261 pyguiadapter-0.2.9/pyguiadapter/res/icons/dashboard-two.svg
+-rw-r--r--   0        0        0     1221 2024-03-09 14:42:51.709446 pyguiadapter-0.2.9/pyguiadapter/res/icons/data-all.svg
+-rw-r--r--   0        0        0     1239 2024-03-09 14:42:51.742529 pyguiadapter-0.2.9/pyguiadapter/res/icons/data-display.svg
+-rw-r--r--   0        0        0     1255 2024-03-09 14:42:51.777672 pyguiadapter-0.2.9/pyguiadapter/res/icons/data-lock.svg
+-rw-r--r--   0        0        0      829 2024-03-09 14:42:51.813216 pyguiadapter-0.2.9/pyguiadapter/res/icons/data-screen.svg
+-rw-r--r--   0        0        0      833 2024-03-09 14:42:51.846297 pyguiadapter-0.2.9/pyguiadapter/res/icons/data-server.svg
+-rw-r--r--   0        0        0     1448 2024-03-09 14:42:51.879954 pyguiadapter-0.2.9/pyguiadapter/res/icons/data-switching.svg
+-rw-r--r--   0        0        0     1209 2024-03-09 14:42:51.911088 pyguiadapter-0.2.9/pyguiadapter/res/icons/data-user.svg
+-rw-r--r--   0        0        0      794 2024-03-09 14:42:51.675906 pyguiadapter-0.2.9/pyguiadapter/res/icons/data.svg
+-rw-r--r--   0        0        0     1588 2024-03-09 14:42:51.944604 pyguiadapter-0.2.9/pyguiadapter/res/icons/database-alert.svg
+-rw-r--r--   0        0        0     1606 2024-03-09 14:42:51.977363 pyguiadapter-0.2.9/pyguiadapter/res/icons/database-code.svg
+-rw-r--r--   0        0        0     1596 2024-03-09 14:42:52.007892 pyguiadapter-0.2.9/pyguiadapter/res/icons/database-config.svg
+-rw-r--r--   0        0        0     1513 2024-03-09 14:42:52.040009 pyguiadapter-0.2.9/pyguiadapter/res/icons/database-download.svg
+-rw-r--r--   0        0        0     1516 2024-03-09 14:42:52.074200 pyguiadapter-0.2.9/pyguiadapter/res/icons/database-enter.svg
+-rw-r--r--   0        0        0     1528 2024-03-09 14:42:52.106242 pyguiadapter-0.2.9/pyguiadapter/res/icons/database-fail.svg
+-rw-r--r--   0        0        0     1513 2024-03-09 14:42:52.137391 pyguiadapter-0.2.9/pyguiadapter/res/icons/database-first.svg
+-rw-r--r--   0        0        0     1492 2024-03-09 14:42:52.170998 pyguiadapter-0.2.9/pyguiadapter/res/icons/database-forbid.svg
+-rw-r--r--   0        0        0     1738 2024-03-09 14:42:52.201569 pyguiadapter-0.2.9/pyguiadapter/res/icons/database-lock.svg
+-rw-r--r--   0        0        0     1195 2024-03-09 14:42:52.268001 pyguiadapter-0.2.9/pyguiadapter/res/icons/database-network-point.svg
+-rw-r--r--   0        0        0     1770 2024-03-09 14:42:52.234122 pyguiadapter-0.2.9/pyguiadapter/res/icons/database-network.svg
+-rw-r--r--   0        0        0     1637 2024-03-09 14:42:52.300547 pyguiadapter-0.2.9/pyguiadapter/res/icons/database-point.svg
+-rw-r--r--   0        0        0     1390 2024-03-09 14:42:52.333068 pyguiadapter-0.2.9/pyguiadapter/res/icons/database-position.svg
+-rw-r--r--   0        0        0     1504 2024-03-09 14:42:52.364241 pyguiadapter-0.2.9/pyguiadapter/res/icons/database-power.svg
+-rw-r--r--   0        0        0     1528 2024-03-09 14:42:52.397951 pyguiadapter-0.2.9/pyguiadapter/res/icons/database-proportion.svg
+-rw-r--r--   0        0        0     1908 2024-03-09 14:42:52.428304 pyguiadapter-0.2.9/pyguiadapter/res/icons/database-search.svg
+-rw-r--r--   0        0        0     1542 2024-03-09 14:42:52.460505 pyguiadapter-0.2.9/pyguiadapter/res/icons/database-setting.svg
+-rw-r--r--   0        0        0     1504 2024-03-09 14:42:52.494171 pyguiadapter-0.2.9/pyguiadapter/res/icons/database-success.svg
+-rw-r--r--   0        0        0     1638 2024-03-09 14:42:52.525731 pyguiadapter-0.2.9/pyguiadapter/res/icons/database-sync.svg
+-rw-r--r--   0        0        0     1492 2024-03-09 14:42:52.559018 pyguiadapter-0.2.9/pyguiadapter/res/icons/database-time.svg
+-rw-r--r--   0        0        0      762 2024-03-09 14:42:52.591111 pyguiadapter-0.2.9/pyguiadapter/res/icons/date-comes-back.svg
+-rw-r--r--   0        0        0      470 2024-03-09 14:42:52.624367 pyguiadapter-0.2.9/pyguiadapter/res/icons/diamond-one.svg
+-rw-r--r--   0        0        0      470 2024-03-09 14:42:52.657545 pyguiadapter-0.2.9/pyguiadapter/res/icons/diamond-three.svg
+-rw-r--r--   0        0        0      466 2024-03-09 14:42:52.689586 pyguiadapter-0.2.9/pyguiadapter/res/icons/diamond-two.svg
+-rw-r--r--   0        0        0      855 2024-03-09 14:42:52.754775 pyguiadapter-0.2.9/pyguiadapter/res/icons/disk-one.svg
+-rw-r--r--   0        0        0      533 2024-03-09 14:42:52.788667 pyguiadapter-0.2.9/pyguiadapter/res/icons/disk-two.svg
+-rw-r--r--   0        0        0      599 2024-03-09 14:42:52.722118 pyguiadapter-0.2.9/pyguiadapter/res/icons/disk.svg
+-rw-r--r--   0        0        0      646 2024-03-09 14:42:52.821412 pyguiadapter-0.2.9/pyguiadapter/res/icons/document-folder.svg
+-rw-r--r--   0        0        0      957 2024-03-09 14:42:52.852474 pyguiadapter-0.2.9/pyguiadapter/res/icons/download-one.svg
+-rw-r--r--   0        0        0      649 2024-03-09 14:42:52.884528 pyguiadapter-0.2.9/pyguiadapter/res/icons/download-three.svg
+-rw-r--r--   0        0        0      730 2024-03-09 14:42:52.917857 pyguiadapter-0.2.9/pyguiadapter/res/icons/download-two.svg
+-rw-r--r--   0        0        0      827 2024-03-09 14:42:52.952370 pyguiadapter-0.2.9/pyguiadapter/res/icons/download-web.svg
+-rw-r--r--   0        0        0      500 2024-03-09 14:42:52.983983 pyguiadapter-0.2.9/pyguiadapter/res/icons/electrocardiogram.svg
+-rw-r--r--   0        0        0      568 2024-03-09 14:42:53.017497 pyguiadapter-0.2.9/pyguiadapter/res/icons/email-down.svg
+-rw-r--r--   0        0        0      567 2024-03-09 14:42:53.052087 pyguiadapter-0.2.9/pyguiadapter/res/icons/email-push.svg
+-rw-r--r--   0        0        0      634 2024-03-09 14:42:53.117840 pyguiadapter-0.2.9/pyguiadapter/res/icons/experiment-one.svg
+-rw-r--r--   0        0        0      731 2024-03-09 14:42:53.084199 pyguiadapter-0.2.9/pyguiadapter/res/icons/experiment.svg
+-rw-r--r--   0        0        0      680 2024-03-09 14:42:53.152428 pyguiadapter-0.2.9/pyguiadapter/res/icons/figma-component.svg
+-rw-r--r--   0        0        0      652 2024-03-09 14:42:53.185744 pyguiadapter-0.2.9/pyguiadapter/res/icons/file-addition.svg
+-rw-r--r--   0        0        0      664 2024-03-09 14:42:53.217973 pyguiadapter-0.2.9/pyguiadapter/res/icons/file-code.svg
+-rw-r--r--   0        0        0      856 2024-03-09 14:42:53.249496 pyguiadapter-0.2.9/pyguiadapter/res/icons/file-conversion.svg
+-rw-r--r--   0        0        0      772 2024-03-09 14:42:53.281733 pyguiadapter-0.2.9/pyguiadapter/res/icons/file-display.svg
+-rw-r--r--   0        0        0     1316 2024-03-09 14:42:53.313837 pyguiadapter-0.2.9/pyguiadapter/res/icons/file-pdf-one.svg
+-rw-r--r--   0        0        0     1381 2024-03-09 14:42:53.347168 pyguiadapter-0.2.9/pyguiadapter/res/icons/file-ppt.svg
+-rw-r--r--   0        0        0      658 2024-03-09 14:42:53.382365 pyguiadapter-0.2.9/pyguiadapter/res/icons/file-protection.svg
+-rw-r--r--   0        0        0      652 2024-03-09 14:42:53.417579 pyguiadapter-0.2.9/pyguiadapter/res/icons/file-text.svg
+-rw-r--r--   0        0        0      468 2024-03-09 14:42:53.455122 pyguiadapter-0.2.9/pyguiadapter/res/icons/file-word.svg
+-rw-r--r--   0        0        0      931 2024-03-09 14:42:53.486147 pyguiadapter-0.2.9/pyguiadapter/res/icons/film.svg
+-rw-r--r--   0        0        0      734 2024-03-09 14:42:53.517258 pyguiadapter-0.2.9/pyguiadapter/res/icons/flask.svg
+-rw-r--r--   0        0        0      851 2024-03-09 14:42:53.549857 pyguiadapter-0.2.9/pyguiadapter/res/icons/game-handle.svg
+-rw-r--r--   0        0        0      989 2024-03-09 14:42:53.581226 pyguiadapter-0.2.9/pyguiadapter/res/icons/help.svg
+-rw-r--r--   0        0        0      545 2024-03-09 14:42:53.612330 pyguiadapter-0.2.9/pyguiadapter/res/icons/hexagon-one.svg
+-rw-r--r--   0        0        0      794 2024-03-09 14:42:53.643884 pyguiadapter-0.2.9/pyguiadapter/res/icons/id-card-h.svg
+-rw-r--r--   0        0        0      935 2024-03-09 14:42:53.676625 pyguiadapter-0.2.9/pyguiadapter/res/icons/info.svg
+-rw-r--r--   0        0        0      696 2024-03-09 14:42:53.708204 pyguiadapter-0.2.9/pyguiadapter/res/icons/install.svg
+-rw-r--r--   0        0        0    11551 2024-03-17 02:22:55.741177 pyguiadapter-0.2.9/pyguiadapter/res/icons/LICENSE.txt
+-rw-r--r--   0        0        0      683 2024-03-09 14:42:53.741316 pyguiadapter-0.2.9/pyguiadapter/res/icons/many-to-many.svg
+-rw-r--r--   0        0        0      602 2024-03-09 14:42:53.805746 pyguiadapter-0.2.9/pyguiadapter/res/icons/message-emoji.svg
+-rw-r--r--   0        0        0      522 2024-03-09 14:42:53.840353 pyguiadapter-0.2.9/pyguiadapter/res/icons/message-one.svg
+-rw-r--r--   0        0        0      763 2024-03-09 14:42:53.871762 pyguiadapter-0.2.9/pyguiadapter/res/icons/message-privacy.svg
+-rw-r--r--   0        0        0      648 2024-03-09 14:42:53.905271 pyguiadapter-0.2.9/pyguiadapter/res/icons/message-search.svg
+-rw-r--r--   0        0        0      679 2024-03-09 14:42:53.935786 pyguiadapter-0.2.9/pyguiadapter/res/icons/message-security.svg
+-rw-r--r--   0        0        0      485 2024-03-09 14:42:53.970910 pyguiadapter-0.2.9/pyguiadapter/res/icons/message-sent.svg
+-rw-r--r--   0        0        0      577 2024-03-09 14:42:54.004586 pyguiadapter-0.2.9/pyguiadapter/res/icons/message-success.svg
+-rw-r--r--   0        0        0      550 2024-03-09 14:42:54.037266 pyguiadapter-0.2.9/pyguiadapter/res/icons/message-unread.svg
+-rw-r--r--   0        0        0      738 2024-03-09 14:42:53.773734 pyguiadapter-0.2.9/pyguiadapter/res/icons/message.svg
+-rw-r--r--   0        0        0      537 2024-03-09 14:42:54.071502 pyguiadapter-0.2.9/pyguiadapter/res/icons/mini-sd-card.svg
+-rw-r--r--   0        0        0      521 2024-03-09 14:42:54.103643 pyguiadapter-0.2.9/pyguiadapter/res/icons/monitor.svg
+-rw-r--r--   0        0        0     1053 2024-03-09 14:42:54.135574 pyguiadapter-0.2.9/pyguiadapter/res/icons/more-app.svg
+-rw-r--r--   0        0        0      971 2024-03-09 14:42:54.204781 pyguiadapter-0.2.9/pyguiadapter/res/icons/movie-board.svg
+-rw-r--r--   0        0        0     1213 2024-03-09 14:42:54.169203 pyguiadapter-0.2.9/pyguiadapter/res/icons/movie.svg
+-rw-r--r--   0        0        0      995 2024-03-09 14:42:54.236957 pyguiadapter-0.2.9/pyguiadapter/res/icons/multi-function-knife.svg
+-rw-r--r--   0        0        0      835 2024-03-09 14:42:54.270059 pyguiadapter-0.2.9/pyguiadapter/res/icons/notebook-one.svg
+-rw-r--r--   0        0        0      626 2024-03-09 14:42:54.305013 pyguiadapter-0.2.9/pyguiadapter/res/icons/octagon.svg
+-rw-r--r--   0        0        0      575 2024-03-09 14:42:54.338102 pyguiadapter-0.2.9/pyguiadapter/res/icons/online-meeting.svg
+-rw-r--r--   0        0        0      227 2024-03-09 14:42:54.370839 pyguiadapter-0.2.9/pyguiadapter/res/icons/oval-one.svg
+-rw-r--r--   0        0        0      537 2024-03-09 14:42:54.440082 pyguiadapter-0.2.9/pyguiadapter/res/icons/page-template.svg
+-rw-r--r--   0        0        0      440 2024-03-09 14:42:54.403964 pyguiadapter-0.2.9/pyguiadapter/res/icons/page.svg
+-rw-r--r--   0        0        0      412 2024-03-09 14:42:54.473151 pyguiadapter-0.2.9/pyguiadapter/res/icons/parallelogram.svg
+-rw-r--r--   0        0        0      633 2024-03-09 14:42:54.508004 pyguiadapter-0.2.9/pyguiadapter/res/icons/pay-code.svg
+-rw-r--r--   0        0        0      509 2024-03-09 14:42:54.540081 pyguiadapter-0.2.9/pyguiadapter/res/icons/pentagon-one.svg
+-rw-r--r--   0        0        0      980 2024-03-09 14:42:54.573293 pyguiadapter-0.2.9/pyguiadapter/res/icons/people-plus-one.svg
+-rw-r--r--   0        0        0     1040 2024-03-09 14:42:54.640249 pyguiadapter-0.2.9/pyguiadapter/res/icons/phone-incoming-one.svg
+-rw-r--r--   0        0        0     1029 2024-03-09 14:42:54.606929 pyguiadapter-0.2.9/pyguiadapter/res/icons/phone-incoming.svg
+-rw-r--r--   0        0        0     1083 2024-03-09 14:42:54.672454 pyguiadapter-0.2.9/pyguiadapter/res/icons/phone-missed.svg
+-rw-r--r--   0        0        0     1015 2024-03-09 14:42:54.735192 pyguiadapter-0.2.9/pyguiadapter/res/icons/phone-outgoing-one.svg
+-rw-r--r--   0        0        0     1008 2024-03-09 14:42:54.704958 pyguiadapter-0.2.9/pyguiadapter/res/icons/phone-outgoing.svg
+-rw-r--r--   0        0        0      811 2024-03-09 14:42:54.769268 pyguiadapter-0.2.9/pyguiadapter/res/icons/phone-telephone.svg
+-rw-r--r--   0        0        0      935 2024-03-09 14:42:54.800614 pyguiadapter-0.2.9/pyguiadapter/res/icons/phone-video-call.svg
+-rw-r--r--   0        0        0      974 2024-03-09 14:42:54.832344 pyguiadapter-0.2.9/pyguiadapter/res/icons/platte.svg
+-rw-r--r--   0        0        0      473 2024-03-09 14:42:54.868011 pyguiadapter-0.2.9/pyguiadapter/res/icons/play.svg
+-rw-r--r--   0        0        0      434 2024-03-09 14:42:54.900949 pyguiadapter-0.2.9/pyguiadapter/res/icons/powerpoint.svg
+-rw-r--r--   0        0        0      612 2024-03-09 14:42:54.933463 pyguiadapter-0.2.9/pyguiadapter/res/icons/ppt.svg
+-rw-r--r--   0        0        0      427 2024-03-09 14:42:54.965026 pyguiadapter-0.2.9/pyguiadapter/res/icons/puzzle.svg
+-rw-r--r--   0        0        0      364 2024-03-09 14:42:54.997189 pyguiadapter-0.2.9/pyguiadapter/res/icons/quadrilateral.svg
+-rw-r--r--   0        0        0      783 2024-03-09 14:42:55.060859 pyguiadapter-0.2.9/pyguiadapter/res/icons/record-disc.svg
+-rw-r--r--   0        0        0      880 2024-03-09 14:42:55.028755 pyguiadapter-0.2.9/pyguiadapter/res/icons/record.svg
+-rw-r--r--   0        0        0      319 2024-03-09 14:42:55.123563 pyguiadapter-0.2.9/pyguiadapter/res/icons/rectangle-one.svg
+-rw-r--r--   0        0        0      328 2024-03-09 14:42:55.156079 pyguiadapter-0.2.9/pyguiadapter/res/icons/rectangle-small.svg
+-rw-r--r--   0        0        0      319 2024-03-09 14:42:55.092477 pyguiadapter-0.2.9/pyguiadapter/res/icons/rectangle.svg
+-rw-r--r--   0        0        0      591 2024-03-09 16:01:09.963050 pyguiadapter-0.2.9/pyguiadapter/res/icons/rename.py
+-rw-r--r--   0        0        0      425 2024-03-09 14:42:55.187919 pyguiadapter-0.2.9/pyguiadapter/res/icons/right-angle.svg
+-rw-r--r--   0        0        0      217 2024-03-09 14:42:55.218332 pyguiadapter-0.2.9/pyguiadapter/res/icons/round.svg
+-rw-r--r--   0        0        0      901 2024-03-09 14:42:55.250585 pyguiadapter-0.2.9/pyguiadapter/res/icons/rule-two.svg
+-rw-r--r--   0        0        0      794 2024-03-09 14:42:55.314442 pyguiadapter-0.2.9/pyguiadapter/res/icons/ruler-one.svg
+-rw-r--r--   0        0        0      926 2024-03-09 14:42:55.282289 pyguiadapter-0.2.9/pyguiadapter/res/icons/ruler.svg
+-rw-r--r--   0        0        0      583 2024-03-09 14:42:55.344890 pyguiadapter-0.2.9/pyguiadapter/res/icons/sd-card.svg
+-rw-r--r--   0        0        0     1259 2024-03-09 14:42:55.377061 pyguiadapter-0.2.9/pyguiadapter/res/icons/setting-computer.svg
+-rw-r--r--   0        0        0     1148 2024-03-09 14:42:55.409597 pyguiadapter-0.2.9/pyguiadapter/res/icons/setting-laptop.svg
+-rw-r--r--   0        0        0     1443 2024-03-09 14:42:55.444676 pyguiadapter-0.2.9/pyguiadapter/res/icons/setting-two.svg
+-rw-r--r--   0        0        0      980 2024-03-09 14:42:55.477262 pyguiadapter-0.2.9/pyguiadapter/res/icons/share-one.svg
+-rw-r--r--   0        0        0      328 2024-03-09 14:42:55.541521 pyguiadapter-0.2.9/pyguiadapter/res/icons/square-small.svg
+-rw-r--r--   0        0        0      317 2024-03-09 14:42:55.509301 pyguiadapter-0.2.9/pyguiadapter/res/icons/square.svg
+-rw-r--r--   0        0        0      954 2024-03-09 14:42:55.574211 pyguiadapter-0.2.9/pyguiadapter/res/icons/system.svg
+-rw-r--r--   0        0        0      895 2024-03-09 14:42:55.606324 pyguiadapter-0.2.9/pyguiadapter/res/icons/table-file.svg
+-rw-r--r--   0        0        0     1216 2024-03-09 14:42:55.637907 pyguiadapter-0.2.9/pyguiadapter/res/icons/tape.svg
+-rw-r--r--   0        0        0      465 2024-03-09 14:42:55.669026 pyguiadapter-0.2.9/pyguiadapter/res/icons/terminal.svg
+-rw-r--r--   0        0        0      751 2024-03-09 14:42:55.704103 pyguiadapter-0.2.9/pyguiadapter/res/icons/test-tube.svg
+-rw-r--r--   0        0        0      724 2024-03-09 14:42:55.736266 pyguiadapter-0.2.9/pyguiadapter/res/icons/thermometer.svg
+-rw-r--r--   0        0        0      425 2024-03-09 14:42:55.768900 pyguiadapter-0.2.9/pyguiadapter/res/icons/tips-one.svg
+-rw-r--r--   0        0        0      510 2024-03-09 14:42:55.800445 pyguiadapter-0.2.9/pyguiadapter/res/icons/tool.svg
+-rw-r--r--   0        0        0      587 2024-03-09 14:42:55.867211 pyguiadapter-0.2.9/pyguiadapter/res/icons/topic-discussion.svg
+-rw-r--r--   0        0        0     1027 2024-03-09 14:42:55.835066 pyguiadapter-0.2.9/pyguiadapter/res/icons/topic.svg
+-rw-r--r--   0        0        0      413 2024-03-09 14:42:55.900240 pyguiadapter-0.2.9/pyguiadapter/res/icons/trapezoid.svg
+-rw-r--r--   0        0        0      831 2024-03-09 14:42:55.935077 pyguiadapter-0.2.9/pyguiadapter/res/icons/tree-list.svg
+-rw-r--r--   0        0        0     1970 2024-03-09 14:42:55.998698 pyguiadapter-0.2.9/pyguiadapter/res/icons/triangle-ruler.svg
+-rw-r--r--   0        0        0      468 2024-03-09 14:42:55.966416 pyguiadapter-0.2.9/pyguiadapter/res/icons/triangle.svg
+-rw-r--r--   0        0        0      717 2024-03-09 14:42:56.029033 pyguiadapter-0.2.9/pyguiadapter/res/icons/vial.svg
+-rw-r--r--   0        0        0     1823 2024-03-09 14:42:56.061697 pyguiadapter-0.2.9/pyguiadapter/res/icons/video.svg
+-rw-r--r--   0        0        0      706 2024-03-09 14:42:56.093308 pyguiadapter-0.2.9/pyguiadapter/res/icons/view-grid-card.svg
+-rw-r--r--   0        0        0      775 2024-03-09 14:42:56.123098 pyguiadapter-0.2.9/pyguiadapter/res/icons/view-grid-detail.svg
+-rw-r--r--   0        0        0      887 2024-03-09 14:42:56.156703 pyguiadapter-0.2.9/pyguiadapter/res/icons/view-grid-list.svg
+-rw-r--r--   0        0        0      642 2024-03-09 14:42:56.218845 pyguiadapter-0.2.9/pyguiadapter/res/icons/voice-input.svg
+-rw-r--r--   0        0        0      903 2024-03-09 14:42:56.251446 pyguiadapter-0.2.9/pyguiadapter/res/icons/voice-message.svg
+-rw-r--r--   0        0        0      685 2024-03-09 14:42:56.284535 pyguiadapter-0.2.9/pyguiadapter/res/icons/voice-one.svg
+-rw-r--r--   0        0        0      508 2024-03-09 14:42:56.187304 pyguiadapter-0.2.9/pyguiadapter/res/icons/voice.svg
+-rw-r--r--   0        0        0     1173 2024-03-09 14:42:56.317102 pyguiadapter-0.2.9/pyguiadapter/res/icons/weixin-mini-app.svg
+-rw-r--r--   0        0        0      809 2024-03-09 14:42:56.349946 pyguiadapter-0.2.9/pyguiadapter/res/icons/wifi.svg
+-rw-r--r--   0        0        0      976 2024-03-09 14:42:56.381588 pyguiadapter-0.2.9/pyguiadapter/res/icons/zip.svg
+-rw-r--r--   0        0        0        0 2024-03-15 05:08:37.625966 pyguiadapter-0.2.9/pyguiadapter/ui/__init__.py
+-rw-r--r--   0        0        0     1462 2024-03-22 14:55:24.908558 pyguiadapter-0.2.9/pyguiadapter/ui/config.py
+-rw-r--r--   0        0        0        0 2024-03-15 11:37:47.907987 pyguiadapter-0.2.9/pyguiadapter/ui/generated/__init__.py
+-rw-r--r--   0        0        0     6996 2024-03-22 12:51:51.481008 pyguiadapter-0.2.9/pyguiadapter/ui/generated/ui_execution_window.py
+-rw-r--r--   0        0        0     2844 2024-03-22 12:51:51.656489 pyguiadapter-0.2.9/pyguiadapter/ui/generated/ui_initialization_window.py
+-rw-r--r--   0        0        0     4413 2024-03-22 12:51:51.830703 pyguiadapter-0.2.9/pyguiadapter/ui/generated/ui_selection_window.py
+-rw-r--r--   0        0        0     1460 2024-03-19 13:11:31.754220 pyguiadapter-0.2.9/pyguiadapter/ui/styles.py
+-rw-r--r--   0        0        0     1109 2024-03-19 13:11:19.291844 pyguiadapter-0.2.9/pyguiadapter/ui/utils.py
+-rw-r--r--   0        0        0        0 2024-03-15 12:09:31.827626 pyguiadapter-0.2.9/pyguiadapter/ui/window/__init__.py
+-rw-r--r--   0        0        0    17385 2024-03-25 16:57:48.958090 pyguiadapter-0.2.9/pyguiadapter/ui/window/execution.py
+-rw-r--r--   0        0        0     6185 2024-03-22 14:58:04.952081 pyguiadapter-0.2.9/pyguiadapter/ui/window/initialization.py
+-rw-r--r--   0        0        0     8273 2024-03-22 14:56:06.155478 pyguiadapter-0.2.9/pyguiadapter/ui/window/selection.py
+-rw-r--r--   0        0        0      688 2024-03-26 15:38:08.448955 pyguiadapter-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     8610 2024-03-24 02:40:52.393460 pyguiadapter-0.2.9/README.md
+-rw-r--r--   0        0        0     9140 1970-01-01 00:00:00.000000 pyguiadapter-0.2.9/PKG-INFO
```

### Comparing `pyguiadapter-0.2.8/License` & `pyguiadapter-0.2.9/License`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/adapter/adapter.py` & `pyguiadapter-0.2.9/pyguiadapter/adapter/adapter.py`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/adapter/bundle.py` & `pyguiadapter-0.2.9/pyguiadapter/adapter/bundle.py`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/adapter/executor.py` & `pyguiadapter-0.2.9/pyguiadapter/adapter/executor.py`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/commons.py` & `pyguiadapter-0.2.9/pyguiadapter/commons.py`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/interact/ulogging.py` & `pyguiadapter-0.2.9/pyguiadapter/interact/ulogging.py`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/interact/upopup.py` & `pyguiadapter-0.2.9/pyguiadapter/interact/upopup.py`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/interact/uprint.py` & `pyguiadapter-0.2.9/pyguiadapter/interact/uprint.py`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/abnormal.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/abnormal.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/acoustic.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/acoustic.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/add-computer.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/add-computer.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/add-picture.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/add-picture.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/add-print.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/add-print.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/add-user.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/add-user.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/add-web.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/add-web.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/api-app.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/api-app.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/application-effect.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/application-effect.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/application-one.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/application-one.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/arithmetic-buttons.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/arithmetic-buttons.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/arithmetic-one.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/arithmetic-one.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/arrow-keys.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/arrow-keys.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/audit.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/audit.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/bitcoin.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/bitcoin.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/blackboard.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/blackboard.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/blocks-and-arrows.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/blocks-and-arrows.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/bookmark-three.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/bookmark-three.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/broadcast.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/broadcast.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/browser.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/browser.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/bug.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/bug.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/bytedance-mini-app.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/bytedance-mini-app.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/carousel-video.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/carousel-video.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/carousel.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/carousel.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/cast-screen.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/cast-screen.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/certificate.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/certificate.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/check-one.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/check-one.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/checklist.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/checklist.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/chip.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/chip.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/classroom.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/classroom.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/close-one.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/close-one.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/cloud-storage.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/cloud-storage.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/code-brackets.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/code-brackets.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/code-download.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/code-download.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/code-laptop.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/code-laptop.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/collect-computer.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/collect-computer.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/collect-laptop.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/collect-laptop.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/collect-picture.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/collect-picture.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/color-card.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/color-card.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/command.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/command.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/comment.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/comment.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/comments.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/comments.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/communication.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/communication.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/compass.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/compass.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/compression.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/compression.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/computer.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/computer.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/connect.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/connect.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/copy-one.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/copy-one.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/copyright.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/copyright.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/cpu.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/cpu.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/cross-ring-two.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/cross-ring-two.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/cube-four.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/cube-four.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/cuvette.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/cuvette.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/dashboard-one.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/dashboard-one.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/dashboard-two.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/dashboard-two.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/data-all.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/data-all.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/data-display.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/data-display.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/data-lock.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/data-lock.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/data-screen.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/data-screen.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/data-server.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/data-server.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/data-switching.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/data-switching.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/data-user.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/data-user.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/data.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/data.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/database-alert.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/database-alert.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/database-code.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/database-code.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/database-config.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/database-config.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/database-download.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/database-download.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/database-enter.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/database-enter.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/database-fail.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/database-fail.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/database-first.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/database-first.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/database-forbid.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/database-forbid.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/database-lock.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/database-lock.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/database-network-point.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/database-network-point.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/database-network.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/database-network.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/database-point.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/database-point.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/database-position.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/database-position.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/database-power.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/database-power.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/database-proportion.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/database-proportion.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/database-search.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/database-search.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/database-setting.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/database-setting.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/database-success.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/database-success.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/database-sync.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/database-sync.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/database-time.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/database-time.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/date-comes-back.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/date-comes-back.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/disk-one.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/disk-one.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/disk-two.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/disk-two.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/disk.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/disk.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/document-folder.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/document-folder.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/download-one.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/download-one.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/download-three.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/download-three.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/download-two.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/download-two.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/download-web.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/download-web.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/email-down.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/email-down.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/email-push.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/email-push.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/experiment-one.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/experiment-one.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/experiment.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/experiment.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/figma-component.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/figma-component.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/file-addition.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/file-addition.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/file-code.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/file-code.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/file-conversion.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/file-conversion.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/file-display.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/file-display.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/file-pdf-one.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/file-pdf-one.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/file-ppt.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/file-ppt.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/file-protection.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/file-protection.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/file-text.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/file-text.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/film.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/film.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/flask.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/flask.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/game-handle.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/game-handle.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/help.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/help.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/hexagon-one.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/hexagon-one.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/id-card-h.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/id-card-h.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/info.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/info.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/install.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/install.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/LICENSE.txt` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/many-to-many.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/many-to-many.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/message-emoji.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/message-emoji.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/message-one.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/message-one.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/message-privacy.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/message-privacy.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/message-search.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/message-search.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/message-security.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/message-security.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/message-success.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/message-success.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/message-unread.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/message-unread.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/message.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/message.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/mini-sd-card.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/mini-sd-card.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/monitor.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/monitor.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/more-app.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/more-app.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/movie-board.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/movie-board.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/movie.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/movie.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/multi-function-knife.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/multi-function-knife.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/notebook-one.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/notebook-one.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/octagon.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/octagon.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/online-meeting.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/online-meeting.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/page-template.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/page-template.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/pay-code.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/pay-code.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/people-plus-one.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/people-plus-one.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/phone-incoming-one.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/phone-incoming-one.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/phone-incoming.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/phone-incoming.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/phone-missed.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/phone-missed.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/phone-outgoing-one.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/phone-outgoing-one.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/phone-outgoing.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/phone-outgoing.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/phone-telephone.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/phone-telephone.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/phone-video-call.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/phone-video-call.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/platte.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/platte.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/ppt.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/ppt.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/record-disc.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/record-disc.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/record.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/record.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/rename.py` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/rename.py`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/rule-two.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/rule-two.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/ruler-one.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/ruler-one.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/ruler.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/ruler.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/sd-card.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/sd-card.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/setting-computer.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/setting-computer.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/setting-laptop.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/setting-laptop.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/setting-two.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/setting-two.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/share-one.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/share-one.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/system.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/system.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/table-file.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/table-file.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/tape.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/tape.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/test-tube.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/test-tube.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/thermometer.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/thermometer.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/topic-discussion.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/topic-discussion.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/topic.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/topic.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/tree-list.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/tree-list.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/triangle-ruler.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/triangle-ruler.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/vial.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/vial.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/video.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/video.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/view-grid-card.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/view-grid-card.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/view-grid-detail.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/view-grid-detail.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/view-grid-list.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/view-grid-list.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/voice-input.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/voice-input.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/voice-message.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/voice-message.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/voice-one.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/voice-one.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/weixin-mini-app.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/weixin-mini-app.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/wifi.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/wifi.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/res/icons/zip.svg` & `pyguiadapter-0.2.9/pyguiadapter/res/icons/zip.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/ui/config.py` & `pyguiadapter-0.2.9/pyguiadapter/ui/config.py`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/ui/generated/ui_execution_window.py` & `pyguiadapter-0.2.9/pyguiadapter/ui/generated/ui_execution_window.py`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/ui/generated/ui_initialization_window.py` & `pyguiadapter-0.2.9/pyguiadapter/ui/generated/ui_initialization_window.py`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/ui/generated/ui_selection_window.py` & `pyguiadapter-0.2.9/pyguiadapter/ui/generated/ui_selection_window.py`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/ui/styles.py` & `pyguiadapter-0.2.9/pyguiadapter/ui/styles.py`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/ui/utils.py` & `pyguiadapter-0.2.9/pyguiadapter/ui/utils.py`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/ui/window/execution.py` & `pyguiadapter-0.2.9/pyguiadapter/ui/window/execution.py`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/ui/window/initialization.py` & `pyguiadapter-0.2.9/pyguiadapter/ui/window/initialization.py`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyguiadapter/ui/window/selection.py` & `pyguiadapter-0.2.9/pyguiadapter/ui/window/selection.py`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/pyproject.toml` & `pyguiadapter-0.2.9/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "pyguiadapter"
-version = "0.2.8"
+version = "0.2.9"
 description = "turn (almost) any python functions into a gui in a few lines of code"
 authors = ["zimolab <zimolab@aliyun.com>"]
 readme = "README.md"
 homepage = "https://github.com/zimolab/PyGUIAdapter"
 repository = "https://github.com/zimolab/PyGUIAdapter"
 documentation = "https://github.com/zimolab/PyGUIAdapter"
 
 
 [tool.poetry.scripts]
 autogen = "autouic:main"
 
 [tool.poetry.dependencies]
 python = ">=3.8, <4.0"
-function2widgets = ">=0.5.2"
+function2widgets = ">=0.5.4"
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.2.0"
 qt-material = "^2.14"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `pyguiadapter-0.2.8/README.md` & `pyguiadapter-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.8/PKG-INFO` & `pyguiadapter-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: pyguiadapter
-Version: 0.2.8
+Version: 0.2.9
 Summary: turn (almost) any python functions into a gui in a few lines of code
 Home-page: https://github.com/zimolab/PyGUIAdapter
 Author: zimolab
 Author-email: zimolab@aliyun.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: function2widgets (>=0.5.2)
+Requires-Dist: function2widgets (>=0.5.4)
 Project-URL: Documentation, https://github.com/zimolab/PyGUIAdapter
 Project-URL: Repository, https://github.com/zimolab/PyGUIAdapter
 Description-Content-Type: text/markdown
 
 # PyGUIAdapter
 
 ---
```

