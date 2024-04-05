# Comparing `tmp/unblob-24.2.20.tar.gz` & `tmp/unblob-24.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unblob-24.2.20.tar", max compression
+gzip compressed data, was "unblob-24.4.5.tar", max compression
```

## Comparing `unblob-24.2.20.tar` & `unblob-24.4.5.tar`

### file list

```diff
@@ -1,81 +1,81 @@
--rw-r--r--   0        0        0     2255 2024-02-20 11:06:44.512011 unblob-24.2.20/LICENSE
--rw-r--r--   0        0        0     5228 2024-02-20 11:06:44.516011 unblob-24.2.20/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/__init__.py
--rwxr-xr-x   0        0        0    14919 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/cli.py
--rw-r--r--   0        0        0      344 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/cli_options.py
--rw-r--r--   0        0        0     1219 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/dependencies.py
--rw-r--r--   0        0        0     4162 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/extractor.py
--rw-r--r--   0        0        0      196 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/extractors/README.md
--rw-r--r--   0        0        0       40 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/extractors/__init__.py
--rw-r--r--   0        0        0     3798 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/extractors/command.py
--rw-r--r--   0        0        0    21647 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/file_utils.py
--rw-r--r--   0        0        0     5731 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/finder.py
--rw-r--r--   0        0        0     2540 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/handlers/__init__.py
--rw-r--r--   0        0        0        0 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/handlers/archive/__init__.py
--rw-r--r--   0        0        0     5864 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/handlers/archive/_safe_tarfile.py
--rw-r--r--   0        0        0     1694 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/handlers/archive/ar.py
--rw-r--r--   0        0        0     2775 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/handlers/archive/arc.py
--rw-r--r--   0        0        0     5683 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/handlers/archive/arj.py
--rw-r--r--   0        0        0     2505 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/handlers/archive/cab.py
--rw-r--r--   0        0        0    12350 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/handlers/archive/cpio.py
--rw-r--r--   0        0        0     2250 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/handlers/archive/dlink/encrpted_img.py
--rw-r--r--   0        0        0     3589 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/handlers/archive/dlink/shrs.py
--rw-r--r--   0        0        0     3700 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/handlers/archive/dmg.py
--rw-r--r--   0        0        0     3018 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/handlers/archive/engeniustech/engenius.py
--rw-r--r--   0        0        0     3282 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/handlers/archive/hp/bdl.py
--rw-r--r--   0        0        0     3330 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/handlers/archive/hp/ipkg.py
--rw-r--r--   0        0        0     2946 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/handlers/archive/instar/bneg.py
--rw-r--r--   0        0        0     1416 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/handlers/archive/instar/instar_hd.py
--rw-r--r--   0        0        0     2553 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/handlers/archive/netgear/chk.py
--rw-r--r--   0        0        0     4005 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/handlers/archive/netgear/trx.py
--rw-r--r--   0        0        0     5543 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/handlers/archive/qnap/qnap_nas.py
--rw-r--r--   0        0        0     1158 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/handlers/archive/rar.py
--rw-r--r--   0        0        0     4075 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/handlers/archive/sevenzip.py
--rw-r--r--   0        0        0     2332 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/handlers/archive/stuffit.py
--rw-r--r--   0        0        0     8195 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/handlers/archive/tar.py
--rw-r--r--   0        0        0     5892 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/handlers/archive/xiaomi/hdr.py
--rw-r--r--   0        0        0     6414 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/handlers/archive/zip.py
--rw-r--r--   0        0        0        0 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/handlers/compression/__init__.py
--rw-r--r--   0        0        0     1299 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/handlers/compression/_gzip_reader.py
--rw-r--r--   0        0        0     4709 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/handlers/compression/bzip2.py
--rw-r--r--   0        0        0     8898 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/handlers/compression/compress.py
--rw-r--r--   0        0        0     5680 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/handlers/compression/gzip.py
--rw-r--r--   0        0        0     5669 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/handlers/compression/lz4.py
--rw-r--r--   0        0        0     2876 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/handlers/compression/lzh.py
--rw-r--r--   0        0        0     1423 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/handlers/compression/lzip.py
--rw-r--r--   0        0        0     3438 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/handlers/compression/lzma.py
--rw-r--r--   0        0        0     4150 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/handlers/compression/lzo.py
--rw-r--r--   0        0        0     6086 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/handlers/compression/xz.py
--rw-r--r--   0        0        0     1935 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/handlers/compression/zlib.py
--rw-r--r--   0        0        0     2809 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/handlers/compression/zstd.py
--rw-r--r--   0        0        0        0 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/handlers/executable/__init__.py
--rw-r--r--   0        0        0    15477 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/handlers/executable/elf.py
--rw-r--r--   0        0        0        0 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/handlers/filesystem/__init__.py
--rw-r--r--   0        0        0        0 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/handlers/filesystem/android/__init__.py
--rw-r--r--   0        0        0     2889 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/handlers/filesystem/android/sparse.py
--rw-r--r--   0        0        0     2320 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/handlers/filesystem/cramfs.py
--rw-r--r--   0        0        0     4853 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/handlers/filesystem/extfs.py
--rw-r--r--   0        0        0     2123 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/handlers/filesystem/fat.py
--rw-r--r--   0        0        0     4604 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/handlers/filesystem/iso9660.py
--rw-r--r--   0        0        0     5213 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/handlers/filesystem/jffs2.py
--rw-r--r--   0        0        0     2246 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/handlers/filesystem/ntfs.py
--rw-r--r--   0        0        0    11455 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/handlers/filesystem/romfs.py
--rw-r--r--   0        0        0    10594 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/handlers/filesystem/squashfs.py
--rw-r--r--   0        0        0     5738 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/handlers/filesystem/ubi.py
--rw-r--r--   0        0        0    26635 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/handlers/filesystem/yaffs.py
--rw-r--r--   0        0        0      557 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/hookspecs.py
--rw-r--r--   0        0        0      515 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/identifiers.py
--rwxr-xr-x   0        0        0     1115 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/install-deps.sh
--rw-r--r--   0        0        0      583 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/iter_utils.py
--rw-r--r--   0        0        0     5097 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/logging.py
--rw-r--r--   0        0        0    14171 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/models.py
--rw-r--r--   0        0        0     2310 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/parser.py
--rw-r--r--   0        0        0     3808 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/plugins.py
--rw-r--r--   0        0        0     4090 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/pool.py
--rw-r--r--   0        0        0    27024 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/processing.py
--rw-r--r--   0        0        0        0 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/py.typed
--rw-r--r--   0        0        0     7779 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/report.py
--rw-r--r--   0        0        0     1538 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/signals.py
--rw-r--r--   0        0        0     3583 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/testing.py
--rw-r--r--   0        0        0     1475 2024-02-20 11:06:44.824008 unblob-24.2.20/unblob/ui.py
--rw-r--r--   0        0        0     1344 1970-01-01 00:00:00.000000 unblob-24.2.20/PKG-INFO
+-rw-r--r--   0        0        0     2255 2024-04-05 07:12:38.828571 unblob-24.4.5/LICENSE
+-rw-r--r--   0        0        0     5228 2024-04-05 07:12:38.832571 unblob-24.4.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-05 07:12:39.744574 unblob-24.4.5/unblob/__init__.py
+-rwxr-xr-x   0        0        0    14919 2024-04-05 07:12:39.744574 unblob-24.4.5/unblob/cli.py
+-rw-r--r--   0        0        0      344 2024-04-05 07:12:39.744574 unblob-24.4.5/unblob/cli_options.py
+-rw-r--r--   0        0        0     1219 2024-04-05 07:12:39.744574 unblob-24.4.5/unblob/dependencies.py
+-rw-r--r--   0        0        0     4162 2024-04-05 07:12:39.744574 unblob-24.4.5/unblob/extractor.py
+-rw-r--r--   0        0        0      196 2024-04-05 07:12:39.744574 unblob-24.4.5/unblob/extractors/README.md
+-rw-r--r--   0        0        0       40 2024-04-05 07:12:39.744574 unblob-24.4.5/unblob/extractors/__init__.py
+-rw-r--r--   0        0        0     3798 2024-04-05 07:12:39.744574 unblob-24.4.5/unblob/extractors/command.py
+-rw-r--r--   0        0        0    21870 2024-04-05 07:12:39.744574 unblob-24.4.5/unblob/file_utils.py
+-rw-r--r--   0        0        0     5731 2024-04-05 07:12:39.744574 unblob-24.4.5/unblob/finder.py
+-rw-r--r--   0        0        0     2540 2024-04-05 07:12:39.744574 unblob-24.4.5/unblob/handlers/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-05 07:12:39.744574 unblob-24.4.5/unblob/handlers/archive/__init__.py
+-rw-r--r--   0        0        0     5864 2024-04-05 07:12:39.744574 unblob-24.4.5/unblob/handlers/archive/_safe_tarfile.py
+-rw-r--r--   0        0        0     1694 2024-04-05 07:12:39.744574 unblob-24.4.5/unblob/handlers/archive/ar.py
+-rw-r--r--   0        0        0     2775 2024-04-05 07:12:39.744574 unblob-24.4.5/unblob/handlers/archive/arc.py
+-rw-r--r--   0        0        0     5683 2024-04-05 07:12:39.744574 unblob-24.4.5/unblob/handlers/archive/arj.py
+-rw-r--r--   0        0        0     2505 2024-04-05 07:12:39.744574 unblob-24.4.5/unblob/handlers/archive/cab.py
+-rw-r--r--   0        0        0    12585 2024-04-05 07:12:39.744574 unblob-24.4.5/unblob/handlers/archive/cpio.py
+-rw-r--r--   0        0        0     2250 2024-04-05 07:12:39.744574 unblob-24.4.5/unblob/handlers/archive/dlink/encrpted_img.py
+-rw-r--r--   0        0        0     3589 2024-04-05 07:12:39.744574 unblob-24.4.5/unblob/handlers/archive/dlink/shrs.py
+-rw-r--r--   0        0        0     3700 2024-04-05 07:12:39.744574 unblob-24.4.5/unblob/handlers/archive/dmg.py
+-rw-r--r--   0        0        0     3018 2024-04-05 07:12:39.744574 unblob-24.4.5/unblob/handlers/archive/engeniustech/engenius.py
+-rw-r--r--   0        0        0     3282 2024-04-05 07:12:39.744574 unblob-24.4.5/unblob/handlers/archive/hp/bdl.py
+-rw-r--r--   0        0        0     3330 2024-04-05 07:12:39.744574 unblob-24.4.5/unblob/handlers/archive/hp/ipkg.py
+-rw-r--r--   0        0        0     2946 2024-04-05 07:12:39.744574 unblob-24.4.5/unblob/handlers/archive/instar/bneg.py
+-rw-r--r--   0        0        0     1416 2024-04-05 07:12:39.744574 unblob-24.4.5/unblob/handlers/archive/instar/instar_hd.py
+-rw-r--r--   0        0        0     2553 2024-04-05 07:12:39.744574 unblob-24.4.5/unblob/handlers/archive/netgear/chk.py
+-rw-r--r--   0        0        0     4005 2024-04-05 07:12:39.744574 unblob-24.4.5/unblob/handlers/archive/netgear/trx.py
+-rw-r--r--   0        0        0     5543 2024-04-05 07:12:39.744574 unblob-24.4.5/unblob/handlers/archive/qnap/qnap_nas.py
+-rw-r--r--   0        0        0     1158 2024-04-05 07:12:39.744574 unblob-24.4.5/unblob/handlers/archive/rar.py
+-rw-r--r--   0        0        0     4075 2024-04-05 07:12:39.744574 unblob-24.4.5/unblob/handlers/archive/sevenzip.py
+-rw-r--r--   0        0        0     2332 2024-04-05 07:12:39.744574 unblob-24.4.5/unblob/handlers/archive/stuffit.py
+-rw-r--r--   0        0        0     8195 2024-04-05 07:12:39.744574 unblob-24.4.5/unblob/handlers/archive/tar.py
+-rw-r--r--   0        0        0     5892 2024-04-05 07:12:39.744574 unblob-24.4.5/unblob/handlers/archive/xiaomi/hdr.py
+-rw-r--r--   0        0        0     7627 2024-04-05 07:12:39.744574 unblob-24.4.5/unblob/handlers/archive/zip.py
+-rw-r--r--   0        0        0        0 2024-04-05 07:12:39.744574 unblob-24.4.5/unblob/handlers/compression/__init__.py
+-rw-r--r--   0        0        0     1299 2024-04-05 07:12:39.744574 unblob-24.4.5/unblob/handlers/compression/_gzip_reader.py
+-rw-r--r--   0        0        0     4709 2024-04-05 07:12:39.744574 unblob-24.4.5/unblob/handlers/compression/bzip2.py
+-rw-r--r--   0        0        0     8898 2024-04-05 07:12:39.744574 unblob-24.4.5/unblob/handlers/compression/compress.py
+-rw-r--r--   0        0        0     5770 2024-04-05 07:12:39.744574 unblob-24.4.5/unblob/handlers/compression/gzip.py
+-rw-r--r--   0        0        0     5669 2024-04-05 07:12:39.744574 unblob-24.4.5/unblob/handlers/compression/lz4.py
+-rw-r--r--   0        0        0     2876 2024-04-05 07:12:39.744574 unblob-24.4.5/unblob/handlers/compression/lzh.py
+-rw-r--r--   0        0        0     1423 2024-04-05 07:12:39.744574 unblob-24.4.5/unblob/handlers/compression/lzip.py
+-rw-r--r--   0        0        0     3438 2024-04-05 07:12:39.744574 unblob-24.4.5/unblob/handlers/compression/lzma.py
+-rw-r--r--   0        0        0     4150 2024-04-05 07:12:39.744574 unblob-24.4.5/unblob/handlers/compression/lzo.py
+-rw-r--r--   0        0        0     6086 2024-04-05 07:12:39.744574 unblob-24.4.5/unblob/handlers/compression/xz.py
+-rw-r--r--   0        0        0     1935 2024-04-05 07:12:39.744574 unblob-24.4.5/unblob/handlers/compression/zlib.py
+-rw-r--r--   0        0        0     2809 2024-04-05 07:12:39.744574 unblob-24.4.5/unblob/handlers/compression/zstd.py
+-rw-r--r--   0        0        0        0 2024-04-05 07:12:39.744574 unblob-24.4.5/unblob/handlers/executable/__init__.py
+-rw-r--r--   0        0        0    15477 2024-04-05 07:12:39.744574 unblob-24.4.5/unblob/handlers/executable/elf.py
+-rw-r--r--   0        0        0        0 2024-04-05 07:12:39.744574 unblob-24.4.5/unblob/handlers/filesystem/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-05 07:12:39.744574 unblob-24.4.5/unblob/handlers/filesystem/android/__init__.py
+-rw-r--r--   0        0        0     2889 2024-04-05 07:12:39.744574 unblob-24.4.5/unblob/handlers/filesystem/android/sparse.py
+-rw-r--r--   0        0        0     2320 2024-04-05 07:12:39.744574 unblob-24.4.5/unblob/handlers/filesystem/cramfs.py
+-rw-r--r--   0        0        0     5078 2024-04-05 07:12:39.744574 unblob-24.4.5/unblob/handlers/filesystem/extfs.py
+-rw-r--r--   0        0        0     2123 2024-04-05 07:12:39.744574 unblob-24.4.5/unblob/handlers/filesystem/fat.py
+-rw-r--r--   0        0        0     4604 2024-04-05 07:12:39.744574 unblob-24.4.5/unblob/handlers/filesystem/iso9660.py
+-rw-r--r--   0        0        0     5213 2024-04-05 07:12:39.744574 unblob-24.4.5/unblob/handlers/filesystem/jffs2.py
+-rw-r--r--   0        0        0     2246 2024-04-05 07:12:39.748574 unblob-24.4.5/unblob/handlers/filesystem/ntfs.py
+-rw-r--r--   0        0        0    11455 2024-04-05 07:12:39.748574 unblob-24.4.5/unblob/handlers/filesystem/romfs.py
+-rw-r--r--   0        0        0    10594 2024-04-05 07:12:39.748574 unblob-24.4.5/unblob/handlers/filesystem/squashfs.py
+-rw-r--r--   0        0        0     5738 2024-04-05 07:12:39.748574 unblob-24.4.5/unblob/handlers/filesystem/ubi.py
+-rw-r--r--   0        0        0    26635 2024-04-05 07:12:39.748574 unblob-24.4.5/unblob/handlers/filesystem/yaffs.py
+-rw-r--r--   0        0        0      557 2024-04-05 07:12:39.748574 unblob-24.4.5/unblob/hookspecs.py
+-rw-r--r--   0        0        0      515 2024-04-05 07:12:39.748574 unblob-24.4.5/unblob/identifiers.py
+-rwxr-xr-x   0        0        0     1115 2024-04-05 07:12:39.748574 unblob-24.4.5/unblob/install-deps.sh
+-rw-r--r--   0        0        0      583 2024-04-05 07:12:39.748574 unblob-24.4.5/unblob/iter_utils.py
+-rw-r--r--   0        0        0     5097 2024-04-05 07:12:39.748574 unblob-24.4.5/unblob/logging.py
+-rw-r--r--   0        0        0    14171 2024-04-05 07:12:39.748574 unblob-24.4.5/unblob/models.py
+-rw-r--r--   0        0        0     2310 2024-04-05 07:12:39.748574 unblob-24.4.5/unblob/parser.py
+-rw-r--r--   0        0        0     3808 2024-04-05 07:12:39.748574 unblob-24.4.5/unblob/plugins.py
+-rw-r--r--   0        0        0     4090 2024-04-05 07:12:39.748574 unblob-24.4.5/unblob/pool.py
+-rw-r--r--   0        0        0    27001 2024-04-05 07:12:39.748574 unblob-24.4.5/unblob/processing.py
+-rw-r--r--   0        0        0        0 2024-04-05 07:12:39.748574 unblob-24.4.5/unblob/py.typed
+-rw-r--r--   0        0        0     7779 2024-04-05 07:12:39.748574 unblob-24.4.5/unblob/report.py
+-rw-r--r--   0        0        0     1538 2024-04-05 07:12:39.748574 unblob-24.4.5/unblob/signals.py
+-rw-r--r--   0        0        0     3583 2024-04-05 07:12:39.748574 unblob-24.4.5/unblob/testing.py
+-rw-r--r--   0        0        0     1475 2024-04-05 07:12:39.748574 unblob-24.4.5/unblob/ui.py
+-rw-r--r--   0        0        0     1343 1970-01-01 00:00:00.000000 unblob-24.4.5/PKG-INFO
```

### Comparing `unblob-24.2.20/LICENSE` & `unblob-24.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `unblob-24.2.20/pyproject.toml` & `unblob-24.4.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "unblob"
-version = "24.2.20"
+version = "24.4.5"
 description = "Extract files from any kind of container formats"
 authors = ["ONEKEY <support@onekey.com>"]
 license = "MIT"
 packages = [
     { include = "unblob" },
 ]
 
@@ -34,24 +34,24 @@
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.0.0"
 pyright = "^1.1.349"
 pre-commit = "^3.5.0"
-pytest-cov = ">=3,<5"
-ruff = ">=0.1.13,<0.3.0"
+pytest-cov = ">=3,<6"
+ruff = ">=0.1.13,<0.4.0"
 pyyaml = "^6.0.1"
 atheris = { version = "^2.3.0", python = "<3.12" }
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
-mkdocs-material = "9.5.9"
+mkdocs-material = "9.5.16"
 mkdocstrings = "^0.24.0"
 pillow = ">=10.2.0,<11.0"
 cairosvg = "^2.7.1"
 mkdocstrings-python = "^1.8.0"
 
 [tool.poetry.scripts]
 unblob = "unblob.cli:main"
```

