# Comparing `tmp/test_esmf_loader-0.0.1.tar.gz` & `tmp/test_esmf_loader-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_esmf_loader-0.0.1.tar", max compression
+gzip compressed data, was "test_esmf_loader-0.0.2.tar", max compression
```

## Comparing `test_esmf_loader-0.0.1.tar` & `test_esmf_loader-0.0.2.tar`

### file list

```diff
@@ -1,190 +1,191 @@
--rw-r--r--   0        0        0     2021 2024-02-14 14:39:42.096721 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/__init__.py
--rw-r--r--   0        0        0     2289 2023-10-31 10:36:17.197378 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/__init__.py
--rw-r--r--   0        0        0     1277 2023-10-31 10:10:40.580805 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/aspect.py
--rw-r--r--   0        0        0     1116 2023-10-31 10:10:40.580805 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/base.py
--rw-r--r--   0        0        0      848 2023-10-31 10:10:40.580805 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/bound_definition.py
--rw-r--r--   0        0        0     2050 2023-10-31 10:10:40.581816 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/cache_strategy.py
--rw-r--r--   0        0        0      426 2023-10-31 10:03:14.801371 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/characteristics/__init__.py
--rw-r--r--   0        0        0      989 2023-10-31 10:10:40.581816 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/characteristics/characteristic.py
--rw-r--r--   0        0        0      683 2023-10-31 10:10:40.581816 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/characteristics/code.py
--rw-r--r--   0        0        0      426 2023-10-31 10:03:14.802370 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/characteristics/collection/__init__.py
--rw-r--r--   0        0        0     1062 2023-10-31 10:10:40.582815 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/characteristics/collection/collection.py
--rw-r--r--   0        0        0      685 2023-10-31 10:10:40.582815 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/characteristics/collection/list.py
--rw-r--r--   0        0        0      685 2023-10-31 10:10:40.582815 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/characteristics/collection/set.py
--rw-r--r--   0        0        0      696 2023-10-31 10:10:40.582815 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/characteristics/collection/sorted_set.py
--rw-r--r--   0        0        0      692 2023-10-31 10:10:40.583815 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/characteristics/collection/time_series.py
--rw-r--r--   0        0        0      847 2023-10-31 10:10:40.583815 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/characteristics/enumeration.py
--rw-r--r--   0        0        0      426 2023-10-31 10:03:14.803370 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/characteristics/quantifiable/__init__.py
--rw-r--r--   0        0        0      689 2023-10-31 10:10:40.584816 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/characteristics/quantifiable/duration.py
--rw-r--r--   0        0        0      691 2023-10-31 10:10:40.584816 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/characteristics/quantifiable/measurement.py
--rw-r--r--   0        0        0      943 2023-10-31 10:10:40.584816 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/characteristics/quantifiable/quantifiable.py
--rw-r--r--   0        0        0      697 2023-10-31 10:10:40.584816 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/characteristics/single_entity.py
--rw-r--r--   0        0        0      779 2023-10-31 10:10:40.585816 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/characteristics/state.py
--rw-r--r--   0        0        0     1070 2023-10-31 10:10:40.585816 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/characteristics/structured_value.py
--rw-r--r--   0        0        0     1177 2023-10-31 10:10:40.585816 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/characteristics/trait.py
--rw-r--r--   0        0        0      426 2023-10-31 10:03:14.804371 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/contraints/__init__.py
--rw-r--r--   0        0        0      747 2023-10-31 10:10:40.585816 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/contraints/constraint.py
--rw-r--r--   0        0        0      816 2023-10-31 10:10:40.586815 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/contraints/encoding_constraint.py
--rw-r--r--   0        0        0     1049 2023-10-31 10:10:40.586815 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/contraints/fixed_point_constraint.py
--rw-r--r--   0        0        0      859 2023-10-31 10:10:40.586815 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/contraints/language_constraint.py
--rw-r--r--   0        0        0     1101 2023-10-31 10:10:40.587815 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/contraints/length_constraint.py
--rw-r--r--   0        0        0      861 2023-10-31 10:10:40.587815 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/contraints/locale_constraint.py
--rw-r--r--   0        0        0     1519 2023-10-31 10:10:40.587815 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/contraints/range_constraint.py
--rw-r--r--   0        0        0      872 2023-10-31 10:10:40.588820 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/contraints/regular_expression_constraint.py
--rw-r--r--   0        0        0      426 2023-10-31 10:03:14.806371 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/data_types/__init__.py
--rw-r--r--   0        0        0      915 2023-10-31 10:10:40.588820 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/data_types/abstract_entity.py
--rw-r--r--   0        0        0     1284 2023-10-31 10:10:40.588820 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/data_types/complex_type.py
--rw-r--r--   0        0        0      990 2023-10-31 10:10:40.588820 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/data_types/data_type.py
--rw-r--r--   0        0        0      760 2023-10-31 10:10:40.589816 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/data_types/entity.py
--rw-r--r--   0        0        0      876 2024-01-29 09:31:02.594330 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/data_types/scalar.py
--rw-r--r--   0        0        0      961 2023-10-31 10:36:17.197378 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/either.py
--rw-r--r--   0        0        0      992 2023-10-31 10:10:40.589816 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/event.py
--rw-r--r--   0        0        0      858 2023-10-31 10:10:40.589816 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/has_properties.py
--rw-r--r--   0        0        0      902 2023-10-31 10:10:40.590814 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/has_urn.py
--rw-r--r--   0        0        0     1549 2023-10-31 10:10:40.590814 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/is_described.py
--rw-r--r--   0        0        0     1104 2023-10-31 10:10:40.590814 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/operation.py
--rw-r--r--   0        0        0     2648 2023-10-31 10:10:40.590814 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/property.py
--rw-r--r--   0        0        0     1811 2023-10-31 10:10:40.590814 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/property_func.py
--rw-r--r--   0        0        0      700 2023-10-31 10:10:40.591817 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/quantity_kind.py
--rw-r--r--   0        0        0     2110 2024-02-19 13:57:01.319640 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/README.md
--rw-r--r--   0        0        0      687 2023-10-31 10:10:40.591817 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/structure_element.py
--rw-r--r--   0        0        0     1414 2023-10-31 10:10:40.591817 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/unit.py
--rw-r--r--   0        0        0     2784 2024-02-19 13:57:01.320643 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/__init__.py
--rw-r--r--   0        0        0     2517 2023-10-31 10:10:40.591817 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/base_impl.py
--rw-r--r--   0        0        0      426 2023-10-31 10:03:14.809370 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/characteristics/__init__.py
--rw-r--r--   0        0        0      426 2023-10-31 10:03:14.809370 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/characteristics/collection/__init__.py
--rw-r--r--   0        0        0     1826 2023-10-31 10:10:40.592815 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/characteristics/collection/default_collection.py
--rw-r--r--   0        0        0      705 2023-10-31 10:10:40.592815 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/characteristics/collection/default_list.py
--rw-r--r--   0        0        0      700 2023-10-31 10:10:40.592815 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/characteristics/collection/default_set.py
--rw-r--r--   0        0        0      732 2023-10-31 10:10:40.592815 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/characteristics/collection/default_sorted_set.py
--rw-r--r--   0        0        0      735 2023-10-31 10:10:40.592815 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/characteristics/collection/default_time_series.py
--rw-r--r--   0        0        0     1371 2023-10-31 10:10:40.593815 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/characteristics/default_characteristic.py
--rw-r--r--   0        0        0      695 2023-10-31 10:10:40.593815 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/characteristics/default_code.py
--rw-r--r--   0        0        0     1291 2023-10-31 10:10:40.593815 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/characteristics/default_enumeration.py
--rw-r--r--   0        0        0      737 2023-10-31 10:10:40.593815 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/characteristics/default_single_entity.py
--rw-r--r--   0        0        0     1321 2023-10-31 10:10:40.594815 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/characteristics/default_state.py
--rw-r--r--   0        0        0     1554 2023-10-31 10:10:40.595049 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/characteristics/default_structured_value.py
--rw-r--r--   0        0        0     1984 2023-10-31 10:10:40.595552 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/characteristics/default_trait.py
--rw-r--r--   0        0        0      426 2023-10-31 10:03:14.811370 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/characteristics/quantifiable/__init__.py
--rw-r--r--   0        0        0      735 2023-10-31 10:10:40.595552 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/characteristics/quantifiable/default_duration.py
--rw-r--r--   0        0        0      750 2023-10-31 10:10:40.595552 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/characteristics/quantifiable/default_measurement.py
--rw-r--r--   0        0        0     1465 2023-10-31 10:10:40.595552 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/characteristics/quantifiable/default_quantifiable.py
--rw-r--r--   0        0        0      426 2023-10-31 10:03:14.812370 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/constraints/__init__.py
--rw-r--r--   0        0        0      702 2023-10-31 10:10:40.595552 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/constraints/default_constraint.py
--rw-r--r--   0        0        0     1118 2023-10-31 10:10:40.596568 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/constraints/default_encoding_constraint.py
--rw-r--r--   0        0        0     1323 2023-10-31 10:10:40.596568 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/constraints/default_fixed_point_constraint.py
--rw-r--r--   0        0        0     1166 2023-10-31 10:10:40.596568 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/constraints/default_language_constraint.py
--rw-r--r--   0        0        0     1408 2023-10-31 10:10:40.596568 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/constraints/default_length_constraint.py
--rw-r--r--   0        0        0     1144 2023-10-31 10:10:40.597568 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/constraints/default_locale_constraint.py
--rw-r--r--   0        0        0     2073 2023-10-31 10:10:40.597568 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/constraints/default_range_constraint.py
--rw-r--r--   0        0        0     1159 2023-10-31 10:10:40.597568 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/constraints/default_regular_expression_constraint.py
--rw-r--r--   0        0        0      426 2023-10-31 10:03:14.814371 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/data_types/__init__.py
--rw-r--r--   0        0        0     1597 2023-10-31 10:10:40.597568 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/data_types/default_abstract_entity.py
--rw-r--r--   0        0        0     3612 2023-10-31 10:10:40.597568 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/data_types/default_complex_type.py
--rw-r--r--   0        0        0      946 2024-02-19 13:57:01.320643 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/data_types/default_data_type.py
--rw-r--r--   0        0        0      687 2023-10-31 10:10:40.598567 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/data_types/default_entity.py
--rw-r--r--   0        0        0      935 2024-02-14 13:17:05.158388 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/data_types/default_scalar.py
--rw-r--r--   0        0        0     2389 2023-10-31 10:10:40.598567 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/default_aspect.py
--rw-r--r--   0        0        0     1408 2023-10-31 10:36:17.197378 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/default_either.py
--rw-r--r--   0        0        0     1167 2023-10-31 10:10:40.598567 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/default_event.py
--rw-r--r--   0        0        0     1876 2023-10-31 10:10:40.598567 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/default_operation.py
--rw-r--r--   0        0        0     3961 2023-10-31 10:10:40.599568 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/default_property.py
--rw-r--r--   0        0        0      666 2023-10-31 10:10:40.599568 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/default_quantity_kind.py
--rw-r--r--   0        0        0     2293 2023-10-31 10:10:40.599568 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/default_unit.py
--rw-r--r--   0        0        0     3974 2023-10-31 10:03:14.751826 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/README.md
--rw-r--r--   0        0        0      426 2023-10-31 10:03:14.816371 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/__init__.py
--rw-r--r--   0        0        0    11378 2024-02-19 13:57:01.321640 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/aspect_loader.py
--rw-r--r--   0        0        0     2253 2023-10-31 10:03:15.165891 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/default_element_cache.py
--rw-r--r--   0        0        0      426 2023-10-31 10:03:14.817371 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/__init__.py
--rw-r--r--   0        0        0     1813 2023-10-31 10:03:15.165891 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/abstract_entity_instantiator.py
--rw-r--r--   0        0        0     4143 2023-10-31 10:10:40.537605 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/abstract_property_instantiator.py
--rw-r--r--   0        0        0     1968 2023-10-31 10:03:15.166897 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/aspect_instantiator.py
--rw-r--r--   0        0        0     1194 2023-10-31 10:03:15.167898 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/characteristic_instantiator.py
--rw-r--r--   0        0        0     1114 2023-10-31 10:03:14.818370 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/code_instantiator.py
--rw-r--r--   0        0        0     1389 2023-10-31 10:03:15.167898 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/collection_instantiator.py
--rw-r--r--   0        0        0     2924 2023-10-31 10:10:40.538374 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/complex_type_instantiator.py
--rw-r--r--   0        0        0     1102 2024-02-19 13:57:01.321640 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/datatype_instantiator.py
--rw-r--r--   0        0        0     1323 2023-10-31 10:03:15.168897 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/duration_instantiator.py
--rw-r--r--   0        0        0     1181 2023-10-31 10:36:17.197378 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/either_instantiator.py
--rw-r--r--   0        0        0     1392 2023-10-31 10:10:40.538374 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/encoding_constraint_instantiator.py
--rw-r--r--   0        0        0     1873 2023-10-31 10:03:15.169897 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/entity_instantiator.py
--rw-r--r--   0        0        0     4726 2023-10-31 10:10:40.538374 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/enumeration_instantiator.py
--rw-r--r--   0        0        0     1200 2023-10-31 10:03:15.169897 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/event_instantiator.py
--rw-r--r--   0        0        0     1554 2023-10-31 10:10:40.539419 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/fixed_point_constraint_instantiator.py
--rw-r--r--   0        0        0     1383 2023-10-31 10:10:40.539419 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/language_constraint_instantiator.py
--rw-r--r--   0        0        0     1538 2023-10-31 10:10:40.539419 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/length_constraint_instantiator.py
--rw-r--r--   0        0        0     1341 2023-10-31 10:03:15.171235 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/list_instantiator.py
--rw-r--r--   0        0        0     1361 2023-10-31 10:10:40.539419 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/locale_constraint_instantiator.py
--rw-r--r--   0        0        0     1364 2023-10-31 10:03:15.172518 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/measurement_instantiator.py
--rw-r--r--   0        0        0     1573 2023-10-31 10:03:15.173018 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/operation_instantiator.py
--rw-r--r--   0        0        0     6016 2023-10-31 10:10:40.540409 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/property_instantiator.py
--rw-r--r--   0        0        0     1355 2023-10-31 10:03:15.173631 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/quantifiable_instantiator.py
--rw-r--r--   0        0        0     3631 2023-10-31 10:03:15.174132 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/range_constraint_instantiator.py
--rw-r--r--   0        0        0     1440 2023-10-31 10:10:40.540409 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/regular_expression_constraint_instantiator.py
--rw-r--r--   0        0        0     1082 2023-10-31 10:03:15.175131 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/scalar_instantiator.py
--rw-r--r--   0        0        0     1333 2023-10-31 10:03:15.175131 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/set_instantiator.py
--rw-r--r--   0        0        0     1187 2023-10-31 10:03:15.175631 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/single_entity_instantiator.py
--rw-r--r--   0        0        0     1383 2023-10-31 10:03:15.175955 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/sorted_set_instantiator.py
--rw-r--r--   0        0        0     2282 2023-10-31 10:03:15.203333 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/structured_value_instantiator.py
--rw-r--r--   0        0        0     1406 2023-10-31 10:03:15.176463 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/time_series_instantiator.py
--rw-r--r--   0        0        0     1801 2023-10-31 10:10:40.540409 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/trait_instantiator.py
--rw-r--r--   0        0        0     2929 2023-10-31 10:10:40.541573 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/unit_instantiator.py
--rw-r--r--   0        0        0     8111 2024-02-08 11:57:59.911659 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator_base.py
--rw-r--r--   0        0        0     7420 2023-10-31 10:10:40.541573 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/meta_model_base_attributes.py
--rw-r--r--   0        0        0     6130 2024-02-09 13:40:32.466027 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/model_element_factory.py
--rw-r--r--   0        0        0     3709 2023-10-31 10:03:15.205333 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/rdf_helper.py
--rw-r--r--   0        0        0     3209 2023-10-31 10:03:14.694486 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/README.md
--rw-r--r--   0        0        0      426 2023-10-31 10:03:14.823372 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/resolver/__init__.py
--rw-r--r--   0        0        0     3054 2024-02-08 11:59:22.930480 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/resolver/aspect_meta_model_resolver.py
--rw-r--r--   0        0        0      966 2023-10-31 10:03:14.756825 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/resolver/README.md
--rw-r--r--   0        0        0        0 2023-10-31 10:03:14.701086 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/__init__.py
--rw-r--r--   0        0        0     2268 2023-10-31 10:10:40.542580 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/download_samm_branch.py
--rw-r--r--   0        0        0     1968 2024-02-15 12:33:41.413670 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/download_samm_release.py
--rw-r--r--   0        0        0      899 2023-10-31 10:03:15.085537 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/github_file.py
--rw-r--r--   0        0        0     2152 2023-10-31 10:03:15.180457 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/github_folder.py
--rw-r--r--   0        0        0    10577 2024-02-06 10:45:05.319832 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/characteristic/1.0.0/characteristic-definitions.ttl
--rw-r--r--   0        0        0     2987 2024-02-06 10:45:05.321832 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/characteristic/1.0.0/characteristic-instances.ttl
--rw-r--r--   0        0        0    29696 2024-02-06 10:45:05.319832 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/characteristic/1.0.0/characteristic-shapes.ttl
--rw-r--r--   0        0        0     7107 2024-02-06 10:45:05.320871 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/characteristic/1.0.0/characteristic-validations.js
--rw-r--r--   0        0        0    11884 2024-02-06 10:45:05.323082 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/characteristic/2.0.0/characteristic-definitions.ttl
--rw-r--r--   0        0        0     2741 2024-02-06 10:45:05.325107 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/characteristic/2.0.0/characteristic-instances.ttl
--rw-r--r--   0        0        0    31188 2024-02-06 10:45:05.321832 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/characteristic/2.0.0/characteristic-shapes.ttl
--rw-r--r--   0        0        0     7107 2024-02-06 10:45:05.324108 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/characteristic/2.0.0/characteristic-validations.js
--rw-r--r--   0        0        0    11884 2024-02-06 10:45:05.327109 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/characteristic/2.1.0/characteristic-definitions.ttl
--rw-r--r--   0        0        0     2741 2024-02-06 10:45:05.328107 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/characteristic/2.1.0/characteristic-instances.ttl
--rw-r--r--   0        0        0    31188 2024-02-06 10:45:05.326154 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/characteristic/2.1.0/characteristic-shapes.ttl
--rw-r--r--   0        0        0     7107 2024-02-06 10:45:05.327109 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/characteristic/2.1.0/characteristic-validations.js
--rw-r--r--   0        0        0     1282 2024-02-06 10:45:05.330108 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/entity/1.0.0/FileResource.ttl
--rw-r--r--   0        0        0     1250 2024-02-06 10:45:05.329108 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/entity/1.0.0/Point3d.ttl
--rw-r--r--   0        0        0     1337 2024-02-06 10:45:05.330108 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/entity/1.0.0/TimeSeriesEntity.ttl
--rw-r--r--   0        0        0     1200 2024-02-06 10:45:05.331341 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/entity/2.0.0/FileResource.ttl
--rw-r--r--   0        0        0     1200 2024-02-06 10:45:05.331151 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/entity/2.0.0/Point3d.ttl
--rw-r--r--   0        0        0     1317 2024-02-06 10:45:05.331839 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/entity/2.0.0/TimeSeriesEntity.ttl
--rw-r--r--   0        0        0     1200 2024-02-06 10:45:05.332896 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/entity/2.1.0/FileResource.ttl
--rw-r--r--   0        0        0     1200 2024-02-06 10:45:05.331839 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/entity/2.1.0/Point3d.ttl
--rw-r--r--   0        0        0     1317 2024-02-06 10:45:05.332896 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/entity/2.1.0/TimeSeriesEntity.ttl
--rw-r--r--   0        0        0     7316 2024-02-06 10:45:05.301461 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/meta-model/1.0.0/aspect-meta-model-definitions.ttl
--rw-r--r--   0        0        0    28815 2024-02-06 10:45:05.300423 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/meta-model/1.0.0/aspect-meta-model-shapes.ttl
--rw-r--r--   0        0        0     2203 2024-02-06 10:45:05.300423 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/meta-model/1.0.0/prefix-declarations.ttl
--rw-r--r--   0        0        0     2669 2024-02-06 10:45:05.299465 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/meta-model/1.0.0/type-conversions.ttl
--rw-r--r--   0        0        0     9210 2024-02-06 10:45:05.304467 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/meta-model/2.0.0/aspect-meta-model-definitions.ttl
--rw-r--r--   0        0        0    36976 2024-02-06 10:45:05.303433 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/meta-model/2.0.0/aspect-meta-model-shapes.ttl
--rw-r--r--   0        0        0     2203 2024-02-06 10:45:05.303433 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/meta-model/2.0.0/prefix-declarations.ttl
--rw-r--r--   0        0        0     2671 2024-02-06 10:45:05.302513 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/meta-model/2.0.0/type-conversions.ttl
--rw-r--r--   0        0        0     9258 2024-02-16 08:31:30.716151 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/meta-model/2.1.0/aspect-meta-model-definitions.ttl
--rw-r--r--   0        0        0    37184 2024-02-06 10:45:05.308100 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/meta-model/2.1.0/aspect-meta-model-shapes.ttl
--rw-r--r--   0        0        0     2203 2024-02-06 10:45:05.306527 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/meta-model/2.1.0/prefix-declarations.ttl
--rw-r--r--   0        0        0     2671 2024-02-06 10:45:05.305508 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/meta-model/2.1.0/type-conversions.ttl
--rw-r--r--   0        0        0    55247 2024-02-06 10:45:05.309835 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/scripts/language-registry.js
--rw-r--r--   0        0        0   784140 2024-02-06 10:45:05.312833 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/unit/1.0.0/units.ttl
--rw-r--r--   0        0        0   674729 2024-02-06 10:45:05.315918 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/unit/2.0.0/units.ttl
--rw-r--r--   0        0        0   674729 2024-02-06 10:45:05.318920 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/unit/2.1.0/units.ttl
--rw-r--r--   0        0        0      426 2023-10-31 10:03:14.825371 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/vocabulary/__init__.py
--rw-r--r--   0        0        0     1262 2024-02-08 11:59:50.266257 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/vocabulary/namespace.py
--rw-r--r--   0        0        0     2516 2024-02-08 11:59:35.884914 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/vocabulary/SAMM.py
--rw-r--r--   0        0        0     2868 2023-10-31 10:03:15.181904 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/vocabulary/SAMMC.py
--rw-r--r--   0        0        0     1252 2023-10-31 10:03:15.181904 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/vocabulary/SAMME.py
--rw-r--r--   0        0        0     1078 2023-10-31 10:03:15.181904 test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/vocabulary/UNIT.py
--rw-r--r--   0        0        0     1659 2024-02-22 10:23:09.870588 test_esmf_loader-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2628 2024-02-19 13:57:01.318644 test_esmf_loader-0.0.1/README.md
--rw-r--r--   0        0        0     3692 1970-01-01 00:00:00.000000 test_esmf_loader-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2021 2024-02-14 14:39:42.096721 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/__init__.py
+-rw-r--r--   0        0        0     2289 2023-10-31 10:36:17.197378 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/__init__.py
+-rw-r--r--   0        0        0     1277 2023-10-31 10:10:40.580805 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/aspect.py
+-rw-r--r--   0        0        0     1116 2023-10-31 10:10:40.580805 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/base.py
+-rw-r--r--   0        0        0      848 2023-10-31 10:10:40.580805 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/bound_definition.py
+-rw-r--r--   0        0        0     2050 2023-10-31 10:10:40.581816 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/cache_strategy.py
+-rw-r--r--   0        0        0      426 2023-10-31 10:03:14.801371 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/characteristics/__init__.py
+-rw-r--r--   0        0        0      989 2023-10-31 10:10:40.581816 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/characteristics/characteristic.py
+-rw-r--r--   0        0        0      683 2023-10-31 10:10:40.581816 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/characteristics/code.py
+-rw-r--r--   0        0        0      426 2023-10-31 10:03:14.802370 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/characteristics/collection/__init__.py
+-rw-r--r--   0        0        0     1062 2023-10-31 10:10:40.582815 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/characteristics/collection/collection.py
+-rw-r--r--   0        0        0      685 2023-10-31 10:10:40.582815 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/characteristics/collection/list.py
+-rw-r--r--   0        0        0      685 2023-10-31 10:10:40.582815 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/characteristics/collection/set.py
+-rw-r--r--   0        0        0      696 2023-10-31 10:10:40.582815 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/characteristics/collection/sorted_set.py
+-rw-r--r--   0        0        0      692 2023-10-31 10:10:40.583815 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/characteristics/collection/time_series.py
+-rw-r--r--   0        0        0      847 2023-10-31 10:10:40.583815 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/characteristics/enumeration.py
+-rw-r--r--   0        0        0      426 2023-10-31 10:03:14.803370 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/characteristics/quantifiable/__init__.py
+-rw-r--r--   0        0        0      689 2023-10-31 10:10:40.584816 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/characteristics/quantifiable/duration.py
+-rw-r--r--   0        0        0      691 2023-10-31 10:10:40.584816 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/characteristics/quantifiable/measurement.py
+-rw-r--r--   0        0        0      943 2023-10-31 10:10:40.584816 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/characteristics/quantifiable/quantifiable.py
+-rw-r--r--   0        0        0      697 2023-10-31 10:10:40.584816 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/characteristics/single_entity.py
+-rw-r--r--   0        0        0      779 2023-10-31 10:10:40.585816 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/characteristics/state.py
+-rw-r--r--   0        0        0     1070 2023-10-31 10:10:40.585816 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/characteristics/structured_value.py
+-rw-r--r--   0        0        0     1177 2023-10-31 10:10:40.585816 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/characteristics/trait.py
+-rw-r--r--   0        0        0      426 2023-10-31 10:03:14.804371 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/contraints/__init__.py
+-rw-r--r--   0        0        0      747 2023-10-31 10:10:40.585816 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/contraints/constraint.py
+-rw-r--r--   0        0        0      816 2023-10-31 10:10:40.586815 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/contraints/encoding_constraint.py
+-rw-r--r--   0        0        0     1049 2023-10-31 10:10:40.586815 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/contraints/fixed_point_constraint.py
+-rw-r--r--   0        0        0      859 2023-10-31 10:10:40.586815 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/contraints/language_constraint.py
+-rw-r--r--   0        0        0     1101 2023-10-31 10:10:40.587815 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/contraints/length_constraint.py
+-rw-r--r--   0        0        0      861 2023-10-31 10:10:40.587815 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/contraints/locale_constraint.py
+-rw-r--r--   0        0        0     1519 2023-10-31 10:10:40.587815 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/contraints/range_constraint.py
+-rw-r--r--   0        0        0      872 2023-10-31 10:10:40.588820 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/contraints/regular_expression_constraint.py
+-rw-r--r--   0        0        0      426 2023-10-31 10:03:14.806371 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/data_types/__init__.py
+-rw-r--r--   0        0        0      915 2023-10-31 10:10:40.588820 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/data_types/abstract_entity.py
+-rw-r--r--   0        0        0     1284 2023-10-31 10:10:40.588820 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/data_types/complex_type.py
+-rw-r--r--   0        0        0      990 2023-10-31 10:10:40.588820 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/data_types/data_type.py
+-rw-r--r--   0        0        0      760 2023-10-31 10:10:40.589816 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/data_types/entity.py
+-rw-r--r--   0        0        0      876 2024-01-29 09:31:02.594330 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/data_types/scalar.py
+-rw-r--r--   0        0        0      961 2023-10-31 10:36:17.197378 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/either.py
+-rw-r--r--   0        0        0      992 2023-10-31 10:10:40.589816 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/event.py
+-rw-r--r--   0        0        0      858 2023-10-31 10:10:40.589816 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/has_properties.py
+-rw-r--r--   0        0        0      902 2023-10-31 10:10:40.590814 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/has_urn.py
+-rw-r--r--   0        0        0     1549 2023-10-31 10:10:40.590814 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/is_described.py
+-rw-r--r--   0        0        0     1104 2023-10-31 10:10:40.590814 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/operation.py
+-rw-r--r--   0        0        0     2648 2023-10-31 10:10:40.590814 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/property.py
+-rw-r--r--   0        0        0     1811 2023-10-31 10:10:40.590814 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/property_func.py
+-rw-r--r--   0        0        0      700 2023-10-31 10:10:40.591817 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/quantity_kind.py
+-rw-r--r--   0        0        0     2082 2024-03-29 11:56:00.175717 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/README.md
+-rw-r--r--   0        0        0      687 2023-10-31 10:10:40.591817 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/structure_element.py
+-rw-r--r--   0        0        0     1414 2023-10-31 10:10:40.591817 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/unit.py
+-rw-r--r--   0        0        0     2784 2024-02-19 13:57:01.320643 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/__init__.py
+-rw-r--r--   0        0        0     2517 2023-10-31 10:10:40.591817 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/base_impl.py
+-rw-r--r--   0        0        0      426 2023-10-31 10:03:14.809370 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/characteristics/__init__.py
+-rw-r--r--   0        0        0      426 2023-10-31 10:03:14.809370 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/characteristics/collection/__init__.py
+-rw-r--r--   0        0        0     1826 2023-10-31 10:10:40.592815 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/characteristics/collection/default_collection.py
+-rw-r--r--   0        0        0      705 2023-10-31 10:10:40.592815 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/characteristics/collection/default_list.py
+-rw-r--r--   0        0        0      700 2023-10-31 10:10:40.592815 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/characteristics/collection/default_set.py
+-rw-r--r--   0        0        0      732 2023-10-31 10:10:40.592815 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/characteristics/collection/default_sorted_set.py
+-rw-r--r--   0        0        0      735 2023-10-31 10:10:40.592815 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/characteristics/collection/default_time_series.py
+-rw-r--r--   0        0        0     1371 2023-10-31 10:10:40.593815 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/characteristics/default_characteristic.py
+-rw-r--r--   0        0        0      695 2023-10-31 10:10:40.593815 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/characteristics/default_code.py
+-rw-r--r--   0        0        0     1291 2023-10-31 10:10:40.593815 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/characteristics/default_enumeration.py
+-rw-r--r--   0        0        0      737 2023-10-31 10:10:40.593815 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/characteristics/default_single_entity.py
+-rw-r--r--   0        0        0     1321 2023-10-31 10:10:40.594815 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/characteristics/default_state.py
+-rw-r--r--   0        0        0     1554 2023-10-31 10:10:40.595049 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/characteristics/default_structured_value.py
+-rw-r--r--   0        0        0     1984 2023-10-31 10:10:40.595552 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/characteristics/default_trait.py
+-rw-r--r--   0        0        0      426 2023-10-31 10:03:14.811370 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/characteristics/quantifiable/__init__.py
+-rw-r--r--   0        0        0      735 2023-10-31 10:10:40.595552 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/characteristics/quantifiable/default_duration.py
+-rw-r--r--   0        0        0      750 2023-10-31 10:10:40.595552 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/characteristics/quantifiable/default_measurement.py
+-rw-r--r--   0        0        0     1465 2023-10-31 10:10:40.595552 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/characteristics/quantifiable/default_quantifiable.py
+-rw-r--r--   0        0        0      426 2023-10-31 10:03:14.812370 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/constraints/__init__.py
+-rw-r--r--   0        0        0      702 2023-10-31 10:10:40.595552 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/constraints/default_constraint.py
+-rw-r--r--   0        0        0     1118 2023-10-31 10:10:40.596568 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/constraints/default_encoding_constraint.py
+-rw-r--r--   0        0        0     1323 2023-10-31 10:10:40.596568 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/constraints/default_fixed_point_constraint.py
+-rw-r--r--   0        0        0     1166 2023-10-31 10:10:40.596568 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/constraints/default_language_constraint.py
+-rw-r--r--   0        0        0     1408 2023-10-31 10:10:40.596568 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/constraints/default_length_constraint.py
+-rw-r--r--   0        0        0     1144 2023-10-31 10:10:40.597568 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/constraints/default_locale_constraint.py
+-rw-r--r--   0        0        0     2073 2023-10-31 10:10:40.597568 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/constraints/default_range_constraint.py
+-rw-r--r--   0        0        0     1159 2023-10-31 10:10:40.597568 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/constraints/default_regular_expression_constraint.py
+-rw-r--r--   0        0        0      426 2023-10-31 10:03:14.814371 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/data_types/__init__.py
+-rw-r--r--   0        0        0     1597 2023-10-31 10:10:40.597568 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/data_types/default_abstract_entity.py
+-rw-r--r--   0        0        0     3612 2023-10-31 10:10:40.597568 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/data_types/default_complex_type.py
+-rw-r--r--   0        0        0      946 2024-02-19 13:57:01.320643 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/data_types/default_data_type.py
+-rw-r--r--   0        0        0      687 2023-10-31 10:10:40.598567 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/data_types/default_entity.py
+-rw-r--r--   0        0        0      935 2024-02-14 13:17:05.158388 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/data_types/default_scalar.py
+-rw-r--r--   0        0        0     2389 2023-10-31 10:10:40.598567 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/default_aspect.py
+-rw-r--r--   0        0        0     1408 2023-10-31 10:36:17.197378 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/default_either.py
+-rw-r--r--   0        0        0     1167 2023-10-31 10:10:40.598567 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/default_event.py
+-rw-r--r--   0        0        0     1876 2023-10-31 10:10:40.598567 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/default_operation.py
+-rw-r--r--   0        0        0     3961 2023-10-31 10:10:40.599568 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/default_property.py
+-rw-r--r--   0        0        0      666 2023-10-31 10:10:40.599568 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/default_quantity_kind.py
+-rw-r--r--   0        0        0     2293 2023-10-31 10:10:40.599568 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/default_unit.py
+-rw-r--r--   0        0        0     3974 2023-10-31 10:03:14.751826 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/README.md
+-rw-r--r--   0        0        0      426 2023-10-31 10:03:14.816371 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/__init__.py
+-rw-r--r--   0        0        0    11421 2024-04-05 07:02:05.993502 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/aspect_loader.py
+-rw-r--r--   0        0        0     2253 2023-10-31 10:03:15.165891 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/default_element_cache.py
+-rw-r--r--   0        0        0      426 2023-10-31 10:03:14.817371 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/__init__.py
+-rw-r--r--   0        0        0     1813 2023-10-31 10:03:15.165891 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/abstract_entity_instantiator.py
+-rw-r--r--   0        0        0     4143 2023-10-31 10:10:40.537605 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/abstract_property_instantiator.py
+-rw-r--r--   0        0        0     1968 2023-10-31 10:03:15.166897 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/aspect_instantiator.py
+-rw-r--r--   0        0        0     1276 2024-03-29 11:56:00.177781 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/characteristic_instantiator.py
+-rw-r--r--   0        0        0     1196 2024-03-29 11:56:00.178890 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/code_instantiator.py
+-rw-r--r--   0        0        0     1471 2024-03-29 11:56:00.179914 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/collection_instantiator.py
+-rw-r--r--   0        0        0     2924 2023-10-31 10:10:40.538374 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/complex_type_instantiator.py
+-rw-r--r--   0        0        0      543 2024-03-29 11:56:00.179914 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/constants.py
+-rw-r--r--   0        0        0     1102 2024-02-26 10:28:02.163063 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/datatype_instantiator.py
+-rw-r--r--   0        0        0     1405 2024-03-29 11:56:00.180983 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/duration_instantiator.py
+-rw-r--r--   0        0        0     1181 2023-10-31 10:36:17.197378 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/either_instantiator.py
+-rw-r--r--   0        0        0     1392 2023-10-31 10:10:40.538374 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/encoding_constraint_instantiator.py
+-rw-r--r--   0        0        0     1873 2023-10-31 10:03:15.169897 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/entity_instantiator.py
+-rw-r--r--   0        0        0     4808 2024-03-29 11:56:00.183053 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/enumeration_instantiator.py
+-rw-r--r--   0        0        0     1200 2023-10-31 10:03:15.169897 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/event_instantiator.py
+-rw-r--r--   0        0        0     1554 2023-10-31 10:10:40.539419 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/fixed_point_constraint_instantiator.py
+-rw-r--r--   0        0        0     1383 2023-10-31 10:10:40.539419 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/language_constraint_instantiator.py
+-rw-r--r--   0        0        0     1538 2023-10-31 10:10:40.539419 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/length_constraint_instantiator.py
+-rw-r--r--   0        0        0     1423 2024-03-29 11:56:00.184173 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/list_instantiator.py
+-rw-r--r--   0        0        0     1361 2023-10-31 10:10:40.539419 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/locale_constraint_instantiator.py
+-rw-r--r--   0        0        0     1444 2024-03-29 11:56:00.184173 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/measurement_instantiator.py
+-rw-r--r--   0        0        0     1573 2023-10-31 10:03:15.173018 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/operation_instantiator.py
+-rw-r--r--   0        0        0     6016 2023-10-31 10:10:40.540409 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/property_instantiator.py
+-rw-r--r--   0        0        0     1437 2024-03-29 11:56:00.185189 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/quantifiable_instantiator.py
+-rw-r--r--   0        0        0     3631 2023-10-31 10:03:15.174132 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/range_constraint_instantiator.py
+-rw-r--r--   0        0        0     1440 2023-10-31 10:10:40.540409 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/regular_expression_constraint_instantiator.py
+-rw-r--r--   0        0        0     1082 2023-10-31 10:03:15.175131 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/scalar_instantiator.py
+-rw-r--r--   0        0        0     1415 2024-03-29 11:56:00.186202 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/set_instantiator.py
+-rw-r--r--   0        0        0     1269 2024-03-29 11:56:00.187245 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/single_entity_instantiator.py
+-rw-r--r--   0        0        0     1465 2024-03-29 11:56:00.187245 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/sorted_set_instantiator.py
+-rw-r--r--   0        0        0     2360 2024-03-29 11:56:00.188264 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/structured_value_instantiator.py
+-rw-r--r--   0        0        0     1473 2024-03-29 11:56:00.189278 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/time_series_instantiator.py
+-rw-r--r--   0        0        0     1801 2023-10-31 10:10:40.540409 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/trait_instantiator.py
+-rw-r--r--   0        0        0     2929 2023-10-31 10:10:40.541573 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/unit_instantiator.py
+-rw-r--r--   0        0        0     8127 2024-03-29 11:56:00.190292 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator_base.py
+-rw-r--r--   0        0        0     7420 2023-10-31 10:10:40.541573 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/meta_model_base_attributes.py
+-rw-r--r--   0        0        0     6114 2024-03-29 11:56:00.191304 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/model_element_factory.py
+-rw-r--r--   0        0        0     3709 2023-10-31 10:03:15.205333 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/rdf_helper.py
+-rw-r--r--   0        0        0     3209 2023-10-31 10:03:14.694486 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/README.md
+-rw-r--r--   0        0        0      426 2023-10-31 10:03:14.823372 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/resolver/__init__.py
+-rw-r--r--   0        0        0     3054 2024-04-04 09:38:25.316010 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/resolver/aspect_meta_model_resolver.py
+-rw-r--r--   0        0        0      966 2023-10-31 10:03:14.756825 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/resolver/README.md
+-rw-r--r--   0        0        0        0 2023-10-31 10:03:14.701086 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/__init__.py
+-rw-r--r--   0        0        0     2268 2023-10-31 10:10:40.542580 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/download_samm_branch.py
+-rw-r--r--   0        0        0     1968 2024-04-01 12:38:41.354644 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/download_samm_release.py
+-rw-r--r--   0        0        0      899 2023-10-31 10:03:15.085537 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/github_file.py
+-rw-r--r--   0        0        0     2152 2023-10-31 10:03:15.180457 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/github_folder.py
+-rw-r--r--   0        0        0    10577 2024-04-01 12:35:01.813916 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/characteristic/1.0.0/characteristic-definitions.ttl
+-rw-r--r--   0        0        0     2987 2024-04-01 12:35:01.813916 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/characteristic/1.0.0/characteristic-instances.ttl
+-rw-r--r--   0        0        0    29696 2024-04-01 12:35:01.813916 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/characteristic/1.0.0/characteristic-shapes.ttl
+-rw-r--r--   0        0        0     7107 2024-04-01 12:35:01.813916 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/characteristic/1.0.0/characteristic-validations.js
+-rw-r--r--   0        0        0    11884 2024-04-01 12:35:01.815063 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/characteristic/2.0.0/characteristic-definitions.ttl
+-rw-r--r--   0        0        0     2741 2024-04-01 12:35:01.815063 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/characteristic/2.0.0/characteristic-instances.ttl
+-rw-r--r--   0        0        0    31188 2024-04-01 12:35:01.815063 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/characteristic/2.0.0/characteristic-shapes.ttl
+-rw-r--r--   0        0        0     7107 2024-04-01 12:35:01.815063 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/characteristic/2.0.0/characteristic-validations.js
+-rw-r--r--   0        0        0    11884 2024-04-01 12:35:01.816102 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/characteristic/2.1.0/characteristic-definitions.ttl
+-rw-r--r--   0        0        0     2741 2024-04-01 12:35:01.816102 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/characteristic/2.1.0/characteristic-instances.ttl
+-rw-r--r--   0        0        0    31188 2024-04-01 12:35:01.816102 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/characteristic/2.1.0/characteristic-shapes.ttl
+-rw-r--r--   0        0        0     7107 2024-04-01 12:35:01.816102 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/characteristic/2.1.0/characteristic-validations.js
+-rw-r--r--   0        0        0     1282 2024-04-01 12:35:01.817152 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/entity/1.0.0/FileResource.ttl
+-rw-r--r--   0        0        0     1250 2024-04-01 12:35:01.817152 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/entity/1.0.0/Point3d.ttl
+-rw-r--r--   0        0        0     1337 2024-04-01 12:35:01.817152 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/entity/1.0.0/TimeSeriesEntity.ttl
+-rw-r--r--   0        0        0     1200 2024-04-01 12:35:01.817152 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/entity/2.0.0/FileResource.ttl
+-rw-r--r--   0        0        0     1200 2024-04-01 12:35:01.817152 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/entity/2.0.0/Point3d.ttl
+-rw-r--r--   0        0        0     1317 2024-04-01 12:35:01.818215 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/entity/2.0.0/TimeSeriesEntity.ttl
+-rw-r--r--   0        0        0     1200 2024-04-01 12:35:01.818215 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/entity/2.1.0/FileResource.ttl
+-rw-r--r--   0        0        0     1200 2024-04-01 12:35:01.818215 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/entity/2.1.0/Point3d.ttl
+-rw-r--r--   0        0        0     1317 2024-04-01 12:35:01.818215 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/entity/2.1.0/TimeSeriesEntity.ttl
+-rw-r--r--   0        0        0     7316 2024-04-01 12:35:01.803933 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/meta-model/1.0.0/aspect-meta-model-definitions.ttl
+-rw-r--r--   0        0        0    28815 2024-04-01 12:35:01.803933 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/meta-model/1.0.0/aspect-meta-model-shapes.ttl
+-rw-r--r--   0        0        0     2203 2024-04-01 12:35:01.803933 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/meta-model/1.0.0/prefix-declarations.ttl
+-rw-r--r--   0        0        0     2669 2024-04-01 12:35:01.802794 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/meta-model/1.0.0/type-conversions.ttl
+-rw-r--r--   0        0        0     9210 2024-04-01 12:35:01.805120 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/meta-model/2.0.0/aspect-meta-model-definitions.ttl
+-rw-r--r--   0        0        0    36976 2024-04-01 12:35:01.805120 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/meta-model/2.0.0/aspect-meta-model-shapes.ttl
+-rw-r--r--   0        0        0     2203 2024-04-01 12:35:01.805120 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/meta-model/2.0.0/prefix-declarations.ttl
+-rw-r--r--   0        0        0     2671 2024-04-01 12:35:01.804936 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/meta-model/2.0.0/type-conversions.ttl
+-rw-r--r--   0        0        0     9214 2024-04-01 12:35:01.806241 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/meta-model/2.1.0/aspect-meta-model-definitions.ttl
+-rw-r--r--   0        0        0    37184 2024-04-01 12:35:01.806241 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/meta-model/2.1.0/aspect-meta-model-shapes.ttl
+-rw-r--r--   0        0        0     2203 2024-04-01 12:35:01.806241 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/meta-model/2.1.0/prefix-declarations.ttl
+-rw-r--r--   0        0        0     2671 2024-04-01 12:35:01.805120 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/meta-model/2.1.0/type-conversions.ttl
+-rw-r--r--   0        0        0    55247 2024-04-01 12:35:01.806241 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/scripts/language-registry.js
+-rw-r--r--   0        0        0   784140 2024-04-01 12:35:01.809460 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/unit/1.0.0/units.ttl
+-rw-r--r--   0        0        0   674729 2024-04-01 12:35:01.811583 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/unit/2.0.0/units.ttl
+-rw-r--r--   0        0        0   674729 2024-04-01 12:35:01.812823 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/unit/2.1.0/units.ttl
+-rw-r--r--   0        0        0      426 2023-10-31 10:03:14.825371 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/vocabulary/__init__.py
+-rw-r--r--   0        0        0     1262 2024-02-08 11:59:50.266257 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/vocabulary/namespace.py
+-rw-r--r--   0        0        0     2516 2024-02-08 11:59:35.884914 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/vocabulary/SAMM.py
+-rw-r--r--   0        0        0     2868 2023-10-31 10:03:15.181904 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/vocabulary/SAMMC.py
+-rw-r--r--   0        0        0     1252 2023-10-31 10:03:15.181904 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/vocabulary/SAMME.py
+-rw-r--r--   0        0        0     1078 2023-10-31 10:03:15.181904 test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/vocabulary/UNIT.py
+-rw-r--r--   0        0        0     1975 2024-04-05 07:22:52.387793 test_esmf_loader-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2628 2024-02-19 13:57:01.318644 test_esmf_loader-0.0.2/README.md
+-rw-r--r--   0        0        0     3692 1970-01-01 00:00:00.000000 test_esmf_loader-0.0.2/PKG-INFO
```

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/__init__.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/__init__.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/__init__.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/__init__.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/aspect.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/aspect.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/base.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/base.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/bound_definition.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/bound_definition.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/cache_strategy.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/cache_strategy.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/characteristics/characteristic.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/characteristics/characteristic.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/characteristics/code.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/characteristics/code.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/characteristics/collection/collection.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/characteristics/collection/collection.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/characteristics/collection/list.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/characteristics/collection/list.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/characteristics/collection/set.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/characteristics/collection/set.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/characteristics/collection/sorted_set.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/characteristics/collection/sorted_set.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/characteristics/collection/time_series.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/characteristics/collection/time_series.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/characteristics/enumeration.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/characteristics/enumeration.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/characteristics/quantifiable/duration.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/characteristics/quantifiable/duration.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/characteristics/quantifiable/measurement.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/characteristics/quantifiable/measurement.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/characteristics/quantifiable/quantifiable.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/characteristics/quantifiable/quantifiable.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/characteristics/single_entity.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/characteristics/single_entity.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/characteristics/state.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/characteristics/state.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/characteristics/structured_value.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/characteristics/structured_value.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/characteristics/trait.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/characteristics/trait.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/contraints/constraint.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/contraints/constraint.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/contraints/encoding_constraint.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/contraints/encoding_constraint.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/contraints/fixed_point_constraint.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/contraints/fixed_point_constraint.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/contraints/language_constraint.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/contraints/language_constraint.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/contraints/length_constraint.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/contraints/length_constraint.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/contraints/locale_constraint.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/contraints/locale_constraint.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/contraints/range_constraint.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/contraints/range_constraint.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/contraints/regular_expression_constraint.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/contraints/regular_expression_constraint.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/data_types/abstract_entity.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/data_types/abstract_entity.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/data_types/complex_type.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/data_types/complex_type.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/data_types/data_type.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/data_types/data_type.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/data_types/entity.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/data_types/entity.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/data_types/scalar.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/data_types/scalar.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/either.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/either.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/event.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/event.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/has_properties.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/has_properties.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/has_urn.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/has_urn.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/is_described.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/is_described.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/operation.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/operation.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/property.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/property.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/property_func.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/property_func.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/quantity_kind.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/quantity_kind.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/README.md` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 HasUrn
 ├───────────────────────────────────────────────── DataType
 └── IsDescribed                                    ├── Scalar
     └── Base                    HasProperties      │
         ├── StructureElement <──┘                  │
         │   ├── Aspect                             │
         │   └── ComplexType <──────────────────────┘
