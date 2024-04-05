# Comparing `tmp/reqstool-0.4.1.tar.gz` & `tmp/reqstool-0.4.2.tar.gz`

## Comparing `reqstool-0.4.1.tar` & `reqstool-0.4.2.tar`

### file list

```diff
@@ -1,197 +1,204 @@
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 reqstool-0.4.1/.github/dependabot.yml
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 reqstool-0.4.1/.github/workflows/build.yml
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 reqstool-0.4.1/.github/workflows/check_release.yml
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 reqstool-0.4.1/.github/workflows/lint.yml
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 reqstool-0.4.1/.github/workflows/publish_gh_pages.yml
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 reqstool-0.4.1/.github/workflows/publish_pypi_prod.yml
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 reqstool-0.4.1/.github/workflows/publish_pypi_test.yml
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 reqstool-0.4.1/docs/antora-playbook.yml
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 reqstool-0.4.1/docs/antora.yml
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 reqstool-0.4.1/docs/examples/requirements/manual_verification_results.yml
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 reqstool-0.4.1/docs/examples/requirements/requirements_external.yml
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 reqstool-0.4.1/docs/examples/requirements/requirements_microservice.yml
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 reqstool-0.4.1/docs/examples/requirements/requirements_system.yml
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 reqstool-0.4.1/docs/examples/requirements/software_verification_cases.yml
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 reqstool-0.4.1/docs/modules/ROOT/nav.adoc
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 reqstool-0.4.1/docs/modules/ROOT/pages/background.adoc
--rw-r--r--   0        0        0    10808 2020-02-02 00:00:00.000000 reqstool-0.4.1/docs/modules/ROOT/pages/data.adoc
--rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 reqstool-0.4.1/docs/modules/ROOT/pages/file_and_directory_set.adoc
--rw-r--r--   0        0        0     6736 2020-02-02 00:00:00.000000 reqstool-0.4.1/docs/modules/ROOT/pages/how_it_works.adoc
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 reqstool-0.4.1/docs/modules/ROOT/pages/index.adoc
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 reqstool-0.4.1/docs/modules/ROOT/pages/installation.adoc
--rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 reqstool-0.4.1/docs/modules/ROOT/pages/overview.adoc
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 reqstool-0.4.1/docs/modules/ROOT/pages/quickstart.adoc
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 reqstool-0.4.1/docs/modules/ROOT/pages/terminology.adoc
--rw-r--r--   0        0        0     3334 2020-02-02 00:00:00.000000 reqstool-0.4.1/docs/modules/ROOT/pages/usage.adoc
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 reqstool-0.4.1/docs/modules/ROOT/pages/yml/annotations.adoc
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 reqstool-0.4.1/docs/modules/ROOT/pages/yml/manual_verification_results.adoc
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 reqstool-0.4.1/docs/modules/ROOT/pages/yml/reqstool_config.adoc
--rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 reqstool-0.4.1/docs/modules/ROOT/pages/yml/requirements.adoc
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 reqstool-0.4.1/docs/modules/ROOT/pages/yml/requirements_annotations.adoc
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 reqstool-0.4.1/docs/modules/ROOT/pages/yml/requirements_external.adoc
--rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 reqstool-0.4.1/docs/modules/ROOT/pages/yml/requirements_microservice.adoc
--rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 reqstool-0.4.1/docs/modules/ROOT/pages/yml/requirements_system.adoc
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 reqstool-0.4.1/docs/modules/ROOT/pages/yml/software_verification_cases.adoc
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 reqstool-0.4.1/docs/modules/ROOT/pages/yml/svcs_annotations.adoc
--rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 reqstool-0.4.1/docs/modules/ROOT/partials/C4_Component.puml
--rw-r--r--   0        0        0    14863 2020-02-02 00:00:00.000000 reqstool-0.4.1/docs/modules/ROOT/partials/C4_Sequence.puml
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 reqstool-0.4.1/docs/modules/examples/partials/requirements/manual_verification_results.yml
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 reqstool-0.4.1/docs/modules/examples/partials/requirements/reqstool_config.yml
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 reqstool-0.4.1/docs/modules/examples/partials/requirements/requirements_external.yml
--rw-r--r--   0        0        0     2091 2020-02-02 00:00:00.000000 reqstool-0.4.1/docs/modules/examples/partials/requirements/requirements_microservice.yml
--rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 reqstool-0.4.1/docs/modules/examples/partials/requirements/requirements_system.yml
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 reqstool-0.4.1/docs/modules/examples/partials/requirements/software_verification_cases.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.1/src/reqstool/__init__.py
--rwxr-xr-x   0        0        0    10490 2020-02-02 00:00:00.000000 reqstool-0.4.1/src/reqstool/command.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 reqstool-0.4.1/src/reqstool/commands/exit_codes.py
--rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 reqstool-0.4.1/src/reqstool/commands/generate_json/generate_json.py
--rw-r--r--   0        0        0    10425 2020-02-02 00:00:00.000000 reqstool-0.4.1/src/reqstool/commands/report/report.py
--rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 reqstool-0.4.1/src/reqstool/commands/report/criterias/group_by.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 reqstool-0.4.1/src/reqstool/commands/report/criterias/sort_by.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 reqstool-0.4.1/src/reqstool/commands/report/templates/annotation_impls.j2
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 reqstool-0.4.1/src/reqstool/commands/report/templates/annotation_tests.j2
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 reqstool-0.4.1/src/reqstool/commands/report/templates/mvrs.j2
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 reqstool-0.4.1/src/reqstool/commands/report/templates/report.j2
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 reqstool-0.4.1/src/reqstool/commands/report/templates/req_references.j2
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 reqstool-0.4.1/src/reqstool/commands/report/templates/requirements.j2
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 reqstool-0.4.1/src/reqstool/commands/report/templates/svcs.j2
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 reqstool-0.4.1/src/reqstool/commands/report/templates/total_statistics.j2
--rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 reqstool-0.4.1/src/reqstool/commands/status/statistics_container.py
--rw-r--r--   0        0        0    13186 2020-02-02 00:00:00.000000 reqstool-0.4.1/src/reqstool/commands/status/statistics_generator.py
--rw-r--r--   0        0        0     9121 2020-02-02 00:00:00.000000 reqstool-0.4.1/src/reqstool/commands/status/status.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 reqstool-0.4.1/src/reqstool/common/jinja2.py
--rw-r--r--   0        0        0     9339 2020-02-02 00:00:00.000000 reqstool-0.4.1/src/reqstool/common/utils.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 reqstool-0.4.1/src/reqstool/common/validator_error_holder.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 reqstool-0.4.1/src/reqstool/common/dataclasses/urn_id.py
--rw-r--r--   0        0        0    11778 2020-02-02 00:00:00.000000 reqstool-0.4.1/src/reqstool/common/validators/semantic_validator.py
--rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 reqstool-0.4.1/src/reqstool/common/validators/syntax_validator.py
--rwxr-xr-x   0        0        0     2575 2020-02-02 00:00:00.000000 reqstool-0.4.1/src/reqstool/expression_languages/generic_el.py
--rwxr-xr-x   0        0        0      235 2020-02-02 00:00:00.000000 reqstool-0.4.1/src/reqstool/expression_languages/requirements_el.py
--rwxr-xr-x   0        0        0      203 2020-02-02 00:00:00.000000 reqstool-0.4.1/src/reqstool/expression_languages/svcs_el.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 reqstool-0.4.1/src/reqstool/filters/id_filters.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 reqstool-0.4.1/src/reqstool/filters/requirements_filters.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 reqstool-0.4.1/src/reqstool/filters/svcs_filters.py
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 reqstool-0.4.1/src/reqstool/location_resolver/location_resolver.py
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 reqstool-0.4.1/src/reqstool/locations/git_location.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 reqstool-0.4.1/src/reqstool/locations/local_location.py
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 reqstool-0.4.1/src/reqstool/locations/location.py
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 reqstool-0.4.1/src/reqstool/locations/maven_location.py
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 reqstool-0.4.1/src/reqstool/model_generators/annotations_model_generator.py
--rw-r--r--   0        0        0    29004 2020-02-02 00:00:00.000000 reqstool-0.4.1/src/reqstool/model_generators/combined_indexed_dataset_generator.py
--rw-r--r--   0        0        0    10917 2020-02-02 00:00:00.000000 reqstool-0.4.1/src/reqstool/model_generators/combined_raw_datasets_generator.py
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 reqstool-0.4.1/src/reqstool/model_generators/mvrs_model_generator.py
--rw-r--r--   0        0        0    12512 2020-02-02 00:00:00.000000 reqstool-0.4.1/src/reqstool/model_generators/requirements_model_generator.py
--rw-r--r--   0        0        0     4515 2020-02-02 00:00:00.000000 reqstool-0.4.1/src/reqstool/model_generators/svcs_model_generator.py
--rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 reqstool-0.4.1/src/reqstool/model_generators/testdata_model_generator.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 reqstool-0.4.1/src/reqstool/models/annotations.py
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 reqstool-0.4.1/src/reqstool/models/combined_indexed_dataset.py
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 reqstool-0.4.1/src/reqstool/models/implementations.py
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 reqstool-0.4.1/src/reqstool/models/imports.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 reqstool-0.4.1/src/reqstool/models/mvrs.py
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 reqstool-0.4.1/src/reqstool/models/raw_datasets.py
--rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 reqstool-0.4.1/src/reqstool/models/requirements.py
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 reqstool-0.4.1/src/reqstool/models/svcs.py
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 reqstool-0.4.1/src/reqstool/models/test_data.py
--rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 reqstool-0.4.1/src/reqstool/reqstool_config/reqstool_config.py
--rw-r--r--   0        0        0     4877 2020-02-02 00:00:00.000000 reqstool-0.4.1/src/reqstool/requirements_indata/requirements_indata.py
--rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 reqstool-0.4.1/src/reqstool/requirements_indata/requirements_indata_paths.py
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 reqstool-0.4.1/src/reqstool/requirements_indata/java/java_maven_requirements_indata_paths.py
--rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 reqstool-0.4.1/src/reqstool/resources/schemas/v1/annotations.schema.json
--rw-r--r--   0        0        0    11023 2020-02-02 00:00:00.000000 reqstool-0.4.1/src/reqstool/resources/schemas/v1/common.schema.json
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 reqstool-0.4.1/src/reqstool/resources/schemas/v1/manual_verification_results.schema.json
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 reqstool-0.4.1/src/reqstool/resources/schemas/v1/reqstool_config.schema.json
--rw-r--r--   0        0        0    10812 2020-02-02 00:00:00.000000 reqstool-0.4.1/src/reqstool/resources/schemas/v1/requirements.schema.json
--rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 reqstool-0.4.1/src/reqstool/resources/schemas/v1/software_verification_cases.schema.json
--rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/integration/reqstool/model_generators/test_included_models_generator.py
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/resources/test_data/data/local/test_basic/baseline/ms-101/annotations.yml
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/resources/test_data/data/local/test_basic/baseline/ms-101/manual_verification_results.yml
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/resources/test_data/data/local/test_basic/baseline/ms-101/requirements.yml
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/resources/test_data/data/local/test_basic/baseline/ms-101/software_verification_cases.yml
--rw-r--r--   0        0        0     6367 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/resources/test_data/data/local/test_basic/baseline/ms-101/test_results/failsafe/TEST-com.example.RequirementsExampleTestsIT.xml
--rw-r--r--   0        0        0     5744 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/resources/test_data/data/local/test_basic/baseline/ms-101/test_results/surefire/TEST-com.example.RequirementsExampleTests.xml
--rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/resources/test_data/data/local/test_basic/layout_maven/ms-101/pom.xml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/resources/test_data/data/local/test_basic/layout_maven/ms-101/src/resources/docs/requirements/manual_verification_results.yml -> ../../../../../../baseline/ms-101/manual_verification_results.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/resources/test_data/data/local/test_basic/layout_maven/ms-101/src/resources/docs/requirements/requirements.yml -> ../../../../../../baseline/ms-101/requirements.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/resources/test_data/data/local/test_basic/layout_maven/ms-101/src/resources/docs/requirements/software_verification_cases.yml -> ../../../../../../baseline/ms-101/software_verification_cases.yml
--rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/resources/test_data/data/local/test_basic/with_requirements_config/README.md
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/resources/test_data/data/local/test_basic/with_requirements_config/ms-101/manual_verification_results.yml -> ../../baseline/ms-101/manual_verification_results.yml
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/resources/test_data/data/local/test_basic/with_requirements_config/ms-101/reqstool_config.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/resources/test_data/data/local/test_basic/with_requirements_config/ms-101/requirements.yml -> ../../baseline/ms-101/requirements.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/resources/test_data/data/local/test_basic/with_requirements_config/ms-101/software_verification_cases.yml -> ../../baseline/ms-101/software_verification_cases.yml
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/resources/test_data/data/local/test_errors/ms-101/annotations.yml
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/resources/test_data/data/local/test_errors/ms-101/errors.adoc
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/resources/test_data/data/local/test_errors/ms-101/manual_verification_results.yml
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/resources/test_data/data/local/test_errors/ms-101/requirements.yml
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/resources/test_data/data/local/test_errors/ms-101/software_verification_cases.yml
--rw-r--r--   0        0        0     6367 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/resources/test_data/data/local/test_errors/ms-101/test_results/failsafe/TEST-com.example.RequirementsExampleTestsIT.xml
--rw-r--r--   0        0        0     5744 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/resources/test_data/data/local/test_errors/ms-101/test_results/surefire/TEST-com.example.RequirementsExampleTests.xml
--rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/resources/test_data/data/local/test_standard/baseline/visualization.adoc
--rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/resources/test_data/data/local/test_standard/baseline/ms-001/annotations.yml
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/resources/test_data/data/local/test_standard/baseline/ms-001/manual_verification_results.yml
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/resources/test_data/data/local/test_standard/baseline/ms-001/requirements.yml
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/resources/test_data/data/local/test_standard/baseline/ms-001/software_verification_cases.yml
--rw-r--r--   0        0        0     7126 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/resources/test_data/data/local/test_standard/baseline/ms-001/test_results/failsafe/TEST-com.reqstool.example.demo.DemoApplicationTestsIT.xml
--rw-r--r--   0        0        0     8258 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/resources/test_data/data/local/test_standard/baseline/ms-001/test_results/surefire/TEST-com.reqstool.example.demo.SVCsTest.xml
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/resources/test_data/data/local/test_standard/baseline/sys-001/requirements.yml
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/resources/test_data/data/local/test_standard/baseline/sys-001/software_verification_cases.yml
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/resources/test_data/data/local/test_standard/baseline/sys-001/ext-001/requirements.yml
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/resources/test_data/data/local/test_standard/baseline/sys-001/ext-002/requirements.yml
--rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/resources/test_data/data/local/test_standard/empty_ms/ms-001/annotations.yml
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/resources/test_data/data/local/test_standard/empty_ms/ms-001/requirements.yml
--rw-r--r--   0        0        0     7125 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/resources/test_data/data/local/test_standard/empty_ms/ms-001/test_results/failsafe/TEST-com.reqstool.example.demo.DemoApplicationTestsIT.xml
--rw-r--r--   0        0        0     8258 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/resources/test_data/data/local/test_standard/empty_ms/ms-001/test_results/surefire/TEST-com.reqstool.example.demo.SVCsTest.xml
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/resources/test_data/data/local/test_standard/empty_ms/sys-001/manual_verification_results.yml
--rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/resources/test_data/data/local/test_standard/empty_ms/sys-001/requirements.yml
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/resources/test_data/data/local/test_standard/empty_ms/sys-001/software_verification_cases.yml
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/resources/test_data/data/local/test_standard/empty_ms/sys-001/ext-001/requirements.yml
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/resources/test_data/data/local/test_standard/empty_ms/sys-001/ext-002/requirements.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/resources/test_data/data/remote/test_standard/test_standard_maven_git/ms-001/annotations.yml -> ../../../../local/test_standard/baseline/ms-001/annotations.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/resources/test_data/data/remote/test_standard/test_standard_maven_git/ms-001/manual_verification_results.yml -> ../../../../local/test_standard/baseline/ms-001/manual_verification_results.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/resources/test_data/data/remote/test_standard/test_standard_maven_git/ms-001/requirements.yml -> ../../../../local/test_standard/baseline/ms-001/requirements.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/resources/test_data/data/remote/test_standard/test_standard_maven_git/ms-001/software_verification_cases.yml -> ../../../../local/test_standard/baseline/ms-001/software_verification_cases.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/resources/test_data/data/remote/test_standard/test_standard_maven_git/sys-001/annotations.yml -> ../../../../local/test_standard/baseline/sys-001/annotations.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/resources/test_data/data/remote/test_standard/test_standard_maven_git/sys-001/manual_verification_results.yml -> ../../../../local/test_standard/baseline/sys-001/manual_verification_results.yml
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/resources/test_data/data/remote/test_standard/test_standard_maven_git/sys-001/requirements.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/resources/test_data/data/remote/test_standard/test_standard_maven_git/sys-001/software_verification_cases.yml -> ../../../../local/test_standard/baseline/sys-001/software_verification_cases.yml
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/resources/unit/reqstool/model_generators/test_annotations_model_generator/test_annotations_model_generator/annotations.yml
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/resources/unit/reqstool/model_generators/test_mvrs_model_generator/test_mvrs_model_generator/manual_verification_results.yml
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/resources/unit/reqstool/model_generators/test_requirements_model_generator/test_external_requirements_model_generator/requirements.yml
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/resources/unit/reqstool/model_generators/test_requirements_model_generator/test_microservice_requirements_model_generator/requirements.yml
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/resources/unit/reqstool/model_generators/test_requirements_model_generator/test_rational_optional_model_generator/requirements.yml
--rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/resources/unit/reqstool/model_generators/test_requirements_model_generator/test_system_requirements_model_generator/requirements.yml
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/resources/unit/reqstool/model_generators/test_svcs_model_generator/test_svcs_model_generator/software_verification_cases.yml
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/unit/conftest.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/unit/reqstool/commands/generate_json/test_generate_json.py
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/unit/reqstool/commands/report/test_report.py
--rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/unit/reqstool/commands/report/criterias/test_criterias.py
--rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/unit/reqstool/commands/status/test_statistics_container.py
--rw-r--r--   0        0        0    18308 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/unit/reqstool/commands/status/test_statistics_generator.py
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/unit/reqstool/commands/status/test_status.py
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/unit/reqstool/common/test_locations.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/unit/reqstool/common/test_utils.py
--rw-r--r--   0        0        0     8041 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/unit/reqstool/common/validators/test_semantic_validator.py
--rw-r--r--   0        0        0     5222 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/unit/reqstool/expression_languages/test_requirements_el.py
--rw-r--r--   0        0        0     3971 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/unit/reqstool/expression_languages/test_svcs_el.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/unit/reqstool/locations/test_git_location.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/unit/reqstool/locations/test_local_location.py
--rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/unit/reqstool/model_generators/test_annotations_model_generator.py
--rw-r--r--   0        0        0     3285 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/unit/reqstool/model_generators/test_combined_indexed_dataset_generator.py
--rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/unit/reqstool/model_generators/test_combined_raw_datasets_generator.py
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/unit/reqstool/model_generators/test_mvrs_model_generator.py
--rw-r--r--   0        0        0    11130 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/unit/reqstool/model_generators/test_requirements_model_generator.py
--rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/unit/reqstool/model_generators/test_svcs_model_generator.py
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/unit/reqstool/model_generators/test_testdata_model_generator.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/unit/reqstool/models/test_annotations.py
--rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/unit/reqstool/models/test_implementations.py
--rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/unit/reqstool/models/test_imports.py
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/unit/reqstool/models/test_mvrs.py
--rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/unit/reqstool/models/test_requirements.py
--rw-r--r--   0        0        0     2922 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/unit/reqstool/models/test_svcs.py
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/unit/reqstool/reqstool_config/test_reqstool_config.py
--rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/unit/reqstool/requirements_indata/test_requirements_indata_paths.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 reqstool-0.4.1/tests/unit/reqstool/resources/schemas/v1/test_json_schemas.py
--rw-r--r--   0        0        0     4213 2020-02-02 00:00:00.000000 reqstool-0.4.1/.gitignore
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 reqstool-0.4.1/LICENSE
--rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 reqstool-0.4.1/README.md
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 reqstool-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     4128 2020-02-02 00:00:00.000000 reqstool-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 reqstool-0.4.2/.github/dependabot.yml
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 reqstool-0.4.2/.github/workflows/build.yml
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 reqstool-0.4.2/.github/workflows/check_release.yml
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 reqstool-0.4.2/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 reqstool-0.4.2/.github/workflows/publish_gh_pages.yml
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 reqstool-0.4.2/.github/workflows/publish_pypi_prod.yml
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 reqstool-0.4.2/.github/workflows/publish_pypi_test.yml
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/antora-playbook.yml
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/antora.yml
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/examples/requirements/manual_verification_results.yml
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/examples/requirements/requirements_external.yml
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/examples/requirements/requirements_microservice.yml
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/examples/requirements/requirements_system.yml
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/examples/requirements/software_verification_cases.yml
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/modules/ROOT/nav.adoc
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/modules/ROOT/pages/background.adoc
+-rw-r--r--   0        0        0    10790 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/modules/ROOT/pages/data.adoc
+-rw-r--r--   0        0        0     3822 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/modules/ROOT/pages/file_and_directory_set.adoc
+-rw-r--r--   0        0        0     6723 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/modules/ROOT/pages/how_it_works.adoc
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/modules/ROOT/pages/index.adoc
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/modules/ROOT/pages/installation.adoc
+-rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/modules/ROOT/pages/overview.adoc
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/modules/ROOT/pages/quickstart.adoc
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/modules/ROOT/pages/terminology.adoc
+-rw-r--r--   0        0        0     3433 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/modules/ROOT/pages/usage.adoc
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/modules/ROOT/pages/yml/annotations.adoc
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/modules/ROOT/pages/yml/manual_verification_results.adoc
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/modules/ROOT/pages/yml/reqstool_config.adoc
+-rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/modules/ROOT/pages/yml/requirements.adoc
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/modules/ROOT/pages/yml/requirements_annotations.adoc
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/modules/ROOT/pages/yml/requirements_external.adoc
+-rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/modules/ROOT/pages/yml/requirements_microservice.adoc
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/modules/ROOT/pages/yml/requirements_system.adoc
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/modules/ROOT/pages/yml/software_verification_cases.adoc
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/modules/ROOT/pages/yml/svcs_annotations.adoc
+-rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/modules/ROOT/partials/C4_Component.puml
+-rw-r--r--   0        0        0    14863 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/modules/ROOT/partials/C4_Sequence.puml
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/modules/examples/partials/requirements/manual_verification_results.yml
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/modules/examples/partials/requirements/reqstool_config.yml
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/modules/examples/partials/requirements/requirements_external.yml
+-rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/modules/examples/partials/requirements/requirements_microservice.yml
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/modules/examples/partials/requirements/requirements_system.yml
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/modules/examples/partials/requirements/software_verification_cases.yml
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/reqstool/manual_verification_results.yml
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/reqstool/reqstool_config.yml
+-rw-r--r--   0        0        0    10690 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/reqstool/requirements.yml
+-rw-r--r--   0        0        0     6822 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/reqstool/software_verification_cases.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/__init__.py
+-rwxr-xr-x   0        0        0    10652 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/command.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/commands/exit_codes.py
+-rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/commands/generate_json/generate_json.py
+-rw-r--r--   0        0        0    10524 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/commands/report/report.py
+-rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/commands/report/criterias/group_by.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/commands/report/criterias/sort_by.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/commands/report/templates/annotation_impls.j2
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/commands/report/templates/annotation_tests.j2
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/commands/report/templates/mvrs.j2
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/commands/report/templates/report.j2
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/commands/report/templates/req_references.j2
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/commands/report/templates/requirements.j2
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/commands/report/templates/svcs.j2
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/commands/report/templates/total_statistics.j2
+-rw-r--r--   0        0        0     3055 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/commands/status/statistics_container.py
+-rw-r--r--   0        0        0    13286 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/commands/status/statistics_generator.py
+-rw-r--r--   0        0        0     9220 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/commands/status/status.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/common/jinja2.py
+-rw-r--r--   0        0        0     9339 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/common/utils.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/common/validator_error_holder.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/common/dataclasses/urn_id.py
+-rw-r--r--   0        0        0    12026 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/common/validators/semantic_validator.py
+-rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/common/validators/syntax_validator.py
+-rwxr-xr-x   0        0        0     2575 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/expression_languages/generic_el.py
+-rwxr-xr-x   0        0        0      235 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/expression_languages/requirements_el.py
+-rwxr-xr-x   0        0        0      203 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/expression_languages/svcs_el.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/filters/id_filters.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/filters/requirements_filters.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/filters/svcs_filters.py
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/location_resolver/location_resolver.py
+-rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/locations/git_location.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/locations/local_location.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/locations/location.py
+-rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/locations/maven_location.py
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/model_generators/annotations_model_generator.py
+-rw-r--r--   0        0        0    29195 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/model_generators/combined_indexed_dataset_generator.py
+-rw-r--r--   0        0        0    10755 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/model_generators/combined_raw_datasets_generator.py
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/model_generators/mvrs_model_generator.py
+-rw-r--r--   0        0        0    12615 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/model_generators/requirements_model_generator.py
+-rw-r--r--   0        0        0     4515 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/model_generators/svcs_model_generator.py
+-rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/model_generators/testdata_model_generator.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/models/annotations.py
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/models/combined_indexed_dataset.py
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/models/implementations.py
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/models/imports.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/models/mvrs.py
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/models/raw_datasets.py
+-rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/models/requirements.py
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/models/svcs.py
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/models/test_data.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/reqstool_config/reqstool_config.py
+-rw-r--r--   0        0        0     5508 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/requirements_indata/requirements_indata.py
+-rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/requirements_indata/requirements_indata_paths.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/requirements_indata/java/java_maven_requirements_indata_paths.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/requirements_indata/python/python_requirements_indata_paths.py
+-rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/resources/schemas/v1/annotations.schema.json
+-rw-r--r--   0        0        0    11023 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/resources/schemas/v1/common.schema.json
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/resources/schemas/v1/manual_verification_results.schema.json
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/resources/schemas/v1/reqstool_config.schema.json
+-rw-r--r--   0        0        0    10841 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/resources/schemas/v1/requirements.schema.json
+-rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/resources/schemas/v1/software_verification_cases.schema.json
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/integration/reqstool/model_generators/test_included_models_generator.py
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_basic/baseline/ms-101/annotations.yml
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_basic/baseline/ms-101/manual_verification_results.yml
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_basic/baseline/ms-101/requirements.yml
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_basic/baseline/ms-101/software_verification_cases.yml
+-rw-r--r--   0        0        0     6367 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_basic/baseline/ms-101/test_results/failsafe/TEST-com.example.RequirementsExampleTestsIT.xml
+-rw-r--r--   0        0        0     5744 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_basic/baseline/ms-101/test_results/surefire/TEST-com.example.RequirementsExampleTests.xml
+-rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_basic/layout_maven/ms-101/pom.xml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_basic/layout_maven/ms-101/src/resources/docs/requirements/manual_verification_results.yml -> ../../../../../../baseline/ms-101/manual_verification_results.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_basic/layout_maven/ms-101/src/resources/docs/requirements/requirements.yml -> ../../../../../../baseline/ms-101/requirements.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_basic/layout_maven/ms-101/src/resources/docs/requirements/software_verification_cases.yml -> ../../../../../../baseline/ms-101/software_verification_cases.yml
+-rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_basic/with_requirements_config/README.md
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_basic/with_requirements_config/ms-101/manual_verification_results.yml -> ../../baseline/ms-101/manual_verification_results.yml
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_basic/with_requirements_config/ms-101/reqstool_config.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_basic/with_requirements_config/ms-101/requirements.yml -> ../../baseline/ms-101/requirements.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_basic/with_requirements_config/ms-101/software_verification_cases.yml -> ../../baseline/ms-101/software_verification_cases.yml
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_errors/ms-101/annotations.yml
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_errors/ms-101/errors.adoc
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_errors/ms-101/manual_verification_results.yml
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_errors/ms-101/requirements.yml
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_errors/ms-101/software_verification_cases.yml
+-rw-r--r--   0        0        0     6367 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_errors/ms-101/test_results/failsafe/TEST-com.example.RequirementsExampleTestsIT.xml
+-rw-r--r--   0        0        0     5744 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_errors/ms-101/test_results/surefire/TEST-com.example.RequirementsExampleTests.xml
+-rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/baseline/visualization.adoc
+-rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/baseline/ms-001/annotations.yml
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/baseline/ms-001/manual_verification_results.yml
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/baseline/ms-001/requirements.yml
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/baseline/ms-001/software_verification_cases.yml
+-rw-r--r--   0        0        0     7126 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/baseline/ms-001/test_results/failsafe/TEST-com.reqstool.example.demo.DemoApplicationTestsIT.xml
+-rw-r--r--   0        0        0     8258 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/baseline/ms-001/test_results/surefire/TEST-com.reqstool.example.demo.SVCsTest.xml
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/baseline/sys-001/requirements.yml
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/baseline/sys-001/software_verification_cases.yml
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/baseline/sys-001/ext-001/requirements.yml
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/baseline/sys-001/ext-002/requirements.yml
+-rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/empty_ms/ms-001/annotations.yml
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/empty_ms/ms-001/requirements.yml
+-rw-r--r--   0        0        0     7125 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/empty_ms/ms-001/test_results/failsafe/TEST-com.reqstool.example.demo.DemoApplicationTestsIT.xml
+-rw-r--r--   0        0        0     8258 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/empty_ms/ms-001/test_results/surefire/TEST-com.reqstool.example.demo.SVCsTest.xml
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/empty_ms/sys-001/manual_verification_results.yml
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/empty_ms/sys-001/requirements.yml
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/empty_ms/sys-001/software_verification_cases.yml
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/empty_ms/sys-001/ext-001/requirements.yml
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/empty_ms/sys-001/ext-002/requirements.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/remote/test_standard/test_standard_maven_git/ms-001/annotations.yml -> ../../../../local/test_standard/baseline/ms-001/annotations.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/remote/test_standard/test_standard_maven_git/ms-001/manual_verification_results.yml -> ../../../../local/test_standard/baseline/ms-001/manual_verification_results.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/remote/test_standard/test_standard_maven_git/ms-001/requirements.yml -> ../../../../local/test_standard/baseline/ms-001/requirements.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/remote/test_standard/test_standard_maven_git/ms-001/software_verification_cases.yml -> ../../../../local/test_standard/baseline/ms-001/software_verification_cases.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/remote/test_standard/test_standard_maven_git/sys-001/annotations.yml -> ../../../../local/test_standard/baseline/sys-001/annotations.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/remote/test_standard/test_standard_maven_git/sys-001/manual_verification_results.yml -> ../../../../local/test_standard/baseline/sys-001/manual_verification_results.yml
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/remote/test_standard/test_standard_maven_git/sys-001/requirements.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/remote/test_standard/test_standard_maven_git/sys-001/software_verification_cases.yml -> ../../../../local/test_standard/baseline/sys-001/software_verification_cases.yml
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/unit/reqstool/model_generators/test_annotations_model_generator/test_annotations_model_generator/annotations.yml
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/unit/reqstool/model_generators/test_mvrs_model_generator/test_mvrs_model_generator/manual_verification_results.yml
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/unit/reqstool/model_generators/test_requirements_model_generator/test_external_requirements_model_generator/requirements.yml
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/unit/reqstool/model_generators/test_requirements_model_generator/test_microservice_requirements_model_generator/requirements.yml
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/unit/reqstool/model_generators/test_requirements_model_generator/test_rational_optional_model_generator/requirements.yml
+-rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/unit/reqstool/model_generators/test_requirements_model_generator/test_system_requirements_model_generator/requirements.yml
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/unit/reqstool/model_generators/test_svcs_model_generator/test_svcs_model_generator/software_verification_cases.yml
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/unit/conftest.py
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/unit/reqstool/commands/generate_json/test_generate_json.py
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/unit/reqstool/commands/report/test_report.py
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/unit/reqstool/commands/report/criterias/test_criterias.py
+-rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/unit/reqstool/commands/status/test_statistics_container.py
+-rw-r--r--   0        0        0    18426 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/unit/reqstool/commands/status/test_statistics_generator.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/unit/reqstool/commands/status/test_status.py
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/unit/reqstool/common/test_locations.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/unit/reqstool/common/test_utils.py
+-rw-r--r--   0        0        0     8209 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/unit/reqstool/common/validators/test_semantic_validator.py
+-rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/unit/reqstool/expression_languages/test_requirements_el.py
+-rw-r--r--   0        0        0     4054 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/unit/reqstool/expression_languages/test_svcs_el.py
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/unit/reqstool/filters/test_requirements_filters.py
+-rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/unit/reqstool/filters/test_software_verification_cases_filters.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/unit/reqstool/locations/test_git_location.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/unit/reqstool/locations/test_local_location.py
+-rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/unit/reqstool/model_generators/test_annotations_model_generator.py
+-rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/unit/reqstool/model_generators/test_combined_indexed_dataset_generator.py
+-rw-r--r--   0        0        0     3887 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/unit/reqstool/model_generators/test_combined_raw_datasets_generator.py
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/unit/reqstool/model_generators/test_mvrs_model_generator.py
+-rw-r--r--   0        0        0    11130 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/unit/reqstool/model_generators/test_requirements_model_generator.py
+-rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/unit/reqstool/model_generators/test_svcs_model_generator.py
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/unit/reqstool/model_generators/test_testdata_model_generator.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/unit/reqstool/models/test_annotations.py
+-rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/unit/reqstool/models/test_implementations.py
+-rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/unit/reqstool/models/test_imports.py
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/unit/reqstool/models/test_mvrs.py
+-rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/unit/reqstool/models/test_requirements.py
+-rw-r--r--   0        0        0     2922 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/unit/reqstool/models/test_svcs.py
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/unit/reqstool/reqstool_config/test_reqstool_config.py
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/unit/reqstool/requirements_indata/test_requirements_indata_paths.py
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/unit/reqstool/resources/schemas/v1/test_json_schemas.py
+-rw-r--r--   0        0        0     4213 2020-02-02 00:00:00.000000 reqstool-0.4.2/.gitignore
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 reqstool-0.4.2/LICENSE
+-rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 reqstool-0.4.2/README.md
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 reqstool-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     4177 2020-02-02 00:00:00.000000 reqstool-0.4.2/PKG-INFO
```

