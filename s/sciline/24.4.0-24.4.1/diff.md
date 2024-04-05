# Comparing `tmp/sciline-24.4.0.tar.gz` & `tmp/sciline-24.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sciline-24.4.0.tar", last modified: Tue Apr  2 13:19:07 2024, max compression
+gzip compressed data, was "sciline-24.4.1.tar", last modified: Fri Apr  5 04:14:01 2024, max compression
```

## Comparing `sciline-24.4.0.tar` & `sciline-24.4.1.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:19:07.089929 sciline-24.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-02 13:18:56.000000 sciline-24.4.0/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:19:07.069929 sciline-24.4.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-02 13:18:56.000000 sciline-24.4.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:19:07.073929 sciline-24.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-04-02 13:18:56.000000 sciline-24.4.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-02 13:18:56.000000 sciline-24.4.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-02 13:18:56.000000 sciline-24.4.0/.github/workflows/nightly_at_main.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-02 13:18:56.000000 sciline-24.4.0/.github/workflows/nightly_at_release.yml
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-02 13:18:56.000000 sciline-24.4.0/.github/workflows/python-version-ci
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-02 13:18:56.000000 sciline-24.4.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-02 13:18:56.000000 sciline-24.4.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-02 13:18:56.000000 sciline-24.4.0/.github/workflows/unpinned.yml
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-02 13:18:56.000000 sciline-24.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-02 13:18:56.000000 sciline-24.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-04-02 13:18:56.000000 sciline-24.4.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-02 13:18:56.000000 sciline-24.4.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-02 13:18:56.000000 sciline-24.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-02 13:18:56.000000 sciline-24.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-04-02 13:19:07.089929 sciline-24.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-02 13:18:56.000000 sciline-24.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:19:07.073929 sciline-24.4.0/conda/
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-02 13:18:56.000000 sciline-24.4.0/conda/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:19:07.073929 sciline-24.4.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:19:07.073929 sciline-24.4.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-04-02 13:18:56.000000 sciline-24.4.0/docs/_static/anaconda-icon.js
--rw-r--r--   0 runner    (1001) docker     (127)   137750 2024-04-02 13:18:56.000000 sciline-24.4.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)    75109 2024-04-02 13:18:56.000000 sciline-24.4.0/docs/_static/logo-dark.svg
--rw-r--r--   0 runner    (1001) docker     (127)    75109 2024-04-02 13:18:56.000000 sciline-24.4.0/docs/_static/logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:19:07.073929 sciline-24.4.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-02 13:18:56.000000 sciline-24.4.0/docs/_templates/class-template.rst
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-02 13:18:56.000000 sciline-24.4.0/docs/_templates/doc_version.html
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-02 13:18:56.000000 sciline-24.4.0/docs/_templates/module-template.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:19:07.073929 sciline-24.4.0/docs/about/
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-02 13:18:56.000000 sciline-24.4.0/docs/about/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:19:07.073929 sciline-24.4.0/docs/api-reference/
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-02 13:18:56.000000 sciline-24.4.0/docs/api-reference/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     6653 2024-04-02 13:18:56.000000 sciline-24.4.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:19:07.073929 sciline-24.4.0/docs/developer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:19:07.073929 sciline-24.4.0/docs/developer/architecture-and-design/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-02 13:18:56.000000 sciline-24.4.0/docs/developer/architecture-and-design/index.md
--rw-r--r--   0 runner    (1001) docker     (127)    12404 2024-04-02 13:18:56.000000 sciline-24.4.0/docs/developer/architecture-and-design/workflow-design.md
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-02 13:18:56.000000 sciline-24.4.0/docs/developer/coding-conventions.md
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-02 13:18:56.000000 sciline-24.4.0/docs/developer/dependency-management.md
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-02 13:18:56.000000 sciline-24.4.0/docs/developer/getting-started.md
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-02 13:18:56.000000 sciline-24.4.0/docs/developer/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     5124 2024-04-02 13:18:56.000000 sciline-24.4.0/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:19:07.077929 sciline-24.4.0/docs/recipes/
--rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-04-02 13:18:56.000000 sciline-24.4.0/docs/recipes/applying-decorators.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4345 2024-04-02 13:18:56.000000 sciline-24.4.0/docs/recipes/continue-from-intermediate-results.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-02 13:18:56.000000 sciline-24.4.0/docs/recipes/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     4601 2024-04-02 13:18:56.000000 sciline-24.4.0/docs/recipes/replacing-providers.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-04-02 13:18:56.000000 sciline-24.4.0/docs/recipes/side-effects-and-file-writing.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:19:07.077929 sciline-24.4.0/docs/user-guide/
--rw-r--r--   0 runner    (1001) docker     (127)    15393 2024-04-02 13:18:56.000000 sciline-24.4.0/docs/user-guide/generic-providers.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9567 2024-04-02 13:18:56.000000 sciline-24.4.0/docs/user-guide/getting-started.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-02 13:18:56.000000 sciline-24.4.0/docs/user-guide/index.md
--rw-r--r--   0 runner    (1001) docker     (127)    14937 2024-04-02 13:18:56.000000 sciline-24.4.0/docs/user-guide/parameter-tables.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8876 2024-04-02 13:18:56.000000 sciline-24.4.0/docs/user-guide/provenance.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-04-02 13:18:56.000000 sciline-24.4.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:19:07.081929 sciline-24.4.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-02 13:18:56.000000 sciline-24.4.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-02 13:18:56.000000 sciline-24.4.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-02 13:18:56.000000 sciline-24.4.0/requirements/basetest.in
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-02 13:18:56.000000 sciline-24.4.0/requirements/basetest.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-02 13:18:56.000000 sciline-24.4.0/requirements/ci.in
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-02 13:18:56.000000 sciline-24.4.0/requirements/ci.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-02 13:18:56.000000 sciline-24.4.0/requirements/dev.in
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-04-02 13:18:56.000000 sciline-24.4.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-02 13:18:56.000000 sciline-24.4.0/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (127)     3602 2024-04-02 13:18:56.000000 sciline-24.4.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-04-02 13:18:56.000000 sciline-24.4.0/requirements/make_base.py
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-02 13:18:56.000000 sciline-24.4.0/requirements/mypy.in
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-02 13:18:56.000000 sciline-24.4.0/requirements/mypy.txt
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-02 13:18:56.000000 sciline-24.4.0/requirements/nightly.in
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-02 13:18:56.000000 sciline-24.4.0/requirements/nightly.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-02 13:18:56.000000 sciline-24.4.0/requirements/static.in
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-02 13:18:56.000000 sciline-24.4.0/requirements/static.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-02 13:18:56.000000 sciline-24.4.0/requirements/test-dask.in
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-02 13:18:56.000000 sciline-24.4.0/requirements/test-dask.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-02 13:18:56.000000 sciline-24.4.0/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-02 13:18:56.000000 sciline-24.4.0/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-02 13:18:56.000000 sciline-24.4.0/requirements/wheels.in
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-02 13:18:56.000000 sciline-24.4.0/requirements/wheels.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:19:07.081929 sciline-24.4.0/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     7947 2024-04-02 13:18:56.000000 sciline-24.4.0/resources/sciline.svg
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-02 13:19:07.089929 sciline-24.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:19:07.069929 sciline-24.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:19:07.081929 sciline-24.4.0/src/sciline/
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-02 13:18:56.000000 sciline-24.4.0/src/sciline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10453 2024-04-02 13:18:56.000000 sciline-24.4.0/src/sciline/_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-04-02 13:18:56.000000 sciline-24.4.0/src/sciline/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-02 13:18:56.000000 sciline-24.4.0/src/sciline/display.py
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-02 13:18:56.000000 sciline-24.4.0/src/sciline/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-02 13:18:56.000000 sciline-24.4.0/src/sciline/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-02 13:18:56.000000 sciline-24.4.0/src/sciline/param_table.py
--rw-r--r--   0 runner    (1001) docker     (127)    35503 2024-04-02 13:18:56.000000 sciline-24.4.0/src/sciline/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 13:18:56.000000 sciline-24.4.0/src/sciline/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-04-02 13:18:56.000000 sciline-24.4.0/src/sciline/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:19:07.085929 sciline-24.4.0/src/sciline/serialize/
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-02 13:18:56.000000 sciline-24.4.0/src/sciline/serialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-04-02 13:18:56.000000 sciline-24.4.0/src/sciline/serialize/_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-04-02 13:18:56.000000 sciline-24.4.0/src/sciline/serialize/graph_json_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-02 13:18:56.000000 sciline-24.4.0/src/sciline/series.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:19:07.085929 sciline-24.4.0/src/sciline/sphinxext/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-02 13:18:56.000000 sciline-24.4.0/src/sciline/sphinxext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5257 2024-04-02 13:18:56.000000 sciline-24.4.0/src/sciline/sphinxext/domain_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5593 2024-04-02 13:18:56.000000 sciline-24.4.0/src/sciline/task_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-02 13:18:56.000000 sciline-24.4.0/src/sciline/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-04-02 13:18:56.000000 sciline-24.4.0/src/sciline/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:19:07.085929 sciline-24.4.0/src/sciline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-04-02 13:19:07.000000 sciline-24.4.0/src/sciline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-04-02 13:19:07.000000 sciline-24.4.0/src/sciline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 13:19:07.000000 sciline-24.4.0/src/sciline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-02 13:19:07.000000 sciline-24.4.0/src/sciline.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:19:07.085929 sciline-24.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-02 13:18:56.000000 sciline-24.4.0/tests/_provider_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-04-02 13:18:56.000000 sciline-24.4.0/tests/complex_workflow_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-02 13:18:56.000000 sciline-24.4.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-02 13:18:56.000000 sciline-24.4.0/tests/dask_scheduler_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-02 13:18:56.000000 sciline-24.4.0/tests/domain_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-02 13:18:56.000000 sciline-24.4.0/tests/package_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-02 13:18:56.000000 sciline-24.4.0/tests/param_table_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    40014 2024-04-02 13:18:56.000000 sciline-24.4.0/tests/pipeline_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7380 2024-04-02 13:18:56.000000 sciline-24.4.0/tests/pipeline_with_optional_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    24917 2024-04-02 13:18:56.000000 sciline-24.4.0/tests/pipeline_with_param_table_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-02 13:18:56.000000 sciline-24.4.0/tests/pipeline_with_postponed_annotations_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:19:07.085929 sciline-24.4.0/tests/serialize/
--rw-r--r--   0 runner    (1001) docker     (127)    11394 2024-04-02 13:18:56.000000 sciline-24.4.0/tests/serialize/json_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-02 13:18:56.000000 sciline-24.4.0/tests/task_graph_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7908 2024-04-02 13:18:56.000000 sciline-24.4.0/tests/utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-02 13:18:56.000000 sciline-24.4.0/tests/visualize_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-04-02 13:18:56.000000 sciline-24.4.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:14:01.683626 sciline-24.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-05 04:13:51.000000 sciline-24.4.1/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:14:01.667626 sciline-24.4.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-05 04:13:51.000000 sciline-24.4.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:14:01.671626 sciline-24.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-04-05 04:13:51.000000 sciline-24.4.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-05 04:13:51.000000 sciline-24.4.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-05 04:13:51.000000 sciline-24.4.1/.github/workflows/nightly_at_main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-05 04:13:51.000000 sciline-24.4.1/.github/workflows/nightly_at_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-05 04:13:51.000000 sciline-24.4.1/.github/workflows/python-version-ci
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-05 04:13:51.000000 sciline-24.4.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-05 04:13:51.000000 sciline-24.4.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-05 04:13:51.000000 sciline-24.4.1/.github/workflows/unpinned.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-05 04:13:51.000000 sciline-24.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-05 04:13:51.000000 sciline-24.4.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-04-05 04:13:51.000000 sciline-24.4.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-05 04:13:51.000000 sciline-24.4.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-05 04:13:51.000000 sciline-24.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-05 04:13:51.000000 sciline-24.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-04-05 04:14:01.683626 sciline-24.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-05 04:13:51.000000 sciline-24.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:14:01.671626 sciline-24.4.1/conda/
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-05 04:13:51.000000 sciline-24.4.1/conda/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:14:01.671626 sciline-24.4.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:14:01.671626 sciline-24.4.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-04-05 04:13:51.000000 sciline-24.4.1/docs/_static/anaconda-icon.js
+-rw-r--r--   0 runner    (1001) docker     (127)   137750 2024-04-05 04:13:51.000000 sciline-24.4.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    75109 2024-04-05 04:13:51.000000 sciline-24.4.1/docs/_static/logo-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    75109 2024-04-05 04:13:51.000000 sciline-24.4.1/docs/_static/logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:14:01.671626 sciline-24.4.1/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-05 04:13:51.000000 sciline-24.4.1/docs/_templates/class-template.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-05 04:13:51.000000 sciline-24.4.1/docs/_templates/doc_version.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-05 04:13:51.000000 sciline-24.4.1/docs/_templates/module-template.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:14:01.671626 sciline-24.4.1/docs/about/
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-05 04:13:51.000000 sciline-24.4.1/docs/about/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:14:01.671626 sciline-24.4.1/docs/api-reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-05 04:13:51.000000 sciline-24.4.1/docs/api-reference/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6653 2024-04-05 04:13:51.000000 sciline-24.4.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:14:01.671626 sciline-24.4.1/docs/developer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:14:01.671626 sciline-24.4.1/docs/developer/architecture-and-design/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-05 04:13:51.000000 sciline-24.4.1/docs/developer/architecture-and-design/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)    12404 2024-04-05 04:13:51.000000 sciline-24.4.1/docs/developer/architecture-and-design/workflow-design.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-05 04:13:51.000000 sciline-24.4.1/docs/developer/coding-conventions.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-05 04:13:51.000000 sciline-24.4.1/docs/developer/dependency-management.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-05 04:13:51.000000 sciline-24.4.1/docs/developer/getting-started.md
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-05 04:13:51.000000 sciline-24.4.1/docs/developer/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5124 2024-04-05 04:13:51.000000 sciline-24.4.1/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:14:01.675626 sciline-24.4.1/docs/recipes/
+-rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-04-05 04:13:51.000000 sciline-24.4.1/docs/recipes/applying-decorators.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4345 2024-04-05 04:13:51.000000 sciline-24.4.1/docs/recipes/continue-from-intermediate-results.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-05 04:13:51.000000 sciline-24.4.1/docs/recipes/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4601 2024-04-05 04:13:51.000000 sciline-24.4.1/docs/recipes/replacing-providers.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-04-05 04:13:51.000000 sciline-24.4.1/docs/recipes/side-effects-and-file-writing.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:14:01.675626 sciline-24.4.1/docs/user-guide/
+-rw-r--r--   0 runner    (1001) docker     (127)    15393 2024-04-05 04:13:51.000000 sciline-24.4.1/docs/user-guide/generic-providers.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9567 2024-04-05 04:13:51.000000 sciline-24.4.1/docs/user-guide/getting-started.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-05 04:13:51.000000 sciline-24.4.1/docs/user-guide/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)    14937 2024-04-05 04:13:51.000000 sciline-24.4.1/docs/user-guide/parameter-tables.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8876 2024-04-05 04:13:51.000000 sciline-24.4.1/docs/user-guide/provenance.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-04-05 04:13:51.000000 sciline-24.4.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:14:01.679626 sciline-24.4.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-05 04:13:51.000000 sciline-24.4.1/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-05 04:13:51.000000 sciline-24.4.1/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-05 04:13:51.000000 sciline-24.4.1/requirements/basetest.in
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-05 04:13:51.000000 sciline-24.4.1/requirements/basetest.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-05 04:13:51.000000 sciline-24.4.1/requirements/ci.in
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-05 04:13:51.000000 sciline-24.4.1/requirements/ci.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-05 04:13:51.000000 sciline-24.4.1/requirements/dev.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-04-05 04:13:51.000000 sciline-24.4.1/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-05 04:13:51.000000 sciline-24.4.1/requirements/docs.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3602 2024-04-05 04:13:51.000000 sciline-24.4.1/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-04-05 04:13:51.000000 sciline-24.4.1/requirements/make_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-05 04:13:51.000000 sciline-24.4.1/requirements/mypy.in
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-05 04:13:51.000000 sciline-24.4.1/requirements/mypy.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-05 04:13:51.000000 sciline-24.4.1/requirements/nightly.in
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-05 04:13:51.000000 sciline-24.4.1/requirements/nightly.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 04:13:51.000000 sciline-24.4.1/requirements/static.in
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-05 04:13:51.000000 sciline-24.4.1/requirements/static.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-05 04:13:51.000000 sciline-24.4.1/requirements/test-dask.in
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-05 04:13:51.000000 sciline-24.4.1/requirements/test-dask.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-05 04:13:51.000000 sciline-24.4.1/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-05 04:13:51.000000 sciline-24.4.1/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-05 04:13:51.000000 sciline-24.4.1/requirements/wheels.in
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-05 04:13:51.000000 sciline-24.4.1/requirements/wheels.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:14:01.679626 sciline-24.4.1/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     7947 2024-04-05 04:13:51.000000 sciline-24.4.1/resources/sciline.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-05 04:14:01.687626 sciline-24.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:14:01.667626 sciline-24.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:14:01.679626 sciline-24.4.1/src/sciline/
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-05 04:13:51.000000 sciline-24.4.1/src/sciline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10453 2024-04-05 04:13:51.000000 sciline-24.4.1/src/sciline/_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-04-05 04:13:51.000000 sciline-24.4.1/src/sciline/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-05 04:13:51.000000 sciline-24.4.1/src/sciline/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-05 04:13:51.000000 sciline-24.4.1/src/sciline/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-05 04:13:51.000000 sciline-24.4.1/src/sciline/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-05 04:13:51.000000 sciline-24.4.1/src/sciline/param_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35503 2024-04-05 04:13:51.000000 sciline-24.4.1/src/sciline/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 04:13:51.000000 sciline-24.4.1/src/sciline/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-04-05 04:13:51.000000 sciline-24.4.1/src/sciline/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:14:01.683626 sciline-24.4.1/src/sciline/serialize/
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-05 04:13:51.000000 sciline-24.4.1/src/sciline/serialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-04-05 04:13:51.000000 sciline-24.4.1/src/sciline/serialize/_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-04-05 04:13:51.000000 sciline-24.4.1/src/sciline/serialize/graph_json_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-05 04:13:51.000000 sciline-24.4.1/src/sciline/series.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:14:01.683626 sciline-24.4.1/src/sciline/sphinxext/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-05 04:13:51.000000 sciline-24.4.1/src/sciline/sphinxext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5257 2024-04-05 04:13:51.000000 sciline-24.4.1/src/sciline/sphinxext/domain_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5593 2024-04-05 04:13:51.000000 sciline-24.4.1/src/sciline/task_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-05 04:13:51.000000 sciline-24.4.1/src/sciline/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6429 2024-04-05 04:13:51.000000 sciline-24.4.1/src/sciline/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:14:01.683626 sciline-24.4.1/src/sciline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-04-05 04:14:01.000000 sciline-24.4.1/src/sciline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-04-05 04:14:01.000000 sciline-24.4.1/src/sciline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 04:14:01.000000 sciline-24.4.1/src/sciline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-05 04:14:01.000000 sciline-24.4.1/src/sciline.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:14:01.683626 sciline-24.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-05 04:13:51.000000 sciline-24.4.1/tests/_provider_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-04-05 04:13:51.000000 sciline-24.4.1/tests/complex_workflow_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-05 04:13:51.000000 sciline-24.4.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-05 04:13:51.000000 sciline-24.4.1/tests/dask_scheduler_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-05 04:13:51.000000 sciline-24.4.1/tests/domain_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-05 04:13:51.000000 sciline-24.4.1/tests/package_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-05 04:13:51.000000 sciline-24.4.1/tests/param_table_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40014 2024-04-05 04:13:51.000000 sciline-24.4.1/tests/pipeline_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7380 2024-04-05 04:13:51.000000 sciline-24.4.1/tests/pipeline_with_optional_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24917 2024-04-05 04:13:51.000000 sciline-24.4.1/tests/pipeline_with_param_table_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-05 04:13:51.000000 sciline-24.4.1/tests/pipeline_with_postponed_annotations_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:14:01.683626 sciline-24.4.1/tests/serialize/
+-rw-r--r--   0 runner    (1001) docker     (127)    11394 2024-04-05 04:13:51.000000 sciline-24.4.1/tests/serialize/json_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-05 04:13:51.000000 sciline-24.4.1/tests/task_graph_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7908 2024-04-05 04:13:51.000000 sciline-24.4.1/tests/utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-05 04:13:51.000000 sciline-24.4.1/tests/visualize_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-04-05 04:13:51.000000 sciline-24.4.1/tox.ini
```

### Comparing `sciline-24.4.0/.github/workflows/ci.yml` & `sciline-24.4.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/.github/workflows/docs.yml` & `sciline-24.4.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/.github/workflows/nightly_at_main.yml` & `sciline-24.4.1/.github/workflows/nightly_at_main.yml`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/.github/workflows/nightly_at_release.yml` & `sciline-24.4.1/.github/workflows/nightly_at_release.yml`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/.github/workflows/release.yml` & `sciline-24.4.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/.github/workflows/test.yml` & `sciline-24.4.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/.github/workflows/unpinned.yml` & `sciline-24.4.1/.github/workflows/unpinned.yml`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/.pre-commit-config.yaml` & `sciline-24.4.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/CODE_OF_CONDUCT.md` & `sciline-24.4.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/CONTRIBUTING.md` & `sciline-24.4.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/LICENSE` & `sciline-24.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/PKG-INFO` & `sciline-24.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sciline
-Version: 24.4.0
+Version: 24.4.1
 Summary: Build scientific pipelines for your data
 Author: Scipp contributors
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Scipp contributors (https://github.com/scipp)
         All rights reserved.
```