-        │       ├── AbstractEntity                 
+        │       ├── AbstractEntity
         │       └── Entity
         ├── Characteristic
         │   ├── Code
         │   ├── Collection
         │   │   ├── List
         │   │   ├── Set
         │   │   └── SortedSet
@@ -37,12 +37,12 @@
         │   ├── LengthConstraint
         │   ├── LocaleConstraint
         │   ├── RangeConstraint
         │   └── RegularExpressionConstraint
         ├── Event
         ├── Operation
         ├── Property
-        ├── QuantityKind           
+        ├── QuantityKind
         └── Unit
 
 BoundDefiniton
 ```
```

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/structure_element.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/structure_element.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/base/unit.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/base/unit.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/__init__.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/__init__.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/base_impl.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/base_impl.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/characteristics/collection/default_collection.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/characteristics/collection/default_collection.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/characteristics/collection/default_list.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/characteristics/collection/default_list.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/characteristics/collection/default_set.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/characteristics/collection/default_set.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/characteristics/collection/default_sorted_set.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/characteristics/collection/default_sorted_set.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/characteristics/collection/default_time_series.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/characteristics/collection/default_time_series.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/characteristics/default_characteristic.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/characteristics/default_characteristic.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/characteristics/default_code.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/characteristics/default_code.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/characteristics/default_enumeration.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/characteristics/default_enumeration.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/characteristics/default_single_entity.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/characteristics/default_single_entity.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/characteristics/default_state.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/characteristics/default_state.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/characteristics/default_structured_value.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/characteristics/default_structured_value.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/characteristics/default_trait.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/characteristics/default_trait.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/characteristics/quantifiable/default_duration.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/characteristics/quantifiable/default_duration.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/characteristics/quantifiable/default_measurement.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/characteristics/quantifiable/default_measurement.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/characteristics/quantifiable/default_quantifiable.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/characteristics/quantifiable/default_quantifiable.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/constraints/default_constraint.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/constraints/default_constraint.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/constraints/default_encoding_constraint.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/constraints/default_encoding_constraint.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/constraints/default_fixed_point_constraint.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/constraints/default_fixed_point_constraint.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/constraints/default_language_constraint.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/constraints/default_language_constraint.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/constraints/default_length_constraint.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/constraints/default_length_constraint.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/constraints/default_locale_constraint.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/constraints/default_locale_constraint.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/constraints/default_range_constraint.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/constraints/default_range_constraint.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/constraints/default_regular_expression_constraint.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/constraints/default_regular_expression_constraint.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/data_types/default_abstract_entity.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/data_types/default_abstract_entity.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/data_types/default_complex_type.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/data_types/default_complex_type.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/data_types/default_data_type.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/data_types/default_data_type.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/data_types/default_entity.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/data_types/default_entity.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/data_types/default_scalar.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/data_types/default_scalar.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/default_aspect.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/default_aspect.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/default_either.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/default_either.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/default_event.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/default_event.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/default_operation.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/default_operation.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/default_property.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/default_property.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/default_quantity_kind.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/default_quantity_kind.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/default_unit.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/default_unit.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/impl/README.md` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/impl/README.md`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/aspect_loader.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/aspect_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         """Load aspect model to RDF GRAPH.
 
         Create an aspect object with all the including properties and operations with the turtle file
 
         :param file_path: path to the turtle file. Can be either a string or a Path object
         :return: instance of the aspect
         """
