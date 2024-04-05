# Comparing `tmp/lst-pressure-1.4.2.tar.gz` & `tmp/lst-pressure-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lst-pressure-1.4.2.tar", last modified: Wed Feb 21 07:48:06 2024, max compression
+gzip compressed data, was "lst-pressure-1.5.0.tar", last modified: Fri Apr  5 13:18:44 2024, max compression
```

## Comparing `lst-pressure-1.4.2.tar` & `lst-pressure-1.5.0.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 07:48:06.438024 lst-pressure-1.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-21 07:47:10.000000 lst-pressure-1.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-02-21 07:47:10.000000 lst-pressure-1.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    14569 2024-02-21 07:48:06.438024 lst-pressure-1.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14039 2024-02-21 07:47:10.000000 lst-pressure-1.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 07:48:06.406023 lst-pressure-1.4.2/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-02-21 07:48:06.442024 lst-pressure-1.4.2/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 07:48:06.410023 lst-pressure-1.4.2/cli/apps/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-02-21 07:47:10.000000 lst-pressure-1.4.2/cli/apps/AppInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-02-21 07:48:06.450024 lst-pressure-1.4.2/cli/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 07:48:06.410023 lst-pressure-1.4.2/cli/apps/aggregate/
--rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-02-21 07:48:06.450024 lst-pressure-1.4.2/cli/apps/aggregate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 07:48:06.410023 lst-pressure-1.4.2/cli/apps/observables/
--rw-r--r--   0 runner    (1001) docker     (127)     8929 2024-02-21 07:48:06.450024 lst-pressure-1.4.2/cli/apps/observables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 07:48:06.410023 lst-pressure-1.4.2/conf/
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-02-21 07:48:06.442024 lst-pressure-1.4.2/conf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 07:48:06.410023 lst-pressure-1.4.2/logger/
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-02-21 07:48:06.438024 lst-pressure-1.4.2/logger/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 07:48:06.438024 lst-pressure-1.4.2/lst_pressure.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14569 2024-02-21 07:48:06.000000 lst-pressure-1.4.2/lst_pressure.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-02-21 07:48:06.000000 lst-pressure-1.4.2/lst_pressure.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-21 07:48:06.000000 lst-pressure-1.4.2/lst_pressure.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-21 07:48:06.000000 lst-pressure-1.4.2/lst_pressure.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 07:48:06.414023 lst-pressure-1.4.2/lstpressure/
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-02-21 07:48:06.442024 lst-pressure-1.4.2/lstpressure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 07:48:06.414023 lst-pressure-1.4.2/lstpressure/lst/
--rw-r--r--   0 runner    (1001) docker     (127)    10924 2024-02-21 07:47:10.000000 lst-pressure-1.4.2/lstpressure/lst/LST.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-02-21 07:48:06.446024 lst-pressure-1.4.2/lstpressure/lst/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 07:48:06.414023 lst-pressure-1.4.2/lstpressure/lst/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-02-21 07:48:06.446024 lst-pressure-1.4.2/lstpressure/lst/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-02-21 07:47:10.000000 lst-pressure-1.4.2/lstpressure/lst/helpers/calculate_observables.py
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-02-21 07:47:10.000000 lst-pressure-1.4.2/lstpressure/lst/helpers/calculate_observations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 07:48:06.418023 lst-pressure-1.4.2/lstpressure/lstcalendar/
--rw-r--r--   0 runner    (1001) docker     (127)     8650 2024-02-21 07:47:10.000000 lst-pressure-1.4.2/lstpressure/lstcalendar/LSTCalendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-02-21 07:47:10.000000 lst-pressure-1.4.2/lstpressure/lstcalendar/LSTCalendarDate.py
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-02-21 07:48:06.446024 lst-pressure-1.4.2/lstpressure/lstcalendar/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 07:48:06.418023 lst-pressure-1.4.2/lstpressure/lstindex/
--rw-r--r--   0 runner    (1001) docker     (127)     4183 2024-02-21 07:47:10.000000 lst-pressure-1.4.2/lstpressure/lstindex/LSTIndex.py
--rw-r--r--   0 runner    (1001) docker     (127)     6508 2024-02-21 07:47:10.000000 lst-pressure-1.4.2/lstpressure/lstindex/LSTInterval.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-02-21 07:47:10.000000 lst-pressure-1.4.2/lstpressure/lstindex/LSTIntervalType.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-02-21 07:48:06.446024 lst-pressure-1.4.2/lstpressure/lstindex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 07:48:06.418023 lst-pressure-1.4.2/lstpressure/observable/
--rw-r--r--   0 runner    (1001) docker     (127)     6388 2024-02-21 07:47:10.000000 lst-pressure-1.4.2/lstpressure/observable/Observable.py
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-02-21 07:48:06.442024 lst-pressure-1.4.2/lstpressure/observable/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 07:48:06.422023 lst-pressure-1.4.2/lstpressure/observation/
--rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-02-21 07:47:10.000000 lst-pressure-1.4.2/lstpressure/observation/Observation.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-02-21 07:48:06.446024 lst-pressure-1.4.2/lstpressure/observation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-02-21 07:47:10.000000 lst-pressure-1.4.2/lstpressure/observation/is_observable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 07:48:06.422023 lst-pressure-1.4.2/lstpressure/sun/
--rw-r--r--   0 runner    (1001) docker     (127)     5347 2024-02-21 07:47:10.000000 lst-pressure-1.4.2/lstpressure/sun/Sun.py
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-02-21 07:48:06.442024 lst-pressure-1.4.2/lstpressure/sun/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 07:48:06.422023 lst-pressure-1.4.2/lstpressure/sun/location_providers/
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-02-21 07:47:10.000000 lst-pressure-1.4.2/lstpressure/sun/location_providers/LocationProvider.py
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-02-21 07:48:06.446024 lst-pressure-1.4.2/lstpressure/sun/location_providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 07:48:06.422023 lst-pressure-1.4.2/lstpressure/sun/location_providers/astral_provider/
--rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-02-21 07:47:10.000000 lst-pressure-1.4.2/lstpressure/sun/location_providers/astral_provider/AstralProvider.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-02-21 07:48:06.446024 lst-pressure-1.4.2/lstpressure/sun/location_providers/astral_provider/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 07:48:06.426024 lst-pressure-1.4.2/lstpressure/sun/location_providers/meerkat_provider/
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-02-21 07:47:10.000000 lst-pressure-1.4.2/lstpressure/sun/location_providers/meerkat_provider/AstroUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-02-21 07:47:10.000000 lst-pressure-1.4.2/lstpressure/sun/location_providers/meerkat_provider/DateTimeUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6280 2024-02-21 07:47:10.000000 lst-pressure-1.4.2/lstpressure/sun/location_providers/meerkat_provider/MeerKATProvider.py
--rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-02-21 07:47:10.000000 lst-pressure-1.4.2/lstpressure/sun/location_providers/meerkat_provider/SolarSystemUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-02-21 07:48:06.446024 lst-pressure-1.4.2/lstpressure/sun/location_providers/meerkat_provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-02-21 07:47:10.000000 lst-pressure-1.4.2/lstpressure/sun/location_providers/meerkat_provider/planets.json
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-02-21 07:47:10.000000 lst-pressure-1.4.2/lstpressure/sun/location_providers/normalize_intervals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 07:48:06.430024 lst-pressure-1.4.2/lstpressure/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-02-21 07:48:06.442024 lst-pressure-1.4.2/lstpressure/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-02-21 07:47:10.000000 lst-pressure-1.4.2/lstpressure/utils/normalize_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-02-21 07:47:10.000000 lst-pressure-1.4.2/lstpressure/utils/normalize_date.py
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-02-21 07:47:10.000000 lst-pressure-1.4.2/lstpressure/utils/time_conversions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 07:48:06.430024 lst-pressure-1.4.2/perf/
--rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-02-21 07:48:06.442024 lst-pressure-1.4.2/perf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-21 07:48:06.438024 lst-pressure-1.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-02-21 07:47:10.000000 lst-pressure-1.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 07:48:06.430024 lst-pressure-1.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-21 07:48:06.442024 lst-pressure-1.4.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 07:47:10.000000 lst-pressure-1.4.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 07:48:06.434024 lst-pressure-1.4.2/tests/lstcalendar/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-21 07:48:06.450024 lst-pressure-1.4.2/tests/lstcalendar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-02-21 07:47:10.000000 lst-pressure-1.4.2/tests/lstcalendar/test_LSTCalendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-02-21 07:47:10.000000 lst-pressure-1.4.2/tests/lstcalendar/test_LSTCalendarDate.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-02-21 07:47:10.000000 lst-pressure-1.4.2/tests/lstcalendar/test_LSTInterval.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 07:48:06.434024 lst-pressure-1.4.2/tests/observation/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-21 07:48:06.450024 lst-pressure-1.4.2/tests/observation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-21 07:47:10.000000 lst-pressure-1.4.2/tests/observation/test_Observation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 07:48:06.434024 lst-pressure-1.4.2/tests/sun/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-21 07:48:06.446024 lst-pressure-1.4.2/tests/sun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-02-21 07:47:10.000000 lst-pressure-1.4.2/tests/sun/test_Sun.py
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-02-21 07:47:10.000000 lst-pressure-1.4.2/tests/test_lib_astral.py
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-02-21 07:47:10.000000 lst-pressure-1.4.2/tests/test_lib_meerkat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 07:48:06.434024 lst-pressure-1.4.2/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-21 07:48:06.450024 lst-pressure-1.4.2/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-02-21 07:47:10.000000 lst-pressure-1.4.2/tests/utils/test_normalize_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-02-21 07:47:10.000000 lst-pressure-1.4.2/tests/utils/test_normalize_dates.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-02-21 07:47:10.000000 lst-pressure-1.4.2/tests/utils/test_time_conversions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:18:44.681361 lst-pressure-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    15132 2024-04-05 13:18:44.681361 lst-pressure-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14602 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:18:44.669361 lst-pressure-1.5.0/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-04-05 13:18:44.685361 lst-pressure-1.5.0/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:18:44.669361 lst-pressure-1.5.0/cli/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/cli/apps/AppInterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-05 13:18:44.689361 lst-pressure-1.5.0/cli/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:18:44.669361 lst-pressure-1.5.0/cli/apps/aggregate/
+-rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-04-05 13:18:44.689361 lst-pressure-1.5.0/cli/apps/aggregate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:18:44.669361 lst-pressure-1.5.0/cli/apps/observables/
+-rw-r--r--   0 runner    (1001) docker     (127)     9970 2024-04-05 13:18:44.689361 lst-pressure-1.5.0/cli/apps/observables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:18:44.669361 lst-pressure-1.5.0/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-05 13:18:44.685361 lst-pressure-1.5.0/conf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:18:44.669361 lst-pressure-1.5.0/logger/
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-05 13:18:44.685361 lst-pressure-1.5.0/logger/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:18:44.681361 lst-pressure-1.5.0/lst_pressure.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15132 2024-04-05 13:18:44.000000 lst-pressure-1.5.0/lst_pressure.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-04-05 13:18:44.000000 lst-pressure-1.5.0/lst_pressure.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 13:18:44.000000 lst-pressure-1.5.0/lst_pressure.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-05 13:18:44.000000 lst-pressure-1.5.0/lst_pressure.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:18:44.673361 lst-pressure-1.5.0/lstpressure/
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-05 13:18:44.685361 lst-pressure-1.5.0/lstpressure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:18:44.673361 lst-pressure-1.5.0/lstpressure/lst/
+-rw-r--r--   0 runner    (1001) docker     (127)    10924 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/lstpressure/lst/LST.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-05 13:18:44.685361 lst-pressure-1.5.0/lstpressure/lst/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:18:44.673361 lst-pressure-1.5.0/lstpressure/lst/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-05 13:18:44.689361 lst-pressure-1.5.0/lstpressure/lst/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/lstpressure/lst/helpers/calculate_observables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/lstpressure/lst/helpers/calculate_observations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:18:44.673361 lst-pressure-1.5.0/lstpressure/lstcalendar/
+-rw-r--r--   0 runner    (1001) docker     (127)     9338 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/lstpressure/lstcalendar/LSTCalendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/lstpressure/lstcalendar/LSTCalendarDate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-05 13:18:44.689361 lst-pressure-1.5.0/lstpressure/lstcalendar/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:18:44.673361 lst-pressure-1.5.0/lstpressure/lstindex/
+-rw-r--r--   0 runner    (1001) docker     (127)     4183 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/lstpressure/lstindex/LSTIndex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5560 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/lstpressure/lstindex/LSTInterval.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/lstpressure/lstindex/LSTIntervalType.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-05 13:18:44.685361 lst-pressure-1.5.0/lstpressure/lstindex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:18:44.673361 lst-pressure-1.5.0/lstpressure/observable/
+-rw-r--r--   0 runner    (1001) docker     (127)     6388 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/lstpressure/observable/Observable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-05 13:18:44.685361 lst-pressure-1.5.0/lstpressure/observable/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:18:44.677361 lst-pressure-1.5.0/lstpressure/observation/
+-rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/lstpressure/observation/Observation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-05 13:18:44.685361 lst-pressure-1.5.0/lstpressure/observation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/lstpressure/observation/is_observable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:18:44.677361 lst-pressure-1.5.0/lstpressure/sun/
+-rw-r--r--   0 runner    (1001) docker     (127)     5347 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/lstpressure/sun/Sun.py
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-05 13:18:44.685361 lst-pressure-1.5.0/lstpressure/sun/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:18:44.677361 lst-pressure-1.5.0/lstpressure/sun/location_providers/
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/lstpressure/sun/location_providers/LocationProvider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-05 13:18:44.689361 lst-pressure-1.5.0/lstpressure/sun/location_providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:18:44.677361 lst-pressure-1.5.0/lstpressure/sun/location_providers/astral_provider/
+-rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/lstpressure/sun/location_providers/astral_provider/AstralProvider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-05 13:18:44.689361 lst-pressure-1.5.0/lstpressure/sun/location_providers/astral_provider/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:18:44.677361 lst-pressure-1.5.0/lstpressure/sun/location_providers/meerkat_provider/
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/lstpressure/sun/location_providers/meerkat_provider/AstroUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/lstpressure/sun/location_providers/meerkat_provider/DateTimeUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6280 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/lstpressure/sun/location_providers/meerkat_provider/MeerKATProvider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/lstpressure/sun/location_providers/meerkat_provider/SolarSystemUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-05 13:18:44.689361 lst-pressure-1.5.0/lstpressure/sun/location_providers/meerkat_provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/lstpressure/sun/location_providers/meerkat_provider/planets.json
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/lstpressure/sun/location_providers/normalize_intervals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:18:44.677361 lst-pressure-1.5.0/lstpressure/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-05 13:18:44.685361 lst-pressure-1.5.0/lstpressure/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/lstpressure/utils/normalize_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/lstpressure/utils/normalize_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/lstpressure/utils/time_conversions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:18:44.681361 lst-pressure-1.5.0/perf/
+-rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-04-05 13:18:44.685361 lst-pressure-1.5.0/perf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 13:18:44.681361 lst-pressure-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:18:44.681361 lst-pressure-1.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-05 13:18:44.685361 lst-pressure-1.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:18:44.681361 lst-pressure-1.5.0/tests/lstcalendar/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-05 13:18:44.689361 lst-pressure-1.5.0/tests/lstcalendar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/tests/lstcalendar/test_LSTCalendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/tests/lstcalendar/test_LSTCalendarDate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/tests/lstcalendar/test_LSTInterval.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:18:44.681361 lst-pressure-1.5.0/tests/observation/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-05 13:18:44.689361 lst-pressure-1.5.0/tests/observation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/tests/observation/test_Observation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:18:44.681361 lst-pressure-1.5.0/tests/sun/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-05 13:18:44.689361 lst-pressure-1.5.0/tests/sun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/tests/sun/test_Sun.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/tests/test_lib_astral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/tests/test_lib_meerkat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:18:44.681361 lst-pressure-1.5.0/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-05 13:18:44.689361 lst-pressure-1.5.0/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/tests/utils/test_normalize_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/tests/utils/test_normalize_dates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-05 13:17:54.000000 lst-pressure-1.5.0/tests/utils/test_time_conversions.py
```

### Comparing `lst-pressure-1.4.2/LICENSE` & `lst-pressure-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.4.2/PKG-INFO` & `lst-pressure-1.5.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lst-pressure
-Version: 1.4.2
+Version: 1.5.0
 Summary: Determine periods of "LST pressure" by querying for intersections between LST/Solar intervals
 Home-page: https://github.com/ska-sa/lst-pressure
 Author: Zach Smith
 Author-email: zsmith@sarao.ac.za
 License: Apache 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -141,37 +141,43 @@
 # Print instructions
 lstpressure
 lstpressure <cmd> -h
 
 # Get a list of today's schedulable observations
 cat observations.csv | lstpressure obs
 
