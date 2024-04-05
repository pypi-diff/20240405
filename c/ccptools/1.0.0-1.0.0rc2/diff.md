# Comparing `tmp/ccptools-1.0.0.tar.gz` & `tmp/ccptools-1.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccptools-1.0.0.tar", last modified: Fri Apr  5 11:38:22 2024, max compression
+gzip compressed data, was "ccptools-1.0.0rc2.tar", last modified: Thu Apr  4 15:33:08 2024, max compression
```

## Comparing `ccptools-1.0.0.tar` & `ccptools-1.0.0rc2.tar`

### file list

```diff
@@ -1,119 +1,146 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:38:22.023016 ccptools-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-05 11:38:10.000000 ccptools-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5938 2024-04-05 11:38:22.023016 ccptools-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-05 11:38:10.000000 ccptools-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:38:22.007016 ccptools-1.0.0/ccptools/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:38:22.007016 ccptools-1.0.0/ccptools/_common/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/_common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/_common/_decode.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:38:22.007016 ccptools-1.0.0/ccptools/dtu/
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/dtu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:38:22.007016 ccptools-1.0.0/ccptools/dtu/casting/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/dtu/casting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/dtu/casting/_any.py
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/dtu/casting/_filetime.py
--rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/dtu/casting/_string.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:38:22.007016 ccptools-1.0.0/ccptools/dtu/formatting/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/dtu/formatting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/dtu/formatting/_delta.py
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/dtu/formatting/_serialize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:38:22.007016 ccptools-1.0.0/ccptools/dtu/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/dtu/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/dtu/parsers/_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/dtu/parsers/_timedelta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:38:22.011016 ccptools-1.0.0/ccptools/dtu/shortcuts/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/dtu/shortcuts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/dtu/shortcuts/_aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/dtu/shortcuts/_checkers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/dtu/shortcuts/_finders.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:38:22.011016 ccptools-1.0.0/ccptools/dtu/structs/
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/dtu/structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/dtu/structs/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11898 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/dtu/structs/_deltasplit.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/dtu/structs/_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/dtu/structs/aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/dtu/structs/consts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:38:22.011016 ccptools-1.0.0/ccptools/legacyapi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/legacyapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:38:22.011016 ccptools-1.0.0/ccptools/legacyapi/datetimeutils/
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/legacyapi/datetimeutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/legacyapi/datetimeutils/_deltasplit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/legacyapi/datetimeutils/_find.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/legacyapi/datetimeutils/_timestamp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:38:22.015015 ccptools-1.0.0/ccptools/legacyapi/typeutils/
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/legacyapi/typeutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/legacyapi/typeutils/bases.py
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/legacyapi/typeutils/casting.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/legacyapi/typeutils/comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/legacyapi/typeutils/empty.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/legacyapi/typeutils/insp.py
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/legacyapi/typeutils/iters.py
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/legacyapi/typeutils/metas.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/legacyapi/typeutils/sentience.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/legacyapi/typeutils/size.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/legacyapi/typeutils/strimp.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/legacyapi/typeutils/string.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:38:22.015015 ccptools-1.0.0/ccptools/structs/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/structs/_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:38:22.015015 ccptools-1.0.0/ccptools/tpu/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/tpu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:38:22.015015 ccptools-1.0.0/ccptools/tpu/casting/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/tpu/casting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/tpu/casting/_currency.py
--rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/tpu/casting/_evals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/tpu/casting/_ip.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/tpu/casting/_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/tpu/casting/_params.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/tpu/casting/_serialize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:38:22.015015 ccptools-1.0.0/ccptools/tpu/comparison/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/tpu/comparison/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/tpu/comparison/_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:38:22.015015 ccptools-1.0.0/ccptools/tpu/insp/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/tpu/insp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13579 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/tpu/insp/_insp_old.py
--rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/tpu/insp/_typecheck.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:38:22.015015 ccptools-1.0.0/ccptools/tpu/iters/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/tpu/iters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/tpu/iters/_attrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4638 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/tpu/iters/_dicts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/tpu/iters/_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/tpu/iters/_lists.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:38:22.015015 ccptools-1.0.0/ccptools/tpu/size/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/tpu/size/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/tpu/size/_total.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:38:22.019015 ccptools-1.0.0/ccptools/tpu/strimp/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/tpu/strimp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11087 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/tpu/strimp/_getters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:38:22.019015 ccptools-1.0.0/ccptools/tpu/string/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/tpu/string/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/tpu/string/_string.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:38:22.019015 ccptools-1.0.0/ccptools/tpu/structs/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/tpu/structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/tpu/structs/_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:38:22.019015 ccptools-1.0.0/ccptools/tpu/structs/empty/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/tpu/structs/empty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9892 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/tpu/structs/empty/_empty.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:38:22.019015 ccptools-1.0.0/ccptools/tpu/structs/fluid/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/tpu/structs/fluid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/tpu/structs/fluid/_attrfluid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:38:22.019015 ccptools-1.0.0/ccptools/tpu/structs/sentience/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/tpu/structs/sentience/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/tpu/structs/sentience/_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:38:22.019015 ccptools-1.0.0/ccptools/tpu/structs/serializers/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/tpu/structs/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/tpu/structs/serializers/_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/tpu/structs/serializers/_jsonsafe.py
--rw-r--r--   0 runner    (1001) docker     (127)     9803 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/tpu/structs/serializers/_universal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:38:22.019015 ccptools-1.0.0/ccptools/tpu/structs/singleton/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/tpu/structs/singleton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-05 11:38:10.000000 ccptools-1.0.0/ccptools/tpu/structs/singleton/_singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:38:22.023016 ccptools-1.0.0/ccptools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5938 2024-04-05 11:38:21.000000 ccptools-1.0.0/ccptools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-04-05 11:38:21.000000 ccptools-1.0.0/ccptools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 11:38:21.000000 ccptools-1.0.0/ccptools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-05 11:38:21.000000 ccptools-1.0.0/ccptools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-04-05 11:38:10.000000 ccptools-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 11:38:22.023016 ccptools-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-05 11:38:10.000000 ccptools-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:33:08.799514 ccptools-1.0.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-04-04 15:33:08.799514 ccptools-1.0.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:33:08.787514 ccptools-1.0.0rc2/ccptools/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:33:08.787514 ccptools-1.0.0rc2/ccptools/_common/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/_common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/_common/_decode.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:33:08.787514 ccptools-1.0.0rc2/ccptools/dtu/
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/dtu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:33:08.787514 ccptools-1.0.0rc2/ccptools/dtu/casting/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/dtu/casting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/dtu/casting/_any.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/dtu/casting/_filetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/dtu/casting/_string.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:33:08.787514 ccptools-1.0.0rc2/ccptools/dtu/formatting/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/dtu/formatting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/dtu/formatting/_delta.py
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/dtu/formatting/_serialize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:33:08.787514 ccptools-1.0.0rc2/ccptools/dtu/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/dtu/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/dtu/parsers/_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/dtu/parsers/_timedelta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:33:08.787514 ccptools-1.0.0rc2/ccptools/dtu/shortcuts/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/dtu/shortcuts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/dtu/shortcuts/_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/dtu/shortcuts/_checkers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/dtu/shortcuts/_finders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:33:08.787514 ccptools-1.0.0rc2/ccptools/dtu/structs/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/dtu/structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/dtu/structs/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11898 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/dtu/structs/_deltasplit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/dtu/structs/_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/dtu/structs/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/dtu/structs/consts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:33:08.791514 ccptools-1.0.0rc2/ccptools/legacyapi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/legacyapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:33:08.791514 ccptools-1.0.0rc2/ccptools/legacyapi/datetimeutils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/legacyapi/datetimeutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/legacyapi/datetimeutils/_deltasplit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/legacyapi/datetimeutils/_find.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/legacyapi/datetimeutils/_timestamp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:33:08.791514 ccptools-1.0.0rc2/ccptools/legacyapi/typeutils/
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/legacyapi/typeutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/legacyapi/typeutils/bases.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/legacyapi/typeutils/casting.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/legacyapi/typeutils/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/legacyapi/typeutils/empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/legacyapi/typeutils/insp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/legacyapi/typeutils/iters.py
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/legacyapi/typeutils/metas.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/legacyapi/typeutils/sentience.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/legacyapi/typeutils/size.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/legacyapi/typeutils/strimp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/legacyapi/typeutils/string.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:33:08.791514 ccptools-1.0.0rc2/ccptools/structs/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/structs/_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:33:08.791514 ccptools-1.0.0rc2/ccptools/tpu/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/tpu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:33:08.791514 ccptools-1.0.0rc2/ccptools/tpu/casting/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/tpu/casting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/tpu/casting/_currency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/tpu/casting/_evals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/tpu/casting/_ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/tpu/casting/_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/tpu/casting/_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/tpu/casting/_serialize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:33:08.791514 ccptools-1.0.0rc2/ccptools/tpu/comparison/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/tpu/comparison/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/tpu/comparison/_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:33:08.795514 ccptools-1.0.0rc2/ccptools/tpu/insp/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/tpu/insp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13579 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/tpu/insp/_insp_old.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/tpu/insp/_typecheck.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:33:08.795514 ccptools-1.0.0rc2/ccptools/tpu/iters/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/tpu/iters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/tpu/iters/_attrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4638 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/tpu/iters/_dicts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/tpu/iters/_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/tpu/iters/_lists.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:33:08.795514 ccptools-1.0.0rc2/ccptools/tpu/size/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/tpu/size/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/tpu/size/_total.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:33:08.795514 ccptools-1.0.0rc2/ccptools/tpu/strimp/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/tpu/strimp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11087 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/tpu/strimp/_getters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:33:08.795514 ccptools-1.0.0rc2/ccptools/tpu/string/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/tpu/string/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/tpu/string/_string.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:33:08.795514 ccptools-1.0.0rc2/ccptools/tpu/structs/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/tpu/structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/tpu/structs/_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:33:08.795514 ccptools-1.0.0rc2/ccptools/tpu/structs/empty/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/tpu/structs/empty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9892 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/tpu/structs/empty/_empty.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:33:08.795514 ccptools-1.0.0rc2/ccptools/tpu/structs/fluid/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/tpu/structs/fluid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/tpu/structs/fluid/_attrfluid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:33:08.795514 ccptools-1.0.0rc2/ccptools/tpu/structs/sentience/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/tpu/structs/sentience/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/tpu/structs/sentience/_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:33:08.795514 ccptools-1.0.0rc2/ccptools/tpu/structs/serializers/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/tpu/structs/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/tpu/structs/serializers/_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/tpu/structs/serializers/_jsonsafe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9803 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/tpu/structs/serializers/_universal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:33:08.795514 ccptools-1.0.0rc2/ccptools/tpu/structs/singleton/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/tpu/structs/singleton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/ccptools/tpu/structs/singleton/_singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:33:08.787514 ccptools-1.0.0rc2/ccptools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-04-04 15:33:08.000000 ccptools-1.0.0rc2/ccptools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-04-04 15:33:08.000000 ccptools-1.0.0rc2/ccptools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 15:33:08.000000 ccptools-1.0.0rc2/ccptools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-04 15:33:08.000000 ccptools-1.0.0rc2/ccptools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 15:33:08.799514 ccptools-1.0.0rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:33:08.783514 ccptools-1.0.0rc2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:33:08.799514 ccptools-1.0.0rc2/tests/datetimeutils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/tests/datetimeutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10442 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/tests/datetimeutils/test_datetimeutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/tests/datetimeutils/test_deltasplit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/tests/datetimeutils/test_filetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/tests/datetimeutils/test_finders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12142 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/tests/datetimeutils/test_legacy_datetimeutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:33:08.799514 ccptools-1.0.0rc2/tests/typeutils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/tests/typeutils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:33:08.799514 ccptools-1.0.0rc2/tests/typeutils/sometypes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/tests/typeutils/sometypes/IamModule.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/tests/typeutils/sometypes/IamOtherModule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/tests/typeutils/sometypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/tests/typeutils/test_any_getter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/tests/typeutils/test_group_by.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4796 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/tests/typeutils/test_legacy_typeutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/tests/typeutils/test_legacy_typeutils_bases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/tests/typeutils/test_legacy_typeutils_casting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-04 15:33:00.000000 ccptools-1.0.0rc2/tests/typeutils/test_legacy_typeutils_empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28318 2024-04-04 15:33:01.000000 ccptools-1.0.0rc2/tests/typeutils/test_legacy_typeutils_insp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6836 2024-04-04 15:33:01.000000 ccptools-1.0.0rc2/tests/typeutils/test_legacy_typeutils_iters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-04 15:33:01.000000 ccptools-1.0.0rc2/tests/typeutils/test_legacy_typeutils_nested_getter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-04 15:33:01.000000 ccptools-1.0.0rc2/tests/typeutils/test_legacy_typeutils_sentient_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16530 2024-04-04 15:33:01.000000 ccptools-1.0.0rc2/tests/typeutils/test_legacy_typeutils_strimp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-04-04 15:33:01.000000 ccptools-1.0.0rc2/tests/typeutils/test_legacy_typeutils_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40931 2024-04-04 15:33:01.000000 ccptools-1.0.0rc2/tests/typeutils/test_legacy_typeutils_typecheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5491 2024-04-04 15:33:01.000000 ccptools-1.0.0rc2/tests/typeutils/test_serializer.py
```

### Comparing `ccptools-1.0.0/LICENSE` & `ccptools-1.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `ccptools-1.0.0/PKG-INFO` & `ccptools-1.0.0rc2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 Metadata-Version: 2.1
 Name: ccptools
-Version: 1.0.0
+Version: 1.0.0rc2
 Summary: The CCP Tools team utilities for date and/or time objects and values and messing with types.
-Author-email: Thordur Matthiasson <thordurm@ccpgames.com>, John Aldis <johnaldis@ccpgames.com>
+Home-page: https://github.com/ccpgames/ccptools
+Author: Thordur Matthiasson
+Author-email: thordurm@ccpgames.com
 License: MIT License
         
         Copyright (c) 2013-2024 CCP Games
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -21,34 +23,21 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: Homepage, https://github.com/ccpgames/ccptools
-Project-URL: Documentation, https://github.com/ccpgames/ccptools/blob/main/README.md
-Project-URL: Repository, https://github.com/ccpgames/ccptools.git
-Project-URL: Issues, https://github.com/ccpgames/ccptools/issues
-Project-URL: Changelog, https://github.com/ccpgames/ccptools/blob/main/CHANGELOG.md
-Keywords: datetimeutils,datetime,typeutils,type,singleton,date,time,timespan,tools,ccp,utils
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CCP Games Python Toolkit
 
 A smooshup of a few Python packages from the CCP Tools Team of old (Team 
 Batcave).
@@ -158,7 +147,8 @@
 
 So in most cases we can cover something like 90% of any imports we tend to 
 need in every Python file with a single line:
 
 ```python
 from ccptools.structs import *
 ```
+
```

