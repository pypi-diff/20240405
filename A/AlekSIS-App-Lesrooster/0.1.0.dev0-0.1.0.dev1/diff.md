# Comparing `tmp/aleksis_app_lesrooster-0.1.0.dev0.tar.gz` & `tmp/aleksis_app_lesrooster-0.1.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aleksis_app_lesrooster-0.1.0.dev0.tar", max compression
+gzip compressed data, was "aleksis_app_lesrooster-0.1.0.dev1.tar", max compression
```

## Comparing `aleksis_app_lesrooster-0.1.0.dev0.tar` & `aleksis_app_lesrooster-0.1.0.dev1.tar`

### file list

```diff
@@ -1,75 +1,76 @@
--rw-r--r--   0        0        0      442 2023-01-30 16:25:16.564535 aleksis_app_lesrooster-0.1.0.dev0/CHANGELOG.rst
--rw-r--r--   0        0        0    14361 2023-01-30 16:25:16.576535 aleksis_app_lesrooster-0.1.0.dev0/LICENCE.rst
--rw-r--r--   0        0        0     1103 2023-01-30 16:25:16.584535 aleksis_app_lesrooster-0.1.0.dev0/README.rst
--rw-r--r--   0        0        0      156 2023-01-30 16:25:16.592535 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/__init__.py
--rw-r--r--   0        0        0     1685 2024-03-13 12:15:27.876536 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/apps.py
--rw-r--r--   0        0        0     1775 2024-02-24 14:16:32.705234 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/breaks_and_slots/Break.vue
--rw-r--r--   0        0        0     6355 2024-02-24 14:16:32.705234 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/breaks_and_slots/LesroosterSlot.vue
--rw-r--r--   0        0        0     1287 2024-02-24 14:16:32.705234 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/breaks_and_slots/break.graphql
--rw-r--r--   0        0        0     2158 2024-02-24 14:16:32.705234 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/breaks_and_slots/slot.graphql
--rw-r--r--   0        0        0     2706 2024-01-22 20:46:16.314844 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/common/ColoredShortNameChip.vue
--rw-r--r--   0        0        0      473 2024-01-22 20:09:13.810245 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/helper.graphql
--rw-r--r--   0        0        0    13607 2024-02-24 14:16:32.705234 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/lesson_raster/LessonRaster.vue
--rw-r--r--   0        0        0     3041 2024-01-22 20:46:16.314844 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/lesson_raster/SlotCard.vue
--rw-r--r--   0        0        0     4856 2024-02-24 14:16:32.705234 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/lesson_raster/SlotCreator.vue
--rw-r--r--   0        0        0     9470 2024-02-24 14:16:32.709234 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/supervision/Supervision.vue
--rw-r--r--   0        0        0     1084 2024-02-24 14:16:32.709234 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/supervision/supervision.graphql
--rw-r--r--   0        0        0     6594 2024-02-24 14:16:32.709234 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/timebound_course_config/TimeboundCourseConfigCRUDTable.vue
--rw-r--r--   0        0        0    15349 2024-02-24 14:16:32.709234 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/timebound_course_config/TimeboundCourseConfigRaster.vue
--rw-r--r--   0        0        0     1930 2024-02-24 14:16:32.709234 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/timebound_course_config/timeboundCourseConfig.graphql
--rw-r--r--   0        0        0      664 2024-01-22 20:46:16.314844 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/timetable_management/BlockingCard.vue
--rw-r--r--   0        0        0     4408 2024-01-22 20:46:16.314844 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/timetable_management/LessonCard.vue
--rw-r--r--   0        0        0      834 2024-01-22 20:09:13.810245 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/timetable_management/LessonRatioChip.vue
--rw-r--r--   0        0        0     2593 2024-01-22 20:46:16.314844 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/timetable_management/PeriodCard.vue
--rw-r--r--   0        0        0    37212 2024-02-24 14:16:32.709234 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/timetable_management/TimetableManagement.vue
--rw-r--r--   0        0        0     2286 2024-02-24 14:16:32.709234 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/timetable_management/TimetableOverlayCard.vue
--rw-r--r--   0        0        0     3631 2024-02-24 14:16:32.709234 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/timetable_management/timetableManagement.graphql
--rw-r--r--   0        0        0     3050 2024-01-22 20:46:16.318844 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/timetable_management/timetables/MiniTimeTable.vue
--rw-r--r--   0        0        0      656 2024-01-22 20:09:13.810245 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/timetable_management/timetables/RoomTimeTable.vue
--rw-r--r--   0        0        0      680 2024-01-22 20:09:13.810245 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/timetable_management/timetables/TeacherTimeTable.vue
--rw-r--r--   0        0        0     1490 2024-01-22 20:09:13.810245 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/timetable_management/timetables/timetables.graphql
--rw-r--r--   0        0        0     2839 2024-01-22 20:46:16.318844 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/validity_range/CopyFromTimeGridMenu.vue
--rw-r--r--   0        0        0      599 2024-01-22 20:09:13.810245 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/validity_range/TimeGridChip.vue
--rw-r--r--   0        0        0     4177 2024-02-24 14:16:32.709234 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/validity_range/TimeGridField.vue
--rw-r--r--   0        0        0    11812 2024-02-24 14:16:32.709234 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/validity_range/ValidityRange.vue
--rw-r--r--   0        0        0     3164 2024-02-24 14:16:32.709234 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/validity_range/ValidityRangeField.vue
--rw-r--r--   0        0        0      614 2024-01-22 20:09:13.810245 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/validity_range/ValidityRangeStatusChip.vue
--rw-r--r--   0        0        0      676 2024-01-22 20:09:13.810245 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/validity_range/ValidityRangeStatusField.vue
--rw-r--r--   0        0        0     1996 2024-02-24 14:16:32.709234 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/validity_range/validityRange.graphql
--rw-r--r--   0        0        0      330 2024-01-22 20:09:13.810245 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/validity_range/validityRangeStatuses.js
--rw-r--r--   0        0        0     4090 2024-02-24 14:16:32.709234 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/index.js
--rw-r--r--   0        0        0     5765 2024-01-22 20:09:13.810245 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/messages/de.json
--rw-r--r--   0        0        0     5323 2024-01-22 20:09:13.810245 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/messages/en.json
--rw-r--r--   0        0        0        0 2023-01-30 16:25:16.592535 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/locale/.keepdir
--rw-r--r--   0        0        0      352 2024-02-17 18:55:54.032297 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/managers.py
--rw-r--r--   0        0        0    21147 2024-02-24 14:16:32.709234 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/migrations/0001_initial.py
--rw-r--r--   0        0        0     3042 2024-01-22 20:46:16.318844 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/migrations/0002_timeboundcourseconfig.py
--rw-r--r--   0        0        0     2383 2024-01-22 20:46:16.318844 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/migrations/0003_timegrid.py
--rw-r--r--   0        0        0     1133 2024-01-22 20:09:13.814246 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/migrations/0004_slot_timegrid.py
--rw-r--r--   0        0        0      753 2024-01-22 20:09:13.814246 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/migrations/0005_migrate_slot_to_timegrid.py
--rw-r--r--   0        0        0     1081 2024-01-22 20:09:13.814246 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/migrations/0006_slot_drop_validityrange.py
--rw-r--r--   0        0        0      407 2024-01-22 20:09:13.814246 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/migrations/0007_rename_scheduled_slot_count_timeboundcourseconfig_lesson_quota.py
--rw-r--r--   0        0        0      569 2024-01-22 20:09:13.814246 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/migrations/0008_one_default_time_grid.py
--rw-r--r--   0        0        0      862 2024-01-22 20:09:13.814246 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/migrations/0009_lesroosterglobalpermissions.py
--rw-r--r--   0        0        0      702 2024-01-22 20:09:13.814246 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/migrations/0010_multiple_validity_ranges_per_time.py
--rw-r--r--   0        0        0      601 2024-01-22 20:09:13.814246 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/migrations/0011_alter_lesroosterglobalpermissions_options.py
--rw-r--r--   0        0        0     1167 2024-01-22 20:09:13.814246 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/migrations/0012_alter_timeboundcourseconfig_lesson_quota_and_more.py
--rw-r--r--   0        0        0     1159 2024-01-22 20:09:13.814246 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/migrations/0013_supervision_subject_supervisionsubstitution_subject.py
--rw-r--r--   0        0        0      373 2024-01-22 20:09:13.814246 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/migrations/0014_remove_breakslot_period_after.py
--rw-r--r--   0        0        0     1291 2024-01-22 20:46:16.318844 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/migrations/0015_drop_site.py
--rw-r--r--   0        0        0      882 2024-03-10 14:39:37.101566 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/migrations/0016_remove_substitutions.py
--rw-r--r--   0        0        0        0 2023-01-30 16:25:16.596535 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/migrations/__init__.py
--rw-r--r--   0        0        0    17536 2024-03-13 12:15:27.876536 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/models.py
--rw-r--r--   0        0        0     9631 2024-03-10 14:39:37.105566 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/rules.py
--rw-r--r--   0        0        0    10617 2024-02-24 14:16:32.709234 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/schema/__init__.py
--rw-r--r--   0        0        0     2317 2024-02-24 14:16:32.709234 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/schema/break_slot.py
--rw-r--r--   0        0        0     2631 2024-02-24 14:16:32.709234 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/schema/lesson.py
--rw-r--r--   0        0        0     5937 2024-02-24 14:16:32.709234 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/schema/slot.py
--rw-r--r--   0        0        0     2731 2024-02-24 14:16:32.709234 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/schema/supervision.py
--rw-r--r--   0        0        0     1959 2024-02-24 14:16:32.709234 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/schema/time_grid.py
--rw-r--r--   0        0        0     3479 2024-02-24 14:16:32.709234 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/schema/timebound_course_config.py
--rw-r--r--   0        0        0     2368 2024-03-13 12:15:27.876536 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/schema/validity_range.py
--rw-r--r--   0        0        0     1829 2024-03-13 12:15:27.876536 aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/util/signal_handlers.py
--rw-r--r--   0        0        0     2585 2024-03-10 14:39:35.037544 aleksis_app_lesrooster-0.1.0.dev0/pyproject.toml
--rw-r--r--   0        0        0     2180 2024-01-22 20:46:16.318844 aleksis_app_lesrooster-0.1.0.dev0/tox.ini
--rw-r--r--   0        0        0     2208 1970-01-01 00:00:00.000000 aleksis_app_lesrooster-0.1.0.dev0/PKG-INFO
+-rw-r--r--   0        0        0      442 2023-01-30 16:25:16.564535 aleksis_app_lesrooster-0.1.0.dev1/CHANGELOG.rst
+-rw-r--r--   0        0        0    14361 2023-01-30 16:25:16.576535 aleksis_app_lesrooster-0.1.0.dev1/LICENCE.rst
+-rw-r--r--   0        0        0     1103 2023-01-30 16:25:16.584535 aleksis_app_lesrooster-0.1.0.dev1/README.rst
+-rw-r--r--   0        0        0      156 2023-01-30 16:25:16.592535 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/__init__.py
+-rw-r--r--   0        0        0     1685 2024-04-04 13:58:03.453827 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/apps.py
+-rw-r--r--   0        0        0     1775 2024-02-24 14:16:32.705234 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/breaks_and_slots/Break.vue
+-rw-r--r--   0        0        0     6355 2024-02-24 14:16:32.705234 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/breaks_and_slots/LesroosterSlot.vue
+-rw-r--r--   0        0        0     1287 2024-02-24 14:16:32.705234 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/breaks_and_slots/break.graphql
+-rw-r--r--   0        0        0     2158 2024-02-24 14:16:32.705234 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/breaks_and_slots/slot.graphql
+-rw-r--r--   0        0        0     2706 2024-01-22 20:46:16.314844 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/common/ColoredShortNameChip.vue
+-rw-r--r--   0        0        0      473 2024-01-22 20:09:13.810245 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/helper.graphql
+-rw-r--r--   0        0        0    13607 2024-02-24 14:16:32.705234 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/lesson_raster/LessonRaster.vue
+-rw-r--r--   0        0        0     3041 2024-01-22 20:46:16.314844 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/lesson_raster/SlotCard.vue
+-rw-r--r--   0        0        0     4856 2024-02-24 14:16:32.705234 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/lesson_raster/SlotCreator.vue
+-rw-r--r--   0        0        0     9470 2024-02-24 14:16:32.709234 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/supervision/Supervision.vue
+-rw-r--r--   0        0        0     1084 2024-02-24 14:16:32.709234 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/supervision/supervision.graphql
+-rw-r--r--   0        0        0     6594 2024-02-24 14:16:32.709234 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/timebound_course_config/TimeboundCourseConfigCRUDTable.vue
+-rw-r--r--   0        0        0    15349 2024-02-24 14:16:32.709234 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/timebound_course_config/TimeboundCourseConfigRaster.vue
+-rw-r--r--   0        0        0     1930 2024-02-24 14:16:32.709234 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/timebound_course_config/timeboundCourseConfig.graphql
+-rw-r--r--   0        0        0      664 2024-01-22 20:46:16.314844 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/timetable_management/BlockingCard.vue
+-rw-r--r--   0        0        0     4408 2024-01-22 20:46:16.314844 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/timetable_management/LessonCard.vue
+-rw-r--r--   0        0        0      834 2024-01-22 20:09:13.810245 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/timetable_management/LessonRatioChip.vue
+-rw-r--r--   0        0        0     2593 2024-01-22 20:46:16.314844 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/timetable_management/PeriodCard.vue
+-rw-r--r--   0        0        0    38472 2024-04-04 13:58:07.030073 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/timetable_management/TimetableManagement.vue
+-rw-r--r--   0        0        0     2286 2024-02-24 14:16:32.709234 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/timetable_management/TimetableOverlayCard.vue
+-rw-r--r--   0        0        0     3631 2024-02-24 14:16:32.709234 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/timetable_management/timetableManagement.graphql
+-rw-r--r--   0        0        0     3050 2024-01-22 20:46:16.318844 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/timetable_management/timetables/MiniTimeTable.vue
+-rw-r--r--   0        0        0      656 2024-01-22 20:09:13.810245 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/timetable_management/timetables/RoomTimeTable.vue
+-rw-r--r--   0        0        0      680 2024-01-22 20:09:13.810245 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/timetable_management/timetables/TeacherTimeTable.vue
+-rw-r--r--   0        0        0     1490 2024-01-22 20:09:13.810245 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/timetable_management/timetables/timetables.graphql
+-rw-r--r--   0        0        0     2839 2024-01-22 20:46:16.318844 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/validity_range/CopyFromTimeGridMenu.vue
+-rw-r--r--   0        0        0      599 2024-01-22 20:09:13.810245 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/validity_range/TimeGridChip.vue
+-rw-r--r--   0        0        0     4177 2024-02-24 14:16:32.709234 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/validity_range/TimeGridField.vue
+-rw-r--r--   0        0        0    11812 2024-04-04 13:58:03.457828 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/validity_range/ValidityRange.vue
+-rw-r--r--   0        0        0     3164 2024-02-24 14:16:32.709234 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/validity_range/ValidityRangeField.vue
+-rw-r--r--   0        0        0      614 2024-01-22 20:09:13.810245 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/validity_range/ValidityRangeStatusChip.vue
+-rw-r--r--   0        0        0      676 2024-01-22 20:09:13.810245 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/validity_range/ValidityRangeStatusField.vue
+-rw-r--r--   0        0        0     2012 2024-04-04 13:58:07.030073 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/validity_range/validityRange.graphql
+-rw-r--r--   0        0        0      330 2024-01-22 20:09:13.810245 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/validity_range/validityRangeStatuses.js
+-rw-r--r--   0        0        0     4110 2024-04-04 13:58:07.030073 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/index.js
+-rw-r--r--   0        0        0     5765 2024-01-22 20:09:13.810245 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/messages/de.json
+-rw-r--r--   0        0        0     5323 2024-04-04 13:58:03.457828 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/messages/en.json
+-rw-r--r--   0        0        0        0 2023-01-30 16:25:16.592535 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/locale/.keepdir
+-rw-r--r--   0        0        0      352 2024-02-17 18:55:54.032297 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/managers.py
+-rw-r--r--   0        0        0    21147 2024-02-24 14:16:32.709234 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/migrations/0001_initial.py
+-rw-r--r--   0        0        0     3042 2024-01-22 20:46:16.318844 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/migrations/0002_timeboundcourseconfig.py
+-rw-r--r--   0        0        0     2383 2024-01-22 20:46:16.318844 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/migrations/0003_timegrid.py
+-rw-r--r--   0        0        0     1133 2024-01-22 20:09:13.814246 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/migrations/0004_slot_timegrid.py
+-rw-r--r--   0        0        0      753 2024-01-22 20:09:13.814246 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/migrations/0005_migrate_slot_to_timegrid.py
+-rw-r--r--   0        0        0     1081 2024-01-22 20:09:13.814246 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/migrations/0006_slot_drop_validityrange.py
+-rw-r--r--   0        0        0      407 2024-01-22 20:09:13.814246 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/migrations/0007_rename_scheduled_slot_count_timeboundcourseconfig_lesson_quota.py
+-rw-r--r--   0        0        0      569 2024-01-22 20:09:13.814246 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/migrations/0008_one_default_time_grid.py
+-rw-r--r--   0        0        0      862 2024-01-22 20:09:13.814246 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/migrations/0009_lesroosterglobalpermissions.py
+-rw-r--r--   0        0        0      702 2024-01-22 20:09:13.814246 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/migrations/0010_multiple_validity_ranges_per_time.py
+-rw-r--r--   0        0        0      601 2024-01-22 20:09:13.814246 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/migrations/0011_alter_lesroosterglobalpermissions_options.py
+-rw-r--r--   0        0        0     1167 2024-01-22 20:09:13.814246 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/migrations/0012_alter_timeboundcourseconfig_lesson_quota_and_more.py
+-rw-r--r--   0        0        0     1159 2024-01-22 20:09:13.814246 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/migrations/0013_supervision_subject_supervisionsubstitution_subject.py
+-rw-r--r--   0        0        0      373 2024-01-22 20:09:13.814246 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/migrations/0014_remove_breakslot_period_after.py
+-rw-r--r--   0        0        0     1291 2024-01-22 20:46:16.318844 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/migrations/0015_drop_site.py
+-rw-r--r--   0        0        0      882 2024-03-10 14:39:37.101566 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/migrations/0016_remove_substitutions.py
+-rw-r--r--   0        0        0        0 2023-01-30 16:25:16.596535 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/migrations/__init__.py
+-rw-r--r--   0        0        0    17679 2024-04-04 13:58:07.030073 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/models.py
+-rw-r--r--   0        0        0     9631 2024-03-10 14:39:37.105566 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/rules.py
+-rw-r--r--   0        0        0    11403 2024-04-04 13:58:07.030073 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/schema/__init__.py
+-rw-r--r--   0        0        0     2317 2024-02-24 14:16:32.709234 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/schema/break_slot.py
+-rw-r--r--   0        0        0     2631 2024-02-24 14:16:32.709234 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/schema/lesson.py
+-rw-r--r--   0        0        0     5937 2024-02-24 14:16:32.709234 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/schema/slot.py
+-rw-r--r--   0        0        0     2731 2024-02-24 14:16:32.709234 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/schema/supervision.py
+-rw-r--r--   0        0        0     1959 2024-02-24 14:16:32.709234 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/schema/time_grid.py
+-rw-r--r--   0        0        0     3479 2024-02-24 14:16:32.709234 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/schema/timebound_course_config.py
+-rw-r--r--   0        0        0     2405 2024-04-04 13:58:07.030073 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/schema/validity_range.py
+-rw-r--r--   0        0        0        0 2024-03-28 16:41:58.004132 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/util/recurrence.py
+-rw-r--r--   0        0        0     1829 2024-04-04 13:58:03.457828 aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/util/signal_handlers.py
+-rw-r--r--   0        0        0     2587 2024-04-05 08:13:04.548610 aleksis_app_lesrooster-0.1.0.dev1/pyproject.toml
+-rw-r--r--   0        0        0     2180 2024-01-22 20:46:16.318844 aleksis_app_lesrooster-0.1.0.dev1/tox.ini
+-rw-r--r--   0        0        0     2271 1970-01-01 00:00:00.000000 aleksis_app_lesrooster-0.1.0.dev1/PKG-INFO
```

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/LICENCE.rst` & `aleksis_app_lesrooster-0.1.0.dev1/LICENCE.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/README.rst` & `aleksis_app_lesrooster-0.1.0.dev1/README.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/apps.py` & `aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/apps.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/breaks_and_slots/Break.vue` & `aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/breaks_and_slots/Break.vue`

 * *Files identical despite different names*

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/breaks_and_slots/LesroosterSlot.vue` & `aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/breaks_and_slots/LesroosterSlot.vue`

 * *Files identical despite different names*

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/breaks_and_slots/break.graphql` & `aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/breaks_and_slots/break.graphql`

 * *Files identical despite different names*

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/breaks_and_slots/slot.graphql` & `aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/breaks_and_slots/slot.graphql`

 * *Files identical despite different names*

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/common/ColoredShortNameChip.vue` & `aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/common/ColoredShortNameChip.vue`

 * *Files identical despite different names*

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/lesson_raster/LessonRaster.vue` & `aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/lesson_raster/LessonRaster.vue`

 * *Files identical despite different names*

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/lesson_raster/SlotCard.vue` & `aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/lesson_raster/SlotCard.vue`

 * *Files identical despite different names*

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/lesson_raster/SlotCreator.vue` & `aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/lesson_raster/SlotCreator.vue`

 * *Files identical despite different names*

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/supervision/Supervision.vue` & `aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/supervision/Supervision.vue`

 * *Files identical despite different names*

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/supervision/supervision.graphql` & `aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/supervision/supervision.graphql`

 * *Files identical despite different names*

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/timebound_course_config/TimeboundCourseConfigCRUDTable.vue` & `aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/timebound_course_config/TimeboundCourseConfigCRUDTable.vue`

 * *Files identical despite different names*

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/timebound_course_config/TimeboundCourseConfigRaster.vue` & `aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/timebound_course_config/TimeboundCourseConfigRaster.vue`

 * *Files identical despite different names*

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/timebound_course_config/timeboundCourseConfig.graphql` & `aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/timebound_course_config/timeboundCourseConfig.graphql`

 * *Files identical despite different names*

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/timetable_management/BlockingCard.vue` & `aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/timetable_management/BlockingCard.vue`

 * *Files identical despite different names*

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/timetable_management/LessonCard.vue` & `aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/timetable_management/LessonCard.vue`

 * *Files identical despite different names*

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/timetable_management/LessonRatioChip.vue` & `aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/timetable_management/LessonRatioChip.vue`

 * *Files identical despite different names*

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/timetable_management/PeriodCard.vue` & `aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/timetable_management/PeriodCard.vue`

 * *Files identical despite different names*

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/timetable_management/TimetableManagement.vue` & `aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/timetable_management/TimetableManagement.vue`

 * *Files 1% similar despite different names*

```diff
@@ -102,20 +102,20 @@
       query: gqlGroups,
       variables() {
         return {
           timeGrid: this.internalTimeGrid.id,
         };
       },
       skip() {
-        return this.internalTimeGrid === null;
+        return this.internalTimeGrid?.id == null;
       },
       result() {
-        if (!this.selectedGroup && this.$route.params.id && this.groups) {
+        if (this.$route.params.group && this.groups) {
           this.selectedGroup = this.groups.find(
-            (group) => group.id === this.$route.params.id,
+            (group) => group.id === this.$route.params.group,
           );
         }
       },
     },
     slots: {
       query: slots,
       variables() {
@@ -194,15 +194,25 @@
           timeGrid: this.internalTimeGrid.id,
           group: this.selectedGroup.id,
         };
       },
       skip() {
         return !this.readyForQueries;
       },