+# ... And format the result nicely using csvlook. It's hard to imaging using this tool without --pretty. To use csvlook with custom args, just omit the --pretty flag
+cat observations.csv | lstpressure obs --pretty
+
 # Get a list of schedulable observations over the next 3 months (including this month)
-cat observations.csv | lstpressure obs --end="+2M"
+cat observations.csv | lstpressure obs --end="+2M" --pretty
 
 # Get a list of schedulable NIGHT observations over the next 3 months
-cat observations.csv | lstpressure obs --end="+2M" --filter night
+cat observations.csv | lstpressure obs --end="+2M" --filter night --pretty
+
+# Get a list of schedulable NIGHT observations over the next 3 months, aggregated by opportunities per month
+cat observations.csv | lstpressure obs --end="+2m" --filter night --aggregate observables-by-month.duckdb --pretty
 
-# Get a list of schedulable NIGHT observations over the next 3 months, aggregated on a yes/no basis
-cat observations.csv | lstpressure obs --end="+2m" --filter night --aggregate lst-pressure-3m
+# Get a list of schedulable NIGHT observations over the next 7 days, aggregated by opportunities per day
+cat observations.csv | lstpressure obs --end="+7d" --filter night --aggregate observables-by-day.duckdb --pretty
 
 # Or split the above steps for bespoke SQL aggregation