### Comparing `ccptools-1.0.0/README.md` & `ccptools-1.0.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `ccptools-1.0.0/ccptools/_common/_decode.py` & `ccptools-1.0.0rc2/ccptools/_common/_decode.py`

 * *Files identical despite different names*

### Comparing `ccptools-1.0.0/ccptools/dtu/casting/_any.py` & `ccptools-1.0.0rc2/ccptools/dtu/casting/_any.py`

 * *Files identical despite different names*

### Comparing `ccptools-1.0.0/ccptools/dtu/casting/_filetime.py` & `ccptools-1.0.0rc2/ccptools/dtu/casting/_filetime.py`

 * *Files identical despite different names*

### Comparing `ccptools-1.0.0/ccptools/dtu/casting/_string.py` & `ccptools-1.0.0rc2/ccptools/dtu/casting/_string.py`

 * *Files identical despite different names*

### Comparing `ccptools-1.0.0/ccptools/dtu/formatting/_delta.py` & `ccptools-1.0.0rc2/ccptools/dtu/formatting/_delta.py`

 * *Files identical despite different names*

### Comparing `ccptools-1.0.0/ccptools/dtu/formatting/_serialize.py` & `ccptools-1.0.0rc2/ccptools/dtu/formatting/_serialize.py`

 * *Files identical despite different names*