### Comparing `unblob-24.2.20/unblob/cli.py` & `unblob-24.4.5/unblob/cli.py`

 * *Files identical despite different names*

### Comparing `unblob-24.2.20/unblob/dependencies.py` & `unblob-24.4.5/unblob/dependencies.py`

 * *Files identical despite different names*

### Comparing `unblob-24.2.20/unblob/extractor.py` & `unblob-24.4.5/unblob/extractor.py`

 * *Files identical despite different names*

### Comparing `unblob-24.2.20/unblob/extractors/command.py` & `unblob-24.4.5/unblob/extractors/command.py`

 * *Files identical despite different names*

### Comparing `unblob-24.2.20/unblob/file_utils.py` & `unblob-24.4.5/unblob/file_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,22 +41,29 @@
 
 
 class File(mmap.mmap):
     access: int
 
     @classmethod
     def from_bytes(cls, content: bytes):
+        if not content:
+            raise ValueError("Can't create File from empty bytes.")
         m = cls(-1, len(content))
         m.write(content)
         m.seek(0)
         m.access = mmap.ACCESS_WRITE
         return m
 
     @classmethod
     def from_path(cls, path: Path, access=mmap.ACCESS_READ):
+        """Create File.
+
+        Needs a valid non-empty file,
+        raises ValueError on empty files.
+        """
         mode = "r+b" if access == mmap.ACCESS_WRITE else "rb"
         with path.open(mode) as base_file:
             m = cls(base_file.fileno(), 0, access=access)
             m.access = access
             return m
 
     def seek(self, pos: int, whence: int = os.SEEK_SET) -> int:
@@ -617,11 +624,11 @@
         safe_path = self._get_extraction_path(path, "open")
 
         self._ensure_parent_dir(safe_path)
         return safe_path.open(mode)
 
     def unlink(self, path):
         """Delete file within extraction path."""
-        logger.debug("unlink file", file_path=path)
+        logger.debug("unlink file", file_path=path, _verbosity=3)
         safe_path = self._get_extraction_path(path, "unlink")
 
         safe_path.unlink(missing_ok=True)
```

### Comparing `unblob-24.2.20/unblob/finder.py` & `unblob-24.4.5/unblob/finder.py`

 * *Files identical despite different names*

### Comparing `unblob-24.2.20/unblob/handlers/__init__.py` & `unblob-24.4.5/unblob/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `unblob-24.2.20/unblob/handlers/archive/_safe_tarfile.py` & `unblob-24.4.5/unblob/handlers/archive/_safe_tarfile.py`

 * *Files identical despite different names*

### Comparing `unblob-24.2.20/unblob/handlers/archive/ar.py` & `unblob-24.4.5/unblob/handlers/archive/ar.py`

 * *Files identical despite different names*

### Comparing `unblob-24.2.20/unblob/handlers/archive/arc.py` & `unblob-24.4.5/unblob/handlers/archive/arc.py`

 * *Files identical despite different names*