-      result({ data: { lessonObjects } }) {
+      result(
+        {
+          data: { lessonObjects = [] } = {
+            lessonObjects: [],
+          },
+        } = {
+          data: {
+            lessonObjects: [],
+          },
+        },
+      ) {
         this.lessonsUsed = {};
         lessonObjects.forEach((lesson) => {
           let increment =
             this.periods.indexOf(lesson.slotEnd.period) -
             this.periods.indexOf(lesson.slotStart.period) +
             1;
           this.lessonsUsed[lesson.course.id] =
@@ -341,28 +351,48 @@
       }
       return this.draggedItem?.data.rooms.map((t) => t.id) || [];
     },
   },
   watch: {
     selectedGroup() {
       if (!this.selectedGroup) return;
-      if (this.selectedGroup.id != this.$route.params.id) {
+      if (
+        this.selectedGroup.id != this.$route.params.group ||
+        this.internalTimeGrid.id != this.$route.params.timeGrid
+      ) {
+        // to be able to select a group, the timeGrid has to be set
         this.$router.push({
           name: "lesrooster.timetable_management",
-          params: { id: this.selectedGroup.id },
+          params: {
+            group: this.selectedGroup.id,
+            timeGrid: this.internalTimeGrid.id,
+          },
         });
       }
       this.$setToolBarTitle(
         this.$t("lesrooster.timetable_management.for_group", {
           group: this.selectedGroup.name,
         }),
       );
       this.$apollo.queries.courses.refetch();
       this.$apollo.queries.lessonObjects.refetch();
     },
+    internalTimeGrid(newTimeGrid, oldTimeGrid) {
+      if (!oldTimeGrid) return;
+
+      if (this.selectedGroup?.id) {
+        this.$router.push({
+          name: "lesrooster.timetable_management",
+          params: {
+            group: this.selectedGroup.id,
+            timeGrid: this.internalTimeGrid.id,
+          },
+        });
+      }
+    },
   },
   methods: {
     itemMovedToLessons(eventData) {
       let newStartSlotId = this.slots.filter(
         (slot) =>
           slot.period === this.periods[eventData.y - 1] &&
           slot.weekday === this.weekdays[eventData.x - 1],
@@ -817,14 +847,26 @@
     handleContainerDrag(element, type) {
       if (type === "start") {
         this.draggedItem = element;
       } else {
         this.draggedItem = null;
       }
     },
+    setInitialTimeGrid(timeGrids) {
+      if (!this.internalTimeGrid?.id) {
+        this.internalTimeGrid = timeGrids.find(
+          this.$route.params.timeGrid
+            ? (timeGrid) => timeGrid.id === this.$route.params.timeGrid
+            : (timeGrid) =>
+                timeGrid.validityRange.isCurrent &&
+                (!timeGrid.group ||
+                  timeGrid.group?.id === this.$route.params.group),
+        );
+      }
+    },
   },
 });
 </script>
 
 <template>
   <div>
     <v-row>
@@ -833,35 +875,37 @@
           <secondary-action-button
             i18n-key="lesrooster.timetable_management.back"
             :to="{ name: 'cursus.school_structure' }"
           />
 
           <v-spacer />
 
+          <time-grid-field
+            outlined
+            filled
+            label="Select Validity Range"
+            hide-details
+            v-model="internalTimeGrid"
+            @items="setInitialTimeGrid"
+          />
+
           <v-autocomplete
             outlined
             filled
             hide-details
             label="Select Group"
             :items="groups"
             item-text="name"
             item-value="id"
             return-object
             v-model="selectedGroup"
-            :loading="$apollo.queries.gqlGroups"
+            :loading="$apollo.queries.groups.loading"
+            :disabled="!internalTimeGrid?.id"
             class="mr-4"
           />
-
-          <time-grid-field
-            outlined
-            filled
-            label="Select Validity Range"
-            hide-details
-            v-model="internalTimeGrid"
-          />
         </div>
       </v-col>
 
       <v-col
         cols="12"
         lg="4"
         xl="3"
```

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/timetable_management/TimetableOverlayCard.vue` & `aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/timetable_management/TimetableOverlayCard.vue`

 * *Files identical despite different names*

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/timetable_management/timetableManagement.graphql` & `aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/timetable_management/timetableManagement.graphql`

 * *Files identical despite different names*

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/timetable_management/timetables/MiniTimeTable.vue` & `aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/timetable_management/timetables/MiniTimeTable.vue`

 * *Files identical despite different names*

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/timetable_management/timetables/RoomTimeTable.vue` & `aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/timetable_management/timetables/RoomTimeTable.vue`

 * *Files identical despite different names*

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/timetable_management/timetables/TeacherTimeTable.vue` & `aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/timetable_management/timetables/TeacherTimeTable.vue`

 * *Files identical despite different names*

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/timetable_management/timetables/timetables.graphql` & `aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/timetable_management/timetables/timetables.graphql`

 * *Files identical despite different names*

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/validity_range/CopyFromTimeGridMenu.vue` & `aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/validity_range/CopyFromTimeGridMenu.vue`

 * *Files identical despite different names*

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/validity_range/TimeGridChip.vue` & `aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/validity_range/TimeGridChip.vue`

 * *Files identical despite different names*

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/validity_range/TimeGridField.vue` & `aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/validity_range/TimeGridField.vue`

 * *Files identical despite different names*

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/validity_range/ValidityRange.vue` & `aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/validity_range/ValidityRange.vue`

 * *Files identical despite different names*

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/validity_range/ValidityRangeField.vue` & `aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/validity_range/ValidityRangeField.vue`

 * *Files identical despite different names*

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/validity_range/ValidityRangeStatusChip.vue` & `aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/validity_range/ValidityRangeStatusChip.vue`

 * *Files identical despite different names*

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/validity_range/ValidityRangeStatusField.vue` & `aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/validity_range/ValidityRangeStatusField.vue`

 * *Files identical despite different names*

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/components/validity_range/validityRange.graphql` & `aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/components/validity_range/validityRange.graphql`

 * *Files 2% similar despite different names*

```diff
@@ -118,12 +118,13 @@
       id
       shortName
       name
     }
     validityRange {
       id
       name
+      isCurrent
       dateStart
       dateEnd
     }
   }
 }