### Comparing `ccptools-1.0.0/ccptools/dtu/parsers/_string.py` & `ccptools-1.0.0rc2/ccptools/dtu/parsers/_string.py`

 * *Files identical despite different names*

### Comparing `ccptools-1.0.0/ccptools/dtu/parsers/_timedelta.py` & `ccptools-1.0.0rc2/ccptools/dtu/parsers/_timedelta.py`

 * *Files identical despite different names*

### Comparing `ccptools-1.0.0/ccptools/dtu/shortcuts/_aliases.py` & `ccptools-1.0.0rc2/ccptools/dtu/shortcuts/_aliases.py`

 * *Files identical despite different names*

### Comparing `ccptools-1.0.0/ccptools/dtu/shortcuts/_finders.py` & `ccptools-1.0.0rc2/ccptools/dtu/shortcuts/_finders.py`

 * *Files identical despite different names*

### Comparing `ccptools-1.0.0/ccptools/dtu/structs/_deltasplit.py` & `ccptools-1.0.0rc2/ccptools/dtu/structs/_deltasplit.py`

 * *Files identical despite different names*

### Comparing `ccptools-1.0.0/ccptools/dtu/structs/_types.py` & `ccptools-1.0.0rc2/ccptools/dtu/structs/_types.py`

 * *Files identical despite different names*