### Comparing `unblob-24.2.20/unblob/handlers/archive/arj.py` & `unblob-24.4.5/unblob/handlers/archive/arj.py`

 * *Files identical despite different names*

### Comparing `unblob-24.2.20/unblob/handlers/archive/cab.py` & `unblob-24.4.5/unblob/handlers/archive/cab.py`

 * *Files identical despite different names*

### Comparing `unblob-24.2.20/unblob/handlers/archive/cpio.py` & `unblob-24.4.5/unblob/handlers/archive/cpio.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,14 +206,19 @@
 
     def dump_entries(self, fs: FileSystem):
         for entry in self.entries:
             # skip entries with "." as filename
             if entry.path.name in ("", "."):
                 continue
 
+            # There are cases where CPIO archives have duplicated entries
+            # We then unlink the files to overwrite them and avoid an error.
+            if not stat.S_ISDIR(entry.mode):
+                fs.unlink(entry.path)
+
             if stat.S_ISREG(entry.mode):
                 fs.carve(entry.path, self.file, entry.start_offset, entry.size)
             elif stat.S_ISDIR(entry.mode):
                 fs.mkdir(
                     entry.path, mode=entry.mode & 0o777, parents=True, exist_ok=True
                 )
             elif stat.S_ISLNK(entry.mode):
