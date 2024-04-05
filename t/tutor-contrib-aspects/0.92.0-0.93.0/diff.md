# Comparing `tmp/tutor-contrib-aspects-0.92.0.tar.gz` & `tmp/tutor-contrib-aspects-0.93.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tutor-contrib-aspects-0.92.0.tar", last modified: Wed Apr  3 17:45:21 2024, max compression
+gzip compressed data, was "tutor-contrib-aspects-0.93.0.tar", last modified: Fri Apr  5 12:45:10 2024, max compression
```

## Comparing `tutor-contrib-aspects-0.92.0.tar` & `tutor-contrib-aspects-0.93.0.tar`

### file list

```diff
@@ -1,268 +1,271 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:45:21.155118 tutor-contrib-aspects-0.92.0/
--rw-r--r--   0 runner    (1001) docker     (127)    34520 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12191 2024-04-03 17:45:21.155118 tutor-contrib-aspects-0.92.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11199 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:45:21.115118 tutor-contrib-aspects-0.92.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-03 17:45:21.155118 tutor-contrib-aspects-0.92.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:45:21.155118 tutor-contrib-aspects-0.92.0/tutor_contrib_aspects.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12191 2024-04-03 17:45:21.000000 tutor-contrib-aspects-0.92.0/tutor_contrib_aspects.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17738 2024-04-03 17:45:21.000000 tutor-contrib-aspects-0.92.0/tutor_contrib_aspects.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 17:45:21.000000 tutor-contrib-aspects-0.92.0/tutor_contrib_aspects.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-03 17:45:21.000000 tutor-contrib-aspects-0.92.0/tutor_contrib_aspects.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-03 17:45:21.000000 tutor-contrib-aspects-0.92.0/tutor_contrib_aspects.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-03 17:45:21.000000 tutor-contrib-aspects-0.92.0/tutor_contrib_aspects.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:45:21.119118 tutor-contrib-aspects-0.92.0/tutoraspects/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12852 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/asset_command_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8361 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/commands_v0.py
--rw-r--r--   0 runner    (1001) docker     (127)     9922 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/commands_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:45:21.123118 tutor-contrib-aspects-0.92.0/tutoraspects/patches/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/patches/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/patches/caddyfile
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/patches/clickhouse-extra-sql
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/patches/clickhouse-server-config
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/patches/clickhouse-user-config
--rw-r--r--   0 runner    (1001) docker     (127)    18341 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/patches/k8s-deployments
--rw-r--r--   0 runner    (1001) docker     (127)     8010 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/patches/k8s-jobs
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/patches/k8s-services
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/patches/k8s-volumes
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/patches/kustomization-configmapgenerator
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/patches/local-docker-compose-dev-services
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/patches/local-docker-compose-jobs-services
--rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/patches/local-docker-compose-services
--rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/patches/openedx-common-settings
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/patches/openedx-dev-dockerfile-post-python-requirements
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/patches/openedx-development-settings
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/patches/openedx-dockerfile-post-python-requirements
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/patches/superset-extra-asset-translations
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/patches/superset-extra-assets
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/patches/superset-extra-roles
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/patches/superset-jinja-filters
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/patches/superset-row-level-security
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/patches/superset-sso-assignment-rules
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/patches/xapi-db-load-config-yaml
--rw-r--r--   0 runner    (1001) docker     (127)    27725 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:45:21.123118 tutor-contrib-aspects-0.92.0/tutoraspects/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:45:21.115118 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:45:21.123118 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:45:21.111117 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/aspects/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:45:21.123118 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/aspects/dbt/
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/aspects/dbt/profiles.yml
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/aspects/dbt/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:45:21.123118 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/aspects/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/aspects/migrations/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:45:21.123118 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/
--rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/env.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/script.py.mako
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:45:21.127118 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0001_get_org_from_course_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0002_raw_xapi_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0007_event_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0008_vector.py
--rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0010_course_dictionaries.py
--rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0011_vector_replacingmergetree_xapi_raw.py
--rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0014_add_course_names_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0015_add_course_key_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0016_event_sink_user_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0017_add_graded_course_block_names.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0020_get_org_from_course_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     6949 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0023_extend_display_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0026_event_sink_external_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0027_partition_event_sink_user_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0028_user_pii.py
--rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0029_drop_json_column.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0030_rename_vector_json_column.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0031_add_email_user_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0032_partition_tables_by_year_and_month.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0033_ccx_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0034_load_test_table.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:45:21.127118 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/aspects/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/aspects/scripts/alembic.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      175 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/aspects/scripts/clickhouse-demo-xapi-data.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/aspects/scripts/dbt.sh
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/aspects/scripts/xapi-db-load-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:45:21.111117 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/clickhouse/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:45:21.127118 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/clickhouse/config/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/clickhouse/config/server_config.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:45:21.127118 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/clickhouse/dev_config/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/clickhouse/dev_config/server_config.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:45:21.131118 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/clickhouse/users/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/clickhouse/users/user_config.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:45:21.111117 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/ralph/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:45:21.131118 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/ralph/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/ralph/config/env
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/ralph/config/logging.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:45:21.131118 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/ralph/config/ralph_auth/
--rwxr-xr-x   0 runner    (1001) docker     (127)      537 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/ralph/config/ralph_auth/auth.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:45:21.131118 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/superset/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/superset/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:45:21.131118 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/superset/conf/
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/superset/conf/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:45:21.131118 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/superset/docker/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2121 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/superset/docker/docker-bootstrap.sh
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/superset/docker/requirements-local.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:45:21.131118 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/superset/pythonpath/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/superset/pythonpath/assets.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     9633 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_assets.py
--rw-r--r--   0 runner    (1001) docker     (127)     7078 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_row_level_security.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/superset/pythonpath/localization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_jinja_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     9555 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_sso_security_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5128 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/superset/pythonpath/performance_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5999 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4627 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config_docker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:45:21.131118 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/superset/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/superset/scripts/import-assets.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:45:21.131118 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/superset/security/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:45:21.131118 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/superset/security/partials/
--rw-r--r--   0 runner    (1001) docker     (127)    14806 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/superset/security/partials/read_only_permissions.json
--rw-r--r--   0 runner    (1001) docker     (127)    76456 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/superset/security/roles.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:45:21.135118 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/vector/
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/vector/file.toml
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/vector/k8s.toml
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/vector/local.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:45:21.135118 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/vector/partials/
--rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/vector/partials/common-post.toml
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/vector/partials/common-pre.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:45:21.135118 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:45:21.135118 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:45:21.135118 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:45:21.135118 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/localization/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/localization/datasets_strings.yaml
--rw-r--r--   0 runner    (1001) docker     (127)   373791 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/localization/locale.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:45:21.115118 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:45:21.115118 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:45:21.143118 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Active_Users_Over_Time_v2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Active_Users_Per_Organization.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Actor_IDs_over_time.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Chart_Count.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Charts_by_Type.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/ClickHouse_metrics.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Course_Enrollments_Over_Time.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Course_Grade_Distribution.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Courses.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Courses_Per_Organization.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Currently_Enrolled_Learners_Per_Day.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Dashboard_Count.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distinct_forum_users.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Attempts.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Hints_Per_Correct_Answer.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Problem_Grades.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Responses.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Enrollment_Events_Per_Day.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Enrollments_By_Enrollment_Mode.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Enrollments_By_Type.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Event_type.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Events_per_course.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Last_Received_Event.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Last_course_syncronized.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Most-used_Charts.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Most-used_Dashboards.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Most_Active_Courses_Per_Day.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Pageview_engagement_by_section_subsection.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Posts_per_user.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Query_performance.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Responses_Per_Problem.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Slowest_ClickHouse_Queries.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Superset_Active_Users.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Superset_Active_Users_Over_Time.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Superset_Registered_Users_Over_Time.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Total_Actors_v2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Total_Organizations.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Transcripts_Captions_Per_Video.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Unique_actors.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/User_Actions.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Watched_Video_Segments.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Watches_Per_Video.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/xAPI_Events_Over_Time.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/xAPI_Events_Over_Time_v2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:45:21.143118 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Individual_Learner_Reports.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    19603 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Instructor_Dashboard.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Learner_Groups_Reports.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    27120 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Operator_Dashboard.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:45:21.143118 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/databases/
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/databases/OpenedX_Clickhouse.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/databases/Superset_Metadata.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:45:21.147118 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/ab_user.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/clickhouse_computed_metrics.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/course_blocks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/course_names.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/course_overviews.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/dashboards.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/dim_course_problems.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/dim_course_videos.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_course_grades.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_enrollments.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_enrollments_by_day.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_forum_interactions.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_learner_problem_course_summary.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_learner_problem_summary.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_pageview_engagement.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_problem_grades.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_problem_responses.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_transcript_usage.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_video_plays.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_watched_video_segments.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/hints_per_success.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/indexed_events.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/posts_per_user.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/query_log.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5828 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/slices.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/slowest_clickhouse_queries.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4182 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/superset_action_log.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5469 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/user_pii.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/xapi_events_all_parsed.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:45:21.115118 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/jobs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:45:21.147118 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/jobs/init/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/jobs/init/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:45:21.151118 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/jobs/init/aspects/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/jobs/init/aspects/init-aspects.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:45:21.151118 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/jobs/init/clickhouse/
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/jobs/init/clickhouse/deduplicate.sh
--rw-r--r--   0 runner    (1001) docker     (127)     4744 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/jobs/init/clickhouse/init-clickhouse.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:45:21.151118 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/jobs/init/lms/
--rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/jobs/init/lms/init-lms.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:45:21.151118 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/jobs/init/mysql/
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/jobs/init/mysql/init-mysql-post-migration.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/jobs/init/mysql/init-mysql.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:45:21.151118 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/jobs/init/superset/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2779 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/jobs/init/superset/init-superset.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/base-docker-compose-services
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:45:21.115118 tutor-contrib-aspects-0.92.0/tutoraspects/templates/openedx-assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:45:21.155118 tutor-contrib-aspects-0.92.0/tutoraspects/templates/openedx-assets/queries/
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/openedx-assets/queries/common_filters.sql
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/openedx-assets/queries/dim_course_problems.sql
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/openedx-assets/queries/dim_course_videos.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/openedx-assets/queries/fact_course_grades.sql
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/openedx-assets/queries/fact_enrollments.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/openedx-assets/queries/fact_enrollments_by_day.sql
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/openedx-assets/queries/fact_forum_interactions.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/openedx-assets/queries/fact_learner_problem_course_summary.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/openedx-assets/queries/fact_learner_problem_summary.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/openedx-assets/queries/fact_pageview_engagement.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/openedx-assets/queries/fact_problem_grades.sql
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/openedx-assets/queries/fact_problem_responses.sql
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/openedx-assets/queries/fact_transcript_usage.sql
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/openedx-assets/queries/fact_video_plays.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/openedx-assets/queries/fact_watched_video_segments.sql
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/openedx-assets/queries/hints_per_success.sql
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/openedx-assets/queries/indexed_events.sql
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/openedx-assets/queries/int_problem_responses.sql
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/openedx-assets/queries/posts_per_user.sql
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/openedx-assets/queries/slowest_clickhouse_queries.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-03 17:45:10.000000 tutor-contrib-aspects-0.92.0/tutoraspects/templates/openedx-assets/queries/superset_action_log.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:10.089259 tutor-contrib-aspects-0.93.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    34520 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12191 2024-04-05 12:45:10.089259 tutor-contrib-aspects-0.93.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11199 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:10.049260 tutor-contrib-aspects-0.93.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-05 12:45:10.089259 tutor-contrib-aspects-0.93.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:10.089259 tutor-contrib-aspects-0.93.0/tutor_contrib_aspects.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12191 2024-04-05 12:45:10.000000 tutor-contrib-aspects-0.93.0/tutor_contrib_aspects.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18049 2024-04-05 12:45:10.000000 tutor-contrib-aspects-0.93.0/tutor_contrib_aspects.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 12:45:10.000000 tutor-contrib-aspects-0.93.0/tutor_contrib_aspects.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-05 12:45:10.000000 tutor-contrib-aspects-0.93.0/tutor_contrib_aspects.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-05 12:45:10.000000 tutor-contrib-aspects-0.93.0/tutor_contrib_aspects.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-05 12:45:10.000000 tutor-contrib-aspects-0.93.0/tutor_contrib_aspects.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:10.053259 tutor-contrib-aspects-0.93.0/tutoraspects/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12852 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/asset_command_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8361 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/commands_v0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9922 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/commands_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:10.057259 tutor-contrib-aspects-0.93.0/tutoraspects/patches/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/patches/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/patches/caddyfile
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/patches/clickhouse-extra-sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/patches/clickhouse-server-config
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/patches/clickhouse-user-config
+-rw-r--r--   0 runner    (1001) docker     (127)    18341 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/patches/k8s-deployments
+-rw-r--r--   0 runner    (1001) docker     (127)     8010 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/patches/k8s-jobs
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/patches/k8s-services
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/patches/k8s-volumes
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/patches/kustomization-configmapgenerator
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/patches/local-docker-compose-dev-services
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/patches/local-docker-compose-jobs-services
+-rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/patches/local-docker-compose-services
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/patches/openedx-common-settings
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/patches/openedx-dev-dockerfile-post-python-requirements
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/patches/openedx-development-settings
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/patches/openedx-dockerfile-post-python-requirements
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/patches/superset-extra-asset-translations
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/patches/superset-extra-assets
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/patches/superset-extra-roles
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/patches/superset-jinja-filters
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/patches/superset-row-level-security
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/patches/superset-sso-assignment-rules
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/patches/xapi-db-load-config-yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    27726 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:10.057259 tutor-contrib-aspects-0.93.0/tutoraspects/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:10.049260 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:10.057259 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:10.045260 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/aspects/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:10.057259 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/aspects/dbt/
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/aspects/dbt/profiles.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/aspects/dbt/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:10.057259 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/aspects/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/aspects/migrations/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:10.057259 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/
+-rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:10.061260 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0001_get_org_from_course_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0002_raw_xapi_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0007_event_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0008_vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0010_course_dictionaries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0011_vector_replacingmergetree_xapi_raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0014_add_course_names_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0015_add_course_key_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0016_event_sink_user_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0017_add_graded_course_block_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0020_get_org_from_course_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6949 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0023_extend_display_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0026_event_sink_external_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0027_partition_event_sink_user_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0028_user_pii.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0029_drop_json_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0030_rename_vector_json_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0031_add_email_user_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0032_partition_tables_by_year_and_month.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0033_ccx_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0034_load_test_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:10.065260 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/aspects/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/aspects/scripts/alembic.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      175 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/aspects/scripts/clickhouse-demo-xapi-data.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/aspects/scripts/dbt.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/aspects/scripts/xapi-db-load-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:10.045260 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/clickhouse/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:10.065260 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/clickhouse/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/clickhouse/config/server_config.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:10.065260 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/clickhouse/dev_config/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/clickhouse/dev_config/server_config.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:10.065260 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/clickhouse/users/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/clickhouse/users/user_config.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:10.045260 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/ralph/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:10.065260 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/ralph/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/ralph/config/env
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/ralph/config/logging.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:10.065260 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/ralph/config/ralph_auth/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      537 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/ralph/config/ralph_auth/auth.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:10.065260 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/superset/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/superset/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:10.065260 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/superset/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/superset/conf/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:10.065260 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/superset/docker/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2121 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/superset/docker/docker-bootstrap.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/superset/docker/requirements-local.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:10.065260 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/superset/pythonpath/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/superset/pythonpath/assets.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9633 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7078 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_row_level_security.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/superset/pythonpath/localization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_jinja_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9555 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_sso_security_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5128 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/superset/pythonpath/performance_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5999 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4627 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config_docker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:10.069260 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/superset/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/superset/scripts/import-assets.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:10.069260 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/superset/security/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:10.069260 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/superset/security/partials/
+-rw-r--r--   0 runner    (1001) docker     (127)    14806 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/superset/security/partials/read_only_permissions.json
+-rw-r--r--   0 runner    (1001) docker     (127)    76456 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/superset/security/roles.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:10.069260 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/vector/
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/vector/file.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/vector/k8s.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/vector/local.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:10.069260 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/vector/partials/
+-rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/vector/partials/common-post.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/vector/partials/common-pre.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:10.069260 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:10.069260 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:10.069260 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:10.069260 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/localization/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/localization/datasets_strings.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)   373791 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/localization/locale.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:10.049260 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:10.049260 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:10.077260 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Active_Users_Over_Time_v2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Active_Users_Per_Organization.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Actor_IDs_over_time.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Chart_Count.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Charts_by_Type.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/ClickHouse_metrics.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Course_Enrollments_Over_Time.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Course_Grade_Distribution.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Courses.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Courses_Per_Organization.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Currently_Enrolled_Learners_Per_Day.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Dashboard_Count.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distinct_forum_users.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Attempts.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Hints_Per_Correct_Answer.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Problem_Grades.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Responses.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Enrollment_Events_Per_Day.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Enrollments_By_Enrollment_Mode.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Enrollments_By_Type.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Event_type.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Events_per_course.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Last_Received_Event.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Last_course_syncronized.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Most-used_Charts.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Most-used_Dashboards.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Most_Active_Courses_Per_Day.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Pageview_engagement_by_section_subsection.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Posts_per_user.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Query_performance.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Responses_Per_Problem.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Slowest_ClickHouse_Queries.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Superset_Active_Users.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Superset_Active_Users_Over_Time.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Superset_Registered_Users_Over_Time.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Total_Actors_v2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Total_Organizations.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Transcripts_Captions_Per_Video.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Unique_actors.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/User_Actions.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5198 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Video_engagement_by_section_subsection.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Watched_Video_Segments.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Watches_Per_Video.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/xAPI_Events_Over_Time.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/xAPI_Events_Over_Time_v2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:10.081260 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Individual_Learner_Reports.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    20495 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Instructor_Dashboard.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Learner_Groups_Reports.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    27120 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Operator_Dashboard.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:10.081260 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/databases/
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/databases/OpenedX_Clickhouse.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/databases/Superset_Metadata.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:10.085260 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/ab_user.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/clickhouse_computed_metrics.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/course_blocks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/course_names.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/course_overviews.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/dashboards.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/dim_course_problems.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/dim_course_videos.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_course_grades.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_enrollments.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_enrollments_by_day.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_forum_interactions.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_learner_problem_course_summary.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_learner_problem_summary.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_pageview_engagement.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_problem_grades.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_problem_responses.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_transcript_usage.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_video_engagement.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_video_plays.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_watched_video_segments.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/hints_per_success.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/indexed_events.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/posts_per_user.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/query_log.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5828 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/slices.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/slowest_clickhouse_queries.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4182 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/superset_action_log.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5469 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/user_pii.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/xapi_events_all_parsed.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:10.049260 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/jobs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:10.085260 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/jobs/init/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/jobs/init/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:10.085260 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/jobs/init/aspects/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/jobs/init/aspects/init-aspects.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:10.085260 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/jobs/init/clickhouse/
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/jobs/init/clickhouse/deduplicate.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     4744 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/jobs/init/clickhouse/init-clickhouse.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:10.085260 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/jobs/init/lms/
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/jobs/init/lms/init-lms.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:10.085260 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/jobs/init/mysql/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/jobs/init/mysql/init-mysql-post-migration.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/jobs/init/mysql/init-mysql.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:10.085260 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/jobs/init/superset/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2779 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/jobs/init/superset/init-superset.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/base-docker-compose-services
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:10.049260 tutor-contrib-aspects-0.93.0/tutoraspects/templates/openedx-assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:10.089259 tutor-contrib-aspects-0.93.0/tutoraspects/templates/openedx-assets/queries/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/openedx-assets/queries/common_filters.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/openedx-assets/queries/dim_course_problems.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/openedx-assets/queries/dim_course_videos.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/openedx-assets/queries/fact_course_grades.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/openedx-assets/queries/fact_enrollments.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/openedx-assets/queries/fact_enrollments_by_day.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/openedx-assets/queries/fact_forum_interactions.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/openedx-assets/queries/fact_learner_problem_course_summary.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/openedx-assets/queries/fact_learner_problem_summary.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/openedx-assets/queries/fact_pageview_engagement.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/openedx-assets/queries/fact_problem_grades.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/openedx-assets/queries/fact_problem_responses.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/openedx-assets/queries/fact_transcript_usage.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/openedx-assets/queries/fact_video_engagement.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/openedx-assets/queries/fact_video_plays.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/openedx-assets/queries/fact_watched_video_segments.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/openedx-assets/queries/hints_per_success.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/openedx-assets/queries/indexed_events.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/openedx-assets/queries/int_problem_responses.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/openedx-assets/queries/posts_per_user.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/openedx-assets/queries/slowest_clickhouse_queries.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-05 12:45:02.000000 tutor-contrib-aspects-0.93.0/tutoraspects/templates/openedx-assets/queries/superset_action_log.sql
```

### Comparing `tutor-contrib-aspects-0.92.0/LICENSE` & `tutor-contrib-aspects-0.93.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/PKG-INFO` & `tutor-contrib-aspects-0.93.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor-contrib-aspects
-Version: 0.92.0
+Version: 0.93.0
 Summary: Aspects plugin for Tutor
 Home-page: https://github.com/openedx/tutor-contrib-aspects
 Author: The Open edX Community
 License: AGPLv3
 Project-URL: Code, https://github.com/openedx/tutor-contrib-aspects
 Project-URL: Issue tracker, https://github.com/openedx/tutor-contrib-aspects/issues
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `tutor-contrib-aspects-0.92.0/README.rst` & `tutor-contrib-aspects-0.93.0/README.rst`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/setup.py` & `tutor-contrib-aspects-0.93.0/setup.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutor_contrib_aspects.egg-info/PKG-INFO` & `tutor-contrib-aspects-0.93.0/tutor_contrib_aspects.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor-contrib-aspects
-Version: 0.92.0
+Version: 0.93.0
 Summary: Aspects plugin for Tutor
 Home-page: https://github.com/openedx/tutor-contrib-aspects
 Author: The Open edX Community
 License: AGPLv3
 Project-URL: Code, https://github.com/openedx/tutor-contrib-aspects
 Project-URL: Issue tracker, https://github.com/openedx/tutor-contrib-aspects/issues
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `tutor-contrib-aspects-0.92.0/tutor_contrib_aspects.egg-info/SOURCES.txt` & `tutor-contrib-aspects-0.93.0/tutor_contrib_aspects.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -144,14 +144,15 @@
 tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Superset_Active_Users_Over_Time.yaml
 tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Superset_Registered_Users_Over_Time.yaml
 tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Total_Actors_v2.yaml
 tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Total_Organizations.yaml
 tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Transcripts_Captions_Per_Video.yaml
 tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Unique_actors.yaml
 tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/User_Actions.yaml
+tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Video_engagement_by_section_subsection.yaml
 tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Watched_Video_Segments.yaml
 tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Watches_Per_Video.yaml
 tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/xAPI_Events_Over_Time.yaml
 tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/xAPI_Events_Over_Time_v2.yaml
 tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Individual_Learner_Reports.yaml
 tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Instructor_Dashboard.yaml
 tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Learner_Groups_Reports.yaml
@@ -172,14 +173,15 @@
 tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_forum_interactions.yaml
 tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_learner_problem_course_summary.yaml
 tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_learner_problem_summary.yaml
 tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_pageview_engagement.yaml
 tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_problem_grades.yaml
 tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_problem_responses.yaml
 tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_transcript_usage.yaml
+tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_video_engagement.yaml
 tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_video_plays.yaml
 tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_watched_video_segments.yaml
 tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/hints_per_success.yaml
 tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/indexed_events.yaml
 tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/posts_per_user.yaml
 tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/query_log.yaml
 tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/slices.yaml
@@ -204,14 +206,15 @@
 tutoraspects/templates/openedx-assets/queries/fact_forum_interactions.sql
 tutoraspects/templates/openedx-assets/queries/fact_learner_problem_course_summary.sql
 tutoraspects/templates/openedx-assets/queries/fact_learner_problem_summary.sql
 tutoraspects/templates/openedx-assets/queries/fact_pageview_engagement.sql
 tutoraspects/templates/openedx-assets/queries/fact_problem_grades.sql
 tutoraspects/templates/openedx-assets/queries/fact_problem_responses.sql
 tutoraspects/templates/openedx-assets/queries/fact_transcript_usage.sql
+tutoraspects/templates/openedx-assets/queries/fact_video_engagement.sql
 tutoraspects/templates/openedx-assets/queries/fact_video_plays.sql
 tutoraspects/templates/openedx-assets/queries/fact_watched_video_segments.sql
 tutoraspects/templates/openedx-assets/queries/hints_per_success.sql
 tutoraspects/templates/openedx-assets/queries/indexed_events.sql
 tutoraspects/templates/openedx-assets/queries/int_problem_responses.sql
 tutoraspects/templates/openedx-assets/queries/posts_per_user.sql
 tutoraspects/templates/openedx-assets/queries/slowest_clickhouse_queries.sql
```

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/asset_command_helpers.py` & `tutor-contrib-aspects-0.93.0/tutoraspects/asset_command_helpers.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/commands_v0.py` & `tutor-contrib-aspects-0.93.0/tutoraspects/commands_v0.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/commands_v1.py` & `tutor-contrib-aspects-0.93.0/tutoraspects/commands_v1.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/patches/clickhouse-server-config` & `tutor-contrib-aspects-0.93.0/tutoraspects/patches/clickhouse-server-config`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/patches/clickhouse-user-config` & `tutor-contrib-aspects-0.93.0/tutoraspects/patches/clickhouse-user-config`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/patches/k8s-deployments` & `tutor-contrib-aspects-0.93.0/tutoraspects/patches/k8s-deployments`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/patches/k8s-jobs` & `tutor-contrib-aspects-0.93.0/tutoraspects/patches/k8s-jobs`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/patches/k8s-services` & `tutor-contrib-aspects-0.93.0/tutoraspects/patches/k8s-services`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/patches/k8s-volumes` & `tutor-contrib-aspects-0.93.0/tutoraspects/patches/k8s-volumes`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/patches/kustomization-configmapgenerator` & `tutor-contrib-aspects-0.93.0/tutoraspects/patches/kustomization-configmapgenerator`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/patches/local-docker-compose-dev-services` & `tutor-contrib-aspects-0.93.0/tutoraspects/patches/local-docker-compose-dev-services`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/patches/local-docker-compose-jobs-services` & `tutor-contrib-aspects-0.93.0/tutoraspects/patches/local-docker-compose-jobs-services`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/patches/local-docker-compose-services` & `tutor-contrib-aspects-0.93.0/tutoraspects/patches/local-docker-compose-services`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/patches/openedx-common-settings` & `tutor-contrib-aspects-0.93.0/tutoraspects/patches/openedx-common-settings`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/patches/xapi-db-load-config-yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/patches/xapi-db-load-config-yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/plugin.py` & `tutor-contrib-aspects-0.93.0/tutoraspects/plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -375,15 +375,15 @@
         ######################
         # dbt Settings
         # For the most part you shouldn't have to touch these
         # DBT_PROFILE_* settings get passed into the dbt_profile.yml file.
         # For now we are pulling this from github, which should allow maximum
         # flexibility for forking, running branches, specific versions, etc.
         ("DBT_REPOSITORY", "https://github.com/openedx/aspects-dbt"),
-        ("DBT_BRANCH", "v3.9.2"),
+        ("DBT_BRANCH", "v3.11.0"),
         ("DBT_SSH_KEY", ""),
         ("DBT_STATE_DIR", "/app/aspects/dbt_state/"),
         # This is a pip compliant list of Python packages to install to run dbt
         # make sure packages with versions are enclosed in double quotes
         ("EXTRA_DBT_PACKAGES", []),
         # This is the name of the database dbt will write to
         ("DBT_PROFILE_TARGET_DATABASE", "reporting"),
```

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/aspects/dbt/profiles.yml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/aspects/dbt/profiles.yml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/aspects/migrations/README.rst` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/aspects/migrations/README.rst`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/env.py` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/env.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0001_get_org_from_course_url.py` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0001_get_org_from_course_url.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0002_raw_xapi_table.py` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0002_raw_xapi_table.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0007_event_sink.py` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0007_event_sink.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0008_vector.py` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0008_vector.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0010_course_dictionaries.py` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0010_course_dictionaries.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0011_vector_replacingmergetree_xapi_raw.py` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0011_vector_replacingmergetree_xapi_raw.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0014_add_course_names_fields.py` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0014_add_course_names_fields.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0015_add_course_key_blocks.py` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0015_add_course_key_blocks.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0016_event_sink_user_profile.py` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0016_event_sink_user_profile.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0017_add_graded_course_block_names.py` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0017_add_graded_course_block_names.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0020_get_org_from_course_url.py` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0020_get_org_from_course_url.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0023_extend_display_names.py` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0023_extend_display_names.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0026_event_sink_external_id.py` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0026_event_sink_external_id.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0027_partition_event_sink_user_profile.py` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0027_partition_event_sink_user_profile.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0028_user_pii.py` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0028_user_pii.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0029_drop_json_column.py` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0029_drop_json_column.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0030_rename_vector_json_column.py` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0030_rename_vector_json_column.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0031_add_email_user_profile.py` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0031_add_email_user_profile.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0032_partition_tables_by_year_and_month.py` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0032_partition_tables_by_year_and_month.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0033_ccx_function.py` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0033_ccx_function.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0034_load_test_table.py` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0034_load_test_table.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic.ini` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/aspects/scripts/dbt.sh` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/aspects/scripts/dbt.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/ralph/config/env` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/ralph/config/env`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/ralph/config/logging.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/ralph/config/logging.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/ralph/config/ralph_auth/auth.json` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/ralph/config/ralph_auth/auth.json`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/superset/conf/README.md` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/superset/conf/README.md`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/superset/docker/docker-bootstrap.sh` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/superset/docker/docker-bootstrap.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_assets.py` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_assets.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_row_level_security.py` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_row_level_security.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/superset/pythonpath/localization.py` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/superset/pythonpath/localization.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_jinja_filters.py` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_jinja_filters.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_sso_security_manager.py` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_sso_security_manager.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/superset/pythonpath/performance_metrics.py` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/superset/pythonpath/performance_metrics.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config.py` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config_docker.py` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config_docker.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/superset/security/partials/read_only_permissions.json` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/superset/security/partials/read_only_permissions.json`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/superset/security/roles.json` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/superset/security/roles.json`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/vector/k8s.toml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/vector/k8s.toml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/apps/vector/partials/common-post.toml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/apps/vector/partials/common-post.toml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/Dockerfile` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/Dockerfile`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/localization/locale.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/localization/locale.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Active_Users_Over_Time_v2.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Active_Users_Over_Time_v2.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Active_Users_Per_Organization.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Active_Users_Per_Organization.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Actor_IDs_over_time.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Actor_IDs_over_time.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Chart_Count.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Chart_Count.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Charts_by_Type.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Charts_by_Type.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/ClickHouse_metrics.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/ClickHouse_metrics.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Course_Enrollments_Over_Time.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Course_Enrollments_Over_Time.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Course_Grade_Distribution.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Course_Grade_Distribution.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Courses.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Courses.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Courses_Per_Organization.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Courses_Per_Organization.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Currently_Enrolled_Learners_Per_Day.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Currently_Enrolled_Learners_Per_Day.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Dashboard_Count.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Dashboard_Count.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distinct_forum_users.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distinct_forum_users.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Attempts.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Attempts.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Hints_Per_Correct_Answer.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Hints_Per_Correct_Answer.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Problem_Grades.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Problem_Grades.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Responses.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Responses.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Enrollment_Events_Per_Day.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Enrollment_Events_Per_Day.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Enrollments_By_Enrollment_Mode.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Enrollments_By_Enrollment_Mode.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Enrollments_By_Type.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Enrollments_By_Type.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Event_type.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Event_type.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Events_per_course.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Events_per_course.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Last_Received_Event.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Last_Received_Event.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Last_course_syncronized.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Last_course_syncronized.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Most-used_Charts.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Most-used_Charts.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Most-used_Dashboards.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Most-used_Dashboards.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Most_Active_Courses_Per_Day.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Most_Active_Courses_Per_Day.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Pageview_engagement_by_section_subsection.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Pageview_engagement_by_section_subsection.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Posts_per_user.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Posts_per_user.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Query_performance.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Query_performance.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Responses_Per_Problem.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Responses_Per_Problem.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Slowest_ClickHouse_Queries.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Slowest_ClickHouse_Queries.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Superset_Active_Users.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Superset_Active_Users.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Superset_Active_Users_Over_Time.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Superset_Active_Users_Over_Time.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Superset_Registered_Users_Over_Time.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Superset_Registered_Users_Over_Time.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Total_Actors_v2.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Total_Actors_v2.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Total_Organizations.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Total_Organizations.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Transcripts_Captions_Per_Video.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Transcripts_Captions_Per_Video.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Unique_actors.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Unique_actors.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/User_Actions.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/User_Actions.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Watched_Video_Segments.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Watched_Video_Segments.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Watches_Per_Video.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Watches_Per_Video.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/xAPI_Events_Over_Time.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/xAPI_Events_Over_Time.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/xAPI_Events_Over_Time_v2.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/xAPI_Events_Over_Time_v2.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Individual_Learner_Reports.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Individual_Learner_Reports.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Instructor_Dashboard.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Instructor_Dashboard.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -2,93 +2,117 @@
 _roles:
 - '{{ SUPERSET_ROLES_MAPPING.instructor }}'
 css: ''
 dashboard_title: Instructor Dashboard
 description: null
 metadata:
   chart_configuration:
-    '1804':
+    '114':
       crossFilters:
         chartsInScope:
-        - 24
-        - 25
-        - 32
-        - 34
-        - 37
-        - 45
-        - 46
-        - 47
-        - 52
-        - 865
-        - 879
-        - 894
-        - 908
-        - 922
+        - 154
+        - 156
+        - 229
+        - 325
+        - 327
+        - 339
+        - 516
+        - 597
+        - 625
+        - 682
+        - 695
+        - 701
+        - 770
+        - 783
+        - 816
         scope: global
-      id: 1804
-    '32':
+      id: 114
+    '156':
       crossFilters:
         chartsInScope:
-        - 24
-        - 25
-        - 34
-        - 37
-        - 45
-        - 46
-        - 47
-        - 52
-        - 865
-        - 879
-        - 894
-        - 908
-        - 922
-        - 1804
+        - 114
+        - 154
+        - 229
+        - 325
+        - 327
+        - 339
+        - 516
+        - 597
+        - 625
+        - 682
+        - 695
+        - 701
+        - 770
+        - 783
+        - 816
         scope: global
-      id: 32
-    '34':
+      id: 156
+    '325':
       crossFilters:
         chartsInScope:
-        - 24
-        - 25
-        - 32
-        - 37
-        - 45
-        - 46
-        - 47
-        - 52
-        - 865
-        - 879
-        - 894
-        - 908
-        - 922
-        - 1804
+        - 114
+        - 154
+        - 156
+        - 229
+        - 327
+        - 339
+        - 516
+        - 597
+        - 625
+        - 682
+        - 695
+        - 701
+        - 770
+        - 783
+        - 816
         scope: global
-      id: 34
+      id: 325
+    '816':
+      crossFilters:
+        chartsInScope:
+        - 114
+        - 154
+        - 156
+        - 229
+        - 325
+        - 327
+        - 339
+        - 516
+        - 597
+        - 625
+        - 682
+        - 695
+        - 701
+        - 770
+        - 783
+        scope: global
+      id: 816
   color_scheme: ''
   color_scheme_domain: []
   cross_filters_enabled: false
   default_filters: '{}'
   expanded_slices: {}
   global_chart_configuration:
     chartsInScope:
-    - 24
-    - 25
-    - 32
-    - 34
-    - 37
-    - 45
-    - 46
-    - 47
-    - 52
-    - 865
-    - 879
-    - 894
-    - 908
-    - 922
-    - 1804
+    - 114
+    - 154
+    - 156
+    - 229
+    - 325
+    - 327
+    - 339
+    - 516
+    - 597
+    - 625
+    - 682
+    - 695
+    - 701
+    - 770
+    - 783
+    - 816
     scope:
       excluded: []
       rootPath:
       - ROOT_ID
   label_colors: {}
   native_filter_configuration:
   - cascadeParentIds: []
@@ -325,234 +349,247 @@
     - TAB-CLiLC4zxo
     targets:
     - column:
         name: video_name_with_location
       datasetUuid: 417b2035-8fa1-4c60-a405-4b1947c3c966
     type: NATIVE_FILTER
   refresh_frequency: 0
-  shared_label_colors:
-    All pages viewed: '#5AC189'
-    At least one page viewed: '#1FA8C9'
+  shared_label_colors: {}
   timed_refresh_immune_slices: []
 position:
   CHART-AZZnl_lpMv:
     children: []
     id: CHART-AZZnl_lpMv
     meta:
-      chartId: 25
+      chartId: 229
       height: 50
       sliceName: Watches Per Video
       uuid: 829c1d5b-2844-4115-876a-34ad3b3cad64
       width: 6
     parents:
     - ROOT_ID
     - TABS-SNeKAJcjhd
     - TAB-7PGDduCA7
     - ROW-BO2IHCiYF8
     type: CHART
   CHART-GFCO8s2cxv:
     children: []
     id: CHART-GFCO8s2cxv
     meta:
-      chartId: 45
+      chartId: 625
       height: 50
       sliceName: Distribution Of Responses
       uuid: f1651c44-a8f4-4b44-ad49-962823009319
       width: 6
     parents:
     - ROOT_ID
     - TABS-SNeKAJcjhd
     - TAB-pOd4znTAV
     - ROW-lZkhTcIAro
     type: CHART
   CHART-GJJ8VYQ03v:
     children: []
     id: CHART-GJJ8VYQ03v
     meta:
-      chartId: 922
+      chartId: 783
       height: 50
       sliceName: Posts per user
       uuid: bc191ce7-f39d-48db-86a9-d19949f4211d
       width: 6
     parents:
     - ROOT_ID
     - TABS-SNeKAJcjhd
     - TAB-eE0OQxuju
     - ROW-la1XxBueHN
     type: CHART
   CHART-Jr-gNVms2Q:
     children: []
     id: CHART-Jr-gNVms2Q
     meta:
-      chartId: 34
+      chartId: 114
       height: 50
       sliceName: Enrollment Events Per Day
       uuid: bb1147cc-b7bc-44b7-b06a-79b0db6626aa
       width: 8
     parents:
     - ROOT_ID
     - TABS-SNeKAJcjhd
     - TAB-8BxDuJd9Jb
     - ROW-je_Wqya3Ga
     type: CHART
   CHART-OMy4wjRBWt:
     children: []
     id: CHART-OMy4wjRBWt
     meta:
-      chartId: 52
+      chartId: 682
       height: 50
       sliceName: Watched Video Segments
       uuid: 2985a9db-c338-4008-af52-2930b81ee2e5
       width: 12
     parents:
     - ROOT_ID
     - TABS-SNeKAJcjhd
     - TAB-CLiLC4zxo
     - ROW-lN_IXnlUhL
     type: CHART
   CHART-RTO33WE9FH:
     children: []
     id: CHART-RTO33WE9FH
     meta:
-      chartId: 894
+      chartId: 597
       height: 50
       sliceName: Responses Per Problem
       uuid: a3e79162-4ace-4349-ab34-89aa60ae75ed
       width: 12
     parents:
     - ROOT_ID
     - TABS-SNeKAJcjhd
     - TAB-NR4UTAs9K
     - ROW-87X0ypdHH_
     type: CHART
   CHART-Tej2oLPBAl:
     children: []
     id: CHART-Tej2oLPBAl
     meta:
-      chartId: 24
+      chartId: 701
       height: 50
       sliceName: Transcripts / Captions Per Video
       uuid: 6b830def-f3ca-4b4c-9455-7a7b7354bce8
       width: 6
     parents:
     - ROOT_ID
     - TABS-SNeKAJcjhd
     - TAB-7PGDduCA7
     - ROW-BO2IHCiYF8
     type: CHART
   CHART-evjVO-ZSSd:
     children: []
     id: CHART-evjVO-ZSSd
     meta:
-      chartId: 32
+      chartId: 156
       height: 50
       sliceName: Enrollments By Enrollment Mode
       uuid: 05ed7102-5464-4e2f-86ae-31700b787cc3
       width: 4
     parents:
     - ROOT_ID
     - TABS-SNeKAJcjhd
     - TAB-8BxDuJd9Jb
     - ROW-je_Wqya3Ga
     type: CHART
   CHART-j3trfNh8_p:
     children: []
     id: CHART-j3trfNh8_p
     meta:
-      chartId: 1804
+      chartId: 325
       height: 50
       sliceName: Pageview engagement by section/subsection
       uuid: 366a8193-30c3-4aaf-a1ac-360609dfa0ed
       width: 12
     parents:
     - ROOT_ID
     - TABS-SNeKAJcjhd
     - TAB-4Z1kfBQZO
     - ROW-Lt0M87yMb3
     type: CHART
+  CHART-jfm-20qPKn:
+    children: []
+    id: CHART-jfm-20qPKn
+    meta:
+      chartId: 816
+      height: 50
+      sliceName: Video engagement by section/subsection
+      uuid: 21861f47-9e8b-4715-b1ff-e7f4aa595c14
+      width: 12
+    parents:
+    - ROOT_ID
+    - TABS-SNeKAJcjhd
+    - TAB-7PGDduCA7
+    - ROW-HPGIhOIs65
+    type: CHART
   CHART-lTr8DL3XuI:
     children: []
     id: CHART-lTr8DL3XuI
     meta:
-      chartId: 46
+      chartId: 695
       height: 50
       sliceName: Distribution Of Hints Per Correct Answer
       uuid: ee94be4c-6fdd-4295-b43c-40890d6c549d
       width: 6
     parents:
     - ROOT_ID
     - TABS-SNeKAJcjhd
     - TAB-pOd4znTAV
     - ROW-GKMT8uEu6K
     type: CHART
   CHART-o56v9yEe2I:
     children: []
     id: CHART-o56v9yEe2I
     meta:
-      chartId: 865
+      chartId: 770
       height: 50
       sliceName: Distribution Of Problem Grades
       uuid: 4f7e3606-f5de-4643-97c0-bbb6340a3df2
       width: 6
     parents:
     - ROOT_ID
     - TABS-SNeKAJcjhd
     - TAB-pOd4znTAV
     - ROW-lZkhTcIAro
     type: CHART
   CHART-qG1WaGKl_b:
     children: []
     id: CHART-qG1WaGKl_b
     meta:
-      chartId: 908
+      chartId: 154
       height: 50
       sliceName: Distinct forum users
       uuid: feb323ad-c819-49ca-a336-584bd9ff1a2e
       width: 6
     parents:
     - ROOT_ID
     - TABS-SNeKAJcjhd
     - TAB-eE0OQxuju
     - ROW-la1XxBueHN
     type: CHART
   CHART-rnb6PSwCOS:
     children: []
     id: CHART-rnb6PSwCOS
     meta:
-      chartId: 37
+      chartId: 339
       height: 50
       sliceName: Currently Enrolled Learners Per Day
       uuid: ed2fe731-6544-422f-bc55-42f399f48b2c
       width: 12
     parents:
     - ROOT_ID
     - TABS-SNeKAJcjhd
     - TAB-8BxDuJd9Jb
     - ROW-K8s_8uq9IP
     type: CHART
   CHART-tWnaoVNNTH:
     children: []
     id: CHART-tWnaoVNNTH
     meta:
-      chartId: 47
+      chartId: 327
       height: 50
       sliceName: Distribution Of Attempts
       uuid: db90930f-f16e-4c32-8050-0e4abae28f4c
       width: 6
     parents:
     - ROOT_ID
     - TABS-SNeKAJcjhd
     - TAB-pOd4znTAV
     - ROW-GKMT8uEu6K
     type: CHART
   CHART-w-k4N2T_L8:
     children: []
     id: CHART-w-k4N2T_L8
     meta:
-      chartId: 879
+      chartId: 516
       height: 50
       sliceName: Course Grade Distribution
       uuid: f9adbc85-1f50-4c04-ace3-31ba7390de5e
       width: 12
     parents:
     - ROOT_ID
     - TABS-SNeKAJcjhd
@@ -739,14 +776,25 @@
     meta:
       background: BACKGROUND_TRANSPARENT
     parents:
     - ROOT_ID
     - TABS-SNeKAJcjhd
     - TAB-pOd4znTAV
     type: ROW
+  ROW-HPGIhOIs65:
+    children:
+    - CHART-jfm-20qPKn
+    id: ROW-HPGIhOIs65
+    meta:
+      background: BACKGROUND_TRANSPARENT
+    parents:
+    - ROOT_ID
+    - TABS-SNeKAJcjhd
+    - TAB-7PGDduCA7
+    type: ROW
   ROW-K8s_8uq9IP:
     children:
     - CHART-rnb6PSwCOS
     id: ROW-K8s_8uq9IP
     meta:
       background: BACKGROUND_TRANSPARENT
     parents:
@@ -857,14 +905,15 @@
     - ROOT_ID
     - TABS-SNeKAJcjhd
     type: TAB
   TAB-7PGDduCA7:
     children:
     - ROW-nNEywSG0jX
     - ROW-BO2IHCiYF8
+    - ROW-HPGIhOIs65
     id: TAB-7PGDduCA7
     meta:
       defaultText: Tab title
       placeholder: Tab title
       text: Video Engagement
     parents:
     - ROOT_ID
```

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Learner_Groups_Reports.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Learner_Groups_Reports.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Operator_Dashboard.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Operator_Dashboard.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/ab_user.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/ab_user.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/clickhouse_computed_metrics.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/clickhouse_computed_metrics.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/course_blocks.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/course_blocks.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/course_names.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/course_names.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/course_overviews.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/course_overviews.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/dashboards.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/dashboards.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/dim_course_problems.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/dim_course_problems.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/dim_course_videos.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/dim_course_videos.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_course_grades.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_course_grades.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_enrollments.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_enrollments.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_enrollments_by_day.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_enrollments_by_day.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_forum_interactions.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_forum_interactions.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_learner_problem_course_summary.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_learner_problem_course_summary.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_learner_problem_summary.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_learner_problem_summary.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_problem_grades.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_problem_grades.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_problem_responses.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_problem_responses.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_transcript_usage.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_transcript_usage.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_video_plays.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_video_plays.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_watched_video_segments.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_watched_video_segments.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/hints_per_success.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/hints_per_success.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/indexed_events.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/indexed_events.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/posts_per_user.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/posts_per_user.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/query_log.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/query_log.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/slices.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/slices.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/slowest_clickhouse_queries.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/slowest_clickhouse_queries.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/superset_action_log.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/superset_action_log.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/user_pii.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/user_pii.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/xapi_events_all_parsed.yaml` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/xapi_events_all_parsed.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/jobs/init/clickhouse/deduplicate.sh` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/jobs/init/clickhouse/deduplicate.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/jobs/init/clickhouse/init-clickhouse.sh` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/jobs/init/clickhouse/init-clickhouse.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/jobs/init/lms/init-lms.sh` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/jobs/init/lms/init-lms.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/jobs/init/mysql/init-mysql.sh` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/jobs/init/mysql/init-mysql.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/aspects/jobs/init/superset/init-superset.sh` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/aspects/jobs/init/superset/init-superset.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/base-docker-compose-services` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/base-docker-compose-services`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/openedx-assets/queries/dim_course_problems.sql` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/openedx-assets/queries/dim_course_problems.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/openedx-assets/queries/dim_course_videos.sql` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/openedx-assets/queries/dim_course_videos.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/openedx-assets/queries/fact_course_grades.sql` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/openedx-assets/queries/fact_course_grades.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/openedx-assets/queries/fact_enrollments_by_day.sql` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/openedx-assets/queries/fact_enrollments_by_day.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/openedx-assets/queries/fact_learner_problem_course_summary.sql` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/openedx-assets/queries/fact_learner_problem_course_summary.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/openedx-assets/queries/fact_learner_problem_summary.sql` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/openedx-assets/queries/fact_learner_problem_summary.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/openedx-assets/queries/fact_pageview_engagement.sql` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/openedx-assets/queries/fact_pageview_engagement.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/openedx-assets/queries/fact_problem_grades.sql` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/openedx-assets/queries/fact_problem_grades.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/openedx-assets/queries/fact_problem_responses.sql` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/openedx-assets/queries/fact_problem_responses.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/openedx-assets/queries/fact_transcript_usage.sql` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/openedx-assets/queries/fact_transcript_usage.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/openedx-assets/queries/fact_video_plays.sql` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/openedx-assets/queries/fact_video_plays.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/openedx-assets/queries/fact_watched_video_segments.sql` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/openedx-assets/queries/fact_watched_video_segments.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/openedx-assets/queries/indexed_events.sql` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/openedx-assets/queries/indexed_events.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.92.0/tutoraspects/templates/openedx-assets/queries/superset_action_log.sql` & `tutor-contrib-aspects-0.93.0/tutoraspects/templates/openedx-assets/queries/superset_action_log.sql`

 * *Files identical despite different names*

