# Comparing `tmp/folio_migration_tools-1.9.0a1.tar.gz` & `tmp/folio_migration_tools-1.9.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "folio_migration_tools-1.9.0a1.tar", max compression
+gzip compressed data, was "folio_migration_tools-1.9.0a2.tar", max compression
```

## Comparing `folio_migration_tools-1.9.0a1.tar` & `folio_migration_tools-1.9.0a2.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0     1072 2023-03-06 22:17:01.793515 folio_migration_tools-1.9.0a1/LICENSE
--rw-r--r--   0        0        0     5962 2023-10-18 13:35:39.048796 folio_migration_tools-1.9.0a1/README.md
--rw-r--r--   0        0        0     1784 2024-01-10 22:31:28.492710 folio_migration_tools-1.9.0a1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-06 22:17:01.810173 folio_migration_tools-1.9.0a1/src/folio_migration_tools/__init__.py
--rw-r--r--   0        0        0     6498 2023-12-06 07:31:23.295073 folio_migration_tools-1.9.0a1/src/folio_migration_tools/__main__.py
--rw-r--r--   0        0        0    14193 2023-12-06 07:31:23.296245 folio_migration_tools-1.9.0a1/src/folio_migration_tools/circulation_helper.py
--rw-r--r--   0        0        0      227 2023-03-06 22:17:01.811146 folio_migration_tools-1.9.0a1/src/folio_migration_tools/colors.py
--rw-r--r--   0        0        0     2822 2023-10-24 20:24:55.166905 folio_migration_tools-1.9.0a1/src/folio_migration_tools/config_file_load.py
--rw-r--r--   0        0        0      648 2023-03-06 22:17:01.811423 folio_migration_tools-1.9.0a1/src/folio_migration_tools/custom_dict.py
--rw-r--r--   0        0        0     2509 2023-10-18 13:35:39.054388 folio_migration_tools-1.9.0a1/src/folio_migration_tools/custom_exceptions.py
--rw-r--r--   0        0        0     1678 2023-06-08 16:57:16.411848 folio_migration_tools-1.9.0a1/src/folio_migration_tools/extradata_writer.py
--rw-r--r--   0        0        0     6573 2023-06-08 16:57:16.412056 folio_migration_tools-1.9.0a1/src/folio_migration_tools/folder_structure.py
--rw-r--r--   0        0        0     2804 2023-10-18 13:35:39.055135 folio_migration_tools-1.9.0a1/src/folio_migration_tools/helper.py
--rw-r--r--   0        0        0     7559 2023-10-18 13:35:39.055414 folio_migration_tools-1.9.0a1/src/folio_migration_tools/holdings_helper.py
--rw-r--r--   0        0        0      228 2023-11-07 15:17:13.511136 folio_migration_tools-1.9.0a1/src/folio_migration_tools/i18n_config.py
--rw-r--r--   0        0        0     3128 2023-12-06 07:31:23.327960 folio_migration_tools-1.9.0a1/src/folio_migration_tools/library_configuration.py
--rw-r--r--   0        0        0    19595 2023-10-18 13:35:39.055823 folio_migration_tools-1.9.0a1/src/folio_migration_tools/mapper_base.py
--rw-r--r--   0        0        0        0 2023-03-06 22:17:01.813766 folio_migration_tools-1.9.0a1/src/folio_migration_tools/mapping_file_transformation/__init__.py
--rw-r--r--   0        0        0     8091 2023-10-18 13:35:39.056238 folio_migration_tools-1.9.0a1/src/folio_migration_tools/mapping_file_transformation/courses_mapper.py
--rw-r--r--   0        0        0     6882 2024-01-10 19:22:00.777947 folio_migration_tools-1.9.0a1/src/folio_migration_tools/mapping_file_transformation/holdings_mapper.py
--rw-r--r--   0        0        0    10511 2024-01-10 20:16:13.520290 folio_migration_tools-1.9.0a1/src/folio_migration_tools/mapping_file_transformation/item_mapper.py
--rw-r--r--   0        0        0    13402 2023-10-18 13:35:39.057023 folio_migration_tools-1.9.0a1/src/folio_migration_tools/mapping_file_transformation/manual_fee_fines_mapper.py
--rw-r--r--   0        0        0    38124 2023-10-24 20:24:55.167539 folio_migration_tools-1.9.0a1/src/folio_migration_tools/mapping_file_transformation/mapping_file_mapper_base.py
--rw-r--r--   0        0        0     3470 2023-10-18 13:35:39.057779 folio_migration_tools-1.9.0a1/src/folio_migration_tools/mapping_file_transformation/notes_mapper.py
--rw-r--r--   0        0        0    16784 2023-10-18 13:35:39.058514 folio_migration_tools-1.9.0a1/src/folio_migration_tools/mapping_file_transformation/order_mapper.py
--rw-r--r--   0        0        0    14569 2023-10-18 13:35:39.059340 folio_migration_tools-1.9.0a1/src/folio_migration_tools/mapping_file_transformation/organization_mapper.py
--rw-r--r--   0        0        0     8864 2023-10-18 13:35:39.060061 folio_migration_tools-1.9.0a1/src/folio_migration_tools/mapping_file_transformation/ref_data_mapping.py
--rw-r--r--   0        0        0     7844 2023-12-21 22:44:14.812490 folio_migration_tools-1.9.0a1/src/folio_migration_tools/mapping_file_transformation/user_mapper.py
--rw-r--r--   0        0        0        0 2023-03-06 22:17:01.816647 folio_migration_tools-1.9.0a1/src/folio_migration_tools/marc_rules_transformation/__init__.py
--rw-r--r--   0        0        0    35773 2023-11-01 16:09:15.672665 folio_migration_tools-1.9.0a1/src/folio_migration_tools/marc_rules_transformation/conditions.py
--rw-r--r--   0        0        0    11855 2023-10-18 13:35:39.061344 folio_migration_tools-1.9.0a1/src/folio_migration_tools/marc_rules_transformation/holdings_statementsparser.py
--rw-r--r--   0        0        0    10026 2023-11-01 02:11:35.293960 folio_migration_tools-1.9.0a1/src/folio_migration_tools/marc_rules_transformation/hrid_handler.py
--rw-r--r--   0        0        0   382912 2023-03-06 22:17:01.818293 folio_migration_tools-1.9.0a1/src/folio_migration_tools/marc_rules_transformation/loc_language_codes.xml
--rw-r--r--   0        0        0    10967 2024-01-10 19:00:16.663605 folio_migration_tools-1.9.0a1/src/folio_migration_tools/marc_rules_transformation/marc_file_processor.py
--rw-r--r--   0        0        0     5194 2023-10-18 13:35:39.062695 folio_migration_tools-1.9.0a1/src/folio_migration_tools/marc_rules_transformation/marc_reader_wrapper.py
--rw-r--r--   0        0        0     9681 2023-11-01 16:09:15.673801 folio_migration_tools-1.9.0a1/src/folio_migration_tools/marc_rules_transformation/rules_mapper_authorities.py
--rw-r--r--   0        0        0    37640 2023-12-06 07:31:23.300626 folio_migration_tools-1.9.0a1/src/folio_migration_tools/marc_rules_transformation/rules_mapper_base.py
--rw-r--r--   0        0        0    27280 2023-10-24 20:24:55.169285 folio_migration_tools-1.9.0a1/src/folio_migration_tools/marc_rules_transformation/rules_mapper_bibs.py
--rw-r--r--   0        0        0    17779 2024-01-10 19:01:50.408081 folio_migration_tools-1.9.0a1/src/folio_migration_tools/marc_rules_transformation/rules_mapper_holdings.py
--rw-r--r--   0        0        0     4258 2023-10-18 13:35:39.065017 folio_migration_tools-1.9.0a1/src/folio_migration_tools/migration_report.py
--rw-r--r--   0        0        0      211 2023-03-06 22:17:01.820491 folio_migration_tools-1.9.0a1/src/folio_migration_tools/migration_tasks/__init__.py
--rw-r--r--   0        0        0     4251 2023-10-18 13:35:39.066574 folio_migration_tools-1.9.0a1/src/folio_migration_tools/migration_tasks/authority_transformer.py
--rw-r--r--   0        0        0    27827 2024-01-10 18:58:02.458894 folio_migration_tools-1.9.0a1/src/folio_migration_tools/migration_tasks/batch_poster.py
--rw-r--r--   0        0        0     7380 2023-10-18 13:35:39.067859 folio_migration_tools-1.9.0a1/src/folio_migration_tools/migration_tasks/bibs_transformer.py
--rw-r--r--   0        0        0     5773 2023-10-18 13:35:39.068533 folio_migration_tools-1.9.0a1/src/folio_migration_tools/migration_tasks/courses_migrator.py
--rw-r--r--   0        0        0    19628 2024-01-10 20:01:02.033353 folio_migration_tools-1.9.0a1/src/folio_migration_tools/migration_tasks/holdings_csv_transformer.py
--rw-r--r--   0        0        0     9622 2023-10-18 13:35:39.069665 folio_migration_tools-1.9.0a1/src/folio_migration_tools/migration_tasks/holdings_marc_transformer.py
--rw-r--r--   0        0        0    15142 2023-10-18 13:35:39.070009 folio_migration_tools-1.9.0a1/src/folio_migration_tools/migration_tasks/items_transformer.py
--rw-r--r--   0        0        0    34399 2024-01-10 18:58:02.460806 folio_migration_tools-1.9.0a1/src/folio_migration_tools/migration_tasks/loans_migrator.py
--rw-r--r--   0        0        0     7356 2023-10-18 13:35:39.070917 folio_migration_tools-1.9.0a1/src/folio_migration_tools/migration_tasks/manual_fee_fines_transformer.py
--rw-r--r--   0        0        0    13875 2023-12-06 07:31:23.328692 folio_migration_tools-1.9.0a1/src/folio_migration_tools/migration_tasks/migration_task_base.py
--rw-r--r--   0        0        0    11477 2023-10-18 13:35:39.071281 folio_migration_tools-1.9.0a1/src/folio_migration_tools/migration_tasks/orders_transformer.py
--rw-r--r--   0        0        0    14920 2023-10-18 13:35:39.071521 folio_migration_tools-1.9.0a1/src/folio_migration_tools/migration_tasks/organization_transformer.py
--rw-r--r--   0        0        0    13309 2023-10-18 13:35:39.071785 folio_migration_tools-1.9.0a1/src/folio_migration_tools/migration_tasks/requests_migrator.py
--rw-r--r--   0        0        0     9213 2023-11-01 02:13:13.352012 folio_migration_tools-1.9.0a1/src/folio_migration_tools/migration_tasks/reserves_migrator.py
--rw-r--r--   0        0        0     9936 2023-12-21 22:44:14.816585 folio_migration_tools-1.9.0a1/src/folio_migration_tools/migration_tasks/user_transformer.py
--rw-r--r--   0        0        0      630 2023-12-06 07:31:23.329344 folio_migration_tools-1.9.0a1/src/folio_migration_tools/task_configuration.py
--rw-r--r--   0        0        0        0 2023-03-06 22:17:01.830348 folio_migration_tools-1.9.0a1/src/folio_migration_tools/test_infrastructure/__init__.py
--rw-r--r--   0        0        0     9150 2023-06-08 16:57:16.438864 folio_migration_tools-1.9.0a1/src/folio_migration_tools/test_infrastructure/mocked_classes.py
--rw-r--r--   0        0        0        0 2023-03-06 22:17:01.831318 folio_migration_tools-1.9.0a1/src/folio_migration_tools/transaction_migration/__init__.py
--rw-r--r--   0        0        0     5459 2023-12-06 07:31:23.306173 folio_migration_tools-1.9.0a1/src/folio_migration_tools/transaction_migration/legacy_loan.py
--rw-r--r--   0        0        0     6124 2023-03-06 22:17:01.831928 folio_migration_tools-1.9.0a1/src/folio_migration_tools/transaction_migration/legacy_request.py
--rw-r--r--   0        0        0     1839 2023-03-06 22:17:01.832344 folio_migration_tools-1.9.0a1/src/folio_migration_tools/transaction_migration/legacy_reserve.py
--rw-r--r--   0        0        0      656 2023-03-06 22:17:01.832638 folio_migration_tools-1.9.0a1/src/folio_migration_tools/transaction_migration/transaction_result.py
--rw-r--r--   0        0        0    38525 2023-11-07 15:17:13.512181 folio_migration_tools-1.9.0a1/src/folio_migration_tools/translations/en.json
--rw-r--r--   0        0        0     7525 1970-01-01 00:00:00.000000 folio_migration_tools-1.9.0a1/setup.py
--rw-r--r--   0        0        0     7256 1970-01-01 00:00:00.000000 folio_migration_tools-1.9.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-03-06 22:17:01.793515 folio_migration_tools-1.9.0a2/LICENSE
+-rw-r--r--   0        0        0     5962 2023-10-18 13:35:39.048796 folio_migration_tools-1.9.0a2/README.md
+-rw-r--r--   0        0        0     1784 2024-02-23 19:38:44.326015 folio_migration_tools-1.9.0a2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-06 22:17:01.810173 folio_migration_tools-1.9.0a2/src/folio_migration_tools/__init__.py
+-rw-r--r--   0        0        0     6498 2023-12-06 07:31:23.295073 folio_migration_tools-1.9.0a2/src/folio_migration_tools/__main__.py
+-rw-r--r--   0        0        0    14193 2023-12-06 07:31:23.296245 folio_migration_tools-1.9.0a2/src/folio_migration_tools/circulation_helper.py
+-rw-r--r--   0        0        0      227 2023-03-06 22:17:01.811146 folio_migration_tools-1.9.0a2/src/folio_migration_tools/colors.py
+-rw-r--r--   0        0        0     2822 2023-10-24 20:24:55.166905 folio_migration_tools-1.9.0a2/src/folio_migration_tools/config_file_load.py
+-rw-r--r--   0        0        0      648 2023-03-06 22:17:01.811423 folio_migration_tools-1.9.0a2/src/folio_migration_tools/custom_dict.py
+-rw-r--r--   0        0        0     2509 2023-10-18 13:35:39.054388 folio_migration_tools-1.9.0a2/src/folio_migration_tools/custom_exceptions.py
+-rw-r--r--   0        0        0     1678 2023-06-08 16:57:16.411848 folio_migration_tools-1.9.0a2/src/folio_migration_tools/extradata_writer.py
+-rw-r--r--   0        0        0     6573 2023-06-08 16:57:16.412056 folio_migration_tools-1.9.0a2/src/folio_migration_tools/folder_structure.py
+-rw-r--r--   0        0        0     2804 2023-10-18 13:35:39.055135 folio_migration_tools-1.9.0a2/src/folio_migration_tools/helper.py
+-rw-r--r--   0        0        0     7559 2023-10-18 13:35:39.055414 folio_migration_tools-1.9.0a2/src/folio_migration_tools/holdings_helper.py
+-rw-r--r--   0        0        0      228 2023-11-07 15:17:13.511136 folio_migration_tools-1.9.0a2/src/folio_migration_tools/i18n_config.py
+-rw-r--r--   0        0        0     3527 2024-02-23 19:36:38.879076 folio_migration_tools-1.9.0a2/src/folio_migration_tools/library_configuration.py
+-rw-r--r--   0        0        0    19595 2023-10-18 13:35:39.055823 folio_migration_tools-1.9.0a2/src/folio_migration_tools/mapper_base.py
+-rw-r--r--   0        0        0        0 2023-03-06 22:17:01.813766 folio_migration_tools-1.9.0a2/src/folio_migration_tools/mapping_file_transformation/__init__.py
+-rw-r--r--   0        0        0     8091 2023-10-18 13:35:39.056238 folio_migration_tools-1.9.0a2/src/folio_migration_tools/mapping_file_transformation/courses_mapper.py
+-rw-r--r--   0        0        0     6882 2024-02-23 19:36:53.901371 folio_migration_tools-1.9.0a2/src/folio_migration_tools/mapping_file_transformation/holdings_mapper.py
+-rw-r--r--   0        0        0    10511 2024-02-23 19:36:53.902140 folio_migration_tools-1.9.0a2/src/folio_migration_tools/mapping_file_transformation/item_mapper.py
+-rw-r--r--   0        0        0    13402 2023-10-18 13:35:39.057023 folio_migration_tools-1.9.0a2/src/folio_migration_tools/mapping_file_transformation/manual_fee_fines_mapper.py
+-rw-r--r--   0        0        0    38124 2023-10-24 20:24:55.167539 folio_migration_tools-1.9.0a2/src/folio_migration_tools/mapping_file_transformation/mapping_file_mapper_base.py
+-rw-r--r--   0        0        0     3470 2023-10-18 13:35:39.057779 folio_migration_tools-1.9.0a2/src/folio_migration_tools/mapping_file_transformation/notes_mapper.py
+-rw-r--r--   0        0        0    16784 2023-10-18 13:35:39.058514 folio_migration_tools-1.9.0a2/src/folio_migration_tools/mapping_file_transformation/order_mapper.py
+-rw-r--r--   0        0        0    14569 2023-10-18 13:35:39.059340 folio_migration_tools-1.9.0a2/src/folio_migration_tools/mapping_file_transformation/organization_mapper.py
+-rw-r--r--   0        0        0     8864 2023-10-18 13:35:39.060061 folio_migration_tools-1.9.0a2/src/folio_migration_tools/mapping_file_transformation/ref_data_mapping.py
+-rw-r--r--   0        0        0     7844 2024-02-01 21:19:09.538989 folio_migration_tools-1.9.0a2/src/folio_migration_tools/mapping_file_transformation/user_mapper.py
+-rw-r--r--   0        0        0        0 2023-03-06 22:17:01.816647 folio_migration_tools-1.9.0a2/src/folio_migration_tools/marc_rules_transformation/__init__.py
+-rw-r--r--   0        0        0    35773 2023-11-01 16:09:15.672665 folio_migration_tools-1.9.0a2/src/folio_migration_tools/marc_rules_transformation/conditions.py
+-rw-r--r--   0        0        0    11855 2024-02-23 19:36:29.954162 folio_migration_tools-1.9.0a2/src/folio_migration_tools/marc_rules_transformation/holdings_statementsparser.py
+-rw-r--r--   0        0        0    10026 2023-11-01 02:11:35.293960 folio_migration_tools-1.9.0a2/src/folio_migration_tools/marc_rules_transformation/hrid_handler.py
+-rw-r--r--   0        0        0   382912 2023-03-06 22:17:01.818293 folio_migration_tools-1.9.0a2/src/folio_migration_tools/marc_rules_transformation/loc_language_codes.xml
+-rw-r--r--   0        0        0    11373 2024-02-23 19:36:53.902917 folio_migration_tools-1.9.0a2/src/folio_migration_tools/marc_rules_transformation/marc_file_processor.py
+-rw-r--r--   0        0        0     5194 2023-10-18 13:35:39.062695 folio_migration_tools-1.9.0a2/src/folio_migration_tools/marc_rules_transformation/marc_reader_wrapper.py
+-rw-r--r--   0        0        0     9681 2023-11-01 16:09:15.673801 folio_migration_tools-1.9.0a2/src/folio_migration_tools/marc_rules_transformation/rules_mapper_authorities.py
+-rw-r--r--   0        0        0    37640 2023-12-06 07:31:23.300626 folio_migration_tools-1.9.0a2/src/folio_migration_tools/marc_rules_transformation/rules_mapper_base.py
+-rw-r--r--   0        0        0    27439 2024-02-23 19:36:38.880521 folio_migration_tools-1.9.0a2/src/folio_migration_tools/marc_rules_transformation/rules_mapper_bibs.py
+-rw-r--r--   0        0        0    18523 2024-02-23 19:36:53.903728 folio_migration_tools-1.9.0a2/src/folio_migration_tools/marc_rules_transformation/rules_mapper_holdings.py
+-rw-r--r--   0        0        0     4258 2023-10-18 13:35:39.065017 folio_migration_tools-1.9.0a2/src/folio_migration_tools/migration_report.py
+-rw-r--r--   0        0        0      211 2023-03-06 22:17:01.820491 folio_migration_tools-1.9.0a2/src/folio_migration_tools/migration_tasks/__init__.py
+-rw-r--r--   0        0        0     4251 2023-10-18 13:35:39.066574 folio_migration_tools-1.9.0a2/src/folio_migration_tools/migration_tasks/authority_transformer.py
+-rw-r--r--   0        0        0    28127 2024-02-16 21:54:14.449259 folio_migration_tools-1.9.0a2/src/folio_migration_tools/migration_tasks/batch_poster.py
+-rw-r--r--   0        0        0     7380 2023-10-18 13:35:39.067859 folio_migration_tools-1.9.0a2/src/folio_migration_tools/migration_tasks/bibs_transformer.py
+-rw-r--r--   0        0        0     5773 2023-10-18 13:35:39.068533 folio_migration_tools-1.9.0a2/src/folio_migration_tools/migration_tasks/courses_migrator.py
+-rw-r--r--   0        0        0    19628 2024-02-23 19:36:53.904729 folio_migration_tools-1.9.0a2/src/folio_migration_tools/migration_tasks/holdings_csv_transformer.py
+-rw-r--r--   0        0        0     9622 2023-10-18 13:35:39.069665 folio_migration_tools-1.9.0a2/src/folio_migration_tools/migration_tasks/holdings_marc_transformer.py
+-rw-r--r--   0        0        0    15142 2023-10-18 13:35:39.070009 folio_migration_tools-1.9.0a2/src/folio_migration_tools/migration_tasks/items_transformer.py
+-rw-r--r--   0        0        0    34336 2024-02-16 21:54:14.450762 folio_migration_tools-1.9.0a2/src/folio_migration_tools/migration_tasks/loans_migrator.py
+-rw-r--r--   0        0        0     7356 2023-10-18 13:35:39.070917 folio_migration_tools-1.9.0a2/src/folio_migration_tools/migration_tasks/manual_fee_fines_transformer.py
+-rw-r--r--   0        0        0    13875 2024-02-01 21:19:09.540978 folio_migration_tools-1.9.0a2/src/folio_migration_tools/migration_tasks/migration_task_base.py
+-rw-r--r--   0        0        0    11477 2023-10-18 13:35:39.071281 folio_migration_tools-1.9.0a2/src/folio_migration_tools/migration_tasks/orders_transformer.py
+-rw-r--r--   0        0        0    14920 2023-10-18 13:35:39.071521 folio_migration_tools-1.9.0a2/src/folio_migration_tools/migration_tasks/organization_transformer.py
+-rw-r--r--   0        0        0    13309 2023-10-18 13:35:39.071785 folio_migration_tools-1.9.0a2/src/folio_migration_tools/migration_tasks/requests_migrator.py
+-rw-r--r--   0        0        0     9213 2023-11-01 02:13:13.352012 folio_migration_tools-1.9.0a2/src/folio_migration_tools/migration_tasks/reserves_migrator.py
+-rw-r--r--   0        0        0     9936 2024-02-01 21:19:09.541641 folio_migration_tools-1.9.0a2/src/folio_migration_tools/migration_tasks/user_transformer.py
+-rw-r--r--   0        0        0      630 2024-02-01 21:19:09.542364 folio_migration_tools-1.9.0a2/src/folio_migration_tools/task_configuration.py
+-rw-r--r--   0        0        0        0 2023-03-06 22:17:01.830348 folio_migration_tools-1.9.0a2/src/folio_migration_tools/test_infrastructure/__init__.py
+-rw-r--r--   0        0        0     9150 2023-06-08 16:57:16.438864 folio_migration_tools-1.9.0a2/src/folio_migration_tools/test_infrastructure/mocked_classes.py
+-rw-r--r--   0        0        0        0 2023-03-06 22:17:01.831318 folio_migration_tools-1.9.0a2/src/folio_migration_tools/transaction_migration/__init__.py
+-rw-r--r--   0        0        0     5459 2023-12-06 07:31:23.306173 folio_migration_tools-1.9.0a2/src/folio_migration_tools/transaction_migration/legacy_loan.py
+-rw-r--r--   0        0        0     6124 2023-03-06 22:17:01.831928 folio_migration_tools-1.9.0a2/src/folio_migration_tools/transaction_migration/legacy_request.py
+-rw-r--r--   0        0        0     1839 2023-03-06 22:17:01.832344 folio_migration_tools-1.9.0a2/src/folio_migration_tools/transaction_migration/legacy_reserve.py
+-rw-r--r--   0        0        0      656 2023-03-06 22:17:01.832638 folio_migration_tools-1.9.0a2/src/folio_migration_tools/transaction_migration/transaction_result.py
+-rw-r--r--   0        0        0    38525 2024-02-23 19:36:29.957776 folio_migration_tools-1.9.0a2/src/folio_migration_tools/translations/en.json
+-rw-r--r--   0        0        0     7525 1970-01-01 00:00:00.000000 folio_migration_tools-1.9.0a2/setup.py
+-rw-r--r--   0        0        0     7256 1970-01-01 00:00:00.000000 folio_migration_tools-1.9.0a2/PKG-INFO
```

### Comparing `folio_migration_tools-1.9.0a1/LICENSE` & `folio_migration_tools-1.9.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.9.0a1/README.md` & `folio_migration_tools-1.9.0a2/README.md`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.9.0a1/pyproject.toml` & `folio_migration_tools-1.9.0a2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "folio_migration_tools"
-version = "1.9.0a1"
+version = "1.9.0a2"
 description =  "A tool allowing you to migrate data from legacy ILS:s (Library systems) into FOLIO LSP"
 authors = ["Theodor Tolstoy <github.teddes@tolstoy.se>", "Lisa Sjögren", "Brooks Travis", "Jeremy Nelson"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/FOLIO-FSE/folio_migration_tools"
 repository = "https://github.com/FOLIO-FSE/folio_migration_tools"
 keywords = ["FOLIO", "ILS", "LSP", "Library Systems", "MARC21", "Library data"]
```

