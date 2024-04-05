# Comparing `tmp/xi-mzidentml-converter-0.1.7.tar.gz` & `tmp/xi-mzidentml-converter-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xi-mzidentml-converter-0.1.7.tar", last modified: Wed Jan 24 15:32:28 2024, max compression
+gzip compressed data, was "xi-mzidentml-converter-0.1.9.tar", last modified: Thu Jan 25 14:23:23 2024, max compression
```

## Comparing `xi-mzidentml-converter-0.1.7.tar` & `xi-mzidentml-converter-0.1.9.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 15:32:28.237480 xi-mzidentml-converter-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-01-24 15:32:19.000000 xi-mzidentml-converter-0.1.7/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-01-24 15:32:28.237480 xi-mzidentml-converter-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-01-24 15:32:19.000000 xi-mzidentml-converter-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 15:32:28.229481 xi-mzidentml-converter-0.1.7/app/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-01-24 15:32:19.000000 xi-mzidentml-converter-0.1.7/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 15:32:28.229481 xi-mzidentml-converter-0.1.7/app/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-24 15:32:19.000000 xi-mzidentml-converter-0.1.7/app/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-01-24 15:32:19.000000 xi-mzidentml-converter-0.1.7/app/config/database.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 15:32:28.233481 xi-mzidentml-converter-0.1.7/app/models/
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-01-24 15:32:19.000000 xi-mzidentml-converter-0.1.7/app/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-01-24 15:32:19.000000 xi-mzidentml-converter-0.1.7/app/models/analysiscollection.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-01-24 15:32:19.000000 xi-mzidentml-converter-0.1.7/app/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-01-24 15:32:19.000000 xi-mzidentml-converter-0.1.7/app/models/dbsequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-01-24 15:32:19.000000 xi-mzidentml-converter-0.1.7/app/models/enzyme.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-24 15:32:19.000000 xi-mzidentml-converter-0.1.7/app/models/index.py
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-01-24 15:32:19.000000 xi-mzidentml-converter-0.1.7/app/models/modifiedpeptide.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-01-24 15:32:19.000000 xi-mzidentml-converter-0.1.7/app/models/peptideevidence.py
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-01-24 15:32:19.000000 xi-mzidentml-converter-0.1.7/app/models/projectdetail.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-01-24 15:32:19.000000 xi-mzidentml-converter-0.1.7/app/models/projectsubdetail.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-01-24 15:32:19.000000 xi-mzidentml-converter-0.1.7/app/models/searchmodification.py
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-01-24 15:32:19.000000 xi-mzidentml-converter-0.1.7/app/models/spectrum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-01-24 15:32:19.000000 xi-mzidentml-converter-0.1.7/app/models/spectrumidentification.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-01-24 15:32:19.000000 xi-mzidentml-converter-0.1.7/app/models/spectrumidentificationprotocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-01-24 15:32:19.000000 xi-mzidentml-converter-0.1.7/app/models/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 15:32:28.233481 xi-mzidentml-converter-0.1.7/parser/
--rw-r--r--   0 runner    (1001) docker     (127)    38392 2024-01-24 15:32:19.000000 xi-mzidentml-converter-0.1.7/parser/MzIdParser.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-01-24 15:32:19.000000 xi-mzidentml-converter-0.1.7/parser/NumpyEncoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-01-24 15:32:19.000000 xi-mzidentml-converter-0.1.7/parser/SimpleFASTA.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-01-24 15:32:19.000000 xi-mzidentml-converter-0.1.7/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4915 2024-01-24 15:32:19.000000 xi-mzidentml-converter-0.1.7/parser/api_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 15:32:28.233481 xi-mzidentml-converter-0.1.7/parser/csv_parser/
--rw-r--r--   0 runner    (1001) docker     (127)    10406 2024-01-24 15:32:19.000000 xi-mzidentml-converter-0.1.7/parser/csv_parser/AbstractCsvParser.py
--rw-r--r--   0 runner    (1001) docker     (127)    20658 2024-01-24 15:32:19.000000 xi-mzidentml-converter-0.1.7/parser/csv_parser/FullCsvParser.py
--rw-r--r--   0 runner    (1001) docker     (127)    12587 2024-01-24 15:32:19.000000 xi-mzidentml-converter-0.1.7/parser/csv_parser/LinksOnlyCsvParser.py
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-01-24 15:32:19.000000 xi-mzidentml-converter-0.1.7/parser/csv_parser/NoPeakListsCsvParser.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-24 15:32:19.000000 xi-mzidentml-converter-0.1.7/parser/csv_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-01-24 15:32:19.000000 xi-mzidentml-converter-0.1.7/parser/csv_parser/xiSPEC_CsvParser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 15:32:28.237480 xi-mzidentml-converter-0.1.7/parser/database/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-24 15:32:19.000000 xi-mzidentml-converter-0.1.7/parser/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-01-24 15:32:19.000000 xi-mzidentml-converter-0.1.7/parser/database/guid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-01-24 15:32:19.000000 xi-mzidentml-converter-0.1.7/parser/database/update_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-01-24 15:32:19.000000 xi-mzidentml-converter-0.1.7/parser/database_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 15:32:28.237480 xi-mzidentml-converter-0.1.7/parser/peaklistReader/
--rw-r--r--   0 runner    (1001) docker     (127)    14552 2024-01-24 15:32:19.000000 xi-mzidentml-converter-0.1.7/parser/peaklistReader/PeakListWrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-24 15:32:19.000000 xi-mzidentml-converter-0.1.7/parser/peaklistReader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-01-24 15:32:19.000000 xi-mzidentml-converter-0.1.7/parser/writer.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-24 15:32:28.237480 xi-mzidentml-converter-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-01-24 15:32:19.000000 xi-mzidentml-converter-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 15:32:28.237480 xi-mzidentml-converter-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-24 15:32:19.000000 xi-mzidentml-converter-0.1.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-01-24 15:32:19.000000 xi-mzidentml-converter-0.1.7/tests/compare.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-01-24 15:32:19.000000 xi-mzidentml-converter-0.1.7/tests/db_pytest_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-01-24 15:32:19.000000 xi-mzidentml-converter-0.1.7/tests/parse_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-01-24 15:32:19.000000 xi-mzidentml-converter-0.1.7/tests/parse_mzid.py
--rw-r--r--   0 runner    (1001) docker     (127)    13892 2024-01-24 15:32:19.000000 xi-mzidentml-converter-0.1.7/tests/test_CsvParsers.py
--rw-r--r--   0 runner    (1001) docker     (127)    39992 2024-01-24 15:32:19.000000 xi-mzidentml-converter-0.1.7/tests/test_MzIdParser_ecoli_dsso.py
--rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-01-24 15:32:19.000000 xi-mzidentml-converter-0.1.7/tests/test_MzIdParser_matrixscience.py
--rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-01-24 15:32:19.000000 xi-mzidentml-converter-0.1.7/tests/test_MzIdParser_matrixscience2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-01-24 15:32:19.000000 xi-mzidentml-converter-0.1.7/tests/test_fasta_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 15:32:28.237480 xi-mzidentml-converter-0.1.7/xi_mzidentml_converter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-01-24 15:32:28.000000 xi-mzidentml-converter-0.1.7/xi_mzidentml_converter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-01-24 15:32:28.000000 xi-mzidentml-converter-0.1.7/xi_mzidentml_converter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-24 15:32:28.000000 xi-mzidentml-converter-0.1.7/xi_mzidentml_converter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-01-24 15:32:28.000000 xi-mzidentml-converter-0.1.7/xi_mzidentml_converter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-01-24 15:32:28.000000 xi-mzidentml-converter-0.1.7/xi_mzidentml_converter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-24 15:32:28.000000 xi-mzidentml-converter-0.1.7/xi_mzidentml_converter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 14:23:23.445494 xi-mzidentml-converter-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-01-25 14:23:09.000000 xi-mzidentml-converter-0.1.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-01-25 14:23:23.445494 xi-mzidentml-converter-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-01-25 14:23:09.000000 xi-mzidentml-converter-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 14:23:23.433493 xi-mzidentml-converter-0.1.9/app/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-01-25 14:23:09.000000 xi-mzidentml-converter-0.1.9/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 14:23:23.437494 xi-mzidentml-converter-0.1.9/app/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 14:23:09.000000 xi-mzidentml-converter-0.1.9/app/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-01-25 14:23:09.000000 xi-mzidentml-converter-0.1.9/app/config/database.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 14:23:23.437494 xi-mzidentml-converter-0.1.9/app/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-01-25 14:23:09.000000 xi-mzidentml-converter-0.1.9/app/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-01-25 14:23:09.000000 xi-mzidentml-converter-0.1.9/app/models/analysiscollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-01-25 14:23:09.000000 xi-mzidentml-converter-0.1.9/app/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-01-25 14:23:09.000000 xi-mzidentml-converter-0.1.9/app/models/dbsequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-01-25 14:23:09.000000 xi-mzidentml-converter-0.1.9/app/models/enzyme.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 14:23:09.000000 xi-mzidentml-converter-0.1.9/app/models/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-01-25 14:23:09.000000 xi-mzidentml-converter-0.1.9/app/models/modifiedpeptide.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-01-25 14:23:09.000000 xi-mzidentml-converter-0.1.9/app/models/peptideevidence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-01-25 14:23:09.000000 xi-mzidentml-converter-0.1.9/app/models/projectdetail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-01-25 14:23:09.000000 xi-mzidentml-converter-0.1.9/app/models/projectsubdetail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-01-25 14:23:09.000000 xi-mzidentml-converter-0.1.9/app/models/searchmodification.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-01-25 14:23:09.000000 xi-mzidentml-converter-0.1.9/app/models/spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-01-25 14:23:09.000000 xi-mzidentml-converter-0.1.9/app/models/spectrumidentification.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-01-25 14:23:09.000000 xi-mzidentml-converter-0.1.9/app/models/spectrumidentificationprotocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-01-25 14:23:09.000000 xi-mzidentml-converter-0.1.9/app/models/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 14:23:23.437494 xi-mzidentml-converter-0.1.9/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)    38392 2024-01-25 14:23:09.000000 xi-mzidentml-converter-0.1.9/parser/MzIdParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-01-25 14:23:09.000000 xi-mzidentml-converter-0.1.9/parser/NumpyEncoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-01-25 14:23:09.000000 xi-mzidentml-converter-0.1.9/parser/SimpleFASTA.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-01-25 14:23:09.000000 xi-mzidentml-converter-0.1.9/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4915 2024-01-25 14:23:09.000000 xi-mzidentml-converter-0.1.9/parser/api_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 14:23:23.441494 xi-mzidentml-converter-0.1.9/parser/csv_parser/
+-rw-r--r--   0 runner    (1001) docker     (127)    10406 2024-01-25 14:23:09.000000 xi-mzidentml-converter-0.1.9/parser/csv_parser/AbstractCsvParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20658 2024-01-25 14:23:09.000000 xi-mzidentml-converter-0.1.9/parser/csv_parser/FullCsvParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12587 2024-01-25 14:23:09.000000 xi-mzidentml-converter-0.1.9/parser/csv_parser/LinksOnlyCsvParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-01-25 14:23:09.000000 xi-mzidentml-converter-0.1.9/parser/csv_parser/NoPeakListsCsvParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 14:23:09.000000 xi-mzidentml-converter-0.1.9/parser/csv_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-01-25 14:23:09.000000 xi-mzidentml-converter-0.1.9/parser/csv_parser/xiSPEC_CsvParser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 14:23:23.441494 xi-mzidentml-converter-0.1.9/parser/database/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 14:23:09.000000 xi-mzidentml-converter-0.1.9/parser/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-01-25 14:23:09.000000 xi-mzidentml-converter-0.1.9/parser/database/guid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-01-25 14:23:09.000000 xi-mzidentml-converter-0.1.9/parser/database/update_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-01-25 14:23:09.000000 xi-mzidentml-converter-0.1.9/parser/database_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 14:23:23.441494 xi-mzidentml-converter-0.1.9/parser/peaklistReader/
+-rw-r--r--   0 runner    (1001) docker     (127)    14552 2024-01-25 14:23:09.000000 xi-mzidentml-converter-0.1.9/parser/peaklistReader/PeakListWrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 14:23:09.000000 xi-mzidentml-converter-0.1.9/parser/peaklistReader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-01-25 14:23:09.000000 xi-mzidentml-converter-0.1.9/parser/writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-25 14:23:23.445494 xi-mzidentml-converter-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-01-25 14:23:09.000000 xi-mzidentml-converter-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 14:23:23.441494 xi-mzidentml-converter-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 14:23:09.000000 xi-mzidentml-converter-0.1.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-01-25 14:23:09.000000 xi-mzidentml-converter-0.1.9/tests/compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-01-25 14:23:09.000000 xi-mzidentml-converter-0.1.9/tests/db_pytest_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-01-25 14:23:09.000000 xi-mzidentml-converter-0.1.9/tests/parse_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-01-25 14:23:09.000000 xi-mzidentml-converter-0.1.9/tests/parse_mzid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13892 2024-01-25 14:23:09.000000 xi-mzidentml-converter-0.1.9/tests/test_CsvParsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39992 2024-01-25 14:23:09.000000 xi-mzidentml-converter-0.1.9/tests/test_MzIdParser_ecoli_dsso.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-01-25 14:23:09.000000 xi-mzidentml-converter-0.1.9/tests/test_MzIdParser_matrixscience.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-01-25 14:23:09.000000 xi-mzidentml-converter-0.1.9/tests/test_MzIdParser_matrixscience2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-01-25 14:23:09.000000 xi-mzidentml-converter-0.1.9/tests/test_fasta_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 14:23:23.441494 xi-mzidentml-converter-0.1.9/xi_mzidentml_converter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-01-25 14:23:23.000000 xi-mzidentml-converter-0.1.9/xi_mzidentml_converter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-01-25 14:23:23.000000 xi-mzidentml-converter-0.1.9/xi_mzidentml_converter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-25 14:23:23.000000 xi-mzidentml-converter-0.1.9/xi_mzidentml_converter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-01-25 14:23:23.000000 xi-mzidentml-converter-0.1.9/xi_mzidentml_converter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-01-25 14:23:23.000000 xi-mzidentml-converter-0.1.9/xi_mzidentml_converter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-25 14:23:23.000000 xi-mzidentml-converter-0.1.9/xi_mzidentml_converter.egg-info/top_level.txt
```

### Comparing `xi-mzidentml-converter-0.1.7/LICENSE.md` & `xi-mzidentml-converter-0.1.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `xi-mzidentml-converter-0.1.7/PKG-INFO` & `xi-mzidentml-converter-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xi-mzidentml-converter
-Version: 0.1.7
+Version: 0.1.9
 Summary: xi-mzidentml-converter uses pyteomics (https://pyteomics.readthedocs.io/en/latest/index.html) to parse mzIdentML files (v1.2.0) and extract crosslink information. Results are written to a relational database (PostgreSQL or SQLite) using sqlalchemy.
 Home-page: https://github.com/PRIDE-Archive/xi-mzidentml-converter
 License: 'Apache 2.0
 Keywords: crosslinking python proteomics
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `xi-mzidentml-converter-0.1.7/README.md` & `xi-mzidentml-converter-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `xi-mzidentml-converter-0.1.7/app/models/analysiscollection.py` & `xi-mzidentml-converter-0.1.9/app/models/analysiscollection.py`

 * *Files identical despite different names*

