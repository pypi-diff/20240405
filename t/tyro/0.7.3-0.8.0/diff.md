# Comparing `tmp/tyro-0.7.3.tar.gz` & `tmp/tyro-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tyro-0.7.3.tar", last modified: Fri Feb 16 19:34:01 2024, max compression
+gzip compressed data, was "tyro-0.8.0.tar", last modified: Thu Apr  4 21:56:18 2024, max compression
```

## Comparing `tyro-0.7.3.tar` & `tyro-0.8.0.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 19:34:01.660168 tyro-0.7.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-02-16 19:31:56.000000 tyro-0.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7677 2024-02-16 19:34:01.660168 tyro-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-02-16 19:33:56.000000 tyro-0.7.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-02-16 19:31:56.000000 tyro-0.7.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-16 19:34:01.660168 tyro-0.7.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 19:34:01.644168 tyro-0.7.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 19:34:01.648167 tyro-0.7.3/src/tyro/
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-02-16 19:31:56.000000 tyro-0.7.3/src/tyro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    54269 2024-02-16 19:31:56.000000 tyro-0.7.3/src/tyro/_argparse_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)    22063 2024-02-16 19:31:56.000000 tyro-0.7.3/src/tyro/_arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)    10584 2024-02-16 19:31:56.000000 tyro-0.7.3/src/tyro/_calling.py
--rw-r--r--   0 runner    (1001) docker     (127)    18723 2024-02-16 19:31:56.000000 tyro-0.7.3/src/tyro/_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-02-16 19:31:56.000000 tyro-0.7.3/src/tyro/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)    12909 2024-02-16 19:31:56.000000 tyro-0.7.3/src/tyro/_docstrings.py
--rw-r--r--   0 runner    (1001) docker     (127)    42688 2024-02-16 19:31:56.000000 tyro-0.7.3/src/tyro/_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)    24353 2024-02-16 19:31:56.000000 tyro-0.7.3/src/tyro/_instantiators.py
--rw-r--r--   0 runner    (1001) docker     (127)    25669 2024-02-16 19:31:56.000000 tyro-0.7.3/src/tyro/_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)    13094 2024-02-16 19:31:56.000000 tyro-0.7.3/src/tyro/_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-02-16 19:31:56.000000 tyro-0.7.3/src/tyro/_singleton.py
--rw-r--r--   0 runner    (1001) docker     (127)     5773 2024-02-16 19:31:56.000000 tyro-0.7.3/src/tyro/_strings.py
--rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-02-16 19:31:56.000000 tyro-0.7.3/src/tyro/_subcommand_matching.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-02-16 19:31:56.000000 tyro-0.7.3/src/tyro/_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-02-16 19:31:56.000000 tyro-0.7.3/src/tyro/_unsafe_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 19:34:01.648167 tyro-0.7.3/src/tyro/conf/
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-02-16 19:31:56.000000 tyro-0.7.3/src/tyro/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-02-16 19:31:56.000000 tyro-0.7.3/src/tyro/conf/_confstruct.py
--rw-r--r--   0 runner    (1001) docker     (127)     6263 2024-02-16 19:31:56.000000 tyro-0.7.3/src/tyro/conf/_markers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 19:34:01.652168 tyro-0.7.3/src/tyro/extras/
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-02-16 19:31:56.000000 tyro-0.7.3/src/tyro/extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-02-16 19:31:56.000000 tyro-0.7.3/src/tyro/extras/_base_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-02-16 19:31:56.000000 tyro-0.7.3/src/tyro/extras/_choices_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     8318 2024-02-16 19:31:56.000000 tyro-0.7.3/src/tyro/extras/_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-02-16 19:31:56.000000 tyro-0.7.3/src/tyro/extras/_subcommand_cli_from_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 19:31:56.000000 tyro-0.7.3/src/tyro/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 19:34:01.656168 tyro-0.7.3/src/tyro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7677 2024-02-16 19:34:01.000000 tyro-0.7.3/src/tyro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-02-16 19:34:01.000000 tyro-0.7.3/src/tyro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-16 19:34:01.000000 tyro-0.7.3/src/tyro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-02-16 19:34:01.000000 tyro-0.7.3/src/tyro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-16 19:34:01.000000 tyro-0.7.3/src/tyro.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 19:34:01.656168 tyro-0.7.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-02-16 19:31:56.000000 tyro-0.7.3/tests/test_attrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-02-16 19:31:56.000000 tyro-0.7.3/tests/test_base_configs_nested.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-02-16 19:31:56.000000 tyro-0.7.3/tests/test_boolean_optional.py
--rw-r--r--   0 runner    (1001) docker     (127)    13842 2024-02-16 19:31:56.000000 tyro-0.7.3/tests/test_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-02-16 19:31:56.000000 tyro-0.7.3/tests/test_completion.py
--rw-r--r--   0 runner    (1001) docker     (127)    39462 2024-02-16 19:31:56.000000 tyro-0.7.3/tests/test_conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    18741 2024-02-16 19:31:56.000000 tyro-0.7.3/tests/test_dcargs.py
--rw-r--r--   0 runner    (1001) docker     (127)    18509 2024-02-16 19:31:56.000000 tyro-0.7.3/tests/test_dict_namedtuple.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-02-16 19:31:56.000000 tyro-0.7.3/tests/test_dynamic_dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (127)    14602 2024-02-16 19:31:56.000000 tyro-0.7.3/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-02-16 19:31:56.000000 tyro-0.7.3/tests/test_errors_new_annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-02-16 19:31:56.000000 tyro-0.7.3/tests/test_flax_min_py38.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-02-16 19:31:56.000000 tyro-0.7.3/tests/test_forward_ref.py
--rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-02-16 19:31:56.000000 tyro-0.7.3/tests/test_functools.py
--rw-r--r--   0 runner    (1001) docker     (127)    12358 2024-02-16 19:31:56.000000 tyro-0.7.3/tests/test_generics_and_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)    25731 2024-02-16 19:31:56.000000 tyro-0.7.3/tests/test_helptext.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-02-16 19:31:56.000000 tyro-0.7.3/tests/test_initvar_min_py38.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-02-16 19:31:56.000000 tyro-0.7.3/tests/test_is_nested_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-02-16 19:31:56.000000 tyro-0.7.3/tests/test_missing.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-02-16 19:31:56.000000 tyro-0.7.3/tests/test_missing_optional_packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-02-16 19:31:56.000000 tyro-0.7.3/tests/test_mixed_unions.py
--rw-r--r--   0 runner    (1001) docker     (127)    33891 2024-02-16 19:31:56.000000 tyro-0.7.3/tests/test_nested.py
--rw-r--r--   0 runner    (1001) docker     (127)     9753 2024-02-16 19:31:56.000000 tyro-0.7.3/tests/test_nested_in_containers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-02-16 19:31:56.000000 tyro-0.7.3/tests/test_new_style_annotations_min_py310.py
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-02-16 19:31:56.000000 tyro-0.7.3/tests/test_new_style_annotations_min_py39.py
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-02-16 19:31:56.000000 tyro-0.7.3/tests/test_partial.py
--rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-02-16 19:31:56.000000 tyro-0.7.3/tests/test_positional_min_py38.py
--rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-02-16 19:31:56.000000 tyro-0.7.3/tests/test_pydantic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-02-16 19:31:56.000000 tyro-0.7.3/tests/test_pydantic_with_newtype.py
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-02-16 19:31:56.000000 tyro-0.7.3/tests/test_self_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-02-16 19:31:56.000000 tyro-0.7.3/tests/test_strings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-02-16 19:31:56.000000 tyro-0.7.3/tests/test_tuple_with_subcommands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-02-16 19:31:56.000000 tyro-0.7.3/tests/test_union_from_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-02-16 19:31:56.000000 tyro-0.7.3/tests/test_unsafe_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-02-16 19:31:56.000000 tyro-0.7.3/tests/test_unsupported_but_should_work.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:56:18.215782 tyro-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-04 21:54:25.000000 tyro-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7851 2024-04-04 21:56:18.215782 tyro-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-04-04 21:56:16.000000 tyro-0.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-04-04 21:54:25.000000 tyro-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 21:56:18.215782 tyro-0.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:56:18.199782 tyro-0.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:56:18.203782 tyro-0.8.0/src/tyro/
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-04 21:54:25.000000 tyro-0.8.0/src/tyro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54289 2024-04-04 21:54:25.000000 tyro-0.8.0/src/tyro/_argparse_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22872 2024-04-04 21:54:25.000000 tyro-0.8.0/src/tyro/_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10584 2024-04-04 21:54:25.000000 tyro-0.8.0/src/tyro/_calling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18700 2024-04-04 21:54:25.000000 tyro-0.8.0/src/tyro/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-04 21:54:25.000000 tyro-0.8.0/src/tyro/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12909 2024-04-04 21:54:25.000000 tyro-0.8.0/src/tyro/_docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42889 2024-04-04 21:54:25.000000 tyro-0.8.0/src/tyro/_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24359 2024-04-04 21:54:25.000000 tyro-0.8.0/src/tyro/_instantiators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25673 2024-04-04 21:54:25.000000 tyro-0.8.0/src/tyro/_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13224 2024-04-04 21:54:25.000000 tyro-0.8.0/src/tyro/_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-04 21:54:25.000000 tyro-0.8.0/src/tyro/_singleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5773 2024-04-04 21:54:25.000000 tyro-0.8.0/src/tyro/_strings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-04-04 21:54:25.000000 tyro-0.8.0/src/tyro/_subcommand_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-04 21:54:25.000000 tyro-0.8.0/src/tyro/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-04 21:54:25.000000 tyro-0.8.0/src/tyro/_unsafe_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:56:18.207782 tyro-0.8.0/src/tyro/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-04 21:54:25.000000 tyro-0.8.0/src/tyro/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6852 2024-04-04 21:54:25.000000 tyro-0.8.0/src/tyro/conf/_confstruct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6403 2024-04-04 21:54:25.000000 tyro-0.8.0/src/tyro/conf/_markers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:56:18.207782 tyro-0.8.0/src/tyro/extras/
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-04 21:54:25.000000 tyro-0.8.0/src/tyro/extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-04 21:54:25.000000 tyro-0.8.0/src/tyro/extras/_base_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-04-04 21:54:25.000000 tyro-0.8.0/src/tyro/extras/_choices_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8319 2024-04-04 21:54:25.000000 tyro-0.8.0/src/tyro/extras/_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-04-04 21:54:25.000000 tyro-0.8.0/src/tyro/extras/_subcommand_cli_from_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 21:54:25.000000 tyro-0.8.0/src/tyro/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:56:18.215782 tyro-0.8.0/src/tyro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7851 2024-04-04 21:56:18.000000 tyro-0.8.0/src/tyro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-04 21:56:18.000000 tyro-0.8.0/src/tyro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 21:56:18.000000 tyro-0.8.0/src/tyro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-04 21:56:18.000000 tyro-0.8.0/src/tyro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-04 21:56:18.000000 tyro-0.8.0/src/tyro.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:56:18.215782 tyro-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-04-04 21:54:25.000000 tyro-0.8.0/tests/test_attrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-04-04 21:54:25.000000 tyro-0.8.0/tests/test_base_configs_nested.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-04 21:54:25.000000 tyro-0.8.0/tests/test_boolean_optional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13842 2024-04-04 21:54:25.000000 tyro-0.8.0/tests/test_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-04 21:54:25.000000 tyro-0.8.0/tests/test_completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40475 2024-04-04 21:54:25.000000 tyro-0.8.0/tests/test_conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18741 2024-04-04 21:54:25.000000 tyro-0.8.0/tests/test_dcargs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18509 2024-04-04 21:54:25.000000 tyro-0.8.0/tests/test_dict_namedtuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-04 21:54:25.000000 tyro-0.8.0/tests/test_dynamic_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14602 2024-04-04 21:54:25.000000 tyro-0.8.0/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-04 21:54:25.000000 tyro-0.8.0/tests/test_flax_min_py38.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-04 21:54:25.000000 tyro-0.8.0/tests/test_forward_ref.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-04-04 21:54:25.000000 tyro-0.8.0/tests/test_functools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12768 2024-04-04 21:54:25.000000 tyro-0.8.0/tests/test_generics_and_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25731 2024-04-04 21:54:25.000000 tyro-0.8.0/tests/test_helptext.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-04 21:54:25.000000 tyro-0.8.0/tests/test_initvar_min_py38.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-04 21:54:25.000000 tyro-0.8.0/tests/test_is_nested_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-04 21:54:25.000000 tyro-0.8.0/tests/test_missing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-04 21:54:25.000000 tyro-0.8.0/tests/test_missing_optional_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-04-04 21:54:25.000000 tyro-0.8.0/tests/test_mixed_unions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33891 2024-04-04 21:54:25.000000 tyro-0.8.0/tests/test_nested.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9753 2024-04-04 21:54:25.000000 tyro-0.8.0/tests/test_nested_in_containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-04 21:54:25.000000 tyro-0.8.0/tests/test_new_style_annotations_min_py310.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-04 21:54:25.000000 tyro-0.8.0/tests/test_new_style_annotations_min_py312.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-04 21:54:25.000000 tyro-0.8.0/tests/test_new_style_annotations_min_py39.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-04 21:54:25.000000 tyro-0.8.0/tests/test_partial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-04-04 21:54:25.000000 tyro-0.8.0/tests/test_positional_min_py38.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-04-04 21:54:25.000000 tyro-0.8.0/tests/test_pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-04 21:54:25.000000 tyro-0.8.0/tests/test_pydantic_with_newtype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-04 21:54:25.000000 tyro-0.8.0/tests/test_self_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-04-04 21:54:25.000000 tyro-0.8.0/tests/test_strings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-04-04 21:54:25.000000 tyro-0.8.0/tests/test_tuple_with_subcommands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-04 21:54:25.000000 tyro-0.8.0/tests/test_union_from_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-04 21:54:25.000000 tyro-0.8.0/tests/test_unsafe_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-04 21:54:25.000000 tyro-0.8.0/tests/test_unsupported_but_should_work.py
```

### Comparing `tyro-0.7.3/LICENSE` & `tyro-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tyro-0.7.3/PKG-INFO` & `tyro-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 Metadata-Version: 2.1
 Name: tyro