### Comparing `ccptools-1.0.0/ccptools/dtu/structs/aliases.py` & `ccptools-1.0.0rc2/ccptools/dtu/structs/aliases.py`

 * *Files identical despite different names*

### Comparing `ccptools-1.0.0/ccptools/dtu/structs/consts.py` & `ccptools-1.0.0rc2/ccptools/dtu/structs/consts.py`

 * *Files identical despite different names*

### Comparing `ccptools-1.0.0/ccptools/legacyapi/datetimeutils/__init__.py` & `ccptools-1.0.0rc2/ccptools/legacyapi/datetimeutils/__init__.py`

 * *Files identical despite different names*

### Comparing `ccptools-1.0.0/ccptools/legacyapi/datetimeutils/_deltasplit.py` & `ccptools-1.0.0rc2/ccptools/legacyapi/datetimeutils/_deltasplit.py`

 * *Files identical despite different names*

### Comparing `ccptools-1.0.0/ccptools/legacyapi/datetimeutils/_find.py` & `ccptools-1.0.0rc2/ccptools/legacyapi/datetimeutils/_find.py`

 * *Files identical despite different names*

### Comparing `ccptools-1.0.0/ccptools/legacyapi/datetimeutils/_timestamp.py` & `ccptools-1.0.0rc2/ccptools/legacyapi/datetimeutils/_timestamp.py`

 * *Files identical despite different names*