### Comparing `reqstool-0.4.1/.github/dependabot.yml` & `reqstool-0.4.2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/.github/workflows/build.yml` & `reqstool-0.4.2/.github/workflows/build.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 name: Build PyPI
 on:
-  workflow_call: 
+  workflow_call:
   workflow_dispatch:
   push:
   pull_request:
     types:
       - opened
       - reopened
       - synchronize
@@ -25,15 +25,15 @@
       - name: Set up Python
         uses: actions/setup-python@v5
         with:
           python-version: "3.10"
       - name: Install dependencies
         run: pip install hatch
       - name: Run unit and integrations tests
-        run: hatch run test:pytest --cov=reqstool-python-decorators --cov-report=xml --cov-report=html 
+        run: hatch run test:pytest --cov=reqstool-client --cov-report=xml --cov-report=html -o junit_family=xunit2 --junitxml=build/junit.xml
       - name: Build project
         run: hatch build
       # Upload artifacts for later use
       - name: Upload Artifacts
         uses: actions/upload-artifact@v4
         with:
           name: dist
```

### Comparing `reqstool-0.4.1/.github/workflows/lint.yml` & `reqstool-0.4.2/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/.github/workflows/publish_gh_pages.yml` & `reqstool-0.4.2/.github/workflows/publish_gh_pages.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/.github/workflows/publish_pypi_prod.yml` & `reqstool-0.4.2/.github/workflows/publish_pypi_prod.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/.github/workflows/publish_pypi_test.yml` & `reqstool-0.4.2/.github/workflows/publish_pypi_test.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/docs/antora-playbook.yml` & `reqstool-0.4.2/docs/antora-playbook.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/docs/examples/requirements/requirements_external.yml` & `reqstool-0.4.2/docs/examples/requirements/requirements_external.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/docs/examples/requirements/requirements_microservice.yml` & `reqstool-0.4.2/docs/examples/requirements/requirements_microservice.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/docs/examples/requirements/requirements_system.yml` & `reqstool-0.4.2/docs/examples/requirements/requirements_system.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/docs/examples/requirements/software_verification_cases.yml` & `reqstool-0.4.2/docs/examples/requirements/software_verification_cases.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/docs/modules/ROOT/pages/background.adoc` & `reqstool-0.4.2/docs/modules/ROOT/pages/background.adoc`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/docs/modules/ROOT/pages/data.adoc` & `reqstool-0.4.2/docs/modules/ROOT/pages/data.adoc`

 * *Files 4% similar despite different names*