### Comparing `xi-mzidentml-converter-0.1.7/app/models/dbsequence.py` & `xi-mzidentml-converter-0.1.9/app/models/dbsequence.py`

 * *Files identical despite different names*

### Comparing `xi-mzidentml-converter-0.1.7/app/models/enzyme.py` & `xi-mzidentml-converter-0.1.9/app/models/enzyme.py`

 * *Files identical despite different names*

### Comparing `xi-mzidentml-converter-0.1.7/app/models/modifiedpeptide.py` & `xi-mzidentml-converter-0.1.9/app/models/modifiedpeptide.py`

 * *Files identical despite different names*

### Comparing `xi-mzidentml-converter-0.1.7/app/models/peptideevidence.py` & `xi-mzidentml-converter-0.1.9/app/models/peptideevidence.py`

 * *Files identical despite different names*

### Comparing `xi-mzidentml-converter-0.1.7/app/models/projectdetail.py` & `xi-mzidentml-converter-0.1.9/app/models/projectdetail.py`

 * *Files identical despite different names*

### Comparing `xi-mzidentml-converter-0.1.7/app/models/projectsubdetail.py` & `xi-mzidentml-converter-0.1.9/app/models/projectsubdetail.py`

 * *Files identical despite different names*

### Comparing `xi-mzidentml-converter-0.1.7/app/models/searchmodification.py` & `xi-mzidentml-converter-0.1.9/app/models/searchmodification.py`

 * *Files identical despite different names*