```

### Comparing `unblob-24.2.20/unblob/handlers/archive/dlink/encrpted_img.py` & `unblob-24.4.5/unblob/handlers/archive/dlink/encrpted_img.py`

 * *Files identical despite different names*

### Comparing `unblob-24.2.20/unblob/handlers/archive/dlink/shrs.py` & `unblob-24.4.5/unblob/handlers/archive/dlink/shrs.py`

 * *Files identical despite different names*

### Comparing `unblob-24.2.20/unblob/handlers/archive/dmg.py` & `unblob-24.4.5/unblob/handlers/archive/dmg.py`

 * *Files identical despite different names*

### Comparing `unblob-24.2.20/unblob/handlers/archive/engeniustech/engenius.py` & `unblob-24.4.5/unblob/handlers/archive/engeniustech/engenius.py`

 * *Files identical despite different names*

### Comparing `unblob-24.2.20/unblob/handlers/archive/hp/bdl.py` & `unblob-24.4.5/unblob/handlers/archive/hp/bdl.py`

 * *Files identical despite different names*

### Comparing `unblob-24.2.20/unblob/handlers/archive/hp/ipkg.py` & `unblob-24.4.5/unblob/handlers/archive/hp/ipkg.py`

 * *Files identical despite different names*

### Comparing `unblob-24.2.20/unblob/handlers/archive/instar/bneg.py` & `unblob-24.4.5/unblob/handlers/archive/instar/bneg.py`

 * *Files identical despite different names*

### Comparing `unblob-24.2.20/unblob/handlers/archive/instar/instar_hd.py` & `unblob-24.4.5/unblob/handlers/archive/instar/instar_hd.py`

 * *Files identical despite different names*

### Comparing `unblob-24.2.20/unblob/handlers/archive/netgear/chk.py` & `unblob-24.4.5/unblob/handlers/archive/netgear/chk.py`

 * *Files identical despite different names*

### Comparing `unblob-24.2.20/unblob/handlers/archive/netgear/trx.py` & `unblob-24.4.5/unblob/handlers/archive/netgear/trx.py`

 * *Files identical despite different names*

### Comparing `unblob-24.2.20/unblob/handlers/archive/qnap/qnap_nas.py` & `unblob-24.4.5/unblob/handlers/archive/qnap/qnap_nas.py`

 * *Files identical despite different names*

### Comparing `unblob-24.2.20/unblob/handlers/archive/rar.py` & `unblob-24.4.5/unblob/handlers/archive/rar.py`

 * *Files identical despite different names*

### Comparing `unblob-24.2.20/unblob/handlers/archive/sevenzip.py` & `unblob-24.4.5/unblob/handlers/archive/sevenzip.py`

 * *Files identical despite different names*

### Comparing `unblob-24.2.20/unblob/handlers/archive/stuffit.py` & `unblob-24.4.5/unblob/handlers/archive/stuffit.py`

 * *Files identical despite different names*

### Comparing `unblob-24.2.20/unblob/handlers/archive/tar.py` & `unblob-24.4.5/unblob/handlers/archive/tar.py`

 * *Files identical despite different names*

### Comparing `unblob-24.2.20/unblob/handlers/archive/xiaomi/hdr.py` & `unblob-24.4.5/unblob/handlers/archive/xiaomi/hdr.py`

 * *Files identical despite different names*

### Comparing `unblob-24.2.20/unblob/handlers/archive/zip.py` & `unblob-24.4.5/unblob/handlers/archive/zip.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,17 +32,17 @@
             uint16 file_name_length;
             uint16 extra_field_length;
             uint16 file_comment_length;
             uint16 disk_number_start;
             uint16 internal_file_attr;
             uint32 external_file_attr;
             uint32 relative_offset_local_header;