### Comparing `ccptools-1.0.0/ccptools/legacyapi/typeutils/__init__.py` & `ccptools-1.0.0rc2/ccptools/legacyapi/typeutils/__init__.py`

 * *Files identical despite different names*

### Comparing `ccptools-1.0.0/ccptools/legacyapi/typeutils/casting.py` & `ccptools-1.0.0rc2/ccptools/legacyapi/typeutils/casting.py`

 * *Files identical despite different names*

### Comparing `ccptools-1.0.0/ccptools/legacyapi/typeutils/insp.py` & `ccptools-1.0.0rc2/ccptools/legacyapi/typeutils/insp.py`

 * *Files identical despite different names*

### Comparing `ccptools-1.0.0/ccptools/legacyapi/typeutils/iters.py` & `ccptools-1.0.0rc2/ccptools/legacyapi/typeutils/iters.py`

 * *Files identical despite different names*

### Comparing `ccptools-1.0.0/ccptools/tpu/casting/_currency.py` & `ccptools-1.0.0rc2/ccptools/tpu/casting/_currency.py`

 * *Files identical despite different names*

### Comparing `ccptools-1.0.0/ccptools/tpu/casting/_evals.py` & `ccptools-1.0.0rc2/ccptools/tpu/casting/_evals.py`

 * *Files identical despite different names*

### Comparing `ccptools-1.0.0/ccptools/tpu/casting/_ip.py` & `ccptools-1.0.0rc2/ccptools/tpu/casting/_ip.py`

 * *Files identical despite different names*

### Comparing `ccptools-1.0.0/ccptools/tpu/casting/_mask.py` & `ccptools-1.0.0rc2/ccptools/tpu/casting/_mask.py`

 * *Files identical despite different names*

### Comparing `ccptools-1.0.0/ccptools/tpu/casting/_params.py` & `ccptools-1.0.0rc2/ccptools/tpu/casting/_params.py`

 * *Files identical despite different names*

### Comparing `ccptools-1.0.0/ccptools/tpu/casting/_serialize.py` & `ccptools-1.0.0rc2/ccptools/tpu/casting/_serialize.py`

 * *Files identical despite different names*

### Comparing `ccptools-1.0.0/ccptools/tpu/comparison/_mixin.py` & `ccptools-1.0.0rc2/ccptools/tpu/comparison/_mixin.py`

 * *Files identical despite different names*

### Comparing `ccptools-1.0.0/ccptools/tpu/insp/_insp_old.py` & `ccptools-1.0.0rc2/ccptools/tpu/insp/_insp_old.py`

 * *Files identical despite different names*

### Comparing `ccptools-1.0.0/ccptools/tpu/insp/_typecheck.py` & `ccptools-1.0.0rc2/ccptools/tpu/insp/_typecheck.py`

 * *Files identical despite different names*

