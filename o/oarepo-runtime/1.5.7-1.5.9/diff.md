# Comparing `tmp/oarepo-runtime-1.5.7.tar.gz` & `tmp/oarepo-runtime-1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-runtime-1.5.7.tar", last modified: Mon Feb 19 15:55:56 2024, max compression
+gzip compressed data, was "oarepo-runtime-1.5.9.tar", last modified: Tue Feb 20 15:23:19 2024, max compression
```

## Comparing `oarepo-runtime-1.5.7.tar` & `oarepo-runtime-1.5.9.tar`

### file list

```diff
@@ -1,154 +1,154 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 15:55:56.929361 oarepo-runtime-1.5.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4774 2024-02-19 15:55:56.929361 oarepo-runtime-1.5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 15:55:56.909361 oarepo-runtime-1.5.7/oarepo_runtime/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 15:55:56.913361 oarepo-runtime-1.5.7/oarepo_runtime/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/cli/assets.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/cli/cf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4935 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/cli/check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/cli/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/cli/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     5447 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/cli/index.py
--rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/cli/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 15:55:56.913361 oarepo-runtime-1.5.7/oarepo_runtime/datastreams/
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/datastreams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7396 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/datastreams/asynchronous.py
--rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/datastreams/catalogue.py
--rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/datastreams/datastreams.py
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/datastreams/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/datastreams/ext.py
--rw-r--r--   0 runner    (1001) docker     (127)     7770 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/datastreams/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/datastreams/json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 15:55:56.917361 oarepo-runtime-1.5.7/oarepo_runtime/datastreams/readers/
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/datastreams/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/datastreams/readers/attachments.py
--rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/datastreams/readers/excel.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/datastreams/readers/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/datastreams/readers/service.py
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/datastreams/readers/yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/datastreams/semi_asynchronous.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/datastreams/synchronous.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/datastreams/transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9908 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/datastreams/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/datastreams/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 15:55:56.917361 oarepo-runtime-1.5.7/oarepo_runtime/datastreams/writers/
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/datastreams/writers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/datastreams/writers/attachments_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/datastreams/writers/attachments_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     3920 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/datastreams/writers/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/datastreams/writers/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/datastreams/writers/validation_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/datastreams/writers/yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/ext.py
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/ext_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 15:55:56.917361 oarepo-runtime-1.5.7/oarepo_runtime/i18n/
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/i18n/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 15:55:56.917361 oarepo-runtime-1.5.7/oarepo_runtime/info/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10399 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/info/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 15:55:56.917361 oarepo-runtime-1.5.7/oarepo_runtime/records/
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/records/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 15:55:56.917361 oarepo-runtime-1.5.7/oarepo_runtime/records/dumpers/
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/records/dumpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/records/dumpers/edtf_interval.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/records/dumpers/multilingual_dumper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 15:55:56.917361 oarepo-runtime-1.5.7/oarepo_runtime/records/entity_resolvers/
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/records/entity_resolvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/records/entity_resolvers/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 15:55:56.921361 oarepo-runtime-1.5.7/oarepo_runtime/records/relations/
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/records/relations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8981 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/records/relations/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/records/relations/internal.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/records/relations/lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/records/relations/pid_relation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 15:55:56.921361 oarepo-runtime-1.5.7/oarepo_runtime/records/systemfields/
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/records/systemfields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/records/systemfields/featured_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/records/systemfields/has_draftcheck.py
--rw-r--r--   0 runner    (1001) docker     (127)     5951 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/records/systemfields/icu.py
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/records/systemfields/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/records/systemfields/record_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/records/systemfields/synthetic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 15:55:56.921361 oarepo-runtime-1.5.7/oarepo_runtime/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/resources/file_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/resources/localized_ui_json_serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 15:55:56.921361 oarepo-runtime-1.5.7/oarepo_runtime/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 15:55:56.921361 oarepo-runtime-1.5.7/oarepo_runtime/services/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/services/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6114 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/services/config/permissions_presets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/services/config/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 15:55:56.921361 oarepo-runtime-1.5.7/oarepo_runtime/services/custom_fields/
--rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/services/custom_fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4433 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/services/custom_fields/mappings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 15:55:56.921361 oarepo-runtime-1.5.7/oarepo_runtime/services/expansions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/services/expansions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/services/expansions/expandable_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/services/expansions/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 15:55:56.925361 oarepo-runtime-1.5.7/oarepo_runtime/services/facets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/services/facets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/services/facets/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/services/facets/date.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/services/facets/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/services/facets/facet_groups_names.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/services/facets/max_facet.py
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/services/facets/nested_facet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/services/facets/params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 15:55:56.925361 oarepo-runtime-1.5.7/oarepo_runtime/services/files/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/services/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/services/files/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 15:55:56.925361 oarepo-runtime-1.5.7/oarepo_runtime/services/relations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/services/relations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/services/relations/components.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/services/relations/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/services/relations/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/services/results.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 15:55:56.925361 oarepo-runtime-1.5.7/oarepo_runtime/services/schema/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/services/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/services/schema/cf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/services/schema/i18n.py
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/services/schema/i18n_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/services/schema/i18n_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/services/schema/marshmallow.py
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/services/schema/polymorphic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/services/schema/ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/services/schema/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/services/search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 15:55:56.929361 oarepo-runtime-1.5.7/oarepo_runtime/translations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 15:55:56.905361 oarepo-runtime-1.5.7/oarepo_runtime/translations/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 15:55:56.929361 oarepo-runtime-1.5.7/oarepo_runtime/translations/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/translations/cs/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/translations/cs/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/translations/default_translations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 15:55:56.905361 oarepo-runtime-1.5.7/oarepo_runtime/translations/en/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 15:55:56.929361 oarepo-runtime-1.5.7/oarepo_runtime/translations/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/translations/en/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/translations/en/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/translations/jinjax_messages.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/translations/messages.pot
--rw-r--r--   0 runner    (1001) docker     (127)     4412 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/uow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 15:55:56.929361 oarepo-runtime-1.5.7/oarepo_runtime/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/utils/functools.py
--rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/oarepo_runtime/utils/path.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 15:55:56.929361 oarepo-runtime-1.5.7/oarepo_runtime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4774 2024-02-19 15:55:56.000000 oarepo-runtime-1.5.7/oarepo_runtime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4904 2024-02-19 15:55:56.000000 oarepo-runtime-1.5.7/oarepo_runtime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 15:55:56.000000 oarepo-runtime-1.5.7/oarepo_runtime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-02-19 15:55:56.000000 oarepo-runtime-1.5.7/oarepo_runtime.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-02-19 15:55:56.000000 oarepo-runtime-1.5.7/oarepo_runtime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-19 15:55:56.000000 oarepo-runtime-1.5.7/oarepo_runtime.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-02-19 15:55:56.929361 oarepo-runtime-1.5.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 15:55:56.905361 oarepo-runtime-1.5.7/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 15:55:56.929361 oarepo-runtime-1.5.7/tests/pkg_data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 15:51:14.000000 oarepo-runtime-1.5.7/tests/pkg_data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 15:23:19.775439 oarepo-runtime-1.5.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4774 2024-02-20 15:23:19.775439 oarepo-runtime-1.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 15:23:19.759439 oarepo-runtime-1.5.9/oarepo_runtime/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 15:23:19.759439 oarepo-runtime-1.5.9/oarepo_runtime/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/cli/assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/cli/cf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4935 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/cli/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/cli/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/cli/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5447 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/cli/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/cli/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 15:23:19.763439 oarepo-runtime-1.5.9/oarepo_runtime/datastreams/
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/datastreams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7396 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/datastreams/asynchronous.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/datastreams/catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/datastreams/datastreams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/datastreams/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/datastreams/ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7770 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/datastreams/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/datastreams/json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 15:23:19.763439 oarepo-runtime-1.5.9/oarepo_runtime/datastreams/readers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/datastreams/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/datastreams/readers/attachments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/datastreams/readers/excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/datastreams/readers/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/datastreams/readers/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/datastreams/readers/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/datastreams/semi_asynchronous.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/datastreams/synchronous.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/datastreams/transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9908 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/datastreams/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/datastreams/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 15:23:19.767439 oarepo-runtime-1.5.9/oarepo_runtime/datastreams/writers/
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/datastreams/writers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/datastreams/writers/attachments_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/datastreams/writers/attachments_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3920 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/datastreams/writers/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/datastreams/writers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/datastreams/writers/validation_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/datastreams/writers/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/ext_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 15:23:19.767439 oarepo-runtime-1.5.9/oarepo_runtime/i18n/
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/i18n/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 15:23:19.767439 oarepo-runtime-1.5.9/oarepo_runtime/info/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10399 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/info/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 15:23:19.767439 oarepo-runtime-1.5.9/oarepo_runtime/records/
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/records/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 15:23:19.767439 oarepo-runtime-1.5.9/oarepo_runtime/records/dumpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/records/dumpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/records/dumpers/edtf_interval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/records/dumpers/multilingual_dumper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 15:23:19.767439 oarepo-runtime-1.5.9/oarepo_runtime/records/entity_resolvers/
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/records/entity_resolvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/records/entity_resolvers/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 15:23:19.767439 oarepo-runtime-1.5.9/oarepo_runtime/records/relations/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/records/relations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8981 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/records/relations/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/records/relations/internal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/records/relations/lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/records/relations/pid_relation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 15:23:19.767439 oarepo-runtime-1.5.9/oarepo_runtime/records/systemfields/
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/records/systemfields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/records/systemfields/featured_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/records/systemfields/has_draftcheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/records/systemfields/icu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/records/systemfields/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/records/systemfields/record_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/records/systemfields/synthetic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 15:23:19.771439 oarepo-runtime-1.5.9/oarepo_runtime/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/resources/file_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/resources/localized_ui_json_serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 15:23:19.771439 oarepo-runtime-1.5.9/oarepo_runtime/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 15:23:19.771439 oarepo-runtime-1.5.9/oarepo_runtime/services/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/services/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6114 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/services/config/permissions_presets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/services/config/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 15:23:19.771439 oarepo-runtime-1.5.9/oarepo_runtime/services/custom_fields/
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/services/custom_fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4433 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/services/custom_fields/mappings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 15:23:19.771439 oarepo-runtime-1.5.9/oarepo_runtime/services/expansions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/services/expansions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/services/expansions/expandable_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/services/expansions/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 15:23:19.771439 oarepo-runtime-1.5.9/oarepo_runtime/services/facets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/services/facets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/services/facets/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/services/facets/date.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/services/facets/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/services/facets/facet_groups_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/services/facets/max_facet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/services/facets/nested_facet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/services/facets/params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 15:23:19.771439 oarepo-runtime-1.5.9/oarepo_runtime/services/files/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/services/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/services/files/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 15:23:19.771439 oarepo-runtime-1.5.9/oarepo_runtime/services/relations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/services/relations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/services/relations/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/services/relations/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/services/relations/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/services/results.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 15:23:19.775439 oarepo-runtime-1.5.9/oarepo_runtime/services/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/services/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/services/schema/cf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/services/schema/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/services/schema/i18n_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/services/schema/i18n_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/services/schema/marshmallow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/services/schema/polymorphic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/services/schema/ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/services/schema/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/services/search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 15:23:19.775439 oarepo-runtime-1.5.9/oarepo_runtime/translations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 15:23:19.755439 oarepo-runtime-1.5.9/oarepo_runtime/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 15:23:19.775439 oarepo-runtime-1.5.9/oarepo_runtime/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/translations/cs/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/translations/cs/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/translations/default_translations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 15:23:19.755439 oarepo-runtime-1.5.9/oarepo_runtime/translations/en/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 15:23:19.775439 oarepo-runtime-1.5.9/oarepo_runtime/translations/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/translations/en/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/translations/en/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/translations/jinjax_messages.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/translations/messages.pot
+-rw-r--r--   0 runner    (1001) docker     (127)     4412 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/uow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 15:23:19.775439 oarepo-runtime-1.5.9/oarepo_runtime/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/utils/functools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/oarepo_runtime/utils/path.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 15:23:19.775439 oarepo-runtime-1.5.9/oarepo_runtime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4774 2024-02-20 15:23:19.000000 oarepo-runtime-1.5.9/oarepo_runtime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4904 2024-02-20 15:23:19.000000 oarepo-runtime-1.5.9/oarepo_runtime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-20 15:23:19.000000 oarepo-runtime-1.5.9/oarepo_runtime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-02-20 15:23:19.000000 oarepo-runtime-1.5.9/oarepo_runtime.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-02-20 15:23:19.000000 oarepo-runtime-1.5.9/oarepo_runtime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-20 15:23:19.000000 oarepo-runtime-1.5.9/oarepo_runtime.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-02-20 15:23:19.779439 oarepo-runtime-1.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 15:23:19.755439 oarepo-runtime-1.5.9/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 15:23:19.775439 oarepo-runtime-1.5.9/tests/pkg_data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 15:18:12.000000 oarepo-runtime-1.5.9/tests/pkg_data/__init__.py
```

### Comparing `oarepo-runtime-1.5.7/LICENSE` & `oarepo-runtime-1.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/PKG-INFO` & `oarepo-runtime-1.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-runtime
-Version: 1.5.7
+Version: 1.5.9
 Summary: A set of runtime extensions of Invenio repository
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: invenio-records>=0.3.1
 Requires-Dist: invenio-search>=2.1.0
 Requires-Dist: invenio_records_resources>=0.21.4
 Requires-Dist: marshmallow