```diff
@@ -124,15 +124,15 @@
 <.> Surefire Reports root
 <.> See xref:yml/requirements_annotations.adoc[requirements_annotations.yml example]
 <.> See xref:yml/svcs_annotations.adoc[svcs_annotations.yml example]
 
 [[maven-artifact-zip-directory-structure]]
 === Maven Artifact Zip Directory Structure
 
-In order to produce a Maven Artifact Zip, you will need to incorporate the https://github.com/Luftfartsverket/requirements-tool-maven-assembly[Maven Assembly Plugin] into your build process. 
+In order to produce a Maven Artifact Zip, you will need to incorporate the https://github.com/Luftfartsverket/reqstool-java-maven-plugin[Reqstool Java Maven Plugin] into your build process. 
 
 During the build process, the plugin creates a zipfile with the static and dynamic files. The zipfile will be named like <<project-id>>-<<version>>-reqstool.zip and will be published under the target/reqstool folder.
 The plugin will also combine the svcs_annotations.yml and the equirements_annotations.yml into one yml file called annotations.yml.
 
 The Reqstool artifact uploaded as a zip to a Maven repository needs to have the following structure:
 
 [listing]
@@ -177,15 +177,15 @@
 === Local import
 
 To import content from other sources (systems) on the same file system as your current project. 
 
 .requirements.yml
 ```yaml
 
-systems:
+imports:
   local:
     - path: ../sys-001
 
 ```
 
 === Git import
 
@@ -196,15 +196,15 @@
 Normally, you should refrain from entering token information explicitly, but rather point towards a secret only accessible through your development/production pipeline or environment variables. 
 
 If no authentication is required in order to access the repository, the field `env_token` can be omitted
 
 
 .requirements.yml
 ```yaml
-systems:
+imports:
   git:
     - url: https://github.com/Luftfartsverket/reqstool-demo
       branch: main
       path: docs/reqstool
       env_token: SECRET_TOKEN
 ```
 
@@ -212,62 +212,63 @@
 
 === Maven import
 
 To import content from other sources (systems) using Maven. 
 
 .requirements.yml
 ```yaml
-systems:
+imports:
   maven:
     - url: https://maven.pkg.github.com/Luftfartsverket/reqstool-client
       group_id: se.lfv.reqstool.testdata
       artifact_id: reqstool-testdata-test-basic-ms101
       path: ""
       version: 0.0.2
 ```
 
 === Import from different sources
 
 It is also possible to import files from different types of sources. 
 
 .requirements.yml
 ```yaml
-systems:
+imports:
   local:
     - path: ../sys-001
   git:
     - url: https://github.com/Luftfartsverket/reqstool-demo
       branch: main
       path: docs/reqstool
 ```
 
 [[filters]]
 == Filters
 
-Filters can be applied on both requirements.yml and software_verification_cases.yml in order to exclude or include certain requirements or software verification cases. Note that the `filter` key is on different levels in the two files
+Filters can be applied on both requirements.yml and software_verification_cases.yml in order to exclude or include certain requirements or software verification cases. 
 
 
 .requiremens.yml
 ```yaml
-systems:
-  local:
-    - path: ../sys-001
-      filters:
-        sys-001:
-          requirement_ids:
-            includes: ["REQ_sys001_103", "ext-001:REQ_ext001_101"]
+filters:
+  sys-001:
+    requirement_ids:
+      includes: 
+        - REQ_sys001_103
+        - ext-001:REQ_ext001_101
 ```
 
 
 .software_verification_cases.yml
 ```yaml
 filters:
   sys-001:
     svc_ids:
-      imports: ["SVC_sys001_101", "SVC_sys001_109"]
+      includes: 
+        - SVC_sys001_101
+        - SVC_sys001_109
 ```
 
 == Categories
 
 A requirement is assigned to one, or multiple categories.
 
 .requirements.yml
@@ -284,20 +285,22 @@
 
 Categories follow the https://iso25000.com/index.php/en/iso-25000-standards/iso-25010[ISO 25010 0 Product Quality Characteristics].
 
 === ISO 25010 Product Quality Characteristics
 
 * **Functional Suitability:** Functional Suitability assesses the degree to which the software provides appropriate functions that meet specified needs under specified conditions. It involves evaluating the completeness and appropriateness of the functions provided by the software.
 
-* **Reliability:** Reliability refers to the degree to which the software performs specified functions under specified conditions without failure for a specified period of time. It involves assessing the software's ability to maintain its performance level over time and under varying conditions.
-
 * **Performance Efficiency:** Performance efficiency evaluates the degree to which the software provides appropriate performance relative to the amount of resources used under specified conditions. It includes considerations such as response time, throughput, and resource utilization.
 
 * **Compatibility:** Compatibility assesses the degree to which the software can exchange information and work together with other systems, products, or environments without requiring special effort. It involves evaluating interoperability and integration capabilities.
 
-* **Usability:** Usability refers to the degree to which the software is easy to use, understand, and attractive to the user when used under specified conditions. It involves assessing aspects such as learnability, efficiency, and user satisfaction.
+* **Interaction Capability:** Describes to which degree a product or system can be interacted with by specified users to exchange information.
+
+* **Reliability:** Reliability refers to the degree to which the software performs specified functions under specified conditions without failure for a specified period of time. It involves assessing the software's ability to maintain its performance level over time and under varying conditions.
+
+* **Security:** Security refers to the degree to which the software protects information and data from unauthorized access, disclosure, alteration, or destruction. It involves assessing aspects such as confidentiality, integrity, authentication, authorization, and non-repudiation.
 
 * **Maintainability:** Maintainability evaluates the degree to which the software can be modified effectively and efficiently without introducing defects or degrading performance. It involves assessing aspects such as modifiability, analyzability, and testability.
 
-* **Portability:** Portability assesses the degree to which the software can be transferred from one environment to another, including the necessary adaptation effort. It involves considerations such as adaptability, installability, and coexistence with other software.
+* **Flexibility:** Portability assesses the degree to which the software can be transferred from one environment to another, including the necessary adaptation effort. It involves considerations such as adaptability, installability, and coexistence with other software.
 
-* **Security:** Security refers to the degree to which the software protects information and data from unauthorized access, disclosure, alteration, or destruction. It involves assessing aspects such as confidentiality, integrity, authentication, authorization, and non-repudiation.
+* **Safety:** This characteristic represents the degree to which a product under defined conditions to avoid a state in which human life, health, property, or the environment is endangered.
```

### Comparing `reqstool-0.4.1/docs/modules/ROOT/pages/file_and_directory_set.adoc` & `reqstool-0.4.2/docs/modules/ROOT/pages/file_and_directory_set.adoc`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 == Standard File and Directory Set
 
-All files have a JSON Schema: https://raw.githubusercontent.com/Luftfartsverket/reqstool-client/main/src/reqstool/resources/schemas/v1/
+All files have a JSON Schema: https://github.com/Luftfartsverket/reqstool-client/tree/main/src/reqstool/resources/schemas/v1
 
 For examples see:
 
 * docs/examples
 * unit tests: [TODO](#todo)
 
 [[reqstool_config]]
@@ -32,17 +32,17 @@
 Below is an example on how to change the default paths to the required *.yml files and folders that are generated when the artifact is produced by Maven. The path specified for should be relative to the -p argument that you provide when Reqstool is run. 
 
 ```yaml
 # yaml-language-server: $schema=https://raw.githubusercontent.com/Luftfartsverket/reqstool-client/main/src/reqstool/resources/schemas/v1/reqstool_config.schema.json
 
 type: custom 
 locations:
-  test_results:
-    failsafe: ../target/some_folder/failsafe
-    surefire: ../target/my_folder/surefire
+  test_results_dirs:
+    - ../target/some_folder/failsafe
+    - ../target/my_folder/surefire
   annotations:
     implementations: ../target/hello/requirements_annotations_impls.yml
     tests: ../target/demo/requirements_annotations_tests.yml
 
 ```
 
 === requirements.yml
@@ -65,7 +65,15 @@
 Typically generated by an annotations parser and lists all requirement annotations 
 
 NOTE: JSON Schema
 
 === svcs_annotations.yml
 
 Typically generated by an annotations parser and lists all software verification cases annotations.
+
+=== annotations.yml
+
+Lists all annotations, containing both requirements and software verification cases annotations.
+
+Generated by default by python annotations parser.
+
+Generated by Maven plugin for Java projects that combines requirements_annotations.yml and svcs_annotations.yml
```

### Comparing `reqstool-0.4.1/docs/modules/ROOT/pages/how_it_works.adoc` & `reqstool-0.4.2/docs/modules/ROOT/pages/how_it_works.adoc`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 === What is it?
 
 Reqstool generates reports and updates on progression of requirement implementations and testing by reading data specified in several *.yml files. 
 
 In order to use the reqstool, you will need to create a requirements.yml file along with a software_verification_cases.yml and/or a manual_verification_results.yml. 
 
-* Examples: https://github.com/Luftfartsverket/reqstool-client/docs/modules/examples/partials/requirements
+* Examples: https://github.com/Luftfartsverket/reqstool-client/tree/main/docs/modules/examples/partials/requirements
 * Demo: https://github.com/Luftfartsverket/reqstool-demo
 
 === How it works
 
 All of the commands available for the user requires an argument specifying a path to where Reqstool should start to look for the required files. When a valid path is provided, the CombinedRawDatasetsGenerator component parses all yaml files in the specified path and validates the generated content with the SemanticValidator component. The -h command of the application can assist you regarding what argument you'll need to provide for each command.
 
 What each command actually does is described under xref:usage.adoc[usage]
@@ -80,22 +80,23 @@
 So, if you have a micro service (let's call i ms-001) that will also inherit requirements from another source (ext-001), you want to start the parsing in the docs/requirements path of ms-001
 
 When the initial source's requirement file are processed, Reqstool will then continue to parse the other sources that are specified within the import parameter of the initial source's requirement file. If filters is applied in the initial source, the data in the following sources will adhere to these settings.
 
 For example, if you want to exclude one requirement from ext-001, then you specify it like this in the requirements.yml file in ms-001 project:
 
 ```yaml
-systems:
+imports:
   local:
     - path: ./ext-001
-      filters:
-        ext-001:
-          requirement_ids:
-            excludes:
-              - REQ_101
+      
+filters:
+  ext-001:
+    requirement_ids:
+      excludes:
+        - REQ_101
 
 ```
 
 When Requirement Tool is reading the data from ext-001, then REQ_101 will not be imported in the returning data, but all other requirements specified in ext-001's requirements.yml file will.  
 
 Filters can currently be applied to requirements.yml and software_verification_cases.yml.
```

### Comparing `reqstool-0.4.1/docs/modules/ROOT/pages/index.adoc` & `reqstool-0.4.2/docs/modules/ROOT/pages/index.adoc`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/docs/modules/ROOT/pages/overview.adoc` & `reqstool-0.4.2/docs/modules/ROOT/pages/overview.adoc`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/docs/modules/ROOT/pages/terminology.adoc` & `reqstool-0.4.2/docs/modules/ROOT/pages/terminology.adoc`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/docs/modules/ROOT/pages/usage.adoc` & `reqstool-0.4.2/docs/modules/ROOT/pages/usage.adoc`

 * *Files 27% similar despite different names*

```diff
@@ -26,30 +26,41 @@
 ```
 
 Example:
 
 STATUS RESULT
 
 |===
-| Req id | Implementation| Automated Test | Manual Test
-| REQ_ms001_101 | +++<span style="color:green">Implemented</span>+++ | +++<span style="color:green">Pass</span>+++ | +++<span style="color:blue">N/A</span>+++
-| REQ_ms001_102 | +++<span style="color:green">Implemented</span>+++ | +++<span style="color:blue">N/A</span>+++ | +++<span style="color:red">Fail</span>+++
-| REQ_sys001_101 | +++<span style="color:red">Lacks implementation</span>+++ | +++<span style="color:green">Pass</span>+++ | +++<span style="color:blue">N/A</span>+++
-| REQ_sys001_102 | +++<span style="color:red">Lacks implementation</span>+++ | +++<span style="color:blue">N/A</span>+++ | +++<span style="color:blue">N/A</span>+++
-| REQ_sys001_103 | +++<span style="color:green">Implemented</span>+++ | +++<span style="color:red">Fail</span>+++ | +++<span style="color:blue">N/A</span>+++
-| REQ_ext001_101 | +++<span style="color:green">Implemented</span>+++ | +++<span style="color:green">Pass</span>+++ | +++<span style="color:blue">N/A</span>+++
-| REQ_ext001_103 | +++<span style="color:red">Lacks implementation</span>+++ | +++<span style="color:blue">N/A</span>+++ | +++<span style="color:blue">N/A</span>+++
-| REQ_ext002_101 | +++<span style="color:red">Lacks implementation</span>+++ | +++<span style="color:blue">N/A</span>+++ | +++<span style="color:blue">N/A</span>+++
-| REQ_ext002_102 | +++<span style="color:red">Lacks implementation</span>+++ | +++<span style="color:blue">N/A</span>+++ | +++<span style="color:blue">N/A</span>+++
-| REQ_ext002_103 | +++<span style="color:red">Lacks implementation</span>+++ | +++<span style="color:blue">N/A</span>+++ | +++<span style="color:blue">N/A</span>+++
+| URN | Req id | Implementation| Automated Test | Manual Test
+| ms001 | +++<span style="color:green">REQ_ms001_101</span>+++ | +++<span style="color:green">Implemented</span>+++ | T2 +++<span style="color:green">P2</span>+++ | N/A
+| ms001 | +++<span style="color:red">REQ_ms001_102</span>+++ | +++<span style="color:green">Implemented</span>+++ | N/A | T1 +++<span style="color:red">F1</span>+++
+| sys001 | +++<span style="color:red">REQ_sys001_101</span>+++ | +++<span style="color:red">Missing</span>+++ | T1 +++<span style="color:green">P1</span>+++ | N/A
+| sys001 | +++<span style="color:red">REQ_sys001_102</span>+++ | +++<span style="color:red">Missing</span>+++ | N/A | N/A
+| sys001 | +++<span style="color:red">REQ_sys001_103</span>+++ | +++<span style="color:green">Implemented</span>+++ | T0 +++<span style="color:red">M1</span>+++ | N/A
+| ext001 | +++<span style="color:green">REQ_ext001_101</span>+++ | +++<span style="color:green">Implemented</span>+++ | T3 +++<span style="color:green">P3</span>+++ | T1 +++<span style="color:green">P1</span>+++
+| ext001 | +++<span style="color:red">REQ_ext001_103</span>+++ | +++<span style="color:red">Missing</span>+++ | N/A | N/A
+| ext002 | +++<span style="color:red">REQ_ext002_101</span>+++ | +++<span style="color:red">Missing</span>+++ | N/A | N/A
+| ext002 | +++<span style="color:red">REQ_ext002_102</span>+++ | +++<span style="color:red">Missing</span>+++ | N/A | N/A
+| ext002 | +++<span style="color:red">REQ_ext002_103</span>+++ | +++<span style="color:red">Missing</span>+++ | N/A | N/A
 |===
 
 |===
-|Total requirements|Not implemented|Missing tests|Failing tests
-| 3 | 0 (0.00%) | 0 (0.00%) | 2 (66.67%)
+| Total Requirements: 10
+|===
+|===
+| Implemented and Verified | Implemented | Not implemented
+| 2 (20.00%) | 2 (20.00%) | 6 (60.00%)
+|===
+
+|===
+| Total Tests: 8 | Total SVCs: 9
+|===
+|===
+| Passed tests | Failed tests | Skipped tests | SVCs missing tests | SVCs missing MVRs
+| 7 (87.50%) | 1 (12.50%) | 0 (60.00%) | 1 (11.11%) | 0 (0.00%)
 |===
 
 [[report]]
 == Command: report-asciidoc
 
 Generates a report in AsciiDoc.
```

### Comparing `reqstool-0.4.1/docs/modules/ROOT/pages/yml/annotations.adoc` & `reqstool-0.4.2/docs/modules/ROOT/pages/yml/annotations.adoc`

 * *Files 9% similar despite different names*

```diff
@@ -23,11 +23,11 @@
         fullyQualifiedName: "package.example.SVCsTest"
     SVC_011:
       - elementKind: "CLASS"
         fullyQualifiedName: "package.example.SVCsTest"
     SVC_025:
       - elementKind: "METHOD"
         fullyQualifiedName: "package.example.SVCsTest.testMethod1"
-    SVC_040:
+    SVC_031:
       - elementKind: "METHOD"
         fullyQualifiedName: "package.example.SVCsTest.testMethod2"
 ----
```

### Comparing `reqstool-0.4.1/docs/modules/ROOT/pages/yml/requirements.adoc` & `reqstool-0.4.2/docs/modules/ROOT/pages/yml/requirements.adoc`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/docs/modules/ROOT/pages/yml/requirements_annotations.adoc` & `reqstool-0.4.2/docs/modules/ROOT/pages/yml/requirements_annotations.adoc`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/docs/modules/ROOT/pages/yml/requirements_external.adoc` & `reqstool-0.4.2/docs/modules/ROOT/pages/yml/requirements_external.adoc`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/docs/modules/ROOT/pages/yml/requirements_microservice.adoc` & `reqstool-0.4.2/docs/modules/ROOT/pages/yml/requirements_microservice.adoc`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/docs/modules/ROOT/pages/yml/requirements_system.adoc` & `reqstool-0.4.2/docs/modules/ROOT/pages/yml/requirements_system.adoc`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/docs/modules/ROOT/pages/yml/software_verification_cases.adoc` & `reqstool-0.4.2/docs/modules/ROOT/pages/yml/software_verification_cases.adoc`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/docs/modules/ROOT/pages/yml/svcs_annotations.adoc` & `reqstool-0.4.2/docs/modules/ROOT/pages/yml/svcs_annotations.adoc`

 * *Files 25% similar despite different names*

```diff
@@ -11,12 +11,12 @@
         fullyQualifiedName: "package.example.ms001.SVCsTest"
     SVC_011:
       - elementKind: "CLASS"
         fullyQualifiedName: "package.example.ms001.SVCsTest"
     SVC_025:
       - elementKind: "METHOD"
         fullyQualifiedName: "package.example.SVCsTest.testMethod1"
-    SVC_040:
+    SVC_031:
       - elementKind: "METHOD"
         fullyQualifiedName: "package.example.SVCsTest.testMethod2"
 
 ----
```

### Comparing `reqstool-0.4.1/docs/modules/ROOT/partials/C4_Component.puml` & `reqstool-0.4.2/docs/modules/ROOT/partials/C4_Component.puml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/docs/modules/ROOT/partials/C4_Sequence.puml` & `reqstool-0.4.2/docs/modules/ROOT/partials/C4_Sequence.puml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/docs/modules/examples/partials/requirements/software_verification_cases.yml` & `reqstool-0.4.2/docs/modules/examples/partials/requirements/software_verification_cases.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # yaml-language-server: $schema=https://raw.githubusercontent.com/Luftfartsverket/reqstool-client/main/src/reqstool/resources/schemas/v1/software_verification_cases.schema.json
 
 filters:
   sys001:
-    svcs_ids:
-      imports: ["SVC_123", "SVC_124"]
+    svc_ids:
+      includes: ["SVC_123", "SVC_124"]
     custom:
-      imports: 'ids == "SVC_123", "SVC_124"'
+      includes: 'ids == "SVC_123", "SVC_124"'
   sys002:
-    svcs_ids:
+    svc_ids:
       excludes: ["SVC_123", "SVC_124"]
     custom:
       exclude: 'ids == "SVC_123", "SVC_124"'
 
 cases:
   - id: # alphanumerical
     requirement_ids: # array of alphanumerical
```

### Comparing `reqstool-0.4.1/src/reqstool/command.py` & `reqstool-0.4.2/src/reqstool/command.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 import sys
 from importlib.metadata import version
 from typing import TextIO, Union
 
 if __package__ is None or len(__package__) == 0:
     sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
 
+from reqstool_python_decorators.decorators.decorators import Requirements
+
 from reqstool.commands.exit_codes import EXIT_CODE_ALL_REQS_NOT_IMPLEMENTED
 from reqstool.commands.generate_json.generate_json import GenerateJsonCommand
 from reqstool.commands.report import report
 from reqstool.commands.report.criterias.group_by import GroupbyOptions
 from reqstool.commands.report.criterias.sort_by import SortByOptions
 from reqstool.commands.status.status import StatusCommand
 from reqstool.common.validators.syntax_validator import JsonSchemaItem
@@ -197,36 +199,39 @@
                 env_token=args_source.env_token if args_source.env_token else None,
             )
         elif "local" in args_source.source:
             location = LocalLocation(path=args_source.path)
 
         return location
 
