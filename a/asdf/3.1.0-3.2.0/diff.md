# Comparing `tmp/asdf-3.1.0.tar.gz` & `tmp/asdf-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asdf-3.1.0.tar", last modified: Tue Feb 27 20:49:49 2024, max compression
+gzip compressed data, was "asdf-3.2.0.tar", last modified: Fri Apr  5 16:10:13 2024, max compression
```

## Comparing `asdf-3.1.0.tar` & `asdf-3.2.0.tar`

### file list

```diff
@@ -1,979 +1,980 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.780959 asdf-3.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.624958 asdf-3.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-02-27 20:49:34.000000 asdf-3.1.0/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-02-27 20:49:34.000000 asdf-3.1.0/.github/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-02-27 20:49:34.000000 asdf-3.1.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-02-27 20:49:34.000000 asdf-3.1.0/.github/issue_template.md
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-02-27 20:49:34.000000 asdf-3.1.0/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.624958 asdf-3.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-02-27 20:49:34.000000 asdf-3.1.0/.github/workflows/changelog.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4141 2024-02-27 20:49:34.000000 asdf-3.1.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-02-27 20:49:34.000000 asdf-3.1.0/.github/workflows/downstream.yml
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-02-27 20:49:34.000000 asdf-3.1.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-02-27 20:49:34.000000 asdf-3.1.0/.github/workflows/s390x.yml
--rw-r--r--   0 runner    (1001) docker     (127)    34653 2024-02-27 20:49:34.000000 asdf-3.1.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-02-27 20:49:34.000000 asdf-3.1.0/CITATION.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-02-27 20:49:34.000000 asdf-3.1.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-02-27 20:49:34.000000 asdf-3.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-02-27 20:49:34.000000 asdf-3.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    14620 2024-02-27 20:49:49.780959 asdf-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11051 2024-02-27 20:49:34.000000 asdf-3.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.632958 asdf-3.1.0/asdf/
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    59908 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_asdf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.632958 asdf-3.1.0/asdf/_block/
--rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_block/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_block/callback.py
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_block/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_block/external.py
--rw-r--r--   0 runner    (1001) docker     (127)    16493 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_block/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_block/key.py
--rw-r--r--   0 runner    (1001) docker     (127)    25629 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_block/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_block/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     9360 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_block/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_block/store.py
--rw-r--r--   0 runner    (1001) docker     (127)     4012 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_block/writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10595 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_compression.py
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_convenience.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.636958 asdf-3.1.0/asdf/_core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.636958 asdf-3.1.0/asdf/_core/_converters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_core/_converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_core/_converters/complex.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_core/_converters/constant.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_core/_converters/external_reference.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_core/_converters/integer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7209 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_core/_converters/ndarray.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_core/_converters/reference.py
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_core/_converters/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_core/_extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_core/_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.636958 asdf-3.1.0/asdf/_core/_validators/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_core/_validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_core/_validators/ndarray.py
--rw-r--r--   0 runner    (1001) docker     (127)     9122 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_display.py
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_entry_points.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.636958 asdf-3.1.0/asdf/_extern/
--rwxr-xr-x   0 runner    (1001) docker     (127)     7095 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_extern/RangeHTTPServer.py
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_extern/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_extern/atomicfile.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.640958 asdf-3.1.0/asdf/_jsonschema/
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14587 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/_format.py
--rw-r--r--   0 runner    (1001) docker     (127)    10561 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/_legacy_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    10429 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15968 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.640958 asdf-3.1.0/asdf/_jsonschema/json/
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16971 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.640958 asdf-3.1.0/asdf/_jsonschema/json/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)    11731 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/bin/jsonschema_suite
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.644958 asdf-3.1.0/asdf/_jsonschema/json/remotes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.644958 asdf-3.1.0/asdf/_jsonschema/json/remotes/baseUriChange/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/baseUriChange/folderInteger.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.644958 asdf-3.1.0/asdf/_jsonschema/json/remotes/baseUriChangeFolder/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/baseUriChangeFolder/folderInteger.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.644958 asdf-3.1.0/asdf/_jsonschema/json/remotes/baseUriChangeFolderInSubschema/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/baseUriChangeFolderInSubschema/folderInteger.json
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/different-id-ref-string.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.644958 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft-next/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.644958 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft-next/baseUriChange/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft-next/baseUriChange/folderInteger.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.644958 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft-next/baseUriChangeFolder/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft-next/baseUriChangeFolder/folderInteger.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.644958 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft-next/baseUriChangeFolderInSubschema/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft-next/baseUriChangeFolderInSubschema/folderInteger.json
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft-next/extendible-dynamic-ref.json
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft-next/format-assertion-false.json
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft-next/format-assertion-true.json
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft-next/integer.json
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft-next/locationIndependentIdentifier.json
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft-next/metaschema-no-validation.json
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft-next/name-defs.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.644958 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft-next/nested/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft-next/nested/foo-ref-string.json
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft-next/nested/string.json
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft-next/ref-and-defs.json
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft-next/subSchemas-defs.json
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft-next/subSchemas.json
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft-next/tree.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.648958 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft2019-09/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.648958 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft2019-09/baseUriChange/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft2019-09/baseUriChange/folderInteger.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.648958 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft2019-09/baseUriChangeFolder/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft2019-09/baseUriChangeFolder/folderInteger.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.648958 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft2019-09/baseUriChangeFolderInSubschema/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft2019-09/baseUriChangeFolderInSubschema/folderInteger.json
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft2019-09/dependentRequired.json
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft2019-09/extendible-dynamic-ref.json
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft2019-09/ignore-prefixItems.json
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft2019-09/integer.json
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft2019-09/locationIndependentIdentifier.json
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft2019-09/metaschema-no-validation.json
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft2019-09/name-defs.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.648958 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft2019-09/nested/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft2019-09/nested/foo-ref-string.json
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft2019-09/nested/string.json
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft2019-09/ref-and-defs.json
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft2019-09/subSchemas-defs.json
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft2019-09/subSchemas.json
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft2019-09/tree.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.652958 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft2020-12/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.652958 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft2020-12/baseUriChange/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft2020-12/baseUriChange/folderInteger.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.652958 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft2020-12/baseUriChangeFolder/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft2020-12/baseUriChangeFolder/folderInteger.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.652958 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft2020-12/baseUriChangeFolderInSubschema/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft2020-12/baseUriChangeFolderInSubschema/folderInteger.json
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft2020-12/extendible-dynamic-ref.json
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft2020-12/format-assertion-false.json
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft2020-12/format-assertion-true.json
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft2020-12/integer.json
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft2020-12/locationIndependentIdentifier.json
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft2020-12/metaschema-no-validation.json
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft2020-12/name-defs.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.652958 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft2020-12/nested/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft2020-12/nested/foo-ref-string.json
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft2020-12/nested/string.json
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft2020-12/prefixItems.json
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft2020-12/ref-and-defs.json
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft2020-12/subSchemas-defs.json
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft2020-12/subSchemas.json
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft2020-12/tree.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.652958 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft7/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/draft7/ignore-dependentRequired.json
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/extendible-dynamic-ref.json
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/integer.json
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/locationIndependentIdentifier.json
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/locationIndependentIdentifierDraft4.json
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/locationIndependentIdentifierPre2019.json
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/name-defs.json
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/name.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.652958 asdf-3.1.0/asdf/_jsonschema/json/remotes/nested/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/nested/foo-ref-string.json
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/nested/string.json
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/nested-absolute-ref-to-string.json
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/ref-and-definitions.json
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/ref-and-defs.json
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/subSchemas-defs.json
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/subSchemas.json
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/tree.json
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/remotes/urn-ref-string.json
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/test-schema.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.616958 asdf-3.1.0/asdf/_jsonschema/json/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.660958 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/
--rw-r--r--   0 runner    (1001) docker     (127)     4924 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/additionalProperties.json
--rw-r--r--   0 runner    (1001) docker     (127)     8665 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/allOf.json
--rw-r--r--   0 runner    (1001) docker     (127)     7136 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/anchor.json
--rw-r--r--   0 runner    (1001) docker     (127)     5437 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/anyOf.json
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/boolean_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)    10936 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/const.json
--rw-r--r--   0 runner    (1001) docker     (127)     8424 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/contains.json
--rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/content.json
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/default.json
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/defs.json
--rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/dependentRequired.json
--rw-r--r--   0 runner    (1001) docker     (127)     3862 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/dependentSchemas.json
--rw-r--r--   0 runner    (1001) docker     (127)    19268 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/dynamicRef.json
--rw-r--r--   0 runner    (1001) docker     (127)     7415 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/enum.json
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/exclusiveMaximum.json
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/exclusiveMinimum.json
--rw-r--r--   0 runner    (1001) docker     (127)    21855 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/format.json
--rw-r--r--   0 runner    (1001) docker     (127)    10224 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/id.json
--rw-r--r--   0 runner    (1001) docker     (127)     7546 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/if-then-else.json
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/infinite-loop-detection.json
--rw-r--r--   0 runner    (1001) docker     (127)     8609 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/items.json
--rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/maxContains.json
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/maxItems.json
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/maxLength.json
--rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/maxProperties.json
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/maximum.json
--rw-r--r--   0 runner    (1001) docker     (127)     6551 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/minContains.json
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/minItems.json
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/minLength.json
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/minProperties.json
--rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/minimum.json
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/multipleOf.json
--rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/not.json
--rw-r--r--   0 runner    (1001) docker     (127)     8087 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/oneOf.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.664958 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/optional/
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/optional/bignum.json
--rw-r--r--   0 runner    (1001) docker     (127)     8123 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/optional/dependencies-compatibility.json
--rw-r--r--   0 runner    (1001) docker     (127)    20388 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/optional/ecmascript-regex.json
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/optional/float-overflow.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.668958 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/optional/format/
--rw-r--r--   0 runner    (1001) docker     (127)     4744 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/optional/format/date-time.json
--rw-r--r--   0 runner    (1001) docker     (127)     7536 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/optional/format/date.json
--rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/optional/format/duration.json
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/optional/format/email.json
--rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/optional/format/hostname.json
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/optional/format/idn-email.json
--rw-r--r--   0 runner    (1001) docker     (127)    14841 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/optional/format/idn-hostname.json
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/optional/format/ipv4.json
--rw-r--r--   0 runner    (1001) docker     (127)     7031 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/optional/format/ipv6.json
--rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/optional/format/iri-reference.json
--rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/optional/format/iri.json
--rw-r--r--   0 runner    (1001) docker     (127)     6795 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/optional/format/json-pointer.json
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/optional/format/regex.json
--rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/optional/format/relative-json-pointer.json
--rw-r--r--   0 runner    (1001) docker     (127)     7374 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/optional/format/time.json
--rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/optional/format/uri-reference.json
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/optional/format/uri-template.json
--rw-r--r--   0 runner    (1001) docker     (127)     4724 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/optional/format/uri.json
--rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/optional/format/uuid.json
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/optional/format-assertion.json
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/optional/non-bmp-regex.json
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/optional/refOfUnknownKeyword.json
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/pattern.json
--rw-r--r--   0 runner    (1001) docker     (127)     5517 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/patternProperties.json
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/prefixItems.json
--rw-r--r--   0 runner    (1001) docker     (127)     7713 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/properties.json
--rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/propertyDependencies.json
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/propertyNames.json
--rw-r--r--   0 runner    (1001) docker     (127)    27406 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/ref.json
--rw-r--r--   0 runner    (1001) docker     (127)     8801 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/refRemote.json
--rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/required.json
--rw-r--r--   0 runner    (1001) docker     (127)    14332 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/type.json
--rw-r--r--   0 runner    (1001) docker     (127)    19715 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/unevaluatedItems.json
--rw-r--r--   0 runner    (1001) docker     (127)    45112 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/unevaluatedProperties.json
--rw-r--r--   0 runner    (1001) docker     (127)    14246 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/uniqueItems.json
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/unknownKeyword.json
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/vocabulary.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.676958 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/
--rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/additionalItems.json
--rw-r--r--   0 runner    (1001) docker     (127)     4945 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/additionalProperties.json
--rw-r--r--   0 runner    (1001) docker     (127)     8701 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/allOf.json
--rw-r--r--   0 runner    (1001) docker     (127)     7206 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/anchor.json
--rw-r--r--   0 runner    (1001) docker     (127)     5461 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/anyOf.json
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/boolean_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)    10981 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/const.json
--rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/contains.json
--rw-r--r--   0 runner    (1001) docker     (127)     4397 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/content.json
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/default.json
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/defs.json
--rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/dependentRequired.json
--rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/dependentSchemas.json
--rw-r--r--   0 runner    (1001) docker     (127)     7445 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/enum.json
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/exclusiveMaximum.json
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/exclusiveMinimum.json
--rw-r--r--   0 runner    (1001) docker     (127)    21912 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/format.json
--rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/id.json
--rw-r--r--   0 runner    (1001) docker     (127)     7576 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/if-then-else.json
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/infinite-loop-detection.json
--rw-r--r--   0 runner    (1001) docker     (127)     8723 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/items.json
--rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/maxContains.json
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/maxItems.json
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/maxLength.json
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/maxProperties.json
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/maximum.json
--rw-r--r--   0 runner    (1001) docker     (127)     6624 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/minContains.json
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/minItems.json
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/minLength.json
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/minProperties.json
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/minimum.json
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/multipleOf.json
--rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/not.json
--rw-r--r--   0 runner    (1001) docker     (127)     8120 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/oneOf.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.676958 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/optional/
--rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/optional/bignum.json
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/optional/cross-draft.json
--rw-r--r--   0 runner    (1001) docker     (127)     8144 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/optional/dependencies-compatibility.json
--rw-r--r--   0 runner    (1001) docker     (127)    20017 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/optional/ecmascript-regex.json
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/optional/float-overflow.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.680958 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/
--rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/date-time.json
--rw-r--r--   0 runner    (1001) docker     (127)     7539 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/date.json
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/duration.json
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/email.json
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/hostname.json
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/idn-email.json
--rw-r--r--   0 runner    (1001) docker     (127)    14844 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/idn-hostname.json
--rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/ipv4.json
--rw-r--r--   0 runner    (1001) docker     (127)     7034 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/ipv6.json
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/iri-reference.json
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/iri.json
--rw-r--r--   0 runner    (1001) docker     (127)     6798 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/json-pointer.json
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/regex.json
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/relative-json-pointer.json
--rw-r--r--   0 runner    (1001) docker     (127)     7377 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/time.json
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/unknown.json
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/uri-reference.json
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/uri-template.json
--rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/uri.json
--rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/uuid.json
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/optional/no-schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/optional/non-bmp-regex.json
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/optional/refOfUnknownKeyword.json
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/pattern.json
--rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/patternProperties.json
--rw-r--r--   0 runner    (1001) docker     (127)     7731 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/properties.json
--rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/propertyNames.json
--rw-r--r--   0 runner    (1001) docker     (127)    14068 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/recursiveRef.json
--rw-r--r--   0 runner    (1001) docker     (127)    27548 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/ref.json
--rw-r--r--   0 runner    (1001) docker     (127)     8851 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/refRemote.json
--rw-r--r--   0 runner    (1001) docker     (127)     4627 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/required.json
--rw-r--r--   0 runner    (1001) docker     (127)    14365 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/type.json
--rw-r--r--   0 runner    (1001) docker     (127)    16095 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/unevaluatedItems.json
--rw-r--r--   0 runner    (1001) docker     (127)    42268 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/unevaluatedProperties.json
--rw-r--r--   0 runner    (1001) docker     (127)    14260 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/uniqueItems.json
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/unknownKeyword.json
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/vocabulary.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.688958 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/
--rw-r--r--   0 runner    (1001) docker     (127)     4945 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/additionalProperties.json
--rw-r--r--   0 runner    (1001) docker     (127)     8701 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/allOf.json
--rw-r--r--   0 runner    (1001) docker     (127)     7206 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/anchor.json
--rw-r--r--   0 runner    (1001) docker     (127)     5461 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/anyOf.json
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/boolean_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)    10981 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/const.json
--rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/contains.json
--rw-r--r--   0 runner    (1001) docker     (127)     4397 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/content.json
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/default.json
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/defs.json
--rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/dependentRequired.json
--rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/dependentSchemas.json
--rw-r--r--   0 runner    (1001) docker     (127)    21588 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/dynamicRef.json
--rw-r--r--   0 runner    (1001) docker     (127)     7445 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/enum.json
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/exclusiveMaximum.json
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/exclusiveMinimum.json
--rw-r--r--   0 runner    (1001) docker     (127)    21912 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/format.json
--rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/id.json
--rw-r--r--   0 runner    (1001) docker     (127)     7576 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/if-then-else.json
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/infinite-loop-detection.json
--rw-r--r--   0 runner    (1001) docker     (127)     8636 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/items.json
--rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/maxContains.json
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/maxItems.json
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/maxLength.json
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/maxProperties.json
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/maximum.json
--rw-r--r--   0 runner    (1001) docker     (127)     6604 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/minContains.json
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/minItems.json
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/minLength.json
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/minProperties.json
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/minimum.json
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/multipleOf.json
--rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/not.json
--rw-r--r--   0 runner    (1001) docker     (127)     8120 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/oneOf.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.688958 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/optional/
--rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/optional/bignum.json
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/optional/cross-draft.json
--rw-r--r--   0 runner    (1001) docker     (127)     8144 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/optional/dependencies-compatibility.json
--rw-r--r--   0 runner    (1001) docker     (127)    20454 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/optional/ecmascript-regex.json
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/optional/float-overflow.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.692958 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/
--rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/date-time.json
--rw-r--r--   0 runner    (1001) docker     (127)     7539 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/date.json
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/duration.json
--rw-r--r--   0 runner    (1001) docker     (127)     4052 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/email.json
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/hostname.json
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/idn-email.json
--rw-r--r--   0 runner    (1001) docker     (127)    14844 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/idn-hostname.json
--rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/ipv4.json
--rw-r--r--   0 runner    (1001) docker     (127)     7034 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/ipv6.json
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/iri-reference.json
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/iri.json
--rw-r--r--   0 runner    (1001) docker     (127)     6798 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/json-pointer.json
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/regex.json
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/relative-json-pointer.json
--rw-r--r--   0 runner    (1001) docker     (127)     7377 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/time.json
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/unknown.json
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/uri-reference.json
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/uri-template.json
--rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/uri.json
--rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/uuid.json
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format-assertion.json
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/optional/no-schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/optional/non-bmp-regex.json
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/optional/refOfUnknownKeyword.json
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/pattern.json
--rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/patternProperties.json
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/prefixItems.json
--rw-r--r--   0 runner    (1001) docker     (127)     7731 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/properties.json
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/propertyNames.json
--rw-r--r--   0 runner    (1001) docker     (127)    27508 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/ref.json
--rw-r--r--   0 runner    (1001) docker     (127)     8851 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/refRemote.json
--rw-r--r--   0 runner    (1001) docker     (127)     4627 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/required.json
--rw-r--r--   0 runner    (1001) docker     (127)    14365 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/type.json
--rw-r--r--   0 runner    (1001) docker     (127)    19784 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/unevaluatedItems.json
--rw-r--r--   0 runner    (1001) docker     (127)    42268 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/unevaluatedProperties.json
--rw-r--r--   0 runner    (1001) docker     (127)    14264 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/uniqueItems.json
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/unknownKeyword.json
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/vocabulary.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.696958 asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/
--rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/additionalItems.json
--rw-r--r--   0 runner    (1001) docker     (127)     4430 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/additionalProperties.json
--rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/default.json
--rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/dependencies.json
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/disallow.json
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/divisibleBy.json
--rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/enum.json
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/extends.json
--rw-r--r--   0 runner    (1001) docker     (127)    10579 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/format.json
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/infinite-loop-detection.json
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/items.json
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/maxItems.json
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/maxLength.json
--rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/maximum.json
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/minItems.json
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/minLength.json
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/minimum.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.696958 asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/optional/
--rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/optional/bignum.json
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/optional/ecmascript-regex.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.700958 asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/optional/format/
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/optional/format/color.json
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/optional/format/date-time.json
--rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/optional/format/date.json
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/optional/format/email.json
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/optional/format/host-name.json
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/optional/format/ip-address.json
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/optional/format/ipv6.json
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/optional/format/regex.json
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/optional/format/time.json
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/optional/format/uri.json
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/optional/non-bmp-regex.json
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/optional/zeroTerminatedFloats.json
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/pattern.json
--rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/patternProperties.json
--rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/properties.json
--rw-r--r--   0 runner    (1001) docker     (127)     8112 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/ref.json
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/refRemote.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/required.json
--rw-r--r--   0 runner    (1001) docker     (127)    13876 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/type.json
--rw-r--r--   0 runner    (1001) docker     (127)    12787 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/uniqueItems.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.704958 asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/
--rw-r--r--   0 runner    (1001) docker     (127)     4711 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/additionalItems.json
--rw-r--r--   0 runner    (1001) docker     (127)     4426 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/additionalProperties.json
--rw-r--r--   0 runner    (1001) docker     (127)     6901 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/allOf.json
--rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/anyOf.json
--rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/default.json
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/definitions.json
--rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/dependencies.json
--rw-r--r--   0 runner    (1001) docker     (127)     6563 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/enum.json
--rw-r--r--   0 runner    (1001) docker     (127)     6345 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/format.json
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/id.json
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/infinite-loop-detection.json
--rw-r--r--   0 runner    (1001) docker     (127)     6564 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/items.json
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/maxItems.json
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/maxLength.json
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/maxProperties.json
--rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/maximum.json
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/minItems.json
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/minLength.json
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/minProperties.json
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/minimum.json
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/multipleOf.json
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/not.json
--rw-r--r--   0 runner    (1001) docker     (127)     6035 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/oneOf.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.704958 asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/optional/
--rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/optional/bignum.json
--rw-r--r--   0 runner    (1001) docker     (127)    18487 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/optional/ecmascript-regex.json
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/optional/float-overflow.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.708958 asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/optional/format/
--rw-r--r--   0 runner    (1001) docker     (127)     4656 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/optional/format/date-time.json
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/optional/format/email.json
--rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/optional/format/hostname.json
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/optional/format/ipv4.json
--rw-r--r--   0 runner    (1001) docker     (127)     6943 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/optional/format/ipv6.json
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/optional/format/unknown.json
--rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/optional/format/uri.json
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/optional/non-bmp-regex.json
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/optional/zeroTerminatedFloats.json
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/pattern.json
--rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/patternProperties.json
--rw-r--r--   0 runner    (1001) docker     (127)     6413 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/properties.json
--rw-r--r--   0 runner    (1001) docker     (127)    14935 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/ref.json
--rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/refRemote.json
--rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/required.json
--rw-r--r--   0 runner    (1001) docker     (127)    13221 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/type.json
--rw-r--r--   0 runner    (1001) docker     (127)    13792 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/uniqueItems.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.712958 asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/
--rw-r--r--   0 runner    (1001) docker     (127)     4711 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/additionalItems.json
--rw-r--r--   0 runner    (1001) docker     (127)     4426 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/additionalProperties.json
--rw-r--r--   0 runner    (1001) docker     (127)     7783 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/allOf.json
--rw-r--r--   0 runner    (1001) docker     (127)     4827 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/anyOf.json
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/boolean_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     9588 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/const.json
--rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/contains.json
--rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/default.json
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/definitions.json
--rw-r--r--   0 runner    (1001) docker     (127)     6876 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/dependencies.json
--rw-r--r--   0 runner    (1001) docker     (127)     6563 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/enum.json
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/exclusiveMaximum.json
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/exclusiveMinimum.json
--rw-r--r--   0 runner    (1001) docker     (127)     9557 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/format.json
--rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/id.json
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/infinite-loop-detection.json
--rw-r--r--   0 runner    (1001) docker     (127)     8076 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/items.json
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/maxItems.json
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/maxLength.json
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/maxProperties.json
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/maximum.json
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/minItems.json
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/minLength.json
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/minProperties.json
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/minimum.json
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/multipleOf.json
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/not.json
--rw-r--r--   0 runner    (1001) docker     (127)     7251 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/oneOf.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.716958 asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/optional/
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/optional/bignum.json
--rw-r--r--   0 runner    (1001) docker     (127)    18497 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/optional/ecmascript-regex.json
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/optional/float-overflow.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.716958 asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/optional/format/
--rw-r--r--   0 runner    (1001) docker     (127)     4656 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/optional/format/date-time.json
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/optional/format/email.json
--rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/optional/format/hostname.json
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/optional/format/ipv4.json
--rw-r--r--   0 runner    (1001) docker     (127)     6943 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/optional/format/ipv6.json
--rw-r--r--   0 runner    (1001) docker     (127)     6707 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/optional/format/json-pointer.json
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/optional/format/unknown.json
--rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/optional/format/uri-reference.json
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/optional/format/uri-template.json
--rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/optional/format/uri.json
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/optional/non-bmp-regex.json
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/pattern.json
--rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/patternProperties.json
--rw-r--r--   0 runner    (1001) docker     (127)     7305 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/properties.json
--rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/propertyNames.json
--rw-r--r--   0 runner    (1001) docker     (127)    23343 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/ref.json
--rw-r--r--   0 runner    (1001) docker     (127)     6688 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/refRemote.json
--rw-r--r--   0 runner    (1001) docker     (127)     4252 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/required.json
--rw-r--r--   0 runner    (1001) docker     (127)    13408 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/type.json
--rw-r--r--   0 runner    (1001) docker     (127)    13792 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/uniqueItems.json
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/unknownKeyword.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.724959 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/
--rw-r--r--   0 runner    (1001) docker     (127)     4711 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/additionalItems.json
--rw-r--r--   0 runner    (1001) docker     (127)     4426 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/additionalProperties.json
--rw-r--r--   0 runner    (1001) docker     (127)     7783 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/allOf.json
--rw-r--r--   0 runner    (1001) docker     (127)     4827 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/anyOf.json
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/boolean_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     9588 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/const.json
--rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/contains.json
--rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/default.json
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/definitions.json
--rw-r--r--   0 runner    (1001) docker     (127)     6876 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/dependencies.json
--rw-r--r--   0 runner    (1001) docker     (127)     6563 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/enum.json
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/exclusiveMaximum.json
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/exclusiveMinimum.json
--rw-r--r--   0 runner    (1001) docker     (127)    18067 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/format.json
--rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/id.json
--rw-r--r--   0 runner    (1001) docker     (127)     6866 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/if-then-else.json
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/infinite-loop-detection.json
--rw-r--r--   0 runner    (1001) docker     (127)     8076 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/items.json
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/maxItems.json
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/maxLength.json
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/maxProperties.json
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/maximum.json
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/minItems.json
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/minLength.json
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/minProperties.json
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/minimum.json
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/multipleOf.json
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/not.json
--rw-r--r--   0 runner    (1001) docker     (127)     7251 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/oneOf.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.724959 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/optional/
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/optional/bignum.json
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/optional/content.json
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/optional/cross-draft.json
--rw-r--r--   0 runner    (1001) docker     (127)    18497 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/optional/ecmascript-regex.json
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/optional/float-overflow.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.728959 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/optional/format/
--rw-r--r--   0 runner    (1001) docker     (127)     4656 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/optional/format/date-time.json
--rw-r--r--   0 runner    (1001) docker     (127)     7448 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/optional/format/date.json
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/optional/format/email.json
--rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/optional/format/hostname.json
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/optional/format/idn-email.json
--rw-r--r--   0 runner    (1001) docker     (127)    14753 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/optional/format/idn-hostname.json
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/optional/format/ipv4.json
--rw-r--r--   0 runner    (1001) docker     (127)     6943 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/optional/format/ipv6.json
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/optional/format/iri-reference.json
--rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/optional/format/iri.json
--rw-r--r--   0 runner    (1001) docker     (127)     6707 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/optional/format/json-pointer.json
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/optional/format/regex.json
--rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/optional/format/relative-json-pointer.json
--rw-r--r--   0 runner    (1001) docker     (127)     7286 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/optional/format/time.json
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/optional/format/unknown.json
--rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/optional/format/uri-reference.json
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/optional/format/uri-template.json
--rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/optional/format/uri.json
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/optional/non-bmp-regex.json
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/pattern.json
--rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/patternProperties.json
--rw-r--r--   0 runner    (1001) docker     (127)     7305 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/properties.json
--rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/propertyNames.json
--rw-r--r--   0 runner    (1001) docker     (127)    24396 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/ref.json
--rw-r--r--   0 runner    (1001) docker     (127)     6688 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/refRemote.json
--rw-r--r--   0 runner    (1001) docker     (127)     4252 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/required.json
--rw-r--r--   0 runner    (1001) docker     (127)    13408 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/type.json
--rw-r--r--   0 runner    (1001) docker     (127)    13792 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/uniqueItems.json
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/unknownKeyword.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.736959 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/
--rw-r--r--   0 runner    (1001) docker     (127)     4945 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/additionalProperties.json
--rw-r--r--   0 runner    (1001) docker     (127)     8701 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/allOf.json
--rw-r--r--   0 runner    (1001) docker     (127)     7206 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/anchor.json
--rw-r--r--   0 runner    (1001) docker     (127)     5461 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/anyOf.json
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/boolean_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)    10981 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/const.json
--rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/contains.json
--rw-r--r--   0 runner    (1001) docker     (127)     4397 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/content.json
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/default.json
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/defs.json
--rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/dependentRequired.json
--rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/dependentSchemas.json
--rw-r--r--   0 runner    (1001) docker     (127)    21588 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/dynamicRef.json
--rw-r--r--   0 runner    (1001) docker     (127)     7445 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/enum.json
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/exclusiveMaximum.json
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/exclusiveMinimum.json
--rw-r--r--   0 runner    (1001) docker     (127)    21912 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/format.json
--rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/id.json
--rw-r--r--   0 runner    (1001) docker     (127)     7576 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/if-then-else.json
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/infinite-loop-detection.json
--rw-r--r--   0 runner    (1001) docker     (127)     8636 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/items.json
--rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/maxContains.json
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/maxItems.json
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/maxLength.json
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/maxProperties.json
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/maximum.json
--rw-r--r--   0 runner    (1001) docker     (127)     6604 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/minContains.json
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/minItems.json
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/minLength.json
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/minProperties.json
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/minimum.json
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/multipleOf.json
--rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/not.json
--rw-r--r--   0 runner    (1001) docker     (127)     8120 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/oneOf.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.736959 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/optional/
--rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/optional/bignum.json
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/optional/cross-draft.json
--rw-r--r--   0 runner    (1001) docker     (127)     8144 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/optional/dependencies-compatibility.json
--rw-r--r--   0 runner    (1001) docker     (127)    20454 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/optional/ecmascript-regex.json
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/optional/float-overflow.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.740959 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/optional/format/
--rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/optional/format/date-time.json
--rw-r--r--   0 runner    (1001) docker     (127)     7539 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/optional/format/date.json
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/optional/format/duration.json
--rw-r--r--   0 runner    (1001) docker     (127)     4052 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/optional/format/email.json
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/optional/format/hostname.json
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/optional/format/idn-email.json
--rw-r--r--   0 runner    (1001) docker     (127)    14844 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/optional/format/idn-hostname.json
--rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/optional/format/ipv4.json
--rw-r--r--   0 runner    (1001) docker     (127)     7034 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/optional/format/ipv6.json
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/optional/format/iri-reference.json
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/optional/format/iri.json
--rw-r--r--   0 runner    (1001) docker     (127)     6798 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/optional/format/json-pointer.json
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/optional/format/regex.json
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/optional/format/relative-json-pointer.json
--rw-r--r--   0 runner    (1001) docker     (127)     7377 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/optional/format/time.json
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/optional/format/unknown.json
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/optional/format/uri-reference.json
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/optional/format/uri-template.json
--rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/optional/format/uri.json
--rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/optional/format/uuid.json
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/optional/format-assertion.json
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/optional/no-schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/optional/non-bmp-regex.json
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/optional/refOfUnknownKeyword.json
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/pattern.json
--rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/patternProperties.json
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/prefixItems.json
--rw-r--r--   0 runner    (1001) docker     (127)     7731 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/properties.json
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/propertyNames.json
--rw-r--r--   0 runner    (1001) docker     (127)    27508 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/ref.json
--rw-r--r--   0 runner    (1001) docker     (127)     8851 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/refRemote.json
--rw-r--r--   0 runner    (1001) docker     (127)     4627 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/required.json
--rw-r--r--   0 runner    (1001) docker     (127)    14365 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/type.json
--rw-r--r--   0 runner    (1001) docker     (127)    19784 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/unevaluatedItems.json
--rw-r--r--   0 runner    (1001) docker     (127)    42268 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/unevaluatedProperties.json
--rw-r--r--   0 runner    (1001) docker     (127)    14264 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/uniqueItems.json
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/unknownKeyword.json
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tests/latest/vocabulary.json
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/json/tox.ini
--rw-r--r--   0 runner    (1001) docker     (127)     7733 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/protocols.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.744959 asdf-3.1.0/asdf/_jsonschema/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/schemas/draft2019-09.json
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/schemas/draft2020-12.json
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/schemas/draft3.json
--rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/schemas/draft4.json
--rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/schemas/draft6.json
--rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/schemas/draft7.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.620958 asdf-3.1.0/asdf/_jsonschema/schemas/vocabularies/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.744959 asdf-3.1.0/asdf/_jsonschema/schemas/vocabularies/draft2019-09/
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/schemas/vocabularies/draft2019-09/applicator
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/schemas/vocabularies/draft2019-09/content
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/schemas/vocabularies/draft2019-09/core
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/schemas/vocabularies/draft2019-09/meta-data
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/schemas/vocabularies/draft2019-09/validation
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.744959 asdf-3.1.0/asdf/_jsonschema/schemas/vocabularies/draft2020-12/
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/schemas/vocabularies/draft2020-12/applicator
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/schemas/vocabularies/draft2020-12/content
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/schemas/vocabularies/draft2020-12/core
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/schemas/vocabularies/draft2020-12/format
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/schemas/vocabularies/draft2020-12/format-annotation
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/schemas/vocabularies/draft2020-12/format-assertion
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/schemas/vocabularies/draft2020-12/meta-data
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/schemas/vocabularies/draft2020-12/unevaluated
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/schemas/vocabularies/draft2020-12/validation
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.748959 asdf-3.1.0/asdf/_jsonschema/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/tests/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7081 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/tests/_suite.py
--rw-r--r--   0 runner    (1001) docker     (127)     8195 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/tests/test_deprecations.py
--rw-r--r--   0 runner    (1001) docker     (127)    19651 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/tests/test_format.py
--rw-r--r--   0 runner    (1001) docker     (127)    18228 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/tests/test_jsonschema_test_suite.py
--rw-r--r--   0 runner    (1001) docker     (127)     7007 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    77231 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/tests/test_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)    37548 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_jsonschema/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)    10450 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_node_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.752959 asdf-3.1.0/asdf/_tests/
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.756959 asdf-3.1.0/asdf/_tests/_block/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/_block/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/_block/test_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/_block/test_external.py
--rw-r--r--   0 runner    (1001) docker     (127)    12602 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/_block/test_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/_block/test_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/_block/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/_block/test_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     7113 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/_block/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/_block/test_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/_block/test_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    15782 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.756959 asdf-3.1.0/asdf/_tests/_regtests/
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/_regtests/test_1013.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/_regtests/test_1334.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/_regtests/test_1505.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/_regtests/test_1523.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/_regtests/test_1525.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/_regtests/test_1526.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/_regtests/test_1530.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/_regtests/test_1538.py
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/_regtests/test_1539.py
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/_regtests/test_1540.py
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/_regtests/test_1541.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/_regtests/test_1542.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/_regtests/test_1553.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/_regtests/test_1558.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.620958 asdf-3.1.0/asdf/_tests/commands/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.760959 asdf-3.1.0/asdf/_tests/commands/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/commands/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.764959 asdf-3.1.0/asdf/_tests/commands/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/commands/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    80427 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/commands/tests/data/block0.asdf
--rw-r--r--   0 runner    (1001) docker     (127)    80427 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/commands/tests/data/block1.asdf
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/commands/tests/data/blocks.diff
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/commands/tests/data/frames.diff
--rw-r--r--   0 runner    (1001) docker     (127)     4191 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/commands/tests/data/frames0.asdf
--rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/commands/tests/data/frames1.asdf
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/commands/tests/data/frames_ignore_asdf_library.diff
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/commands/tests/data/frames_ignore_both.diff
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/commands/tests/data/frames_ignore_reference_frame.diff
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/commands/tests/data/frames_minimal.diff
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/commands/tests/data/ndarray0.asdf
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/commands/tests/data/ndarray1.asdf
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/commands/tests/data/ndarray_in_list.diff
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/commands/tests/data/ndarray_in_list0.asdf
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/commands/tests/data/ndarray_in_list1.asdf
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/commands/tests/data/ndarrays.diff
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/commands/tests/data/simple_inline_array.diff
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/commands/tests/data/simple_inline_array0.asdf
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/commands/tests/data/simple_inline_array1.asdf
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/commands/tests/test_defragment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/commands/tests/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (127)    10009 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/commands/tests/test_edit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/commands/tests/test_exploded.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/commands/tests/test_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/commands/tests/test_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/commands/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/commands/tests/test_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/commands/tests/test_to_yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.764959 asdf-3.1.0/asdf/_tests/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.764959 asdf-3.1.0/asdf/_tests/core/_converters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/core/_converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/core/_converters/test_complex.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/core/_converters/test_constant.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/core/_converters/test_external_reference.py
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/core/_converters/test_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.764959 asdf-3.1.0/asdf/_tests/core/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/core/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/core/tests/test_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.764959 asdf-3.1.0/asdf/_tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/data/complex-42.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/data/custom-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/data/custom_schema.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/data/custom_schema_definitions.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/data/custom_schema_external_ref.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)     2203 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/data/example_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/data/fraction-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/data/fraction_with_inverse-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/data/fractional_2d_coord-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/data/missing-1.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/data/self_referencing-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/httpserver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.764959 asdf-3.1.0/asdf/_tests/tags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/tags/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.768959 asdf-3.1.0/asdf/_tests/tags/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/tags/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.768959 asdf-3.1.0/asdf/_tests/tags/core/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/tags/core/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/tags/core/tests/test_integer.py
--rw-r--r--   0 runner    (1001) docker     (127)    29840 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/tags/core/tests/test_ndarray.py
--rw-r--r--   0 runner    (1001) docker     (127)    15260 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    32897 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/test_array_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)    12576 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/test_asdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     8999 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/test_block_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7760 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/test_compression.py
--rw-r--r--   0 runner    (1001) docker     (127)    14039 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/test_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/test_entry_points.py
--rw-r--r--   0 runner    (1001) docker     (127)    32311 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/test_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/test_file_format.py
--rw-r--r--   0 runner    (1001) docker     (127)    27571 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/test_generic_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     8661 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/test_history.py
--rw-r--r--   0 runner    (1001) docker     (127)    23463 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/test_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4300 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     9930 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/test_reference.py
--rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/test_reference_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/test_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    37921 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5516 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     5762 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/test_serialization_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/test_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/test_tagged.py
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/test_treeutil.py
--rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5160 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     7288 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/test_versioning.py
--rw-r--r--   0 runner    (1001) docker     (127)     9270 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/_tests/test_yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-27 20:49:49.000000 asdf-3.1.0/asdf/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/asdf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.768959 asdf-3.1.0/asdf/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/commands/defragment.py
--rw-r--r--   0 runner    (1001) docker     (127)    13541 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/commands/diff.py
--rw-r--r--   0 runner    (1001) docker     (127)    12956 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/commands/edit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/commands/exploded.py
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/commands/extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/commands/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/commands/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/commands/tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/commands/to_yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)    15890 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.768959 asdf-3.1.0/asdf/extension/
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/extension/_compressor.py
--rw-r--r--   0 runner    (1001) docker     (127)    11763 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/extension/_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    11497 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/extension/_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     9074 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/extension/_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/extension/_manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)    10195 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/extension/_serialization_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/extension/_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/extension/_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)    36400 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/generic_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/reference.py
--rw-r--r--   0 runner    (1001) docker     (127)     5066 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    25560 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    13131 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/search.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/tagged.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.772959 asdf-3.1.0/asdf/tags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/tags/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.772959 asdf-3.1.0/asdf/tags/core/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/tags/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/tags/core/constant.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/tags/core/external_reference.py
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/tags/core/integer.py
--rw-r--r--   0 runner    (1001) docker     (127)    18244 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/tags/core/ndarray.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/tags/core/stream.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.772959 asdf-3.1.0/asdf/testing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/testing/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    14785 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/treeutil.py
--rw-r--r--   0 runner    (1001) docker     (127)    16834 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/versioning.py
--rw-r--r--   0 runner    (1001) docker     (127)    14995 2024-02-27 20:49:34.000000 asdf-3.1.0/asdf/yamlutil.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.780959 asdf-3.1.0/asdf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14620 2024-02-27 20:49:49.000000 asdf-3.1.0/asdf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    43720 2024-02-27 20:49:49.000000 asdf-3.1.0/asdf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-27 20:49:49.000000 asdf-3.1.0/asdf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-02-27 20:49:49.000000 asdf-3.1.0/asdf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-02-27 20:49:49.000000 asdf-3.1.0/asdf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-27 20:49:49.000000 asdf-3.1.0/asdf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-02-27 20:49:34.000000 asdf-3.1.0/asv.conf.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.772959 asdf-3.1.0/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:34.000000 asdf-3.1.0/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-02-27 20:49:34.000000 asdf-3.1.0/benchmarks/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-02-27 20:49:34.000000 asdf-3.1.0/benchmarks/asdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-02-27 20:49:34.000000 asdf-3.1.0/benchmarks/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-02-27 20:49:34.000000 asdf-3.1.0/benchmarks/treeutil.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-02-27 20:49:34.000000 asdf-3.1.0/benchmarks/yamlutil.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.772959 asdf-3.1.0/compatibility_tests/
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-02-27 20:49:34.000000 asdf-3.1.0/compatibility_tests/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-02-27 20:49:34.000000 asdf-3.1.0/compatibility_tests/assert_file_correct.py
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-02-27 20:49:34.000000 asdf-3.1.0/compatibility_tests/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-02-27 20:49:34.000000 asdf-3.1.0/compatibility_tests/generate_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     7700 2024-02-27 20:49:34.000000 asdf-3.1.0/compatibility_tests/test_file_compatibility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.772959 asdf-3.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     4724 2024-02-27 20:49:34.000000 asdf-3.1.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.776959 asdf-3.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     5694 2024-02-27 20:49:34.000000 asdf-3.1.0/docs/_static/logo.ico
--rw-r--r--   0 runner    (1001) docker     (127)    10668 2024-02-27 20:49:34.000000 asdf-3.1.0/docs/_static/logo.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    16762 2024-02-27 20:49:34.000000 asdf-3.1.0/docs/_static/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.776959 asdf-3.1.0/docs/asdf/
--rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-02-27 20:49:34.000000 asdf-3.1.0/docs/asdf/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9266 2024-02-27 20:49:34.000000 asdf-3.1.0/docs/asdf/arrays.rst
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-02-27 20:49:34.000000 asdf-3.1.0/docs/asdf/asdf_tool.rst
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-02-27 20:49:34.000000 asdf-3.1.0/docs/asdf/changes.rst
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-02-27 20:49:34.000000 asdf-3.1.0/docs/asdf/citation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7847 2024-02-27 20:49:34.000000 asdf-3.1.0/docs/asdf/config.rst
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-02-27 20:49:34.000000 asdf-3.1.0/docs/asdf/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4355 2024-02-27 20:49:34.000000 asdf-3.1.0/docs/asdf/deprecations.rst
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-02-27 20:49:34.000000 asdf-3.1.0/docs/asdf/developer_api.rst
--rw-r--r--   0 runner    (1001) docker     (127)    38449 2024-02-27 20:49:34.000000 asdf-3.1.0/docs/asdf/developer_overview.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.780959 asdf-3.1.0/docs/asdf/extending/
--rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-02-27 20:49:34.000000 asdf-3.1.0/docs/asdf/extending/compressors.rst
--rw-r--r--   0 runner    (1001) docker     (127)    19441 2024-02-27 20:49:34.000000 asdf-3.1.0/docs/asdf/extending/converters.rst
--rw-r--r--   0 runner    (1001) docker     (127)    15738 2024-02-27 20:49:34.000000 asdf-3.1.0/docs/asdf/extending/extensions.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-02-27 20:49:34.000000 asdf-3.1.0/docs/asdf/extending/manifests.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9183 2024-02-27 20:49:34.000000 asdf-3.1.0/docs/asdf/extending/resources.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10634 2024-02-27 20:49:34.000000 asdf-3.1.0/docs/asdf/extending/schemas.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4783 2024-02-27 20:49:34.000000 asdf-3.1.0/docs/asdf/extending/uris.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9449 2024-02-27 20:49:34.000000 asdf-3.1.0/docs/asdf/extending/use_cases.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-02-27 20:49:34.000000 asdf-3.1.0/docs/asdf/extending/validators.rst
--rw-r--r--   0 runner    (1001) docker     (127)    25182 2024-02-27 20:49:34.000000 asdf-3.1.0/docs/asdf/features.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-02-27 20:49:34.000000 asdf-3.1.0/docs/asdf/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-02-27 20:49:34.000000 asdf-3.1.0/docs/asdf/overview.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-02-27 20:49:34.000000 asdf-3.1.0/docs/asdf/release_and_support.rst
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-02-27 20:49:34.000000 asdf-3.1.0/docs/asdf/user_api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9165 2024-02-27 20:49:34.000000 asdf-3.1.0/docs/asdf/using_extensions.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5091 2024-02-27 20:49:34.000000 asdf-3.1.0/docs/asdf/whats_new.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-02-27 20:49:34.000000 asdf-3.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-02-27 20:49:34.000000 asdf-3.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-02-27 20:49:34.000000 asdf-3.1.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-02-27 20:49:34.000000 asdf-3.1.0/docs/rtd_environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.780959 asdf-3.1.0/licenses/
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-02-27 20:49:34.000000 asdf-3.1.0/licenses/JSONSCHEMA_LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-02-27 20:49:34.000000 asdf-3.1.0/licenses/JSON_LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-02-27 20:49:34.000000 asdf-3.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:49.780959 asdf-3.1.0/pytest_asdf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 20:49:34.000000 asdf-3.1.0/pytest_asdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10987 2024-02-27 20:49:34.000000 asdf-3.1.0/pytest_asdf/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-02-27 20:49:34.000000 asdf-3.1.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-27 20:49:49.780959 asdf-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     9613 2024-02-27 20:49:34.000000 asdf-3.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.396895 asdf-3.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.240893 asdf-3.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-05 16:10:02.000000 asdf-3.2.0/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-05 16:10:02.000000 asdf-3.2.0/.github/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-05 16:10:02.000000 asdf-3.2.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-05 16:10:02.000000 asdf-3.2.0/.github/issue_template.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-05 16:10:02.000000 asdf-3.2.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.244894 asdf-3.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-05 16:10:02.000000 asdf-3.2.0/.github/workflows/changelog.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-04-05 16:10:02.000000 asdf-3.2.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-04-05 16:10:02.000000 asdf-3.2.0/.github/workflows/downstream.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-05 16:10:02.000000 asdf-3.2.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-04-05 16:10:02.000000 asdf-3.2.0/.github/workflows/s390x.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    34895 2024-04-05 16:10:02.000000 asdf-3.2.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-04-05 16:10:02.000000 asdf-3.2.0/CITATION.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-04-05 16:10:02.000000 asdf-3.2.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-05 16:10:02.000000 asdf-3.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-05 16:10:02.000000 asdf-3.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    14530 2024-04-05 16:10:13.396895 asdf-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11051 2024-04-05 16:10:02.000000 asdf-3.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.248894 asdf-3.2.0/asdf/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60319 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_asdf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.248894 asdf-3.2.0/asdf/_block/
+-rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_block/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_block/callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_block/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_block/external.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16493 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_block/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_block/key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25629 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_block/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_block/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9360 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_block/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_block/store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4012 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_block/writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10595 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_compression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_convenience.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.252894 asdf-3.2.0/asdf/_core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.252894 asdf-3.2.0/asdf/_core/_converters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_core/_converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_core/_converters/complex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_core/_converters/constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_core/_converters/external_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_core/_converters/integer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7257 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_core/_converters/ndarray.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_core/_converters/reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_core/_converters/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_core/_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_core/_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.252894 asdf-3.2.0/asdf/_core/_validators/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_core/_validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_core/_validators/ndarray.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9122 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_entry_points.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.252894 asdf-3.2.0/asdf/_extern/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7095 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_extern/RangeHTTPServer.py
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_extern/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_extern/atomicfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.256894 asdf-3.2.0/asdf/_jsonschema/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14587 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10561 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/_legacy_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10429 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15968 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.256894 asdf-3.2.0/asdf/_jsonschema/json/
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16971 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.256894 asdf-3.2.0/asdf/_jsonschema/json/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11731 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/bin/jsonschema_suite
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.260894 asdf-3.2.0/asdf/_jsonschema/json/remotes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.260894 asdf-3.2.0/asdf/_jsonschema/json/remotes/baseUriChange/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/baseUriChange/folderInteger.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.260894 asdf-3.2.0/asdf/_jsonschema/json/remotes/baseUriChangeFolder/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/baseUriChangeFolder/folderInteger.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.260894 asdf-3.2.0/asdf/_jsonschema/json/remotes/baseUriChangeFolderInSubschema/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/baseUriChangeFolderInSubschema/folderInteger.json
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/different-id-ref-string.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.260894 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft-next/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.260894 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft-next/baseUriChange/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft-next/baseUriChange/folderInteger.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.260894 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft-next/baseUriChangeFolder/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft-next/baseUriChangeFolder/folderInteger.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.260894 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft-next/baseUriChangeFolderInSubschema/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft-next/baseUriChangeFolderInSubschema/folderInteger.json
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft-next/extendible-dynamic-ref.json
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft-next/format-assertion-false.json
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft-next/format-assertion-true.json
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft-next/integer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft-next/locationIndependentIdentifier.json
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft-next/metaschema-no-validation.json
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft-next/name-defs.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.260894 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft-next/nested/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft-next/nested/foo-ref-string.json
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft-next/nested/string.json
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft-next/ref-and-defs.json
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft-next/subSchemas-defs.json
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft-next/subSchemas.json
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft-next/tree.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.264894 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft2019-09/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.264894 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft2019-09/baseUriChange/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft2019-09/baseUriChange/folderInteger.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.264894 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft2019-09/baseUriChangeFolder/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft2019-09/baseUriChangeFolder/folderInteger.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.264894 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft2019-09/baseUriChangeFolderInSubschema/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft2019-09/baseUriChangeFolderInSubschema/folderInteger.json
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft2019-09/dependentRequired.json
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft2019-09/extendible-dynamic-ref.json
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft2019-09/ignore-prefixItems.json
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft2019-09/integer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft2019-09/locationIndependentIdentifier.json
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft2019-09/metaschema-no-validation.json
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft2019-09/name-defs.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.264894 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft2019-09/nested/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft2019-09/nested/foo-ref-string.json
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft2019-09/nested/string.json
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft2019-09/ref-and-defs.json
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft2019-09/subSchemas-defs.json
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft2019-09/subSchemas.json
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft2019-09/tree.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.268894 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft2020-12/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.268894 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft2020-12/baseUriChange/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft2020-12/baseUriChange/folderInteger.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.268894 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft2020-12/baseUriChangeFolder/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft2020-12/baseUriChangeFolder/folderInteger.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.268894 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft2020-12/baseUriChangeFolderInSubschema/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft2020-12/baseUriChangeFolderInSubschema/folderInteger.json
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft2020-12/extendible-dynamic-ref.json
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft2020-12/format-assertion-false.json
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft2020-12/format-assertion-true.json
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft2020-12/integer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft2020-12/locationIndependentIdentifier.json
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft2020-12/metaschema-no-validation.json
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft2020-12/name-defs.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.268894 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft2020-12/nested/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft2020-12/nested/foo-ref-string.json
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft2020-12/nested/string.json
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft2020-12/prefixItems.json
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft2020-12/ref-and-defs.json
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft2020-12/subSchemas-defs.json
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft2020-12/subSchemas.json
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft2020-12/tree.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.268894 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft7/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/draft7/ignore-dependentRequired.json
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/extendible-dynamic-ref.json
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/integer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/locationIndependentIdentifier.json
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/locationIndependentIdentifierDraft4.json
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/locationIndependentIdentifierPre2019.json
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/name-defs.json
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/name.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.268894 asdf-3.2.0/asdf/_jsonschema/json/remotes/nested/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/nested/foo-ref-string.json
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/nested/string.json
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/nested-absolute-ref-to-string.json
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/ref-and-definitions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/ref-and-defs.json
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/subSchemas-defs.json
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/subSchemas.json
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/tree.json
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/remotes/urn-ref-string.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/test-schema.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.236894 asdf-3.2.0/asdf/_jsonschema/json/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.276894 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/
+-rw-r--r--   0 runner    (1001) docker     (127)     4924 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/additionalProperties.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8665 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/allOf.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7136 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/anchor.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5437 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/anyOf.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/boolean_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10936 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/const.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8424 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/contains.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/content.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/default.json
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/defs.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/dependentRequired.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3862 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/dependentSchemas.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19268 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/dynamicRef.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7415 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/enum.json
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/exclusiveMaximum.json
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/exclusiveMinimum.json
+-rw-r--r--   0 runner    (1001) docker     (127)    21855 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/format.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10224 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/id.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7546 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/if-then-else.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/infinite-loop-detection.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8609 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/items.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/maxContains.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/maxItems.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/maxLength.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/maxProperties.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/maximum.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6551 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/minContains.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/minItems.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/minLength.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/minProperties.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/minimum.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/multipleOf.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/not.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8087 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/oneOf.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.276894 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/optional/
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/optional/bignum.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8123 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/optional/dependencies-compatibility.json
+-rw-r--r--   0 runner    (1001) docker     (127)    20388 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/optional/ecmascript-regex.json
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/optional/float-overflow.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.280894 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/optional/format/
+-rw-r--r--   0 runner    (1001) docker     (127)     4744 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/optional/format/date-time.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7536 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/optional/format/date.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/optional/format/duration.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/optional/format/email.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/optional/format/hostname.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/optional/format/idn-email.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14841 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/optional/format/idn-hostname.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/optional/format/ipv4.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7031 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/optional/format/ipv6.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/optional/format/iri-reference.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/optional/format/iri.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6795 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/optional/format/json-pointer.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/optional/format/regex.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/optional/format/relative-json-pointer.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7374 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/optional/format/time.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/optional/format/uri-reference.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/optional/format/uri-template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4724 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/optional/format/uri.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/optional/format/uuid.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/optional/format-assertion.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/optional/non-bmp-regex.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/optional/refOfUnknownKeyword.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/pattern.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5517 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/patternProperties.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/prefixItems.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7713 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/properties.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/propertyDependencies.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/propertyNames.json
+-rw-r--r--   0 runner    (1001) docker     (127)    27406 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/ref.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8801 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/refRemote.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/required.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14332 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/type.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19715 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/unevaluatedItems.json
+-rw-r--r--   0 runner    (1001) docker     (127)    45112 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/unevaluatedProperties.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14246 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/uniqueItems.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/unknownKeyword.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/vocabulary.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.288894 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/
+-rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/additionalItems.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4945 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/additionalProperties.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8701 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/allOf.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7206 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/anchor.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5461 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/anyOf.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/boolean_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10981 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/const.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/contains.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4397 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/content.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/default.json
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/defs.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/dependentRequired.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/dependentSchemas.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7445 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/enum.json
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/exclusiveMaximum.json
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/exclusiveMinimum.json
+-rw-r--r--   0 runner    (1001) docker     (127)    21912 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/format.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/id.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7576 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/if-then-else.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/infinite-loop-detection.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8723 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/items.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/maxContains.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/maxItems.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/maxLength.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/maxProperties.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/maximum.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6624 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/minContains.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/minItems.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/minLength.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/minProperties.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/minimum.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/multipleOf.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/not.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8120 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/oneOf.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.292894 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/optional/
+-rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/optional/bignum.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/optional/cross-draft.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8144 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/optional/dependencies-compatibility.json
+-rw-r--r--   0 runner    (1001) docker     (127)    20017 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/optional/ecmascript-regex.json
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/optional/float-overflow.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.292894 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/date-time.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7539 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/date.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/duration.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/email.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/hostname.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/idn-email.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14844 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/idn-hostname.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/ipv4.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7034 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/ipv6.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/iri-reference.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/iri.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6798 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/json-pointer.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/regex.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/relative-json-pointer.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7377 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/time.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/unknown.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/uri-reference.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/uri-template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/uri.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/uuid.json
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/optional/no-schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/optional/non-bmp-regex.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/optional/refOfUnknownKeyword.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/pattern.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/patternProperties.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7731 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/properties.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/propertyNames.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14068 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/recursiveRef.json
+-rw-r--r--   0 runner    (1001) docker     (127)    27548 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/ref.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8851 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/refRemote.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4627 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/required.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14365 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/type.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16095 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/unevaluatedItems.json
+-rw-r--r--   0 runner    (1001) docker     (127)    42268 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/unevaluatedProperties.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14260 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/uniqueItems.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/unknownKeyword.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/vocabulary.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.300894 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/
+-rw-r--r--   0 runner    (1001) docker     (127)     4945 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/additionalProperties.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8701 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/allOf.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7206 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/anchor.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5461 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/anyOf.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/boolean_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10981 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/const.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/contains.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4397 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/content.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/default.json
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/defs.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/dependentRequired.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/dependentSchemas.json
+-rw-r--r--   0 runner    (1001) docker     (127)    21588 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/dynamicRef.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7445 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/enum.json
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/exclusiveMaximum.json
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/exclusiveMinimum.json
+-rw-r--r--   0 runner    (1001) docker     (127)    21912 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/format.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/id.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7576 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/if-then-else.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/infinite-loop-detection.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8636 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/items.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/maxContains.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/maxItems.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/maxLength.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/maxProperties.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/maximum.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6604 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/minContains.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/minItems.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/minLength.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/minProperties.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/minimum.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/multipleOf.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/not.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8120 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/oneOf.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.304894 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/optional/
+-rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/optional/bignum.json
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/optional/cross-draft.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8144 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/optional/dependencies-compatibility.json
+-rw-r--r--   0 runner    (1001) docker     (127)    20454 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/optional/ecmascript-regex.json
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/optional/float-overflow.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.308894 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/date-time.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7539 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/date.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/duration.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4052 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/email.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/hostname.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/idn-email.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14844 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/idn-hostname.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/ipv4.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7034 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/ipv6.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/iri-reference.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/iri.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6798 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/json-pointer.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/regex.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/relative-json-pointer.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7377 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/time.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/unknown.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/uri-reference.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/uri-template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/uri.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/uuid.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format-assertion.json
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/optional/no-schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/optional/non-bmp-regex.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/optional/refOfUnknownKeyword.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/pattern.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/patternProperties.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/prefixItems.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7731 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/properties.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/propertyNames.json
+-rw-r--r--   0 runner    (1001) docker     (127)    27508 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/ref.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8851 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/refRemote.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4627 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/required.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14365 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/type.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19784 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/unevaluatedItems.json
+-rw-r--r--   0 runner    (1001) docker     (127)    42268 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/unevaluatedProperties.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14264 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/uniqueItems.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/unknownKeyword.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/vocabulary.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.312894 asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/
+-rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/additionalItems.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4430 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/additionalProperties.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/default.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/dependencies.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/disallow.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/divisibleBy.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/enum.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/extends.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10579 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/format.json
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/infinite-loop-detection.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/items.json
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/maxItems.json
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/maxLength.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/maximum.json
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/minItems.json
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/minLength.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/minimum.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.312894 asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/optional/
+-rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/optional/bignum.json
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/optional/ecmascript-regex.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.312894 asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/optional/format/
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/optional/format/color.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/optional/format/date-time.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/optional/format/date.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/optional/format/email.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/optional/format/host-name.json
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/optional/format/ip-address.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/optional/format/ipv6.json
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/optional/format/regex.json
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/optional/format/time.json
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/optional/format/uri.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/optional/non-bmp-regex.json
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/optional/zeroTerminatedFloats.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/pattern.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/patternProperties.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/properties.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8112 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/ref.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/refRemote.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/required.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13876 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/type.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12787 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/uniqueItems.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.320894 asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/
+-rw-r--r--   0 runner    (1001) docker     (127)     4711 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/additionalItems.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4426 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/additionalProperties.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6901 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/allOf.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/anyOf.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/default.json
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/definitions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/dependencies.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6563 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/enum.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6345 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/format.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/id.json
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/infinite-loop-detection.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6564 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/items.json
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/maxItems.json
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/maxLength.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/maxProperties.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/maximum.json
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/minItems.json
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/minLength.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/minProperties.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/minimum.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/multipleOf.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/not.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6035 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/oneOf.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.320894 asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/optional/
+-rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/optional/bignum.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18487 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/optional/ecmascript-regex.json
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/optional/float-overflow.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.320894 asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/optional/format/
+-rw-r--r--   0 runner    (1001) docker     (127)     4656 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/optional/format/date-time.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/optional/format/email.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/optional/format/hostname.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/optional/format/ipv4.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6943 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/optional/format/ipv6.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/optional/format/unknown.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/optional/format/uri.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/optional/non-bmp-regex.json
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/optional/zeroTerminatedFloats.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/pattern.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/patternProperties.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6413 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/properties.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14935 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/ref.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/refRemote.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/required.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13221 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/type.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13792 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/uniqueItems.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.328894 asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/
+-rw-r--r--   0 runner    (1001) docker     (127)     4711 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/additionalItems.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4426 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/additionalProperties.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7783 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/allOf.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4827 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/anyOf.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/boolean_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9588 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/const.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/contains.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/default.json
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/definitions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6876 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/dependencies.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6563 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/enum.json
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/exclusiveMaximum.json
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/exclusiveMinimum.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9557 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/format.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/id.json
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/infinite-loop-detection.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8076 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/items.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/maxItems.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/maxLength.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/maxProperties.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/maximum.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/minItems.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/minLength.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/minProperties.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/minimum.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/multipleOf.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/not.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7251 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/oneOf.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.328894 asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/optional/
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/optional/bignum.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18497 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/optional/ecmascript-regex.json
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/optional/float-overflow.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.332894 asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/optional/format/
+-rw-r--r--   0 runner    (1001) docker     (127)     4656 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/optional/format/date-time.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/optional/format/email.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/optional/format/hostname.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/optional/format/ipv4.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6943 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/optional/format/ipv6.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6707 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/optional/format/json-pointer.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/optional/format/unknown.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/optional/format/uri-reference.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/optional/format/uri-template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/optional/format/uri.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/optional/non-bmp-regex.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/pattern.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/patternProperties.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7305 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/properties.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/propertyNames.json
+-rw-r--r--   0 runner    (1001) docker     (127)    23343 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/ref.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6688 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/refRemote.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4252 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/required.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13408 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/type.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13792 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/uniqueItems.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/unknownKeyword.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.340894 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/
+-rw-r--r--   0 runner    (1001) docker     (127)     4711 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/additionalItems.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4426 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/additionalProperties.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7783 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/allOf.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4827 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/anyOf.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/boolean_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9588 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/const.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/contains.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/default.json
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/definitions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6876 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/dependencies.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6563 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/enum.json
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/exclusiveMaximum.json
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/exclusiveMinimum.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18067 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/format.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/id.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6866 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/if-then-else.json
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/infinite-loop-detection.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8076 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/items.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/maxItems.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/maxLength.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/maxProperties.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/maximum.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/minItems.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/minLength.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/minProperties.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/minimum.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/multipleOf.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/not.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7251 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/oneOf.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.340894 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/optional/
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/optional/bignum.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/optional/content.json
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/optional/cross-draft.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18497 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/optional/ecmascript-regex.json
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/optional/float-overflow.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.344894 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/optional/format/
+-rw-r--r--   0 runner    (1001) docker     (127)     4656 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/optional/format/date-time.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7448 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/optional/format/date.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/optional/format/email.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/optional/format/hostname.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/optional/format/idn-email.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14753 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/optional/format/idn-hostname.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/optional/format/ipv4.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6943 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/optional/format/ipv6.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/optional/format/iri-reference.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/optional/format/iri.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6707 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/optional/format/json-pointer.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/optional/format/regex.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/optional/format/relative-json-pointer.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7286 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/optional/format/time.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/optional/format/unknown.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/optional/format/uri-reference.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/optional/format/uri-template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/optional/format/uri.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/optional/non-bmp-regex.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/pattern.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/patternProperties.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7305 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/properties.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/propertyNames.json
+-rw-r--r--   0 runner    (1001) docker     (127)    24396 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/ref.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6688 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/refRemote.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4252 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/required.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13408 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/type.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13792 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/uniqueItems.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/unknownKeyword.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.352894 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/
+-rw-r--r--   0 runner    (1001) docker     (127)     4945 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/additionalProperties.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8701 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/allOf.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7206 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/anchor.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5461 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/anyOf.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/boolean_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10981 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/const.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/contains.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4397 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/content.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/default.json
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/defs.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/dependentRequired.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/dependentSchemas.json
+-rw-r--r--   0 runner    (1001) docker     (127)    21588 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/dynamicRef.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7445 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/enum.json
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/exclusiveMaximum.json
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/exclusiveMinimum.json
+-rw-r--r--   0 runner    (1001) docker     (127)    21912 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/format.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/id.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7576 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/if-then-else.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/infinite-loop-detection.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8636 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/items.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/maxContains.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/maxItems.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/maxLength.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/maxProperties.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/maximum.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6604 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/minContains.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/minItems.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/minLength.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/minProperties.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/minimum.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/multipleOf.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/not.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8120 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/oneOf.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.352894 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/optional/
+-rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/optional/bignum.json
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/optional/cross-draft.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8144 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/optional/dependencies-compatibility.json
+-rw-r--r--   0 runner    (1001) docker     (127)    20454 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/optional/ecmascript-regex.json
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/optional/float-overflow.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.356894 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/optional/format/
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/optional/format/date-time.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7539 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/optional/format/date.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/optional/format/duration.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4052 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/optional/format/email.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/optional/format/hostname.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/optional/format/idn-email.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14844 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/optional/format/idn-hostname.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/optional/format/ipv4.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7034 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/optional/format/ipv6.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/optional/format/iri-reference.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/optional/format/iri.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6798 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/optional/format/json-pointer.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/optional/format/regex.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/optional/format/relative-json-pointer.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7377 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/optional/format/time.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/optional/format/unknown.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/optional/format/uri-reference.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/optional/format/uri-template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/optional/format/uri.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/optional/format/uuid.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/optional/format-assertion.json
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/optional/no-schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/optional/non-bmp-regex.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/optional/refOfUnknownKeyword.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/pattern.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/patternProperties.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/prefixItems.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7731 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/properties.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/propertyNames.json
+-rw-r--r--   0 runner    (1001) docker     (127)    27508 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/ref.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8851 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/refRemote.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4627 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/required.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14365 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/type.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19784 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/unevaluatedItems.json
+-rw-r--r--   0 runner    (1001) docker     (127)    42268 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/unevaluatedProperties.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14264 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/uniqueItems.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/unknownKeyword.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tests/latest/vocabulary.json
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/json/tox.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     7733 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/protocols.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.356894 asdf-3.2.0/asdf/_jsonschema/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/schemas/draft2019-09.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/schemas/draft2020-12.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/schemas/draft3.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/schemas/draft4.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/schemas/draft6.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/schemas/draft7.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.236894 asdf-3.2.0/asdf/_jsonschema/schemas/vocabularies/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.360895 asdf-3.2.0/asdf/_jsonschema/schemas/vocabularies/draft2019-09/
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/schemas/vocabularies/draft2019-09/applicator
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/schemas/vocabularies/draft2019-09/content
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/schemas/vocabularies/draft2019-09/core
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/schemas/vocabularies/draft2019-09/meta-data
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/schemas/vocabularies/draft2019-09/validation
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.360895 asdf-3.2.0/asdf/_jsonschema/schemas/vocabularies/draft2020-12/
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/schemas/vocabularies/draft2020-12/applicator
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/schemas/vocabularies/draft2020-12/content
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/schemas/vocabularies/draft2020-12/core
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/schemas/vocabularies/draft2020-12/format
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/schemas/vocabularies/draft2020-12/format-annotation
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/schemas/vocabularies/draft2020-12/format-assertion
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/schemas/vocabularies/draft2020-12/meta-data
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/schemas/vocabularies/draft2020-12/unevaluated
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/schemas/vocabularies/draft2020-12/validation
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.360895 asdf-3.2.0/asdf/_jsonschema/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/tests/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7081 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/tests/_suite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8195 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/tests/test_deprecations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19651 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/tests/test_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18228 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/tests/test_jsonschema_test_suite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7007 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77231 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/tests/test_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37548 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_jsonschema/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10450 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_node_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.368894 asdf-3.2.0/asdf/_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.368894 asdf-3.2.0/asdf/_tests/_block/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/_block/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/_block/test_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/_block/test_external.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12602 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/_block/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/_block/test_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/_block/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/_block/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7113 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/_block/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/_block/test_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/_block/test_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11417 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.372895 asdf-3.2.0/asdf/_tests/_regtests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/_regtests/test_1013.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/_regtests/test_1334.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/_regtests/test_1505.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/_regtests/test_1523.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/_regtests/test_1525.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/_regtests/test_1526.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/_regtests/test_1530.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/_regtests/test_1538.py
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/_regtests/test_1539.py
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/_regtests/test_1540.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/_regtests/test_1541.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/_regtests/test_1542.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/_regtests/test_1553.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/_regtests/test_1558.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.236894 asdf-3.2.0/asdf/_tests/commands/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.372895 asdf-3.2.0/asdf/_tests/commands/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/commands/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.376895 asdf-3.2.0/asdf/_tests/commands/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/commands/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80427 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/commands/tests/data/block0.asdf
+-rw-r--r--   0 runner    (1001) docker     (127)    80427 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/commands/tests/data/block1.asdf
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/commands/tests/data/blocks.diff
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/commands/tests/data/frames.diff
+-rw-r--r--   0 runner    (1001) docker     (127)     4191 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/commands/tests/data/frames0.asdf
+-rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/commands/tests/data/frames1.asdf
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/commands/tests/data/frames_ignore_asdf_library.diff
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/commands/tests/data/frames_ignore_both.diff
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/commands/tests/data/frames_ignore_reference_frame.diff
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/commands/tests/data/frames_minimal.diff
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/commands/tests/data/ndarray0.asdf
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/commands/tests/data/ndarray1.asdf
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/commands/tests/data/ndarray_in_list.diff
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/commands/tests/data/ndarray_in_list0.asdf
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/commands/tests/data/ndarray_in_list1.asdf
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/commands/tests/data/ndarrays.diff
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/commands/tests/data/simple_inline_array.diff
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/commands/tests/data/simple_inline_array0.asdf
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/commands/tests/data/simple_inline_array1.asdf
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/commands/tests/test_defragment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/commands/tests/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10009 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/commands/tests/test_edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/commands/tests/test_exploded.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/commands/tests/test_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/commands/tests/test_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/commands/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/commands/tests/test_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/commands/tests/test_to_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.376895 asdf-3.2.0/asdf/_tests/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.376895 asdf-3.2.0/asdf/_tests/core/_converters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/core/_converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/core/_converters/test_complex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/core/_converters/test_constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/core/_converters/test_external_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/core/_converters/test_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.376895 asdf-3.2.0/asdf/_tests/core/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/core/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/core/tests/test_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.380895 asdf-3.2.0/asdf/_tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/data/complex-42.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/data/custom-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/data/custom_schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/data/custom_schema_definitions.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/data/custom_schema_external_ref.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2203 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/data/example_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/data/fraction-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/data/fraction_with_inverse-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/data/fractional_2d_coord-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/data/missing-1.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/data/self_referencing-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/httpserver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.380895 asdf-3.2.0/asdf/_tests/tags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/tags/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.380895 asdf-3.2.0/asdf/_tests/tags/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/tags/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.380895 asdf-3.2.0/asdf/_tests/tags/core/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/tags/core/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/tags/core/tests/test_integer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29761 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/tags/core/tests/test_ndarray.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15354 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32830 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/test_array_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12429 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/test_asdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8999 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/test_block_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7760 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/test_compression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14039 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4191 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/test_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/test_entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32311 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/test_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/test_file_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27571 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/test_generic_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8661 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/test_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23463 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/test_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4300 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9930 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/test_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/test_reference_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/test_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37895 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5516 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5762 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/test_serialization_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/test_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/test_tagged.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/test_treeutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5160 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7288 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/test_versioning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9155 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/_tests/test_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-05 16:10:13.000000 asdf-3.2.0/asdf/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/asdf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.384895 asdf-3.2.0/asdf/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/commands/defragment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13541 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/commands/diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12956 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/commands/edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/commands/exploded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/commands/extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/commands/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/commands/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/commands/tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/commands/to_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15890 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.384895 asdf-3.2.0/asdf/extension/
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/extension/_compressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11763 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/extension/_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11497 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/extension/_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9074 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/extension/_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/extension/_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10195 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/extension/_serialization_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/extension/_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/extension/_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36400 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/generic_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5066 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25560 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13131 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/tagged.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.384895 asdf-3.2.0/asdf/tags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/tags/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.384895 asdf-3.2.0/asdf/tags/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/tags/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/tags/core/constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/tags/core/external_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/tags/core/integer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18265 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/tags/core/ndarray.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/tags/core/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.384895 asdf-3.2.0/asdf/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/testing/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14785 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/treeutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16833 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5929 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/versioning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14925 2024-04-05 16:10:02.000000 asdf-3.2.0/asdf/yamlutil.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.396895 asdf-3.2.0/asdf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14530 2024-04-05 16:10:13.000000 asdf-3.2.0/asdf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    43737 2024-04-05 16:10:13.000000 asdf-3.2.0/asdf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 16:10:13.000000 asdf-3.2.0/asdf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-05 16:10:13.000000 asdf-3.2.0/asdf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-05 16:10:13.000000 asdf-3.2.0/asdf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-05 16:10:13.000000 asdf-3.2.0/asdf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-05 16:10:02.000000 asdf-3.2.0/asv.conf.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.388895 asdf-3.2.0/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:02.000000 asdf-3.2.0/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-05 16:10:02.000000 asdf-3.2.0/benchmarks/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-04-05 16:10:02.000000 asdf-3.2.0/benchmarks/asdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-05 16:10:02.000000 asdf-3.2.0/benchmarks/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-05 16:10:02.000000 asdf-3.2.0/benchmarks/treeutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-05 16:10:02.000000 asdf-3.2.0/benchmarks/yamlutil.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.388895 asdf-3.2.0/compatibility_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-05 16:10:02.000000 asdf-3.2.0/compatibility_tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-05 16:10:02.000000 asdf-3.2.0/compatibility_tests/assert_file_correct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-05 16:10:02.000000 asdf-3.2.0/compatibility_tests/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-05 16:10:02.000000 asdf-3.2.0/compatibility_tests/generate_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8234 2024-04-05 16:10:02.000000 asdf-3.2.0/compatibility_tests/test_file_compatibility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.388895 asdf-3.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4724 2024-04-05 16:10:02.000000 asdf-3.2.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.388895 asdf-3.2.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     5694 2024-04-05 16:10:02.000000 asdf-3.2.0/docs/_static/logo.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    10668 2024-04-05 16:10:02.000000 asdf-3.2.0/docs/_static/logo.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    16762 2024-04-05 16:10:02.000000 asdf-3.2.0/docs/_static/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.392895 asdf-3.2.0/docs/asdf/
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-04-05 16:10:02.000000 asdf-3.2.0/docs/asdf/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9266 2024-04-05 16:10:02.000000 asdf-3.2.0/docs/asdf/arrays.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-05 16:10:02.000000 asdf-3.2.0/docs/asdf/asdf_tool.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-05 16:10:02.000000 asdf-3.2.0/docs/asdf/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-05 16:10:02.000000 asdf-3.2.0/docs/asdf/citation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7847 2024-04-05 16:10:02.000000 asdf-3.2.0/docs/asdf/config.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-05 16:10:02.000000 asdf-3.2.0/docs/asdf/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4355 2024-04-05 16:10:02.000000 asdf-3.2.0/docs/asdf/deprecations.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-05 16:10:02.000000 asdf-3.2.0/docs/asdf/developer_api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    38449 2024-04-05 16:10:02.000000 asdf-3.2.0/docs/asdf/developer_overview.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.392895 asdf-3.2.0/docs/asdf/extending/
+-rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-04-05 16:10:02.000000 asdf-3.2.0/docs/asdf/extending/compressors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    19441 2024-04-05 16:10:02.000000 asdf-3.2.0/docs/asdf/extending/converters.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    15738 2024-04-05 16:10:02.000000 asdf-3.2.0/docs/asdf/extending/extensions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-04-05 16:10:02.000000 asdf-3.2.0/docs/asdf/extending/manifests.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9183 2024-04-05 16:10:02.000000 asdf-3.2.0/docs/asdf/extending/resources.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10680 2024-04-05 16:10:02.000000 asdf-3.2.0/docs/asdf/extending/schemas.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4783 2024-04-05 16:10:02.000000 asdf-3.2.0/docs/asdf/extending/uris.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9449 2024-04-05 16:10:02.000000 asdf-3.2.0/docs/asdf/extending/use_cases.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-04-05 16:10:02.000000 asdf-3.2.0/docs/asdf/extending/validators.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    25567 2024-04-05 16:10:02.000000 asdf-3.2.0/docs/asdf/features.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-05 16:10:02.000000 asdf-3.2.0/docs/asdf/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-04-05 16:10:02.000000 asdf-3.2.0/docs/asdf/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-04-05 16:10:02.000000 asdf-3.2.0/docs/asdf/release_and_support.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-05 16:10:02.000000 asdf-3.2.0/docs/asdf/user_api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9165 2024-04-05 16:10:02.000000 asdf-3.2.0/docs/asdf/using_extensions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5091 2024-04-05 16:10:02.000000 asdf-3.2.0/docs/asdf/whats_new.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-04-05 16:10:02.000000 asdf-3.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-05 16:10:02.000000 asdf-3.2.0/docs/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-05 16:10:02.000000 asdf-3.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-04-05 16:10:02.000000 asdf-3.2.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-05 16:10:02.000000 asdf-3.2.0/docs/rtd_environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.396895 asdf-3.2.0/licenses/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-05 16:10:02.000000 asdf-3.2.0/licenses/JSONSCHEMA_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-05 16:10:02.000000 asdf-3.2.0/licenses/JSON_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-04-05 16:10:02.000000 asdf-3.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:13.396895 asdf-3.2.0/pytest_asdf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 16:10:02.000000 asdf-3.2.0/pytest_asdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10972 2024-04-05 16:10:02.000000 asdf-3.2.0/pytest_asdf/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-05 16:10:02.000000 asdf-3.2.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 16:10:13.396895 asdf-3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     9058 2024-04-05 16:10:02.000000 asdf-3.2.0/tox.ini
```

### Comparing `asdf-3.1.0/.github/issue_template.md` & `asdf-3.2.0/.github/issue_template.md`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/.github/pull_request_template.md` & `asdf-3.2.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/.github/workflows/changelog.yml` & `asdf-3.2.0/.github/workflows/changelog.yml`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/.github/workflows/ci.yml` & `asdf-3.2.0/.github/workflows/ci.yml`

 * *Files 4% similar despite different names*

```diff
@@ -66,64 +66,63 @@
     with:
       submodules: false
       # Any env name which does not start with `pyXY` will use this Python version.
       default_python: '3.10'
       envs: |
         - linux: asdf-standard
         - linux: asdf-transform-schemas
