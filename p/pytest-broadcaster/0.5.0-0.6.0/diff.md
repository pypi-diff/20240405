# Comparing `tmp/pytest_broadcaster-0.5.0.tar.gz` & `tmp/pytest_broadcaster-0.6.0.tar.gz`

## Comparing `pytest_broadcaster-0.5.0.tar` & `pytest_broadcaster-0.6.0.tar`

### file list

```diff
@@ -1,159 +1,164 @@
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/.python-version
--rw-r--r--   0        0        0     3432 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/mkdocs.yml
--rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/requirements-dev.lock
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/requirements.lock
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/.github/workflows/docs.yml
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/docs/SUMMARY.md
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/docs/index.md
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/docs/.overrides/main.html
--rwxr-xr-x   0        0        0     8775 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/docs/assets/pytest-discover-logo-darkmode-transparent.svg
--rwxr-xr-x   0        0        0     8760 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/docs/assets/pytest-discover-logo-transparent.svg
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/docs/css/material.css
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/docs/css/mkdocstrings.css
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/docs/css/style.css
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/docs/recipes/SUMMARY.md
--rw-r--r--   0        0        0     3961 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/docs/recipes/code_generation.md
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/docs/reference/SUMMARY.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/docs/reference/index.md
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/docs/reference/events/SUMMARY.md
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/docs/reference/events/error_message.md
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/docs/reference/events/index.md
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/docs/reference/events/session_finish.md
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/docs/reference/events/session_start.md
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/docs/reference/events/warning_message.md
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/docs/reference/events/collect_report/index.md
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/docs/reference/events/collect_report/test_case.md
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/docs/reference/events/collect_report/test_directory.md
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/docs/reference/events/collect_report/test_module.md
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/docs/reference/events/collect_report/test_suite.md
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/docs/reference/events/steps/index.md
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/docs/reference/events/steps/test_case_call.md
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/docs/reference/events/steps/test_case_finished.md
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/docs/reference/events/steps/test_case_setup.md
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/docs/reference/events/steps/test_case_teardown.md
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/docs/reference/hooks/SUMMARY.md
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/docs/reference/hooks/pytest_broadcaster_add_destination.md
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/docs/reference/hooks/pytest_broadcaster_set_reporter.md
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/docs/reference/interfaces/SUMMARY.md
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/docs/reference/interfaces/destination.md
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/docs/reference/interfaces/reporter.md
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/docs/reference/result/SUMMARY.md
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/docs/reference/result/session_result/index.md
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/docs/reference/result/session_result/test_case_report.md
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/docs/schemas/collect_report.json
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/docs/schemas/error_message.json
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/docs/schemas/location.json
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/docs/schemas/outcome.json
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/docs/schemas/session_event.json
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/docs/schemas/session_finish.json
--rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/docs/schemas/session_result.json
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/docs/schemas/session_start.json
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/docs/schemas/test_case.json
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/docs/schemas/test_case_call.json
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/docs/schemas/test_case_error.json
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/docs/schemas/test_case_finished.json
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/docs/schemas/test_case_report.json
--rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/docs/schemas/test_case_setup.json
--rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/docs/schemas/test_case_teardown.json
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/docs/schemas/test_directory.json
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/docs/schemas/test_module.json
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/docs/schemas/test_suite.json
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/docs/schemas/traceback.json
--rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/docs/schemas/warning_message.json
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/docs/usage/SUMMARY.md
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/docs/usage/http_webhook.md
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/docs/usage/http_webhook_stream.md
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/docs/usage/json_file.md
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/docs/usage/json_lines.md
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/scripts/deploy-docs.sh
--rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/scripts/generate-documentation.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/src/fake_lib/__init__.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/src/fake_lib/with_errors.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/src/fake_lib/with_warnings.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/src/pytest_broadcaster/__about__.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/src/pytest_broadcaster/__about__.pyi
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/src/pytest_broadcaster/__init__.py
--rw-r--r--   0        0        0    11060 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/src/pytest_broadcaster/plugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/src/pytest_broadcaster/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/src/pytest_broadcaster/_internal/__init__.py
--rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/src/pytest_broadcaster/_internal/_fields.py
--rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/src/pytest_broadcaster/_internal/_json_files.py
--rw-r--r--   0        0        0    11894 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/src/pytest_broadcaster/_internal/_reporter.py
--rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/src/pytest_broadcaster/_internal/_utils.py
--rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/src/pytest_broadcaster/_internal/_webhook.py
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/src/pytest_broadcaster/hooks/__init__.py
--rw-r--r--   0        0        0     2989 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/src/pytest_broadcaster/interfaces/__init__.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/src/pytest_broadcaster/models/__init__.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/src/pytest_broadcaster/models/collect_report.py
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/src/pytest_broadcaster/models/error_message.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/src/pytest_broadcaster/models/location.py
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/src/pytest_broadcaster/models/outcome.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/src/pytest_broadcaster/models/session_event.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/src/pytest_broadcaster/models/session_finish.py
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/src/pytest_broadcaster/models/session_result.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/src/pytest_broadcaster/models/session_start.py
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/src/pytest_broadcaster/models/test_case.py
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/src/pytest_broadcaster/models/test_case_call.py
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/src/pytest_broadcaster/models/test_case_error.py
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/src/pytest_broadcaster/models/test_case_finished.py
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/src/pytest_broadcaster/models/test_case_report.py
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/src/pytest_broadcaster/models/test_case_setup.py
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/src/pytest_broadcaster/models/test_case_teardown.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/src/pytest_broadcaster/models/test_directory.py
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/src/pytest_broadcaster/models/test_module.py
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/src/pytest_broadcaster/models/test_suite.py
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/src/pytest_broadcaster/models/traceback.py
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/src/pytest_broadcaster/models/warning_message.py
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/src/schemas/collect_report.json
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/src/schemas/error_message.json
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/src/schemas/location.json
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/src/schemas/outcome.json
--rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/src/schemas/session_event.json
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/src/schemas/session_finish.json
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/src/schemas/session_result.json
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/src/schemas/session_start.json
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/src/schemas/test_case.json
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/src/schemas/test_case_call.json
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/src/schemas/test_case_error.json
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/src/schemas/test_case_finished.json
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/src/schemas/test_case_report.json
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/src/schemas/test_case_setup.json
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/src/schemas/test_case_teardown.json
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/src/schemas/test_directory.json
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/src/schemas/test_module.json
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/src/schemas/test_suite.json
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/src/schemas/traceback.json
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/src/schemas/warning_message.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/tests/__init__.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/tests/conftest.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/tests/test_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/tests/call/__init__.py
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/tests/call/_utils.py
--rw-r--r--   0        0        0     9796 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/tests/call/test_basic.py
--rw-r--r--   0        0        0    10046 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/tests/call/test_basic_failure.py
--rw-r--r--   0        0        0     8237 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/tests/call/test_basic_skip.py
--rw-r--r--   0        0        0    14594 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/tests/call/test_basic_xfail.py
--rw-r--r--   0        0        0     8947 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/tests/call/test_skip_within_test.py
--rw-r--r--   0        0        0     9029 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/tests/call/test_xfail_within_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/tests/collect/__init__.py
--rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/tests/collect/_utils.py
--rw-r--r--   0        0        0     5634 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/tests/collect/test_basic.py
--rw-r--r--   0        0        0     5685 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/tests/collect/test_basic_marker.py
--rw-r--r--   0        0        0     8747 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/tests/collect/test_basic_parametrization.py
--rw-r--r--   0        0        0     8821 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/tests/collect/test_basic_suite.py
--rw-r--r--   0        0        0     5135 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/tests/collect/test_errors.py
--rw-r--r--   0        0        0     4342 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/tests/collect/test_errors_third_party.py
--rw-r--r--   0        0        0     7058 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/tests/collect/test_multi_cases.py
--rw-r--r--   0        0        0    11235 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/tests/collect/test_multi_files.py
--rw-r--r--   0        0        0    23526 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/tests/collect/test_multi_suite.py
--rw-r--r--   0        0        0    11495 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/tests/collect/test_nested_directories.py
--rw-r--r--   0        0        0     7117 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/tests/collect/test_nested_markers.py
--rw-r--r--   0        0        0     7886 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/tests/collect/test_warnings.py
--rw-r--r--   0        0        0     7334 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/tests/collect/test_warnings_third_party.py
--rw-r--r--   0        0        0     6418 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/tests/destination/test_http_webhook.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/LICENSE
--rw-r--r--   0        0        0     8103 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/README.md
--rw-r--r--   0        0        0     5108 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     9130 2020-02-02 00:00:00.000000 pytest_broadcaster-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/.python-version
+-rw-r--r--   0        0        0     3432 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/mkdocs.yml
+-rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/requirements-dev.lock
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/requirements.lock
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/.github/workflows/cd.yml
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/SUMMARY.md
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/index.md
+-rw-r--r--   0        0        0     3020 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/why.md
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/.overrides/main.html
+-rwxr-xr-x   0        0        0     8775 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/assets/pytest-discover-logo-darkmode-transparent.svg
+-rwxr-xr-x   0        0        0     8760 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/assets/pytest-discover-logo-transparent.svg
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/css/material.css
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/css/mkdocstrings.css
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/css/style.css
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/recipes/SUMMARY.md
+-rw-r--r--   0        0        0     3961 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/recipes/code_generation.md
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/reference/SUMMARY.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/reference/index.md
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/reference/events/SUMMARY.md
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/reference/events/error_message.md
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/reference/events/index.md
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/reference/events/location.md
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/reference/events/session_finish.md
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/reference/events/session_start.md
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/reference/events/traceback.md
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/reference/events/warning_message.md
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/reference/events/collect_report/index.md
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/reference/events/collect_report/test_case.md
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/reference/events/collect_report/test_directory.md
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/reference/events/collect_report/test_module.md
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/reference/events/collect_report/test_suite.md
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/reference/events/steps/index.md
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/reference/events/steps/outcome.md
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/reference/events/steps/test_case_call.md
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/reference/events/steps/test_case_error.md
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/reference/events/steps/test_case_finished.md
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/reference/events/steps/test_case_setup.md
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/reference/events/steps/test_case_teardown.md
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/reference/hooks/SUMMARY.md
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/reference/hooks/pytest_broadcaster_add_destination.md
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/reference/hooks/pytest_broadcaster_set_reporter.md
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/reference/interfaces/SUMMARY.md
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/reference/interfaces/destination.md
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/reference/interfaces/reporter.md
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/reference/result/SUMMARY.md
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/reference/result/session_result/index.md
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/reference/result/session_result/test_case_report.md
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/schemas/collect_report.json
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/schemas/error_message.json
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/schemas/location.json
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/schemas/outcome.json
+-rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/schemas/session_event.json
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/schemas/session_finish.json
+-rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/schemas/session_result.json
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/schemas/session_start.json
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/schemas/test_case.json
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/schemas/test_case_call.json
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/schemas/test_case_error.json
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/schemas/test_case_finished.json
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/schemas/test_case_report.json
+-rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/schemas/test_case_setup.json
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/schemas/test_case_teardown.json
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/schemas/test_directory.json
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/schemas/test_module.json
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/schemas/test_suite.json
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/schemas/traceback.json
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/schemas/warning_message.json
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/usage/SUMMARY.md
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/usage/http_webhook.md
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/usage/http_webhook_stream.md
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/usage/json_file.md
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/usage/json_lines.md
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/scripts/deploy-docs.sh
+-rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/scripts/generate-documentation.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/fake_lib/__init__.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/fake_lib/with_errors.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/fake_lib/with_warnings.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/__about__.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/__about__.pyi
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/__init__.py
+-rw-r--r--   0        0        0    11060 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/_internal/__init__.py
+-rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/_internal/_fields.py
+-rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/_internal/_json_files.py
+-rw-r--r--   0        0        0    11894 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/_internal/_reporter.py
+-rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/_internal/_utils.py
+-rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/_internal/_webhook.py
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/hooks/__init__.py
+-rw-r--r--   0        0        0     2989 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/interfaces/__init__.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/__init__.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/collect_report.py
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/error_message.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/location.py
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/outcome.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/session_event.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/session_finish.py
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/session_result.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/session_start.py
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/test_case.py
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/test_case_call.py
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/test_case_error.py
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/test_case_finished.py
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/test_case_report.py
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/test_case_setup.py
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/test_case_teardown.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/test_directory.py
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/test_module.py
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/test_suite.py
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/traceback.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/warning_message.py
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/schemas/collect_report.json
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/schemas/error_message.json
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/schemas/location.json
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/schemas/outcome.json
+-rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/schemas/session_event.json
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/schemas/session_finish.json
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/schemas/session_result.json
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/schemas/session_start.json
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/schemas/test_case.json
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/schemas/test_case_call.json
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/schemas/test_case_error.json
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/schemas/test_case_finished.json
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/schemas/test_case_report.json
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/schemas/test_case_setup.json
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/schemas/test_case_teardown.json
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/schemas/test_directory.json
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/schemas/test_module.json
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/schemas/test_suite.json
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/schemas/traceback.json
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/schemas/warning_message.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/tests/__init__.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/tests/conftest.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/tests/test_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/tests/call/__init__.py
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/tests/call/_utils.py
+-rw-r--r--   0        0        0     9796 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/tests/call/test_basic.py
+-rw-r--r--   0        0        0    10046 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/tests/call/test_basic_failure.py
+-rw-r--r--   0        0        0     8237 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/tests/call/test_basic_skip.py
+-rw-r--r--   0        0        0    14594 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/tests/call/test_basic_xfail.py
+-rw-r--r--   0        0        0     8947 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/tests/call/test_skip_within_test.py
+-rw-r--r--   0        0        0     9029 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/tests/call/test_xfail_within_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/tests/collect/__init__.py
+-rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/tests/collect/_utils.py
+-rw-r--r--   0        0        0     5634 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/tests/collect/test_basic.py
+-rw-r--r--   0        0        0     5685 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/tests/collect/test_basic_marker.py
+-rw-r--r--   0        0        0     8747 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/tests/collect/test_basic_parametrization.py
+-rw-r--r--   0        0        0     8821 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/tests/collect/test_basic_suite.py
+-rw-r--r--   0        0        0     5135 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/tests/collect/test_errors.py
+-rw-r--r--   0        0        0     4342 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/tests/collect/test_errors_third_party.py
+-rw-r--r--   0        0        0     7058 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/tests/collect/test_multi_cases.py
+-rw-r--r--   0        0        0    11235 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/tests/collect/test_multi_files.py
+-rw-r--r--   0        0        0    23526 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/tests/collect/test_multi_suite.py
+-rw-r--r--   0        0        0    11495 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/tests/collect/test_nested_directories.py
+-rw-r--r--   0        0        0     7117 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/tests/collect/test_nested_markers.py
+-rw-r--r--   0        0        0     7886 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/tests/collect/test_warnings.py
+-rw-r--r--   0        0        0     7334 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/tests/collect/test_warnings_third_party.py
+-rw-r--r--   0        0        0     6418 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/tests/destination/test_http_webhook.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/LICENSE
+-rw-r--r--   0        0        0     8103 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/README.md
+-rw-r--r--   0        0        0     5108 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     9130 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/PKG-INFO
```