-        return self.load_aspect_model_from_multiple_files([file_path])
+        return self._load_aspect_model_from_multiple_files([file_path])
 
     @staticmethod
     def _get_additional_files_from_dir(file_path: str) -> list[str]:
         """Get additional files from specific directory.
 
         :param file_path: path list to the turtle files
         :return: list of the additional turtle files
@@ -152,15 +152,15 @@
 
         for file_path in self._prepare_file_paths(file_paths):
             aspect_graph.parse(file_path, format="turtle")
             self._extend_graph_with_prefix_files(aspect_graph, file_path)
 
         return aspect_graph
 
-    def load_aspect_model_from_multiple_files(
+    def _load_aspect_model_from_multiple_files(
         self,
         file_paths: list[Union[str, Path]],
         aspect_urn: rdflib.URIRef | str = "",
     ) -> Aspect:
         """Load aspect model from multiple files.
 
         Create aspect specified in urn with all the including properties and operations with the turtle files
@@ -180,16 +180,17 @@
             aspect_urn = aspect_graph.value(predicate=rdflib.RDF.type, object=samm.get_urn(SAMM.aspect))  # type: ignore
 
         if aspect_urn is not rdflib.URIRef:
             aspect_urn = rdflib.URIRef(aspect_urn)
 
         AspectMetaModelResolver.resolve_meta_model(aspect_graph, meta_model_version)
         model_element_factory = ModelElementFactory(meta_model_version, aspect_graph, self._cache)
