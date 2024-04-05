# Comparing `tmp/cml-pam-0.3.1.tar.gz` & `tmp/cml-pam-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cml-pam-0.3.1.tar", last modified: Tue Nov  7 17:24:18 2023, max compression
+gzip compressed data, was "cml-pam-0.3.2.tar", last modified: Fri Apr  5 18:53:36 2024, max compression
```

## Comparing `cml-pam-0.3.1.tar` & `cml-pam-0.3.2.tar`

### file list

```diff
@@ -1,142 +1,144 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 17:24:18.710449 cml-pam-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2023-11-07 17:24:08.000000 cml-pam-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7836 2023-11-07 17:24:18.710449 cml-pam-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5769 2023-11-07 17:24:08.000000 cml-pam-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 17:24:18.694449 cml-pam-0.3.1/cml_pam.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7836 2023-11-07 17:24:18.000000 cml-pam-0.3.1/cml_pam.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3291 2023-11-07 17:24:18.000000 cml-pam-0.3.1/cml_pam.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-07 17:24:18.000000 cml-pam-0.3.1/cml_pam.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-11-07 17:24:18.000000 cml-pam-0.3.1/cml_pam.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      456 2023-11-07 17:24:18.000000 cml-pam-0.3.1/cml_pam.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2023-11-07 17:24:18.000000 cml-pam-0.3.1/cml_pam.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 17:24:18.698449 cml-pam-0.3.1/pam/
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2023-11-07 17:24:08.000000 cml-pam-0.3.1/pam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    47167 2023-11-07 17:24:08.000000 cml-pam-0.3.1/pam/activity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 17:24:18.698449 cml-pam-0.3.1/pam/array/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-07 17:24:08.000000 cml-pam-0.3.1/pam/array/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5034 2023-11-07 17:24:08.000000 cml-pam-0.3.1/pam/array/decode.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2023-11-07 17:24:08.000000 cml-pam-0.3.1/pam/array/distance.py
--rw-r--r--   0 runner    (1001) docker     (127)     4086 2023-11-07 17:24:08.000000 cml-pam-0.3.1/pam/array/encode.py
--rw-r--r--   0 runner    (1001) docker     (127)    23872 2023-11-07 17:24:08.000000 cml-pam-0.3.1/pam/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    49406 2023-11-07 17:24:08.000000 cml-pam-0.3.1/pam/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 17:24:18.694449 cml-pam-0.3.1/pam/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 17:24:18.698449 cml-pam-0.3.1/pam/fixtures/dtd/
--rw-r--r--   0 runner    (1001) docker     (127)      754 2023-11-07 17:24:08.000000 cml-pam-0.3.1/pam/fixtures/dtd/electric_vehicles_v1.dtd
--rw-r--r--   0 runner    (1001) docker     (127)      351 2023-11-07 17:24:08.000000 cml-pam-0.3.1/pam/fixtures/dtd/objectattributes_v1.dtd
--rw-r--r--   0 runner    (1001) docker     (127)     7084 2023-11-07 17:24:08.000000 cml-pam-0.3.1/pam/fixtures/dtd/population_v5.dtd
--rw-r--r--   0 runner    (1001) docker     (127)     6885 2023-11-07 17:24:08.000000 cml-pam-0.3.1/pam/fixtures/dtd/population_v6.dtd
--rw-r--r--   0 runner    (1001) docker     (127)     6334 2023-11-07 17:24:08.000000 cml-pam-0.3.1/pam/fixtures/dtd/vehicleDefinitions_v2.0.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2023-11-07 17:24:08.000000 cml-pam-0.3.1/pam/location.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 17:24:18.698449 cml-pam-0.3.1/pam/operations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-07 17:24:08.000000 cml-pam-0.3.1/pam/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2023-11-07 17:24:08.000000 cml-pam-0.3.1/pam/operations/combine.py
--rw-r--r--   0 runner    (1001) docker     (127)     7517 2023-11-07 17:24:08.000000 cml-pam-0.3.1/pam/operations/cropping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 17:24:18.698449 cml-pam-0.3.1/pam/optimise/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-07 17:24:08.000000 cml-pam-0.3.1/pam/optimise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3804 2023-11-07 17:24:08.000000 cml-pam-0.3.1/pam/optimise/grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3712 2023-11-07 17:24:08.000000 cml-pam-0.3.1/pam/optimise/random.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 17:24:18.698449 cml-pam-0.3.1/pam/planner/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-07 17:24:08.000000 cml-pam-0.3.1/pam/planner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17808 2023-11-07 17:24:08.000000 cml-pam-0.3.1/pam/planner/choice_location.py
--rw-r--r--   0 runner    (1001) docker     (127)     5961 2023-11-07 17:24:08.000000 cml-pam-0.3.1/pam/planner/clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)     5248 2023-11-07 17:24:08.000000 cml-pam-0.3.1/pam/planner/encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     9227 2023-11-07 17:24:08.000000 cml-pam-0.3.1/pam/planner/ipf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4975 2023-11-07 17:24:08.000000 cml-pam-0.3.1/pam/planner/od.py
--rw-r--r--   0 runner    (1001) docker     (127)     5549 2023-11-07 17:24:08.000000 cml-pam-0.3.1/pam/planner/utils_planner.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2023-11-07 17:24:08.000000 cml-pam-0.3.1/pam/planner/zones.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 17:24:18.698449 cml-pam-0.3.1/pam/plot/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2023-11-07 17:24:08.000000 cml-pam-0.3.1/pam/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17713 2023-11-07 17:24:08.000000 cml-pam-0.3.1/pam/plot/plans.py
--rw-r--r--   0 runner    (1001) docker     (127)     9344 2023-11-07 17:24:08.000000 cml-pam-0.3.1/pam/plot/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 17:24:18.702449 cml-pam-0.3.1/pam/policy/
--rw-r--r--   0 runner    (1001) docker     (127)      757 2023-11-07 17:24:08.000000 cml-pam-0.3.1/pam/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3345 2023-11-07 17:24:08.000000 cml-pam-0.3.1/pam/policy/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)    12245 2023-11-07 17:24:08.000000 cml-pam-0.3.1/pam/policy/modifiers.py
--rw-r--r--   0 runner    (1001) docker     (127)    18186 2023-11-07 17:24:08.000000 cml-pam-0.3.1/pam/policy/policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     8441 2023-11-07 17:24:08.000000 cml-pam-0.3.1/pam/policy/probability_samplers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 17:24:18.702449 cml-pam-0.3.1/pam/read/
--rw-r--r--   0 runner    (1001) docker     (127)      792 2023-11-07 17:24:08.000000 cml-pam-0.3.1/pam/read/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32486 2023-11-07 17:24:08.000000 cml-pam-0.3.1/pam/read/diary.py
--rw-r--r--   0 runner    (1001) docker     (127)    18294 2023-11-07 17:24:08.000000 cml-pam-0.3.1/pam/read/matsim.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 17:24:18.702449 cml-pam-0.3.1/pam/report/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-07 17:24:08.000000 cml-pam-0.3.1/pam/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6858 2023-11-07 17:24:08.000000 cml-pam-0.3.1/pam/report/benchmarks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2023-11-07 17:24:08.000000 cml-pam-0.3.1/pam/report/stringify.py
--rw-r--r--   0 runner    (1001) docker     (127)     6223 2023-11-07 17:24:08.000000 cml-pam-0.3.1/pam/report/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 17:24:18.702449 cml-pam-0.3.1/pam/samplers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-07 17:24:08.000000 cml-pam-0.3.1/pam/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2023-11-07 17:24:08.000000 cml-pam-0.3.1/pam/samplers/attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2023-11-07 17:24:08.000000 cml-pam-0.3.1/pam/samplers/basic.py
--rw-r--r--   0 runner    (1001) docker     (127)    18182 2023-11-07 17:24:08.000000 cml-pam-0.3.1/pam/samplers/facility.py
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2023-11-07 17:24:08.000000 cml-pam-0.3.1/pam/samplers/population.py
--rw-r--r--   0 runner    (1001) docker     (127)     7535 2023-11-07 17:24:08.000000 cml-pam-0.3.1/pam/samplers/spatial.py
--rw-r--r--   0 runner    (1001) docker     (127)     2584 2023-11-07 17:24:08.000000 cml-pam-0.3.1/pam/samplers/time.py
--rw-r--r--   0 runner    (1001) docker     (127)    29913 2023-11-07 17:24:08.000000 cml-pam-0.3.1/pam/samplers/tour.py
--rw-r--r--   0 runner    (1001) docker     (127)    14370 2023-11-07 17:24:08.000000 cml-pam-0.3.1/pam/scoring.py
--rw-r--r--   0 runner    (1001) docker     (127)    10938 2023-11-07 17:24:08.000000 cml-pam-0.3.1/pam/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2023-11-07 17:24:08.000000 cml-pam-0.3.1/pam/variables.py
--rw-r--r--   0 runner    (1001) docker     (127)    15713 2023-11-07 17:24:08.000000 cml-pam-0.3.1/pam/vehicles.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 17:24:18.702449 cml-pam-0.3.1/pam/write/
--rw-r--r--   0 runner    (1001) docker     (127)      344 2023-11-07 17:24:08.000000 cml-pam-0.3.1/pam/write/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7293 2023-11-07 17:24:08.000000 cml-pam-0.3.1/pam/write/diary.py
--rw-r--r--   0 runner    (1001) docker     (127)     4419 2023-11-07 17:24:08.000000 cml-pam-0.3.1/pam/write/matrices.py
--rw-r--r--   0 runner    (1001) docker     (127)    11496 2023-11-07 17:24:08.000000 cml-pam-0.3.1/pam/write/matsim.py
--rw-r--r--   0 runner    (1001) docker     (127)     4010 2023-11-07 17:24:08.000000 cml-pam-0.3.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 17:24:18.702449 cml-pam-0.3.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      335 2023-11-07 17:24:08.000000 cml-pam-0.3.1/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (127)      200 2023-11-07 17:24:08.000000 cml-pam-0.3.1/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-07 17:24:18.710449 cml-pam-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 17:24:18.710449 cml-pam-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    14068 2023-11-07 17:24:08.000000 cml-pam-0.3.1/tests/test_00_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    19372 2023-11-07 17:24:08.000000 cml-pam-0.3.1/tests/test_01_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    17496 2023-11-07 17:24:08.000000 cml-pam-0.3.1/tests/test_01_core_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2608 2023-11-07 17:24:08.000000 cml-pam-0.3.1/tests/test_01_core_sample_locs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2023-11-07 17:24:08.000000 cml-pam-0.3.1/tests/test_02_activity.py
--rw-r--r--   0 runner    (1001) docker     (127)     4326 2023-11-07 17:24:08.000000 cml-pam-0.3.1/tests/test_02_activity_components.py
--rw-r--r--   0 runner    (1001) docker     (127)     8011 2023-11-07 17:24:08.000000 cml-pam-0.3.1/tests/test_02_activity_fix.py
--rw-r--r--   0 runner    (1001) docker     (127)    22998 2023-11-07 17:24:08.000000 cml-pam-0.3.1/tests/test_02_activity_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)    10542 2023-11-07 17:24:08.000000 cml-pam-0.3.1/tests/test_02_activity_trips.py
--rw-r--r--   0 runner    (1001) docker     (127)     6331 2023-11-07 17:24:08.000000 cml-pam-0.3.1/tests/test_02_activity_validate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5360 2023-11-07 17:24:08.000000 cml-pam-0.3.1/tests/test_03_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     2034 2023-11-07 17:24:08.000000 cml-pam-0.3.1/tests/test_03_read_activity_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     5763 2023-11-07 17:24:08.000000 cml-pam-0.3.1/tests/test_03_read_challenge.py
--rw-r--r--   0 runner    (1001) docker     (127)     7925 2023-11-07 17:24:08.000000 cml-pam-0.3.1/tests/test_03_read_matsim.py
--rw-r--r--   0 runner    (1001) docker     (127)    13223 2023-11-07 17:24:08.000000 cml-pam-0.3.1/tests/test_03_read_travel_diary.py
--rw-r--r--   0 runner    (1001) docker     (127)     3629 2023-11-07 17:24:08.000000 cml-pam-0.3.1/tests/test_04_household_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     3455 2023-11-07 17:24:08.000000 cml-pam-0.3.1/tests/test_05_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      372 2023-11-07 17:24:08.000000 cml-pam-0.3.1/tests/test_05_modifiers.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2023-11-07 17:24:08.000000 cml-pam-0.3.1/tests/test_05_modifiers_AddActivity.py
--rw-r--r--   0 runner    (1001) docker     (127)     7369 2023-11-07 17:24:08.000000 cml-pam-0.3.1/tests/test_05_modifiers_MoveActivity.py
--rw-r--r--   0 runner    (1001) docker     (127)    12797 2023-11-07 17:24:08.000000 cml-pam-0.3.1/tests/test_05_modifiers_ReduceSharedActivity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2023-11-07 17:24:08.000000 cml-pam-0.3.1/tests/test_05_modifiers_RemoveActivity.py
--rw-r--r--   0 runner    (1001) docker     (127)    41607 2023-11-07 17:24:08.000000 cml-pam-0.3.1/tests/test_05_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2023-11-07 17:24:08.000000 cml-pam-0.3.1/tests/test_05_policies_prebaked.py
--rw-r--r--   0 runner    (1001) docker     (127)     9549 2023-11-07 17:24:08.000000 cml-pam-0.3.1/tests/test_05_policy_levels.py
--rw-r--r--   0 runner    (1001) docker     (127)    11728 2023-11-07 17:24:08.000000 cml-pam-0.3.1/tests/test_05_probability_samplers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2023-11-07 17:24:08.000000 cml-pam-0.3.1/tests/test_06_activity_remove_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2979 2023-11-07 17:24:08.000000 cml-pam-0.3.1/tests/test_07_activity_fill_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)    27592 2023-11-07 17:24:08.000000 cml-pam-0.3.1/tests/test_08_write.py
--rw-r--r--   0 runner    (1001) docker     (127)    21808 2023-11-07 17:24:08.000000 cml-pam-0.3.1/tests/test_09_samplers.py
--rw-r--r--   0 runner    (1001) docker     (127)    15609 2023-11-07 17:24:08.000000 cml-pam-0.3.1/tests/test_09_samplers_tour.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2023-11-07 17:24:08.000000 cml-pam-0.3.1/tests/test_100_memory_profiling.py
--rw-r--r--   0 runner    (1001) docker     (127)     8400 2023-11-07 17:24:08.000000 cml-pam-0.3.1/tests/test_10_plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2023-11-07 17:24:08.000000 cml-pam-0.3.1/tests/test_11_population_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2023-11-07 17:24:08.000000 cml-pam-0.3.1/tests/test_11_spatial_sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     5083 2023-11-07 17:24:08.000000 cml-pam-0.3.1/tests/test_12_scoring.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2023-11-07 17:24:08.000000 cml-pam-0.3.1/tests/test_13_sample_time.py
--rw-r--r--   0 runner    (1001) docker     (127)    12157 2023-11-07 17:24:08.000000 cml-pam-0.3.1/tests/test_14_encode_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     6179 2023-11-07 17:24:08.000000 cml-pam-0.3.1/tests/test_15_cropping.py
--rw-r--r--   0 runner    (1001) docker     (127)    19013 2023-11-07 17:24:08.000000 cml-pam-0.3.1/tests/test_17_vehicles.py
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2023-11-07 17:24:08.000000 cml-pam-0.3.1/tests/test_18_reporting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2023-11-07 17:24:08.000000 cml-pam-0.3.1/tests/test_18_reporting_bms.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2023-11-07 17:24:08.000000 cml-pam-0.3.1/tests/test_19_combining.py
--rw-r--r--   0 runner    (1001) docker     (127)     3887 2023-11-07 17:24:08.000000 cml-pam-0.3.1/tests/test_20_planner_clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2023-11-07 17:24:08.000000 cml-pam-0.3.1/tests/test_21_planner_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2734 2023-11-07 17:24:08.000000 cml-pam-0.3.1/tests/test_22_planner_od.py
--rw-r--r--   0 runner    (1001) docker     (127)      298 2023-11-07 17:24:08.000000 cml-pam-0.3.1/tests/test_23_planner_zones.py
--rw-r--r--   0 runner    (1001) docker     (127)     7233 2023-11-07 17:24:08.000000 cml-pam-0.3.1/tests/test_24_planner_choice_location.py
--rw-r--r--   0 runner    (1001) docker     (127)     2920 2023-11-07 17:24:08.000000 cml-pam-0.3.1/tests/test_25_planner_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2023-11-07 17:24:08.000000 cml-pam-0.3.1/tests/test_26_optimise_grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3508 2023-11-07 17:24:08.000000 cml-pam-0.3.1/tests/test_27_optimise_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     3315 2023-11-07 17:24:08.000000 cml-pam-0.3.1/tests/test_28_planner_ipf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5482 2023-11-07 17:24:08.000000 cml-pam-0.3.1/tests/test_99_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:53:36.001021 cml-pam-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-05 18:53:27.000000 cml-pam-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8167 2024-04-05 18:53:36.001021 cml-pam-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5984 2024-04-05 18:53:27.000000 cml-pam-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-04-05 18:53:27.000000 cml-pam-0.3.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:53:35.977021 cml-pam-0.3.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-05 18:53:27.000000 cml-pam-0.3.2/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-05 18:53:27.000000 cml-pam-0.3.2/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 18:53:36.001021 cml-pam-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:53:35.977021 cml-pam-0.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:53:35.997021 cml-pam-0.3.2/src/cml_pam.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8167 2024-04-05 18:53:35.000000 cml-pam-0.3.2/src/cml_pam.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-04-05 18:53:35.000000 cml-pam-0.3.2/src/cml_pam.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 18:53:35.000000 cml-pam-0.3.2/src/cml_pam.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-05 18:53:35.000000 cml-pam-0.3.2/src/cml_pam.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-05 18:53:35.000000 cml-pam-0.3.2/src/cml_pam.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-05 18:53:35.000000 cml-pam-0.3.2/src/cml_pam.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:53:35.981021 cml-pam-0.3.2/src/pam/
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-05 18:53:27.000000 cml-pam-0.3.2/src/pam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47167 2024-04-05 18:53:27.000000 cml-pam-0.3.2/src/pam/activity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:53:35.981021 cml-pam-0.3.2/src/pam/array/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 18:53:27.000000 cml-pam-0.3.2/src/pam/array/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5034 2024-04-05 18:53:27.000000 cml-pam-0.3.2/src/pam/array/decode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-05 18:53:27.000000 cml-pam-0.3.2/src/pam/array/distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-04-05 18:53:27.000000 cml-pam-0.3.2/src/pam/array/encode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23872 2024-04-05 18:53:27.000000 cml-pam-0.3.2/src/pam/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49406 2024-04-05 18:53:27.000000 cml-pam-0.3.2/src/pam/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:53:35.977021 cml-pam-0.3.2/src/pam/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:53:35.981021 cml-pam-0.3.2/src/pam/fixtures/dtd/
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-05 18:53:27.000000 cml-pam-0.3.2/src/pam/fixtures/dtd/electric_vehicles_v1.dtd
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-05 18:53:27.000000 cml-pam-0.3.2/src/pam/fixtures/dtd/objectattributes_v1.dtd
+-rw-r--r--   0 runner    (1001) docker     (127)     7084 2024-04-05 18:53:27.000000 cml-pam-0.3.2/src/pam/fixtures/dtd/population_v5.dtd
+-rw-r--r--   0 runner    (1001) docker     (127)     6885 2024-04-05 18:53:27.000000 cml-pam-0.3.2/src/pam/fixtures/dtd/population_v6.dtd
+-rw-r--r--   0 runner    (1001) docker     (127)     6334 2024-04-05 18:53:27.000000 cml-pam-0.3.2/src/pam/fixtures/dtd/vehicleDefinitions_v2.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-05 18:53:27.000000 cml-pam-0.3.2/src/pam/location.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:53:35.981021 cml-pam-0.3.2/src/pam/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 18:53:27.000000 cml-pam-0.3.2/src/pam/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-05 18:53:27.000000 cml-pam-0.3.2/src/pam/operations/combine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7518 2024-04-05 18:53:27.000000 cml-pam-0.3.2/src/pam/operations/cropping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:53:35.985021 cml-pam-0.3.2/src/pam/optimise/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 18:53:27.000000 cml-pam-0.3.2/src/pam/optimise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-04-05 18:53:27.000000 cml-pam-0.3.2/src/pam/optimise/grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3712 2024-04-05 18:53:27.000000 cml-pam-0.3.2/src/pam/optimise/random.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:53:35.985021 cml-pam-0.3.2/src/pam/planner/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 18:53:27.000000 cml-pam-0.3.2/src/pam/planner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17809 2024-04-05 18:53:27.000000 cml-pam-0.3.2/src/pam/planner/choice_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-04-05 18:53:27.000000 cml-pam-0.3.2/src/pam/planner/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-04-05 18:53:27.000000 cml-pam-0.3.2/src/pam/planner/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9227 2024-04-05 18:53:27.000000 cml-pam-0.3.2/src/pam/planner/ipf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4976 2024-04-05 18:53:27.000000 cml-pam-0.3.2/src/pam/planner/od.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5549 2024-04-05 18:53:27.000000 cml-pam-0.3.2/src/pam/planner/utils_planner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-05 18:53:27.000000 cml-pam-0.3.2/src/pam/planner/zones.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:53:35.985021 cml-pam-0.3.2/src/pam/plot/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-05 18:53:27.000000 cml-pam-0.3.2/src/pam/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17713 2024-04-05 18:53:27.000000 cml-pam-0.3.2/src/pam/plot/plans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9344 2024-04-05 18:53:27.000000 cml-pam-0.3.2/src/pam/plot/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:53:35.985021 cml-pam-0.3.2/src/pam/policy/
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-05 18:53:27.000000 cml-pam-0.3.2/src/pam/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-04-05 18:53:27.000000 cml-pam-0.3.2/src/pam/policy/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12245 2024-04-05 18:53:27.000000 cml-pam-0.3.2/src/pam/policy/modifiers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18186 2024-04-05 18:53:27.000000 cml-pam-0.3.2/src/pam/policy/policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8441 2024-04-05 18:53:27.000000 cml-pam-0.3.2/src/pam/policy/probability_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 18:53:27.000000 cml-pam-0.3.2/src/pam/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:53:35.985021 cml-pam-0.3.2/src/pam/read/
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-05 18:53:27.000000 cml-pam-0.3.2/src/pam/read/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32486 2024-04-05 18:53:27.000000 cml-pam-0.3.2/src/pam/read/diary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18294 2024-04-05 18:53:27.000000 cml-pam-0.3.2/src/pam/read/matsim.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:53:35.989021 cml-pam-0.3.2/src/pam/report/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 18:53:27.000000 cml-pam-0.3.2/src/pam/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6858 2024-04-05 18:53:27.000000 cml-pam-0.3.2/src/pam/report/benchmarks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-05 18:53:27.000000 cml-pam-0.3.2/src/pam/report/stringify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6223 2024-04-05 18:53:27.000000 cml-pam-0.3.2/src/pam/report/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:53:35.989021 cml-pam-0.3.2/src/pam/samplers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 18:53:27.000000 cml-pam-0.3.2/src/pam/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-05 18:53:27.000000 cml-pam-0.3.2/src/pam/samplers/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-05 18:53:27.000000 cml-pam-0.3.2/src/pam/samplers/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18182 2024-04-05 18:53:27.000000 cml-pam-0.3.2/src/pam/samplers/facility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-04-05 18:53:27.000000 cml-pam-0.3.2/src/pam/samplers/population.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7535 2024-04-05 18:53:27.000000 cml-pam-0.3.2/src/pam/samplers/spatial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-04-05 18:53:27.000000 cml-pam-0.3.2/src/pam/samplers/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29913 2024-04-05 18:53:27.000000 cml-pam-0.3.2/src/pam/samplers/tour.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14370 2024-04-05 18:53:27.000000 cml-pam-0.3.2/src/pam/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10938 2024-04-05 18:53:27.000000 cml-pam-0.3.2/src/pam/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-05 18:53:27.000000 cml-pam-0.3.2/src/pam/variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15713 2024-04-05 18:53:27.000000 cml-pam-0.3.2/src/pam/vehicles.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:53:35.989021 cml-pam-0.3.2/src/pam/write/
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-05 18:53:27.000000 cml-pam-0.3.2/src/pam/write/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7293 2024-04-05 18:53:27.000000 cml-pam-0.3.2/src/pam/write/diary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4419 2024-04-05 18:53:27.000000 cml-pam-0.3.2/src/pam/write/matrices.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11496 2024-04-05 18:53:27.000000 cml-pam-0.3.2/src/pam/write/matsim.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:53:35.997021 cml-pam-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    14067 2024-04-05 18:53:27.000000 cml-pam-0.3.2/tests/test_00_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19371 2024-04-05 18:53:27.000000 cml-pam-0.3.2/tests/test_01_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17495 2024-04-05 18:53:27.000000 cml-pam-0.3.2/tests/test_01_core_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-04-05 18:53:27.000000 cml-pam-0.3.2/tests/test_01_core_sample_locs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6911 2024-04-05 18:53:27.000000 cml-pam-0.3.2/tests/test_02_activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-04-05 18:53:27.000000 cml-pam-0.3.2/tests/test_02_activity_components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8011 2024-04-05 18:53:27.000000 cml-pam-0.3.2/tests/test_02_activity_fix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22997 2024-04-05 18:53:27.000000 cml-pam-0.3.2/tests/test_02_activity_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10541 2024-04-05 18:53:27.000000 cml-pam-0.3.2/tests/test_02_activity_trips.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6330 2024-04-05 18:53:27.000000 cml-pam-0.3.2/tests/test_02_activity_validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-04-05 18:53:27.000000 cml-pam-0.3.2/tests/test_03_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-04-05 18:53:27.000000 cml-pam-0.3.2/tests/test_03_read_activity_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5762 2024-04-05 18:53:27.000000 cml-pam-0.3.2/tests/test_03_read_challenge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7924 2024-04-05 18:53:27.000000 cml-pam-0.3.2/tests/test_03_read_matsim.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13222 2024-04-05 18:53:27.000000 cml-pam-0.3.2/tests/test_03_read_travel_diary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-04-05 18:53:27.000000 cml-pam-0.3.2/tests/test_04_household_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-05 18:53:27.000000 cml-pam-0.3.2/tests/test_05_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-05 18:53:27.000000 cml-pam-0.3.2/tests/test_05_modifiers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-05 18:53:27.000000 cml-pam-0.3.2/tests/test_05_modifiers_AddActivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7368 2024-04-05 18:53:27.000000 cml-pam-0.3.2/tests/test_05_modifiers_MoveActivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12796 2024-04-05 18:53:27.000000 cml-pam-0.3.2/tests/test_05_modifiers_ReduceSharedActivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-04-05 18:53:27.000000 cml-pam-0.3.2/tests/test_05_modifiers_RemoveActivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41606 2024-04-05 18:53:27.000000 cml-pam-0.3.2/tests/test_05_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-05 18:53:27.000000 cml-pam-0.3.2/tests/test_05_policies_prebaked.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9548 2024-04-05 18:53:27.000000 cml-pam-0.3.2/tests/test_05_policy_levels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11727 2024-04-05 18:53:27.000000 cml-pam-0.3.2/tests/test_05_probability_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-04-05 18:53:27.000000 cml-pam-0.3.2/tests/test_06_activity_remove_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-04-05 18:53:27.000000 cml-pam-0.3.2/tests/test_07_activity_fill_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27591 2024-04-05 18:53:27.000000 cml-pam-0.3.2/tests/test_08_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21807 2024-04-05 18:53:27.000000 cml-pam-0.3.2/tests/test_09_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15608 2024-04-05 18:53:27.000000 cml-pam-0.3.2/tests/test_09_samplers_tour.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-05 18:53:27.000000 cml-pam-0.3.2/tests/test_100_memory_profiling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8399 2024-04-05 18:53:27.000000 cml-pam-0.3.2/tests/test_10_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-05 18:53:27.000000 cml-pam-0.3.2/tests/test_11_population_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-05 18:53:27.000000 cml-pam-0.3.2/tests/test_11_spatial_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-04-05 18:53:27.000000 cml-pam-0.3.2/tests/test_12_scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-05 18:53:27.000000 cml-pam-0.3.2/tests/test_13_sample_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12156 2024-04-05 18:53:27.000000 cml-pam-0.3.2/tests/test_14_encode_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6178 2024-04-05 18:53:27.000000 cml-pam-0.3.2/tests/test_15_cropping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19012 2024-04-05 18:53:27.000000 cml-pam-0.3.2/tests/test_17_vehicles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-04-05 18:53:27.000000 cml-pam-0.3.2/tests/test_18_reporting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-04-05 18:53:27.000000 cml-pam-0.3.2/tests/test_18_reporting_bms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-05 18:53:27.000000 cml-pam-0.3.2/tests/test_19_combining.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3886 2024-04-05 18:53:27.000000 cml-pam-0.3.2/tests/test_20_planner_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-04-05 18:53:27.000000 cml-pam-0.3.2/tests/test_21_planner_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-04-05 18:53:27.000000 cml-pam-0.3.2/tests/test_22_planner_od.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-05 18:53:27.000000 cml-pam-0.3.2/tests/test_23_planner_zones.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7232 2024-04-05 18:53:27.000000 cml-pam-0.3.2/tests/test_24_planner_choice_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-04-05 18:53:27.000000 cml-pam-0.3.2/tests/test_25_planner_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-05 18:53:27.000000 cml-pam-0.3.2/tests/test_26_optimise_grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-04-05 18:53:27.000000 cml-pam-0.3.2/tests/test_27_optimise_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-04-05 18:53:27.000000 cml-pam-0.3.2/tests/test_28_planner_ipf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5481 2024-04-05 18:53:27.000000 cml-pam-0.3.2/tests/test_99_cli.py
```

### Comparing `cml-pam-0.3.1/LICENSE` & `cml-pam-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cml-pam-0.3.1/PKG-INFO` & `cml-pam-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cml-pam
-Version: 0.3.1
+Version: 0.3.2
 Summary: The Population activity Modeller (PAM) is a python API for activity sequence modelling.
 Author-email: Fred Shone <fred.shone@arup.com>
 Maintainer-email: Michael Fitzmaurice <michael.fitzmaurice@arup.com>, Kasia Kozlowska <kasia.kozlowska@arup.com>, Theodore Chatziioannou <theodore.chatziioannou@arup.com>, Bryn Pickering <17178478+brynpickering@users.noreply.github.com>
 License: MIT
 Project-URL: repository, https://github.com/arup-group/pam
 Project-URL: documentation, https://arup-group.github.io/pam
 Project-URL: changelog, https://github.com/arup-group/pam/blob/main/CHANGELOG.md