### Comparing `sciline-24.4.0/README.md` & `sciline-24.4.1/README.md`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/conda/meta.yaml` & `sciline-24.4.1/conda/meta.yaml`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/docs/_static/anaconda-icon.js` & `sciline-24.4.1/docs/_static/anaconda-icon.js`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/docs/_static/favicon.ico` & `sciline-24.4.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/docs/_static/logo-dark.svg` & `sciline-24.4.1/docs/_static/logo-dark.svg`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/docs/_static/logo.svg` & `sciline-24.4.1/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/docs/_templates/class-template.rst` & `sciline-24.4.1/docs/_templates/class-template.rst`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/docs/_templates/module-template.rst` & `sciline-24.4.1/docs/_templates/module-template.rst`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/docs/about/index.md` & `sciline-24.4.1/docs/about/index.md`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/docs/api-reference/index.md` & `sciline-24.4.1/docs/api-reference/index.md`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/docs/conf.py` & `sciline-24.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/docs/developer/architecture-and-design/workflow-design.md` & `sciline-24.4.1/docs/developer/architecture-and-design/workflow-design.md`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/docs/developer/coding-conventions.md` & `sciline-24.4.1/docs/developer/coding-conventions.md`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/docs/developer/dependency-management.md` & `sciline-24.4.1/docs/developer/dependency-management.md`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/docs/developer/getting-started.md` & `sciline-24.4.1/docs/developer/getting-started.md`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/docs/index.md` & `sciline-24.4.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/docs/recipes/applying-decorators.ipynb` & `sciline-24.4.1/docs/recipes/applying-decorators.ipynb`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/docs/recipes/continue-from-intermediate-results.ipynb` & `sciline-24.4.1/docs/recipes/continue-from-intermediate-results.ipynb`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/docs/recipes/replacing-providers.ipynb` & `sciline-24.4.1/docs/recipes/replacing-providers.ipynb`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/docs/recipes/side-effects-and-file-writing.ipynb` & `sciline-24.4.1/docs/recipes/side-effects-and-file-writing.ipynb`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/docs/user-guide/generic-providers.ipynb` & `sciline-24.4.1/docs/user-guide/generic-providers.ipynb`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/docs/user-guide/getting-started.ipynb` & `sciline-24.4.1/docs/user-guide/getting-started.ipynb`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/docs/user-guide/parameter-tables.ipynb` & `sciline-24.4.1/docs/user-guide/parameter-tables.ipynb`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/docs/user-guide/provenance.ipynb` & `sciline-24.4.1/docs/user-guide/provenance.ipynb`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/pyproject.toml` & `sciline-24.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/requirements/base.txt` & `sciline-24.4.1/requirements/base.txt`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/requirements/basetest.txt` & `sciline-24.4.1/requirements/basetest.txt`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/requirements/ci.txt` & `sciline-24.4.1/requirements/ci.txt`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/requirements/dev.txt` & `sciline-24.4.1/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/requirements/docs.txt` & `sciline-24.4.1/requirements/docs.txt`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/requirements/make_base.py` & `sciline-24.4.1/requirements/make_base.py`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/requirements/static.txt` & `sciline-24.4.1/requirements/static.txt`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/requirements/test-dask.txt` & `sciline-24.4.1/requirements/test-dask.txt`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/resources/sciline.svg` & `sciline-24.4.1/resources/sciline.svg`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/src/sciline/__init__.py` & `sciline-24.4.1/src/sciline/__init__.py`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/src/sciline/_provider.py` & `sciline-24.4.1/src/sciline/_provider.py`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/src/sciline/_utils.py` & `sciline-24.4.1/src/sciline/_utils.py`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/src/sciline/display.py` & `sciline-24.4.1/src/sciline/display.py`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/src/sciline/domain.py` & `sciline-24.4.1/src/sciline/domain.py`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/src/sciline/handler.py` & `sciline-24.4.1/src/sciline/handler.py`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/src/sciline/param_table.py` & `sciline-24.4.1/src/sciline/param_table.py`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/src/sciline/pipeline.py` & `sciline-24.4.1/src/sciline/pipeline.py`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/src/sciline/scheduler.py` & `sciline-24.4.1/src/sciline/scheduler.py`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/src/sciline/serialize/_json.py` & `sciline-24.4.1/src/sciline/serialize/_json.py`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/src/sciline/serialize/graph_json_schema.json` & `sciline-24.4.1/src/sciline/serialize/graph_json_schema.json`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/src/sciline/series.py` & `sciline-24.4.1/src/sciline/series.py`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/src/sciline/sphinxext/domain_types.py` & `sciline-24.4.1/src/sciline/sphinxext/domain_types.py`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/src/sciline/task_graph.py` & `sciline-24.4.1/src/sciline/task_graph.py`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/src/sciline/typing.py` & `sciline-24.4.1/src/sciline/typing.py`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/src/sciline/visualize.py` & `sciline-24.4.1/src/sciline/visualize.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 
 
 def _to_subgraphs(graph: FormattedGraph) -> Dict[str, FormattedGraph]:
     def get_subgraph_name(name: str, kind: str) -> str:
         if kind == 'series':
             # Example: Series[RowId, Material[Country]] -> RowId, Material[Country]
             return name.partition('[')[-1].rpartition(']')[0]