### Comparing `pytest_broadcaster-0.5.0/mkdocs.yml` & `pytest_broadcaster-0.6.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/requirements-dev.lock` & `pytest_broadcaster-0.6.0/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/.github/workflows/ci.yml` & `pytest_broadcaster-0.6.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/.github/workflows/docs.yml` & `pytest_broadcaster-0.6.0/.github/workflows/cd.yml`

 * *Files 11% similar despite different names*

```diff
@@ -34,7 +34,11 @@
 
       - name: Build the docs
         run: rye run ci-docs
         env:
           VERSION: "${{  github.ref_name }}"
           ALIAS: latest
 
+      - name: Build and publish the packag on pypi
+        run: |
+          rye build --clean
+          rye publish --yes --token ${{ secrets.PYPI_TOKEN }}
```

### Comparing `pytest_broadcaster-0.5.0/docs/assets/pytest-discover-logo-darkmode-transparent.svg` & `pytest_broadcaster-0.6.0/docs/assets/pytest-discover-logo-darkmode-transparent.svg`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/docs/assets/pytest-discover-logo-transparent.svg` & `pytest_broadcaster-0.6.0/docs/assets/pytest-discover-logo-transparent.svg`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/docs/css/mkdocstrings.css` & `pytest_broadcaster-0.6.0/docs/css/mkdocstrings.css`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/docs/css/style.css` & `pytest_broadcaster-0.6.0/docs/css/style.css`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/docs/recipes/code_generation.md` & `pytest_broadcaster-0.6.0/docs/recipes/code_generation.md`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/docs/reference/events/SUMMARY.md` & `pytest_broadcaster-0.6.0/docs/reference/events/SUMMARY.md`

 * *Files 12% similar despite different names*