### Comparing `folio_migration_tools-1.9.0a1/src/folio_migration_tools/__main__.py` & `folio_migration_tools-1.9.0a2/src/folio_migration_tools/__main__.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.9.0a1/src/folio_migration_tools/circulation_helper.py` & `folio_migration_tools-1.9.0a2/src/folio_migration_tools/circulation_helper.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.9.0a1/src/folio_migration_tools/config_file_load.py` & `folio_migration_tools-1.9.0a2/src/folio_migration_tools/config_file_load.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.9.0a1/src/folio_migration_tools/custom_dict.py` & `folio_migration_tools-1.9.0a2/src/folio_migration_tools/custom_dict.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.9.0a1/src/folio_migration_tools/custom_exceptions.py` & `folio_migration_tools-1.9.0a2/src/folio_migration_tools/custom_exceptions.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.9.0a1/src/folio_migration_tools/extradata_writer.py` & `folio_migration_tools-1.9.0a2/src/folio_migration_tools/extradata_writer.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.9.0a1/src/folio_migration_tools/folder_structure.py` & `folio_migration_tools-1.9.0a2/src/folio_migration_tools/folder_structure.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.9.0a1/src/folio_migration_tools/helper.py` & `folio_migration_tools-1.9.0a2/src/folio_migration_tools/helper.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.9.0a1/src/folio_migration_tools/holdings_helper.py` & `folio_migration_tools-1.9.0a2/src/folio_migration_tools/holdings_helper.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.9.0a1/src/folio_migration_tools/library_configuration.py` & `folio_migration_tools-1.9.0a2/src/folio_migration_tools/library_configuration.py`

 * *Files 14% similar despite different names*