-        return name
+        return name.split('[')[0]
 
     subgraphs: Dict[str, FormattedGraph] = {}
     for p, formatted_p in graph.items():
         subgraph_name = get_subgraph_name(formatted_p.ret.name, formatted_p.kind)
         subgraphs.setdefault(subgraph_name, {})
         subgraphs[subgraph_name][p] = formatted_p
     return subgraphs
```

### Comparing `sciline-24.4.0/src/sciline.egg-info/PKG-INFO` & `sciline-24.4.1/src/sciline.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sciline
-Version: 24.4.0
+Version: 24.4.1
 Summary: Build scientific pipelines for your data
 Author: Scipp contributors
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Scipp contributors (https://github.com/scipp)
         All rights reserved.
```

### Comparing `sciline-24.4.0/src/sciline.egg-info/SOURCES.txt` & `sciline-24.4.1/src/sciline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/tests/_provider_test.py` & `sciline-24.4.1/tests/_provider_test.py`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/tests/complex_workflow_test.py` & `sciline-24.4.1/tests/complex_workflow_test.py`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/tests/conftest.py` & `sciline-24.4.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/tests/domain_test.py` & `sciline-24.4.1/tests/domain_test.py`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/tests/param_table_test.py` & `sciline-24.4.1/tests/param_table_test.py`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/tests/pipeline_test.py` & `sciline-24.4.1/tests/pipeline_test.py`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/tests/pipeline_with_optional_test.py` & `sciline-24.4.1/tests/pipeline_with_optional_test.py`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/tests/pipeline_with_param_table_test.py` & `sciline-24.4.1/tests/pipeline_with_param_table_test.py`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/tests/pipeline_with_postponed_annotations_test.py` & `sciline-24.4.1/tests/pipeline_with_postponed_annotations_test.py`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/tests/serialize/json_test.py` & `sciline-24.4.1/tests/serialize/json_test.py`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/tests/task_graph_test.py` & `sciline-24.4.1/tests/task_graph_test.py`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/tests/utils_test.py` & `sciline-24.4.1/tests/utils_test.py`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/tests/visualize_test.py` & `sciline-24.4.1/tests/visualize_test.py`

 * *Files identical despite different names*

### Comparing `sciline-24.4.0/tox.ini` & `sciline-24.4.1/tox.ini`

 * *Files identical despite different names*