### Comparing `xi-mzidentml-converter-0.1.7/app/models/spectrum.py` & `xi-mzidentml-converter-0.1.9/app/models/spectrum.py`

 * *Files identical despite different names*

### Comparing `xi-mzidentml-converter-0.1.7/app/models/spectrumidentification.py` & `xi-mzidentml-converter-0.1.9/app/models/spectrumidentification.py`

 * *Files identical despite different names*

### Comparing `xi-mzidentml-converter-0.1.7/app/models/spectrumidentificationprotocol.py` & `xi-mzidentml-converter-0.1.9/app/models/spectrumidentificationprotocol.py`

 * *Files identical despite different names*

### Comparing `xi-mzidentml-converter-0.1.7/app/models/upload.py` & `xi-mzidentml-converter-0.1.9/app/models/upload.py`

 * *Files identical despite different names*

### Comparing `xi-mzidentml-converter-0.1.7/parser/MzIdParser.py` & `xi-mzidentml-converter-0.1.9/parser/MzIdParser.py`

 * *Files identical despite different names*

### Comparing `xi-mzidentml-converter-0.1.7/parser/SimpleFASTA.py` & `xi-mzidentml-converter-0.1.9/parser/SimpleFASTA.py`

 * *Files identical despite different names*

### Comparing `xi-mzidentml-converter-0.1.7/parser/api_writer.py` & `xi-mzidentml-converter-0.1.9/parser/api_writer.py`

 * *Files identical despite different names*