```diff
@@ -31,14 +31,25 @@
                 "The location of the file depends on the context"
             ),
         ),
     ] = ""
     discovery_suppressed: Annotated[bool, Field(title="Discovery suppressed")] = False
     staff_suppressed: Annotated[bool, Field(title="Staff suppressed")] = False
     service_point_id: Annotated[str, Field(title="Service point ID")] = ""
+    create_source_records: Annotated[
+        bool,
+        Field(
+            title="Create source records",
+            description=(
+                "If set to true, the source records will be created in FOLIO. "
+                "If set to false, the source records will not be created in FOLIO. "
+                "Only applied for MARC-based transformations."
+            ),
+        ),
+    ] = True
 
 
 class IlsFlavour(str, Enum):
     """ """
 
     aleph = "aleph"
     voyager = "voyager"
@@ -68,17 +79,17 @@
     tenant_id: str
     ecs_tenant_id: Annotated[
         str,
         Field(
             title="ECS tenant ID",
             description=(
                 "For use in ECS environments when the configuration file is meant to target a ",
-                "data tenant. Set to the tenant ID of the data tenant."
-            )
-        )
+                "data tenant. Set to the tenant ID of the data tenant.",
+            ),
+        ),
     ] = ""
     okapi_username: str
     okapi_password: str
     base_folder: DirectoryPath = Field(
         description=(
             "The base folder for migration. "
             "Should ideally be a github clone of the migration_repo_template"
@@ -97,11 +108,10 @@
         description=(
             "The Flavour of the ILS you are migrating from. This choice is "
             "maninly tied to the handling of legacy identifiers and thereby the "
             "deterministic UUIDs generated from them."
         )
     )
     iteration_identifier: str
-    add_time_stamp_to_file_names: Annotated[
-        bool, 
-        Field(title="Add time stamp to file names")
-    ] = False
+    add_time_stamp_to_file_names: Annotated[bool, Field(title="Add time stamp to file names")] = (
+        False
+    )
```