-        - linux: asdf-unit-schemas
 
   test:
-    needs: [core, asdf-schemas]
+    needs: [core]
     uses: OpenAstronomy/github-actions-workflows/.github/workflows/tox.yml@v1
     with:
       submodules: false
       # Any env name which does not start with `pyXY` will use this Python version.
       default_python: '3.9'
       envs: |
         - macos: py39-parallel
         - windows: py39-parallel
 
   dev:
-    needs: [core, asdf-schemas]
+    needs: [core]
     uses: OpenAstronomy/github-actions-workflows/.github/workflows/tox.yml@v1
     with:
       submodules: false
       # Any env name which does not start with `pyXY` will use this Python version.
       default_python: '3.9'
       envs: |
         - linux: py39-devdeps-parallel
         - linux: py310-devdeps-parallel
         - linux: py311-devdeps-parallel
         - linux: py312-devdeps-parallel
         # separate pytest so a failure here doesn't cause the whole suite to fail
         - linux: py311-pytestdev-parallel
 
   oldest:
-    needs: [core, asdf-schemas]
+    needs: [core]
     uses: OpenAstronomy/github-actions-workflows/.github/workflows/tox.yml@v1
     with:
       submodules: false
       # Any env name which does not start with `pyXY` will use this Python version.
       default_python: '3.9'
       envs: |
         - linux: py39-oldestdeps-parallel
 
   compatibility:
-    needs: [core, asdf-schemas]
+    needs: [core]
     uses: OpenAstronomy/github-actions-workflows/.github/workflows/tox.yml@v1
     with:
       submodules: false
       # Any env name which does not start with `pyXY` will use this Python version.
       default_python: '3.9'
       envs: |
         - linux: compatibility
 
   package:
-    needs: [core, asdf-schemas]
+    needs: [core]
     uses: OpenAstronomy/github-actions-workflows/.github/workflows/publish_pure_python.yml@v1
     with:
       python-version: "3.11"
       upload_to_pypi: false
       upload_to_anaconda: false
       test_extras: tests
       test_command: pytest --pyargs asdf
```

### Comparing `asdf-3.1.0/.github/workflows/downstream.yml` & `asdf-3.2.0/.github/workflows/downstream.yml`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/.github/workflows/s390x.yml` & `asdf-3.2.0/.github/workflows/s390x.yml`

 * *Files 5% similar despite different names*

```diff
@@ -65,11 +65,11 @@
                                   python3-scipy \
                                   python3-venv \
                                   python3-wheel
 
           run: |
             python3 -m venv --system-site-packages tests
             source tests/bin/activate
-            pip3 install --upgrade pip setuptools pytest pytest-doctestplus pytest-remotedata
+            pip3 install --upgrade pip setuptools pytest pytest-remotedata
             pip3 install -e .[all,tests]
             pip3 list
             python3 -m pytest --remote-data
```