+    @Requirements("REQ_035")
     def command_report(self, report_args: argparse.Namespace):
         initial_source = self._get_initial_source(report_args)
 
         output = report_args.output  # where to put the generated report
         result = report.ReportCommand(
             location=initial_source,
             group_by=GroupbyOptions(report_args.group_by),
             sort_by=[SortByOptions(s) for s in report_args.sort_by],
         )
 
         output.write(result.result)
 
+    @Requirements("REQ_031")
     def command_generate_json(self, generate_json_args: argparse.Namespace):
         initial_source = self._get_initial_source(generate_json_args)
 
         filter_data = not generate_json_args.no_filter
 
         result = GenerateJsonCommand(location=initial_source, filter_data=filter_data)
 
         output = generate_json_args.output  # where to put the generated report
         output.write(result.result)
 
+    @Requirements("REQ_029")
     def command_status(self, status_args: argparse.Namespace) -> int:
         initial_source = self._get_initial_source(status_args)
         output = status_args.output  # where to put the generated report
 
         result = StatusCommand(location=initial_source)
         status, nr_of_incomplete_requirements = result.result
```

### Comparing `reqstool-0.4.1/src/reqstool/commands/generate_json/generate_json.py` & `reqstool-0.4.2/src/reqstool/commands/generate_json/generate_json.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Copyright © LFV
 
 
 import re
 from enum import Enum
 
 import jsonpickle
+from reqstool_python_decorators.decorators.decorators import Requirements
 
 from reqstool.common.dataclasses.urn_id import UrnId
 from reqstool.common.validator_error_holder import ValidationErrorHolder
 from reqstool.common.validators.semantic_validator import SemanticValidator
 from reqstool.locations.location import LOCATIONTYPES, LocationInterface
 from reqstool.model_generators.combined_indexed_dataset_generator import CombinedIndexedDatasetGenerator
 from reqstool.model_generators.combined_raw_datasets_generator import CombinedRawDatasetsGenerator
@@ -30,14 +31,15 @@
     def restore(self, obj):
         pass
 
     def flatten(self, obj: Enum, data):
         return obj.value
 
 
+@Requirements("REQ_030")
 class GenerateJsonCommand:
     def __init__(self, location: LocationInterface, filter_data: bool):
         self.__initial_location: LocationInterface = location
         self.__filter_data: bool = filter_data
         self.result = self.__run()
 
     def __run(self) -> str:
```

### Comparing `reqstool-0.4.1/src/reqstool/commands/report/report.py` & `reqstool-0.4.2/src/reqstool/commands/report/report.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Copyright © LFV
 
 from enum import Enum
 from typing import Dict, List, Union
 
 from jinja2 import Template
+from reqstool_python_decorators.decorators.decorators import Requirements
 
 from reqstool.commands.report.criterias.group_by import GroupbyOptions, GroupByOrganizor
 from reqstool.commands.report.criterias.sort_by import SortByOptions
 from reqstool.commands.status.statistics_container import StatisticsContainer
 from reqstool.commands.status.statistics_generator import StatisticsGenerator
 from reqstool.common.dataclasses.urn_id import UrnId
 from reqstool.common.jinja2 import Jinja2Utils
@@ -37,14 +38,15 @@
         obj = object.__new__(cls)
         obj._value_ = value
         obj.filename = filename
         obj.jinja2_template = None
         return obj
 
 
+@Requirements("REQ_032")
 class ReportCommand:
     def __init__(
         self,
         location: LocationInterface,
         group_by: GroupbyOptions,
         sort_by: List[SortByOptions],
     ):
```

### Comparing `reqstool-0.4.1/src/reqstool/commands/report/criterias/group_by.py` & `reqstool-0.4.2/src/reqstool/commands/report/criterias/group_by.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,25 +4,28 @@
 from collections import defaultdict
 from dataclasses import dataclass, field
 from enum import Enum
 from operator import attrgetter
 from types import MappingProxyType
 from typing import Callable, Dict, Iterator, List, Tuple
 
+from reqstool_python_decorators.decorators.decorators import Requirements
+
 from reqstool.commands.report.criterias.sort_by import SortByOptions
 from reqstool.common.dataclasses.urn_id import UrnId
 from reqstool.models.combined_indexed_dataset import CombinedIndexedDataset
 from reqstool.models.requirements import RequirementData
 
 
 class GroupbyOptions(Enum):
     INITIAL_IMPORTS = "initial/imports"
     CATEGORY = "category"
 
 
+@Requirements("REQ_033")
 @dataclass(kw_only=True)
 class GroupByOrganizor(ABC):
     cid: CombinedIndexedDataset
     group_by: GroupbyOptions
     sort_by: List[SortByOptions]
 
     grouped_requirements: Dict[str, List[UrnId]] = field(init=False, default_factory=lambda: defaultdict(list))
@@ -35,14 +38,15 @@
 
     def __iter__(self) -> Iterator[Tuple[str, List[UrnId]]]:
         return iter(self.grouped_requirements.items())
 
     def _add_req_to_group(self, group: str, urn_id: UrnId):
         self.grouped_requirements[group].append(urn_id)
 
+    @Requirements("REQ_034")
     def _sort(self):
         if len(self.sort_by) == 0:
             return
 
         for group, urn_ids in self.grouped_requirements.items():
             urn_ids.sort(
                 key=lambda urn_id: attrgetter(*[sort_option.value for sort_option in self.sort_by])(
```

### Comparing `reqstool-0.4.1/src/reqstool/commands/report/templates/total_statistics.j2` & `reqstool-0.4.2/src/reqstool/commands/report/templates/total_statistics.j2`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/src/reqstool/commands/status/statistics_container.py` & `reqstool-0.4.2/src/reqstool/commands/status/statistics_container.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # Copyright © LFV
 
 from dataclasses import dataclass, field
 
+from reqstool_python_decorators.decorators.decorators import Requirements
+
 from reqstool.common.dataclasses.urn_id import UrnId
 
 
+@Requirements("REQ_028")
 @dataclass(kw_only=True)
 class TestStatisticsItem:
     nr_of_failed_tests: int = 0
     nr_of_missing_automated_tests: int = 0
     nr_of_missing_manual_tests: int = 0
     nr_of_skipped_tests: int = 0
     nr_of_passed_tests: int = 0
@@ -17,22 +20,24 @@
 
     def is_completed(self):
         if self.nr_of_missing_automated_tests or self.nr_of_missing_manual_tests > 0:
             return False
         return self.nr_of_total_tests == self.nr_of_passed_tests
 
 
+@Requirements("REQ_028")
 @dataclass(kw_only=True, frozen=True)
 class CombinedRequirementTestItem:
     completed: bool = field(default=bool)
     nr_of_implementations: int = field(default=int)
     automated_tests_stats: TestStatisticsItem = field(default_factory=TestStatisticsItem)
     mvrs_stats: TestStatisticsItem = field(default_factory=TestStatisticsItem)
 
 
+@Requirements("REQ_028")
 @dataclass(kw_only=True)
 class TotalStatisticsItem:
     nr_of_failed_tests: int = 0
     nr_of_missing_automated_tests: int = 0
     nr_of_missing_manual_tests: int = 0
     nr_of_skipped_tests: int = 0
     nr_of_passed_tests: int = 0
@@ -48,14 +53,15 @@
         self.nr_of_missing_manual_tests += combined_req_test_item.mvrs_stats.nr_of_missing_manual_tests
         self.nr_of_reqs_with_implementation += combined_req_test_item.nr_of_implementations
 
         if completed:
             self.nr_of_completed_requirements += 1
 
 
+@Requirements("REQ_028")
 @dataclass(kw_only=True, frozen=True)
 class StatisticsContainer:
     _requirement_statistics: dict[str, CombinedRequirementTestItem] = field(default_factory=lambda: {})
 
     _total_statistics: TotalStatisticsItem = field(default_factory=TotalStatisticsItem)
 
     def add_stats_for_requirement(
```

### Comparing `reqstool-0.4.1/src/reqstool/commands/status/statistics_generator.py` & `reqstool-0.4.2/src/reqstool/commands/status/statistics_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # Copyright © LFV
 
 from enum import Enum
 from typing import Dict, List, Sequence
 
+from reqstool_python_decorators.decorators.decorators import Requirements
+
 from reqstool.commands.status.statistics_container import StatisticsContainer, TestStatisticsItem
 from reqstool.common.dataclasses.urn_id import UrnId
 from reqstool.common.validators.semantic_validator import SemanticValidator
 from reqstool.locations.location import LocationInterface
 from reqstool.model_generators.combined_indexed_dataset_generator import CombinedIndexedDatasetGenerator
 from reqstool.model_generators.combined_raw_datasets_generator import CombinedRawDatasetsGenerator
 from reqstool.models.combined_indexed_dataset import CombinedIndexedDataset
@@ -27,14 +29,15 @@
     PASSED = "passed"
     FAILED = "failed"
     SKIPPED = "skipped"
     MISSING = "missing"
     NA = "N/A"
 
 
+@Requirements("REQ_028")
 class StatisticsGenerator:
     def __init__(self, initial_location: LocationInterface, semantic_validator: SemanticValidator, apply_filter=True):
         self.cid: CombinedIndexedDataset = self._get_combined_index_data(
             initial_location=initial_location, semantic_validator=semantic_validator, apply_filter=apply_filter
         )
         self.stats_container = self.calculate_totals()
         self.result: StatisticsContainer = self._calculate(self.cid)
```

### Comparing `reqstool-0.4.1/src/reqstool/commands/status/status.py` & `reqstool-0.4.2/src/reqstool/commands/status/status.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # Copyright © LFV
 
 from typing import List, Tuple
 
 from colorama import Fore, Style
+from reqstool_python_decorators.decorators.decorators import Requirements
 from tabulate import tabulate
 
 from reqstool.commands.status.statistics_container import StatisticsContainer, TestStatisticsItem
 from reqstool.commands.status.statistics_generator import StatisticsGenerator
 from reqstool.common.validator_error_holder import ValidationErrorHolder
 from reqstool.common.validators.semantic_validator import SemanticValidator
 from reqstool.locations.location import LocationInterface
 
 
+@Requirements("REQ_027")
 class StatusCommand:
     def __init__(self, location: LocationInterface):
         self.__initial_location: LocationInterface = location
         self.result = self.__status_result()
 
     def __status_result(self) -> Tuple[str, int]:
         statistics: StatisticsContainer = StatisticsGenerator(
```

### Comparing `reqstool-0.4.1/src/reqstool/common/jinja2.py` & `reqstool-0.4.2/src/reqstool/common/jinja2.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/src/reqstool/common/utils.py` & `reqstool-0.4.2/src/reqstool/common/utils.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/src/reqstool/common/validator_error_holder.py` & `reqstool-0.4.2/src/reqstool/common/validator_error_holder.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/src/reqstool/common/dataclasses/urn_id.py` & `reqstool-0.4.2/src/reqstool/common/dataclasses/urn_id.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/src/reqstool/common/validators/semantic_validator.py` & `reqstool-0.4.2/src/reqstool/common/validators/semantic_validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Copyright © LFV
 
 import logging
 import re
 from typing import List
 
 from colorama import Fore, Style
+from reqstool_python_decorators.decorators.decorators import Requirements
 from tabulate import tabulate
 
 import reqstool.common.utils as utils
 from reqstool.common.dataclasses.urn_id import UrnId
 from reqstool.common.validator_error_holder import ValidationError, ValidationErrorHolder
 from reqstool.models.imports import ImportDataInterface
 from reqstool.models.raw_datasets import CombinedRawDataset
@@ -66,14 +67,15 @@
 
         title = f"\n\nVALIDATION: {validation_result}"
         table = tabulate(tablefmt="fancy_grid", tabular_data=table_data)
         table_with_title = f"{title}\n{table}\n"
 
         logging.info(table_with_title)
 
+    @Requirements("REQ_022")
     def _validate_no_duplicate_requirement_ids(self, data: RequirementData) -> bool:
         # if there are no requirements or systems defined, add a validation error
         if "requirements" not in data and "systems" not in data:
             urn = data["metadata"]["urn"]
             self._validation_error_holder.add_error(ValidationError(msg=f"No requirements found for (urn: {urn})!"))
         # only look for duplicates if requirements exists
         elif "requirements" in data:
@@ -88,14 +90,15 @@
                         ValidationError(
                             msg=f"REQ {req_id} (urn: {urn}) has already been parsed. Value will not be updated."
                         )
                     )
 
         return self._validation_error_holder.get_no_of_errors() > 0
 
+    @Requirements("REQ_023")
     def _validate_no_duplicate_svc_ids(self, data: SVCData) -> bool:
         if "cases" not in data:
             self._validation_error_holder.add_error(ValidationError(msg="No svc cases found!"))
         else:
             all_svcs = set()
             for case in data["cases"]:
                 svc_id = case["id"]
@@ -108,14 +111,15 @@
                             The svc relates to {case['requirement_ids']}
                             """
                         )
                     )
 
         return self._validation_error_holder.get_no_of_errors() > 0
 
+    @Requirements("REQ_024")
     def _validate_svc_refers_to_existing_requirement_ids(
         self,  # NOSONAR
         combined_raw_dataset: CombinedRawDataset,
     ) -> List[ValidationError]:
         errors: List[ValidationError] = []
 
         # get urn and model
@@ -136,14 +140,15 @@
                                     non-existing requirement id: {self.prettify_urn_id(urn_req_id)}
                                     """
                                 )
                             )
 
         return errors
 
+    @Requirements("REQ_024")
     def _validate_annotation_impls_refers_to_existing_requirement_ids(
         self,
         combined_raw_dataset: CombinedRawDataset,
     ) -> List[ValidationError]:
         errors: List[ValidationError] = []
         for model, model_data in combined_raw_dataset.raw_datasets.items():
             # Continue if model is not inital_urn