```

### Comparing `oarepo-runtime-1.5.7/README.md` & `oarepo-runtime-1.5.9/README.md`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/cli/assets.py` & `oarepo-runtime-1.5.9/oarepo_runtime/cli/assets.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/cli/base.py` & `oarepo-runtime-1.5.9/oarepo_runtime/cli/base.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/cli/check.py` & `oarepo-runtime-1.5.9/oarepo_runtime/cli/check.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/cli/configuration.py` & `oarepo-runtime-1.5.9/oarepo_runtime/cli/configuration.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/cli/fixtures.py` & `oarepo-runtime-1.5.9/oarepo_runtime/cli/fixtures.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/cli/index.py` & `oarepo-runtime-1.5.9/oarepo_runtime/cli/index.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/cli/validate.py` & `oarepo-runtime-1.5.9/oarepo_runtime/cli/validate.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/datastreams/__init__.py` & `oarepo-runtime-1.5.9/oarepo_runtime/datastreams/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/datastreams/asynchronous.py` & `oarepo-runtime-1.5.9/oarepo_runtime/datastreams/asynchronous.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/datastreams/catalogue.py` & `oarepo-runtime-1.5.9/oarepo_runtime/datastreams/catalogue.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/datastreams/datastreams.py` & `oarepo-runtime-1.5.9/oarepo_runtime/datastreams/datastreams.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/datastreams/errors.py` & `oarepo-runtime-1.5.9/oarepo_runtime/datastreams/errors.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/datastreams/ext.py` & `oarepo-runtime-1.5.9/oarepo_runtime/datastreams/ext.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/datastreams/fixtures.py` & `oarepo-runtime-1.5.9/oarepo_runtime/datastreams/fixtures.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/datastreams/readers/__init__.py` & `oarepo-runtime-1.5.9/oarepo_runtime/datastreams/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/datastreams/readers/attachments.py` & `oarepo-runtime-1.5.9/oarepo_runtime/datastreams/readers/attachments.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/datastreams/readers/excel.py` & `oarepo-runtime-1.5.9/oarepo_runtime/datastreams/readers/excel.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/datastreams/readers/json.py` & `oarepo-runtime-1.5.9/oarepo_runtime/datastreams/readers/json.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/datastreams/readers/service.py` & `oarepo-runtime-1.5.9/oarepo_runtime/datastreams/readers/service.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/datastreams/semi_asynchronous.py` & `oarepo-runtime-1.5.9/oarepo_runtime/datastreams/semi_asynchronous.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/datastreams/synchronous.py` & `oarepo-runtime-1.5.9/oarepo_runtime/datastreams/synchronous.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/datastreams/transformers.py` & `oarepo-runtime-1.5.9/oarepo_runtime/datastreams/transformers.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/datastreams/types.py` & `oarepo-runtime-1.5.9/oarepo_runtime/datastreams/types.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/datastreams/utils.py` & `oarepo-runtime-1.5.9/oarepo_runtime/datastreams/utils.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/datastreams/writers/__init__.py` & `oarepo-runtime-1.5.9/oarepo_runtime/datastreams/writers/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/datastreams/writers/attachments_file.py` & `oarepo-runtime-1.5.9/oarepo_runtime/datastreams/writers/attachments_file.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/datastreams/writers/attachments_service.py` & `oarepo-runtime-1.5.9/oarepo_runtime/datastreams/writers/attachments_service.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/datastreams/writers/service.py` & `oarepo-runtime-1.5.9/oarepo_runtime/datastreams/writers/service.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/datastreams/writers/utils.py` & `oarepo-runtime-1.5.9/oarepo_runtime/datastreams/writers/utils.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/datastreams/writers/validation_errors.py` & `oarepo-runtime-1.5.9/oarepo_runtime/datastreams/writers/validation_errors.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/datastreams/writers/yaml.py` & `oarepo-runtime-1.5.9/oarepo_runtime/datastreams/writers/yaml.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/ext.py` & `oarepo-runtime-1.5.9/oarepo_runtime/ext.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/ext_config.py` & `oarepo-runtime-1.5.9/oarepo_runtime/ext_config.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/info/views.py` & `oarepo-runtime-1.5.9/oarepo_runtime/info/views.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/profile.py` & `oarepo-runtime-1.5.9/oarepo_runtime/profile.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/records/dumpers/edtf_interval.py` & `oarepo-runtime-1.5.9/oarepo_runtime/records/dumpers/edtf_interval.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/records/dumpers/multilingual_dumper.py` & `oarepo-runtime-1.5.9/oarepo_runtime/records/dumpers/multilingual_dumper.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/records/entity_resolvers/__init__.py` & `oarepo-runtime-1.5.9/oarepo_runtime/records/entity_resolvers/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/records/entity_resolvers/proxies.py` & `oarepo-runtime-1.5.9/oarepo_runtime/records/entity_resolvers/proxies.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/records/relations/base.py` & `oarepo-runtime-1.5.9/oarepo_runtime/records/relations/base.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/records/relations/internal.py` & `oarepo-runtime-1.5.9/oarepo_runtime/records/relations/internal.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/records/relations/lookup.py` & `oarepo-runtime-1.5.9/oarepo_runtime/records/relations/lookup.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/records/relations/pid_relation.py` & `oarepo-runtime-1.5.9/oarepo_runtime/records/relations/pid_relation.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/records/systemfields/featured_file.py` & `oarepo-runtime-1.5.9/oarepo_runtime/records/systemfields/featured_file.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,44 +2,44 @@
 from invenio_records.systemfields import SystemField
 from invenio_records_resources.proxies import current_service_registry
 
 from oarepo_runtime.datastreams.utils import get_file_service_for_record_service
 from oarepo_runtime.records.systemfields.mapping import MappingSystemFieldMixin
 
 
-class FeaturedFileFieldResult(MappingSystemFieldMixin):
+class FeaturedFileFieldResult:
     def __init__(self, record=None):
         super().__init__()
         self.record = record
 
-    def search_dump(self, data):
+
+class FeaturedFileField(MappingSystemFieldMixin, SystemField):
+    def __init__(self, source_field):
+        super(FeaturedFileField, self).__init__(source_field)
+
+    def __get__(self, instance, owner):
+        if instance is None:
+            return self
+        result = FeaturedFileFieldResult(record=instance)
+        return result
+
+    def search_dump(self, data, record):
         for service in current_service_registry._services:
             if getattr(
                 current_service_registry._services[service], "record_cls"
-            ) == type(self.record):
+            ) == type(record):
                 file_service = get_file_service_for_record_service(
                     record_service=current_service_registry._services[service],
-                    record=self.record,
+                    record=record,
                 )
 
-                files = file_service.list_files(system_identity, self.record["id"])
+                files = file_service.list_files(system_identity, record["id"])
                 file_list = list(files.entries)
 
                 for file in file_list:
                     if (
                         file["metadata"]
                         and "featured" in file["metadata"]
                         and file["metadata"]["featured"]
                     ):
-                        self.record["metadata"].update({"featured": file})
-                        self.record.commit()
-
-
-class FeaturedFileField(SystemField):
-    def __init__(self, source_field):
-        super(FeaturedFileField, self).__init__()
-
-    def __get__(self, instance, owner):
-        if instance is None:
-            return None
-        result = FeaturedFileFieldResult(record=instance)
-        return result
+                        record["metadata"].update({"featured": file})
+                        record.commit()
```

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/records/systemfields/has_draftcheck.py` & `oarepo-runtime-1.5.9/oarepo_runtime/records/systemfields/has_draftcheck.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/records/systemfields/icu.py` & `oarepo-runtime-1.5.9/oarepo_runtime/records/systemfields/icu.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from flask import current_app
 from invenio_records.systemfields import SystemField
 
 from oarepo_runtime.records.relations.lookup import lookup_key
 from oarepo_runtime.records.systemfields.mapping import MappingSystemFieldMixin
 
 