### Comparing `xi-mzidentml-converter-0.1.7/parser/csv_parser/AbstractCsvParser.py` & `xi-mzidentml-converter-0.1.9/parser/csv_parser/AbstractCsvParser.py`

 * *Files identical despite different names*

### Comparing `xi-mzidentml-converter-0.1.7/parser/csv_parser/FullCsvParser.py` & `xi-mzidentml-converter-0.1.9/parser/csv_parser/FullCsvParser.py`

 * *Files identical despite different names*

### Comparing `xi-mzidentml-converter-0.1.7/parser/csv_parser/LinksOnlyCsvParser.py` & `xi-mzidentml-converter-0.1.9/parser/csv_parser/LinksOnlyCsvParser.py`

 * *Files identical despite different names*

### Comparing `xi-mzidentml-converter-0.1.7/parser/csv_parser/NoPeakListsCsvParser.py` & `xi-mzidentml-converter-0.1.9/parser/csv_parser/NoPeakListsCsvParser.py`

 * *Files identical despite different names*

### Comparing `xi-mzidentml-converter-0.1.7/parser/csv_parser/xiSPEC_CsvParser.py` & `xi-mzidentml-converter-0.1.9/parser/csv_parser/xiSPEC_CsvParser.py`

 * *Files identical despite different names*