### Comparing `folio_migration_tools-1.9.0a1/src/folio_migration_tools/mapper_base.py` & `folio_migration_tools-1.9.0a2/src/folio_migration_tools/mapper_base.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.9.0a1/src/folio_migration_tools/mapping_file_transformation/courses_mapper.py` & `folio_migration_tools-1.9.0a2/src/folio_migration_tools/mapping_file_transformation/courses_mapper.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.9.0a1/src/folio_migration_tools/mapping_file_transformation/holdings_mapper.py` & `folio_migration_tools-1.9.0a2/src/folio_migration_tools/mapping_file_transformation/holdings_mapper.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.9.0a1/src/folio_migration_tools/mapping_file_transformation/item_mapper.py` & `folio_migration_tools-1.9.0a2/src/folio_migration_tools/mapping_file_transformation/item_mapper.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.9.0a1/src/folio_migration_tools/mapping_file_transformation/manual_fee_fines_mapper.py` & `folio_migration_tools-1.9.0a2/src/folio_migration_tools/mapping_file_transformation/manual_fee_fines_mapper.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.9.0a1/src/folio_migration_tools/mapping_file_transformation/mapping_file_mapper_base.py` & `folio_migration_tools-1.9.0a2/src/folio_migration_tools/mapping_file_transformation/mapping_file_mapper_base.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.9.0a1/src/folio_migration_tools/mapping_file_transformation/notes_mapper.py` & `folio_migration_tools-1.9.0a2/src/folio_migration_tools/mapping_file_transformation/notes_mapper.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.9.0a1/src/folio_migration_tools/mapping_file_transformation/order_mapper.py` & `folio_migration_tools-1.9.0a2/src/folio_migration_tools/mapping_file_transformation/order_mapper.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.9.0a1/src/folio_migration_tools/mapping_file_transformation/organization_mapper.py` & `folio_migration_tools-1.9.0a2/src/folio_migration_tools/mapping_file_transformation/organization_mapper.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.9.0a1/src/folio_migration_tools/mapping_file_transformation/ref_data_mapping.py` & `folio_migration_tools-1.9.0a2/src/folio_migration_tools/mapping_file_transformation/ref_data_mapping.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.9.0a1/src/folio_migration_tools/mapping_file_transformation/user_mapper.py` & `folio_migration_tools-1.9.0a2/src/folio_migration_tools/mapping_file_transformation/user_mapper.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.9.0a1/src/folio_migration_tools/marc_rules_transformation/conditions.py` & `folio_migration_tools-1.9.0a2/src/folio_migration_tools/marc_rules_transformation/conditions.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.9.0a1/src/folio_migration_tools/marc_rules_transformation/holdings_statementsparser.py` & `folio_migration_tools-1.9.0a2/src/folio_migration_tools/marc_rules_transformation/holdings_statementsparser.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.9.0a1/src/folio_migration_tools/marc_rules_transformation/hrid_handler.py` & `folio_migration_tools-1.9.0a2/src/folio_migration_tools/marc_rules_transformation/hrid_handler.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.9.0a1/src/folio_migration_tools/marc_rules_transformation/loc_language_codes.xml` & `folio_migration_tools-1.9.0a2/src/folio_migration_tools/marc_rules_transformation/loc_language_codes.xml`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.9.0a1/src/folio_migration_tools/marc_rules_transformation/marc_file_processor.py` & `folio_migration_tools-1.9.0a2/src/folio_migration_tools/marc_rules_transformation/marc_file_processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,16 @@
     def __init__(
         self, mapper: RulesMapperBase, folder_structure: FolderStructure, created_objects_file
     ):
         self.object_type: FOLIONamespaces = folder_structure.object_type
         self.folder_structure: FolderStructure = folder_structure
         self.mapper: RulesMapperBase = mapper
         self.created_objects_file = created_objects_file