```diff
@@ -6,10 +6,16 @@
     * [Test Suite](./collect_report/test_suite.md)
     * [Test Case](./collect_report/test_case.md)
 * [Test Case Steps](./steps/index.md)
     * [Test Case Setup](./steps/test_case_setup.md)
     * [Test Case Call](./steps/test_case_call.md)
     * [Test Case Teardown](./steps/test_case_teardown.md)
     * [Test Case Finished](./steps/test_case_finished.md)
+    * Test Case Fields
+        * [Test Case Error](./steps/test_case_error.md)
+        * [Outcome](./steps/outcome.md)
 * [Warning Message](./warning_message.md)
 * [Error Message](./error_message.md)
-* [Session Finish](./session_finish.md)
+* Warning & Errors Fields
+    * [Location](./location.md)
+    * [Traceback](./traceback.md)
+* [Session Finish](./session_finish.md)
```

### Comparing `pytest_broadcaster-0.5.0/docs/schemas/collect_report.json` & `pytest_broadcaster-0.6.0/docs/schemas/collect_report.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/docs/schemas/error_message.json` & `pytest_broadcaster-0.6.0/docs/schemas/error_message.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/docs/schemas/session_event.json` & `pytest_broadcaster-0.6.0/docs/schemas/session_event.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/docs/schemas/session_finish.json` & `pytest_broadcaster-0.6.0/docs/schemas/session_finish.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/docs/schemas/session_result.json` & `pytest_broadcaster-0.6.0/docs/schemas/session_result.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/docs/schemas/session_start.json` & `pytest_broadcaster-0.6.0/docs/schemas/session_start.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/docs/schemas/test_case.json` & `pytest_broadcaster-0.6.0/docs/schemas/test_case.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/docs/schemas/test_case_call.json` & `pytest_broadcaster-0.6.0/docs/schemas/test_case_call.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/docs/schemas/test_case_error.json` & `pytest_broadcaster-0.6.0/docs/schemas/test_case_error.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/docs/schemas/test_case_finished.json` & `pytest_broadcaster-0.6.0/docs/schemas/test_case_finished.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/docs/schemas/test_case_report.json` & `pytest_broadcaster-0.6.0/docs/schemas/test_case_report.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/docs/schemas/test_case_setup.json` & `pytest_broadcaster-0.6.0/docs/schemas/test_case_setup.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/docs/schemas/test_case_teardown.json` & `pytest_broadcaster-0.6.0/docs/schemas/test_case_teardown.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/docs/schemas/test_directory.json` & `pytest_broadcaster-0.6.0/docs/schemas/test_directory.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/docs/schemas/test_module.json` & `pytest_broadcaster-0.6.0/docs/schemas/test_module.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/docs/schemas/test_suite.json` & `pytest_broadcaster-0.6.0/docs/schemas/test_suite.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/docs/schemas/traceback.json` & `pytest_broadcaster-0.6.0/docs/schemas/traceback.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/docs/schemas/warning_message.json` & `pytest_broadcaster-0.6.0/docs/schemas/warning_message.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/docs/usage/http_webhook.md` & `pytest_broadcaster-0.6.0/docs/usage/http_webhook.md`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/docs/usage/http_webhook_stream.md` & `pytest_broadcaster-0.6.0/docs/usage/http_webhook_stream.md`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/scripts/generate-documentation.py` & `pytest_broadcaster-0.6.0/scripts/generate-documentation.py`

 * *Files 24% similar despite different names*