-Version: 0.7.3
+Version: 0.8.0
 Summary: Strongly typed, zero-effort CLI interfaces
 Author-email: brentyi <brentyi@berkeley.edu>
 License: MIT
 Project-URL: GitHub, https://github.com/brentyi/tyro
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: docstring-parser>=0.14.1
 Requires-Dist: typing-extensions>=4.3.0
 Requires-Dist: backports.cached-property>=1.0.2; python_version < "3.8"
 Requires-Dist: colorama>=0.4.0; platform_system == "Windows"
 Requires-Dist: rich>=11.1.0
 Requires-Dist: shtab>=1.5.6
+Requires-Dist: eval_type_backport>=0.1.3; python_version < "3.10"
 Provides-Extra: dev
 Requires-Dist: PyYAML>=6.0; extra == "dev"
 Requires-Dist: frozendict>=2.3.4; extra == "dev"
 Requires-Dist: pytest>=7.1.2; extra == "dev"
 Requires-Dist: pytest-cov>=3.0.0; extra == "dev"
 Requires-Dist: omegaconf>=2.2.2; extra == "dev"
 Requires-Dist: attrs>=21.4.0; extra == "dev"
@@ -33,14 +35,15 @@
 Requires-Dist: pyright>=1.1.349; extra == "dev"
 Requires-Dist: ruff>=0.1.13; extra == "dev"
 Requires-Dist: mypy>=1.4.1; extra == "dev"
 Requires-Dist: numpy>=1.20.0; extra == "dev"
 Requires-Dist: flax>=0.6.9; python_version >= "3.8" and extra == "dev"
 Requires-Dist: pydantic>=2.5.2; extra == "dev"
 Requires-Dist: coverage[toml]>=6.5.0; extra == "dev"
+Requires-Dist: eval_type_backport>=0.1.3; extra == "dev"
 
 <br />
 <p align="center">
     <!--
     Note that this README will be used for both GitHub and PyPI.
     We therefore:
     - Keep all image URLs absolute.
```

#### html2text {}

```diff
@@ -1,30 +1,32 @@
-Metadata-Version: 2.1 Name: tyro Version: 0.7.3 Summary: Strongly typed, zero-
+Metadata-Version: 2.1 Name: tyro Version: 0.8.0 Summary: Strongly typed, zero-
 effort CLI interfaces Author-email: brentyi
 berkeley.edu> License: MIT Project-URL: GitHub, https://github.com/brentyi/tyro
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
-:: OS Independent Requires-Python: >=3.7 Description-Content-Type: text/
-markdown License-File: LICENSE Requires-Dist: docstring-parser>=0.14.1
-Requires-Dist: typing-extensions>=4.3.0 Requires-Dist: backports.cached-
-property>=1.0.2; python_version < "3.8" Requires-Dist: colorama>=0.4.0;
-platform_system == "Windows" Requires-Dist: rich>=11.1.0 Requires-Dist:
-shtab>=1.5.6 Provides-Extra: dev Requires-Dist: PyYAML>=6.0; extra == "dev"
-Requires-Dist: frozendict>=2.3.4; extra == "dev" Requires-Dist: pytest>=7.1.2;
-extra == "dev" Requires-Dist: pytest-cov>=3.0.0; extra == "dev" Requires-Dist:
-omegaconf>=2.2.2; extra == "dev" Requires-Dist: attrs>=21.4.0; extra == "dev"
-Requires-Dist: torch>=1.10.0; extra == "dev" Requires-Dist: pyright>=1.1.349;
-extra == "dev" Requires-Dist: ruff>=0.1.13; extra == "dev" Requires-Dist:
-mypy>=1.4.1; extra == "dev" Requires-Dist: numpy>=1.20.0; extra == "dev"
-Requires-Dist: flax>=0.6.9; python_version >= "3.8" and extra == "dev"
-Requires-Dist: pydantic>=2.5.2; extra == "dev" Requires-Dist: coverage
-[toml]>=6.5.0; extra == "dev"
+Classifier: Programming Language :: Python :: 3.12 Classifier: License :: OSI
+Approved :: MIT License Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
+LICENSE Requires-Dist: docstring-parser>=0.14.1 Requires-Dist: typing-
+extensions>=4.3.0 Requires-Dist: backports.cached-property>=1.0.2;
+python_version < "3.8" Requires-Dist: colorama>=0.4.0; platform_system ==
+"Windows" Requires-Dist: rich>=11.1.0 Requires-Dist: shtab>=1.5.6 Requires-
+Dist: eval_type_backport>=0.1.3; python_version < "3.10" Provides-Extra: dev
+Requires-Dist: PyYAML>=6.0; extra == "dev" Requires-Dist: frozendict>=2.3.4;
+extra == "dev" Requires-Dist: pytest>=7.1.2; extra == "dev" Requires-Dist:
+pytest-cov>=3.0.0; extra == "dev" Requires-Dist: omegaconf>=2.2.2; extra ==
+"dev" Requires-Dist: attrs>=21.4.0; extra == "dev" Requires-Dist:
+torch>=1.10.0; extra == "dev" Requires-Dist: pyright>=1.1.349; extra == "dev"
+Requires-Dist: ruff>=0.1.13; extra == "dev" Requires-Dist: mypy>=1.4.1; extra
+== "dev" Requires-Dist: numpy>=1.20.0; extra == "dev" Requires-Dist:
+flax>=0.6.9; python_version >= "3.8" and extra == "dev" Requires-Dist:
+pydantic>=2.5.2; extra == "dev" Requires-Dist: coverage[toml]>=6.5.0; extra ==
+"dev" Requires-Dist: eval_type_backport>=0.1.3; extra == "dev"
                                   [tyro logo]
                      _DD_oo_cc_uu_mm_ee_nn_tt_aa_tt_ii_oo_nn   •   ppiipp iinnssttaallll ttyyrroo
                 [build][mypy][pyright][ruff]_[_c_o_d_e_c_o_v_]_[_c_o_d_e_c_o_v_]
 
 ttyyrroo is a tool for generating command-line interfaces and configuration objects
 in Python. Our core API, `tyro.cli()`, - **Generates CLI interfaces** from
 Python type signatures. - **Populates helptext automatically** from defaults,