### Comparing `xi-mzidentml-converter-0.1.7/parser/database/guid.py` & `xi-mzidentml-converter-0.1.9/parser/database/guid.py`

 * *Files identical despite different names*

### Comparing `xi-mzidentml-converter-0.1.7/parser/database/update_sqlite.py` & `xi-mzidentml-converter-0.1.9/parser/database/update_sqlite.py`

 * *Files identical despite different names*

### Comparing `xi-mzidentml-converter-0.1.7/parser/database_writer.py` & `xi-mzidentml-converter-0.1.9/parser/database_writer.py`

 * *Files identical despite different names*

### Comparing `xi-mzidentml-converter-0.1.7/parser/peaklistReader/PeakListWrapper.py` & `xi-mzidentml-converter-0.1.9/parser/peaklistReader/PeakListWrapper.py`

 * *Files identical despite different names*

### Comparing `xi-mzidentml-converter-0.1.7/parser/writer.py` & `xi-mzidentml-converter-0.1.9/parser/writer.py`

 * *Files identical despite different names*

### Comparing `xi-mzidentml-converter-0.1.7/setup.py` & `xi-mzidentml-converter-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `xi-mzidentml-converter-0.1.7/tests/compare.py` & `xi-mzidentml-converter-0.1.9/tests/compare.py`

 * *Files identical despite different names*