@@ -12,41 +12,43 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click<9
-Requires-Dist: gdal<3.6
-Requires-Dist: geopandas<0.14,>=0.13
+Requires-Dist: gdal>=3.5
+Requires-Dist: geopandas<0.15,>=0.13
 Requires-Dist: importlib_resources<7,>=6
 Requires-Dist: ipykernel<7
 Requires-Dist: lxml<5
 Requires-Dist: matplotlib<4,>=3
 Requires-Dist: numpy<2,>=1
 Requires-Dist: pandas<3,>=1.5
 Requires-Dist: plotly<6,>=4
 Requires-Dist: prettytable<4,>=3
-Requires-Dist: python-Levenshtein<0.22,>=0.21
+Requires-Dist: python-Levenshtein<0.26,>=0.21
 Requires-Dist: rich<14,>=12
 Requires-Dist: Rtree<2,>=1
 Requires-Dist: s2sphere<0.3
 Requires-Dist: scikit-learn<2,>=1.2
 Requires-Dist: shapely<3,>=1
 Requires-Dist: xlrd<3,>=2
 Provides-Extra: dev
+Requires-Dist: cruft<3,>=2; extra == "dev"
 Requires-Dist: jupyter<2; extra == "dev"
-Requires-Dist: mike<2; extra == "dev"
+Requires-Dist: mike<3,>=2; extra == "dev"
 Requires-Dist: mkdocs<2; extra == "dev"