```

### Comparing `tyro-0.7.3/README.md` & `tyro-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `tyro-0.7.3/pyproject.toml` & `tyro-0.8.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -3,36 +3,38 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tyro"
 authors = [
     {name = "brentyi", email = "brentyi@berkeley.edu"},
 ]
-version = "0.7.3"  # TODO: currently needs to be synchronized manually with __init__.py.
+version = "0.8.0"  # TODO: currently needs to be synchronized manually with __init__.py.
 description = "Strongly typed, zero-effort CLI interfaces"
 readme = "README.md"
 license = { text="MIT" }
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 dependencies = [
     "docstring-parser>=0.14.1",
     "typing-extensions>=4.3.0",
     "backports.cached-property>=1.0.2; python_version<'3.8'",
     "colorama>=0.4.0; platform_system=='Windows'",
     "rich>=11.1.0",
-    "shtab>=1.5.6"
+    "shtab>=1.5.6",
+    "eval_type_backport>=0.1.3; python_version<'3.10'",
 ]
 
 [project.optional-dependencies]
 dev = [
     "PyYAML>=6.0",
     "frozendict>=2.3.4",
     "pytest>=7.1.2",
@@ -44,28 +46,29 @@
     "ruff>=0.1.13",
     "mypy>=1.4.1",
     "numpy>=1.20.0",
     # As of 7/27/2023, flax install fails for Python 3.7 without pinning to an
     # old version. But doing so breaks other Python versions.
     "flax>=0.6.9;python_version>='3.8'",
     "pydantic>=2.5.2",
-    "coverage[toml]>=6.5.0"
+    "coverage[toml]>=6.5.0",
+    "eval_type_backport>=0.1.3",
 ]
 
 [project.urls]
 "GitHub" = "https://github.com/brentyi/tyro"
 
 [tool.setuptools.package-data]
 tyro = ["py.typed"]
 
 [tool.isort]
 profile = "black"
 
 [tool.mypy]
-python_version = "3.10"
+python_version = "3.12"
 ignore_missing_imports = true
 warn_unused_configs = true
 exclude = "^tests/test_py311_generated/.*"
 
 [tool.coverage.report]
 exclude_lines = [
     # Have to re-enable the standard pragma
@@ -97,24 +100,24 @@
 
     # or anything that's deprecated
     "deprecated"
 ]
 
 [tool.ruff]
 src = ["src"]  # Needed to recognize first-party import location in GitHub action.
-select = [
+lint.select = [
     "E",  # pycodestyle errors.
     "F",  # Pyflakes rules.
     "PLC",  # Pylint convention warnings.
     "PLE",  # Pylint errors.
     "PLR",  # Pylint refactor recommendations.
     "PLW",  # Pylint warnings.
     "I"  # Import sorting.
 ]
-ignore = [
+lint.ignore = [
     "E741", # Ambiguous variable name. (l, O, or I)
     "E501",  # Line too long.
     "PLR2004",  # Magic value used in comparison.
     "PLR0915",  # Too many statements.
     "PLR0913",  # Too many arguments.
     "PLC0414",  # Import alias does not rename variable. (this is used for exporting names)
     "PLC1901",  # Use falsey strings.
```

### Comparing `tyro-0.7.3/src/tyro/_argparse_formatter.py` & `tyro-0.8.0/src/tyro/_argparse_formatter.py`

 * *Files 0% similar despite different names*

```diff
@@ -877,15 +877,15 @@
         # Patch to avoid super long arguments from shifting the helptext of all of the
         # fields.
         prev_max_length = self._action_max_length
         super().add_argument(action)
         if self._action_max_length > self._max_help_position + 2:
             self._action_max_length = prev_max_length
 
-    def _split_lines(self, text, width):
+    def _split_lines(self, text, width):  # pragma: no cover
         text = self._whitespace_matcher.sub(" ", text).strip()
         # The textwrap module is used only for formatting help.
         # Delay its import for speeding up the common usage of argparse.
         import textwrap as textwrap
 
         # Sketchy, but seems to work.
         textwrap.len = monkeypatch_len  # type: ignore
```

### Comparing `tyro-0.7.3/src/tyro/_arguments.py` & `tyro-0.8.0/src/tyro/_arguments.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Rules for taking high-level field definitions and lowering them into inputs for
 argparse's `add_argument()`."""
+
 from __future__ import annotations
 
 import argparse
 import dataclasses
 import enum
 import functools
 import itertools
@@ -127,17 +128,17 @@
             name_or_flag = _strings.dummy_field_name
 
         # We're actually going to skip the default field: if an argument is unset, the
         # MISSING value will be detected in _calling.py and the field default will
         # directly be used. This helps reduce the likelihood of issues with converting
         # the field default to a string format, then back to the desired type.
         action = kwargs.get("action", None)
-        if action != "append":
+        if action not in {"append", "count"}:
             kwargs["default"] = _fields.MISSING_NONPROP
-        elif action == BooleanOptionalAction:
+        elif action in {BooleanOptionalAction, "count"}:
             pass
         else:
             kwargs["default"] = []
 
         # Apply overrides in our arg configuration object.
         # Note that the `name` field is applied when the field object is instantiated!
         if self.field.argconf.metavar is not None:
@@ -188,14 +189,15 @@
     def lowered(self) -> LoweredArgumentDefinition:
         """Lowered argument definition, generated by applying a sequence of rules."""
         rules = (
             _rule_handle_defaults,
             _rule_handle_boolean_flags,
             _rule_recursive_instantiator_from_type,
             _rule_convert_defaults_to_strings,
+            _rule_counters,
             _rule_generate_helptext,
             _rule_set_name_or_flag_and_dest,
             _rule_positional_special_handling,
             _rule_static_cast_choices_to_patched_list,
         )
         return functools.reduce(
             lambda lowered, rule: rule(self, lowered),
@@ -400,14 +402,36 @@
 
 # TODO: this function is also called outside of _arguments.py. Should be revisited.
 def _rich_tag_if_enabled(x: str, tag: str) -> str:
     x = rich.markup.escape(_strings.strip_ansi_sequences(x))
     return x if not USE_RICH else f"[{tag}]{x}[/{tag}]"
 
 
+def _rule_counters(
+    arg: ArgumentDefinition,
+    lowered: LoweredArgumentDefinition,
+) -> LoweredArgumentDefinition:
+    """Handle counters, like -vvv for level-3 verbosity."""
+    if (
+        _markers.UseCounterAction in arg.field.markers
+        and arg.field.type_or_callable is int
+        and not arg.field.is_positional()
+    ):
+        return dataclasses.replace(
+            lowered,
+            metavar=None,
+            nargs=None,
+            action="count",
+            default=0,
+            required=False,
+            instantiator=lambda x: x,  # argparse will directly give us an int!
+        )
+    return lowered
+
+
 def _rule_generate_helptext(
     arg: ArgumentDefinition,
     lowered: LoweredArgumentDefinition,
 ) -> LoweredArgumentDefinition:
     """Generate helptext from docstring, argument name, default values."""
 
     # If the suppress marker is attached, hide the argument.
@@ -460,14 +484,17 @@
         # Include default value in helptext. We intentionally don't use the % template
         # because the types of all arguments are set to strings, which will cause the
         # default to be casted to a string and introduce extra quotation marks.
         if lowered.instantiator is None:
             # Intentionally not quoted via shlex, since this can't actually be passed
             # in via the commandline.
             default_text = f"(fixed to: {default_label})"
+        elif lowered.action == "count":
+            # Repeatable argument.
+            default_text = "(repeatable)"
         elif lowered.action == "append" and (
             default in _fields.MISSING_SINGLETONS or len(cast(tuple, default)) == 0
         ):
             default_text = "(repeatable)"
         elif lowered.action == "append" and len(cast(tuple, default)) > 0:
             assert default is not None  # Just for type checker.
             default_text = f"(repeatable, appends to: {default_label})"
```

### Comparing `tyro-0.7.3/src/tyro/_calling.py` & `tyro-0.8.0/src/tyro/_calling.py`

 * *Files identical despite different names*

### Comparing `tyro-0.7.3/src/tyro/_cli.py` & `tyro-0.8.0/src/tyro/_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Core public API."""
+
 import argparse
 import dataclasses
 import pathlib
 import sys
 import warnings
 from typing import (
     Callable,
@@ -47,30 +48,28 @@
     *,
     prog: Optional[str] = None,
     description: Optional[str] = None,
     args: Optional[Sequence[str]] = None,
     default: Optional[OutT] = None,
     return_unknown_args: Literal[False] = False,
     use_underscores: bool = False,
-) -> OutT:
-    ...
+) -> OutT: ...
 
 
 @overload
 def cli(
     f: TypeForm[OutT],
     *,
     prog: Optional[str] = None,
     description: Optional[str] = None,
     args: Optional[Sequence[str]] = None,
     default: Optional[OutT] = None,
     return_unknown_args: Literal[True],
     use_underscores: bool = False,
-) -> Tuple[OutT, List[str]]:
-    ...
+) -> Tuple[OutT, List[str]]: ...
 
 
 @overload
 def cli(
     f: Callable[..., OutT],
     *,
     prog: Optional[str] = None,
@@ -78,16 +77,15 @@
     args: Optional[Sequence[str]] = None,
     # Note that passing a default makes sense for things like dataclasses, but are not
     # supported for general callables. These can, however, be specified in the signature
     # of the callable itself.
     default: None = None,
     return_unknown_args: Literal[False] = False,
     use_underscores: bool = False,
-) -> OutT:
-    ...
+) -> OutT: ...
 
 
 @overload
 def cli(
     f: Callable[..., OutT],
     *,
     prog: Optional[str] = None,
@@ -95,16 +93,15 @@
     args: Optional[Sequence[str]] = None,
     # Note that passing a default makes sense for things like dataclasses, but are not
     # supported for general callables. These can, however, be specified in the signature
     # of the callable itself.
     default: None = None,
     return_unknown_args: Literal[True],
     use_underscores: bool = False,
-) -> Tuple[OutT, List[str]]:
-    ...
+) -> Tuple[OutT, List[str]]: ...
 
 
 def cli(
     f: Union[TypeForm[OutT], Callable[..., OutT]],
     *,
     prog: Optional[str] = None,
     description: Optional[str] = None,
@@ -209,28 +206,26 @@
 def get_parser(
     f: TypeForm[OutT],
     *,
     prog: Optional[str] = None,
     description: Optional[str] = None,
     default: Optional[OutT] = None,
     use_underscores: bool = False,
-) -> argparse.ArgumentParser:
-    ...
+) -> argparse.ArgumentParser: ...
 
 
 @overload
 def get_parser(
     f: Callable[..., OutT],
     *,
     prog: Optional[str] = None,
     description: Optional[str] = None,
     default: Optional[OutT] = None,
     use_underscores: bool = False,
-) -> argparse.ArgumentParser:
-    ...
+) -> argparse.ArgumentParser: ...
 
 
 def get_parser(
     f: Union[TypeForm[OutT], Callable[..., OutT]],
     *,
     # Note that we have no `args` argument, since this is only used when
     # parser.parse_args() is called.
```

### Comparing `tyro-0.7.3/src/tyro/_docstrings.py` & `tyro-0.8.0/src/tyro/_docstrings.py`

 * *Files identical despite different names*

### Comparing `tyro-0.7.3/src/tyro/_fields.py` & `tyro-0.8.0/src/tyro/_fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Abstractions for pulling out 'field' definitions, which specify inputs, types, and # type: ignore
 defaults, from general callables."""
+
 from __future__ import annotations
 
 import collections
 import collections.abc
 import dataclasses
 import enum
 import functools
@@ -467,15 +468,17 @@
         default_instance not in MISSING_SINGLETONS
         and default_instance is not EXCLUDE_FROM_CALL
     )
     assert not valid_default_instance or isinstance(default_instance, dict)
     total = getattr(cls, "__total__", True)
     assert isinstance(total, bool)
     assert not valid_default_instance or isinstance(default_instance, dict)
-    for name, typ in _resolver.get_type_hints(cls, include_extras=True).items():
+    for name, typ in _resolver.get_type_hints_with_backported_syntax(
+        cls, include_extras=True
+    ).items():
         typ_origin = get_origin(typ)
         is_default_from_default_instance = False
         if valid_default_instance and name in cast(dict, default_instance):
             default = cast(dict, default_instance)[name]
             is_default_from_default_instance = True
         elif typ_origin is Required and total is False:
             # Support total=False.
@@ -527,15 +530,17 @@
     # TODO: in terms of helptext, we currently do display the default NamedTuple
     # helptext. But we (intentionally) don't for dataclasses; this is somewhat
     # inconsistent.
     field_list = []
     field_defaults = getattr(cls, "_field_defaults")
 
     # Note that _field_types is removed in Python 3.9.
-    for name, typ in _resolver.get_type_hints(cls, include_extras=True).items():
+    for name, typ in _resolver.get_type_hints_with_backported_syntax(
+        cls, include_extras=True
+    ).items():
         # Get default, with priority for `default_instance`.
         default = field_defaults.get(name, MISSING_NONPROP)
         if hasattr(default_instance, name):
             default = getattr(default_instance, name)
         if default_instance is MISSING_PROP:
             default = MISSING_PROP
 
@@ -604,20 +609,24 @@
 
 # Support attrs and pydantic if they're installed.
 try:
     import pydantic
 except ImportError:
     if not TYPE_CHECKING:
         pydantic = None  # type: ignore
+    else:
+        import pydantic
 
 try:
     from pydantic import v1 as pydantic_v1
 except ImportError:
     if not TYPE_CHECKING:
         pydantic_v1 = None  # type: ignore
+    else:
+        from pydantic import v1 as pydantic_v1
 
 
 def _is_pydantic(cls: TypeForm[Any]) -> bool:
     if pydantic is not None and issubclass(cls, pydantic.BaseModel):
         return True
     if pydantic_v1 is not None and issubclass(cls, pydantic_v1.BaseModel):
         return True
@@ -728,15 +737,15 @@
                     stacklevel=2,
                 )
         elif default is attr.NOTHING:
             default = MISSING_NONPROP
         elif isinstance(default, attr.Factory):  # type: ignore
             default = default.factory()  # type: ignore
 