-        self.srs_records_file = open(self.folder_structure.srs_records_path, "w+")
+        if mapper.task_configuration.create_source_records:
+            self.srs_records_file = open(self.folder_structure.srs_records_path, "w+")
         self.unique_001s: set = set()
         self.failed_records_count: int = 0
         self.records_count: int = 0
         self.start: float = time.time()
         self.legacy_ids: set = set()
         if (
             self.object_type == FOLIONamespaces.holdings
@@ -70,21 +71,25 @@
             for idx, folio_rec in enumerate(folio_recs):
                 if idx == 0:
                     filtered_legacy_ids = self.get_valid_folio_record_ids(
                         legacy_ids, self.legacy_ids, self.mapper.migration_report
                     )
                     self.add_legacy_ids_to_map(folio_rec, filtered_legacy_ids)
 
-                    self.save_srs_record(
-                        marc_record,
-                        file_def,
-                        folio_rec,
-                        legacy_ids,
-                        self.object_type,
-                    )
+                    if (
+                        file_def.create_source_records
+                        and self.mapper.task_configuration.create_source_records
+                    ):
+                        self.save_srs_record(
+                            marc_record,
+                            file_def,
+                            folio_rec,
+                            legacy_ids,
+                            self.object_type,
+                        )
                 Helper.write_to_file(self.created_objects_file, folio_rec)
                 self.mapper.migration_report.add_general_statistics(
                     i18n.t("Inventory records written to disk")
                 )
                 self.exit_on_too_many_exceptions()
 
         except TransformationRecordFailedError as error:
@@ -121,15 +126,17 @@
         self,
         marc_record: Record,
         file_def: FileDefinition,
         folio_rec,
         legacy_ids: List[str],
         object_type: FOLIONamespaces,
     ):
-        if not self.mapper.task_configuration.create_source_records:
+        if not all(
+            [file_def.create_source_records, self.mapper.task_configuration.create_source_records]
+        ):
             return
         if object_type in [FOLIONamespaces.holdings]:
             if "008" in marc_record and len(marc_record["008"].data) > 32:
                 remain, rest = (
                     marc_record["008"].data[:32],
                     marc_record["008"].data[32:],
                 )
@@ -235,15 +242,16 @@
             )
             Helper.print_mapping_report(
                 report_file,
                 self.mapper.parsed_records,
                 self.mapper.mapped_folio_fields,
                 self.mapper.mapped_legacy_fields,
             )
-        self.srs_records_file.close()
+        if self.mapper.task_configuration.create_source_records:
+            self.srs_records_file.close()
         self.mapper.wrap_up()
 
         logging.info("Transformation report written to %s", report_file.name)
         logging.info("Processor is done.")
 
     def add_legacy_ids_to_map(self, folio_rec, filtered_legacy_ids):
         for legacy_id in filtered_legacy_ids:
```

### Comparing `folio_migration_tools-1.9.0a1/src/folio_migration_tools/marc_rules_transformation/marc_reader_wrapper.py` & `folio_migration_tools-1.9.0a2/src/folio_migration_tools/marc_rules_transformation/marc_reader_wrapper.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.9.0a1/src/folio_migration_tools/marc_rules_transformation/rules_mapper_authorities.py` & `folio_migration_tools-1.9.0a2/src/folio_migration_tools/marc_rules_transformation/rules_mapper_authorities.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.9.0a1/src/folio_migration_tools/marc_rules_transformation/rules_mapper_base.py` & `folio_migration_tools-1.9.0a2/src/folio_migration_tools/marc_rules_transformation/rules_mapper_base.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.9.0a1/src/folio_migration_tools/marc_rules_transformation/rules_mapper_bibs.py` & `folio_migration_tools-1.9.0a2/src/folio_migration_tools/marc_rules_transformation/rules_mapper_bibs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """The default mapper, responsible for parsing MARC21 records acording to the
 FOLIO community specifications"""