-            char file_name[file_name_length];
-            char extra_field[extra_field_length];
-        } cd_file_header_t;
+            // char file_name[file_name_length];
+            // char extra_field[extra_field_length];
+        } partial_cd_file_header_t;
 
         typedef struct end_of_central_directory
         {
             uint32 end_of_central_signature;
             uint16 disk_number;
             uint16 disk_number_with_cd;
             uint16 disk_entries;
@@ -90,16 +90,20 @@
         self,
         file: File,
         start_offset: int,
         end_of_central_directory: Instance,
     ) -> bool:
         file.seek(start_offset + end_of_central_directory.offset_of_cd, io.SEEK_SET)
         for _ in range(end_of_central_directory.total_entries):
-            cd_header = self.cparser_le.cd_file_header_t(file)
-            if cd_header.flags & self.ENCRYPTED_FLAG:
+            file_header = self.cparser_le.partial_cd_file_header_t(file)
+            file.seek(
+                file_header.file_name_length + file_header.extra_field_length,
+                io.SEEK_CUR,
+            )
+            if file_header.flags & self.ENCRYPTED_FLAG:
                 return True
         return False
 
     @staticmethod
     def is_zip64_eocd(end_of_central_directory: Instance):
         # see https://pkware.cachefly.net/webdocs/APPNOTE/APPNOTE-6.3.1.TXT section J
         return (
@@ -107,14 +111,22 @@
             or end_of_central_directory.disk_number_with_cd == 0xFFFF
             or end_of_central_directory.disk_entries == 0xFFFF
             or end_of_central_directory.total_entries == 0xFFFF
             or end_of_central_directory.central_directory_size == 0xFFFFFFFF
             or end_of_central_directory.offset_of_cd == 0xFFFFFFFF
         )
 
+    @staticmethod
+    def is_zip64_cd_file(file_header: Instance):
+        # see https://pkware.cachefly.net/webdocs/casestudies/APPNOTE.TXT section 4.3.9.2
+        return (
+            file_header.file_size == 0xFFFFFFFF
+            or file_header.compress_size == 0xFFFFFFFF
+        )
+
     def _parse_zip64(self, file: File, start_offset: int, offset: int) -> Instance:
         file.seek(start_offset, io.SEEK_SET)
         for eocd_locator_offset in iterate_patterns(
             file, struct.pack("<I", self.ZIP64_EOCD_LOCATOR_HEADER)
         ):
             file.seek(eocd_locator_offset, io.SEEK_SET)
             eocd_locator = self.cparser_le.zip64_end_of_central_directory_locator_t(
@@ -133,25 +145,40 @@
                         "Missing ZIP64 EOCD header record header in ZIP chunk."
                     )
                 return zip64_eocd
         raise InvalidInputFormat(
             "Missing ZIP64 EOCD locator record header in ZIP chunk."
         )
 