```

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/index.js` & `aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/index.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -55,15 +55,15 @@
             titleKey: "lesrooster.timetable_management.menu_title",
             toolbarTitle: "lesrooster.timetable_management.menu_title",
             icon: "mdi-magnet",
             permission: "lesrooster.plan_timetables_rule",
             fullWidth: true,
         },
         children: [{
-            path: ":id(\\d+)/",
+            path: ":group(\\d+)/:timeGrid(\\d+)?/",
             component: () =>
                 import("./components/timetable_management/TimetableManagement.vue"),
             name: "lesrooster.timetable_management",
             props: true,
             meta: {
                 titleKey: "lesrooster.timetable_management.menu_title",
                 toolbarTitle: "lesrooster.timetable_management.menu_title",
```

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/messages/de.json` & `aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/messages/de.json`

 * *Files identical despite different names*

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/frontend/messages/en.json` & `aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/frontend/messages/en.json`

 * *Files identical despite different names*

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/migrations/0001_initial.py` & `aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/migrations/0002_timeboundcourseconfig.py` & `aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/migrations/0002_timeboundcourseconfig.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/migrations/0003_timegrid.py` & `aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/migrations/0003_timegrid.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/migrations/0004_slot_timegrid.py` & `aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/migrations/0004_slot_timegrid.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/migrations/0005_migrate_slot_to_timegrid.py` & `aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/migrations/0005_migrate_slot_to_timegrid.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/migrations/0006_slot_drop_validityrange.py` & `aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/migrations/0006_slot_drop_validityrange.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/migrations/0008_one_default_time_grid.py` & `aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/migrations/0008_one_default_time_grid.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/migrations/0009_lesroosterglobalpermissions.py` & `aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/migrations/0009_lesroosterglobalpermissions.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/migrations/0010_multiple_validity_ranges_per_time.py` & `aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/migrations/0010_multiple_validity_ranges_per_time.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/migrations/0011_alter_lesroosterglobalpermissions_options.py` & `aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/migrations/0011_alter_lesroosterglobalpermissions_options.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/migrations/0012_alter_timeboundcourseconfig_lesson_quota_and_more.py` & `aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/migrations/0012_alter_timeboundcourseconfig_lesson_quota_and_more.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/migrations/0013_supervision_subject_supervisionsubstitution_subject.py` & `aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/migrations/0013_supervision_subject_supervisionsubstitution_subject.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/migrations/0015_drop_site.py` & `aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/migrations/0015_drop_site.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/migrations/0016_remove_substitutions.py` & `aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/migrations/0016_remove_substitutions.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/models.py` & `aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,14 +68,18 @@
             return None
 
     @classproperty
     def current(cls) -> Optional["ValidityRange"]:
         """Get the currently active validity range."""
         return cls.get_current()
 