### Comparing `asdf-3.1.0/CHANGES.rst` & `asdf-3.2.0/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+3.2.0 (2024-04-05)
+------------------
+
+- Deprecate ``AsdfFile.version_map`` [#1745]
+
+- Fix ``numpy.ma.MaskedArray`` saving for numpy 2.x [#1769]
+
+- Add ``float16`` support [#1692]
+
+- Removed unused ``asdf-unit-schemas`` dependency [#1767]
+
+
 3.1.0 (2024-02-27)
 ------------------
 
 The ASDF Standard is at v1.6.0
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 - Cleanup ``asdf.util`` including deprecating: ``human_list``
@@ -41,14 +53,15 @@
   prevented other warning filters (like those provided with ``-W``)
   from working. If you want these warnings to produce errors you can
   now add your own warning filter [#1757]
 
 - Only show ``str`` representation during ``info`` and ``search``
   if it contains a single line (and does not fail)  [#1748]
 
+
 3.0.1 (2023-10-30)
 ------------------
 
 The ASDF Standard is at v1.6.0
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 - Fix bug in ``asdftool diff`` for arrays within a list [#1672]
```

### Comparing `asdf-3.1.0/CITATION.rst` & `asdf-3.2.0/CITATION.rst`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/CONTRIBUTING.rst` & `asdf-3.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/LICENSE` & `asdf-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/PKG-INFO` & `asdf-3.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asdf
-Version: 3.1.0
+Version: 3.2.0
 Summary: Python implementation of the ASDF Standard
 Author-email: The ASDF Developers <help@stsci.edu>
 License: BSD 3-Clause License
         
         Copyright (c) 2021 Association of Universities for Research in Astronomy.
         All rights reserved.
         
@@ -43,17 +43,16 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: asdf-standard>=1.0.1
+Requires-Dist: asdf-standard>=1.1.0
 Requires-Dist: asdf-transform-schemas>=0.3
-Requires-Dist: asdf-unit-schemas>=0.1
 Requires-Dist: importlib-metadata>=4.11.4
 Requires-Dist: jmespath>=0.6.2
 Requires-Dist: numpy>=1.22
 Requires-Dist: packaging>=19
 Requires-Dist: pyyaml>=5.4.1
 Requires-Dist: semantic_version>=2.8
 Requires-Dist: attrs>=20.1.0
@@ -65,15 +64,14 @@
 Requires-Dist: sphinx-inline-tabs; extra == "docs"
 Requires-Dist: tomli; python_version < "3.11" and extra == "docs"
 Provides-Extra: tests
 Requires-Dist: fsspec[http]>=2022.8.2; extra == "tests"
 Requires-Dist: lz4>=0.10; extra == "tests"
 Requires-Dist: psutil; extra == "tests"
 Requires-Dist: pytest>=7; extra == "tests"
-Requires-Dist: pytest-doctestplus; extra == "tests"
 Requires-Dist: pytest-remotedata; extra == "tests"
 
 ASDF - Advanced Scientific Data Format
 ======================================
 
 .. _begin-badges:
```

### Comparing `asdf-3.1.0/README.rst` & `asdf-3.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/__init__.py` & `asdf-3.2.0/asdf/__init__.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_asdf.py` & `asdf-3.2.0/asdf/_asdf.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,14 +139,17 @@
             Path to a custom schema file that will be used for a secondary
             validation pass. This can be used to ensure that particular ASDF
             files follow custom conventions beyond those enforced by the
             standard.
         """
         self._fname = ""
 
+        # make a new AsdfVersion instance here so files don't share the same instance
+        self._file_format_version = versioning.AsdfVersion(versioning._FILE_FORMAT_VERSION)
+
         # Don't use the version setter here; it tries to access
         # the extensions, which haven't been assigned yet.
         if version is None:
             self._version = versioning.AsdfVersion(get_config().default_version)
         else:
             self._version = versioning.AsdfVersion(validate_version(version))
 
@@ -163,16 +166,14 @@
         self._ignore_unrecognized_tag = ignore_unrecognized_tag
         self._ignore_implicit_conversion = ignore_implicit_conversion
 
         # Set of (string, string) tuples representing tag version mismatches
         # that we've already warned about for this file.
         self._warned_tag_pairs = set()
 
-        self._file_format_version = None
-
         # Context of a call to treeutil.walk_and_modify, needed in the AsdfFile
         # in case walk_and_modify is re-entered by extension code (via
         # custom_tree_to_tagged_tree or tagged_tree_to_custom_tree).
         self._tree_modification_context = treeutil._TreeModificationContext()
 
         self._fd = None
         self._closed = False
@@ -254,15 +255,19 @@
         -------
         str
         """
         return str(self._version)
 
     @property
     def version_map(self):
-        return versioning.get_version_map(self.version_string)
+        warnings.warn(
+            "AsdfFile.version_map is deprecated. Please use the extension_manager",
+            AsdfDeprecationWarning,
+        )
+        return versioning._get_version_map(self.version_string)
 
     @property
     def extensions(self):
         """
         Get the list of user extensions that are enabled for
         use with this AsdfFile.
 
@@ -466,17 +471,14 @@
                     tree["history"]["extensions"][i] = ext_meta
                     break
             else:
                 tree["history"]["extensions"].append(ext_meta)
 
     @property
     def file_format_version(self):
-        if self._file_format_version is None:
-            return versioning.AsdfVersion(self.version_map["FILE_FORMAT"])
-
         return self._file_format_version
 
     def close(self):
         """
         Close the file handles associated with the `asdf.AsdfFile`.
         """
         if self._fd and not self._closed:
@@ -744,14 +746,18 @@
 
         try:
             version = versioning.AsdfVersion(parts[1].decode("ascii"))
         except ValueError as err:
             msg = f"Unparsable version in ASDF file: {parts[1]}"
             raise ValueError(msg) from err
 
+        if version != versioning._FILE_FORMAT_VERSION:
+            msg = f"Unsupported ASDF file format version {version}"
+            raise ValueError(msg)
+
         return version
 
     @classmethod
     def _read_comment_section(cls, fd):
         """
         Reads the comment section, between the header line and the
         Tree or first block.
@@ -819,21 +825,23 @@
             self._fname = self._fd._uri if self._fd._uri else ""
             try:
                 header_line = fd.read_until(b"\r?\n", 2, "newline", include=True)
             except DelimiterNotFoundError as e:
                 msg = "Does not appear to be a ASDF file."
                 raise ValueError(msg) from e
             self._file_format_version = cls._parse_header_line(header_line)
-            self.version = self._file_format_version
 
             self._comments = cls._read_comment_section(fd)
 
             version = cls._find_asdf_version_in_comments(self._comments)
             if version is not None:
                 self.version = version
+            else:
+                # If no ASDF_STANDARD comment is found...
+                self.version = versioning.AsdfVersion("1.0.0")
 
             # Now that version is set for good, we can add any additional
             # extensions, which may have narrow ASDF Standard version
             # requirements.
             if extensions:
                 self.extensions = extensions
 
@@ -927,15 +935,15 @@
             if close_on_fail:
                 generic_file.close()
             raise
 
     def _write_tree(self, tree, fd, pad_blocks):
         fd.write(constants.ASDF_MAGIC)
         fd.write(b" ")
-        fd.write(self.version_map["FILE_FORMAT"].encode("ascii"))
+        fd.write(f"{self.file_format_version}".encode("ascii"))
         fd.write(b"\n")
 
         fd.write(b"#")
         fd.write(constants.ASDF_STANDARD_COMMENT)
         fd.write(b" ")
         fd.write(self.version_string.encode("ascii"))
         fd.write(b"\n")
```

### Comparing `asdf-3.1.0/asdf/_block/__init__.py` & `asdf-3.2.0/asdf/_block/__init__.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_block/callback.py` & `asdf-3.2.0/asdf/_block/callback.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_block/external.py` & `asdf-3.2.0/asdf/_block/external.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_block/io.py` & `asdf-3.2.0/asdf/_block/io.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_block/key.py` & `asdf-3.2.0/asdf/_block/key.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_block/manager.py` & `asdf-3.2.0/asdf/_block/manager.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_block/options.py` & `asdf-3.2.0/asdf/_block/options.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_block/reader.py` & `asdf-3.2.0/asdf/_block/reader.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_block/store.py` & `asdf-3.2.0/asdf/_block/store.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_block/writer.py` & `asdf-3.2.0/asdf/_block/writer.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_compression.py` & `asdf-3.2.0/asdf/_compression.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_convenience.py` & `asdf-3.2.0/asdf/_convenience.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_core/_converters/complex.py` & `asdf-3.2.0/asdf/_core/_converters/complex.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_core/_converters/external_reference.py` & `asdf-3.2.0/asdf/_core/_converters/external_reference.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_core/_converters/integer.py` & `asdf-3.2.0/asdf/_core/_converters/integer.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_core/_converters/ndarray.py` & `asdf-3.2.0/asdf/_core/_converters/ndarray.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 class NDArrayConverter(Converter):
     tags = [
         "tag:stsci.edu:asdf/core/ndarray-1.0.0",
         "tag:stsci.edu:asdf/core/ndarray-1.1.0",
     ]
     types = [
         np.ndarray,  # we use the type here so the extension can find the sub-classes
+        "numpy.ma.MaskedArray",  # in numpy 2.0
         "numpy.ma.core.MaskedArray",
         "asdf.tags.core.ndarray.NDArrayType",
         "asdf.tags.core.stream.Stream",
     ]
 
     def to_yaml_tree(self, obj, tag, ctx):
         import numpy as np
```

### Comparing `asdf-3.1.0/asdf/_core/_converters/reference.py` & `asdf-3.2.0/asdf/_core/_converters/reference.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_core/_converters/tree.py` & `asdf-3.2.0/asdf/_core/_converters/tree.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_core/_extensions.py` & `asdf-3.2.0/asdf/_core/_extensions.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_core/_validators/ndarray.py` & `asdf-3.2.0/asdf/_core/_validators/ndarray.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_display.py` & `asdf-3.2.0/asdf/_display.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_entry_points.py` & `asdf-3.2.0/asdf/_entry_points.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_extern/RangeHTTPServer.py` & `asdf-3.2.0/asdf/_extern/RangeHTTPServer.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_extern/atomicfile.py` & `asdf-3.2.0/asdf/_extern/atomicfile.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_helpers.py` & `asdf-3.2.0/asdf/_helpers.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/COPYING` & `asdf-3.2.0/asdf/_jsonschema/COPYING`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/__init__.py` & `asdf-3.2.0/asdf/_jsonschema/__init__.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/_format.py` & `asdf-3.2.0/asdf/_jsonschema/_format.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/_legacy_validators.py` & `asdf-3.2.0/asdf/_jsonschema/_legacy_validators.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/_types.py` & `asdf-3.2.0/asdf/_jsonschema/_types.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/_utils.py` & `asdf-3.2.0/asdf/_jsonschema/_utils.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/_validators.py` & `asdf-3.2.0/asdf/_jsonschema/_validators.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/exceptions.py` & `asdf-3.2.0/asdf/_jsonschema/exceptions.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/.gitignore` & `asdf-3.2.0/asdf/_jsonschema/json/.gitignore`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/CONTRIBUTING.md` & `asdf-3.2.0/asdf/_jsonschema/json/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/LICENSE` & `asdf-3.2.0/asdf/_jsonschema/json/LICENSE`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/README.md` & `asdf-3.2.0/asdf/_jsonschema/json/README.md`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/bin/jsonschema_suite` & `asdf-3.2.0/asdf/_jsonschema/json/bin/jsonschema_suite`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/remotes/draft-next/extendible-dynamic-ref.json` & `asdf-3.2.0/asdf/_jsonschema/json/remotes/draft-next/extendible-dynamic-ref.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/remotes/draft2019-09/extendible-dynamic-ref.json` & `asdf-3.2.0/asdf/_jsonschema/json/remotes/draft2019-09/extendible-dynamic-ref.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/remotes/draft2020-12/extendible-dynamic-ref.json` & `asdf-3.2.0/asdf/_jsonschema/json/remotes/draft2020-12/extendible-dynamic-ref.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/test-schema.json` & `asdf-3.2.0/asdf/_jsonschema/json/test-schema.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/additionalProperties.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/additionalProperties.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/allOf.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/allOf.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/anchor.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/anchor.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/anyOf.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/anyOf.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/boolean_schema.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/boolean_schema.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/const.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/const.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/contains.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/contains.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/content.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/content.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/default.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/default.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/defs.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/defs.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/dependentRequired.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/dependentRequired.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/dependentSchemas.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/dependentSchemas.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/dynamicRef.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/dynamicRef.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/enum.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/enum.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/exclusiveMaximum.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/exclusiveMaximum.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/exclusiveMinimum.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/exclusiveMinimum.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/format.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/format.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/id.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/id.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/if-then-else.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/if-then-else.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/infinite-loop-detection.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/infinite-loop-detection.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/items.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/items.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/maxContains.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/maxContains.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/maxItems.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/maxItems.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/maxLength.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/maxLength.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/maxProperties.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/maxProperties.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/maximum.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/maximum.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/minContains.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/minContains.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/minItems.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/minItems.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/minLength.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/minLength.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/minProperties.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/minProperties.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/minimum.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/minimum.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/multipleOf.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/multipleOf.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/not.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/not.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/oneOf.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/oneOf.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/optional/bignum.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/optional/bignum.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/optional/dependencies-compatibility.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/optional/dependencies-compatibility.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/optional/ecmascript-regex.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/optional/ecmascript-regex.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/optional/format/date-time.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/optional/format/date-time.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/optional/format/date.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/optional/format/date.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/optional/format/duration.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/optional/format/duration.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/optional/format/email.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/optional/format/email.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/optional/format/hostname.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/optional/format/hostname.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/optional/format/idn-email.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/optional/format/idn-email.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/optional/format/idn-hostname.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/optional/format/idn-hostname.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/optional/format/ipv4.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/optional/format/ipv4.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/optional/format/ipv6.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/optional/format/ipv6.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/optional/format/iri-reference.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/optional/format/iri-reference.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/optional/format/iri.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/optional/format/iri.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/optional/format/json-pointer.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/optional/format/json-pointer.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/optional/format/regex.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/optional/format/regex.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/optional/format/relative-json-pointer.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/optional/format/relative-json-pointer.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/optional/format/time.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/optional/format/time.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/optional/format/uri-reference.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/optional/format/uri-reference.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/optional/format/uri-template.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/optional/format/uri-template.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/optional/format/uri.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/optional/format/uri.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/optional/format/uuid.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/optional/format/uuid.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/optional/format-assertion.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/optional/format-assertion.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/optional/non-bmp-regex.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/optional/non-bmp-regex.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/optional/refOfUnknownKeyword.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/optional/refOfUnknownKeyword.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/pattern.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/pattern.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/patternProperties.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/patternProperties.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/prefixItems.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/prefixItems.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/properties.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/properties.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/propertyDependencies.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/propertyDependencies.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/propertyNames.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/propertyNames.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/ref.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/ref.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/refRemote.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/refRemote.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/required.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/required.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/type.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/type.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/unevaluatedItems.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/unevaluatedItems.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/unevaluatedProperties.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/unevaluatedProperties.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/uniqueItems.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/uniqueItems.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/unknownKeyword.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/unknownKeyword.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft-next/vocabulary.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft-next/vocabulary.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/additionalItems.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/additionalItems.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/additionalProperties.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/additionalProperties.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/allOf.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/allOf.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/anchor.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/anchor.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/anyOf.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/anyOf.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/boolean_schema.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/boolean_schema.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/const.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/const.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/contains.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/contains.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/content.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/content.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/default.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/default.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/defs.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/defs.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/dependentRequired.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/dependentRequired.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/dependentSchemas.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/dependentSchemas.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/enum.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/enum.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/exclusiveMaximum.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/exclusiveMaximum.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/exclusiveMinimum.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/exclusiveMinimum.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/format.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/format.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/id.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/id.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/if-then-else.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/if-then-else.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/infinite-loop-detection.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/infinite-loop-detection.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/items.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/items.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/maxContains.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/maxContains.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/maxItems.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/maxItems.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/maxLength.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/maxLength.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/maxProperties.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/maxProperties.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/maximum.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/maximum.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/minContains.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/minContains.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/minItems.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/minItems.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/minLength.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/minLength.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/minProperties.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/minProperties.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/minimum.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/minimum.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/multipleOf.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/multipleOf.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/not.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/not.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/oneOf.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/oneOf.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/optional/bignum.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/optional/bignum.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/optional/cross-draft.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/optional/cross-draft.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/optional/dependencies-compatibility.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/optional/dependencies-compatibility.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/optional/ecmascript-regex.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/optional/ecmascript-regex.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/date-time.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/date-time.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/date.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/date.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/duration.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/duration.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/email.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/email.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/hostname.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/hostname.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/idn-email.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/idn-email.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/idn-hostname.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/idn-hostname.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/ipv4.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/ipv4.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/ipv6.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/ipv6.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/iri-reference.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/iri-reference.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/iri.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/iri.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/json-pointer.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/json-pointer.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/regex.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/regex.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/relative-json-pointer.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/relative-json-pointer.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/time.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/time.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/unknown.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/unknown.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/uri-reference.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/uri-reference.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/uri-template.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/uri-template.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/uri.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/uri.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/uuid.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/optional/format/uuid.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/optional/no-schema.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/optional/no-schema.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/optional/non-bmp-regex.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/optional/non-bmp-regex.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/optional/refOfUnknownKeyword.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/optional/refOfUnknownKeyword.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/pattern.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/pattern.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/patternProperties.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/patternProperties.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/properties.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/properties.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/propertyNames.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/propertyNames.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/recursiveRef.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/recursiveRef.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/ref.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/ref.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/refRemote.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/refRemote.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/required.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/required.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/type.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/type.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/unevaluatedItems.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/unevaluatedItems.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/unevaluatedProperties.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/unevaluatedProperties.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/uniqueItems.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/uniqueItems.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/unknownKeyword.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/unknownKeyword.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2019-09/vocabulary.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2019-09/vocabulary.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/additionalProperties.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/additionalProperties.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/allOf.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/allOf.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/anchor.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/anchor.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/anyOf.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/anyOf.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/boolean_schema.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/boolean_schema.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/const.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/const.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/contains.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/contains.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/content.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/content.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/default.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/default.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/defs.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/defs.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/dependentRequired.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/dependentRequired.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/dependentSchemas.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/dependentSchemas.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/dynamicRef.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/dynamicRef.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/enum.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/enum.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/exclusiveMaximum.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/exclusiveMaximum.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/exclusiveMinimum.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/exclusiveMinimum.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/format.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/format.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/id.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/id.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/if-then-else.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/if-then-else.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/infinite-loop-detection.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/infinite-loop-detection.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/items.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/items.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/maxContains.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/maxContains.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/maxItems.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/maxItems.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/maxLength.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/maxLength.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/maxProperties.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/maxProperties.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/maximum.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/maximum.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/minContains.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/minContains.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/minItems.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/minItems.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/minLength.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/minLength.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/minProperties.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/minProperties.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/minimum.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/minimum.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/multipleOf.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/multipleOf.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/not.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/not.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/oneOf.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/oneOf.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/optional/bignum.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/optional/bignum.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/optional/cross-draft.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/optional/cross-draft.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/optional/dependencies-compatibility.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/optional/dependencies-compatibility.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/optional/ecmascript-regex.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/optional/ecmascript-regex.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/date-time.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/date-time.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/date.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/date.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/duration.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/duration.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/email.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/email.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/hostname.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/hostname.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/idn-email.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/idn-email.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/idn-hostname.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/idn-hostname.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/ipv4.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/ipv4.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/ipv6.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/ipv6.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/iri-reference.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/iri-reference.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/iri.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/iri.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/json-pointer.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/json-pointer.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/regex.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/regex.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/relative-json-pointer.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/relative-json-pointer.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/time.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/time.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/unknown.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/unknown.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/uri-reference.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/uri-reference.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/uri-template.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/uri-template.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/uri.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/uri.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/uuid.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format/uuid.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format-assertion.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/optional/format-assertion.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/optional/no-schema.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/optional/no-schema.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/optional/non-bmp-regex.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/optional/non-bmp-regex.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/optional/refOfUnknownKeyword.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/optional/refOfUnknownKeyword.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/pattern.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/pattern.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/patternProperties.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/patternProperties.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/prefixItems.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/prefixItems.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/properties.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/properties.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/propertyNames.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/propertyNames.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/ref.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/ref.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/refRemote.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/refRemote.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/required.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/required.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/type.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/type.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/unevaluatedItems.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/unevaluatedItems.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/unevaluatedProperties.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/unevaluatedProperties.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/uniqueItems.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/uniqueItems.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/unknownKeyword.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/unknownKeyword.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft2020-12/vocabulary.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft2020-12/vocabulary.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/additionalItems.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/additionalItems.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/additionalProperties.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/additionalProperties.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/default.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/default.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/dependencies.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/dependencies.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/disallow.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/disallow.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/divisibleBy.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/divisibleBy.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/enum.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/enum.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/extends.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/extends.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/format.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/format.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/infinite-loop-detection.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/infinite-loop-detection.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/items.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/items.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/maxItems.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/maxItems.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/maxLength.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/maxLength.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/maximum.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/maximum.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/minItems.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/minItems.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/minLength.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/minLength.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/minimum.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/minimum.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/optional/bignum.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/optional/bignum.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/optional/format/color.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/optional/format/color.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/optional/format/date-time.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/optional/format/date-time.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/optional/format/date.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/optional/format/date.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/optional/format/email.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/optional/format/email.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/optional/format/host-name.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/optional/format/host-name.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/optional/format/ip-address.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/optional/format/ip-address.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/optional/format/ipv6.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/optional/format/ipv6.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/optional/format/uri.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/optional/format/uri.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/optional/non-bmp-regex.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/optional/non-bmp-regex.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/pattern.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/pattern.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/patternProperties.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/patternProperties.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/properties.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/properties.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/ref.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/ref.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/refRemote.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/refRemote.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/required.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/required.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/type.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/type.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft3/uniqueItems.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft3/uniqueItems.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/additionalItems.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/additionalItems.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/additionalProperties.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/additionalProperties.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/allOf.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/allOf.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/anyOf.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/anyOf.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/default.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/default.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/definitions.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/definitions.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/dependencies.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/dependencies.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/enum.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/enum.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/format.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/format.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/id.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/id.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/infinite-loop-detection.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/infinite-loop-detection.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/items.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/items.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/maxItems.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/maxItems.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/maxLength.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/maxLength.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/maxProperties.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/maxProperties.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/maximum.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/maximum.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/minItems.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/minItems.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/minLength.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/minLength.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/minProperties.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/minProperties.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/minimum.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/minimum.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/multipleOf.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/multipleOf.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/not.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/not.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/oneOf.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/oneOf.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/optional/bignum.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/optional/bignum.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/optional/ecmascript-regex.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/optional/ecmascript-regex.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/optional/format/date-time.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/optional/format/date-time.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/optional/format/email.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/optional/format/email.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/optional/format/hostname.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/optional/format/hostname.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/optional/format/ipv4.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/optional/format/ipv4.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/optional/format/ipv6.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/optional/format/ipv6.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/optional/format/unknown.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/optional/format/unknown.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/optional/format/uri.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/optional/format/uri.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/optional/non-bmp-regex.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/optional/non-bmp-regex.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/pattern.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/pattern.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/patternProperties.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/patternProperties.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/properties.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/properties.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/ref.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/ref.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/refRemote.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/refRemote.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/required.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/required.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/type.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/type.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft4/uniqueItems.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft4/uniqueItems.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/additionalItems.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/additionalItems.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/additionalProperties.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/additionalProperties.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/allOf.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/allOf.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/anyOf.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/anyOf.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/boolean_schema.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/boolean_schema.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/const.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/const.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/contains.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/contains.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/default.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/default.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/definitions.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/definitions.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/dependencies.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/dependencies.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/enum.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/enum.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/exclusiveMaximum.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/exclusiveMaximum.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/exclusiveMinimum.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/exclusiveMinimum.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/format.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/format.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/id.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/id.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/infinite-loop-detection.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/infinite-loop-detection.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/items.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/items.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/maxItems.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/maxItems.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/maxLength.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/maxLength.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/maxProperties.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/maxProperties.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/maximum.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/maximum.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/minItems.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/minItems.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/minLength.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/minLength.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/minProperties.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/minProperties.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/minimum.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/minimum.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/multipleOf.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/multipleOf.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/not.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/not.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/oneOf.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/oneOf.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/optional/bignum.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/optional/bignum.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/optional/ecmascript-regex.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/optional/ecmascript-regex.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/optional/format/date-time.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/optional/format/date-time.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/optional/format/email.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/optional/format/email.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/optional/format/hostname.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/optional/format/hostname.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/optional/format/ipv4.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/optional/format/ipv4.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/optional/format/ipv6.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/optional/format/ipv6.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/optional/format/json-pointer.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/optional/format/json-pointer.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/optional/format/unknown.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/optional/format/unknown.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/optional/format/uri-reference.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/optional/format/uri-reference.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/optional/format/uri-template.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/optional/format/uri-template.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/optional/format/uri.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/optional/format/uri.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/optional/non-bmp-regex.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/optional/non-bmp-regex.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/pattern.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/pattern.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/patternProperties.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/patternProperties.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/properties.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/properties.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/propertyNames.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/propertyNames.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/ref.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/ref.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/refRemote.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/refRemote.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/required.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/required.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/type.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/type.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/uniqueItems.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/uniqueItems.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft6/unknownKeyword.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft6/unknownKeyword.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/additionalItems.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/additionalItems.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/additionalProperties.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/additionalProperties.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/allOf.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/allOf.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/anyOf.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/anyOf.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/boolean_schema.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/boolean_schema.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/const.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/const.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/contains.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/contains.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/default.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/default.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/definitions.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/definitions.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/dependencies.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/dependencies.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/enum.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/enum.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/exclusiveMaximum.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/exclusiveMaximum.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/exclusiveMinimum.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/exclusiveMinimum.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/format.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/format.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/id.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/id.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/if-then-else.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/if-then-else.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/infinite-loop-detection.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/infinite-loop-detection.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/items.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/items.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/maxItems.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/maxItems.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/maxLength.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/maxLength.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/maxProperties.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/maxProperties.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/maximum.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/maximum.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/minItems.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/minItems.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/minLength.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/minLength.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/minProperties.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/minProperties.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/minimum.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/minimum.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/multipleOf.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/multipleOf.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/not.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/not.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/oneOf.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/oneOf.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/optional/bignum.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/optional/bignum.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/optional/content.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/optional/content.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/optional/cross-draft.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/optional/cross-draft.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/optional/ecmascript-regex.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/optional/ecmascript-regex.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/optional/format/date-time.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/optional/format/date-time.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/optional/format/date.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/optional/format/date.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/optional/format/email.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/optional/format/email.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/optional/format/hostname.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/optional/format/hostname.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/optional/format/idn-email.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/optional/format/idn-email.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/optional/format/idn-hostname.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/optional/format/idn-hostname.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/optional/format/ipv4.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/optional/format/ipv4.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/optional/format/ipv6.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/optional/format/ipv6.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/optional/format/iri-reference.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/optional/format/iri-reference.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/optional/format/iri.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/optional/format/iri.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/optional/format/json-pointer.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/optional/format/json-pointer.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/optional/format/regex.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/optional/format/regex.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/optional/format/relative-json-pointer.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/optional/format/relative-json-pointer.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/optional/format/time.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/optional/format/time.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/optional/format/unknown.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/optional/format/unknown.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/optional/format/uri-reference.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/optional/format/uri-reference.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/optional/format/uri-template.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/optional/format/uri-template.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/optional/format/uri.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/optional/format/uri.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/optional/non-bmp-regex.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/optional/non-bmp-regex.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/pattern.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/pattern.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/patternProperties.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/patternProperties.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/properties.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/properties.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/propertyNames.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/propertyNames.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/ref.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/ref.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/refRemote.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/refRemote.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/required.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/required.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/type.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/type.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/uniqueItems.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/uniqueItems.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/draft7/unknownKeyword.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/draft7/unknownKeyword.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/additionalProperties.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/additionalProperties.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/allOf.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/allOf.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/anchor.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/anchor.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/anyOf.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/anyOf.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/boolean_schema.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/boolean_schema.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/const.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/const.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/contains.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/contains.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/content.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/content.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/default.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/default.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/defs.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/defs.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/dependentRequired.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/dependentRequired.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/dependentSchemas.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/dependentSchemas.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/dynamicRef.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/dynamicRef.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/enum.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/enum.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/exclusiveMaximum.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/exclusiveMaximum.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/exclusiveMinimum.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/exclusiveMinimum.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/format.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/format.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/id.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/id.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/if-then-else.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/if-then-else.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/infinite-loop-detection.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/infinite-loop-detection.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/items.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/items.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/maxContains.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/maxContains.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/maxItems.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/maxItems.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/maxLength.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/maxLength.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/maxProperties.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/maxProperties.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/maximum.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/maximum.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/minContains.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/minContains.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/minItems.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/minItems.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/minLength.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/minLength.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/minProperties.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/minProperties.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/minimum.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/minimum.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/multipleOf.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/multipleOf.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/not.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/not.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/oneOf.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/oneOf.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/optional/bignum.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/optional/bignum.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/optional/cross-draft.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/optional/cross-draft.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/optional/dependencies-compatibility.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/optional/dependencies-compatibility.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/optional/ecmascript-regex.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/optional/ecmascript-regex.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/optional/format/date-time.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/optional/format/date-time.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/optional/format/date.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/optional/format/date.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/optional/format/duration.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/optional/format/duration.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/optional/format/email.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/optional/format/email.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/optional/format/hostname.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/optional/format/hostname.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/optional/format/idn-email.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/optional/format/idn-email.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/optional/format/idn-hostname.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/optional/format/idn-hostname.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/optional/format/ipv4.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/optional/format/ipv4.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/optional/format/ipv6.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/optional/format/ipv6.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/optional/format/iri-reference.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/optional/format/iri-reference.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/optional/format/iri.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/optional/format/iri.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/optional/format/json-pointer.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/optional/format/json-pointer.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/optional/format/regex.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/optional/format/regex.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/optional/format/relative-json-pointer.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/optional/format/relative-json-pointer.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/optional/format/time.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/optional/format/time.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/optional/format/unknown.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/optional/format/unknown.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/optional/format/uri-reference.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/optional/format/uri-reference.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/optional/format/uri-template.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/optional/format/uri-template.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/optional/format/uri.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/optional/format/uri.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/optional/format/uuid.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/optional/format/uuid.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/optional/format-assertion.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/optional/format-assertion.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/optional/no-schema.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/optional/no-schema.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/optional/non-bmp-regex.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/optional/non-bmp-regex.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/optional/refOfUnknownKeyword.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/optional/refOfUnknownKeyword.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/pattern.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/pattern.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/patternProperties.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/patternProperties.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/prefixItems.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/prefixItems.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/properties.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/properties.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/propertyNames.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/propertyNames.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/ref.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/ref.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/refRemote.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/refRemote.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/required.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/required.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/type.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/type.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/unevaluatedItems.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/unevaluatedItems.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/unevaluatedProperties.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/unevaluatedProperties.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/uniqueItems.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/uniqueItems.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/unknownKeyword.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/unknownKeyword.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/json/tests/latest/vocabulary.json` & `asdf-3.2.0/asdf/_jsonschema/json/tests/latest/vocabulary.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/protocols.py` & `asdf-3.2.0/asdf/_jsonschema/protocols.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/schemas/draft2019-09.json` & `asdf-3.2.0/asdf/_jsonschema/schemas/draft2019-09.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/schemas/draft2020-12.json` & `asdf-3.2.0/asdf/_jsonschema/schemas/draft2020-12.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/schemas/draft3.json` & `asdf-3.2.0/asdf/_jsonschema/schemas/draft3.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/schemas/draft4.json` & `asdf-3.2.0/asdf/_jsonschema/schemas/draft4.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/schemas/draft6.json` & `asdf-3.2.0/asdf/_jsonschema/schemas/draft6.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/schemas/draft7.json` & `asdf-3.2.0/asdf/_jsonschema/schemas/draft7.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/schemas/vocabularies/draft2019-09/applicator` & `asdf-3.2.0/asdf/_jsonschema/schemas/vocabularies/draft2019-09/applicator`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/schemas/vocabularies/draft2019-09/content` & `asdf-3.2.0/asdf/_jsonschema/schemas/vocabularies/draft2019-09/content`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/schemas/vocabularies/draft2019-09/core` & `asdf-3.2.0/asdf/_jsonschema/schemas/vocabularies/draft2019-09/core`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/schemas/vocabularies/draft2019-09/meta-data` & `asdf-3.2.0/asdf/_jsonschema/schemas/vocabularies/draft2019-09/meta-data`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/schemas/vocabularies/draft2019-09/validation` & `asdf-3.2.0/asdf/_jsonschema/schemas/vocabularies/draft2019-09/validation`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/schemas/vocabularies/draft2020-12/applicator` & `asdf-3.2.0/asdf/_jsonschema/schemas/vocabularies/draft2020-12/applicator`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/schemas/vocabularies/draft2020-12/content` & `asdf-3.2.0/asdf/_jsonschema/schemas/vocabularies/draft2020-12/content`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/schemas/vocabularies/draft2020-12/core` & `asdf-3.2.0/asdf/_jsonschema/schemas/vocabularies/draft2020-12/core`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/schemas/vocabularies/draft2020-12/meta-data` & `asdf-3.2.0/asdf/_jsonschema/schemas/vocabularies/draft2020-12/meta-data`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/schemas/vocabularies/draft2020-12/validation` & `asdf-3.2.0/asdf/_jsonschema/schemas/vocabularies/draft2020-12/validation`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/tests/_helpers.py` & `asdf-3.2.0/asdf/_jsonschema/tests/_helpers.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/tests/_suite.py` & `asdf-3.2.0/asdf/_jsonschema/tests/_suite.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/tests/test_deprecations.py` & `asdf-3.2.0/asdf/_jsonschema/tests/test_deprecations.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/tests/test_exceptions.py` & `asdf-3.2.0/asdf/_jsonschema/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/tests/test_format.py` & `asdf-3.2.0/asdf/_jsonschema/tests/test_format.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/tests/test_jsonschema_test_suite.py` & `asdf-3.2.0/asdf/_jsonschema/tests/test_jsonschema_test_suite.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/tests/test_types.py` & `asdf-3.2.0/asdf/_jsonschema/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/tests/test_utils.py` & `asdf-3.2.0/asdf/_jsonschema/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/tests/test_validators.py` & `asdf-3.2.0/asdf/_jsonschema/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_jsonschema/validators.py` & `asdf-3.2.0/asdf/_jsonschema/validators.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_node_info.py` & `asdf-3.2.0/asdf/_node_info.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/__init__.py` & `asdf-3.2.0/asdf/_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/_block/test_callback.py` & `asdf-3.2.0/asdf/_tests/_block/test_callback.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/_block/test_external.py` & `asdf-3.2.0/asdf/_tests/_block/test_external.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/_block/test_io.py` & `asdf-3.2.0/asdf/_tests/_block/test_io.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/_block/test_key.py` & `asdf-3.2.0/asdf/_tests/_block/test_key.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/_block/test_manager.py` & `asdf-3.2.0/asdf/_tests/_block/test_manager.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/_block/test_options.py` & `asdf-3.2.0/asdf/_tests/_block/test_options.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/_block/test_reader.py` & `asdf-3.2.0/asdf/_tests/_block/test_reader.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/_block/test_store.py` & `asdf-3.2.0/asdf/_tests/_block/test_store.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/_block/test_writer.py` & `asdf-3.2.0/asdf/_tests/_block/test_writer.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/_helpers.py` & `asdf-3.2.0/asdf/_tests/_helpers.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,43 +16,32 @@
 
 try:
     from astropy.coordinates.representation import CartesianDifferential
 except ImportError:
     CartesianDifferential = None
 
 import numpy as np
-import yaml
 
 import asdf
-from asdf import generic_io, versioning
 from asdf._asdf import AsdfFile, _get_asdf_library_info
-from asdf.constants import YAML_TAG_PREFIX
 from asdf.exceptions import AsdfConversionWarning
 from asdf.tags.core import AsdfObject
-from asdf.versioning import (
-    AsdfVersion,
-    asdf_standard_development_version,
-    get_version_map,
-    split_tag_version,
-    supported_versions,
-)
 
 from .httpserver import RangeHTTPServer
 
 try:
     from pytest_remotedata.disable_internet import INTERNET_OFF
 except ImportError:
     INTERNET_OFF = False
 
 
 __all__ = [
     "get_test_data_path",
     "assert_tree_match",
     "assert_roundtrip_tree",
-    "yaml_to_asdf",
     "get_file_sizes",
     "display_warnings",
 ]
 
 
 def get_test_data_path(name, module=None):
     if module is None:
@@ -282,65 +271,14 @@
         for block in ff._blocks.blocks:
             assert block._data is not None and not callable(block._data)
         assert_tree_match(tree, ff.tree, ff, funcname=tree_match_func)
         if asdf_check_func:
             asdf_check_func(ff)
 
 
-def yaml_to_asdf(yaml_content, yaml_headers=True, standard_version=None):
-    """
-    Given a string of YAML content, adds the extra pre-
-    and post-amble to make it an ASDF file.
-
-    Parameters
-    ----------
-    yaml_content : string
-
-    yaml_headers : bool, optional
-        When True (default) add the standard ASDF YAML headers.
-
-    Returns
-    -------
-    buff : io.BytesIO()
-        A file-like object containing the ASDF-like content.
-    """
-    if isinstance(yaml_content, str):
-        yaml_content = yaml_content.encode("utf-8")
-
-    buff = io.BytesIO()
-
-    if standard_version is None:
-        standard_version = versioning.default_version
-
-    standard_version = AsdfVersion(standard_version)
-
-    vm = get_version_map(standard_version)
-    file_format_version = vm["FILE_FORMAT"]
-    yaml_version = vm["YAML_VERSION"]
-    tree_version = vm["tags"]["tag:stsci.edu:asdf/core/asdf"]
-
-    if yaml_headers:
-        buff.write(
-            f"""#ASDF {file_format_version}
-#ASDF_STANDARD {standard_version}
-%YAML {yaml_version}
-%TAG ! tag:stsci.edu:asdf/
---- !core/asdf-{tree_version}
-""".encode(
-                "ascii",
-            ),
-        )
-    buff.write(yaml_content)
-    if yaml_headers:
-        buff.write(b"\n...\n")
-
-    buff.seek(0)
-    return buff
-
-
 def get_file_sizes(dirname):
     """
     Get the file sizes in a directory.
 
     Parameters
     ----------
     dirname : string
@@ -404,66 +342,7 @@
     else:
         with pytest.warns(Warning) as recorded_warnings:
             yield
 
         assert not any(isinstance(w.message, warning_class) for w in recorded_warnings), display_warnings(
             recorded_warnings,
         )
-
-
-def _assert_extension_type_correctness(extension, extension_type, resolver):
-    __tracebackhide__ = True
-
-    if extension_type.yaml_tag is not None and extension_type.yaml_tag.startswith(YAML_TAG_PREFIX):
-        return
-
-    if extension_type == asdf.Stream:
-        # Stream is a special case.  It was implemented as a subclass of NDArrayType,
-        # but shares a tag with that class, so it isn't really a distinct type.
-        return
-
-    assert extension_type.name is not None, f"{extension_type.__name__} must set the 'name' class attribute"
-
-    # Currently ExtensionType sets a default version of 1.0.0,
-    # but we want to encourage an explicit version on the subclass.
-    assert "version" in extension_type.__dict__, f"{extension_type.__name__} must set the 'version' class attribute"
-
-    # check the default version
-    types_to_check = [extension_type]
-
-    # Adding or updating a schema/type version might involve updating multiple
-    # packages. This can result in types without schema and schema without types
-    # for the development version of the asdf-standard. To account for this,
-    # don't include versioned siblings of types with versions that are not
-    # in one of the asdf-standard versions in supported_versions (excluding the
-    # current development version).
-    asdf_standard_versions = supported_versions.copy()
-    if asdf_standard_development_version in asdf_standard_versions:
-        asdf_standard_versions.remove(asdf_standard_development_version)
-    for sibling in extension_type.versioned_siblings:
-        tag_base, version = split_tag_version(sibling.yaml_tag)
-        for asdf_standard_version in asdf_standard_versions:
-            vm = get_version_map(asdf_standard_version)
-            if tag_base in vm["tags"] and AsdfVersion(vm["tags"][tag_base]) == version:
-                types_to_check.append(sibling)
-                break
-
-    for check_type in types_to_check:
-        schema_location = resolver(check_type.yaml_tag)
-
-        assert schema_location is not None, (
-            f"{extension_type.__name__} supports tag, {check_type.yaml_tag}, "
-            "but tag does not resolve.  Check the tag_mapping and uri_mapping "
-            f"properties on the related extension ({extension_type.__name__})."
-        )
-
-        if schema_location not in asdf.get_config().resource_manager:
-            try:
-                with generic_io.get_file(schema_location) as f:
-                    yaml.safe_load(f.read())
-            except Exception as err:
-                msg = (
-                    f"{extension_type.__name__} supports tag, {check_type.yaml_tag}, "
-                    f"which resolves to schema at {schema_location}, but "
-                    "schema cannot be read."
-                )
-                raise AssertionError(msg) from err
```

### Comparing `asdf-3.1.0/asdf/_tests/_regtests/test_1013.py` & `asdf-3.2.0/asdf/_tests/_regtests/test_1013.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/_regtests/test_1523.py` & `asdf-3.2.0/asdf/_tests/_regtests/test_1523.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/_regtests/test_1525.py` & `asdf-3.2.0/asdf/_tests/_regtests/test_1525.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/_regtests/test_1526.py` & `asdf-3.2.0/asdf/_tests/_regtests/test_1526.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/_regtests/test_1530.py` & `asdf-3.2.0/asdf/_tests/_regtests/test_1530.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/_regtests/test_1539.py` & `asdf-3.2.0/asdf/_tests/_regtests/test_1539.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/_regtests/test_1540.py` & `asdf-3.2.0/asdf/_tests/_regtests/test_1540.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/_regtests/test_1541.py` & `asdf-3.2.0/asdf/_tests/_regtests/test_1541.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/_regtests/test_1542.py` & `asdf-3.2.0/asdf/_tests/_regtests/test_1542.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/_regtests/test_1558.py` & `asdf-3.2.0/asdf/_tests/_regtests/test_1558.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/commands/tests/data/block0.asdf` & `asdf-3.2.0/asdf/_tests/commands/tests/data/block0.asdf`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/commands/tests/data/block1.asdf` & `asdf-3.2.0/asdf/_tests/commands/tests/data/block1.asdf`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/commands/tests/data/frames.diff` & `asdf-3.2.0/asdf/_tests/commands/tests/data/frames.diff`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/commands/tests/data/frames0.asdf` & `asdf-3.2.0/asdf/_tests/commands/tests/data/frames0.asdf`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/commands/tests/data/frames1.asdf` & `asdf-3.2.0/asdf/_tests/commands/tests/data/frames1.asdf`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/commands/tests/data/frames_ignore_asdf_library.diff` & `asdf-3.2.0/asdf/_tests/commands/tests/data/frames_ignore_asdf_library.diff`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/commands/tests/data/ndarray0.asdf` & `asdf-3.2.0/asdf/_tests/commands/tests/data/ndarray0.asdf`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/commands/tests/data/ndarray1.asdf` & `asdf-3.2.0/asdf/_tests/commands/tests/data/ndarray1.asdf`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/commands/tests/data/ndarray_in_list0.asdf` & `asdf-3.2.0/asdf/_tests/commands/tests/data/ndarray_in_list0.asdf`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/commands/tests/data/ndarray_in_list1.asdf` & `asdf-3.2.0/asdf/_tests/commands/tests/data/ndarray_in_list1.asdf`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/commands/tests/test_defragment.py` & `asdf-3.2.0/asdf/_tests/commands/tests/test_defragment.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/commands/tests/test_diff.py` & `asdf-3.2.0/asdf/_tests/commands/tests/test_diff.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/commands/tests/test_edit.py` & `asdf-3.2.0/asdf/_tests/commands/tests/test_edit.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/commands/tests/test_exploded.py` & `asdf-3.2.0/asdf/_tests/commands/tests/test_exploded.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/commands/tests/test_extension.py` & `asdf-3.2.0/asdf/_tests/commands/tests/test_extension.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/commands/tests/test_info.py` & `asdf-3.2.0/asdf/_tests/commands/tests/test_info.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/commands/tests/test_tags.py` & `asdf-3.2.0/asdf/_tests/commands/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/commands/tests/test_to_yaml.py` & `asdf-3.2.0/asdf/_tests/commands/tests/test_to_yaml.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/conftest.py` & `asdf-3.2.0/asdf/_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/core/_converters/test_complex.py` & `asdf-3.2.0/asdf/_tests/core/_converters/test_complex.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/core/_converters/test_tree.py` & `asdf-3.2.0/asdf/_tests/core/_converters/test_tree.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/core/tests/test_integration.py` & `asdf-3.2.0/asdf/_tests/core/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/data/custom_schema.yaml` & `asdf-3.2.0/asdf/_tests/data/custom_schema.yaml`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/data/example_schema.json` & `asdf-3.2.0/asdf/_tests/data/example_schema.json`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/data/fraction-1.0.0.yaml` & `asdf-3.2.0/asdf/_tests/data/fraction-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/httpserver.py` & `asdf-3.2.0/asdf/_tests/httpserver.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/tags/core/tests/test_integer.py` & `asdf-3.2.0/asdf/_tests/tags/core/tests/test_integer.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/tags/core/tests/test_ndarray.py` & `asdf-3.2.0/asdf/_tests/tags/core/tests/test_ndarray.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,17 +113,17 @@
     max_ndim: 2""",
             }
         )
         yield
 
 
 @contextlib.contextmanager
-def roundtrip(af, raw=False):
+def roundtrip(af, raw=False, standard_version=None):
     if not isinstance(af, asdf.AsdfFile):
-        af = asdf.AsdfFile(af)
+        af = asdf.AsdfFile(af, version=standard_version)
     b = io.BytesIO()
     af.write_to(b)
     b.seek(0)
     if raw:
         bs = b.read()
         if asdf.constants.BLOCK_MAGIC in bs:
             bs, *_ = bs.split(asdf.constants.BLOCK_MAGIC)
@@ -167,29 +167,22 @@
             assert my_tree["bigendian"].dtype.byteorder == ">"
             assert my_tree["little"].dtype.byteorder == "="
         else:
             assert my_tree["bigendian"].dtype.byteorder == "="
             assert my_tree["little"].dtype.byteorder == "<"
 
 
-def test_all_dtypes(tmp_path):
+@pytest.mark.parametrize("dtype", ndarray._datatype_names.values())
+def test_all_dtypes(dtype):
+    standard_version = "1.6.0" if dtype == "f2" else None
     tree = {}
     for byteorder in (">", "<"):
-        for dtype in ndarray._datatype_names.values():
-            # Python 3 can't expose these dtypes in non-native byte
-            # order, because it's using the new Python buffer
-            # interface.
-            if dtype in ("c32", "f16"):
-                continue
-
-            arr = np.array([True, False]) if dtype == "b1" else np.arange(0, 10, dtype=str(byteorder + dtype))
-
-            tree[byteorder + dtype] = arr
-
-    with roundtrip(tree) as af:
+        arr = np.array([True, False]) if dtype == "b1" else np.arange(0, 10, dtype=str(byteorder + dtype))
+        tree[byteorder + dtype] = arr
+    with roundtrip(tree, standard_version=standard_version) as af:
         for k in tree:
             pre = tree[k]
             post = af[k]
             assert_array_equal(pre, post)
 
 
 def test_dont_load_data():
```

### Comparing `asdf-3.1.0/asdf/_tests/test_api.py` & `asdf-3.2.0/asdf/_tests/test_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,17 @@
 import pytest
 from numpy.testing import assert_array_equal
 
 import asdf
 from asdf import config_context, get_config, treeutil, versioning
 from asdf.exceptions import AsdfDeprecationWarning, AsdfWarning, ValidationError
 from asdf.extension import ExtensionProxy
+from asdf.testing.helpers import yaml_to_asdf
 
-from ._helpers import assert_no_warnings, assert_roundtrip_tree, assert_tree_match, yaml_to_asdf
+from ._helpers import assert_no_warnings, assert_roundtrip_tree, assert_tree_match
 
 RNG = np.random.default_rng(97)
 
 
 def test_get_data_from_closed_file(tmp_path):
     path = str(tmp_path / "test.asdf")
 
@@ -117,19 +118,19 @@
         ff.write_to(tmpfile)
 
 
 def test_default_version():
     """
     See https://github.com/asdf-format/asdf/issues/364
     """
-
-    version_map = versioning.get_version_map(versioning.default_version)
-
     ff = asdf.AsdfFile()
-    assert ff.file_format_version == version_map["FILE_FORMAT"]
+    assert ff.file_format_version == versioning._FILE_FORMAT_VERSION
+
+    # make sure these are different AsdfVersion instances
+    assert ff.file_format_version is not versioning._FILE_FORMAT_VERSION
 
 
 def test_update_exceptions(tmp_path):
     path = str(tmp_path / "test.asdf")
 
     my_array = RNG.normal(size=(8, 8))
     tree = {"my_array": my_array}
```

### Comparing `asdf-3.1.0/asdf/_tests/test_array_blocks.py` & `asdf-3.2.0/asdf/_tests/test_array_blocks.py`

 * *Files 0% similar despite different names*

```diff
@@ -745,22 +745,21 @@
     # incorrectly pointing to a non-block offset
     buff.seek(0)
     bs = buff.read()
     block_index_header_start = bs.index(constants.INDEX_HEADER)
     block_index_start = block_index_header_start + len(constants.INDEX_HEADER)
     block_index = yaml.load(bs[block_index_start:], yaml.SafeLoader)
     block_index[block_index_index] -= 4
-    yaml_version = tuple(int(x) for x in ff.version_map["YAML_VERSION"].split("."))
     buff.seek(block_index_start)
     yaml.dump(
         block_index,
         stream=buff,
         explicit_start=True,
         explicit_end=True,
-        version=yaml_version,
+        version=asdf.versioning._YAML_VERSION,
         allow_unicode=True,
         encoding="utf-8",
     )
 
     buff.seek(0)
     with pytest.warns(AsdfBlockIndexWarning, match="Invalid block index contents"):
         with asdf.open(buff) as ff:
```

### Comparing `asdf-3.1.0/asdf/_tests/test_asdf.py` & `asdf-3.2.0/asdf/_tests/test_asdf.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import os
 
 import pytest
 
 from asdf import config_context
 from asdf._asdf import AsdfFile, open_asdf
 from asdf._entry_points import get_extensions
-from asdf._tests._helpers import assert_no_warnings, assert_tree_match, yaml_to_asdf
-from asdf.exceptions import AsdfWarning
+from asdf._tests._helpers import assert_no_warnings, assert_tree_match
+from asdf.exceptions import AsdfDeprecationWarning, AsdfWarning
 from asdf.extension import ExtensionProxy
+from asdf.testing.helpers import yaml_to_asdf
 from asdf.versioning import AsdfVersion
 
 
 def test_no_warnings_get_extensions():
     """
     Smoke test for changes to the `importlib.metadata` entry points API.
     """
@@ -99,18 +100,20 @@
         with pytest.raises(ValueError, match=r"ASDF Standard version .* is not supported by asdf==.*"):
             af.version = "0.5.4"
 
         with pytest.raises(ValueError, match=r"ASDF Standard version .* is not supported by asdf==.*"):
             af.version = AsdfVersion("2.5.4")
 
         af.version = "1.0.0"
-        assert af.version_map["tags"]["tag:stsci.edu:asdf/core/asdf"] == "1.0.0"
+        with pytest.warns(AsdfDeprecationWarning, match="AsdfFile.version_map is deprecated"):
+            assert af.version_map["tags"]["tag:stsci.edu:asdf/core/asdf"] == "1.0.0"
 
         af.version = "1.2.0"
-        assert af.version_map["tags"]["tag:stsci.edu:asdf/core/asdf"] == "1.1.0"
+        with pytest.warns(AsdfDeprecationWarning, match="AsdfFile.version_map is deprecated"):
+            assert af.version_map["tags"]["tag:stsci.edu:asdf/core/asdf"] == "1.1.0"
 
 
 def test_asdf_file_extensions():
     af = AsdfFile()
     assert af.extensions == []
 
     extension = TestExtension(extension_uri="asdf://somewhere.org/extensions/foo-1.0")
@@ -209,121 +212,121 @@
     with config_context() as config:
         config.add_extension(extension_with_uri)
         config.add_extension(extension_without_uri)
         config.add_extension(extension_with_legacy_class_names)
 
         # Test missing history:
         content = """
-        foo: bar
+foo: bar
         """
         buff = yaml_to_asdf(content)
         with assert_no_warnings():
             open_asdf(buff)
 
         # Test the old history format:
         content = """
-        history:
-          - !core/history_entry-1.0.0
-            description: Once upon a time, there was a carnivorous panda.
-          - !core/history_entry-1.0.0
-            description: This entry intentionally left blank.
-        foo: bar
+history:
+  - !core/history_entry-1.0.0
+    description: Once upon a time, there was a carnivorous panda.
+  - !core/history_entry-1.0.0
+    description: This entry intentionally left blank.
+foo: bar
         """
-        buff = yaml_to_asdf(content, standard_version="1.0.0")
+        buff = yaml_to_asdf(content, version="1.0.0")
         with assert_no_warnings():
             open_asdf(buff)
 
         # Test matching by URI:
         content = """
-        history:
-          extensions:
-            - !core/extension_metadata-1.0.0
-              extension_uri: asdf://somewhere.org/extensions/foo-1.0
-              extension_class: some.unrecognized.extension.class.Name
+history:
+  extensions:
+    - !core/extension_metadata-1.0.0
+      extension_uri: asdf://somewhere.org/extensions/foo-1.0
+      extension_class: some.unrecognized.extension.class.Name
         """
         buff = yaml_to_asdf(content)
         with assert_no_warnings():
             open_asdf(buff)
 
         # Test matching by legacy class name:
         content = """
-        history:
-          extensions:
-            - !core/extension_metadata-1.0.0
-              extension_class: some.legacy.class.Name
+history:
+  extensions:
+    - !core/extension_metadata-1.0.0
+      extension_class: some.legacy.class.Name
         """
         buff = yaml_to_asdf(content)
         with assert_no_warnings():
             open_asdf(buff)
 
         # Warn when the URI is missing, even if there's
         # a class name match:
         content = f"""
-        history:
-          extensions:
-            - !core/extension_metadata-1.0.0
-              extension_uri: some-missing-URI
-              extension_class: {extension_with_uri.class_name}
+history:
+  extensions:
+    - !core/extension_metadata-1.0.0
+      extension_uri: some-missing-URI
+      extension_class: {extension_with_uri.class_name}
         """
         buff = yaml_to_asdf(content)
         with pytest.warns(AsdfWarning, match=r"URI 'some-missing-URI'"):
             open_asdf(buff)
 
         # Warn when the class name is missing:
         content = """
-        history:
-          extensions:
-            - !core/extension_metadata-1.0.0
-              extension_class: some.missing.class.Name
+history:
+  extensions:
+    - !core/extension_metadata-1.0.0
+      extension_class: some.missing.class.Name
         """
         buff = yaml_to_asdf(content)
         with pytest.warns(AsdfWarning, match=r"class 'some.missing.class.Name'"):
             open_asdf(buff)
 
         # Warn when the package version is older:
         content = """
-        history:
-          extensions:
-            - !core/extension_metadata-1.0.0
-              extension_uri: asdf://somewhere.org/extensions/foo-1.0
-              extension_class: some.class.Name
-              software: !core/software-1.0.0
-                name: foo
-                version: 9.2.4
+history:
+  extensions:
+    - !core/extension_metadata-1.0.0
+      extension_uri: asdf://somewhere.org/extensions/foo-1.0
+      extension_class: some.class.Name
+      software: !core/software-1.0.0
+        name: foo
+        version: 9.2.4
         """
         buff = yaml_to_asdf(content)
         with pytest.warns(AsdfWarning, match=r"older package"):
             open_asdf(buff)
 
         # Shouldn't warn when the package version is later:
         content = """
-        history:
-          extensions:
-            - !core/extension_metadata-1.0.0
-              extension_uri: asdf://somewhere.org/extensions/foo-1.0
-              extension_class: some.class.Name
-              software: !core/software-1.0.0
-                name: foo
-                version: 0.1.2
+history:
+  extensions:
+    - !core/extension_metadata-1.0.0
+      extension_uri: asdf://somewhere.org/extensions/foo-1.0
+      extension_class: some.class.Name
+      software: !core/software-1.0.0
+        name: foo
+        version: 0.1.2
         """
         buff = yaml_to_asdf(content)
         with assert_no_warnings():
             open_asdf(buff)
 
         # Shouldn't receive a warning when the package
         # name changes, even if the version is later:
         content = """
-        history:
-          extensions:
-            - !core/extension_metadata-1.0.0
-              extension_uri: asdf://somewhere.org/extensions/foo-1.0
-              extension_class: some.class.Name
-              software: !core/software-1.0.0
-                name: bar
-                version: 9.4.5
+history:
+  extensions:
+    - !core/extension_metadata-1.0.0
+      extension_uri: asdf://somewhere.org/extensions/foo-1.0
+      extension_class: some.class.Name
+      software: !core/software-1.0.0
+        name: bar
+        version: 9.4.5
         """
         buff = yaml_to_asdf(content)
         with assert_no_warnings():
             open_asdf(buff)
 
 
 def test_bad_input(tmp_path):
```

### Comparing `asdf-3.1.0/asdf/_tests/test_block_converter.py` & `asdf-3.2.0/asdf/_tests/test_block_converter.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/test_compression.py` & `asdf-3.2.0/asdf/_tests/test_compression.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/test_config.py` & `asdf-3.2.0/asdf/_tests/test_config.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/test_deprecated.py` & `asdf-3.2.0/asdf/_tests/test_deprecated.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,7 +113,13 @@
 
 def test_AsdfFile_init_validation_deprecation():
     with (
         pytest.warns(AsdfDeprecationWarning, match="Validation during AsdfFile.__init__ is deprecated"),
         pytest.raises(ValidationError),
     ):
         asdf.AsdfFile({"history": 42})
+
+
+def test_asdffile_version_map_deprecation():
+    af = asdf.AsdfFile()
+    with pytest.warns(AsdfDeprecationWarning, match="AsdfFile.version_map is deprecated"):
+        af.version_map
```

### Comparing `asdf-3.1.0/asdf/_tests/test_entry_points.py` & `asdf-3.2.0/asdf/_tests/test_entry_points.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/test_extension.py` & `asdf-3.2.0/asdf/_tests/test_extension.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/test_file_format.py` & `asdf-3.2.0/asdf/_tests/test_file_format.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,15 +171,15 @@
     content = b"""#ASDF 0.1.0
 %YAML 1.1
 %TAG ! tag:stsci.edu:asdf/
 --- !core/asdf-0.1.0
 foo : bar
 ..."""
     buff = io.BytesIO(content)
-    with pytest.raises(ValueError, match=r"ASDF Standard version .* is not supported by asdf==.*"), asdf.open(buff):
+    with pytest.raises(ValueError, match=r"Unsupported ASDF file format version*"), asdf.open(buff):
         pass
 
 
 def test_valid_version(tmp_path):
     content = b"""#ASDF 1.0.0
 %YAML 1.1
 %TAG ! tag:stsci.edu:asdf/
```

### Comparing `asdf-3.1.0/asdf/_tests/test_generic_io.py` & `asdf-3.2.0/asdf/_tests/test_generic_io.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/test_history.py` & `asdf-3.2.0/asdf/_tests/test_history.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/test_info.py` & `asdf-3.2.0/asdf/_tests/test_info.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/test_integration.py` & `asdf-3.2.0/asdf/_tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/test_reference.py` & `asdf-3.2.0/asdf/_tests/test_reference.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/test_reference_files.py` & `asdf-3.2.0/asdf/_tests/test_reference_files.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/test_resource.py` & `asdf-3.2.0/asdf/_tests/test_resource.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/test_schema.py` & `asdf-3.2.0/asdf/_tests/test_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 import asdf
 import asdf.testing.helpers
 from asdf import config_context, constants, get_config, schema, tagged, util, yamlutil
 from asdf._tests import _helpers as helpers
 from asdf.exceptions import AsdfConversionWarning, AsdfDeprecationWarning, AsdfWarning, ValidationError
 from asdf.extension import TagDefinition
+from asdf.testing.helpers import yaml_to_asdf
 
 
 @contextlib.contextmanager
 def tag_reference_extension():
     class TagReference:
         def __init__(self, name, things):
             self.name = name
@@ -89,15 +90,15 @@
 tagged: !<{scalar_tag}>
   m
 not_tagged:
   m
     """
     with asdf.config_context() as cfg:
         cfg.add_extension(ScalarExtension())
-        buff = helpers.yaml_to_asdf(yaml)
+        buff = yaml_to_asdf(yaml)
         with asdf.open(buff) as ff:
             assert isinstance(ff.tree["tagged"], Scalar)
             assert not isinstance(ff.tree["not_tagged"], Scalar)
             assert isinstance(ff.tree["not_tagged"], str)
 
             assert ff.tree["tagged"].value == "m"
             assert ff.tree["not_tagged"] == "m"
@@ -446,15 +447,15 @@
         tags = [tag_def]
         converters = [CustomConverter()]
 
     yaml = f"""
 custom: !<{tag_uri}>
   foo
     """
-    buff = helpers.yaml_to_asdf(yaml)
+    buff = yaml_to_asdf(yaml)
     # This should cause a warning but not an error because without explicitly
     # providing an extension, our custom type will not be recognized and will
     # simply be converted to a raw type.
     with pytest.warns(AsdfConversionWarning, match=tag_uri), asdf.open(buff):
         pass
 
     buff.seek(0)
@@ -473,15 +474,15 @@
         # nothing about them.
         yaml = f"""
     array: !core/ndarray-1.0.0
       data: [0, 1, 2]
       custom: !<{tag_uri}>
         foo
         """
-        buff = helpers.yaml_to_asdf(yaml)
+        buff = yaml_to_asdf(yaml)
         with (
             pytest.raises(ValidationError, match=r".* is not of type .*"),
             asdf.open(
                 buff,
             ),
         ):
             pass
@@ -628,15 +629,15 @@
 custom: !<http://nowhere.org/tags/custom/default-1.0.0>
   b: {}
   d: {}
   g: {}
   j:
     l: 362
         """
-        buff = helpers.yaml_to_asdf(yaml)
+        buff = yaml_to_asdf(yaml)
         with asdf.open(buff) as ff:
             assert "a" in ff.tree["custom"]
             assert ff.tree["custom"]["a"] == 42
             assert ff.tree["custom"]["b"]["c"] == 82
             # allOf combiner should fill defaults from all subschemas:
             assert ff.tree["custom"]["d"]["e"] == 122
             assert ff.tree["custom"]["d"]["f"] == 162
@@ -740,30 +741,30 @@
   value: foo
     """
 
     with config_context() as cfg:
         cfg.add_extension(OneOfExtension())
         cfg.add_resource_mapping({schema_uri: tag_schema})
 
-        buff = helpers.yaml_to_asdf(yaml)
+        buff = yaml_to_asdf(yaml)
         with asdf.open(buff) as ff:
             assert ff["one_of"].value == "foo"
 
 
 def test_tag_reference_validation():
     yaml = """
 custom: !<tag:nowhere.org:custom/tag_reference-1.0.0>
   name:
     "Something"
   things: !core/ndarray-1.0.0
     data: [1, 2, 3]
     """
 
     with tag_reference_extension():
-        buff = helpers.yaml_to_asdf(yaml)
+        buff = yaml_to_asdf(yaml)
         with asdf.open(buff) as ff:
             custom = ff.tree["custom"]
             assert custom.name == "Something"
             assert_array_equal(custom.things, [1, 2, 3])
 
 
 def test_foreign_tag_reference_validation():
@@ -816,15 +817,15 @@
     """
 
     with tag_reference_extension():
         cfg = asdf.get_config()
         cfg.add_resource_mapping({schema_uri: tag_schema})
         cfg.add_extension(ForeignTagReferenceExtension())
 
-        buff = helpers.yaml_to_asdf(yaml)
+        buff = yaml_to_asdf(yaml)
         with asdf.open(buff) as ff:
             a = ff.tree["custom"].a
             assert a.name == "Something"
             assert_array_equal(a.things, [1, 2, 3])
 
 
 def test_self_reference_resolution():
@@ -887,22 +888,22 @@
     af.close()
 
 
 @pytest.mark.parametrize("value", [constants.MAX_NUMBER + 1, constants.MIN_NUMBER - 1])
 def test_read_large_literal(value):
     yaml = f"integer: {value}"
 
-    buff = helpers.yaml_to_asdf(yaml)
+    buff = yaml_to_asdf(yaml)
 
     with pytest.warns(AsdfWarning, match=r"Invalid integer literal value"), asdf.open(buff) as af:
         assert af["integer"] == value
 
     yaml = f"{value}: foo"
 
-    buff = helpers.yaml_to_asdf(yaml)
+    buff = yaml_to_asdf(yaml)
 
     with pytest.warns(AsdfWarning, match=r"Invalid integer literal value"), asdf.open(buff) as af:
         assert af[value] == "foo"
 
 
 @pytest.mark.parametrize(
     ("version", "keys"),
```

### Comparing `asdf-3.1.0/asdf/_tests/test_search.py` & `asdf-3.2.0/asdf/_tests/test_search.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/test_serialization_context.py` & `asdf-3.2.0/asdf/_tests/test_serialization_context.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/test_stream.py` & `asdf-3.2.0/asdf/_tests/test_stream.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/test_tagged.py` & `asdf-3.2.0/asdf/_tests/test_tagged.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/test_treeutil.py` & `asdf-3.2.0/asdf/_tests/test_treeutil.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/test_types.py` & `asdf-3.2.0/asdf/_tests/test_types.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import pytest
 
 import asdf
 from asdf.exceptions import AsdfConversionWarning
-
-from . import _helpers as helpers
+from asdf.testing.helpers import yaml_to_asdf
 
 
 def test_undefined_tag():
     # This tests makes sure that ASDF still returns meaningful structured data
     # even when it encounters a schema tag that it does not specifically
     # implement as an extension
     from numpy import array
@@ -19,15 +18,15 @@
     - {'message': 'there is no tag'}
     - !core/ndarray-1.0.0
       [[1, 2, 3], [4, 5, 6]]
     - !<tag:nowhere.org:custom/also_undefined-1.3.0>
         - !core/ndarray-1.0.0 [[7],[8],[9],[10]]
         - !core/complex-1.0.0 3.14j
 """
-    buff = helpers.yaml_to_asdf(yaml)
+    buff = yaml_to_asdf(yaml)
     with pytest.warns(Warning) as warning:
         afile = asdf.open(buff)
         missing = afile.tree["undefined_data"]
 
     assert missing[0] == 5
     assert missing[1] == {"message": "there is no tag"}
     assert (missing[2] == array([[1, 2, 3], [4, 5, 6]])).all()
@@ -42,9 +41,8 @@
         assert (
             str(warning[i].message)
             == f"tag:nowhere.org:custom/{tag} is not recognized, converting to raw Python data structure"
         )
 
     # Make sure no warning occurs if explicitly ignored
     buff.seek(0)
-    with helpers.assert_no_warnings():
-        afile = asdf.open(buff, ignore_unrecognized_tag=True)
+    afile = asdf.open(buff, ignore_unrecognized_tag=True)
```

### Comparing `asdf-3.1.0/asdf/_tests/test_util.py` & `asdf-3.2.0/asdf/_tests/test_util.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/test_versioning.py` & `asdf-3.2.0/asdf/_tests/test_versioning.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/_tests/test_yaml.py` & `asdf-3.2.0/asdf/_tests/test_yaml.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import numpy as np
 import pytest
 import yaml
 
 import asdf
 from asdf import tagged, treeutil, yamlutil
 from asdf.exceptions import AsdfConversionWarning, AsdfWarning
+from asdf.testing.helpers import yaml_to_asdf
 
 from . import _helpers as helpers
 
 
 def test_ordered_dict(tmp_path):
     """
     Test that we can write out and read in ordered dicts.
@@ -195,22 +196,23 @@
             if node != asdf.tree:
                 assert not isinstance(node, tagged.Tagged)
 
     helpers.assert_roundtrip_tree(tree, tmp_path, asdf_check_func=check_asdf)
 
 
 def test_explicit_tags():
-    yaml = f"""#ASDF {asdf.versioning.default_version}
+    yaml = b"""#ASDF 1.0.0
+#ASDF_STANDARD 1.5.0
 %YAML 1.1
 --- !<tag:stsci.edu:asdf/core/asdf-1.1.0>
 foo: !<tag:stsci.edu:asdf/core/ndarray-1.0.0> [1, 2, 3]
 ..."""
 
     # Check that fully qualified explicit tags work
-    buff = helpers.yaml_to_asdf(yaml, yaml_headers=False)
+    buff = io.BytesIO(yaml)
 
     with asdf.open(buff) as ff:
         assert all(ff.tree["foo"] == [1, 2, 3])
 
 
 def test_yaml_internal_reference(tmp_path):
     """
@@ -316,20 +318,16 @@
     [
         "  1: a",  # not a sequence
         "- !!omap\n  - 1",  # sequence item, not a mapping
         "- !!omap\n  1: a\n  2: a",  # sequence item, not a one element mapping
     ],
 )
 def test_invalid_omap(payload):
-    test_yaml = f"""#ASDF {asdf.versioning.default_version}
-%YAML 1.1
---- !<tag:stsci.edu:asdf/core/asdf-1.1.0>
-od: !!omap
-{payload}
-..."""
+    test_yaml = f"""od: !!omap
+{payload}"""
 
     # Check that fully qualified explicit tags work
-    buff = helpers.yaml_to_asdf(test_yaml, yaml_headers=False)
+    buff = yaml_to_asdf(test_yaml)
 
     with pytest.raises(yaml.constructor.ConstructorError):
         with asdf.open(buff) as ff:
             ff["od"]
```

### Comparing `asdf-3.1.0/asdf/commands/defragment.py` & `asdf-3.2.0/asdf/commands/defragment.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/commands/diff.py` & `asdf-3.2.0/asdf/commands/diff.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/commands/edit.py` & `asdf-3.2.0/asdf/commands/edit.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/commands/exploded.py` & `asdf-3.2.0/asdf/commands/exploded.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/commands/extension.py` & `asdf-3.2.0/asdf/commands/extension.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/commands/info.py` & `asdf-3.2.0/asdf/commands/info.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/commands/main.py` & `asdf-3.2.0/asdf/commands/main.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/commands/tags.py` & `asdf-3.2.0/asdf/commands/tags.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/commands/to_yaml.py` & `asdf-3.2.0/asdf/commands/to_yaml.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/config.py` & `asdf-3.2.0/asdf/config.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/conftest.py` & `asdf-3.2.0/asdf/conftest.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/constants.py` & `asdf-3.2.0/asdf/constants.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/exceptions.py` & `asdf-3.2.0/asdf/exceptions.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/extension/__init__.py` & `asdf-3.2.0/asdf/extension/__init__.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/extension/_compressor.py` & `asdf-3.2.0/asdf/extension/_compressor.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/extension/_converter.py` & `asdf-3.2.0/asdf/extension/_converter.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/extension/_extension.py` & `asdf-3.2.0/asdf/extension/_extension.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/extension/_manager.py` & `asdf-3.2.0/asdf/extension/_manager.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/extension/_manifest.py` & `asdf-3.2.0/asdf/extension/_manifest.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/extension/_serialization_context.py` & `asdf-3.2.0/asdf/extension/_serialization_context.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/extension/_tag.py` & `asdf-3.2.0/asdf/extension/_tag.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/extension/_validator.py` & `asdf-3.2.0/asdf/extension/_validator.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/generic_io.py` & `asdf-3.2.0/asdf/generic_io.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/reference.py` & `asdf-3.2.0/asdf/reference.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/resource.py` & `asdf-3.2.0/asdf/resource.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/schema.py` & `asdf-3.2.0/asdf/schema.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/search.py` & `asdf-3.2.0/asdf/search.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/tagged.py` & `asdf-3.2.0/asdf/tagged.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/tags/core/__init__.py` & `asdf-3.2.0/asdf/tags/core/__init__.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/tags/core/external_reference.py` & `asdf-3.2.0/asdf/tags/core/external_reference.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/tags/core/integer.py` & `asdf-3.2.0/asdf/tags/core/integer.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/tags/core/ndarray.py` & `asdf-3.2.0/asdf/tags/core/ndarray.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     "int16": "i2",
     "int32": "i4",
     "int64": "i8",
     "uint8": "u1",
     "uint16": "u2",
     "uint32": "u4",
     "uint64": "u8",
+    "float16": "f2",
     "float32": "f4",
     "float64": "f8",
     "complex64": "c8",
     "complex128": "c16",
     "bool8": "b1",
 }
```

### Comparing `asdf-3.1.0/asdf/tags/core/stream.py` & `asdf-3.2.0/asdf/tags/core/stream.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/testing/helpers.py` & `asdf-3.2.0/asdf/testing/helpers.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/treeutil.py` & `asdf-3.2.0/asdf/treeutil.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/asdf/util.py` & `asdf-3.2.0/asdf/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -467,15 +467,15 @@
         ...     def wiggle(self):
         ...         "Wiggle the thingamajig"
         ...         pass
         >>> class B(A):
         ...     def wiggle(self):
         ...         pass
         >>> B.wiggle.__doc__
-        u'Wiggle the thingamajig'
+        'Wiggle the thingamajig'
     """
 
     def __init__(cls, name, bases, dct):
         def is_public_member(key):
             return (key.startswith("__") and key.endswith("__") and len(key) > 4) or not key.startswith("_")
 
         for key, val in dct.items():
```

### Comparing `asdf-3.1.0/asdf/versioning.py` & `asdf-3.2.0/asdf/versioning.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     """
     return f"{name}-{version}"
 
 
 _version_map = {}
 
 
-def get_version_map(version):
+def _get_version_map(version):
     version_map = _version_map.get(version)
 
     if version_map is None:
         from .config import get_config
 
         uri = f"http://stsci.edu/schemas/asdf/version_map-{version}"
         # The following call to yaml.load is safe because we're
@@ -170,7 +170,14 @@
 # mapping keys to string, integer, and boolean only.
 RESTRICTED_KEYS_MIN_VERSION = AsdfVersion("1.6.0")
 
 
 # This library never removed defaults for ASDF Standard versions
 # later than 1.5.0, so filling them isn't necessary.
 FILL_DEFAULTS_MAX_VERSION = AsdfVersion("1.5.0")
+
+# ASDF currently only defined a single file format version
+_FILE_FORMAT_VERSION = AsdfVersion("1.0.0")
+
+# ASDF currently only supports a single yaml version
+# use a tuple as that is what yaml expects
+_YAML_VERSION = (1, 1)
```

### Comparing `asdf-3.1.0/asdf/yamlutil.py` & `asdf-3.2.0/asdf/yamlutil.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import yaml
 
 from . import config, schema, tagged, treeutil, util
 from .constants import STSCI_SCHEMA_TAG_BASE, YAML_TAG_PREFIX
 from .exceptions import AsdfConversionWarning
 from .extension._serialization_context import BlockAccess
 from .tags.core import AsdfObject
-from .versioning import _yaml_base_loader
+from .versioning import _YAML_VERSION, _yaml_base_loader
 
 __all__ = ["custom_tree_to_tagged_tree", "tagged_tree_to_custom_tree"]
 
 
 _yaml_base_dumper = yaml.CSafeDumper if getattr(yaml, "__with_libyaml__", None) else yaml.SafeDumper
 
 
@@ -392,27 +392,25 @@
 
     tags = {"!": STSCI_SCHEMA_TAG_BASE + "/"}
     tree = custom_tree_to_tagged_tree(tree, ctx, _serialization_context=_serialization_context)
     if tree_finalizer is not None:
         tree_finalizer(tree)
     schema.validate(tree, ctx)
 
-    yaml_version = tuple(int(x) for x in ctx.version_map["YAML_VERSION"].split("."))
-
     # add yaml %TAG definitions from extensions
     if _serialization_context:
         for ext in _serialization_context._extensions_used:
             for key, val in ext.yaml_tag_handles.items():
                 if key not in tags:
                     tags[key] = val
 
     yaml.dump_all(
         [tree],
         stream=fd,
         Dumper=AsdfDumper,
         explicit_start=True,
         explicit_end=True,
-        version=yaml_version,
+        version=_YAML_VERSION,
         allow_unicode=True,
         encoding="utf-8",
         tags=tags,
     )
```

### Comparing `asdf-3.1.0/asdf.egg-info/PKG-INFO` & `asdf-3.2.0/asdf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asdf
-Version: 3.1.0
+Version: 3.2.0
 Summary: Python implementation of the ASDF Standard
 Author-email: The ASDF Developers <help@stsci.edu>
 License: BSD 3-Clause License
         
         Copyright (c) 2021 Association of Universities for Research in Astronomy.
         All rights reserved.
         
@@ -43,17 +43,16 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: asdf-standard>=1.0.1
+Requires-Dist: asdf-standard>=1.1.0
 Requires-Dist: asdf-transform-schemas>=0.3
-Requires-Dist: asdf-unit-schemas>=0.1
 Requires-Dist: importlib-metadata>=4.11.4
 Requires-Dist: jmespath>=0.6.2
 Requires-Dist: numpy>=1.22
 Requires-Dist: packaging>=19
 Requires-Dist: pyyaml>=5.4.1
 Requires-Dist: semantic_version>=2.8
 Requires-Dist: attrs>=20.1.0
@@ -65,15 +64,14 @@
 Requires-Dist: sphinx-inline-tabs; extra == "docs"
 Requires-Dist: tomli; python_version < "3.11" and extra == "docs"
 Provides-Extra: tests
 Requires-Dist: fsspec[http]>=2022.8.2; extra == "tests"
 Requires-Dist: lz4>=0.10; extra == "tests"
 Requires-Dist: psutil; extra == "tests"
 Requires-Dist: pytest>=7; extra == "tests"
-Requires-Dist: pytest-doctestplus; extra == "tests"
 Requires-Dist: pytest-remotedata; extra == "tests"
 
 ASDF - Advanced Scientific Data Format
 ======================================
 
 .. _begin-badges:
```

### Comparing `asdf-3.1.0/asdf.egg-info/SOURCES.txt` & `asdf-3.2.0/asdf.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -845,14 +845,15 @@
 compatibility_tests/README.md
 compatibility_tests/assert_file_correct.py
 compatibility_tests/common.py
 compatibility_tests/generate_file.py
 compatibility_tests/test_file_compatibility.py
 docs/Makefile
 docs/conf.py
+docs/conftest.py
 docs/index.rst
 docs/make.bat
 docs/rtd_environment.yaml
 docs/_static/logo.ico
 docs/_static/logo.pdf
 docs/_static/logo.png
 docs/asdf/CODE_OF_CONDUCT.rst
```

### Comparing `asdf-3.1.0/benchmarks/_utils.py` & `asdf-3.2.0/benchmarks/_utils.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/benchmarks/asdf.py` & `asdf-3.2.0/benchmarks/asdf.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/benchmarks/schema.py` & `asdf-3.2.0/benchmarks/schema.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/benchmarks/yamlutil.py` & `asdf-3.2.0/benchmarks/yamlutil.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/compatibility_tests/README.md` & `asdf-3.2.0/compatibility_tests/README.md`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/compatibility_tests/common.py` & `asdf-3.2.0/compatibility_tests/common.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/compatibility_tests/generate_file.py` & `asdf-3.2.0/compatibility_tests/generate_file.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/compatibility_tests/test_file_compatibility.py` & `asdf-3.2.0/compatibility_tests/test_file_compatibility.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,14 +32,19 @@
 # ASDF library versions older than this version would sometimes write newer
 # tags that were not listed in the supported standard
 MIN_VERSION_1_0_0_STANDARD = Version("2.7.0")
 
 GENERATE_SCRIPT_PATH = Path(__file__).parent / "generate_file.py"
 ASSERT_SCRIPT_PATH = Path(__file__).parent / "assert_file_correct.py"
 
+# Starting at this version ndarray tag version 1.1.0 is supported
+# this is required for asdf standard 1.6.0 or later
+NDARRAY_1_1_0_ASDF_VERSION = Version("2.14.0")
+NDARRAY_1_1_0_STANDARD_VERSION = AsdfVersion("1.6.0")
+
 
 @contextmanager
 def internet_temporarily_enabled(verbose=False):
     """
     Context manager that temporarily enables pytest_remotedata
     internet.
     """
@@ -181,14 +186,20 @@
     if asdf_version < MIN_VERSION_1_0_0_STANDARD:
         standard_versions.remove(AsdfVersion("1.0.0"))
 
     # Confirm that this test isn't giving us a false sense of security.
     assert len(standard_versions) > 0
 
     for standard_version in sorted(standard_versions):
+        # older versions of asdf reported support for 1.6.0 (the development
+        # version of the standard) yet did not support the tags in that
+        # version.
+        if standard_version >= NDARRAY_1_1_0_STANDARD_VERSION:
+            if asdf_version < NDARRAY_1_1_0_ASDF_VERSION:
+                continue
         # Confirm that a file generated by the current version of the code
         # can be read by the older version of the library.
         if asdf_version >= MIN_VERSION_NEW_FILES:
             current_file_path = Path(str(tmp_path)) / "test-current.asdf"
             generate_file(current_file_path, standard_version)
             assert env_run(env_path, "python3", ASSERT_SCRIPT_PATH, current_file_path, capture_output=True), (
                 f"asdf library version {asdf_version} failed to read an ASDF Standard {standard_version} "
```

### Comparing `asdf-3.1.0/docs/Makefile` & `asdf-3.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/docs/_static/logo.ico` & `asdf-3.2.0/docs/_static/logo.ico`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/docs/_static/logo.pdf` & `asdf-3.2.0/docs/_static/logo.pdf`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/docs/_static/logo.png` & `asdf-3.2.0/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/docs/asdf/CODE_OF_CONDUCT.rst` & `asdf-3.2.0/docs/asdf/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/docs/asdf/arrays.rst` & `asdf-3.2.0/docs/asdf/arrays.rst`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/docs/asdf/asdf_tool.rst` & `asdf-3.2.0/docs/asdf/asdf_tool.rst`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/docs/asdf/config.rst` & `asdf-3.2.0/docs/asdf/config.rst`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/docs/asdf/deprecations.rst` & `asdf-3.2.0/docs/asdf/deprecations.rst`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/docs/asdf/developer_api.rst` & `asdf-3.2.0/docs/asdf/developer_api.rst`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/docs/asdf/developer_overview.rst` & `asdf-3.2.0/docs/asdf/developer_overview.rst`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/docs/asdf/extending/compressors.rst` & `asdf-3.2.0/docs/asdf/extending/compressors.rst`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/docs/asdf/extending/converters.rst` & `asdf-3.2.0/docs/asdf/extending/converters.rst`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/docs/asdf/extending/extensions.rst` & `asdf-3.2.0/docs/asdf/extending/extensions.rst`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/docs/asdf/extending/manifests.rst` & `asdf-3.2.0/docs/asdf/extending/manifests.rst`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/docs/asdf/extending/resources.rst` & `asdf-3.2.0/docs/asdf/extending/resources.rst`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/docs/asdf/extending/schemas.rst` & `asdf-3.2.0/docs/asdf/extending/schemas.rst`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
           - tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
       unit:
         description: The unit corresponding to the values
         tag: tag:stsci.edu:asdf/unit/unit-1.0.0
       required: [value, unit]
     ...
 
-This is similar to the quantity schema, found :ref:`here <asdf-standard:unit-schema>`, of the ASDF Standard, but
+This is similar to the quantity schema, found :ref:`here <asdf-standard:stsci.edu/asdf/unit/quantity-1.1.0>`, of the ASDF Standard, but
 has been updated to reflect current recommendations regarding schemas.
 Let's walk through this schema line by line.
 
 .. code-block:: yaml
     :linenos:
 
     %YAML 1.1
@@ -299,8 +299,8 @@
 See also:
 =========
 
 - `JSON Schema Draft 4 <https://json-schema.org/specification-links.html#draft-4>`_
 
 - `Understanding JSON Schema <https://json-schema.org/understanding-json-schema/>`_
 
-- :ref:`Unit Schemas <asdf-standard:unit-schema>`
+- :ref:`Unit Schemas <asdf-standard:stsci.edu/asdf/unit/quantity-1.1.0>`
```

### Comparing `asdf-3.1.0/docs/asdf/extending/uris.rst` & `asdf-3.2.0/docs/asdf/extending/uris.rst`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/docs/asdf/extending/use_cases.rst` & `asdf-3.2.0/docs/asdf/extending/use_cases.rst`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/docs/asdf/extending/validators.rst` & `asdf-3.2.0/docs/asdf/extending/validators.rst`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/docs/asdf/features.rst` & `asdf-3.2.0/docs/asdf/features.rst`

 * *Files 2% similar despite different names*

```diff
@@ -219,20 +219,27 @@
 file format, and core tags.  However, since deserializing custom tags
 requires other software packages, backwards compatibility is often
 contingent on the available versions of such software packages.
 
 In general, forward compatibility with newer versions of the ASDF Standard and
 ASDF file format is not supported by the software.
 
-When creating new ASDF files, it is possible to control the version of the file
-format that is used. This can be specified by passing the ``version`` argument to
+When creating new ASDF files, it is possible to control the version of the ASDF
+standard that is used. This can be specified by passing the ``version`` argument to
 either the `AsdfFile` constructor when the file object is created, or to the
-`AsdfFile.write_to` method when it is written. By default, the latest version
-of the file format will be used. Note that this option has no effect on the
-versions of tags from custom extensions.
+`AsdfFile.write_to` method when it is written. By default, the latest stable
+version of the ASDF standard will be used.
+
+.. warning::
+   Take care when providing ``version`` to `AsdfFile.write_to` to select a version
+   that is stable. Writing files with a ``development`` (unstable) version may
+   produce files that will become unreadable as that version evolves. The default
+   version will always be stable and is often the best choice unless you are trying
+   to write out a file that is readable by older software (where you will want to
+   use an older, stable version).
 
 External References
 ===================
 
 Tree References
 ---------------
```

### Comparing `asdf-3.1.0/docs/asdf/install.rst` & `asdf-3.2.0/docs/asdf/install.rst`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/docs/asdf/overview.rst` & `asdf-3.2.0/docs/asdf/overview.rst`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/docs/asdf/release_and_support.rst` & `asdf-3.2.0/docs/asdf/release_and_support.rst`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/docs/asdf/using_extensions.rst` & `asdf-3.2.0/docs/asdf/using_extensions.rst`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/docs/asdf/whats_new.rst` & `asdf-3.2.0/docs/asdf/whats_new.rst`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/docs/conf.py` & `asdf-3.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/docs/index.rst` & `asdf-3.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/docs/make.bat` & `asdf-3.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/licenses/JSONSCHEMA_LICENSE` & `asdf-3.2.0/licenses/JSONSCHEMA_LICENSE`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/licenses/JSON_LICENSE` & `asdf-3.2.0/licenses/JSON_LICENSE`

 * *Files identical despite different names*

### Comparing `asdf-3.1.0/pyproject.toml` & `asdf-3.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -15,17 +15,16 @@
   'Programming Language :: Python :: 3.11',
   'Programming Language :: Python :: 3.12',
 ]
 dynamic = [
   'version',
 ]
 dependencies = [
-  "asdf-standard>=1.0.1",
-  "asdf-transform-schemas>=0.3",
-  "asdf-unit-schemas>=0.1",
+  "asdf-standard>=1.1.0",
+  "asdf-transform-schemas>=0.3",  # required for asdf-1.0.0 schema
   "importlib-metadata>=4.11.4",
   "jmespath>=0.6.2",
   "numpy>=1.22",
   "packaging>=19",
   "pyyaml>=5.4.1",
   "semantic_version>=2.8",
   # for vendorized jsonschema
@@ -43,15 +42,14 @@
   'tomli; python_version < "3.11"',
 ]
 tests = [
   "fsspec[http]>=2022.8.2",
   "lz4>=0.10",
   "psutil",
   "pytest>=7",
-  "pytest-doctestplus",
   "pytest-remotedata",
 ]
 [project.urls]
 'documentation' = 'https://asdf.readthedocs.io/en/stable'
 'repository' = 'https://github.com/asdf-format/asdf'
 'tracker' = 'https://github.com/asdf-format/asdf/issues'
 [project.entry-points]
@@ -75,15 +73,15 @@
 
 [tool.setuptools.package-data]
 'asdf.commands.tests.data' = ["*"]
 'asdf.tags.core.tests.data' = ["*"]
 'asdf.tests.data' = ["*"]
 
 [tool.setuptools_scm]
-write_to = "asdf/_version.py"
+version_file = "asdf/_version.py"
 
 [tool.black]
 line-length = 120
 force-exclude = '''
 ^/(
   (
       \.eggs
@@ -97,26 +95,23 @@
   )/
 )
 '''
 
 [tool.pytest.ini_options]
 testpaths = ['asdf', 'docs']
 minversion = 4.6
-norecursedirs = ['build', 'docs/_build', 'docs/sphinxext']
-doctest_plus = 'enabled'
 remote_data_strict = true
 filterwarnings = [
     'error',
     'ignore:numpy.ndarray size changed:RuntimeWarning',
 ]
-# Configuration for pytest-doctestplus
-text_file_format = 'rst'
 addopts = [
+    '--doctest-modules',
+    '--doctest-glob=*.rst',
     '--color=yes',
-    '--doctest-rst',
     '-rsxfE',
     '-p no:legacypath',
 ]
 
 [tool.coverage.run]
 omit = [
     'asdf/_astropy_init*',
```

### Comparing `asdf-3.1.0/pytest_asdf/plugin.py` & `asdf-3.2.0/pytest_asdf/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,19 +207,19 @@
         result.example = SchemaExample.from_schema(example)
         result.ignore_unrecognized_tag = ignore_unrecognized_tag
         result.ignore_version_mismatch = ignore_version_mismatch
         return result
 
     def runtest(self):
         from asdf import AsdfFile, _block, generic_io, util
-        from asdf._tests import _helpers as helpers
+        from asdf.testing.helpers import yaml_to_asdf
 
         # Make sure that the examples in the schema files (and thus the
         # ASDF standard document) are valid.
-        buff = helpers.yaml_to_asdf("example: " + self.example.example.strip(), standard_version=self.example.version)
+        buff = yaml_to_asdf("example: " + self.example.example.strip(), version=self.example.version)
 
         ff = AsdfFile(
             uri=util.filepath_to_url(os.path.abspath(self.filename)),
             ignore_unrecognized_tag=self.ignore_unrecognized_tag,
             ignore_version_mismatch=self.ignore_version_mismatch,
         )
```

### Comparing `asdf-3.1.0/tox.ini` & `asdf-3.2.0/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -21,16 +21,14 @@
     compatibility: virtualenv
     coverage: coverage
     devdeps: -rrequirements-dev.txt
     numpydev: cython
     oldestdeps: minimum_dependencies
     parallel: pytest-xdist
     pytestdev: git+https://github.com/pytest-dev/pytest
-# released versions of doctestplus aren't compatible with pytest-dev
-    pytestdev: git+https://github.com/scientific-python/pytest-doctestplus
 extras = all,tests
 # astropy will complain if the home directory is missing
 pass_env = HOME
 package = editable
 commands_pre =
     python -m pip install --upgrade pip
 
@@ -113,29 +111,14 @@
     git clone https://github.com/asdf-format/asdf-transform-schemas.git
     pip install -e asdf-transform-schemas[test]
     pip install -r {env_tmp_dir}/requirements.txt
     pip freeze
 commands =
     pytest asdf-transform-schemas
 
-[testenv:asdf-unit-schemas]
-change_dir = {env_tmp_dir}
-allowlist_externals =
-    git
-    bash
-extras =
-commands_pre =
-    bash -c "pip freeze -q | grep 'asdf @' > {env_tmp_dir}/requirements.txt"
-    git clone https://github.com/asdf-format/asdf-unit-schemas.git
-    pip install -e asdf-unit-schemas[test]
-    pip install -r {env_tmp_dir}/requirements.txt
-    pip freeze
-commands =
-    pytest asdf-unit-schemas
-
 [testenv:asdf-wcs-schemas]
 change_dir = {env_tmp_dir}
 allowlist_externals =
     git
     bash
 extras =
 commands_pre =
```