+
 import logging
 import sys
 import time
 import typing
 import uuid
 from pathlib import Path
 from typing import Generator
@@ -139,15 +140,18 @@
 
         Args:
             folio_instance (dict): _description_
             marc_record (Record): _description_
             legacy_ids (List[str]): _description_
             file_def (FileDefinition): _description_
         """
-        folio_instance["source"] = "MARC"
+        if file_def.create_source_records and self.task_configuration.create_source_records:
+            folio_instance["source"] = "MARC"
+        else:
+            folio_instance["source"] = "FOLIO"
         folio_instance["instanceFormatIds"] = list(
             set(self.get_instance_format_ids(marc_record, legacy_ids))
         )
         folio_instance["instanceTypeId"] = self.get_instance_type_id(marc_record, legacy_ids)
 
         folio_instance["modeOfIssuanceId"] = self.get_mode_of_issuance_id(marc_record, legacy_ids)
         self.handle_languages(folio_instance, marc_record, legacy_ids)
```

### Comparing `folio_migration_tools-1.9.0a1/src/folio_migration_tools/marc_rules_transformation/rules_mapper_holdings.py` & `folio_migration_tools-1.9.0a2/src/folio_migration_tools/marc_rules_transformation/rules_mapper_holdings.py`

 * *Files 2% similar despite different names*

```diff
@@ -248,46 +248,49 @@
             TransformationRecordFailedError: _description_
         """
         self.set_holdings_type(marc_record, folio_holding, legacy_ids)
         self.set_default_call_number_type_if_empty(folio_holding)
         self.pick_first_location_if_many(folio_holding, legacy_ids)
         self.parse_coded_holdings_statements(marc_record, folio_holding, legacy_ids)
         HoldingsHelper.handle_notes(folio_holding)
+        create_source_records = all(
+            [file_def.create_source_records, self.task_configuration.create_source_records]
+        )
         if (
-            self.task_configuration.create_source_records
+            create_source_records
             or self.task_configuration.hrid_handling == HridHandling.preserve001
         ):
             self.hrid_handler.handle_hrid(
                 FOLIONamespaces.holdings, folio_holding, marc_record, legacy_ids
             )
         else:
             del folio_holding["hrid"]
         if not folio_holding.get("instanceId", ""):
             raise TransformationRecordFailedError(
                 "".join(folio_holding.get("formerIds", [])),
                 "Missing instance ids. Something is wrong.",
                 "",
             )
         self.handle_suppression(folio_holding, file_def, True)
-        self.set_source_id(self.task_configuration, folio_holding, self.holdingssources)
+        self.set_source_id(self.task_configuration, folio_holding, self.holdingssources, file_def)
 
     def pick_first_location_if_many(self, folio_holding, legacy_ids: List[str]):
         if " " in folio_holding.get("permanentLocationId", ""):
             Helper.log_data_issue(
                 legacy_ids,
                 "Space in permanentLocationId. Was this MFHD attached to multiple holdings?",
                 folio_holding["permanentLocationId"],
             )
             folio_holding["permanentLocationId"] = folio_holding["permanentLocationId"].split(" ")[
                 0
             ]
 
     @staticmethod
-    def set_source_id(task_configuration, folio_rec, holdingssources):
-        if task_configuration.create_source_records:
+    def set_source_id(task_configuration, folio_rec, holdingssources, file_def):
+        if file_def.create_source_records and task_configuration.create_source_records:
             folio_rec["sourceId"] = holdingssources.get("MARC")
         else:
             folio_rec["sourceId"] = holdingssources.get("FOLIO")
 
     def parse_coded_holdings_statements(
         self, marc_record: Record, folio_holding, legacy_ids: List[str]
     ):
@@ -313,16 +316,28 @@
                     self.migration_report.add("HoldingsStatementsParsing", f"{mr[0]} -- {mr[1]}")
             except TransformationFieldMappingError as tfme:
                 Helper.log_data_issue(tfme.index_or_id, tfme.message, tfme.data_value)
                 self.migration_report.add("FieldMappingErrors", tfme.message)
 
     def wrap_up(self):
         logging.info("Mapper wrapping up")
+        source_file_create_source_records = [
+            x["create_source_records"] for x in self.task_configuration.files
+        ]
+        if all(source_file_create_source_records):
+            create_source_records = self.task_configuration.create_source_records
+        else:
+            logging.info(
+                "If all source files have create_source_records set to false, "
+                "this will override the task configuration setting"
+            )
+            create_source_records = any(source_file_create_source_records)
         if self.task_configuration.update_hrid_settings:
-            if self.task_configuration.create_source_records:
+            if create_source_records:
+                logging.info("Storing HRID settings")
                 self.hrid_handler.store_hrid_settings()
             else:
                 logging.info("NOT storing HRID settings since that is managed by FOLIO")
 
     def fetch_holdings_schema(self, folio_client: FolioClient):
         logging.info("Fetching HoldingsRecord schema...")
         return folio_client.get_from_github(
```

### Comparing `folio_migration_tools-1.9.0a1/src/folio_migration_tools/migration_report.py` & `folio_migration_tools-1.9.0a2/src/folio_migration_tools/migration_report.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.9.0a1/src/folio_migration_tools/migration_tasks/authority_transformer.py` & `folio_migration_tools-1.9.0a2/src/folio_migration_tools/migration_tasks/authority_transformer.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.9.0a1/src/folio_migration_tools/migration_tasks/batch_poster.py` & `folio_migration_tools-1.9.0a2/src/folio_migration_tools/migration_tasks/batch_poster.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import copy
 import json
 import logging
 import sys
 import time
 import traceback
-import i18n
 from datetime import datetime
 from typing import Annotated
 from typing import List
 from uuid import uuid4
 
 import httpx
+import i18n
 from folio_uuid.folio_namespaces import FOLIONamespaces
 from pydantic import Field
 
 from folio_migration_tools.custom_exceptions import TransformationProcessError
 from folio_migration_tools.custom_exceptions import TransformationRecordFailedError
 from folio_migration_tools.library_configuration import FileDefinition
 from folio_migration_tools.library_configuration import LibraryConfiguration
@@ -103,15 +103,15 @@
         self.failed_fields: set = set()
         self.num_failures = 0
         self.num_posted = 0
         self.okapi_headers = self.folio_client.okapi_headers
         self.http_client = None
 
     def do_work(self):
-        with httpx.Client(timeout=None, headers=self.folio_client.okapi_headers) as httpx_client:
+        with httpx.Client(timeout=None) as httpx_client:
             self.http_client = httpx_client
             try:
                 batch = []
                 if self.task_configuration.object_type == "SRS":
                     self.create_snapshot()
                 with open(self.folder_structure.failed_recs_path, "w") as failed_recs_file:
                     for file_def in self.task_configuration.files:
@@ -239,15 +239,17 @@
                 "%s records posted successfully. %s failed",
                 self.num_posted,
                 self.num_failures,
             )
 
     def post_objects(self, url, body):
         if self.http_client and not self.http_client.is_closed:
-            return self.http_client.post(url, data=body.encode("utf-8"))
+            return self.http_client.post(
+                url, data=body.encode("utf-8"), headers=self.folio_client.okapi_headers
+            )
         else:
             return httpx.post(
                 url, headers=self.okapi_headers, data=body.encode("utf-8"), timeout=None
             )
 
     def handle_generic_exception(self, exception, last_row, batch, num_records, failed_recs_file):
         logging.error("%s", exception)