-        assert attr_field.type is not None
+        assert attr_field.type is not None, attr_field
         field_list.append(
             FieldDefinition.make(
                 name=name,
                 type_or_callable=attr_field.type,
                 default=default,
                 is_default_from_default_instance=is_default_from_default_instance,
                 helptext=_docstrings.get_field_docstring(cls, name),
@@ -957,15 +966,15 @@
     if docstring is not None:
         for param_doc in docstring_parser.parse(docstring).params:
             docstring_from_arg_name[param_doc.arg_name] = param_doc.description
     del docstring
 
     # This will throw a type error for torch.device, typing.Dict, etc.
     try:
-        hints = _resolver.get_type_hints(f, include_extras=True)
+        hints = _resolver.get_type_hints_with_backported_syntax(f, include_extras=True)
     except TypeError:
         return UnsupportedNestedTypeMessage(f"Could not get hints for {f}!")
 
     field_list = []
     for param in params:
         # Get default value.
         default = param.default
```

### Comparing `tyro-0.7.3/src/tyro/_instantiators.py` & `tyro-0.8.0/src/tyro/_instantiators.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
             for typ, x in zip(
                 (int, float),
                 strings,
             )
         )
 ```
 """
+
 import collections.abc
 import dataclasses
 import enum
 import inspect
 import os
 import pathlib
 from collections import deque
@@ -117,15 +118,15 @@
     try:
         signature = inspect.signature(typ)
     except ValueError:
         # pybind objects might not have a parsable signature. We try to be tolerant in this case.
         # One day this should be fixed with `__text_signature__`.
         return True
 
-    type_annotations = _resolver.get_type_hints_with_nicer_errors(typ)
+    type_annotations = _resolver.get_type_hints_with_backported_syntax(typ)
     # Some checks we can do if the signature is available!
     for i, param in enumerate(signature.parameters.values()):
         annotation = type_annotations.get(param.name, param.annotation)
 
         # Hack: apply_type_from_typevar applies shims, like UnionType => Union
         # conversion.
         annotation = _resolver.apply_type_from_typevar(annotation, {})
@@ -183,30 +184,30 @@
 
     # Instantiate os.PathLike annotations using pathlib.Path.
     # Ideally this should be implemented in a more general way, eg using
     # https://github.com/brentyi/tyro/pull/30
     if typ is os.PathLike:
         typ = pathlib.Path
 
+    # Unwrap NewType + set metavar based on NewType name.
+    # `isinstance(x, NewType)` doesn't work because NewType isn't a class until
+    # Python 3.10, so we instead do a duck typing-style check.
+    metavar = getattr(typ, "__name__", "").upper()
+    typ, maybe_newtype_name = _resolver.unwrap_newtype_and_aliases(typ)
+    if maybe_newtype_name is not None:
+        metavar = maybe_newtype_name.upper()
+
     # Address container types. If a matching container is found, this will recursively
     # call instantiator_from_type().
     container_out = _instantiator_from_container_type(
         cast(TypeForm[Any], typ), type_from_typevar, markers
     )
     if container_out is not None:
         return container_out
 
-    # Unwrap NewType + set metavar based on NewType name.
-    # `isinstance(x, NewType)` doesn't work because NewType isn't a class until
-    # Python 3.10, so we instead do a duck typing-style check.
-    metavar = getattr(typ, "__name__", "").upper()
-    typ, maybe_newtype_name = _resolver.unwrap_newtype(typ)
-    if maybe_newtype_name is not None:
-        metavar = maybe_newtype_name.upper()
-
     # Validate that typ is a `(arg: str) -> T` type converter, as expected by argparse.
     if typ in _builtin_set:
         pass
     elif not callable(typ):
         raise UnsupportedTypeAnnotationError(
             f"Expected {typ} to be an `(arg: str) -> T` type converter, but is not"
             " callable."
@@ -265,36 +266,33 @@
 
 @overload
 def _instantiator_from_type_inner(
     typ: TypeForm,
     type_from_typevar: Dict[TypeVar, TypeForm[Any]],
     allow_sequences: Literal["fixed_length"],
     markers: FrozenSet[_markers.Marker],
-) -> Tuple[Instantiator, InstantiatorMetadata]:
-    ...
+) -> Tuple[Instantiator, InstantiatorMetadata]: ...
 
 
 @overload
 def _instantiator_from_type_inner(
     typ: TypeForm,
     type_from_typevar: Dict[TypeVar, TypeForm[Any]],
     allow_sequences: Literal[False],
     markers: FrozenSet[_markers.Marker],
-) -> Tuple[_StandardInstantiator, InstantiatorMetadata]:
-    ...
+) -> Tuple[_StandardInstantiator, InstantiatorMetadata]: ...
 
 
 @overload
 def _instantiator_from_type_inner(
     typ: TypeForm,
     type_from_typevar: Dict[TypeVar, TypeForm[Any]],
     allow_sequences: Literal[True],
     markers: FrozenSet[_markers.Marker],
-) -> Tuple[Instantiator, InstantiatorMetadata]:
-    ...
+) -> Tuple[Instantiator, InstantiatorMetadata]: ...
 
 
 def _instantiator_from_type_inner(
     typ: TypeForm,
     type_from_typevar: Dict[TypeVar, TypeForm[Any]],
     allow_sequences: Literal["fixed_length", True, False],
     markers: FrozenSet[_markers.Marker],
```

### Comparing `tyro-0.7.3/src/tyro/_parsers.py` & `tyro-0.8.0/src/tyro/_parsers.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,21 +146,21 @@
                     subparsers = add_subparsers_to_leaves(
                         subparsers, nested_parser.subparsers
                     )
 
                 # Helptext for this field; used as description for grouping arguments.
                 class_field_name = _strings.make_field_name([field.intern_name])
                 if field.helptext is not None:
-                    helptext_from_intern_prefixed_field_name[
-                        class_field_name
-                    ] = field.helptext
+                    helptext_from_intern_prefixed_field_name[class_field_name] = (
+                        field.helptext
+                    )
                 else:
-                    helptext_from_intern_prefixed_field_name[
-                        class_field_name
-                    ] = _docstrings.get_callable_description(nested_parser.f)
+                    helptext_from_intern_prefixed_field_name[class_field_name] = (
+                        _docstrings.get_callable_description(nested_parser.f)
+                    )
 
                 # If arguments are in an optional group, it indicates that the default_instance
                 # will be used if none of the arguments are passed in.
                 if (
                     len(nested_parser.args) >= 1
                     and _markers._OPTIONAL_GROUP in nested_parser.args[0].field.markers
                 ):
```

### Comparing `tyro-0.7.3/src/tyro/_resolver.py` & `tyro-0.8.0/src/tyro/_resolver.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Utilities for resolving types and forward references."""
+
 import collections.abc
 import copy
 import dataclasses
 import inspect
 import sys
 import types
 import warnings
@@ -17,15 +18,23 @@
     Set,
     Tuple,
     TypeVar,
     Union,
     cast,
 )
 
-from typing_extensions import Annotated, Self, get_args, get_origin, get_type_hints
+from typing_extensions import (
+    Annotated,
+    ForwardRef,
+    Self,
+    TypeAliasType,
+    get_args,
+    get_origin,
+    get_type_hints,
+)
 
 from . import _fields, _unsafe_cache
 from ._typing import TypeForm
 
 TypeOrCallable = TypeVar("TypeOrCallable", TypeForm[Any], Callable)
 
 
@@ -57,15 +66,15 @@
     if get_origin(cls) is Annotated:
         # ^We need this `if` statement for an obscure edge case: when `cls` is a
         # function with `__tyro_markers__` set, we don't want/need to return
         # Annotated[func, markers].
         cls, annotations = unwrap_annotated(cls)
 
     # We'll ignore NewType when getting the origin + args for generics.
-    origin_cls = get_origin(unwrap_newtype(cls)[0])
+    origin_cls = get_origin(unwrap_newtype_and_aliases(cls)[0])
     type_from_typevar: Dict[TypeVar, TypeForm[Any]] = {}
 
     # Support typing.Self.
     # We'll do this by pretending that `Self` is a TypeVar...
     if hasattr(cls, "__self__"):
         self_type = getattr(cls, "__self__")
         if inspect.isclass(self_type):
@@ -76,15 +85,15 @@
     if (
         # Apply some heuristics for generic types. Should revisit this.
         origin_cls is not None
         and hasattr(origin_cls, "__parameters__")
         and hasattr(origin_cls.__parameters__, "__len__")
     ):
         typevars = origin_cls.__parameters__
-        typevar_values = get_args(unwrap_newtype(cls)[0])
+        typevar_values = get_args(unwrap_newtype_and_aliases(cls)[0])
         assert len(typevars) == len(typevar_values)
         cls = origin_cls
         type_from_typevar.update(dict(zip(typevars, typevar_values)))
 
     if hasattr(cls, "__orig_bases__"):
         bases = getattr(cls, "__orig_bases__")
         for base in bases:
@@ -107,15 +116,17 @@
 @_unsafe_cache.unsafe_cache(maxsize=1024)
 def resolved_fields(cls: TypeForm) -> List[dataclasses.Field]:
     """Similar to dataclasses.fields(), but includes dataclasses.InitVar types and
     resolves forward references."""
 
     assert dataclasses.is_dataclass(cls)
     fields = []
-    annotations = get_type_hints(cast(Callable, cls), include_extras=True)
+    annotations = get_type_hints_with_backported_syntax(
+        cast(Callable, cls), include_extras=True
+    )
     for field in getattr(cls, "__dataclass_fields__").values():
         # Avoid mutating original field.
         field = copy.copy(field)
 
         # Resolve forward references.
         field.type = annotations[field.name]
 
@@ -153,17 +164,21 @@
             return Union.__getitem__(typ.__constraints__)  # type: ignore
     return typ
 
 
 TypeOrCallableOrNone = TypeVar("TypeOrCallableOrNone", Callable, TypeForm[Any], None)
 
 
-def unwrap_newtype(
+def unwrap_newtype_and_aliases(
     typ: TypeOrCallableOrNone,
 ) -> Tuple[TypeOrCallableOrNone, Optional[str]]:
+    # Handle type aliases, eg via the `type` statement in Python 3.12.
+    if isinstance(typ, TypeAliasType):
+        return unwrap_newtype_and_aliases(typ.__value__)  # type: ignore
+
     # We'll unwrap NewType annotations here; this is needed before issubclass
     # checks!
     #
     # `isinstance(x, NewType)` doesn't work because NewType isn't a class until
     # Python 3.10, so we instead do a duck typing-style check.
     return_name = None
     while hasattr(typ, "__name__") and hasattr(typ, "__supertype__"):
@@ -183,15 +198,15 @@
     we should parse as Cat.
 
     This should generally only be applied to fields used as nested structures, not
     individual arguments/fields. (if a field is annotated as Union[int, str], and a
     string default is passed in, we don't want to narrow the type to always be
     strings!)"""
 
-    typ, unused_name = unwrap_newtype(typ)
+    typ, unused_name = unwrap_newtype_and_aliases(typ)
     del unused_name
 
     try:
         potential_subclass = type(default_instance)
 
         if potential_subclass is type:
             # Don't narrow to `type`. This happens when the default instance is a class;
@@ -345,36 +360,35 @@
             return Union.__getitem__(options + (type(default_instance),))  # type: ignore
     except TypeError:
         pass
 
     return typ
 
 
-def get_type_hints_with_nicer_errors(
+def get_type_hints_with_backported_syntax(
     obj: Callable[..., Any], include_extras: bool = False
 ) -> Dict[str, Any]:
+    """Same as `typing.get_type_hints()`, but supports new union syntax (X | Y)
+    and generics (list[str]) in older versions of Python."""
     try:
         return get_type_hints(obj, include_extras=include_extras)
     except TypeError as e:  # pragma: no cover
-        common_message = f"\n-----\n\nError calling typing.get_type_hints() on {obj}! "
-        message = e.args[0]
-        if message.startswith(
-            "unsupported operand type(s) for |"
-        ) and sys.version_info < (3, 10):
-            # PEP 604. Requires Python 3.10.
-            raise TypeError(
-                e.args[0]
-                + common_message
-                + "You may be using a Union in the form of `X | Y`; to support Python versions that lower than 3.10, you need to use `typing.Union[X, Y]` instead of `X | Y` and `typing.Optional[X]` instead of `X | None`.",
-                *e.args[1:],
-            )
-        elif message == "'type' object is not subscriptable" and (
-            sys.version_info < (3, 9)
-        ):
-            # PEP 585. Requires Python 3.9.
-            raise TypeError(
-                e.args[0]
-                + common_message
-                + "You may be using a standard collection as a generic, like `list[T]` or `tuple[T1, T2]`. To support Python versions lower than 3.9, you need to using `typing.List[T]` and `typing.Tuple[T1, T2]`.",
-                *e.args[1:],
-            )
+        # Resolve new type syntax using eval_type_backport.
+        if hasattr(obj, "__annotations__"):
+            try:
+                from eval_type_backport import eval_type_backport
+
+                # Get global namespace for functions.
+                globalns = getattr(obj, "__globals__", None)
+
+                # Get global namespace for classes.
+                if globalns is None and hasattr(globalns, "__init__"):
+                    globalns = getattr(getattr(obj, "__init__"), "__globals__", None)
+
+                out = {
+                    k: eval_type_backport(ForwardRef(v), globalns=globalns, localns={})
+                    for k, v in getattr(obj, "__annotations__").items()
+                }
+                return out
+            except ImportError:
+                pass
         raise e
```

### Comparing `tyro-0.7.3/src/tyro/_strings.py` & `tyro-0.8.0/src/tyro/_strings.py`

 * *Files identical despite different names*

### Comparing `tyro-0.7.3/src/tyro/_subcommand_matching.py` & `tyro-0.8.0/src/tyro/_subcommand_matching.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,18 +93,18 @@
 
         self_types = _get_type_options(self.typ)
         super_types = _get_type_options(supertype.typ)
 
         # Check against supertypes.
         for self_type in self_types:
             self_type = _resolver.unwrap_annotated(self_type)[0]
-            self_type, _ = _resolver.unwrap_newtype(self_type)
+            self_type, _ = _resolver.unwrap_newtype_and_aliases(self_type)
             ok = False
             for super_type in super_types:
                 super_type = _resolver.unwrap_annotated(super_type)[0]
-                self_type, _ = _resolver.unwrap_newtype(self_type)
+                self_type, _ = _resolver.unwrap_newtype_and_aliases(self_type)
                 if issubclass(self_type, super_type):
                     ok = True
             if not ok:
                 return False
 
         return True
```

### Comparing `tyro-0.7.3/src/tyro/_typing.py` & `tyro-0.8.0/src/tyro/_typing.py`

 * *Files identical despite different names*

### Comparing `tyro-0.7.3/src/tyro/_unsafe_cache.py` & `tyro-0.8.0/src/tyro/_unsafe_cache.py`

 * *Files identical despite different names*

### Comparing `tyro-0.7.3/src/tyro/conf/__init__.py` & `tyro-0.8.0/src/tyro/conf/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,8 +17,9 @@
 from ._markers import OmitArgPrefixes as OmitArgPrefixes
 from ._markers import OmitSubcommandPrefixes as OmitSubcommandPrefixes
 from ._markers import Positional as Positional
 from ._markers import PositionalRequiredArgs as PositionalRequiredArgs
 from ._markers import Suppress as Suppress
 from ._markers import SuppressFixed as SuppressFixed
 from ._markers import UseAppendAction as UseAppendAction
+from ._markers import UseCounterAction as UseCounterAction
 from ._markers import configure as configure
```

### Comparing `tyro-0.7.3/src/tyro/conf/_confstruct.py` & `tyro-0.8.0/src/tyro/conf/_confstruct.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,29 +21,27 @@
     name: Optional[str] = None,
     *,
     default: Any = MISSING_NONPROP,
     description: Optional[str] = None,
     prefix_name: bool = True,
     constructor: None = None,
     constructor_factory: Optional[Callable[[], Union[Type, Callable]]] = None,
-) -> Any:
-    ...
+) -> Any: ...
 
 
 @overload
 def subcommand(
     name: Optional[str] = None,
     *,
     default: Any = MISSING_NONPROP,
     description: Optional[str] = None,
     prefix_name: bool = True,
     constructor: Optional[Union[Type, Callable]] = None,
     constructor_factory: None = None,
-) -> Any:
-    ...
+) -> Any: ...
 
 
 def subcommand(
     name: Optional[str] = None,
     *,
     default: Any = MISSING_NONPROP,
     description: Optional[str] = None,
@@ -128,30 +126,28 @@
     name: Optional[str] = None,
     metavar: Optional[str] = None,
     help: Optional[str] = None,
     aliases: Optional[Sequence[str]] = None,
     prefix_name: Optional[bool] = None,
     constructor: None = None,
     constructor_factory: Optional[Callable[[], Union[Type, Callable]]] = None,
-) -> Any:
-    ...
+) -> Any: ...
 
 
 @overload
 def arg(
     *,
     name: Optional[str] = None,
     metavar: Optional[str] = None,
     help: Optional[str] = None,
     aliases: Optional[Sequence[str]] = None,
     prefix_name: Optional[bool] = None,
     constructor: Optional[Union[Type, Callable]] = None,
     constructor_factory: None = None,
-) -> Any:
-    ...
+) -> Any: ...
 
 
 def arg(
     *,
     name: Optional[str] = None,
     metavar: Optional[str] = None,
     help: Optional[str] = None,
```

### Comparing `tyro-0.7.3/src/tyro/conf/_markers.py` & `tyro-0.8.0/src/tyro/conf/_markers.py`

 * *Files 3% similar despite different names*

```diff
@@ -119,14 +119,18 @@
 The resulting syntax may be more user-friendly; for `tyro`, it also enables support for
 otherwise ambiguous annotations like `List[List[int]]`.
 
 Can be applied to all variable-length sequences (`List[T]`, `Sequence[T]`,
 `Tuple[T, ...]`, etc), including dictionaries without default values.
 """
 
+UseCounterAction = Annotated[T, None]
+"""Use "counter" actions for integer arguments. Example usage: `verbose: UseCounterAction[int]`."""
+
+
 CallableType = TypeVar("CallableType", bound=Callable)
 
 # Dynamically generate marker singletons.
 # These can be used one of two ways:
 # - Marker[T]
 # - Annotated[T, Marker]
```

### Comparing `tyro-0.7.3/src/tyro/extras/__init__.py` & `tyro-0.8.0/src/tyro/extras/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """The :mod:`tyro.extras` submodule contains helpers that complement :func:`tyro.cli()`.
 
-Compared to the core interface, APIs here are more likely to be changed or deprecated. """
+Compared to the core interface, APIs here are more likely to be changed or deprecated."""
 
 from .._argparse_formatter import set_accent_color as set_accent_color
 from .._cli import get_parser as get_parser
 from ._base_configs import (
     subcommand_type_from_defaults as subcommand_type_from_defaults,
 )
 from ._choices_type import literal_type_from_choices as literal_type_from_choices
```

### Comparing `tyro-0.7.3/src/tyro/extras/_base_configs.py` & `tyro-0.8.0/src/tyro/extras/_base_configs.py`

 * *Files identical despite different names*

### Comparing `tyro-0.7.3/src/tyro/extras/_choices_type.py` & `tyro-0.8.0/src/tyro/extras/_choices_type.py`

 * *Files identical despite different names*

### Comparing `tyro-0.7.3/src/tyro/extras/_serialization.py` & `tyro-0.8.0/src/tyro/extras/_serialization.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Type-safe, human-readable serialization helpers for dataclasses."""
+
 from __future__ import annotations
 
 import dataclasses
 import enum
 import functools
 from typing import IO, TYPE_CHECKING, Any, Optional, Set, Type, TypeVar, Union
```

### Comparing `tyro-0.7.3/src/tyro/extras/_subcommand_cli_from_dict.py` & `tyro-0.8.0/src/tyro/extras/_subcommand_cli_from_dict.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,30 +12,28 @@
 def subcommand_cli_from_dict(
     subcommands: Dict[str, Callable[..., T]],
     *,
     prog: Optional[str] = None,
     description: Optional[str] = None,
     args: Optional[Sequence[str]] = None,
     use_underscores: bool = False,
-) -> T:
-    ...
+) -> T: ...
 
 
 # TODO: hack. We prefer the above signature, which Pyright understands, but as of 1.6.1
 # mypy doesn't reason about the generics properly.
 @overload
 def subcommand_cli_from_dict(
     subcommands: Dict[str, Callable[..., Any]],
     *,
     prog: Optional[str] = None,
     description: Optional[str] = None,
     args: Optional[Sequence[str]] = None,
     use_underscores: bool = False,
-) -> Any:
-    ...
+) -> Any: ...
 
 
 def subcommand_cli_from_dict(
     subcommands: Dict[str, Callable[..., Any]],
     *,
     prog: Optional[str] = None,
     description: Optional[str] = None,
```

### Comparing `tyro-0.7.3/src/tyro.egg-info/PKG-INFO` & `tyro-0.8.0/src/tyro.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 Metadata-Version: 2.1
 Name: tyro
-Version: 0.7.3
+Version: 0.8.0
 Summary: Strongly typed, zero-effort CLI interfaces
 Author-email: brentyi <brentyi@berkeley.edu>
 License: MIT
 Project-URL: GitHub, https://github.com/brentyi/tyro
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: docstring-parser>=0.14.1
 Requires-Dist: typing-extensions>=4.3.0
 Requires-Dist: backports.cached-property>=1.0.2; python_version < "3.8"
 Requires-Dist: colorama>=0.4.0; platform_system == "Windows"
 Requires-Dist: rich>=11.1.0
 Requires-Dist: shtab>=1.5.6
+Requires-Dist: eval_type_backport>=0.1.3; python_version < "3.10"
 Provides-Extra: dev
 Requires-Dist: PyYAML>=6.0; extra == "dev"
 Requires-Dist: frozendict>=2.3.4; extra == "dev"
 Requires-Dist: pytest>=7.1.2; extra == "dev"
 Requires-Dist: pytest-cov>=3.0.0; extra == "dev"
 Requires-Dist: omegaconf>=2.2.2; extra == "dev"
 Requires-Dist: attrs>=21.4.0; extra == "dev"
@@ -33,14 +35,15 @@
 Requires-Dist: pyright>=1.1.349; extra == "dev"
 Requires-Dist: ruff>=0.1.13; extra == "dev"
 Requires-Dist: mypy>=1.4.1; extra == "dev"
 Requires-Dist: numpy>=1.20.0; extra == "dev"
 Requires-Dist: flax>=0.6.9; python_version >= "3.8" and extra == "dev"
 Requires-Dist: pydantic>=2.5.2; extra == "dev"
 Requires-Dist: coverage[toml]>=6.5.0; extra == "dev"
+Requires-Dist: eval_type_backport>=0.1.3; extra == "dev"
 
 <br />
 <p align="center">
     <!--
     Note that this README will be used for both GitHub and PyPI.
     We therefore:
     - Keep all image URLs absolute.
```

#### html2text {}

```diff
@@ -1,30 +1,32 @@
-Metadata-Version: 2.1 Name: tyro Version: 0.7.3 Summary: Strongly typed, zero-
+Metadata-Version: 2.1 Name: tyro Version: 0.8.0 Summary: Strongly typed, zero-
 effort CLI interfaces Author-email: brentyi
 berkeley.edu> License: MIT Project-URL: GitHub, https://github.com/brentyi/tyro
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
-:: OS Independent Requires-Python: >=3.7 Description-Content-Type: text/
-markdown License-File: LICENSE Requires-Dist: docstring-parser>=0.14.1
-Requires-Dist: typing-extensions>=4.3.0 Requires-Dist: backports.cached-
-property>=1.0.2; python_version < "3.8" Requires-Dist: colorama>=0.4.0;
-platform_system == "Windows" Requires-Dist: rich>=11.1.0 Requires-Dist:
-shtab>=1.5.6 Provides-Extra: dev Requires-Dist: PyYAML>=6.0; extra == "dev"
-Requires-Dist: frozendict>=2.3.4; extra == "dev" Requires-Dist: pytest>=7.1.2;
-extra == "dev" Requires-Dist: pytest-cov>=3.0.0; extra == "dev" Requires-Dist:
-omegaconf>=2.2.2; extra == "dev" Requires-Dist: attrs>=21.4.0; extra == "dev"
-Requires-Dist: torch>=1.10.0; extra == "dev" Requires-Dist: pyright>=1.1.349;
-extra == "dev" Requires-Dist: ruff>=0.1.13; extra == "dev" Requires-Dist:
-mypy>=1.4.1; extra == "dev" Requires-Dist: numpy>=1.20.0; extra == "dev"
-Requires-Dist: flax>=0.6.9; python_version >= "3.8" and extra == "dev"
-Requires-Dist: pydantic>=2.5.2; extra == "dev" Requires-Dist: coverage
-[toml]>=6.5.0; extra == "dev"
+Classifier: Programming Language :: Python :: 3.12 Classifier: License :: OSI
+Approved :: MIT License Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
+LICENSE Requires-Dist: docstring-parser>=0.14.1 Requires-Dist: typing-
+extensions>=4.3.0 Requires-Dist: backports.cached-property>=1.0.2;
+python_version < "3.8" Requires-Dist: colorama>=0.4.0; platform_system ==
+"Windows" Requires-Dist: rich>=11.1.0 Requires-Dist: shtab>=1.5.6 Requires-
+Dist: eval_type_backport>=0.1.3; python_version < "3.10" Provides-Extra: dev
+Requires-Dist: PyYAML>=6.0; extra == "dev" Requires-Dist: frozendict>=2.3.4;
+extra == "dev" Requires-Dist: pytest>=7.1.2; extra == "dev" Requires-Dist:
+pytest-cov>=3.0.0; extra == "dev" Requires-Dist: omegaconf>=2.2.2; extra ==
+"dev" Requires-Dist: attrs>=21.4.0; extra == "dev" Requires-Dist:
+torch>=1.10.0; extra == "dev" Requires-Dist: pyright>=1.1.349; extra == "dev"
+Requires-Dist: ruff>=0.1.13; extra == "dev" Requires-Dist: mypy>=1.4.1; extra
+== "dev" Requires-Dist: numpy>=1.20.0; extra == "dev" Requires-Dist:
+flax>=0.6.9; python_version >= "3.8" and extra == "dev" Requires-Dist:
+pydantic>=2.5.2; extra == "dev" Requires-Dist: coverage[toml]>=6.5.0; extra ==
+"dev" Requires-Dist: eval_type_backport>=0.1.3; extra == "dev"
                                   [tyro logo]
                      _DD_oo_cc_uu_mm_ee_nn_tt_aa_tt_ii_oo_nn   •   ppiipp iinnssttaallll ttyyrroo
                 [build][mypy][pyright][ruff]_[_c_o_d_e_c_o_v_]_[_c_o_d_e_c_o_v_]
 
 ttyyrroo is a tool for generating command-line interfaces and configuration objects
 in Python. Our core API, `tyro.cli()`, - **Generates CLI interfaces** from
 Python type signatures. - **Populates helptext automatically** from defaults,
```

### Comparing `tyro-0.7.3/src/tyro.egg-info/SOURCES.txt` & `tyro-0.8.0/src/tyro.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -37,28 +37,28 @@
 tests/test_collections.py
 tests/test_completion.py
 tests/test_conf.py
 tests/test_dcargs.py
 tests/test_dict_namedtuple.py
 tests/test_dynamic_dataclasses.py
 tests/test_errors.py
-tests/test_errors_new_annotations.py
 tests/test_flax_min_py38.py
 tests/test_forward_ref.py
 tests/test_functools.py
 tests/test_generics_and_serialization.py
 tests/test_helptext.py
 tests/test_initvar_min_py38.py
 tests/test_is_nested_type.py
 tests/test_missing.py
 tests/test_missing_optional_packages.py
 tests/test_mixed_unions.py
 tests/test_nested.py
 tests/test_nested_in_containers.py
 tests/test_new_style_annotations_min_py310.py
+tests/test_new_style_annotations_min_py312.py
 tests/test_new_style_annotations_min_py39.py
 tests/test_partial.py
 tests/test_positional_min_py38.py
 tests/test_pydantic.py
 tests/test_pydantic_with_newtype.py
 tests/test_self_type.py
 tests/test_strings.py
```

### Comparing `tyro-0.7.3/tests/test_attrs.py` & `tyro-0.8.0/tests/test_attrs.py`

 * *Files identical despite different names*

### Comparing `tyro-0.7.3/tests/test_base_configs_nested.py` & `tyro-0.8.0/tests/test_base_configs_nested.py`

 * *Files identical despite different names*

### Comparing `tyro-0.7.3/tests/test_boolean_optional.py` & `tyro-0.8.0/tests/test_boolean_optional.py`

 * *Files identical despite different names*

### Comparing `tyro-0.7.3/tests/test_collections.py` & `tyro-0.8.0/tests/test_collections.py`

 * *Files identical despite different names*

### Comparing `tyro-0.7.3/tests/test_completion.py` & `tyro-0.8.0/tests/test_completion.py`

 * *Files identical despite different names*

### Comparing `tyro-0.7.3/tests/test_conf.py` & `tyro-0.8.0/tests/test_conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import argparse
 import contextlib
 import dataclasses
 import io
 import json as json_
 import shlex
+import sys
 from typing import Any, Dict, Generic, List, Tuple, Type, TypeVar, Union
 
 import pytest
 from helptext_utils import get_helptext
 from typing_extensions import Annotated
 
 import tyro
@@ -1356,7 +1357,30 @@
     )
     target = io.StringIO()
     with pytest.raises(SystemExit), contextlib.redirect_stdout(target):
         instantiate_dataclasses((OptimizerConfig, DatasetConfig), args=["--help"])
     helptext = target.getvalue()
     assert "OptimizerConfig options" in helptext
     assert "DatasetConfig options" in helptext
+
+
+def test_counter_action() -> None:
+    def main(
+        verbosity: tyro.conf.UseCounterAction[int],
+        aliased_verbosity: Annotated[
+            tyro.conf.UseCounterAction[int], tyro.conf.arg(aliases=["-v"])
+        ],
+    ) -> Tuple[int, int]:
+        """Example showing how to use counter actions.
+        Args:
+            verbosity: Verbosity level.
+            aliased_verbosity: Same as above, but can also be specified with -v, -vv, -vvv, etc.
+        """
+        return verbosity, aliased_verbosity
+
+    assert tyro.cli(main, args=[]) == (0, 0)
+    assert tyro.cli(main, args="--verbosity --verbosity".split(" ")) == (2, 0)
+    assert tyro.cli(main, args="--verbosity --verbosity -v".split(" ")) == (2, 1)
+    if sys.version_info >= (3, 8):
+        # Doesn't work in Python 3.7 because of argparse limitations.
+        assert tyro.cli(main, args="--verbosity --verbosity -vv".split(" ")) == (2, 2)
+        assert tyro.cli(main, args="--verbosity --verbosity -vvv".split(" ")) == (2, 3)
```

### Comparing `tyro-0.7.3/tests/test_dcargs.py` & `tyro-0.8.0/tests/test_dcargs.py`

 * *Files identical despite different names*

### Comparing `tyro-0.7.3/tests/test_dict_namedtuple.py` & `tyro-0.8.0/tests/test_dict_namedtuple.py`

 * *Files identical despite different names*

### Comparing `tyro-0.7.3/tests/test_errors.py` & `tyro-0.8.0/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `tyro-0.7.3/tests/test_flax_min_py38.py` & `tyro-0.8.0/tests/test_flax_min_py38.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests initializing flax modules directly via tyro."""
+
 from typing import cast
 
 import jax
 import pytest
 from flax import linen as nn
 from helptext_utils import get_helptext
 from jax import numpy as jnp
```

### Comparing `tyro-0.7.3/tests/test_forward_ref.py` & `tyro-0.8.0/tests/test_forward_ref.py`

 * *Files identical despite different names*

### Comparing `tyro-0.7.3/tests/test_functools.py` & `tyro-0.8.0/tests/test_functools.py`

 * *Files identical despite different names*

### Comparing `tyro-0.7.3/tests/test_generics_and_serialization.py` & `tyro-0.8.0/tests/test_generics_and_serialization.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,25 @@
 
     SpecialInt = NewType("SpecialInt", int)
     assert tyro.cli(
         TupleGenericVariable[SpecialInt], args=["--xyz", "1", "2", "3"]
     ) == TupleGenericVariable((SpecialInt(1), SpecialInt(2), SpecialInt(3)))
 
 
+def test_tuple_generic_variable_newtype_container() -> None:
+    @dataclasses.dataclass
+    class TupleGenericVariable(Generic[ScalarType]):
+        xyz: Tuple[ScalarType, ...]
+
+    SpecialInt = NewType("SpecialInt", Tuple[int])
+    assert tyro.cli(
+        TupleGenericVariable[SpecialInt], args=["--xyz", "1", "2", "3"]
+    ) == TupleGenericVariable((SpecialInt((1,)), SpecialInt((2,)), SpecialInt((3,))))
+
+
 def test_tuple_generic_variable_more_newtype() -> None:
     @dataclasses.dataclass
     class TupleGenericVariable(Generic[ScalarType]):
         xyz: Tuple[ScalarType, ...]
 
     SpecialInt = NewType("SpecialInt", int)
     SpecialTuple = NewType("SpecialTuple", TupleGenericVariable[SpecialInt])
```

### Comparing `tyro-0.7.3/tests/test_helptext.py` & `tyro-0.8.0/tests/test_helptext.py`

 * *Files identical despite different names*

### Comparing `tyro-0.7.3/tests/test_initvar_min_py38.py` & `tyro-0.8.0/tests/test_initvar_min_py38.py`

 * *Files identical despite different names*

### Comparing `tyro-0.7.3/tests/test_is_nested_type.py` & `tyro-0.8.0/tests/test_is_nested_type.py`

 * *Files identical despite different names*

### Comparing `tyro-0.7.3/tests/test_missing.py` & `tyro-0.8.0/tests/test_missing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests for tyro.MISSING."""
+
 import contextlib
 import dataclasses
 import io
 from typing import Tuple
 
 import pytest
```

### Comparing `tyro-0.7.3/tests/test_missing_optional_packages.py` & `tyro-0.8.0/tests/test_missing_optional_packages.py`

 * *Files identical despite different names*

### Comparing `tyro-0.7.3/tests/test_mixed_unions.py` & `tyro-0.8.0/tests/test_mixed_unions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Tests for unsupported union types.
 
 Unions like `int | str` or `SomeDataclassA | SomeDataclassB` are OK (note that the latter
 will produce a pair of subcommands); when we write things like `int | SomeDataclassA`
 handling gets more complicated but should still be supported!
 """
 
-
 import dataclasses
 from typing import Any, Dict, List, Tuple, Union
 
 import pytest
 
 import tyro
```

### Comparing `tyro-0.7.3/tests/test_nested.py` & `tyro-0.8.0/tests/test_nested.py`

 * *Files identical despite different names*

### Comparing `tyro-0.7.3/tests/test_nested_in_containers.py` & `tyro-0.8.0/tests/test_nested_in_containers.py`

 * *Files identical despite different names*

### Comparing `tyro-0.7.3/tests/test_new_style_annotations_min_py310.py` & `tyro-0.8.0/tests/test_new_style_annotations_min_py310.py`

 * *Files identical despite different names*

### Comparing `tyro-0.7.3/tests/test_new_style_annotations_min_py39.py` & `tyro-0.8.0/tests/test_new_style_annotations_min_py39.py`

 * *Files identical despite different names*

### Comparing `tyro-0.7.3/tests/test_partial.py` & `tyro-0.8.0/tests/test_partial.py`

 * *Files identical despite different names*

### Comparing `tyro-0.7.3/tests/test_positional_min_py38.py` & `tyro-0.8.0/tests/test_positional_min_py38.py`

 * *Files identical despite different names*

### Comparing `tyro-0.7.3/tests/test_pydantic.py` & `tyro-0.8.0/tests/test_pydantic.py`

 * *Files identical despite different names*

### Comparing `tyro-0.7.3/tests/test_pydantic_with_newtype.py` & `tyro-0.8.0/tests/test_pydantic_with_newtype.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 import tyro
 
 Microliter = NewType("Microliter", int)
 
 
 class Measurements(BaseModel):
     single: Microliter = pydantic.Field(10)
-    renamed_single: Annotated[
-        Microliter, tyro.conf.arg(name="other_single")
-    ] = pydantic.Field(10)
+    renamed_single: Annotated[Microliter, tyro.conf.arg(name="other_single")] = (
+        pydantic.Field(10)
+    )
     pair: Tuple[Microliter, Microliter] = pydantic.Field((20, 30))
 
 
 IncorrectMeasurements = NewType("IncorrectMeasurements", Measurements)
 
 
 def test_pydantic_with_newtype():
```

### Comparing `tyro-0.7.3/tests/test_self_type.py` & `tyro-0.8.0/tests/test_self_type.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,90 +2,89 @@
 
 import pytest
 from typing_extensions import Self
 
 import tyro
 
 
-class TestClass:
+class SomeClass:
     def __init__(self, a: int, b: int) -> None:
         self.a = a
         self.b = b
 
     def method1(self, x: Self) -> None:
         self.effect = x
 
     @classmethod
-    def method2(cls, x: Self) -> TestClass:
+    def method2(cls, x: Self) -> SomeClass:
         return x
 
     # Self is not valid in static methods.
     # https://peps.python.org/pep-0673/#valid-locations-for-self
     #
     # @staticmethod
     # def method3(x: Self) -> TestClass:
     #     return x
 
 
-class TestSubclass(TestClass):
-    ...
+class SomeSubclass(SomeClass): ...
 
 
 def test_method() -> None:
-    x = TestClass(0, 0)
+    x = SomeClass(0, 0)
     with pytest.raises(SystemExit):
         tyro.cli(x.method1, args=[])
 
     assert tyro.cli(x.method1, args="--x.a 3 --x.b 3".split(" ")) is None
     assert x.effect.a == 3 and x.effect.b == 3
-    assert isinstance(x, TestClass)
+    assert isinstance(x, SomeClass)
 
 
 def test_classmethod() -> None:
-    x = TestClass(0, 0)
+    x = SomeClass(0, 0)
     with pytest.raises(SystemExit):
         tyro.cli(x.method2, args=[])
     with pytest.raises(SystemExit):
-        tyro.cli(TestClass.method2, args=[])
+        tyro.cli(SomeClass.method2, args=[])
 
     y = tyro.cli(x.method2, args="--x.a 3 --x.b 3".split(" "))
     assert y.a == 3
     assert y.b == 3
-    assert isinstance(y, TestClass)
+    assert isinstance(y, SomeClass)
 
-    y = tyro.cli(TestClass.method2, args="--x.a 3 --x.b 3".split(" "))
+    y = tyro.cli(SomeClass.method2, args="--x.a 3 --x.b 3".split(" "))
     assert y.a == 3
     assert y.b == 3
-    assert isinstance(y, TestClass)
+    assert isinstance(y, SomeClass)
 
 
 def test_subclass_method() -> None:
-    x = TestSubclass(0, 0)
+    x = SomeSubclass(0, 0)
     with pytest.raises(SystemExit):
         tyro.cli(x.method1, args=[])
 
     assert tyro.cli(x.method1, args="--x.a 3 --x.b 3".split(" ")) is None
     assert x.effect.a == 3 and x.effect.b == 3
-    assert isinstance(x, TestSubclass)
+    assert isinstance(x, SomeSubclass)
 
     y = tyro.cli(x.method2, args="--x.a 3 --x.b 3".split(" "))
     assert y.a == 3
     assert y.b == 3
-    assert isinstance(y, TestClass)
+    assert isinstance(y, SomeClass)
 
 
 def test_subclass_classmethod() -> None:
-    x = TestSubclass(0, 0)
+    x = SomeSubclass(0, 0)
     with pytest.raises(SystemExit):
         tyro.cli(x.method2, args=[])
     with pytest.raises(SystemExit):
-        tyro.cli(TestSubclass.method2, args=[])
+        tyro.cli(SomeSubclass.method2, args=[])
 
     y = tyro.cli(x.method2, args="--x.a 3 --x.b 3".split(" "))
     assert y.a == 3
     assert y.b == 3
-    assert isinstance(y, TestClass)
+    assert isinstance(y, SomeClass)
 
-    y = tyro.cli(TestSubclass.method2, args="--x.a 3 --x.b 3".split(" "))
+    y = tyro.cli(SomeSubclass.method2, args="--x.a 3 --x.b 3".split(" "))
     assert y.a == 3
     assert y.b == 3
-    assert isinstance(y, TestClass)
+    assert isinstance(y, SomeClass)
```

### Comparing `tyro-0.7.3/tests/test_strings.py` & `tyro-0.8.0/tests/test_strings.py`

 * *Files identical despite different names*

### Comparing `tyro-0.7.3/tests/test_tuple_with_subcommands.py` & `tyro-0.8.0/tests/test_tuple_with_subcommands.py`

 * *Files identical despite different names*

### Comparing `tyro-0.7.3/tests/test_union_from_mapping.py` & `tyro-0.8.0/tests/test_union_from_mapping.py`

 * *Files identical despite different names*

### Comparing `tyro-0.7.3/tests/test_unsupported_but_should_work.py` & `tyro-0.8.0/tests/test_unsupported_but_should_work.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Tests for features that are not officially features, but should work.
 
 Includes things like omegaconf.MISSING, attrs, etc, which mostly work but either likely
 have corner cases or just seem sketchy.
 """
+
 from typing import Tuple
 
 import omegaconf
 import pytest
 
 import tyro
 import tyro._strings
```