@@ -163,14 +168,15 @@
                             non-existing requirement id: {self.prettify_urn_id(requirement_id)}
                             """
                         )
                     )
 
         return errors
 
+    @Requirements("REQ_025")
     def _validate_annotation_tests_refers_to_existing_svc_ids(
         self,
         combined_raw_dataset: CombinedRawDataset,
     ) -> List[ValidationError]:
         errors: List[ValidationError] = []
         for model, model_data in combined_raw_dataset.raw_datasets.items():
             # Continue if no annotations data
@@ -180,14 +186,15 @@
                 if not self._svc_id_exists(svc_id, combined_raw_dataset=combined_raw_dataset):
                     errors.append(
                         ValidationError(msg=f"Annotation refers to non-existing svc id: {self.prettify_urn_id(svc_id)}")
                     )
 
         return errors
 
+    @Requirements("REQ_025")
     def _validate_mvr_refers_to_existing_svc_ids(
         self, combined_raw_dataset: CombinedRawDataset
     ) -> List[ValidationError]:
         errors: List[ValidationError] = []
         for model, model_data in combined_raw_dataset.raw_datasets.items():
             # Continue if model is not inital_urn
             if model is not combined_raw_dataset.initial_model_urn or not model_data.mvrs_data:
```

### Comparing `reqstool-0.4.1/src/reqstool/common/validators/syntax_validator.py` & `reqstool-0.4.2/src/reqstool/common/validators/syntax_validator.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import logging
 from dataclasses import dataclass, field
 from enum import Enum, unique
 from importlib.resources import files
 
 from jsonschema import Draft202012Validator
 from referencing import Registry, Resource
+from reqstool_python_decorators.decorators.decorators import Requirements
 
 import reqstool.resources.schemas.v1
 
 
 @dataclass
 class JsonSchemaItem:
     short_uri: str
@@ -36,14 +37,15 @@
 
 class SyntaxValidator:
     registry = Registry()
     resource = Resource.from_contents(JsonSchemaTypes.COMMON.value.schema)
     registry = resource @ registry
     registry = registry.with_resource(uri="common.schema.json", resource=resource)
 
+    @Requirements("REQ_012", "REQ_021")
     @staticmethod
     def is_valid_data(json_schema_type: JsonSchemaTypes, data: dict, urn: str) -> bool:
         jsonvalidator_draft202012 = Draft202012Validator(
             schema=json_schema_type.value.schema,
             registry=SyntaxValidator.registry,
             format_checker=Draft202012Validator.FORMAT_CHECKER,
         )
```

### Comparing `reqstool-0.4.1/src/reqstool/expression_languages/generic_el.py` & `reqstool-0.4.2/src/reqstool/expression_languages/generic_el.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/src/reqstool/filters/id_filters.py` & `reqstool-0.4.2/src/reqstool/filters/id_filters.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/src/reqstool/location_resolver/location_resolver.py` & `reqstool-0.4.2/src/reqstool/location_resolver/location_resolver.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/src/reqstool/locations/git_location.py` & `reqstool-0.4.2/src/reqstool/locations/git_location.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # Copyright © LFV
 
-from dataclasses import dataclass
 import logging
 import os
+from dataclasses import dataclass
 
-from reqstool.locations.location import LocationInterface
+from pygit2 import RemoteCallbacks, UserPass, clone_repository
+from reqstool_python_decorators.decorators.decorators import Requirements
 
-from pygit2 import clone_repository, UserPass, RemoteCallbacks
+from reqstool.locations.location import LocationInterface
 
 
+@Requirements("REQ_002")
 @dataclass(kw_only=True)
 class GitLocation(LocationInterface):
     url: str
     branch: str
     env_token: str
 
     def _make_available_on_localdisk(self, dst_path: str):
```

### Comparing `reqstool-0.4.1/src/reqstool/locations/local_location.py` & `reqstool-0.4.2/src/reqstool/locations/local_location.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 # Copyright © LFV
 
-from dataclasses import dataclass
 import os
+from dataclasses import dataclass
+
+from reqstool_python_decorators.decorators.decorators import Requirements
 
 from reqstool.locations.location import LocationInterface
 
 
+@Requirements("REQ_001")
 @dataclass
 class LocalLocation(LocationInterface):
     def _make_available_on_localdisk(self, dst_path: str):
         # dst_directory already exists but should a symlimk, remove
         os.rmdir(dst_path)
 
         src_path = os.path.abspath(self.path)
```

### Comparing `reqstool-0.4.1/src/reqstool/locations/maven_location.py` & `reqstool-0.4.2/src/reqstool/locations/maven_location.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 # Copyright © LFV
 
 import logging
 import os
-from dataclasses import dataclass
 import sys
+from dataclasses import dataclass
 from zipfile import ZipFile
-from reqstool.locations.location import LocationInterface
+
 from maven_artifact import Artifact, Downloader, RequestException, Utils
+from reqstool_python_decorators.decorators.decorators import Requirements
+
+from reqstool.locations.location import LocationInterface
 
 
+@Requirements("REQ_003", "REQ_017")
 @dataclass(kw_only=True)
 class MavenLocation(LocationInterface):
     url: str
     group_id: str
     artifact_id: str
     version: str
     classifier: str = "requirements"
```

### Comparing `reqstool-0.4.1/src/reqstool/model_generators/annotations_model_generator.py` & `reqstool-0.4.2/src/reqstool/model_generators/annotations_model_generator.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/src/reqstool/model_generators/combined_indexed_dataset_generator.py` & `reqstool-0.4.2/src/reqstool/model_generators/combined_indexed_dataset_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Copyright © LFV
 
 import logging
 from dataclasses import dataclass, field, replace
 from typing import Dict, List, Set, Tuple
 
+from reqstool_python_decorators.decorators.decorators import Requirements
+
 from reqstool.common.dataclasses.urn_id import UrnId
 from reqstool.common.utils import append_data_item_to_dict_list_entry, create_accessible_nodes_dict
 from reqstool.expression_languages.requirements_el import RequirementsELTransformer
 from reqstool.expression_languages.svcs_el import SVCsELTransformer
 from reqstool.filters.id_filters import IDFilters
 from reqstool.filters.requirements_filters import RequirementFilter
 from reqstool.filters.svcs_filters import SVCFilter
@@ -290,14 +292,15 @@
 
         return test_data
 
     def __process_filters(self):
         self.__process_req_filters()
         self.__process_svc_filters()
 
+    @Requirements("REQ_018")
     def __process_req_filters(self):
         logging.debug(f"Starting filtering of requirements from {self._crd.initial_model_urn}")
 
         kept_requirements, filtered_out_reqs = self.__process_req_filters_per_urn(self._crd.initial_model_urn)
 
         # use dict comphrehension to find requirements to be removed
         filtered_out_reqs: List(UrnId) = [
@@ -379,14 +382,15 @@
         filtered_out_reqs.update(filtered_out_reqs_imports)
         logging.debug(f"Total filtered out {len(filtered_out_reqs)} requirements URN {urn} : {filtered_out_reqs}")
 
         self._visited_urns_during_filtering.append(urn)
 
         return kept_requirements, filtered_out_reqs
 
+    @Requirements("REQ_020")
     def __get_filtered_out_requirements_for_filter_urn(  # noqa C901 # NOSONAR
         self, accessible_requirements: set[UrnId], urn: str, req_filter: RequirementFilter
     ) -> List[UrnId]:
         logging.debug(f"Applying filter for urn {urn} on {len(accessible_requirements)} accessible reqs: {req_filter}")
 
         filtered_out_requirements: List[UrnId] = []
 
@@ -439,14 +443,15 @@
                 logging.debug(f"Filtering in requirement: {req_urn_id}")
             else:
                 logging.debug(f"Filtering OUT requirement: {req_urn_id}")
                 filtered_out_requirements.append(req_urn_id)
 
         return filtered_out_requirements
 
+    @Requirements("REQ_019")
     def __process_svc_filters(self):
         logging.debug(f"Starting filtering of svcs from {self._crd.initial_model_urn}")
 
         kept_svs, filtered_out_svcs = self.__process_svc_filters_per_urn(self._crd.initial_model_urn)
 
         logging.debug(f"Deleting {len(filtered_out_svcs)} svcs")
         logging.debug(f"Deleting svcs: {filtered_out_svcs}")
@@ -512,14 +517,15 @@
         logging.debug(f"URN {urn} filtered out {len(filtered_out_svcs)} svcs: {filtered_out_svcs}")
 
         filtered_out_svcs.update(filtered_out_svcs_imports)
         logging.debug(f"Total filtered out {len(filtered_out_svcs)} svcs URN {urn} : {filtered_out_svcs}")
 
         return kept_svcs, filtered_out_svcs
 
+    @Requirements("REQ_020")
     def __get_filtered_out_svcs_for_filter_urn(  # noqa C901 # NOSONAR
         self, accessible_svcs: set[UrnId], urn: str, svc_filter: SVCFilter
     ) -> List[UrnId]:
         logging.debug(f"Applying filter for urn {urn} on {len(accessible_svcs)} accessible svcs: {svc_filter}")
 
         filtered_out_svcs: List[UrnId] = []
```

### Comparing `reqstool-0.4.1/src/reqstool/model_generators/combined_raw_datasets_generator.py` & `reqstool-0.4.2/src/reqstool/model_generators/combined_raw_datasets_generator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Copyright © LFV
 
 import logging
 import sys
 from typing import Dict, List
 
+from reqstool_python_decorators.decorators.decorators import Requirements
+
 from reqstool.common import utils
 from reqstool.common.utils import TempDirectoryUtil
 from reqstool.common.validators.semantic_validator import SemanticValidator
 from reqstool.location_resolver.location_resolver import LocationResolver
 from reqstool.locations.location import LocationInterface
 from reqstool.model_generators.annotations_model_generator import AnnotationsModelGenerator
 from reqstool.model_generators.mvrs_model_generator import MVRsModelGenerator
@@ -20,14 +22,15 @@
 from reqstool.models.raw_datasets import CombinedRawDataset, RawDataset
 from reqstool.models.requirements import VARIANTS, RequirementsData
 from reqstool.models.svcs import SVCsData
 from reqstool.models.test_data import TestsData
 from reqstool.requirements_indata.requirements_indata import RequirementsIndata
 
 
+@Requirements("REQ_005", "REQ_006", "REQ_007")
 class CombinedRawDatasetsGenerator:
     def __init__(self, initial_location: LocationInterface, semantic_validator: SemanticValidator):
         self.__level: int = 0
         self.__initial_source_type: VARIANTS = None
         self.__initial_location_handler: LocationResolver = LocationResolver(
             parent=None, _current_unresolved=initial_location
         )
@@ -146,14 +149,15 @@
 
             raw_datasets[current_urn] = parsed_model
 
         self.__level += 1
 
         return parsed_urns
 
+    @Requirements("REQ_008", "REQ_026")
     def __parse_source(self, current_location_handler: LocationResolver) -> RawDataset:
         annotations_data = None
         svcs_data = None
         mvrs_data = None
         automated_tests = None
 
         tmp_path = TempDirectoryUtil.get_suffix_path("can_we_use_urn_here").absolute()
@@ -197,14 +201,15 @@
             svcs_data=svcs_data,
             mvrs_data=mvrs_data,
             automated_tests=automated_tests,
         )
 
         return raw_dataset
 
+    @Requirements("REQ_009", "REQ_010", "REQ_013")
     def __parse_source_other(self, requirements_indata: RequirementsIndata, rmg: RequirementsModelGenerator):
         annotations_data: AnnotationsData = None
         svcs_data: SVCsData = None
         mvrs_data: MVRsData = None
         automated_tests: TestsData = None
         tests = {}
         # get current urn
@@ -215,27 +220,20 @@
                 uri=requirements_indata.requirements_indata_paths.svcs_yml.path,
                 semantic_validator=self.semantic_validator,
                 urn=current_urn,
             ).model
 
         # handle automated test results
 
-        if requirements_indata.requirements_indata_paths.test_results_failsafe_dir.exists:
-            automated_tests_failsafe = TestDataModelGenerator(
-                path=requirements_indata.requirements_indata_paths.test_results_failsafe_dir.path, urn=current_urn
-            ).model
-
-            tests |= automated_tests_failsafe.tests
+        for test_results_dir in requirements_indata.requirements_indata_paths.test_results_dirs:
 
-        if requirements_indata.requirements_indata_paths.test_results_surefire_dir.exists:
-            automated_tests_surefire = TestDataModelGenerator(
-                path=requirements_indata.requirements_indata_paths.test_results_surefire_dir.path, urn=current_urn
-            ).model
+            if test_results_dir.exists:
+                automated_tests_results = TestDataModelGenerator(path=test_results_dir.path, urn=current_urn).model
 
-            tests |= automated_tests_surefire.tests
+                tests |= automated_tests_results.tests
 
         automated_tests = TestsData(tests=tests)
 
         # handle manual verification results
 
         if requirements_indata.requirements_indata_paths.mvrs_yml.exists:
             mvrs_data = MVRsModelGenerator(
```

### Comparing `reqstool-0.4.1/src/reqstool/model_generators/mvrs_model_generator.py` & `reqstool-0.4.2/src/reqstool/model_generators/mvrs_model_generator.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/src/reqstool/model_generators/requirements_model_generator.py` & `reqstool-0.4.2/src/reqstool/model_generators/requirements_model_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Copyright © LFV
 
 import re
 import sys
 from typing import Dict, List, Set
 
 from packaging.version import InvalidVersion, Version
+from reqstool_python_decorators.decorators.decorators import Requirements
 from ruamel.yaml import YAML
 
 from reqstool.commands.exit_codes import EXIT_CODE_SYNTAX_VALIDATION_ERROR
 from reqstool.common import utils
 from reqstool.common.dataclasses.urn_id import UrnId
 from reqstool.common.validators.semantic_validator import SemanticValidator
 from reqstool.common.validators.syntax_validator import JsonSchemaTypes, SyntaxValidator
@@ -270,14 +271,15 @@
                     custom_exclude=custom_exclude,
                 )
 
                 r_filters[urn] = req_filter
 
         return r_filters
 
+    @Requirements("REQ_004")
     def __parse_requirements(self, data):  # NOSONAR
         r_reqs = {}
 
         self.semantic_validator._validate_no_duplicate_requirement_ids(data=data)
 
         if "requirements" in data:
             for req in data["requirements"]:
```

### Comparing `reqstool-0.4.1/src/reqstool/model_generators/svcs_model_generator.py` & `reqstool-0.4.2/src/reqstool/model_generators/svcs_model_generator.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/src/reqstool/model_generators/testdata_model_generator.py` & `reqstool-0.4.2/src/reqstool/model_generators/testdata_model_generator.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 import logging
 import re
 import xml.etree.ElementTree as ET
 from pathlib import Path
 from typing import Dict
 
+from reqstool_python_decorators.decorators.decorators import Requirements
+
 from reqstool.common.dataclasses.urn_id import UrnId
 from reqstool.models.test_data import TestData, TestRunStatus, TestsData
 
 
 class TestDataModelGenerator:
     UNIT_METHOD_IDENTIFIER_REGEX = r"^([a-zA-Z_$][a-zA-Z0-9_$]*).*$"
     KARATE_METHOD_IDENTIFIER_REGEX = r"\[\d+(?:\.\d+)?:\d+\]\s*(.+)"
@@ -21,24 +23,25 @@
         self.model: Dict[UrnId, TestData] = self.__generate(path, urn)
 
     def __generate(self, path: str, urn: str) -> TestsData:
         tests = self.__parse_test_data(path, urn)
 
         return TestsData(tests=tests)
 
+    @Requirements("REQ_014", "REQ_015")
     def __parse_test_data(self, path: str, urn: str) -> Dict[str, TestData]:
         r_testdata: Dict[str, TestData] = {}
 
-        xml_files = list(Path(path).glob("*.xml"))
+        xml_files = list(Path(path).glob("**/*.xml"))
 
         for xml_file in xml_files:
             tree = ET.parse(xml_file)
             root = tree.getroot()
 
-            for testcase in root.findall("./testcase"):
+            for testcase in root.findall(".//testcase"):
                 # Check if there is a match
                 match_unit = re.match(self.UNIT_METHOD_IDENTIFIER_REGEX, testcase.attrib["name"])
                 match_karate = re.match(self.KARATE_METHOD_IDENTIFIER_REGEX, testcase.attrib["name"])
 
                 if match_unit:
                     methodname = match_unit.group(1)
                 elif match_karate:
```

### Comparing `reqstool-0.4.1/src/reqstool/models/combined_indexed_dataset.py` & `reqstool-0.4.2/src/reqstool/models/combined_indexed_dataset.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/src/reqstool/models/raw_datasets.py` & `reqstool-0.4.2/src/reqstool/models/raw_datasets.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/src/reqstool/models/requirements.py` & `reqstool-0.4.2/src/reqstool/models/requirements.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,22 +36,23 @@
         if self.__class__ is other.__class__:
             return self._member_names_.index(self.name) < other._member_names_.index(other.name)
         return NotImplemented
 
 
 @unique
 class CATEGORIES(Enum):
-    COMPATIBILITY = "compatibility"
     FUNCTIONAL_SUITABILITY = "functional-suitability"
-    MAINTAINABILITY = "maintainability"
     PERFORMANCE_EFFICIENCY = "performance-efficiency"
-    PORTABILITY = "portability"
+    COMPATIBILITY = "compatibility"
+    INTERACTION_CAPABILITY = "interaction-capability"
     RELIABILITY = "reliability"
     SECURITY = "security"
-    USABILITY = "usability"
+    MAINTAINABILITY = "maintainability"
+    FLEXIBILITY = "flexibility"
+    SAFETY = "safety"
 
 
 @dataclass
 class ReferenceData:
     requirement_ids: Set[UrnId] = set[UrnId]
```

### Comparing `reqstool-0.4.1/src/reqstool/models/svcs.py` & `reqstool-0.4.2/src/reqstool/models/svcs.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/src/reqstool/reqstool_config/reqstool_config.py` & `reqstool-0.4.2/src/reqstool/reqstool_config/reqstool_config.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,24 @@
 # Copyright © LFV
 
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from enum import Enum, unique
-from typing import Optional
+from typing import List, Optional
 
 
 @unique
 class TYPES(Enum):
     DEFAULT = "default"
     JAVA_MAVEN = "java-maven"
-
-
-@dataclass
-class TestResults:
-    failsafe: Optional[str] = None
-    surefire: Optional[str] = None
+    PYTHON = "python"
 
 
 @dataclass
 class Locations:
-    test_results: TestResults
+    test_results: List[str] = field(default_factory=lambda: [])
     annotations: Optional[str] = None
 
 
 @dataclass
 class ReqstoolConfig:
     project_root_dir: str
     type: TYPES
@@ -31,29 +26,22 @@
 
     @staticmethod
     def _parse(yaml_data: dict) -> "ReqstoolConfig":
         r_type = TYPES(yaml_data["type"])
 
         r_project_root_dir = "." if "project_root_dir" not in yaml_data else yaml_data["project_root_dir"]
 
-        r_locations = Locations(annotations=None, test_results=TestResults())
-
-        if "locations" not in yaml_data:
-            return ReqstoolConfig(type=r_type, project_root_dir=r_project_root_dir, locations=r_locations)
-
-        locations = yaml_data["locations"]
+        r_locations = Locations(annotations=None, test_results=[])
 
-        if "annotations" in locations:
-            annotations = locations["annotations"]
+        if "locations" in yaml_data:
 
-            r_locations.annotations = annotations
+            locations = yaml_data["locations"]
 
-        if "test_results" in locations:
-            test_results = locations["test_results"]
+            if "annotations" in locations:
+                annotations = locations["annotations"]
 
-            if "failsafe" in test_results:
-                r_locations.test_results.failsafe = test_results["failsafe"]
+                r_locations.annotations = annotations
 
-            if "surefire" in test_results:
-                r_locations.test_results.surefire = test_results["surefire"]
+            if "test_results_dirs" in locations:
+                r_locations.test_results = locations["test_results_dirs"]
 
         return ReqstoolConfig(type=r_type, project_root_dir=r_project_root_dir, locations=r_locations)
```

### Comparing `reqstool-0.4.1/src/reqstool/requirements_indata/requirements_indata.py` & `reqstool-0.4.2/src/reqstool/requirements_indata/requirements_indata.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,43 @@
 # Copyright © LFV
 
 import os
 import sys
+from collections.abc import Sequence
 from dataclasses import dataclass, field, fields
+from typing import List, Union
 
+from reqstool_python_decorators.decorators.decorators import Requirements
 from ruamel.yaml import YAML
 
 from reqstool.commands.exit_codes import EXIT_CODE_SYNTAX_VALIDATION_ERROR
 from reqstool.common.utils import open_file_https_file
 from reqstool.common.validators.syntax_validator import JsonSchemaTypes, SyntaxValidator
 from reqstool.locations.git_location import GitLocation
 from reqstool.locations.local_location import LocalLocation
 from reqstool.locations.location import LocationInterface
 from reqstool.locations.maven_location import MavenLocation
 from reqstool.reqstool_config.reqstool_config import TYPES, ReqstoolConfig
-from reqstool.requirements_indata.java.java_maven_requirements_indata_paths import (
-    JavaMavenRequirementsIndataPaths,
-    RequirementsIndataPathItem,
-)
-from reqstool.requirements_indata.requirements_indata_paths import (
-    RequirementsIndataPaths,
-    RequirementsIndataStructureItem,
-)
+from reqstool.requirements_indata.java.java_maven_requirements_indata_paths import JavaMavenRequirementsIndataPaths
+from reqstool.requirements_indata.python.python_requirements_indata_paths import PythonRequirementsIndataPaths
+from reqstool.requirements_indata.requirements_indata_paths import RequirementsIndataPathItem, RequirementsIndataPaths
 
 
 @dataclass(kw_only=True)
 class RequirementsIndata:
     dst_path: str  # tmp path
     location: LocationInterface  # current location
-    reqstool_config: ReqstoolConfig = field(default=None)
+    reqstool_config: ReqstoolConfig = field(init=False, default=None)
     requirements_indata_paths: RequirementsIndataPaths = field(default_factory=RequirementsIndataPaths)
 
     def __post_init__(self):
         self._handle_requirements_config()
-        self._ensure_absolute_paths()
-        self._check_what_indata_that_exists()
+        self._ensure_absolute_paths_and_check_existance()
 
+    @Requirements("REQ_011")
     def _handle_requirements_config(self):
 
         if os.path.exists(os.path.join(self.dst_path, "reqstool_config.yml")):
             response = open_file_https_file(os.path.join(self.dst_path, "reqstool_config.yml"))
 
             yaml = YAML(typ="safe")
 
@@ -51,65 +49,76 @@
                 sys.exit(EXIT_CODE_SYNTAX_VALIDATION_ERROR)
 
             self.reqstool_config = ReqstoolConfig._parse(yaml_data=data)
 
             match self.reqstool_config.type:
                 case TYPES.JAVA_MAVEN:
                     self.requirements_indata_paths = JavaMavenRequirementsIndataPaths()
+                case TYPES.PYTHON:
+                    self.requirements_indata_paths = PythonRequirementsIndataPaths()
 
             self._handle_custom()
 
             if self.reqstool_config.project_root_dir is not None:
                 self.requirements_indata_paths.prepend_paths(self.reqstool_config.project_root_dir)
 
-    def _ensure_absolute_paths(self):
+    def _ensure_absolute_paths_and_check_existance(self):
         # iterate over all fields and ensure absolute paths
 
         for f in fields(self.requirements_indata_paths):
             field_name = f.name
-            original_item: RequirementsIndataPathItem = getattr(self.requirements_indata_paths, field_name)
-            transformed_value = None
+            original: Union[RequirementsIndataPathItem, List[RequirementsIndataPathItem]] = getattr(
+                self.requirements_indata_paths, field_name
+            )
 
             if isinstance(self.location, GitLocation):
                 # Include self.location.path when resolving a git repository
-                transformed_value = os.path.abspath(os.path.join(self.dst_path, self.location.path, original_item.path))
+                RequirementsIndata._ensure_absolute_path_and_check_existance(
+                    paths=[self.dst_path, self.location.path], original=original
+                )
             elif isinstance(self.location, MavenLocation):
                 # Include self.location.path when resolving a git repository
-                transformed_value = os.path.abspath(os.path.join(self.dst_path, self.location.path, original_item.path))
+                RequirementsIndata._ensure_absolute_path_and_check_existance(
+                    paths=[self.dst_path, self.location.path], original=original
+                )
             elif isinstance(self.location, LocalLocation):
                 # resolve soft link
                 abs_dst_path = os.readlink(self.dst_path)
-                transformed_value = os.path.abspath(os.path.join(abs_dst_path, original_item.path))
+                RequirementsIndata._ensure_absolute_path_and_check_existance(paths=[abs_dst_path], original=original)
             else:
                 raise TypeError
 
-            original_item.path = transformed_value
-
-    def _check_what_indata_that_exists(self):
-        # iterate over all fields and check for existance
-
-        for f in fields(self.requirements_indata_paths):
-            field_name = f.name
-            original_item: RequirementsIndataPathItem = getattr(self.requirements_indata_paths, field_name)
-            original_item.exists = os.path.exists(original_item.path)
+    def _ensure_absolute_path_and_check_existance(
+        paths: List[str], original: Union[RequirementsIndataPathItem, List[RequirementsIndataPathItem]]
+    ):
+
+        if isinstance(original, RequirementsIndataPathItem):
+            new_abs_path = os.path.abspath(os.path.join(*paths, original.path))
+            original.path = new_abs_path
+            original.exists = os.path.exists(original.path)
+
+        elif isinstance(original, Sequence):
+            for item in original:
+                new_abs_path = os.path.abspath(os.path.join(*paths, item.path))
+                item.path = new_abs_path
+                item.exists = os.path.exists(item.path)
+        else:
+            raise TypeError(type(original))
 
     def _handle_custom(self):
         # replace default values with custom if specified
 
         if self.reqstool_config.locations:
             test_results = self.reqstool_config.locations.test_results
 
-            if test_results:
-                if test_results.failsafe:
-                    self.requirements_indata_paths.test_results_failsafe_dir = RequirementsIndataStructureItem(
-                        path=test_results.failsafe
-                    )
-
-                if test_results.surefire:
-                    self.requirements_indata_paths.test_results_surefire_dir = RequirementsIndataStructureItem(
-                        path=test_results.surefire
-                    )
+            if isinstance(test_results, Sequence):
+                r_test_results = []
+
+                for test_result_dir in test_results:
+                    r_test_results.append(RequirementsIndataPathItem(path=test_result_dir))
+
+                self.requirements_indata_paths.test_results_dirs = r_test_results
 
             if self.reqstool_config.locations.annotations:
-                self.requirements_indata_paths.annotations_yml = RequirementsIndataStructureItem(
+                self.requirements_indata_paths.annotations_yml = RequirementsIndataPathItem(
                     path=self.reqstool_config.locations.annotations
                 )
```

### Comparing `reqstool-0.4.1/src/reqstool/requirements_indata/requirements_indata_paths.py` & `reqstool-0.4.2/src/reqstool/requirements_indata/requirements_indata_paths.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,50 @@
 # Copyright © LFV
 
 from dataclasses import dataclass, field
 from pathlib import PurePath
+from typing import List
+
+from reqstool_python_decorators.decorators.decorators import Requirements
 
 
 @dataclass(kw_only=True)
-class RequirementsIndataStructureItem:
+class RequirementsIndataPathItem:
     path: str
     exists: bool = False
 
 
+@Requirements("REQ_016")
 @dataclass(kw_only=True)
 class RequirementsIndataPaths:
     # static
-    requirements_yml: RequirementsIndataStructureItem = field(
-        default_factory=lambda: RequirementsIndataStructureItem(path="requirements.yml")
+    requirements_yml: RequirementsIndataPathItem = field(
+        default_factory=lambda: RequirementsIndataPathItem(path="requirements.yml")
     )
 
-    svcs_yml: RequirementsIndataStructureItem = field(
-        default_factory=lambda: RequirementsIndataStructureItem(path="software_verification_cases.yml")
+    svcs_yml: RequirementsIndataPathItem = field(
+        default_factory=lambda: RequirementsIndataPathItem(path="software_verification_cases.yml")
     )
-    mvrs_yml: RequirementsIndataStructureItem = field(
-        default_factory=lambda: RequirementsIndataStructureItem(path="manual_verification_results.yml")
+    mvrs_yml: RequirementsIndataPathItem = field(
+        default_factory=lambda: RequirementsIndataPathItem(path="manual_verification_results.yml")
     )
 
     # dynamic
-    annotations_yml: RequirementsIndataStructureItem = field(
-        default_factory=lambda: RequirementsIndataStructureItem(path="annotations.yml")
-    )
-    test_results_failsafe_dir: RequirementsIndataStructureItem = field(
-        default_factory=lambda: RequirementsIndataStructureItem(path="test_results/failsafe")
+    annotations_yml: RequirementsIndataPathItem = field(
+        default_factory=lambda: RequirementsIndataPathItem(path="annotations.yml")
     )
-    test_results_surefire_dir: RequirementsIndataStructureItem = field(
-        default_factory=lambda: RequirementsIndataStructureItem(path="test_results/surefire")
+    test_results_dirs: List[RequirementsIndataPathItem] = field(
+        default_factory=lambda: [RequirementsIndataPathItem(path="test_results")]
     )
 
     def prepend_paths(self, prepend_dir):
         for prop in dir(self):
             if (
                 not prop.startswith("__")
-                and isinstance(getattr(self, prop), RequirementsIndataStructureItem)
+                and isinstance(getattr(self, prop), RequirementsIndataPathItem)
                 and prop not in ["requirements_yml", "svcs_yml", "mvrs_yml"]
             ):
                 path_item = getattr(self, prop)
                 if path_item.path is not None:
                     path_item.path = str(PurePath(prepend_dir, path_item.path))
 
     # other has precedence
```

### Comparing `reqstool-0.4.1/src/reqstool/resources/schemas/v1/annotations.schema.json` & `reqstool-0.4.2/src/reqstool/resources/schemas/v1/annotations.schema.json`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/src/reqstool/resources/schemas/v1/common.schema.json` & `reqstool-0.4.2/src/reqstool/resources/schemas/v1/common.schema.json`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/src/reqstool/resources/schemas/v1/manual_verification_results.schema.json` & `reqstool-0.4.2/src/reqstool/resources/schemas/v1/manual_verification_results.schema.json`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/src/reqstool/resources/schemas/v1/reqstool_config.schema.json` & `reqstool-0.4.2/src/reqstool/resources/schemas/v1/reqstool_config.schema.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9991319444444444%*

 * *Differences: {"'properties'": "{'locations': {'properties': {'test_results_dirs': OrderedDict([('type', "*

 * *                 "'array'), ('items', OrderedDict([('type', 'string'), ('description', 'Path to "*

 * *                 "test result directory')])), ('additionalProperties', False), ('description', "*

 * *                 "'Paths to test results directories')]), delete: ['test_results']}}}"}*

```diff
@@ -8,28 +8,22 @@
             "additionalProperties": false,
             "description": "Locations for test results and annotations",
             "properties": {
                 "annotations": {
                     "description": "Path to annotations file",
                     "type": "string"
                 },
-                "test_results": {
+                "test_results_dirs": {
                     "additionalProperties": false,
                     "description": "Paths to test results directories",
-                    "properties": {
-                        "failsafe": {
-                            "description": "Path to Failsafe test results",
-                            "type": "string"
-                        },
-                        "surefire": {
-                            "description": "Path to Surefire test results",
-                            "type": "string"
-                        }
+                    "items": {
+                        "description": "Path to test result directory",
+                        "type": "string"
                     },
-                    "type": "object"
+                    "type": "array"
                 }
             },
             "type": "object"
         },
         "project_root_dir": {
             "description": "Path to project root dir (e.g. where pom.xml, pyproject.toml are) (default: \"./\")",
             "type": "string"
```

### Comparing `reqstool-0.4.1/src/reqstool/resources/schemas/v1/requirements.schema.json` & `reqstool-0.4.2/src/reqstool/resources/schemas/v1/requirements.schema.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999925475999695%*

 * *Differences: {"'$defs'": "{'requirements': {'properties': {'categories': {'items': {'enum': {insert: [(2, "*

 * *            "'compatibility'), (3, 'interaction-capability'), (6, 'maintainability'), (7, "*

 * *            "'flexibility'), (8, 'safety')], delete: [7, 4, 2, 0]}, 'description': 'Enum for "*

 * *            'requirement categories. E.g. functional-suitability, performance-efficiency, '*

 * *            "security, reliability, maintainability'}, 'description': 'Array of requirement "*

 * *            'categories. E.g. functional-sui […]*

```diff
@@ -143,26 +143,27 @@
             ],
             "type": "object"
         },
         "requirements": {
             "additionalProperties": false,
             "properties": {
                 "categories": {
-                    "description": "Array of requirement categories. E.g. functional-suitability, usability, performance-efficiency, security, reliability, maintainability",
+                    "description": "Array of requirement categories. E.g. functional-suitability, performance-efficiency, security, reliability, maintainability",
                     "items": {
-                        "description": "Enum for requirement categories. E.g. functional-suitability, usability, performance-efficiency, security, reliability, maintainability",
+                        "description": "Enum for requirement categories. E.g. functional-suitability, performance-efficiency, security, reliability, maintainability",
                         "enum": [
-                            "compatibility",
                             "functional-suitability",
-                            "maintainability",
                             "performance-efficiency",
-                            "portability",
+                            "compatibility",
+                            "interaction-capability",
                             "reliability",
                             "security",
-                            "usability"
+                            "maintainability",
+                            "flexibility",
+                            "safety"
                         ],
                         "type": "string"
                     },
                     "type": "array"
                 },
                 "description": {
                     "description": "High level description for the requirement",
```

### Comparing `reqstool-0.4.1/src/reqstool/resources/schemas/v1/software_verification_cases.schema.json` & `reqstool-0.4.2/src/reqstool/resources/schemas/v1/software_verification_cases.schema.json`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/tests/integration/reqstool/model_generators/test_included_models_generator.py` & `reqstool-0.4.2/tests/integration/reqstool/model_generators/test_included_models_generator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright © LFV
 
 import os
 
 import pytest
+from reqstool_python_decorators.decorators.decorators import SVCs
 
 from reqstool.common.validator_error_holder import ValidationErrorHolder
 from reqstool.common.validators.semantic_validator import SemanticValidator
 from reqstool.locations.git_location import GitLocation
 from reqstool.locations.maven_location import MavenLocation
 from reqstool.model_generators import combined_raw_datasets_generator
 
@@ -14,14 +15,15 @@
 def choose_token() -> str:
     if os.getenv("GITHUB_TOKEN"):
         return "GITHUB_TOKEN"
     else:
         return "GITLAB_TOKEN"
 
 
+@SVCs("SVC_002")
 @pytest.mark.skipif(
     not (os.getenv("GITHUB_TOKEN") or os.getenv("GITLAB_TOKEN")),
     reason="Test needs GITLAB_TOKEN or GITLAB environment variable to be set",
 )
 def test_basic_git():
     semantic_validator = SemanticValidator(validation_error_holder=ValidationErrorHolder())
 
@@ -32,14 +34,15 @@
             path="tests/resources/test_data/data/remote/test_standard/test_standard_maven_git/ms-001",
             branch="main",
         ),
         semantic_validator=semantic_validator,
     )
 
 
+@SVCs("SVC_003", "SVC_008")
 @pytest.mark.skipif(
     not (os.getenv("GITHUB_TOKEN") or os.getenv("GITLAB_TOKEN")),
     reason="Test needs GITLAB_TOKEN or GITHUB_TOKEN environment variable to be set",
 )
 def test_basic_maven():
     semantic_validator = SemanticValidator(validation_error_holder=ValidationErrorHolder())
```

### Comparing `reqstool-0.4.1/tests/resources/test_data/data/local/test_basic/baseline/ms-101/annotations.yml` & `reqstool-0.4.2/tests/resources/test_data/data/local/test_basic/baseline/ms-101/annotations.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/tests/resources/test_data/data/local/test_basic/baseline/ms-101/requirements.yml` & `reqstool-0.4.2/tests/resources/test_data/data/local/test_errors/ms-101/requirements.yml`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     title: Title REQ_101
     significance: may
     description: Description REQ_101
     rationale: Rationale REQ_001
     categories: ["maintainability", "functional-suitability"]
     revision: 0.0.1
 
-  - id: REQ_102
+  - id: REQ_101
     title: Title REQ_102
     significance: shall
     description: Description REQ_102
     rationale: Rationale REQ_002
     categories: ["security", "maintainability"]
     revision: 0.0.1
 
@@ -34,9 +34,9 @@
     revision: 0.0.1
 
   - id: REQ_202
     title: Title REQ_202
     significance: should
     description: Description REQ_202
     rationale: Rationale REQ_201
-    categories: ["reliability", "usability"]
+    categories: ["reliability"]
     revision: 0.0.1
```

### Comparing `reqstool-0.4.1/tests/resources/test_data/data/local/test_basic/baseline/ms-101/software_verification_cases.yml` & `reqstool-0.4.2/tests/resources/test_data/data/local/test_basic/baseline/ms-101/software_verification_cases.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/tests/resources/test_data/data/local/test_basic/baseline/ms-101/test_results/failsafe/TEST-com.example.RequirementsExampleTestsIT.xml` & `reqstool-0.4.2/tests/resources/test_data/data/local/test_basic/baseline/ms-101/test_results/failsafe/TEST-com.example.RequirementsExampleTestsIT.xml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/tests/resources/test_data/data/local/test_basic/baseline/ms-101/test_results/surefire/TEST-com.example.RequirementsExampleTests.xml` & `reqstool-0.4.2/tests/resources/test_data/data/local/test_basic/baseline/ms-101/test_results/surefire/TEST-com.example.RequirementsExampleTests.xml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/tests/resources/test_data/data/local/test_basic/layout_maven/ms-101/pom.xml` & `reqstool-0.4.2/tests/resources/test_data/data/local/test_basic/layout_maven/ms-101/pom.xml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/tests/resources/test_data/data/local/test_basic/with_requirements_config/README.md` & `reqstool-0.4.2/tests/resources/test_data/data/local/test_basic/with_requirements_config/README.md`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/tests/resources/test_data/data/local/test_errors/ms-101/annotations.yml` & `reqstool-0.4.2/tests/resources/test_data/data/local/test_errors/ms-101/annotations.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/tests/resources/test_data/data/local/test_errors/ms-101/requirements.yml` & `reqstool-0.4.2/tests/resources/test_data/data/local/test_basic/baseline/ms-101/requirements.yml`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     title: Title REQ_101
     significance: may
     description: Description REQ_101
     rationale: Rationale REQ_001
     categories: ["maintainability", "functional-suitability"]
     revision: 0.0.1
 
-  - id: REQ_101
+  - id: REQ_102
     title: Title REQ_102
     significance: shall
     description: Description REQ_102
     rationale: Rationale REQ_002
     categories: ["security", "maintainability"]
     revision: 0.0.1
 
@@ -34,9 +34,9 @@
     revision: 0.0.1
 
   - id: REQ_202
     title: Title REQ_202
     significance: should
     description: Description REQ_202
     rationale: Rationale REQ_201
-    categories: ["reliability", "usability"]
+    categories: ["reliability"]
     revision: 0.0.1
```

### Comparing `reqstool-0.4.1/tests/resources/test_data/data/local/test_errors/ms-101/software_verification_cases.yml` & `reqstool-0.4.2/tests/resources/test_data/data/local/test_errors/ms-101/software_verification_cases.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/tests/resources/test_data/data/local/test_errors/ms-101/test_results/failsafe/TEST-com.example.RequirementsExampleTestsIT.xml` & `reqstool-0.4.2/tests/resources/test_data/data/local/test_errors/ms-101/test_results/failsafe/TEST-com.example.RequirementsExampleTestsIT.xml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/tests/resources/test_data/data/local/test_errors/ms-101/test_results/surefire/TEST-com.example.RequirementsExampleTests.xml` & `reqstool-0.4.2/tests/resources/test_data/data/local/test_errors/ms-101/test_results/surefire/TEST-com.example.RequirementsExampleTests.xml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/tests/resources/test_data/data/local/test_standard/baseline/visualization.adoc` & `reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/baseline/visualization.adoc`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/tests/resources/test_data/data/local/test_standard/baseline/ms-001/annotations.yml` & `reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/baseline/ms-001/annotations.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/tests/resources/test_data/data/local/test_standard/baseline/ms-001/requirements.yml` & `reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/baseline/ms-001/requirements.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/tests/resources/test_data/data/local/test_standard/baseline/ms-001/software_verification_cases.yml` & `reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/baseline/ms-001/software_verification_cases.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/tests/resources/test_data/data/local/test_standard/baseline/ms-001/test_results/failsafe/TEST-com.reqstool.example.demo.DemoApplicationTestsIT.xml` & `reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/baseline/ms-001/test_results/failsafe/TEST-com.reqstool.example.demo.DemoApplicationTestsIT.xml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/tests/resources/test_data/data/local/test_standard/baseline/ms-001/test_results/surefire/TEST-com.reqstool.example.demo.SVCsTest.xml` & `reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/baseline/ms-001/test_results/surefire/TEST-com.reqstool.example.demo.SVCsTest.xml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/tests/resources/test_data/data/local/test_standard/baseline/sys-001/requirements.yml` & `reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/baseline/sys-001/requirements.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/tests/resources/test_data/data/local/test_standard/baseline/sys-001/software_verification_cases.yml` & `reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/baseline/sys-001/software_verification_cases.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/tests/resources/test_data/data/local/test_standard/baseline/sys-001/ext-001/requirements.yml` & `reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/baseline/sys-001/ext-001/requirements.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/tests/resources/test_data/data/local/test_standard/baseline/sys-001/ext-002/requirements.yml` & `reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/baseline/sys-001/ext-002/requirements.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/tests/resources/test_data/data/local/test_standard/empty_ms/ms-001/annotations.yml` & `reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/empty_ms/ms-001/annotations.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/tests/resources/test_data/data/local/test_standard/empty_ms/ms-001/test_results/failsafe/TEST-com.reqstool.example.demo.DemoApplicationTestsIT.xml` & `reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/empty_ms/ms-001/test_results/failsafe/TEST-com.reqstool.example.demo.DemoApplicationTestsIT.xml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/tests/resources/test_data/data/local/test_standard/empty_ms/ms-001/test_results/surefire/TEST-com.reqstool.example.demo.SVCsTest.xml` & `reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/empty_ms/ms-001/test_results/surefire/TEST-com.reqstool.example.demo.SVCsTest.xml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/tests/resources/test_data/data/local/test_standard/empty_ms/sys-001/requirements.yml` & `reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/empty_ms/sys-001/requirements.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/tests/resources/test_data/data/local/test_standard/empty_ms/sys-001/software_verification_cases.yml` & `reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/empty_ms/sys-001/software_verification_cases.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/tests/resources/test_data/data/local/test_standard/empty_ms/sys-001/ext-001/requirements.yml` & `reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/empty_ms/sys-001/ext-001/requirements.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/tests/resources/test_data/data/local/test_standard/empty_ms/sys-001/ext-002/requirements.yml` & `reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/empty_ms/sys-001/ext-002/requirements.yml`

 * *Files 3% similar despite different names*

```diff
@@ -16,17 +16,17 @@
     revision: 0.0.1
 
   - id: REQ_ext002_300
     title: Title REQ_ext002_300
     significance: may
     description: Implemented requirement with SVC missing automated-test
     rationale: Rationale REQ_ext002_300
-    categories: ["usability", "performance-efficiency"]
+    categories: ["performance-efficiency"]
     revision: 0.0.1
 
   - id: REQ_ext002_400
     title: Title REQ_ext002_400
     significance: shall
     description: Implemented requirement with SVC missing MVR and one passing automated-test
     rationale: Rationale REQ_ext002_400
-    categories: ["security", "usability"]
+    categories: ["security"]
     revision: 0.0.1
```

### Comparing `reqstool-0.4.1/tests/resources/test_data/data/remote/test_standard/test_standard_maven_git/sys-001/requirements.yml` & `reqstool-0.4.2/tests/resources/test_data/data/remote/test_standard/test_standard_maven_git/sys-001/requirements.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/tests/resources/unit/reqstool/model_generators/test_annotations_model_generator/test_annotations_model_generator/annotations.yml` & `reqstool-0.4.2/tests/resources/unit/reqstool/model_generators/test_annotations_model_generator/test_annotations_model_generator/annotations.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/tests/resources/unit/reqstool/model_generators/test_requirements_model_generator/test_external_requirements_model_generator/requirements.yml` & `reqstool-0.4.2/tests/resources/unit/reqstool/model_generators/test_requirements_model_generator/test_external_requirements_model_generator/requirements.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/tests/resources/unit/reqstool/model_generators/test_requirements_model_generator/test_microservice_requirements_model_generator/requirements.yml` & `reqstool-0.4.2/tests/resources/unit/reqstool/model_generators/test_requirements_model_generator/test_microservice_requirements_model_generator/requirements.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/tests/resources/unit/reqstool/model_generators/test_requirements_model_generator/test_rational_optional_model_generator/requirements.yml` & `reqstool-0.4.2/tests/resources/unit/reqstool/model_generators/test_requirements_model_generator/test_rational_optional_model_generator/requirements.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/tests/resources/unit/reqstool/model_generators/test_requirements_model_generator/test_system_requirements_model_generator/requirements.yml` & `reqstool-0.4.2/tests/resources/unit/reqstool/model_generators/test_requirements_model_generator/test_system_requirements_model_generator/requirements.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/tests/resources/unit/reqstool/model_generators/test_svcs_model_generator/test_svcs_model_generator/software_verification_cases.yml` & `reqstool-0.4.2/tests/resources/unit/reqstool/model_generators/test_svcs_model_generator/test_svcs_model_generator/software_verification_cases.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/tests/unit/conftest.py` & `reqstool-0.4.2/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/tests/unit/reqstool/commands/report/test_report.py` & `reqstool-0.4.2/tests/unit/reqstool/commands/report/test_report.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 # Copyright © LFV
 
+from reqstool_python_decorators.decorators.decorators import SVCs
 
 from reqstool.commands.report import report
 from reqstool.commands.report.criterias.group_by import GroupbyOptions
 from reqstool.commands.report.criterias.sort_by import SortByOptions
 from reqstool.locations.local_location import LocalLocation
 
 
+@SVCs("SVC_029", "SVC_030", "SVC_032")
 def test_get_template_medium_ms001(local_testdata_resources_rootdir_w_path):
     rc = report.ReportCommand(
         location=LocalLocation(path=local_testdata_resources_rootdir_w_path("test_standard/baseline/ms-001")),
         group_by=GroupbyOptions.CATEGORY,
         sort_by=[SortByOptions.ID],
     )
     assert rc.result
 
 
+@SVCs("SVC_029", "SVC_031", "SVC_033")
 def test_get_template_standard_sys001(local_testdata_resources_rootdir_w_path):
     rc = report.ReportCommand(
         location=LocalLocation(
             path=local_testdata_resources_rootdir_w_path("test_standard/baseline/sys-001"),
         ),
         group_by=GroupbyOptions.INITIAL_IMPORTS,
         sort_by=[SortByOptions.SIGNIFICANCE],
```

### Comparing `reqstool-0.4.1/tests/unit/reqstool/commands/report/criterias/test_criterias.py` & `reqstool-0.4.2/tests/unit/reqstool/commands/report/criterias/test_criterias.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 # Copyright © LFV
 
+from reqstool_python_decorators.decorators.decorators import SVCs
+
 from reqstool.commands.report.criterias.group_by import GroupbyOptions, GroupByOrganizor
 from reqstool.commands.report.criterias.sort_by import SortByOptions
 from reqstool.common.validator_error_holder import ValidationErrorHolder
 from reqstool.common.validators.semantic_validator import SemanticValidator
 from reqstool.locations.local_location import LocalLocation
 from reqstool.model_generators.combined_indexed_dataset_generator import CombinedIndexedDatasetGenerator
 from reqstool.model_generators.combined_raw_datasets_generator import CombinedRawDatasetsGenerator
 from reqstool.models.raw_datasets import CombinedRawDataset
 
 
+@SVCs("SVC_034")
 def test_basic_baseline(resource_funcname_rootdir, local_testdata_resources_rootdir_w_path):
     semantic_validator = SemanticValidator(validation_error_holder=ValidationErrorHolder())
     crd: CombinedRawDataset = CombinedRawDatasetsGenerator(
         initial_location=LocalLocation(path=local_testdata_resources_rootdir_w_path("test_basic/baseline/ms-101")),
         semantic_validator=semantic_validator,
     ).combined_raw_datasets
```

### Comparing `reqstool-0.4.1/tests/unit/reqstool/commands/status/test_statistics_container.py` & `reqstool-0.4.2/tests/unit/reqstool/commands/status/test_statistics_container.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/tests/unit/reqstool/commands/status/test_statistics_generator.py` & `reqstool-0.4.2/tests/unit/reqstool/commands/status/test_statistics_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 # Copyright © LFV
 
+from reqstool_python_decorators.decorators.decorators import SVCs
+
 from reqstool.commands.status.statistics_container import (
     CombinedRequirementTestItem,
     StatisticsContainer,
     TestStatisticsItem,
     TotalStatisticsItem,
 )
 from reqstool.commands.status.statistics_generator import StatisticsGenerator
 from reqstool.common.dataclasses.urn_id import UrnId
 from reqstool.common.validator_error_holder import ValidationErrorHolder
 from reqstool.common.validators.semantic_validator import SemanticValidator
 from reqstool.locations.local_location import LocalLocation
 
 
+@SVCs("SVC_022")
 def test_calculate_test_basic(local_testdata_resources_rootdir_w_path):
     result: StatisticsContainer = StatisticsGenerator(
         initial_location=LocalLocation(path=local_testdata_resources_rootdir_w_path("test_basic/baseline/ms-101")),
         semantic_validator=SemanticValidator(validation_error_holder=ValidationErrorHolder()),
     ).result
 
     expected = StatisticsContainer(
@@ -122,14 +125,15 @@
             nr_of_reqs_with_implementation=2,
             nr_of_total_svcs=4,
         ),
     )
     assert result == expected
 
 
+@SVCs("SVC_023")
 def test_calculate_test_standard_ms001(local_testdata_resources_rootdir_w_path):
     result: StatisticsContainer = StatisticsGenerator(
         initial_location=LocalLocation(path=local_testdata_resources_rootdir_w_path("test_standard/baseline/ms-001")),
         semantic_validator=SemanticValidator(validation_error_holder=ValidationErrorHolder()),
     ).result
 
     expected = StatisticsContainer(
@@ -279,14 +283,15 @@
             nr_of_reqs_with_implementation=5,
             nr_of_total_svcs=9,
         ),
     )
     assert result == expected
 
 
+@SVCs("SVC_024")
 def test_calculate_empty_standard_ms001(local_testdata_resources_rootdir_w_path):
     result: StatisticsContainer = StatisticsGenerator(
         initial_location=LocalLocation(path=local_testdata_resources_rootdir_w_path("test_standard/empty_ms/ms-001")),
         semantic_validator=SemanticValidator(validation_error_holder=ValidationErrorHolder()),
     ).result
 
     expected = StatisticsContainer(
```

### Comparing `reqstool-0.4.1/tests/unit/reqstool/commands/status/test_status.py` & `reqstool-0.4.2/tests/unit/reqstool/commands/status/test_status.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 # Copyright © LFV
+from reqstool_python_decorators.decorators.decorators import SVCs
+
 from reqstool.commands.status.status import StatusCommand
 from reqstool.locations.local_location import LocalLocation
 
 
+@SVCs("SVC_021")
 def test_status_incomplete_implementation(local_testdata_resources_rootdir_w_path):
     result = StatusCommand(
         location=LocalLocation(path=local_testdata_resources_rootdir_w_path("test_standard/baseline/ms-001"))
     )
 
     status, nr_of_incomplete_requirements = result.result
 
     assert nr_of_incomplete_requirements == 5
 
 
+@SVCs("SVC_021")
 def test_status_report_generation_sys_ms(local_testdata_resources_rootdir_w_path):
     result = StatusCommand(
         location=LocalLocation(path=local_testdata_resources_rootdir_w_path("test_standard/empty_ms/ms-001"))
     )
 
     status, nr_of_incomplete_requirements = result.result
```

### Comparing `reqstool-0.4.1/tests/unit/reqstool/common/test_locations.py` & `reqstool-0.4.2/tests/unit/reqstool/common/test_locations.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/tests/unit/reqstool/common/validators/test_semantic_validator.py` & `reqstool-0.4.2/tests/unit/reqstool/common/validators/test_semantic_validator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Copyright © LFV
 
 import pytest
+from reqstool_python_decorators.decorators.decorators import SVCs
 
 from reqstool.common.validators.semantic_validator import SemanticValidator, ValidationErrorHolder
 from reqstool.locations.local_location import LocalLocation
 from reqstool.model_generators import combined_raw_datasets_generator
 
 
 @pytest.fixture
@@ -135,53 +136,59 @@
     assert img.combined_raw_datasets.raw_datasets
 
     errors = semantic_validator._validation_error_holder.get_errors()
 
     assert len(errors) == 7
 
 
+@SVCs("SVC_016")
 def test_validate_no_duplicate_reqs(get_requirements_data_raw):
     holder = ValidationErrorHolder()
     semantic_validator = SemanticValidator(validation_error_holder=holder)
     has_errors = semantic_validator._validate_no_duplicate_requirement_ids(get_requirements_data_raw)
     assert has_errors is True
 
 
+@SVCs("SVC_017")
 def test_validate_no_duplicate_svcs(get_svc_data):
     holder = ValidationErrorHolder()
     semantic_validator = SemanticValidator(validation_error_holder=holder)
     has_errors = semantic_validator._validate_no_duplicate_svc_ids(get_svc_data)
     assert has_errors is True
 
 
+@SVCs("SVC_018")
 def test_validate_svc_to_existing_reqs(get_validation):
     semantic_validator = SemanticValidator(validation_error_holder=ValidationErrorHolder())
     errors = semantic_validator._validate_svc_refers_to_existing_requirement_ids(get_validation)
     expected_error = """SVC '<ms-101:SVC_201>' refers to
                                     non-existing requirement id: <ms-101:REQ_20101>"""
     assert expected_error in errors[0].msg
 
 
+@SVCs("SVC_018")
 def test_validate_impls_to_existing_reqs(get_validation):
     semantic_validator = SemanticValidator(validation_error_holder=ValidationErrorHolder())
     errors = semantic_validator._validate_annotation_impls_refers_to_existing_requirement_ids(get_validation)
     expected_error = """Annotation refers to
                             non-existing requirement id: <ms-101:REQ_10101>"""
     assert expected_error in errors[0].msg
 
 
+@SVCs("SVC_019")
 def test_validate_tests_to_existing_svcs(get_validation):
     semantic_validator = SemanticValidator(validation_error_holder=ValidationErrorHolder())
     errors = semantic_validator._validate_annotation_tests_refers_to_existing_svc_ids(get_validation)
     expected_error_1 = "Annotation refers to non-existing svc id: <ms-101:SVC_101121>"
     expected_error_2 = "Annotation refers to non-existing svc id: <ms-101:SVC_102>"
     assert expected_error_1 in errors[0].msg
     assert expected_error_2 in errors[1].msg
 
 
+@SVCs("SVC_019")
 def test_validate_mvrs_to_existing_svcs(get_validation):
     semantic_validator = SemanticValidator(validation_error_holder=ValidationErrorHolder())
     errors = semantic_validator._validate_mvr_refers_to_existing_svc_ids(get_validation)
     expected_error = "MVR refers to non-existing svc id: <ms-101:SVC_20111>"
     assert expected_error in errors[0].msg
```

### Comparing `reqstool-0.4.1/tests/unit/reqstool/expression_languages/test_requirements_el.py` & `reqstool-0.4.2/tests/unit/reqstool/expression_languages/test_requirements_el.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Copyright © LFV
 
 import pytest
+from reqstool_python_decorators.decorators.decorators import SVCs
 
 from reqstool.expression_languages.requirements_el import RequirementsELTransformer
 from reqstool.models.requirements import SIGNIFANCETYPES, RequirementData
 
 
 @pytest.fixture
 def create_tree():
@@ -68,14 +69,15 @@
 
     tree = create_tree(el)
 
     assert RequirementsELTransformer(urn="urn", data=requirement_data("urn:REQ_001")).transform(tree) is False
     assert RequirementsELTransformer(urn="urn", data=requirement_data("urn:REQ_101")).transform(tree) is True
 
 
+@SVCs("SVC_013")
 def test_comp_id_regex_equals(create_tree, requirement_data):
     el = "ids == /urn\\:REQ_(\\d{2,3}|123)$/"
     tree = create_tree(el)
 
     assert RequirementsELTransformer(urn="urn", data=requirement_data("urn:123")).transform(tree) is False
     assert RequirementsELTransformer(urn="urn", data=requirement_data("urn:REQ_")).transform(tree) is False
     assert RequirementsELTransformer(urn="urn", data=requirement_data("urn:REQ_1")).transform(tree) is False
```

### Comparing `reqstool-0.4.1/tests/unit/reqstool/expression_languages/test_svcs_el.py` & `reqstool-0.4.2/tests/unit/reqstool/expression_languages/test_svcs_el.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Copyright © LFV
 
 import pytest
+from reqstool_python_decorators.decorators.decorators import SVCs
 
 from reqstool.expression_languages.svcs_el import SVCsELTransformer
 from reqstool.models.svcs import VERIFICATIONTYPES, SVCData
 
 
 @pytest.fixture
 def create_tree():
@@ -51,14 +52,15 @@
 
     tree = create_tree(el)
 
     assert SVCsELTransformer(urn="urn", data=svc_data("urn:SVC_001")).transform(tree) is False
     assert SVCsELTransformer(urn="urn", data=svc_data("urn:SVC_101")).transform(tree) is True
 
 
+@SVCs("SVC_014")
 def test_comp_id_regex_equals(create_tree, svc_data):
     el = "ids == /urn\\:SVC_(\\d{2,3}|123)$/"
     tree = create_tree(el)
 
     assert SVCsELTransformer(urn="urn", data=svc_data("urn:123")).transform(tree) is False
     assert SVCsELTransformer(urn="urn", data=svc_data("urn:SVC_")).transform(tree) is False
     assert SVCsELTransformer(urn="urn", data=svc_data("urn:SVC_1")).transform(tree) is False
```

### Comparing `reqstool-0.4.1/tests/unit/reqstool/locations/test_git_location.py` & `reqstool-0.4.2/tests/unit/reqstool/locations/test_git_location.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/tests/unit/reqstool/model_generators/test_annotations_model_generator.py` & `reqstool-0.4.2/tests/unit/reqstool/model_generators/test_annotations_model_generator.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/tests/unit/reqstool/model_generators/test_combined_indexed_dataset_generator.py` & `reqstool-0.4.2/tests/unit/reqstool/model_generators/test_combined_indexed_dataset_generator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Copyright © LFV
 
+from reqstool_python_decorators.decorators.decorators import SVCs
+
 from reqstool.common.dataclasses.urn_id import UrnId
 from reqstool.common.validator_error_holder import ValidationErrorHolder
 from reqstool.common.validators.semantic_validator import SemanticValidator
 from reqstool.locations.local_location import LocalLocation
 from reqstool.model_generators.combined_indexed_dataset_generator import CombinedIndexedDatasetGenerator
 from reqstool.model_generators.combined_raw_datasets_generator import CombinedRawDatasetsGenerator
 from reqstool.models.raw_datasets import CombinedRawDataset
@@ -29,14 +31,15 @@
     ).combined_raw_datasets
 
     cids = CombinedIndexedDatasetGenerator(_crd=crd, _filtered=False).combined_indexed_dataset
 
     assert len(cids.requirements) == 8
 
 
+@SVCs("SVC_005")
 def test_standard_baseline_ms001(resource_funcname_rootdir, local_testdata_resources_rootdir_w_path):
     semantic_validator = SemanticValidator(validation_error_holder=ValidationErrorHolder())
     crd: CombinedRawDataset = CombinedRawDatasetsGenerator(
         initial_location=LocalLocation(path=local_testdata_resources_rootdir_w_path("test_standard/baseline/ms-001")),
         semantic_validator=semantic_validator,
     ).combined_raw_datasets
```

### Comparing `reqstool-0.4.1/tests/unit/reqstool/model_generators/test_combined_raw_datasets_generator.py` & `reqstool-0.4.2/tests/unit/reqstool/filters/test_software_verification_cases_filters.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,44 +1,25 @@
 # Copyright © LFV
+from reqstool_python_decorators.decorators.decorators import SVCs
 
-import pytest
-
+from reqstool.common.dataclasses.urn_id import UrnId
 from reqstool.common.validator_error_holder import ValidationErrorHolder
 from reqstool.common.validators.semantic_validator import SemanticValidator
 from reqstool.locations.local_location import LocalLocation
-from reqstool.model_generators import combined_raw_datasets_generator
-
-
-def test_basic_local(resource_funcname_rootdir, local_testdata_resources_rootdir_w_path):
-    semantic_validator = SemanticValidator(validation_error_holder=ValidationErrorHolder())
-    combined_raw_datasets_generator.CombinedRawDatasetsGenerator(
-        initial_location=LocalLocation(path=local_testdata_resources_rootdir_w_path("test_basic/baseline/ms-101")),
-        semantic_validator=semantic_validator,
-    )
-
-
-def test_basic_requirements_config(resource_funcname_rootdir, local_testdata_resources_rootdir_w_path):
-    semantic_validator = SemanticValidator(validation_error_holder=ValidationErrorHolder())
-    combined_raw_datasets_generator.CombinedRawDatasetsGenerator(
-        initial_location=LocalLocation(
-            path=local_testdata_resources_rootdir_w_path("test_basic/with_requirements_config/ms-101")
-        ),
-        semantic_validator=semantic_validator,
-    )
+from reqstool.model_generators.combined_indexed_dataset_generator import CombinedIndexedDatasetGenerator
+from reqstool.model_generators.combined_raw_datasets_generator import CombinedRawDatasetsGenerator
+from reqstool.models.raw_datasets import CombinedRawDataset
 
 
-@pytest.mark.skip(reason="Test should target combined indexed data set instead of CombinedRawDataset")
-def test_standard_ms001_initial(local_testdata_resources_rootdir_w_path):
+@SVCs("SVC_011", "SVC_012")
+def test_include_exclude_for_svcs(local_testdata_resources_rootdir_w_path):
     semantic_validator = SemanticValidator(validation_error_holder=ValidationErrorHolder())
-
-    combined_raw_datasets_generator.CombinedRawDatasetsGenerator(
+    crd: CombinedRawDataset = CombinedRawDatasetsGenerator(
         initial_location=LocalLocation(path=local_testdata_resources_rootdir_w_path("test_standard/baseline/ms-001")),
         semantic_validator=semantic_validator,
     ).combined_raw_datasets
 
+    cids = CombinedIndexedDatasetGenerator(_crd=crd, _filtered=True).combined_indexed_dataset
 
-def test_standard_sys001_initial(local_testdata_resources_rootdir_w_path):
-    semantic_validator = SemanticValidator(validation_error_holder=ValidationErrorHolder())
-    combined_raw_datasets_generator.CombinedRawDatasetsGenerator(
-        initial_location=LocalLocation(path=local_testdata_resources_rootdir_w_path("test_standard/baseline/sys-001")),
-        semantic_validator=semantic_validator,
-    )
+    assert UrnId(urn="sys-001", id="SVC_sys001_500") in cids.svcs
+    assert UrnId(urn="sys-001", id="SVC_sys001_600") in cids.svcs
+    assert UrnId(urn="sys-001", id="SVC_sys001_000") not in cids.svcs
```

### Comparing `reqstool-0.4.1/tests/unit/reqstool/model_generators/test_mvrs_model_generator.py` & `reqstool-0.4.2/tests/unit/reqstool/model_generators/test_mvrs_model_generator.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/tests/unit/reqstool/model_generators/test_requirements_model_generator.py` & `reqstool-0.4.2/tests/unit/reqstool/model_generators/test_requirements_model_generator.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/tests/unit/reqstool/model_generators/test_svcs_model_generator.py` & `reqstool-0.4.2/tests/unit/reqstool/model_generators/test_svcs_model_generator.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/tests/unit/reqstool/model_generators/test_testdata_model_generator.py` & `reqstool-0.4.2/tests/unit/reqstool/model_generators/test_testdata_model_generator.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright © LFV
 
 import re
 
 import pytest
+from reqstool_python_decorators.decorators.decorators import SVCs
 
 from reqstool.model_generators.testdata_model_generator import TestDataModelGenerator
 
 karate_method_names = [
     "[1.4:55] Create a subscripiton with filter and receive messages",
     "[1:38] Create a subscripiton with filter and receive messages",
     "[1.2:53] Create a subscripiton with filter and receive messages",
@@ -14,27 +15,33 @@
 
 unit_method_names = [
     "testFlightIdAircraftId",
     "testFlightIdAircraftId(String, int)[1]",
 ]
 
 
+@SVCs("SVC_006")
 @pytest.mark.parametrize("method_name", karate_method_names)
 def test_karate_method_identifier_regex(method_name):
     karate_match = re.match(TestDataModelGenerator.KARATE_METHOD_IDENTIFIER_REGEX, method_name)
     assert karate_match is not None
     assert karate_match.group(1) == "Create a subscripiton with filter and receive messages"
 
 
+@SVCs("SVC_007")
 @pytest.mark.parametrize("method_name", unit_method_names)
 def test_unit_method_identifier_regex(method_name):
     unit_match = re.match(TestDataModelGenerator.UNIT_METHOD_IDENTIFIER_REGEX, method_name)
     assert unit_match is not None
     assert unit_match.group(1) == "testFlightIdAircraftId"
 
 
-@pytest.mark.skip(reason="Awaiting testdata update")
-def test_testdata_model_generator():
+def test_testdata_model_generator(local_testdata_resources_rootdir_w_path):
     # TODO:
     # * Test the different variants: passed, skipped, failure etc
     # * Test different types of file structure (Java, Python, Frontend Typescript)
-    pass
+
+    tdmg = (
+        TestDataModelGenerator(path=local_testdata_resources_rootdir_w_path("test_basic/baseline/ms-101"), urn="test"),
+    )
+
+    assert tdmg is not None
```

### Comparing `reqstool-0.4.1/tests/unit/reqstool/models/test_annotations.py` & `reqstool-0.4.2/tests/unit/reqstool/models/test_annotations.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/tests/unit/reqstool/models/test_implementations.py` & `reqstool-0.4.2/tests/unit/reqstool/models/test_implementations.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/tests/unit/reqstool/models/test_imports.py` & `reqstool-0.4.2/tests/unit/reqstool/models/test_imports.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/tests/unit/reqstool/models/test_mvrs.py` & `reqstool-0.4.2/tests/unit/reqstool/models/test_mvrs.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/tests/unit/reqstool/models/test_requirements.py` & `reqstool-0.4.2/tests/unit/reqstool/models/test_requirements.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/tests/unit/reqstool/models/test_svcs.py` & `reqstool-0.4.2/tests/unit/reqstool/models/test_svcs.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/tests/unit/reqstool/reqstool_config/test_reqstool_config.py` & `reqstool-0.4.2/tests/unit/reqstool/reqstool_config/test_reqstool_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 def rc_yaml_config_all() -> dict:
     YAML_STR = """
     type: java-maven
 
     project_root_dir: /some_root_dir
 
     locations:
-        annotations: custom_annotations.yml
-        test_results:
-            failsafe: target/failsafe
-            surefire: target/surefire
+      annotations: custom_annotations.yml
+      test_results_dirs:
+        - target/failsafe
+        - target/surefire
     """
     yaml = YAML(typ="safe")
     data = yaml.load(YAML_STR)
 
     return data
 
 
@@ -51,16 +51,16 @@
 
 def test_all(rc_yaml_config_all):
     rc = ReqstoolConfig._parse(yaml_data=rc_yaml_config_all)
 
     assert rc.type == TYPES.JAVA_MAVEN
     assert rc.project_root_dir == "/some_root_dir"
     assert rc.locations.annotations == "custom_annotations.yml"
-    assert rc.locations.test_results.failsafe == "target/failsafe"
-    assert rc.locations.test_results.surefire == "target/surefire"
+    assert rc.locations.test_results[0] == "target/failsafe"
+    assert rc.locations.test_results[1] == "target/surefire"
 
 
 def test_minimal(rc_yaml_config_minimal):
     rc = ReqstoolConfig._parse(yaml_data=rc_yaml_config_minimal)
 
     assert rc.type == TYPES.JAVA_MAVEN
```

### Comparing `reqstool-0.4.1/tests/unit/reqstool/requirements_indata/test_requirements_indata_paths.py` & `reqstool-0.4.2/tests/unit/reqstool/requirements_indata/test_requirements_indata_paths.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,22 +32,23 @@
     prepend_str = "/path/to/prepend"
     a.prepend_paths(prepend_str)
 
     assert a.requirements_yml.path == b.requirements_yml.path
     assert a.svcs_yml.path == b.svcs_yml.path
     assert a.mvrs_yml.path == b.mvrs_yml.path
     assert a.annotations_yml.path == str(PurePath(prepend_str, b.annotations_yml.path))
-    assert a.test_results_failsafe_dir.path == str(PurePath(prepend_str, b.test_results_failsafe_dir.path))
-    assert a.test_results_surefire_dir.path == str(PurePath(prepend_str, b.test_results_surefire_dir.path))
+    assert len(a.test_results_dirs) == 1
 
 
 # Test the merge method with properties that can be None
 def test_merge_with_none_properties(default_instance, java_instance):
     java_instance.ra_tests_yml = None
-    merged_instance = default_instance.merge(java_instance)
+    java_merged_instance = default_instance.merge(java_instance)
 
-    assert merged_instance.requirements_yml.path == "requirements.yml"
-    assert merged_instance.svcs_yml.path == "software_verification_cases.yml"
-    assert merged_instance.mvrs_yml.path == "manual_verification_results.yml"
-    assert merged_instance.annotations_yml.path == "target/reqstool/annotations.yml"
-    assert merged_instance.test_results_failsafe_dir.path == "target/failsafe-reports"
-    assert merged_instance.test_results_surefire_dir.path == "target/surefire-reports"
+    assert java_merged_instance.requirements_yml.path == "requirements.yml"
+    assert java_merged_instance.svcs_yml.path == "software_verification_cases.yml"
+    assert java_merged_instance.mvrs_yml.path == "manual_verification_results.yml"
+    assert java_merged_instance.annotations_yml.path == "target/reqstool/annotations.yml"
+    assert len(java_merged_instance.test_results_dirs) == 2
+
+    expected_paths = ["target/failfire-reports", "target/surefire-reports"]
+    assert all(item.path in expected_paths for item in java_merged_instance.test_results_dirs)
```

### Comparing `reqstool-0.4.1/tests/unit/reqstool/resources/schemas/v1/test_json_schemas.py` & `reqstool-0.4.2/tests/unit/reqstool/resources/schemas/v1/test_json_schemas.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,37 @@
 # Copyright © LFV
 
 
 from jsonschema import Draft202012Validator
+from reqstool_python_decorators.decorators.decorators import SVCs
 
 from reqstool.common.validators.syntax_validator import JsonSchemaTypes
 
 
+@SVCs("SVC_015")
 def test_validate_annotations_schema_json():
     Draft202012Validator.check_schema(JsonSchemaTypes.ANNOTATIONS.value.schema)
 
 
+@SVCs("SVC_015")
 def test_validate_common_schema_json():
     Draft202012Validator.check_schema(JsonSchemaTypes.COMMON.value.schema)
 
 
+@SVCs("SVC_015")
 def test_validate_manual_verification_results_schema_json():
     Draft202012Validator.check_schema(JsonSchemaTypes.MANUAL_VERIFICATION_RESULTS.value.schema)
 
 
+@SVCs("SVC_015")
 def test_validate_requirements_config_schema_json():
     Draft202012Validator.check_schema(JsonSchemaTypes.REQSTOOL_CONFIG.value.schema)
 
 
+@SVCs("SVC_015")
 def test_validate_requirements_schema_json():
     Draft202012Validator.check_schema(JsonSchemaTypes.REQUIREMENTS.value.schema)
 
 
+@SVCs("SVC_015")
 def test_validate_software_verification_cases_schema_json():
     Draft202012Validator.check_schema(JsonSchemaTypes.SOFTWARE_VERIFICATION_CASES.value.schema)
```

### Comparing `reqstool-0.4.1/.gitignore` & `reqstool-0.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/LICENSE` & `reqstool-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/README.md` & `reqstool-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.1/pyproject.toml` & `reqstool-0.4.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -37,25 +37,30 @@
     "maven-artifact==0.3.4",
     "pygit2==1.14.1",
     "referencing==0.34.0",
     "requests-file==2.0.0",
     "ruamel.yaml==0.18.6",
     "tabulate==0.9.0",
     "xmldict==0.4.1",
+    "reqstool-python-decorators ==0.0.4",
 ]
 
 [project.scripts]
 reqstool = "reqstool.command:main"
 
 [tool.hatch.version]
 source = "vcs"
 
 [tool.hatch.version.raw-options]
 local_scheme = "no-local-version"
 
+[tool.hatch.build.targets.wheel.hooks.decorators]
+dependencies = ["reqstool-python-hatch-plugin==0.0.3"]
+path = ["src","tests"]
+
 [tool.hatch.envs.test]
 dependencies = ["pytest==8.0.0", "pytest-sugar==1.0.0", "pytest-cov==4.1.0"]
 
 [tool.hatch.envs.lint]
 detached = true
 
 dependencies = ["black==24.1.1", "flake8==7.0.0", "flake8-pyproject==1.2.3"]
```

### Comparing `reqstool-0.4.1/PKG-INFO` & `reqstool-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: reqstool
-Version: 0.4.1
+Version: 0.4.2
 Summary: A tool for managing requirements with related tests and test results.
 Project-URL: Source, https://github.com/Luftfartsverket/reqstool-client
 Author-email: LFV <info@lfv.se>
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -13,14 +13,15 @@
 Requires-Dist: jinja2==3.1.3
 Requires-Dist: jsonpickle==3.0.3
 Requires-Dist: jsonschema[format-nongpl]==4.21.1
 Requires-Dist: lark==1.1.9
 Requires-Dist: maven-artifact==0.3.4
 Requires-Dist: pygit2==1.14.1
 Requires-Dist: referencing==0.34.0
+Requires-Dist: reqstool-python-decorators==0.0.4
 Requires-Dist: requests-file==2.0.0
 Requires-Dist: ruamel-yaml==0.18.6
 Requires-Dist: tabulate==0.9.0
 Requires-Dist: xmldict==0.4.1
 Description-Content-Type: text/markdown
```