+    @property
+    def is_current(self) -> bool:
+        return self.date_start <= (today := timezone.now().date()) and self.date_end >= today
+
     def clean(self):
         """Ensure that there is only one validity range at each point of time."""
         if self.date_end < self.date_start:
             raise ValidationError(_("The start date must be earlier than the end date."))
 
         if self.school_term and (
             self.date_end > self.school_term.date_end
```

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/rules.py` & `aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/rules.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/schema/__init__.py` & `aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/schema/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -255,16 +255,37 @@
         ).distinct()
 
     @staticmethod
     def resolve_groups_by_time_grid(root, info, time_grid=None, **kwargs):
         if not info.context.user.has_perm("lesrooster.plan_timetables_rule"):
             return []
 
+        # This will fail if the ID is invalid, but won't, if it is empty
+        time_grid_obj: TimeGrid | None = (
+            TimeGrid.objects.get(pk=time_grid) if time_grid is not None else None
+        )
+
+        # If there is no time_grid, or it is a generic one, filter groups
+        # to have a fitting school_term
+        if time_grid_obj is None or time_grid_obj.group is None:
+            return (
+                Group.objects.filter(school_term__lr_validity_ranges__time_grids__id=time_grid)
+                .annotate(has_cg=Q(child_groups__isnull=False))
+                .order_by("-has_cg", "name")
+            )
+
+        group_id = time_grid_obj.group.pk
+
         return (
-            Group.objects.filter(school_term__lr_validity_ranges__time_grids__id=time_grid)
+            Group.objects.filter(
+                Q(pk=group_id)
+                | Q(parent_groups=group_id)
+                | Q(parent_groups__parent_groups=group_id)
+            )
+            .distinct()
             .annotate(has_cg=Q(child_groups__isnull=False))
             .order_by("-has_cg", "name")
         )
 
 
 class Mutation(graphene.ObjectType):
     create_break_slots = BreakSlotBatchCreateMutation.Field()
```

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/schema/break_slot.py` & `aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/schema/break_slot.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/schema/lesson.py` & `aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/schema/lesson.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/schema/slot.py` & `aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/schema/slot.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/schema/supervision.py` & `aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/schema/supervision.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/schema/time_grid.py` & `aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/schema/time_grid.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/schema/timebound_course_config.py` & `aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/schema/timebound_course_config.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/schema/validity_range.py` & `aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/schema/validity_range.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,16 @@
     PermissionsTypeMixin,
 )
 
 from ..models import ValidityRange
 
 
 class ValidityRangeType(PermissionsTypeMixin, DjangoFilterMixin, DjangoObjectType):