```diff
@@ -57,18 +57,56 @@
         output_directory = output_directory[:-1]
     # Build full repository URL
     target = output_directory
     if target.startswith("docs"):
         target = target[5:]
     ref_prefix = urljoin(ref_prefix, target)
     # Generate all schemas
+    schemas: dict[str, dict[str, Any]] = {}
     for source in SOURCES.glob("*.json"):
+        module = source.name.replace(".json", "")
+        schema_content = json.loads(source.read_text())
+        title = "".join(
+            [
+                part.capitalize()
+                for part in schema_content.get("title", module).split(" ")
+            ]
+        )
+        schema_import = f"pytest_broadcaster.models.{module}.{title}"
+        schema_url = f"{ref_prefix}/{source.name}"
+        schema_description = schema_content.get("description", "")
+        name = f"[{title}][{schema_import}]"
+        schemas[name] = {
+            "description": schema_description,
+            "url": schema_url,
+        }
         create_schema(
             source=source, output_directory=destination, ref_prefix=ref_prefix
         )
+    generate_schemas_index(schemas)
+
+
+def generate_schemas_index(schemas: dict[str, dict[str, Any]]) -> None:
+    """Generate the schemas index page."""
+    with mkdocs_gen_files.open("schemas/index.md", "w") as index:
+        content = ""
+        content += "# JSON Schemas"
+        content += "\n\n"
+        content += "The table below contains the JSON schemas used in the project:"
+        content += "\n\n"
+        content += "| Schema | Description | URL |"
+        content += "\n"
+        content += "| ------ | ----------- | --- |"
+        content += "\n"
+        for schema_name, schema in schemas.items():
+            schema_description = schema["description"]
+            schema_url = schema["url"]
+            content += f"| {schema_name} | {schema_description} | [{schema_url}]({schema_url}) |"
+            content += "\n"
+        index.write(content)
 
 
 def generate_license_file() -> None:
     """Generate the LICENSE.md file."""
 
     with mkdocs_gen_files.open("LICENSE.md", "w") as license_file:
         license = Path("LICENSE")
```