-cat observations.csv | lstpressure obs --end="+2m" --filter night > night_obs_next_3m.csv
-cat night_obs_next_3m.csv | lstpressure agg --query lst-pressure-3m
+cat observations.csv | lstpressure obs --end="+2m" --filter night > night_obs_next_3m.csv --pretty
+cat night_obs_next_3m.csv | lstpressure agg --query observables-by-month.duckdb --pretty
 
 # Use the DuckDB query engine by specifying a query that includes "duckdb", or including "duckdb" in a comment in a query
-cat night_obs_next_3m.csv | lstpressure agg --query observables-by-month.duckdb
+cat night_obs_next_3m.csv | lstpressure agg --query observables-by-month.duckdb --pretty
 # or..
-cat night_obs_next_3m.csv | lstpressure agg --query "select * from stdin -- duckdb"
+cat night_obs_next_3m.csv | lstpressure agg --query "select * from stdin -- duckdb" --pretty
 
 # Write bespoke aggregations (SQLite syntax, in the case of multiple statements, the last is returned)
-cat night_obs_next_3m.csv | lstpressure agg --query "select * from stdin;"
+cat night_obs_next_3m.csv | lstpressure agg --query "select * from stdin;" --pretty
 
-# Interrogate what the "lst-pressure-3m" query looks like
-lstpressure agg --query lst-pressure-3m --echo
+# Interrogate what the "observables-by-month.duckdb" query looks like
+lstpressure agg --query observables-by-month.duckdb --echo
 
 # .. Write your own SQL in a file
 # Using the CLI via the Docker image requires filepaths to be specified as absolute paths, i.e. --query $(pwd)/my-report.sql
 echo "select * from stdin;" > my-report.sql
 cat night_obs_next_3m.csv | lstpressure agg --query $(pwd)/my-report.sql # or ...
 cat observations.csv | lstpressure obs --end="+2m" --filter night --aggregate $(pwd)/my-report.sql
 ```
```

### Comparing `lst-pressure-1.4.2/README.md` & `lst-pressure-1.5.0/lst_pressure.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: lst-pressure
+Version: 1.5.0
+Summary: Determine periods of "LST pressure" by querying for intersections between LST/Solar intervals
+Home-page: https://github.com/ska-sa/lst-pressure
+Author: Zach Smith
+Author-email: zsmith@sarao.ac.za
+License: Apache 2.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.12
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # lst-pressure
 
 Python module for calculating LST pressure based on scheduled observations
 
 <!-- START doctoc generated TOC please keep comment here to allow auto update -->
 <!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
 