+Requires-Dist: mkdocs-material<10,>=9.4; extra == "dev"
 Requires-Dist: mkdocs-click<0.7; extra == "dev"
 Requires-Dist: mkdocs-jupyter<0.25; extra == "dev"
 Requires-Dist: mkdocstrings-python<2; extra == "dev"
-Requires-Dist: nbmake<2; extra == "dev"
+Requires-Dist: nbmake<2,>=1.5.1; extra == "dev"
 Requires-Dist: pre-commit<4; extra == "dev"
-Requires-Dist: pytest<8; extra == "dev"
+Requires-Dist: pytest<9,>=8; extra == "dev"
 Requires-Dist: pytest-cov<5; extra == "dev"
 Requires-Dist: pytest-mock<4; extra == "dev"
 Requires-Dist: pytest-timeout<3; extra == "dev"
 Requires-Dist: pytest-xdist<4; extra == "dev"
 
 <!--- the "--8<--" html comments define what part of the README to add to the index page of the documentation -->
 <!--- --8<-- [start:docs] -->
@@ -160,7 +162,11 @@
 
 ```
 mike deploy 0.2
 mike serve
 ```
 
 Then you can view the documentation in a browser at <http://localhost:8000/>.
+
+## Credits
+
+This package was created with [Cookiecutter](https://github.com/audreyr/cookiecutter) and the [arup-group/cookiecutter-pypackage](https://github.com/arup-group/cookiecutter-pypackage) project template.
```

### Comparing `cml-pam-0.3.1/README.md` & `cml-pam-0.3.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -110,7 +110,11 @@
 
 ```
 mike deploy 0.2
 mike serve
 ```
 
 Then you can view the documentation in a browser at <http://localhost:8000/>.
+
+## Credits
+
+This package was created with [Cookiecutter](https://github.com/audreyr/cookiecutter) and the [arup-group/cookiecutter-pypackage](https://github.com/arup-group/cookiecutter-pypackage) project template.
```

### Comparing `cml-pam-0.3.1/cml_pam.egg-info/PKG-INFO` & `cml-pam-0.3.2/src/cml_pam.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cml-pam
-Version: 0.3.1
+Version: 0.3.2
 Summary: The Population activity Modeller (PAM) is a python API for activity sequence modelling.
 Author-email: Fred Shone <fred.shone@arup.com>
 Maintainer-email: Michael Fitzmaurice <michael.fitzmaurice@arup.com>, Kasia Kozlowska <kasia.kozlowska@arup.com>, Theodore Chatziioannou <theodore.chatziioannou@arup.com>, Bryn Pickering <17178478+brynpickering@users.noreply.github.com>
 License: MIT
 Project-URL: repository, https://github.com/arup-group/pam
 Project-URL: documentation, https://arup-group.github.io/pam
 Project-URL: changelog, https://github.com/arup-group/pam/blob/main/CHANGELOG.md
@@ -12,41 +12,43 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click<9
-Requires-Dist: gdal<3.6
-Requires-Dist: geopandas<0.14,>=0.13
+Requires-Dist: gdal>=3.5
+Requires-Dist: geopandas<0.15,>=0.13
 Requires-Dist: importlib_resources<7,>=6
 Requires-Dist: ipykernel<7
 Requires-Dist: lxml<5
 Requires-Dist: matplotlib<4,>=3
 Requires-Dist: numpy<2,>=1
 Requires-Dist: pandas<3,>=1.5
 Requires-Dist: plotly<6,>=4
 Requires-Dist: prettytable<4,>=3
-Requires-Dist: python-Levenshtein<0.22,>=0.21
+Requires-Dist: python-Levenshtein<0.26,>=0.21
 Requires-Dist: rich<14,>=12
 Requires-Dist: Rtree<2,>=1
 Requires-Dist: s2sphere<0.3
 Requires-Dist: scikit-learn<2,>=1.2
 Requires-Dist: shapely<3,>=1
 Requires-Dist: xlrd<3,>=2
 Provides-Extra: dev
+Requires-Dist: cruft<3,>=2; extra == "dev"
 Requires-Dist: jupyter<2; extra == "dev"
-Requires-Dist: mike<2; extra == "dev"
+Requires-Dist: mike<3,>=2; extra == "dev"
 Requires-Dist: mkdocs<2; extra == "dev"
+Requires-Dist: mkdocs-material<10,>=9.4; extra == "dev"
 Requires-Dist: mkdocs-click<0.7; extra == "dev"
 Requires-Dist: mkdocs-jupyter<0.25; extra == "dev"
 Requires-Dist: mkdocstrings-python<2; extra == "dev"
-Requires-Dist: nbmake<2; extra == "dev"
+Requires-Dist: nbmake<2,>=1.5.1; extra == "dev"
 Requires-Dist: pre-commit<4; extra == "dev"
-Requires-Dist: pytest<8; extra == "dev"
+Requires-Dist: pytest<9,>=8; extra == "dev"
 Requires-Dist: pytest-cov<5; extra == "dev"
 Requires-Dist: pytest-mock<4; extra == "dev"
 Requires-Dist: pytest-timeout<3; extra == "dev"
 Requires-Dist: pytest-xdist<4; extra == "dev"
 
 <!--- the "--8<--" html comments define what part of the README to add to the index page of the documentation -->
 <!--- --8<-- [start:docs] -->
@@ -160,7 +162,11 @@
 
 ```
 mike deploy 0.2
 mike serve
 ```
 
 Then you can view the documentation in a browser at <http://localhost:8000/>.
+
+## Credits
+
+This package was created with [Cookiecutter](https://github.com/audreyr/cookiecutter) and the [arup-group/cookiecutter-pypackage](https://github.com/arup-group/cookiecutter-pypackage) project template.
```

### Comparing `cml-pam-0.3.1/pam/__init__.py` & `cml-pam-0.3.2/src/pam/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,17 @@
-__version__ = "0.3.1"
+"""Top-level module for pam."""
+
+import pyproj
+
+__author__ = """Fred Shone"""  # triple quotes in case the name has quotes in it.
+__email__ = "fred.shone@arup.com"
+__version__ = "0.3.2"
+
+
+pyproj.network.set_network_enabled(False)
 
 
 class PAMValidationError(Exception):
     """Custom exception raised for an Activity Plan validation Error."""
 
 
 class PAMSequenceValidationError(PAMValidationError):
```

### Comparing `cml-pam-0.3.1/pam/activity.py` & `cml-pam-0.3.2/src/pam/activity.py`

 * *Files identical despite different names*

### Comparing `cml-pam-0.3.1/pam/array/decode.py` & `cml-pam-0.3.2/src/pam/array/decode.py`

 * *Files identical despite different names*

### Comparing `cml-pam-0.3.1/pam/array/distance.py` & `cml-pam-0.3.2/src/pam/array/distance.py`

 * *Files identical despite different names*

### Comparing `cml-pam-0.3.1/pam/array/encode.py` & `cml-pam-0.3.2/src/pam/array/encode.py`

 * *Files identical despite different names*

### Comparing `cml-pam-0.3.1/pam/cli.py` & `cml-pam-0.3.2/src/pam/cli.py`

 * *Files identical despite different names*

### Comparing `cml-pam-0.3.1/pam/core.py` & `cml-pam-0.3.2/src/pam/core.py`

 * *Files identical despite different names*

### Comparing `cml-pam-0.3.1/pam/fixtures/dtd/electric_vehicles_v1.dtd` & `cml-pam-0.3.2/src/pam/fixtures/dtd/electric_vehicles_v1.dtd`

 * *Files identical despite different names*

### Comparing `cml-pam-0.3.1/pam/fixtures/dtd/population_v5.dtd` & `cml-pam-0.3.2/src/pam/fixtures/dtd/population_v5.dtd`

 * *Files identical despite different names*

### Comparing `cml-pam-0.3.1/pam/fixtures/dtd/population_v6.dtd` & `cml-pam-0.3.2/src/pam/fixtures/dtd/population_v6.dtd`

 * *Files identical despite different names*

### Comparing `cml-pam-0.3.1/pam/fixtures/dtd/vehicleDefinitions_v2.0.xsd` & `cml-pam-0.3.2/src/pam/fixtures/dtd/vehicleDefinitions_v2.0.xsd`

 * *Files identical despite different names*

### Comparing `cml-pam-0.3.1/pam/location.py` & `cml-pam-0.3.2/src/pam/location.py`

 * *Files identical despite different names*

### Comparing `cml-pam-0.3.1/pam/operations/combine.py` & `cml-pam-0.3.2/src/pam/operations/combine.py`

 * *Files identical despite different names*

### Comparing `cml-pam-0.3.1/pam/operations/cropping.py` & `cml-pam-0.3.2/src/pam/operations/cropping.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Methods for cropping plans outside core areas."""
+
 from typing import List
 
 from shapely.geometry import LineString, Polygon
 
 import pam
 from pam.activity import Activity, Leg, Plan
 from pam.core import Population
```

### Comparing `cml-pam-0.3.1/pam/optimise/grid.py` & `cml-pam-0.3.2/src/pam/optimise/grid.py`

 * *Files identical despite different names*

### Comparing `cml-pam-0.3.1/pam/optimise/random.py` & `cml-pam-0.3.2/src/pam/optimise/random.py`

 * *Files identical despite different names*

### Comparing `cml-pam-0.3.1/pam/planner/choice_location.py` & `cml-pam-0.3.2/src/pam/planner/choice_location.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Location and mode choice models for activity modelling."""
+
 import itertools
 import logging
 from abc import ABC, abstractmethod
 from collections.abc import Callable
 from copy import deepcopy
 from dataclasses import dataclass
 from typing import Literal, NamedTuple, Optional, Union
```

### Comparing `cml-pam-0.3.1/pam/planner/clustering.py` & `cml-pam-0.3.2/src/pam/planner/clustering.py`

 * *Files identical despite different names*

### Comparing `cml-pam-0.3.1/pam/planner/encoder.py` & `cml-pam-0.3.2/src/pam/planner/encoder.py`

 * *Files identical despite different names*

### Comparing `cml-pam-0.3.1/pam/planner/ipf.py` & `cml-pam-0.3.2/src/pam/planner/ipf.py`

 * *Files identical despite different names*

### Comparing `cml-pam-0.3.1/pam/planner/od.py` & `cml-pam-0.3.2/src/pam/planner/od.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Manages origin-destination data required by the planner module."""
+
 import itertools
 from typing import NamedTuple, Union
 
 import numpy as np
 
 
 class Labels(NamedTuple):
```

### Comparing `cml-pam-0.3.1/pam/planner/utils_planner.py` & `cml-pam-0.3.2/src/pam/planner/utils_planner.py`

 * *Files identical despite different names*

### Comparing `cml-pam-0.3.1/pam/planner/zones.py` & `cml-pam-0.3.2/src/pam/planner/zones.py`

 * *Files identical despite different names*

### Comparing `cml-pam-0.3.1/pam/plot/plans.py` & `cml-pam-0.3.2/src/pam/plot/plans.py`

 * *Files identical despite different names*

### Comparing `cml-pam-0.3.1/pam/plot/stats.py` & `cml-pam-0.3.2/src/pam/plot/stats.py`

 * *Files identical despite different names*

### Comparing `cml-pam-0.3.1/pam/policy/__init__.py` & `cml-pam-0.3.2/src/pam/policy/__init__.py`

 * *Files identical despite different names*

### Comparing `cml-pam-0.3.1/pam/policy/filters.py` & `cml-pam-0.3.2/src/pam/policy/filters.py`

 * *Files identical despite different names*

### Comparing `cml-pam-0.3.1/pam/policy/modifiers.py` & `cml-pam-0.3.2/src/pam/policy/modifiers.py`

 * *Files identical despite different names*

### Comparing `cml-pam-0.3.1/pam/policy/policies.py` & `cml-pam-0.3.2/src/pam/policy/policies.py`

 * *Files identical despite different names*

### Comparing `cml-pam-0.3.1/pam/policy/probability_samplers.py` & `cml-pam-0.3.2/src/pam/policy/probability_samplers.py`

 * *Files identical despite different names*

### Comparing `cml-pam-0.3.1/pam/read/__init__.py` & `cml-pam-0.3.2/src/pam/read/__init__.py`

 * *Files identical despite different names*

### Comparing `cml-pam-0.3.1/pam/read/diary.py` & `cml-pam-0.3.2/src/pam/read/diary.py`

 * *Files identical despite different names*

### Comparing `cml-pam-0.3.1/pam/read/matsim.py` & `cml-pam-0.3.2/src/pam/read/matsim.py`

 * *Files identical despite different names*

### Comparing `cml-pam-0.3.1/pam/report/benchmarks.py` & `cml-pam-0.3.2/src/pam/report/benchmarks.py`

 * *Files identical despite different names*

### Comparing `cml-pam-0.3.1/pam/report/stringify.py` & `cml-pam-0.3.2/src/pam/report/stringify.py`

 * *Files identical despite different names*

### Comparing `cml-pam-0.3.1/pam/report/summary.py` & `cml-pam-0.3.2/src/pam/report/summary.py`

 * *Files identical despite different names*

### Comparing `cml-pam-0.3.1/pam/samplers/attributes.py` & `cml-pam-0.3.2/src/pam/samplers/attributes.py`

 * *Files identical despite different names*

### Comparing `cml-pam-0.3.1/pam/samplers/basic.py` & `cml-pam-0.3.2/src/pam/samplers/basic.py`

 * *Files identical despite different names*

### Comparing `cml-pam-0.3.1/pam/samplers/facility.py` & `cml-pam-0.3.2/src/pam/samplers/facility.py`

 * *Files identical despite different names*

### Comparing `cml-pam-0.3.1/pam/samplers/population.py` & `cml-pam-0.3.2/src/pam/samplers/population.py`

 * *Files identical despite different names*

### Comparing `cml-pam-0.3.1/pam/samplers/spatial.py` & `cml-pam-0.3.2/src/pam/samplers/spatial.py`

 * *Files identical despite different names*

### Comparing `cml-pam-0.3.1/pam/samplers/time.py` & `cml-pam-0.3.2/src/pam/samplers/time.py`

 * *Files identical despite different names*

### Comparing `cml-pam-0.3.1/pam/samplers/tour.py` & `cml-pam-0.3.2/src/pam/samplers/tour.py`

 * *Files identical despite different names*

### Comparing `cml-pam-0.3.1/pam/scoring.py` & `cml-pam-0.3.2/src/pam/scoring.py`

 * *Files identical despite different names*

### Comparing `cml-pam-0.3.1/pam/utils.py` & `cml-pam-0.3.2/src/pam/utils.py`

 * *Files identical despite different names*

### Comparing `cml-pam-0.3.1/pam/variables.py` & `cml-pam-0.3.2/src/pam/variables.py`

 * *Files identical despite different names*

### Comparing `cml-pam-0.3.1/pam/vehicles.py` & `cml-pam-0.3.2/src/pam/vehicles.py`

 * *Files identical despite different names*

### Comparing `cml-pam-0.3.1/pam/write/diary.py` & `cml-pam-0.3.2/src/pam/write/diary.py`

 * *Files identical despite different names*

### Comparing `cml-pam-0.3.1/pam/write/matrices.py` & `cml-pam-0.3.2/src/pam/write/matrices.py`

 * *Files identical despite different names*

### Comparing `cml-pam-0.3.1/pam/write/matsim.py` & `cml-pam-0.3.2/src/pam/write/matsim.py`

 * *Files identical despite different names*

### Comparing `cml-pam-0.3.1/pyproject.toml` & `cml-pam-0.3.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -14,69 +14,71 @@
 filterwarnings = [
     # https://github.com/pytest-dev/pytest-xdist/issues/825
     "ignore:The --rsyncdir command line argument and rsyncdirs config variable are deprecated.:DeprecationWarning",
 ]
 
 [tool.coverage.run]
 branch = true
-source = ["pam/"]
+source = ["src/"]
 
 [tool.coverage.report]
 fail_under = 89
 
 [tool.coverage.html]
 directory = "reports/coverage"
 
 [tool.coverage.xml]
 output = "reports/coverage/coverage.xml"
 
 [tool.black]
 line-length = 100
-skip_magic_trailing_comma = true
+skip-magic-trailing-comma = true
 
 [tool.ruff]
 line-length = 100
+
+[tool.ruff.lint]
 select = ["E", "F", "I", "Q"]
 
 ignore = [
     "E501", # line too long: Black will handle this.
     "D1",   # Ignore missing docstrings in public functions/modules. There are just too many of them missing...
 ]
 
 # Exclude a variety of commonly ignored directories.
 exclude = [".*", "__pypackages__", "build", "dist", "venv", "reports/"]
 
 # Allow unused variables when underscore-prefixed.
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
 
-[tool.ruff.pydocstyle]
+[tool.ruff.lint.pydocstyle]
 convention = "google"
 
-[tool.ruff.mccabe]
+[tool.ruff.lint.mccabe]
 # Unlike Flake8, default to a complexity level of 10.
 max-complexity = 10
 
+[tool.ruff.lint.per-file-ignores]
 # Ignore `E402` (import violations) and `F401` (unused imports) in all `__init__.py` files
-[tool.ruff.per-file-ignores]
 "__init__.py" = ["E402", "F401"]
-"*.ipynb" = ["E402"]
+
+[tool.ruff.lint.flake8-quotes]
+docstring-quotes = "double"
 
 # Ignore `E402` for all notebooks
 [tool.nbqa.addopts]
 ruff = ["--extend-ignore=E402"]
 
-
-[tool.ruff.flake8-quotes]
-docstring-quotes = "double"
-
 [tool.setuptools.packages.find]
+where = ["src"]
 include = ["pam*"]
 
 [tool.setuptools.package-data]
-pam = ["fixtures/**/*"]
+# "py.typed" is added by default. It allows `mypy` to register the package as having type hints.
+pam = ["py.typed", "fixtures/**/*"]
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cml-pam"
```

### Comparing `cml-pam-0.3.1/tests/test_00_utils.py` & `cml-pam-0.3.2/tests/test_00_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from datetime import datetime, timedelta
 from pathlib import Path
 
 import numpy as np
 import pandas as pd
 import pytest
 from geopandas import GeoDataFrame
+from pam import utils
+from pam.core import Population
 from pandas import Timestamp
 from pandas.testing import assert_frame_equal
 from s2sphere import CellId
 from shapely.geometry import LineString
 
-from pam import utils
-from pam.core import Population
-
 
 @pytest.fixture()
 def correct_pt_person_geodataframe():
     return GeoDataFrame(
         {
             "distance": {
                 0: 6412.774690,
```

### Comparing `cml-pam-0.3.1/tests/test_01_core.py` & `cml-pam-0.3.2/tests/test_01_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from datetime import datetime, timedelta
 
 import pytest
-
 from pam import PAMSequenceValidationError, PAMTimesValidationError, PAMValidationLocationsError
 from pam.activity import Activity, Leg
 from pam.core import Household, Person, Population
 from pam.utils import minutes_to_datetime as mtdt
 from pam.utils import timedelta_to_matsim_time as tdtm
 from pam.variables import END_OF_DAY
```

### Comparing `cml-pam-0.3.1/tests/test_01_core_operations.py` & `cml-pam-0.3.2/tests/test_01_core_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pytest
-
 from pam.activity import Activity, Leg
 from pam.core import Household, Person, Population
 
 
 def test_get_last_component_activity():
     p = Person(0)
     p.add(Activity())
```

### Comparing `cml-pam-0.3.1/tests/test_01_core_sample_locs.py` & `cml-pam-0.3.2/tests/test_01_core_sample_locs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from random import random
 
-from shapely.geometry import Point
-
 from pam.core import Population
 from pam.location import Location
+from shapely.geometry import Point
 
 
 def test_assign_same_locs_to_household(SmithHousehold):
     population = Population()
     population.add(SmithHousehold)
 
     class FakeSampler:
```

### Comparing `cml-pam-0.3.1/tests/test_02_activity.py` & `cml-pam-0.3.2/tests/test_02_activity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pytest
-
 from pam.activity import Activity, Leg, Plan
 from pam.utils import minutes_to_datetime as mtdt
 
 
 @pytest.fixture()
 def list_of_acts():
     a_1 = Activity(2, "act", "loc", start_time=mtdt(18 * 60), end_time=mtdt(19 * 60))
```

### Comparing `cml-pam-0.3.1/tests/test_02_activity_components.py` & `cml-pam-0.3.2/tests/test_02_activity_components.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from datetime import timedelta
 
 import pytest
-
 from pam.activity import Activity, Leg, Location, Plan
 from pam.utils import minutes_to_datetime as mtdt
 from pam.variables import END_OF_DAY
 
 
 def test_act_init():
     act = Activity()
```

### Comparing `cml-pam-0.3.1/tests/test_02_activity_fix.py` & `cml-pam-0.3.2/tests/test_02_activity_fix.py`

 * *Files identical despite different names*

### Comparing `cml-pam-0.3.1/tests/test_02_activity_plan.py` & `cml-pam-0.3.2/tests/test_02_activity_plan.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from datetime import timedelta
 
 import pytest
-
 from pam import PAMSequenceValidationError
 from pam.activity import Activity, Leg, Location, Plan
 from pam.utils import minutes_to_datetime as mtdt
 from pam.variables import END_OF_DAY
 
 
 def test_plan_init():
```

### Comparing `cml-pam-0.3.1/tests/test_02_activity_trips.py` & `cml-pam-0.3.2/tests/test_02_activity_trips.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import pytest
-from shapely import Point
-
 from pam.activity import Activity, Leg, Plan, Trip
+from shapely import Point
 
 
 @pytest.mark.parametrize(
     "day,expected",
     [
         ([], []),
         ([Activity(act="home", loc=Point(0, 0))], []),
```

### Comparing `cml-pam-0.3.1/tests/test_02_activity_validate.py` & `cml-pam-0.3.2/tests/test_02_activity_validate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pytest
-
 from pam import PAMSequenceValidationError, PAMTimesValidationError, PAMValidationLocationsError
 from pam.activity import Activity, Leg, Plan
 from pam.core import Person
 from pam.utils import minutes_to_datetime as mtdt
 from pam.variables import END_OF_DAY
```

### Comparing `cml-pam-0.3.1/tests/test_03_read.py` & `cml-pam-0.3.2/tests/test_03_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import os
 
 import pandas as pd
 import pytest
-
 from pam.core import Household, Population
 from pam.read import load_pickle, load_travel_diary
 
 test_trips_path = (pytest.test_data_dir / "simple_travel_diaries.csv").as_posix()
 test_attributes_path = (pytest.test_data_dir / "simple_persons_data.csv").as_posix()
```

### Comparing `cml-pam-0.3.1/tests/test_03_read_activity_plan.py` & `cml-pam-0.3.2/tests/test_03_read_activity_plan.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import pandas as pd
 import pytest
-
 from pam.read import trip_based_travel_diary_read
 
 test_activities_path = pytest.test_data_dir / "test_activity_plans.csv"
 test_attributes_path = pytest.test_data_dir / "simple_persons_data.csv"
 
 
 @pytest.fixture
```

### Comparing `cml-pam-0.3.1/tests/test_03_read_challenge.py` & `cml-pam-0.3.2/tests/test_03_read_challenge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import pandas as pd
 import pytest
-
 from pam.read import load_travel_diary
 
 test_trips_path = pytest.test_data_dir / "simple_travel_diaries.csv"
 test_attributes_path = pytest.test_data_dir / "simple_persons_data.csv"
 
 
 @pytest.fixture
```

### Comparing `cml-pam-0.3.1/tests/test_03_read_matsim.py` & `cml-pam-0.3.2/tests/test_03_read_matsim.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import pytest
 from lxml import etree as et
-
 from pam.activity import Plan
 from pam.read import (
     get_attributes_from_person,
     load_attributes_map,
     parse_veh_attribute,
     read_matsim,
     stream_matsim_persons,
```

### Comparing `cml-pam-0.3.1/tests/test_03_read_travel_diary.py` & `cml-pam-0.3.2/tests/test_03_read_travel_diary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from io import StringIO
 
 import pandas as pd
 import pytest
-
 from pam import PAMValidationLocationsError
 from pam.core import Person
 from pam.read import build_population, load_travel_diary
 
 
 @pytest.fixture
 def trips():
```

### Comparing `cml-pam-0.3.1/tests/test_04_household_policies.py` & `cml-pam-0.3.2/tests/test_04_household_policies.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pytest
-
 from pam.activity import Activity, Leg
 from pam.core import Household, Person, Population
 from pam.policy import policies, probability_samplers
 from pam.utils import minutes_to_datetime as mtdt
 from pam.variables import END_OF_DAY
```

### Comparing `cml-pam-0.3.1/tests/test_05_filters.py` & `cml-pam-0.3.2/tests/test_05_filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from random import choice
 
 import pytest
-
 from pam.activity import Activity
 from pam.core import Household, Person
 from pam.policy.filters import PersonAttributeFilter
 
 
 def test_subclass_name_features_in_repr_string():
     attrib_filter = PersonAttributeFilter({})
```

### Comparing `cml-pam-0.3.1/tests/test_05_modifiers_AddActivity.py` & `cml-pam-0.3.2/tests/test_05_modifiers_AddActivity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pytest
-
 from pam.activity import Activity
 from pam.policy import modifiers
 from pam.utils import minutes_to_datetime as mtdt
 from pam.variables import END_OF_DAY
 
 
 def assert_correct_activities(person, ordered_activities_list):
```

### Comparing `cml-pam-0.3.1/tests/test_05_modifiers_MoveActivity.py` & `cml-pam-0.3.2/tests/test_05_modifiers_MoveActivity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pytest
-
 from pam.activity import Activity, Plan
 from pam.policy.modifiers import MoveActivityTourToHomeLocation
 from pam.utils import minutes_to_datetime as mtdt
 from pam.variables import END_OF_DAY
 
 
 def assert_correct_activities(person, ordered_activities_list):
```

### Comparing `cml-pam-0.3.1/tests/test_05_modifiers_ReduceSharedActivity.py` & `cml-pam-0.3.2/tests/test_05_modifiers_ReduceSharedActivity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import random
 
 import pytest
-
 from pam.activity import Activity, Leg
 from pam.core import Person
 from pam.policy import modifiers
 from pam.utils import minutes_to_datetime as mtdt
 from pam.variables import END_OF_DAY
```

### Comparing `cml-pam-0.3.1/tests/test_05_modifiers_RemoveActivity.py` & `cml-pam-0.3.2/tests/test_05_modifiers_RemoveActivity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pytest
-
 from pam.activity import Activity
 from pam.policy import modifiers
 
 
 def test_RemoveActivity_apply_to_delegates_to_remove_individual_activities_when_given_person_and_activities(
     mocker, SmithHousehold
 ):
```

### Comparing `cml-pam-0.3.1/tests/test_05_policies.py` & `cml-pam-0.3.2/tests/test_05_policies.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import random
 
 import pytest
-
 from pam.activity import Activity, Leg
 from pam.core import Person
 from pam.policy import filters, modifiers, policies, probability_samplers
 from pam.utils import minutes_to_datetime as mtdt
 from pam.variables import END_OF_DAY
```

### Comparing `cml-pam-0.3.1/tests/test_05_policies_prebaked.py` & `cml-pam-0.3.2/tests/test_05_policies_prebaked.py`

 * *Files identical despite different names*

### Comparing `cml-pam-0.3.1/tests/test_05_policy_levels.py` & `cml-pam-0.3.2/tests/test_05_policy_levels.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import random
 
 import pytest
-
 from pam.activity import Activity
 from pam.policy import filters, modifiers, policies, probability_samplers
 from pam.utils import minutes_to_datetime as mtdt
 from pam.variables import END_OF_DAY
 
 
 def assert_correct_activities(person, ordered_activities_list):
```

### Comparing `cml-pam-0.3.1/tests/test_05_probability_samplers.py` & `cml-pam-0.3.2/tests/test_05_probability_samplers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import random
 
 import pytest
-
 from pam.activity import Activity
 from pam.core import Household, Person
 from pam.policy import probability_samplers
 
 
 @pytest.fixture()
 def SmithHousehold_alt(instantiate_household_with, Steve, Hilda):
```

### Comparing `cml-pam-0.3.1/tests/test_06_activity_remove_plan.py` & `cml-pam-0.3.2/tests/test_06_activity_remove_plan.py`

 * *Files identical despite different names*

### Comparing `cml-pam-0.3.1/tests/test_07_activity_fill_plan.py` & `cml-pam-0.3.2/tests/test_07_activity_fill_plan.py`

 * *Files identical despite different names*

### Comparing `cml-pam-0.3.1/tests/test_08_write.py` & `cml-pam-0.3.2/tests/test_08_write.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,23 +2,22 @@
 from copy import deepcopy
 from datetime import datetime
 
 import geopandas as gp
 import lxml
 import pandas as pd
 import pytest
-from shapely.geometry import Point
-
 from pam import write
 from pam.activity import Activity, Leg
 from pam.core import Household, Person, Population
 from pam.read import read_matsim
 from pam.utils import minutes_to_datetime as mtdt
 from pam.variables import END_OF_DAY
 from pam.write import Writer, write_matsim, write_matsim_population_v6, write_od_matrices
+from shapely.geometry import Point
 
 
 def test_writer_enters(tmp_path):
     path = str(tmp_path / "test.xml")
     with Writer(path):
         assert os.path.exists(os.path.dirname(path))
         assert os.path.exists(path)
```

### Comparing `cml-pam-0.3.1/tests/test_09_samplers.py` & `cml-pam-0.3.2/tests/test_09_samplers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 import random
 from collections.abc import Iterator
 
 import geopandas as gp
 import pandas as pd
 import pytest
+from pam.samplers import attributes, basic, facility, spatial
 from shapely.geometry import (
     LinearRing,
     LineString,
     MultiLineString,
     MultiPoint,
     MultiPolygon,
     Point,
     Polygon,
 )
 
-from pam.samplers import attributes, basic, facility, spatial
-
 
 @pytest.fixture
 def michael():
     return {"age": 16, "agebin": "younger", "gender": "male"}
 
 
 @pytest.fixture
```

### Comparing `cml-pam-0.3.1/tests/test_09_samplers_tour.py` & `cml-pam-0.3.2/tests/test_09_samplers_tour.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # %% import packages
 
 import geopandas as gp
 import pandas as pd
 import pytest
 from matplotlib.figure import Figure
-from shapely.geometry import Point, Polygon
-
 from pam.core import Person
 from pam.samplers import tour
 from pam.samplers.facility import FacilitySampler
 from pam.variables import END_OF_DAY
+from shapely.geometry import Point, Polygon
 
 # %% Test input data
 
 
 @pytest.fixture
 def facility_gdf():
     facility_df = pd.DataFrame(
```

### Comparing `cml-pam-0.3.1/tests/test_100_memory_profiling.py` & `cml-pam-0.3.2/tests/test_100_memory_profiling.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from pathlib import Path
 
 import pandas as pd
 import pytest
-
 from pam import read
 
 BENCHMARK_MEM = "1400 MB"
 BENCHMARK_SECONDS = 250
 
 data_dir = Path(__file__).parent / "test_data"
```

### Comparing `cml-pam-0.3.1/tests/test_10_plotting.py` & `cml-pam-0.3.2/tests/test_10_plotting.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,17 +2,14 @@
 
 import numpy as np
 import pandas as pd
 import pytest
 from matplotlib.axes import Axes
 from matplotlib.figure import Figure
 from matplotlib.legend import Legend
-from plotly.graph_objs import Scattermapbox
-from shapely.geometry import Point
-
 from pam.core import Household, Population
 from pam.plot.plans import (
     build_cmap,
     build_person_df,
     build_person_travel_geodataframe,
     build_rgb_travel_cmap,
     plot_activities,
@@ -26,14 +23,16 @@
     plot_activity_times,
     plot_leg_times,
     plot_population_comparisons,
     time_binner,
 )
 from pam.policy import policies
 from pam.variables import DEFAULT_ACTIVITIES_FONTSIZE, DEFAULT_ACTIVITIES_PLOT_WIDTH
+from plotly.graph_objs import Scattermapbox
+from shapely.geometry import Point
 
 
 @pytest.fixture
 def person_df(person_heh):
     return build_person_df(person_heh)
```

### Comparing `cml-pam-0.3.1/tests/test_11_population_sample.py` & `cml-pam-0.3.2/tests/test_11_population_sample.py`

 * *Files identical despite different names*

### Comparing `cml-pam-0.3.1/tests/test_11_spatial_sampling.py` & `cml-pam-0.3.2/tests/test_11_spatial_sampling.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pytest
-
 from pam.samplers import spatial
 
 geojson_path = pytest.test_data_dir / "test_geometry.geojson"
 
 
 @pytest.fixture
 def geo_sampler():
```

### Comparing `cml-pam-0.3.1/tests/test_12_scoring.py` & `cml-pam-0.3.2/tests/test_12_scoring.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pytest
-
 from pam.read import read_matsim
 from pam.scoring import CharyparNagelPlanScorer
 
 TEST_EXPERIENCED_PLANS_PATH = pytest.test_data_dir / "test_matsim_experienced_plans_v12.xml"
 
 
 def test_score_plan_monetary_cost(default_config):
```

### Comparing `cml-pam-0.3.1/tests/test_13_sample_time.py` & `cml-pam-0.3.2/tests/test_13_sample_time.py`

 * *Files identical despite different names*

### Comparing `cml-pam-0.3.1/tests/test_14_encode_array.py` & `cml-pam-0.3.2/tests/test_14_encode_array.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from datetime import datetime
 
 import numpy as np
-
 from pam.activity import Activity, Leg, Plan
 from pam.array import decode, distance, encode
 from pam.utils import minutes_to_datetime as mtdt
 from pam.variables import END_OF_DAY
 
 # One hot
```

### Comparing `cml-pam-0.3.1/tests/test_15_cropping.py` & `cml-pam-0.3.2/tests/test_15_cropping.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import os
 from copy import deepcopy
 
 import geopandas as gp
 import pytest
-from shapely.geometry import Point, Polygon
-
 from pam.activity import Activity, Leg, Plan
 from pam.core import Household, Person, Population
 from pam.operations import cropping
 from pam.utils import minutes_to_datetime as mtdt
 from pam.variables import END_OF_DAY
+from shapely.geometry import Point, Polygon
 
 
 @pytest.fixture
 def test_plan() -> Plan:
     plan = Plan()
     plan.day = [
         Activity(seq=1, act="home", loc=Point(0.31, 0.81), start_time=mtdt(0), end_time=mtdt(420)),
```

### Comparing `cml-pam-0.3.1/tests/test_17_vehicles.py` & `cml-pam-0.3.2/tests/test_17_vehicles.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from copy import deepcopy
 
 import importlib_resources
 import lxml
 import pytest
-
 from pam import PAMVehicleIdError, PAMVehicleTypeError
 from pam.core import Person, Population
 from pam.read.matsim import read_matsim
 from pam.vehicles import ElectricVehicle, Vehicle, VehicleManager, VehicleType
 from pam.write.matsim import write_matsim
```

### Comparing `cml-pam-0.3.1/tests/test_18_reporting.py` & `cml-pam-0.3.2/tests/test_18_reporting.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import numpy as np
-
 from pam.report import stringify, summary
 
 # summary
 
 
 def test_calc_stats_for_all(population):
     report = summary.calc_stats(population=population, key=None, value=None)
```

### Comparing `cml-pam-0.3.1/tests/test_18_reporting_bms.py` & `cml-pam-0.3.2/tests/test_18_reporting_bms.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pandas as pd
-
 from pam.report import benchmarks
 
 
 def test_get_trips_data(population):
     trips = population.trips_df()
     assert len(trips) == 10
     assert list(trips["mode"]) == [
```

### Comparing `cml-pam-0.3.1/tests/test_19_combining.py` & `cml-pam-0.3.2/tests/test_19_combining.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import os
 
 import pytest
-
 from pam.operations import combine
 
 
 @pytest.fixture
 def path_population_A():
     return os.path.join("tests", "test_data", "test_matsim_population_A.xml")
```

### Comparing `cml-pam-0.3.1/tests/test_20_planner_clustering.py` & `cml-pam-0.3.2/tests/test_20_planner_clustering.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import numpy as np
 import pytest
-
 from pam.planner import clustering
 
 
 @pytest.fixture
 def clusters(population_no_args):
     clusters = clustering.PlanClusters(population_no_args)
     n_clusters = 2
```

### Comparing `cml-pam-0.3.1/tests/test_21_planner_encoder.py` & `cml-pam-0.3.2/tests/test_21_planner_encoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pytest
-
 from pam.planner.encoder import (
     PlanCharacterEncoder,
     PlanOneHotEncoder,
     PlansCharacterEncoder,
     PlansOneHotEncoder,
     StringCharacterEncoder,
     StringIntEncoder,
```

### Comparing `cml-pam-0.3.1/tests/test_22_planner_od.py` & `cml-pam-0.3.2/tests/test_22_planner_od.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from copy import deepcopy
 
 import numpy as np
 import pytest
-
 from pam.planner.od import OD, Labels, ODFactory, ODMatrix
 
 
 @pytest.fixture
 def od_matrices():
     zone_labels = ["a", "b"]
     matrices = [
```

### Comparing `cml-pam-0.3.1/tests/test_24_planner_choice_location.py` & `cml-pam-0.3.2/tests/test_24_planner_choice_location.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import random
 from copy import deepcopy
 
 import numpy as np
 import pytest
-from pytest import approx
-
 from pam.planner.choice_location import (
     ChoiceConfiguration,
     ChoiceMNL,
     ChoiceModel,
     DiscretionaryTripOD,
     DiscretionaryTrips,
 )
 from pam.planner.utils_planner import get_trip_chains_either_anchor, sample_weighted
+from pytest import approx
 
 
 @pytest.fixture
 def population_planner_choice(population_no_args):
     for hid, pid, person in population_no_args.people():
         for act in person.activities:
             act.location.area = "a"
```

### Comparing `cml-pam-0.3.1/tests/test_25_planner_utils.py` & `cml-pam-0.3.2/tests/test_25_planner_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import random
 
 import numpy as np
 import pytest
-
 from pam.activity import Leg
 from pam.operations.cropping import link_population
 from pam.planner.utils_planner import (
     apply_mode_to_home_chain,
     calculate_mnl_probabilities,
     convert_single_anchor_roundtrip,
     get_act_names,
```

### Comparing `cml-pam-0.3.1/tests/test_26_optimise_grid.py` & `cml-pam-0.3.2/tests/test_26_optimise_grid.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Tests for pam/optimise/grid.py"""
-import pytest
 
+import pytest
 from pam.activity import Activity, Leg, Plan
 from pam.core import Person
 from pam.optimise import grid
 from pam.scoring import PlanScorer
 from pam.utils import minutes_to_datetime as mtdt
 from pam.variables import END_OF_DAY
```

### Comparing `cml-pam-0.3.1/tests/test_27_optimise_random.py` & `cml-pam-0.3.2/tests/test_27_optimise_random.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Tests for pam/optimise/random.py"""
-import pytest
 
+import pytest
 from pam.activity import Activity, Leg, Plan
 from pam.core import Person
 from pam.optimise import random
 from pam.scoring import PlanScorer
 from pam.utils import minutes_to_datetime as mtdt
 from pam.variables import END_OF_DAY
```

### Comparing `cml-pam-0.3.1/tests/test_28_planner_ipf.py` & `cml-pam-0.3.2/tests/test_28_planner_ipf.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import numpy as np
 import pandas as pd
 import pytest
-
 from pam.planner import ipf
 
 
 @pytest.fixture
 def marginals():
     m = [np.array([20, 80]), np.array([60, 40]), np.array([30, 60, 10])]
     return m
```

### Comparing `cml-pam-0.3.1/tests/test_99_cli.py` & `cml-pam-0.3.2/tests/test_99_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import os
 
 import pytest
 from click.testing import CliRunner
-
 from pam import read
 from pam.cli import cli
 
 
 @pytest.fixture
 def path_test_plan():
     return os.path.join("tests", "test_data", "test_matsim_plansv12.xml")
```