+    def is_zip64(self, file, start_offset, offset, end_of_central_directory):
+        absolute_offset_of_cd = start_offset + end_of_central_directory.offset_of_cd
+
+        if 0 < absolute_offset_of_cd < offset:
+            file.seek(absolute_offset_of_cd, io.SEEK_SET)
+            file_header = self.cparser_le.partial_cd_file_header_t(file)
+            if self.is_zip64_cd_file(file_header):
+                return True
+
+        # some values in the CD can be FFFF, indicating its a zip64
+        # if the offset of the CD is 0xFFFFFFFF, its definitely one
+        # otherwise we check every other header indicating zip64
+        return self.is_zip64_eocd(end_of_central_directory)
+
     def calculate_chunk(self, file: File, start_offset: int) -> Optional[ValidChunk]:
         has_encrypted_files = False
         file.seek(start_offset, io.SEEK_SET)
 
         for offset in iterate_patterns(
             file, struct.pack("<I", self.EOCD_RECORD_HEADER)
         ):
             file.seek(offset, io.SEEK_SET)
             end_of_central_directory = self.parse_header(file)
 
-            if self.is_zip64_eocd(end_of_central_directory):
+            if self.is_zip64(file, start_offset, offset, end_of_central_directory):
+                file.seek(offset, io.SEEK_SET)
                 end_of_central_directory = self._parse_zip64(file, start_offset, offset)
                 break
 
             # the EOCD offset is equal to the offset of CD + size of CD
             end_of_central_directory_offset = (
                 start_offset
                 + end_of_central_directory.offset_of_cd
```

### Comparing `unblob-24.2.20/unblob/handlers/compression/_gzip_reader.py` & `unblob-24.4.5/unblob/handlers/compression/_gzip_reader.py`

 * *Files identical despite different names*

### Comparing `unblob-24.2.20/unblob/handlers/compression/bzip2.py` & `unblob-24.4.5/unblob/handlers/compression/bzip2.py`

 * *Files identical despite different names*

### Comparing `unblob-24.2.20/unblob/handlers/compression/compress.py` & `unblob-24.4.5/unblob/handlers/compression/compress.py`

 * *Files identical despite different names*

### Comparing `unblob-24.2.20/unblob/handlers/compression/gzip.py` & `unblob-24.4.5/unblob/handlers/compression/gzip.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,20 @@
 class MultiVolumeGzipHandler(DirectoryHandler):
     NAME = "multi-gzip"
     EXTRACTOR = MultiGZIPExtractor()
 
     PATTERN = Glob("*.gz.*")
 
     def is_valid_gzip(self, path: Path) -> bool:
-        with File.from_path(path) as f:
+        try:
+            file = File.from_path(path)
+        except ValueError:
+            return False
+
+        with file as f:
             try:
                 fp = SingleMemberGzipReader(f)
                 if not fp.read_header():
                     return False
             except gzip.BadGzipFile:
                 return False
         return True
```

### Comparing `unblob-24.2.20/unblob/handlers/compression/lz4.py` & `unblob-24.4.5/unblob/handlers/compression/lz4.py`

 * *Files identical despite different names*

### Comparing `unblob-24.2.20/unblob/handlers/compression/lzh.py` & `unblob-24.4.5/unblob/handlers/compression/lzh.py`

 * *Files identical despite different names*

### Comparing `unblob-24.2.20/unblob/handlers/compression/lzip.py` & `unblob-24.4.5/unblob/handlers/compression/lzip.py`

 * *Files identical despite different names*

### Comparing `unblob-24.2.20/unblob/handlers/compression/lzma.py` & `unblob-24.4.5/unblob/handlers/compression/lzma.py`

 * *Files identical despite different names*

### Comparing `unblob-24.2.20/unblob/handlers/compression/lzo.py` & `unblob-24.4.5/unblob/handlers/compression/lzo.py`

 * *Files identical despite different names*

### Comparing `unblob-24.2.20/unblob/handlers/compression/xz.py` & `unblob-24.4.5/unblob/handlers/compression/xz.py`

 * *Files identical despite different names*

### Comparing `unblob-24.2.20/unblob/handlers/compression/zlib.py` & `unblob-24.4.5/unblob/handlers/compression/zlib.py`

 * *Files identical despite different names*

### Comparing `unblob-24.2.20/unblob/handlers/compression/zstd.py` & `unblob-24.4.5/unblob/handlers/compression/zstd.py`

 * *Files identical despite different names*

### Comparing `unblob-24.2.20/unblob/handlers/executable/elf.py` & `unblob-24.4.5/unblob/handlers/executable/elf.py`

 * *Files identical despite different names*

### Comparing `unblob-24.2.20/unblob/handlers/filesystem/android/sparse.py` & `unblob-24.4.5/unblob/handlers/filesystem/android/sparse.py`

 * *Files identical despite different names*

### Comparing `unblob-24.2.20/unblob/handlers/filesystem/cramfs.py` & `unblob-24.4.5/unblob/handlers/filesystem/cramfs.py`

 * *Files identical despite different names*

### Comparing `unblob-24.2.20/unblob/handlers/filesystem/extfs.py` & `unblob-24.4.5/unblob/handlers/filesystem/extfs.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,20 @@
             logger.debug("Creator OS value not valid.", creator_os=header.s_creator_os)
             return False
         if header.s_rev_level > 2:
             logger.debug(
                 "ExtFS header major version too high", rev_level=header.s_rev_level
             )
             return False
+        if header.s_log_block_size > 6:
+            logger.debug(
+                "ExtFS header s_log_block_size is too large",
+                s_log_block_size=header.s_log_block_size,
+            )
+            return False
         return True
 
     def calculate_chunk(self, file: File, start_offset: int) -> Optional[ValidChunk]:
         header = self.parse_header(file)
         end_offset = start_offset + (
             header.s_blocks_count_lo * (EXT_BLOCK_SIZE << header.s_log_block_size)
         )
```

### Comparing `unblob-24.2.20/unblob/handlers/filesystem/fat.py` & `unblob-24.4.5/unblob/handlers/filesystem/fat.py`

 * *Files identical despite different names*

### Comparing `unblob-24.2.20/unblob/handlers/filesystem/iso9660.py` & `unblob-24.4.5/unblob/handlers/filesystem/iso9660.py`

 * *Files identical despite different names*

### Comparing `unblob-24.2.20/unblob/handlers/filesystem/jffs2.py` & `unblob-24.4.5/unblob/handlers/filesystem/jffs2.py`

 * *Files identical despite different names*

### Comparing `unblob-24.2.20/unblob/handlers/filesystem/ntfs.py` & `unblob-24.4.5/unblob/handlers/filesystem/ntfs.py`

 * *Files identical despite different names*

### Comparing `unblob-24.2.20/unblob/handlers/filesystem/romfs.py` & `unblob-24.4.5/unblob/handlers/filesystem/romfs.py`

 * *Files identical despite different names*

### Comparing `unblob-24.2.20/unblob/handlers/filesystem/squashfs.py` & `unblob-24.4.5/unblob/handlers/filesystem/squashfs.py`

 * *Files identical despite different names*

### Comparing `unblob-24.2.20/unblob/handlers/filesystem/ubi.py` & `unblob-24.4.5/unblob/handlers/filesystem/ubi.py`

 * *Files identical despite different names*

### Comparing `unblob-24.2.20/unblob/handlers/filesystem/yaffs.py` & `unblob-24.4.5/unblob/handlers/filesystem/yaffs.py`

 * *Files identical despite different names*

### Comparing `unblob-24.2.20/unblob/hookspecs.py` & `unblob-24.4.5/unblob/hookspecs.py`

 * *Files identical despite different names*

### Comparing `unblob-24.2.20/unblob/identifiers.py` & `unblob-24.4.5/unblob/identifiers.py`

 * *Files identical despite different names*

### Comparing `unblob-24.2.20/unblob/install-deps.sh` & `unblob-24.4.5/unblob/install-deps.sh`

 * *Files identical despite different names*

### Comparing `unblob-24.2.20/unblob/iter_utils.py` & `unblob-24.4.5/unblob/iter_utils.py`

 * *Files identical despite different names*

### Comparing `unblob-24.2.20/unblob/logging.py` & `unblob-24.4.5/unblob/logging.py`

 * *Files identical despite different names*

### Comparing `unblob-24.2.20/unblob/models.py` & `unblob-24.4.5/unblob/models.py`

 * *Files identical despite different names*

### Comparing `unblob-24.2.20/unblob/parser.py` & `unblob-24.4.5/unblob/parser.py`

 * *Files identical despite different names*

### Comparing `unblob-24.2.20/unblob/plugins.py` & `unblob-24.4.5/unblob/plugins.py`

 * *Files identical despite different names*

### Comparing `unblob-24.2.20/unblob/pool.py` & `unblob-24.4.5/unblob/pool.py`

 * *Files identical despite different names*

### Comparing `unblob-24.2.20/unblob/processing.py` & `unblob-24.4.5/unblob/processing.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,14 @@
     "Intel serial flash for PCH ROM",
     "JPEG",
     "Java module image",
     "MPEG",
     "MS Windows icon resource",
     "Macromedia Flash data",
     "Microsoft Excel",
-    "Microsoft OOXML",
     "Microsoft PowerPoint",
     "Microsoft Word",
     "OpenDocument",
     "PDF document",
     "PNG",
     "SQLite",
     "TrueType Font data",
```

### Comparing `unblob-24.2.20/unblob/report.py` & `unblob-24.4.5/unblob/report.py`

 * *Files identical despite different names*

### Comparing `unblob-24.2.20/unblob/signals.py` & `unblob-24.4.5/unblob/signals.py`

 * *Files identical despite different names*

### Comparing `unblob-24.2.20/unblob/testing.py` & `unblob-24.4.5/unblob/testing.py`

 * *Files identical despite different names*

### Comparing `unblob-24.2.20/unblob/ui.py` & `unblob-24.4.5/unblob/ui.py`

 * *Files identical despite different names*

### Comparing `unblob-24.2.20/PKG-INFO` & `unblob-24.4.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unblob
-Version: 24.2.20
+Version: 24.4.5
 Summary: Extract files from any kind of container formats
 License: MIT
 Author: ONEKEY
 Author-email: support@onekey.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