+        aspect_element = model_element_factory.create_element(aspect_urn)  # type: ignore
 
-        return model_element_factory.create_element(aspect_urn)  # type: ignore
+        return aspect_element
 
     @staticmethod
     def __extract_samm_version(aspect_graph: rdflib.Graph) -> str:
         """Get samm version.
 
         searches the aspect graph for the currently used version of the SAMM and returns it
```

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/default_element_cache.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/default_element_cache.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/abstract_entity_instantiator.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/abstract_entity_instantiator.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/abstract_property_instantiator.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/abstract_property_instantiator.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/aspect_instantiator.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/aspect_instantiator.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/characteristic_instantiator.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/characteristic_instantiator.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,19 +9,20 @@
 #
 #   SPDX-License-Identifier: MPL-2.0
 
 from rdflib.term import Node
 
 from esmf_aspect_meta_model_python.base.characteristics.characteristic import Characteristic
 from esmf_aspect_meta_model_python.impl.characteristics.default_characteristic import DefaultCharacteristic
+from esmf_aspect_meta_model_python.loader.instantiator.constants import DATA_TYPE_ERROR_MSG
 from esmf_aspect_meta_model_python.loader.instantiator_base import InstantiatorBase
 
 
 class CharacteristicInstantiator(InstantiatorBase[Characteristic]):
     def _create_instance(self, element_node: Node) -> Characteristic:
-        meta_model_base_attributes = self._get_base_attributes(element_node)
         data_type = self._get_data_type(element_node)
+        if not data_type:
+            raise TypeError(DATA_TYPE_ERROR_MSG)
 
-        if data_type is None:
-            raise TypeError("Data type can't be None.")
+        meta_model_base_attributes = self._get_base_attributes(element_node)
 
         return DefaultCharacteristic(meta_model_base_attributes, data_type)
```

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/code_instantiator.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/event_instantiator.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 #
 #   SPDX-License-Identifier: MPL-2.0
 
+from typing import List
+
 from rdflib.term import Node
 
-from esmf_aspect_meta_model_python.base.characteristics.code import Code
-from esmf_aspect_meta_model_python.impl.characteristics.default_code import DefaultCode
+from esmf_aspect_meta_model_python import Property
+from esmf_aspect_meta_model_python.base.event import Event
+from esmf_aspect_meta_model_python.impl.default_event import DefaultEvent
 from esmf_aspect_meta_model_python.loader.instantiator_base import InstantiatorBase
+from esmf_aspect_meta_model_python.vocabulary.SAMM import SAMM
 
 
-class CodeInstantiator(InstantiatorBase[Code]):
-    def _create_instance(self, element_node: Node) -> Code:
+class EventInstantiator(InstantiatorBase[Event]):
+    def _create_instance(self, element_node: Node) -> Event:
         meta_model_base_attributes = self._get_base_attributes(element_node)
-        data_type = self._get_data_type(element_node)
-
-        if data_type is None:
-            raise TypeError("Data type can't be None.")
-
-        return DefaultCode(meta_model_base_attributes, data_type)
+        parameters: List[Property] = self._get_list_children(element_node, self._samm.get_urn(SAMM.parameters))
+        return DefaultEvent(meta_model_base_attributes, parameters)
```

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/collection_instantiator.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/collection_instantiator.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,21 +9,22 @@
 #
 #   SPDX-License-Identifier: MPL-2.0
 
 from rdflib.term import Node
 
 from esmf_aspect_meta_model_python.base.characteristics.collection.collection import Collection
 from esmf_aspect_meta_model_python.impl.characteristics.collection.default_collection import DefaultCollection
+from esmf_aspect_meta_model_python.loader.instantiator.constants import DATA_TYPE_ERROR_MSG
 from esmf_aspect_meta_model_python.loader.instantiator_base import InstantiatorBase
 from esmf_aspect_meta_model_python.vocabulary.SAMMC import SAMMC
 
 
 class CollectionInstantiator(InstantiatorBase[Collection]):
     def _create_instance(self, element_node: Node) -> Collection:
-        meta_model_base_attributes = self._get_base_attributes(element_node)
-        element_characteristic = self._get_child(element_node, self._sammc.get_urn(SAMMC.element_characteristic))
         data_type = self._get_data_type(element_node)
+        if not data_type:
+            raise TypeError(DATA_TYPE_ERROR_MSG)
 
-        if data_type is None:
-            raise TypeError("Data type can't be None.")
+        meta_model_base_attributes = self._get_base_attributes(element_node)
+        element_characteristic = self._get_child(element_node, self._sammc.get_urn(SAMMC.element_characteristic))
 
         return DefaultCollection(meta_model_base_attributes, data_type, element_characteristic)
```

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/complex_type_instantiator.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/complex_type_instantiator.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/datatype_instantiator.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/datatype_instantiator.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/duration_instantiator.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/encoding_constraint_instantiator.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,23 +7,22 @@
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 #
 #   SPDX-License-Identifier: MPL-2.0
 
 from rdflib.term import Node
 
-from esmf_aspect_meta_model_python.base.characteristics.quantifiable.duration import Duration
-from esmf_aspect_meta_model_python.impl.characteristics.quantifiable.default_duration import DefaultDuration
+from esmf_aspect_meta_model_python.base.contraints.encoding_constraint import EncodingConstraint
+from esmf_aspect_meta_model_python.impl.constraints.default_encoding_constraint import DefaultEncodingConstraint
 from esmf_aspect_meta_model_python.loader.instantiator_base import InstantiatorBase
-from esmf_aspect_meta_model_python.vocabulary.SAMMC import SAMMC
+from esmf_aspect_meta_model_python.loader.rdf_helper import RdfHelper
+from esmf_aspect_meta_model_python.vocabulary.SAMM import SAMM
 
 
-class DurationInstantiator(InstantiatorBase[Duration]):
-    def _create_instance(self, element_node: Node) -> Duration:
+class EncodingConstraintInstantiator(InstantiatorBase[EncodingConstraint]):
+    def _create_instance(self, element_node: Node) -> EncodingConstraint:
         meta_model_base_attributes = self._get_base_attributes(element_node)
-        data_type = self._get_data_type(element_node)
-        unit = self._get_child(element_node, self._sammc.get_urn(SAMMC.unit))
-
-        if data_type is None:
-            raise TypeError("Data type can't be None.")
-
-        return DefaultDuration(meta_model_base_attributes, data_type, unit)
+        value = RdfHelper.to_python(
+            self._aspect_graph.value(subject=element_node, predicate=self._samm.get_urn(SAMM.value)),
+        )
+        value = value.split("#")[1]
+        return DefaultEncodingConstraint(meta_model_base_attributes, value)
```

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/either_instantiator.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/either_instantiator.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/encoding_constraint_instantiator.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/fixed_point_constraint_instantiator.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,22 +7,24 @@
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 #
 #   SPDX-License-Identifier: MPL-2.0
 
 from rdflib.term import Node
 
-from esmf_aspect_meta_model_python.base.contraints.encoding_constraint import EncodingConstraint
-from esmf_aspect_meta_model_python.impl.constraints.default_encoding_constraint import DefaultEncodingConstraint
+from esmf_aspect_meta_model_python.base.contraints.fixed_point_constraint import FixedPointConstraint
+from esmf_aspect_meta_model_python.impl.constraints.default_fixed_point_constraint import DefaultFixedPointConstraint
 from esmf_aspect_meta_model_python.loader.instantiator_base import InstantiatorBase
 from esmf_aspect_meta_model_python.loader.rdf_helper import RdfHelper
-from esmf_aspect_meta_model_python.vocabulary.SAMM import SAMM
+from esmf_aspect_meta_model_python.vocabulary.SAMMC import SAMMC
 
 
-class EncodingConstraintInstantiator(InstantiatorBase[EncodingConstraint]):
-    def _create_instance(self, element_node: Node) -> EncodingConstraint:
+class FixedPointConstraintInstantiator(InstantiatorBase[FixedPointConstraint]):
+    def _create_instance(self, element_node: Node) -> FixedPointConstraint:
         meta_model_base_attributes = self._get_base_attributes(element_node)
-        value = RdfHelper.to_python(
-            self._aspect_graph.value(subject=element_node, predicate=self._samm.get_urn(SAMM.value)),
+        scale = RdfHelper.to_python(
+            self._aspect_graph.value(subject=element_node, predicate=self._sammc.get_urn(SAMMC.scale)),
         )
-        value = value.split("#")[1]
-        return DefaultEncodingConstraint(meta_model_base_attributes, value)
+        integer = RdfHelper.to_python(
+            self._aspect_graph.value(subject=element_node, predicate=self._sammc.get_urn(SAMMC.integer)),
+        )
+        return DefaultFixedPointConstraint(meta_model_base_attributes, int(scale), int(integer))
```

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/entity_instantiator.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/entity_instantiator.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/enumeration_instantiator.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/enumeration_instantiator.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,36 +13,35 @@
 
 import rdflib  # type: ignore
 
 from rdflib.term import Node
 
 from esmf_aspect_meta_model_python.base.characteristics.enumeration import Enumeration
 from esmf_aspect_meta_model_python.impl.characteristics.default_enumeration import DefaultEnumeration
+from esmf_aspect_meta_model_python.loader.instantiator.constants import DATA_TYPE_ERROR_MSG
 from esmf_aspect_meta_model_python.loader.instantiator_base import InstantiatorBase
 from esmf_aspect_meta_model_python.loader.rdf_helper import RdfHelper
 from esmf_aspect_meta_model_python.vocabulary.SAMM import SAMM
 from esmf_aspect_meta_model_python.vocabulary.SAMMC import SAMMC
 
 
 class EnumerationInstantiator(InstantiatorBase[Enumeration]):
     def _create_instance(self, element_node: Node) -> Enumeration:
-        meta_model_base_attributes = self._get_base_attributes(element_node)
-
         data_type = self._get_data_type(element_node)
+        if data_type is None:
+            raise TypeError(DATA_TYPE_ERROR_MSG)
 
+        meta_model_base_attributes = self._get_base_attributes(element_node)
         value_collection_node = self._aspect_graph.value(
             subject=element_node,
             predicate=self._sammc.get_urn(SAMMC.values),
         )
         value_nodes = RdfHelper.get_rdf_list_values(value_collection_node, self._aspect_graph)
         values = [self.__to_enum_node_value(value_node) for value_node in value_nodes]
 
-        if data_type is None:
-            raise TypeError("Data type can't be None.")
-
         return DefaultEnumeration(meta_model_base_attributes, data_type, values)
 
     def __to_enum_node_value(self, value_node: Node) -> typing.Dict:
         """
         This method instantiates one possible value of an enumeration.
         :param value_node:  Node of the Graph that represents one enumeration value.
         The Argument can either be a Literal or a URIRef.