+    is_current = graphene.Boolean()
+
     class Meta:
         model = ValidityRange
         fields = ("id", "school_term", "name", "date_start", "date_end", "status", "time_grids")
         filter_fields = {
             "id": ["exact"],
             "school_term": ["exact", "in"],
             "status": ["exact"],
```

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/aleksis/apps/lesrooster/util/signal_handlers.py` & `aleksis_app_lesrooster-0.1.0.dev1/aleksis/apps/lesrooster/util/signal_handlers.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/pyproject.toml` & `aleksis_app_lesrooster-0.1.0.dev1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AlekSIS-App-Lesrooster"
-version = "0.1.0.dev0"
+version = "0.1.0.dev1"
 packages = [
     { include = "aleksis" }
 ]
 readme = "README.rst"
 include = [
     { path = "aleksis/**/*.mo", format = ["sdist", "wheel"] },
     { path = "*.rst", format = "sdist" },
@@ -31,17 +31,17 @@
 [[tool.poetry.source]]
 name = "gitlab"
 url = "https://edugit.org/api/v4/projects/461/packages/pypi/simple"
 priority = "supplemental"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-AlekSIS-Core = "^4.0.0.dev4"
-AlekSIS-App-Chronos = "^4.0.0.dev1"
-AlekSIS-App-Cursus = "^0.1.dev0"
+AlekSIS-Core = "^4.0.0.dev6"
+AlekSIS-App-Chronos = "^4.0.0.dev3"
+AlekSIS-App-Cursus = "^0.1.0.dev1"
 django-recurrence = "^1.11.1"
 
 [tool.poetry.plugins."aleksis.app"]
 lesrooster = "aleksis.apps.lesrooster.apps:DefaultConfig"
 
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/tox.ini` & `aleksis_app_lesrooster-0.1.0.dev1/tox.ini`

 * *Files identical despite different names*

### Comparing `aleksis_app_lesrooster-0.1.0.dev0/PKG-INFO` & `aleksis_app_lesrooster-0.1.0.dev1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: AlekSIS-App-Lesrooster
-Version: 0.1.0.dev0
+Version: 0.1.0.dev1
 Summary: AlekSIS (School Information System) — App Lesrooster (Manage lessons in a timetable schema)
 Home-page: https://aleksis.org
 License: EUPL-1.2-or-later
 Author: Jonathan Weth
 Author-email: dev@jonathanweth.de
 Maintainer: Jonathan Weth
 Maintainer-email: dev@jonathanweth.de
 Requires-Python: >=3.10,<4.0
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Education
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Education
-Requires-Dist: AlekSIS-App-Chronos (>=4.0.0.dev1,<5.0.0)
-Requires-Dist: AlekSIS-App-Cursus (==0.1.*)
-Requires-Dist: AlekSIS-Core (>=4.0.0.dev4,<5.0.0)
+Requires-Dist: AlekSIS-App-Chronos (>=4.0.0.dev3,<5.0.0)
+Requires-Dist: AlekSIS-App-Cursus (>=0.1.0.dev1,<0.2.0)
+Requires-Dist: AlekSIS-Core (>=4.0.0.dev6,<5.0.0)
 Requires-Dist: django-recurrence (>=1.11.1,<2.0.0)
 Project-URL: Documentation, https://aleksis.org/official/AlekSIS/docs/html/
 Project-URL: Repository, https://edugit.org/AlekSIS/onboarding//AlekSIS-App-Lesrooster
 Description-Content-Type: text/x-rst
 
 AlekSIS (School Information System) — App Lesrooster (Manage lessons in a timetable schema)
 ==================================================================================================
```