@@ -126,37 +141,43 @@
 # Print instructions
 lstpressure
 lstpressure <cmd> -h
 
 # Get a list of today's schedulable observations
 cat observations.csv | lstpressure obs
 
+# ... And format the result nicely using csvlook. It's hard to imaging using this tool without --pretty. To use csvlook with custom args, just omit the --pretty flag
+cat observations.csv | lstpressure obs --pretty
+
 # Get a list of schedulable observations over the next 3 months (including this month)
-cat observations.csv | lstpressure obs --end="+2M"
+cat observations.csv | lstpressure obs --end="+2M" --pretty
 
 # Get a list of schedulable NIGHT observations over the next 3 months
-cat observations.csv | lstpressure obs --end="+2M" --filter night
+cat observations.csv | lstpressure obs --end="+2M" --filter night --pretty
+
+# Get a list of schedulable NIGHT observations over the next 3 months, aggregated by opportunities per month
+cat observations.csv | lstpressure obs --end="+2m" --filter night --aggregate observables-by-month.duckdb --pretty
 
-# Get a list of schedulable NIGHT observations over the next 3 months, aggregated on a yes/no basis
-cat observations.csv | lstpressure obs --end="+2m" --filter night --aggregate lst-pressure-3m
+# Get a list of schedulable NIGHT observations over the next 7 days, aggregated by opportunities per day
+cat observations.csv | lstpressure obs --end="+7d" --filter night --aggregate observables-by-day.duckdb --pretty
 
 # Or split the above steps for bespoke SQL aggregation
-cat observations.csv | lstpressure obs --end="+2m" --filter night > night_obs_next_3m.csv
-cat night_obs_next_3m.csv | lstpressure agg --query lst-pressure-3m
+cat observations.csv | lstpressure obs --end="+2m" --filter night > night_obs_next_3m.csv --pretty
+cat night_obs_next_3m.csv | lstpressure agg --query observables-by-month.duckdb --pretty
 
 # Use the DuckDB query engine by specifying a query that includes "duckdb", or including "duckdb" in a comment in a query
-cat night_obs_next_3m.csv | lstpressure agg --query observables-by-month.duckdb
+cat night_obs_next_3m.csv | lstpressure agg --query observables-by-month.duckdb --pretty
 # or..
-cat night_obs_next_3m.csv | lstpressure agg --query "select * from stdin -- duckdb"
+cat night_obs_next_3m.csv | lstpressure agg --query "select * from stdin -- duckdb" --pretty
 
 # Write bespoke aggregations (SQLite syntax, in the case of multiple statements, the last is returned)
-cat night_obs_next_3m.csv | lstpressure agg --query "select * from stdin;"
+cat night_obs_next_3m.csv | lstpressure agg --query "select * from stdin;" --pretty
 
-# Interrogate what the "lst-pressure-3m" query looks like
-lstpressure agg --query lst-pressure-3m --echo
+# Interrogate what the "observables-by-month.duckdb" query looks like
+lstpressure agg --query observables-by-month.duckdb --echo
 
 # .. Write your own SQL in a file
 # Using the CLI via the Docker image requires filepaths to be specified as absolute paths, i.e. --query $(pwd)/my-report.sql
 echo "select * from stdin;" > my-report.sql
 cat night_obs_next_3m.csv | lstpressure agg --query $(pwd)/my-report.sql # or ...
 cat observations.csv | lstpressure obs --end="+2m" --filter night --aggregate $(pwd)/my-report.sql
 ```
```

### Comparing `lst-pressure-1.4.2/cli/__init__.py` & `lst-pressure-1.5.0/cli/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,19 +29,30 @@
     prog = "lstpressure"
     description = f"(NRF SARAO) LST Pressure v{version}"
 
     parser = argparse.ArgumentParser(
         prog=prog, description=description, formatter_class=CustomHelpFormatter
     )
     parser.add_argument("-v", "--version", action="version", version=version)
-    parser.add_argument("--debug", action="store_true", help='Show logs of "DEBUG" level or higher')
     parser.add_argument(
-        "--info", action="store_true", help='Show logs of "INFO" level or higher (default)'
+        "--debug", action="store_true", help='Show logs of "DEBUG" level or higher'
+    )
+    parser.add_argument(
+        "--info",
+        action="store_true",
+        help='Show logs of "INFO" level or higher (default)',
+    )
+    parser.add_argument(
+        "--warn", action="store_true", help='Show logs of "WARN" level or higher'
+    )
+    parser.add_argument(
+        "--update",
+        action="store_true",
+        help="Output instructions for updating lstpressure",
     )
-    parser.add_argument("--warn", action="store_true", help='Show logs of "WARN" level or higher')
 
     module_parser = parser.add_subparsers(title="Modules", dest="command")
 
     # Build the CLI
     apps = {
         app.id[0:3]: app(
             module_parser.add_parser(
@@ -52,14 +63,22 @@
                 aliases=[app.id[0:3]],
             )
         )
         for app in app_lib
     }
     args = parser.parse_args()
 
+    if args.update:
+        print(
+            """(Docker) Please run the following command to pull the most recent Docker image:
+    => docker pull ghcr.io/ska-sa/lst-pressure_dist:latest
+"""
+        )
+        return
+
     # Override environment configuration
     if args.warn:
         conf.LOG_LEVEL = LogLevel.WARN
     if args.info:
         conf.LOG_LEVEL = LogLevel.INFO
     if args.debug:
         conf.LOG_LEVEL = LogLevel.DEBUG
@@ -75,8 +94,8 @@
         parser.print_help()
         return
 
     # Otherwise execute the application
     app.parse(args).exe()
 
 # Automatically added by katversion
-__version__ = '1.4.2'
+__version__ = '1.5.0'
```

### Comparing `lst-pressure-1.4.2/cli/apps/AppInterface.py` & `lst-pressure-1.5.0/cli/apps/AppInterface.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.4.2/cli/apps/aggregate/__init__.py` & `lst-pressure-1.5.0/cli/apps/aggregate/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -35,28 +35,41 @@
             "--query",
             required=True,
             type=str,
             metavar="",
             help=f'SQL string to apply to input CSV (i.e. "select * from stdin"), or apply a built-in aggregation: {quoted_existing_reports}. By default the SQLite engine is used, and you can enable the DuckDB engine by including "duckdb" either in a filename or as a comment somewhere in the query text',
         )
         self.parser.add_argument(
+            "--pretty",
+            required=False,
+            default=False,
+            action="store_true",
+            help=f"Format CSV output using the csvlook tool (included in this CLI)",
+        )
+        self.parser.add_argument(
             "--echo",
             required=False,
             default=False,
             action="store_true",
             help=f"Echo the aggregation query back - useful for evaluating .sql file contents that would otherwise be opaque. For example: --echo --query {existing_reports[0]}",
         )
 
         return self
 
     def parse(self, args) -> Self:
         self.args = args
         self.echo = args.echo
         self.input = args.input
         self.query = parse_sql_query(args.query)