### Comparing `xi-mzidentml-converter-0.1.7/tests/db_pytest_fixtures.py` & `xi-mzidentml-converter-0.1.9/tests/db_pytest_fixtures.py`

 * *Files identical despite different names*

### Comparing `xi-mzidentml-converter-0.1.7/tests/parse_csv.py` & `xi-mzidentml-converter-0.1.9/tests/parse_csv.py`

 * *Files identical despite different names*

### Comparing `xi-mzidentml-converter-0.1.7/tests/parse_mzid.py` & `xi-mzidentml-converter-0.1.9/tests/parse_mzid.py`

 * *Files identical despite different names*

### Comparing `xi-mzidentml-converter-0.1.7/tests/test_CsvParsers.py` & `xi-mzidentml-converter-0.1.9/tests/test_CsvParsers.py`

 * *Files identical despite different names*

### Comparing `xi-mzidentml-converter-0.1.7/tests/test_MzIdParser_ecoli_dsso.py` & `xi-mzidentml-converter-0.1.9/tests/test_MzIdParser_ecoli_dsso.py`

 * *Files identical despite different names*

### Comparing `xi-mzidentml-converter-0.1.7/tests/test_MzIdParser_matrixscience.py` & `xi-mzidentml-converter-0.1.9/tests/test_MzIdParser_matrixscience.py`

 * *Files identical despite different names*

### Comparing `xi-mzidentml-converter-0.1.7/tests/test_MzIdParser_matrixscience2.py` & `xi-mzidentml-converter-0.1.9/tests/test_MzIdParser_matrixscience2.py`

 * *Files identical despite different names*

### Comparing `xi-mzidentml-converter-0.1.7/tests/test_fasta_reader.py` & `xi-mzidentml-converter-0.1.9/tests/test_fasta_reader.py`

 * *Files identical despite different names*

### Comparing `xi-mzidentml-converter-0.1.7/xi_mzidentml_converter.egg-info/PKG-INFO` & `xi-mzidentml-converter-0.1.9/xi_mzidentml_converter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xi-mzidentml-converter
-Version: 0.1.7
+Version: 0.1.9
 Summary: xi-mzidentml-converter uses pyteomics (https://pyteomics.readthedocs.io/en/latest/index.html) to parse mzIdentML files (v1.2.0) and extract crosslink information. Results are written to a relational database (PostgreSQL or SQLite) using sqlalchemy.
 Home-page: https://github.com/PRIDE-Archive/xi-mzidentml-converter
 License: 'Apache 2.0
 Keywords: crosslinking python proteomics
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `xi-mzidentml-converter-0.1.7/xi_mzidentml_converter.egg-info/SOURCES.txt` & `xi-mzidentml-converter-0.1.9/xi_mzidentml_converter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