-class ICUField(SystemField):
+class ICUField(MappingSystemFieldMixin, SystemField):
     """
     A system field that acts as an opensearch "proxy" to another field.
     It creates a top-level mapping field with the same name and copies
     content of {another field}.language into {mapping field}.language.
 
     The language accessor can be modified by overriding get_values method.
     """
@@ -40,28 +40,28 @@
                 ret.append(l.value)
             elif isinstance(l.value, dict):
                 val = l.value.get(language)
                 if val:
                     ret.append(val)
         return ret
 
-    def search_dump(self, data):
+    def search_dump(self, data, record):
         ret = {}
         for lang in self.languages:
             ret[lang] = self.get_values(data, lang)
         data[self.attr_name] = ret
 
-    def search_load(self, data):
+    def search_load(self, data, record_cls):
         data.pop(self.attr_name, None)
 
     def __get__(self, instance, owner):
         return self
 
 
-class ICUSortField(MappingSystemFieldMixin, ICUField):
+class ICUSortField(ICUField):
     """
     A field that adds icu sorting field
     """
 
     def __init__(self, *, source_field, key=None):
         super().__init__(source_field=source_field, key=key)
 
@@ -79,15 +79,15 @@
                     }
                     for lang, setting in self.languages.items()
                 },
             },
         }
 
 