+        self.pretty = args.pretty
+
+        if self.echo and self.pretty:
+            error("Don't use --pretty and --echo together.")
+            exit(1)
+
         return self
 
     def exe(self) -> None:
         if self.echo:
             print(self.query)
             exit()
 
@@ -69,14 +82,15 @@
                 )
                 exit(1)
         else:
             with open(self.input, "r") as file:
                 input_csv = file.read()
 
         result = execute_csvsql(input_csv, self.query, self.args.query)
+        result = execute_csvlook(result) if self.pretty else result
 
         # Print result to stdout
         print(result)
         exit()
 
 
 def parse_sql_query(str_input):
@@ -98,14 +112,45 @@
         with open(path + ".sql", "r") as file:
             return file.read().strip()
 
     # If not a file, assume it's a SQL string
     return str_input
 
 
+def execute_csvlook(input_content):
+    csvlook_opts = [
+        "-I",
+        "--null-value",
+        "0",
+    ]
+
+    command = ["csvlook", *csvlook_opts]
+
+    try:
+        # Use subprocess.Popen to run the command
+        process = subprocess.Popen(
+            command, stdin=subprocess.PIPE, stdout=subprocess.PIPE, text=True
+        )
+
+        # Pass input content to the subprocess
+        output, _ = process.communicate(input=input_content)
+
+        # Wait for the process to finish and get the return code
+        return_code = process.wait()
+
+        if return_code == 0:
+            return output
+        else:
+            error(f"csvlook process returned a non-zero exit code: {return_code}")
+            error(f"Command output: {output}")
+            return None
+    except Exception as e:
+        raise e
+
+
 def execute_csvsql(input_content, sql, query_name=""):
     duck_opts = (
         [
             "--db",
             "duckdb:///:memory:",
             "--insert",
         ]
@@ -133,11 +178,11 @@
             error(f"csvsql process returned a non-zero exit code: {return_code}")
             error(f"Command output: {output}")
             return None
     except Exception as e:
         raise e
 
 
-__all__ = ["parse_sql_query", "Aggregate", "execute_csvsql"]
+__all__ = ["parse_sql_query", "Aggregate", "execute_csvsql", "execute_csvlook"]
 
 # Automatically added by katversion
-__version__ = '1.4.2'
+__version__ = '1.5.0'
```

### Comparing `lst-pressure-1.4.2/cli/apps/observables/__init__.py` & `lst-pressure-1.5.0/cli/apps/observables/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 from typing import Self
 from datetime import datetime, timedelta
 import re
 from conf import Conf, LocationProviderType
 from lstpressure import LSTIntervalType as I, Observation, LST
 from ..AppInterface import AppInterface
-from ..aggregate import parse_sql_query, execute_csvsql, quoted_existing_reports
+from ..aggregate import (
+    parse_sql_query,
+    execute_csvsql,
+    execute_csvlook,
+    quoted_existing_reports,
+)
 from logger import error
 import sys
 import pandas as pd
 from io import StringIO
 
 conf = Conf()
 
@@ -63,15 +68,19 @@
 
             year = current_date.year + new_month // 12
             month = new_month % 12 + 1
             day = min(
                 current_date.day,
                 [
                     31,
-                    29 if year % 4 == 0 and not year % 100 == 0 or year % 400 == 0 else 28,
+                    (
+                        29
+                        if year % 4 == 0 and not year % 100 == 0 or year % 400 == 0
+                        else 28
+                    ),
                     31,
                     30,
                     31,
                     30,
                     31,
                     31,
                     30,
@@ -93,15 +102,17 @@
     # If the input format is unrecognized
     raise ValueError("Invalid input format")
 
 
 class Observables(AppInterface):
     id = "observables"
     usage = "lstpressure observables -h"
-    description = "Generate a list of observables (slots where OPT observations can be observed)"
+    description = (
+        "Generate a list of observables (slots where OPT observations can be observed)"
+    )
 
     def __init__(self, parser) -> None:
         super().__init__(parser)
 
     def build(self) -> Self:
         self.parser.add_argument(
             "--start",
@@ -141,22 +152,27 @@
             type=lambda s: s.upper(),
             choices=list(LocationProviderType.__members__),
             default="MEERKAT",
             help="Specify the location provider for calculating sun statistics and for calculating intervals. Choose between: ASTRAL or MEERKAT (default). MeerKAT: intervals calculated using sunrise/sunset values (including NIGHT), ASTRAL: intervals calculated using dawn, sunrise, sunset, dusk",
             metavar="",
         )
 
+        filter_choices = [
+            choice
+            for choice in list(I.__members__)
+            if choice.upper() != I.OBSERVATION_WINDOW.name.upper()
+        ]
         self.parser.add_argument(
             "--filter",
             type=lambda s: kebab_to_snake(s.upper()),
-            choices=list(I.__members__),
+            choices=filter_choices,
             default=None,
             required=False,
             metavar="",
-            help=f"Select from: {', '.join(list(I.__members__))}",
+            help=f"Select from: {', '.join(filter_choices)}. If multiple filters are passed, only the last filter value is used (multiple filters not supported)",
         )
 
         self.parser.add_argument(
             "--lat",
             metavar="D:M:S",
             default=None,
             nargs="?",
@@ -174,15 +190,23 @@
         )
 
         self.parser.add_argument(
             "--aggregate",
             required=False,
             type=str,
             metavar="",
-            help=f'Apply a SQL aggregation to the CSV before printing to a file/stdout, or apply a built-in aggregation: {quoted_existing_reports}. The CSV is provided as a relation called "stdin"',
+            help=f'Apply a SQL aggregation to the CSV before printing to a file/stdout, or apply a built-in aggregation: {quoted_existing_reports}. The CSV is provided as a relation called "stdin". SQLite and DuckDB engines are supported, include ".duckdb" in the filename or as a comment in the SQL to enable DuckDB engine. Functionality is provided by the excellent csvsql library',
+        )
+
+        self.parser.add_argument(
+            "--pretty",
+            required=False,
+            default=False,
+            action="store_true",
+            help=f"Format CSV output using the csvlook tool (included in this CLI)",
         )
 
         return self
 
     def parse(self, args) -> Self:
         if args.lat or args.long:
             if LocationProviderType[args.loc_provider] == LocationProviderType.MEERKAT:
@@ -201,22 +225,25 @@
         self.input = args.input
         self.start = parseDateInput(args.start)
         self.end = parseDateInput(args.end, self.start) if args.end else self.start
         conf.LOC_PROVIDER = LocationProviderType[args.loc_provider]
 
         filter_name = args.filter
         if filter_name and not filter_mapping.get(filter_name.upper()):
-            error(f"Invalid filter name, valid options: {', '.join(list(filter_mapping.keys()))}")
+            error(
+                f"Invalid filter name, valid options: {', '.join(list(filter_mapping.keys()))}"
+            )
             exit(1)
         self.filter_value = (
             None if not filter_name else filter_mapping.get(filter_name.upper(), None)
         )
 
         self.output = args.output if args.output else None
         self.aggregate = args.aggregate if args.aggregate else None
+        self.pretty = args.pretty if args.pretty else None
         return self
 
     def exe(self) -> None:
         sql = parse_sql_query(self.aggregate) if self.aggregate else None
 
         def observation_filter(observation: Observation):
             if self.filter_value in observation.utc_constraints:
@@ -241,18 +268,22 @@
             calendar_end=self.end,
             observation_filter=observation_filter if self.filter_value else None,
             latitude=conf.LATITUDE,
             longitude=conf.LONGITUDE,
         ).to_csv_string()
 
         output_string = (
-            execute_csvsql(output_csv_string, sql, self.aggregate) if sql else output_csv_string
+            execute_csvsql(output_csv_string, sql, self.aggregate)
+            if sql
+            else output_csv_string
         )
 
+        output_string = execute_csvlook(output_string) if self.pretty else output_string
+
         if self.output:
             with open(self.output, "w") as f:
                 f.write(output_string)
         else:
             print(output_string)
 
 # Automatically added by katversion
-__version__ = '1.4.2'
+__version__ = '1.5.0'
```

### Comparing `lst-pressure-1.4.2/conf/__init__.py` & `lst-pressure-1.5.0/conf/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,8 +91,8 @@
     def PY_ENV(self, value):
         self._py_env = value
 
 
 __all__ = ["Conf", "LogLevel"]
 
 # Automatically added by katversion
-__version__ = '1.4.2'
+__version__ = '1.5.0'
```

### Comparing `lst-pressure-1.4.2/logger/__init__.py` & `lst-pressure-1.5.0/logger/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,8 +27,8 @@
 def error(*args, **kwargs):
     print("ERROR", *args, **kwargs, file=sys.stderr)
 
 
 __all__ = ["debug", "info", "warn", "error"]
 
 # Automatically added by katversion
-__version__ = '1.4.2'
+__version__ = '1.5.0'
```

### Comparing `lst-pressure-1.4.2/lst_pressure.egg-info/PKG-INFO` & `lst-pressure-1.5.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: lst-pressure
-Version: 1.4.2
-Summary: Determine periods of "LST pressure" by querying for intersections between LST/Solar intervals
-Home-page: https://github.com/ska-sa/lst-pressure
-Author: Zach Smith
-Author-email: zsmith@sarao.ac.za
-License: Apache 2.0
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.12
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # lst-pressure
 
 Python module for calculating LST pressure based on scheduled observations
 
 <!-- START doctoc generated TOC please keep comment here to allow auto update -->
 <!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
 
@@ -141,37 +126,43 @@
 # Print instructions
 lstpressure
 lstpressure <cmd> -h
 
 # Get a list of today's schedulable observations
 cat observations.csv | lstpressure obs
 
+# ... And format the result nicely using csvlook. It's hard to imaging using this tool without --pretty. To use csvlook with custom args, just omit the --pretty flag
+cat observations.csv | lstpressure obs --pretty
+
 # Get a list of schedulable observations over the next 3 months (including this month)
-cat observations.csv | lstpressure obs --end="+2M"
+cat observations.csv | lstpressure obs --end="+2M" --pretty
 
 # Get a list of schedulable NIGHT observations over the next 3 months
-cat observations.csv | lstpressure obs --end="+2M" --filter night
+cat observations.csv | lstpressure obs --end="+2M" --filter night --pretty
+
+# Get a list of schedulable NIGHT observations over the next 3 months, aggregated by opportunities per month
+cat observations.csv | lstpressure obs --end="+2m" --filter night --aggregate observables-by-month.duckdb --pretty
 
-# Get a list of schedulable NIGHT observations over the next 3 months, aggregated on a yes/no basis
-cat observations.csv | lstpressure obs --end="+2m" --filter night --aggregate lst-pressure-3m
+# Get a list of schedulable NIGHT observations over the next 7 days, aggregated by opportunities per day
+cat observations.csv | lstpressure obs --end="+7d" --filter night --aggregate observables-by-day.duckdb --pretty
 
 # Or split the above steps for bespoke SQL aggregation
-cat observations.csv | lstpressure obs --end="+2m" --filter night > night_obs_next_3m.csv
-cat night_obs_next_3m.csv | lstpressure agg --query lst-pressure-3m
+cat observations.csv | lstpressure obs --end="+2m" --filter night > night_obs_next_3m.csv --pretty
+cat night_obs_next_3m.csv | lstpressure agg --query observables-by-month.duckdb --pretty
 
 # Use the DuckDB query engine by specifying a query that includes "duckdb", or including "duckdb" in a comment in a query
-cat night_obs_next_3m.csv | lstpressure agg --query observables-by-month.duckdb
+cat night_obs_next_3m.csv | lstpressure agg --query observables-by-month.duckdb --pretty
 # or..
-cat night_obs_next_3m.csv | lstpressure agg --query "select * from stdin -- duckdb"
+cat night_obs_next_3m.csv | lstpressure agg --query "select * from stdin -- duckdb" --pretty
 
 # Write bespoke aggregations (SQLite syntax, in the case of multiple statements, the last is returned)
-cat night_obs_next_3m.csv | lstpressure agg --query "select * from stdin;"
+cat night_obs_next_3m.csv | lstpressure agg --query "select * from stdin;" --pretty
 
-# Interrogate what the "lst-pressure-3m" query looks like
-lstpressure agg --query lst-pressure-3m --echo
+# Interrogate what the "observables-by-month.duckdb" query looks like
+lstpressure agg --query observables-by-month.duckdb --echo
 
 # .. Write your own SQL in a file
 # Using the CLI via the Docker image requires filepaths to be specified as absolute paths, i.e. --query $(pwd)/my-report.sql
 echo "select * from stdin;" > my-report.sql
 cat night_obs_next_3m.csv | lstpressure agg --query $(pwd)/my-report.sql # or ...
 cat observations.csv | lstpressure obs --end="+2m" --filter night --aggregate $(pwd)/my-report.sql
 ```
```

### Comparing `lst-pressure-1.4.2/lst_pressure.egg-info/SOURCES.txt` & `lst-pressure-1.5.0/lst_pressure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.4.2/lstpressure/__init__.py` & `lst-pressure-1.5.0/lstpressure/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,8 +34,8 @@
     "Sun",
     "utils",
     "LSTConf",
     "LocationProviderType",
 ]
 
 # Automatically added by katversion
-__version__ = '1.4.2'
+__version__ = '1.5.0'
```

### Comparing `lst-pressure-1.4.2/lstpressure/lst/LST.py` & `lst-pressure-1.5.0/lstpressure/lst/LST.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.4.2/lstpressure/lst/helpers/calculate_observables.py` & `lst-pressure-1.5.0/lstpressure/lst/helpers/calculate_observables.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.4.2/lstpressure/lst/helpers/calculate_observations.py` & `lst-pressure-1.5.0/lstpressure/lst/helpers/calculate_observations.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 import math
 from typing import Tuple
 from perf import track_total_runtime
 
 
 def convert_to_hours(x):
     try:
-        result = round((int(x.split(":")[0]) * 3600 + int(x.split(":")[1]) * 60) / 3600, 2)
+        result = round(
+            (int(x.split(":")[0]) * 3600 + int(x.split(":")[1]) * 60) / 3600, 2
+        )
         return result
     except:
         return None
 
 
 @track_total_runtime
 def calculate_constraints(row) -> list[I]:
@@ -43,18 +45,19 @@
 
         # Build observations using list comprehension for efficiency
         observations = [
             Observation(
                 id=row["id"],
                 lst_window_start=row["lst_start_hours"],
                 lst_window_end=row["lst_end_hours"],
-                utc_constraints=calculate_constraints(row),
+                utc_constraints=constraint,
                 duration=row["duration_hours"],
                 proposal_id=row["proposal_id"],
             )
             for _, row in dataFrame.iterrows()
             if row["lst_end_hours"] - row["lst_start_hours"] > 0
+            for constraint in calculate_constraints(row)
         ]
 
         return tuple(filter(observation_filter, observations))
     except Exception as e:
         raise ValueError("Error parsing CSV - please check input.", e)
```

### Comparing `lst-pressure-1.4.2/lstpressure/lstcalendar/LSTCalendar.py` & `lst-pressure-1.5.0/lstpressure/lstcalendar/LSTCalendar.py`

 * *Files 15% similar despite different names*

```diff
@@ -167,24 +167,37 @@
         Returns
         -------
         LSTCalendar
             The LSTCalendar object.
         """
         self._observations = []
         self._observations_index = LSTIndex()
-        _ids = set()
+        _primary_keys = set()
         for observation in observations:
-            if observation.id in _ids:
+            # Create a composite key using both id and utc_constraints
+            composite_key = (
+                observation.id,
+                "".join([c.name for c in observation.utc_constraints]),
+            )
+
+            # Check if the composite key is already in the set
+            if composite_key in _primary_keys:
                 raise ValueError(
-                    f"Duplicate ID detected: '{observation.id}'. "
-                    "Each observation must have a unique ID to be loaded into the calendar."
+                    f"Duplicate composite key detected: ID '{observation.id}' with UTC constraints '{observation.utc_constraints}'. "
+                    "Each observation must have a unique combination of ID and UTC constraints to be loaded into the calendar."
                 )
-            _ids.add(observation.id)
+
+            # Add the composite key to the set for future checks
+            _primary_keys.add(composite_key)
+
+            # Assign the calendar to the observation and append it to the calendar's list of observations
             observation.calendar = self
             self._observations.append(observation)
+
+            # Insert intervals from the observation into the calendar's observation index
             for interval in observation.intervals:
                 self.observations_index.insert(interval.interval)
         return self
 
     @property
     def observations(self) -> list[Dict[str, LSTInterval | Observation]]:
         """
@@ -209,15 +222,17 @@
 
         Returns
         -------
         None
         """
         self.load_observations(observations)
 
-    def observables(self, observations: Optional[list[Observation]] = None) -> list[Observable]:
+    def observables(
+        self, observations: Optional[list[Observation]] = None
+    ) -> list[Observable]:
         """
         Retrieve observable observations for the dates maintained by this calendar.
 
         This method processes a list of dates within the calendar and aggregates their observable observations into observation windows. If a list of observations is provided, it replaces the current observations of the calendar with the new list.
 
         Parameters
         ----------
```

### Comparing `lst-pressure-1.4.2/lstpressure/lstcalendar/LSTCalendarDate.py` & `lst-pressure-1.5.0/lstpressure/lstcalendar/LSTCalendarDate.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.4.2/lstpressure/lstindex/LSTIndex.py` & `lst-pressure-1.5.0/lstpressure/lstindex/LSTIndex.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.4.2/lstpressure/lstindex/LSTInterval.py` & `lst-pressure-1.5.0/lstpressure/lstindex/LSTInterval.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,18 @@
 
 from datetime import datetime
 from intervaltree import Interval
 from .LSTIntervalType import LSTIntervalType
 from ..lstcalendar import LSTCalendarDate
 from ..sun import Sun
 from ..observation import Observation
-from typing import Optional, Union  # TODO The new | type (instead of Union doesn't work here)
+from typing import (
+    Optional,
+    Union,
+)  # TODO The new | type (instead of Union doesn't work here)
 from ..utils import normalize_yyyymmdd_to_datetime
 from perf import track_total_runtime, decorate_all
 
 
 @track_total_runtime
 def normalize_interval(start, end, days=1):
     """
@@ -38,45 +41,14 @@
         end += 24
     end += 24 * (days - 1)
     return (start, end)
 
 
 @decorate_all(track_total_runtime)
 class LSTInterval:
-    """
-    A wrapper around the intervaltree Interval class for easier access in the context of lst-pressure.
-
-    Attributes
-    ----------
-    parent : LSTCalendarDate | Observation, optional
-        The parent object associated with the interval.
-    interval : Interval
-        The underlying interval object.
-    start : float
-        The start time of the interval (in hours).
-    start_utc : datetime | float
-        The start time of the interval in UTC.
-    end : float
-        The end time of the interval (in hours).
-    end_utc : datetime | float
-        The end time of the interval in UTC.
-    type : LSTIntervalType, optional
-        The type of the interval.
-    dt : datetime, optional
-        The datetime associated with the interval.
-    sun : Sun, optional
-        The Sun object associated with the interval.
-    tomorrow_sun : Sun, optional
-        The Sun object associated with the next day.
-
-    Methods
-    -------
-    None
-    """
-
     def __init__(
         self,
         start: float,
         end: float,
         start_utc: datetime | float,
         end_utc: datetime | float,
         parent: Optional[Union[LSTCalendarDate, Observation]] = None,
```

### Comparing `lst-pressure-1.4.2/lstpressure/lstindex/LSTIntervalType.py` & `lst-pressure-1.5.0/lstpressure/lstindex/LSTIntervalType.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.4.2/lstpressure/observable/Observable.py` & `lst-pressure-1.5.0/lstpressure/observable/Observable.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.4.2/lstpressure/observation/Observation.py` & `lst-pressure-1.5.0/lstpressure/observation/Observation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 lstpressure.observation.Observation
 """
+
 from typing import Optional, Tuple
 from ..lstcalendar.LSTCalendarDate import LSTCalendar, Observable
 from ..lstindex import LSTIntervalType, LSTInterval, normalize_interval
 from perf import track_total_runtime, decorate_all
 
 
 @decorate_all(track_total_runtime)
@@ -25,15 +26,15 @@
     """
 
     def __init__(
         self,
         id: any,
         lst_window_start: float,
         lst_window_end: float,
-        utc_constraints: list[LSTIntervalType] = None,
+        utc_constraints: LSTIntervalType | list[LSTIntervalType] = None,
         duration: float = None,
         proposal_id: str = None,
     ) -> None:
         """
         Initializes an instance of Block.
 
         Parameters
@@ -46,30 +47,36 @@
             The ending value of the LST window.
         utc_constraints : list[LSTInterval]
             The UTC constraints for the observation block represented as a list of LSTInterval values. Defaults to 0.
         """
         self.id = id
         self.lst_window_start = lst_window_start
         self.lst_window_end = lst_window_end
-        self.utc_constraints = utc_constraints
+        self.utc_constraints = (
+            utc_constraints
+            if utc_constraints and isinstance(utc_constraints, list)
+            else [utc_constraints]
+        )
         self.proposal_id = proposal_id
         self._duration = duration if duration else 0
         self._cal: Optional[LSTCalendar] = None  # Reference to the calendar
         self._intervals = []
         self._intervals.append(
             LSTInterval(
                 *normalize_interval(self.lst_window_start, self.lst_window_end),
                 None,
                 None,
                 parent=self,
                 type=LSTIntervalType.OBSERVATION_WINDOW,
             )
         )
         if self.lst_window_end < self.lst_window_start:
-            self._intervals.append(LSTInterval(0, self.lst_window_end, None, None, self))
+            self._intervals.append(
+                LSTInterval(0, self.lst_window_end, None, None, self)
+            )
 
     @property
     def duration(self) -> float:
         """
         Required observation duration in hours (decimal)
         """
         return self._duration
@@ -87,35 +94,40 @@
     @calendar.setter
     def calendar(self, cal: LSTCalendar):
         self._cal = cal
 
     def __hash__(self) -> int:
         return hash((self.id, self.lst_window_start, self.lst_window_end))
 
-    def observables(self, lstcalendar: Optional[LSTCalendar] = None) -> Tuple[Observable]:
+    def observables(
+        self, lstcalendar: Optional[LSTCalendar] = None
+    ) -> Tuple[Observable]:
         lstcalendar = self._cal if not lstcalendar else lstcalendar
 
         if not lstcalendar:
             raise ValueError(
                 "'lstcalendar' is not specified. To check observability, either associate this observation with an existing LSTCalendar instance or pass an LSTCalendar instance as an argument to this method."
             )
 
         results = set()
 
         # Note that overlap() returns a set
         query_result = set()
         for obs_window in self.intervals:
-            query_result = query_result | lstcalendar.interval_index.overlap(obs_window.interval)
+            query_result = query_result | lstcalendar.interval_index.overlap(
+                obs_window.interval
+            )
 
             for cal_interval_raw in query_result:
                 cal_interval_start, cal_interval_end, cal_interval = cal_interval_raw
                 interval_type = cal_interval.type
 
                 if (self.utc_constraints is None or len(self.utc_constraints) == 0) or (
-                    len(self.utc_constraints) > 0 and interval_type in self.utc_constraints
+                    len(self.utc_constraints) > 0
+                    and interval_type in self.utc_constraints
                 ):
                     if obs_window.end > cal_interval_start:
                         if (
                             obs_window.start + self.duration < cal_interval_end
                             or obs_window.end + self.duration < cal_interval_end
                         ):
                             results.add(Observable(cal_interval, self))
```

### Comparing `lst-pressure-1.4.2/lstpressure/observation/is_observable.py` & `lst-pressure-1.5.0/lstpressure/observation/is_observable.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.4.2/lstpressure/sun/Sun.py` & `lst-pressure-1.5.0/lstpressure/sun/Sun.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.4.2/lstpressure/sun/location_providers/astral_provider/AstralProvider.py` & `lst-pressure-1.5.0/lstpressure/sun/location_providers/astral_provider/AstralProvider.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.4.2/lstpressure/sun/location_providers/meerkat_provider/AstroUtils.py` & `lst-pressure-1.5.0/lstpressure/sun/location_providers/meerkat_provider/AstroUtils.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.4.2/lstpressure/sun/location_providers/meerkat_provider/DateTimeUtils.py` & `lst-pressure-1.5.0/lstpressure/sun/location_providers/meerkat_provider/DateTimeUtils.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.4.2/lstpressure/sun/location_providers/meerkat_provider/MeerKATProvider.py` & `lst-pressure-1.5.0/lstpressure/sun/location_providers/meerkat_provider/MeerKATProvider.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.4.2/lstpressure/sun/location_providers/meerkat_provider/SolarSystemUtils.py` & `lst-pressure-1.5.0/lstpressure/sun/location_providers/meerkat_provider/SolarSystemUtils.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.4.2/lstpressure/utils/normalize_coordinates.py` & `lst-pressure-1.5.0/lstpressure/utils/normalize_coordinates.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.4.2/lstpressure/utils/normalize_date.py` & `lst-pressure-1.5.0/lstpressure/utils/normalize_date.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.4.2/lstpressure/utils/time_conversions.py` & `lst-pressure-1.5.0/lstpressure/utils/time_conversions.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.4.2/perf/__init__.py` & `lst-pressure-1.5.0/perf/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,8 +106,8 @@
 
     return decorate
 
 
 __all__ = ["monitor_perf", "track_total_runtime", "decorate_all"]
 
 # Automatically added by katversion
-__version__ = '1.4.2'
+__version__ = '1.5.0'
```

### Comparing `lst-pressure-1.4.2/setup.py` & `lst-pressure-1.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.4.2/tests/lstcalendar/test_LSTCalendar.py` & `lst-pressure-1.5.0/tests/lstcalendar/test_LSTCalendar.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.4.2/tests/lstcalendar/test_LSTCalendarDate.py` & `lst-pressure-1.5.0/tests/lstcalendar/test_LSTCalendarDate.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.4.2/tests/lstcalendar/test_LSTInterval.py` & `lst-pressure-1.5.0/tests/lstcalendar/test_LSTInterval.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.4.2/tests/sun/test_Sun.py` & `lst-pressure-1.5.0/tests/sun/test_Sun.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.4.2/tests/test_lib_astral.py` & `lst-pressure-1.5.0/tests/test_lib_astral.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.4.2/tests/test_lib_meerkat.py` & `lst-pressure-1.5.0/tests/test_lib_meerkat.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.4.2/tests/utils/test_normalize_coordinates.py` & `lst-pressure-1.5.0/tests/utils/test_normalize_coordinates.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.4.2/tests/utils/test_normalize_dates.py` & `lst-pressure-1.5.0/tests/utils/test_normalize_dates.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.4.2/tests/utils/test_time_conversions.py` & `lst-pressure-1.5.0/tests/utils/test_time_conversions.py`

 * *Files identical despite different names*