```

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/event_instantiator.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/code_instantiator.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,23 +5,24 @@
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 #
 #   SPDX-License-Identifier: MPL-2.0
 
-from typing import List
-
 from rdflib.term import Node
 
-from esmf_aspect_meta_model_python import Property
-from esmf_aspect_meta_model_python.base.event import Event
-from esmf_aspect_meta_model_python.impl.default_event import DefaultEvent
+from esmf_aspect_meta_model_python.base.characteristics.code import Code
+from esmf_aspect_meta_model_python.impl.characteristics.default_code import DefaultCode
+from esmf_aspect_meta_model_python.loader.instantiator.constants import DATA_TYPE_ERROR_MSG
 from esmf_aspect_meta_model_python.loader.instantiator_base import InstantiatorBase
-from esmf_aspect_meta_model_python.vocabulary.SAMM import SAMM
 
 
-class EventInstantiator(InstantiatorBase[Event]):
-    def _create_instance(self, element_node: Node) -> Event:
+class CodeInstantiator(InstantiatorBase[Code]):
+    def _create_instance(self, element_node: Node) -> Code:
+        data_type = self._get_data_type(element_node)
+        if not data_type:
+            raise TypeError(DATA_TYPE_ERROR_MSG)
+
         meta_model_base_attributes = self._get_base_attributes(element_node)
-        parameters: List[Property] = self._get_list_children(element_node, self._samm.get_urn(SAMM.parameters))
-        return DefaultEvent(meta_model_base_attributes, parameters)
+
+        return DefaultCode(meta_model_base_attributes, data_type)
```

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/fixed_point_constraint_instantiator.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/language_constraint_instantiator.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,24 +7,21 @@
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 #
 #   SPDX-License-Identifier: MPL-2.0
 
 from rdflib.term import Node
 