### Comparing `pytest_broadcaster-0.5.0/src/pytest_broadcaster/plugin.py` & `pytest_broadcaster-0.6.0/src/pytest_broadcaster/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/src/pytest_broadcaster/_internal/_fields.py` & `pytest_broadcaster-0.6.0/src/pytest_broadcaster/_internal/_fields.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/src/pytest_broadcaster/_internal/_json_files.py` & `pytest_broadcaster-0.6.0/src/pytest_broadcaster/_internal/_json_files.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/src/pytest_broadcaster/_internal/_reporter.py` & `pytest_broadcaster-0.6.0/src/pytest_broadcaster/_internal/_reporter.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/src/pytest_broadcaster/_internal/_utils.py` & `pytest_broadcaster-0.6.0/src/pytest_broadcaster/_internal/_utils.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/src/pytest_broadcaster/_internal/_webhook.py` & `pytest_broadcaster-0.6.0/src/pytest_broadcaster/_internal/_webhook.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/src/pytest_broadcaster/hooks/__init__.py` & `pytest_broadcaster-0.6.0/src/pytest_broadcaster/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/src/pytest_broadcaster/interfaces/__init__.py` & `pytest_broadcaster-0.6.0/src/pytest_broadcaster/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/src/pytest_broadcaster/models/collect_report.py` & `pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/collect_report.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/src/pytest_broadcaster/models/error_message.py` & `pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/error_message.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/src/pytest_broadcaster/models/session_event.py` & `pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/session_event.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/src/pytest_broadcaster/models/session_result.py` & `pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/session_result.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/src/pytest_broadcaster/models/session_start.py` & `pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/session_start.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/src/pytest_broadcaster/models/test_case.py` & `pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/test_case.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/src/pytest_broadcaster/models/test_case_call.py` & `pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/test_case_call.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/src/pytest_broadcaster/models/test_case_finished.py` & `pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/test_case_finished.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/src/pytest_broadcaster/models/test_case_report.py` & `pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/test_case_report.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/src/pytest_broadcaster/models/test_case_setup.py` & `pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/test_case_setup.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/src/pytest_broadcaster/models/test_case_teardown.py` & `pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/test_case_teardown.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/src/pytest_broadcaster/models/test_module.py` & `pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/test_module.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/src/pytest_broadcaster/models/test_suite.py` & `pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/test_suite.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/src/pytest_broadcaster/models/traceback.py` & `pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/traceback.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/src/pytest_broadcaster/models/warning_message.py` & `pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/warning_message.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/src/schemas/collect_report.json` & `pytest_broadcaster-0.6.0/src/schemas/collect_report.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/src/schemas/error_message.json` & `pytest_broadcaster-0.6.0/src/schemas/error_message.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/src/schemas/session_event.json` & `pytest_broadcaster-0.6.0/src/schemas/session_event.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/src/schemas/session_finish.json` & `pytest_broadcaster-0.6.0/src/schemas/session_finish.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/src/schemas/session_result.json` & `pytest_broadcaster-0.6.0/src/schemas/session_result.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/src/schemas/session_start.json` & `pytest_broadcaster-0.6.0/src/schemas/session_start.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/src/schemas/test_case.json` & `pytest_broadcaster-0.6.0/src/schemas/test_case.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/src/schemas/test_case_call.json` & `pytest_broadcaster-0.6.0/src/schemas/test_case_call.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/src/schemas/test_case_finished.json` & `pytest_broadcaster-0.6.0/src/schemas/test_case_finished.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/src/schemas/test_case_report.json` & `pytest_broadcaster-0.6.0/src/schemas/test_case_report.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/src/schemas/test_case_setup.json` & `pytest_broadcaster-0.6.0/src/schemas/test_case_setup.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/src/schemas/test_case_teardown.json` & `pytest_broadcaster-0.6.0/src/schemas/test_case_teardown.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/src/schemas/test_directory.json` & `pytest_broadcaster-0.6.0/src/schemas/test_directory.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/src/schemas/test_module.json` & `pytest_broadcaster-0.6.0/src/schemas/test_module.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/src/schemas/test_suite.json` & `pytest_broadcaster-0.6.0/src/schemas/test_suite.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/src/schemas/traceback.json` & `pytest_broadcaster-0.6.0/src/schemas/traceback.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/src/schemas/warning_message.json` & `pytest_broadcaster-0.6.0/src/schemas/warning_message.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/tests/call/_utils.py` & `pytest_broadcaster-0.6.0/tests/call/_utils.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/tests/call/test_basic.py` & `pytest_broadcaster-0.6.0/tests/call/test_basic.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/tests/call/test_basic_failure.py` & `pytest_broadcaster-0.6.0/tests/call/test_basic_failure.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/tests/call/test_basic_skip.py` & `pytest_broadcaster-0.6.0/tests/call/test_basic_skip.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/tests/call/test_basic_xfail.py` & `pytest_broadcaster-0.6.0/tests/call/test_basic_xfail.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/tests/call/test_skip_within_test.py` & `pytest_broadcaster-0.6.0/tests/call/test_skip_within_test.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/tests/call/test_xfail_within_test.py` & `pytest_broadcaster-0.6.0/tests/call/test_xfail_within_test.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/tests/collect/_utils.py` & `pytest_broadcaster-0.6.0/tests/collect/_utils.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/tests/collect/test_basic.py` & `pytest_broadcaster-0.6.0/tests/collect/test_basic.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/tests/collect/test_basic_marker.py` & `pytest_broadcaster-0.6.0/tests/collect/test_basic_marker.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/tests/collect/test_basic_parametrization.py` & `pytest_broadcaster-0.6.0/tests/collect/test_basic_parametrization.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/tests/collect/test_basic_suite.py` & `pytest_broadcaster-0.6.0/tests/collect/test_basic_suite.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/tests/collect/test_errors.py` & `pytest_broadcaster-0.6.0/tests/collect/test_errors.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/tests/collect/test_errors_third_party.py` & `pytest_broadcaster-0.6.0/tests/collect/test_errors_third_party.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/tests/collect/test_multi_cases.py` & `pytest_broadcaster-0.6.0/tests/collect/test_multi_cases.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/tests/collect/test_multi_files.py` & `pytest_broadcaster-0.6.0/tests/collect/test_multi_files.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/tests/collect/test_multi_suite.py` & `pytest_broadcaster-0.6.0/tests/collect/test_multi_suite.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/tests/collect/test_nested_directories.py` & `pytest_broadcaster-0.6.0/tests/collect/test_nested_directories.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/tests/collect/test_nested_markers.py` & `pytest_broadcaster-0.6.0/tests/collect/test_nested_markers.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/tests/collect/test_warnings.py` & `pytest_broadcaster-0.6.0/tests/collect/test_warnings.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/tests/collect/test_warnings_third_party.py` & `pytest_broadcaster-0.6.0/tests/collect/test_warnings_third_party.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/tests/destination/test_http_webhook.py` & `pytest_broadcaster-0.6.0/tests/destination/test_http_webhook.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/LICENSE` & `pytest_broadcaster-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/README.md` & `pytest_broadcaster-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/pyproject.toml` & `pytest_broadcaster-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.5.0/PKG-INFO` & `pytest_broadcaster-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pytest-broadcaster
-Version: 0.5.0
+Version: 0.6.0
 Summary: Pytest plugin to broadcast pytest output to various destinations
 Project-URL: Source, https://github.com/charbonnierg/pytest-broadcaster
 Project-URL: Tracker, https://github.com/charbonnierg/pytest-broadcaster/issues
 Author-email: Guillaume Charbonnier <gu.charbon@gmail.com>
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Pytest
```