### Comparing `ccptools-1.0.0/ccptools/tpu/iters/_attrs.py` & `ccptools-1.0.0rc2/ccptools/tpu/iters/_attrs.py`

 * *Files identical despite different names*

### Comparing `ccptools-1.0.0/ccptools/tpu/iters/_dicts.py` & `ccptools-1.0.0rc2/ccptools/tpu/iters/_dicts.py`

 * *Files identical despite different names*

### Comparing `ccptools-1.0.0/ccptools/tpu/iters/_group.py` & `ccptools-1.0.0rc2/ccptools/tpu/iters/_group.py`

 * *Files identical despite different names*

### Comparing `ccptools-1.0.0/ccptools/tpu/iters/_lists.py` & `ccptools-1.0.0rc2/ccptools/tpu/iters/_lists.py`

 * *Files identical despite different names*

### Comparing `ccptools-1.0.0/ccptools/tpu/size/_total.py` & `ccptools-1.0.0rc2/ccptools/tpu/size/_total.py`

 * *Files identical despite different names*

### Comparing `ccptools-1.0.0/ccptools/tpu/strimp/_getters.py` & `ccptools-1.0.0rc2/ccptools/tpu/strimp/_getters.py`

 * *Files identical despite different names*

### Comparing `ccptools-1.0.0/ccptools/tpu/string/_string.py` & `ccptools-1.0.0rc2/ccptools/tpu/string/_string.py`

 * *Files identical despite different names*

### Comparing `ccptools-1.0.0/ccptools/tpu/structs/empty/_empty.py` & `ccptools-1.0.0rc2/ccptools/tpu/structs/empty/_empty.py`

 * *Files identical despite different names*

### Comparing `ccptools-1.0.0/ccptools/tpu/structs/fluid/_attrfluid.py` & `ccptools-1.0.0rc2/ccptools/tpu/structs/fluid/_attrfluid.py`

 * *Files identical despite different names*

### Comparing `ccptools-1.0.0/ccptools/tpu/structs/sentience/_builder.py` & `ccptools-1.0.0rc2/ccptools/tpu/structs/sentience/_builder.py`

 * *Files identical despite different names*

### Comparing `ccptools-1.0.0/ccptools/tpu/structs/serializers/_jsonsafe.py` & `ccptools-1.0.0rc2/ccptools/tpu/structs/serializers/_jsonsafe.py`

 * *Files identical despite different names*

### Comparing `ccptools-1.0.0/ccptools/tpu/structs/serializers/_universal.py` & `ccptools-1.0.0rc2/ccptools/tpu/structs/serializers/_universal.py`

 * *Files identical despite different names*

### Comparing `ccptools-1.0.0/ccptools/tpu/structs/singleton/_singleton.py` & `ccptools-1.0.0rc2/ccptools/tpu/structs/singleton/_singleton.py`

 * *Files identical despite different names*

### Comparing `ccptools-1.0.0/ccptools.egg-info/PKG-INFO` & `ccptools-1.0.0rc2/ccptools.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 Metadata-Version: 2.1
 Name: ccptools
-Version: 1.0.0
+Version: 1.0.0rc2
 Summary: The CCP Tools team utilities for date and/or time objects and values and messing with types.
-Author-email: Thordur Matthiasson <thordurm@ccpgames.com>, John Aldis <johnaldis@ccpgames.com>
+Home-page: https://github.com/ccpgames/ccptools
+Author: Thordur Matthiasson
+Author-email: thordurm@ccpgames.com
 License: MIT License
         
         Copyright (c) 2013-2024 CCP Games
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -21,34 +23,21 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: Homepage, https://github.com/ccpgames/ccptools
-Project-URL: Documentation, https://github.com/ccpgames/ccptools/blob/main/README.md
-Project-URL: Repository, https://github.com/ccpgames/ccptools.git
-Project-URL: Issues, https://github.com/ccpgames/ccptools/issues
-Project-URL: Changelog, https://github.com/ccpgames/ccptools/blob/main/CHANGELOG.md
-Keywords: datetimeutils,datetime,typeutils,type,singleton,date,time,timespan,tools,ccp,utils
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CCP Games Python Toolkit
 
 A smooshup of a few Python packages from the CCP Tools Team of old (Team 
 Batcave).
@@ -158,7 +147,8 @@
 
 So in most cases we can cover something like 90% of any imports we tend to 
 need in every Python file with a single line:
 
 ```python
 from ccptools.structs import *
 ```
+
```

