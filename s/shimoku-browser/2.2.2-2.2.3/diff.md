# Comparing `tmp/shimoku-browser-2.2.2.tar.gz` & `tmp/shimoku-browser-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shimoku-browser-2.2.2.tar", last modified: Fri Mar 22 14:01:31 2024, max compression
+gzip compressed data, was "shimoku-browser-2.2.3.tar", last modified: Fri Apr  5 07:07:29 2024, max compression
```

## Comparing `shimoku-browser-2.2.2.tar` & `shimoku-browser-2.2.3.tar`

### file list

```diff
@@ -1,308 +1,308 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:01:31.124296 shimoku-browser-2.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:01:31.072295 shimoku-browser-2.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:01:31.072295 shimoku-browser-2.2.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:01:31.076295 shimoku-browser-2.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/.github/workflows/publish-testpypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7334 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-03-22 14:01:31.124296 shimoku-browser-2.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8321 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:01:31.076295 shimoku-browser-2.2.2/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     5818 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/scripts/user_classes_header_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-03-22 14:01:31.124296 shimoku-browser-2.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/setup_browser.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:01:31.068295 shimoku-browser-2.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:01:31.076295 shimoku-browser-2.2.2/src/shimoku/
--rw-r--r--   0 runner    (1001) docker     (127)    17476 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:01:31.076295 shimoku-browser-2.2.2/src/shimoku/actions_execution/
--rw-r--r--   0 runner    (1001) docker     (127)    15087 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/actions_execution/execute_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/actions_execution/front_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:01:31.076295 shimoku-browser-2.2.2/src/shimoku/ai/
--rw-r--r--   0 runner    (1001) docker     (127)    33016 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/ai/ai_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:01:31.076295 shimoku-browser-2.2.2/src/shimoku/ai/generated_headers/
--rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/ai/generated_headers/AILayerHeader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:01:31.076295 shimoku-browser-2.2.2/src/shimoku/api/
--rw-r--r--   0 runner    (1001) docker     (127)    29626 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/api/base_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    19692 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/api/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:01:31.080295 shimoku-browser-2.2.2/src/shimoku/api/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/api/resources/action.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/api/resources/action_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     9183 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/api/resources/activity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/api/resources/activity_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    17613 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/api/resources/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     7631 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/api/resources/business.py
--rw-r--r--   0 runner    (1001) docker     (127)     4993 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/api/resources/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)    11235 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/api/resources/data_set.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/api/resources/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/api/resources/file.py
--rw-r--r--   0 runner    (1001) docker     (127)    10082 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/api/resources/report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:01:31.080295 shimoku-browser-2.2.2/src/shimoku/api/resources/reports/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:01:31.080295 shimoku-browser-2.2.2/src/shimoku/api/resources/reports/charts/
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/api/resources/reports/charts/annotated_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/api/resources/reports/charts/button.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/api/resources/reports/charts/echart.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/api/resources/reports/charts/html.py
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/api/resources/reports/charts/iframe.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/api/resources/reports/charts/indicator.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/api/resources/reports/charts/input_form.py
--rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/api/resources/reports/charts/table.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/api/resources/reports/filter_data_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/api/resources/reports/modal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/api/resources/reports/tabs_group.py
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/api/resources/reports/unsupported.py
--rw-r--r--   0 runner    (1001) docker     (127)     6665 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/api/resources/role.py
--rw-r--r--   0 runner    (1001) docker     (127)     6653 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/api/resources/universe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:01:31.084295 shimoku-browser-2.2.2/src/shimoku/api/user_access_classes/
--rw-r--r--   0 runner    (1001) docker     (127)     5868 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/api/user_access_classes/actions_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11082 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/api/user_access_classes/activities_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/api/user_access_classes/activity_templates_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10255 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/api/user_access_classes/apps_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11417 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/api/user_access_classes/businesses_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9947 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/api/user_access_classes/dashboards_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/api/user_access_classes/data_sets_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9899 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/api/user_access_classes/files_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:01:31.084295 shimoku-browser-2.2.2/src/shimoku/api/user_access_classes/generated_headers/
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/api/user_access_classes/generated_headers/ActionsLayerHeader.py
--rw-r--r--   0 runner    (1001) docker     (127)     6666 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/api/user_access_classes/generated_headers/ActivitiesLayerHeader.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/api/user_access_classes/generated_headers/ActivityTemplatesLayerHeader.py
--rw-r--r--   0 runner    (1001) docker     (127)     6979 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/api/user_access_classes/generated_headers/BoardsLayerHeader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/api/user_access_classes/generated_headers/ComponentsLayerHeader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/api/user_access_classes/generated_headers/DataSetsLayerHeader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/api/user_access_classes/generated_headers/FilesLayerHeader.py
--rw-r--r--   0 runner    (1001) docker     (127)     6887 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/api/user_access_classes/generated_headers/MenuPathsLayerHeader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/api/user_access_classes/generated_headers/UniversesLayerHeader.py
--rw-r--r--   0 runner    (1001) docker     (127)     6026 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/api/user_access_classes/generated_headers/WorkspacesLayerHeader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/api/user_access_classes/reports_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/api/user_access_classes/universes_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)    20693 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/api/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7129 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/async_execution_pool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:01:31.088295 shimoku-browser-2.2.2/src/shimoku/cli/
--rw-r--r--   0 runner    (1001) docker     (127)    20258 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:01:31.088295 shimoku-browser-2.2.2/src/shimoku/cli/cloud/
--rw-r--r--   0 runner    (1001) docker     (127)    14095 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/cli/cloud/cascade_get_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)    10845 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/cli/cloud/create.py
--rw-r--r--   0 runner    (1001) docker     (127)    18300 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/cli/cloud/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/cli/cloud/execute.py
--rw-r--r--   0 runner    (1001) docker     (127)     9860 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/cli/cloud/get.py
--rw-r--r--   0 runner    (1001) docker     (127)    30825 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/cli/cloud/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     9309 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/cli/cloud/update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/cli/cloud_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/cli/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/cli/listen.py
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     8608 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/cli/persistence.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/cli/playground.py
--rw-r--r--   0 runner    (1001) docker     (127)    14917 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:01:31.088295 shimoku-browser-2.2.2/src/shimoku/code_gen/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:01:31.088295 shimoku-browser-2.2.2/src/shimoku/code_gen/business_code_gen/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:01:31.088295 shimoku-browser-2.2.2/src/shimoku/code_gen/business_code_gen/apps_code_gen/
--rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/code_gen/business_code_gen/apps_code_gen/code_gen_from_apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:01:31.088295 shimoku-browser-2.2.2/src/shimoku/code_gen/business_code_gen/apps_code_gen/data_sets_code_gen/
--rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/code_gen/business_code_gen/apps_code_gen/data_sets_code_gen/code_gen_from_data_sets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:01:31.092296 shimoku-browser-2.2.2/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/code_gen_from_reports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:01:31.092296 shimoku-browser-2.2.2/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_annotated_echart.py
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_button.py
--rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_echarts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_form.py
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_html.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_iframe.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_indicators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_modal.py
--rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_other.py
--rw-r--r--   0 runner    (1001) docker     (127)     6631 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     5810 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_tabs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5418 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/code_gen/business_code_gen/code_gen_from_business.py
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/code_gen/file_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/code_gen/main_code_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)    10222 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/code_gen/tree_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/code_gen/utils_code_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)     3067 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6258 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/execution_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:01:31.092296 shimoku-browser-2.2.2/src/shimoku/playground/
--rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/playground/execute_local_server.py
--rw-r--r--   0 runner    (1001) docker     (127)    33599 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/playground/local_server.py
--rw-r--r--   0 runner    (1001) docker     (127)    40234 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/playground/schema_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)    14949 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/playground/schema_parameter_classses.py
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/playground/websockets_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:01:31.096295 shimoku-browser-2.2.2/src/shimoku/plt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:01:31.096295 shimoku-browser-2.2.2/src/shimoku/plt/EChart_definitions/
--rw-r--r--   0 runner    (1001) docker     (127)    12979 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/plt/EChart_definitions/bar.py
--rw-r--r--   0 runner    (1001) docker     (127)    16008 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/plt/EChart_definitions/default_echart_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/plt/EChart_definitions/funnel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/plt/EChart_definitions/gauge.py
--rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/plt/EChart_definitions/gauge_indicator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/plt/EChart_definitions/heatmap.py
--rw-r--r--   0 runner    (1001) docker     (127)    20924 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/plt/EChart_definitions/line.py
--rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/plt/EChart_definitions/line_and_bar.py
--rw-r--r--   0 runner    (1001) docker     (127)     5164 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/plt/EChart_definitions/pie.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/plt/EChart_definitions/radar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/plt/EChart_definitions/sankey.py
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/plt/EChart_definitions/scatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5580 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/plt/EChart_definitions/shimoku_gauge.py
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/plt/EChart_definitions/sunburst.py
--rw-r--r--   0 runner    (1001) docker     (127)     6576 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/plt/EChart_definitions/top_bottom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/plt/EChart_definitions/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/plt/EChart_definitions/treemap.py
--rw-r--r--   0 runner    (1001) docker     (127)     7822 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/plt/EChart_definitions/waterfall.py
--rw-r--r--   0 runner    (1001) docker     (127)    13178 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/plt/bentobox_charts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:01:31.096295 shimoku-browser-2.2.2/src/shimoku/plt/generated_headers/
--rw-r--r--   0 runner    (1001) docker     (127)    36867 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/plt/generated_headers/PlotLayerHeader.py
--rw-r--r--   0 runner    (1001) docker     (127)    86654 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/plt/plt_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)    19762 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/plt/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/src/shimoku/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:01:31.124296 shimoku-browser-2.2.2/src/shimoku_browser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-03-22 14:01:31.000000 shimoku-browser-2.2.2/src/shimoku_browser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14935 2024-03-22 14:01:31.000000 shimoku-browser-2.2.2/src/shimoku_browser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 14:01:31.000000 shimoku-browser-2.2.2/src/shimoku_browser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 14:01:30.000000 shimoku-browser-2.2.2/src/shimoku_browser.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-22 14:01:31.000000 shimoku-browser-2.2.2/src/shimoku_browser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-22 14:01:31.000000 shimoku-browser-2.2.2/src/shimoku_browser.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:01:31.100295 shimoku-browser-2.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4939 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/Jupyter_notebook_test.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:01:31.100295 shimoku-browser-2.2.2/tests/mockable_tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:01:31.104296 shimoku-browser-2.2.2/tests/mockable_tests/correct_action_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/correct_action_scripts/correct_action.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:01:31.108296 shimoku-browser-2.2.2/tests/mockable_tests/error_action_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/error_action_scripts/action_cant_have_no_params.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/error_action_scripts/action_param_must_be_Client.py
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/error_action_scripts/action_param_must_be_annotated.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/error_action_scripts/action_param_must_be_shimoku_client.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/error_action_scripts/cant_annotate_client_param_to_arb_name.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/error_action_scripts/cant_assign_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/error_action_scripts/cant_assign_client_in_class.py
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/error_action_scripts/cant_assign_client_to_subscript.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/error_action_scripts/cant_assign_to_shimoku_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/error_action_scripts/cant_define_action_in_class.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/error_action_scripts/cant_define_async_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/error_action_scripts/cant_define_more_than_one_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/error_action_scripts/cant_have_arb_params_in_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/error_action_scripts/cant_have_client_as_part_of_annotation.py
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/error_action_scripts/cant_have_non_annotated_param.py
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/error_action_scripts/cant_import_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/error_action_scripts/cant_import_from_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/error_action_scripts/cant_pass_incorrect_type_to_function.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/error_action_scripts/cant_pass_incorrect_type_to_kwargs.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/error_action_scripts/cant_rename_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/error_action_scripts/cant_return_shimoku_client.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/error_action_scripts/needs_action_function.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/error_action_scripts/needs_import_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/error_action_scripts/shimoku_client_param_must_be_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/mock_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)    14050 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_activity_metadata_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4926 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_app_metadata_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6922 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_business_metadata_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    15969 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_code_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_dashboard_metadata_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    22109 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:01:31.116296 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/annotation_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/area.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/bar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/bar_and_line_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/bentobox.py
--rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/chart_and_indicators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:01:31.124296 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/data/annotation_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/data/bar_and_line.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/data/bentobox_indicator.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/data/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/data/dynamic_conditional_and_auto_send_input_form.py
--rw-r--r--   0 runner    (1001) docker     (127)   129464 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/data/flow_and_rainfall.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/data/free_echarts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/data/free_echarts_raw.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/data/funnel.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/data/heatmap.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/data/horizontal_bar.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/data/html.py
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/data/indicator.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/data/indicator_color_by_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/data/input_form.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/data/line_with_confidence_area.py
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/data/noise.py
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/data/pie.py
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/data/radar.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/data/random_waterfall.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/data/sankey.py
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/data/scatter_test.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/data/scatter_with_effect.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/data/segmented_line.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/data/stacked_area.py
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/data/suburst.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/data/summary_line.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/data/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     9810 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/data/table_with_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/data/test_stack_distribution.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/data/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/data/waterfall.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/data/zero_centered.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/doughnut.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/dynamic_conditional_and_auto_send_input_form.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/free_echarts.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/free_echarts_raw.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/funnel.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/gauge_indicator.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/get_input_forms.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/heatmap.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/horizontal_bar.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/html.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/iframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/indicator.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/indicator_color_by_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     7594 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/infographics.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/input_form.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/line.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/line_with_confidence_area.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/marked_line.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/modal.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/pie.py
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/predictive_line.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/radar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/rainfall_area.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/rainfall_line.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/rose.py
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/sankey.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/scatter.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/scatter_with_effect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/segmented_area_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/segmented_line_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/shimoku_gauges.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/speed_gauge.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/stacked_area.py
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/stacked_bar.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/stacked_horizontal_bar.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/summary_line.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/sunburst.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/table_with_lables.py
--rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/tabs.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/treemap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/variants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/waterfall.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/zero_centered_bar.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_report_metadata_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/test_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/mockable_tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7905 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/test_ai_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/test_components_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/test_data_managing_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/test_file_metadata_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-03-22 14:01:16.000000 shimoku-browser-2.2.2/tests/test_universe_metadata_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.795218 shimoku-browser-2.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.751218 shimoku-browser-2.2.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.755218 shimoku-browser-2.2.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.755218 shimoku-browser-2.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/.github/workflows/publish-testpypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7425 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-05 07:07:29.795218 shimoku-browser-2.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8321 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.755218 shimoku-browser-2.2.3/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     5818 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/scripts/user_classes_header_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-05 07:07:29.795218 shimoku-browser-2.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/setup_browser.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.751218 shimoku-browser-2.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.755218 shimoku-browser-2.2.3/src/shimoku/
+-rw-r--r--   0 runner    (1001) docker     (127)    17476 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.755218 shimoku-browser-2.2.3/src/shimoku/actions_execution/
+-rw-r--r--   0 runner    (1001) docker     (127)    15087 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/actions_execution/execute_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/actions_execution/front_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.755218 shimoku-browser-2.2.3/src/shimoku/ai/
+-rw-r--r--   0 runner    (1001) docker     (127)    33016 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/ai/ai_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.755218 shimoku-browser-2.2.3/src/shimoku/ai/generated_headers/
+-rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/ai/generated_headers/AILayerHeader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.755218 shimoku-browser-2.2.3/src/shimoku/api/
+-rw-r--r--   0 runner    (1001) docker     (127)    29626 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/base_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19704 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.759218 shimoku-browser-2.2.3/src/shimoku/api/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/resources/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/resources/action_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9183 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/resources/activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/resources/activity_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17613 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/resources/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7631 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/resources/business.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4993 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/resources/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11235 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/resources/data_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/resources/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/resources/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10082 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/resources/report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.759218 shimoku-browser-2.2.3/src/shimoku/api/resources/reports/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.759218 shimoku-browser-2.2.3/src/shimoku/api/resources/reports/charts/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/resources/reports/charts/annotated_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/resources/reports/charts/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/resources/reports/charts/echart.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/resources/reports/charts/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/resources/reports/charts/iframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/resources/reports/charts/indicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/resources/reports/charts/input_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/resources/reports/charts/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/resources/reports/filter_data_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/resources/reports/modal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/resources/reports/tabs_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/resources/reports/unsupported.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6665 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/resources/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6653 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/resources/universe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.763218 shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/
+-rw-r--r--   0 runner    (1001) docker     (127)     5868 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/actions_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11082 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/activities_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/activity_templates_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10255 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/apps_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11417 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/businesses_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9947 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/dashboards_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/data_sets_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9899 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/files_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.763218 shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/generated_headers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/generated_headers/ActionsLayerHeader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6666 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/generated_headers/ActivitiesLayerHeader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/generated_headers/ActivityTemplatesLayerHeader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6979 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/generated_headers/BoardsLayerHeader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/generated_headers/ComponentsLayerHeader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/generated_headers/DataSetsLayerHeader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/generated_headers/FilesLayerHeader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6887 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/generated_headers/MenuPathsLayerHeader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/generated_headers/UniversesLayerHeader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6026 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/generated_headers/WorkspacesLayerHeader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/reports_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/universes_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20693 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/api/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7129 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/async_execution_pool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.763218 shimoku-browser-2.2.3/src/shimoku/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)    20258 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.767218 shimoku-browser-2.2.3/src/shimoku/cli/cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)    14095 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/cli/cloud/cascade_get_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10845 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/cli/cloud/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18300 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/cli/cloud/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/cli/cloud/execute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9860 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/cli/cloud/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30825 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/cli/cloud/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9309 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/cli/cloud/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/cli/cloud_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/cli/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/cli/listen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8608 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/cli/persistence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/cli/playground.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14917 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.767218 shimoku-browser-2.2.3/src/shimoku/code_gen/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.767218 shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.767218 shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/
+-rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/code_gen_from_apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.767218 shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/data_sets_code_gen/
+-rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/data_sets_code_gen/code_gen_from_data_sets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.767218 shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/code_gen_from_reports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.767218 shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_annotated_echart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_echarts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_html.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_iframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_indicators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_modal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_other.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6631 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5810 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_tabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5418 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/code_gen_from_business.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/code_gen/file_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/code_gen/main_code_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10222 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/code_gen/tree_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/code_gen/utils_code_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3067 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6258 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/execution_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.771218 shimoku-browser-2.2.3/src/shimoku/playground/
+-rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/playground/execute_local_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35011 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/playground/local_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40234 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/playground/schema_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14949 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/playground/schema_parameter_classses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/playground/websockets_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.771218 shimoku-browser-2.2.3/src/shimoku/plt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.771218 shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/
+-rw-r--r--   0 runner    (1001) docker     (127)    12979 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16008 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/default_echart_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/funnel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/gauge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/gauge_indicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20924 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/line_and_bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5164 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/pie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/radar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/sankey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/scatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5580 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/shimoku_gauge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/sunburst.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6576 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/top_bottom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/treemap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7822 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/waterfall.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13178 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/plt/bentobox_charts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.771218 shimoku-browser-2.2.3/src/shimoku/plt/generated_headers/
+-rw-r--r--   0 runner    (1001) docker     (127)    37704 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/plt/generated_headers/PlotLayerHeader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    88204 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/plt/plt_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19762 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/plt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/src/shimoku/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.795218 shimoku-browser-2.2.3/src/shimoku_browser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-05 07:07:29.000000 shimoku-browser-2.2.3/src/shimoku_browser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14935 2024-04-05 07:07:29.000000 shimoku-browser-2.2.3/src/shimoku_browser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 07:07:29.000000 shimoku-browser-2.2.3/src/shimoku_browser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 07:07:29.000000 shimoku-browser-2.2.3/src/shimoku_browser.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-05 07:07:29.000000 shimoku-browser-2.2.3/src/shimoku_browser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-05 07:07:29.000000 shimoku-browser-2.2.3/src/shimoku_browser.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.775218 shimoku-browser-2.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4939 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/Jupyter_notebook_test.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.775218 shimoku-browser-2.2.3/tests/mockable_tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.775218 shimoku-browser-2.2.3/tests/mockable_tests/correct_action_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/correct_action_scripts/correct_action.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.779218 shimoku-browser-2.2.3/tests/mockable_tests/error_action_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/error_action_scripts/action_cant_have_no_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/error_action_scripts/action_param_must_be_Client.py
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/error_action_scripts/action_param_must_be_annotated.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/error_action_scripts/action_param_must_be_shimoku_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/error_action_scripts/cant_annotate_client_param_to_arb_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/error_action_scripts/cant_assign_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/error_action_scripts/cant_assign_client_in_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/error_action_scripts/cant_assign_client_to_subscript.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/error_action_scripts/cant_assign_to_shimoku_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/error_action_scripts/cant_define_action_in_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/error_action_scripts/cant_define_async_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/error_action_scripts/cant_define_more_than_one_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/error_action_scripts/cant_have_arb_params_in_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/error_action_scripts/cant_have_client_as_part_of_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/error_action_scripts/cant_have_non_annotated_param.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/error_action_scripts/cant_import_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/error_action_scripts/cant_import_from_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/error_action_scripts/cant_pass_incorrect_type_to_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/error_action_scripts/cant_pass_incorrect_type_to_kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/error_action_scripts/cant_rename_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/error_action_scripts/cant_return_shimoku_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/error_action_scripts/needs_action_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/error_action_scripts/needs_import_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/error_action_scripts/shimoku_client_param_must_be_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/mock_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14050 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_activity_metadata_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4926 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_app_metadata_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6922 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_business_metadata_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16015 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_code_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_dashboard_metadata_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22109 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.787218 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/annotation_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/area.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/bar_and_line_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/bentobox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/chart_and_indicators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:07:29.795218 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/annotation_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/bar_and_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/bentobox_indicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/dynamic_conditional_and_auto_send_input_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)   129464 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/flow_and_rainfall.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/free_echarts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/free_echarts_raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/funnel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/horizontal_bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/indicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/indicator_color_by_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/input_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/line_with_confidence_area.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/pie.py
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/radar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/random_waterfall.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/sankey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/scatter_test.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/scatter_with_effect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/segmented_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/stacked_area.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/suburst.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/summary_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9810 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/table_with_labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/test_stack_distribution.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/waterfall.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/zero_centered.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/doughnut.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/dynamic_conditional_and_auto_send_input_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/free_echarts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/free_echarts_raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/funnel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/gauge_indicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/get_input_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/horizontal_bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/iframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/indicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/indicator_color_by_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7594 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/infographics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/input_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/line.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/line_with_confidence_area.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/marked_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/modal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/pie.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/predictive_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/radar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/rainfall_area.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/rainfall_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/rose.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/sankey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/scatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/scatter_with_effect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/segmented_area_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/segmented_line_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/shimoku_gauges.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/speed_gauge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/stacked_area.py
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/stacked_bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/stacked_horizontal_bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/summary_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/sunburst.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/table_with_lables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/tabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/treemap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/variants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/waterfall.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/zero_centered_bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_report_metadata_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/test_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/mockable_tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7905 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/test_ai_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/test_components_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/test_data_managing_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/test_file_metadata_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-05 07:07:16.000000 shimoku-browser-2.2.3/tests/test_universe_metadata_api.py
```

### Comparing `shimoku-browser-2.2.2/.coveragerc` & `shimoku-browser-2.2.3/.coveragerc`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/.github/ISSUE_TEMPLATE/bug_report.md` & `shimoku-browser-2.2.3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/.github/ISSUE_TEMPLATE/feature_request.md` & `shimoku-browser-2.2.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/.github/pull_request_template.md` & `shimoku-browser-2.2.3/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/.github/workflows/publish-testpypi.yml` & `shimoku-browser-2.2.3/.github/workflows/publish-testpypi.yml`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/.github/workflows/publish-to-pypi.yml` & `shimoku-browser-2.2.3/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/.gitignore` & `shimoku-browser-2.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/CHANGELOG.md` & `shimoku-browser-2.2.3/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # CHANGELOG
 
+## 2.2.3 (2024-05-04)
+
+-  Fixed CORS error with the API from the execution of the Actions
+
 ## 2.2.2 (2024-22-03)
 
 ### Fixed
 
 - Fixed communication with the front end in the actions execution
 
 ## 2.2.1 (2024-19-03)
```

### Comparing `shimoku-browser-2.2.2/CODE_OF_CONDUCT.md` & `shimoku-browser-2.2.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/CONTRIBUTING.md` & `shimoku-browser-2.2.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/LICENSE.txt` & `shimoku-browser-2.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/PKG-INFO` & `shimoku-browser-2.2.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shimoku-browser
-Version: 2.2.2
+Version: 2.2.3
 Summary: Shimoku enables you to build Data Products in just hours and allows you to create Predictive Analytics Products with Artificial Intelligence capabilities.
 Home-page: https://github.com/shimoku-tech/shimoku-api-python
 Author: Shimoku
 Author-email: contact@shimoku.com
 License: MIT
 Project-URL: Documentation, https://docs.shimoku.com/
 Platform: any
```

### Comparing `shimoku-browser-2.2.2/README.md` & `shimoku-browser-2.2.3/README.md`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/SECURITY.md` & `shimoku-browser-2.2.3/SECURITY.md`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/scripts/user_classes_header_generator.py` & `shimoku-browser-2.2.3/scripts/user_classes_header_generator.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/setup.cfg` & `shimoku-browser-2.2.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/setup.py` & `shimoku-browser-2.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/setup_browser.cfg` & `shimoku-browser-2.2.3/setup_browser.cfg`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/__init__.py` & `shimoku-browser-2.2.3/src/shimoku/__init__.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/actions_execution/execute_action.py` & `shimoku-browser-2.2.3/src/shimoku/actions_execution/execute_action.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/actions_execution/front_connection.py` & `shimoku-browser-2.2.3/src/shimoku/actions_execution/front_connection.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/ai/ai_layer.py` & `shimoku-browser-2.2.3/src/shimoku/ai/ai_layer.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/ai/generated_headers/AILayerHeader.py` & `shimoku-browser-2.2.3/src/shimoku/ai/generated_headers/AILayerHeader.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/api/base_resource.py` & `shimoku-browser-2.2.3/src/shimoku/api/base_resource.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/api/client.py` & `shimoku-browser-2.2.3/src/shimoku/api/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,15 +175,14 @@
         self.is_oauth: bool = False
         # General
         self.server: str = "invalid-server"
         self.timeout: int = 120
 
         self.default_headers = {
             "Content-Type": "application/json",
-            "User-Agent": "Swagger-Codegen/0.0/python",
         }
         self.set_config(config)
         self.call_counter = 0
         # Default vars
 
     def set_config(self, config={}):
         """Set all config values"""
@@ -403,21 +402,22 @@
         limit: Optional[int] = None,
         elastic_supported: bool = False,
         to_tazawa: bool = True,
     ):
         headers = headers or {}
         if to_tazawa:
             headers.update({"Authorization": "Bearer " + self.access_token})
-            headers.update(
-                {
-                    SHIMOKU_VERSION_KEY: get_distribution("shimoku").version
-                    if not IN_BROWSER
-                    else "2.0.0"
-                }
-            )
+            # TODO see how to handle from the browser
+            # headers.update(
+            #     {
+            #         SHIMOKU_VERSION_KEY: get_distribution("shimoku").version
+            #         if not IN_BROWSER
+            #         else "2.0.0"
+            #     }
+            # )
 
         if method not in ["GET", "HEAD", "OPTIONS", "DELETE", "POST", "PUT", "PATCH"]:
             raise ValueError(
                 "http method must be `GET`, `HEAD`, `OPTIONS`,"
                 " `POST`, `PATCH`, `PUT` or `DELETE`."
             )
         body_from = 0
```

### Comparing `shimoku-browser-2.2.2/src/shimoku/api/resources/action.py` & `shimoku-browser-2.2.3/src/shimoku/api/resources/action.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/api/resources/action_template.py` & `shimoku-browser-2.2.3/src/shimoku/api/resources/action_template.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/api/resources/activity.py` & `shimoku-browser-2.2.3/src/shimoku/api/resources/activity.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/api/resources/activity_template.py` & `shimoku-browser-2.2.3/src/shimoku/api/resources/activity_template.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/api/resources/app.py` & `shimoku-browser-2.2.3/src/shimoku/api/resources/app.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/api/resources/business.py` & `shimoku-browser-2.2.3/src/shimoku/api/resources/business.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/api/resources/dashboard.py` & `shimoku-browser-2.2.3/src/shimoku/api/resources/dashboard.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/api/resources/data_set.py` & `shimoku-browser-2.2.3/src/shimoku/api/resources/data_set.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/api/resources/event.py` & `shimoku-browser-2.2.3/src/shimoku/api/resources/event.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/api/resources/file.py` & `shimoku-browser-2.2.3/src/shimoku/api/resources/file.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/api/resources/report.py` & `shimoku-browser-2.2.3/src/shimoku/api/resources/report.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/api/resources/reports/charts/indicator.py` & `shimoku-browser-2.2.3/src/shimoku/api/resources/reports/charts/indicator.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/api/resources/reports/charts/table.py` & `shimoku-browser-2.2.3/src/shimoku/api/resources/reports/charts/table.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/api/resources/reports/filter_data_set.py` & `shimoku-browser-2.2.3/src/shimoku/api/resources/reports/filter_data_set.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/api/resources/reports/modal.py` & `shimoku-browser-2.2.3/src/shimoku/api/resources/reports/modal.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/api/resources/reports/tabs_group.py` & `shimoku-browser-2.2.3/src/shimoku/api/resources/reports/tabs_group.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/api/resources/role.py` & `shimoku-browser-2.2.3/src/shimoku/api/resources/role.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/api/resources/universe.py` & `shimoku-browser-2.2.3/src/shimoku/api/resources/universe.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/api/user_access_classes/actions_layer.py` & `shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/actions_layer.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/api/user_access_classes/activities_layer.py` & `shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/activities_layer.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/api/user_access_classes/activity_templates_layer.py` & `shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/activity_templates_layer.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/api/user_access_classes/apps_layer.py` & `shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/apps_layer.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/api/user_access_classes/businesses_layer.py` & `shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/businesses_layer.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/api/user_access_classes/dashboards_layer.py` & `shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/dashboards_layer.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/api/user_access_classes/data_sets_layer.py` & `shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/data_sets_layer.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/api/user_access_classes/files_layer.py` & `shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/files_layer.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/api/user_access_classes/generated_headers/ActionsLayerHeader.py` & `shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/generated_headers/ActionsLayerHeader.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/api/user_access_classes/generated_headers/ActivitiesLayerHeader.py` & `shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/generated_headers/ActivitiesLayerHeader.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/api/user_access_classes/generated_headers/ActivityTemplatesLayerHeader.py` & `shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/generated_headers/ActivityTemplatesLayerHeader.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/api/user_access_classes/generated_headers/BoardsLayerHeader.py` & `shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/generated_headers/BoardsLayerHeader.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/api/user_access_classes/generated_headers/ComponentsLayerHeader.py` & `shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/generated_headers/ComponentsLayerHeader.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/api/user_access_classes/generated_headers/DataSetsLayerHeader.py` & `shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/generated_headers/DataSetsLayerHeader.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/api/user_access_classes/generated_headers/FilesLayerHeader.py` & `shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/generated_headers/FilesLayerHeader.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/api/user_access_classes/generated_headers/MenuPathsLayerHeader.py` & `shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/generated_headers/MenuPathsLayerHeader.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/api/user_access_classes/generated_headers/UniversesLayerHeader.py` & `shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/generated_headers/UniversesLayerHeader.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/api/user_access_classes/generated_headers/WorkspacesLayerHeader.py` & `shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/generated_headers/WorkspacesLayerHeader.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/api/user_access_classes/reports_layer.py` & `shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/reports_layer.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/api/user_access_classes/universes_layer.py` & `shimoku-browser-2.2.3/src/shimoku/api/user_access_classes/universes_layer.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/api/utils.py` & `shimoku-browser-2.2.3/src/shimoku/api/utils.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/async_execution_pool.py` & `shimoku-browser-2.2.3/src/shimoku/async_execution_pool.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/cli/__init__.py` & `shimoku-browser-2.2.3/src/shimoku/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/cli/cloud/cascade_get_resources.py` & `shimoku-browser-2.2.3/src/shimoku/cli/cloud/cascade_get_resources.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/cli/cloud/create.py` & `shimoku-browser-2.2.3/src/shimoku/cli/cloud/create.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/cli/cloud/delete.py` & `shimoku-browser-2.2.3/src/shimoku/cli/cloud/delete.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/cli/cloud/execute.py` & `shimoku-browser-2.2.3/src/shimoku/cli/cloud/execute.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/cli/cloud/get.py` & `shimoku-browser-2.2.3/src/shimoku/cli/cloud/get.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/cli/cloud/list.py` & `shimoku-browser-2.2.3/src/shimoku/cli/cloud/list.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/cli/cloud/update.py` & `shimoku-browser-2.2.3/src/shimoku/cli/cloud/update.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/cli/cloud_parser.py` & `shimoku-browser-2.2.3/src/shimoku/cli/cloud_parser.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/cli/configuration.py` & `shimoku-browser-2.2.3/src/shimoku/cli/configuration.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/cli/listen.py` & `shimoku-browser-2.2.3/src/shimoku/cli/listen.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/cli/main.py` & `shimoku-browser-2.2.3/src/shimoku/cli/main.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/cli/persistence.py` & `shimoku-browser-2.2.3/src/shimoku/cli/persistence.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/cli/playground.py` & `shimoku-browser-2.2.3/src/shimoku/cli/playground.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/cli/utils.py` & `shimoku-browser-2.2.3/src/shimoku/cli/utils.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/code_gen/business_code_gen/apps_code_gen/code_gen_from_apps.py` & `shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/code_gen_from_apps.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/code_gen/business_code_gen/apps_code_gen/data_sets_code_gen/code_gen_from_data_sets.py` & `shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/data_sets_code_gen/code_gen_from_data_sets.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/code_gen_from_reports.py` & `shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/code_gen_from_reports.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_annotated_echart.py` & `shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_annotated_echart.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_button.py` & `shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_button.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_echarts.py` & `shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_echarts.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_filter.py` & `shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_filter.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_form.py` & `shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_form.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_html.py` & `shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_html.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_iframe.py` & `shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_iframe.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_indicators.py` & `shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_indicators.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_modal.py` & `shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_modal.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_other.py` & `shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_other.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_table.py` & `shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_table.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_tabs.py` & `shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_tabs.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/code_gen/business_code_gen/code_gen_from_business.py` & `shimoku-browser-2.2.3/src/shimoku/code_gen/business_code_gen/code_gen_from_business.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/code_gen/file_generator.py` & `shimoku-browser-2.2.3/src/shimoku/code_gen/file_generator.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/code_gen/main_code_gen.py` & `shimoku-browser-2.2.3/src/shimoku/code_gen/main_code_gen.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/code_gen/tree_generation.py` & `shimoku-browser-2.2.3/src/shimoku/code_gen/tree_generation.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/code_gen/utils_code_gen.py` & `shimoku-browser-2.2.3/src/shimoku/code_gen/utils_code_gen.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/exceptions.py` & `shimoku-browser-2.2.3/src/shimoku/exceptions.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/execution_logger.py` & `shimoku-browser-2.2.3/src/shimoku/execution_logger.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/playground/execute_local_server.py` & `shimoku-browser-2.2.3/src/shimoku/playground/execute_local_server.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/playground/local_server.py` & `shimoku-browser-2.2.3/src/shimoku/playground/local_server.py`

 * *Files 4% similar despite different names*

```diff
@@ -155,15 +155,55 @@
 
         if type_name in is_child_of:
             parent_type = is_child_of[type_name]
             name = "list" + get_plural(get_resource_name(type_name, to_lower=False))
             query_fields[name] = list_query_field(types, db, parent_type, type_name)
 
     Query = type("Query", (graphene.ObjectType,), query_fields)
-    schema = graphene.Schema(query=Query, subscription=Subscription)
+
+    # TODO: Implement mutations
+    ##################-TEMPORAL!-#####################
+    ####-just so frontend doesnt display an error-####
+    ###########-fix when mutations needed-############
+    from graphene import Mutation, InputObjectType
+
+    class UpdateUserInputExposed(InputObjectType):
+        id = graphene.ID(required=True)
+        name = graphene.String()
+        email = graphene.String()
+        companyName = graphene.String()
+        companyRole = graphene.String()
+        createdAt = graphene.String()
+        phoneNumber = graphene.String()
+        birthDate = graphene.String()
+        accountInUseId = graphene.String()
+        shopifyMasterAccountId = graphene.String()
+        cognitoId = graphene.String()
+        updateApiToken = graphene.Boolean()
+        kindOfUser = graphene.String()
+        newsletterAccepted = graphene.String()
+
+    class UpdateUser(Mutation):
+        class Arguments:
+            input = UpdateUserInputExposed(required=True)
+
+        id = graphene.String()
+        ok = graphene.Boolean()
+
+        def mutate(self, info, input):
+            return UpdateUser(ok=True, id=input.id)
+
+    class MyMutations(graphene.ObjectType):
+        updateUser = UpdateUser.Field()
+
+    ##################################################
+    ##################################################
+    ##################################################
+
+    schema = graphene.Schema(query=Query, subscription=Subscription, mutation=MyMutations)
 
     # Integrate with FastAPI (assuming you have a way to do this)
     graphql_app = GraphQLApp(schema, on_get=make_graphiql_handler())
     fast_api_app.add_route("/graphql", graphql_app)
     fast_api_app.add_websocket_route("/graphql", graphql_app)
```

### Comparing `shimoku-browser-2.2.2/src/shimoku/playground/schema_classes.py` & `shimoku-browser-2.2.3/src/shimoku/playground/schema_classes.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/playground/schema_parameter_classses.py` & `shimoku-browser-2.2.3/src/shimoku/playground/schema_parameter_classses.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/playground/websockets_server.py` & `shimoku-browser-2.2.3/src/shimoku/playground/websockets_server.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/plt/EChart_definitions/bar.py` & `shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/bar.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/plt/EChart_definitions/default_echart_options.py` & `shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/default_echart_options.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/plt/EChart_definitions/funnel.py` & `shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/funnel.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/plt/EChart_definitions/gauge.py` & `shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/gauge.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/plt/EChart_definitions/gauge_indicator.py` & `shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/gauge_indicator.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/plt/EChart_definitions/heatmap.py` & `shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/heatmap.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/plt/EChart_definitions/line.py` & `shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/line.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/plt/EChart_definitions/line_and_bar.py` & `shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/line_and_bar.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/plt/EChart_definitions/pie.py` & `shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/pie.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/plt/EChart_definitions/radar.py` & `shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/radar.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/plt/EChart_definitions/sankey.py` & `shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/sankey.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/plt/EChart_definitions/scatter.py` & `shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/scatter.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/plt/EChart_definitions/shimoku_gauge.py` & `shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/shimoku_gauge.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/plt/EChart_definitions/sunburst.py` & `shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/sunburst.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/plt/EChart_definitions/top_bottom.py` & `shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/top_bottom.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/plt/EChart_definitions/tree.py` & `shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/tree.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/plt/EChart_definitions/treemap.py` & `shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/treemap.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/plt/EChart_definitions/waterfall.py` & `shimoku-browser-2.2.3/src/shimoku/plt/EChart_definitions/waterfall.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/plt/bentobox_charts.py` & `shimoku-browser-2.2.3/src/shimoku/plt/bentobox_charts.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/plt/generated_headers/PlotLayerHeader.py` & `shimoku-browser-2.2.3/src/shimoku/plt/generated_headers/PlotLayerHeader.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,36 @@
 
 
 class PlotLayerHeader:
     """
     This class is a high level abstraction of the API, it is used to create components and data sets easily.
     """
 
+    def action_button(
+        self,
+        label: str,
+        order: int,
+        action_id: str,
+        rows_size: Optional[int] = 1,
+        cols_size: int = 2,
+        align: Optional[str] = "stretch",
+        padding: Optional[str] = None,
+    ):
+        """
+        Create a button in the dashboard that executes an action.
+        :param label: the label of the button
+        :param order: the order of the button
+        :param action_id: the id of the action
+        :param rows_size: the size of the rows in the button
+        :param cols_size: the size of the columns in the button
+        :param align: the alignment of the button
+        :param padding: the padding of the button
+        """
+        pass
+
     def activity_button(
         self,
         label: str,
         order: int,
         rows_size: Optional[int] = 1,
         cols_size: int = 2,
         align: Optional[str] = "stretch",
@@ -500,25 +522,27 @@
         order: int,
         padding: Optional[str] = None,
         rows_size: Optional[int] = None,
         cols_size: Optional[int] = None,
         modal: Optional[str] = None,
         activity_id: Optional[str] = None,
         activity_name: Optional[str] = None,
+        action_id: Optional[str] = None,
         on_submit_events: Optional[list[dict]] = None,
     ):
         """Creates an input form.
         :param options: the options for the input form
         :param order: the order of the input form
         :param padding: the padding of the input form
         :param rows_size: the rows size of the input form
         :param cols_size: the columns size of the input form
         :param modal: the modal to open after submitting the form
         :param activity_id: the activity id to run after submitting the form
         :param activity_name: the activity name to run after submitting the form
+        :param action_id: the action id to run after submitting the form
         :param on_submit_events: the events to run after submitting the form
         """
         pass
 
     def line(
         self,
         data: Union[str, DataFrame, list[dict]],
```

### Comparing `shimoku-browser-2.2.2/src/shimoku/plt/plt_layer.py` & `shimoku-browser-2.2.3/src/shimoku/plt/plt_layer.py`

 * *Files 2% similar despite different names*

```diff
@@ -3124,2293 +3124,2390 @@
 0000c330: 7479 5f69 642c 0a20 2020 2020 2020 2020  ty_id,.         
 0000c340: 2020 2020 2020 2020 2020 2029 2c0a 2020             ),.  
 0000c350: 2020 2020 2020 2020 2020 2020 2020 290a                ).
 0000c360: 2020 2020 2020 2020 2020 2020 5d2c 0a20              ],. 
 0000c370: 2020 2020 2020 2029 0a0a 2020 2020 4061         )..    @a
 0000c380: 6464 5f74 6f5f 6765 6e65 7261 6c5f 6173  dd_to_general_as
 0000c390: 796e 635f 6772 6f75 700a 2020 2020 6173  ync_group.    as
-0000c3a0: 796e 6320 6465 6620 7461 626c 6528 0a20  ync def table(. 
-0000c3b0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-0000c3c0: 2020 2020 206f 7264 6572 3a20 696e 742c       order: int,
-0000c3d0: 0a20 2020 2020 2020 2064 6174 613a 2055  .        data: U
-0000c3e0: 6e69 6f6e 5b73 7472 2c20 7064 2e44 6174  nion[str, pd.Dat
-0000c3f0: 6146 7261 6d65 2c20 6c69 7374 5b64 6963  aFrame, list[dic
-0000c400: 745d 2c20 6469 6374 5d2c 0a20 2020 2020  t], dict],.     
-0000c410: 2020 2063 6f6c 756d 6e73 3a20 4f70 7469     columns: Opti
-0000c420: 6f6e 616c 5b6c 6973 745b 7374 725d 5d20  onal[list[str]] 
-0000c430: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-0000c440: 636f 6c75 6d6e 735f 6275 7474 6f6e 3a20  columns_button: 
-0000c450: 626f 6f6c 203d 2054 7275 652c 0a20 2020  bool = True,.   
-0000c460: 2020 2020 2066 696c 7465 7273 3a20 626f       filters: bo
-0000c470: 6f6c 203d 2054 7275 652c 0a20 2020 2020  ol = True,.     
-0000c480: 2020 2065 7870 6f72 745f 746f 5f63 7376     export_to_csv
-0000c490: 3a20 626f 6f6c 203d 2054 7275 652c 0a20  : bool = True,. 
-0000c4a0: 2020 2020 2020 2073 6561 7263 683a 2062         search: b
-0000c4b0: 6f6f 6c20 3d20 5472 7565 2c0a 2020 2020  ool = True,.    
-0000c4c0: 2020 2020 7061 6765 5f73 697a 653a 2069      page_size: i
-0000c4d0: 6e74 203d 2031 302c 0a20 2020 2020 2020  nt = 10,.       
-0000c4e0: 2070 6167 655f 7369 7a65 5f6f 7074 696f   page_size_optio
-0000c4f0: 6e73 3a20 4f70 7469 6f6e 616c 5b6c 6973  ns: Optional[lis
-0000c500: 745b 696e 745d 5d20 3d20 4e6f 6e65 2c0a  t[int]] = None,.
-0000c510: 2020 2020 2020 2020 696e 6974 6961 6c5f          initial_
-0000c520: 736f 7274 5f63 6f6c 756d 6e3a 204f 7074  sort_column: Opt
-0000c530: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-0000c540: 652c 0a20 2020 2020 2020 2073 6f72 745f  e,.        sort_
-0000c550: 6465 7363 656e 6469 6e67 3a20 626f 6f6c  descending: bool
-0000c560: 203d 2046 616c 7365 2c0a 2020 2020 2020   = False,.      
-0000c570: 2020 636f 6c75 6d6e 735f 6f70 7469 6f6e    columns_option
-0000c580: 733a 204f 7074 696f 6e61 6c5b 6469 6374  s: Optional[dict
-0000c590: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-0000c5a0: 2020 6361 7465 676f 7269 6361 6c5f 636f    categorical_co
-0000c5b0: 6c75 6d6e 733a 204f 7074 696f 6e61 6c5b  lumns: Optional[
-0000c5c0: 6c69 7374 5b73 7472 5d5d 203d 204e 6f6e  list[str]] = Non
-0000c5d0: 652c 0a20 2020 2020 2020 206c 6162 656c  e,.        label
-0000c5e0: 5f63 6f6c 756d 6e73 3a20 4f70 7469 6f6e  _columns: Option
-0000c5f0: 616c 5b64 6963 745d 203d 204e 6f6e 652c  al[dict] = None,
-0000c600: 0a20 2020 2020 2020 2077 6562 5f6c 696e  .        web_lin
-0000c610: 6b5f 636f 6c75 6d6e 3a20 4f70 7469 6f6e  k_column: Option
-0000c620: 616c 5b73 7472 5d20 3d20 4e6f 6e65 2c0a  al[str] = None,.
-0000c630: 2020 2020 2020 2020 6f70 656e 5f6c 696e          open_lin
-0000c640: 6b5f 696e 5f6e 6577 5f74 6162 3a20 626f  k_in_new_tab: bo
-0000c650: 6f6c 203d 2046 616c 7365 2c0a 2020 2020  ol = False,.    
-0000c660: 2020 2020 7469 746c 653a 204f 7074 696f      title: Optio
-0000c670: 6e61 6c5b 7374 725d 203d 204e 6f6e 652c  nal[str] = None,
-0000c680: 0a20 2020 2020 2020 2070 6164 6469 6e67  .        padding
-0000c690: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
-0000c6a0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-0000c6b0: 726f 7773 5f73 697a 653a 204f 7074 696f  rows_size: Optio
-0000c6c0: 6e61 6c5b 696e 745d 203d 204e 6f6e 652c  nal[int] = None,
-0000c6d0: 0a20 2020 2020 2020 2063 6f6c 735f 7369  .        cols_si
-0000c6e0: 7a65 3a20 4f70 7469 6f6e 616c 5b69 6e74  ze: Optional[int
-0000c6f0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 293a  ] = None,.    ):
-0000c700: 0a20 2020 2020 2020 2022 2222 4372 6561  .        """Crea
-0000c710: 7465 2061 2074 6162 6c65 2072 6570 6f72  te a table repor
-0000c720: 7420 696e 2074 6865 2064 6173 6862 6f61  t in the dashboa
-0000c730: 7264 2e0a 2020 2020 2020 2020 3a70 6172  rd..        :par
-0000c740: 616d 206f 7264 6572 3a20 7468 6520 6f72  am order: the or
-0000c750: 6465 7220 6f66 2074 6865 2074 6162 6c65  der of the table
-0000c760: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-0000c770: 6461 7461 3a20 7468 6520 6461 7461 206f  data: the data o
-0000c780: 6620 7468 6520 7461 626c 650a 2020 2020  f the table.    
-0000c790: 2020 2020 3a70 6172 616d 2063 6f6c 756d      :param colum
-0000c7a0: 6e73 3a20 7468 6520 636f 6c75 6d6e 7320  ns: the columns 
-0000c7b0: 6f66 2074 6865 2074 6162 6c65 0a20 2020  of the table.   
-0000c7c0: 2020 2020 203a 7061 7261 6d20 636f 6c75       :param colu
-0000c7d0: 6d6e 735f 6275 7474 6f6e 3a20 7768 6574  mns_button: whet
-0000c7e0: 6865 7220 746f 2073 686f 7720 7468 6520  her to show the 
-0000c7f0: 636f 6c75 6d6e 7320 6275 7474 6f6e 0a20  columns button. 
-0000c800: 2020 2020 2020 203a 7061 7261 6d20 6669         :param fi
-0000c810: 6c74 6572 733a 2077 6865 7468 6572 2074  lters: whether t
-0000c820: 6f20 7368 6f77 2074 6865 2066 696c 7465  o show the filte
-0000c830: 7273 2062 7574 746f 6e0a 2020 2020 2020  rs button.      
-0000c840: 2020 3a70 6172 616d 2065 7870 6f72 745f    :param export_
-0000c850: 746f 5f63 7376 3a20 7768 6574 6865 7220  to_csv: whether 
-0000c860: 746f 2073 686f 7720 7468 6520 6578 706f  to show the expo
-0000c870: 7274 2074 6f20 6373 7620 6275 7474 6f6e  rt to csv button
-0000c880: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-0000c890: 7365 6172 6368 3a20 7768 6574 6865 7220  search: whether 
-0000c8a0: 746f 2073 686f 7720 7468 6520 7365 6172  to show the sear
-0000c8b0: 6368 2062 6172 0a20 2020 2020 2020 203a  ch bar.        :
-0000c8c0: 7061 7261 6d20 7061 6765 5f73 697a 653a  param page_size:
-0000c8d0: 2074 6865 206e 756d 6265 7220 6f66 2072   the number of r
-0000c8e0: 6f77 7320 7065 7220 7061 6765 0a20 2020  ows per page.   
-0000c8f0: 2020 2020 203a 7061 7261 6d20 7061 6765       :param page
-0000c900: 5f73 697a 655f 6f70 7469 6f6e 733a 2074  _size_options: t
-0000c910: 6865 206f 7074 696f 6e73 2066 6f72 2074  he options for t
-0000c920: 6865 206e 756d 6265 7220 6f66 2072 6f77  he number of row
-0000c930: 7320 7065 7220 7061 6765 0a20 2020 2020  s per page.     
-0000c940: 2020 203a 7061 7261 6d20 696e 6974 6961     :param initia
-0000c950: 6c5f 736f 7274 5f63 6f6c 756d 6e3a 2074  l_sort_column: t
-0000c960: 6865 2069 6e69 7469 616c 2073 6f72 7469  he initial sorti
-0000c970: 6e67 2063 6f6c 756d 6e0a 2020 2020 2020  ng column.      
-0000c980: 2020 3a70 6172 616d 2073 6f72 745f 6465    :param sort_de
-0000c990: 7363 656e 6469 6e67 3a20 7768 6574 6865  scending: whethe
-0000c9a0: 7220 746f 2073 6f72 7420 6465 7363 656e  r to sort descen
-0000c9b0: 6469 6e67 2062 7920 7468 6520 696e 6974  ding by the init
-0000c9c0: 6961 6c20 736f 7274 696e 6720 636f 6c75  ial sorting colu
-0000c9d0: 6d6e 0a20 2020 2020 2020 203a 7061 7261  mn.        :para
-0000c9e0: 6d20 636f 6c75 6d6e 735f 6f70 7469 6f6e  m columns_option
-0000c9f0: 733a 2074 6865 206f 7074 696f 6e73 2066  s: the options f
-0000ca00: 6f72 2074 6865 2063 6f6c 756d 6e73 0a20  or the columns. 
-0000ca10: 2020 2020 2020 203a 7061 7261 6d20 6361         :param ca
-0000ca20: 7465 676f 7269 6361 6c5f 636f 6c75 6d6e  tegorical_column
-0000ca30: 733a 2074 6865 2063 6174 6567 6f72 6963  s: the categoric
-0000ca40: 616c 2063 6f6c 756d 6e73 0a20 2020 2020  al columns.     
-0000ca50: 2020 203a 7061 7261 6d20 6c61 6265 6c5f     :param label_
-0000ca60: 636f 6c75 6d6e 733a 2074 6865 206c 6162  columns: the lab
-0000ca70: 656c 2063 6f6c 756d 6e73 0a20 2020 2020  el columns.     
-0000ca80: 2020 203a 7061 7261 6d20 7265 706f 7274     :param report
-0000ca90: 5f70 6172 616d 733a 2061 6464 6974 696f  _params: additio
-0000caa0: 6e61 6c20 7265 706f 7274 2070 6172 616d  nal report param
-0000cab0: 6574 6572 7320 6173 206b 6579 2d76 616c  eters as key-val
-0000cac0: 7565 2070 6169 7273 0a20 2020 2020 2020  ue pairs.       
-0000cad0: 203a 7061 7261 6d20 7765 625f 6c69 6e6b   :param web_link
-0000cae0: 5f63 6f6c 756d 6e3a 2074 6865 2063 6f6c  _column: the col
-0000caf0: 756d 6e20 746f 2075 7365 2061 7320 7765  umn to use as we
-0000cb00: 6220 6c69 6e6b 0a20 2020 2020 2020 203a  b link.        :
-0000cb10: 7061 7261 6d20 6f70 656e 5f6c 696e 6b5f  param open_link_
-0000cb20: 696e 5f6e 6577 5f74 6162 3a20 7768 6574  in_new_tab: whet
-0000cb30: 6865 7220 746f 206f 7065 6e20 7468 6520  her to open the 
-0000cb40: 7765 6220 6c69 6e6b 2069 6e20 6120 6e65  web link in a ne
-0000cb50: 7720 7461 620a 2020 2020 2020 2020 3a70  w tab.        :p
-0000cb60: 6172 616d 2074 6974 6c65 3a20 7468 6520  aram title: the 
-0000cb70: 7469 746c 6520 6f66 2074 6865 2074 6162  title of the tab
-0000cb80: 6c65 0a20 2020 2020 2020 203a 7061 7261  le.        :para
-0000cb90: 6d20 7061 6464 696e 673a 2074 6865 2070  m padding: the p
-0000cba0: 6164 6469 6e67 206f 6620 7468 6520 7461  adding of the ta
-0000cbb0: 626c 650a 2020 2020 2020 2020 3a70 6172  ble.        :par
-0000cbc0: 616d 2072 6f77 735f 7369 7a65 3a20 7468  am rows_size: th
-0000cbd0: 6520 726f 7773 2073 697a 6520 6f66 2074  e rows size of t
-0000cbe0: 6865 2074 6162 6c65 0a20 2020 2020 2020  he table.       
-0000cbf0: 203a 7061 7261 6d20 636f 6c73 5f73 697a   :param cols_siz
-0000cc00: 653a 2074 6865 2063 6f6c 756d 6e73 2073  e: the columns s
-0000cc10: 697a 6520 6f66 2074 6865 2074 6162 6c65  ize of the table
-0000cc20: 0a20 2020 2020 2020 2022 2222 0a0a 2020  .        """..  
-0000cc30: 2020 2020 2020 6461 7461 5f6d 6170 7069        data_mappi
-0000cc40: 6e67 735f 746f 5f74 7570 6c65 7320 3d20  ngs_to_tuples = 
-0000cc50: 6177 6169 7420 7365 6c66 2e5f 6368 6f6f  await self._choo
-0000cc60: 7365 5f64 6174 6128 6f72 6465 722c 2064  se_data(order, d
-0000cc70: 6174 612c 2054 6162 6c65 290a 2020 2020  ata, Table).    
-0000cc80: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
-0000cc90: 6528 6461 7461 2c20 7374 7229 3a0a 2020  e(data, str):.  
-0000cca0: 2020 2020 2020 2020 2020 6461 7461 203d            data =
-0000ccb0: 2073 656c 662e 5f73 6861 7265 645f 6461   self._shared_da
-0000ccc0: 7461 5b64 6174 615d 0a0a 2020 2020 2020  ta[data]..      
-0000ccd0: 2020 6466 203d 2076 616c 6964 6174 655f    df = validate_
-0000cce0: 6461 7461 5f69 735f 7061 6e64 6172 6162  data_is_pandarab
-0000ccf0: 6c65 2864 6174 6129 0a0a 2020 2020 2020  le(data)..      
-0000cd00: 2020 6966 206e 6f74 2063 6f6c 756d 6e73    if not columns
-0000cd10: 3a0a 2020 2020 2020 2020 2020 2020 636f  :.            co
-0000cd20: 6c75 6d6e 7320 3d20 6c69 7374 2864 6174  lumns = list(dat
-0000cd30: 615f 6d61 7070 696e 6773 5f74 6f5f 7475  a_mappings_to_tu
-0000cd40: 706c 6573 2e6b 6579 7328 2929 0a20 2020  ples.keys()).   
-0000cd50: 2020 2020 2069 6620 6e6f 7420 636f 6c75       if not colu
-0000cd60: 6d6e 735f 6f70 7469 6f6e 733a 0a20 2020  mns_options:.   
-0000cd70: 2020 2020 2020 2020 2063 6f6c 756d 6e73           columns
-0000cd80: 5f6f 7074 696f 6e73 203d 207b 7d0a 2020  _options = {}.  
-0000cd90: 2020 2020 2020 6966 206e 6f74 2063 6174        if not cat
-0000cda0: 6567 6f72 6963 616c 5f63 6f6c 756d 6e73  egorical_columns
-0000cdb0: 3a0a 2020 2020 2020 2020 2020 2020 6361  :.            ca
-0000cdc0: 7465 676f 7269 6361 6c5f 636f 6c75 6d6e  tegorical_column
-0000cdd0: 7320 3d20 5b5d 0a20 2020 2020 2020 2069  s = [].        i
-0000cde0: 6620 6e6f 7420 6c61 6265 6c5f 636f 6c75  f not label_colu
-0000cdf0: 6d6e 733a 0a20 2020 2020 2020 2020 2020  mns:.           
-0000ce00: 206c 6162 656c 5f63 6f6c 756d 6e73 203d   label_columns =
-0000ce10: 207b 7d0a 2020 2020 2020 2020 656c 7365   {}.        else
-0000ce20: 3a0a 2020 2020 2020 2020 2020 2020 6175  :.            au
-0000ce30: 785f 6c61 6265 6c5f 636f 6c75 6d6e 7320  x_label_columns 
-0000ce40: 3d20 6c61 6265 6c5f 636f 6c75 6d6e 730a  = label_columns.
-0000ce50: 2020 2020 2020 2020 2020 2020 6c61 6265              labe
-0000ce60: 6c5f 636f 6c75 6d6e 7320 3d20 7b7d 0a20  l_columns = {}. 
-0000ce70: 2020 2020 2020 2020 2020 2066 6f72 2068             for h
-0000ce80: 6173 5f74 6f5f 6265 5f74 7570 6c65 2069  as_to_be_tuple i
-0000ce90: 6e20 6175 785f 6c61 6265 6c5f 636f 6c75  n aux_label_colu
-0000cea0: 6d6e 733a 0a20 2020 2020 2020 2020 2020  mns:.           
-0000ceb0: 2020 2020 2076 203d 2061 7578 5f6c 6162       v = aux_lab
-0000cec0: 656c 5f63 6f6c 756d 6e73 5b68 6173 5f74  el_columns[has_t
-0000ced0: 6f5f 6265 5f74 7570 6c65 5d0a 2020 2020  o_be_tuple].    
-0000cee0: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-0000cef0: 7369 6e73 7461 6e63 6528 6861 735f 746f  sinstance(has_to
-0000cf00: 5f62 655f 7475 706c 652c 2073 7472 293a  _be_tuple, str):
-0000cf10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000cf20: 2020 2020 206c 6162 656c 5f63 6f6c 756d       label_colum
-0000cf30: 6e73 5b28 6861 735f 746f 5f62 655f 7475  ns[(has_to_be_tu
-0000cf40: 706c 652c 2022 6669 6c6c 6564 2229 5d20  ple, "filled")] 
-0000cf50: 3d20 760a 2020 2020 2020 2020 2020 2020  = v.            
-0000cf60: 2020 2020 656c 6966 2069 7369 6e73 7461      elif isinsta
-0000cf70: 6e63 6528 6861 735f 746f 5f62 655f 7475  nce(has_to_be_tu
-0000cf80: 706c 652c 2074 7570 6c65 293a 0a20 2020  ple, tuple):.   
-0000cf90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cfa0: 206c 6162 656c 5f63 6f6c 756d 6e73 5b68   label_columns[h
-0000cfb0: 6173 5f74 6f5f 6265 5f74 7570 6c65 5d20  as_to_be_tuple] 
-0000cfc0: 3d20 760a 2020 2020 2020 2020 2020 2020  = v.            
-0000cfd0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0000cfe0: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-0000cff0: 675f 6572 726f 7228 0a20 2020 2020 2020  g_error(.       
-0000d000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d010: 206c 6f67 6765 722c 0a20 2020 2020 2020   logger,.       
-0000d020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d030: 2066 2249 6e76 616c 6964 206c 6162 656c   f"Invalid label
-0000d040: 5f63 6f6c 756d 6e73 206b 6579 3a20 7b68  _columns key: {h
-0000d050: 6173 5f74 6f5f 6265 5f74 7570 6c65 7d22  as_to_be_tuple}"
-0000d060: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000d070: 2020 2020 2020 2020 2020 5661 6c75 6545            ValueE
-0000d080: 7272 6f72 2c0a 2020 2020 2020 2020 2020  rror,.          
-0000d090: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-0000d0a0: 2020 2020 6c61 6265 6c5f 6a75 7374 5f63      label_just_c
-0000d0b0: 6f6c 756d 6e73 203d 205b 785b 305d 2066  olumns = [x[0] f
-0000d0c0: 6f72 2078 2069 6e20 6c61 6265 6c5f 636f  or x in label_co
-0000d0d0: 6c75 6d6e 732e 6b65 7973 2829 5d0a 0a20  lumns.keys()].. 
-0000d0e0: 2020 2020 2020 205f 2c20 6461 7461 5f73         _, data_s
-0000d0f0: 6574 2c20 5f20 3d20 6461 7461 5f6d 6170  et, _ = data_map
-0000d100: 7069 6e67 735f 746f 5f74 7570 6c65 735b  pings_to_tuples[
-0000d110: 636f 6c75 6d6e 735b 305d 5d0a 2020 2020  columns[0]].    
-0000d120: 2020 2020 636f 6c75 6d6e 735f 6469 6374      columns_dict
-0000d130: 7320 3d20 5b5d 0a20 2020 2020 2020 2072  s = [].        r
-0000d140: 6f77 735f 6469 6374 203d 207b 226d 6170  ows_dict = {"map
-0000d150: 7069 6e67 223a 207b 7d7d 0a20 2020 2020  ping": {}}.     
-0000d160: 2020 2066 6f72 2069 2c20 6e61 6d65 2069     for i, name i
-0000d170: 6e20 656e 756d 6572 6174 6528 636f 6c75  n enumerate(colu
-0000d180: 6d6e 7329 3a0a 2020 2020 2020 2020 2020  mns):.          
-0000d190: 2020 636f 6c75 6d6e 5f6f 7074 696f 6e73    column_options
-0000d1a0: 203d 207b 2266 6965 6c64 223a 206e 616d   = {"field": nam
-0000d1b0: 652c 2022 6865 6164 6572 4e61 6d65 223a  e, "headerName":
-0000d1c0: 206e 616d 652c 2022 6f72 6465 7222 3a20   name, "order": 
-0000d1d0: 697d 0a0a 2020 2020 2020 2020 2020 2020  i}..            
-0000d1e0: 6966 206e 616d 6520 696e 2063 6f6c 756d  if name in colum
-0000d1f0: 6e73 5f6f 7074 696f 6e73 3a0a 2020 2020  ns_options:.    
-0000d200: 2020 2020 2020 2020 2020 2020 636f 6c75              colu
-0000d210: 6d6e 5f6f 7074 696f 6e73 2e75 7064 6174  mn_options.updat
-0000d220: 6528 636f 6c75 6d6e 735f 6f70 7469 6f6e  e(columns_option
-0000d230: 735b 6e61 6d65 5d29 0a0a 2020 2020 2020  s[name])..      
-0000d240: 2020 2020 2020 6966 206e 616d 6520 696e        if name in
-0000d250: 2063 6174 6567 6f72 6963 616c 5f63 6f6c   categorical_col
-0000d260: 756d 6e73 3a0a 2020 2020 2020 2020 2020  umns:.          
-0000d270: 2020 2020 2020 6966 206e 616d 6520 696e        if name in
-0000d280: 206c 6162 656c 5f63 6f6c 756d 6e73 3a0a   label_columns:.
-0000d290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d2a0: 2020 2020 6c6f 675f 6572 726f 7228 0a20      log_error(. 
-0000d2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d2c0: 2020 2020 2020 206c 6f67 6765 722c 0a20         logger,. 
-0000d2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d2e0: 2020 2020 2020 2066 2243 6f6c 756d 6e73         f"Columns
-0000d2f0: 2063 616e 6e6f 7420 6265 2062 6f74 6820   cannot be both 
-0000d300: 696e 636c 7564 6564 2069 6e20 6361 7465  included in cate
-0000d310: 676f 7269 6361 6c5f 636f 6c75 6d6e 7320  gorical_columns 
-0000d320: 616e 6420 6c61 6265 6c5f 636f 6c75 6d6e  and label_column
-0000d330: 733a 207b 6e61 6d65 7d22 2c0a 2020 2020  s: {name}",.    
-0000d340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d350: 2020 2020 5661 6c75 6545 7272 6f72 2c0a      ValueError,.
-0000d360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d370: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-0000d380: 2020 2020 2020 636f 6c75 6d6e 5f6f 7074        column_opt
-0000d390: 696f 6e73 5b22 7479 7065 225d 203d 2022  ions["type"] = "
-0000d3a0: 7369 6e67 6c65 5365 6c65 6374 220a 2020  singleSelect".  
-0000d3b0: 2020 2020 2020 2020 2020 2020 2020 636f                co
-0000d3c0: 6c75 6d6e 5f6f 7074 696f 6e73 5b22 6f70  lumn_options["op
-0000d3d0: 7469 6f6e 7322 5d20 3d20 6466 5b6e 616d  tions"] = df[nam
-0000d3e0: 655d 2e75 6e69 7175 6528 292e 746f 6c69  e].unique().toli
-0000d3f0: 7374 2829 0a0a 2020 2020 2020 2020 2020  st()..          
-0000d400: 2020 6966 206e 616d 6520 696e 206c 6162    if name in lab
-0000d410: 656c 5f6a 7573 745f 636f 6c75 6d6e 733a  el_just_columns:
-0000d420: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d430: 2069 6e64 6578 203d 206c 6162 656c 5f6a   index = label_j
-0000d440: 7573 745f 636f 6c75 6d6e 732e 696e 6465  ust_columns.inde
-0000d450: 7828 6e61 6d65 290a 2020 2020 2020 2020  x(name).        
-0000d460: 2020 2020 2020 2020 285f 2c20 7661 7269          (_, vari
-0000d470: 616e 7429 2c20 6c61 6265 6c5f 6f70 7469  ant), label_opti
-0000d480: 6f6e 7320 3d20 6c69 7374 286c 6162 656c  ons = list(label
-0000d490: 5f63 6f6c 756d 6e73 2e69 7465 6d73 2829  _columns.items()
-0000d4a0: 295b 696e 6465 785d 0a20 2020 2020 2020  )[index].       
-0000d4b0: 2020 2020 2020 2020 2063 6f6c 756d 6e5f           column_
-0000d4c0: 6f70 7469 6f6e 735b 2263 6869 7073 225d  options["chips"]
-0000d4d0: 203d 207b 7d0a 2020 2020 2020 2020 2020   = {}.          
-0000d4e0: 2020 2020 2020 636f 6c75 6d6e 5f6f 7074        column_opt
-0000d4f0: 696f 6e73 5b22 6368 6970 7322 5d5b 2276  ions["chips"]["v
-0000d500: 6172 6961 6e74 225d 203d 2076 6172 6961  ariant"] = varia
-0000d510: 6e74 0a20 2020 2020 2020 2020 2020 2020  nt.             
-0000d520: 2020 2063 6f6c 756d 6e5f 6f70 7469 6f6e     column_option
-0000d530: 735b 2263 6869 7073 225d 5b22 6f70 7469  s["chips"]["opti
-0000d540: 6f6e 7322 5d20 3d20 696e 7465 7270 7265  ons"] = interpre
-0000d550: 745f 6c61 6265 6c5f 696e 666f 280a 2020  t_label_info(.  
-0000d560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d570: 2020 6466 2c20 6e61 6d65 2c20 6c61 6265    df, name, labe
-0000d580: 6c5f 6f70 7469 6f6e 732c 2076 6172 6961  l_options, varia
-0000d590: 6e74 0a20 2020 2020 2020 2020 2020 2020  nt.             
-0000d5a0: 2020 2029 0a0a 2020 2020 2020 2020 2020     )..          
-0000d5b0: 2020 6966 206e 616d 6520 3d3d 2077 6562    if name == web
-0000d5c0: 5f6c 696e 6b5f 636f 6c75 6d6e 3a0a 2020  _link_column:.  
-0000d5d0: 2020 2020 2020 2020 2020 2020 2020 636f                co
-0000d5e0: 6c75 6d6e 5f6f 7074 696f 6e73 5b22 6c69  lumn_options["li
-0000d5f0: 6e6b 225d 203d 207b 0a20 2020 2020 2020  nk"] = {.       
-0000d600: 2020 2020 2020 2020 2020 2020 2022 7572               "ur
-0000d610: 6c22 3a20 2277 6562 4c69 6e6b 222c 0a20  l": "webLink",. 
-0000d620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d630: 2020 2022 6f70 656e 4e65 7754 6162 223a     "openNewTab":
-0000d640: 206f 7065 6e5f 6c69 6e6b 5f69 6e5f 6e65   open_link_in_ne
-0000d650: 775f 7461 622c 0a20 2020 2020 2020 2020  w_tab,.         
-0000d660: 2020 2020 2020 207d 0a0a 2020 2020 2020         }..      
-0000d670: 2020 2020 2020 636f 6c75 6d6e 735f 6469        columns_di
-0000d680: 6374 732e 6170 7065 6e64 2863 6f6c 756d  cts.append(colum
-0000d690: 6e5f 6f70 7469 6f6e 7329 0a20 2020 2020  n_options).     
-0000d6a0: 2020 2020 2020 2072 6f77 735f 6469 6374         rows_dict
-0000d6b0: 5b22 6d61 7070 696e 6722 5d5b 6e61 6d65  ["mapping"][name
-0000d6c0: 5d20 3d20 6461 7461 5f6d 6170 7069 6e67  ] = data_mapping
-0000d6d0: 735f 746f 5f74 7570 6c65 735b 6e61 6d65  s_to_tuples[name
-0000d6e0: 5d5b 305d 0a0a 2020 2020 2020 2020 6966  ][0]..        if
-0000d6f0: 2077 6562 5f6c 696e 6b5f 636f 6c75 6d6e   web_link_column
-0000d700: 3a0a 2020 2020 2020 2020 2020 2020 726f  :.            ro
-0000d710: 7773 5f64 6963 745b 226d 6170 7069 6e67  ws_dict["mapping
-0000d720: 225d 5b22 7765 6222 5d20 3d20 6461 7461  "]["web"] = data
-0000d730: 5f6d 6170 7069 6e67 735f 746f 5f74 7570  _mappings_to_tup
-0000d740: 6c65 735b 7765 625f 6c69 6e6b 5f63 6f6c  les[web_link_col
-0000d750: 756d 6e5d 5b30 5d0a 2020 2020 2020 2020  umn][0].        
-0000d760: 2020 2020 726f 7773 5f64 6963 745b 226d      rows_dict["m
-0000d770: 6170 7069 6e67 225d 5b22 7765 624c 696e  apping"]["webLin
-0000d780: 6b22 5d20 3d20 6461 7461 5f6d 6170 7069  k"] = data_mappi
-0000d790: 6e67 735f 746f 5f74 7570 6c65 735b 7765  ngs_to_tuples[we
-0000d7a0: 625f 6c69 6e6b 5f63 6f6c 756d 6e5d 5b0a  b_link_column][.
-0000d7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d7c0: 300a 2020 2020 2020 2020 2020 2020 5d0a  0.            ].
-0000d7d0: 0a20 2020 2020 2020 205f 2c20 7265 706f  .        _, repo
-0000d7e0: 7274 203d 2061 7761 6974 2073 656c 662e  rt = await self.
-0000d7f0: 5f67 6574 5f63 6861 7274 5f72 6570 6f72  _get_chart_repor
-0000d800: 7428 6f72 6465 722c 2054 6162 6c65 290a  t(order, Table).
-0000d810: 0a20 2020 2020 2020 2072 6473 203d 2061  .        rds = a
-0000d820: 7761 6974 2072 6570 6f72 742e 6765 745f  wait report.get_
-0000d830: 7265 706f 7274 5f64 6174 615f 7365 7473  report_data_sets
-0000d840: 2829 0a0a 2020 2020 2020 2020 6966 2028  ()..        if (
-0000d850: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000d860: 662e 7265 7573 655f 6461 7461 5f73 6574  f.reuse_data_set
-0000d870: 730a 2020 2020 2020 2020 2020 2020 616e  s.            an
-0000d880: 6420 7265 706f 7274 5b22 7072 6f70 6572  d report["proper
-0000d890: 7469 6573 225d 2e67 6574 2822 636f 6c75  ties"].get("colu
-0000d8a0: 6d6e 7322 290a 2020 2020 2020 2020 2020  mns").          
-0000d8b0: 2020 616e 6420 7265 706f 7274 5b22 7072    and report["pr
-0000d8c0: 6f70 6572 7469 6573 225d 5b22 636f 6c75  operties"]["colu
-0000d8d0: 6d6e 7322 5d20 213d 2063 6f6c 756d 6e73  mns"] != columns
-0000d8e0: 5f64 6963 7473 0a20 2020 2020 2020 2029  _dicts.        )
-0000d8f0: 3a0a 2020 2020 2020 2020 2020 2020 6c6f  :.            lo
-0000d900: 675f 6572 726f 7228 0a20 2020 2020 2020  g_error(.       
-0000d910: 2020 2020 2020 2020 206c 6f67 6765 722c           logger,
-0000d920: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d930: 2022 436f 6c75 6d6e 7320 6f70 7469 6f6e   "Columns option
-0000d940: 7320 646f 206e 6f74 206d 6174 6368 2074  s do not match t
-0000d950: 6865 2070 7265 7669 6f75 7320 636f 6c75  he previous colu
-0000d960: 6d6e 732c 206d 6f73 7420 6c69 6b65 6c79  mns, most likely
-0000d970: 2064 6174 6120 6861 7320 6368 616e 6765   data has change
-0000d980: 642c 220a 2020 2020 2020 2020 2020 2020  d,".            
-0000d990: 2020 2020 2220 646f 6e27 7420 7573 6520      " don't use 
-0000d9a0: 7468 6520 7265 7573 655f 6461 7461 5f73  the reuse_data_s
-0000d9b0: 6574 7320 6f70 7469 6f6e 2069 6e20 7468  ets option in th
-0000d9c0: 6973 2063 6173 6522 2c0a 2020 2020 2020  is case",.      
-0000d9d0: 2020 2020 2020 2020 2020 4461 7461 4572            DataEr
-0000d9e0: 726f 722c 0a20 2020 2020 2020 2020 2020  ror,.           
-0000d9f0: 2029 0a0a 2020 2020 2020 2020 6966 2072   )..        if r
-0000da00: 6473 2061 6e64 2028 0a20 2020 2020 2020  ds and (.       
-0000da10: 2020 2020 206e 6f74 2073 656c 662e 7265       not self.re
-0000da20: 7573 655f 6461 7461 5f73 6574 730a 2020  use_data_sets.  
-0000da30: 2020 2020 2020 2020 2020 6f72 2061 6e79            or any
-0000da40: 2872 645b 2264 6174 6153 6574 4964 225d  (rd["dataSetId"]
-0000da50: 2021 3d20 6461 7461 5f73 6574 5b22 6964   != data_set["id
-0000da60: 225d 2066 6f72 2072 6420 696e 2072 6473  "] for rd in rds
-0000da70: 290a 2020 2020 2020 2020 293a 0a20 2020  ).        ):.   
-0000da80: 2020 2020 2020 2020 2061 7761 6974 2072           await r
-0000da90: 6570 6f72 742e 6465 6c65 7465 5f72 6570  eport.delete_rep
-0000daa0: 6f72 745f 6461 7461 5f73 6574 7328 6c6f  ort_data_sets(lo
-0000dab0: 673d 5472 7565 290a 2020 2020 2020 2020  g=True).        
-0000dac0: 2020 2020 7264 7320 3d20 5b5d 0a0a 2020      rds = []..  
-0000dad0: 2020 2020 2020 6966 206e 6f74 2072 6473        if not rds
-0000dae0: 3a0a 2020 2020 2020 2020 2020 2020 6177  :.            aw
-0000daf0: 6169 7420 7265 706f 7274 2e63 7265 6174  ait report.creat
-0000db00: 655f 7265 706f 7274 5f64 6174 615f 7365  e_report_data_se
-0000db10: 7428 284e 6f6e 652c 2064 6174 615f 7365  t((None, data_se
-0000db20: 742c 204e 6f6e 6529 290a 0a20 2020 2020  t, None))..     
-0000db30: 2020 2070 6167 696e 6174 696f 6e20 3d20     pagination = 
-0000db40: 7b22 7061 6765 5369 7a65 223a 2070 6167  {"pageSize": pag
-0000db50: 655f 7369 7a65 7d0a 2020 2020 2020 2020  e_size}.        
-0000db60: 6966 2070 6167 655f 7369 7a65 5f6f 7074  if page_size_opt
-0000db70: 696f 6e73 3a0a 2020 2020 2020 2020 2020  ions:.          
-0000db80: 2020 7061 6769 6e61 7469 6f6e 5b22 7061    pagination["pa
-0000db90: 6765 5369 7a65 4f70 7469 6f6e 7322 5d20  geSizeOptions"] 
-0000dba0: 3d20 7061 6765 5f73 697a 655f 6f70 7469  = page_size_opti
-0000dbb0: 6f6e 730a 0a20 2020 2020 2020 2073 6f72  ons..        sor
-0000dbc0: 7420 3d20 7b7d 0a20 2020 2020 2020 2069  t = {}.        i
-0000dbd0: 6620 696e 6974 6961 6c5f 736f 7274 5f63  f initial_sort_c
-0000dbe0: 6f6c 756d 6e3a 0a20 2020 2020 2020 2020  olumn:.         
-0000dbf0: 2020 2073 6f72 745b 2266 6965 6c64 225d     sort["field"]
-0000dc00: 203d 2064 6174 615f 6d61 7070 696e 6773   = data_mappings
-0000dc10: 5f74 6f5f 7475 706c 6573 5b69 6e69 7469  _to_tuples[initi
-0000dc20: 616c 5f73 6f72 745f 636f 6c75 6d6e 5d5b  al_sort_column][
-0000dc30: 305d 0a20 2020 2020 2020 2020 2020 2073  0].            s
-0000dc40: 6f72 745b 2264 6972 6563 7469 6f6e 225d  ort["direction"]
-0000dc50: 203d 2022 6173 6322 2069 6620 6e6f 7420   = "asc" if not 
-0000dc60: 736f 7274 5f64 6573 6365 6e64 696e 6720  sort_descending 
-0000dc70: 656c 7365 2022 6465 7363 220a 0a20 2020  else "desc"..   
-0000dc80: 2020 2020 2061 7761 6974 2073 656c 662e       await self.
-0000dc90: 5f63 7265 6174 655f 6368 6172 7428 0a20  _create_chart(. 
-0000dca0: 2020 2020 2020 2020 2020 2063 6861 7274             chart
-0000dcb0: 5f63 6c61 7373 3d54 6162 6c65 2c0a 2020  _class=Table,.  
-0000dcc0: 2020 2020 2020 2020 2020 6f72 6465 723d            order=
-0000dcd0: 6f72 6465 722c 0a20 2020 2020 2020 2020  order,.         
-0000dce0: 2020 2073 697a 6550 6164 6469 6e67 3d70     sizePadding=p
-0000dcf0: 6164 6469 6e67 2c0a 2020 2020 2020 2020  adding,.        
-0000dd00: 2020 2020 7369 7a65 526f 7773 3d72 6f77      sizeRows=row
-0000dd10: 735f 7369 7a65 2c0a 2020 2020 2020 2020  s_size,.        
-0000dd20: 2020 2020 7369 7a65 436f 6c75 6d6e 733d      sizeColumns=
-0000dd30: 636f 6c73 5f73 697a 652c 0a20 2020 2020  cols_size,.     
-0000dd40: 2020 2020 2020 2074 6974 6c65 3d74 6974         title=tit
-0000dd50: 6c65 2c0a 2020 2020 2020 2020 2020 2020  le,.            
-0000dd60: 7072 6f70 6572 7469 6573 3d64 6963 7428  properties=dict(
-0000dd70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000dd80: 2063 6f6c 756d 6e73 3d63 6f6c 756d 6e73   columns=columns
-0000dd90: 5f64 6963 7473 2c0a 2020 2020 2020 2020  _dicts,.        
-0000dda0: 2020 2020 2020 2020 726f 7773 3d72 6f77          rows=row
-0000ddb0: 735f 6469 6374 2c0a 2020 2020 2020 2020  s_dict,.        
-0000ddc0: 2020 2020 2020 2020 636f 6c75 6d6e 7342          columnsB
-0000ddd0: 7574 746f 6e3d 636f 6c75 6d6e 735f 6275  utton=columns_bu
-0000dde0: 7474 6f6e 2c0a 2020 2020 2020 2020 2020  tton,.          
-0000ddf0: 2020 2020 2020 6669 6c74 6572 7342 7574        filtersBut
-0000de00: 746f 6e3d 6669 6c74 6572 732c 0a20 2020  ton=filters,.   
-0000de10: 2020 2020 2020 2020 2020 2020 2065 7870               exp
-0000de20: 6f72 7442 7574 746f 6e3d 6578 706f 7274  ortButton=export
-0000de30: 5f74 6f5f 6373 762c 0a20 2020 2020 2020  _to_csv,.       
-0000de40: 2020 2020 2020 2020 2073 6561 7263 683d           search=
-0000de50: 7365 6172 6368 2c0a 2020 2020 2020 2020  search,.        
-0000de60: 2020 2020 2020 2020 7061 6769 6e61 7469          paginati
-0000de70: 6f6e 3d70 6167 696e 6174 696f 6e2c 0a20  on=pagination,. 
-0000de80: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000de90: 6f72 743d 736f 7274 2c0a 2020 2020 2020  ort=sort,.      
-0000dea0: 2020 2020 2020 292c 0a20 2020 2020 2020        ),.       
-0000deb0: 2029 0a0a 2020 2020 4061 6464 5f74 6f5f   )..    @add_to_
-0000dec0: 6765 6e65 7261 6c5f 6173 796e 635f 6772  general_async_gr
-0000ded0: 6f75 700a 2020 2020 6173 796e 6320 6465  oup.    async de
-0000dee0: 6620 696e 7075 745f 666f 726d 280a 2020  f input_form(.  
-0000def0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-0000df00: 2020 2020 6f70 7469 6f6e 733a 2064 6963      options: dic
-0000df10: 742c 0a20 2020 2020 2020 206f 7264 6572  t,.        order
-0000df20: 3a20 696e 742c 0a20 2020 2020 2020 2070  : int,.        p
-0000df30: 6164 6469 6e67 3a20 4f70 7469 6f6e 616c  adding: Optional
-0000df40: 5b73 7472 5d20 3d20 4e6f 6e65 2c0a 2020  [str] = None,.  
-0000df50: 2020 2020 2020 726f 7773 5f73 697a 653a        rows_size:
-0000df60: 204f 7074 696f 6e61 6c5b 696e 745d 203d   Optional[int] =
-0000df70: 204e 6f6e 652c 0a20 2020 2020 2020 2063   None,.        c
-0000df80: 6f6c 735f 7369 7a65 3a20 4f70 7469 6f6e  ols_size: Option
-0000df90: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 2c0a  al[int] = None,.
-0000dfa0: 2020 2020 2020 2020 6d6f 6461 6c3a 204f          modal: O
-0000dfb0: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
-0000dfc0: 6f6e 652c 0a20 2020 2020 2020 2061 6374  one,.        act
-0000dfd0: 6976 6974 795f 6964 3a20 4f70 7469 6f6e  ivity_id: Option
-0000dfe0: 616c 5b73 7472 5d20 3d20 4e6f 6e65 2c0a  al[str] = None,.
-0000dff0: 2020 2020 2020 2020 6163 7469 7669 7479          activity
-0000e000: 5f6e 616d 653a 204f 7074 696f 6e61 6c5b  _name: Optional[
-0000e010: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
-0000e020: 2020 2020 206f 6e5f 7375 626d 6974 5f65       on_submit_e
-0000e030: 7665 6e74 733a 204f 7074 696f 6e61 6c5b  vents: Optional[
-0000e040: 6c69 7374 5b64 6963 745d 5d20 3d20 4e6f  list[dict]] = No
-0000e050: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
-0000e060: 2020 2022 2222 4372 6561 7465 7320 616e     """Creates an
-0000e070: 2069 6e70 7574 2066 6f72 6d2e 0a20 2020   input form..   
-0000e080: 2020 2020 203a 7061 7261 6d20 6f70 7469       :param opti
-0000e090: 6f6e 733a 2074 6865 206f 7074 696f 6e73  ons: the options
-0000e0a0: 2066 6f72 2074 6865 2069 6e70 7574 2066   for the input f
-0000e0b0: 6f72 6d0a 2020 2020 2020 2020 3a70 6172  orm.        :par
-0000e0c0: 616d 206f 7264 6572 3a20 7468 6520 6f72  am order: the or
-0000e0d0: 6465 7220 6f66 2074 6865 2069 6e70 7574  der of the input
-0000e0e0: 2066 6f72 6d0a 2020 2020 2020 2020 3a70   form.        :p
-0000e0f0: 6172 616d 2070 6164 6469 6e67 3a20 7468  aram padding: th
-0000e100: 6520 7061 6464 696e 6720 6f66 2074 6865  e padding of the
-0000e110: 2069 6e70 7574 2066 6f72 6d0a 2020 2020   input form.    
-0000e120: 2020 2020 3a70 6172 616d 2072 6f77 735f      :param rows_
-0000e130: 7369 7a65 3a20 7468 6520 726f 7773 2073  size: the rows s
-0000e140: 697a 6520 6f66 2074 6865 2069 6e70 7574  ize of the input
-0000e150: 2066 6f72 6d0a 2020 2020 2020 2020 3a70   form.        :p
-0000e160: 6172 616d 2063 6f6c 735f 7369 7a65 3a20  aram cols_size: 
-0000e170: 7468 6520 636f 6c75 6d6e 7320 7369 7a65  the columns size
-0000e180: 206f 6620 7468 6520 696e 7075 7420 666f   of the input fo
-0000e190: 726d 0a20 2020 2020 2020 203a 7061 7261  rm.        :para
-0000e1a0: 6d20 6d6f 6461 6c3a 2074 6865 206d 6f64  m modal: the mod
-0000e1b0: 616c 2074 6f20 6f70 656e 2061 6674 6572  al to open after
-0000e1c0: 2073 7562 6d69 7474 696e 6720 7468 6520   submitting the 
-0000e1d0: 666f 726d 0a20 2020 2020 2020 203a 7061  form.        :pa
-0000e1e0: 7261 6d20 6163 7469 7669 7479 5f69 643a  ram activity_id:
-0000e1f0: 2074 6865 2061 6374 6976 6974 7920 6964   the activity id
-0000e200: 2074 6f20 7275 6e20 6166 7465 7220 7375   to run after su
-0000e210: 626d 6974 7469 6e67 2074 6865 2066 6f72  bmitting the for
-0000e220: 6d0a 2020 2020 2020 2020 3a70 6172 616d  m.        :param
-0000e230: 2061 6374 6976 6974 795f 6e61 6d65 3a20   activity_name: 
-0000e240: 7468 6520 6163 7469 7669 7479 206e 616d  the activity nam
-0000e250: 6520 746f 2072 756e 2061 6674 6572 2073  e to run after s
-0000e260: 7562 6d69 7474 696e 6720 7468 6520 666f  ubmitting the fo
-0000e270: 726d 0a20 2020 2020 2020 203a 7061 7261  rm.        :para
-0000e280: 6d20 6f6e 5f73 7562 6d69 745f 6576 656e  m on_submit_even
-0000e290: 7473 3a20 7468 6520 6576 656e 7473 2074  ts: the events t
-0000e2a0: 6f20 7275 6e20 6166 7465 7220 7375 626d  o run after subm
-0000e2b0: 6974 7469 6e67 2074 6865 2066 6f72 6d0a  itting the form.
-0000e2c0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000e2d0: 2020 2020 7661 6c69 6461 7465 5f69 6e70      validate_inp
-0000e2e0: 7574 5f66 6f72 6d5f 6461 7461 2873 656c  ut_form_data(sel
-0000e2f0: 662c 206f 7074 696f 6e73 290a 0a20 2020  f, options)..   
-0000e300: 2020 2020 2069 6620 6f6e 5f73 7562 6d69       if on_submi
-0000e310: 745f 6576 656e 7473 2069 7320 4e6f 6e65  t_events is None
-0000e320: 3a0a 2020 2020 2020 2020 2020 2020 6f6e  :.            on
-0000e330: 5f73 7562 6d69 745f 6576 656e 7473 203d  _submit_events =
-0000e340: 205b 5d0a 0a20 2020 2020 2020 2069 6620   []..        if 
-0000e350: 6d6f 6461 6c3a 0a20 2020 2020 2020 2020  modal:.         
-0000e360: 2020 206d 6f64 616c 5f69 6420 3d20 2861     modal_id = (a
-0000e370: 7761 6974 2073 656c 662e 5f67 6574 5f6d  wait self._get_m
-0000e380: 6f64 616c 286d 6f64 616c 2929 5b22 6964  odal(modal))["id
-0000e390: 225d 0a20 2020 2020 2020 2020 2020 206f  "].            o
-0000e3a0: 6e5f 7375 626d 6974 5f65 7665 6e74 732e  n_submit_events.
-0000e3b0: 6170 7065 6e64 280a 2020 2020 2020 2020  append(.        
-0000e3c0: 2020 2020 2020 2020 7b22 6163 7469 6f6e          {"action
-0000e3d0: 223a 2022 6f70 656e 4d6f 6461 6c22 2c20  ": "openModal", 
-0000e3e0: 2270 6172 616d 7322 3a20 7b22 6d6f 6461  "params": {"moda
-0000e3f0: 6c49 6422 3a20 6d6f 6461 6c5f 6964 7d7d  lId": modal_id}}
-0000e400: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
-0000e410: 2020 2020 2020 2020 6966 2061 6374 6976          if activ
-0000e420: 6974 795f 6964 206f 7220 6163 7469 7669  ity_id or activi
-0000e430: 7479 5f6e 616d 653a 0a20 2020 2020 2020  ty_name:.       
-0000e440: 2020 2020 2061 6374 6976 6974 795f 6964       activity_id
-0000e450: 203d 2028 6177 6169 7420 7365 6c66 2e5f   = (await self._
-0000e460: 6170 702e 6765 745f 6163 7469 7669 7479  app.get_activity
-0000e470: 2861 6374 6976 6974 795f 6964 2c20 6163  (activity_id, ac
-0000e480: 7469 7669 7479 5f6e 616d 6529 295b 0a20  tivity_name))[. 
-0000e490: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0000e4a0: 6964 220a 2020 2020 2020 2020 2020 2020  id".            
-0000e4b0: 5d0a 0a20 2020 2020 2020 2020 2020 206f  ]..            o
-0000e4c0: 6e5f 7375 626d 6974 5f65 7665 6e74 732e  n_submit_events.
-0000e4d0: 6170 7065 6e64 280a 2020 2020 2020 2020  append(.        
-0000e4e0: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
-0000e4f0: 2020 2020 2020 2020 2020 2020 2020 2261                "a
-0000e500: 6374 696f 6e22 3a20 2272 756e 4163 7469  ction": "runActi
-0000e510: 7669 7479 222c 0a20 2020 2020 2020 2020  vity",.         
-0000e520: 2020 2020 2020 2020 2020 2022 7061 7261             "para
-0000e530: 6d73 223a 207b 0a20 2020 2020 2020 2020  ms": {.         
-0000e540: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0000e550: 6163 7469 7669 7479 4964 223a 2061 6374  activityId": act
-0000e560: 6976 6974 795f 6964 2c0a 2020 2020 2020  ivity_id,.      
-0000e570: 2020 2020 2020 2020 2020 2020 2020 7d2c                },
-0000e580: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e590: 207d 0a20 2020 2020 2020 2020 2020 2029   }.            )
-0000e5a0: 0a0a 2020 2020 2020 2020 696e 6974 6961  ..        initia
-0000e5b0: 6c5f 6461 7461 3a20 6469 6374 203d 207b  l_data: dict = {
-0000e5c0: 7d0a 2020 2020 2020 2020 666f 7220 6669  }.        for fi
-0000e5d0: 656c 6473 2069 6e20 6f70 7469 6f6e 735b  elds in options[
-0000e5e0: 2266 6965 6c64 7322 5d3a 0a20 2020 2020  "fields"]:.     
-0000e5f0: 2020 2020 2020 2066 6f72 2066 6965 6c64         for field
-0000e600: 2069 6e20 6669 656c 6473 5b22 6669 656c   in fields["fiel
-0000e610: 6473 225d 3a0a 2020 2020 2020 2020 2020  ds"]:.          
-0000e620: 2020 2020 2020 6669 656c 645f 6e61 6d65        field_name
-0000e630: 3a20 7374 7220 3d20 6669 656c 645b 2266  : str = field["f
-0000e640: 6965 6c64 4e61 6d65 225d 0a20 2020 2020  ieldName"].     
-0000e650: 2020 2020 2020 2020 2020 2069 6e70 7574             input
-0000e660: 5f74 7970 653a 204f 7074 696f 6e61 6c5b  _type: Optional[
-0000e670: 7374 725d 203d 2066 6965 6c64 2e67 6574  str] = field.get
-0000e680: 2822 696e 7075 7454 7970 6522 290a 2020  ("inputType").  
-0000e690: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0000e6a0: 2069 6e70 7574 5f74 7970 6520 3d3d 2022   input_type == "
-0000e6b0: 636f 6c6f 7222 3a0a 2020 2020 2020 2020  color":.        
-0000e6c0: 2020 2020 2020 2020 2020 2020 696e 6974              init
-0000e6d0: 6961 6c5f 6461 7461 5b66 6965 6c64 5f6e  ial_data[field_n
-0000e6e0: 616d 655d 203d 2022 2330 3030 3030 3022  ame] = "#000000"
-0000e6f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e700: 2065 6c69 6620 696e 7075 745f 7479 7065   elif input_type
-0000e710: 203d 3d20 226e 756d 6265 7222 3a0a 2020   == "number":.  
-0000e720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e730: 2020 696e 6974 6961 6c5f 6461 7461 5b66    initial_data[f
-0000e740: 6965 6c64 5f6e 616d 655d 203d 2030 0a20  ield_name] = 0. 
-0000e750: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-0000e760: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0000e770: 2020 2020 2020 2020 2069 6e69 7469 616c           initial
-0000e780: 5f64 6174 615b 6669 656c 645f 6e61 6d65  _data[field_name
-0000e790: 5d20 3d20 2222 0a0a 2020 2020 2020 2020  ] = ""..        
-0000e7a0: 725f 6861 7368 2c20 7265 706f 7274 203d  r_hash, report =
-0000e7b0: 2061 7761 6974 2073 656c 662e 5f67 6574   await self._get
-0000e7c0: 5f63 6861 7274 5f72 6570 6f72 7428 6f72  _chart_report(or
-0000e7d0: 6465 722c 2049 6e70 7574 466f 726d 290a  der, InputForm).
-0000e7e0: 2020 2020 2020 2020 5f2c 2064 6174 615f          _, data_
-0000e7f0: 7365 742c 205f 203d 206c 6973 7428 0a20  set, _ = list(. 
-0000e800: 2020 2020 2020 2020 2020 2028 0a20 2020             (.   
-0000e810: 2020 2020 2020 2020 2020 2020 2061 7761               awa
-0000e820: 6974 2073 656c 662e 5f63 7265 6174 655f  it self._create_
-0000e830: 6461 7461 5f73 6574 2872 6570 6f72 745b  data_set(report[
-0000e840: 2269 6422 5d2c 2069 6e69 7469 616c 5f64  "id"], initial_d
-0000e850: 6174 612c 2064 756d 705f 7768 6f6c 653d  ata, dump_whole=
-0000e860: 5472 7565 290a 2020 2020 2020 2020 2020  True).          
-0000e870: 2020 292e 7661 6c75 6573 2829 0a20 2020    ).values().   
-0000e880: 2020 2020 2029 5b30 5d0a 0a20 2020 2020       )[0]..     
-0000e890: 2020 2072 6473 203d 2061 7761 6974 2072     rds = await r
-0000e8a0: 6570 6f72 742e 6765 745f 7265 706f 7274  eport.get_report
-0000e8b0: 5f64 6174 615f 7365 7473 2829 0a20 2020  _data_sets().   
-0000e8c0: 2020 2020 2069 6620 6c65 6e28 7264 7329       if len(rds)
-0000e8d0: 203e 2031 3a0a 2020 2020 2020 2020 2020   > 1:.          
-0000e8e0: 2020 6c6f 675f 6572 726f 7228 0a20 2020    log_error(.   
-0000e8f0: 2020 2020 2020 2020 2020 2020 206c 6f67               log
-0000e900: 6765 722c 0a20 2020 2020 2020 2020 2020  ger,.           
-0000e910: 2020 2020 2022 496e 7075 7420 666f 726d       "Input form
-0000e920: 2063 616e 206f 6e6c 7920 6861 7665 206f   can only have o
-0000e930: 6e65 2063 6f6d 706f 6e65 6e74 2064 6174  ne component dat
-0000e940: 6120 7365 7420 6c69 6e6b 2c20 220a 2020  a set link, ".  
-0000e950: 2020 2020 2020 2020 2020 2020 2020 2274                "t
-0000e960: 6869 7320 6973 2061 6e20 5344 4b20 6275  his is an SDK bu
-0000e970: 6720 706c 6561 7365 2072 6570 6f72 7420  g please report 
-0000e980: 6974 2061 6e64 2022 0a20 2020 2020 2020  it and ".       
-0000e990: 2020 2020 2020 2020 2022 6465 6c65 7465           "delete
-0000e9a0: 2074 6865 2066 6f72 6d20 746f 2073 6f6c   the form to sol
-0000e9b0: 7665 2074 6865 2069 7373 7565 222c 0a20  ve the issue",. 
-0000e9c0: 2020 2020 2020 2020 2020 2020 2020 2044                 D
-0000e9d0: 6174 6145 7272 6f72 2c0a 2020 2020 2020  ataError,.      
-0000e9e0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-0000e9f0: 2069 6620 7264 7320 616e 6420 280a 2020   if rds and (.  
-0000ea00: 2020 2020 2020 2020 2020 6e6f 7420 7365            not se
-0000ea10: 6c66 2e72 6575 7365 5f64 6174 615f 7365  lf.reuse_data_se
-0000ea20: 7473 0a20 2020 2020 2020 2020 2020 206f  ts.            o
-0000ea30: 7220 7264 735b 305d 5b22 6461 7461 5365  r rds[0]["dataSe
-0000ea40: 7449 6422 5d20 213d 2064 6174 615f 7365  tId"] != data_se
-0000ea50: 745b 2269 6422 5d0a 2020 2020 2020 2020  t["id"].        
-0000ea60: 2020 2020 6f72 2072 6473 5b30 5d5b 2270      or rds[0]["p
-0000ea70: 726f 7065 7274 6965 7322 5d5b 2266 6965  roperties"]["fie
-0000ea80: 6c64 7322 5d20 213d 206f 7074 696f 6e73  lds"] != options
-0000ea90: 5b22 6669 656c 6473 225d 0a20 2020 2020  ["fields"].     
-0000eaa0: 2020 2029 3a0a 2020 2020 2020 2020 2020     ):.          
-0000eab0: 2020 6177 6169 7420 7265 706f 7274 2e64    await report.d
-0000eac0: 656c 6574 655f 7265 706f 7274 5f64 6174  elete_report_dat
-0000ead0: 615f 7365 7473 286c 6f67 3d54 7275 6529  a_sets(log=True)
-0000eae0: 0a20 2020 2020 2020 2020 2020 2072 6473  .            rds
-0000eaf0: 203d 205b 5d0a 0a20 2020 2020 2020 2069   = []..        i
-0000eb00: 6620 6e6f 7420 7264 733a 0a20 2020 2020  f not rds:.     
-0000eb10: 2020 2020 2020 2061 7761 6974 2072 6570         await rep
-0000eb20: 6f72 742e 6372 6561 7465 5f72 6570 6f72  ort.create_repor
-0000eb30: 745f 6461 7461 5f73 6574 280a 2020 2020  t_data_set(.    
-0000eb40: 2020 2020 2020 2020 2020 2020 2822 6375              ("cu
-0000eb50: 7374 6f6d 4669 656c 6431 222c 2064 6174  stomField1", dat
-0000eb60: 615f 7365 742c 204e 6f6e 6529 2c20 7072  a_set, None), pr
-0000eb70: 6f70 6572 7469 6573 3d6f 7074 696f 6e73  operties=options
-0000eb80: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-0000eb90: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
-0000eba0: 722e 696e 666f 2866 2243 7265 6174 6564  r.info(f"Created
-0000ebb0: 2031 2063 6f6d 706f 6e65 6e74 2064 6174   1 component dat
-0000ebc0: 6120 7365 7420 6c69 6e6b 2066 6f72 2069  a set link for i
-0000ebd0: 6e70 7574 2066 6f72 6d20 6174 207b 725f  nput form at {r_
-0000ebe0: 6861 7368 7d22 290a 0a20 2020 2020 2020  hash}")..       
-0000ebf0: 2061 7761 6974 2073 656c 662e 5f63 7265   await self._cre
-0000ec00: 6174 655f 6368 6172 7428 0a20 2020 2020  ate_chart(.     
-0000ec10: 2020 2020 2020 2063 6861 7274 5f63 6c61         chart_cla
-0000ec20: 7373 3d49 6e70 7574 466f 726d 2c0a 2020  ss=InputForm,.  
-0000ec30: 2020 2020 2020 2020 2020 6f72 6465 723d            order=
-0000ec40: 6f72 6465 722c 0a20 2020 2020 2020 2020  order,.         
-0000ec50: 2020 2073 697a 6550 6164 6469 6e67 3d70     sizePadding=p
-0000ec60: 6164 6469 6e67 2c0a 2020 2020 2020 2020  adding,.        
-0000ec70: 2020 2020 7369 7a65 526f 7773 3d72 6f77      sizeRows=row
-0000ec80: 735f 7369 7a65 2c0a 2020 2020 2020 2020  s_size,.        
-0000ec90: 2020 2020 7369 7a65 436f 6c75 6d6e 733d      sizeColumns=
-0000eca0: 636f 6c73 5f73 697a 652c 0a20 2020 2020  cols_size,.     
-0000ecb0: 2020 2020 2020 2070 726f 7065 7274 6965         propertie
-0000ecc0: 733d 7b22 6576 656e 7473 223a 207b 226f  s={"events": {"o
-0000ecd0: 6e53 7562 6d69 7422 3a20 6f6e 5f73 7562  nSubmit": on_sub
-0000ece0: 6d69 745f 6576 656e 7473 7d7d 2c0a 2020  mit_events}},.  
-0000ecf0: 2020 2020 2020 290a 0a20 2020 2064 6566        )..    def
-0000ed00: 2067 656e 6572 6174 655f 696e 7075 745f   generate_input_
-0000ed10: 666f 726d 5f67 726f 7570 7328 0a20 2020  form_groups(.   
-0000ed20: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-0000ed30: 2020 206f 7264 6572 3a20 696e 742c 0a20     order: int,. 
-0000ed40: 2020 2020 2020 2066 6f72 6d5f 6772 6f75         form_grou
-0000ed50: 7073 3a20 6469 6374 2c0a 2020 2020 2020  ps: dict,.      
-0000ed60: 2020 6479 6e61 6d69 635f 7365 7175 656e    dynamic_sequen
-0000ed70: 7469 616c 5f73 686f 773a 204f 7074 696f  tial_show: Optio
-0000ed80: 6e61 6c5b 626f 6f6c 5d20 3d20 4661 6c73  nal[bool] = Fals
-0000ed90: 652c 0a20 2020 2020 2020 2061 7574 6f5f  e,.        auto_
-0000eda0: 7365 6e64 3a20 4f70 7469 6f6e 616c 5b62  send: Optional[b
-0000edb0: 6f6f 6c5d 203d 2046 616c 7365 2c0a 2020  ool] = False,.  
-0000edc0: 2020 2020 2020 6e65 7874 5f67 726f 7570        next_group
-0000edd0: 5f6c 6162 656c 3a20 4f70 7469 6f6e 616c  _label: Optional
-0000ede0: 5b73 7472 5d20 3d20 224e 6578 7422 2c0a  [str] = "Next",.
-0000edf0: 2020 2020 2020 2020 726f 7773 5f73 697a          rows_siz
-0000ee00: 653a 204f 7074 696f 6e61 6c5b 696e 745d  e: Optional[int]
-0000ee10: 203d 2033 2c0a 2020 2020 2020 2020 636f   = 3,.        co
-0000ee20: 6c73 5f73 697a 653a 2069 6e74 203d 2031  ls_size: int = 1
-0000ee30: 322c 0a20 2020 2020 2020 2070 6164 6469  2,.        paddi
-0000ee40: 6e67 3a20 4f70 7469 6f6e 616c 5b73 7472  ng: Optional[str
-0000ee50: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-0000ee60: 2020 6d6f 6461 6c3a 204f 7074 696f 6e61    modal: Optiona
-0000ee70: 6c5b 7374 725d 203d 204e 6f6e 652c 0a20  l[str] = None,. 
-0000ee80: 2020 2020 2020 2061 6374 6976 6974 795f         activity_
-0000ee90: 6964 3a20 4f70 7469 6f6e 616c 5b73 7472  id: Optional[str
-0000eea0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-0000eeb0: 2020 6163 7469 7669 7479 5f6e 616d 653a    activity_name:
-0000eec0: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
-0000eed0: 204e 6f6e 652c 0a20 2020 2020 2020 206f   None,.        o
-0000eee0: 6e5f 7375 626d 6974 5f65 7665 6e74 733a  n_submit_events:
-0000eef0: 204f 7074 696f 6e61 6c5b 6c69 7374 5b64   Optional[list[d
-0000ef00: 6963 745d 5d20 3d20 4e6f 6e65 2c0a 2020  ict]] = None,.  
-0000ef10: 2020 293a 0a20 2020 2020 2020 2022 2222    ):.        """
-0000ef20: 4561 7369 6572 2077 6179 2074 6f20 6372  Easier way to cr
-0000ef30: 6561 7465 2061 6e20 696e 7075 7420 666f  eate an input fo
-0000ef40: 726d 2e0a 2020 2020 2020 2020 3a70 6172  rm..        :par
-0000ef50: 616d 206d 656e 755f 7061 7468 3a20 7468  am menu_path: th
-0000ef60: 6520 6d65 6e75 2070 6174 6820 6f66 2074  e menu path of t
-0000ef70: 6865 2069 6e70 7574 2066 6f72 6d0a 2020  he input form.  
-0000ef80: 2020 2020 2020 3a70 6172 616d 206f 7264        :param ord
-0000ef90: 6572 3a20 7468 6520 6f72 6465 7220 6f66  er: the order of
-0000efa0: 2074 6865 2069 6e70 7574 2066 6f72 6d0a   the input form.
-0000efb0: 2020 2020 2020 2020 3a70 6172 616d 2066          :param f
-0000efc0: 6f72 6d5f 6772 6f75 7073 3a20 7468 6520  orm_groups: the 
-0000efd0: 666f 726d 2067 726f 7570 7320 6f66 2074  form groups of t
-0000efe0: 6865 2069 6e70 7574 2066 6f72 6d0a 2020  he input form.  
-0000eff0: 2020 2020 2020 3a70 6172 616d 2064 796e        :param dyn
-0000f000: 616d 6963 5f73 6571 7565 6e74 6961 6c5f  amic_sequential_
-0000f010: 7368 6f77 3a20 7768 6574 6865 7220 746f  show: whether to
-0000f020: 2073 686f 7720 7468 6520 6e65 7874 2067   show the next g
-0000f030: 726f 7570 2061 6674 6572 2073 7562 6d69  roup after submi
-0000f040: 7474 696e 6720 7468 6520 6375 7272 656e  tting the curren
-0000f050: 7420 6772 6f75 700a 2020 2020 2020 2020  t group.        
-0000f060: 3a70 6172 616d 2061 7574 6f5f 7365 6e64  :param auto_send
-0000f070: 3a20 7768 6574 6865 7220 746f 2061 7574  : whether to aut
-0000f080: 6f6d 6174 6963 616c 6c79 2073 656e 6420  omatically send 
-0000f090: 7468 6520 666f 726d 2061 6674 6572 2074  the form after t
-0000f0a0: 6865 206c 6173 7420 6772 6f75 700a 2020  he last group.  
-0000f0b0: 2020 2020 2020 3a70 6172 616d 206e 6578        :param nex
-0000f0c0: 745f 6772 6f75 705f 6c61 6265 6c3a 2074  t_group_label: t
-0000f0d0: 6865 206c 6162 656c 206f 6620 7468 6520  he label of the 
-0000f0e0: 6e65 7874 2067 726f 7570 2062 7574 746f  next group butto
-0000f0f0: 6e0a 2020 2020 2020 2020 3a70 6172 616d  n.        :param
-0000f100: 2072 6f77 735f 7369 7a65 3a20 7468 6520   rows_size: the 
-0000f110: 726f 7773 2073 697a 6520 6f66 2074 6865  rows size of the
-0000f120: 2069 6e70 7574 2066 6f72 6d0a 2020 2020   input form.    
-0000f130: 2020 2020 3a70 6172 616d 2063 6f6c 735f      :param cols_
-0000f140: 7369 7a65 3a20 7468 6520 636f 6c75 6d6e  size: the column
-0000f150: 7320 7369 7a65 206f 6620 7468 6520 696e  s size of the in
-0000f160: 7075 7420 666f 726d 0a20 2020 2020 2020  put form.       
-0000f170: 203a 7061 7261 6d20 7061 6464 696e 673a   :param padding:
-0000f180: 2074 6865 2070 6164 6469 6e67 206f 6620   the padding of 
-0000f190: 7468 6520 696e 7075 7420 666f 726d 0a20  the input form. 
-0000f1a0: 2020 2020 2020 203a 7061 7261 6d20 6d6f         :param mo
-0000f1b0: 6461 6c3a 2074 6865 206d 6f64 616c 2074  dal: the modal t
-0000f1c0: 6f20 6f70 656e 2061 6674 6572 2073 7562  o open after sub
-0000f1d0: 6d69 7474 696e 6720 7468 6520 666f 726d  mitting the form
-0000f1e0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-0000f1f0: 6163 7469 7669 7479 5f69 643a 2074 6865  activity_id: the
-0000f200: 2061 6374 6976 6974 7920 6964 2074 6f20   activity id to 
-0000f210: 7275 6e20 6166 7465 7220 7375 626d 6974  run after submit
-0000f220: 7469 6e67 2074 6865 2066 6f72 6d0a 2020  ting the form.  
-0000f230: 2020 2020 2020 3a70 6172 616d 2061 6374        :param act
-0000f240: 6976 6974 795f 6e61 6d65 3a20 7468 6520  ivity_name: the 
-0000f250: 6163 7469 7669 7479 206e 616d 6520 746f  activity name to
-0000f260: 2072 756e 2061 6674 6572 2073 7562 6d69   run after submi
-0000f270: 7474 696e 6720 7468 6520 666f 726d 0a20  tting the form. 
-0000f280: 2020 2020 2020 203a 7061 7261 6d20 6f6e         :param on
-0000f290: 5f73 7562 6d69 745f 6576 656e 7473 3a20  _submit_events: 
-0000f2a0: 7468 6520 6576 656e 7473 2074 6f20 7275  the events to ru
-0000f2b0: 6e20 6166 7465 7220 7375 626d 6974 7469  n after submitti
-0000f2c0: 6e67 2074 6865 2066 6f72 6d0a 2020 2020  ng the form.    
-0000f2d0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0000f2e0: 7265 706f 7274 5f64 6174 615f 7365 745f  report_data_set_
-0000f2f0: 7072 6f70 6572 7469 6573 203d 207b 2266  properties = {"f
-0000f300: 6965 6c64 7322 3a20 5b5d 7d0a 2020 2020  ields": []}.    
-0000f310: 2020 2020 6966 2061 7574 6f5f 7365 6e64      if auto_send
-0000f320: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0000f330: 706f 7274 5f64 6174 615f 7365 745f 7072  port_data_set_pr
-0000f340: 6f70 6572 7469 6573 5b22 7661 7269 616e  operties["varian
-0000f350: 7422 5d20 3d20 2261 7574 6f53 656e 6422  t"] = "autoSend"
-0000f360: 0a0a 2020 2020 2020 2020 725f 6861 7368  ..        r_hash
-0000f370: 203d 2073 656c 662e 5f67 6574 5f63 6861   = self._get_cha
-0000f380: 7274 5f68 6173 6828 6f72 6465 7229 0a0a  rt_hash(order)..
-0000f390: 2020 2020 2020 2020 6e65 7874 5f69 6420          next_id 
-0000f3a0: 3d20 6622 7b72 5f68 6173 687d 5f30 2220  = f"{r_hash}_0" 
-0000f3b0: 6966 2064 796e 616d 6963 5f73 6571 7565  if dynamic_seque
-0000f3c0: 6e74 6961 6c5f 7368 6f77 2065 6c73 6520  ntial_show else 
-0000f3d0: 4e6f 6e65 0a0a 2020 2020 2020 2020 6e65  None..        ne
-0000f3e0: 7874 5f67 726f 7570 5f69 6e64 6578 203d  xt_group_index =
-0000f3f0: 2031 0a20 2020 2020 2020 2066 6f72 2066   1.        for f
-0000f400: 6f72 6d5f 6772 6f75 705f 6e61 6d65 2c20  orm_group_name, 
-0000f410: 666f 726d 5f67 726f 7570 2069 6e20 666f  form_group in fo
-0000f420: 726d 5f67 726f 7570 732e 6974 656d 7328  rm_groups.items(
-0000f430: 293a 0a20 2020 2020 2020 2020 2020 2066  ):.            f
-0000f440: 6f72 6d5f 6772 6f75 705f 6a73 6f6e 203d  orm_group_json =
-0000f450: 207b 2274 6974 6c65 223a 2066 6f72 6d5f   {"title": form_
-0000f460: 6772 6f75 705f 6e61 6d65 2c20 2266 6965  group_name, "fie
-0000f470: 6c64 7322 3a20 666f 726d 5f67 726f 7570  lds": form_group
-0000f480: 7d0a 2020 2020 2020 2020 2020 2020 6966  }.            if
-0000f490: 206e 6578 745f 6964 3a0a 2020 2020 2020   next_id:.      
-0000f4a0: 2020 2020 2020 2020 2020 666f 726d 5f67            form_g
-0000f4b0: 726f 7570 5f6a 736f 6e5b 2269 6422 5d20  roup_json["id"] 
-0000f4c0: 3d20 6e65 7874 5f69 640a 2020 2020 2020  = next_id.      
-0000f4d0: 2020 2020 2020 2020 2020 6e65 7874 5f69            next_i
-0000f4e0: 6420 3d20 6622 7b72 5f68 6173 687d 5f7b  d = f"{r_hash}_{
-0000f4f0: 6e65 7874 5f67 726f 7570 5f69 6e64 6578  next_group_index
-0000f500: 7d22 0a20 2020 2020 2020 2020 2020 2020  }".             
-0000f510: 2020 2066 6f72 6d5f 6772 6f75 705f 6a73     form_group_js
-0000f520: 6f6e 5b22 6e65 7874 466f 726d 4772 6f75  on["nextFormGrou
-0000f530: 7022 5d20 3d20 7b0a 2020 2020 2020 2020  p"] = {.        
-0000f540: 2020 2020 2020 2020 2020 2020 2269 6422              "id"
-0000f550: 3a20 6e65 7874 5f69 642c 0a20 2020 2020  : next_id,.     
-0000f560: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0000f570: 6c61 6265 6c22 3a20 6e65 7874 5f67 726f  label": next_gro
-0000f580: 7570 5f6c 6162 656c 2c0a 2020 2020 2020  up_label,.      
-0000f590: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
-0000f5a0: 2020 2020 2020 2020 2020 2020 6e65 7874              next
-0000f5b0: 5f67 726f 7570 5f69 6e64 6578 202b 3d20  _group_index += 
-0000f5c0: 310a 2020 2020 2020 2020 2020 2020 7265  1.            re
-0000f5d0: 706f 7274 5f64 6174 615f 7365 745f 7072  port_data_set_pr
-0000f5e0: 6f70 6572 7469 6573 5b22 6669 656c 6473  operties["fields
-0000f5f0: 225d 202b 3d20 5b66 6f72 6d5f 6772 6f75  "] += [form_grou
-0000f600: 705f 6a73 6f6e 5d0a 0a20 2020 2020 2020  p_json]..       
-0000f610: 2069 6620 6e65 7874 5f69 643a 0a20 2020   if next_id:.   
-0000f620: 2020 2020 2020 2020 2064 656c 2072 6570           del rep
-0000f630: 6f72 745f 6461 7461 5f73 6574 5f70 726f  ort_data_set_pro
-0000f640: 7065 7274 6965 735b 2266 6965 6c64 7322  perties["fields"
-0000f650: 5d5b 2d31 5d5b 226e 6578 7446 6f72 6d47  ][-1]["nextFormG
-0000f660: 726f 7570 225d 0a0a 2020 2020 2020 2020  roup"]..        
-0000f670: 7365 6c66 2e69 6e70 7574 5f66 6f72 6d28  self.input_form(
-0000f680: 0a20 2020 2020 2020 2020 2020 206f 7074  .            opt
-0000f690: 696f 6e73 3d72 6570 6f72 745f 6461 7461  ions=report_data
-0000f6a0: 5f73 6574 5f70 726f 7065 7274 6965 732c  _set_properties,
-0000f6b0: 0a20 2020 2020 2020 2020 2020 206f 7264  .            ord
-0000f6c0: 6572 3d6f 7264 6572 2c0a 2020 2020 2020  er=order,.      
-0000f6d0: 2020 2020 2020 726f 7773 5f73 697a 653d        rows_size=
-0000f6e0: 726f 7773 5f73 697a 652c 0a20 2020 2020  rows_size,.     
-0000f6f0: 2020 2020 2020 2063 6f6c 735f 7369 7a65         cols_size
-0000f700: 3d63 6f6c 735f 7369 7a65 2c0a 2020 2020  =cols_size,.    
-0000f710: 2020 2020 2020 2020 7061 6464 696e 673d          padding=
-0000f720: 7061 6464 696e 672c 0a20 2020 2020 2020  padding,.       
-0000f730: 2020 2020 206d 6f64 616c 3d6d 6f64 616c       modal=modal
-0000f740: 2c0a 2020 2020 2020 2020 2020 2020 6163  ,.            ac
-0000f750: 7469 7669 7479 5f69 643d 6163 7469 7669  tivity_id=activi
-0000f760: 7479 5f69 642c 0a20 2020 2020 2020 2020  ty_id,.         
-0000f770: 2020 2061 6374 6976 6974 795f 6e61 6d65     activity_name
-0000f780: 3d61 6374 6976 6974 795f 6e61 6d65 2c0a  =activity_name,.
-0000f790: 2020 2020 2020 2020 2020 2020 6f6e 5f73              on_s
-0000f7a0: 7562 6d69 745f 6576 656e 7473 3d6f 6e5f  ubmit_events=on_
-0000f7b0: 7375 626d 6974 5f65 7665 6e74 732c 0a20  submit_events,. 
-0000f7c0: 2020 2020 2020 2029 0a0a 2020 2020 6173         )..    as
-0000f7d0: 796e 6320 6465 6620 5f67 6574 5f69 6e70  ync def _get_inp
-0000f7e0: 7574 5f66 6f72 6d5f 6461 7461 2873 656c  ut_form_data(sel
-0000f7f0: 662c 2069 6e70 7574 5f66 6f72 6d3a 2049  f, input_form: I
-0000f800: 6e70 7574 466f 726d 2920 2d3e 2064 6963  nputForm) -> dic
-0000f810: 743a 0a20 2020 2020 2020 2022 2222 4765  t:.        """Ge
-0000f820: 7420 7468 6520 696e 7075 7420 666f 726d  t the input form
-0000f830: 2064 6174 612e 2222 220a 2020 2020 2020   data.""".      
-0000f840: 2020 7265 706f 7274 5f64 6174 615f 7365    report_data_se
-0000f850: 7420 3d20 2861 7761 6974 2069 6e70 7574  t = (await input
-0000f860: 5f66 6f72 6d2e 6765 745f 7265 706f 7274  _form.get_report
-0000f870: 5f64 6174 615f 7365 7473 2829 295b 305d  _data_sets())[0]
-0000f880: 0a20 2020 2020 2020 2064 6174 615f 7365  .        data_se
-0000f890: 7420 3d20 6177 6169 7420 7365 6c66 2e5f  t = await self._
-0000f8a0: 6170 702e 6765 745f 6461 7461 5f73 6574  app.get_data_set
-0000f8b0: 2872 6570 6f72 745f 6461 7461 5f73 6574  (report_data_set
-0000f8c0: 5b22 6461 7461 5365 7449 6422 5d29 0a20  ["dataSetId"]). 
-0000f8d0: 2020 2020 2020 2064 6174 615f 706f 696e         data_poin
-0000f8e0: 7420 3d20 6177 6169 7420 6461 7461 5f73  t = await data_s
-0000f8f0: 6574 2e67 6574 5f6f 6e65 5f64 6174 615f  et.get_one_data_
-0000f900: 706f 696e 7428 290a 2020 2020 2020 2020  point().        
-0000f910: 6c6f 6767 6572 2e69 6e66 6f28 6622 476f  logger.info(f"Go
-0000f920: 7420 696e 7075 7420 666f 726d 2064 6174  t input form dat
-0000f930: 6120 666f 7220 7b73 7472 2869 6e70 7574  a for {str(input
-0000f940: 5f66 6f72 6d29 7d22 290a 2020 2020 2020  _form)}").      
-0000f950: 2020 7265 7475 726e 207b 0a20 2020 2020    return {.     
-0000f960: 2020 2020 2020 2022 7265 706f 7274 4964         "reportId
-0000f970: 223a 2069 6e70 7574 5f66 6f72 6d5b 2269  ": input_form["i
-0000f980: 6422 5d2c 0a20 2020 2020 2020 2020 2020  d"],.           
-0000f990: 2022 6f72 6465 7222 3a20 696e 7075 745f   "order": input_
-0000f9a0: 666f 726d 5b22 6f72 6465 7222 5d2c 0a20  form["order"],. 
-0000f9b0: 2020 2020 2020 2020 2020 2022 6461 7461             "data
-0000f9c0: 223a 2064 6174 615f 706f 696e 745b 2263  ": data_point["c
-0000f9d0: 7573 746f 6d46 6965 6c64 3122 5d20 6966  ustomField1"] if
-0000f9e0: 2064 6174 615f 706f 696e 7420 656c 7365   data_point else
-0000f9f0: 204e 6f6e 652c 0a20 2020 2020 2020 207d   None,.        }
-0000fa00: 0a0a 2020 2020 6173 796e 6320 6465 6620  ..    async def 
-0000fa10: 6765 745f 696e 7075 745f 666f 726d 7328  get_input_forms(
-0000fa20: 7365 6c66 2920 2d3e 206c 6973 745b 6469  self) -> list[di
-0000fa30: 6374 5d3a 0a20 2020 2020 2020 2022 2222  ct]:.        """
-0000fa40: 4765 7420 616c 6c20 7468 6520 696e 7075  Get all the inpu
-0000fa50: 7420 666f 726d 7320 696e 2074 6865 2063  t forms in the c
-0000fa60: 7572 7265 6e74 206d 656e 755f 7061 7468  urrent menu_path
-0000fa70: 2e22 2222 0a20 2020 2020 2020 2072 6570  .""".        rep
-0000fa80: 6f72 7473 3a20 6c69 7374 203d 205b 0a20  orts: list = [. 
-0000fa90: 2020 2020 2020 2020 2020 2072 6570 6f72             repor
-0000faa0: 740a 2020 2020 2020 2020 2020 2020 666f  t.            fo
-0000fab0: 7220 7265 706f 7274 2069 6e20 6177 6169  r report in awai
-0000fac0: 7420 7365 6c66 2e5f 6170 702e 6765 745f  t self._app.get_
-0000fad0: 7265 706f 7274 7328 290a 2020 2020 2020  reports().      
-0000fae0: 2020 2020 2020 6966 2072 6570 6f72 745b        if report[
-0000faf0: 2272 6570 6f72 7454 7970 6522 5d20 3d3d  "reportType"] ==
-0000fb00: 2022 464f 524d 220a 2020 2020 2020 2020   "FORM".        
-0000fb10: 2020 2020 616e 6420 2872 6570 6f72 745b      and (report[
-0000fb20: 2270 6174 6822 5d20 3d3d 2073 656c 662e  "path"] == self.
-0000fb30: 5f63 7572 7265 6e74 5f70 6174 6820 6f72  _current_path or
-0000fb40: 206e 6f74 2073 656c 662e 5f63 7572 7265   not self._curre
-0000fb50: 6e74 5f70 6174 6829 0a20 2020 2020 2020  nt_path).       
-0000fb60: 205d 0a20 2020 2020 2020 2072 6574 7572   ].        retur
-0000fb70: 6e20 6c69 7374 280a 2020 2020 2020 2020  n list(.        
-0000fb80: 2020 2020 6177 6169 7420 6173 796e 6369      await asynci
-0000fb90: 6f2e 6761 7468 6572 280a 2020 2020 2020  o.gather(.      
-0000fba0: 2020 2020 2020 2020 2020 2a5b 7365 6c66            *[self
-0000fbb0: 2e5f 6765 745f 696e 7075 745f 666f 726d  ._get_input_form
-0000fbc0: 5f64 6174 6128 7265 706f 7274 2920 666f  _data(report) fo
-0000fbd0: 7220 7265 706f 7274 2069 6e20 7265 706f  r report in repo
-0000fbe0: 7274 735d 0a20 2020 2020 2020 2020 2020  rts].           
-0000fbf0: 2029 0a20 2020 2020 2020 2029 0a0a 2020   ).        )..  
-0000fc00: 2020 4061 6464 5f74 6f5f 6765 6e65 7261    @add_to_genera
-0000fc10: 6c5f 6173 796e 635f 6772 6f75 700a 2020  l_async_group.  
-0000fc20: 2020 6173 796e 6320 6465 6620 616e 6e6f    async def anno
-0000fc30: 7461 7465 645f 6368 6172 7428 0a20 2020  tated_chart(.   
-0000fc40: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-0000fc50: 2020 2064 6174 613a 2055 6e69 6f6e 5b6c     data: Union[l
-0000fc60: 6973 745b 4461 7461 4672 616d 655d 2c20  ist[DataFrame], 
-0000fc70: 6c69 7374 5b6c 6973 745b 6469 6374 5d5d  list[list[dict]]
-0000fc80: 5d2c 0a20 2020 2020 2020 206f 7264 6572  ],.        order
-0000fc90: 3a20 696e 742c 0a20 2020 2020 2020 2078  : int,.        x
-0000fca0: 3a20 7374 722c 0a20 2020 2020 2020 2079  : str,.        y
-0000fcb0: 3a20 556e 696f 6e5b 7374 722c 206c 6973  : Union[str, lis
-0000fcc0: 745b 7374 725d 5d2c 0a20 2020 2020 2020  t[str]],.       
-0000fcd0: 2061 6e6e 6f74 6174 696f 6e73 3a20 7374   annotations: st
-0000fce0: 7220 3d20 2261 6e6e 6f74 6174 696f 6e22  r = "annotation"
-0000fcf0: 2c0a 2020 2020 2020 2020 726f 7773 5f73  ,.        rows_s
-0000fd00: 697a 653a 204f 7074 696f 6e61 6c5b 696e  ize: Optional[in
-0000fd10: 745d 203d 204e 6f6e 652c 0a20 2020 2020  t] = None,.     
-0000fd20: 2020 2063 6f6c 735f 7369 7a65 3a20 4f70     cols_size: Op
-0000fd30: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
-0000fd40: 6e65 2c0a 2020 2020 2020 2020 7061 6464  ne,.        padd
-0000fd50: 696e 673a 204f 7074 696f 6e61 6c5b 7374  ing: Optional[st
-0000fd60: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
-0000fd70: 2020 2074 6974 6c65 3a20 4f70 7469 6f6e     title: Option
-0000fd80: 616c 5b73 7472 5d20 3d20 4e6f 6e65 2c0a  al[str] = None,.
-0000fd90: 2020 2020 2020 2020 795f 6178 6973 5f6e          y_axis_n
-0000fda0: 616d 653a 204f 7074 696f 6e61 6c5b 7374  ame: Optional[st
-0000fdb0: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
-0000fdc0: 2020 2073 6c69 6465 725f 636f 6e66 6967     slider_config
-0000fdd0: 3a20 4f70 7469 6f6e 616c 5b64 6963 745d  : Optional[dict]
-0000fde0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-0000fdf0: 2073 6c69 6465 725f 6d61 726b 733a 204f   slider_marks: O
-0000fe00: 7074 696f 6e61 6c5b 6c69 7374 5b74 7570  ptional[list[tup
-0000fe10: 6c65 5d5d 203d 204e 6f6e 652c 0a20 2020  le]] = None,.   
-0000fe20: 2029 3a0a 2020 2020 2020 2020 2222 220a   ):.        """.
-0000fe30: 2020 2020 2020 2020 4372 6561 7465 2061          Create a
-0000fe40: 6e20 616e 6e6f 7461 7465 6420 6368 6172  n annotated char
-0000fe50: 7420 696e 2074 6865 206d 656e 7520 7061  t in the menu pa
-0000fe60: 7468 2e0a 2020 2020 2020 2020 3a70 6172  th..        :par
-0000fe70: 616d 2064 6174 613a 2074 6865 2064 6174  am data: the dat
-0000fe80: 6120 6f66 2074 6865 2063 6861 7274 0a20  a of the chart. 
-0000fe90: 2020 2020 2020 203a 7061 7261 6d20 6f72         :param or
-0000fea0: 6465 723a 2074 6865 206f 7264 6572 206f  der: the order o
-0000feb0: 6620 7468 6520 6368 6172 740a 2020 2020  f the chart.    
-0000fec0: 2020 2020 3a70 6172 616d 2078 3a20 7468      :param x: th
-0000fed0: 6520 7820 6178 6973 0a20 2020 2020 2020  e x axis.       
-0000fee0: 203a 7061 7261 6d20 793a 2074 6865 2079   :param y: the y
-0000fef0: 2061 7869 730a 2020 2020 2020 2020 3a70   axis.        :p
-0000ff00: 6172 616d 2061 6e6e 6f74 6174 696f 6e73  aram annotations
-0000ff10: 3a20 7468 6520 616e 6e6f 7461 7469 6f6e  : the annotation
-0000ff20: 730a 2020 2020 2020 2020 3a70 6172 616d  s.        :param
-0000ff30: 2072 6f77 735f 7369 7a65 3a20 7468 6520   rows_size: the 
-0000ff40: 726f 7773 2073 697a 6520 6f66 2074 6865  rows size of the
-0000ff50: 2063 6861 7274 0a20 2020 2020 2020 203a   chart.        :
-0000ff60: 7061 7261 6d20 636f 6c73 5f73 697a 653a  param cols_size:
-0000ff70: 2074 6865 2063 6f6c 756d 6e73 2073 697a   the columns siz
-0000ff80: 6520 6f66 2074 6865 2063 6861 7274 0a20  e of the chart. 
-0000ff90: 2020 2020 2020 203a 7061 7261 6d20 7061         :param pa
-0000ffa0: 6464 696e 673a 2074 6865 2070 6164 6469  dding: the paddi
-0000ffb0: 6e67 206f 6620 7468 6520 6368 6172 740a  ng of the chart.
-0000ffc0: 2020 2020 2020 2020 3a70 6172 616d 2074          :param t
-0000ffd0: 6974 6c65 3a20 7468 6520 7469 746c 6520  itle: the title 
-0000ffe0: 6f66 2074 6865 2063 6861 7274 0a20 2020  of the chart.   
-0000fff0: 2020 2020 203a 7061 7261 6d20 795f 6178       :param y_ax
-00010000: 6973 5f6e 616d 653a 2074 6865 206e 616d  is_name: the nam
-00010010: 6520 6f66 2074 6865 2079 2061 7869 730a  e of the y axis.
-00010020: 2020 2020 2020 2020 3a70 6172 616d 2073          :param s
-00010030: 6c69 6465 725f 636f 6e66 6967 3a20 7468  lider_config: th
-00010040: 6520 736c 6964 6572 2063 6f6e 6669 670a  e slider config.
-00010050: 2020 2020 2020 2020 3a70 6172 616d 2073          :param s
-00010060: 6c69 6465 725f 6d61 726b 733a 2074 6865  lider_marks: the
-00010070: 2073 6c69 6465 7220 6d61 726b 730a 2020   slider marks.  
-00010080: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00010090: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
-000100a0: 6461 7461 2c20 7374 7229 3a0a 2020 2020  data, str):.    
-000100b0: 2020 2020 2020 2020 6c6f 675f 6572 726f          log_erro
-000100c0: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
-000100d0: 2020 206c 6f67 6765 722c 0a20 2020 2020     logger,.     
-000100e0: 2020 2020 2020 2020 2020 2022 416e 6e6f             "Anno
-000100f0: 7461 7465 6420 6368 6172 7420 646f 6573  tated chart does
-00010100: 206e 6f74 2073 7570 706f 7274 2074 6865   not support the
-00010110: 2075 7365 206f 6620 7368 6172 6564 2064   use of shared d
-00010120: 6174 6122 2c0a 2020 2020 2020 2020 2020  ata",.          
-00010130: 2020 2020 2020 4461 7461 4572 726f 722c        DataError,
-00010140: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
-00010150: 2020 2020 2020 2020 6966 2073 6c69 6465          if slide
-00010160: 725f 636f 6e66 6967 2069 7320 4e6f 6e65  r_config is None
-00010170: 3a0a 2020 2020 2020 2020 2020 2020 736c  :.            sl
-00010180: 6964 6572 5f63 6f6e 6669 6720 3d20 7b7d  ider_config = {}
-00010190: 0a0a 2020 2020 2020 2020 6966 2073 6c69  ..        if sli
-000101a0: 6465 725f 6d61 726b 733a 0a20 2020 2020  der_marks:.     
-000101b0: 2020 2020 2020 2073 6c69 6465 725f 636f         slider_co
-000101c0: 6e66 6967 5b22 6d61 726b 7322 5d20 3d20  nfig["marks"] = 
-000101d0: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
-000101e0: 2020 7b22 6c61 6265 6c22 3a20 6d61 726b    {"label": mark
-000101f0: 5b30 5d2c 2022 7661 6c75 6522 3a20 6d61  [0], "value": ma
-00010200: 726b 5b31 5d7d 2066 6f72 206d 6172 6b20  rk[1]} for mark 
-00010210: 696e 2073 6c69 6465 725f 6d61 726b 730a  in slider_marks.
-00010220: 2020 2020 2020 2020 2020 2020 5d0a 0a20              ].. 
-00010230: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
-00010240: 616e 6365 2879 2c20 7374 7229 3a0a 2020  ance(y, str):.  
-00010250: 2020 2020 2020 2020 2020 7920 3d20 5b79            y = [y
-00010260: 5d0a 0a20 2020 2020 2020 2069 6620 6e6f  ]..        if no
-00010270: 7420 6c65 6e28 7929 203d 3d20 6c65 6e28  t len(y) == len(
-00010280: 6461 7461 293a 0a20 2020 2020 2020 2020  data):.         
-00010290: 2020 206c 6f67 5f65 7272 6f72 280a 2020     log_error(.  
-000102a0: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-000102b0: 6767 6572 2c0a 2020 2020 2020 2020 2020  gger,.          
-000102c0: 2020 2020 2020 6622 4e75 6d62 6572 206f        f"Number o
-000102d0: 6620 7920 7661 6c75 6573 2028 7b6c 656e  f y values ({len
-000102e0: 2879 297d 2920 646f 6573 206e 6f74 206d  (y)}) does not m
-000102f0: 6174 6368 206e 756d 6265 7220 6f66 2064  atch number of d
-00010300: 6174 6166 7261 6d65 7320 287b 6c65 6e28  ataframes ({len(
-00010310: 6461 7461 297d 2922 2c0a 2020 2020 2020  data)})",.      
-00010320: 2020 2020 2020 2020 2020 4461 7461 4572            DataEr
-00010330: 726f 722c 0a20 2020 2020 2020 2020 2020  ror,.           
-00010340: 2029 0a0a 2020 2020 2020 2020 5f2c 2072   )..        _, r
-00010350: 6570 6f72 7420 3d20 6177 6169 7420 7365  eport = await se
-00010360: 6c66 2e5f 6765 745f 6368 6172 745f 7265  lf._get_chart_re
-00010370: 706f 7274 286f 7264 6572 2c20 416e 6e6f  port(order, Anno
-00010380: 7461 7465 6445 4368 6172 7429 0a0a 2020  tatedEChart)..  
-00010390: 2020 2020 2020 6466 7320 3d20 5b76 616c        dfs = [val
-000103a0: 6964 6174 655f 6461 7461 5f69 735f 7061  idate_data_is_pa
-000103b0: 6e64 6172 6162 6c65 2864 6629 2066 6f72  ndarable(df) for
-000103c0: 2064 6620 696e 2064 6174 615d 0a20 2020   df in data].   
-000103d0: 2020 2020 2064 6174 615f 7365 745f 7461       data_set_ta
-000103e0: 736b 7320 3d20 5b5d 0a20 2020 2020 2020  sks = [].       
-000103f0: 2066 6f72 2064 662c 2079 5f76 616c 2069   for df, y_val i
-00010400: 6e20 7a69 7028 6466 732c 2079 293a 0a20  n zip(dfs, y):. 
-00010410: 2020 2020 2020 2020 2020 2064 665b 785d             df[x]
-00010420: 203d 2070 642e 746f 5f64 6174 6574 696d   = pd.to_datetim
-00010430: 6528 6466 5b78 5d29 0a20 2020 2020 2020  e(df[x]).       
-00010440: 2020 2020 2069 6620 616e 6e6f 7461 7469       if annotati
-00010450: 6f6e 7320 696e 2064 663a 0a20 2020 2020  ons in df:.     
-00010460: 2020 2020 2020 2020 2020 2064 665b 616e             df[an
-00010470: 6e6f 7461 7469 6f6e 735d 203d 2028 0a20  notations] = (. 
-00010480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010490: 2020 2064 665b 616e 6e6f 7461 7469 6f6e     df[annotation
-000104a0: 735d 2e72 6570 6c61 6365 286e 702e 6e61  s].replace(np.na
-000104b0: 6e2c 2022 222c 2072 6567 6578 3d54 7275  n, "", regex=Tru
-000104c0: 6529 2e61 7374 7970 6528 7374 7229 0a20  e).astype(str). 
-000104d0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-000104e0: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
-000104f0: 615f 7365 745f 7461 736b 732e 6170 7065  a_set_tasks.appe
-00010500: 6e64 280a 2020 2020 2020 2020 2020 2020  nd(.            
-00010510: 2020 2020 7365 6c66 2e5f 6372 6561 7465      self._create
-00010520: 5f64 6174 615f 7365 7428 6e61 6d65 3d66  _data_set(name=f
-00010530: 227b 7265 706f 7274 5b27 6964 275d 7d5f  "{report['id']}_
-00010540: 7b79 5f76 616c 7d22 2c20 6461 7461 3d64  {y_val}", data=d
-00010550: 6629 0a20 2020 2020 2020 2020 2020 2029  f).            )
-00010560: 0a0a 2020 2020 2020 2020 6461 7461 5f73  ..        data_s
-00010570: 6574 5f64 6963 7473 203d 2061 7761 6974  et_dicts = await
-00010580: 2061 7379 6e63 696f 2e67 6174 6865 7228   asyncio.gather(
-00010590: 2a64 6174 615f 7365 745f 7461 736b 7329  *data_set_tasks)
-000105a0: 0a20 2020 2020 2020 2064 6174 615f 7365  .        data_se
-000105b0: 7473 203d 205b 6473 5b79 5f76 616c 5d5b  ts = [ds[y_val][
-000105c0: 315d 2066 6f72 2064 732c 2079 5f76 616c  1] for ds, y_val
-000105d0: 2069 6e20 7a69 7028 6461 7461 5f73 6574   in zip(data_set
-000105e0: 5f64 6963 7473 2c20 7929 5d0a 0a20 2020  _dicts, y)]..   
-000105f0: 2020 2020 2072 645f 6964 7320 3d20 4e6f       rd_ids = No
-00010600: 6e65 0a20 2020 2020 2020 2069 6620 7365  ne.        if se
-00010610: 6c66 2e72 6575 7365 5f64 6174 615f 7365  lf.reuse_data_se
-00010620: 7473 3a0a 2020 2020 2020 2020 2020 2020  ts:.            
-00010630: 7264 5f69 6473 203d 2067 6574 5f75 7569  rd_ids = get_uui
-00010640: 6473 5f66 726f 6d5f 6469 6374 2872 6570  ds_from_dict(rep
-00010650: 6f72 745b 2270 726f 7065 7274 6965 7322  ort["properties"
-00010660: 5d5b 226f 7074 696f 6e22 5d29 0a20 2020  ]["option"]).   
-00010670: 2020 2020 2020 2020 2069 6620 6c65 6e28           if len(
-00010680: 7264 5f69 6473 2920 3d3d 206c 656e 2879  rd_ids) == len(y
-00010690: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-000106a0: 2020 2072 6570 5f64 733a 206c 6973 745b     rep_ds: list[
-000106b0: 5265 706f 7274 2e52 6570 6f72 7444 6174  Report.ReportDat
-000106c0: 6153 6574 5d20 3d20 6177 6169 7420 7265  aSet] = await re
-000106d0: 706f 7274 2e67 6574 5f72 6570 6f72 745f  port.get_report_
-000106e0: 6461 7461 5f73 6574 7328 290a 2020 2020  data_sets().    
-000106f0: 2020 2020 2020 2020 2020 2020 7265 705f              rep_
-00010700: 6473 203d 205b 0a20 2020 2020 2020 2020  ds = [.         
-00010710: 2020 2020 2020 2020 2020 206e 6578 7428             next(
-00010720: 2872 6420 666f 7220 7264 2069 6e20 7265  (rd for rd in re
-00010730: 705f 6473 2069 6620 7264 5b22 6964 225d  p_ds if rd["id"]
-00010740: 203d 3d20 7264 5f69 6429 2c20 4e6f 6e65   == rd_id), None
-00010750: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00010760: 2020 2020 2020 666f 7220 7264 5f69 6420        for rd_id 
-00010770: 696e 2072 645f 6964 730a 2020 2020 2020  in rd_ids.      
-00010780: 2020 2020 2020 2020 2020 5d0a 2020 2020            ].    
-00010790: 2020 2020 2020 2020 2020 2020 6966 2061              if a
-000107a0: 6e79 280a 2020 2020 2020 2020 2020 2020  ny(.            
-000107b0: 2020 2020 2020 2020 7264 5b22 6461 7461          rd["data
-000107c0: 5365 7449 6422 5d20 213d 2064 735b 2269  SetId"] != ds["i
-000107d0: 6422 5d0a 2020 2020 2020 2020 2020 2020  d"].            
-000107e0: 2020 2020 2020 2020 6f72 2072 645b 2270          or rd["p
-000107f0: 726f 7065 7274 6965 7322 5d5b 226d 6170  roperties"]["map
-00010800: 7069 6e67 225d 0a20 2020 2020 2020 2020  ping"].         
-00010810: 2020 2020 2020 2020 2020 2021 3d20 7b22             != {"
-00010820: 7661 6c75 6573 223a 205b 2264 6174 6546  values": ["dateF
-00010830: 6965 6c64 3122 2c20 2269 6e74 4669 656c  ield1", "intFiel
-00010840: 6431 225d 2c20 226c 6162 656c 223a 2022  d1"], "label": "
-00010850: 7374 7269 6e67 4669 656c 6431 227d 0a20  stringField1"}. 
-00010860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010870: 2020 2066 6f72 2072 642c 2064 7320 696e     for rd, ds in
-00010880: 207a 6970 2872 6570 5f64 732c 2064 6174   zip(rep_ds, dat
-00010890: 615f 7365 7473 290a 2020 2020 2020 2020  a_sets).        
-000108a0: 2020 2020 2020 2020 293a 0a20 2020 2020          ):.     
-000108b0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-000108c0: 645f 6964 7320 3d20 4e6f 6e65 0a0a 2020  d_ids = None..  
-000108d0: 2020 2020 2020 6966 206e 6f74 2072 645f        if not rd_
-000108e0: 6964 733a 0a20 2020 2020 2020 2020 2020  ids:.           
-000108f0: 2061 7761 6974 2072 6570 6f72 742e 6465   await report.de
-00010900: 6c65 7465 5f72 6570 6f72 745f 6461 7461  lete_report_data
-00010910: 5f73 6574 7328 6c6f 673d 5472 7565 290a  _sets(log=True).
-00010920: 2020 2020 2020 2020 2020 2020 6d61 7070              mapp
-00010930: 696e 673a 204d 6170 7069 6e67 203d 207b  ing: Mapping = {
-00010940: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010950: 2022 7661 6c75 6573 223a 205b 2264 6174   "values": ["dat
-00010960: 6546 6965 6c64 3122 2c20 2269 6e74 4669  eField1", "intFi
-00010970: 656c 6431 225d 2c0a 2020 2020 2020 2020  eld1"],.        
-00010980: 2020 2020 2020 2020 226c 6162 656c 223a          "label":
-00010990: 2022 7374 7269 6e67 4669 656c 6431 222c   "stringField1",
-000109a0: 0a20 2020 2020 2020 2020 2020 207d 0a20  .            }. 
-000109b0: 2020 2020 2020 2020 2020 2072 6570 6f72             repor
-000109c0: 745f 6461 7461 5f73 6574 7320 3d20 6177  t_data_sets = aw
-000109d0: 6169 7420 6173 796e 6369 6f2e 6761 7468  ait asyncio.gath
-000109e0: 6572 280a 2020 2020 2020 2020 2020 2020  er(.            
-000109f0: 2020 2020 2a5b 0a20 2020 2020 2020 2020      *[.         
-00010a00: 2020 2020 2020 2020 2020 2072 6570 6f72             repor
-00010a10: 742e 6372 6561 7465 5f72 6570 6f72 745f  t.create_report_
-00010a20: 6461 7461 5f73 6574 2828 6d61 7070 696e  data_set((mappin
-00010a30: 672c 2064 6174 615f 7365 742c 204e 6f6e  g, data_set, Non
-00010a40: 6529 290a 2020 2020 2020 2020 2020 2020  e)).            
-00010a50: 2020 2020 2020 2020 666f 7220 6461 7461          for data
-00010a60: 5f73 6574 2069 6e20 6461 7461 5f73 6574  _set in data_set
-00010a70: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
-00010a80: 2020 5d0a 2020 2020 2020 2020 2020 2020    ].            
-00010a90: 290a 2020 2020 2020 2020 2020 2020 7264  ).            rd
-00010aa0: 5f69 6473 203d 205b 7264 5b22 6964 225d  _ids = [rd["id"]
-00010ab0: 2066 6f72 2072 6420 696e 2072 6570 6f72   for rd in repor
-00010ac0: 745f 6461 7461 5f73 6574 735d 0a0a 2020  t_data_sets]..  
-00010ad0: 2020 2020 2020 6368 6172 745f 6f70 7469        chart_opti
-00010ae0: 6f6e 7320 3d20 7b0a 2020 2020 2020 2020  ons = {.        
-00010af0: 2020 2020 2279 4178 6973 223a 207b 0a20      "yAxis": {. 
-00010b00: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00010b10: 6e61 6d65 223a 2079 5f61 7869 735f 6e61  name": y_axis_na
-00010b20: 6d65 206f 7220 2222 2c0a 2020 2020 2020  me or "",.      
-00010b30: 2020 2020 2020 2020 2020 2266 6f6e 7422            "font"
-00010b40: 2022 7479 7065 223a 2022 7661 6c75 6522   "type": "value"
-00010b50: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00010b60: 2020 226e 616d 654c 6f63 6174 696f 6e22    "nameLocation"
-00010b70: 3a20 226d 6964 646c 6522 2c0a 2020 2020  : "middle",.    
-00010b80: 2020 2020 2020 2020 2020 2020 226e 616d              "nam
-00010b90: 6547 6170 223a 2033 302c 0a20 2020 2020  eGap": 30,.     
-00010ba0: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
-00010bb0: 2020 2020 2020 2278 4178 6973 223a 207b        "xAxis": {
-00010bc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010bd0: 2022 7479 7065 223a 2022 7469 6d65 222c   "type": "time",
-00010be0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010bf0: 2022 6e61 6d65 4c6f 6361 7469 6f6e 223a   "nameLocation":
-00010c00: 2022 6d69 6464 6c65 222c 0a20 2020 2020   "middle",.     
-00010c10: 2020 2020 2020 2020 2020 2022 6e61 6d65             "name
-00010c20: 4761 7022 3a20 3330 2c0a 2020 2020 2020  Gap": 30,.      
-00010c30: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-00010c40: 2020 2020 2022 7365 7269 6573 223a 205b       "series": [
-00010c50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010c60: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-00010c70: 2020 2020 2020 2022 6461 7461 223a 2022         "data": "
-00010c80: 237b 2220 2b20 7264 5f69 6420 2b20 227d  #{" + rd_id + "}
-00010c90: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00010ca0: 2020 2020 2020 2022 7479 7065 223a 2022         "type": "
-00010cb0: 6c69 6e65 222c 0a20 2020 2020 2020 2020  line",.         
-00010cc0: 2020 2020 2020 2020 2020 2022 6e61 6d65             "name
-00010cd0: 223a 2079 5f6e 616d 652c 0a20 2020 2020  ": y_name,.     
-00010ce0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00010cf0: 6974 656d 5374 796c 6522 3a20 7b0a 2020  itemStyle": {.  
-00010d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010d10: 2020 2020 2020 2262 6f72 6465 7252 6164        "borderRad
-00010d20: 6975 7322 3a20 5b39 2c20 392c 2030 2c20  ius": [9, 9, 0, 
-00010d30: 305d 2c0a 2020 2020 2020 2020 2020 2020  0],.            
-00010d40: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-00010d50: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
-00010d60: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00010d70: 2079 5f6e 616d 652c 2072 645f 6964 2069   y_name, rd_id i
-00010d80: 6e20 7a69 7028 792c 2072 645f 6964 7329  n zip(y, rd_ids)
-00010d90: 0a20 2020 2020 2020 2020 2020 205d 2c0a  .            ],.
-00010da0: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-00010db0: 2020 6177 6169 7420 7365 6c66 2e5f 6372    await self._cr
-00010dc0: 6561 7465 5f63 6861 7274 280a 2020 2020  eate_chart(.    
-00010dd0: 2020 2020 2020 2020 6368 6172 745f 636c          chart_cl
-00010de0: 6173 733d 416e 6e6f 7461 7465 6445 4368  ass=AnnotatedECh
-00010df0: 6172 742c 0a20 2020 2020 2020 2020 2020  art,.           
-00010e00: 206f 7264 6572 3d6f 7264 6572 2c0a 2020   order=order,.  
-00010e10: 2020 2020 2020 2020 2020 7369 7a65 5061            sizePa
-00010e20: 6464 696e 673d 7061 6464 696e 672c 0a20  dding=padding,. 
-00010e30: 2020 2020 2020 2020 2020 2073 697a 6552             sizeR
-00010e40: 6f77 733d 726f 7773 5f73 697a 652c 0a20  ows=rows_size,. 
-00010e50: 2020 2020 2020 2020 2020 2073 697a 6543             sizeC
-00010e60: 6f6c 756d 6e73 3d63 6f6c 735f 7369 7a65  olumns=cols_size
-00010e70: 2c0a 2020 2020 2020 2020 2020 2020 7469  ,.            ti
-00010e80: 746c 653d 7469 746c 652c 0a20 2020 2020  tle=title,.     
-00010e90: 2020 2020 2020 2070 726f 7065 7274 6965         propertie
-00010ea0: 733d 6469 6374 280a 2020 2020 2020 2020  s=dict(.        
-00010eb0: 2020 2020 2020 2020 736c 6964 6572 3d73          slider=s
-00010ec0: 6c69 6465 725f 636f 6e66 6967 2c0a 2020  lider_config,.  
-00010ed0: 2020 2020 2020 2020 2020 2020 2020 6f70                op
-00010ee0: 7469 6f6e 3d63 6861 7274 5f6f 7074 696f  tion=chart_optio
-00010ef0: 6e73 2c0a 2020 2020 2020 2020 2020 2020  ns,.            
-00010f00: 292c 0a20 2020 2020 2020 2029 0a0a 2020  ),.        )..  
-00010f10: 2020 6173 796e 6320 6465 6620 5f67 6574    async def _get
-00010f20: 5f72 6570 6f72 745f 6461 7461 5f73 6574  _report_data_set
-00010f30: 735f 7065 725f 6d61 7070 696e 6728 0a20  s_per_mapping(. 
-00010f40: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-00010f50: 2020 2020 2072 6570 6f72 743a 2052 6570       report: Rep
-00010f60: 6f72 742c 0a20 2020 2020 2020 2064 6174  ort,.        dat
-00010f70: 615f 6d61 7070 696e 675f 746f 5f74 7570  a_mapping_to_tup
-00010f80: 6c65 3a20 6469 6374 2c0a 2020 2020 2020  le: dict,.      
-00010f90: 2020 6669 656c 6473 3a20 6c69 7374 5b55    fields: list[U
-00010fa0: 6e69 6f6e 5b74 7570 6c65 2c20 6469 6374  nion[tuple, dict
-00010fb0: 5d5d 2c0a 2020 2020 2920 2d3e 206c 6973  ]],.    ) -> lis
-00010fc0: 745b 5265 706f 7274 2e52 6570 6f72 7444  t[Report.ReportD
-00010fd0: 6174 6153 6574 5d3a 0a20 2020 2020 2020  ataSet]:.       
-00010fe0: 2022 2222 4372 6561 7465 2061 2064 6174   """Create a dat
-00010ff0: 615f 7365 7420 7065 7220 6669 656c 6420  a_set per field 
-00011000: 6f66 2061 2064 6174 6166 7261 6d65 2e0a  of a dataframe..
-00011010: 2020 2020 2020 2020 3a70 6172 616d 2072          :param r
-00011020: 6570 6f72 743a 2074 6865 2072 6570 6f72  eport: the repor
-00011030: 740a 2020 2020 2020 2020 3a70 6172 616d  t.        :param
-00011040: 2064 6174 615f 6d61 7070 696e 675f 746f   data_mapping_to
-00011050: 5f74 7570 6c65 3a20 7468 6520 6d61 7070  _tuple: the mapp
-00011060: 696e 6720 6f66 2074 6865 2064 6174 610a  ing of the data.
-00011070: 2020 2020 2020 2020 3a70 6172 616d 2066          :param f
-00011080: 6965 6c64 733a 2074 6865 2066 6965 6c64  ields: the field
-00011090: 7320 6f66 2074 6865 2064 6174 6120 746f  s of the data to
-000110a0: 2062 6520 7573 6564 0a20 2020 2020 2020   be used.       
-000110b0: 203a 7265 7475 726e 3a20 7468 6520 6c69   :return: the li
-000110c0: 7374 206f 6620 6461 7461 2073 6574 7320  st of data sets 
-000110d0: 7061 7274 6974 696f 6e65 6420 6279 2061  partitioned by a
-000110e0: 7869 7320 616e 6420 6669 656c 6473 0a20  xis and fields. 
-000110f0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00011100: 2020 2074 6173 6b73 203d 205b 5d0a 2020     tasks = [].  
-00011110: 2020 2020 2020 6669 656c 6473 203d 2066        fields = f
-00011120: 6965 6c64 7320 6966 2066 6965 6c64 7320  ields if fields 
-00011130: 656c 7365 205b 5d0a 2020 2020 2020 2020  else [].        
-00011140: 666f 7220 692c 2066 2069 6e20 656e 756d  for i, f in enum
-00011150: 6572 6174 6528 6669 656c 6473 293a 0a20  erate(fields):. 
-00011160: 2020 2020 2020 2020 2020 206d 6170 7069             mappi
-00011170: 6e67 203d 205b 5d0a 2020 2020 2020 2020  ng = [].        
-00011180: 2020 2020 6461 7461 5f73 6574 203d 204e      data_set = N
-00011190: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
-000111a0: 7265 735f 736f 7274 203d 204e 6f6e 650a  res_sort = None.
-000111b0: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-000111c0: 7369 6e73 7461 6e63 6528 662c 2073 7472  sinstance(f, str
-000111d0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-000111e0: 2020 2069 6620 6620 6e6f 7420 696e 2064     if f not in d
-000111f0: 6174 615f 6d61 7070 696e 675f 746f 5f74  ata_mapping_to_t
-00011200: 7570 6c65 3a0a 2020 2020 2020 2020 2020  uple:.          
-00011210: 2020 2020 2020 2020 2020 6c6f 675f 6572            log_er
-00011220: 726f 7228 6c6f 6767 6572 2c20 6622 4669  ror(logger, f"Fi
-00011230: 656c 6420 7b66 7d20 6e6f 7420 666f 756e  eld {f} not foun
-00011240: 6420 696e 2064 6174 6122 2c20 4461 7461  d in data", Data
-00011250: 4572 726f 7229 0a20 2020 2020 2020 2020  Error).         
-00011260: 2020 2020 2020 206d 6170 7069 6e67 2c20         mapping, 
-00011270: 6461 7461 5f73 6574 2c20 7265 735f 736f  data_set, res_so
-00011280: 7274 203d 2064 6174 615f 6d61 7070 696e  rt = data_mappin
-00011290: 675f 746f 5f74 7570 6c65 5b66 5d0a 2020  g_to_tuple[f].  
-000112a0: 2020 2020 2020 2020 2020 656c 6966 2069            elif i
-000112b0: 7369 6e73 7461 6e63 6528 662c 2028 7475  sinstance(f, (tu
-000112c0: 706c 652c 206c 6973 7429 293a 0a20 2020  ple, list)):.   
-000112d0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-000112e0: 2066 5f20 696e 2066 3a0a 2020 2020 2020   f_ in f:.      
-000112f0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00011300: 2066 5f20 6e6f 7420 696e 2064 6174 615f   f_ not in data_
-00011310: 6d61 7070 696e 675f 746f 5f74 7570 6c65  mapping_to_tuple
-00011320: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00011330: 2020 2020 2020 2020 2020 6c6f 675f 6572            log_er
-00011340: 726f 7228 6c6f 6767 6572 2c20 6622 4669  ror(logger, f"Fi
-00011350: 656c 6420 7b66 5f7d 206e 6f74 2066 6f75  eld {f_} not fou
-00011360: 6e64 2069 6e20 6461 7461 222c 2044 6174  nd in data", Dat
-00011370: 6145 7272 6f72 290a 2020 2020 2020 2020  aError).        
-00011380: 2020 2020 2020 2020 2020 2020 6d61 7070              mapp
-00011390: 696e 675f 2c20 6461 7461 5f73 6574 5f2c  ing_, data_set_,
-000113a0: 2072 6573 5f73 6f72 745f 203d 2064 6174   res_sort_ = dat
-000113b0: 615f 6d61 7070 696e 675f 746f 5f74 7570  a_mapping_to_tup
-000113c0: 6c65 5b66 5f5d 0a20 2020 2020 2020 2020  le[f_].         
-000113d0: 2020 2020 2020 2020 2020 206d 6170 7069             mappi
-000113e0: 6e67 2e61 7070 656e 6428 6d61 7070 696e  ng.append(mappin
-000113f0: 675f 290a 2020 2020 2020 2020 2020 2020  g_).            
-00011400: 2020 2020 2020 2020 6461 7461 5f73 6574          data_set
-00011410: 203d 2064 6174 615f 7365 7420 6966 2064   = data_set if d
-00011420: 6174 615f 7365 7420 656c 7365 2064 6174  ata_set else dat
-00011430: 615f 7365 745f 0a20 2020 2020 2020 2020  a_set_.         
-00011440: 2020 2020 2020 2020 2020 2072 6573 5f73             res_s
-00011450: 6f72 7420 3d20 7265 735f 736f 7274 2069  ort = res_sort i
-00011460: 6620 7265 735f 736f 7274 2065 6c73 6520  f res_sort else 
-00011470: 7265 735f 736f 7274 5f0a 2020 2020 2020  res_sort_.      
-00011480: 2020 2020 2020 2020 2020 2020 2020 6173                as
-00011490: 7365 7274 2064 6174 615f 7365 7420 3d3d  sert data_set ==
-000114a0: 2064 6174 615f 7365 745f 0a20 2020 2020   data_set_.     
-000114b0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-000114c0: 7373 6572 7420 7265 735f 736f 7274 203d  ssert res_sort =
-000114d0: 3d20 7265 735f 736f 7274 5f0a 2020 2020  = res_sort_.    
-000114e0: 2020 2020 2020 2020 656c 6966 2069 7369          elif isi
-000114f0: 6e73 7461 6e63 6528 662c 2064 6963 7429  nstance(f, dict)
-00011500: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00011510: 2020 6d61 7070 696e 6720 3d20 7b6b 3a20    mapping = {k: 
-00011520: 5b5d 2066 6f72 206b 2069 6e20 662e 6b65  [] for k in f.ke
-00011530: 7973 2829 7d0a 2020 2020 2020 2020 2020  ys()}.          
-00011540: 2020 2020 2020 666f 7220 6b2c 2066 5f20        for k, f_ 
-00011550: 696e 2066 2e69 7465 6d73 2829 3a0a 2020  in f.items():.  
-00011560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011570: 2020 6966 2066 5f20 6e6f 7420 696e 2064    if f_ not in d
-00011580: 6174 615f 6d61 7070 696e 675f 746f 5f74  ata_mapping_to_t
-00011590: 7570 6c65 3a0a 2020 2020 2020 2020 2020  uple:.          
-000115a0: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-000115b0: 675f 6572 726f 7228 6c6f 6767 6572 2c20  g_error(logger, 
-000115c0: 6622 4669 656c 6420 7b66 5f7d 206e 6f74  f"Field {f_} not
-000115d0: 2066 6f75 6e64 2069 6e20 6461 7461 222c   found in data",
-000115e0: 2044 6174 6145 7272 6f72 290a 2020 2020   DataError).    
-000115f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011600: 6d61 7070 696e 675f 2c20 6461 7461 5f73  mapping_, data_s
-00011610: 6574 5f2c 2072 6573 5f73 6f72 745f 203d  et_, res_sort_ =
-00011620: 2064 6174 615f 6d61 7070 696e 675f 746f   data_mapping_to
-00011630: 5f74 7570 6c65 5b66 5f5d 0a20 2020 2020  _tuple[f_].     
-00011640: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00011650: 6170 7069 6e67 5b6b 5d20 3d20 6d61 7070  apping[k] = mapp
-00011660: 696e 675f 0a20 2020 2020 2020 2020 2020  ing_.           
-00011670: 2020 2020 2020 2020 2064 6174 615f 7365           data_se
-00011680: 7420 3d20 6461 7461 5f73 6574 2069 6620  t = data_set if 
-00011690: 6461 7461 5f73 6574 2065 6c73 6520 6461  data_set else da
-000116a0: 7461 5f73 6574 5f0a 2020 2020 2020 2020  ta_set_.        
-000116b0: 2020 2020 2020 2020 2020 2020 7265 735f              res_
-000116c0: 736f 7274 203d 2072 6573 5f73 6f72 7420  sort = res_sort 
-000116d0: 6966 2072 6573 5f73 6f72 7420 656c 7365  if res_sort else
-000116e0: 2072 6573 5f73 6f72 745f 0a20 2020 2020   res_sort_.     
-000116f0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00011700: 7373 6572 7420 6461 7461 5f73 6574 203d  ssert data_set =
-00011710: 3d20 6461 7461 5f73 6574 5f0a 2020 2020  = data_set_.    
-00011720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011730: 6173 7365 7274 2072 6573 5f73 6f72 7420  assert res_sort 
-00011740: 3d3d 2072 6573 5f73 6f72 745f 0a20 2020  == res_sort_.   
-00011750: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-00011760: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00011770: 6f67 5f65 7272 6f72 280a 2020 2020 2020  og_error(.      
-00011780: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-00011790: 6767 6572 2c20 6622 4669 656c 6420 7b66  gger, f"Field {f
-000117a0: 7d20 6973 206e 6f74 2061 2073 7472 696e  } is not a strin
-000117b0: 672c 2074 7570 6c65 2c20 6c69 7374 206f  g, tuple, list o
-000117c0: 7220 6469 6374 222c 2044 6174 6145 7272  r dict", DataErr
-000117d0: 6f72 0a20 2020 2020 2020 2020 2020 2020  or.             
-000117e0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-000117f0: 2074 6173 6b73 2e61 7070 656e 6428 0a20   tasks.append(. 
-00011800: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00011810: 6570 6f72 742e 6372 6561 7465 5f72 6570  eport.create_rep
-00011820: 6f72 745f 6461 7461 5f73 6574 280a 2020  ort_data_set(.  
-00011830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011840: 2020 6d61 7070 696e 675f 6461 7461 5f73    mapping_data_s
-00011850: 6574 5f73 6f72 743d 286d 6170 7069 6e67  et_sort=(mapping
-00011860: 2c20 6461 7461 5f73 6574 2c20 7265 735f  , data_set, res_
-00011870: 736f 7274 290a 2020 2020 2020 2020 2020  sort).          
-00011880: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00011890: 2020 2020 290a 0a20 2020 2020 2020 2072      )..        r
-000118a0: 6570 6f72 745f 6461 7461 5f73 6574 7320  eport_data_sets 
-000118b0: 3d20 6177 6169 7420 6173 796e 6369 6f2e  = await asyncio.
-000118c0: 6761 7468 6572 282a 7461 736b 7329 0a20  gather(*tasks). 
-000118d0: 2020 2020 2020 206c 6f67 6765 722e 696e         logger.in
-000118e0: 666f 280a 2020 2020 2020 2020 2020 2020  fo(.            
-000118f0: 6622 4372 6561 7465 6420 7b6c 656e 2872  f"Created {len(r
-00011900: 6570 6f72 745f 6461 7461 5f73 6574 7329  eport_data_sets)
-00011910: 7d20 636f 6d70 6f6e 656e 7420 6461 7461  } component data
-00011920: 2073 6574 206c 696e 6b73 2066 6f72 2063   set links for c
-00011930: 6f6d 706f 6e65 6e74 207b 7374 7228 7265  omponent {str(re
-00011940: 706f 7274 297d 220a 2020 2020 2020 2020  port)}".        
-00011950: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00011960: 2072 6570 6f72 745f 6461 7461 5f73 6574   report_data_set
-00011970: 730a 0a20 2020 2064 6566 205f 7570 6461  s..    def _upda
-00011980: 7465 5f6f 7074 696f 6e73 2873 656c 662c  te_options(self,
-00011990: 206f 7074 696f 6e73 3a20 6469 6374 2c20   options: dict, 
-000119a0: 6f70 7469 6f6e 5f6d 6f64 6966 6963 6174  option_modificat
-000119b0: 696f 6e73 3a20 4f70 7469 6f6e 616c 5b64  ions: Optional[d
-000119c0: 6963 745d 293a 0a20 2020 2020 2020 2022  ict]):.        "
-000119d0: 2222 5570 6461 7465 2074 6865 206f 7074  ""Update the opt
-000119e0: 696f 6e73 206f 6620 616e 2065 6368 6172  ions of an echar
-000119f0: 742e 0a20 2020 2020 2020 203a 7061 7261  t..        :para
-00011a00: 6d20 6f70 7469 6f6e 733a 2074 6865 206f  m options: the o
-00011a10: 7074 696f 6e73 206f 6620 7468 6520 6563  ptions of the ec
-00011a20: 6861 7274 0a20 2020 2020 2020 203a 7061  hart.        :pa
-00011a30: 7261 6d20 6f70 7469 6f6e 5f6d 6f64 6966  ram option_modif
-00011a40: 6963 6174 696f 6e73 3a20 7468 6520 6d6f  ications: the mo
-00011a50: 6469 6669 6361 7469 6f6e 7320 746f 2061  difications to a
-00011a60: 7070 6c79 2074 6f20 7468 6520 6f70 7469  pply to the opti
-00011a70: 6f6e 730a 2020 2020 2020 2020 2222 220a  ons.        """.
-00011a80: 2020 2020 2020 2020 6966 206e 6f74 206f          if not o
-00011a90: 7074 696f 6e5f 6d6f 6469 6669 6361 7469  ption_modificati
-00011aa0: 6f6e 733a 0a20 2020 2020 2020 2020 2020  ons:.           
-00011ab0: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
-00011ac0: 666f 7220 6b2c 2076 2069 6e20 6f70 7469  for k, v in opti
-00011ad0: 6f6e 5f6d 6f64 6966 6963 6174 696f 6e73  on_modifications
-00011ae0: 2e69 7465 6d73 2829 3a0a 2020 2020 2020  .items():.      
-00011af0: 2020 2020 2020 6966 206b 203d 3d20 2273        if k == "s
-00011b00: 6572 6965 7322 3a0a 2020 2020 2020 2020  eries":.        
-00011b10: 2020 2020 2020 2020 6c6f 675f 6572 726f          log_erro
-00011b20: 7228 6c6f 6767 6572 2c20 2253 6572 6965  r(logger, "Serie
-00011b30: 7320 6361 6e6e 6f74 2062 6520 6d6f 6469  s cannot be modi
-00011b40: 6669 6564 222c 2044 6174 6145 7272 6f72  fied", DataError
-00011b50: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-00011b60: 206b 203d 3d20 2278 4178 6973 2220 6f72   k == "xAxis" or
-00011b70: 206b 203d 3d20 2279 4178 6973 223a 0a20   k == "yAxis":. 
-00011b80: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00011b90: 6620 6973 696e 7374 616e 6365 2876 2c20  f isinstance(v, 
-00011ba0: 6469 6374 293a 0a20 2020 2020 2020 2020  dict):.         
-00011bb0: 2020 2020 2020 2020 2020 2076 203d 205b             v = [
-00011bc0: 765d 0a20 2020 2020 2020 2020 2020 2020  v].             
-00011bd0: 2020 2069 6620 6c65 6e28 7629 2021 3d20     if len(v) != 
-00011be0: 6c65 6e28 6f70 7469 6f6e 735b 6b5d 293a  len(options[k]):
-00011bf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011c00: 2020 2020 206c 6f67 5f65 7272 6f72 286c       log_error(l
-00011c10: 6f67 6765 722c 2066 2254 6865 206e 756d  ogger, f"The num
-00011c20: 6265 7220 6f66 207b 6b7d 206d 7573 7420  ber of {k} must 
-00011c30: 6265 207b 6c65 6e28 7629 7d22 2c20 4461  be {len(v)}", Da
-00011c40: 7461 4572 726f 7229 0a20 2020 2020 2020  taError).       
-00011c50: 2020 2020 2020 2020 2066 6f72 2069 2c20           for i, 
-00011c60: 765f 2069 6e20 656e 756d 6572 6174 6528  v_ in enumerate(
-00011c70: 7629 3a0a 2020 2020 2020 2020 2020 2020  v):.            
-00011c80: 2020 2020 2020 2020 6f70 7469 6f6e 735b          options[
-00011c90: 6b5d 5b69 5d2e 7570 6461 7465 2876 5f29  k][i].update(v_)
-00011ca0: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-00011cb0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00011cc0: 2020 206f 7074 696f 6e73 5b6b 5d20 3d20     options[k] = 
-00011cd0: 760a 0a20 2020 2061 7379 6e63 2064 6566  v..    async def
-00011ce0: 205f 6372 6561 7465 5f65 6368 6172 7428   _create_echart(
-00011cf0: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-00011d00: 2020 2020 2020 206f 7074 696f 6e73 3a20         options: 
-00011d10: 6469 6374 2c0a 2020 2020 2020 2020 6f72  dict,.        or
-00011d20: 6465 723a 2069 6e74 2c0a 2020 2020 2020  der: int,.      
-00011d30: 2020 6669 656c 6473 3a20 6c69 7374 5b55    fields: list[U
-00011d40: 6e69 6f6e 5b73 7472 2c20 7475 706c 652c  nion[str, tuple,
-00011d50: 2064 6963 745d 5d2c 0a20 2020 2020 2020   dict]],.       
-00011d60: 2064 6174 615f 6d61 7070 696e 675f 746f   data_mapping_to
-00011d70: 5f74 7570 6c65 733a 204f 7074 696f 6e61  _tuples: Optiona
-00011d80: 6c5b 6469 6374 5d20 3d20 4e6f 6e65 2c0a  l[dict] = None,.
-00011d90: 2020 2020 2020 2020 6461 7461 3a20 4f70          data: Op
-00011da0: 7469 6f6e 616c 5b55 6e69 6f6e 5b73 7472  tional[Union[str
-00011db0: 2c20 7064 2e44 6174 6146 7261 6d65 5d5d  , pd.DataFrame]]
-00011dc0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-00011dd0: 2064 756d 705f 7768 6f6c 653a 2062 6f6f   dump_whole: boo
-00011de0: 6c20 3d20 4661 6c73 652c 0a20 2020 2020  l = False,.     
-00011df0: 2020 206f 7074 696f 6e5f 6d6f 6469 6669     option_modifi
-00011e00: 6361 7469 6f6e 733a 204f 7074 696f 6e61  cations: Optiona
-00011e10: 6c5b 6469 6374 5d20 3d20 4e6f 6e65 2c0a  l[dict] = None,.
-00011e20: 2020 2020 2020 2020 7469 746c 653a 204f          title: O
-00011e30: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
-00011e40: 6f6e 652c 0a20 2020 2020 2020 2072 6f77  one,.        row
-00011e50: 735f 7369 7a65 3a20 4f70 7469 6f6e 616c  s_size: Optional
-00011e60: 5b69 6e74 5d20 3d20 4e6f 6e65 2c0a 2020  [int] = None,.  
-00011e70: 2020 2020 2020 636f 6c73 5f73 697a 653a        cols_size:
-00011e80: 204f 7074 696f 6e61 6c5b 696e 745d 203d   Optional[int] =
-00011e90: 204e 6f6e 652c 0a20 2020 2020 2020 2070   None,.        p
-00011ea0: 6164 6469 6e67 3a20 4f70 7469 6f6e 616c  adding: Optional
-00011eb0: 5b73 7472 5d20 3d20 4e6f 6e65 2c0a 2020  [str] = None,.  
-00011ec0: 2020 293a 0a20 2020 2020 2020 2022 2222    ):.        """
-00011ed0: 0a20 2020 2020 2020 2043 7265 6174 6520  .        Create 
-00011ee0: 616e 2065 6368 6172 7420 696e 2074 6865  an echart in the
-00011ef0: 2064 6173 6862 6f61 7264 2c20 6669 6c6c   dashboard, fill
-00011f00: 2069 6e20 7468 6520 6461 7461 2072 6566   in the data ref
-00011f10: 6572 656e 6365 6420 696e 2074 6865 2065  erenced in the e
-00011f20: 6368 6172 745f 6f70 7469 6f6e 7320 616e  chart_options an
-00011f30: 6420 6372 6561 7465 206f 720a 2020 2020  d create or.    
-00011f40: 2020 2020 7570 6461 7465 2074 6865 2063      update the c
-00011f50: 6861 7274 2061 6e64 2064 6174 6120 7365  hart and data se
-00011f60: 7420 6c69 6e6b 732e 0a20 2020 2020 2020  t links..       
-00011f70: 203a 7061 7261 6d20 6f70 7469 6f6e 733a   :param options:
-00011f80: 2074 6865 206f 7074 696f 6e73 206f 6620   the options of 
-00011f90: 7468 6520 6563 6861 7274 0a20 2020 2020  the echart.     
-00011fa0: 2020 203a 7061 7261 6d20 6461 7461 5f6d     :param data_m
-00011fb0: 6170 7069 6e67 5f74 6f5f 7475 706c 6573  apping_to_tuples
-00011fc0: 3a20 7468 6520 6d61 7070 696e 6720 6f66  : the mapping of
-00011fd0: 2074 6865 2064 6174 6120 746f 2074 6865   the data to the
-00011fe0: 2074 7570 6c65 730a 2020 2020 2020 2020   tuples.        
-00011ff0: 3a70 6172 616d 2064 6174 613a 2074 6865  :param data: the
-00012000: 2064 6174 6120 6f66 2074 6865 2065 6368   data of the ech
-00012010: 6172 740a 2020 2020 2020 2020 3a70 6172  art.        :par
-00012020: 616d 2064 756d 705f 7768 6f6c 653a 2077  am dump_whole: w
-00012030: 6865 7468 6572 2074 6f20 6475 6d70 2074  hether to dump t
-00012040: 6865 2077 686f 6c65 2064 6174 610a 2020  he whole data.  
-00012050: 2020 2020 2020 3a70 6172 616d 206f 7074        :param opt
-00012060: 696f 6e5f 6d6f 6469 6669 6361 7469 6f6e  ion_modification
-00012070: 733a 2074 6865 206d 6f64 6966 6963 6174  s: the modificat
-00012080: 696f 6e73 2074 6f20 6170 706c 7920 746f  ions to apply to
-00012090: 2074 6865 206f 7074 696f 6e73 0a20 2020   the options.   
-000120a0: 2020 2020 203a 7061 7261 6d20 7469 746c       :param titl
-000120b0: 653a 2074 6865 2074 6974 6c65 206f 6620  e: the title of 
-000120c0: 7468 6520 6563 6861 7274 0a20 2020 2020  the echart.     
-000120d0: 2020 203a 7061 7261 6d20 726f 7773 5f73     :param rows_s
-000120e0: 697a 653a 2074 6865 2072 6f77 7320 7369  ize: the rows si
-000120f0: 7a65 206f 6620 7468 6520 6563 6861 7274  ze of the echart
-00012100: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00012110: 636f 6c73 5f73 697a 653a 2074 6865 2063  cols_size: the c
-00012120: 6f6c 756d 6e73 2073 697a 6520 6f66 2074  olumns size of t
-00012130: 6865 2065 6368 6172 740a 2020 2020 2020  he echart.      
-00012140: 2020 3a70 6172 616d 2070 6164 6469 6e67    :param padding
-00012150: 3a20 7468 6520 7061 6464 696e 6720 6f66  : the padding of
-00012160: 2074 6865 2065 6368 6172 740a 2020 2020   the echart.    
-00012170: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
-00012180: 2069 6620 6461 7461 2069 7320 6e6f 7420   if data is not 
-00012190: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000121a0: 2020 6461 7461 5f6d 6170 7069 6e67 5f74    data_mapping_t
-000121b0: 6f5f 7475 706c 6573 203d 2061 7761 6974  o_tuples = await
-000121c0: 2073 656c 662e 5f63 686f 6f73 655f 6461   self._choose_da
-000121d0: 7461 280a 2020 2020 2020 2020 2020 2020  ta(.            
-000121e0: 2020 2020 6f72 6465 722c 2064 6174 612c      order, data,
-000121f0: 2064 756d 705f 7768 6f6c 653d 6475 6d70   dump_whole=dump
-00012200: 5f77 686f 6c65 0a20 2020 2020 2020 2020  _whole.         
-00012210: 2020 2029 0a0a 2020 2020 2020 2020 6461     )..        da
-00012220: 7461 5f6b 6579 5f65 6e74 7269 6573 203d  ta_key_entries =
-00012230: 2067 6574 5f64 6174 615f 7265 6665 7265   get_data_refere
-00012240: 6e63 6573 5f66 726f 6d5f 6469 6374 286f  nces_from_dict(o
-00012250: 7074 696f 6e73 290a 2020 2020 2020 2020  ptions).        
-00012260: 5f2c 2072 6570 6f72 7420 3d20 6177 6169  _, report = awai
-00012270: 7420 7365 6c66 2e5f 6765 745f 6368 6172  t self._get_char
-00012280: 745f 7265 706f 7274 286f 7264 6572 2c20  t_report(order, 
-00012290: 4543 6861 7274 290a 0a20 2020 2020 2020  EChart)..       
-000122a0: 2072 645f 6964 7320 3d20 4e6f 6e65 0a20   rd_ids = None. 
-000122b0: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
-000122c0: 6575 7365 5f64 6174 615f 7365 7473 3a0a  euse_data_sets:.
-000122d0: 2020 2020 2020 2020 2020 2020 7264 5f69              rd_i
-000122e0: 6473 203d 2067 6574 5f75 7569 6473 5f66  ds = get_uuids_f
-000122f0: 726f 6d5f 6469 6374 2872 6570 6f72 745b  rom_dict(report[
-00012300: 2270 726f 7065 7274 6965 7322 5d5b 226f  "properties"]["o
-00012310: 7074 696f 6e22 5d29 0a20 2020 2020 2020  ption"]).       
-00012320: 2020 2020 2069 6620 6c65 6e28 7264 5f69       if len(rd_i
-00012330: 6473 2920 3d3d 206c 656e 2866 6965 6c64  ds) == len(field
-00012340: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
-00012350: 2020 2020 7265 705f 6473 3a20 6c69 7374      rep_ds: list
-00012360: 5b52 6570 6f72 742e 5265 706f 7274 4461  [Report.ReportDa
-00012370: 7461 5365 745d 203d 2061 7761 6974 2072  taSet] = await r
-00012380: 6570 6f72 742e 6765 745f 7265 706f 7274  eport.get_report
-00012390: 5f64 6174 615f 7365 7473 2829 0a20 2020  _data_sets().   
-000123a0: 2020 2020 2020 2020 2020 2020 206d 6170               map
-000123b0: 7065 645f 6620 3d20 5b0a 2020 2020 2020  ped_f = [.      
-000123c0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000123d0: 6c66 2e5f 6765 745f 6669 656c 645f 6d61  lf._get_field_ma
-000123e0: 7070 696e 6728 6669 656c 642c 2064 6174  pping(field, dat
-000123f0: 615f 6d61 7070 696e 675f 746f 5f74 7570  a_mapping_to_tup
-00012400: 6c65 7329 0a20 2020 2020 2020 2020 2020  les).           
-00012410: 2020 2020 2020 2020 2066 6f72 2066 6965           for fie
-00012420: 6c64 2069 6e20 6669 656c 6473 0a20 2020  ld in fields.   
-00012430: 2020 2020 2020 2020 2020 2020 205d 0a20               ]. 
-00012440: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00012450: 6f72 2069 2c20 7264 5f69 6420 696e 2065  or i, rd_id in e
-00012460: 6e75 6d65 7261 7465 2872 645f 6964 7329  numerate(rd_ids)
-00012470: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00012480: 2020 2020 2020 7265 706f 7274 5f64 6174        report_dat
-00012490: 615f 7365 7420 3d20 6e65 7874 280a 2020  a_set = next(.  
-000124a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000124b0: 2020 2020 2020 2872 6420 666f 7220 7264        (rd for rd
-000124c0: 2069 6e20 7265 705f 6473 2069 6620 7264   in rep_ds if rd
-000124d0: 5b22 6964 225d 203d 3d20 7264 5f69 6429  ["id"] == rd_id)
-000124e0: 2c20 4e6f 6e65 0a20 2020 2020 2020 2020  , None.         
-000124f0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00012500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012510: 2069 6620 280a 2020 2020 2020 2020 2020   if (.          
-00012520: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
-00012530: 7420 7265 706f 7274 5f64 6174 615f 7365  t report_data_se
-00012540: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
-00012550: 2020 2020 2020 2020 2020 6f72 206e 6f74            or not
-00012560: 2073 656c 662e 5f63 6865 636b 5f6d 6170   self._check_map
-00012570: 7069 6e67 5f69 6e5f 7265 706f 7274 5f64  ping_in_report_d
-00012580: 6174 615f 7365 7428 0a20 2020 2020 2020  ata_set(.       
-00012590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000125a0: 2020 2020 2072 6570 6f72 745f 6461 7461       report_data
-000125b0: 5f73 6574 2c20 6d61 7070 6564 5f66 5b69  _set, mapped_f[i
-000125c0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-000125d0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-000125e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000125f0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00012600: 2020 2020 2020 2020 2020 2072 645f 6964             rd_id
-00012610: 7320 3d20 4e6f 6e65 0a20 2020 2020 2020  s = None.       
-00012620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012630: 2062 7265 616b 0a20 2020 2020 2020 2020   break.         
-00012640: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00012650: 2020 2020 2020 2020 2072 645f 6964 7320           rd_ids 
-00012660: 3d20 4e6f 6e65 0a0a 2020 2020 2020 2020  = None..        
-00012670: 6966 206e 6f74 2072 645f 6964 733a 0a20  if not rd_ids:. 
-00012680: 2020 2020 2020 2020 2020 2061 7761 6974             await
-00012690: 2072 6570 6f72 742e 6465 6c65 7465 5f72   report.delete_r
-000126a0: 6570 6f72 745f 6461 7461 5f73 6574 7328  eport_data_sets(
-000126b0: 6c6f 673d 5472 7565 290a 2020 2020 2020  log=True).      
-000126c0: 2020 2020 2020 7265 706f 7274 5f64 6174        report_dat
-000126d0: 615f 7365 7473 203d 2061 7761 6974 2073  a_sets = await s
-000126e0: 656c 662e 5f67 6574 5f72 6570 6f72 745f  elf._get_report_
-000126f0: 6461 7461 5f73 6574 735f 7065 725f 6d61  data_sets_per_ma
-00012700: 7070 696e 6728 0a20 2020 2020 2020 2020  pping(.         
-00012710: 2020 2020 2020 2072 6570 6f72 742c 2064         report, d
-00012720: 6174 615f 6d61 7070 696e 675f 746f 5f74  ata_mapping_to_t
-00012730: 7570 6c65 732c 2066 6965 6c64 730a 2020  uples, fields.  
-00012740: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00012750: 2020 2020 2020 2020 7264 5f69 6473 203d          rd_ids =
-00012760: 205b 7264 5b22 6964 225d 2066 6f72 2072   [rd["id"] for r
-00012770: 6420 696e 2072 6570 6f72 745f 6461 7461  d in report_data
-00012780: 5f73 6574 735d 0a0a 2020 2020 2020 2020  _sets]..        
-00012790: 7365 6c66 2e5f 7570 6461 7465 5f6f 7074  self._update_opt
-000127a0: 696f 6e73 286f 7074 696f 6e73 2c20 6f70  ions(options, op
-000127b0: 7469 6f6e 5f6d 6f64 6966 6963 6174 696f  tion_modificatio
-000127c0: 6e73 290a 0a20 2020 2020 2020 2069 6620  ns)..        if 
-000127d0: 6c65 6e28 7264 5f69 6473 2920 213d 206c  len(rd_ids) != l
-000127e0: 656e 2864 6174 615f 6b65 795f 656e 7472  en(data_key_entr
-000127f0: 6965 7329 3a0a 2020 2020 2020 2020 2020  ies):.          
-00012800: 2020 6c6f 675f 6572 726f 7228 0a20 2020    log_error(.   
-00012810: 2020 2020 2020 2020 2020 2020 206c 6f67               log
-00012820: 6765 722c 0a20 2020 2020 2020 2020 2020  ger,.           
-00012830: 2020 2020 2066 2254 6865 206e 756d 6265       f"The numbe
-00012840: 7220 6f66 2064 6174 6120 7265 6665 7265  r of data refere
-00012850: 6e63 6573 2061 6e64 2066 6965 6c64 7320  nces and fields 
-00012860: 6d75 7374 2062 6520 6571 7561 6c2c 2022  must be equal, "
-00012870: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012880: 2066 2274 6865 7920 6172 6520 7b6c 656e   f"they are {len
-00012890: 2864 6174 615f 6b65 795f 656e 7472 6965  (data_key_entrie
-000128a0: 7329 7d20 616e 6420 7b6c 656e 2872 645f  s)} and {len(rd_
-000128b0: 6964 7329 7d20 7265 7370 6563 7469 7665  ids)} respective
-000128c0: 6c79 2e22 2c0a 2020 2020 2020 2020 2020  ly.",.          
-000128d0: 2020 2020 2020 4461 7461 4572 726f 722c        DataError,
-000128e0: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
-000128f0: 2020 2020 2020 2020 666f 7220 692c 2064          for i, d
-00012900: 6174 615f 6b65 795f 656e 7472 7920 696e  ata_key_entry in
-00012910: 2065 6e75 6d65 7261 7465 2864 6174 615f   enumerate(data_
-00012920: 6b65 795f 656e 7472 6965 7329 3a0a 2020  key_entries):.  
-00012930: 2020 2020 2020 2020 2020 6461 7461 203d            data =
-00012940: 206f 7074 696f 6e73 0a20 2020 2020 2020   options.       
-00012950: 2020 2020 2066 6f72 206b 6579 2069 6e20       for key in 
-00012960: 6461 7461 5f6b 6579 5f65 6e74 7279 5b3a  data_key_entry[:
-00012970: 2d31 5d3a 0a20 2020 2020 2020 2020 2020  -1]:.           
-00012980: 2020 2020 2064 6174 6120 3d20 6461 7461       data = data
-00012990: 5b6b 6579 5d0a 2020 2020 2020 2020 2020  [key].          
-000129a0: 2020 6461 7461 5b64 6174 615f 6b65 795f    data[data_key_
-000129b0: 656e 7472 795b 2d31 5d5d 203d 2022 237b  entry[-1]] = "#{
-000129c0: 2220 2b20 7264 5f69 6473 5b69 5d20 2b20  " + rd_ids[i] + 
-000129d0: 227d 220a 0a20 2020 2020 2020 2061 7761  "}"..        awa
-000129e0: 6974 2073 656c 662e 5f63 7265 6174 655f  it self._create_
-000129f0: 6368 6172 7428 0a20 2020 2020 2020 2020  chart(.         
-00012a00: 2020 2063 6861 7274 5f63 6c61 7373 3d45     chart_class=E
-00012a10: 4368 6172 742c 0a20 2020 2020 2020 2020  Chart,.         
-00012a20: 2020 2070 726f 7065 7274 6965 733d 7b22     properties={"
-00012a30: 6f70 7469 6f6e 223a 206f 7074 696f 6e73  option": options
-00012a40: 7d2c 0a20 2020 2020 2020 2020 2020 206f  },.            o
-00012a50: 7264 6572 3d6f 7264 6572 2c0a 2020 2020  rder=order,.    
-00012a60: 2020 2020 2020 2020 7469 746c 653d 7469          title=ti
-00012a70: 746c 652c 0a20 2020 2020 2020 2020 2020  tle,.           
-00012a80: 2073 697a 6550 6164 6469 6e67 3d70 6164   sizePadding=pad
-00012a90: 6469 6e67 2c0a 2020 2020 2020 2020 2020  ding,.          
-00012aa0: 2020 7369 7a65 526f 7773 3d72 6f77 735f    sizeRows=rows_
-00012ab0: 7369 7a65 2c0a 2020 2020 2020 2020 2020  size,.          
-00012ac0: 2020 7369 7a65 436f 6c75 6d6e 733d 636f    sizeColumns=co
-00012ad0: 6c73 5f73 697a 652c 0a20 2020 2020 2020  ls_size,.       
-00012ae0: 2029 0a0a 2020 2020 4073 7461 7469 636d   )..    @staticm
-00012af0: 6574 686f 640a 2020 2020 6465 6620 5f61  ethod.    def _a
-00012b00: 7070 6c79 5f76 6172 6961 6e74 2865 6368  pply_variant(ech
-00012b10: 6172 745f 6f70 7469 6f6e 733a 2064 6963  art_options: dic
-00012b20: 742c 2076 6172 6961 6e74 3a20 4f70 7469  t, variant: Opti
-00012b30: 6f6e 616c 5b73 7472 5d29 3a0a 2020 2020  onal[str]):.    
-00012b40: 2020 2020 6966 2076 6172 6961 6e74 203d      if variant =
-00012b50: 3d20 2263 6c65 616e 223a 0a20 2020 2020  = "clean":.     
-00012b60: 2020 2020 2020 2065 6368 6172 745f 6f70         echart_op
-00012b70: 7469 6f6e 732e 7570 6461 7465 280a 2020  tions.update(.  
-00012b80: 2020 2020 2020 2020 2020 2020 2020 7b22                {"
-00012b90: 746f 6f6c 626f 7822 3a20 7b22 7368 6f77  toolbox": {"show
-00012ba0: 223a 2046 616c 7365 7d2c 2022 6c65 6765  ": False}, "lege
-00012bb0: 6e64 223a 207b 2273 686f 7722 3a20 4661  nd": {"show": Fa
-00012bc0: 6c73 657d 2c20 2267 7269 6422 3a20 7b7d  lse}, "grid": {}
-00012bd0: 7d0a 2020 2020 2020 2020 2020 2020 290a  }.            ).
-00012be0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00012bf0: 6178 6973 6c69 7374 2069 6e20 5b65 6368  axislist in [ech
-00012c00: 6172 745f 6f70 7469 6f6e 735b 2278 4178  art_options["xAx
-00012c10: 6973 225d 2c20 6563 6861 7274 5f6f 7074  is"], echart_opt
-00012c20: 696f 6e73 5b22 7941 7869 7322 5d5d 3a0a  ions["yAxis"]]:.
-00012c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012c40: 666f 7220 6178 6973 2069 6e20 6178 6973  for axis in axis
-00012c50: 6c69 7374 3a0a 2020 2020 2020 2020 2020  list:.          
-00012c60: 2020 2020 2020 2020 2020 6178 6973 2e75            axis.u
-00012c70: 7064 6174 6528 0a20 2020 2020 2020 2020  pdate(.         
-00012c80: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-00012c90: 2261 7869 734c 696e 6522 3a20 7b22 7368  "axisLine": {"sh
-00012ca0: 6f77 223a 2046 616c 7365 7d2c 2022 6178  ow": False}, "ax
-00012cb0: 6973 5469 636b 223a 207b 2273 686f 7722  isTick": {"show"
-00012cc0: 3a20 4661 6c73 657d 7d0a 2020 2020 2020  : False}}.      
-00012cd0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-00012ce0: 2020 2020 2020 2020 656c 6966 2076 6172          elif var
-00012cf0: 6961 6e74 203d 3d20 226d 696e 696d 616c  iant == "minimal
-00012d00: 223a 0a20 2020 2020 2020 2020 2020 2065  ":.            e
-00012d10: 6368 6172 745f 6f70 7469 6f6e 732e 7570  chart_options.up
-00012d20: 6461 7465 280a 2020 2020 2020 2020 2020  date(.          
-00012d30: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
-00012d40: 2020 2020 2020 2020 2020 2020 2274 6f6f              "too
-00012d50: 6c62 6f78 223a 207b 2273 686f 7722 3a20  lbox": {"show": 
-00012d60: 4661 6c73 657d 2c0a 2020 2020 2020 2020  False},.        
-00012d70: 2020 2020 2020 2020 2020 2020 226c 6567              "leg
-00012d80: 656e 6422 3a20 7b22 7368 6f77 223a 2046  end": {"show": F
-00012d90: 616c 7365 7d2c 0a20 2020 2020 2020 2020  alse},.         
-00012da0: 2020 2020 2020 2020 2020 2022 6772 6964             "grid
-00012db0: 223a 207b 226c 6566 7422 3a20 2231 2522  ": {"left": "1%"
-00012dc0: 2c20 2272 6967 6874 223a 2022 3125 222c  , "right": "1%",
-00012dd0: 2022 746f 7022 3a20 2231 2522 2c20 2262   "top": "1%", "b
-00012de0: 6f74 746f 6d22 3a20 2231 2522 7d2c 0a20  ottom": "1%"},. 
-00012df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012e00: 2020 2022 746f 6f6c 7469 7022 3a20 7b22     "tooltip": {"
-00012e10: 7368 6f77 223a 2046 616c 7365 7d2c 0a20  show": False},. 
-00012e20: 2020 2020 2020 2020 2020 2020 2020 207d                 }
-00012e30: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-00012e40: 2020 2020 2020 2020 2020 2066 6f72 2061             for a
-00012e50: 7869 736c 6973 7420 696e 205b 6563 6861  xislist in [echa
-00012e60: 7274 5f6f 7074 696f 6e73 5b22 7841 7869  rt_options["xAxi
-00012e70: 7322 5d2c 2065 6368 6172 745f 6f70 7469  s"], echart_opti
-00012e80: 6f6e 735b 2279 4178 6973 225d 5d3a 0a20  ons["yAxis"]]:. 
-00012e90: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00012ea0: 6f72 2061 7869 7320 696e 2061 7869 736c  or axis in axisl
-00012eb0: 6973 743a 0a20 2020 2020 2020 2020 2020  ist:.           
-00012ec0: 2020 2020 2020 2020 2061 7869 732e 7570           axis.up
-00012ed0: 6461 7465 280a 2020 2020 2020 2020 2020  date(.          
-00012ee0: 2020 2020 2020 2020 2020 2020 2020 7b0a                {.
-00012ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012f00: 2020 2020 2020 2020 2020 2020 2261 7869              "axi
-00012f10: 734c 696e 6522 3a20 7b22 7368 6f77 223a  sLine": {"show":
-00012f20: 2046 616c 7365 7d2c 0a20 2020 2020 2020   False},.       
-00012f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012f40: 2020 2020 2022 6178 6973 5469 636b 223a       "axisTick":
-00012f50: 207b 2273 686f 7722 3a20 4661 6c73 657d   {"show": False}
-00012f60: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00012f70: 2020 2020 2020 2020 2020 2020 2020 2273                "s
-00012f80: 706c 6974 4c69 6e65 223a 207b 2273 686f  plitLine": {"sho
-00012f90: 7722 3a20 4661 6c73 657d 2c0a 2020 2020  w": False},.    
-00012fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012fb0: 2020 2020 2020 2020 2261 7869 734c 6162          "axisLab
-00012fc0: 656c 223a 207b 2273 686f 7722 3a20 4661  el": {"show": Fa
-00012fd0: 6c73 657d 2c0a 2020 2020 2020 2020 2020  lse},.          
-00012fe0: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
-00012ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013000: 2020 2020 290a 0a20 2020 2061 7379 6e63      )..    async
-00013010: 2064 6566 205f 6372 6561 7465 5f74 7265   def _create_tre
-00013020: 6e64 5f63 6861 7274 280a 2020 2020 2020  nd_chart(.      
-00013030: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-00013040: 6178 6573 3a20 556e 696f 6e5b 6c69 7374  axes: Union[list
-00013050: 5b73 7472 5d2c 2073 7472 5d2c 0a20 2020  [str], str],.   
-00013060: 2020 2020 206f 7264 6572 3a20 696e 742c       order: int,
-00013070: 0a20 2020 2020 2020 2064 6174 615f 6d61  .        data_ma
-00013080: 7070 696e 675f 746f 5f74 7570 6c65 733a  pping_to_tuples:
-00013090: 204f 7074 696f 6e61 6c5b 6469 6374 5d2c   Optional[dict],
-000130a0: 0a20 2020 2020 2020 2065 6368 6172 745f  .        echart_
-000130b0: 6f70 7469 6f6e 733a 2064 6963 742c 0a20  options: dict,. 
-000130c0: 2020 2020 2020 2073 6572 6965 735f 6f70         series_op
-000130d0: 7469 6f6e 733a 2055 6e69 6f6e 5b64 6963  tions: Union[dic
-000130e0: 742c 206c 6973 745b 6469 6374 5d5d 2c0a  t, list[dict]],.
-000130f0: 2020 2020 2020 2020 7661 6c75 6573 3a20          values: 
-00013100: 4f70 7469 6f6e 616c 5b55 6e69 6f6e 5b6c  Optional[Union[l
-00013110: 6973 745b 556e 696f 6e5b 7374 722c 2074  ist[Union[str, t
-00013120: 7570 6c65 5d5d 2c20 7374 722c 2074 7570  uple]], str, tup
-00013130: 6c65 5d5d 203d 204e 6f6e 652c 0a20 2020  le]] = None,.   
-00013140: 2020 2020 2078 5f61 7869 735f 6e61 6d65       x_axis_name
-00013150: 733a 204f 7074 696f 6e61 6c5b 556e 696f  s: Optional[Unio
-00013160: 6e5b 7374 722c 206c 6973 745b 7374 725d  n[str, list[str]
-00013170: 5d5d 203d 204e 6f6e 652c 0a20 2020 2020  ]] = None,.     
-00013180: 2020 2079 5f61 7869 735f 6e61 6d65 733a     y_axis_names:
-00013190: 204f 7074 696f 6e61 6c5b 556e 696f 6e5b   Optional[Union[
-000131a0: 7374 722c 206c 6973 745b 7374 725d 5d5d  str, list[str]]]
-000131b0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-000131c0: 2073 686f 775f 7661 6c75 6573 3a20 4f70   show_values: Op
-000131d0: 7469 6f6e 616c 5b55 6e69 6f6e 5b6c 6973  tional[Union[lis
-000131e0: 745b 7374 725d 2c20 7374 725d 5d20 3d20  t[str], str]] = 
-000131f0: 4e6f 6e65 2c0a 2020 2020 2020 2020 7661  None,.        va
-00013200: 7269 616e 743a 204f 7074 696f 6e61 6c5b  riant: Optional[
-00013210: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
-00013220: 2020 2020 202a 2a72 6570 6f72 745f 7061       **report_pa
-00013230: 7261 6d73 2c0a 2020 2020 293a 0a20 2020  rams,.    ):.   
-00013240: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00013250: 2043 7265 6174 6520 6120 6c69 6e65 2063   Create a line c
-00013260: 6861 7274 2069 6e20 7468 6520 6461 7368  hart in the dash
-00013270: 626f 6172 642e 0a20 2020 2020 2020 203a  board..        :
-00013280: 7061 7261 6d20 6461 7461 3a20 7468 6520  param data: the 
-00013290: 6461 7461 206f 6620 7468 6520 6368 6172  data of the char
-000132a0: 740a 2020 2020 2020 2020 3a70 6172 616d  t.        :param
-000132b0: 2061 7865 733a 2074 6865 206e 616d 6573   axes: the names
-000132c0: 206f 6620 7468 6520 636f 6c75 6d6e 7320   of the columns 
-000132d0: 746f 2062 6520 7573 6564 2061 7320 6178  to be used as ax
-000132e0: 6973 0a20 2020 2020 2020 203a 7061 7261  is.        :para
-000132f0: 6d20 7661 6c75 6573 3a20 7468 6520 6e61  m values: the na
-00013300: 6d65 7320 6f66 2074 6865 2063 6f6c 756d  mes of the colum
-00013310: 6e73 2074 6f20 6265 2075 7365 6420 6173  ns to be used as
-00013320: 2076 616c 7565 730a 2020 2020 2020 2020   values.        
-00013330: 3a70 6172 616d 2078 5f61 7869 735f 6e61  :param x_axis_na
-00013340: 6d65 733a 2074 6865 206e 616d 6520 6f66  mes: the name of
-00013350: 2074 6865 2078 2061 7865 730a 2020 2020   the x axes.    
-00013360: 2020 2020 3a70 6172 616d 2079 5f61 7869      :param y_axi
-00013370: 735f 6e61 6d65 733a 2074 6865 206e 616d  s_names: the nam
-00013380: 6520 6f66 2074 6865 2079 2061 7865 730a  e of the y axes.
-00013390: 2020 2020 2020 2020 3a70 6172 616d 2065          :param e
-000133a0: 6368 6172 745f 6f70 7469 6f6e 733a 2074  chart_options: t
-000133b0: 6865 206f 7074 696f 6e73 206f 6620 7468  he options of th
-000133c0: 6520 6368 6172 740a 2020 2020 2020 2020  e chart.        
-000133d0: 3a70 6172 616d 2073 6572 6965 735f 6f70  :param series_op
-000133e0: 7469 6f6e 733a 2074 6865 206f 7074 696f  tions: the optio
-000133f0: 6e73 206f 6620 7468 6520 7365 7269 6573  ns of the series
-00013400: 206f 6620 7468 6520 6368 6172 740a 2020   of the chart.  
-00013410: 2020 2020 2020 3a70 6172 616d 2062 6f74        :param bot
-00013420: 746f 6d5f 746f 6f6c 626f 783a 2077 6865  tom_toolbox: whe
-00013430: 7468 6572 2074 6f20 7368 6f77 2074 6865  ther to show the
-00013440: 2074 6f6f 6c62 6f78 206f 6e20 746f 7020   toolbox on top 
-00013450: 6f66 2074 6865 2063 6861 7274 0a20 2020  of the chart.   
-00013460: 2020 2020 203a 7061 7261 6d20 6f72 6465       :param orde
-00013470: 723a 2074 6865 206f 7264 6572 206f 6620  r: the order of 
-00013480: 7468 6520 6368 6172 7420 696e 2074 6865  the chart in the
-00013490: 2064 6173 6862 6f61 7264 0a20 2020 2020   dashboard.     
-000134a0: 2020 203a 7061 7261 6d20 7265 706f 7274     :param report
-000134b0: 5f70 6172 616d 733a 2061 6464 6974 696f  _params: additio
-000134c0: 6e61 6c20 7265 706f 7274 2070 6172 616d  nal report param
-000134d0: 6574 6572 7320 6173 206b 6579 2d76 616c  eters as key-val
-000134e0: 7565 2070 6169 7273 0a20 2020 2020 2020  ue pairs.       
-000134f0: 2022 2222 0a20 2020 2020 2020 2073 656c   """.        sel
-00013500: 662e 5f61 7070 6c79 5f76 6172 6961 6e74  f._apply_variant
-00013510: 2865 6368 6172 745f 6f70 7469 6f6e 732c  (echart_options,
-00013520: 2076 6172 6961 6e74 290a 2020 2020 2020   variant).      
-00013530: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
-00013540: 6178 6573 2c20 7374 7229 3a0a 2020 2020  axes, str):.    
-00013550: 2020 2020 2020 2020 6178 6573 203d 205b          axes = [
-00013560: 6178 6573 5d0a 2020 2020 2020 2020 6966  axes].        if
-00013570: 2069 7369 6e73 7461 6e63 6528 7661 6c75   isinstance(valu
-00013580: 6573 2c20 7374 7229 206f 7220 6973 696e  es, str) or isin
-00013590: 7374 616e 6365 2876 616c 7565 732c 2074  stance(values, t
-000135a0: 7570 6c65 293a 0a20 2020 2020 2020 2020  uple):.         
-000135b0: 2020 2076 616c 7565 7320 3d20 5b76 616c     values = [val
-000135c0: 7565 735d 0a20 2020 2020 2020 2069 6620  ues].        if 
-000135d0: 7368 6f77 5f76 616c 7565 7320 6973 204e  show_values is N
-000135e0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000135f0: 2073 686f 775f 7661 6c75 6573 203d 205b   show_values = [
-00013600: 5d0a 0a20 2020 2020 2020 2069 6620 2278  ]..        if "x
-00013610: 5f61 7869 735f 6e61 6d65 2220 696e 2072  _axis_name" in r
-00013620: 6570 6f72 745f 7061 7261 6d73 3a0a 2020  eport_params:.  
-00013630: 2020 2020 2020 2020 2020 785f 6178 6973            x_axis
-00013640: 5f6e 616d 6573 203d 205b 7265 706f 7274  _names = [report
-00013650: 5f70 6172 616d 735b 2278 5f61 7869 735f  _params["x_axis_
-00013660: 6e61 6d65 225d 5d0a 2020 2020 2020 2020  name"]].        
-00013670: 656c 6966 2069 7369 6e73 7461 6e63 6528  elif isinstance(
-00013680: 785f 6178 6973 5f6e 616d 6573 2c20 7374  x_axis_names, st
-00013690: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
-000136a0: 785f 6178 6973 5f6e 616d 6573 203d 205b  x_axis_names = [
-000136b0: 785f 6178 6973 5f6e 616d 6573 5d0a 2020  x_axis_names].  
-000136c0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-000136d0: 2020 2020 2020 2020 785f 6178 6973 5f6e          x_axis_n
-000136e0: 616d 6573 203d 205b 5d0a 0a20 2020 2020  ames = []..     
-000136f0: 2020 2069 6620 2279 5f61 7869 735f 6e61     if "y_axis_na
-00013700: 6d65 2220 696e 2072 6570 6f72 745f 7061  me" in report_pa
-00013710: 7261 6d73 3a0a 2020 2020 2020 2020 2020  rams:.          
-00013720: 2020 795f 6178 6973 5f6e 616d 6573 203d    y_axis_names =
-00013730: 205b 7265 706f 7274 5f70 6172 616d 735b   [report_params[
-00013740: 2279 5f61 7869 735f 6e61 6d65 225d 5d0a  "y_axis_name"]].
-00013750: 2020 2020 2020 2020 656c 6966 2069 7369          elif isi
-00013760: 6e73 7461 6e63 6528 795f 6178 6973 5f6e  nstance(y_axis_n
-00013770: 616d 6573 2c20 7374 7229 3a0a 2020 2020  ames, str):.    
-00013780: 2020 2020 2020 2020 795f 6178 6973 5f6e          y_axis_n
-00013790: 616d 6573 203d 205b 795f 6178 6973 5f6e  ames = [y_axis_n
-000137a0: 616d 6573 5d0a 2020 2020 2020 2020 656c  ames].        el
-000137b0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-000137c0: 795f 6178 6973 5f6e 616d 6573 203d 205b  y_axis_names = [
-000137d0: 5d0a 0a20 2020 2020 2020 2076 616c 7565  ]..        value
-000137e0: 7320 3d20 280a 2020 2020 2020 2020 2020  s = (.          
-000137f0: 2020 5b76 2066 6f72 2076 2069 6e20 6461    [v for v in da
-00013800: 7461 5f6d 6170 7069 6e67 5f74 6f5f 7475  ta_mapping_to_tu
-00013810: 706c 6573 2e6b 6579 7328 2920 6966 2076  ples.keys() if v
-00013820: 206e 6f74 2069 6e20 6178 6573 5d0a 2020   not in axes].  
-00013830: 2020 2020 2020 2020 2020 6966 2076 616c            if val
-00013840: 7565 7320 6973 204e 6f6e 650a 2020 2020  ues is None.    
-00013850: 2020 2020 2020 2020 656c 7365 2076 616c          else val
-00013860: 7565 730a 2020 2020 2020 2020 290a 2020  ues.        ).  
-00013870: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
-00013880: 6e63 6528 7365 7269 6573 5f6f 7074 696f  nce(series_optio
-00013890: 6e73 2c20 6469 6374 293a 0a20 2020 2020  ns, dict):.     
-000138a0: 2020 2020 2020 2073 6572 6965 735f 6f70         series_op
-000138b0: 7469 6f6e 7320 3d20 5b73 6572 6965 735f  tions = [series_
-000138c0: 6f70 7469 6f6e 735d 202a 206c 656e 2876  options] * len(v
-000138d0: 616c 7565 7329 0a20 2020 2020 2020 2065  alues).        e
-000138e0: 6c69 6620 6c65 6e28 7365 7269 6573 5f6f  lif len(series_o
-000138f0: 7074 696f 6e73 2920 3c20 6c65 6e28 7661  ptions) < len(va
-00013900: 6c75 6573 293a 0a20 2020 2020 2020 2020  lues):.         
-00013910: 2020 2073 6572 6965 735f 6f70 7469 6f6e     series_option
-00013920: 7320 3d20 7365 7269 6573 5f6f 7074 696f  s = series_optio
-00013930: 6e73 202b 205b 7365 7269 6573 5f6f 7074  ns + [series_opt
-00013940: 696f 6e73 5b2d 315d 5d20 2a20 280a 2020  ions[-1]] * (.  
-00013950: 2020 2020 2020 2020 2020 2020 2020 6c65                le
-00013960: 6e28 7661 6c75 6573 2920 2d20 6c65 6e28  n(values) - len(
-00013970: 7365 7269 6573 5f6f 7074 696f 6e73 290a  series_options).
-00013980: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00013990: 2020 2020 2020 656c 6966 206c 656e 2873        elif len(s
-000139a0: 6572 6965 735f 6f70 7469 6f6e 7329 203e  eries_options) >
-000139b0: 206c 656e 2876 616c 7565 7329 3a0a 2020   len(values):.  
-000139c0: 2020 2020 2020 2020 2020 7365 7269 6573            series
-000139d0: 5f6f 7074 696f 6e73 203d 2073 6572 6965  _options = serie
-000139e0: 735f 6f70 7469 6f6e 735b 3a20 6c65 6e28  s_options[: len(
-000139f0: 7661 6c75 6573 295d 0a0a 2020 2020 2020  values)]..      
-00013a00: 2020 6563 6861 7274 5f6f 7074 696f 6e73    echart_options
-00013a10: 5b22 7365 7269 6573 225d 203d 205b 0a20  ["series"] = [. 
-00013a20: 2020 2020 2020 2020 2020 2064 6565 705f             deep_
-00013a30: 7570 6461 7465 280a 2020 2020 2020 2020  update(.        
-00013a40: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
-00013a50: 2020 2020 2020 2020 2020 2020 2020 226e                "n
-00013a60: 616d 6522 3a20 6e61 6d65 2069 6620 6973  ame": name if is
-00013a70: 696e 7374 616e 6365 286e 616d 652c 2073  instance(name, s
-00013a80: 7472 2920 656c 7365 2022 20c3 9720 222e  tr) else " .. ".
-00013a90: 6a6f 696e 286e 616d 6529 2c0a 2020 2020  join(name),.    
-00013aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013ab0: 226c 6162 656c 223a 207b 2273 686f 7722  "label": {"show"
-00013ac0: 3a20 7368 6f77 5f76 616c 7565 7320 3d3d  : show_values ==
-00013ad0: 2022 616c 6c22 206f 7220 6e61 6d65 2069   "all" or name i
-00013ae0: 6e20 7368 6f77 5f76 616c 7565 737d 2c0a  n show_values},.
-00013af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013b00: 7d2c 0a20 2020 2020 2020 2020 2020 2020  },.             
-00013b10: 2020 2073 6572 6965 735f 6f70 7469 6f6e     series_option
-00013b20: 735b 695d 2c0a 2020 2020 2020 2020 2020  s[i],.          
-00013b30: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-00013b40: 666f 7220 692c 206e 616d 6520 696e 2065  for i, name in e
-00013b50: 6e75 6d65 7261 7465 2876 616c 7565 7329  numerate(values)
-00013b60: 0a20 2020 2020 2020 205d 0a0a 2020 2020  .        ]..    
-00013b70: 2020 2020 666f 7220 692c 2061 7869 735f      for i, axis_
-00013b80: 6f70 7469 6f6e 7320 696e 2065 6e75 6d65  options in enume
-00013b90: 7261 7465 2865 6368 6172 745f 6f70 7469  rate(echart_opti
-00013ba0: 6f6e 735b 2278 4178 6973 225d 293a 0a20  ons["xAxis"]):. 
-00013bb0: 2020 2020 2020 2020 2020 2061 7869 735f             axis_
-00013bc0: 6f70 7469 6f6e 735b 226e 616d 6522 5d20  options["name"] 
-00013bd0: 3d20 785f 6178 6973 5f6e 616d 6573 5b69  = x_axis_names[i
-00013be0: 5d20 6966 2069 203c 206c 656e 2878 5f61  ] if i < len(x_a
-00013bf0: 7869 735f 6e61 6d65 7329 2065 6c73 6520  xis_names) else 
-00013c00: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
-00013c10: 2069 6620 6178 6973 5f6f 7074 696f 6e73   if axis_options
-00013c20: 5b22 6e61 6d65 225d 2061 6e64 2022 6e61  ["name"] and "na
-00013c30: 6d65 4761 7022 206e 6f74 2069 6e20 6178  meGap" not in ax
-00013c40: 6973 5f6f 7074 696f 6e73 3a0a 2020 2020  is_options:.    
-00013c50: 2020 2020 2020 2020 2020 2020 6178 6973              axis
-00013c60: 5f6f 7074 696f 6e73 5b22 6e61 6d65 4761  _options["nameGa
-00013c70: 7022 5d20 3d20 3332 0a0a 2020 2020 2020  p"] = 32..      
-00013c80: 2020 666f 7220 692c 2061 7869 735f 6f70    for i, axis_op
-00013c90: 7469 6f6e 7320 696e 2065 6e75 6d65 7261  tions in enumera
-00013ca0: 7465 2865 6368 6172 745f 6f70 7469 6f6e  te(echart_option
-00013cb0: 735b 2279 4178 6973 225d 293a 0a20 2020  s["yAxis"]):.   
-00013cc0: 2020 2020 2020 2020 2061 7869 735f 6f70           axis_op
-00013cd0: 7469 6f6e 735b 226e 616d 6522 5d20 3d20  tions["name"] = 
-00013ce0: 795f 6178 6973 5f6e 616d 6573 5b69 5d20  y_axis_names[i] 
-00013cf0: 6966 2069 203c 206c 656e 2879 5f61 7869  if i < len(y_axi
-00013d00: 735f 6e61 6d65 7329 2065 6c73 6520 4e6f  s_names) else No
-00013d10: 6e65 0a20 2020 2020 2020 2020 2020 2069  ne.            i
-00013d20: 6620 6178 6973 5f6f 7074 696f 6e73 5b22  f axis_options["
-00013d30: 6e61 6d65 225d 2061 6e64 2022 6e61 6d65  name"] and "name
-00013d40: 4761 7022 206e 6f74 2069 6e20 6178 6973  Gap" not in axis
-00013d50: 5f6f 7074 696f 6e73 3a0a 2020 2020 2020  _options:.      
-00013d60: 2020 2020 2020 2020 2020 6178 6973 5f6f            axis_o
-00013d70: 7074 696f 6e73 5b22 6e61 6d65 4761 7022  ptions["nameGap"
-00013d80: 5d20 3d20 2d32 340a 2020 2020 2020 2020  ] = -24.        
-00013d90: 2020 2020 2020 2020 6178 6973 5f6f 7074          axis_opt
-00013da0: 696f 6e73 5b22 6f66 6673 6574 225d 203d  ions["offset"] =
-00013db0: 2033 360a 2020 2020 2020 2020 2020 2020   36.            
-00013dc0: 2020 2020 6563 6861 7274 5f6f 7074 696f      echart_optio
-00013dd0: 6e73 5b22 6772 6964 225d 5b22 6c65 6674  ns["grid"]["left
-00013de0: 225d 203d 2022 3425 220a 2020 2020 2020  "] = "4%".      
-00013df0: 2020 2020 2020 2020 2020 6178 6973 5f6f            axis_o
-00013e00: 7074 696f 6e73 5b22 6178 6973 5469 636b  ptions["axisTick
-00013e10: 225d 203d 207b 2273 686f 7722 3a20 4661  "] = {"show": Fa
-00013e20: 6c73 657d 0a20 2020 2020 2020 2020 2020  lse}.           
-00013e30: 2020 2020 2061 7869 735f 6f70 7469 6f6e       axis_option
-00013e40: 735b 2261 7869 734c 696e 6522 5d20 3d20  s["axisLine"] = 
-00013e50: 7b22 7368 6f77 223a 2046 616c 7365 7d0a  {"show": False}.
-00013e60: 0a20 2020 2020 2020 2061 7761 6974 2073  .        await s
-00013e70: 656c 662e 5f63 7265 6174 655f 6563 6861  elf._create_echa
-00013e80: 7274 280a 2020 2020 2020 2020 2020 2020  rt(.            
-00013e90: 6f72 6465 723d 6f72 6465 722c 0a20 2020  order=order,.   
-00013ea0: 2020 2020 2020 2020 206f 7074 696f 6e73           options
-00013eb0: 3d65 6368 6172 745f 6f70 7469 6f6e 732c  =echart_options,
-00013ec0: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
-00013ed0: 615f 6d61 7070 696e 675f 746f 5f74 7570  a_mapping_to_tup
-00013ee0: 6c65 733d 6461 7461 5f6d 6170 7069 6e67  les=data_mapping
-00013ef0: 5f74 6f5f 7475 706c 6573 2c0a 2020 2020  _to_tuples,.    
-00013f00: 2020 2020 2020 2020 6669 656c 6473 3d61          fields=a
-00013f10: 7865 7320 2b20 7661 6c75 6573 2c0a 2020  xes + values,.  
-00013f20: 2020 2020 2020 2020 2020 2a2a 7265 706f            **repo
-00013f30: 7274 5f70 6172 616d 732c 0a20 2020 2020  rt_params,.     
-00013f40: 2020 2029 0a0a 2020 2020 4061 6464 5f74     )..    @add_t
-00013f50: 6f5f 6765 6e65 7261 6c5f 6173 796e 635f  o_general_async_
-00013f60: 6772 6f75 700a 2020 2020 6173 796e 6320  group.    async 
-00013f70: 6465 6620 6672 6565 5f65 6368 6172 7473  def free_echarts
-00013f80: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-00013f90: 2020 2020 2020 2020 6461 7461 3a20 4f70          data: Op
-00013fa0: 7469 6f6e 616c 5b55 6e69 6f6e 5b73 7472  tional[Union[str
-00013fb0: 2c20 4461 7461 4672 616d 652c 206c 6973  , DataFrame, lis
-00013fc0: 745b 6469 6374 5d5d 5d20 3d20 4e6f 6e65  t[dict]]] = None
-00013fd0: 2c0a 2020 2020 2020 2020 6f70 7469 6f6e  ,.        option
-00013fe0: 733a 204f 7074 696f 6e61 6c5b 6469 6374  s: Optional[dict
-00013ff0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-00014000: 2020 7261 775f 6f70 7469 6f6e 733a 204f    raw_options: O
-00014010: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
-00014020: 6f6e 652c 0a20 2020 2020 2020 206f 7264  one,.        ord
-00014030: 6572 3a20 4f70 7469 6f6e 616c 5b69 6e74  er: Optional[int
-00014040: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-00014050: 2020 7469 746c 653a 204f 7074 696f 6e61    title: Optiona
-00014060: 6c5b 7374 725d 203d 204e 6f6e 652c 0a20  l[str] = None,. 
-00014070: 2020 2020 2020 2072 6f77 735f 7369 7a65         rows_size
-00014080: 3a20 4f70 7469 6f6e 616c 5b69 6e74 5d20  : Optional[int] 
-00014090: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-000140a0: 636f 6c73 5f73 697a 653a 204f 7074 696f  cols_size: Optio
-000140b0: 6e61 6c5b 696e 745d 203d 204e 6f6e 652c  nal[int] = None,
-000140c0: 0a20 2020 2020 2020 2070 6164 6469 6e67  .        padding
-000140d0: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
-000140e0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-000140f0: 6669 656c 6473 3a20 4f70 7469 6f6e 616c  fields: Optional
-00014100: 5b6c 6973 745d 203d 204e 6f6e 652c 0a20  [list] = None,. 
-00014110: 2020 2020 2020 2064 6174 615f 6973 5f6e         data_is_n
-00014120: 6f74 5f64 663a 2062 6f6f 6c20 3d20 4661  ot_df: bool = Fa
-00014130: 6c73 652c 0a20 2020 2029 3a0a 2020 2020  lse,.    ):.    
-00014140: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00014150: 4372 6561 7465 2061 6e20 6563 6861 7274  Create an echart
-00014160: 7320 6368 6172 7420 7769 7468 2063 7573  s chart with cus
-00014170: 746f 6d20 6f70 7469 6f6e 732e 0a20 2020  tom options..   
-00014180: 2020 2020 203a 7061 7261 6d20 6461 7461       :param data
-00014190: 3a20 7468 6520 6461 7461 206f 6620 7468  : the data of th
-000141a0: 6520 6368 6172 740a 2020 2020 2020 2020  e chart.        
-000141b0: 3a70 6172 616d 206f 7074 696f 6e73 3a20  :param options: 
-000141c0: 7468 6520 6f70 7469 6f6e 7320 6f66 2074  the options of t
-000141d0: 6865 2063 6861 7274 0a20 2020 2020 2020  he chart.       
-000141e0: 203a 7061 7261 6d20 7261 775f 6f70 7469   :param raw_opti
-000141f0: 6f6e 733a 2074 6865 2072 6177 206f 7074  ons: the raw opt
-00014200: 696f 6e73 206f 6620 7468 6520 6368 6172  ions of the char
-00014210: 740a 2020 2020 2020 2020 3a70 6172 616d  t.        :param
-00014220: 206f 7264 6572 3a20 7468 6520 6f72 6465   order: the orde
-00014230: 7220 6f66 2074 6865 2063 6861 7274 2069  r of the chart i
-00014240: 6e20 7468 6520 6461 7368 626f 6172 640a  n the dashboard.
-00014250: 2020 2020 2020 2020 3a70 6172 616d 2074          :param t
-00014260: 6974 6c65 3a20 7468 6520 7469 746c 6520  itle: the title 
-00014270: 6f66 2074 6865 2063 6861 7274 0a20 2020  of the chart.   
-00014280: 2020 2020 203a 7061 7261 6d20 726f 7773       :param rows
-00014290: 5f73 697a 653a 2074 6865 2072 6f77 7320  _size: the rows 
-000142a0: 7369 7a65 206f 6620 7468 6520 6368 6172  size of the char
-000142b0: 740a 2020 2020 2020 2020 3a70 6172 616d  t.        :param
-000142c0: 2063 6f6c 735f 7369 7a65 3a20 7468 6520   cols_size: the 
-000142d0: 636f 6c75 6d6e 7320 7369 7a65 206f 6620  columns size of 
-000142e0: 7468 6520 6368 6172 740a 2020 2020 2020  the chart.      
-000142f0: 2020 3a70 6172 616d 2070 6164 6469 6e67    :param padding
-00014300: 3a20 7468 6520 7061 6464 696e 6720 6f66  : the padding of
-00014310: 2074 6865 2063 6861 7274 0a20 2020 2020   the chart.     
-00014320: 2020 203a 7061 7261 6d20 6669 656c 6473     :param fields
-00014330: 3a20 7468 6520 6669 656c 6473 206f 6620  : the fields of 
-00014340: 7468 6520 6368 6172 740a 2020 2020 2020  the chart.      
-00014350: 2020 3a70 6172 616d 2064 6174 615f 6973    :param data_is
-00014360: 5f6e 6f74 5f64 663a 2077 6865 7468 6572  _not_df: whether
-00014370: 2074 6865 2064 6174 6120 6973 206e 6f74   the data is not
-00014380: 2061 2064 6174 6166 7261 6d65 0a20 2020   a dataframe.   
-00014390: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-000143a0: 2069 6620 6e6f 7420 6f70 7469 6f6e 7320   if not options 
-000143b0: 616e 6420 6e6f 7420 7261 775f 6f70 7469  and not raw_opti
-000143c0: 6f6e 733a 0a20 2020 2020 2020 2020 2020  ons:.           
-000143d0: 206c 6f67 5f65 7272 6f72 280a 2020 2020   log_error(.    
-000143e0: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
-000143f0: 6572 2c20 2245 6974 6865 7220 6f70 7469  er, "Either opti
-00014400: 6f6e 7320 6f72 2072 6177 5f6f 7074 696f  ons or raw_optio
-00014410: 6e73 206d 7573 7420 6265 2070 726f 7669  ns must be provi
-00014420: 6465 6422 2c20 5661 6c75 6545 7272 6f72  ded", ValueError
-00014430: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-00014440: 2020 2020 2020 2069 6620 6f70 7469 6f6e         if option
-00014450: 7320 616e 6420 6e6f 7420 6973 696e 7374  s and not isinst
-00014460: 616e 6365 2864 6174 612c 2044 6174 6146  ance(data, DataF
-00014470: 7261 6d65 2920 616e 6420 6461 7461 2069  rame) and data i
-00014480: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-00014490: 2020 2020 6c6f 675f 6572 726f 7228 0a20      log_error(. 
-000144a0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-000144b0: 6f67 6765 722c 2022 6461 7461 206d 7573  ogger, "data mus
-000144c0: 7420 6265 2070 726f 7669 6465 6420 7768  t be provided wh
-000144d0: 656e 206f 7074 696f 6e73 2069 7320 7072  en options is pr
-000144e0: 6f76 6964 6564 222c 2044 6174 6145 7272  ovided", DataErr
-000144f0: 6f72 0a20 2020 2020 2020 2020 2020 2029  or.            )
-00014500: 0a20 2020 2020 2020 2069 6620 6f70 7469  .        if opti
-00014510: 6f6e 7320 616e 6420 7261 775f 6f70 7469  ons and raw_opti
-00014520: 6f6e 733a 0a20 2020 2020 2020 2020 2020  ons:.           
-00014530: 206c 6f67 5f65 7272 6f72 280a 2020 2020   log_error(.    
-00014540: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
-00014550: 6572 2c0a 2020 2020 2020 2020 2020 2020  er,.            
-00014560: 2020 2020 224f 6e6c 7920 6f6e 6520 6f66      "Only one of
-00014570: 206f 7074 696f 6e73 2061 6e64 2072 6177   options and raw
-00014580: 5f6f 7074 696f 6e73 2063 616e 2062 6520  _options can be 
-00014590: 7072 6f76 6964 6564 222c 0a20 2020 2020  provided",.     
-000145a0: 2020 2020 2020 2020 2020 2056 616c 7565             Value
-000145b0: 4572 726f 722c 0a20 2020 2020 2020 2020  Error,.         
-000145c0: 2020 2029 0a0a 2020 2020 2020 2020 6966     )..        if
-000145d0: 2072 6177 5f6f 7074 696f 6e73 3a0a 2020   raw_options:.  
-000145e0: 2020 2020 2020 2020 2020 6f70 7469 6f6e            option
-000145f0: 7320 3d20 7472 616e 7366 6f72 6d5f 6469  s = transform_di
-00014600: 6374 5f6a 735f 746f 5f70 7928 7261 775f  ct_js_to_py(raw_
-00014610: 6f70 7469 6f6e 7329 0a20 2020 2020 2020  options).       
-00014620: 2020 2020 2064 6174 6120 3d20 7265 7472       data = retr
-00014630: 6965 7665 5f64 6174 615f 6672 6f6d 5f6f  ieve_data_from_o
-00014640: 7074 696f 6e73 286f 7074 696f 6e73 290a  ptions(options).
-00014650: 2020 2020 2020 2020 2020 2020 6f70 7469              opti
-00014660: 6f6e 735b 2264 6174 6173 6574 225d 203d  ons["dataset"] =
-00014670: 207b 2273 6f75 7263 6522 3a20 2223 7365   {"source": "#se
-00014680: 745f 6461 7461 2322 7d0a 2020 2020 2020  t_data#"}.      
-00014690: 2020 2020 2020 6669 656c 6473 203d 205b        fields = [
-000146a0: 6c69 7374 2864 6174 615b 305d 2e6b 6579  list(data[0].key
-000146b0: 7328 2929 5d0a 2020 2020 2020 2020 656c  s())].        el
-000146c0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-000146d0: 6f70 7469 6f6e 7320 3d20 6465 6570 636f  options = deepco
-000146e0: 7079 286f 7074 696f 6e73 290a 0a20 2020  py(options)..   
-000146f0: 2020 2020 2061 7761 6974 2073 656c 662e       await self.
-00014700: 5f63 7265 6174 655f 6563 6861 7274 280a  _create_echart(.
-00014710: 2020 2020 2020 2020 2020 2020 6f72 6465              orde
-00014720: 723d 6f72 6465 722c 0a20 2020 2020 2020  r=order,.       
-00014730: 2020 2020 2064 6174 615f 6d61 7070 696e       data_mappin
-00014740: 675f 746f 5f74 7570 6c65 733d 6177 6169  g_to_tuples=awai
-00014750: 7420 7365 6c66 2e5f 6368 6f6f 7365 5f64  t self._choose_d
-00014760: 6174 6128 0a20 2020 2020 2020 2020 2020  ata(.           
-00014770: 2020 2020 206f 7264 6572 2c20 6461 7461       order, data
-00014780: 2c20 6475 6d70 5f77 686f 6c65 3d64 6174  , dump_whole=dat
-00014790: 615f 6973 5f6e 6f74 5f64 660a 2020 2020  a_is_not_df.    
-000147a0: 2020 2020 2020 2020 292c 0a20 2020 2020          ),.     
-000147b0: 2020 2020 2020 2066 6965 6c64 733d 6669         fields=fi
-000147c0: 656c 6473 2c0a 2020 2020 2020 2020 2020  elds,.          
-000147d0: 2020 6f70 7469 6f6e 733d 6f70 7469 6f6e    options=option
-000147e0: 732c 0a20 2020 2020 2020 2020 2020 2074  s,.            t
-000147f0: 6974 6c65 3d74 6974 6c65 2c0a 2020 2020  itle=title,.    
-00014800: 2020 2020 2020 2020 726f 7773 5f73 697a          rows_siz
-00014810: 653d 726f 7773 5f73 697a 652c 0a20 2020  e=rows_size,.   
-00014820: 2020 2020 2020 2020 2063 6f6c 735f 7369           cols_si
-00014830: 7a65 3d63 6f6c 735f 7369 7a65 2c0a 2020  ze=cols_size,.  
-00014840: 2020 2020 2020 2020 2020 7061 6464 696e            paddin
-00014850: 673d 7061 6464 696e 672c 0a20 2020 2020  g=padding,.     
-00014860: 2020 2029 0a0a 2020 2020 2320 4543 6861     )..    # ECha
-00014870: 7274 730a 2020 2020 6c69 6e65 203d 2061  rts.    line = a
-00014880: 6464 5f74 6f5f 6765 6e65 7261 6c5f 6173  dd_to_general_as
-00014890: 796e 635f 6772 6f75 7028 6c69 6e65 5f63  ync_group(line_c
-000148a0: 6861 7274 290a 2020 2020 6261 7220 3d20  hart).    bar = 
-000148b0: 6164 645f 746f 5f67 656e 6572 616c 5f61  add_to_general_a
-000148c0: 7379 6e63 5f67 726f 7570 2862 6172 5f63  sync_group(bar_c
-000148d0: 6861 7274 290a 2020 2020 7374 6163 6b65  hart).    stacke
-000148e0: 645f 6261 7220 3d20 6164 645f 746f 5f67  d_bar = add_to_g
-000148f0: 656e 6572 616c 5f61 7379 6e63 5f67 726f  eneral_async_gro
-00014900: 7570 2873 7461 636b 6564 5f62 6172 5f63  up(stacked_bar_c
-00014910: 6861 7274 290a 2020 2020 6172 6561 203d  hart).    area =
-00014920: 2061 6464 5f74 6f5f 6765 6e65 7261 6c5f   add_to_general_
-00014930: 6173 796e 635f 6772 6f75 7028 6172 6561  async_group(area
-00014940: 5f63 6861 7274 290a 2020 2020 7374 6163  _chart).    stac
-00014950: 6b65 645f 6172 6561 203d 2061 6464 5f74  ked_area = add_t
-00014960: 6f5f 6765 6e65 7261 6c5f 6173 796e 635f  o_general_async_
-00014970: 6772 6f75 7028 7374 6163 6b65 645f 6172  group(stacked_ar
-00014980: 6561 5f63 6861 7274 290a 2020 2020 7363  ea_chart).    sc
-00014990: 6174 7465 7220 3d20 6164 645f 746f 5f67  atter = add_to_g
-000149a0: 656e 6572 616c 5f61 7379 6e63 5f67 726f  eneral_async_gro
-000149b0: 7570 2873 6361 7474 6572 5f63 6861 7274  up(scatter_chart
-000149c0: 290a 2020 2020 686f 7269 7a6f 6e74 616c  ).    horizontal
-000149d0: 5f62 6172 203d 2061 6464 5f74 6f5f 6765  _bar = add_to_ge
-000149e0: 6e65 7261 6c5f 6173 796e 635f 6772 6f75  neral_async_grou
-000149f0: 7028 686f 7269 7a6f 6e74 616c 5f62 6172  p(horizontal_bar
-00014a00: 5f63 6861 7274 290a 2020 2020 7374 6163  _chart).    stac
-00014a10: 6b65 645f 686f 7269 7a6f 6e74 616c 5f62  ked_horizontal_b
-00014a20: 6172 203d 2061 6464 5f74 6f5f 6765 6e65  ar = add_to_gene
-00014a30: 7261 6c5f 6173 796e 635f 6772 6f75 7028  ral_async_group(
-00014a40: 7374 6163 6b65 645f 686f 7269 7a6f 6e74  stacked_horizont
-00014a50: 616c 5f62 6172 5f63 6861 7274 290a 2020  al_bar_chart).  
-00014a60: 2020 7a65 726f 5f63 656e 7465 7265 645f    zero_centered_
-00014a70: 6261 7220 3d20 6164 645f 746f 5f67 656e  bar = add_to_gen
-00014a80: 6572 616c 5f61 7379 6e63 5f67 726f 7570  eral_async_group
-00014a90: 287a 6572 6f5f 6365 6e74 6572 6564 5f62  (zero_centered_b
-00014aa0: 6172 5f63 6861 7274 290a 2020 2020 6675  ar_chart).    fu
-00014ab0: 6e6e 656c 203d 2061 6464 5f74 6f5f 6765  nnel = add_to_ge
-00014ac0: 6e65 7261 6c5f 6173 796e 635f 6772 6f75  neral_async_grou
-00014ad0: 7028 6675 6e6e 656c 5f63 6861 7274 290a  p(funnel_chart).
-00014ae0: 2020 2020 7472 6565 203d 2061 6464 5f74      tree = add_t
-00014af0: 6f5f 6765 6e65 7261 6c5f 6173 796e 635f  o_general_async_
-00014b00: 6772 6f75 7028 7472 6565 5f63 6861 7274  group(tree_chart
-00014b10: 290a 2020 2020 7261 6461 7220 3d20 6164  ).    radar = ad
-00014b20: 645f 746f 5f67 656e 6572 616c 5f61 7379  d_to_general_asy
-00014b30: 6e63 5f67 726f 7570 2872 6164 6172 5f63  nc_group(radar_c
-00014b40: 6861 7274 290a 2020 2020 7069 6520 3d20  hart).    pie = 
-00014b50: 6164 645f 746f 5f67 656e 6572 616c 5f61  add_to_general_a
-00014b60: 7379 6e63 5f67 726f 7570 2870 6965 5f63  sync_group(pie_c
-00014b70: 6861 7274 290a 2020 2020 646f 7567 686e  hart).    doughn
-00014b80: 7574 203d 2061 6464 5f74 6f5f 6765 6e65  ut = add_to_gene
-00014b90: 7261 6c5f 6173 796e 635f 6772 6f75 7028  ral_async_group(
-00014ba0: 646f 7567 686e 7574 5f63 6861 7274 290a  doughnut_chart).
-00014bb0: 2020 2020 726f 7365 203d 2061 6464 5f74      rose = add_t
-00014bc0: 6f5f 6765 6e65 7261 6c5f 6173 796e 635f  o_general_async_
-00014bd0: 6772 6f75 7028 726f 7365 5f63 6861 7274  group(rose_chart
-00014be0: 290a 2020 2020 7375 6e62 7572 7374 203d  ).    sunburst =
-00014bf0: 2061 6464 5f74 6f5f 6765 6e65 7261 6c5f   add_to_general_
-00014c00: 6173 796e 635f 6772 6f75 7028 7375 6e62  async_group(sunb
-00014c10: 7572 7374 5f63 6861 7274 290a 2020 2020  urst_chart).    
-00014c20: 7472 6565 6d61 7020 3d20 6164 645f 746f  treemap = add_to
-00014c30: 5f67 656e 6572 616c 5f61 7379 6e63 5f67  _general_async_g
-00014c40: 726f 7570 2874 7265 656d 6170 5f63 6861  roup(treemap_cha
-00014c50: 7274 290a 2020 2020 7361 6e6b 6579 203d  rt).    sankey =
-00014c60: 2061 6464 5f74 6f5f 6765 6e65 7261 6c5f   add_to_general_
-00014c70: 6173 796e 635f 6772 6f75 7028 7361 6e6b  async_group(sank
-00014c80: 6579 5f63 6861 7274 290a 2020 2020 6865  ey_chart).    he
-00014c90: 6174 6d61 7020 3d20 6164 645f 746f 5f67  atmap = add_to_g
-00014ca0: 656e 6572 616c 5f61 7379 6e63 5f67 726f  eneral_async_gro
-00014cb0: 7570 2868 6561 746d 6170 5f63 6861 7274  up(heatmap_chart
-00014cc0: 290a 2020 2020 7072 6564 6963 7469 7665  ).    predictive
-00014cd0: 5f6c 696e 6520 3d20 6164 645f 746f 5f67  _line = add_to_g
-00014ce0: 656e 6572 616c 5f61 7379 6e63 5f67 726f  eneral_async_gro
-00014cf0: 7570 2870 7265 6469 6374 6976 655f 6c69  up(predictive_li
-00014d00: 6e65 5f63 6861 7274 290a 2020 2020 7370  ne_chart).    sp
-00014d10: 6565 645f 6761 7567 6520 3d20 6164 645f  eed_gauge = add_
-00014d20: 746f 5f67 656e 6572 616c 5f61 7379 6e63  to_general_async
-00014d30: 5f67 726f 7570 2873 7065 6564 5f67 6175  _group(speed_gau
-00014d40: 6765 5f63 6861 7274 290a 2020 2020 7368  ge_chart).    sh
-00014d50: 696d 6f6b 755f 6761 7567 6520 3d20 6164  imoku_gauge = ad
-00014d60: 645f 746f 5f67 656e 6572 616c 5f61 7379  d_to_general_asy
-00014d70: 6e63 5f67 726f 7570 2873 6869 6d6f 6b75  nc_group(shimoku
-00014d80: 5f67 6175 6765 5f63 6861 7274 290a 2020  _gauge_chart).  
-00014d90: 2020 7368 696d 6f6b 755f 6761 7567 6573    shimoku_gauges
-00014da0: 5f67 726f 7570 203d 2061 6464 5f74 6f5f  _group = add_to_
-00014db0: 6765 6e65 7261 6c5f 6173 796e 635f 6772  general_async_gr
-00014dc0: 6f75 7028 7368 696d 6f6b 755f 6761 7567  oup(shimoku_gaug
-00014dd0: 6573 5f67 726f 7570 290a 2020 2020 6761  es_group).    ga
-00014de0: 7567 655f 696e 6469 6361 746f 7220 3d20  uge_indicator = 
-00014df0: 6164 645f 746f 5f67 656e 6572 616c 5f61  add_to_general_a
-00014e00: 7379 6e63 5f67 726f 7570 2867 6175 6765  sync_group(gauge
-00014e10: 5f69 6e64 6963 6174 6f72 290a 2020 2020  _indicator).    
-00014e20: 746f 705f 626f 7474 6f6d 5f61 7265 6120  top_bottom_area 
-00014e30: 3d20 6164 645f 746f 5f67 656e 6572 616c  = add_to_general
-00014e40: 5f61 7379 6e63 5f67 726f 7570 2874 6f70  _async_group(top
-00014e50: 5f62 6f74 746f 6d5f 6172 6561 5f63 6861  _bottom_area_cha
-00014e60: 7274 7329 0a20 2020 2074 6f70 5f62 6f74  rts).    top_bot
-00014e70: 746f 6d5f 6c69 6e65 203d 2061 6464 5f74  tom_line = add_t
-00014e80: 6f5f 6765 6e65 7261 6c5f 6173 796e 635f  o_general_async_
-00014e90: 6772 6f75 7028 746f 705f 626f 7474 6f6d  group(top_bottom
-00014ea0: 5f6c 696e 655f 6368 6172 7473 290a 2020  _line_charts).  
-00014eb0: 2020 6c69 6e65 5f77 6974 685f 636f 6e66    line_with_conf
-00014ec0: 6964 656e 6365 5f61 7265 6120 3d20 6164  idence_area = ad
-00014ed0: 645f 746f 5f67 656e 6572 616c 5f61 7379  d_to_general_asy
-00014ee0: 6e63 5f67 726f 7570 280a 2020 2020 2020  nc_group(.      
-00014ef0: 2020 6c69 6e65 5f77 6974 685f 636f 6e66    line_with_conf
-00014f00: 6964 656e 6365 5f61 7265 615f 6368 6172  idence_area_char
-00014f10: 740a 2020 2020 290a 2020 2020 7363 6174  t.    ).    scat
-00014f20: 7465 725f 7769 7468 5f65 6666 6563 7420  ter_with_effect 
-00014f30: 3d20 6164 645f 746f 5f67 656e 6572 616c  = add_to_general
-00014f40: 5f61 7379 6e63 5f67 726f 7570 2873 6361  _async_group(sca
-00014f50: 7474 6572 5f77 6974 685f 6566 6665 6374  tter_with_effect
-00014f60: 5f63 6861 7274 290a 2020 2020 7761 7465  _chart).    wate
-00014f70: 7266 616c 6c20 3d20 6164 645f 746f 5f67  rfall = add_to_g
-00014f80: 656e 6572 616c 5f61 7379 6e63 5f67 726f  eneral_async_gro
-00014f90: 7570 2877 6174 6572 6661 6c6c 5f63 6861  up(waterfall_cha
-00014fa0: 7274 290a 2020 2020 6c69 6e65 5f61 6e64  rt).    line_and
-00014fb0: 5f62 6172 5f63 6861 7274 7320 3d20 6164  _bar_charts = ad
-00014fc0: 645f 746f 5f67 656e 6572 616c 5f61 7379  d_to_general_asy
-00014fd0: 6e63 5f67 726f 7570 286c 696e 655f 616e  nc_group(line_an
-00014fe0: 645f 6261 725f 6368 6172 7473 290a 2020  d_bar_charts).  
-00014ff0: 2020 7365 676d 656e 7465 645f 6c69 6e65    segmented_line
-00015000: 203d 2061 6464 5f74 6f5f 6765 6e65 7261   = add_to_genera
-00015010: 6c5f 6173 796e 635f 6772 6f75 7028 7365  l_async_group(se
-00015020: 676d 656e 7465 645f 6c69 6e65 5f63 6861  gmented_line_cha
-00015030: 7274 290a 2020 2020 6d61 726b 6564 5f6c  rt).    marked_l
-00015040: 696e 6520 3d20 6164 645f 746f 5f67 656e  ine = add_to_gen
-00015050: 6572 616c 5f61 7379 6e63 5f67 726f 7570  eral_async_group
-00015060: 286d 6172 6b65 645f 6c69 6e65 5f63 6861  (marked_line_cha
-00015070: 7274 290a 2020 2020 7365 676d 656e 7465  rt).    segmente
-00015080: 645f 6172 6561 203d 2061 6464 5f74 6f5f  d_area = add_to_
-00015090: 6765 6e65 7261 6c5f 6173 796e 635f 6772  general_async_gr
-000150a0: 6f75 7028 7365 676d 656e 7465 645f 6172  oup(segmented_ar
-000150b0: 6561 5f63 6861 7274 290a 0a20 2020 2023  ea_chart)..    #
-000150c0: 2042 656e 746f 626f 7820 6368 6172 7473   Bentobox charts
-000150d0: 2064 6566 696e 6564 2069 6e20 7468 6520   defined in the 
-000150e0: 6265 6e74 6f62 6f78 5f63 6861 7274 732e  bentobox_charts.
-000150f0: 7079 2066 696c 650a 2020 2020 696e 666f  py file.    info
-00015100: 6772 6170 6869 6373 5f74 6578 745f 6275  graphics_text_bu
-00015110: 6262 6c65 203d 2061 6464 5f74 6f5f 6765  bble = add_to_ge
-00015120: 6e65 7261 6c5f 6173 796e 635f 6772 6f75  neral_async_grou
-00015130: 7028 696e 666f 6772 6170 6869 6373 5f74  p(infographics_t
-00015140: 6578 745f 6275 6262 6c65 290a 2020 2020  ext_bubble).    
-00015150: 6368 6172 745f 616e 645f 6d6f 6461 6c5f  chart_and_modal_
-00015160: 6275 7474 6f6e 203d 2061 6464 5f74 6f5f  button = add_to_
-00015170: 6765 6e65 7261 6c5f 6173 796e 635f 6772  general_async_gr
-00015180: 6f75 7028 6368 6172 745f 616e 645f 6d6f  oup(chart_and_mo
-00015190: 6461 6c5f 6275 7474 6f6e 290a 2020 2020  dal_button).    
-000151a0: 6368 6172 745f 616e 645f 696e 6469 6361  chart_and_indica
-000151b0: 746f 7273 203d 2061 6464 5f74 6f5f 6765  tors = add_to_ge
-000151c0: 6e65 7261 6c5f 6173 796e 635f 6772 6f75  neral_async_grou
-000151d0: 7028 6368 6172 745f 616e 645f 696e 6469  p(chart_and_indi
-000151e0: 6361 746f 7273 290a 2020 2020 696e 6469  cators).    indi
-000151f0: 6361 746f 7273 5f77 6974 685f 6865 6164  cators_with_head
-00015200: 6572 203d 2061 6464 5f74 6f5f 6765 6e65  er = add_to_gene
-00015210: 7261 6c5f 6173 796e 635f 6772 6f75 7028  ral_async_group(
-00015220: 696e 6469 6361 746f 7273 5f77 6974 685f  indicators_with_
-00015230: 6865 6164 6572 290a 2020 2020 6c69 6e65  header).    line
-00015240: 5f77 6974 685f 7375 6d6d 6172 7920 3d20  _with_summary = 
-00015250: 6164 645f 746f 5f67 656e 6572 616c 5f61  add_to_general_a
-00015260: 7379 6e63 5f67 726f 7570 286c 696e 655f  sync_group(line_
-00015270: 7769 7468 5f73 756d 6d61 7279 290a       with_summary).
+0000c3a0: 796e 6320 6465 6620 6163 7469 6f6e 5f62  ync def action_b
+0000c3b0: 7574 746f 6e28 0a20 2020 2020 2020 2073  utton(.        s
+0000c3c0: 656c 662c 0a20 2020 2020 2020 206c 6162  elf,.        lab
+0000c3d0: 656c 3a20 7374 722c 0a20 2020 2020 2020  el: str,.       
+0000c3e0: 206f 7264 6572 3a20 696e 742c 0a20 2020   order: int,.   
+0000c3f0: 2020 2020 2061 6374 696f 6e5f 6964 3a20       action_id: 
+0000c400: 7374 722c 0a20 2020 2020 2020 2072 6f77  str,.        row
+0000c410: 735f 7369 7a65 3a20 4f70 7469 6f6e 616c  s_size: Optional
+0000c420: 5b69 6e74 5d20 3d20 312c 0a20 2020 2020  [int] = 1,.     
+0000c430: 2020 2063 6f6c 735f 7369 7a65 3a20 696e     cols_size: in
+0000c440: 7420 3d20 322c 0a20 2020 2020 2020 2061  t = 2,.        a
+0000c450: 6c69 676e 3a20 4f70 7469 6f6e 616c 5b73  lign: Optional[s
+0000c460: 7472 5d20 3d20 2273 7472 6574 6368 222c  tr] = "stretch",
+0000c470: 0a20 2020 2020 2020 2070 6164 6469 6e67  .        padding
+0000c480: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
+0000c490: 3d20 4e6f 6e65 2c0a 2020 2020 293a 0a20  = None,.    ):. 
+0000c4a0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000c4b0: 2020 2043 7265 6174 6520 6120 6275 7474     Create a butt
+0000c4c0: 6f6e 2069 6e20 7468 6520 6461 7368 626f  on in the dashbo
+0000c4d0: 6172 6420 7468 6174 2065 7865 6375 7465  ard that execute
+0000c4e0: 7320 616e 2061 6374 696f 6e2e 0a20 2020  s an action..   
+0000c4f0: 2020 2020 203a 7061 7261 6d20 6c61 6265       :param labe
+0000c500: 6c3a 2074 6865 206c 6162 656c 206f 6620  l: the label of 
+0000c510: 7468 6520 6275 7474 6f6e 0a20 2020 2020  the button.     
+0000c520: 2020 203a 7061 7261 6d20 6f72 6465 723a     :param order:
+0000c530: 2074 6865 206f 7264 6572 206f 6620 7468   the order of th
+0000c540: 6520 6275 7474 6f6e 0a20 2020 2020 2020  e button.       
+0000c550: 203a 7061 7261 6d20 6163 7469 6f6e 5f69   :param action_i
+0000c560: 643a 2074 6865 2069 6420 6f66 2074 6865  d: the id of the
+0000c570: 2061 6374 696f 6e0a 2020 2020 2020 2020   action.        
+0000c580: 3a70 6172 616d 2072 6f77 735f 7369 7a65  :param rows_size
+0000c590: 3a20 7468 6520 7369 7a65 206f 6620 7468  : the size of th
+0000c5a0: 6520 726f 7773 2069 6e20 7468 6520 6275  e rows in the bu
+0000c5b0: 7474 6f6e 0a20 2020 2020 2020 203a 7061  tton.        :pa
+0000c5c0: 7261 6d20 636f 6c73 5f73 697a 653a 2074  ram cols_size: t
+0000c5d0: 6865 2073 697a 6520 6f66 2074 6865 2063  he size of the c
+0000c5e0: 6f6c 756d 6e73 2069 6e20 7468 6520 6275  olumns in the bu
+0000c5f0: 7474 6f6e 0a20 2020 2020 2020 203a 7061  tton.        :pa
+0000c600: 7261 6d20 616c 6967 6e3a 2074 6865 2061  ram align: the a
+0000c610: 6c69 676e 6d65 6e74 206f 6620 7468 6520  lignment of the 
+0000c620: 6275 7474 6f6e 0a20 2020 2020 2020 203a  button.        :
+0000c630: 7061 7261 6d20 7061 6464 696e 673a 2074  param padding: t
+0000c640: 6865 2070 6164 6469 6e67 206f 6620 7468  he padding of th
+0000c650: 6520 6275 7474 6f6e 0a20 2020 2020 2020  e button.       
+0000c660: 2022 2222 0a20 2020 2020 2020 2061 7761   """.        awa
+0000c670: 6974 2073 656c 662e 5f62 7574 746f 6e28  it self._button(
+0000c680: 0a20 2020 2020 2020 2020 2020 206c 6162  .            lab
+0000c690: 656c 3d6c 6162 656c 2c0a 2020 2020 2020  el=label,.      
+0000c6a0: 2020 2020 2020 6f72 6465 723d 6f72 6465        order=orde
+0000c6b0: 722c 0a20 2020 2020 2020 2020 2020 2070  r,.            p
+0000c6c0: 6164 6469 6e67 3d70 6164 6469 6e67 2c0a  adding=padding,.
+0000c6d0: 2020 2020 2020 2020 2020 2020 726f 7773              rows
+0000c6e0: 5f73 697a 653d 726f 7773 5f73 697a 652c  _size=rows_size,
+0000c6f0: 0a20 2020 2020 2020 2020 2020 2063 6f6c  .            col
+0000c700: 735f 7369 7a65 3d63 6f6c 735f 7369 7a65  s_size=cols_size
+0000c710: 2c0a 2020 2020 2020 2020 2020 2020 616c  ,.            al
+0000c720: 6967 6e3d 616c 6967 6e2c 0a20 2020 2020  ign=align,.     
+0000c730: 2020 2020 2020 206f 6e5f 636c 6963 6b5f         on_click_
+0000c740: 6576 656e 7473 3d5b 0a20 2020 2020 2020  events=[.       
+0000c750: 2020 2020 2020 2020 2064 6963 7428 0a20           dict(. 
+0000c760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c770: 2020 2061 6374 696f 6e3d 2272 756e 4163     action="runAc
+0000c780: 7469 6f6e 222c 0a20 2020 2020 2020 2020  tion",.         
+0000c790: 2020 2020 2020 2020 2020 2070 6172 616d             param
+0000c7a0: 733d 6469 6374 280a 2020 2020 2020 2020  s=dict(.        
+0000c7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c7c0: 6163 7469 6f6e 4964 3d61 6374 696f 6e5f  actionId=action_
+0000c7d0: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
+0000c7e0: 2020 2020 2020 2020 292c 0a20 2020 2020          ),.     
+0000c7f0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0000c800: 2020 2020 2020 2020 205d 2c0a 2020 2020           ],.    
+0000c810: 2020 2020 290a 0a20 2020 2040 6164 645f      )..    @add_
+0000c820: 746f 5f67 656e 6572 616c 5f61 7379 6e63  to_general_async
+0000c830: 5f67 726f 7570 0a20 2020 2061 7379 6e63  _group.    async
+0000c840: 2064 6566 2074 6162 6c65 280a 2020 2020   def table(.    
+0000c850: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+0000c860: 2020 6f72 6465 723a 2069 6e74 2c0a 2020    order: int,.  
+0000c870: 2020 2020 2020 6461 7461 3a20 556e 696f        data: Unio
+0000c880: 6e5b 7374 722c 2070 642e 4461 7461 4672  n[str, pd.DataFr
+0000c890: 616d 652c 206c 6973 745b 6469 6374 5d2c  ame, list[dict],
+0000c8a0: 2064 6963 745d 2c0a 2020 2020 2020 2020   dict],.        
+0000c8b0: 636f 6c75 6d6e 733a 204f 7074 696f 6e61  columns: Optiona
+0000c8c0: 6c5b 6c69 7374 5b73 7472 5d5d 203d 204e  l[list[str]] = N
+0000c8d0: 6f6e 652c 0a20 2020 2020 2020 2063 6f6c  one,.        col
+0000c8e0: 756d 6e73 5f62 7574 746f 6e3a 2062 6f6f  umns_button: boo
+0000c8f0: 6c20 3d20 5472 7565 2c0a 2020 2020 2020  l = True,.      
+0000c900: 2020 6669 6c74 6572 733a 2062 6f6f 6c20    filters: bool 
+0000c910: 3d20 5472 7565 2c0a 2020 2020 2020 2020  = True,.        
+0000c920: 6578 706f 7274 5f74 6f5f 6373 763a 2062  export_to_csv: b
+0000c930: 6f6f 6c20 3d20 5472 7565 2c0a 2020 2020  ool = True,.    
+0000c940: 2020 2020 7365 6172 6368 3a20 626f 6f6c      search: bool
+0000c950: 203d 2054 7275 652c 0a20 2020 2020 2020   = True,.       
+0000c960: 2070 6167 655f 7369 7a65 3a20 696e 7420   page_size: int 
+0000c970: 3d20 3130 2c0a 2020 2020 2020 2020 7061  = 10,.        pa
+0000c980: 6765 5f73 697a 655f 6f70 7469 6f6e 733a  ge_size_options:
+0000c990: 204f 7074 696f 6e61 6c5b 6c69 7374 5b69   Optional[list[i
+0000c9a0: 6e74 5d5d 203d 204e 6f6e 652c 0a20 2020  nt]] = None,.   
+0000c9b0: 2020 2020 2069 6e69 7469 616c 5f73 6f72       initial_sor
+0000c9c0: 745f 636f 6c75 6d6e 3a20 4f70 7469 6f6e  t_column: Option
+0000c9d0: 616c 5b73 7472 5d20 3d20 4e6f 6e65 2c0a  al[str] = None,.
+0000c9e0: 2020 2020 2020 2020 736f 7274 5f64 6573          sort_des
+0000c9f0: 6365 6e64 696e 673a 2062 6f6f 6c20 3d20  cending: bool = 
+0000ca00: 4661 6c73 652c 0a20 2020 2020 2020 2063  False,.        c
+0000ca10: 6f6c 756d 6e73 5f6f 7074 696f 6e73 3a20  olumns_options: 
+0000ca20: 4f70 7469 6f6e 616c 5b64 6963 745d 203d  Optional[dict] =
+0000ca30: 204e 6f6e 652c 0a20 2020 2020 2020 2063   None,.        c
+0000ca40: 6174 6567 6f72 6963 616c 5f63 6f6c 756d  ategorical_colum
+0000ca50: 6e73 3a20 4f70 7469 6f6e 616c 5b6c 6973  ns: Optional[lis
+0000ca60: 745b 7374 725d 5d20 3d20 4e6f 6e65 2c0a  t[str]] = None,.
+0000ca70: 2020 2020 2020 2020 6c61 6265 6c5f 636f          label_co
+0000ca80: 6c75 6d6e 733a 204f 7074 696f 6e61 6c5b  lumns: Optional[
+0000ca90: 6469 6374 5d20 3d20 4e6f 6e65 2c0a 2020  dict] = None,.  
+0000caa0: 2020 2020 2020 7765 625f 6c69 6e6b 5f63        web_link_c
+0000cab0: 6f6c 756d 6e3a 204f 7074 696f 6e61 6c5b  olumn: Optional[
+0000cac0: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
+0000cad0: 2020 2020 206f 7065 6e5f 6c69 6e6b 5f69       open_link_i
+0000cae0: 6e5f 6e65 775f 7461 623a 2062 6f6f 6c20  n_new_tab: bool 
+0000caf0: 3d20 4661 6c73 652c 0a20 2020 2020 2020  = False,.       
+0000cb00: 2074 6974 6c65 3a20 4f70 7469 6f6e 616c   title: Optional
+0000cb10: 5b73 7472 5d20 3d20 4e6f 6e65 2c0a 2020  [str] = None,.  
+0000cb20: 2020 2020 2020 7061 6464 696e 673a 204f        padding: O
+0000cb30: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+0000cb40: 6f6e 652c 0a20 2020 2020 2020 2072 6f77  one,.        row
+0000cb50: 735f 7369 7a65 3a20 4f70 7469 6f6e 616c  s_size: Optional
+0000cb60: 5b69 6e74 5d20 3d20 4e6f 6e65 2c0a 2020  [int] = None,.  
+0000cb70: 2020 2020 2020 636f 6c73 5f73 697a 653a        cols_size:
+0000cb80: 204f 7074 696f 6e61 6c5b 696e 745d 203d   Optional[int] =
+0000cb90: 204e 6f6e 652c 0a20 2020 2029 3a0a 2020   None,.    ):.  
+0000cba0: 2020 2020 2020 2222 2243 7265 6174 6520        """Create 
+0000cbb0: 6120 7461 626c 6520 7265 706f 7274 2069  a table report i
+0000cbc0: 6e20 7468 6520 6461 7368 626f 6172 642e  n the dashboard.
+0000cbd0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+0000cbe0: 6f72 6465 723a 2074 6865 206f 7264 6572  order: the order
+0000cbf0: 206f 6620 7468 6520 7461 626c 650a 2020   of the table.  
+0000cc00: 2020 2020 2020 3a70 6172 616d 2064 6174        :param dat
+0000cc10: 613a 2074 6865 2064 6174 6120 6f66 2074  a: the data of t
+0000cc20: 6865 2074 6162 6c65 0a20 2020 2020 2020  he table.       
+0000cc30: 203a 7061 7261 6d20 636f 6c75 6d6e 733a   :param columns:
+0000cc40: 2074 6865 2063 6f6c 756d 6e73 206f 6620   the columns of 
+0000cc50: 7468 6520 7461 626c 650a 2020 2020 2020  the table.      
+0000cc60: 2020 3a70 6172 616d 2063 6f6c 756d 6e73    :param columns
+0000cc70: 5f62 7574 746f 6e3a 2077 6865 7468 6572  _button: whether
+0000cc80: 2074 6f20 7368 6f77 2074 6865 2063 6f6c   to show the col
+0000cc90: 756d 6e73 2062 7574 746f 6e0a 2020 2020  umns button.    
+0000cca0: 2020 2020 3a70 6172 616d 2066 696c 7465      :param filte
+0000ccb0: 7273 3a20 7768 6574 6865 7220 746f 2073  rs: whether to s
+0000ccc0: 686f 7720 7468 6520 6669 6c74 6572 7320  how the filters 
+0000ccd0: 6275 7474 6f6e 0a20 2020 2020 2020 203a  button.        :
+0000cce0: 7061 7261 6d20 6578 706f 7274 5f74 6f5f  param export_to_
+0000ccf0: 6373 763a 2077 6865 7468 6572 2074 6f20  csv: whether to 
+0000cd00: 7368 6f77 2074 6865 2065 7870 6f72 7420  show the export 
+0000cd10: 746f 2063 7376 2062 7574 746f 6e0a 2020  to csv button.  
+0000cd20: 2020 2020 2020 3a70 6172 616d 2073 6561        :param sea
+0000cd30: 7263 683a 2077 6865 7468 6572 2074 6f20  rch: whether to 
+0000cd40: 7368 6f77 2074 6865 2073 6561 7263 6820  show the search 
+0000cd50: 6261 720a 2020 2020 2020 2020 3a70 6172  bar.        :par
+0000cd60: 616d 2070 6167 655f 7369 7a65 3a20 7468  am page_size: th
+0000cd70: 6520 6e75 6d62 6572 206f 6620 726f 7773  e number of rows
+0000cd80: 2070 6572 2070 6167 650a 2020 2020 2020   per page.      
+0000cd90: 2020 3a70 6172 616d 2070 6167 655f 7369    :param page_si
+0000cda0: 7a65 5f6f 7074 696f 6e73 3a20 7468 6520  ze_options: the 
+0000cdb0: 6f70 7469 6f6e 7320 666f 7220 7468 6520  options for the 
+0000cdc0: 6e75 6d62 6572 206f 6620 726f 7773 2070  number of rows p
+0000cdd0: 6572 2070 6167 650a 2020 2020 2020 2020  er page.        
+0000cde0: 3a70 6172 616d 2069 6e69 7469 616c 5f73  :param initial_s
+0000cdf0: 6f72 745f 636f 6c75 6d6e 3a20 7468 6520  ort_column: the 
+0000ce00: 696e 6974 6961 6c20 736f 7274 696e 6720  initial sorting 
+0000ce10: 636f 6c75 6d6e 0a20 2020 2020 2020 203a  column.        :
+0000ce20: 7061 7261 6d20 736f 7274 5f64 6573 6365  param sort_desce
+0000ce30: 6e64 696e 673a 2077 6865 7468 6572 2074  nding: whether t
+0000ce40: 6f20 736f 7274 2064 6573 6365 6e64 696e  o sort descendin
+0000ce50: 6720 6279 2074 6865 2069 6e69 7469 616c  g by the initial
+0000ce60: 2073 6f72 7469 6e67 2063 6f6c 756d 6e0a   sorting column.
+0000ce70: 2020 2020 2020 2020 3a70 6172 616d 2063          :param c
+0000ce80: 6f6c 756d 6e73 5f6f 7074 696f 6e73 3a20  olumns_options: 
+0000ce90: 7468 6520 6f70 7469 6f6e 7320 666f 7220  the options for 
+0000cea0: 7468 6520 636f 6c75 6d6e 730a 2020 2020  the columns.    
+0000ceb0: 2020 2020 3a70 6172 616d 2063 6174 6567      :param categ
+0000cec0: 6f72 6963 616c 5f63 6f6c 756d 6e73 3a20  orical_columns: 
+0000ced0: 7468 6520 6361 7465 676f 7269 6361 6c20  the categorical 
+0000cee0: 636f 6c75 6d6e 730a 2020 2020 2020 2020  columns.        
+0000cef0: 3a70 6172 616d 206c 6162 656c 5f63 6f6c  :param label_col
+0000cf00: 756d 6e73 3a20 7468 6520 6c61 6265 6c20  umns: the label 
+0000cf10: 636f 6c75 6d6e 730a 2020 2020 2020 2020  columns.        
+0000cf20: 3a70 6172 616d 2072 6570 6f72 745f 7061  :param report_pa
+0000cf30: 7261 6d73 3a20 6164 6469 7469 6f6e 616c  rams: additional
+0000cf40: 2072 6570 6f72 7420 7061 7261 6d65 7465   report paramete
+0000cf50: 7273 2061 7320 6b65 792d 7661 6c75 6520  rs as key-value 
+0000cf60: 7061 6972 730a 2020 2020 2020 2020 3a70  pairs.        :p
+0000cf70: 6172 616d 2077 6562 5f6c 696e 6b5f 636f  aram web_link_co
+0000cf80: 6c75 6d6e 3a20 7468 6520 636f 6c75 6d6e  lumn: the column
+0000cf90: 2074 6f20 7573 6520 6173 2077 6562 206c   to use as web l
+0000cfa0: 696e 6b0a 2020 2020 2020 2020 3a70 6172  ink.        :par
+0000cfb0: 616d 206f 7065 6e5f 6c69 6e6b 5f69 6e5f  am open_link_in_
+0000cfc0: 6e65 775f 7461 623a 2077 6865 7468 6572  new_tab: whether
+0000cfd0: 2074 6f20 6f70 656e 2074 6865 2077 6562   to open the web
+0000cfe0: 206c 696e 6b20 696e 2061 206e 6577 2074   link in a new t
+0000cff0: 6162 0a20 2020 2020 2020 203a 7061 7261  ab.        :para
+0000d000: 6d20 7469 746c 653a 2074 6865 2074 6974  m title: the tit
+0000d010: 6c65 206f 6620 7468 6520 7461 626c 650a  le of the table.
+0000d020: 2020 2020 2020 2020 3a70 6172 616d 2070          :param p
+0000d030: 6164 6469 6e67 3a20 7468 6520 7061 6464  adding: the padd
+0000d040: 696e 6720 6f66 2074 6865 2074 6162 6c65  ing of the table
+0000d050: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+0000d060: 726f 7773 5f73 697a 653a 2074 6865 2072  rows_size: the r
+0000d070: 6f77 7320 7369 7a65 206f 6620 7468 6520  ows size of the 
+0000d080: 7461 626c 650a 2020 2020 2020 2020 3a70  table.        :p
+0000d090: 6172 616d 2063 6f6c 735f 7369 7a65 3a20  aram cols_size: 
+0000d0a0: 7468 6520 636f 6c75 6d6e 7320 7369 7a65  the columns size
+0000d0b0: 206f 6620 7468 6520 7461 626c 650a 2020   of the table.  
+0000d0c0: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
+0000d0d0: 2020 2064 6174 615f 6d61 7070 696e 6773     data_mappings
+0000d0e0: 5f74 6f5f 7475 706c 6573 203d 2061 7761  _to_tuples = awa
+0000d0f0: 6974 2073 656c 662e 5f63 686f 6f73 655f  it self._choose_
+0000d100: 6461 7461 286f 7264 6572 2c20 6461 7461  data(order, data
+0000d110: 2c20 5461 626c 6529 0a20 2020 2020 2020  , Table).       
+0000d120: 2069 6620 6973 696e 7374 616e 6365 2864   if isinstance(d
+0000d130: 6174 612c 2073 7472 293a 0a20 2020 2020  ata, str):.     
+0000d140: 2020 2020 2020 2064 6174 6120 3d20 7365         data = se
+0000d150: 6c66 2e5f 7368 6172 6564 5f64 6174 615b  lf._shared_data[
+0000d160: 6461 7461 5d0a 0a20 2020 2020 2020 2064  data]..        d
+0000d170: 6620 3d20 7661 6c69 6461 7465 5f64 6174  f = validate_dat
+0000d180: 615f 6973 5f70 616e 6461 7261 626c 6528  a_is_pandarable(
+0000d190: 6461 7461 290a 0a20 2020 2020 2020 2069  data)..        i
+0000d1a0: 6620 6e6f 7420 636f 6c75 6d6e 733a 0a20  f not columns:. 
+0000d1b0: 2020 2020 2020 2020 2020 2063 6f6c 756d             colum
+0000d1c0: 6e73 203d 206c 6973 7428 6461 7461 5f6d  ns = list(data_m
+0000d1d0: 6170 7069 6e67 735f 746f 5f74 7570 6c65  appings_to_tuple
+0000d1e0: 732e 6b65 7973 2829 290a 2020 2020 2020  s.keys()).      
+0000d1f0: 2020 6966 206e 6f74 2063 6f6c 756d 6e73    if not columns
+0000d200: 5f6f 7074 696f 6e73 3a0a 2020 2020 2020  _options:.      
+0000d210: 2020 2020 2020 636f 6c75 6d6e 735f 6f70        columns_op
+0000d220: 7469 6f6e 7320 3d20 7b7d 0a20 2020 2020  tions = {}.     
+0000d230: 2020 2069 6620 6e6f 7420 6361 7465 676f     if not catego
+0000d240: 7269 6361 6c5f 636f 6c75 6d6e 733a 0a20  rical_columns:. 
+0000d250: 2020 2020 2020 2020 2020 2063 6174 6567             categ
+0000d260: 6f72 6963 616c 5f63 6f6c 756d 6e73 203d  orical_columns =
+0000d270: 205b 5d0a 2020 2020 2020 2020 6966 206e   [].        if n
+0000d280: 6f74 206c 6162 656c 5f63 6f6c 756d 6e73  ot label_columns
+0000d290: 3a0a 2020 2020 2020 2020 2020 2020 6c61  :.            la
+0000d2a0: 6265 6c5f 636f 6c75 6d6e 7320 3d20 7b7d  bel_columns = {}
+0000d2b0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+0000d2c0: 2020 2020 2020 2020 2020 2061 7578 5f6c             aux_l
+0000d2d0: 6162 656c 5f63 6f6c 756d 6e73 203d 206c  abel_columns = l
+0000d2e0: 6162 656c 5f63 6f6c 756d 6e73 0a20 2020  abel_columns.   
+0000d2f0: 2020 2020 2020 2020 206c 6162 656c 5f63           label_c
+0000d300: 6f6c 756d 6e73 203d 207b 7d0a 2020 2020  olumns = {}.    
+0000d310: 2020 2020 2020 2020 666f 7220 6861 735f          for has_
+0000d320: 746f 5f62 655f 7475 706c 6520 696e 2061  to_be_tuple in a
+0000d330: 7578 5f6c 6162 656c 5f63 6f6c 756d 6e73  ux_label_columns
+0000d340: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000d350: 2020 7620 3d20 6175 785f 6c61 6265 6c5f    v = aux_label_
+0000d360: 636f 6c75 6d6e 735b 6861 735f 746f 5f62  columns[has_to_b
+0000d370: 655f 7475 706c 655d 0a20 2020 2020 2020  e_tuple].       
+0000d380: 2020 2020 2020 2020 2069 6620 6973 696e           if isin
+0000d390: 7374 616e 6365 2868 6173 5f74 6f5f 6265  stance(has_to_be
+0000d3a0: 5f74 7570 6c65 2c20 7374 7229 3a0a 2020  _tuple, str):.  
+0000d3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d3c0: 2020 6c61 6265 6c5f 636f 6c75 6d6e 735b    label_columns[
+0000d3d0: 2868 6173 5f74 6f5f 6265 5f74 7570 6c65  (has_to_be_tuple
+0000d3e0: 2c20 2266 696c 6c65 6422 295d 203d 2076  , "filled")] = v
+0000d3f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d400: 2065 6c69 6620 6973 696e 7374 616e 6365   elif isinstance
+0000d410: 2868 6173 5f74 6f5f 6265 5f74 7570 6c65  (has_to_be_tuple
+0000d420: 2c20 7475 706c 6529 3a0a 2020 2020 2020  , tuple):.      
+0000d430: 2020 2020 2020 2020 2020 2020 2020 6c61                la
+0000d440: 6265 6c5f 636f 6c75 6d6e 735b 6861 735f  bel_columns[has_
+0000d450: 746f 5f62 655f 7475 706c 655d 203d 2076  to_be_tuple] = v
+0000d460: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d470: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0000d480: 2020 2020 2020 2020 2020 206c 6f67 5f65             log_e
+0000d490: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
+0000d4a0: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+0000d4b0: 6767 6572 2c0a 2020 2020 2020 2020 2020  gger,.          
+0000d4c0: 2020 2020 2020 2020 2020 2020 2020 6622                f"
+0000d4d0: 496e 7661 6c69 6420 6c61 6265 6c5f 636f  Invalid label_co
+0000d4e0: 6c75 6d6e 7320 6b65 793a 207b 6861 735f  lumns key: {has_
+0000d4f0: 746f 5f62 655f 7475 706c 657d 222c 0a20  to_be_tuple}",. 
+0000d500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d510: 2020 2020 2020 2056 616c 7565 4572 726f         ValueErro
+0000d520: 722c 0a20 2020 2020 2020 2020 2020 2020  r,.             
+0000d530: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0000d540: 206c 6162 656c 5f6a 7573 745f 636f 6c75   label_just_colu
+0000d550: 6d6e 7320 3d20 5b78 5b30 5d20 666f 7220  mns = [x[0] for 
+0000d560: 7820 696e 206c 6162 656c 5f63 6f6c 756d  x in label_colum
+0000d570: 6e73 2e6b 6579 7328 295d 0a0a 2020 2020  ns.keys()]..    
+0000d580: 2020 2020 5f2c 2064 6174 615f 7365 742c      _, data_set,
+0000d590: 205f 203d 2064 6174 615f 6d61 7070 696e   _ = data_mappin
+0000d5a0: 6773 5f74 6f5f 7475 706c 6573 5b63 6f6c  gs_to_tuples[col
+0000d5b0: 756d 6e73 5b30 5d5d 0a20 2020 2020 2020  umns[0]].       
+0000d5c0: 2063 6f6c 756d 6e73 5f64 6963 7473 203d   columns_dicts =
+0000d5d0: 205b 5d0a 2020 2020 2020 2020 726f 7773   [].        rows
+0000d5e0: 5f64 6963 7420 3d20 7b22 6d61 7070 696e  _dict = {"mappin
+0000d5f0: 6722 3a20 7b7d 7d0a 2020 2020 2020 2020  g": {}}.        
+0000d600: 666f 7220 692c 206e 616d 6520 696e 2065  for i, name in e
+0000d610: 6e75 6d65 7261 7465 2863 6f6c 756d 6e73  numerate(columns
+0000d620: 293a 0a20 2020 2020 2020 2020 2020 2063  ):.            c
+0000d630: 6f6c 756d 6e5f 6f70 7469 6f6e 7320 3d20  olumn_options = 
+0000d640: 7b22 6669 656c 6422 3a20 6e61 6d65 2c20  {"field": name, 
+0000d650: 2268 6561 6465 724e 616d 6522 3a20 6e61  "headerName": na
+0000d660: 6d65 2c20 226f 7264 6572 223a 2069 7d0a  me, "order": i}.
+0000d670: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000d680: 6e61 6d65 2069 6e20 636f 6c75 6d6e 735f  name in columns_
+0000d690: 6f70 7469 6f6e 733a 0a20 2020 2020 2020  options:.       
+0000d6a0: 2020 2020 2020 2020 2063 6f6c 756d 6e5f           column_
+0000d6b0: 6f70 7469 6f6e 732e 7570 6461 7465 2863  options.update(c
+0000d6c0: 6f6c 756d 6e73 5f6f 7074 696f 6e73 5b6e  olumns_options[n
+0000d6d0: 616d 655d 290a 0a20 2020 2020 2020 2020  ame])..         
+0000d6e0: 2020 2069 6620 6e61 6d65 2069 6e20 6361     if name in ca
+0000d6f0: 7465 676f 7269 6361 6c5f 636f 6c75 6d6e  tegorical_column
+0000d700: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+0000d710: 2020 2069 6620 6e61 6d65 2069 6e20 6c61     if name in la
+0000d720: 6265 6c5f 636f 6c75 6d6e 733a 0a20 2020  bel_columns:.   
+0000d730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d740: 206c 6f67 5f65 7272 6f72 280a 2020 2020   log_error(.    
+0000d750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d760: 2020 2020 6c6f 6767 6572 2c0a 2020 2020      logger,.    
+0000d770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d780: 2020 2020 6622 436f 6c75 6d6e 7320 6361      f"Columns ca
+0000d790: 6e6e 6f74 2062 6520 626f 7468 2069 6e63  nnot be both inc
+0000d7a0: 6c75 6465 6420 696e 2063 6174 6567 6f72  luded in categor
+0000d7b0: 6963 616c 5f63 6f6c 756d 6e73 2061 6e64  ical_columns and
+0000d7c0: 206c 6162 656c 5f63 6f6c 756d 6e73 3a20   label_columns: 
+0000d7d0: 7b6e 616d 657d 222c 0a20 2020 2020 2020  {name}",.       
+0000d7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d7f0: 2056 616c 7565 4572 726f 722c 0a20 2020   ValueError,.   
+0000d800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d810: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+0000d820: 2020 2063 6f6c 756d 6e5f 6f70 7469 6f6e     column_option
+0000d830: 735b 2274 7970 6522 5d20 3d20 2273 696e  s["type"] = "sin
+0000d840: 676c 6553 656c 6563 7422 0a20 2020 2020  gleSelect".     
+0000d850: 2020 2020 2020 2020 2020 2063 6f6c 756d             colum
+0000d860: 6e5f 6f70 7469 6f6e 735b 226f 7074 696f  n_options["optio
+0000d870: 6e73 225d 203d 2064 665b 6e61 6d65 5d2e  ns"] = df[name].
+0000d880: 756e 6971 7565 2829 2e74 6f6c 6973 7428  unique().tolist(
+0000d890: 290a 0a20 2020 2020 2020 2020 2020 2069  )..            i
+0000d8a0: 6620 6e61 6d65 2069 6e20 6c61 6265 6c5f  f name in label_
+0000d8b0: 6a75 7374 5f63 6f6c 756d 6e73 3a0a 2020  just_columns:.  
+0000d8c0: 2020 2020 2020 2020 2020 2020 2020 696e                in
+0000d8d0: 6465 7820 3d20 6c61 6265 6c5f 6a75 7374  dex = label_just
+0000d8e0: 5f63 6f6c 756d 6e73 2e69 6e64 6578 286e  _columns.index(n
+0000d8f0: 616d 6529 0a20 2020 2020 2020 2020 2020  ame).           
+0000d900: 2020 2020 2028 5f2c 2076 6172 6961 6e74       (_, variant
+0000d910: 292c 206c 6162 656c 5f6f 7074 696f 6e73  ), label_options
+0000d920: 203d 206c 6973 7428 6c61 6265 6c5f 636f   = list(label_co
+0000d930: 6c75 6d6e 732e 6974 656d 7328 2929 5b69  lumns.items())[i
+0000d940: 6e64 6578 5d0a 2020 2020 2020 2020 2020  ndex].          
+0000d950: 2020 2020 2020 636f 6c75 6d6e 5f6f 7074        column_opt
+0000d960: 696f 6e73 5b22 6368 6970 7322 5d20 3d20  ions["chips"] = 
+0000d970: 7b7d 0a20 2020 2020 2020 2020 2020 2020  {}.             
+0000d980: 2020 2063 6f6c 756d 6e5f 6f70 7469 6f6e     column_option
+0000d990: 735b 2263 6869 7073 225d 5b22 7661 7269  s["chips"]["vari
+0000d9a0: 616e 7422 5d20 3d20 7661 7269 616e 740a  ant"] = variant.
+0000d9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d9c0: 636f 6c75 6d6e 5f6f 7074 696f 6e73 5b22  column_options["
+0000d9d0: 6368 6970 7322 5d5b 226f 7074 696f 6e73  chips"]["options
+0000d9e0: 225d 203d 2069 6e74 6572 7072 6574 5f6c  "] = interpret_l
+0000d9f0: 6162 656c 5f69 6e66 6f28 0a20 2020 2020  abel_info(.     
+0000da00: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+0000da10: 662c 206e 616d 652c 206c 6162 656c 5f6f  f, name, label_o
+0000da20: 7074 696f 6e73 2c20 7661 7269 616e 740a  ptions, variant.
+0000da30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000da40: 290a 0a20 2020 2020 2020 2020 2020 2069  )..            i
+0000da50: 6620 6e61 6d65 203d 3d20 7765 625f 6c69  f name == web_li
+0000da60: 6e6b 5f63 6f6c 756d 6e3a 0a20 2020 2020  nk_column:.     
+0000da70: 2020 2020 2020 2020 2020 2063 6f6c 756d             colum
+0000da80: 6e5f 6f70 7469 6f6e 735b 226c 696e 6b22  n_options["link"
+0000da90: 5d20 3d20 7b0a 2020 2020 2020 2020 2020  ] = {.          
+0000daa0: 2020 2020 2020 2020 2020 2275 726c 223a            "url":
+0000dab0: 2022 7765 624c 696e 6b22 2c0a 2020 2020   "webLink",.    
+0000dac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dad0: 226f 7065 6e4e 6577 5461 6222 3a20 6f70  "openNewTab": op
+0000dae0: 656e 5f6c 696e 6b5f 696e 5f6e 6577 5f74  en_link_in_new_t
+0000daf0: 6162 2c0a 2020 2020 2020 2020 2020 2020  ab,.            
+0000db00: 2020 2020 7d0a 0a20 2020 2020 2020 2020      }..         
+0000db10: 2020 2063 6f6c 756d 6e73 5f64 6963 7473     columns_dicts
+0000db20: 2e61 7070 656e 6428 636f 6c75 6d6e 5f6f  .append(column_o
+0000db30: 7074 696f 6e73 290a 2020 2020 2020 2020  ptions).        
+0000db40: 2020 2020 726f 7773 5f64 6963 745b 226d      rows_dict["m
+0000db50: 6170 7069 6e67 225d 5b6e 616d 655d 203d  apping"][name] =
+0000db60: 2064 6174 615f 6d61 7070 696e 6773 5f74   data_mappings_t
+0000db70: 6f5f 7475 706c 6573 5b6e 616d 655d 5b30  o_tuples[name][0
+0000db80: 5d0a 0a20 2020 2020 2020 2069 6620 7765  ]..        if we
+0000db90: 625f 6c69 6e6b 5f63 6f6c 756d 6e3a 0a20  b_link_column:. 
+0000dba0: 2020 2020 2020 2020 2020 2072 6f77 735f             rows_
+0000dbb0: 6469 6374 5b22 6d61 7070 696e 6722 5d5b  dict["mapping"][
+0000dbc0: 2277 6562 225d 203d 2064 6174 615f 6d61  "web"] = data_ma
+0000dbd0: 7070 696e 6773 5f74 6f5f 7475 706c 6573  ppings_to_tuples
+0000dbe0: 5b77 6562 5f6c 696e 6b5f 636f 6c75 6d6e  [web_link_column
+0000dbf0: 5d5b 305d 0a20 2020 2020 2020 2020 2020  ][0].           
+0000dc00: 2072 6f77 735f 6469 6374 5b22 6d61 7070   rows_dict["mapp
+0000dc10: 696e 6722 5d5b 2277 6562 4c69 6e6b 225d  ing"]["webLink"]
+0000dc20: 203d 2064 6174 615f 6d61 7070 696e 6773   = data_mappings
+0000dc30: 5f74 6f5f 7475 706c 6573 5b77 6562 5f6c  _to_tuples[web_l
+0000dc40: 696e 6b5f 636f 6c75 6d6e 5d5b 0a20 2020  ink_column][.   
+0000dc50: 2020 2020 2020 2020 2020 2020 2030 0a20               0. 
+0000dc60: 2020 2020 2020 2020 2020 205d 0a0a 2020             ]..  
+0000dc70: 2020 2020 2020 5f2c 2072 6570 6f72 7420        _, report 
+0000dc80: 3d20 6177 6169 7420 7365 6c66 2e5f 6765  = await self._ge
+0000dc90: 745f 6368 6172 745f 7265 706f 7274 286f  t_chart_report(o
+0000dca0: 7264 6572 2c20 5461 626c 6529 0a0a 2020  rder, Table)..  
+0000dcb0: 2020 2020 2020 7264 7320 3d20 6177 6169        rds = awai
+0000dcc0: 7420 7265 706f 7274 2e67 6574 5f72 6570  t report.get_rep
+0000dcd0: 6f72 745f 6461 7461 5f73 6574 7328 290a  ort_data_sets().
+0000dce0: 0a20 2020 2020 2020 2069 6620 280a 2020  .        if (.  
+0000dcf0: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
+0000dd00: 6575 7365 5f64 6174 615f 7365 7473 0a20  euse_data_sets. 
+0000dd10: 2020 2020 2020 2020 2020 2061 6e64 2072             and r
+0000dd20: 6570 6f72 745b 2270 726f 7065 7274 6965  eport["propertie
+0000dd30: 7322 5d2e 6765 7428 2263 6f6c 756d 6e73  s"].get("columns
+0000dd40: 2229 0a20 2020 2020 2020 2020 2020 2061  ").            a
+0000dd50: 6e64 2072 6570 6f72 745b 2270 726f 7065  nd report["prope
+0000dd60: 7274 6965 7322 5d5b 2263 6f6c 756d 6e73  rties"]["columns
+0000dd70: 225d 2021 3d20 636f 6c75 6d6e 735f 6469  "] != columns_di
+0000dd80: 6374 730a 2020 2020 2020 2020 293a 0a20  cts.        ):. 
+0000dd90: 2020 2020 2020 2020 2020 206c 6f67 5f65             log_e
+0000dda0: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
+0000ddb0: 2020 2020 2020 6c6f 6767 6572 2c0a 2020        logger,.  
+0000ddc0: 2020 2020 2020 2020 2020 2020 2020 2243                "C
+0000ddd0: 6f6c 756d 6e73 206f 7074 696f 6e73 2064  olumns options d
+0000dde0: 6f20 6e6f 7420 6d61 7463 6820 7468 6520  o not match the 
+0000ddf0: 7072 6576 696f 7573 2063 6f6c 756d 6e73  previous columns
+0000de00: 2c20 6d6f 7374 206c 696b 656c 7920 6461  , most likely da
+0000de10: 7461 2068 6173 2063 6861 6e67 6564 2c22  ta has changed,"
+0000de20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000de30: 2022 2064 6f6e 2774 2075 7365 2074 6865   " don't use the
+0000de40: 2072 6575 7365 5f64 6174 615f 7365 7473   reuse_data_sets
+0000de50: 206f 7074 696f 6e20 696e 2074 6869 7320   option in this 
+0000de60: 6361 7365 222c 0a20 2020 2020 2020 2020  case",.         
+0000de70: 2020 2020 2020 2044 6174 6145 7272 6f72         DataError
+0000de80: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
+0000de90: 0a20 2020 2020 2020 2069 6620 7264 7320  .        if rds 
+0000dea0: 616e 6420 280a 2020 2020 2020 2020 2020  and (.          
+0000deb0: 2020 6e6f 7420 7365 6c66 2e72 6575 7365    not self.reuse
+0000dec0: 5f64 6174 615f 7365 7473 0a20 2020 2020  _data_sets.     
+0000ded0: 2020 2020 2020 206f 7220 616e 7928 7264         or any(rd
+0000dee0: 5b22 6461 7461 5365 7449 6422 5d20 213d  ["dataSetId"] !=
+0000def0: 2064 6174 615f 7365 745b 2269 6422 5d20   data_set["id"] 
+0000df00: 666f 7220 7264 2069 6e20 7264 7329 0a20  for rd in rds). 
+0000df10: 2020 2020 2020 2029 3a0a 2020 2020 2020         ):.      
+0000df20: 2020 2020 2020 6177 6169 7420 7265 706f        await repo
+0000df30: 7274 2e64 656c 6574 655f 7265 706f 7274  rt.delete_report
+0000df40: 5f64 6174 615f 7365 7473 286c 6f67 3d54  _data_sets(log=T
+0000df50: 7275 6529 0a20 2020 2020 2020 2020 2020  rue).           
+0000df60: 2072 6473 203d 205b 5d0a 0a20 2020 2020   rds = []..     
+0000df70: 2020 2069 6620 6e6f 7420 7264 733a 0a20     if not rds:. 
+0000df80: 2020 2020 2020 2020 2020 2061 7761 6974             await
+0000df90: 2072 6570 6f72 742e 6372 6561 7465 5f72   report.create_r
+0000dfa0: 6570 6f72 745f 6461 7461 5f73 6574 2828  eport_data_set((
+0000dfb0: 4e6f 6e65 2c20 6461 7461 5f73 6574 2c20  None, data_set, 
+0000dfc0: 4e6f 6e65 2929 0a0a 2020 2020 2020 2020  None))..        
+0000dfd0: 7061 6769 6e61 7469 6f6e 203d 207b 2270  pagination = {"p
+0000dfe0: 6167 6553 697a 6522 3a20 7061 6765 5f73  ageSize": page_s
+0000dff0: 697a 657d 0a20 2020 2020 2020 2069 6620  ize}.        if 
+0000e000: 7061 6765 5f73 697a 655f 6f70 7469 6f6e  page_size_option
+0000e010: 733a 0a20 2020 2020 2020 2020 2020 2070  s:.            p
+0000e020: 6167 696e 6174 696f 6e5b 2270 6167 6553  agination["pageS
+0000e030: 697a 654f 7074 696f 6e73 225d 203d 2070  izeOptions"] = p
+0000e040: 6167 655f 7369 7a65 5f6f 7074 696f 6e73  age_size_options
+0000e050: 0a0a 2020 2020 2020 2020 736f 7274 203d  ..        sort =
+0000e060: 207b 7d0a 2020 2020 2020 2020 6966 2069   {}.        if i
+0000e070: 6e69 7469 616c 5f73 6f72 745f 636f 6c75  nitial_sort_colu
+0000e080: 6d6e 3a0a 2020 2020 2020 2020 2020 2020  mn:.            
+0000e090: 736f 7274 5b22 6669 656c 6422 5d20 3d20  sort["field"] = 
+0000e0a0: 6461 7461 5f6d 6170 7069 6e67 735f 746f  data_mappings_to
+0000e0b0: 5f74 7570 6c65 735b 696e 6974 6961 6c5f  _tuples[initial_
+0000e0c0: 736f 7274 5f63 6f6c 756d 6e5d 5b30 5d0a  sort_column][0].
+0000e0d0: 2020 2020 2020 2020 2020 2020 736f 7274              sort
+0000e0e0: 5b22 6469 7265 6374 696f 6e22 5d20 3d20  ["direction"] = 
+0000e0f0: 2261 7363 2220 6966 206e 6f74 2073 6f72  "asc" if not sor
+0000e100: 745f 6465 7363 656e 6469 6e67 2065 6c73  t_descending els
+0000e110: 6520 2264 6573 6322 0a0a 2020 2020 2020  e "desc"..      
+0000e120: 2020 6177 6169 7420 7365 6c66 2e5f 6372    await self._cr
+0000e130: 6561 7465 5f63 6861 7274 280a 2020 2020  eate_chart(.    
+0000e140: 2020 2020 2020 2020 6368 6172 745f 636c          chart_cl
+0000e150: 6173 733d 5461 626c 652c 0a20 2020 2020  ass=Table,.     
+0000e160: 2020 2020 2020 206f 7264 6572 3d6f 7264         order=ord
+0000e170: 6572 2c0a 2020 2020 2020 2020 2020 2020  er,.            
+0000e180: 7369 7a65 5061 6464 696e 673d 7061 6464  sizePadding=padd
+0000e190: 696e 672c 0a20 2020 2020 2020 2020 2020  ing,.           
+0000e1a0: 2073 697a 6552 6f77 733d 726f 7773 5f73   sizeRows=rows_s
+0000e1b0: 697a 652c 0a20 2020 2020 2020 2020 2020  ize,.           
+0000e1c0: 2073 697a 6543 6f6c 756d 6e73 3d63 6f6c   sizeColumns=col
+0000e1d0: 735f 7369 7a65 2c0a 2020 2020 2020 2020  s_size,.        
+0000e1e0: 2020 2020 7469 746c 653d 7469 746c 652c      title=title,
+0000e1f0: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
+0000e200: 7065 7274 6965 733d 6469 6374 280a 2020  perties=dict(.  
+0000e210: 2020 2020 2020 2020 2020 2020 2020 636f                co
+0000e220: 6c75 6d6e 733d 636f 6c75 6d6e 735f 6469  lumns=columns_di
+0000e230: 6374 732c 0a20 2020 2020 2020 2020 2020  cts,.           
+0000e240: 2020 2020 2072 6f77 733d 726f 7773 5f64       rows=rows_d
+0000e250: 6963 742c 0a20 2020 2020 2020 2020 2020  ict,.           
+0000e260: 2020 2020 2063 6f6c 756d 6e73 4275 7474       columnsButt
+0000e270: 6f6e 3d63 6f6c 756d 6e73 5f62 7574 746f  on=columns_butto
+0000e280: 6e2c 0a20 2020 2020 2020 2020 2020 2020  n,.             
+0000e290: 2020 2066 696c 7465 7273 4275 7474 6f6e     filtersButton
+0000e2a0: 3d66 696c 7465 7273 2c0a 2020 2020 2020  =filters,.      
+0000e2b0: 2020 2020 2020 2020 2020 6578 706f 7274            export
+0000e2c0: 4275 7474 6f6e 3d65 7870 6f72 745f 746f  Button=export_to
+0000e2d0: 5f63 7376 2c0a 2020 2020 2020 2020 2020  _csv,.          
+0000e2e0: 2020 2020 2020 7365 6172 6368 3d73 6561        search=sea
+0000e2f0: 7263 682c 0a20 2020 2020 2020 2020 2020  rch,.           
+0000e300: 2020 2020 2070 6167 696e 6174 696f 6e3d       pagination=
+0000e310: 7061 6769 6e61 7469 6f6e 2c0a 2020 2020  pagination,.    
+0000e320: 2020 2020 2020 2020 2020 2020 736f 7274              sort
+0000e330: 3d73 6f72 742c 0a20 2020 2020 2020 2020  =sort,.         
+0000e340: 2020 2029 2c0a 2020 2020 2020 2020 290a     ),.        ).
+0000e350: 0a20 2020 2040 6164 645f 746f 5f67 656e  .    @add_to_gen
+0000e360: 6572 616c 5f61 7379 6e63 5f67 726f 7570  eral_async_group
+0000e370: 0a20 2020 2061 7379 6e63 2064 6566 2069  .    async def i
+0000e380: 6e70 7574 5f66 6f72 6d28 0a20 2020 2020  nput_form(.     
+0000e390: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+0000e3a0: 206f 7074 696f 6e73 3a20 6469 6374 2c0a   options: dict,.
+0000e3b0: 2020 2020 2020 2020 6f72 6465 723a 2069          order: i
+0000e3c0: 6e74 2c0a 2020 2020 2020 2020 7061 6464  nt,.        padd
+0000e3d0: 696e 673a 204f 7074 696f 6e61 6c5b 7374  ing: Optional[st
+0000e3e0: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
+0000e3f0: 2020 2072 6f77 735f 7369 7a65 3a20 4f70     rows_size: Op
+0000e400: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
+0000e410: 6e65 2c0a 2020 2020 2020 2020 636f 6c73  ne,.        cols
+0000e420: 5f73 697a 653a 204f 7074 696f 6e61 6c5b  _size: Optional[
+0000e430: 696e 745d 203d 204e 6f6e 652c 0a20 2020  int] = None,.   
+0000e440: 2020 2020 206d 6f64 616c 3a20 4f70 7469       modal: Opti
+0000e450: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+0000e460: 2c0a 2020 2020 2020 2020 6163 7469 7669  ,.        activi
+0000e470: 7479 5f69 643a 204f 7074 696f 6e61 6c5b  ty_id: Optional[
+0000e480: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
+0000e490: 2020 2020 2061 6374 6976 6974 795f 6e61       activity_na
+0000e4a0: 6d65 3a20 4f70 7469 6f6e 616c 5b73 7472  me: Optional[str
+0000e4b0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+0000e4c0: 2020 6163 7469 6f6e 5f69 643a 204f 7074    action_id: Opt
+0000e4d0: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+0000e4e0: 652c 0a20 2020 2020 2020 206f 6e5f 7375  e,.        on_su
+0000e4f0: 626d 6974 5f65 7665 6e74 733a 204f 7074  bmit_events: Opt
+0000e500: 696f 6e61 6c5b 6c69 7374 5b64 6963 745d  ional[list[dict]
+0000e510: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 293a  ] = None,.    ):
+0000e520: 0a20 2020 2020 2020 2022 2222 4372 6561  .        """Crea
+0000e530: 7465 7320 616e 2069 6e70 7574 2066 6f72  tes an input for
+0000e540: 6d2e 0a20 2020 2020 2020 203a 7061 7261  m..        :para
+0000e550: 6d20 6f70 7469 6f6e 733a 2074 6865 206f  m options: the o
+0000e560: 7074 696f 6e73 2066 6f72 2074 6865 2069  ptions for the i
+0000e570: 6e70 7574 2066 6f72 6d0a 2020 2020 2020  nput form.      
+0000e580: 2020 3a70 6172 616d 206f 7264 6572 3a20    :param order: 
+0000e590: 7468 6520 6f72 6465 7220 6f66 2074 6865  the order of the
+0000e5a0: 2069 6e70 7574 2066 6f72 6d0a 2020 2020   input form.    
+0000e5b0: 2020 2020 3a70 6172 616d 2070 6164 6469      :param paddi
+0000e5c0: 6e67 3a20 7468 6520 7061 6464 696e 6720  ng: the padding 
+0000e5d0: 6f66 2074 6865 2069 6e70 7574 2066 6f72  of the input for
+0000e5e0: 6d0a 2020 2020 2020 2020 3a70 6172 616d  m.        :param
+0000e5f0: 2072 6f77 735f 7369 7a65 3a20 7468 6520   rows_size: the 
+0000e600: 726f 7773 2073 697a 6520 6f66 2074 6865  rows size of the
+0000e610: 2069 6e70 7574 2066 6f72 6d0a 2020 2020   input form.    
+0000e620: 2020 2020 3a70 6172 616d 2063 6f6c 735f      :param cols_
+0000e630: 7369 7a65 3a20 7468 6520 636f 6c75 6d6e  size: the column
+0000e640: 7320 7369 7a65 206f 6620 7468 6520 696e  s size of the in
+0000e650: 7075 7420 666f 726d 0a20 2020 2020 2020  put form.       
+0000e660: 203a 7061 7261 6d20 6d6f 6461 6c3a 2074   :param modal: t
+0000e670: 6865 206d 6f64 616c 2074 6f20 6f70 656e  he modal to open
+0000e680: 2061 6674 6572 2073 7562 6d69 7474 696e   after submittin
+0000e690: 6720 7468 6520 666f 726d 0a20 2020 2020  g the form.     
+0000e6a0: 2020 203a 7061 7261 6d20 6163 7469 7669     :param activi
+0000e6b0: 7479 5f69 643a 2074 6865 2061 6374 6976  ty_id: the activ
+0000e6c0: 6974 7920 6964 2074 6f20 7275 6e20 6166  ity id to run af
+0000e6d0: 7465 7220 7375 626d 6974 7469 6e67 2074  ter submitting t
+0000e6e0: 6865 2066 6f72 6d0a 2020 2020 2020 2020  he form.        
+0000e6f0: 3a70 6172 616d 2061 6374 6976 6974 795f  :param activity_
+0000e700: 6e61 6d65 3a20 7468 6520 6163 7469 7669  name: the activi
+0000e710: 7479 206e 616d 6520 746f 2072 756e 2061  ty name to run a
+0000e720: 6674 6572 2073 7562 6d69 7474 696e 6720  fter submitting 
+0000e730: 7468 6520 666f 726d 0a20 2020 2020 2020  the form.       
+0000e740: 203a 7061 7261 6d20 6163 7469 6f6e 5f69   :param action_i
+0000e750: 643a 2074 6865 2061 6374 696f 6e20 6964  d: the action id
+0000e760: 2074 6f20 7275 6e20 6166 7465 7220 7375   to run after su
+0000e770: 626d 6974 7469 6e67 2074 6865 2066 6f72  bmitting the for
+0000e780: 6d0a 2020 2020 2020 2020 3a70 6172 616d  m.        :param
+0000e790: 206f 6e5f 7375 626d 6974 5f65 7665 6e74   on_submit_event
+0000e7a0: 733a 2074 6865 2065 7665 6e74 7320 746f  s: the events to
+0000e7b0: 2072 756e 2061 6674 6572 2073 7562 6d69   run after submi
+0000e7c0: 7474 696e 6720 7468 6520 666f 726d 0a20  tting the form. 
+0000e7d0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000e7e0: 2020 2076 616c 6964 6174 655f 696e 7075     validate_inpu
+0000e7f0: 745f 666f 726d 5f64 6174 6128 7365 6c66  t_form_data(self
+0000e800: 2c20 6f70 7469 6f6e 7329 0a0a 2020 2020  , options)..    
+0000e810: 2020 2020 6966 206f 6e5f 7375 626d 6974      if on_submit
+0000e820: 5f65 7665 6e74 7320 6973 204e 6f6e 653a  _events is None:
+0000e830: 0a20 2020 2020 2020 2020 2020 206f 6e5f  .            on_
+0000e840: 7375 626d 6974 5f65 7665 6e74 7320 3d20  submit_events = 
+0000e850: 5b5d 0a0a 2020 2020 2020 2020 6966 206d  []..        if m
+0000e860: 6f64 616c 3a0a 2020 2020 2020 2020 2020  odal:.          
+0000e870: 2020 6d6f 6461 6c5f 6964 203d 2028 6177    modal_id = (aw
+0000e880: 6169 7420 7365 6c66 2e5f 6765 745f 6d6f  ait self._get_mo
+0000e890: 6461 6c28 6d6f 6461 6c29 295b 2269 6422  dal(modal))["id"
+0000e8a0: 5d0a 2020 2020 2020 2020 2020 2020 6f6e  ].            on
+0000e8b0: 5f73 7562 6d69 745f 6576 656e 7473 2e61  _submit_events.a
+0000e8c0: 7070 656e 6428 0a20 2020 2020 2020 2020  ppend(.         
+0000e8d0: 2020 2020 2020 207b 2261 6374 696f 6e22         {"action"
+0000e8e0: 3a20 226f 7065 6e4d 6f64 616c 222c 2022  : "openModal", "
+0000e8f0: 7061 7261 6d73 223a 207b 226d 6f64 616c  params": {"modal
+0000e900: 4964 223a 206d 6f64 616c 5f69 647d 7d0a  Id": modal_id}}.
+0000e910: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
+0000e920: 2020 2020 2020 2069 6620 6163 7469 7669         if activi
+0000e930: 7479 5f69 6420 6f72 2061 6374 6976 6974  ty_id or activit
+0000e940: 795f 6e61 6d65 3a0a 2020 2020 2020 2020  y_name:.        
+0000e950: 2020 2020 6163 7469 7669 7479 5f69 6420      activity_id 
+0000e960: 3d20 2861 7761 6974 2073 656c 662e 5f61  = (await self._a
+0000e970: 7070 2e67 6574 5f61 6374 6976 6974 7928  pp.get_activity(
+0000e980: 6163 7469 7669 7479 5f69 642c 2061 6374  activity_id, act
+0000e990: 6976 6974 795f 6e61 6d65 2929 5b0a 2020  ivity_name))[.  
+0000e9a0: 2020 2020 2020 2020 2020 2020 2020 2269                "i
+0000e9b0: 6422 0a20 2020 2020 2020 2020 2020 205d  d".            ]
+0000e9c0: 0a0a 2020 2020 2020 2020 2020 2020 6f6e  ..            on
+0000e9d0: 5f73 7562 6d69 745f 6576 656e 7473 2e61  _submit_events.a
+0000e9e0: 7070 656e 6428 0a20 2020 2020 2020 2020  ppend(.         
+0000e9f0: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+0000ea00: 2020 2020 2020 2020 2020 2020 2022 6163               "ac
+0000ea10: 7469 6f6e 223a 2022 7275 6e41 6374 6976  tion": "runActiv
+0000ea20: 6974 7922 2c0a 2020 2020 2020 2020 2020  ity",.          
+0000ea30: 2020 2020 2020 2020 2020 2270 6172 616d            "param
+0000ea40: 7322 3a20 7b0a 2020 2020 2020 2020 2020  s": {.          
+0000ea50: 2020 2020 2020 2020 2020 2020 2020 2261                "a
+0000ea60: 6374 6976 6974 7949 6422 3a20 6163 7469  ctivityId": acti
+0000ea70: 7669 7479 5f69 642c 0a20 2020 2020 2020  vity_id,.       
+0000ea80: 2020 2020 2020 2020 2020 2020 207d 2c0a               },.
+0000ea90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eaa0: 7d0a 2020 2020 2020 2020 2020 2020 290a  }.            ).
+0000eab0: 0a20 2020 2020 2020 2069 6620 6163 7469  .        if acti
+0000eac0: 6f6e 5f69 643a 0a20 2020 2020 2020 2020  on_id:.         
+0000ead0: 2020 206f 6e5f 7375 626d 6974 5f65 7665     on_submit_eve
+0000eae0: 6e74 732e 6170 7065 6e64 280a 2020 2020  nts.append(.    
+0000eaf0: 2020 2020 2020 2020 2020 2020 7b0a 2020              {.  
+0000eb00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eb10: 2020 2261 6374 696f 6e22 3a20 2272 756e    "action": "run
+0000eb20: 4163 7469 6f6e 222c 0a20 2020 2020 2020  Action",.       
+0000eb30: 2020 2020 2020 2020 2020 2020 2022 7061               "pa
+0000eb40: 7261 6d73 223a 207b 0a20 2020 2020 2020  rams": {.       
+0000eb50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eb60: 2022 6163 7469 6f6e 4964 223a 2061 6374   "actionId": act
+0000eb70: 696f 6e5f 6964 2c0a 2020 2020 2020 2020  ion_id,.        
+0000eb80: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
+0000eb90: 2020 2020 2020 2020 2020 2020 2020 207d                 }
+0000eba0: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
+0000ebb0: 2020 2020 2020 2020 696e 6974 6961 6c5f          initial_
+0000ebc0: 6461 7461 3a20 6469 6374 203d 207b 7d0a  data: dict = {}.
+0000ebd0: 2020 2020 2020 2020 666f 7220 6669 656c          for fiel
+0000ebe0: 6473 2069 6e20 6f70 7469 6f6e 735b 2266  ds in options["f
+0000ebf0: 6965 6c64 7322 5d3a 0a20 2020 2020 2020  ields"]:.       
+0000ec00: 2020 2020 2066 6f72 2066 6965 6c64 2069       for field i
+0000ec10: 6e20 6669 656c 6473 5b22 6669 656c 6473  n fields["fields
+0000ec20: 225d 3a0a 2020 2020 2020 2020 2020 2020  "]:.            
+0000ec30: 2020 2020 6669 656c 645f 6e61 6d65 3a20      field_name: 
+0000ec40: 7374 7220 3d20 6669 656c 645b 2266 6965  str = field["fie
+0000ec50: 6c64 4e61 6d65 225d 0a20 2020 2020 2020  ldName"].       
+0000ec60: 2020 2020 2020 2020 2069 6e70 7574 5f74           input_t
+0000ec70: 7970 653a 204f 7074 696f 6e61 6c5b 7374  ype: Optional[st
+0000ec80: 725d 203d 2066 6965 6c64 2e67 6574 2822  r] = field.get("
+0000ec90: 696e 7075 7454 7970 6522 290a 2020 2020  inputType").    
+0000eca0: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+0000ecb0: 6e70 7574 5f74 7970 6520 3d3d 2022 636f  nput_type == "co
+0000ecc0: 6c6f 7222 3a0a 2020 2020 2020 2020 2020  lor":.          
+0000ecd0: 2020 2020 2020 2020 2020 696e 6974 6961            initia
+0000ece0: 6c5f 6461 7461 5b66 6965 6c64 5f6e 616d  l_data[field_nam
+0000ecf0: 655d 203d 2022 2330 3030 3030 3022 0a20  e] = "#000000". 
+0000ed00: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+0000ed10: 6c69 6620 696e 7075 745f 7479 7065 203d  lif input_type =
+0000ed20: 3d20 226e 756d 6265 7222 3a0a 2020 2020  = "number":.    
+0000ed30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ed40: 696e 6974 6961 6c5f 6461 7461 5b66 6965  initial_data[fie
+0000ed50: 6c64 5f6e 616d 655d 203d 2030 0a20 2020  ld_name] = 0.   
+0000ed60: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+0000ed70: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0000ed80: 2020 2020 2020 2069 6e69 7469 616c 5f64         initial_d
+0000ed90: 6174 615b 6669 656c 645f 6e61 6d65 5d20  ata[field_name] 
+0000eda0: 3d20 2222 0a0a 2020 2020 2020 2020 725f  = ""..        r_
+0000edb0: 6861 7368 2c20 7265 706f 7274 203d 2061  hash, report = a
+0000edc0: 7761 6974 2073 656c 662e 5f67 6574 5f63  wait self._get_c
+0000edd0: 6861 7274 5f72 6570 6f72 7428 6f72 6465  hart_report(orde
+0000ede0: 722c 2049 6e70 7574 466f 726d 290a 2020  r, InputForm).  
+0000edf0: 2020 2020 2020 5f2c 2064 6174 615f 7365        _, data_se
+0000ee00: 742c 205f 203d 206c 6973 7428 0a20 2020  t, _ = list(.   
+0000ee10: 2020 2020 2020 2020 2028 0a20 2020 2020           (.     
+0000ee20: 2020 2020 2020 2020 2020 2061 7761 6974             await
+0000ee30: 2073 656c 662e 5f63 7265 6174 655f 6461   self._create_da
+0000ee40: 7461 5f73 6574 2872 6570 6f72 745b 2269  ta_set(report["i
+0000ee50: 6422 5d2c 2069 6e69 7469 616c 5f64 6174  d"], initial_dat
+0000ee60: 612c 2064 756d 705f 7768 6f6c 653d 5472  a, dump_whole=Tr
+0000ee70: 7565 290a 2020 2020 2020 2020 2020 2020  ue).            
+0000ee80: 292e 7661 6c75 6573 2829 0a20 2020 2020  ).values().     
+0000ee90: 2020 2029 5b30 5d0a 0a20 2020 2020 2020     )[0]..       
+0000eea0: 2072 6473 203d 2061 7761 6974 2072 6570   rds = await rep
+0000eeb0: 6f72 742e 6765 745f 7265 706f 7274 5f64  ort.get_report_d
+0000eec0: 6174 615f 7365 7473 2829 0a20 2020 2020  ata_sets().     
+0000eed0: 2020 2069 6620 6c65 6e28 7264 7329 203e     if len(rds) >
+0000eee0: 2031 3a0a 2020 2020 2020 2020 2020 2020   1:.            
+0000eef0: 6c6f 675f 6572 726f 7228 0a20 2020 2020  log_error(.     
+0000ef00: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+0000ef10: 722c 0a20 2020 2020 2020 2020 2020 2020  r,.             
+0000ef20: 2020 2022 496e 7075 7420 666f 726d 2063     "Input form c
+0000ef30: 616e 206f 6e6c 7920 6861 7665 206f 6e65  an only have one
+0000ef40: 2063 6f6d 706f 6e65 6e74 2064 6174 6120   component data 
+0000ef50: 7365 7420 6c69 6e6b 2c20 220a 2020 2020  set link, ".    
+0000ef60: 2020 2020 2020 2020 2020 2020 2274 6869              "thi
+0000ef70: 7320 6973 2061 6e20 5344 4b20 6275 6720  s is an SDK bug 
+0000ef80: 706c 6561 7365 2072 6570 6f72 7420 6974  please report it
+0000ef90: 2061 6e64 2022 0a20 2020 2020 2020 2020   and ".         
+0000efa0: 2020 2020 2020 2022 6465 6c65 7465 2074         "delete t
+0000efb0: 6865 2066 6f72 6d20 746f 2073 6f6c 7665  he form to solve
+0000efc0: 2074 6865 2069 7373 7565 222c 0a20 2020   the issue",.   
+0000efd0: 2020 2020 2020 2020 2020 2020 2044 6174               Dat
+0000efe0: 6145 7272 6f72 2c0a 2020 2020 2020 2020  aError,.        
+0000eff0: 2020 2020 290a 0a20 2020 2020 2020 2069      )..        i
+0000f000: 6620 7264 7320 616e 6420 280a 2020 2020  f rds and (.    
+0000f010: 2020 2020 2020 2020 6e6f 7420 7365 6c66          not self
+0000f020: 2e72 6575 7365 5f64 6174 615f 7365 7473  .reuse_data_sets
+0000f030: 0a20 2020 2020 2020 2020 2020 206f 7220  .            or 
+0000f040: 7264 735b 305d 5b22 6461 7461 5365 7449  rds[0]["dataSetI
+0000f050: 6422 5d20 213d 2064 6174 615f 7365 745b  d"] != data_set[
+0000f060: 2269 6422 5d0a 2020 2020 2020 2020 2020  "id"].          
+0000f070: 2020 6f72 2072 6473 5b30 5d5b 2270 726f    or rds[0]["pro
+0000f080: 7065 7274 6965 7322 5d5b 2266 6965 6c64  perties"]["field
+0000f090: 7322 5d20 213d 206f 7074 696f 6e73 5b22  s"] != options["
+0000f0a0: 6669 656c 6473 225d 0a20 2020 2020 2020  fields"].       
+0000f0b0: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
+0000f0c0: 6177 6169 7420 7265 706f 7274 2e64 656c  await report.del
+0000f0d0: 6574 655f 7265 706f 7274 5f64 6174 615f  ete_report_data_
+0000f0e0: 7365 7473 286c 6f67 3d54 7275 6529 0a20  sets(log=True). 
+0000f0f0: 2020 2020 2020 2020 2020 2072 6473 203d             rds =
+0000f100: 205b 5d0a 0a20 2020 2020 2020 2069 6620   []..        if 
+0000f110: 6e6f 7420 7264 733a 0a20 2020 2020 2020  not rds:.       
+0000f120: 2020 2020 2061 7761 6974 2072 6570 6f72       await repor
+0000f130: 742e 6372 6561 7465 5f72 6570 6f72 745f  t.create_report_
+0000f140: 6461 7461 5f73 6574 280a 2020 2020 2020  data_set(.      
+0000f150: 2020 2020 2020 2020 2020 2822 6375 7374            ("cust
+0000f160: 6f6d 4669 656c 6431 222c 2064 6174 615f  omField1", data_
+0000f170: 7365 742c 204e 6f6e 6529 2c20 7072 6f70  set, None), prop
+0000f180: 6572 7469 6573 3d6f 7074 696f 6e73 0a20  erties=options. 
+0000f190: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0000f1a0: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
+0000f1b0: 696e 666f 2866 2243 7265 6174 6564 2031  info(f"Created 1
+0000f1c0: 2063 6f6d 706f 6e65 6e74 2064 6174 6120   component data 
+0000f1d0: 7365 7420 6c69 6e6b 2066 6f72 2069 6e70  set link for inp
+0000f1e0: 7574 2066 6f72 6d20 6174 207b 725f 6861  ut form at {r_ha
+0000f1f0: 7368 7d22 290a 0a20 2020 2020 2020 2061  sh}")..        a
+0000f200: 7761 6974 2073 656c 662e 5f63 7265 6174  wait self._creat
+0000f210: 655f 6368 6172 7428 0a20 2020 2020 2020  e_chart(.       
+0000f220: 2020 2020 2063 6861 7274 5f63 6c61 7373       chart_class
+0000f230: 3d49 6e70 7574 466f 726d 2c0a 2020 2020  =InputForm,.    
+0000f240: 2020 2020 2020 2020 6f72 6465 723d 6f72          order=or
+0000f250: 6465 722c 0a20 2020 2020 2020 2020 2020  der,.           
+0000f260: 2073 697a 6550 6164 6469 6e67 3d70 6164   sizePadding=pad
+0000f270: 6469 6e67 2c0a 2020 2020 2020 2020 2020  ding,.          
+0000f280: 2020 7369 7a65 526f 7773 3d72 6f77 735f    sizeRows=rows_
+0000f290: 7369 7a65 2c0a 2020 2020 2020 2020 2020  size,.          
+0000f2a0: 2020 7369 7a65 436f 6c75 6d6e 733d 636f    sizeColumns=co
+0000f2b0: 6c73 5f73 697a 652c 0a20 2020 2020 2020  ls_size,.       
+0000f2c0: 2020 2020 2070 726f 7065 7274 6965 733d       properties=
+0000f2d0: 7b22 6576 656e 7473 223a 207b 226f 6e53  {"events": {"onS
+0000f2e0: 7562 6d69 7422 3a20 6f6e 5f73 7562 6d69  ubmit": on_submi
+0000f2f0: 745f 6576 656e 7473 7d7d 2c0a 2020 2020  t_events}},.    
+0000f300: 2020 2020 290a 0a20 2020 2064 6566 2067      )..    def g
+0000f310: 656e 6572 6174 655f 696e 7075 745f 666f  enerate_input_fo
+0000f320: 726d 5f67 726f 7570 7328 0a20 2020 2020  rm_groups(.     
+0000f330: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+0000f340: 206f 7264 6572 3a20 696e 742c 0a20 2020   order: int,.   
+0000f350: 2020 2020 2066 6f72 6d5f 6772 6f75 7073       form_groups
+0000f360: 3a20 6469 6374 2c0a 2020 2020 2020 2020  : dict,.        
+0000f370: 6479 6e61 6d69 635f 7365 7175 656e 7469  dynamic_sequenti
+0000f380: 616c 5f73 686f 773a 204f 7074 696f 6e61  al_show: Optiona
+0000f390: 6c5b 626f 6f6c 5d20 3d20 4661 6c73 652c  l[bool] = False,
+0000f3a0: 0a20 2020 2020 2020 2061 7574 6f5f 7365  .        auto_se
+0000f3b0: 6e64 3a20 4f70 7469 6f6e 616c 5b62 6f6f  nd: Optional[boo
+0000f3c0: 6c5d 203d 2046 616c 7365 2c0a 2020 2020  l] = False,.    
+0000f3d0: 2020 2020 6e65 7874 5f67 726f 7570 5f6c      next_group_l
+0000f3e0: 6162 656c 3a20 4f70 7469 6f6e 616c 5b73  abel: Optional[s
+0000f3f0: 7472 5d20 3d20 224e 6578 7422 2c0a 2020  tr] = "Next",.  
+0000f400: 2020 2020 2020 726f 7773 5f73 697a 653a        rows_size:
+0000f410: 204f 7074 696f 6e61 6c5b 696e 745d 203d   Optional[int] =
+0000f420: 2033 2c0a 2020 2020 2020 2020 636f 6c73   3,.        cols
+0000f430: 5f73 697a 653a 2069 6e74 203d 2031 322c  _size: int = 12,
+0000f440: 0a20 2020 2020 2020 2070 6164 6469 6e67  .        padding
+0000f450: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
+0000f460: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+0000f470: 6d6f 6461 6c3a 204f 7074 696f 6e61 6c5b  modal: Optional[
+0000f480: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
+0000f490: 2020 2020 2061 6374 6976 6974 795f 6964       activity_id
+0000f4a0: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
+0000f4b0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+0000f4c0: 6163 7469 7669 7479 5f6e 616d 653a 204f  activity_name: O
+0000f4d0: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+0000f4e0: 6f6e 652c 0a20 2020 2020 2020 206f 6e5f  one,.        on_
+0000f4f0: 7375 626d 6974 5f65 7665 6e74 733a 204f  submit_events: O
+0000f500: 7074 696f 6e61 6c5b 6c69 7374 5b64 6963  ptional[list[dic
+0000f510: 745d 5d20 3d20 4e6f 6e65 2c0a 2020 2020  t]] = None,.    
+0000f520: 293a 0a20 2020 2020 2020 2022 2222 4561  ):.        """Ea
+0000f530: 7369 6572 2077 6179 2074 6f20 6372 6561  sier way to crea
+0000f540: 7465 2061 6e20 696e 7075 7420 666f 726d  te an input form
+0000f550: 2e0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
+0000f560: 206d 656e 755f 7061 7468 3a20 7468 6520   menu_path: the 
+0000f570: 6d65 6e75 2070 6174 6820 6f66 2074 6865  menu path of the
+0000f580: 2069 6e70 7574 2066 6f72 6d0a 2020 2020   input form.    
+0000f590: 2020 2020 3a70 6172 616d 206f 7264 6572      :param order
+0000f5a0: 3a20 7468 6520 6f72 6465 7220 6f66 2074  : the order of t
+0000f5b0: 6865 2069 6e70 7574 2066 6f72 6d0a 2020  he input form.  
+0000f5c0: 2020 2020 2020 3a70 6172 616d 2066 6f72        :param for
+0000f5d0: 6d5f 6772 6f75 7073 3a20 7468 6520 666f  m_groups: the fo
+0000f5e0: 726d 2067 726f 7570 7320 6f66 2074 6865  rm groups of the
+0000f5f0: 2069 6e70 7574 2066 6f72 6d0a 2020 2020   input form.    
+0000f600: 2020 2020 3a70 6172 616d 2064 796e 616d      :param dynam
+0000f610: 6963 5f73 6571 7565 6e74 6961 6c5f 7368  ic_sequential_sh
+0000f620: 6f77 3a20 7768 6574 6865 7220 746f 2073  ow: whether to s
+0000f630: 686f 7720 7468 6520 6e65 7874 2067 726f  how the next gro
+0000f640: 7570 2061 6674 6572 2073 7562 6d69 7474  up after submitt
+0000f650: 696e 6720 7468 6520 6375 7272 656e 7420  ing the current 
+0000f660: 6772 6f75 700a 2020 2020 2020 2020 3a70  group.        :p
+0000f670: 6172 616d 2061 7574 6f5f 7365 6e64 3a20  aram auto_send: 
+0000f680: 7768 6574 6865 7220 746f 2061 7574 6f6d  whether to autom
+0000f690: 6174 6963 616c 6c79 2073 656e 6420 7468  atically send th
+0000f6a0: 6520 666f 726d 2061 6674 6572 2074 6865  e form after the
+0000f6b0: 206c 6173 7420 6772 6f75 700a 2020 2020   last group.    
+0000f6c0: 2020 2020 3a70 6172 616d 206e 6578 745f      :param next_
+0000f6d0: 6772 6f75 705f 6c61 6265 6c3a 2074 6865  group_label: the
+0000f6e0: 206c 6162 656c 206f 6620 7468 6520 6e65   label of the ne
+0000f6f0: 7874 2067 726f 7570 2062 7574 746f 6e0a  xt group button.
+0000f700: 2020 2020 2020 2020 3a70 6172 616d 2072          :param r
+0000f710: 6f77 735f 7369 7a65 3a20 7468 6520 726f  ows_size: the ro
+0000f720: 7773 2073 697a 6520 6f66 2074 6865 2069  ws size of the i
+0000f730: 6e70 7574 2066 6f72 6d0a 2020 2020 2020  nput form.      
+0000f740: 2020 3a70 6172 616d 2063 6f6c 735f 7369    :param cols_si
+0000f750: 7a65 3a20 7468 6520 636f 6c75 6d6e 7320  ze: the columns 
+0000f760: 7369 7a65 206f 6620 7468 6520 696e 7075  size of the inpu
+0000f770: 7420 666f 726d 0a20 2020 2020 2020 203a  t form.        :
+0000f780: 7061 7261 6d20 7061 6464 696e 673a 2074  param padding: t
+0000f790: 6865 2070 6164 6469 6e67 206f 6620 7468  he padding of th
+0000f7a0: 6520 696e 7075 7420 666f 726d 0a20 2020  e input form.   
+0000f7b0: 2020 2020 203a 7061 7261 6d20 6d6f 6461       :param moda
+0000f7c0: 6c3a 2074 6865 206d 6f64 616c 2074 6f20  l: the modal to 
+0000f7d0: 6f70 656e 2061 6674 6572 2073 7562 6d69  open after submi
+0000f7e0: 7474 696e 6720 7468 6520 666f 726d 0a20  tting the form. 
+0000f7f0: 2020 2020 2020 203a 7061 7261 6d20 6163         :param ac
+0000f800: 7469 7669 7479 5f69 643a 2074 6865 2061  tivity_id: the a
+0000f810: 6374 6976 6974 7920 6964 2074 6f20 7275  ctivity id to ru
+0000f820: 6e20 6166 7465 7220 7375 626d 6974 7469  n after submitti
+0000f830: 6e67 2074 6865 2066 6f72 6d0a 2020 2020  ng the form.    
+0000f840: 2020 2020 3a70 6172 616d 2061 6374 6976      :param activ
+0000f850: 6974 795f 6e61 6d65 3a20 7468 6520 6163  ity_name: the ac
+0000f860: 7469 7669 7479 206e 616d 6520 746f 2072  tivity name to r
+0000f870: 756e 2061 6674 6572 2073 7562 6d69 7474  un after submitt
+0000f880: 696e 6720 7468 6520 666f 726d 0a20 2020  ing the form.   
+0000f890: 2020 2020 203a 7061 7261 6d20 6f6e 5f73       :param on_s
+0000f8a0: 7562 6d69 745f 6576 656e 7473 3a20 7468  ubmit_events: th
+0000f8b0: 6520 6576 656e 7473 2074 6f20 7275 6e20  e events to run 
+0000f8c0: 6166 7465 7220 7375 626d 6974 7469 6e67  after submitting
+0000f8d0: 2074 6865 2066 6f72 6d0a 2020 2020 2020   the form.      
+0000f8e0: 2020 2222 220a 2020 2020 2020 2020 7265    """.        re
+0000f8f0: 706f 7274 5f64 6174 615f 7365 745f 7072  port_data_set_pr
+0000f900: 6f70 6572 7469 6573 203d 207b 2266 6965  operties = {"fie
+0000f910: 6c64 7322 3a20 5b5d 7d0a 2020 2020 2020  lds": []}.      
+0000f920: 2020 6966 2061 7574 6f5f 7365 6e64 3a0a    if auto_send:.
+0000f930: 2020 2020 2020 2020 2020 2020 7265 706f              repo
+0000f940: 7274 5f64 6174 615f 7365 745f 7072 6f70  rt_data_set_prop
+0000f950: 6572 7469 6573 5b22 7661 7269 616e 7422  erties["variant"
+0000f960: 5d20 3d20 2261 7574 6f53 656e 6422 0a0a  ] = "autoSend"..
+0000f970: 2020 2020 2020 2020 725f 6861 7368 203d          r_hash =
+0000f980: 2073 656c 662e 5f67 6574 5f63 6861 7274   self._get_chart
+0000f990: 5f68 6173 6828 6f72 6465 7229 0a0a 2020  _hash(order)..  
+0000f9a0: 2020 2020 2020 6e65 7874 5f69 6420 3d20        next_id = 
+0000f9b0: 6622 7b72 5f68 6173 687d 5f30 2220 6966  f"{r_hash}_0" if
+0000f9c0: 2064 796e 616d 6963 5f73 6571 7565 6e74   dynamic_sequent
+0000f9d0: 6961 6c5f 7368 6f77 2065 6c73 6520 4e6f  ial_show else No
+0000f9e0: 6e65 0a0a 2020 2020 2020 2020 6e65 7874  ne..        next
+0000f9f0: 5f67 726f 7570 5f69 6e64 6578 203d 2031  _group_index = 1
+0000fa00: 0a20 2020 2020 2020 2066 6f72 2066 6f72  .        for for
+0000fa10: 6d5f 6772 6f75 705f 6e61 6d65 2c20 666f  m_group_name, fo
+0000fa20: 726d 5f67 726f 7570 2069 6e20 666f 726d  rm_group in form
+0000fa30: 5f67 726f 7570 732e 6974 656d 7328 293a  _groups.items():
+0000fa40: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+0000fa50: 6d5f 6772 6f75 705f 6a73 6f6e 203d 207b  m_group_json = {
+0000fa60: 2274 6974 6c65 223a 2066 6f72 6d5f 6772  "title": form_gr
+0000fa70: 6f75 705f 6e61 6d65 2c20 2266 6965 6c64  oup_name, "field
+0000fa80: 7322 3a20 666f 726d 5f67 726f 7570 7d0a  s": form_group}.
+0000fa90: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+0000faa0: 6578 745f 6964 3a0a 2020 2020 2020 2020  ext_id:.        
+0000fab0: 2020 2020 2020 2020 666f 726d 5f67 726f          form_gro
+0000fac0: 7570 5f6a 736f 6e5b 2269 6422 5d20 3d20  up_json["id"] = 
+0000fad0: 6e65 7874 5f69 640a 2020 2020 2020 2020  next_id.        
+0000fae0: 2020 2020 2020 2020 6e65 7874 5f69 6420          next_id 
+0000faf0: 3d20 6622 7b72 5f68 6173 687d 5f7b 6e65  = f"{r_hash}_{ne
+0000fb00: 7874 5f67 726f 7570 5f69 6e64 6578 7d22  xt_group_index}"
+0000fb10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000fb20: 2066 6f72 6d5f 6772 6f75 705f 6a73 6f6e   form_group_json
+0000fb30: 5b22 6e65 7874 466f 726d 4772 6f75 7022  ["nextFormGroup"
+0000fb40: 5d20 3d20 7b0a 2020 2020 2020 2020 2020  ] = {.          
+0000fb50: 2020 2020 2020 2020 2020 2269 6422 3a20            "id": 
+0000fb60: 6e65 7874 5f69 642c 0a20 2020 2020 2020  next_id,.       
+0000fb70: 2020 2020 2020 2020 2020 2020 2022 6c61               "la
+0000fb80: 6265 6c22 3a20 6e65 7874 5f67 726f 7570  bel": next_group
+0000fb90: 5f6c 6162 656c 2c0a 2020 2020 2020 2020  _label,.        
+0000fba0: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+0000fbb0: 2020 2020 2020 2020 2020 6e65 7874 5f67            next_g
+0000fbc0: 726f 7570 5f69 6e64 6578 202b 3d20 310a  roup_index += 1.
+0000fbd0: 2020 2020 2020 2020 2020 2020 7265 706f              repo
+0000fbe0: 7274 5f64 6174 615f 7365 745f 7072 6f70  rt_data_set_prop
+0000fbf0: 6572 7469 6573 5b22 6669 656c 6473 225d  erties["fields"]
+0000fc00: 202b 3d20 5b66 6f72 6d5f 6772 6f75 705f   += [form_group_
+0000fc10: 6a73 6f6e 5d0a 0a20 2020 2020 2020 2069  json]..        i
+0000fc20: 6620 6e65 7874 5f69 643a 0a20 2020 2020  f next_id:.     
+0000fc30: 2020 2020 2020 2064 656c 2072 6570 6f72         del repor
+0000fc40: 745f 6461 7461 5f73 6574 5f70 726f 7065  t_data_set_prope
+0000fc50: 7274 6965 735b 2266 6965 6c64 7322 5d5b  rties["fields"][
+0000fc60: 2d31 5d5b 226e 6578 7446 6f72 6d47 726f  -1]["nextFormGro
+0000fc70: 7570 225d 0a0a 2020 2020 2020 2020 7365  up"]..        se
+0000fc80: 6c66 2e69 6e70 7574 5f66 6f72 6d28 0a20  lf.input_form(. 
+0000fc90: 2020 2020 2020 2020 2020 206f 7074 696f             optio
+0000fca0: 6e73 3d72 6570 6f72 745f 6461 7461 5f73  ns=report_data_s
+0000fcb0: 6574 5f70 726f 7065 7274 6965 732c 0a20  et_properties,. 
+0000fcc0: 2020 2020 2020 2020 2020 206f 7264 6572             order
+0000fcd0: 3d6f 7264 6572 2c0a 2020 2020 2020 2020  =order,.        
+0000fce0: 2020 2020 726f 7773 5f73 697a 653d 726f      rows_size=ro
+0000fcf0: 7773 5f73 697a 652c 0a20 2020 2020 2020  ws_size,.       
+0000fd00: 2020 2020 2063 6f6c 735f 7369 7a65 3d63       cols_size=c
+0000fd10: 6f6c 735f 7369 7a65 2c0a 2020 2020 2020  ols_size,.      
+0000fd20: 2020 2020 2020 7061 6464 696e 673d 7061        padding=pa
+0000fd30: 6464 696e 672c 0a20 2020 2020 2020 2020  dding,.         
+0000fd40: 2020 206d 6f64 616c 3d6d 6f64 616c 2c0a     modal=modal,.
+0000fd50: 2020 2020 2020 2020 2020 2020 6163 7469              acti
+0000fd60: 7669 7479 5f69 643d 6163 7469 7669 7479  vity_id=activity
+0000fd70: 5f69 642c 0a20 2020 2020 2020 2020 2020  _id,.           
+0000fd80: 2061 6374 6976 6974 795f 6e61 6d65 3d61   activity_name=a
+0000fd90: 6374 6976 6974 795f 6e61 6d65 2c0a 2020  ctivity_name,.  
+0000fda0: 2020 2020 2020 2020 2020 6f6e 5f73 7562            on_sub
+0000fdb0: 6d69 745f 6576 656e 7473 3d6f 6e5f 7375  mit_events=on_su
+0000fdc0: 626d 6974 5f65 7665 6e74 732c 0a20 2020  bmit_events,.   
+0000fdd0: 2020 2020 2029 0a0a 2020 2020 6173 796e       )..    asyn
+0000fde0: 6320 6465 6620 5f67 6574 5f69 6e70 7574  c def _get_input
+0000fdf0: 5f66 6f72 6d5f 6461 7461 2873 656c 662c  _form_data(self,
+0000fe00: 2069 6e70 7574 5f66 6f72 6d3a 2049 6e70   input_form: Inp
+0000fe10: 7574 466f 726d 2920 2d3e 2064 6963 743a  utForm) -> dict:
+0000fe20: 0a20 2020 2020 2020 2022 2222 4765 7420  .        """Get 
+0000fe30: 7468 6520 696e 7075 7420 666f 726d 2064  the input form d
+0000fe40: 6174 612e 2222 220a 2020 2020 2020 2020  ata.""".        
+0000fe50: 7265 706f 7274 5f64 6174 615f 7365 7420  report_data_set 
+0000fe60: 3d20 2861 7761 6974 2069 6e70 7574 5f66  = (await input_f
+0000fe70: 6f72 6d2e 6765 745f 7265 706f 7274 5f64  orm.get_report_d
+0000fe80: 6174 615f 7365 7473 2829 295b 305d 0a20  ata_sets())[0]. 
+0000fe90: 2020 2020 2020 2064 6174 615f 7365 7420         data_set 
+0000fea0: 3d20 6177 6169 7420 7365 6c66 2e5f 6170  = await self._ap
+0000feb0: 702e 6765 745f 6461 7461 5f73 6574 2872  p.get_data_set(r
+0000fec0: 6570 6f72 745f 6461 7461 5f73 6574 5b22  eport_data_set["
+0000fed0: 6461 7461 5365 7449 6422 5d29 0a20 2020  dataSetId"]).   
+0000fee0: 2020 2020 2064 6174 615f 706f 696e 7420       data_point 
+0000fef0: 3d20 6177 6169 7420 6461 7461 5f73 6574  = await data_set
+0000ff00: 2e67 6574 5f6f 6e65 5f64 6174 615f 706f  .get_one_data_po
+0000ff10: 696e 7428 290a 2020 2020 2020 2020 6c6f  int().        lo
+0000ff20: 6767 6572 2e69 6e66 6f28 6622 476f 7420  gger.info(f"Got 
+0000ff30: 696e 7075 7420 666f 726d 2064 6174 6120  input form data 
+0000ff40: 666f 7220 7b73 7472 2869 6e70 7574 5f66  for {str(input_f
+0000ff50: 6f72 6d29 7d22 290a 2020 2020 2020 2020  orm)}").        
+0000ff60: 7265 7475 726e 207b 0a20 2020 2020 2020  return {.       
+0000ff70: 2020 2020 2022 7265 706f 7274 4964 223a       "reportId":
+0000ff80: 2069 6e70 7574 5f66 6f72 6d5b 2269 6422   input_form["id"
+0000ff90: 5d2c 0a20 2020 2020 2020 2020 2020 2022  ],.            "
+0000ffa0: 6f72 6465 7222 3a20 696e 7075 745f 666f  order": input_fo
+0000ffb0: 726d 5b22 6f72 6465 7222 5d2c 0a20 2020  rm["order"],.   
+0000ffc0: 2020 2020 2020 2020 2022 6461 7461 223a           "data":
+0000ffd0: 2064 6174 615f 706f 696e 745b 2263 7573   data_point["cus
+0000ffe0: 746f 6d46 6965 6c64 3122 5d20 6966 2064  tomField1"] if d
+0000fff0: 6174 615f 706f 696e 7420 656c 7365 204e  ata_point else N
+00010000: 6f6e 652c 0a20 2020 2020 2020 207d 0a0a  one,.        }..
+00010010: 2020 2020 6173 796e 6320 6465 6620 6765      async def ge
+00010020: 745f 696e 7075 745f 666f 726d 7328 7365  t_input_forms(se
+00010030: 6c66 2920 2d3e 206c 6973 745b 6469 6374  lf) -> list[dict
+00010040: 5d3a 0a20 2020 2020 2020 2022 2222 4765  ]:.        """Ge
+00010050: 7420 616c 6c20 7468 6520 696e 7075 7420  t all the input 
+00010060: 666f 726d 7320 696e 2074 6865 2063 7572  forms in the cur
+00010070: 7265 6e74 206d 656e 755f 7061 7468 2e22  rent menu_path."
+00010080: 2222 0a20 2020 2020 2020 2072 6570 6f72  "".        repor
+00010090: 7473 3a20 6c69 7374 203d 205b 0a20 2020  ts: list = [.   
+000100a0: 2020 2020 2020 2020 2072 6570 6f72 740a           report.
+000100b0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+000100c0: 7265 706f 7274 2069 6e20 6177 6169 7420  report in await 
+000100d0: 7365 6c66 2e5f 6170 702e 6765 745f 7265  self._app.get_re
+000100e0: 706f 7274 7328 290a 2020 2020 2020 2020  ports().        
+000100f0: 2020 2020 6966 2072 6570 6f72 745b 2272      if report["r
+00010100: 6570 6f72 7454 7970 6522 5d20 3d3d 2022  eportType"] == "
+00010110: 464f 524d 220a 2020 2020 2020 2020 2020  FORM".          
+00010120: 2020 616e 6420 2872 6570 6f72 745b 2270    and (report["p
+00010130: 6174 6822 5d20 3d3d 2073 656c 662e 5f63  ath"] == self._c
+00010140: 7572 7265 6e74 5f70 6174 6820 6f72 206e  urrent_path or n
+00010150: 6f74 2073 656c 662e 5f63 7572 7265 6e74  ot self._current
+00010160: 5f70 6174 6829 0a20 2020 2020 2020 205d  _path).        ]
+00010170: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00010180: 6c69 7374 280a 2020 2020 2020 2020 2020  list(.          
+00010190: 2020 6177 6169 7420 6173 796e 6369 6f2e    await asyncio.
+000101a0: 6761 7468 6572 280a 2020 2020 2020 2020  gather(.        
+000101b0: 2020 2020 2020 2020 2a5b 7365 6c66 2e5f          *[self._
+000101c0: 6765 745f 696e 7075 745f 666f 726d 5f64  get_input_form_d
+000101d0: 6174 6128 7265 706f 7274 2920 666f 7220  ata(report) for 
+000101e0: 7265 706f 7274 2069 6e20 7265 706f 7274  report in report
+000101f0: 735d 0a20 2020 2020 2020 2020 2020 2029  s].            )
+00010200: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+00010210: 4061 6464 5f74 6f5f 6765 6e65 7261 6c5f  @add_to_general_
+00010220: 6173 796e 635f 6772 6f75 700a 2020 2020  async_group.    
+00010230: 6173 796e 6320 6465 6620 616e 6e6f 7461  async def annota
+00010240: 7465 645f 6368 6172 7428 0a20 2020 2020  ted_chart(.     
+00010250: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+00010260: 2064 6174 613a 2055 6e69 6f6e 5b6c 6973   data: Union[lis
+00010270: 745b 4461 7461 4672 616d 655d 2c20 6c69  t[DataFrame], li
+00010280: 7374 5b6c 6973 745b 6469 6374 5d5d 5d2c  st[list[dict]]],
+00010290: 0a20 2020 2020 2020 206f 7264 6572 3a20  .        order: 
+000102a0: 696e 742c 0a20 2020 2020 2020 2078 3a20  int,.        x: 
+000102b0: 7374 722c 0a20 2020 2020 2020 2079 3a20  str,.        y: 
+000102c0: 556e 696f 6e5b 7374 722c 206c 6973 745b  Union[str, list[
+000102d0: 7374 725d 5d2c 0a20 2020 2020 2020 2061  str]],.        a
+000102e0: 6e6e 6f74 6174 696f 6e73 3a20 7374 7220  nnotations: str 
+000102f0: 3d20 2261 6e6e 6f74 6174 696f 6e22 2c0a  = "annotation",.
+00010300: 2020 2020 2020 2020 726f 7773 5f73 697a          rows_siz
+00010310: 653a 204f 7074 696f 6e61 6c5b 696e 745d  e: Optional[int]
+00010320: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+00010330: 2063 6f6c 735f 7369 7a65 3a20 4f70 7469   cols_size: Opti
+00010340: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
+00010350: 2c0a 2020 2020 2020 2020 7061 6464 696e  ,.        paddin
+00010360: 673a 204f 7074 696f 6e61 6c5b 7374 725d  g: Optional[str]
+00010370: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+00010380: 2074 6974 6c65 3a20 4f70 7469 6f6e 616c   title: Optional
+00010390: 5b73 7472 5d20 3d20 4e6f 6e65 2c0a 2020  [str] = None,.  
+000103a0: 2020 2020 2020 795f 6178 6973 5f6e 616d        y_axis_nam
+000103b0: 653a 204f 7074 696f 6e61 6c5b 7374 725d  e: Optional[str]
+000103c0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+000103d0: 2073 6c69 6465 725f 636f 6e66 6967 3a20   slider_config: 
+000103e0: 4f70 7469 6f6e 616c 5b64 6963 745d 203d  Optional[dict] =
+000103f0: 204e 6f6e 652c 0a20 2020 2020 2020 2073   None,.        s
+00010400: 6c69 6465 725f 6d61 726b 733a 204f 7074  lider_marks: Opt
+00010410: 696f 6e61 6c5b 6c69 7374 5b74 7570 6c65  ional[list[tuple
+00010420: 5d5d 203d 204e 6f6e 652c 0a20 2020 2029  ]] = None,.    )
+00010430: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00010440: 2020 2020 2020 4372 6561 7465 2061 6e20        Create an 
+00010450: 616e 6e6f 7461 7465 6420 6368 6172 7420  annotated chart 
+00010460: 696e 2074 6865 206d 656e 7520 7061 7468  in the menu path
+00010470: 2e0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
+00010480: 2064 6174 613a 2074 6865 2064 6174 6120   data: the data 
+00010490: 6f66 2074 6865 2063 6861 7274 0a20 2020  of the chart.   
+000104a0: 2020 2020 203a 7061 7261 6d20 6f72 6465       :param orde
+000104b0: 723a 2074 6865 206f 7264 6572 206f 6620  r: the order of 
+000104c0: 7468 6520 6368 6172 740a 2020 2020 2020  the chart.      
+000104d0: 2020 3a70 6172 616d 2078 3a20 7468 6520    :param x: the 
+000104e0: 7820 6178 6973 0a20 2020 2020 2020 203a  x axis.        :
+000104f0: 7061 7261 6d20 793a 2074 6865 2079 2061  param y: the y a
+00010500: 7869 730a 2020 2020 2020 2020 3a70 6172  xis.        :par
+00010510: 616d 2061 6e6e 6f74 6174 696f 6e73 3a20  am annotations: 
+00010520: 7468 6520 616e 6e6f 7461 7469 6f6e 730a  the annotations.
+00010530: 2020 2020 2020 2020 3a70 6172 616d 2072          :param r
+00010540: 6f77 735f 7369 7a65 3a20 7468 6520 726f  ows_size: the ro
+00010550: 7773 2073 697a 6520 6f66 2074 6865 2063  ws size of the c
+00010560: 6861 7274 0a20 2020 2020 2020 203a 7061  hart.        :pa
+00010570: 7261 6d20 636f 6c73 5f73 697a 653a 2074  ram cols_size: t
+00010580: 6865 2063 6f6c 756d 6e73 2073 697a 6520  he columns size 
+00010590: 6f66 2074 6865 2063 6861 7274 0a20 2020  of the chart.   
+000105a0: 2020 2020 203a 7061 7261 6d20 7061 6464       :param padd
+000105b0: 696e 673a 2074 6865 2070 6164 6469 6e67  ing: the padding
+000105c0: 206f 6620 7468 6520 6368 6172 740a 2020   of the chart.  
+000105d0: 2020 2020 2020 3a70 6172 616d 2074 6974        :param tit
+000105e0: 6c65 3a20 7468 6520 7469 746c 6520 6f66  le: the title of
+000105f0: 2074 6865 2063 6861 7274 0a20 2020 2020   the chart.     
+00010600: 2020 203a 7061 7261 6d20 795f 6178 6973     :param y_axis
+00010610: 5f6e 616d 653a 2074 6865 206e 616d 6520  _name: the name 
+00010620: 6f66 2074 6865 2079 2061 7869 730a 2020  of the y axis.  
+00010630: 2020 2020 2020 3a70 6172 616d 2073 6c69        :param sli
+00010640: 6465 725f 636f 6e66 6967 3a20 7468 6520  der_config: the 
+00010650: 736c 6964 6572 2063 6f6e 6669 670a 2020  slider config.  
+00010660: 2020 2020 2020 3a70 6172 616d 2073 6c69        :param sli
+00010670: 6465 725f 6d61 726b 733a 2074 6865 2073  der_marks: the s
+00010680: 6c69 6465 7220 6d61 726b 730a 2020 2020  lider marks.    
+00010690: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+000106a0: 6966 2069 7369 6e73 7461 6e63 6528 6461  if isinstance(da
+000106b0: 7461 2c20 7374 7229 3a0a 2020 2020 2020  ta, str):.      
+000106c0: 2020 2020 2020 6c6f 675f 6572 726f 7228        log_error(
+000106d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000106e0: 206c 6f67 6765 722c 0a20 2020 2020 2020   logger,.       
+000106f0: 2020 2020 2020 2020 2022 416e 6e6f 7461           "Annota
+00010700: 7465 6420 6368 6172 7420 646f 6573 206e  ted chart does n
+00010710: 6f74 2073 7570 706f 7274 2074 6865 2075  ot support the u
+00010720: 7365 206f 6620 7368 6172 6564 2064 6174  se of shared dat
+00010730: 6122 2c0a 2020 2020 2020 2020 2020 2020  a",.            
+00010740: 2020 2020 4461 7461 4572 726f 722c 0a20      DataError,. 
+00010750: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
+00010760: 2020 2020 2020 6966 2073 6c69 6465 725f        if slider_
+00010770: 636f 6e66 6967 2069 7320 4e6f 6e65 3a0a  config is None:.
+00010780: 2020 2020 2020 2020 2020 2020 736c 6964              slid
+00010790: 6572 5f63 6f6e 6669 6720 3d20 7b7d 0a0a  er_config = {}..
+000107a0: 2020 2020 2020 2020 6966 2073 6c69 6465          if slide
+000107b0: 725f 6d61 726b 733a 0a20 2020 2020 2020  r_marks:.       
+000107c0: 2020 2020 2073 6c69 6465 725f 636f 6e66       slider_conf
+000107d0: 6967 5b22 6d61 726b 7322 5d20 3d20 5b0a  ig["marks"] = [.
+000107e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000107f0: 7b22 6c61 6265 6c22 3a20 6d61 726b 5b30  {"label": mark[0
+00010800: 5d2c 2022 7661 6c75 6522 3a20 6d61 726b  ], "value": mark
+00010810: 5b31 5d7d 2066 6f72 206d 6172 6b20 696e  [1]} for mark in
+00010820: 2073 6c69 6465 725f 6d61 726b 730a 2020   slider_marks.  
+00010830: 2020 2020 2020 2020 2020 5d0a 0a20 2020            ]..   
+00010840: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
+00010850: 6365 2879 2c20 7374 7229 3a0a 2020 2020  ce(y, str):.    
+00010860: 2020 2020 2020 2020 7920 3d20 5b79 5d0a          y = [y].
+00010870: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+00010880: 6c65 6e28 7929 203d 3d20 6c65 6e28 6461  len(y) == len(da
+00010890: 7461 293a 0a20 2020 2020 2020 2020 2020  ta):.           
+000108a0: 206c 6f67 5f65 7272 6f72 280a 2020 2020   log_error(.    
+000108b0: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
+000108c0: 6572 2c0a 2020 2020 2020 2020 2020 2020  er,.            
+000108d0: 2020 2020 6622 4e75 6d62 6572 206f 6620      f"Number of 
+000108e0: 7920 7661 6c75 6573 2028 7b6c 656e 2879  y values ({len(y
+000108f0: 297d 2920 646f 6573 206e 6f74 206d 6174  )}) does not mat
+00010900: 6368 206e 756d 6265 7220 6f66 2064 6174  ch number of dat
+00010910: 6166 7261 6d65 7320 287b 6c65 6e28 6461  aframes ({len(da
+00010920: 7461 297d 2922 2c0a 2020 2020 2020 2020  ta)})",.        
+00010930: 2020 2020 2020 2020 4461 7461 4572 726f          DataErro
+00010940: 722c 0a20 2020 2020 2020 2020 2020 2029  r,.            )
+00010950: 0a0a 2020 2020 2020 2020 5f2c 2072 6570  ..        _, rep
+00010960: 6f72 7420 3d20 6177 6169 7420 7365 6c66  ort = await self
+00010970: 2e5f 6765 745f 6368 6172 745f 7265 706f  ._get_chart_repo
+00010980: 7274 286f 7264 6572 2c20 416e 6e6f 7461  rt(order, Annota
+00010990: 7465 6445 4368 6172 7429 0a0a 2020 2020  tedEChart)..    
+000109a0: 2020 2020 6466 7320 3d20 5b76 616c 6964      dfs = [valid
+000109b0: 6174 655f 6461 7461 5f69 735f 7061 6e64  ate_data_is_pand
+000109c0: 6172 6162 6c65 2864 6629 2066 6f72 2064  arable(df) for d
+000109d0: 6620 696e 2064 6174 615d 0a20 2020 2020  f in data].     
+000109e0: 2020 2064 6174 615f 7365 745f 7461 736b     data_set_task
+000109f0: 7320 3d20 5b5d 0a20 2020 2020 2020 2066  s = [].        f
+00010a00: 6f72 2064 662c 2079 5f76 616c 2069 6e20  or df, y_val in 
+00010a10: 7a69 7028 6466 732c 2079 293a 0a20 2020  zip(dfs, y):.   
+00010a20: 2020 2020 2020 2020 2064 665b 785d 203d           df[x] =
+00010a30: 2070 642e 746f 5f64 6174 6574 696d 6528   pd.to_datetime(
+00010a40: 6466 5b78 5d29 0a20 2020 2020 2020 2020  df[x]).         
+00010a50: 2020 2069 6620 616e 6e6f 7461 7469 6f6e     if annotation
+00010a60: 7320 696e 2064 663a 0a20 2020 2020 2020  s in df:.       
+00010a70: 2020 2020 2020 2020 2064 665b 616e 6e6f           df[anno
+00010a80: 7461 7469 6f6e 735d 203d 2028 0a20 2020  tations] = (.   
+00010a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010aa0: 2064 665b 616e 6e6f 7461 7469 6f6e 735d   df[annotations]
+00010ab0: 2e72 6570 6c61 6365 286e 702e 6e61 6e2c  .replace(np.nan,
+00010ac0: 2022 222c 2072 6567 6578 3d54 7275 6529   "", regex=True)
+00010ad0: 2e61 7374 7970 6528 7374 7229 0a20 2020  .astype(str).   
+00010ae0: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+00010af0: 2020 2020 2020 2020 2020 2064 6174 615f             data_
+00010b00: 7365 745f 7461 736b 732e 6170 7065 6e64  set_tasks.append
+00010b10: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00010b20: 2020 7365 6c66 2e5f 6372 6561 7465 5f64    self._create_d
+00010b30: 6174 615f 7365 7428 6e61 6d65 3d66 227b  ata_set(name=f"{
+00010b40: 7265 706f 7274 5b27 6964 275d 7d5f 7b79  report['id']}_{y
+00010b50: 5f76 616c 7d22 2c20 6461 7461 3d64 6629  _val}", data=df)
+00010b60: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
+00010b70: 2020 2020 2020 2020 6461 7461 5f73 6574          data_set
+00010b80: 5f64 6963 7473 203d 2061 7761 6974 2061  _dicts = await a
+00010b90: 7379 6e63 696f 2e67 6174 6865 7228 2a64  syncio.gather(*d
+00010ba0: 6174 615f 7365 745f 7461 736b 7329 0a20  ata_set_tasks). 
+00010bb0: 2020 2020 2020 2064 6174 615f 7365 7473         data_sets
+00010bc0: 203d 205b 6473 5b79 5f76 616c 5d5b 315d   = [ds[y_val][1]
+00010bd0: 2066 6f72 2064 732c 2079 5f76 616c 2069   for ds, y_val i
+00010be0: 6e20 7a69 7028 6461 7461 5f73 6574 5f64  n zip(data_set_d
+00010bf0: 6963 7473 2c20 7929 5d0a 0a20 2020 2020  icts, y)]..     
+00010c00: 2020 2072 645f 6964 7320 3d20 4e6f 6e65     rd_ids = None
+00010c10: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00010c20: 2e72 6575 7365 5f64 6174 615f 7365 7473  .reuse_data_sets
+00010c30: 3a0a 2020 2020 2020 2020 2020 2020 7264  :.            rd
+00010c40: 5f69 6473 203d 2067 6574 5f75 7569 6473  _ids = get_uuids
+00010c50: 5f66 726f 6d5f 6469 6374 2872 6570 6f72  _from_dict(repor
+00010c60: 745b 2270 726f 7065 7274 6965 7322 5d5b  t["properties"][
+00010c70: 226f 7074 696f 6e22 5d29 0a20 2020 2020  "option"]).     
+00010c80: 2020 2020 2020 2069 6620 6c65 6e28 7264         if len(rd
+00010c90: 5f69 6473 2920 3d3d 206c 656e 2879 293a  _ids) == len(y):
+00010ca0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010cb0: 2072 6570 5f64 733a 206c 6973 745b 5265   rep_ds: list[Re
+00010cc0: 706f 7274 2e52 6570 6f72 7444 6174 6153  port.ReportDataS
+00010cd0: 6574 5d20 3d20 6177 6169 7420 7265 706f  et] = await repo
+00010ce0: 7274 2e67 6574 5f72 6570 6f72 745f 6461  rt.get_report_da
+00010cf0: 7461 5f73 6574 7328 290a 2020 2020 2020  ta_sets().      
+00010d00: 2020 2020 2020 2020 2020 7265 705f 6473            rep_ds
+00010d10: 203d 205b 0a20 2020 2020 2020 2020 2020   = [.           
+00010d20: 2020 2020 2020 2020 206e 6578 7428 2872           next((r
+00010d30: 6420 666f 7220 7264 2069 6e20 7265 705f  d for rd in rep_
+00010d40: 6473 2069 6620 7264 5b22 6964 225d 203d  ds if rd["id"] =
+00010d50: 3d20 7264 5f69 6429 2c20 4e6f 6e65 290a  = rd_id), None).
+00010d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010d70: 2020 2020 666f 7220 7264 5f69 6420 696e      for rd_id in
+00010d80: 2072 645f 6964 730a 2020 2020 2020 2020   rd_ids.        
+00010d90: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
+00010da0: 2020 2020 2020 2020 2020 6966 2061 6e79            if any
+00010db0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00010dc0: 2020 2020 2020 7264 5b22 6461 7461 5365        rd["dataSe
+00010dd0: 7449 6422 5d20 213d 2064 735b 2269 6422  tId"] != ds["id"
+00010de0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+00010df0: 2020 2020 2020 6f72 2072 645b 2270 726f        or rd["pro
+00010e00: 7065 7274 6965 7322 5d5b 226d 6170 7069  perties"]["mappi
+00010e10: 6e67 225d 0a20 2020 2020 2020 2020 2020  ng"].           
+00010e20: 2020 2020 2020 2020 2021 3d20 7b22 7661           != {"va
+00010e30: 6c75 6573 223a 205b 2264 6174 6546 6965  lues": ["dateFie
+00010e40: 6c64 3122 2c20 2269 6e74 4669 656c 6431  ld1", "intField1
+00010e50: 225d 2c20 226c 6162 656c 223a 2022 7374  "], "label": "st
+00010e60: 7269 6e67 4669 656c 6431 227d 0a20 2020  ringField1"}.   
+00010e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010e80: 2066 6f72 2072 642c 2064 7320 696e 207a   for rd, ds in z
+00010e90: 6970 2872 6570 5f64 732c 2064 6174 615f  ip(rep_ds, data_
+00010ea0: 7365 7473 290a 2020 2020 2020 2020 2020  sets).          
+00010eb0: 2020 2020 2020 293a 0a20 2020 2020 2020        ):.       
+00010ec0: 2020 2020 2020 2020 2020 2020 2072 645f               rd_
+00010ed0: 6964 7320 3d20 4e6f 6e65 0a0a 2020 2020  ids = None..    
+00010ee0: 2020 2020 6966 206e 6f74 2072 645f 6964      if not rd_id
+00010ef0: 733a 0a20 2020 2020 2020 2020 2020 2061  s:.            a
+00010f00: 7761 6974 2072 6570 6f72 742e 6465 6c65  wait report.dele
+00010f10: 7465 5f72 6570 6f72 745f 6461 7461 5f73  te_report_data_s
+00010f20: 6574 7328 6c6f 673d 5472 7565 290a 2020  ets(log=True).  
+00010f30: 2020 2020 2020 2020 2020 6d61 7070 696e            mappin
+00010f40: 673a 204d 6170 7069 6e67 203d 207b 0a20  g: Mapping = {. 
+00010f50: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00010f60: 7661 6c75 6573 223a 205b 2264 6174 6546  values": ["dateF
+00010f70: 6965 6c64 3122 2c20 2269 6e74 4669 656c  ield1", "intFiel
+00010f80: 6431 225d 2c0a 2020 2020 2020 2020 2020  d1"],.          
+00010f90: 2020 2020 2020 226c 6162 656c 223a 2022        "label": "
+00010fa0: 7374 7269 6e67 4669 656c 6431 222c 0a20  stringField1",. 
+00010fb0: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
+00010fc0: 2020 2020 2020 2020 2072 6570 6f72 745f           report_
+00010fd0: 6461 7461 5f73 6574 7320 3d20 6177 6169  data_sets = awai
+00010fe0: 7420 6173 796e 6369 6f2e 6761 7468 6572  t asyncio.gather
+00010ff0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00011000: 2020 2a5b 0a20 2020 2020 2020 2020 2020    *[.           
+00011010: 2020 2020 2020 2020 2072 6570 6f72 742e           report.
+00011020: 6372 6561 7465 5f72 6570 6f72 745f 6461  create_report_da
+00011030: 7461 5f73 6574 2828 6d61 7070 696e 672c  ta_set((mapping,
+00011040: 2064 6174 615f 7365 742c 204e 6f6e 6529   data_set, None)
+00011050: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00011060: 2020 2020 2020 666f 7220 6461 7461 5f73        for data_s
+00011070: 6574 2069 6e20 6461 7461 5f73 6574 730a  et in data_sets.
+00011080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011090: 5d0a 2020 2020 2020 2020 2020 2020 290a  ].            ).
+000110a0: 2020 2020 2020 2020 2020 2020 7264 5f69              rd_i
+000110b0: 6473 203d 205b 7264 5b22 6964 225d 2066  ds = [rd["id"] f
+000110c0: 6f72 2072 6420 696e 2072 6570 6f72 745f  or rd in report_
+000110d0: 6461 7461 5f73 6574 735d 0a0a 2020 2020  data_sets]..    
+000110e0: 2020 2020 6368 6172 745f 6f70 7469 6f6e      chart_option
+000110f0: 7320 3d20 7b0a 2020 2020 2020 2020 2020  s = {.          
+00011100: 2020 2279 4178 6973 223a 207b 0a20 2020    "yAxis": {.   
+00011110: 2020 2020 2020 2020 2020 2020 2022 6e61               "na
+00011120: 6d65 223a 2079 5f61 7869 735f 6e61 6d65  me": y_axis_name
+00011130: 206f 7220 2222 2c0a 2020 2020 2020 2020   or "",.        
+00011140: 2020 2020 2020 2020 2266 6f6e 7422 2022          "font" "
+00011150: 7479 7065 223a 2022 7661 6c75 6522 2c0a  type": "value",.
+00011160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011170: 226e 616d 654c 6f63 6174 696f 6e22 3a20  "nameLocation": 
+00011180: 226d 6964 646c 6522 2c0a 2020 2020 2020  "middle",.      
+00011190: 2020 2020 2020 2020 2020 226e 616d 6547            "nameG
+000111a0: 6170 223a 2033 302c 0a20 2020 2020 2020  ap": 30,.       
+000111b0: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+000111c0: 2020 2020 2278 4178 6973 223a 207b 0a20      "xAxis": {. 
+000111d0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000111e0: 7479 7065 223a 2022 7469 6d65 222c 0a20  type": "time",. 
+000111f0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00011200: 6e61 6d65 4c6f 6361 7469 6f6e 223a 2022  nameLocation": "
+00011210: 6d69 6464 6c65 222c 0a20 2020 2020 2020  middle",.       
+00011220: 2020 2020 2020 2020 2022 6e61 6d65 4761           "nameGa
+00011230: 7022 3a20 3330 2c0a 2020 2020 2020 2020  p": 30,.        
+00011240: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
+00011250: 2020 2022 7365 7269 6573 223a 205b 0a20     "series": [. 
+00011260: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+00011270: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011280: 2020 2020 2022 6461 7461 223a 2022 237b       "data": "#{
+00011290: 2220 2b20 7264 5f69 6420 2b20 227d 222c  " + rd_id + "}",
+000112a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000112b0: 2020 2020 2022 7479 7065 223a 2022 6c69       "type": "li
+000112c0: 6e65 222c 0a20 2020 2020 2020 2020 2020  ne",.           
+000112d0: 2020 2020 2020 2020 2022 6e61 6d65 223a           "name":
+000112e0: 2079 5f6e 616d 652c 0a20 2020 2020 2020   y_name,.       
+000112f0: 2020 2020 2020 2020 2020 2020 2022 6974               "it
+00011300: 656d 5374 796c 6522 3a20 7b0a 2020 2020  emStyle": {.    
+00011310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011320: 2020 2020 2262 6f72 6465 7252 6164 6975      "borderRadiu
+00011330: 7322 3a20 5b39 2c20 392c 2030 2c20 305d  s": [9, 9, 0, 0]
+00011340: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00011350: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+00011360: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
+00011370: 2020 2020 2020 2020 2020 2066 6f72 2079             for y
+00011380: 5f6e 616d 652c 2072 645f 6964 2069 6e20  _name, rd_id in 
+00011390: 7a69 7028 792c 2072 645f 6964 7329 0a20  zip(y, rd_ids). 
+000113a0: 2020 2020 2020 2020 2020 205d 2c0a 2020             ],.  
+000113b0: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+000113c0: 6177 6169 7420 7365 6c66 2e5f 6372 6561  await self._crea
+000113d0: 7465 5f63 6861 7274 280a 2020 2020 2020  te_chart(.      
+000113e0: 2020 2020 2020 6368 6172 745f 636c 6173        chart_clas
+000113f0: 733d 416e 6e6f 7461 7465 6445 4368 6172  s=AnnotatedEChar
+00011400: 742c 0a20 2020 2020 2020 2020 2020 206f  t,.            o
+00011410: 7264 6572 3d6f 7264 6572 2c0a 2020 2020  rder=order,.    
+00011420: 2020 2020 2020 2020 7369 7a65 5061 6464          sizePadd
+00011430: 696e 673d 7061 6464 696e 672c 0a20 2020  ing=padding,.   
+00011440: 2020 2020 2020 2020 2073 697a 6552 6f77           sizeRow
+00011450: 733d 726f 7773 5f73 697a 652c 0a20 2020  s=rows_size,.   
+00011460: 2020 2020 2020 2020 2073 697a 6543 6f6c           sizeCol
+00011470: 756d 6e73 3d63 6f6c 735f 7369 7a65 2c0a  umns=cols_size,.
+00011480: 2020 2020 2020 2020 2020 2020 7469 746c              titl
+00011490: 653d 7469 746c 652c 0a20 2020 2020 2020  e=title,.       
+000114a0: 2020 2020 2070 726f 7065 7274 6965 733d       properties=
+000114b0: 6469 6374 280a 2020 2020 2020 2020 2020  dict(.          
+000114c0: 2020 2020 2020 736c 6964 6572 3d73 6c69        slider=sli
+000114d0: 6465 725f 636f 6e66 6967 2c0a 2020 2020  der_config,.    
+000114e0: 2020 2020 2020 2020 2020 2020 6f70 7469              opti
+000114f0: 6f6e 3d63 6861 7274 5f6f 7074 696f 6e73  on=chart_options
+00011500: 2c0a 2020 2020 2020 2020 2020 2020 292c  ,.            ),
+00011510: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+00011520: 6173 796e 6320 6465 6620 5f67 6574 5f72  async def _get_r
+00011530: 6570 6f72 745f 6461 7461 5f73 6574 735f  eport_data_sets_
+00011540: 7065 725f 6d61 7070 696e 6728 0a20 2020  per_mapping(.   
+00011550: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+00011560: 2020 2072 6570 6f72 743a 2052 6570 6f72     report: Repor
+00011570: 742c 0a20 2020 2020 2020 2064 6174 615f  t,.        data_
+00011580: 6d61 7070 696e 675f 746f 5f74 7570 6c65  mapping_to_tuple
+00011590: 3a20 6469 6374 2c0a 2020 2020 2020 2020  : dict,.        
+000115a0: 6669 656c 6473 3a20 6c69 7374 5b55 6e69  fields: list[Uni
+000115b0: 6f6e 5b74 7570 6c65 2c20 6469 6374 5d5d  on[tuple, dict]]
+000115c0: 2c0a 2020 2020 2920 2d3e 206c 6973 745b  ,.    ) -> list[
+000115d0: 5265 706f 7274 2e52 6570 6f72 7444 6174  Report.ReportDat
+000115e0: 6153 6574 5d3a 0a20 2020 2020 2020 2022  aSet]:.        "
+000115f0: 2222 4372 6561 7465 2061 2064 6174 615f  ""Create a data_
+00011600: 7365 7420 7065 7220 6669 656c 6420 6f66  set per field of
+00011610: 2061 2064 6174 6166 7261 6d65 2e0a 2020   a dataframe..  
+00011620: 2020 2020 2020 3a70 6172 616d 2072 6570        :param rep
+00011630: 6f72 743a 2074 6865 2072 6570 6f72 740a  ort: the report.
+00011640: 2020 2020 2020 2020 3a70 6172 616d 2064          :param d
+00011650: 6174 615f 6d61 7070 696e 675f 746f 5f74  ata_mapping_to_t
+00011660: 7570 6c65 3a20 7468 6520 6d61 7070 696e  uple: the mappin
+00011670: 6720 6f66 2074 6865 2064 6174 610a 2020  g of the data.  
+00011680: 2020 2020 2020 3a70 6172 616d 2066 6965        :param fie
+00011690: 6c64 733a 2074 6865 2066 6965 6c64 7320  lds: the fields 
+000116a0: 6f66 2074 6865 2064 6174 6120 746f 2062  of the data to b
+000116b0: 6520 7573 6564 0a20 2020 2020 2020 203a  e used.        :
+000116c0: 7265 7475 726e 3a20 7468 6520 6c69 7374  return: the list
+000116d0: 206f 6620 6461 7461 2073 6574 7320 7061   of data sets pa
+000116e0: 7274 6974 696f 6e65 6420 6279 2061 7869  rtitioned by axi
+000116f0: 7320 616e 6420 6669 656c 6473 0a20 2020  s and fields.   
+00011700: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00011710: 2074 6173 6b73 203d 205b 5d0a 2020 2020   tasks = [].    
+00011720: 2020 2020 6669 656c 6473 203d 2066 6965      fields = fie
+00011730: 6c64 7320 6966 2066 6965 6c64 7320 656c  lds if fields el
+00011740: 7365 205b 5d0a 2020 2020 2020 2020 666f  se [].        fo
+00011750: 7220 692c 2066 2069 6e20 656e 756d 6572  r i, f in enumer
+00011760: 6174 6528 6669 656c 6473 293a 0a20 2020  ate(fields):.   
+00011770: 2020 2020 2020 2020 206d 6170 7069 6e67           mapping
+00011780: 203d 205b 5d0a 2020 2020 2020 2020 2020   = [].          
+00011790: 2020 6461 7461 5f73 6574 203d 204e 6f6e    data_set = Non
+000117a0: 650a 2020 2020 2020 2020 2020 2020 7265  e.            re
+000117b0: 735f 736f 7274 203d 204e 6f6e 650a 2020  s_sort = None.  
+000117c0: 2020 2020 2020 2020 2020 6966 2069 7369            if isi
+000117d0: 6e73 7461 6e63 6528 662c 2073 7472 293a  nstance(f, str):
+000117e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000117f0: 2069 6620 6620 6e6f 7420 696e 2064 6174   if f not in dat
+00011800: 615f 6d61 7070 696e 675f 746f 5f74 7570  a_mapping_to_tup
+00011810: 6c65 3a0a 2020 2020 2020 2020 2020 2020  le:.            
+00011820: 2020 2020 2020 2020 6c6f 675f 6572 726f          log_erro
+00011830: 7228 6c6f 6767 6572 2c20 6622 4669 656c  r(logger, f"Fiel
+00011840: 6420 7b66 7d20 6e6f 7420 666f 756e 6420  d {f} not found 
+00011850: 696e 2064 6174 6122 2c20 4461 7461 4572  in data", DataEr
+00011860: 726f 7229 0a20 2020 2020 2020 2020 2020  ror).           
+00011870: 2020 2020 206d 6170 7069 6e67 2c20 6461       mapping, da
+00011880: 7461 5f73 6574 2c20 7265 735f 736f 7274  ta_set, res_sort
+00011890: 203d 2064 6174 615f 6d61 7070 696e 675f   = data_mapping_
+000118a0: 746f 5f74 7570 6c65 5b66 5d0a 2020 2020  to_tuple[f].    
+000118b0: 2020 2020 2020 2020 656c 6966 2069 7369          elif isi
+000118c0: 6e73 7461 6e63 6528 662c 2028 7475 706c  nstance(f, (tupl
+000118d0: 652c 206c 6973 7429 293a 0a20 2020 2020  e, list)):.     
+000118e0: 2020 2020 2020 2020 2020 2066 6f72 2066             for f
+000118f0: 5f20 696e 2066 3a0a 2020 2020 2020 2020  _ in f:.        
+00011900: 2020 2020 2020 2020 2020 2020 6966 2066              if f
+00011910: 5f20 6e6f 7420 696e 2064 6174 615f 6d61  _ not in data_ma
+00011920: 7070 696e 675f 746f 5f74 7570 6c65 3a0a  pping_to_tuple:.
+00011930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011940: 2020 2020 2020 2020 6c6f 675f 6572 726f          log_erro
+00011950: 7228 6c6f 6767 6572 2c20 6622 4669 656c  r(logger, f"Fiel
+00011960: 6420 7b66 5f7d 206e 6f74 2066 6f75 6e64  d {f_} not found
+00011970: 2069 6e20 6461 7461 222c 2044 6174 6145   in data", DataE
+00011980: 7272 6f72 290a 2020 2020 2020 2020 2020  rror).          
+00011990: 2020 2020 2020 2020 2020 6d61 7070 696e            mappin
+000119a0: 675f 2c20 6461 7461 5f73 6574 5f2c 2072  g_, data_set_, r
+000119b0: 6573 5f73 6f72 745f 203d 2064 6174 615f  es_sort_ = data_
+000119c0: 6d61 7070 696e 675f 746f 5f74 7570 6c65  mapping_to_tuple
+000119d0: 5b66 5f5d 0a20 2020 2020 2020 2020 2020  [f_].           
+000119e0: 2020 2020 2020 2020 206d 6170 7069 6e67           mapping
+000119f0: 2e61 7070 656e 6428 6d61 7070 696e 675f  .append(mapping_
+00011a00: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00011a10: 2020 2020 2020 6461 7461 5f73 6574 203d        data_set =
+00011a20: 2064 6174 615f 7365 7420 6966 2064 6174   data_set if dat
+00011a30: 615f 7365 7420 656c 7365 2064 6174 615f  a_set else data_
+00011a40: 7365 745f 0a20 2020 2020 2020 2020 2020  set_.           
+00011a50: 2020 2020 2020 2020 2072 6573 5f73 6f72           res_sor
+00011a60: 7420 3d20 7265 735f 736f 7274 2069 6620  t = res_sort if 
+00011a70: 7265 735f 736f 7274 2065 6c73 6520 7265  res_sort else re
+00011a80: 735f 736f 7274 5f0a 2020 2020 2020 2020  s_sort_.        
+00011a90: 2020 2020 2020 2020 2020 2020 6173 7365              asse
+00011aa0: 7274 2064 6174 615f 7365 7420 3d3d 2064  rt data_set == d
+00011ab0: 6174 615f 7365 745f 0a20 2020 2020 2020  ata_set_.       
+00011ac0: 2020 2020 2020 2020 2020 2020 2061 7373               ass
+00011ad0: 6572 7420 7265 735f 736f 7274 203d 3d20  ert res_sort == 
+00011ae0: 7265 735f 736f 7274 5f0a 2020 2020 2020  res_sort_.      
+00011af0: 2020 2020 2020 656c 6966 2069 7369 6e73        elif isins
+00011b00: 7461 6e63 6528 662c 2064 6963 7429 3a0a  tance(f, dict):.
+00011b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011b20: 6d61 7070 696e 6720 3d20 7b6b 3a20 5b5d  mapping = {k: []
+00011b30: 2066 6f72 206b 2069 6e20 662e 6b65 7973   for k in f.keys
+00011b40: 2829 7d0a 2020 2020 2020 2020 2020 2020  ()}.            
+00011b50: 2020 2020 666f 7220 6b2c 2066 5f20 696e      for k, f_ in
+00011b60: 2066 2e69 7465 6d73 2829 3a0a 2020 2020   f.items():.    
+00011b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011b80: 6966 2066 5f20 6e6f 7420 696e 2064 6174  if f_ not in dat
+00011b90: 615f 6d61 7070 696e 675f 746f 5f74 7570  a_mapping_to_tup
+00011ba0: 6c65 3a0a 2020 2020 2020 2020 2020 2020  le:.            
+00011bb0: 2020 2020 2020 2020 2020 2020 6c6f 675f              log_
+00011bc0: 6572 726f 7228 6c6f 6767 6572 2c20 6622  error(logger, f"
+00011bd0: 4669 656c 6420 7b66 5f7d 206e 6f74 2066  Field {f_} not f
+00011be0: 6f75 6e64 2069 6e20 6461 7461 222c 2044  ound in data", D
+00011bf0: 6174 6145 7272 6f72 290a 2020 2020 2020  ataError).      
+00011c00: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
+00011c10: 7070 696e 675f 2c20 6461 7461 5f73 6574  pping_, data_set
+00011c20: 5f2c 2072 6573 5f73 6f72 745f 203d 2064  _, res_sort_ = d
+00011c30: 6174 615f 6d61 7070 696e 675f 746f 5f74  ata_mapping_to_t
+00011c40: 7570 6c65 5b66 5f5d 0a20 2020 2020 2020  uple[f_].       
+00011c50: 2020 2020 2020 2020 2020 2020 206d 6170               map
+00011c60: 7069 6e67 5b6b 5d20 3d20 6d61 7070 696e  ping[k] = mappin
+00011c70: 675f 0a20 2020 2020 2020 2020 2020 2020  g_.             
+00011c80: 2020 2020 2020 2064 6174 615f 7365 7420         data_set 
+00011c90: 3d20 6461 7461 5f73 6574 2069 6620 6461  = data_set if da
+00011ca0: 7461 5f73 6574 2065 6c73 6520 6461 7461  ta_set else data
+00011cb0: 5f73 6574 5f0a 2020 2020 2020 2020 2020  _set_.          
+00011cc0: 2020 2020 2020 2020 2020 7265 735f 736f            res_so
+00011cd0: 7274 203d 2072 6573 5f73 6f72 7420 6966  rt = res_sort if
+00011ce0: 2072 6573 5f73 6f72 7420 656c 7365 2072   res_sort else r
+00011cf0: 6573 5f73 6f72 745f 0a20 2020 2020 2020  es_sort_.       
+00011d00: 2020 2020 2020 2020 2020 2020 2061 7373               ass
+00011d10: 6572 7420 6461 7461 5f73 6574 203d 3d20  ert data_set == 
+00011d20: 6461 7461 5f73 6574 5f0a 2020 2020 2020  data_set_.      
+00011d30: 2020 2020 2020 2020 2020 2020 2020 6173                as
+00011d40: 7365 7274 2072 6573 5f73 6f72 7420 3d3d  sert res_sort ==
+00011d50: 2072 6573 5f73 6f72 745f 0a20 2020 2020   res_sort_.     
+00011d60: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00011d70: 2020 2020 2020 2020 2020 2020 206c 6f67               log
+00011d80: 5f65 7272 6f72 280a 2020 2020 2020 2020  _error(.        
+00011d90: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
+00011da0: 6572 2c20 6622 4669 656c 6420 7b66 7d20  er, f"Field {f} 
+00011db0: 6973 206e 6f74 2061 2073 7472 696e 672c  is not a string,
+00011dc0: 2074 7570 6c65 2c20 6c69 7374 206f 7220   tuple, list or 
+00011dd0: 6469 6374 222c 2044 6174 6145 7272 6f72  dict", DataError
+00011de0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011df0: 2029 0a20 2020 2020 2020 2020 2020 2074   ).            t
+00011e00: 6173 6b73 2e61 7070 656e 6428 0a20 2020  asks.append(.   
+00011e10: 2020 2020 2020 2020 2020 2020 2072 6570               rep
+00011e20: 6f72 742e 6372 6561 7465 5f72 6570 6f72  ort.create_repor
+00011e30: 745f 6461 7461 5f73 6574 280a 2020 2020  t_data_set(.    
+00011e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011e50: 6d61 7070 696e 675f 6461 7461 5f73 6574  mapping_data_set
+00011e60: 5f73 6f72 743d 286d 6170 7069 6e67 2c20  _sort=(mapping, 
+00011e70: 6461 7461 5f73 6574 2c20 7265 735f 736f  data_set, res_so
+00011e80: 7274 290a 2020 2020 2020 2020 2020 2020  rt).            
+00011e90: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00011ea0: 2020 290a 0a20 2020 2020 2020 2072 6570    )..        rep
+00011eb0: 6f72 745f 6461 7461 5f73 6574 7320 3d20  ort_data_sets = 
+00011ec0: 6177 6169 7420 6173 796e 6369 6f2e 6761  await asyncio.ga
+00011ed0: 7468 6572 282a 7461 736b 7329 0a20 2020  ther(*tasks).   
+00011ee0: 2020 2020 206c 6f67 6765 722e 696e 666f       logger.info
+00011ef0: 280a 2020 2020 2020 2020 2020 2020 6622  (.            f"
+00011f00: 4372 6561 7465 6420 7b6c 656e 2872 6570  Created {len(rep
+00011f10: 6f72 745f 6461 7461 5f73 6574 7329 7d20  ort_data_sets)} 
+00011f20: 636f 6d70 6f6e 656e 7420 6461 7461 2073  component data s
+00011f30: 6574 206c 696e 6b73 2066 6f72 2063 6f6d  et links for com
+00011f40: 706f 6e65 6e74 207b 7374 7228 7265 706f  ponent {str(repo
+00011f50: 7274 297d 220a 2020 2020 2020 2020 290a  rt)}".        ).
+00011f60: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+00011f70: 6570 6f72 745f 6461 7461 5f73 6574 730a  eport_data_sets.
+00011f80: 0a20 2020 2064 6566 205f 7570 6461 7465  .    def _update
+00011f90: 5f6f 7074 696f 6e73 2873 656c 662c 206f  _options(self, o
+00011fa0: 7074 696f 6e73 3a20 6469 6374 2c20 6f70  ptions: dict, op
+00011fb0: 7469 6f6e 5f6d 6f64 6966 6963 6174 696f  tion_modificatio
+00011fc0: 6e73 3a20 4f70 7469 6f6e 616c 5b64 6963  ns: Optional[dic
+00011fd0: 745d 293a 0a20 2020 2020 2020 2022 2222  t]):.        """
+00011fe0: 5570 6461 7465 2074 6865 206f 7074 696f  Update the optio
+00011ff0: 6e73 206f 6620 616e 2065 6368 6172 742e  ns of an echart.
+00012000: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00012010: 6f70 7469 6f6e 733a 2074 6865 206f 7074  options: the opt
+00012020: 696f 6e73 206f 6620 7468 6520 6563 6861  ions of the echa
+00012030: 7274 0a20 2020 2020 2020 203a 7061 7261  rt.        :para
+00012040: 6d20 6f70 7469 6f6e 5f6d 6f64 6966 6963  m option_modific
+00012050: 6174 696f 6e73 3a20 7468 6520 6d6f 6469  ations: the modi
+00012060: 6669 6361 7469 6f6e 7320 746f 2061 7070  fications to app
+00012070: 6c79 2074 6f20 7468 6520 6f70 7469 6f6e  ly to the option
+00012080: 730a 2020 2020 2020 2020 2222 220a 2020  s.        """.  
+00012090: 2020 2020 2020 6966 206e 6f74 206f 7074        if not opt
+000120a0: 696f 6e5f 6d6f 6469 6669 6361 7469 6f6e  ion_modification
+000120b0: 733a 0a20 2020 2020 2020 2020 2020 2072  s:.            r
+000120c0: 6574 7572 6e0a 2020 2020 2020 2020 666f  eturn.        fo
+000120d0: 7220 6b2c 2076 2069 6e20 6f70 7469 6f6e  r k, v in option
+000120e0: 5f6d 6f64 6966 6963 6174 696f 6e73 2e69  _modifications.i
+000120f0: 7465 6d73 2829 3a0a 2020 2020 2020 2020  tems():.        
+00012100: 2020 2020 6966 206b 203d 3d20 2273 6572      if k == "ser
+00012110: 6965 7322 3a0a 2020 2020 2020 2020 2020  ies":.          
+00012120: 2020 2020 2020 6c6f 675f 6572 726f 7228        log_error(
+00012130: 6c6f 6767 6572 2c20 2253 6572 6965 7320  logger, "Series 
+00012140: 6361 6e6e 6f74 2062 6520 6d6f 6469 6669  cannot be modifi
+00012150: 6564 222c 2044 6174 6145 7272 6f72 290a  ed", DataError).
+00012160: 2020 2020 2020 2020 2020 2020 6966 206b              if k
+00012170: 203d 3d20 2278 4178 6973 2220 6f72 206b   == "xAxis" or k
+00012180: 203d 3d20 2279 4178 6973 223a 0a20 2020   == "yAxis":.   
+00012190: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000121a0: 6973 696e 7374 616e 6365 2876 2c20 6469  isinstance(v, di
+000121b0: 6374 293a 0a20 2020 2020 2020 2020 2020  ct):.           
+000121c0: 2020 2020 2020 2020 2076 203d 205b 765d           v = [v]
+000121d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000121e0: 2069 6620 6c65 6e28 7629 2021 3d20 6c65   if len(v) != le
+000121f0: 6e28 6f70 7469 6f6e 735b 6b5d 293a 0a20  n(options[k]):. 
+00012200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012210: 2020 206c 6f67 5f65 7272 6f72 286c 6f67     log_error(log
+00012220: 6765 722c 2066 2254 6865 206e 756d 6265  ger, f"The numbe
+00012230: 7220 6f66 207b 6b7d 206d 7573 7420 6265  r of {k} must be
+00012240: 207b 6c65 6e28 7629 7d22 2c20 4461 7461   {len(v)}", Data
+00012250: 4572 726f 7229 0a20 2020 2020 2020 2020  Error).         
+00012260: 2020 2020 2020 2066 6f72 2069 2c20 765f         for i, v_
+00012270: 2069 6e20 656e 756d 6572 6174 6528 7629   in enumerate(v)
+00012280: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00012290: 2020 2020 2020 6f70 7469 6f6e 735b 6b5d        options[k]
+000122a0: 5b69 5d2e 7570 6461 7465 2876 5f29 0a20  [i].update(v_). 
+000122b0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+000122c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000122d0: 206f 7074 696f 6e73 5b6b 5d20 3d20 760a   options[k] = v.
+000122e0: 0a20 2020 2061 7379 6e63 2064 6566 205f  .    async def _
+000122f0: 6372 6561 7465 5f65 6368 6172 7428 0a20  create_echart(. 
+00012300: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+00012310: 2020 2020 206f 7074 696f 6e73 3a20 6469       options: di
+00012320: 6374 2c0a 2020 2020 2020 2020 6f72 6465  ct,.        orde
+00012330: 723a 2069 6e74 2c0a 2020 2020 2020 2020  r: int,.        
+00012340: 6669 656c 6473 3a20 6c69 7374 5b55 6e69  fields: list[Uni
+00012350: 6f6e 5b73 7472 2c20 7475 706c 652c 2064  on[str, tuple, d
+00012360: 6963 745d 5d2c 0a20 2020 2020 2020 2064  ict]],.        d
+00012370: 6174 615f 6d61 7070 696e 675f 746f 5f74  ata_mapping_to_t
+00012380: 7570 6c65 733a 204f 7074 696f 6e61 6c5b  uples: Optional[
+00012390: 6469 6374 5d20 3d20 4e6f 6e65 2c0a 2020  dict] = None,.  
+000123a0: 2020 2020 2020 6461 7461 3a20 4f70 7469        data: Opti
+000123b0: 6f6e 616c 5b55 6e69 6f6e 5b73 7472 2c20  onal[Union[str, 
+000123c0: 7064 2e44 6174 6146 7261 6d65 5d5d 203d  pd.DataFrame]] =
+000123d0: 204e 6f6e 652c 0a20 2020 2020 2020 2064   None,.        d
+000123e0: 756d 705f 7768 6f6c 653a 2062 6f6f 6c20  ump_whole: bool 
+000123f0: 3d20 4661 6c73 652c 0a20 2020 2020 2020  = False,.       
+00012400: 206f 7074 696f 6e5f 6d6f 6469 6669 6361   option_modifica
+00012410: 7469 6f6e 733a 204f 7074 696f 6e61 6c5b  tions: Optional[
+00012420: 6469 6374 5d20 3d20 4e6f 6e65 2c0a 2020  dict] = None,.  
+00012430: 2020 2020 2020 7469 746c 653a 204f 7074        title: Opt
+00012440: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+00012450: 652c 0a20 2020 2020 2020 2072 6f77 735f  e,.        rows_
+00012460: 7369 7a65 3a20 4f70 7469 6f6e 616c 5b69  size: Optional[i
+00012470: 6e74 5d20 3d20 4e6f 6e65 2c0a 2020 2020  nt] = None,.    
+00012480: 2020 2020 636f 6c73 5f73 697a 653a 204f      cols_size: O
+00012490: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
+000124a0: 6f6e 652c 0a20 2020 2020 2020 2070 6164  one,.        pad
+000124b0: 6469 6e67 3a20 4f70 7469 6f6e 616c 5b73  ding: Optional[s
+000124c0: 7472 5d20 3d20 4e6f 6e65 2c0a 2020 2020  tr] = None,.    
+000124d0: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+000124e0: 2020 2020 2020 2043 7265 6174 6520 616e         Create an
+000124f0: 2065 6368 6172 7420 696e 2074 6865 2064   echart in the d
+00012500: 6173 6862 6f61 7264 2c20 6669 6c6c 2069  ashboard, fill i
+00012510: 6e20 7468 6520 6461 7461 2072 6566 6572  n the data refer
+00012520: 656e 6365 6420 696e 2074 6865 2065 6368  enced in the ech
+00012530: 6172 745f 6f70 7469 6f6e 7320 616e 6420  art_options and 
+00012540: 6372 6561 7465 206f 720a 2020 2020 2020  create or.      
+00012550: 2020 7570 6461 7465 2074 6865 2063 6861    update the cha
+00012560: 7274 2061 6e64 2064 6174 6120 7365 7420  rt and data set 
+00012570: 6c69 6e6b 732e 0a20 2020 2020 2020 203a  links..        :
+00012580: 7061 7261 6d20 6f70 7469 6f6e 733a 2074  param options: t
+00012590: 6865 206f 7074 696f 6e73 206f 6620 7468  he options of th
+000125a0: 6520 6563 6861 7274 0a20 2020 2020 2020  e echart.       
+000125b0: 203a 7061 7261 6d20 6461 7461 5f6d 6170   :param data_map
+000125c0: 7069 6e67 5f74 6f5f 7475 706c 6573 3a20  ping_to_tuples: 
+000125d0: 7468 6520 6d61 7070 696e 6720 6f66 2074  the mapping of t
+000125e0: 6865 2064 6174 6120 746f 2074 6865 2074  he data to the t
+000125f0: 7570 6c65 730a 2020 2020 2020 2020 3a70  uples.        :p
+00012600: 6172 616d 2064 6174 613a 2074 6865 2064  aram data: the d
+00012610: 6174 6120 6f66 2074 6865 2065 6368 6172  ata of the echar
+00012620: 740a 2020 2020 2020 2020 3a70 6172 616d  t.        :param
+00012630: 2064 756d 705f 7768 6f6c 653a 2077 6865   dump_whole: whe
+00012640: 7468 6572 2074 6f20 6475 6d70 2074 6865  ther to dump the
+00012650: 2077 686f 6c65 2064 6174 610a 2020 2020   whole data.    
+00012660: 2020 2020 3a70 6172 616d 206f 7074 696f      :param optio
+00012670: 6e5f 6d6f 6469 6669 6361 7469 6f6e 733a  n_modifications:
+00012680: 2074 6865 206d 6f64 6966 6963 6174 696f   the modificatio
+00012690: 6e73 2074 6f20 6170 706c 7920 746f 2074  ns to apply to t
+000126a0: 6865 206f 7074 696f 6e73 0a20 2020 2020  he options.     
+000126b0: 2020 203a 7061 7261 6d20 7469 746c 653a     :param title:
+000126c0: 2074 6865 2074 6974 6c65 206f 6620 7468   the title of th
+000126d0: 6520 6563 6861 7274 0a20 2020 2020 2020  e echart.       
+000126e0: 203a 7061 7261 6d20 726f 7773 5f73 697a   :param rows_siz
+000126f0: 653a 2074 6865 2072 6f77 7320 7369 7a65  e: the rows size
+00012700: 206f 6620 7468 6520 6563 6861 7274 0a20   of the echart. 
+00012710: 2020 2020 2020 203a 7061 7261 6d20 636f         :param co
+00012720: 6c73 5f73 697a 653a 2074 6865 2063 6f6c  ls_size: the col
+00012730: 756d 6e73 2073 697a 6520 6f66 2074 6865  umns size of the
+00012740: 2065 6368 6172 740a 2020 2020 2020 2020   echart.        
+00012750: 3a70 6172 616d 2070 6164 6469 6e67 3a20  :param padding: 
+00012760: 7468 6520 7061 6464 696e 6720 6f66 2074  the padding of t
+00012770: 6865 2065 6368 6172 740a 2020 2020 2020  he echart.      
+00012780: 2020 2222 220a 0a20 2020 2020 2020 2069    """..        i
+00012790: 6620 6461 7461 2069 7320 6e6f 7420 4e6f  f data is not No
+000127a0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000127b0: 6461 7461 5f6d 6170 7069 6e67 5f74 6f5f  data_mapping_to_
+000127c0: 7475 706c 6573 203d 2061 7761 6974 2073  tuples = await s
+000127d0: 656c 662e 5f63 686f 6f73 655f 6461 7461  elf._choose_data
+000127e0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+000127f0: 2020 6f72 6465 722c 2064 6174 612c 2064    order, data, d
+00012800: 756d 705f 7768 6f6c 653d 6475 6d70 5f77  ump_whole=dump_w
+00012810: 686f 6c65 0a20 2020 2020 2020 2020 2020  hole.           
+00012820: 2029 0a0a 2020 2020 2020 2020 6461 7461   )..        data
+00012830: 5f6b 6579 5f65 6e74 7269 6573 203d 2067  _key_entries = g
+00012840: 6574 5f64 6174 615f 7265 6665 7265 6e63  et_data_referenc
+00012850: 6573 5f66 726f 6d5f 6469 6374 286f 7074  es_from_dict(opt
+00012860: 696f 6e73 290a 2020 2020 2020 2020 5f2c  ions).        _,
+00012870: 2072 6570 6f72 7420 3d20 6177 6169 7420   report = await 
+00012880: 7365 6c66 2e5f 6765 745f 6368 6172 745f  self._get_chart_
+00012890: 7265 706f 7274 286f 7264 6572 2c20 4543  report(order, EC
+000128a0: 6861 7274 290a 0a20 2020 2020 2020 2072  hart)..        r
+000128b0: 645f 6964 7320 3d20 4e6f 6e65 0a20 2020  d_ids = None.   
+000128c0: 2020 2020 2069 6620 7365 6c66 2e72 6575       if self.reu
+000128d0: 7365 5f64 6174 615f 7365 7473 3a0a 2020  se_data_sets:.  
+000128e0: 2020 2020 2020 2020 2020 7264 5f69 6473            rd_ids
+000128f0: 203d 2067 6574 5f75 7569 6473 5f66 726f   = get_uuids_fro
+00012900: 6d5f 6469 6374 2872 6570 6f72 745b 2270  m_dict(report["p
+00012910: 726f 7065 7274 6965 7322 5d5b 226f 7074  roperties"]["opt
+00012920: 696f 6e22 5d29 0a20 2020 2020 2020 2020  ion"]).         
+00012930: 2020 2069 6620 6c65 6e28 7264 5f69 6473     if len(rd_ids
+00012940: 2920 3d3d 206c 656e 2866 6965 6c64 7329  ) == len(fields)
+00012950: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00012960: 2020 7265 705f 6473 3a20 6c69 7374 5b52    rep_ds: list[R
+00012970: 6570 6f72 742e 5265 706f 7274 4461 7461  eport.ReportData
+00012980: 5365 745d 203d 2061 7761 6974 2072 6570  Set] = await rep
+00012990: 6f72 742e 6765 745f 7265 706f 7274 5f64  ort.get_report_d
+000129a0: 6174 615f 7365 7473 2829 0a20 2020 2020  ata_sets().     
+000129b0: 2020 2020 2020 2020 2020 206d 6170 7065             mappe
+000129c0: 645f 6620 3d20 5b0a 2020 2020 2020 2020  d_f = [.        
+000129d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000129e0: 2e5f 6765 745f 6669 656c 645f 6d61 7070  ._get_field_mapp
+000129f0: 696e 6728 6669 656c 642c 2064 6174 615f  ing(field, data_
+00012a00: 6d61 7070 696e 675f 746f 5f74 7570 6c65  mapping_to_tuple
+00012a10: 7329 0a20 2020 2020 2020 2020 2020 2020  s).             
+00012a20: 2020 2020 2020 2066 6f72 2066 6965 6c64         for field
+00012a30: 2069 6e20 6669 656c 6473 0a20 2020 2020   in fields.     
+00012a40: 2020 2020 2020 2020 2020 205d 0a20 2020             ].   
+00012a50: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+00012a60: 2069 2c20 7264 5f69 6420 696e 2065 6e75   i, rd_id in enu
+00012a70: 6d65 7261 7465 2872 645f 6964 7329 3a0a  merate(rd_ids):.
+00012a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012a90: 2020 2020 7265 706f 7274 5f64 6174 615f      report_data_
+00012aa0: 7365 7420 3d20 6e65 7874 280a 2020 2020  set = next(.    
+00012ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012ac0: 2020 2020 2872 6420 666f 7220 7264 2069      (rd for rd i
+00012ad0: 6e20 7265 705f 6473 2069 6620 7264 5b22  n rep_ds if rd["
+00012ae0: 6964 225d 203d 3d20 7264 5f69 6429 2c20  id"] == rd_id), 
+00012af0: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
+00012b00: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00012b10: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00012b20: 6620 280a 2020 2020 2020 2020 2020 2020  f (.            
+00012b30: 2020 2020 2020 2020 2020 2020 6e6f 7420              not 
+00012b40: 7265 706f 7274 5f64 6174 615f 7365 740a  report_data_set.
+00012b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012b60: 2020 2020 2020 2020 6f72 206e 6f74 2073          or not s
+00012b70: 656c 662e 5f63 6865 636b 5f6d 6170 7069  elf._check_mappi
+00012b80: 6e67 5f69 6e5f 7265 706f 7274 5f64 6174  ng_in_report_dat
+00012b90: 615f 7365 7428 0a20 2020 2020 2020 2020  a_set(.         
+00012ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012bb0: 2020 2072 6570 6f72 745f 6461 7461 5f73     report_data_s
+00012bc0: 6574 2c20 6d61 7070 6564 5f66 5b69 5d0a  et, mapped_f[i].
+00012bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012be0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00012bf0: 2020 2020 2020 2020 2020 2020 2020 293a                ):
+00012c00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012c10: 2020 2020 2020 2020 2072 645f 6964 7320           rd_ids 
+00012c20: 3d20 4e6f 6e65 0a20 2020 2020 2020 2020  = None.         
+00012c30: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+00012c40: 7265 616b 0a20 2020 2020 2020 2020 2020  reak.           
+00012c50: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00012c60: 2020 2020 2020 2072 645f 6964 7320 3d20         rd_ids = 
+00012c70: 4e6f 6e65 0a0a 2020 2020 2020 2020 6966  None..        if
+00012c80: 206e 6f74 2072 645f 6964 733a 0a20 2020   not rd_ids:.   
+00012c90: 2020 2020 2020 2020 2061 7761 6974 2072           await r
+00012ca0: 6570 6f72 742e 6465 6c65 7465 5f72 6570  eport.delete_rep
+00012cb0: 6f72 745f 6461 7461 5f73 6574 7328 6c6f  ort_data_sets(lo
+00012cc0: 673d 5472 7565 290a 2020 2020 2020 2020  g=True).        
+00012cd0: 2020 2020 7265 706f 7274 5f64 6174 615f      report_data_
+00012ce0: 7365 7473 203d 2061 7761 6974 2073 656c  sets = await sel
+00012cf0: 662e 5f67 6574 5f72 6570 6f72 745f 6461  f._get_report_da
+00012d00: 7461 5f73 6574 735f 7065 725f 6d61 7070  ta_sets_per_mapp
+00012d10: 696e 6728 0a20 2020 2020 2020 2020 2020  ing(.           
+00012d20: 2020 2020 2072 6570 6f72 742c 2064 6174       report, dat
+00012d30: 615f 6d61 7070 696e 675f 746f 5f74 7570  a_mapping_to_tup
+00012d40: 6c65 732c 2066 6965 6c64 730a 2020 2020  les, fields.    
+00012d50: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00012d60: 2020 2020 2020 7264 5f69 6473 203d 205b        rd_ids = [
+00012d70: 7264 5b22 6964 225d 2066 6f72 2072 6420  rd["id"] for rd 
+00012d80: 696e 2072 6570 6f72 745f 6461 7461 5f73  in report_data_s
+00012d90: 6574 735d 0a0a 2020 2020 2020 2020 7365  ets]..        se
+00012da0: 6c66 2e5f 7570 6461 7465 5f6f 7074 696f  lf._update_optio
+00012db0: 6e73 286f 7074 696f 6e73 2c20 6f70 7469  ns(options, opti
+00012dc0: 6f6e 5f6d 6f64 6966 6963 6174 696f 6e73  on_modifications
+00012dd0: 290a 0a20 2020 2020 2020 2069 6620 6c65  )..        if le
+00012de0: 6e28 7264 5f69 6473 2920 213d 206c 656e  n(rd_ids) != len
+00012df0: 2864 6174 615f 6b65 795f 656e 7472 6965  (data_key_entrie
+00012e00: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
+00012e10: 6c6f 675f 6572 726f 7228 0a20 2020 2020  log_error(.     
+00012e20: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+00012e30: 722c 0a20 2020 2020 2020 2020 2020 2020  r,.             
+00012e40: 2020 2066 2254 6865 206e 756d 6265 7220     f"The number 
+00012e50: 6f66 2064 6174 6120 7265 6665 7265 6e63  of data referenc
+00012e60: 6573 2061 6e64 2066 6965 6c64 7320 6d75  es and fields mu
+00012e70: 7374 2062 6520 6571 7561 6c2c 2022 0a20  st be equal, ". 
+00012e80: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00012e90: 2274 6865 7920 6172 6520 7b6c 656e 2864  "they are {len(d
+00012ea0: 6174 615f 6b65 795f 656e 7472 6965 7329  ata_key_entries)
+00012eb0: 7d20 616e 6420 7b6c 656e 2872 645f 6964  } and {len(rd_id
+00012ec0: 7329 7d20 7265 7370 6563 7469 7665 6c79  s)} respectively
+00012ed0: 2e22 2c0a 2020 2020 2020 2020 2020 2020  .",.            
+00012ee0: 2020 2020 4461 7461 4572 726f 722c 0a20      DataError,. 
+00012ef0: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
+00012f00: 2020 2020 2020 666f 7220 692c 2064 6174        for i, dat
+00012f10: 615f 6b65 795f 656e 7472 7920 696e 2065  a_key_entry in e
+00012f20: 6e75 6d65 7261 7465 2864 6174 615f 6b65  numerate(data_ke
+00012f30: 795f 656e 7472 6965 7329 3a0a 2020 2020  y_entries):.    
+00012f40: 2020 2020 2020 2020 6461 7461 203d 206f          data = o
+00012f50: 7074 696f 6e73 0a20 2020 2020 2020 2020  ptions.         
+00012f60: 2020 2066 6f72 206b 6579 2069 6e20 6461     for key in da
+00012f70: 7461 5f6b 6579 5f65 6e74 7279 5b3a 2d31  ta_key_entry[:-1
+00012f80: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
+00012f90: 2020 2064 6174 6120 3d20 6461 7461 5b6b     data = data[k
+00012fa0: 6579 5d0a 2020 2020 2020 2020 2020 2020  ey].            
+00012fb0: 6461 7461 5b64 6174 615f 6b65 795f 656e  data[data_key_en
+00012fc0: 7472 795b 2d31 5d5d 203d 2022 237b 2220  try[-1]] = "#{" 
+00012fd0: 2b20 7264 5f69 6473 5b69 5d20 2b20 227d  + rd_ids[i] + "}
+00012fe0: 220a 0a20 2020 2020 2020 2061 7761 6974  "..        await
+00012ff0: 2073 656c 662e 5f63 7265 6174 655f 6368   self._create_ch
+00013000: 6172 7428 0a20 2020 2020 2020 2020 2020  art(.           
+00013010: 2063 6861 7274 5f63 6c61 7373 3d45 4368   chart_class=ECh
+00013020: 6172 742c 0a20 2020 2020 2020 2020 2020  art,.           
+00013030: 2070 726f 7065 7274 6965 733d 7b22 6f70   properties={"op
+00013040: 7469 6f6e 223a 206f 7074 696f 6e73 7d2c  tion": options},
+00013050: 0a20 2020 2020 2020 2020 2020 206f 7264  .            ord
+00013060: 6572 3d6f 7264 6572 2c0a 2020 2020 2020  er=order,.      
+00013070: 2020 2020 2020 7469 746c 653d 7469 746c        title=titl
+00013080: 652c 0a20 2020 2020 2020 2020 2020 2073  e,.            s
+00013090: 697a 6550 6164 6469 6e67 3d70 6164 6469  izePadding=paddi
+000130a0: 6e67 2c0a 2020 2020 2020 2020 2020 2020  ng,.            
+000130b0: 7369 7a65 526f 7773 3d72 6f77 735f 7369  sizeRows=rows_si
+000130c0: 7a65 2c0a 2020 2020 2020 2020 2020 2020  ze,.            
+000130d0: 7369 7a65 436f 6c75 6d6e 733d 636f 6c73  sizeColumns=cols
+000130e0: 5f73 697a 652c 0a20 2020 2020 2020 2029  _size,.        )
+000130f0: 0a0a 2020 2020 4073 7461 7469 636d 6574  ..    @staticmet
+00013100: 686f 640a 2020 2020 6465 6620 5f61 7070  hod.    def _app
+00013110: 6c79 5f76 6172 6961 6e74 2865 6368 6172  ly_variant(echar
+00013120: 745f 6f70 7469 6f6e 733a 2064 6963 742c  t_options: dict,
+00013130: 2076 6172 6961 6e74 3a20 4f70 7469 6f6e   variant: Option
+00013140: 616c 5b73 7472 5d29 3a0a 2020 2020 2020  al[str]):.      
+00013150: 2020 6966 2076 6172 6961 6e74 203d 3d20    if variant == 
+00013160: 2263 6c65 616e 223a 0a20 2020 2020 2020  "clean":.       
+00013170: 2020 2020 2065 6368 6172 745f 6f70 7469       echart_opti
+00013180: 6f6e 732e 7570 6461 7465 280a 2020 2020  ons.update(.    
+00013190: 2020 2020 2020 2020 2020 2020 7b22 746f              {"to
+000131a0: 6f6c 626f 7822 3a20 7b22 7368 6f77 223a  olbox": {"show":
+000131b0: 2046 616c 7365 7d2c 2022 6c65 6765 6e64   False}, "legend
+000131c0: 223a 207b 2273 686f 7722 3a20 4661 6c73  ": {"show": Fals
+000131d0: 657d 2c20 2267 7269 6422 3a20 7b7d 7d0a  e}, "grid": {}}.
+000131e0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+000131f0: 2020 2020 2020 2020 2020 666f 7220 6178            for ax
+00013200: 6973 6c69 7374 2069 6e20 5b65 6368 6172  islist in [echar
+00013210: 745f 6f70 7469 6f6e 735b 2278 4178 6973  t_options["xAxis
+00013220: 225d 2c20 6563 6861 7274 5f6f 7074 696f  "], echart_optio
+00013230: 6e73 5b22 7941 7869 7322 5d5d 3a0a 2020  ns["yAxis"]]:.  
+00013240: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00013250: 7220 6178 6973 2069 6e20 6178 6973 6c69  r axis in axisli
+00013260: 7374 3a0a 2020 2020 2020 2020 2020 2020  st:.            
+00013270: 2020 2020 2020 2020 6178 6973 2e75 7064          axis.upd
+00013280: 6174 6528 0a20 2020 2020 2020 2020 2020  ate(.           
+00013290: 2020 2020 2020 2020 2020 2020 207b 2261               {"a
+000132a0: 7869 734c 696e 6522 3a20 7b22 7368 6f77  xisLine": {"show
+000132b0: 223a 2046 616c 7365 7d2c 2022 6178 6973  ": False}, "axis
+000132c0: 5469 636b 223a 207b 2273 686f 7722 3a20  Tick": {"show": 
+000132d0: 4661 6c73 657d 7d0a 2020 2020 2020 2020  False}}.        
+000132e0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+000132f0: 2020 2020 2020 656c 6966 2076 6172 6961        elif varia
+00013300: 6e74 203d 3d20 226d 696e 696d 616c 223a  nt == "minimal":
+00013310: 0a20 2020 2020 2020 2020 2020 2065 6368  .            ech
+00013320: 6172 745f 6f70 7469 6f6e 732e 7570 6461  art_options.upda
+00013330: 7465 280a 2020 2020 2020 2020 2020 2020  te(.            
+00013340: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
+00013350: 2020 2020 2020 2020 2020 2274 6f6f 6c62            "toolb
+00013360: 6f78 223a 207b 2273 686f 7722 3a20 4661  ox": {"show": Fa
+00013370: 6c73 657d 2c0a 2020 2020 2020 2020 2020  lse},.          
+00013380: 2020 2020 2020 2020 2020 226c 6567 656e            "legen
+00013390: 6422 3a20 7b22 7368 6f77 223a 2046 616c  d": {"show": Fal
+000133a0: 7365 7d2c 0a20 2020 2020 2020 2020 2020  se},.           
+000133b0: 2020 2020 2020 2020 2022 6772 6964 223a           "grid":
+000133c0: 207b 226c 6566 7422 3a20 2231 2522 2c20   {"left": "1%", 
+000133d0: 2272 6967 6874 223a 2022 3125 222c 2022  "right": "1%", "
+000133e0: 746f 7022 3a20 2231 2522 2c20 2262 6f74  top": "1%", "bot
+000133f0: 746f 6d22 3a20 2231 2522 7d2c 0a20 2020  tom": "1%"},.   
+00013400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013410: 2022 746f 6f6c 7469 7022 3a20 7b22 7368   "tooltip": {"sh
+00013420: 6f77 223a 2046 616c 7365 7d2c 0a20 2020  ow": False},.   
+00013430: 2020 2020 2020 2020 2020 2020 207d 0a20               }. 
+00013440: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00013450: 2020 2020 2020 2020 2066 6f72 2061 7869           for axi
+00013460: 736c 6973 7420 696e 205b 6563 6861 7274  slist in [echart
+00013470: 5f6f 7074 696f 6e73 5b22 7841 7869 7322  _options["xAxis"
+00013480: 5d2c 2065 6368 6172 745f 6f70 7469 6f6e  ], echart_option
+00013490: 735b 2279 4178 6973 225d 5d3a 0a20 2020  s["yAxis"]]:.   
+000134a0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+000134b0: 2061 7869 7320 696e 2061 7869 736c 6973   axis in axislis
+000134c0: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
+000134d0: 2020 2020 2020 2061 7869 732e 7570 6461         axis.upda
+000134e0: 7465 280a 2020 2020 2020 2020 2020 2020  te(.            
+000134f0: 2020 2020 2020 2020 2020 2020 7b0a 2020              {.  
+00013500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013510: 2020 2020 2020 2020 2020 2261 7869 734c            "axisL
+00013520: 696e 6522 3a20 7b22 7368 6f77 223a 2046  ine": {"show": F
+00013530: 616c 7365 7d2c 0a20 2020 2020 2020 2020  alse},.         
+00013540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013550: 2020 2022 6178 6973 5469 636b 223a 207b     "axisTick": {
+00013560: 2273 686f 7722 3a20 4661 6c73 657d 2c0a  "show": False},.
+00013570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013580: 2020 2020 2020 2020 2020 2020 2273 706c              "spl
+00013590: 6974 4c69 6e65 223a 207b 2273 686f 7722  itLine": {"show"
+000135a0: 3a20 4661 6c73 657d 2c0a 2020 2020 2020  : False},.      
+000135b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000135c0: 2020 2020 2020 2261 7869 734c 6162 656c        "axisLabel
+000135d0: 223a 207b 2273 686f 7722 3a20 4661 6c73  ": {"show": Fals
+000135e0: 657d 2c0a 2020 2020 2020 2020 2020 2020  e},.            
+000135f0: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
+00013600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013610: 2020 290a 0a20 2020 2061 7379 6e63 2064    )..    async d
+00013620: 6566 205f 6372 6561 7465 5f74 7265 6e64  ef _create_trend
+00013630: 5f63 6861 7274 280a 2020 2020 2020 2020  _chart(.        
+00013640: 7365 6c66 2c0a 2020 2020 2020 2020 6178  self,.        ax
+00013650: 6573 3a20 556e 696f 6e5b 6c69 7374 5b73  es: Union[list[s
+00013660: 7472 5d2c 2073 7472 5d2c 0a20 2020 2020  tr], str],.     
+00013670: 2020 206f 7264 6572 3a20 696e 742c 0a20     order: int,. 
+00013680: 2020 2020 2020 2064 6174 615f 6d61 7070         data_mapp
+00013690: 696e 675f 746f 5f74 7570 6c65 733a 204f  ing_to_tuples: O
+000136a0: 7074 696f 6e61 6c5b 6469 6374 5d2c 0a20  ptional[dict],. 
+000136b0: 2020 2020 2020 2065 6368 6172 745f 6f70         echart_op
+000136c0: 7469 6f6e 733a 2064 6963 742c 0a20 2020  tions: dict,.   
+000136d0: 2020 2020 2073 6572 6965 735f 6f70 7469       series_opti
+000136e0: 6f6e 733a 2055 6e69 6f6e 5b64 6963 742c  ons: Union[dict,
+000136f0: 206c 6973 745b 6469 6374 5d5d 2c0a 2020   list[dict]],.  
+00013700: 2020 2020 2020 7661 6c75 6573 3a20 4f70        values: Op
+00013710: 7469 6f6e 616c 5b55 6e69 6f6e 5b6c 6973  tional[Union[lis
+00013720: 745b 556e 696f 6e5b 7374 722c 2074 7570  t[Union[str, tup
+00013730: 6c65 5d5d 2c20 7374 722c 2074 7570 6c65  le]], str, tuple
+00013740: 5d5d 203d 204e 6f6e 652c 0a20 2020 2020  ]] = None,.     
+00013750: 2020 2078 5f61 7869 735f 6e61 6d65 733a     x_axis_names:
+00013760: 204f 7074 696f 6e61 6c5b 556e 696f 6e5b   Optional[Union[
+00013770: 7374 722c 206c 6973 745b 7374 725d 5d5d  str, list[str]]]
+00013780: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+00013790: 2079 5f61 7869 735f 6e61 6d65 733a 204f   y_axis_names: O
+000137a0: 7074 696f 6e61 6c5b 556e 696f 6e5b 7374  ptional[Union[st
+000137b0: 722c 206c 6973 745b 7374 725d 5d5d 203d  r, list[str]]] =
+000137c0: 204e 6f6e 652c 0a20 2020 2020 2020 2073   None,.        s
+000137d0: 686f 775f 7661 6c75 6573 3a20 4f70 7469  how_values: Opti
+000137e0: 6f6e 616c 5b55 6e69 6f6e 5b6c 6973 745b  onal[Union[list[
+000137f0: 7374 725d 2c20 7374 725d 5d20 3d20 4e6f  str], str]] = No
+00013800: 6e65 2c0a 2020 2020 2020 2020 7661 7269  ne,.        vari
+00013810: 616e 743a 204f 7074 696f 6e61 6c5b 7374  ant: Optional[st
+00013820: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
+00013830: 2020 202a 2a72 6570 6f72 745f 7061 7261     **report_para
+00013840: 6d73 2c0a 2020 2020 293a 0a20 2020 2020  ms,.    ):.     
+00013850: 2020 2022 2222 0a20 2020 2020 2020 2043     """.        C
+00013860: 7265 6174 6520 6120 6c69 6e65 2063 6861  reate a line cha
+00013870: 7274 2069 6e20 7468 6520 6461 7368 626f  rt in the dashbo
+00013880: 6172 642e 0a20 2020 2020 2020 203a 7061  ard..        :pa
+00013890: 7261 6d20 6461 7461 3a20 7468 6520 6461  ram data: the da
+000138a0: 7461 206f 6620 7468 6520 6368 6172 740a  ta of the chart.
+000138b0: 2020 2020 2020 2020 3a70 6172 616d 2061          :param a
+000138c0: 7865 733a 2074 6865 206e 616d 6573 206f  xes: the names o
+000138d0: 6620 7468 6520 636f 6c75 6d6e 7320 746f  f the columns to
+000138e0: 2062 6520 7573 6564 2061 7320 6178 6973   be used as axis
+000138f0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00013900: 7661 6c75 6573 3a20 7468 6520 6e61 6d65  values: the name
+00013910: 7320 6f66 2074 6865 2063 6f6c 756d 6e73  s of the columns
+00013920: 2074 6f20 6265 2075 7365 6420 6173 2076   to be used as v
+00013930: 616c 7565 730a 2020 2020 2020 2020 3a70  alues.        :p
+00013940: 6172 616d 2078 5f61 7869 735f 6e61 6d65  aram x_axis_name
+00013950: 733a 2074 6865 206e 616d 6520 6f66 2074  s: the name of t
+00013960: 6865 2078 2061 7865 730a 2020 2020 2020  he x axes.      
+00013970: 2020 3a70 6172 616d 2079 5f61 7869 735f    :param y_axis_
+00013980: 6e61 6d65 733a 2074 6865 206e 616d 6520  names: the name 
+00013990: 6f66 2074 6865 2079 2061 7865 730a 2020  of the y axes.  
+000139a0: 2020 2020 2020 3a70 6172 616d 2065 6368        :param ech
+000139b0: 6172 745f 6f70 7469 6f6e 733a 2074 6865  art_options: the
+000139c0: 206f 7074 696f 6e73 206f 6620 7468 6520   options of the 
+000139d0: 6368 6172 740a 2020 2020 2020 2020 3a70  chart.        :p
+000139e0: 6172 616d 2073 6572 6965 735f 6f70 7469  aram series_opti
+000139f0: 6f6e 733a 2074 6865 206f 7074 696f 6e73  ons: the options
+00013a00: 206f 6620 7468 6520 7365 7269 6573 206f   of the series o
+00013a10: 6620 7468 6520 6368 6172 740a 2020 2020  f the chart.    
+00013a20: 2020 2020 3a70 6172 616d 2062 6f74 746f      :param botto
+00013a30: 6d5f 746f 6f6c 626f 783a 2077 6865 7468  m_toolbox: wheth
+00013a40: 6572 2074 6f20 7368 6f77 2074 6865 2074  er to show the t
+00013a50: 6f6f 6c62 6f78 206f 6e20 746f 7020 6f66  oolbox on top of
+00013a60: 2074 6865 2063 6861 7274 0a20 2020 2020   the chart.     
+00013a70: 2020 203a 7061 7261 6d20 6f72 6465 723a     :param order:
+00013a80: 2074 6865 206f 7264 6572 206f 6620 7468   the order of th
+00013a90: 6520 6368 6172 7420 696e 2074 6865 2064  e chart in the d
+00013aa0: 6173 6862 6f61 7264 0a20 2020 2020 2020  ashboard.       
+00013ab0: 203a 7061 7261 6d20 7265 706f 7274 5f70   :param report_p
+00013ac0: 6172 616d 733a 2061 6464 6974 696f 6e61  arams: additiona
+00013ad0: 6c20 7265 706f 7274 2070 6172 616d 6574  l report paramet
+00013ae0: 6572 7320 6173 206b 6579 2d76 616c 7565  ers as key-value
+00013af0: 2070 6169 7273 0a20 2020 2020 2020 2022   pairs.        "
+00013b00: 2222 0a20 2020 2020 2020 2073 656c 662e  "".        self.
+00013b10: 5f61 7070 6c79 5f76 6172 6961 6e74 2865  _apply_variant(e
+00013b20: 6368 6172 745f 6f70 7469 6f6e 732c 2076  chart_options, v
+00013b30: 6172 6961 6e74 290a 2020 2020 2020 2020  ariant).        
+00013b40: 6966 2069 7369 6e73 7461 6e63 6528 6178  if isinstance(ax
+00013b50: 6573 2c20 7374 7229 3a0a 2020 2020 2020  es, str):.      
+00013b60: 2020 2020 2020 6178 6573 203d 205b 6178        axes = [ax
+00013b70: 6573 5d0a 2020 2020 2020 2020 6966 2069  es].        if i
+00013b80: 7369 6e73 7461 6e63 6528 7661 6c75 6573  sinstance(values
+00013b90: 2c20 7374 7229 206f 7220 6973 696e 7374  , str) or isinst
+00013ba0: 616e 6365 2876 616c 7565 732c 2074 7570  ance(values, tup
+00013bb0: 6c65 293a 0a20 2020 2020 2020 2020 2020  le):.           
+00013bc0: 2076 616c 7565 7320 3d20 5b76 616c 7565   values = [value
+00013bd0: 735d 0a20 2020 2020 2020 2069 6620 7368  s].        if sh
+00013be0: 6f77 5f76 616c 7565 7320 6973 204e 6f6e  ow_values is Non
+00013bf0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00013c00: 686f 775f 7661 6c75 6573 203d 205b 5d0a  how_values = [].
+00013c10: 0a20 2020 2020 2020 2069 6620 2278 5f61  .        if "x_a
+00013c20: 7869 735f 6e61 6d65 2220 696e 2072 6570  xis_name" in rep
+00013c30: 6f72 745f 7061 7261 6d73 3a0a 2020 2020  ort_params:.    
+00013c40: 2020 2020 2020 2020 785f 6178 6973 5f6e          x_axis_n
+00013c50: 616d 6573 203d 205b 7265 706f 7274 5f70  ames = [report_p
+00013c60: 6172 616d 735b 2278 5f61 7869 735f 6e61  arams["x_axis_na
+00013c70: 6d65 225d 5d0a 2020 2020 2020 2020 656c  me"]].        el
+00013c80: 6966 2069 7369 6e73 7461 6e63 6528 785f  if isinstance(x_
+00013c90: 6178 6973 5f6e 616d 6573 2c20 7374 7229  axis_names, str)
+00013ca0: 3a0a 2020 2020 2020 2020 2020 2020 785f  :.            x_
+00013cb0: 6178 6973 5f6e 616d 6573 203d 205b 785f  axis_names = [x_
+00013cc0: 6178 6973 5f6e 616d 6573 5d0a 2020 2020  axis_names].    
+00013cd0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00013ce0: 2020 2020 2020 785f 6178 6973 5f6e 616d        x_axis_nam
+00013cf0: 6573 203d 205b 5d0a 0a20 2020 2020 2020  es = []..       
+00013d00: 2069 6620 2279 5f61 7869 735f 6e61 6d65   if "y_axis_name
+00013d10: 2220 696e 2072 6570 6f72 745f 7061 7261  " in report_para
+00013d20: 6d73 3a0a 2020 2020 2020 2020 2020 2020  ms:.            
+00013d30: 795f 6178 6973 5f6e 616d 6573 203d 205b  y_axis_names = [
+00013d40: 7265 706f 7274 5f70 6172 616d 735b 2279  report_params["y
+00013d50: 5f61 7869 735f 6e61 6d65 225d 5d0a 2020  _axis_name"]].  
+00013d60: 2020 2020 2020 656c 6966 2069 7369 6e73        elif isins
+00013d70: 7461 6e63 6528 795f 6178 6973 5f6e 616d  tance(y_axis_nam
+00013d80: 6573 2c20 7374 7229 3a0a 2020 2020 2020  es, str):.      
+00013d90: 2020 2020 2020 795f 6178 6973 5f6e 616d        y_axis_nam
+00013da0: 6573 203d 205b 795f 6178 6973 5f6e 616d  es = [y_axis_nam
+00013db0: 6573 5d0a 2020 2020 2020 2020 656c 7365  es].        else
+00013dc0: 3a0a 2020 2020 2020 2020 2020 2020 795f  :.            y_
+00013dd0: 6178 6973 5f6e 616d 6573 203d 205b 5d0a  axis_names = [].
+00013de0: 0a20 2020 2020 2020 2076 616c 7565 7320  .        values 
+00013df0: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
+00013e00: 5b76 2066 6f72 2076 2069 6e20 6461 7461  [v for v in data
+00013e10: 5f6d 6170 7069 6e67 5f74 6f5f 7475 706c  _mapping_to_tupl
+00013e20: 6573 2e6b 6579 7328 2920 6966 2076 206e  es.keys() if v n
+00013e30: 6f74 2069 6e20 6178 6573 5d0a 2020 2020  ot in axes].    
+00013e40: 2020 2020 2020 2020 6966 2076 616c 7565          if value
+00013e50: 7320 6973 204e 6f6e 650a 2020 2020 2020  s is None.      
+00013e60: 2020 2020 2020 656c 7365 2076 616c 7565        else value
+00013e70: 730a 2020 2020 2020 2020 290a 2020 2020  s.        ).    
+00013e80: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
+00013e90: 6528 7365 7269 6573 5f6f 7074 696f 6e73  e(series_options
+00013ea0: 2c20 6469 6374 293a 0a20 2020 2020 2020  , dict):.       
+00013eb0: 2020 2020 2073 6572 6965 735f 6f70 7469       series_opti
+00013ec0: 6f6e 7320 3d20 5b73 6572 6965 735f 6f70  ons = [series_op
+00013ed0: 7469 6f6e 735d 202a 206c 656e 2876 616c  tions] * len(val
+00013ee0: 7565 7329 0a20 2020 2020 2020 2065 6c69  ues).        eli
+00013ef0: 6620 6c65 6e28 7365 7269 6573 5f6f 7074  f len(series_opt
+00013f00: 696f 6e73 2920 3c20 6c65 6e28 7661 6c75  ions) < len(valu
+00013f10: 6573 293a 0a20 2020 2020 2020 2020 2020  es):.           
+00013f20: 2073 6572 6965 735f 6f70 7469 6f6e 7320   series_options 
+00013f30: 3d20 7365 7269 6573 5f6f 7074 696f 6e73  = series_options
+00013f40: 202b 205b 7365 7269 6573 5f6f 7074 696f   + [series_optio
+00013f50: 6e73 5b2d 315d 5d20 2a20 280a 2020 2020  ns[-1]] * (.    
+00013f60: 2020 2020 2020 2020 2020 2020 6c65 6e28              len(
+00013f70: 7661 6c75 6573 2920 2d20 6c65 6e28 7365  values) - len(se
+00013f80: 7269 6573 5f6f 7074 696f 6e73 290a 2020  ries_options).  
+00013f90: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00013fa0: 2020 2020 656c 6966 206c 656e 2873 6572      elif len(ser
+00013fb0: 6965 735f 6f70 7469 6f6e 7329 203e 206c  ies_options) > l
+00013fc0: 656e 2876 616c 7565 7329 3a0a 2020 2020  en(values):.    
+00013fd0: 2020 2020 2020 2020 7365 7269 6573 5f6f          series_o
+00013fe0: 7074 696f 6e73 203d 2073 6572 6965 735f  ptions = series_
+00013ff0: 6f70 7469 6f6e 735b 3a20 6c65 6e28 7661  options[: len(va
+00014000: 6c75 6573 295d 0a0a 2020 2020 2020 2020  lues)]..        
+00014010: 6563 6861 7274 5f6f 7074 696f 6e73 5b22  echart_options["
+00014020: 7365 7269 6573 225d 203d 205b 0a20 2020  series"] = [.   
+00014030: 2020 2020 2020 2020 2064 6565 705f 7570           deep_up
+00014040: 6461 7465 280a 2020 2020 2020 2020 2020  date(.          
+00014050: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
+00014060: 2020 2020 2020 2020 2020 2020 226e 616d              "nam
+00014070: 6522 3a20 6e61 6d65 2069 6620 6973 696e  e": name if isin
+00014080: 7374 616e 6365 286e 616d 652c 2073 7472  stance(name, str
+00014090: 2920 656c 7365 2022 20c3 9720 222e 6a6f  ) else " .. ".jo
+000140a0: 696e 286e 616d 6529 2c0a 2020 2020 2020  in(name),.      
+000140b0: 2020 2020 2020 2020 2020 2020 2020 226c                "l
+000140c0: 6162 656c 223a 207b 2273 686f 7722 3a20  abel": {"show": 
+000140d0: 7368 6f77 5f76 616c 7565 7320 3d3d 2022  show_values == "
+000140e0: 616c 6c22 206f 7220 6e61 6d65 2069 6e20  all" or name in 
+000140f0: 7368 6f77 5f76 616c 7565 737d 2c0a 2020  show_values},.  
+00014100: 2020 2020 2020 2020 2020 2020 2020 7d2c                },
+00014110: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014120: 2073 6572 6965 735f 6f70 7469 6f6e 735b   series_options[
+00014130: 695d 2c0a 2020 2020 2020 2020 2020 2020  i],.            
+00014140: 290a 2020 2020 2020 2020 2020 2020 666f  ).            fo
+00014150: 7220 692c 206e 616d 6520 696e 2065 6e75  r i, name in enu
+00014160: 6d65 7261 7465 2876 616c 7565 7329 0a20  merate(values). 
+00014170: 2020 2020 2020 205d 0a0a 2020 2020 2020         ]..      
+00014180: 2020 666f 7220 692c 2061 7869 735f 6f70    for i, axis_op
+00014190: 7469 6f6e 7320 696e 2065 6e75 6d65 7261  tions in enumera
+000141a0: 7465 2865 6368 6172 745f 6f70 7469 6f6e  te(echart_option
+000141b0: 735b 2278 4178 6973 225d 293a 0a20 2020  s["xAxis"]):.   
+000141c0: 2020 2020 2020 2020 2061 7869 735f 6f70           axis_op
+000141d0: 7469 6f6e 735b 226e 616d 6522 5d20 3d20  tions["name"] = 
+000141e0: 785f 6178 6973 5f6e 616d 6573 5b69 5d20  x_axis_names[i] 
+000141f0: 6966 2069 203c 206c 656e 2878 5f61 7869  if i < len(x_axi
+00014200: 735f 6e61 6d65 7329 2065 6c73 6520 4e6f  s_names) else No
+00014210: 6e65 0a20 2020 2020 2020 2020 2020 2069  ne.            i
+00014220: 6620 6178 6973 5f6f 7074 696f 6e73 5b22  f axis_options["
+00014230: 6e61 6d65 225d 2061 6e64 2022 6e61 6d65  name"] and "name
+00014240: 4761 7022 206e 6f74 2069 6e20 6178 6973  Gap" not in axis
+00014250: 5f6f 7074 696f 6e73 3a0a 2020 2020 2020  _options:.      
+00014260: 2020 2020 2020 2020 2020 6178 6973 5f6f            axis_o
+00014270: 7074 696f 6e73 5b22 6e61 6d65 4761 7022  ptions["nameGap"
+00014280: 5d20 3d20 3332 0a0a 2020 2020 2020 2020  ] = 32..        
+00014290: 666f 7220 692c 2061 7869 735f 6f70 7469  for i, axis_opti
+000142a0: 6f6e 7320 696e 2065 6e75 6d65 7261 7465  ons in enumerate
+000142b0: 2865 6368 6172 745f 6f70 7469 6f6e 735b  (echart_options[
+000142c0: 2279 4178 6973 225d 293a 0a20 2020 2020  "yAxis"]):.     
+000142d0: 2020 2020 2020 2061 7869 735f 6f70 7469         axis_opti
+000142e0: 6f6e 735b 226e 616d 6522 5d20 3d20 795f  ons["name"] = y_
+000142f0: 6178 6973 5f6e 616d 6573 5b69 5d20 6966  axis_names[i] if
+00014300: 2069 203c 206c 656e 2879 5f61 7869 735f   i < len(y_axis_
+00014310: 6e61 6d65 7329 2065 6c73 6520 4e6f 6e65  names) else None
+00014320: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00014330: 6178 6973 5f6f 7074 696f 6e73 5b22 6e61  axis_options["na
+00014340: 6d65 225d 2061 6e64 2022 6e61 6d65 4761  me"] and "nameGa
+00014350: 7022 206e 6f74 2069 6e20 6178 6973 5f6f  p" not in axis_o
+00014360: 7074 696f 6e73 3a0a 2020 2020 2020 2020  ptions:.        
+00014370: 2020 2020 2020 2020 6178 6973 5f6f 7074          axis_opt
+00014380: 696f 6e73 5b22 6e61 6d65 4761 7022 5d20  ions["nameGap"] 
+00014390: 3d20 2d32 340a 2020 2020 2020 2020 2020  = -24.          
+000143a0: 2020 2020 2020 6178 6973 5f6f 7074 696f        axis_optio
+000143b0: 6e73 5b22 6f66 6673 6574 225d 203d 2033  ns["offset"] = 3
+000143c0: 360a 2020 2020 2020 2020 2020 2020 2020  6.              
+000143d0: 2020 6563 6861 7274 5f6f 7074 696f 6e73    echart_options
+000143e0: 5b22 6772 6964 225d 5b22 6c65 6674 225d  ["grid"]["left"]
+000143f0: 203d 2022 3425 220a 2020 2020 2020 2020   = "4%".        
+00014400: 2020 2020 2020 2020 6178 6973 5f6f 7074          axis_opt
+00014410: 696f 6e73 5b22 6178 6973 5469 636b 225d  ions["axisTick"]
+00014420: 203d 207b 2273 686f 7722 3a20 4661 6c73   = {"show": Fals
+00014430: 657d 0a20 2020 2020 2020 2020 2020 2020  e}.             
+00014440: 2020 2061 7869 735f 6f70 7469 6f6e 735b     axis_options[
+00014450: 2261 7869 734c 696e 6522 5d20 3d20 7b22  "axisLine"] = {"
+00014460: 7368 6f77 223a 2046 616c 7365 7d0a 0a20  show": False}.. 
+00014470: 2020 2020 2020 2061 7761 6974 2073 656c         await sel
+00014480: 662e 5f63 7265 6174 655f 6563 6861 7274  f._create_echart
+00014490: 280a 2020 2020 2020 2020 2020 2020 6f72  (.            or
+000144a0: 6465 723d 6f72 6465 722c 0a20 2020 2020  der=order,.     
+000144b0: 2020 2020 2020 206f 7074 696f 6e73 3d65         options=e
+000144c0: 6368 6172 745f 6f70 7469 6f6e 732c 0a20  chart_options,. 
+000144d0: 2020 2020 2020 2020 2020 2064 6174 615f             data_
+000144e0: 6d61 7070 696e 675f 746f 5f74 7570 6c65  mapping_to_tuple
+000144f0: 733d 6461 7461 5f6d 6170 7069 6e67 5f74  s=data_mapping_t
+00014500: 6f5f 7475 706c 6573 2c0a 2020 2020 2020  o_tuples,.      
+00014510: 2020 2020 2020 6669 656c 6473 3d61 7865        fields=axe
+00014520: 7320 2b20 7661 6c75 6573 2c0a 2020 2020  s + values,.    
+00014530: 2020 2020 2020 2020 2a2a 7265 706f 7274          **report
+00014540: 5f70 6172 616d 732c 0a20 2020 2020 2020  _params,.       
+00014550: 2029 0a0a 2020 2020 4061 6464 5f74 6f5f   )..    @add_to_
+00014560: 6765 6e65 7261 6c5f 6173 796e 635f 6772  general_async_gr
+00014570: 6f75 700a 2020 2020 6173 796e 6320 6465  oup.    async de
+00014580: 6620 6672 6565 5f65 6368 6172 7473 280a  f free_echarts(.
+00014590: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+000145a0: 2020 2020 2020 6461 7461 3a20 4f70 7469        data: Opti
+000145b0: 6f6e 616c 5b55 6e69 6f6e 5b73 7472 2c20  onal[Union[str, 
+000145c0: 4461 7461 4672 616d 652c 206c 6973 745b  DataFrame, list[
+000145d0: 6469 6374 5d5d 5d20 3d20 4e6f 6e65 2c0a  dict]]] = None,.
+000145e0: 2020 2020 2020 2020 6f70 7469 6f6e 733a          options:
+000145f0: 204f 7074 696f 6e61 6c5b 6469 6374 5d20   Optional[dict] 
+00014600: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+00014610: 7261 775f 6f70 7469 6f6e 733a 204f 7074  raw_options: Opt
+00014620: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+00014630: 652c 0a20 2020 2020 2020 206f 7264 6572  e,.        order
+00014640: 3a20 4f70 7469 6f6e 616c 5b69 6e74 5d20  : Optional[int] 
+00014650: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+00014660: 7469 746c 653a 204f 7074 696f 6e61 6c5b  title: Optional[
+00014670: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
+00014680: 2020 2020 2072 6f77 735f 7369 7a65 3a20       rows_size: 
+00014690: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
+000146a0: 4e6f 6e65 2c0a 2020 2020 2020 2020 636f  None,.        co
+000146b0: 6c73 5f73 697a 653a 204f 7074 696f 6e61  ls_size: Optiona
+000146c0: 6c5b 696e 745d 203d 204e 6f6e 652c 0a20  l[int] = None,. 
+000146d0: 2020 2020 2020 2070 6164 6469 6e67 3a20         padding: 
+000146e0: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+000146f0: 4e6f 6e65 2c0a 2020 2020 2020 2020 6669  None,.        fi
+00014700: 656c 6473 3a20 4f70 7469 6f6e 616c 5b6c  elds: Optional[l
+00014710: 6973 745d 203d 204e 6f6e 652c 0a20 2020  ist] = None,.   
+00014720: 2020 2020 2064 6174 615f 6973 5f6e 6f74       data_is_not
+00014730: 5f64 663a 2062 6f6f 6c20 3d20 4661 6c73  _df: bool = Fals
+00014740: 652c 0a20 2020 2029 3a0a 2020 2020 2020  e,.    ):.      
+00014750: 2020 2222 220a 2020 2020 2020 2020 4372    """.        Cr
+00014760: 6561 7465 2061 6e20 6563 6861 7274 7320  eate an echarts 
+00014770: 6368 6172 7420 7769 7468 2063 7573 746f  chart with custo
+00014780: 6d20 6f70 7469 6f6e 732e 0a20 2020 2020  m options..     
+00014790: 2020 203a 7061 7261 6d20 6461 7461 3a20     :param data: 
+000147a0: 7468 6520 6461 7461 206f 6620 7468 6520  the data of the 
+000147b0: 6368 6172 740a 2020 2020 2020 2020 3a70  chart.        :p
+000147c0: 6172 616d 206f 7074 696f 6e73 3a20 7468  aram options: th
+000147d0: 6520 6f70 7469 6f6e 7320 6f66 2074 6865  e options of the
+000147e0: 2063 6861 7274 0a20 2020 2020 2020 203a   chart.        :
+000147f0: 7061 7261 6d20 7261 775f 6f70 7469 6f6e  param raw_option
+00014800: 733a 2074 6865 2072 6177 206f 7074 696f  s: the raw optio
+00014810: 6e73 206f 6620 7468 6520 6368 6172 740a  ns of the chart.
+00014820: 2020 2020 2020 2020 3a70 6172 616d 206f          :param o
+00014830: 7264 6572 3a20 7468 6520 6f72 6465 7220  rder: the order 
+00014840: 6f66 2074 6865 2063 6861 7274 2069 6e20  of the chart in 
+00014850: 7468 6520 6461 7368 626f 6172 640a 2020  the dashboard.  
+00014860: 2020 2020 2020 3a70 6172 616d 2074 6974        :param tit
+00014870: 6c65 3a20 7468 6520 7469 746c 6520 6f66  le: the title of
+00014880: 2074 6865 2063 6861 7274 0a20 2020 2020   the chart.     
+00014890: 2020 203a 7061 7261 6d20 726f 7773 5f73     :param rows_s
+000148a0: 697a 653a 2074 6865 2072 6f77 7320 7369  ize: the rows si
+000148b0: 7a65 206f 6620 7468 6520 6368 6172 740a  ze of the chart.
+000148c0: 2020 2020 2020 2020 3a70 6172 616d 2063          :param c
+000148d0: 6f6c 735f 7369 7a65 3a20 7468 6520 636f  ols_size: the co
+000148e0: 6c75 6d6e 7320 7369 7a65 206f 6620 7468  lumns size of th
+000148f0: 6520 6368 6172 740a 2020 2020 2020 2020  e chart.        
+00014900: 3a70 6172 616d 2070 6164 6469 6e67 3a20  :param padding: 
+00014910: 7468 6520 7061 6464 696e 6720 6f66 2074  the padding of t
+00014920: 6865 2063 6861 7274 0a20 2020 2020 2020  he chart.       
+00014930: 203a 7061 7261 6d20 6669 656c 6473 3a20   :param fields: 
+00014940: 7468 6520 6669 656c 6473 206f 6620 7468  the fields of th
+00014950: 6520 6368 6172 740a 2020 2020 2020 2020  e chart.        
+00014960: 3a70 6172 616d 2064 6174 615f 6973 5f6e  :param data_is_n
+00014970: 6f74 5f64 663a 2077 6865 7468 6572 2074  ot_df: whether t
+00014980: 6865 2064 6174 6120 6973 206e 6f74 2061  he data is not a
+00014990: 2064 6174 6166 7261 6d65 0a20 2020 2020   dataframe.     
+000149a0: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
+000149b0: 6620 6e6f 7420 6f70 7469 6f6e 7320 616e  f not options an
+000149c0: 6420 6e6f 7420 7261 775f 6f70 7469 6f6e  d not raw_option
+000149d0: 733a 0a20 2020 2020 2020 2020 2020 206c  s:.            l
+000149e0: 6f67 5f65 7272 6f72 280a 2020 2020 2020  og_error(.      
+000149f0: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
+00014a00: 2c20 2245 6974 6865 7220 6f70 7469 6f6e  , "Either option
+00014a10: 7320 6f72 2072 6177 5f6f 7074 696f 6e73  s or raw_options
+00014a20: 206d 7573 7420 6265 2070 726f 7669 6465   must be provide
+00014a30: 6422 2c20 5661 6c75 6545 7272 6f72 0a20  d", ValueError. 
+00014a40: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00014a50: 2020 2020 2069 6620 6f70 7469 6f6e 7320       if options 
+00014a60: 616e 6420 6e6f 7420 6973 696e 7374 616e  and not isinstan
+00014a70: 6365 2864 6174 612c 2044 6174 6146 7261  ce(data, DataFra
+00014a80: 6d65 2920 616e 6420 6461 7461 2069 7320  me) and data is 
+00014a90: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00014aa0: 2020 6c6f 675f 6572 726f 7228 0a20 2020    log_error(.   
+00014ab0: 2020 2020 2020 2020 2020 2020 206c 6f67               log
+00014ac0: 6765 722c 2022 6461 7461 206d 7573 7420  ger, "data must 
+00014ad0: 6265 2070 726f 7669 6465 6420 7768 656e  be provided when
+00014ae0: 206f 7074 696f 6e73 2069 7320 7072 6f76   options is prov
+00014af0: 6964 6564 222c 2044 6174 6145 7272 6f72  ided", DataError
+00014b00: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+00014b10: 2020 2020 2020 2069 6620 6f70 7469 6f6e         if option
+00014b20: 7320 616e 6420 7261 775f 6f70 7469 6f6e  s and raw_option
+00014b30: 733a 0a20 2020 2020 2020 2020 2020 206c  s:.            l
+00014b40: 6f67 5f65 7272 6f72 280a 2020 2020 2020  og_error(.      
+00014b50: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
+00014b60: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00014b70: 2020 224f 6e6c 7920 6f6e 6520 6f66 206f    "Only one of o
+00014b80: 7074 696f 6e73 2061 6e64 2072 6177 5f6f  ptions and raw_o
+00014b90: 7074 696f 6e73 2063 616e 2062 6520 7072  ptions can be pr
+00014ba0: 6f76 6964 6564 222c 0a20 2020 2020 2020  ovided",.       
+00014bb0: 2020 2020 2020 2020 2056 616c 7565 4572           ValueEr
+00014bc0: 726f 722c 0a20 2020 2020 2020 2020 2020  ror,.           
+00014bd0: 2029 0a0a 2020 2020 2020 2020 6966 2072   )..        if r
+00014be0: 6177 5f6f 7074 696f 6e73 3a0a 2020 2020  aw_options:.    
+00014bf0: 2020 2020 2020 2020 6f70 7469 6f6e 7320          options 
+00014c00: 3d20 7472 616e 7366 6f72 6d5f 6469 6374  = transform_dict
+00014c10: 5f6a 735f 746f 5f70 7928 7261 775f 6f70  _js_to_py(raw_op
+00014c20: 7469 6f6e 7329 0a20 2020 2020 2020 2020  tions).         
+00014c30: 2020 2064 6174 6120 3d20 7265 7472 6965     data = retrie
+00014c40: 7665 5f64 6174 615f 6672 6f6d 5f6f 7074  ve_data_from_opt
+00014c50: 696f 6e73 286f 7074 696f 6e73 290a 2020  ions(options).  
+00014c60: 2020 2020 2020 2020 2020 6f70 7469 6f6e            option
+00014c70: 735b 2264 6174 6173 6574 225d 203d 207b  s["dataset"] = {
+00014c80: 2273 6f75 7263 6522 3a20 2223 7365 745f  "source": "#set_
+00014c90: 6461 7461 2322 7d0a 2020 2020 2020 2020  data#"}.        
+00014ca0: 2020 2020 6669 656c 6473 203d 205b 6c69      fields = [li
+00014cb0: 7374 2864 6174 615b 305d 2e6b 6579 7328  st(data[0].keys(
+00014cc0: 2929 5d0a 2020 2020 2020 2020 656c 7365  ))].        else
+00014cd0: 3a0a 2020 2020 2020 2020 2020 2020 6f70  :.            op
+00014ce0: 7469 6f6e 7320 3d20 6465 6570 636f 7079  tions = deepcopy
+00014cf0: 286f 7074 696f 6e73 290a 0a20 2020 2020  (options)..     
+00014d00: 2020 2061 7761 6974 2073 656c 662e 5f63     await self._c
+00014d10: 7265 6174 655f 6563 6861 7274 280a 2020  reate_echart(.  
+00014d20: 2020 2020 2020 2020 2020 6f72 6465 723d            order=
+00014d30: 6f72 6465 722c 0a20 2020 2020 2020 2020  order,.         
+00014d40: 2020 2064 6174 615f 6d61 7070 696e 675f     data_mapping_
+00014d50: 746f 5f74 7570 6c65 733d 6177 6169 7420  to_tuples=await 
+00014d60: 7365 6c66 2e5f 6368 6f6f 7365 5f64 6174  self._choose_dat
+00014d70: 6128 0a20 2020 2020 2020 2020 2020 2020  a(.             
+00014d80: 2020 206f 7264 6572 2c20 6461 7461 2c20     order, data, 
+00014d90: 6475 6d70 5f77 686f 6c65 3d64 6174 615f  dump_whole=data_
+00014da0: 6973 5f6e 6f74 5f64 660a 2020 2020 2020  is_not_df.      
+00014db0: 2020 2020 2020 292c 0a20 2020 2020 2020        ),.       
+00014dc0: 2020 2020 2066 6965 6c64 733d 6669 656c       fields=fiel
+00014dd0: 6473 2c0a 2020 2020 2020 2020 2020 2020  ds,.            
+00014de0: 6f70 7469 6f6e 733d 6f70 7469 6f6e 732c  options=options,
+00014df0: 0a20 2020 2020 2020 2020 2020 2074 6974  .            tit
+00014e00: 6c65 3d74 6974 6c65 2c0a 2020 2020 2020  le=title,.      
+00014e10: 2020 2020 2020 726f 7773 5f73 697a 653d        rows_size=
+00014e20: 726f 7773 5f73 697a 652c 0a20 2020 2020  rows_size,.     
+00014e30: 2020 2020 2020 2063 6f6c 735f 7369 7a65         cols_size
+00014e40: 3d63 6f6c 735f 7369 7a65 2c0a 2020 2020  =cols_size,.    
+00014e50: 2020 2020 2020 2020 7061 6464 696e 673d          padding=
+00014e60: 7061 6464 696e 672c 0a20 2020 2020 2020  padding,.       
+00014e70: 2029 0a0a 2020 2020 2320 4543 6861 7274   )..    # EChart
+00014e80: 730a 2020 2020 6c69 6e65 203d 2061 6464  s.    line = add
+00014e90: 5f74 6f5f 6765 6e65 7261 6c5f 6173 796e  _to_general_asyn
+00014ea0: 635f 6772 6f75 7028 6c69 6e65 5f63 6861  c_group(line_cha
+00014eb0: 7274 290a 2020 2020 6261 7220 3d20 6164  rt).    bar = ad
+00014ec0: 645f 746f 5f67 656e 6572 616c 5f61 7379  d_to_general_asy
+00014ed0: 6e63 5f67 726f 7570 2862 6172 5f63 6861  nc_group(bar_cha
+00014ee0: 7274 290a 2020 2020 7374 6163 6b65 645f  rt).    stacked_
+00014ef0: 6261 7220 3d20 6164 645f 746f 5f67 656e  bar = add_to_gen
+00014f00: 6572 616c 5f61 7379 6e63 5f67 726f 7570  eral_async_group
+00014f10: 2873 7461 636b 6564 5f62 6172 5f63 6861  (stacked_bar_cha
+00014f20: 7274 290a 2020 2020 6172 6561 203d 2061  rt).    area = a
+00014f30: 6464 5f74 6f5f 6765 6e65 7261 6c5f 6173  dd_to_general_as
+00014f40: 796e 635f 6772 6f75 7028 6172 6561 5f63  ync_group(area_c
+00014f50: 6861 7274 290a 2020 2020 7374 6163 6b65  hart).    stacke
+00014f60: 645f 6172 6561 203d 2061 6464 5f74 6f5f  d_area = add_to_
+00014f70: 6765 6e65 7261 6c5f 6173 796e 635f 6772  general_async_gr
+00014f80: 6f75 7028 7374 6163 6b65 645f 6172 6561  oup(stacked_area
+00014f90: 5f63 6861 7274 290a 2020 2020 7363 6174  _chart).    scat
+00014fa0: 7465 7220 3d20 6164 645f 746f 5f67 656e  ter = add_to_gen
+00014fb0: 6572 616c 5f61 7379 6e63 5f67 726f 7570  eral_async_group
+00014fc0: 2873 6361 7474 6572 5f63 6861 7274 290a  (scatter_chart).
+00014fd0: 2020 2020 686f 7269 7a6f 6e74 616c 5f62      horizontal_b
+00014fe0: 6172 203d 2061 6464 5f74 6f5f 6765 6e65  ar = add_to_gene
+00014ff0: 7261 6c5f 6173 796e 635f 6772 6f75 7028  ral_async_group(
+00015000: 686f 7269 7a6f 6e74 616c 5f62 6172 5f63  horizontal_bar_c
+00015010: 6861 7274 290a 2020 2020 7374 6163 6b65  hart).    stacke
+00015020: 645f 686f 7269 7a6f 6e74 616c 5f62 6172  d_horizontal_bar
+00015030: 203d 2061 6464 5f74 6f5f 6765 6e65 7261   = add_to_genera
+00015040: 6c5f 6173 796e 635f 6772 6f75 7028 7374  l_async_group(st
+00015050: 6163 6b65 645f 686f 7269 7a6f 6e74 616c  acked_horizontal
+00015060: 5f62 6172 5f63 6861 7274 290a 2020 2020  _bar_chart).    
+00015070: 7a65 726f 5f63 656e 7465 7265 645f 6261  zero_centered_ba
+00015080: 7220 3d20 6164 645f 746f 5f67 656e 6572  r = add_to_gener
+00015090: 616c 5f61 7379 6e63 5f67 726f 7570 287a  al_async_group(z
+000150a0: 6572 6f5f 6365 6e74 6572 6564 5f62 6172  ero_centered_bar
+000150b0: 5f63 6861 7274 290a 2020 2020 6675 6e6e  _chart).    funn
+000150c0: 656c 203d 2061 6464 5f74 6f5f 6765 6e65  el = add_to_gene
+000150d0: 7261 6c5f 6173 796e 635f 6772 6f75 7028  ral_async_group(
+000150e0: 6675 6e6e 656c 5f63 6861 7274 290a 2020  funnel_chart).  
+000150f0: 2020 7472 6565 203d 2061 6464 5f74 6f5f    tree = add_to_
+00015100: 6765 6e65 7261 6c5f 6173 796e 635f 6772  general_async_gr
+00015110: 6f75 7028 7472 6565 5f63 6861 7274 290a  oup(tree_chart).
+00015120: 2020 2020 7261 6461 7220 3d20 6164 645f      radar = add_
+00015130: 746f 5f67 656e 6572 616c 5f61 7379 6e63  to_general_async
+00015140: 5f67 726f 7570 2872 6164 6172 5f63 6861  _group(radar_cha
+00015150: 7274 290a 2020 2020 7069 6520 3d20 6164  rt).    pie = ad
+00015160: 645f 746f 5f67 656e 6572 616c 5f61 7379  d_to_general_asy
+00015170: 6e63 5f67 726f 7570 2870 6965 5f63 6861  nc_group(pie_cha
+00015180: 7274 290a 2020 2020 646f 7567 686e 7574  rt).    doughnut
+00015190: 203d 2061 6464 5f74 6f5f 6765 6e65 7261   = add_to_genera
+000151a0: 6c5f 6173 796e 635f 6772 6f75 7028 646f  l_async_group(do
+000151b0: 7567 686e 7574 5f63 6861 7274 290a 2020  ughnut_chart).  
+000151c0: 2020 726f 7365 203d 2061 6464 5f74 6f5f    rose = add_to_
+000151d0: 6765 6e65 7261 6c5f 6173 796e 635f 6772  general_async_gr
+000151e0: 6f75 7028 726f 7365 5f63 6861 7274 290a  oup(rose_chart).
+000151f0: 2020 2020 7375 6e62 7572 7374 203d 2061      sunburst = a
+00015200: 6464 5f74 6f5f 6765 6e65 7261 6c5f 6173  dd_to_general_as
+00015210: 796e 635f 6772 6f75 7028 7375 6e62 7572  ync_group(sunbur
+00015220: 7374 5f63 6861 7274 290a 2020 2020 7472  st_chart).    tr
+00015230: 6565 6d61 7020 3d20 6164 645f 746f 5f67  eemap = add_to_g
+00015240: 656e 6572 616c 5f61 7379 6e63 5f67 726f  eneral_async_gro
+00015250: 7570 2874 7265 656d 6170 5f63 6861 7274  up(treemap_chart
+00015260: 290a 2020 2020 7361 6e6b 6579 203d 2061  ).    sankey = a
+00015270: 6464 5f74 6f5f 6765 6e65 7261 6c5f 6173  dd_to_general_as
+00015280: 796e 635f 6772 6f75 7028 7361 6e6b 6579  ync_group(sankey
+00015290: 5f63 6861 7274 290a 2020 2020 6865 6174  _chart).    heat
+000152a0: 6d61 7020 3d20 6164 645f 746f 5f67 656e  map = add_to_gen
+000152b0: 6572 616c 5f61 7379 6e63 5f67 726f 7570  eral_async_group
+000152c0: 2868 6561 746d 6170 5f63 6861 7274 290a  (heatmap_chart).
+000152d0: 2020 2020 7072 6564 6963 7469 7665 5f6c      predictive_l
+000152e0: 696e 6520 3d20 6164 645f 746f 5f67 656e  ine = add_to_gen
+000152f0: 6572 616c 5f61 7379 6e63 5f67 726f 7570  eral_async_group
+00015300: 2870 7265 6469 6374 6976 655f 6c69 6e65  (predictive_line
+00015310: 5f63 6861 7274 290a 2020 2020 7370 6565  _chart).    spee
+00015320: 645f 6761 7567 6520 3d20 6164 645f 746f  d_gauge = add_to
+00015330: 5f67 656e 6572 616c 5f61 7379 6e63 5f67  _general_async_g
+00015340: 726f 7570 2873 7065 6564 5f67 6175 6765  roup(speed_gauge
+00015350: 5f63 6861 7274 290a 2020 2020 7368 696d  _chart).    shim
+00015360: 6f6b 755f 6761 7567 6520 3d20 6164 645f  oku_gauge = add_
+00015370: 746f 5f67 656e 6572 616c 5f61 7379 6e63  to_general_async
+00015380: 5f67 726f 7570 2873 6869 6d6f 6b75 5f67  _group(shimoku_g
+00015390: 6175 6765 5f63 6861 7274 290a 2020 2020  auge_chart).    
+000153a0: 7368 696d 6f6b 755f 6761 7567 6573 5f67  shimoku_gauges_g
+000153b0: 726f 7570 203d 2061 6464 5f74 6f5f 6765  roup = add_to_ge
+000153c0: 6e65 7261 6c5f 6173 796e 635f 6772 6f75  neral_async_grou
+000153d0: 7028 7368 696d 6f6b 755f 6761 7567 6573  p(shimoku_gauges
+000153e0: 5f67 726f 7570 290a 2020 2020 6761 7567  _group).    gaug
+000153f0: 655f 696e 6469 6361 746f 7220 3d20 6164  e_indicator = ad
+00015400: 645f 746f 5f67 656e 6572 616c 5f61 7379  d_to_general_asy
+00015410: 6e63 5f67 726f 7570 2867 6175 6765 5f69  nc_group(gauge_i
+00015420: 6e64 6963 6174 6f72 290a 2020 2020 746f  ndicator).    to
+00015430: 705f 626f 7474 6f6d 5f61 7265 6120 3d20  p_bottom_area = 
+00015440: 6164 645f 746f 5f67 656e 6572 616c 5f61  add_to_general_a
+00015450: 7379 6e63 5f67 726f 7570 2874 6f70 5f62  sync_group(top_b
+00015460: 6f74 746f 6d5f 6172 6561 5f63 6861 7274  ottom_area_chart
+00015470: 7329 0a20 2020 2074 6f70 5f62 6f74 746f  s).    top_botto
+00015480: 6d5f 6c69 6e65 203d 2061 6464 5f74 6f5f  m_line = add_to_
+00015490: 6765 6e65 7261 6c5f 6173 796e 635f 6772  general_async_gr
+000154a0: 6f75 7028 746f 705f 626f 7474 6f6d 5f6c  oup(top_bottom_l
+000154b0: 696e 655f 6368 6172 7473 290a 2020 2020  ine_charts).    
+000154c0: 6c69 6e65 5f77 6974 685f 636f 6e66 6964  line_with_confid
+000154d0: 656e 6365 5f61 7265 6120 3d20 6164 645f  ence_area = add_
+000154e0: 746f 5f67 656e 6572 616c 5f61 7379 6e63  to_general_async
+000154f0: 5f67 726f 7570 280a 2020 2020 2020 2020  _group(.        
+00015500: 6c69 6e65 5f77 6974 685f 636f 6e66 6964  line_with_confid
+00015510: 656e 6365 5f61 7265 615f 6368 6172 740a  ence_area_chart.
+00015520: 2020 2020 290a 2020 2020 7363 6174 7465      ).    scatte
+00015530: 725f 7769 7468 5f65 6666 6563 7420 3d20  r_with_effect = 
+00015540: 6164 645f 746f 5f67 656e 6572 616c 5f61  add_to_general_a
+00015550: 7379 6e63 5f67 726f 7570 2873 6361 7474  sync_group(scatt
+00015560: 6572 5f77 6974 685f 6566 6665 6374 5f63  er_with_effect_c
+00015570: 6861 7274 290a 2020 2020 7761 7465 7266  hart).    waterf
+00015580: 616c 6c20 3d20 6164 645f 746f 5f67 656e  all = add_to_gen
+00015590: 6572 616c 5f61 7379 6e63 5f67 726f 7570  eral_async_group
+000155a0: 2877 6174 6572 6661 6c6c 5f63 6861 7274  (waterfall_chart
+000155b0: 290a 2020 2020 6c69 6e65 5f61 6e64 5f62  ).    line_and_b
+000155c0: 6172 5f63 6861 7274 7320 3d20 6164 645f  ar_charts = add_
+000155d0: 746f 5f67 656e 6572 616c 5f61 7379 6e63  to_general_async
+000155e0: 5f67 726f 7570 286c 696e 655f 616e 645f  _group(line_and_
+000155f0: 6261 725f 6368 6172 7473 290a 2020 2020  bar_charts).    
+00015600: 7365 676d 656e 7465 645f 6c69 6e65 203d  segmented_line =
+00015610: 2061 6464 5f74 6f5f 6765 6e65 7261 6c5f   add_to_general_
+00015620: 6173 796e 635f 6772 6f75 7028 7365 676d  async_group(segm
+00015630: 656e 7465 645f 6c69 6e65 5f63 6861 7274  ented_line_chart
+00015640: 290a 2020 2020 6d61 726b 6564 5f6c 696e  ).    marked_lin
+00015650: 6520 3d20 6164 645f 746f 5f67 656e 6572  e = add_to_gener
+00015660: 616c 5f61 7379 6e63 5f67 726f 7570 286d  al_async_group(m
+00015670: 6172 6b65 645f 6c69 6e65 5f63 6861 7274  arked_line_chart
+00015680: 290a 2020 2020 7365 676d 656e 7465 645f  ).    segmented_
+00015690: 6172 6561 203d 2061 6464 5f74 6f5f 6765  area = add_to_ge
+000156a0: 6e65 7261 6c5f 6173 796e 635f 6772 6f75  neral_async_grou
+000156b0: 7028 7365 676d 656e 7465 645f 6172 6561  p(segmented_area
+000156c0: 5f63 6861 7274 290a 0a20 2020 2023 2042  _chart)..    # B
+000156d0: 656e 746f 626f 7820 6368 6172 7473 2064  entobox charts d
+000156e0: 6566 696e 6564 2069 6e20 7468 6520 6265  efined in the be
+000156f0: 6e74 6f62 6f78 5f63 6861 7274 732e 7079  ntobox_charts.py
+00015700: 2066 696c 650a 2020 2020 696e 666f 6772   file.    infogr
+00015710: 6170 6869 6373 5f74 6578 745f 6275 6262  aphics_text_bubb
+00015720: 6c65 203d 2061 6464 5f74 6f5f 6765 6e65  le = add_to_gene
+00015730: 7261 6c5f 6173 796e 635f 6772 6f75 7028  ral_async_group(
+00015740: 696e 666f 6772 6170 6869 6373 5f74 6578  infographics_tex
+00015750: 745f 6275 6262 6c65 290a 2020 2020 6368  t_bubble).    ch
+00015760: 6172 745f 616e 645f 6d6f 6461 6c5f 6275  art_and_modal_bu
+00015770: 7474 6f6e 203d 2061 6464 5f74 6f5f 6765  tton = add_to_ge
+00015780: 6e65 7261 6c5f 6173 796e 635f 6772 6f75  neral_async_grou
+00015790: 7028 6368 6172 745f 616e 645f 6d6f 6461  p(chart_and_moda
+000157a0: 6c5f 6275 7474 6f6e 290a 2020 2020 6368  l_button).    ch
+000157b0: 6172 745f 616e 645f 696e 6469 6361 746f  art_and_indicato
+000157c0: 7273 203d 2061 6464 5f74 6f5f 6765 6e65  rs = add_to_gene
+000157d0: 7261 6c5f 6173 796e 635f 6772 6f75 7028  ral_async_group(
+000157e0: 6368 6172 745f 616e 645f 696e 6469 6361  chart_and_indica
+000157f0: 746f 7273 290a 2020 2020 696e 6469 6361  tors).    indica
+00015800: 746f 7273 5f77 6974 685f 6865 6164 6572  tors_with_header
+00015810: 203d 2061 6464 5f74 6f5f 6765 6e65 7261   = add_to_genera
+00015820: 6c5f 6173 796e 635f 6772 6f75 7028 696e  l_async_group(in
+00015830: 6469 6361 746f 7273 5f77 6974 685f 6865  dicators_with_he
+00015840: 6164 6572 290a 2020 2020 6c69 6e65 5f77  ader).    line_w
+00015850: 6974 685f 7375 6d6d 6172 7920 3d20 6164  ith_summary = ad
+00015860: 645f 746f 5f67 656e 6572 616c 5f61 7379  d_to_general_asy
+00015870: 6e63 5f67 726f 7570 286c 696e 655f 7769  nc_group(line_wi
+00015880: 7468 5f73 756d 6d61 7279 290a            th_summary).
```

### Comparing `shimoku-browser-2.2.2/src/shimoku/plt/utils.py` & `shimoku-browser-2.2.3/src/shimoku/plt/utils.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku/utils.py` & `shimoku-browser-2.2.3/src/shimoku/utils.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/src/shimoku_browser.egg-info/PKG-INFO` & `shimoku-browser-2.2.3/src/shimoku_browser.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shimoku-browser
-Version: 2.2.2
+Version: 2.2.3
 Summary: Shimoku enables you to build Data Products in just hours and allows you to create Predictive Analytics Products with Artificial Intelligence capabilities.
 Home-page: https://github.com/shimoku-tech/shimoku-api-python
 Author: Shimoku
 Author-email: contact@shimoku.com
 License: MIT
 Project-URL: Documentation, https://docs.shimoku.com/
 Platform: any
```

### Comparing `shimoku-browser-2.2.2/src/shimoku_browser.egg-info/SOURCES.txt` & `shimoku-browser-2.2.3/src/shimoku_browser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/tests/Jupyter_notebook_test.ipynb` & `shimoku-browser-2.2.3/tests/Jupyter_notebook_test.ipynb`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/tests/mockable_tests/correct_action_scripts/correct_action.py` & `shimoku-browser-2.2.3/tests/mockable_tests/correct_action_scripts/correct_action.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/tests/mockable_tests/mock_classes.py` & `shimoku-browser-2.2.3/tests/mockable_tests/mock_classes.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/tests/mockable_tests/test_actions.py` & `shimoku-browser-2.2.3/tests/mockable_tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/tests/mockable_tests/test_activity_metadata_api.py` & `shimoku-browser-2.2.3/tests/mockable_tests/test_activity_metadata_api.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/tests/mockable_tests/test_app_metadata_api.py` & `shimoku-browser-2.2.3/tests/mockable_tests/test_app_metadata_api.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/tests/mockable_tests/test_business_metadata_api.py` & `shimoku-browser-2.2.3/tests/mockable_tests/test_business_metadata_api.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/tests/mockable_tests/test_code_generation.py` & `shimoku-browser-2.2.3/tests/mockable_tests/test_code_generation.py`

 * *Files 1% similar despite different names*

```diff
@@ -394,20 +394,20 @@
             return
         self.shimoku_client.set_workspace(self.workspace_id)
         clear_workspace(self.shimoku_client)
         self.shimoku_client.set_board("Pull-board")
         self.shimoku_client.set_menu_path("Pull-menu-path")
         create_bar_chart(self.shimoku_client)
         self.shimoku_client.pop_out_of_board()
+        self.shimoku_client.disable_caching()
         tpa_boards, tpa_menu_paths, tpa_components, tpa_data = get_workspace_contents(
             self.shimoku_client
         )
 
         local_shimoku_client = Client(verbosity="INFO")
-        local_shimoku_client.disable_caching()
         local_shimoku_client.set_workspace()
         clear_workspace(local_shimoku_client)
         subprocess.run(
             [
                 "shimoku",
                 "persist",
                 "pull",
@@ -421,14 +421,15 @@
                 self.shimoku_client.universe_id,
                 "--origin-workspace",
                 self.workspace_id,
                 "--origin-environment",
                 self.shimoku_client.environment,
             ]
         )
+        local_shimoku_client.disable_caching()
         (
             local_boards,
             local_menu_paths,
             local_components,
             local_data,
         ) = get_workspace_contents(local_shimoku_client)
 
@@ -438,10 +439,10 @@
         results = {
             "boards": (get_diff_percentage(tpa_boards, local_boards)),
             "menu_paths": (get_diff_percentage(tpa_menu_paths, local_menu_paths)),
             "components": (get_diff_percentage(tpa_components, local_components)),
             "data": (get_diff_percentage(tpa_data, local_data)),
         }
         print(json.dumps(results, indent=4))
-        print(local_menu_paths)
         print(tpa_menu_paths)
+        print(local_menu_paths)
         assert all([value == 0 for value in results.values()])
```

### Comparing `shimoku-browser-2.2.2/tests/mockable_tests/test_dashboard_metadata_api.py` & `shimoku-browser-2.2.3/tests/mockable_tests/test_dashboard_metadata_api.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api.py` & `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/annotation_chart.py` & `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/annotation_chart.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/bar_and_line_chart.py` & `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/bar_and_line_chart.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/bentobox.py` & `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/bentobox.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/chart_and_indicators.py` & `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/chart_and_indicators.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/data/annotation_chart.py` & `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/annotation_chart.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/data/bar_and_line.py` & `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/bar_and_line.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/data/dynamic_conditional_and_auto_send_input_form.py` & `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/dynamic_conditional_and_auto_send_input_form.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/data/flow_and_rainfall.py` & `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/flow_and_rainfall.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/data/free_echarts.py` & `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/free_echarts.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/data/free_echarts_raw.py` & `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/free_echarts_raw.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/data/heatmap.py` & `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/heatmap.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/data/indicator.py` & `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/indicator.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/data/input_form.py` & `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/input_form.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/data/noise.py` & `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/noise.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/data/scatter_test.csv` & `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/scatter_test.csv`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/data/scatter_with_effect.py` & `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/scatter_with_effect.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/data/stacked_area.py` & `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/stacked_area.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/data/suburst.py` & `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/suburst.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/data/table.py` & `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/table.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/data/table_with_labels.py` & `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/table_with_labels.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/data/tree.py` & `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/tree.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/data/waterfall.py` & `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/data/waterfall.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/doughnut.py` & `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/doughnut.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/dynamic_conditional_and_auto_send_input_form.py` & `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/dynamic_conditional_and_auto_send_input_form.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/gauge_indicator.py` & `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/gauge_indicator.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/heatmap.py` & `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/heatmap.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/horizontal_bar.py` & `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/horizontal_bar.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/indicator.py` & `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/indicator.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/infographics.py` & `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/infographics.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/line_with_confidence_area.py` & `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/line_with_confidence_area.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/modal.py` & `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/modal.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/radar.py` & `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/radar.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/rainfall_area.py` & `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/rainfall_area.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/rainfall_line.py` & `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/rainfall_line.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/rose.py` & `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/rose.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/scatter.py` & `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/scatter.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/segmented_area_chart.py` & `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/segmented_area_chart.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/segmented_line_chart.py` & `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/segmented_line_chart.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/shimoku_gauges.py` & `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/shimoku_gauges.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/table_with_lables.py` & `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/table_with_lables.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/tabs.py` & `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/tabs.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/tree.py` & `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/tree.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/variants.py` & `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/variants.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/waterfall.py` & `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/waterfall.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/tests/mockable_tests/test_plot_api_functions/zero_centered_bar.py` & `shimoku-browser-2.2.3/tests/mockable_tests/test_plot_api_functions/zero_centered_bar.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/tests/mockable_tests/test_report_metadata_api.py` & `shimoku-browser-2.2.3/tests/mockable_tests/test_report_metadata_api.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/tests/mockable_tests/test_roles.py` & `shimoku-browser-2.2.3/tests/mockable_tests/test_roles.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/tests/mockable_tests/utils.py` & `shimoku-browser-2.2.3/tests/mockable_tests/utils.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/tests/test_ai_api.py` & `shimoku-browser-2.2.3/tests/test_ai_api.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/tests/test_components_catalog.py` & `shimoku-browser-2.2.3/tests/test_components_catalog.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/tests/test_data_managing_api.py` & `shimoku-browser-2.2.3/tests/test_data_managing_api.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.2.2/tests/test_file_metadata_api.py` & `shimoku-browser-2.2.3/tests/test_file_metadata_api.py`

 * *Files identical despite different names*