-from esmf_aspect_meta_model_python.base.contraints.fixed_point_constraint import FixedPointConstraint
-from esmf_aspect_meta_model_python.impl.constraints.default_fixed_point_constraint import DefaultFixedPointConstraint
+from esmf_aspect_meta_model_python.base.contraints.language_constraint import LanguageConstraint
+from esmf_aspect_meta_model_python.impl.constraints.default_language_constraint import DefaultLanguageConstraint
 from esmf_aspect_meta_model_python.loader.instantiator_base import InstantiatorBase
 from esmf_aspect_meta_model_python.loader.rdf_helper import RdfHelper
 from esmf_aspect_meta_model_python.vocabulary.SAMMC import SAMMC
 
 
-class FixedPointConstraintInstantiator(InstantiatorBase[FixedPointConstraint]):
-    def _create_instance(self, element_node: Node) -> FixedPointConstraint:
+class LanguageConstraintInstantiator(InstantiatorBase[LanguageConstraint]):
+    def _create_instance(self, element_node: Node) -> LanguageConstraint:
         meta_model_base_attributes = self._get_base_attributes(element_node)
-        scale = RdfHelper.to_python(
-            self._aspect_graph.value(subject=element_node, predicate=self._sammc.get_urn(SAMMC.scale)),
+        language_code = RdfHelper.to_python(
+            self._aspect_graph.value(subject=element_node, predicate=self._sammc.get_urn(SAMMC.language_code)),
         )
-        integer = RdfHelper.to_python(
-            self._aspect_graph.value(subject=element_node, predicate=self._sammc.get_urn(SAMMC.integer)),
-        )
-        return DefaultFixedPointConstraint(meta_model_base_attributes, int(scale), int(integer))
+        return DefaultLanguageConstraint(meta_model_base_attributes, language_code)
```

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/language_constraint_instantiator.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/length_constraint_instantiator.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,21 +7,24 @@
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 #
 #   SPDX-License-Identifier: MPL-2.0
 
 from rdflib.term import Node
 
-from esmf_aspect_meta_model_python.base.contraints.language_constraint import LanguageConstraint
-from esmf_aspect_meta_model_python.impl.constraints.default_language_constraint import DefaultLanguageConstraint
+from esmf_aspect_meta_model_python.base.contraints.length_constraint import LengthConstraint
+from esmf_aspect_meta_model_python.impl.constraints.default_length_constraint import DefaultLengthConstraint
 from esmf_aspect_meta_model_python.loader.instantiator_base import InstantiatorBase
 from esmf_aspect_meta_model_python.loader.rdf_helper import RdfHelper
 from esmf_aspect_meta_model_python.vocabulary.SAMMC import SAMMC
 
 
-class LanguageConstraintInstantiator(InstantiatorBase[LanguageConstraint]):
-    def _create_instance(self, element_node: Node) -> LanguageConstraint:
+class LengthConstraintInstantiator(InstantiatorBase[LengthConstraint]):
+    def _create_instance(self, element_node: Node) -> LengthConstraint:
         meta_model_base_attributes = self._get_base_attributes(element_node)
-        language_code = RdfHelper.to_python(
-            self._aspect_graph.value(subject=element_node, predicate=self._sammc.get_urn(SAMMC.language_code)),
+        min_value = RdfHelper.to_python(
+            self._aspect_graph.value(subject=element_node, predicate=self._sammc.get_urn(SAMMC.min_value)),
         )
-        return DefaultLanguageConstraint(meta_model_base_attributes, language_code)
+        max_value = RdfHelper.to_python(
+            self._aspect_graph.value(subject=element_node, predicate=self._sammc.get_urn(SAMMC.max_value)),
+        )
+        return DefaultLengthConstraint(meta_model_base_attributes, int(min_value), int(max_value))
```

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/length_constraint_instantiator.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/regular_expression_constraint_instantiator.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,24 +7,23 @@
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 #
 #   SPDX-License-Identifier: MPL-2.0
 
 from rdflib.term import Node
 
-from esmf_aspect_meta_model_python.base.contraints.length_constraint import LengthConstraint
-from esmf_aspect_meta_model_python.impl.constraints.default_length_constraint import DefaultLengthConstraint
+from esmf_aspect_meta_model_python.base.contraints.regular_expression_constraint import RegularExpressionConstraint
+from esmf_aspect_meta_model_python.impl.constraints.default_regular_expression_constraint import (
+    DefaultRegularExpressionConstraint,
+)
 from esmf_aspect_meta_model_python.loader.instantiator_base import InstantiatorBase
 from esmf_aspect_meta_model_python.loader.rdf_helper import RdfHelper
-from esmf_aspect_meta_model_python.vocabulary.SAMMC import SAMMC
+from esmf_aspect_meta_model_python.vocabulary.SAMM import SAMM
 
 
-class LengthConstraintInstantiator(InstantiatorBase[LengthConstraint]):
-    def _create_instance(self, element_node: Node) -> LengthConstraint:
+class RegularExpressionConstraintInstantiator(InstantiatorBase[RegularExpressionConstraint]):
+    def _create_instance(self, element_node: Node) -> RegularExpressionConstraint:
         meta_model_base_attributes = self._get_base_attributes(element_node)
-        min_value = RdfHelper.to_python(
-            self._aspect_graph.value(subject=element_node, predicate=self._sammc.get_urn(SAMMC.min_value)),
+        value = RdfHelper.to_python(
+            self._aspect_graph.value(subject=element_node, predicate=self._samm.get_urn(SAMM.value)),
         )
-        max_value = RdfHelper.to_python(
-            self._aspect_graph.value(subject=element_node, predicate=self._sammc.get_urn(SAMMC.max_value)),
-        )
-        return DefaultLengthConstraint(meta_model_base_attributes, int(min_value), int(max_value))
+        return DefaultRegularExpressionConstraint(meta_model_base_attributes, value)
```

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/list_instantiator.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/list_instantiator.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,21 +9,22 @@
 #
 #   SPDX-License-Identifier: MPL-2.0
 
 from rdflib.term import Node
 
 from esmf_aspect_meta_model_python.base.characteristics.collection.list import List
 from esmf_aspect_meta_model_python.impl.characteristics.collection.default_list import DefaultList
+from esmf_aspect_meta_model_python.loader.instantiator.constants import DATA_TYPE_ERROR_MSG
 from esmf_aspect_meta_model_python.loader.instantiator_base import InstantiatorBase
 from esmf_aspect_meta_model_python.vocabulary.SAMMC import SAMMC
 
 
 class ListInstantiator(InstantiatorBase[List]):
     def _create_instance(self, element_node: Node) -> List:
-        meta_model_base_attributes = self._get_base_attributes(element_node)
-        element_characteristic = self._get_child(element_node, self._sammc.get_urn(SAMMC.element_characteristic))
         data_type = self._get_data_type(element_node)
+        if not data_type:
+            raise TypeError(DATA_TYPE_ERROR_MSG)
 
-        if data_type is None:
-            raise TypeError("Data type can't be None.")
+        meta_model_base_attributes = self._get_base_attributes(element_node)
+        element_characteristic = self._get_child(element_node, self._sammc.get_urn(SAMMC.element_characteristic))
 
         return DefaultList(meta_model_base_attributes, data_type, element_characteristic)
```

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/locale_constraint_instantiator.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/locale_constraint_instantiator.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/measurement_instantiator.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/measurement_instantiator.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,22 +9,22 @@
 #
 #   SPDX-License-Identifier: MPL-2.0
 
 from rdflib.term import Node
 
 from esmf_aspect_meta_model_python.base.characteristics.quantifiable.measurement import Measurement
 from esmf_aspect_meta_model_python.impl.characteristics.quantifiable.default_measurement import DefaultMeasurement
+from esmf_aspect_meta_model_python.loader.instantiator.constants import DATA_TYPE_ERROR_MSG
 from esmf_aspect_meta_model_python.loader.instantiator_base import InstantiatorBase
 from esmf_aspect_meta_model_python.vocabulary.SAMMC import SAMMC
 
 
 class MeasurementInstantiator(InstantiatorBase[Measurement]):
     def _create_instance(self, element_node: Node) -> Measurement:
-        meta_model_base_attributes = self._get_base_attributes(element_node)
-
         data_type = self._get_data_type(element_node)
-        unit = self._get_child(element_node, self._sammc.get_urn(SAMMC.unit), required=True)
+        if not data_type:
+            raise TypeError(DATA_TYPE_ERROR_MSG)
 
-        if data_type is None:
-            raise TypeError("Data type can't be None.")
+        meta_model_base_attributes = self._get_base_attributes(element_node)
+        unit = self._get_child(element_node, self._sammc.get_urn(SAMMC.unit), required=True)
 
         return DefaultMeasurement(meta_model_base_attributes, data_type, unit)
```

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/operation_instantiator.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/operation_instantiator.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/property_instantiator.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/property_instantiator.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/quantifiable_instantiator.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/quantifiable_instantiator.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,21 +9,22 @@
 #
 #   SPDX-License-Identifier: MPL-2.0
 
 from rdflib.term import Node
 
 from esmf_aspect_meta_model_python.base.characteristics.quantifiable.quantifiable import Quantifiable
 from esmf_aspect_meta_model_python.impl.characteristics.quantifiable.default_quantifiable import DefaultQuantifiable
+from esmf_aspect_meta_model_python.loader.instantiator.constants import DATA_TYPE_ERROR_MSG
 from esmf_aspect_meta_model_python.loader.instantiator_base import InstantiatorBase
 from esmf_aspect_meta_model_python.vocabulary.SAMMC import SAMMC
 
 
 class QuantifiableInstantiator(InstantiatorBase[Quantifiable]):
     def _create_instance(self, element_node: Node) -> Quantifiable:
-        meta_model_base_attributes = self._get_base_attributes(element_node)
         data_type = self._get_data_type(element_node)
-        unit = self._get_child(element_node, self._sammc.get_urn(SAMMC.unit))
+        if not data_type:
+            raise TypeError(DATA_TYPE_ERROR_MSG)
 
-        if data_type is None:
-            raise TypeError("Data type can't be None.")
+        meta_model_base_attributes = self._get_base_attributes(element_node)
+        unit = self._get_child(element_node, self._sammc.get_urn(SAMMC.unit))
 
         return DefaultQuantifiable(meta_model_base_attributes, data_type, unit)
```

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/range_constraint_instantiator.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/range_constraint_instantiator.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/scalar_instantiator.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/scalar_instantiator.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/set_instantiator.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/sorted_set_instantiator.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,23 +7,24 @@
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 #
 #   SPDX-License-Identifier: MPL-2.0
 
 from rdflib.term import Node
 
-from esmf_aspect_meta_model_python.base.characteristics.collection.set import Set
-from esmf_aspect_meta_model_python.impl.characteristics.collection.default_set import DefaultSet
+from esmf_aspect_meta_model_python.base.characteristics.collection.sorted_set import SortedSet
+from esmf_aspect_meta_model_python.impl.characteristics.collection.default_sorted_set import DefaultSortedSet
+from esmf_aspect_meta_model_python.loader.instantiator.constants import DATA_TYPE_ERROR_MSG
 from esmf_aspect_meta_model_python.loader.instantiator_base import InstantiatorBase
 from esmf_aspect_meta_model_python.vocabulary.SAMMC import SAMMC
 
 
-class SetInstantiator(InstantiatorBase[Set]):
-    def _create_instance(self, element_node: Node) -> Set:
-        meta_model_base_attributes = self._get_base_attributes(element_node)
-        element_characteristic = self._get_child(element_node, self._sammc.get_urn(SAMMC.element_characteristic))
+class SortedSetInstantiator(InstantiatorBase[SortedSet]):
+    def _create_instance(self, element_node: Node) -> SortedSet:
         data_type = self._get_data_type(element_node)
+        if not data_type:
+            raise TypeError(DATA_TYPE_ERROR_MSG)
 
-        if data_type is None:
-            raise TypeError("Data type can't be None.")
+        meta_model_base_attributes = self._get_base_attributes(element_node)
+        element_characteristic = self._get_child(element_node, self._sammc.get_urn(SAMMC.element_characteristic))
 
-        return DefaultSet(meta_model_base_attributes, data_type, element_characteristic)
+        return DefaultSortedSet(meta_model_base_attributes, data_type, element_characteristic)
```

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/single_entity_instantiator.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/single_entity_instantiator.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,19 +9,20 @@
 #
 #   SPDX-License-Identifier: MPL-2.0
 
 from rdflib.term import Node
 
 from esmf_aspect_meta_model_python.base.characteristics.characteristic import Characteristic
 from esmf_aspect_meta_model_python.impl.characteristics.default_single_entity import DefaultSingleEntity
+from esmf_aspect_meta_model_python.loader.instantiator.constants import DATA_TYPE_ERROR_MSG
 from esmf_aspect_meta_model_python.loader.instantiator_base import InstantiatorBase
 
 
 class SingleEntityInstantiator(InstantiatorBase[Characteristic]):
     def _create_instance(self, element_node: Node) -> Characteristic:
-        meta_model_base_attributes = self._get_base_attributes(element_node)
         data_type = self._get_data_type(element_node)
+        if not data_type:
+            raise TypeError(DATA_TYPE_ERROR_MSG)
 
-        if data_type is None:
-            raise TypeError("Data type can't be None.")
+        meta_model_base_attributes = self._get_base_attributes(element_node)
 
         return DefaultSingleEntity(meta_model_base_attributes, data_type)
```

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/sorted_set_instantiator.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/set_instantiator.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,23 +7,24 @@
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 #
 #   SPDX-License-Identifier: MPL-2.0
 
 from rdflib.term import Node
 
-from esmf_aspect_meta_model_python.base.characteristics.collection.sorted_set import SortedSet
-from esmf_aspect_meta_model_python.impl.characteristics.collection.default_sorted_set import DefaultSortedSet
+from esmf_aspect_meta_model_python.base.characteristics.collection.set import Set
+from esmf_aspect_meta_model_python.impl.characteristics.collection.default_set import DefaultSet
+from esmf_aspect_meta_model_python.loader.instantiator.constants import DATA_TYPE_ERROR_MSG
 from esmf_aspect_meta_model_python.loader.instantiator_base import InstantiatorBase
 from esmf_aspect_meta_model_python.vocabulary.SAMMC import SAMMC
 
 
-class SortedSetInstantiator(InstantiatorBase[SortedSet]):
-    def _create_instance(self, element_node: Node) -> SortedSet:
-        meta_model_base_attributes = self._get_base_attributes(element_node)
-        element_characteristic = self._get_child(element_node, self._sammc.get_urn(SAMMC.element_characteristic))
+class SetInstantiator(InstantiatorBase[Set]):
+    def _create_instance(self, element_node: Node) -> Set:
         data_type = self._get_data_type(element_node)
+        if not data_type:
+            raise TypeError(DATA_TYPE_ERROR_MSG)
 
-        if data_type is None:
-            raise TypeError("Data type can't be None.")
+        meta_model_base_attributes = self._get_base_attributes(element_node)
+        element_characteristic = self._get_child(element_node, self._sammc.get_urn(SAMMC.element_characteristic))
 
-        return DefaultSortedSet(meta_model_base_attributes, data_type, element_characteristic)
+        return DefaultSet(meta_model_base_attributes, data_type, element_characteristic)
```

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/structured_value_instantiator.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/structured_value_instantiator.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,38 +12,37 @@
 from typing import Any
 
 from rdflib import Literal
 from rdflib.term import Node
 
 from esmf_aspect_meta_model_python.base.characteristics.structured_value import StructuredValue
 from esmf_aspect_meta_model_python.impl.characteristics.default_structured_value import DefaultStructuredValue
+from esmf_aspect_meta_model_python.loader.instantiator.constants import DATA_TYPE_ERROR_MSG
 from esmf_aspect_meta_model_python.loader.instantiator_base import InstantiatorBase
 from esmf_aspect_meta_model_python.loader.rdf_helper import RdfHelper
 from esmf_aspect_meta_model_python.vocabulary.SAMMC import SAMMC
 
 
 class StructuredValueInstantiator(InstantiatorBase[StructuredValue]):
     def _create_instance(self, element_node: Node) -> StructuredValue:
-        meta_model_base_attributes = self._get_base_attributes(element_node)
         data_type = self._get_data_type(element_node)
+        if not data_type:
+            raise TypeError(DATA_TYPE_ERROR_MSG)
 
+        meta_model_base_attributes = self._get_base_attributes(element_node)
         deconstruction_rule = RdfHelper.to_python(
             self._aspect_graph.value(
                 subject=element_node,
                 predicate=self._sammc.get_urn(SAMMC.deconstruction_rule),
             )
         )
-
         element_nodes = self._aspect_graph.value(subject=element_node, predicate=self._sammc.get_urn(SAMMC.elements))
         element_node_list = RdfHelper.get_rdf_list_values(element_nodes, self._aspect_graph)
         elements = [self.__to_element_node_value(element_node) for element_node in element_node_list]
 
-        if data_type is None:
-            raise TypeError("Data type can't be None.")
-
         return DefaultStructuredValue(meta_model_base_attributes, data_type, deconstruction_rule, elements)
 
     def __to_element_node_value(self, element_node: Node) -> Any:
         """creates a property that is wrapped in a structured value"""
         if isinstance(element_node, Literal):
             return element_node.toPython()
         return self._model_element_factory.create_element(element_node)
```

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/time_series_instantiator.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/time_series_instantiator.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,21 +9,22 @@
 #
 #   SPDX-License-Identifier: MPL-2.0
 
 from rdflib.term import Node
 
 from esmf_aspect_meta_model_python.base.characteristics.collection.time_series import TimeSeries
 from esmf_aspect_meta_model_python.impl.characteristics.collection.default_time_series import DefaultTimeSeries
+from esmf_aspect_meta_model_python.loader.instantiator.constants import DATA_TYPE_ERROR_MSG
 from esmf_aspect_meta_model_python.loader.instantiator_base import InstantiatorBase
 from esmf_aspect_meta_model_python.vocabulary.SAMMC import SAMMC
 
 
 class TimeSeriesInstantiator(InstantiatorBase[TimeSeries]):
     def _create_instance(self, element_node: Node) -> TimeSeries:
-        meta_model_base_attributes = self._get_base_attributes(element_node)
-        element_characteristic = self._get_child(element_node, self._sammc.get_urn(SAMMC.element_characteristic))
         data_type = self._get_data_type(element_node)
+        if not data_type:
+            raise TypeError(DATA_TYPE_ERROR_MSG)
 
-        if data_type is None:
-            raise ValueError("Data type can't be none in TimeSeries.")
+        meta_model_base_attributes = self._get_base_attributes(element_node)
+        element_characteristic = self._get_child(element_node, self._sammc.get_urn(SAMMC.element_characteristic))
 
         return DefaultTimeSeries(meta_model_base_attributes, data_type, element_characteristic)
```

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/trait_instantiator.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/trait_instantiator.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator/unit_instantiator.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator/unit_instantiator.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/instantiator_base.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/instantiator_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,24 +166,26 @@
         Returns:
             Data type object or none
         """
         element_characteristic_node = self._aspect_graph.value(
             subject=element_node,
             predicate=self._sammc.get_urn(SAMMC.element_characteristic),
         )
-        if element_characteristic_node is None:
-            data_type_node = self._aspect_graph.value(
-                subject=element_node,
-                predicate=self._samm.get_urn(SAMM.data_type),
-            )
-        else:
+        if element_characteristic_node:
             # some characteristics (Collection, List, TimeSeries, etc.) may have
             # an attribute "element_characteristic". If it is given, then take
             # the data type of the element_characteristic.
             data_type_node = self._aspect_graph.value(
                 subject=element_characteristic_node,
                 predicate=self._samm.get_urn(SAMM.data_type),
             )
-        if data_type_node is None:
-            return None
         else:
+            data_type_node = self._aspect_graph.value(
+                subject=element_node,
+                predicate=self._samm.get_urn(SAMM.data_type),
+            )
+
+        data_type_element = None
+        if data_type_node:
             return self._model_element_factory.create_element(data_type_node)
+
+        return data_type_element
```

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/meta_model_base_attributes.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/meta_model_base_attributes.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/model_element_factory.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/model_element_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,16 @@
             element_node: node in the aspect graph that represents the
             needed element
 
         Returns:
             an instance of a the element with all the child attributes
         """
         element_type = self._get_element_type(element_node)
-        if self._instantiators.keys().__contains__(element_type):
+
+        if element_type in self._instantiators:
             instance = self._instantiators[element_type].get_instance(element_node)
         else:
             instance = self._create_instantiator(element_type).get_instance(element_node)
 
         if isinstance(instance, Base):
             self._cache.resolve_instance(instance)
```

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/rdf_helper.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/rdf_helper.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/loader/README.md` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/loader/README.md`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/resolver/aspect_meta_model_resolver.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/resolver/aspect_meta_model_resolver.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/resolver/README.md` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/resolver/README.md`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/download_samm_branch.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/download_samm_branch.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/download_samm_release.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/download_samm_release.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/github_file.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/github_file.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/github_folder.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/github_folder.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/characteristic/1.0.0/characteristic-definitions.ttl` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/characteristic/1.0.0/characteristic-definitions.ttl`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/characteristic/1.0.0/characteristic-instances.ttl` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/characteristic/1.0.0/characteristic-instances.ttl`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/characteristic/1.0.0/characteristic-shapes.ttl` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/characteristic/1.0.0/characteristic-shapes.ttl`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/characteristic/1.0.0/characteristic-validations.js` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/characteristic/1.0.0/characteristic-validations.js`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/characteristic/2.0.0/characteristic-definitions.ttl` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/characteristic/2.0.0/characteristic-definitions.ttl`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/characteristic/2.0.0/characteristic-instances.ttl` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/characteristic/2.0.0/characteristic-instances.ttl`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/characteristic/2.0.0/characteristic-shapes.ttl` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/characteristic/2.0.0/characteristic-shapes.ttl`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/characteristic/2.0.0/characteristic-validations.js` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/characteristic/2.0.0/characteristic-validations.js`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/characteristic/2.1.0/characteristic-definitions.ttl` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/characteristic/2.1.0/characteristic-definitions.ttl`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/characteristic/2.1.0/characteristic-instances.ttl` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/characteristic/2.1.0/characteristic-instances.ttl`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/characteristic/2.1.0/characteristic-shapes.ttl` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/characteristic/2.1.0/characteristic-shapes.ttl`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/characteristic/2.1.0/characteristic-validations.js` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/characteristic/2.1.0/characteristic-validations.js`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/entity/1.0.0/FileResource.ttl` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/entity/1.0.0/FileResource.ttl`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/entity/1.0.0/Point3d.ttl` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/entity/1.0.0/Point3d.ttl`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/entity/1.0.0/TimeSeriesEntity.ttl` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/entity/1.0.0/TimeSeriesEntity.ttl`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/entity/2.0.0/FileResource.ttl` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/entity/2.0.0/FileResource.ttl`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/entity/2.0.0/Point3d.ttl` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/entity/2.0.0/Point3d.ttl`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/entity/2.0.0/TimeSeriesEntity.ttl` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/entity/2.0.0/TimeSeriesEntity.ttl`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/entity/2.1.0/FileResource.ttl` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/entity/2.1.0/FileResource.ttl`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/entity/2.1.0/Point3d.ttl` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/entity/2.1.0/Point3d.ttl`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/entity/2.1.0/TimeSeriesEntity.ttl` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/entity/2.1.0/TimeSeriesEntity.ttl`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/meta-model/1.0.0/aspect-meta-model-definitions.ttl` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/meta-model/1.0.0/aspect-meta-model-definitions.ttl`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/meta-model/1.0.0/aspect-meta-model-shapes.ttl` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/meta-model/1.0.0/aspect-meta-model-shapes.ttl`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/meta-model/1.0.0/prefix-declarations.ttl` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/meta-model/1.0.0/prefix-declarations.ttl`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/meta-model/1.0.0/type-conversions.ttl` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/meta-model/1.0.0/type-conversions.ttl`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/meta-model/2.0.0/aspect-meta-model-definitions.ttl` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/meta-model/2.0.0/aspect-meta-model-definitions.ttl`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/meta-model/2.0.0/aspect-meta-model-shapes.ttl` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/meta-model/2.0.0/aspect-meta-model-shapes.ttl`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/meta-model/2.0.0/prefix-declarations.ttl` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/meta-model/2.0.0/prefix-declarations.ttl`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/meta-model/2.0.0/type-conversions.ttl` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/meta-model/2.0.0/type-conversions.ttl`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/meta-model/2.1.0/aspect-meta-model-definitions.ttl` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/meta-model/2.1.0/aspect-meta-model-definitions.ttl`

 * *Files 0% similar despite different names*

```diff
@@ -234,11 +234,10 @@
 samm:UTF-16 a mmm:Constant .
 
 samm:UTF-16BE a mmm:Constant .
 
 samm:UTF-16LE a mmm:Constant .
 
 # Datatypes
-# can be represent as string or Curie class
 samm:curie a rdfs:Datatype ;
    rdfs:comment "The ·lexical space· of curie is finite-length character sequences which represent a valid curie as defined here https://www.w3.org/TR/2010/NOTE-curie-20101216/#s_schema.";
    rdfs:label "curie" .
```

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/meta-model/2.1.0/aspect-meta-model-shapes.ttl` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/meta-model/2.1.0/aspect-meta-model-shapes.ttl`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/meta-model/2.1.0/prefix-declarations.ttl` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/meta-model/2.1.0/prefix-declarations.ttl`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/meta-model/2.1.0/type-conversions.ttl` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/meta-model/2.1.0/type-conversions.ttl`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/scripts/language-registry.js` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/scripts/language-registry.js`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/unit/1.0.0/units.ttl` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/unit/1.0.0/units.ttl`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/unit/2.0.0/units.ttl` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/unit/2.0.0/units.ttl`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/unit/2.1.0/units.ttl` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/unit/2.1.0/units.ttl`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/vocabulary/namespace.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/vocabulary/namespace.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/vocabulary/SAMM.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/vocabulary/SAMM.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/vocabulary/SAMMC.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/vocabulary/SAMMC.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/vocabulary/SAMME.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/vocabulary/SAMME.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/esmf_aspect_meta_model_python/vocabulary/UNIT.py` & `test_esmf_loader-0.0.2/esmf_aspect_meta_model_python/vocabulary/UNIT.py`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/pyproject.toml` & `test_esmf_loader-0.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 [tool.poetry]
+#name = "esmf-aspect-model-loader"
+#version = "2.1.1"
 name = "test-esmf-loader"
-version = "0.0.1"
+version = "0.0.2"
 description = "Load Aspect Models based on the Semantic Aspect Meta Model"
-authors = ["Hanna Shalamitskaya <external.Hanna.Shalamitskaya@de.bosch.com>"]
-packages = [{include = "esmf_aspect_meta_model_python"}]
-include = [
-    "esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/**/*",
-#    "samm.exe",
+authors = [
+#    "Eclipse Semantic Modeling Framework",
+    "Hanna Shalamitskaya <external.Hanna.Shalamitskaya@de.bosch.com>",
+#    "Andreas Textor <Andreas.Textor@de.bosch.com> ",
+#    "Georg Schmidt-Dumont <Georg.Schmidt-Dumont@de.bosch.com>",
+#    "Nico Makowe",
+#    "Aghyad Farrouh",
 ]
+packages = [{include = "esmf_aspect_meta_model_python"}]
+include = ["esmf_aspect_meta_model_python/samm_aspect_meta_model/samm/**/*"]
 license = "MPL-2.0"
 classifiers = [
     "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.10",
 ]
 readme = "README.md"
@@ -41,11 +47,12 @@
 
 [tool.pytest.ini_options]
 cache_dir = ".pytest_cache"
 
 [tool.poetry.scripts]
 download-samm-release = "esmf_aspect_meta_model_python.samm_aspect_meta_model.download_samm_release:main"
 download-samm-branch = "esmf_aspect_meta_model_python.samm_aspect_meta_model.download_samm_branch:main"
+download-samm-cli = "scripts.download_samm_cli:download_samm_cli"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `test_esmf_loader-0.0.1/README.md` & `test_esmf_loader-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `test_esmf_loader-0.0.1/PKG-INFO` & `test_esmf_loader-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test-esmf-loader
-Version: 0.0.1
+Version: 0.0.2
 Summary: Load Aspect Models based on the Semantic Aspect Meta Model
 Home-page: https://projects.eclipse.org/projects/dt.esmf
 License: MPL-2.0
 Keywords: samm,esmf,digital twin,idta,model loader,semantic api,semantics,aspect
 Author: Hanna Shalamitskaya
 Author-email: external.Hanna.Shalamitskaya@de.bosch.com
 Requires-Python: >=3.10,<4.0
```