-class ICUSuggestField(MappingSystemFieldMixin, ICUField):
+class ICUSuggestField(ICUField):
     """
     A field that adds icu-aware suggestion field
     """
 
     def __init__(self, source_field, key=None):
         super().__init__(source_field=source_field, key=key)
 
@@ -128,15 +128,15 @@
                         "filter": ["lowercase", "asciifolding"],
                     }
                 }
             }
         }
 
 
-class ICUSearchField(MappingSystemFieldMixin, ICUField):
+class ICUSearchField(ICUField):
     """
     A field that adds stemming-aware search field
     """
 
     default_stemming_analyzers = {
         "stemming_analyzer_cs": {
             "tokenizer": "standard",
```

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/records/systemfields/record_status.py` & `oarepo-runtime-1.5.9/oarepo_runtime/records/systemfields/record_status.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 from invenio_records.systemfields import SystemField
 
 from .mapping import MappingSystemFieldMixin
 
 
-class RecordStatusResult(MappingSystemFieldMixin):
+class RecordStatusResult:
     def __init__(self, record, attr_name):
         self.record = record
         self.attr_name = attr_name
 
-    def search_dump(self, data):
-        if getattr(self.record, "is_draft"):
-            data[self.attr_name] = "draft"
-        else:
-            data[self.attr_name] = "published"
-
 
 class RecordStatusSystemField(MappingSystemFieldMixin, SystemField):
     @property
     def mapping(self):
         return {
             self.attr_name: {
                 "type": "keyword",
             },
         }
 
-    def search_load(self, data):
+    def search_load(self, data, record_cls):
         data.pop(self.attr_name, None)
 
+    def search_dump(self, data, record):
+        if getattr(record, "is_draft"):
+            data[self.attr_name] = "draft"
+        else:
+            data[self.attr_name] = "published"
+
     def __get__(self, record, owner=None):
         """Accessing the attribute."""
         # Class access
         if record is None:
             return self
         return RecordStatusResult(record, self.attr_name)
```

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/records/systemfields/synthetic.py` & `oarepo-runtime-1.5.9/oarepo_runtime/records/systemfields/synthetic.py`

 * *Files 7% similar despite different names*

```diff
@@ -58,21 +58,21 @@
             facet-groups:
             - default
           label.cs: Rok obhajoby
           label.en: Defense year
            ```
     """
 
-    def search_dump(self, data):
+    def search_dump(self, data, record):
         dt = self._value(data)
         if dt:
             data[self.key] = dt
 
-    def search_load(self, data):
-        data.pop(self.key)
+    def search_load(self, data, record_cls):
+        data.pop(self.key, None)
 
     def __get__(self, record, owner=None):
         if record is None:
             return self
         return self._value(record)
 
     def _value(self, data):
```

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/resources/localized_ui_json_serializer.py` & `oarepo-runtime-1.5.9/oarepo_runtime/resources/localized_ui_json_serializer.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/services/config/permissions_presets.py` & `oarepo-runtime-1.5.9/oarepo_runtime/services/config/permissions_presets.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/services/config/service.py` & `oarepo-runtime-1.5.9/oarepo_runtime/services/config/service.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/services/custom_fields/__init__.py` & `oarepo-runtime-1.5.9/oarepo_runtime/services/custom_fields/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,22 +17,22 @@
         custom_fields: List[BaseCF] = current_app.config[self.config_key]
         return {cf.name: cf.mapping for cf in custom_fields}
 
     @property
     def mapping_settings(self):
         return {}
 
-    def search_dump(self, data):
+    def search_dump(self, data, record):
         custom_fields = current_app.config.get(self.config_key, {})
 
         for cf in custom_fields:
             cf.dump(data, cf_key=self.key)
         return data
 
-    def search_load(self, data):
+    def search_load(self, data, record_cls):
         custom_fields = current_app.config.get(self.config_key, {})
 
         for cf in custom_fields:
             cf.load(data, cf_key=self.key)
         return data
```

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/services/custom_fields/mappings.py` & `oarepo-runtime-1.5.9/oarepo_runtime/services/custom_fields/mappings.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/services/expansions/expandable_fields.py` & `oarepo-runtime-1.5.9/oarepo_runtime/services/expansions/expandable_fields.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/services/facets/date.py` & `oarepo-runtime-1.5.9/oarepo_runtime/services/facets/date.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/services/facets/nested_facet.py` & `oarepo-runtime-1.5.9/oarepo_runtime/services/facets/nested_facet.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/services/facets/params.py` & `oarepo-runtime-1.5.9/oarepo_runtime/services/facets/params.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/services/files/service.py` & `oarepo-runtime-1.5.9/oarepo_runtime/services/files/service.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/services/relations/components.py` & `oarepo-runtime-1.5.9/oarepo_runtime/services/relations/components.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/services/relations/errors.py` & `oarepo-runtime-1.5.9/oarepo_runtime/services/relations/errors.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/services/relations/mapping.py` & `oarepo-runtime-1.5.9/oarepo_runtime/services/relations/mapping.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/services/results.py` & `oarepo-runtime-1.5.9/oarepo_runtime/services/results.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/services/schema/i18n.py` & `oarepo-runtime-1.5.9/oarepo_runtime/services/schema/i18n.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/services/schema/i18n_ui.py` & `oarepo-runtime-1.5.9/oarepo_runtime/services/schema/i18n_ui.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/services/schema/marshmallow.py` & `oarepo-runtime-1.5.9/oarepo_runtime/services/schema/marshmallow.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/services/schema/ui.py` & `oarepo-runtime-1.5.9/oarepo_runtime/services/schema/ui.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/services/schema/validation.py` & `oarepo-runtime-1.5.9/oarepo_runtime/services/schema/validation.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/services/search.py` & `oarepo-runtime-1.5.9/oarepo_runtime/services/search.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/translations/cs/LC_MESSAGES/messages.mo` & `oarepo-runtime-1.5.9/oarepo_runtime/translations/cs/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/translations/cs/LC_MESSAGES/messages.po` & `oarepo-runtime-1.5.9/oarepo_runtime/translations/cs/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/translations/en/LC_MESSAGES/messages.po` & `oarepo-runtime-1.5.9/oarepo_runtime/translations/en/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/translations/messages.pot` & `oarepo-runtime-1.5.9/oarepo_runtime/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/uow.py` & `oarepo-runtime-1.5.9/oarepo_runtime/uow.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime/utils/path.py` & `oarepo-runtime-1.5.9/oarepo_runtime/utils/path.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime.egg-info/PKG-INFO` & `oarepo-runtime-1.5.9/oarepo_runtime.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-runtime
-Version: 1.5.7
+Version: 1.5.9
 Summary: A set of runtime extensions of Invenio repository
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: invenio-records>=0.3.1
 Requires-Dist: invenio-search>=2.1.0
 Requires-Dist: invenio_records_resources>=0.21.4
 Requires-Dist: marshmallow
```

### Comparing `oarepo-runtime-1.5.7/oarepo_runtime.egg-info/SOURCES.txt` & `oarepo-runtime-1.5.9/oarepo_runtime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.5.7/setup.cfg` & `oarepo-runtime-1.5.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oarepo-runtime
-version = 1.5.7
+version = 1.5.9
 description = A set of runtime extensions of Invenio repository
 authors = Alzbeta Pokorna
 readme = README.md
 long_description = file:README.md
 long_description_content_type = text/markdown
 
 [options]
```