@@ -391,15 +393,17 @@
         if self.api_info["object_name"] == "users":
             payload = {self.api_info["object_name"]: list(batch), "totalRecords": len(batch)}
         elif self.api_info["total_records"]:
             payload = {"records": list(batch), "totalRecords": len(batch)}
         else:
             payload = {self.api_info["object_name"]: batch}
         if self.http_client and not self.http_client.is_closed:
-            return self.http_client.post(url, json=payload)
+            return self.http_client.post(
+                url, json=payload, headers=self.folio_client.okapi_headers
+            )
         else:
             return httpx.post(url, headers=self.okapi_headers, json=payload, timeout=None)
 
     def wrap_up(self):
         logging.info("Done. Wrapping up")
         self.extradata_writer.flush()
         if self.task_configuration.object_type == "SRS":
@@ -468,26 +472,28 @@
             "jobExecutionId": self.snapshot_id,
             "status": "PARSING_IN_PROGRESS",
             "processingStartedDate": datetime.utcnow().isoformat(timespec="milliseconds"),
         }
         try:
             url = f"{self.folio_client.okapi_url}/source-storage/snapshots"
             if self.http_client and not self.http_client.is_closed:
-                res = self.http_client.post(url, json=snapshot)
+                res = self.http_client.post(
+                    url, json=snapshot, headers=self.folio_client.okapi_headers
+                )
             else:
                 res = httpx.post(url, headers=self.okapi_headers, json=snapshot, timeout=None)
             res.raise_for_status()
             logging.info("Posted Snapshot to FOLIO: %s", json.dumps(snapshot, indent=4))
             get_url = f"{self.folio_client.okapi_url}/source-storage/snapshots/{self.snapshot_id}"
             getted = False
             while not getted:
                 logging.info("Sleeping while waiting for the snapshot to get created")
                 time.sleep(5)
                 if self.http_client and not self.http_client.is_closed:
-                    res = self.http_client.get(get_url)
+                    res = self.http_client.get(get_url, headers=self.folio_client.okapi_headers)
                 else:
                     res = httpx.get(get_url, headers=self.okapi_headers, timeout=None)
                 if res.status_code == 200:
                     getted = True
                 else:
                     logging.info(res.status_code)
         except Exception:
@@ -495,15 +501,17 @@
             sys.exit(1)
 
     def commit_snapshot(self):
         snapshot = {"jobExecutionId": self.snapshot_id, "status": "COMMITTED"}
         try:
             url = f"{self.folio_client.okapi_url}/source-storage/snapshots/{self.snapshot_id}"
             if self.http_client and not self.http_client.is_closed:
-                res = self.http_client.put(url, json=snapshot)
+                res = self.http_client.put(
+                    url, json=snapshot, headers=self.folio_client.okapi_headers
+                )
             else:
                 res = httpx.put(url, headers=self.okapi_headers, json=snapshot, timeout=None)
             res.raise_for_status()
             logging.info("Posted Committed snapshot to FOLIO: %s", json.dumps(snapshot, indent=4))
         except Exception:
             logging.exception(
                 "Could not commit snapshot with id %s. Post this to /source-storage/snapshots/%s:",
```

### Comparing `folio_migration_tools-1.9.0a1/src/folio_migration_tools/migration_tasks/bibs_transformer.py` & `folio_migration_tools-1.9.0a2/src/folio_migration_tools/migration_tasks/bibs_transformer.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.9.0a1/src/folio_migration_tools/migration_tasks/courses_migrator.py` & `folio_migration_tools-1.9.0a2/src/folio_migration_tools/migration_tasks/courses_migrator.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.9.0a1/src/folio_migration_tools/migration_tasks/holdings_csv_transformer.py` & `folio_migration_tools-1.9.0a2/src/folio_migration_tools/migration_tasks/holdings_csv_transformer.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.9.0a1/src/folio_migration_tools/migration_tasks/holdings_marc_transformer.py` & `folio_migration_tools-1.9.0a2/src/folio_migration_tools/migration_tasks/holdings_marc_transformer.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.9.0a1/src/folio_migration_tools/migration_tasks/items_transformer.py` & `folio_migration_tools-1.9.0a2/src/folio_migration_tools/migration_tasks/items_transformer.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.9.0a1/src/folio_migration_tools/migration_tasks/loans_migrator.py` & `folio_migration_tools-1.9.0a2/src/folio_migration_tools/migration_tasks/loans_migrator.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,17 +164,15 @@
             for i in range(10, 0, -1):
                 sys.stdout.write("Pausing for {:02d} seconds. Press Ctrl+C to exit...\r".format(i))
                 time.sleep(1)
         else:
             logging.info("SMTP connection is disabled...")
 
     def do_work(self):
-        with httpx.Client(
-            timeout=None, headers=self.folio_client.okapi_headers
-        ) as self.http_client:
+        with httpx.Client(timeout=None) as self.http_client:
             logging.info("Starting")
             starting_index = (
                 self.task_configuration.starting_row - 1
                 if self.task_configuration.starting_row > 0
                 else 0
             )
             if self.task_configuration.starting_row > 1:
```

### Comparing `folio_migration_tools-1.9.0a1/src/folio_migration_tools/migration_tasks/manual_fee_fines_transformer.py` & `folio_migration_tools-1.9.0a2/src/folio_migration_tools/migration_tasks/manual_fee_fines_transformer.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.9.0a1/src/folio_migration_tools/migration_tasks/migration_task_base.py` & `folio_migration_tools-1.9.0a2/src/folio_migration_tools/migration_tasks/migration_task_base.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.9.0a1/src/folio_migration_tools/migration_tasks/orders_transformer.py` & `folio_migration_tools-1.9.0a2/src/folio_migration_tools/migration_tasks/orders_transformer.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.9.0a1/src/folio_migration_tools/migration_tasks/organization_transformer.py` & `folio_migration_tools-1.9.0a2/src/folio_migration_tools/migration_tasks/organization_transformer.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.9.0a1/src/folio_migration_tools/migration_tasks/requests_migrator.py` & `folio_migration_tools-1.9.0a2/src/folio_migration_tools/migration_tasks/requests_migrator.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.9.0a1/src/folio_migration_tools/migration_tasks/reserves_migrator.py` & `folio_migration_tools-1.9.0a2/src/folio_migration_tools/migration_tasks/reserves_migrator.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.9.0a1/src/folio_migration_tools/migration_tasks/user_transformer.py` & `folio_migration_tools-1.9.0a2/src/folio_migration_tools/migration_tasks/user_transformer.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.9.0a1/src/folio_migration_tools/task_configuration.py` & `folio_migration_tools-1.9.0a2/src/folio_migration_tools/task_configuration.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.9.0a1/src/folio_migration_tools/test_infrastructure/mocked_classes.py` & `folio_migration_tools-1.9.0a2/src/folio_migration_tools/test_infrastructure/mocked_classes.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.9.0a1/src/folio_migration_tools/transaction_migration/legacy_loan.py` & `folio_migration_tools-1.9.0a2/src/folio_migration_tools/transaction_migration/legacy_loan.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.9.0a1/src/folio_migration_tools/transaction_migration/legacy_request.py` & `folio_migration_tools-1.9.0a2/src/folio_migration_tools/transaction_migration/legacy_request.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.9.0a1/src/folio_migration_tools/transaction_migration/legacy_reserve.py` & `folio_migration_tools-1.9.0a2/src/folio_migration_tools/transaction_migration/legacy_reserve.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.9.0a1/src/folio_migration_tools/transaction_migration/transaction_result.py` & `folio_migration_tools-1.9.0a2/src/folio_migration_tools/transaction_migration/transaction_result.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.9.0a1/src/folio_migration_tools/translations/en.json` & `folio_migration_tools-1.9.0a2/src/folio_migration_tools/translations/en.json`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.9.0a1/setup.py` & `folio_migration_tools-1.9.0a2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
  'pyhumps>=3.7.3,<4.0.0',
  'pymarc>=5.0.0,<6.0.0',
  'python-dateutil>=2.8.2,<3.0.0',
  'python-i18n>=0.3.9,<0.4.0']
 
 setup_kwargs = {
     'name': 'folio-migration-tools',
-    'version': '1.9.0a1',
+    'version': '1.9.0a2',
     'description': 'A tool allowing you to migrate data from legacy ILS:s (Library systems) into FOLIO LSP',
     'long_description': '# FOLIO Migration Tools\n![example workflow](https://github.com/FOLIO-FSE/MARC21-To-FOLIO/actions/workflows/python-app.yml/badge.svg)[![codecov](https://codecov.io/gh/FOLIO-FSE/folio_migration_tools/branch/main/graph/badge.svg?token=ZQL5ILWWGT)](https://codecov.io/gh/FOLIO-FSE/folio_migration_tools)   [![readthedocs](https://readthedocs.org/projects/docs/badge/?version=latest)](https://folio-migration-tools.readthedocs.io/)\n\nA toolkit that enables you to migrate data over from a legacy ILS system into [FOLIO LSP](https://www.folio.org/)\n\n# What is it good for?\nFOLIO Migration tools enables you to migrate libraries with the most common ILS:s over to FOLIO without data losses or any major data transformation tasks. \nThe tools transforms and loads the data providing you and the library with good actionable logs and data cleaning task lists together with the migrated data.\n\n## What data does it cover?\nFOLIO Migration Tools currently covers the following data sets:\n* Catalog (Inventory and SRS in FOLIO terminology)\n* Circulation transactions (Open loans and requests)\n* Users/Patrons (In FOLIO, these share the same app/database)\n* Courses and Reserves (Course reserves)\n* Organizations (Vendor records)\n* Orders (limited support)\n\n### What additional functionality is on the roadmap?\nThis is the loose roadmap, in order of most likely implementations first\n* ERM-related objects\n* Financial records\n\n### Can I use the tools for ongoing imports and integrations?\nThe tools are primarliy maintained for performing initial data migrations. We recommend that you use native FOLIO functionality for ongoing loads where possible. \nIn theory, these tools can be used for ongoing patron loads from systems like Banner, Workday, or PeopleSoft. But we recommend you to weigh your options carefully before going down this path. \n\n# Contributing\nWant to contribute? Read the [CONTRIBUTING.MD](https://github.com/FOLIO-FSE/folio_migration_tools/blob/main/CONTRIBUTING.md)\n\n# Found an issue?\nReport it on the [Github Issue tracker](https://github.com/FOLIO-FSE/folio_migration_tools/issues)\n\nThe scripts requires a FOLIO tenant with reference data properly set up. The script will throw messages telling what reference data is missing.\n# Installing\nMake sure you are running Python 3.9 or above. \n## 1. Using pip and venv\n### 2.1. Create and activate a [virtual environment](https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/#creating-a-virtual-environment)   \n```   \npython -m venv ./.venv     # Creates a virtual env in the current folder\nsource .venv/bin/activate  # Activates the venv    \n```\n### 2. Install using pip: \n```\npython -m pip install folio_migration_tools\n```\n### 3. Test the installation by showing the help pages \n```   \npython -m folio_migration_tools -h\n```    \n\n## 2. Using pipenv\n### 1. Run\n```   \npipenv install folio-migration-tools\n```   \n### 2. Test the installation by showing the help pages\n```  \npipenv run python3 -m folio_migration_tools -h\n```\n\n# FOLIO migration process\nThis repo plays the main part in a process using a collection of tools. The process itself is documented in more detail, including example configuration files, at [this template repository](https://github.com/FOLIO-FSE/migration_repo_template)\nIn order to perform migrations according to this process, you need the following:\n* An Installation of [FOLIO Migration Tools](https://pypi.org/project/folio-migration-tools/). Installation instructions above.\n* A clone, or a separate repo created from [migration_repo_template](https://github.com/FOLIO-FSE/migration_repo_template)\n* Access to the [Data mapping file creator](https://data-mapping-file-creator.folio.ebsco.com/data_mapping_creation) web tool\n* A FOLIO tenant running the latest or the second latest version of FOLIO\n\n# Internationalization\n\nThis repo uses [Python-i18n](https://github.com/danhper/python-i18n) to translate reports between languages, and to handle large strings for templates.\n\n**Any English string which will end up in a report** should be wrapped in the function `i18n.t` from `i18n`:\n\n## Keys/Usage\n\n```js\ni18n.t("Reports")+":"\n```\n\nTemplating is achieved with `%{[key]}` blocks, and keyword arguments in the internationaliation:\n\n```js\ni18n.t("Code \'%{code}\' not found in FOLIO",code=folio_code)\n```\n\nLong strings can use a placeholder key:\n\n```js\ni18n.t("blurbs.Introduction.description")\n```\n\nWith the full string in ```translations/en.json```:\n\n```json\n"blurbs.Introduction.description": "<br/>Data errors preventing records from being migrated\n```\n\n## Translations Files\n\nTranslation files live in the `translations` directory, with `en.json` as the default.\n\nExtract template files with the `extract_translations` script:\n\n```bash\npython scripts/extract_translations.py\n```\n\n## Internationalizations\n\nOther langauges translations live in `translations/[locale].json`.\nFor example, Spanish would be `es.json`. \n\nThe keys must match the English keys, but the Values should be translated.\n\nYou can update a language file\'s keys with:\n\n```bash\npython scripts/update_language.py --target-lang [locale]\n```\n\nTranslate all new strings, which begin with `TRANSLATE`, then commit.\n\n## Tips\n\n* Internationalize entire phrases or paragraphs, not just the constitutent words. Syntax and grammar vary significantly between languages.\n* Name template variables as generically as possible in the circumstance, and check translations for reusable translations.\n* In a block with sentences separately followed by values, such as a table, you only need to translate the sentences. \n\n# Running the scripts\nFor information on syntax, what files are needed and produced by the toolkit, refer to the documentation and example files in the [template repository](https://github.com/FOLIO-FSE/migration_repo_template). We are building out the docs section in this repository as well:[Documentation](https://folio-migration-tools.readthedocs.io/en/latest/)\n¨\n',
     'author': 'Theodor Tolstoy',
     'author_email': 'github.teddes@tolstoy.se',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/FOLIO-FSE/folio_migration_tools',
```

### Comparing `folio_migration_tools-1.9.0a1/PKG-INFO` & `folio_migration_tools-1.9.0a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: folio-migration-tools
-Version: 1.9.0a1
+Version: 1.9.0a2
 Summary: A tool allowing you to migrate data from legacy ILS:s (Library systems) into FOLIO LSP
 Home-page: https://github.com/FOLIO-FSE/folio_migration_tools
 License: MIT
 Keywords: FOLIO,ILS,LSP,Library Systems,MARC21,Library data
 Author: Theodor Tolstoy
 Author-email: github.teddes@tolstoy.se
 Requires-Python: >=3.9,<4.0
```

